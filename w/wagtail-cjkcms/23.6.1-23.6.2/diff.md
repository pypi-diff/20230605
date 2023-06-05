# Comparing `tmp/wagtail-cjkcms-23.6.1.tar.gz` & `tmp/wagtail-cjkcms-23.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-cjkcms-23.6.1.tar", last modified: Wed May 31 16:43:44 2023, max compression
+gzip compressed data, was "wagtail-cjkcms-23.6.2.tar", last modified: Mon Jun  5 13:56:33 2023, max compression
```

## Comparing `wagtail-cjkcms-23.6.1.tar` & `wagtail-cjkcms-23.6.2.tar`

### file list

```diff
@@ -1,266 +1,267 @@
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-05-31 16:43:44.282574 wagtail-cjkcms-23.6.1/
--rw-r--r--   0 grze      (1000) grze      (1000)     7161 2023-05-31 16:30:59.000000 wagtail-cjkcms-23.6.1/CHANGELOG.md
--rw-r--r--   0 grze      (1000) grze      (1000)     1542 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/LICENSE
--rw-r--r--   0 grze      (1000) grze      (1000)      239 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/MANIFEST.in
--rw-r--r--   0 grze      (1000) grze      (1000)     2828 2023-05-31 16:43:44.282574 wagtail-cjkcms-23.6.1/PKG-INFO
--rw-r--r--   0 grze      (1000) grze      (1000)     1688 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/README.md
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-05-31 16:43:44.260908 wagtail-cjkcms-23.6.1/cjkcms/
--rw-r--r--   0 grze      (1000) grze      (1000)      272 2023-05-31 16:29:17.000000 wagtail-cjkcms-23.6.1/cjkcms/__init__.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-05-31 16:43:44.260908 wagtail-cjkcms-23.6.1/cjkcms/api/
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/api/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2832 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/api/mailchimp.py
--rw-r--r--   0 grze      (1000) grze      (1000)      173 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/apps.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-05-31 16:43:44.260908 wagtail-cjkcms-23.6.1/cjkcms/bin/
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/bin/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)     5752 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/bin/cjkcms.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-05-31 16:43:44.260908 wagtail-cjkcms-23.6.1/cjkcms/blocks/
--rw-r--r--   0 grze      (1000) grze      (1000)     3166 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/blocks/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)    10455 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/blocks/base_blocks.py
--rw-r--r--   0 grze      (1000) grze      (1000)     8476 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/blocks/content_blocks.py
--rw-r--r--   0 grze      (1000) grze      (1000)     9251 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/blocks/html_blocks.py
--rw-r--r--   0 grze      (1000) grze      (1000)     3337 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/blocks/layout_blocks.py
--rw-r--r--   0 grze      (1000) grze      (1000)      171 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/blocks/searchable_html_block.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-05-31 16:43:44.260908 wagtail-cjkcms-23.6.1/cjkcms/draftail/
--rw-r--r--   0 grze      (1000) grze      (1000)      305 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/draftail/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)     3157 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/draftail/draftail_extensions.py
--rw-r--r--   0 grze      (1000) grze      (1000)     5157 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/draftail/draftail_icons.py
--rw-r--r--   0 grze      (1000) grze      (1000)     3191 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/fields.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-05-31 16:43:44.260908 wagtail-cjkcms-23.6.1/cjkcms/finders/
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/finders/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2459 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/finders/oembed.py
--rw-r--r--   0 grze      (1000) grze      (1000)      361 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/forms.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1804 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/image_formats.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-05-31 16:43:44.250074 wagtail-cjkcms-23.6.1/cjkcms/management/
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-05-31 16:43:44.260908 wagtail-cjkcms-23.6.1/cjkcms/management/commands/
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/management/commands/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)      453 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/management/commands/clear-embeds.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2565 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/management/commands/import-csv.py
--rw-r--r--   0 grze      (1000) grze      (1000)      952 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/management/commands/init-collections.py
--rw-r--r--   0 grze      (1000) grze      (1000)     3560 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/management/commands/init-navbar.py
--rw-r--r--   0 grze      (1000) grze      (1000)     3820 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/management/commands/init-website.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-05-31 16:43:44.260908 wagtail-cjkcms-23.6.1/cjkcms/migrations/
--rw-r--r--   0 grze      (1000) grze      (1000)   216350 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/migrations/0001_initial.py
--rw-r--r--   0 grze      (1000) grze      (1000)      835 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/migrations/0002_alter_body_to_cjkcmsstreamfield.py
--rw-r--r--   0 grze      (1000) grze      (1000)      668 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/migrations/0003_alter_footer_content_alter_navbar_menu_items.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1027 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/migrations/0004_layoutsettings_articles_date_format_and_more.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1709 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/migrations/0005_layoutsettings_custom_font_and_more.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2886 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/migrations/0006_analyticssettings_consent_modal_layout_and_more.py
--rw-r--r--   0 grze      (1000) grze      (1000)      594 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/migrations/0007_layoutsettings_bootstrap_icons.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1334 2023-05-31 15:55:06.000000 wagtail-cjkcms-23.6.1/cjkcms/migrations/0008_alter_layoutsettings_navbar_langselector.py
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/migrations/__init__.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-05-31 16:43:44.260908 wagtail-cjkcms-23.6.1/cjkcms/models/
--rw-r--r--   0 grze      (1000) grze      (1000)      232 2023-05-31 15:50:31.000000 wagtail-cjkcms-23.6.1/cjkcms/models/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)      335 2023-05-31 16:04:59.000000 wagtail-cjkcms-23.6.1/cjkcms/models/admin_sidebar.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2356 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/models/cms_models.py
--rw-r--r--   0 grze      (1000) grze      (1000)     6302 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/models/integration_models.py
--rw-r--r--   0 grze      (1000) grze      (1000)    19637 2023-05-31 15:57:04.000000 wagtail-cjkcms-23.6.1/cjkcms/models/page_models.py
--rw-r--r--   0 grze      (1000) grze      (1000)    12522 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/models/snippet_models.py
--rw-r--r--   0 grze      (1000) grze      (1000)    18513 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/models/wagtailsettings_models.py
--rw-r--r--   0 grze      (1000) grze      (1000)      125 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/search_urls.py
--rw-r--r--   0 grze      (1000) grze      (1000)     9500 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/settings.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-05-31 16:43:44.260908 wagtail-cjkcms-23.6.1/cjkcms/static/
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-05-31 16:43:44.260908 wagtail-cjkcms-23.6.1/cjkcms/static/cjkcms/
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-05-31 16:43:44.260908 wagtail-cjkcms-23.6.1/cjkcms/static/cjkcms/bi/
--rw-r--r--   0 grze      (1000) grze      (1000)    93729 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/static/cjkcms/bi/bootstrap-icons.css
--rw-r--r--   0 grze      (1000) grze      (1000)    49971 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/static/cjkcms/bi/bootstrap-icons.json
--rw-r--r--   0 grze      (1000) grze      (1000)    55169 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/static/cjkcms/bi/bootstrap-icons.scss
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-05-31 16:43:44.260908 wagtail-cjkcms-23.6.1/cjkcms/static/cjkcms/bi/fonts/
--rw-r--r--   0 grze      (1000) grze      (1000)   164360 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/static/cjkcms/bi/fonts/bootstrap-icons.woff
--rw-r--r--   0 grze      (1000) grze      (1000)   121340 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/static/cjkcms/bi/fonts/bootstrap-icons.woff2
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-05-31 16:43:44.260908 wagtail-cjkcms-23.6.1/cjkcms/static/cjkcms/css/
--rw-r--r--   0 grze      (1000) grze      (1000)      846 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/static/cjkcms/css/cjkcms-admin.css
--rw-r--r--   0 grze      (1000) grze      (1000)     1039 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/static/cjkcms/css/cjkcms-editor.css
--rw-r--r--   0 grze      (1000) grze      (1000)     4375 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/static/cjkcms/css/cjkcms-front.css
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-05-31 16:43:44.260908 wagtail-cjkcms-23.6.1/cjkcms/static/cjkcms/images/
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-05-31 16:43:44.260908 wagtail-cjkcms-23.6.1/cjkcms/static/cjkcms/images/avatars/
--rw-r--r--   0 grze      (1000) grze      (1000)      535 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/static/cjkcms/images/avatars/default.png
--rw-r--r--   0 grze      (1000) grze      (1000)      384 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/static/cjkcms/images/avatars/default.svg
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-05-31 16:43:44.260908 wagtail-cjkcms-23.6.1/cjkcms/static/cjkcms/images/icons/
--rw-r--r--   0 grze      (1000) grze      (1000)      705 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/static/cjkcms/images/icons/quote.svg
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-05-31 16:43:44.260908 wagtail-cjkcms-23.6.1/cjkcms/static/cjkcms/images/logos/
--rw-r--r--   0 grze      (1000) grze      (1000)     4166 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/static/cjkcms/images/logos/cms-logo-long.svg
--rw-r--r--   0 grze      (1000) grze      (1000)     4218 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/static/cjkcms/images/logos/cms-logo-square.svg
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-05-31 16:43:44.260908 wagtail-cjkcms-23.6.1/cjkcms/static/cjkcms/images/patterns/
--rw-r--r--   0 grze      (1000) grze      (1000)    47935 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/static/cjkcms/images/patterns/pattern1.jpg
--rw-r--r--   0 grze      (1000) grze      (1000)    31707 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/static/cjkcms/images/patterns/pattern2.jpg
--rw-r--r--   0 grze      (1000) grze      (1000)    38190 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/static/cjkcms/images/patterns/pattern3.jpg
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-05-31 16:43:44.260908 wagtail-cjkcms-23.6.1/cjkcms/static/cjkcms/js/
--rw-r--r--   0 grze      (1000) grze      (1000)      444 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/static/cjkcms/js/cjkcms-editor.js
--rw-r--r--   0 grze      (1000) grze      (1000)     5780 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/static/cjkcms/js/cjkcms-front.js
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-05-31 16:43:44.260908 wagtail-cjkcms-23.6.1/cjkcms/static/cookieconsent/
--rw-r--r--   0 grze      (1000) grze      (1000)    18803 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/static/cookieconsent/cookieconsent.css
--rw-r--r--   0 grze      (1000) grze      (1000)    18743 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/static/cookieconsent/cookieconsent.js
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-05-31 16:43:44.260908 wagtail-cjkcms-23.6.1/cjkcms/templates/
--rw-r--r--   0 grze      (1000) grze      (1000)     4176 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/404.html
--rw-r--r--   0 grze      (1000) grze      (1000)     4802 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/500.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-05-31 16:43:44.260908 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-05-31 16:43:44.271741 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/
--rw-r--r--   0 grze      (1000) grze      (1000)     1443 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/accordion_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      974 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/article_block_card.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1132 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/article_masonry_card.html
--rw-r--r--   0 grze      (1000) grze      (1000)      188 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/base_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)     2505 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/base_link_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      740 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/button_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      746 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/card_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      856 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/card_blurb.html
--rw-r--r--   0 grze      (1000) grze      (1000)      786 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/card_foot.html
--rw-r--r--   0 grze      (1000) grze      (1000)      730 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/card_head.html
--rw-r--r--   0 grze      (1000) grze      (1000)      771 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/card_head_foot.html
--rw-r--r--   0 grze      (1000) grze      (1000)      990 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/card_horizontal.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1104 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/card_horizontal2.html
--rw-r--r--   0 grze      (1000) grze      (1000)      786 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/card_img.html
--rw-r--r--   0 grze      (1000) grze      (1000)     2618 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/card_landing1.html
--rw-r--r--   0 grze      (1000) grze      (1000)     2758 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/card_landing2.html
--rw-r--r--   0 grze      (1000) grze      (1000)      678 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/cardgrid_columns.html
--rw-r--r--   0 grze      (1000) grze      (1000)      450 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/cardgrid_deck.html
--rw-r--r--   0 grze      (1000) grze      (1000)      277 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/cardgrid_group.html
--rw-r--r--   0 grze      (1000) grze      (1000)      276 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/cardgrid_zero.html
--rw-r--r--   0 grze      (1000) grze      (1000)     2698 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/carousel_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      406 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/column_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      137 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/document_link_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      920 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/download_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      103 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/embed_video_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)       95 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/external_link_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      424 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/grid_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      200 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/h1_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      200 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/h2_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      200 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/h3_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      790 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/hero_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      275 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/image_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1400 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/image_gallery_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      627 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/image_link_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1020 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/modal_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      164 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/page_link_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      787 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/pagelist_article_card_columns.html
--rw-r--r--   0 grze      (1000) grze      (1000)      642 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/pagelist_article_card_deck.html
--rw-r--r--   0 grze      (1000) grze      (1000)      361 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/pagelist_article_card_group.html
--rw-r--r--   0 grze      (1000) grze      (1000)      956 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/pagelist_article_media.html
--rw-r--r--   0 grze      (1000) grze      (1000)      397 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/pagelist_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      610 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/pagelist_list_group.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1224 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/pagelist_toc_nextprev.html
--rw-r--r--   0 grze      (1000) grze      (1000)      300 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/pagepreview_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      793 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/pagepreview_card.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1065 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/pagepreview_form.html
--rw-r--r--   0 grze      (1000) grze      (1000)      244 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/pricelist_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      513 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/pricelistitem_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      353 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/quote_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      852 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/quote_block_leftbar.html
--rw-r--r--   0 grze      (1000) grze      (1000)      998 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/quote_block_start_end_quote.html
--rw-r--r--   0 grze      (1000) grze      (1000)      216 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/reusable_content_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)       91 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/rich_text_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1095 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/table_block.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-05-31 16:43:44.271741 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/cookieconsent/
--rw-r--r--   0 grze      (1000) grze      (1000)     3672 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/cookieconsent/languages.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-05-31 16:43:44.271741 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/formfields/
--rw-r--r--   0 grze      (1000) grze      (1000)      267 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/formfields/date.html
--rw-r--r--   0 grze      (1000) grze      (1000)      416 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/formfields/datetime.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-05-31 16:43:44.271741 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/formfields/mailchimp/
--rw-r--r--   0 grze      (1000) grze      (1000)     9267 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/formfields/mailchimp/_2vanilla_subscriber_integration_js.html
--rw-r--r--   0 grze      (1000) grze      (1000)     6469 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_js.html
--rw-r--r--   0 grze      (1000) grze      (1000)      793 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_widget.html
--rw-r--r--   0 grze      (1000) grze      (1000)      264 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/formfields/time.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-05-31 16:43:44.271741 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/icons/
--rw-r--r--   0 grze      (1000) grze      (1000)      465 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/icons/align-left.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      573 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/icons/check-square-o.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      277 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/icons/columns.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      359 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/icons/desktop.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      571 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/icons/font.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      292 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/icons/google.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      813 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/icons/hand-pointer-o.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      666 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/icons/hashtag.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      840 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/icons/header.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      835 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/icons/list-alt.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      459 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/icons/map.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      448 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/icons/newspaper-o.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      721 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/icons/puzzle-piece.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      635 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/icons/recycle.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      174 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/icons/stop.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      505 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/icons/th-large.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      762 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/icons/universal-access.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      548 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/icons/usd.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      225 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/icons/window-maximize.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      199 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/icons/window-minimize.svg
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-05-31 16:43:44.271741 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/includes/
--rw-r--r--   0 grze      (1000) grze      (1000)      286 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/includes/cjkcms_banner.html
--rw-r--r--   0 grze      (1000) grze      (1000)      689 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/includes/classifier_dropdowns.html
--rw-r--r--   0 grze      (1000) grze      (1000)      579 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/includes/classifier_nav.html
--rw-r--r--   0 grze      (1000) grze      (1000)      286 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/includes/codered_banner.html
--rw-r--r--   0 grze      (1000) grze      (1000)      268 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/includes/form_honeypot.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1061 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/includes/pagination.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-05-31 16:43:44.271741 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/includes/stream_forms/
--rw-r--r--   0 grze      (1000) grze      (1000)      532 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/includes/stream_forms/render_field.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-05-31 16:43:44.271741 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/pages/
--rw-r--r--   0 grze      (1000) grze      (1000)     2002 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/pages/article_index_page.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1705 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/pages/article_page.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1018 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/pages/article_page.search.html
--rw-r--r--   0 grze      (1000) grze      (1000)     7931 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/pages/base.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1104 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/pages/form_page.html
--rw-r--r--   0 grze      (1000) grze      (1000)      248 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/pages/form_page_landing.html
--rw-r--r--   0 grze      (1000) grze      (1000)       50 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/pages/home_page.html
--rw-r--r--   0 grze      (1000) grze      (1000)     2610 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/pages/search.html
--rw-r--r--   0 grze      (1000) grze      (1000)      582 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/pages/search_result.html
--rw-r--r--   0 grze      (1000) grze      (1000)     2462 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/pages/stream_form_page.html
--rw-r--r--   0 grze      (1000) grze      (1000)      838 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/pages/web_page.html
--rw-r--r--   0 grze      (1000) grze      (1000)      623 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/pages/web_page_notitle.html
--rw-r--r--   0 grze      (1000) grze      (1000)      122 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/robots.txt
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-05-31 16:43:44.282574 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/snippets/
--rw-r--r--   0 grze      (1000) grze      (1000)     1943 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/snippets/bottom_corner_lang_selector.html
--rw-r--r--   0 grze      (1000) grze      (1000)      430 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/snippets/footer.html
--rw-r--r--   0 grze      (1000) grze      (1000)     2027 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/snippets/frontend_assets.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1196 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/snippets/frontend_scripts.html
--rw-r--r--   0 grze      (1000) grze      (1000)     2600 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/snippets/navbar.html
--rw-r--r--   0 grze      (1000) grze      (1000)      836 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/snippets/navbar_lang_selector.html
--rw-r--r--   0 grze      (1000) grze      (1000)      386 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/snippets/navbar_search.html
--rw-r--r--   0 grze      (1000) grze      (1000)      158 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/snippets/tracking_g3.html
--rw-r--r--   0 grze      (1000) grze      (1000)      831 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/snippets/tracking_g4.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-05-31 16:43:44.282574 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/widgets/
--rw-r--r--   0 grze      (1000) grze      (1000)     1384 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/widgets/checkbox_classifiers.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-05-31 16:43:44.260908 wagtail-cjkcms-23.6.1/cjkcms/templates/wagtailadmin/
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-05-31 16:43:44.282574 wagtail-cjkcms-23.6.1/cjkcms/templates/wagtailadmin/block_forms/
--rw-r--r--   0 grze      (1000) grze      (1000)      754 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/wagtailadmin/block_forms/base_block_settings_struct.html
--rw-r--r--   0 grze      (1000) grze      (1000)      550 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/wagtailadmin/block_forms/struct.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-05-31 16:43:44.282574 wagtail-cjkcms-23.6.1/cjkcms/templates/wagtailadmin/shared/
--rw-r--r--   0 grze      (1000) grze      (1000)      885 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templates/wagtailadmin/shared/cr_main_nav_2fix.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-05-31 16:43:44.282574 wagtail-cjkcms-23.6.1/cjkcms/templatetags/
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templatetags/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)      327 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templatetags/auth_extras.py
--rw-r--r--   0 grze      (1000) grze      (1000)     6785 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templatetags/cjkcms_tags.py
--rw-r--r--   0 grze      (1000) grze      (1000)     4962 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templatetags/friendly_loader.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1127 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templatetags/gravatar.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1224 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/templatetags/txtutils_tags.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-05-31 16:43:44.282574 wagtail-cjkcms-23.6.1/cjkcms/tests/
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/tests/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)     4226 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/tests/test_articlepages.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2629 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/tests/test_gravatar.py
--rw-r--r--   0 grze      (1000) grze      (1000)     4639 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/tests/test_search_blocks.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2665 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/tests/test_settings.py
--rw-r--r--   0 grze      (1000) grze      (1000)     3511 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/tests/test_templatetags.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2678 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/tests/test_urls.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1520 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/tests/test_webpage.py
--rw-r--r--   0 grze      (1000) grze      (1000)      506 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/urls.py
--rw-r--r--   0 grze      (1000) grze      (1000)      573 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/utils.py
--rw-r--r--   0 grze      (1000) grze      (1000)     4488 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/views.py
--rw-r--r--   0 grze      (1000) grze      (1000)     6557 2023-05-31 16:27:47.000000 wagtail-cjkcms-23.6.1/cjkcms/wagtail_hooks.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1531 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/cjkcms/widgets.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-05-31 16:43:44.282574 wagtail-cjkcms-23.6.1/docs/
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-05-31 16:43:44.282574 wagtail-cjkcms-23.6.1/docs/how-to/
--rw-r--r--   0 grze      (1000) grze      (1000)     1481 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/docs/how-to/oembed_finder.md
--rw-r--r--   0 grze      (1000) grze      (1000)      537 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/docs/index.md
--rw-r--r--   0 grze      (1000) grze      (1000)     5520 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/docs/installation.md
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-05-31 16:43:44.282574 wagtail-cjkcms-23.6.1/docs/management_commands/
--rw-r--r--   0 grze      (1000) grze      (1000)      318 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/docs/management_commands/clear-embeds.md
--rw-r--r--   0 grze      (1000) grze      (1000)      193 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/docs/management_commands/index.md
--rw-r--r--   0 grze      (1000) grze      (1000)      420 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/docs/management_commands/init-collections.md
--rw-r--r--   0 grze      (1000) grze      (1000)      936 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/docs/quick-start.md
--rw-r--r--   0 grze      (1000) grze      (1000)       13 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/docs/requirements.txt
--rw-r--r--   0 grze      (1000) grze      (1000)     1220 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/docs/why-another-cms.md
--rw-r--r--   0 grze      (1000) grze      (1000)       93 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/pyproject.toml
--rw-r--r--   0 grze      (1000) grze      (1000)     1541 2023-05-31 16:43:44.293408 wagtail-cjkcms-23.6.1/setup.cfg
--rw-r--r--   0 grze      (1000) grze      (1000)       38 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.1/setup.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-05-31 16:43:44.282574 wagtail-cjkcms-23.6.1/wagtail_cjkcms.egg-info/
--rw-r--r--   0 grze      (1000) grze      (1000)     2828 2023-05-31 16:43:44.000000 wagtail-cjkcms-23.6.1/wagtail_cjkcms.egg-info/PKG-INFO
--rw-r--r--   0 grze      (1000) grze      (1000)     9491 2023-05-31 16:43:44.000000 wagtail-cjkcms-23.6.1/wagtail_cjkcms.egg-info/SOURCES.txt
--rw-r--r--   0 grze      (1000) grze      (1000)        1 2023-05-31 16:43:44.000000 wagtail-cjkcms-23.6.1/wagtail_cjkcms.egg-info/dependency_links.txt
--rw-r--r--   0 grze      (1000) grze      (1000)       50 2023-05-31 16:43:44.000000 wagtail-cjkcms-23.6.1/wagtail_cjkcms.egg-info/entry_points.txt
--rw-r--r--   0 grze      (1000) grze      (1000)       79 2023-05-31 16:43:44.000000 wagtail-cjkcms-23.6.1/wagtail_cjkcms.egg-info/requires.txt
--rw-r--r--   0 grze      (1000) grze      (1000)        7 2023-05-31 16:43:44.000000 wagtail-cjkcms-23.6.1/wagtail_cjkcms.egg-info/top_level.txt
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.262377 wagtail-cjkcms-23.6.2/
+-rw-r--r--   0 grze      (1000) grze      (1000)     7412 2023-06-05 13:55:53.000000 wagtail-cjkcms-23.6.2/CHANGELOG.md
+-rw-r--r--   0 grze      (1000) grze      (1000)     1542 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/LICENSE
+-rw-r--r--   0 grze      (1000) grze      (1000)      239 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/MANIFEST.in
+-rw-r--r--   0 grze      (1000) grze      (1000)     2828 2023-06-05 13:56:33.262377 wagtail-cjkcms-23.6.2/PKG-INFO
+-rw-r--r--   0 grze      (1000) grze      (1000)     1688 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/README.md
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.202377 wagtail-cjkcms-23.6.2/cjkcms/
+-rw-r--r--   0 grze      (1000) grze      (1000)      272 2023-06-05 13:54:14.000000 wagtail-cjkcms-23.6.2/cjkcms/__init__.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.202377 wagtail-cjkcms-23.6.2/cjkcms/api/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/api/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2832 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/api/mailchimp.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      173 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/apps.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.202377 wagtail-cjkcms-23.6.2/cjkcms/bin/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/bin/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     5752 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/bin/cjkcms.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.202377 wagtail-cjkcms-23.6.2/cjkcms/blocks/
+-rw-r--r--   0 grze      (1000) grze      (1000)     3166 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/blocks/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)    10455 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/blocks/base_blocks.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     8476 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/blocks/content_blocks.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     9251 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/blocks/html_blocks.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     3337 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/blocks/layout_blocks.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      171 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/blocks/searchable_html_block.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.202377 wagtail-cjkcms-23.6.2/cjkcms/draftail/
+-rw-r--r--   0 grze      (1000) grze      (1000)      305 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/draftail/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     3157 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/draftail/draftail_extensions.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     5157 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/draftail/draftail_icons.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     3191 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/fields.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.202377 wagtail-cjkcms-23.6.2/cjkcms/finders/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/finders/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2459 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/finders/oembed.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      361 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/forms.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1804 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/image_formats.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.182377 wagtail-cjkcms-23.6.2/cjkcms/management/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.212377 wagtail-cjkcms-23.6.2/cjkcms/management/commands/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/management/commands/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      453 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/management/commands/clear-embeds.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2565 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/management/commands/import-csv.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      952 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/management/commands/init-collections.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     3560 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/management/commands/init-navbar.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     3820 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/management/commands/init-website.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.212377 wagtail-cjkcms-23.6.2/cjkcms/migrations/
+-rw-r--r--   0 grze      (1000) grze      (1000)   216350 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/migrations/0001_initial.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      835 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/migrations/0002_alter_body_to_cjkcmsstreamfield.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      668 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/migrations/0003_alter_footer_content_alter_navbar_menu_items.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1027 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/migrations/0004_layoutsettings_articles_date_format_and_more.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1709 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/migrations/0005_layoutsettings_custom_font_and_more.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2886 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/migrations/0006_analyticssettings_consent_modal_layout_and_more.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      594 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/migrations/0007_layoutsettings_bootstrap_icons.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1334 2023-05-31 15:55:06.000000 wagtail-cjkcms-23.6.2/cjkcms/migrations/0008_alter_layoutsettings_navbar_langselector.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      685 2023-06-04 21:40:37.000000 wagtail-cjkcms-23.6.2/cjkcms/migrations/0009_navbar_language.py
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/migrations/__init__.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.212377 wagtail-cjkcms-23.6.2/cjkcms/models/
+-rw-r--r--   0 grze      (1000) grze      (1000)      232 2023-05-31 15:50:31.000000 wagtail-cjkcms-23.6.2/cjkcms/models/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      335 2023-05-31 16:04:59.000000 wagtail-cjkcms-23.6.2/cjkcms/models/admin_sidebar.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2356 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/models/cms_models.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     6302 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/models/integration_models.py
+-rw-r--r--   0 grze      (1000) grze      (1000)    19637 2023-05-31 15:57:04.000000 wagtail-cjkcms-23.6.2/cjkcms/models/page_models.py
+-rw-r--r--   0 grze      (1000) grze      (1000)    13532 2023-06-05 10:56:37.000000 wagtail-cjkcms-23.6.2/cjkcms/models/snippet_models.py
+-rw-r--r--   0 grze      (1000) grze      (1000)    18513 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/models/wagtailsettings_models.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      125 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/search_urls.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     9500 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/settings.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.192377 wagtail-cjkcms-23.6.2/cjkcms/static/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.192377 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.212377 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/bi/
+-rw-r--r--   0 grze      (1000) grze      (1000)    93729 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/bi/bootstrap-icons.css
+-rw-r--r--   0 grze      (1000) grze      (1000)    49971 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/bi/bootstrap-icons.json
+-rw-r--r--   0 grze      (1000) grze      (1000)    55169 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/bi/bootstrap-icons.scss
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.212377 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/bi/fonts/
+-rw-r--r--   0 grze      (1000) grze      (1000)   164360 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/bi/fonts/bootstrap-icons.woff
+-rw-r--r--   0 grze      (1000) grze      (1000)   121340 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/bi/fonts/bootstrap-icons.woff2
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.222377 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/css/
+-rw-r--r--   0 grze      (1000) grze      (1000)      846 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/css/cjkcms-admin.css
+-rw-r--r--   0 grze      (1000) grze      (1000)     1104 2023-06-04 21:08:12.000000 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/css/cjkcms-editor.css
+-rw-r--r--   0 grze      (1000) grze      (1000)     4375 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/css/cjkcms-front.css
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.192377 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/images/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.222377 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/images/avatars/
+-rw-r--r--   0 grze      (1000) grze      (1000)      535 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/images/avatars/default.png
+-rw-r--r--   0 grze      (1000) grze      (1000)      384 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/images/avatars/default.svg
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.222377 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/images/icons/
+-rw-r--r--   0 grze      (1000) grze      (1000)      705 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/images/icons/quote.svg
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.222377 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/images/logos/
+-rw-r--r--   0 grze      (1000) grze      (1000)     4166 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/images/logos/cms-logo-long.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)     4218 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/images/logos/cms-logo-square.svg
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.222377 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/images/patterns/
+-rw-r--r--   0 grze      (1000) grze      (1000)    47935 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/images/patterns/pattern1.jpg
+-rw-r--r--   0 grze      (1000) grze      (1000)    31707 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/images/patterns/pattern2.jpg
+-rw-r--r--   0 grze      (1000) grze      (1000)    38190 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/images/patterns/pattern3.jpg
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.222377 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/js/
+-rw-r--r--   0 grze      (1000) grze      (1000)      444 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/js/cjkcms-editor.js
+-rw-r--r--   0 grze      (1000) grze      (1000)     5780 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/js/cjkcms-front.js
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.222377 wagtail-cjkcms-23.6.2/cjkcms/static/cookieconsent/
+-rw-r--r--   0 grze      (1000) grze      (1000)    18803 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/static/cookieconsent/cookieconsent.css
+-rw-r--r--   0 grze      (1000) grze      (1000)    18743 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/static/cookieconsent/cookieconsent.js
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.222377 wagtail-cjkcms-23.6.2/cjkcms/templates/
+-rw-r--r--   0 grze      (1000) grze      (1000)     4176 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/404.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     4802 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/500.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.222377 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.242377 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/
+-rw-r--r--   0 grze      (1000) grze      (1000)     1443 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/accordion_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      974 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/article_block_card.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1132 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/article_masonry_card.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      188 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/base_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     2505 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/base_link_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      740 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/button_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      746 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/card_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      856 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/card_blurb.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      786 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/card_foot.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      730 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/card_head.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      771 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/card_head_foot.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      990 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/card_horizontal.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1104 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/card_horizontal2.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      786 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/card_img.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     2618 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/card_landing1.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     2758 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/card_landing2.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      678 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/cardgrid_columns.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      450 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/cardgrid_deck.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      277 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/cardgrid_group.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      276 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/cardgrid_zero.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     2698 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/carousel_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      406 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/column_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      137 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/document_link_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      920 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/download_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      103 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/embed_video_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)       95 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/external_link_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      424 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/grid_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      200 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/h1_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      200 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/h2_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      200 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/h3_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      790 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/hero_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      275 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/image_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1400 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/image_gallery_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      627 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/image_link_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1020 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/modal_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      164 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/page_link_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      787 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/pagelist_article_card_columns.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      642 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/pagelist_article_card_deck.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      361 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/pagelist_article_card_group.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      956 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/pagelist_article_media.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      397 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/pagelist_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      610 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/pagelist_list_group.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1224 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/pagelist_toc_nextprev.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      300 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/pagepreview_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      793 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/pagepreview_card.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1065 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/pagepreview_form.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      244 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/pricelist_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      513 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/pricelistitem_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      353 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/quote_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      852 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/quote_block_leftbar.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      998 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/quote_block_start_end_quote.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      216 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/reusable_content_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)       91 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/rich_text_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1095 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/table_block.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.242377 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/cookieconsent/
+-rw-r--r--   0 grze      (1000) grze      (1000)     3672 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/cookieconsent/languages.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.242377 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/formfields/
+-rw-r--r--   0 grze      (1000) grze      (1000)      267 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/formfields/date.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      416 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/formfields/datetime.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.242377 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/formfields/mailchimp/
+-rw-r--r--   0 grze      (1000) grze      (1000)     9267 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/formfields/mailchimp/_2vanilla_subscriber_integration_js.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     6469 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_js.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      793 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_widget.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      264 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/formfields/time.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.242377 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/
+-rw-r--r--   0 grze      (1000) grze      (1000)      465 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/align-left.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      573 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/check-square-o.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      277 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/columns.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      359 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/desktop.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      571 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/font.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      292 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/google.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      813 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/hand-pointer-o.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      666 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/hashtag.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      840 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/header.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      835 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/list-alt.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      459 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/map.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      448 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/newspaper-o.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      721 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/puzzle-piece.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      635 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/recycle.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      174 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/stop.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      505 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/th-large.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      762 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/universal-access.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      548 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/usd.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      225 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/window-maximize.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      199 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/window-minimize.svg
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.242377 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/includes/
+-rw-r--r--   0 grze      (1000) grze      (1000)      286 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/includes/cjkcms_banner.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      689 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/includes/classifier_dropdowns.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      579 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/includes/classifier_nav.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      286 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/includes/codered_banner.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      268 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/includes/form_honeypot.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1061 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/includes/pagination.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.242377 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/includes/stream_forms/
+-rw-r--r--   0 grze      (1000) grze      (1000)      532 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/includes/stream_forms/render_field.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.252377 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/pages/
+-rw-r--r--   0 grze      (1000) grze      (1000)     2002 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/pages/article_index_page.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1705 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/pages/article_page.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1018 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/pages/article_page.search.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     7931 2023-06-05 10:34:33.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/pages/base.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1104 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/pages/form_page.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      248 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/pages/form_page_landing.html
+-rw-r--r--   0 grze      (1000) grze      (1000)       50 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/pages/home_page.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     2610 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/pages/search.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      582 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/pages/search_result.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     2462 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/pages/stream_form_page.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      838 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/pages/web_page.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      623 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/pages/web_page_notitle.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      122 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/robots.txt
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.252377 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/snippets/
+-rw-r--r--   0 grze      (1000) grze      (1000)     1943 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/snippets/bottom_corner_lang_selector.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      430 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/snippets/footer.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     2027 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/snippets/frontend_assets.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1196 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/snippets/frontend_scripts.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     2712 2023-06-05 10:52:40.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/snippets/navbar.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      836 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/snippets/navbar_lang_selector.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      386 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/snippets/navbar_search.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      158 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/snippets/tracking_g3.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      831 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/snippets/tracking_g4.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.252377 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/widgets/
+-rw-r--r--   0 grze      (1000) grze      (1000)     1384 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/widgets/checkbox_classifiers.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.192377 wagtail-cjkcms-23.6.2/cjkcms/templates/wagtailadmin/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.252377 wagtail-cjkcms-23.6.2/cjkcms/templates/wagtailadmin/block_forms/
+-rw-r--r--   0 grze      (1000) grze      (1000)      839 2023-06-04 21:09:36.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/wagtailadmin/block_forms/base_block_settings_struct.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      550 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/wagtailadmin/block_forms/struct.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.252377 wagtail-cjkcms-23.6.2/cjkcms/templates/wagtailadmin/shared/
+-rw-r--r--   0 grze      (1000) grze      (1000)      885 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/wagtailadmin/shared/cr_main_nav_2fix.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.252377 wagtail-cjkcms-23.6.2/cjkcms/templatetags/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templatetags/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      327 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templatetags/auth_extras.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     6785 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templatetags/cjkcms_tags.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     4962 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templatetags/friendly_loader.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1127 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templatetags/gravatar.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1224 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templatetags/txtutils_tags.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.262377 wagtail-cjkcms-23.6.2/cjkcms/tests/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/tests/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     4226 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/tests/test_articlepages.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2629 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/tests/test_gravatar.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     4639 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/tests/test_search_blocks.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2665 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/tests/test_settings.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     3511 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/tests/test_templatetags.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2678 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/tests/test_urls.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1520 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/tests/test_webpage.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      506 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/urls.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      573 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/utils.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     4488 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/views.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     6557 2023-05-31 16:27:47.000000 wagtail-cjkcms-23.6.2/cjkcms/wagtail_hooks.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1531 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/widgets.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.262377 wagtail-cjkcms-23.6.2/docs/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.262377 wagtail-cjkcms-23.6.2/docs/how-to/
+-rw-r--r--   0 grze      (1000) grze      (1000)     1481 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/docs/how-to/oembed_finder.md
+-rw-r--r--   0 grze      (1000) grze      (1000)      537 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/docs/index.md
+-rw-r--r--   0 grze      (1000) grze      (1000)     5520 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/docs/installation.md
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.262377 wagtail-cjkcms-23.6.2/docs/management_commands/
+-rw-r--r--   0 grze      (1000) grze      (1000)      318 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/docs/management_commands/clear-embeds.md
+-rw-r--r--   0 grze      (1000) grze      (1000)      193 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/docs/management_commands/index.md
+-rw-r--r--   0 grze      (1000) grze      (1000)      420 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/docs/management_commands/init-collections.md
+-rw-r--r--   0 grze      (1000) grze      (1000)      936 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/docs/quick-start.md
+-rw-r--r--   0 grze      (1000) grze      (1000)       13 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/docs/requirements.txt
+-rw-r--r--   0 grze      (1000) grze      (1000)     1220 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/docs/why-another-cms.md
+-rw-r--r--   0 grze      (1000) grze      (1000)       93 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/pyproject.toml
+-rw-r--r--   0 grze      (1000) grze      (1000)     1555 2023-06-05 13:56:33.282377 wagtail-cjkcms-23.6.2/setup.cfg
+-rw-r--r--   0 grze      (1000) grze      (1000)       38 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/setup.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.262377 wagtail-cjkcms-23.6.2/wagtail_cjkcms.egg-info/
+-rw-r--r--   0 grze      (1000) grze      (1000)     2828 2023-06-05 13:56:33.000000 wagtail-cjkcms-23.6.2/wagtail_cjkcms.egg-info/PKG-INFO
+-rw-r--r--   0 grze      (1000) grze      (1000)     9533 2023-06-05 13:56:33.000000 wagtail-cjkcms-23.6.2/wagtail_cjkcms.egg-info/SOURCES.txt
+-rw-r--r--   0 grze      (1000) grze      (1000)        1 2023-06-05 13:56:33.000000 wagtail-cjkcms-23.6.2/wagtail_cjkcms.egg-info/dependency_links.txt
+-rw-r--r--   0 grze      (1000) grze      (1000)       50 2023-06-05 13:56:33.000000 wagtail-cjkcms-23.6.2/wagtail_cjkcms.egg-info/entry_points.txt
+-rw-r--r--   0 grze      (1000) grze      (1000)       79 2023-06-05 13:56:33.000000 wagtail-cjkcms-23.6.2/wagtail_cjkcms.egg-info/requires.txt
+-rw-r--r--   0 grze      (1000) grze      (1000)        7 2023-06-05 13:56:33.000000 wagtail-cjkcms-23.6.2/wagtail_cjkcms.egg-info/top_level.txt
```

### Comparing `wagtail-cjkcms-23.6.1/CHANGELOG.md` & `wagtail-cjkcms-23.6.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -176,8 +176,13 @@
 - Add possibility to choose between menu dropdown and bottom corner language selectors.
 
 # 23.5.1 (2023-05-21)
 - Fixed regression from previous update, where change of langue chooser setting from Boolean to Char caused missing template crash if applied to existing project with Boolean value of True. Now all previous values will be changed to None upon migration.
 
 # 23.6.1 (2023-05-31)
 - Basic compatibility with Wagtail 5.0
-- Due to wagtail-seo and wagtail-cache not being compatible with Wagtail 5.0, they were replaced with forked versions downloadable from github. This is a temporary solution until the original packages are updated.
+- Due to wagtail-seo and wagtail-cache not being compatible with Wagtail 5.0, they were replaced with forked versions downloadable from github. This is a temporary solution until the original packages are updated.
+
+# 23.6.2 (2023-06-05)
+- Added new project template with webpack support (untested as of yet)
+- Modified the navbar model to support multilingual websites: new column "language" allows setting navbar
+visibility to all languages or just one selected.
```

### Comparing `wagtail-cjkcms-23.6.1/LICENSE` & `wagtail-cjkcms-23.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/PKG-INFO` & `wagtail-cjkcms-23.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-cjkcms
-Version: 23.6.1
+Version: 23.6.2
 Summary: Wagtail Content Management System, installable as a Django app into any Wagtail 4.x site. Based on Codered CRX.
 Home-page: https://github.com/cjkpl/wagtail-cjkcms
 Author: Grzegorz Krol
 Author-email: gk@cjk.pl
 License: BSD-3-Clause  # Example license
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `wagtail-cjkcms-23.6.1/README.md` & `wagtail-cjkcms-23.6.2/README.md`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/api/mailchimp.py` & `wagtail-cjkcms-23.6.2/cjkcms/api/mailchimp.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/bin/cjkcms.py` & `wagtail-cjkcms-23.6.2/cjkcms/bin/cjkcms.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/blocks/__init__.py` & `wagtail-cjkcms-23.6.2/cjkcms/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/blocks/base_blocks.py` & `wagtail-cjkcms-23.6.2/cjkcms/blocks/base_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/blocks/content_blocks.py` & `wagtail-cjkcms-23.6.2/cjkcms/blocks/content_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/blocks/html_blocks.py` & `wagtail-cjkcms-23.6.2/cjkcms/blocks/html_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/blocks/layout_blocks.py` & `wagtail-cjkcms-23.6.2/cjkcms/blocks/layout_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/draftail/draftail_extensions.py` & `wagtail-cjkcms-23.6.2/cjkcms/draftail/draftail_extensions.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/draftail/draftail_icons.py` & `wagtail-cjkcms-23.6.2/cjkcms/draftail/draftail_icons.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/fields.py` & `wagtail-cjkcms-23.6.2/cjkcms/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/finders/oembed.py` & `wagtail-cjkcms-23.6.2/cjkcms/finders/oembed.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/image_formats.py` & `wagtail-cjkcms-23.6.2/cjkcms/image_formats.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/management/commands/import-csv.py` & `wagtail-cjkcms-23.6.2/cjkcms/management/commands/import-csv.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/management/commands/init-collections.py` & `wagtail-cjkcms-23.6.2/cjkcms/management/commands/init-collections.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/management/commands/init-navbar.py` & `wagtail-cjkcms-23.6.2/cjkcms/management/commands/init-navbar.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/management/commands/init-website.py` & `wagtail-cjkcms-23.6.2/cjkcms/management/commands/init-website.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/migrations/0001_initial.py` & `wagtail-cjkcms-23.6.2/cjkcms/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/migrations/0002_alter_body_to_cjkcmsstreamfield.py` & `wagtail-cjkcms-23.6.2/cjkcms/migrations/0002_alter_body_to_cjkcmsstreamfield.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/migrations/0003_alter_footer_content_alter_navbar_menu_items.py` & `wagtail-cjkcms-23.6.2/cjkcms/migrations/0003_alter_footer_content_alter_navbar_menu_items.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/migrations/0004_layoutsettings_articles_date_format_and_more.py` & `wagtail-cjkcms-23.6.2/cjkcms/migrations/0004_layoutsettings_articles_date_format_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/migrations/0005_layoutsettings_custom_font_and_more.py` & `wagtail-cjkcms-23.6.2/cjkcms/migrations/0005_layoutsettings_custom_font_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/migrations/0006_analyticssettings_consent_modal_layout_and_more.py` & `wagtail-cjkcms-23.6.2/cjkcms/migrations/0006_analyticssettings_consent_modal_layout_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/migrations/0007_layoutsettings_bootstrap_icons.py` & `wagtail-cjkcms-23.6.2/cjkcms/migrations/0007_layoutsettings_bootstrap_icons.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/migrations/0008_alter_layoutsettings_navbar_langselector.py` & `wagtail-cjkcms-23.6.2/cjkcms/migrations/0008_alter_layoutsettings_navbar_langselector.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/models/cms_models.py` & `wagtail-cjkcms-23.6.2/cjkcms/models/cms_models.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/models/integration_models.py` & `wagtail-cjkcms-23.6.2/cjkcms/models/integration_models.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/models/page_models.py` & `wagtail-cjkcms-23.6.2/cjkcms/models/page_models.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/models/snippet_models.py` & `wagtail-cjkcms-23.6.2/cjkcms/models/snippet_models.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 from cjkcms.blocks import (
     HTML_STREAMBLOCKS,
     LAYOUT_STREAMBLOCKS,
     NAVIGATION_STREAMBLOCKS,
 )
 from cjkcms.settings import cms_settings
+from django.conf import settings
 from cjkcms.fields import CjkcmsStreamField
 
 
 @register_snippet
 class Carousel(ClusterableModel):
     """
     Model that represents a Carousel. Can be modified through the snippets UI.
@@ -247,14 +248,24 @@
         verbose_name=_("Custom CSS Class"),
     )
     custom_id = models.CharField(
         max_length=255,
         blank=True,
         verbose_name=_("Custom ID"),
     )
+
+    language = models.CharField(
+        blank=True,
+        max_length=10,
+        choices=[("_all_", _("All languages"))],
+        default="_all_",
+        verbose_name=_("Show in language"),
+        help_text=_("Select a language to limit display to specific locale."),
+    )
+
     menu_items = CjkcmsStreamField(
         NAVIGATION_STREAMBLOCKS,
         verbose_name=_("Navigation links"),
         use_json_field=True,
     )
 
     panels = [
@@ -262,20 +273,38 @@
         MultiFieldPanel(
             [
                 FieldPanel("custom_css_class"),
                 FieldPanel("custom_id"),
             ],
             heading=_("Attributes"),
         ),
+        FieldPanel("language"),
         FieldPanel("menu_items"),
     ]
 
     def __str__(self):
         return self.name
 
+    def __init__(self, *args, **kwargs):
+        """
+        Inject custom choices and defaults into the form fields
+        to enable customization of settings without causing migration issues.
+        """
+        super().__init__(*args, **kwargs)
+        # Set choices dynamically.
+
+        available_langs = [("_all_", _("All languages"))]
+        if hasattr(settings, "WAGTAIL_CONTENT_LANGUAGES"):
+            available_langs += settings.WAGTAIL_CONTENT_LANGUAGES
+
+        self._meta.get_field("language").choices = available_langs  # type: ignore
+        # Set default dynamically.
+        if not self.id:  # type: ignore
+            self.language = "_all_"
+
 
 @register_snippet
 class Footer(models.Model):
     """
     Snippet for website footer content.
     """
```

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/models/wagtailsettings_models.py` & `wagtail-cjkcms-23.6.2/cjkcms/models/wagtailsettings_models.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/settings.py` & `wagtail-cjkcms-23.6.2/cjkcms/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/static/cjkcms/bi/bootstrap-icons.css` & `wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/bi/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/static/cjkcms/bi/bootstrap-icons.json` & `wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/bi/bootstrap-icons.json`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/static/cjkcms/bi/bootstrap-icons.scss` & `wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/bi/bootstrap-icons.scss`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/static/cjkcms/bi/fonts/bootstrap-icons.woff` & `wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/bi/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/static/cjkcms/bi/fonts/bootstrap-icons.woff2` & `wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/bi/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/static/cjkcms/css/cjkcms-admin.css` & `wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/css/cjkcms-admin.css`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/static/cjkcms/css/cjkcms-editor.css` & `wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/css/cjkcms-editor.css`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,15 @@
+.cjkcms-collapsible4 {
+    padding: 0;
+    margin-top: -38px;
+}
+
 .cjkcms-collapsible {
     padding: 0;
-    margin-top: -40px;
+    margin-top: -20px;
 }
 
 .cjkcms-collapsible .cjkcms-collapsible-target {
     padding: 10px 0 0;
 }
 
 .cjkcms-collapsible>button {
```

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/static/cjkcms/css/cjkcms-front.css` & `wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/css/cjkcms-front.css`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/static/cjkcms/images/avatars/default.png` & `wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/images/avatars/default.png`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/static/cjkcms/images/icons/quote.svg` & `wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/images/icons/quote.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/static/cjkcms/images/logos/cms-logo-long.svg` & `wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/images/logos/cms-logo-long.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/static/cjkcms/images/logos/cms-logo-square.svg` & `wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/images/logos/cms-logo-square.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/static/cjkcms/images/patterns/pattern1.jpg` & `wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/images/patterns/pattern1.jpg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/static/cjkcms/images/patterns/pattern2.jpg` & `wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/images/patterns/pattern2.jpg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/static/cjkcms/images/patterns/pattern3.jpg` & `wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/images/patterns/pattern3.jpg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/static/cjkcms/js/cjkcms-front.js` & `wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/js/cjkcms-front.js`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/static/cookieconsent/cookieconsent.css` & `wagtail-cjkcms-23.6.2/cjkcms/static/cookieconsent/cookieconsent.css`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/static/cookieconsent/cookieconsent.js` & `wagtail-cjkcms-23.6.2/cjkcms/static/cookieconsent/cookieconsent.js`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/404.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/404.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/500.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/500.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/accordion_block.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/accordion_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/article_block_card.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/article_block_card.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/article_masonry_card.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/article_masonry_card.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/base_link_block.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/base_link_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/button_block.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/button_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/card_block.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/card_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/card_blurb.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/card_blurb.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/card_foot.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/card_foot.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/card_head.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/card_head.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/card_head_foot.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/card_head_foot.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/card_horizontal.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/card_horizontal.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/card_horizontal2.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/card_horizontal2.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/card_img.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/card_img.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/card_landing1.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/card_landing1.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/card_landing2.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/card_landing2.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/cardgrid_columns.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/cardgrid_columns.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/carousel_block.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/carousel_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/download_block.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/download_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/hero_block.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/hero_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/image_gallery_block.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/image_gallery_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/image_link_block.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/image_link_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/modal_block.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/modal_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/pagelist_article_card_columns.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/pagelist_article_card_columns.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/pagelist_article_card_deck.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/pagelist_article_card_deck.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/pagelist_article_media.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/pagelist_article_media.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/pagelist_list_group.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/pagelist_list_group.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/pagelist_toc_nextprev.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/pagelist_toc_nextprev.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/pagepreview_card.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/pagepreview_card.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/pagepreview_form.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/pagepreview_form.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/pricelistitem_block.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/pricelistitem_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/quote_block_leftbar.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/quote_block_leftbar.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/quote_block_start_end_quote.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/quote_block_start_end_quote.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/blocks/table_block.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/table_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/cookieconsent/languages.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/cookieconsent/languages.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/formfields/mailchimp/_2vanilla_subscriber_integration_js.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/formfields/mailchimp/_2vanilla_subscriber_integration_js.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_js.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_js.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_widget.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_widget.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/icons/check-square-o.svg` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/check-square-o.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/icons/font.svg` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/font.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/icons/hand-pointer-o.svg` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/hand-pointer-o.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/icons/hashtag.svg` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/hashtag.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/icons/header.svg` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/header.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/icons/list-alt.svg` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/list-alt.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/icons/puzzle-piece.svg` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/puzzle-piece.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/icons/recycle.svg` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/recycle.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/icons/universal-access.svg` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/universal-access.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/icons/usd.svg` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/usd.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/includes/classifier_dropdowns.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/includes/classifier_dropdowns.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/includes/classifier_nav.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/includes/classifier_nav.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/includes/pagination.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/includes/pagination.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/includes/stream_forms/render_field.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/includes/stream_forms/render_field.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/pages/article_index_page.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/pages/article_index_page.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/pages/article_page.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/pages/article_page.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/pages/article_page.search.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/pages/article_page.search.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/pages/base.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/pages/base.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/pages/form_page.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/pages/form_page.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/pages/search.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/pages/search.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/pages/search_result.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/pages/search_result.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/pages/stream_form_page.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/pages/stream_form_page.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/pages/web_page.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/pages/web_page.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/pages/web_page_notitle.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/pages/web_page_notitle.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/snippets/bottom_corner_lang_selector.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/snippets/bottom_corner_lang_selector.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/snippets/frontend_assets.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/snippets/frontend_assets.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/snippets/frontend_scripts.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/snippets/frontend_scripts.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/snippets/navbar.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/snippets/navbar.html`

 * *Files 3% similar despite different names*

```diff
@@ -27,20 +27,22 @@
     <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-mdb-target="#navbar" data-mdb-toggle="collapse" data-bs-target="#navbar" aria-controls="navbar" aria-expanded="false" aria-label="Toggle navigation">
           <svg xmlns="http://www.w3.org/2000/svg" height="24px" viewBox="0 0 24 24" width="24px" fill="currentColor"><path d="M0 0h24v24H0z" fill="none"/><path d="M3 18h18v-2H3v2zm0-5h18v-2H3v2zm0-7v2h18V6H3z"/></svg>
     </button>
 
     <div class="collapse navbar-collapse" id="navbar">
       {% get_navbars as navbars %}
       {% for navbar in navbars %}
-      <ul class="navbar-nav me-auto mb-2 mb-md-0 {{navbar.custom_css_class}}"
-        {% if navbar.custom_id %}id="{{navbar.custom_id}}"{% endif %} >
-        {% for item in navbar.menu_items %}
-                {% include_block item with liclass="nav-item" aclass="nav-link" ga_event_category="Navbar" %}
-        {% endfor %}
-      </ul>
+        {% if navbar.language == LANGUAGE_CODE or navbar.language == '_all_' %}
+        <ul class="navbar-nav me-auto mb-2 mb-md-0 {{navbar.custom_css_class}}"
+          {% if navbar.custom_id %}id="{{navbar.custom_id}}"{% endif %} >
+          {% for item in navbar.menu_items %}
+                  {% include_block item with liclass="nav-item" aclass="nav-link" ga_event_category="Navbar" %}
+          {% endfor %}
+        </ul>
+        {% endif %}
       {% endfor %}
 
       {% if settings.cjkcms.LayoutSettings.navbar_langselector %}
         {% include settings.cjkcms.LayoutSettings.navbar_langselector %}
       {% endif %}
 
       {% if settings.cjkcms.LayoutSettings.navbar_search %}
```

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/snippets/navbar_lang_selector.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/snippets/navbar_lang_selector.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/snippets/tracking_g4.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/snippets/tracking_g4.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/cjkcms/widgets/checkbox_classifiers.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/widgets/checkbox_classifiers.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/wagtailadmin/block_forms/base_block_settings_struct.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/wagtailadmin/block_forms/base_block_settings_struct.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-{% load wagtailadmin_tags  %}
+{% load wagtailadmin_tags wagtailcore_tags %}
 
-<div class="{{ classname }} cjkcms-collapsible collapsed c-sf-container">
+<div class="{{ classname }} collapsed c-sf-container {% if wagtail_version < 5  %}cjkcms-collapsible4{% else %}cjkcms-collapsible{% endif %}">
     <button type="button" class="button button-small">
       <i class="icon icon-fa-cog" aria-hidden="true"></i> Advanced Settings
     </button>
     <div class="cjkcms-collapsible-target" style="display:none;">
       {% for child in children.values %}
       <div class="field {% if child.block.required %}required{% endif %}" data-contentpath="{{ child.block.name }}">
         {% if child.block.label %}
```

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/wagtailadmin/block_forms/struct.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/wagtailadmin/block_forms/struct.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templates/wagtailadmin/shared/cr_main_nav_2fix.html` & `wagtail-cjkcms-23.6.2/cjkcms/templates/wagtailadmin/shared/cr_main_nav_2fix.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templatetags/cjkcms_tags.py` & `wagtail-cjkcms-23.6.2/cjkcms/templatetags/cjkcms_tags.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templatetags/friendly_loader.py` & `wagtail-cjkcms-23.6.2/cjkcms/templatetags/friendly_loader.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templatetags/gravatar.py` & `wagtail-cjkcms-23.6.2/cjkcms/templatetags/gravatar.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/templatetags/txtutils_tags.py` & `wagtail-cjkcms-23.6.2/cjkcms/templatetags/txtutils_tags.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/tests/test_articlepages.py` & `wagtail-cjkcms-23.6.2/cjkcms/tests/test_articlepages.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/tests/test_gravatar.py` & `wagtail-cjkcms-23.6.2/cjkcms/tests/test_gravatar.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/tests/test_search_blocks.py` & `wagtail-cjkcms-23.6.2/cjkcms/tests/test_search_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/tests/test_settings.py` & `wagtail-cjkcms-23.6.2/cjkcms/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/tests/test_templatetags.py` & `wagtail-cjkcms-23.6.2/cjkcms/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/tests/test_urls.py` & `wagtail-cjkcms-23.6.2/cjkcms/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/tests/test_webpage.py` & `wagtail-cjkcms-23.6.2/cjkcms/tests/test_webpage.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/utils.py` & `wagtail-cjkcms-23.6.2/cjkcms/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/views.py` & `wagtail-cjkcms-23.6.2/cjkcms/views.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/wagtail_hooks.py` & `wagtail-cjkcms-23.6.2/cjkcms/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/cjkcms/widgets.py` & `wagtail-cjkcms-23.6.2/cjkcms/widgets.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/docs/how-to/oembed_finder.md` & `wagtail-cjkcms-23.6.2/docs/how-to/oembed_finder.md`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/docs/index.md` & `wagtail-cjkcms-23.6.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/docs/installation.md` & `wagtail-cjkcms-23.6.2/docs/installation.md`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/docs/quick-start.md` & `wagtail-cjkcms-23.6.2/docs/quick-start.md`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/docs/why-another-cms.md` & `wagtail-cjkcms-23.6.2/docs/why-another-cms.md`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.1/setup.cfg` & `wagtail-cjkcms-23.6.2/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 [flake8]
 max-line-length = 100
 exclude = .*,migrations,build,dist
 
 [codespell]
 ignore-words-list = worl
-skip = migrations,build,dist,*.map
+skip = migrations,build,dist,*.map,package*.json
 
 [mypy]
 ignore_missing_imports = True
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `wagtail-cjkcms-23.6.1/wagtail_cjkcms.egg-info/PKG-INFO` & `wagtail-cjkcms-23.6.2/wagtail_cjkcms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-cjkcms
-Version: 23.6.1
+Version: 23.6.2
 Summary: Wagtail Content Management System, installable as a Django app into any Wagtail 4.x site. Based on Codered CRX.
 Home-page: https://github.com/cjkpl/wagtail-cjkcms
 Author: Grzegorz Krol
 Author-email: gk@cjk.pl
 License: BSD-3-Clause  # Example license
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `wagtail-cjkcms-23.6.1/wagtail_cjkcms.egg-info/SOURCES.txt` & `wagtail-cjkcms-23.6.2/wagtail_cjkcms.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 cjkcms/migrations/0002_alter_body_to_cjkcmsstreamfield.py
 cjkcms/migrations/0003_alter_footer_content_alter_navbar_menu_items.py
 cjkcms/migrations/0004_layoutsettings_articles_date_format_and_more.py
 cjkcms/migrations/0005_layoutsettings_custom_font_and_more.py
 cjkcms/migrations/0006_analyticssettings_consent_modal_layout_and_more.py
 cjkcms/migrations/0007_layoutsettings_bootstrap_icons.py
 cjkcms/migrations/0008_alter_layoutsettings_navbar_langselector.py
+cjkcms/migrations/0009_navbar_language.py
 cjkcms/migrations/__init__.py
 cjkcms/models/__init__.py
 cjkcms/models/admin_sidebar.py
 cjkcms/models/cms_models.py
 cjkcms/models/integration_models.py
 cjkcms/models/page_models.py
 cjkcms/models/snippet_models.py
```

