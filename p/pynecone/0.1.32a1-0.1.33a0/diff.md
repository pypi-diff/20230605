# Comparing `tmp/pynecone-0.1.32a1.tar.gz` & `tmp/pynecone-0.1.33a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynecone-0.1.32a1.tar", max compression
+gzip compressed data, was "pynecone-0.1.33a0.tar", max compression
```

## Comparing `pynecone-0.1.32a1.tar` & `pynecone-0.1.33a0.tar`

### file list

```diff
@@ -1,161 +1,169 @@
--rw-r--r--   0        0        0    11356 2023-01-24 01:31:44.826695 pynecone-0.1.32a1/LICENSE
--rw-r--r--   0        0        0     7876 2023-05-18 00:14:14.758659 pynecone-0.1.32a1/README.md
--rw-r--r--   0        0        0        0 2023-04-27 02:06:35.747147 pynecone-0.1.32a1/pynecone/.templates/apps/counter/__init__.py
--rw-r--r--   0        0        0     1340 2023-05-26 18:52:36.266023 pynecone-0.1.32a1/pynecone/.templates/apps/counter/counter.py
--rw-r--r--   0        0        0        0 2023-04-27 02:06:35.747631 pynecone-0.1.32a1/pynecone/.templates/apps/default/__init__.py
--rw-r--r--   0        0        0     1036 2023-04-27 02:06:35.747905 pynecone-0.1.32a1/pynecone/.templates/apps/default/default.py
--rw-r--r--   0        0        0    15406 2022-11-18 20:43:33.740339 pynecone-0.1.32a1/pynecone/.templates/assets/favicon.ico
--rw-r--r--   0        0        0      183 2023-05-15 02:04:07.604358 pynecone-0.1.32a1/pynecone/.templates/jinja/app/pcconfig.py.jinja2
--rw-r--r--   0        0        0      182 2023-05-15 02:04:07.604515 pynecone-0.1.32a1/pynecone/.templates/jinja/web/pages/_document.js.jinja2
--rw-r--r--   0        0        0      241 2023-05-18 18:33:16.414872 pynecone-0.1.32a1/pynecone/.templates/jinja/web/pages/base_page.js.jinja2
--rw-r--r--   0        0        0      252 2023-05-15 02:04:07.604642 pynecone-0.1.32a1/pynecone/.templates/jinja/web/pages/custom_component.js.jinja2
--rw-r--r--   0        0        0     2318 2023-05-26 18:45:47.400012 pynecone-0.1.32a1/pynecone/.templates/jinja/web/pages/index.js.jinja2
--rw-r--r--   0        0        0     3170 2023-05-22 21:40:04.765805 pynecone-0.1.32a1/pynecone/.templates/jinja/web/pages/utils.js.jinja2
--rw-r--r--   0        0        0       38 2023-05-15 02:04:07.604905 pynecone-0.1.32a1/pynecone/.templates/jinja/web/utils/theme.js.jinja2
--rw-r--r--   0        0        0      417 2022-12-27 07:35:12.085907 pynecone-0.1.32a1/pynecone/.templates/web/.gitignore
--rwxr-xr-x   0        0        0   257247 2023-05-26 18:45:47.401731 pynecone-0.1.32a1/pynecone/.templates/web/bun.lockb
--rw-r--r--   0        0        0       50 2023-05-26 18:45:47.402096 pynecone-0.1.32a1/pynecone/.templates/web/jsconfig.json
--rw-r--r--   0        0        0       47 2022-12-20 23:31:29.590974 pynecone-0.1.32a1/pynecone/.templates/web/next.config.js
--rw-r--r--   0        0        0      964 2023-05-26 18:45:47.402562 pynecone-0.1.32a1/pynecone/.templates/web/package.json
--rw-r--r--   0        0        0      502 2022-11-18 20:43:33.740024 pynecone-0.1.32a1/pynecone/.templates/web/pages/404.js
--rw-r--r--   0        0        0      564 2023-01-12 05:38:04.342282 pynecone-0.1.32a1/pynecone/.templates/web/pages/_app.js
--rw-r--r--   0        0        0    29404 2022-12-20 23:31:29.592485 pynecone-0.1.32a1/pynecone/.templates/web/styles/code/prism.js
--rw-r--r--   0        0        0     7919 2023-05-26 18:45:47.402930 pynecone-0.1.32a1/pynecone/.templates/web/utils/state.js
--rw-r--r--   0        0        0     1406 2023-05-26 18:52:40.786510 pynecone-0.1.32a1/pynecone/__init__.py
--rw-r--r--   0        0        0    19719 2023-05-22 21:40:04.766707 pynecone-0.1.32a1/pynecone/app.py
--rw-r--r--   0        0        0     2524 2023-05-18 00:14:14.759391 pynecone-0.1.32a1/pynecone/base.py
--rw-r--r--   0        0        0       29 2022-11-18 20:43:33.740719 pynecone-0.1.32a1/pynecone/compiler/__init__.py
--rw-r--r--   0        0        0     6216 2023-05-26 18:45:47.403217 pynecone-0.1.32a1/pynecone/compiler/compiler.py
--rw-r--r--   0        0        0     2565 2023-05-15 02:04:07.607300 pynecone-0.1.32a1/pynecone/compiler/templates.py
--rw-r--r--   0        0        0     7761 2023-05-26 18:52:40.786731 pynecone-0.1.32a1/pynecone/compiler/utils.py
--rw-r--r--   0        0        0     6808 2023-05-26 18:45:51.486169 pynecone-0.1.32a1/pynecone/components/__init__.py
--rw-r--r--   0        0        0      226 2023-03-13 04:10:28.615930 pynecone-0.1.32a1/pynecone/components/base/__init__.py
--rw-r--r--   0        0        0      727 2023-05-15 02:04:07.607680 pynecone-0.1.32a1/pynecone/components/base/bare.py
--rw-r--r--   0        0        0      153 2023-03-13 04:10:28.760655 pynecone-0.1.32a1/pynecone/components/base/body.py
--rw-r--r--   0        0        0      725 2023-01-30 22:40:32.678074 pynecone-0.1.32a1/pynecone/components/base/document.py
--rw-r--r--   0        0        0      265 2023-05-15 02:04:07.607851 pynecone-0.1.32a1/pynecone/components/base/head.py
--rw-r--r--   0        0        0      930 2023-05-15 02:04:07.607989 pynecone-0.1.32a1/pynecone/components/base/link.py
--rw-r--r--   0        0        0     1340 2023-05-15 02:04:07.608303 pynecone-0.1.32a1/pynecone/components/base/meta.py
--rw-r--r--   0        0        0    24243 2023-05-26 18:52:40.786960 pynecone-0.1.32a1/pynecone/components/component.py
--rw-r--r--   0        0        0      496 2023-05-26 18:45:47.404646 pynecone-0.1.32a1/pynecone/components/datadisplay/__init__.py
--rw-r--r--   0        0        0      334 2023-05-15 02:04:07.608726 pynecone-0.1.32a1/pynecone/components/datadisplay/badge.py
--rw-r--r--   0        0        0     2513 2023-05-15 02:04:07.608840 pynecone-0.1.32a1/pynecone/components/datadisplay/code.py
--rw-r--r--   0        0        0     4033 2023-05-15 02:04:07.608953 pynecone-0.1.32a1/pynecone/components/datadisplay/datatable.py
--rw-r--r--   0        0        0      537 2023-05-15 02:04:07.609045 pynecone-0.1.32a1/pynecone/components/datadisplay/divider.py
--rw-r--r--   0        0        0      187 2023-04-02 23:51:14.632124 pynecone-0.1.32a1/pynecone/components/datadisplay/keyboard_key.py
--rw-r--r--   0        0        0     1430 2023-05-15 02:04:07.609140 pynecone-0.1.32a1/pynecone/components/datadisplay/list.py
--rw-r--r--   0        0        0     2157 2023-05-15 02:04:07.609232 pynecone-0.1.32a1/pynecone/components/datadisplay/stat.py
--rw-r--r--   0        0        0     5793 2023-05-26 18:45:47.405454 pynecone-0.1.32a1/pynecone/components/datadisplay/table.py
--rw-r--r--   0        0        0     2188 2023-05-26 18:45:47.406072 pynecone-0.1.32a1/pynecone/components/datadisplay/tag.py
--rw-r--r--   0        0        0      384 2023-05-26 18:45:47.406587 pynecone-0.1.32a1/pynecone/components/disclosure/__init__.py
--rw-r--r--   0        0        0     2941 2023-05-15 02:04:07.609439 pynecone-0.1.32a1/pynecone/components/disclosure/accordion.py
--rw-r--r--   0        0        0     2777 2023-05-15 02:04:07.609534 pynecone-0.1.32a1/pynecone/components/disclosure/tabs.py
--rw-r--r--   0        0        0     1741 2023-05-26 18:45:47.406922 pynecone-0.1.32a1/pynecone/components/disclosure/transition.py
--rw-r--r--   0        0        0      285 2022-12-05 22:26:47.605453 pynecone-0.1.32a1/pynecone/components/disclosure/visuallyhidden.py
--rw-r--r--   0        0        0      313 2022-11-18 20:43:33.723246 pynecone-0.1.32a1/pynecone/components/feedback/__init__.py
--rw-r--r--   0        0        0     1571 2023-05-15 02:04:07.609649 pynecone-0.1.32a1/pynecone/components/feedback/alert.py
--rw-r--r--   0        0        0     1905 2023-05-15 02:04:07.609745 pynecone-0.1.32a1/pynecone/components/feedback/circularprogress.py
--rw-r--r--   0        0        0      879 2023-05-15 02:04:07.609838 pynecone-0.1.32a1/pynecone/components/feedback/progress.py
--rw-r--r--   0        0        0     1785 2023-05-15 02:04:07.609925 pynecone-0.1.32a1/pynecone/components/feedback/skeleton.py
--rw-r--r--   0        0        0      678 2023-05-15 02:04:07.610013 pynecone-0.1.32a1/pynecone/components/feedback/spinner.py
--rw-r--r--   0        0        0     1102 2023-05-26 18:45:47.407173 pynecone-0.1.32a1/pynecone/components/forms/__init__.py
--rw-r--r--   0        0        0     1765 2023-05-15 17:32:17.392510 pynecone-0.1.32a1/pynecone/components/forms/button.py
--rw-r--r--   0        0        0     2454 2023-05-18 00:14:14.760429 pynecone-0.1.32a1/pynecone/components/forms/checkbox.py
--rw-r--r--   0        0        0      578 2023-05-18 00:14:14.760629 pynecone-0.1.32a1/pynecone/components/forms/copytoclipboard.py
--rw-r--r--   0        0        0     1949 2023-05-18 00:14:14.760816 pynecone-0.1.32a1/pynecone/components/forms/editable.py
--rw-r--r--   0        0        0     2996 2023-05-26 18:45:47.407573 pynecone-0.1.32a1/pynecone/components/forms/form.py
--rw-r--r--   0        0        0      802 2023-05-15 02:04:07.610729 pynecone-0.1.32a1/pynecone/components/forms/iconbutton.py
--rw-r--r--   0        0        0     2880 2023-05-18 00:14:14.761287 pynecone-0.1.32a1/pynecone/components/forms/input.py
--rw-r--r--   0        0        0     3897 2023-05-18 00:14:14.761460 pynecone-0.1.32a1/pynecone/components/forms/numberinput.py
--rw-r--r--   0        0        0      253 2023-05-15 02:04:07.611101 pynecone-0.1.32a1/pynecone/components/forms/password.py
--rw-r--r--   0        0        0     2670 2023-05-18 00:14:14.761619 pynecone-0.1.32a1/pynecone/components/forms/pininput.py
--rw-r--r--   0        0        0     3043 2023-05-18 00:14:14.761823 pynecone-0.1.32a1/pynecone/components/forms/radio.py
--rw-r--r--   0        0        0     2853 2023-05-18 00:14:14.761962 pynecone-0.1.32a1/pynecone/components/forms/rangeslider.py
--rw-r--r--   0        0        0    12667 2023-05-26 18:45:47.407983 pynecone-0.1.32a1/pynecone/components/forms/select.py
--rw-r--r--   0        0        0     3124 2023-05-18 00:14:14.762261 pynecone-0.1.32a1/pynecone/components/forms/slider.py
--rw-r--r--   0        0        0     1552 2023-05-18 00:14:14.762398 pynecone-0.1.32a1/pynecone/components/forms/switch.py
--rw-r--r--   0        0        0     1531 2023-05-18 00:14:14.762541 pynecone-0.1.32a1/pynecone/components/forms/textarea.py
--rw-r--r--   0        0        0     2915 2023-05-18 00:14:14.762683 pynecone-0.1.32a1/pynecone/components/forms/upload.py
--rw-r--r--   0        0        0      351 2023-01-24 02:43:48.879007 pynecone-0.1.32a1/pynecone/components/graphing/__init__.py
--rw-r--r--   0        0        0     1357 2023-05-15 02:04:07.613685 pynecone-0.1.32a1/pynecone/components/graphing/plotly.py
--rw-r--r--   0        0        0    17360 2023-05-15 02:04:07.613960 pynecone-0.1.32a1/pynecone/components/graphing/victory.py
--rw-r--r--   0        0        0      872 2023-05-22 21:39:53.010163 pynecone-0.1.32a1/pynecone/components/layout/__init__.py
--rw-r--r--   0        0        0      324 2023-05-15 02:04:07.614167 pynecone-0.1.32a1/pynecone/components/layout/aspect_ratio.py
--rw-r--r--   0        0        0      769 2023-05-15 02:04:07.614311 pynecone-0.1.32a1/pynecone/components/layout/box.py
--rw-r--r--   0        0        0     2859 2023-05-22 21:39:53.010378 pynecone-0.1.32a1/pynecone/components/layout/card.py
--rw-r--r--   0        0        0      396 2022-12-07 23:08:48.792563 pynecone-0.1.32a1/pynecone/components/layout/center.py
--rw-r--r--   0        0        0     3844 2023-05-18 00:14:14.762938 pynecone-0.1.32a1/pynecone/components/layout/cond.py
--rw-r--r--   0        0        0      363 2023-05-15 02:04:07.614634 pynecone-0.1.32a1/pynecone/components/layout/container.py
--rw-r--r--   0        0        0      656 2023-05-15 02:04:07.614740 pynecone-0.1.32a1/pynecone/components/layout/flex.py
--rw-r--r--   0        0        0     3167 2023-05-26 18:45:47.408238 pynecone-0.1.32a1/pynecone/components/layout/foreach.py
--rw-r--r--   0        0        0      314 2022-12-20 23:31:29.595612 pynecone-0.1.32a1/pynecone/components/layout/fragment.py
--rw-r--r--   0        0        0     2418 2023-05-15 02:04:07.614987 pynecone-0.1.32a1/pynecone/components/layout/grid.py
--rw-r--r--   0        0        0      979 2023-04-27 02:06:35.755389 pynecone-0.1.32a1/pynecone/components/layout/html.py
--rw-r--r--   0        0        0     1900 2023-03-10 00:25:42.702272 pynecone-0.1.32a1/pynecone/components/layout/responsive.py
--rw-r--r--   0        0        0      186 2022-12-07 23:08:48.793614 pynecone-0.1.32a1/pynecone/components/layout/spacer.py
--rw-r--r--   0        0        0      995 2023-05-15 02:04:07.615111 pynecone-0.1.32a1/pynecone/components/layout/stack.py
--rw-r--r--   0        0        0     1471 2023-05-15 02:04:07.615242 pynecone-0.1.32a1/pynecone/components/layout/wrap.py
--rw-r--r--   0        0        0       33 2022-11-18 20:43:33.727543 pynecone-0.1.32a1/pynecone/components/libs/__init__.py
--rw-r--r--   0        0        0      222 2022-11-18 20:43:33.727419 pynecone-0.1.32a1/pynecone/components/libs/chakra.py
--rw-r--r--   0        0        0      190 2022-11-18 20:43:33.736163 pynecone-0.1.32a1/pynecone/components/media/__init__.py
--rw-r--r--   0        0        0     1524 2023-05-18 00:14:14.763360 pynecone-0.1.32a1/pynecone/components/media/avatar.py
--rw-r--r--   0        0        0     2391 2023-03-16 23:52:12.745547 pynecone-0.1.32a1/pynecone/components/media/icon.py
--rw-r--r--   0        0        0     1400 2023-05-18 00:14:14.763528 pynecone-0.1.32a1/pynecone/components/media/image.py
--rw-r--r--   0        0        0      282 2023-01-24 02:43:48.884756 pynecone-0.1.32a1/pynecone/components/navigation/__init__.py
--rw-r--r--   0        0        0     2023 2023-05-15 02:04:07.615856 pynecone-0.1.32a1/pynecone/components/navigation/breadcrumb.py
--rw-r--r--   0        0        0     1082 2023-05-26 18:45:47.408434 pynecone-0.1.32a1/pynecone/components/navigation/link.py
--rw-r--r--   0        0        0      530 2023-05-15 02:04:07.616129 pynecone-0.1.32a1/pynecone/components/navigation/linkoverlay.py
--rw-r--r--   0        0        0      507 2023-05-15 02:04:07.616229 pynecone-0.1.32a1/pynecone/components/navigation/nextlink.py
--rw-r--r--   0        0        0      850 2023-01-24 02:43:48.892006 pynecone-0.1.32a1/pynecone/components/overlay/__init__.py
--rw-r--r--   0        0        0     5027 2023-05-18 00:14:14.763711 pynecone-0.1.32a1/pynecone/components/overlay/alertdialog.py
--rw-r--r--   0        0        0     4681 2023-05-18 00:14:14.763867 pynecone-0.1.32a1/pynecone/components/overlay/drawer.py
--rw-r--r--   0        0        0     5530 2023-05-18 00:14:14.764021 pynecone-0.1.32a1/pynecone/components/overlay/menu.py
--rw-r--r--   0        0        0     4917 2023-05-18 00:14:14.764177 pynecone-0.1.32a1/pynecone/components/overlay/modal.py
--rw-r--r--   0        0        0     5688 2023-05-18 00:14:14.764341 pynecone-0.1.32a1/pynecone/components/overlay/popover.py
--rw-r--r--   0        0        0     1949 2023-05-18 00:14:14.764530 pynecone-0.1.32a1/pynecone/components/overlay/tooltip.py
--rw-r--r--   0        0        0      120 2022-11-18 20:43:33.725191 pynecone-0.1.32a1/pynecone/components/tags/__init__.py
--rw-r--r--   0        0        0      451 2023-05-15 02:04:07.617454 pynecone-0.1.32a1/pynecone/components/tags/cond_tag.py
--rw-r--r--   0        0        0     2306 2023-05-15 02:04:07.617560 pynecone-0.1.32a1/pynecone/components/tags/iter_tag.py
--rw-r--r--   0        0        0     5018 2023-05-18 00:14:14.764773 pynecone-0.1.32a1/pynecone/components/tags/tag.py
--rw-r--r--   0        0        0      591 2023-03-16 23:52:12.746470 pynecone-0.1.32a1/pynecone/components/tags/tagless.py
--rw-r--r--   0        0        0      304 2023-05-26 18:45:51.486474 pynecone-0.1.32a1/pynecone/components/typography/__init__.py
--rw-r--r--   0        0        0      282 2023-05-15 02:04:07.617958 pynecone-0.1.32a1/pynecone/components/typography/heading.py
--rw-r--r--   0        0        0      682 2023-05-26 18:45:51.486717 pynecone-0.1.32a1/pynecone/components/typography/highlight.py
--rw-r--r--   0        0        0     3288 2023-05-15 02:04:07.618181 pynecone-0.1.32a1/pynecone/components/typography/markdown.py
--rw-r--r--   0        0        0      337 2023-05-15 02:04:07.618372 pynecone-0.1.32a1/pynecone/components/typography/span.py
--rw-r--r--   0        0        0      306 2023-05-15 02:04:07.618520 pynecone-0.1.32a1/pynecone/components/typography/text.py
--rw-r--r--   0        0        0     5368 2023-05-26 18:45:47.409429 pynecone-0.1.32a1/pynecone/config.py
--rw-r--r--   0        0        0     9018 2023-05-26 18:45:47.409730 pynecone-0.1.32a1/pynecone/constants.py
--rw-r--r--   0        0        0       73 2023-04-27 02:06:35.757531 pynecone-0.1.32a1/pynecone/el/__init__.py
--rw-r--r--   0        0        0      115 2023-04-27 02:06:35.757829 pynecone-0.1.32a1/pynecone/el/constants/__init__.py
--rw-r--r--   0        0        0     7175 2023-04-27 02:06:35.758045 pynecone-0.1.32a1/pynecone/el/constants/html.py
--rw-r--r--   0        0        0     1719 2023-04-27 02:06:35.758325 pynecone-0.1.32a1/pynecone/el/constants/pynecone.py
--rw-r--r--   0        0        0    15554 2023-04-27 02:06:35.758673 pynecone-0.1.32a1/pynecone/el/constants/react.py
--rw-r--r--   0        0        0     1283 2023-05-15 02:04:07.619213 pynecone-0.1.32a1/pynecone/el/element.py
--rw-r--r--   0        0        0   108518 2023-05-15 02:04:07.619552 pynecone-0.1.32a1/pynecone/el/elements/__init__.py
--rwxr-xr-x   0        0        0     2667 2023-05-15 02:04:07.619858 pynecone-0.1.32a1/pynecone/el/precompile.py
--rw-r--r--   0        0        0    10669 2023-05-26 18:45:47.410006 pynecone-0.1.32a1/pynecone/event.py
--rw-r--r--   0        0        0      113 2023-05-15 02:04:07.620772 pynecone-0.1.32a1/pynecone/middleware/__init__.py
--rw-r--r--   0        0        0     1738 2023-05-15 02:04:07.621034 pynecone-0.1.32a1/pynecone/middleware/hydrate_middleware.py
--rw-r--r--   0        0        0     1167 2023-05-15 02:04:07.621188 pynecone-0.1.32a1/pynecone/middleware/middleware.py
--rw-r--r--   0        0        0     2085 2023-04-27 23:08:51.380631 pynecone-0.1.32a1/pynecone/model.py
--rw-r--r--   0        0        0     8099 2023-05-26 18:45:47.410229 pynecone-0.1.32a1/pynecone/pc.py
--rw-r--r--   0        0        0        0 2023-03-10 00:25:42.707141 pynecone-0.1.32a1/pynecone/py.typed
--rw-r--r--   0        0        0     4108 2023-03-16 23:52:12.748303 pynecone-0.1.32a1/pynecone/route.py
--rw-r--r--   0        0        0    29790 2023-05-15 02:04:07.621653 pynecone-0.1.32a1/pynecone/state.py
--rw-r--r--   0        0        0     1060 2023-05-15 02:04:07.621889 pynecone-0.1.32a1/pynecone/style.py
--rw-r--r--   0        0        0       26 2023-05-15 02:04:07.622076 pynecone-0.1.32a1/pynecone/utils/__init__.py
--rw-r--r--   0        0        0     7211 2023-05-26 18:45:47.410540 pynecone-0.1.32a1/pynecone/utils/build.py
--rw-r--r--   0        0        0     1759 2023-05-15 02:04:07.622587 pynecone-0.1.32a1/pynecone/utils/console.py
--rw-r--r--   0        0        0     5211 2023-05-26 18:45:47.410760 pynecone-0.1.32a1/pynecone/utils/exec.py
--rw-r--r--   0        0        0    11334 2023-05-18 00:14:14.765753 pynecone-0.1.32a1/pynecone/utils/format.py
--rw-r--r--   0        0        0      587 2023-05-15 02:04:07.623144 pynecone-0.1.32a1/pynecone/utils/imports.py
--rw-r--r--   0        0        0     2451 2023-03-16 23:52:12.757162 pynecone-0.1.32a1/pynecone/utils/path_ops.py
--rw-r--r--   0        0        0    10033 2023-05-17 03:31:04.698132 pynecone-0.1.32a1/pynecone/utils/prerequisites.py
--rw-r--r--   0        0        0     3021 2023-03-16 23:52:12.757337 pynecone-0.1.32a1/pynecone/utils/processes.py
--rw-r--r--   0        0        0     2397 2023-05-15 02:04:07.623496 pynecone-0.1.32a1/pynecone/utils/telemetry.py
--rw-r--r--   0        0        0     4394 2023-05-18 00:14:14.765933 pynecone-0.1.32a1/pynecone/utils/types.py
--rw-r--r--   0        0        0     2634 2023-05-15 02:04:07.623722 pynecone-0.1.32a1/pynecone/utils/watch.py
--rw-r--r--   0        0        0    30928 2023-05-18 00:14:14.766310 pynecone-0.1.32a1/pynecone/vars.py
--rw-r--r--   0        0        0     1798 2023-05-26 18:57:43.917351 pynecone-0.1.32a1/pyproject.toml
--rw-r--r--   0        0        0     9407 1970-01-01 00:00:00.000000 pynecone-0.1.32a1/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-01-24 01:31:44.826695 pynecone-0.1.33a0/LICENSE
+-rw-r--r--   0        0        0     7876 2023-05-18 00:14:14.758659 pynecone-0.1.33a0/README.md
+-rw-r--r--   0        0        0        0 2023-04-27 02:06:35.747147 pynecone-0.1.33a0/pynecone/.templates/apps/counter/__init__.py
+-rw-r--r--   0        0        0     1340 2023-06-03 03:13:15.297910 pynecone-0.1.33a0/pynecone/.templates/apps/counter/counter.py
+-rw-r--r--   0        0        0        0 2023-04-27 02:06:35.747631 pynecone-0.1.33a0/pynecone/.templates/apps/default/__init__.py
+-rw-r--r--   0        0        0     1036 2023-04-27 02:06:35.747905 pynecone-0.1.33a0/pynecone/.templates/apps/default/default.py
+-rw-r--r--   0        0        0    15406 2022-11-18 20:43:33.740339 pynecone-0.1.33a0/pynecone/.templates/assets/favicon.ico
+-rw-r--r--   0        0        0      183 2023-05-15 02:04:07.604358 pynecone-0.1.33a0/pynecone/.templates/jinja/app/pcconfig.py.jinja2
+-rw-r--r--   0        0        0      182 2023-05-15 02:04:07.604515 pynecone-0.1.33a0/pynecone/.templates/jinja/web/pages/_document.js.jinja2
+-rw-r--r--   0        0        0      241 2023-05-18 18:33:16.414872 pynecone-0.1.33a0/pynecone/.templates/jinja/web/pages/base_page.js.jinja2
+-rw-r--r--   0        0        0      252 2023-05-15 02:04:07.604642 pynecone-0.1.33a0/pynecone/.templates/jinja/web/pages/custom_component.js.jinja2
+-rw-r--r--   0        0        0     2558 2023-06-05 21:02:06.179237 pynecone-0.1.33a0/pynecone/.templates/jinja/web/pages/index.js.jinja2
+-rw-r--r--   0        0        0     3170 2023-05-22 21:40:04.765805 pynecone-0.1.33a0/pynecone/.templates/jinja/web/pages/utils.js.jinja2
+-rw-r--r--   0        0        0       38 2023-05-15 02:04:07.604905 pynecone-0.1.33a0/pynecone/.templates/jinja/web/utils/theme.js.jinja2
+-rw-r--r--   0        0        0      417 2022-12-27 07:35:12.085907 pynecone-0.1.33a0/pynecone/.templates/web/.gitignore
+-rwxr-xr-x   0        0        0   257247 2023-05-26 18:45:47.401731 pynecone-0.1.33a0/pynecone/.templates/web/bun.lockb
+-rw-r--r--   0        0        0       50 2023-05-26 18:45:47.402096 pynecone-0.1.33a0/pynecone/.templates/web/jsconfig.json
+-rw-r--r--   0        0        0       47 2022-12-20 23:31:29.590974 pynecone-0.1.33a0/pynecone/.templates/web/next.config.js
+-rw-r--r--   0        0        0      995 2023-06-01 03:15:26.563786 pynecone-0.1.33a0/pynecone/.templates/web/package.json
+-rw-r--r--   0        0        0      502 2022-11-18 20:43:33.740024 pynecone-0.1.33a0/pynecone/.templates/web/pages/404.js
+-rw-r--r--   0        0        0      564 2023-01-12 05:38:04.342282 pynecone-0.1.33a0/pynecone/.templates/web/pages/_app.js
+-rw-r--r--   0        0        0    29404 2022-12-20 23:31:29.592485 pynecone-0.1.33a0/pynecone/.templates/web/styles/code/prism.js
+-rw-r--r--   0        0        0     8262 2023-06-05 21:02:06.181267 pynecone-0.1.33a0/pynecone/.templates/web/utils/state.js
+-rw-r--r--   0        0        0     1448 2023-06-01 03:12:11.084175 pynecone-0.1.33a0/pynecone/__init__.py
+-rw-r--r--   0        0        0    20197 2023-06-05 21:02:06.182089 pynecone-0.1.33a0/pynecone/app.py
+-rw-r--r--   0        0        0     2524 2023-05-18 00:14:14.759391 pynecone-0.1.33a0/pynecone/base.py
+-rw-r--r--   0        0        0       29 2022-11-18 20:43:33.740719 pynecone-0.1.33a0/pynecone/compiler/__init__.py
+-rw-r--r--   0        0        0     6688 2023-06-05 21:02:06.185518 pynecone-0.1.33a0/pynecone/compiler/compiler.py
+-rw-r--r--   0        0        0     2565 2023-05-15 02:04:07.607300 pynecone-0.1.33a0/pynecone/compiler/templates.py
+-rw-r--r--   0        0        0     7761 2023-06-01 00:32:59.071818 pynecone-0.1.33a0/pynecone/compiler/utils.py
+-rw-r--r--   0        0        0     7062 2023-06-05 21:02:06.186808 pynecone-0.1.33a0/pynecone/components/__init__.py
+-rw-r--r--   0        0        0      226 2023-03-13 04:10:28.615930 pynecone-0.1.33a0/pynecone/components/base/__init__.py
+-rw-r--r--   0        0        0      727 2023-05-15 02:04:07.607680 pynecone-0.1.33a0/pynecone/components/base/bare.py
+-rw-r--r--   0        0        0      153 2023-03-13 04:10:28.760655 pynecone-0.1.33a0/pynecone/components/base/body.py
+-rw-r--r--   0        0        0      725 2023-01-30 22:40:32.678074 pynecone-0.1.33a0/pynecone/components/base/document.py
+-rw-r--r--   0        0        0      265 2023-05-15 02:04:07.607851 pynecone-0.1.33a0/pynecone/components/base/head.py
+-rw-r--r--   0        0        0      930 2023-05-15 02:04:07.607989 pynecone-0.1.33a0/pynecone/components/base/link.py
+-rw-r--r--   0        0        0     1340 2023-05-15 02:04:07.608303 pynecone-0.1.33a0/pynecone/components/base/meta.py
+-rw-r--r--   0        0        0    24243 2023-06-01 00:32:59.072142 pynecone-0.1.33a0/pynecone/components/component.py
+-rw-r--r--   0        0        0      496 2023-05-26 18:45:47.404646 pynecone-0.1.33a0/pynecone/components/datadisplay/__init__.py
+-rw-r--r--   0        0        0      334 2023-05-15 02:04:07.608726 pynecone-0.1.33a0/pynecone/components/datadisplay/badge.py
+-rw-r--r--   0        0        0     2513 2023-05-15 02:04:07.608840 pynecone-0.1.33a0/pynecone/components/datadisplay/code.py
+-rw-r--r--   0        0        0     4033 2023-05-15 02:04:07.608953 pynecone-0.1.33a0/pynecone/components/datadisplay/datatable.py
+-rw-r--r--   0        0        0      537 2023-05-15 02:04:07.609045 pynecone-0.1.33a0/pynecone/components/datadisplay/divider.py
+-rw-r--r--   0        0        0      187 2023-04-02 23:51:14.632124 pynecone-0.1.33a0/pynecone/components/datadisplay/keyboard_key.py
+-rw-r--r--   0        0        0     1430 2023-05-15 02:04:07.609140 pynecone-0.1.33a0/pynecone/components/datadisplay/list.py
+-rw-r--r--   0        0        0     2157 2023-05-15 02:04:07.609232 pynecone-0.1.33a0/pynecone/components/datadisplay/stat.py
+-rw-r--r--   0        0        0     5793 2023-05-26 18:45:47.405454 pynecone-0.1.33a0/pynecone/components/datadisplay/table.py
+-rw-r--r--   0        0        0     2188 2023-05-26 18:45:47.406072 pynecone-0.1.33a0/pynecone/components/datadisplay/tag.py
+-rw-r--r--   0        0        0      384 2023-05-26 18:45:47.406587 pynecone-0.1.33a0/pynecone/components/disclosure/__init__.py
+-rw-r--r--   0        0        0     2941 2023-05-15 02:04:07.609439 pynecone-0.1.33a0/pynecone/components/disclosure/accordion.py
+-rw-r--r--   0        0        0     2777 2023-05-15 02:04:07.609534 pynecone-0.1.33a0/pynecone/components/disclosure/tabs.py
+-rw-r--r--   0        0        0     1741 2023-05-26 18:45:47.406922 pynecone-0.1.33a0/pynecone/components/disclosure/transition.py
+-rw-r--r--   0        0        0      285 2022-12-05 22:26:47.605453 pynecone-0.1.33a0/pynecone/components/disclosure/visuallyhidden.py
+-rw-r--r--   0        0        0      313 2022-11-18 20:43:33.723246 pynecone-0.1.33a0/pynecone/components/feedback/__init__.py
+-rw-r--r--   0        0        0     1571 2023-05-15 02:04:07.609649 pynecone-0.1.33a0/pynecone/components/feedback/alert.py
+-rw-r--r--   0        0        0     1905 2023-05-15 02:04:07.609745 pynecone-0.1.33a0/pynecone/components/feedback/circularprogress.py
+-rw-r--r--   0        0        0      879 2023-05-15 02:04:07.609838 pynecone-0.1.33a0/pynecone/components/feedback/progress.py
+-rw-r--r--   0        0        0     1785 2023-05-15 02:04:07.609925 pynecone-0.1.33a0/pynecone/components/feedback/skeleton.py
+-rw-r--r--   0        0        0      678 2023-05-15 02:04:07.610013 pynecone-0.1.33a0/pynecone/components/feedback/spinner.py
+-rw-r--r--   0        0        0     1308 2023-06-05 03:00:53.230974 pynecone-0.1.33a0/pynecone/components/forms/__init__.py
+-rw-r--r--   0        0        0     1765 2023-05-15 17:32:17.392510 pynecone-0.1.33a0/pynecone/components/forms/button.py
+-rw-r--r--   0        0        0     2454 2023-05-18 00:14:14.760429 pynecone-0.1.33a0/pynecone/components/forms/checkbox.py
+-rw-r--r--   0        0        0      578 2023-05-18 00:14:14.760629 pynecone-0.1.33a0/pynecone/components/forms/copytoclipboard.py
+-rw-r--r--   0        0        0      243 2023-06-05 03:00:53.231067 pynecone-0.1.33a0/pynecone/components/forms/date_picker.py
+-rw-r--r--   0        0        0      277 2023-06-05 03:00:53.231162 pynecone-0.1.33a0/pynecone/components/forms/date_time_picker.py
+-rw-r--r--   0        0        0     1949 2023-05-18 00:14:14.760816 pynecone-0.1.33a0/pynecone/components/forms/editable.py
+-rw-r--r--   0        0        0      243 2023-06-01 00:48:48.431001 pynecone-0.1.33a0/pynecone/components/forms/email.py
+-rw-r--r--   0        0        0     2996 2023-05-26 18:45:47.407573 pynecone-0.1.33a0/pynecone/components/forms/form.py
+-rw-r--r--   0        0        0      802 2023-05-15 02:04:07.610729 pynecone-0.1.33a0/pynecone/components/forms/iconbutton.py
+-rw-r--r--   0        0        0     2880 2023-05-18 00:14:14.761287 pynecone-0.1.33a0/pynecone/components/forms/input.py
+-rw-r--r--   0        0        0    12667 2023-06-03 03:13:18.319215 pynecone-0.1.33a0/pynecone/components/forms/multiselect.py
+-rw-r--r--   0        0        0     3897 2023-05-18 00:14:14.761460 pynecone-0.1.33a0/pynecone/components/forms/numberinput.py
+-rw-r--r--   0        0        0      253 2023-05-15 02:04:07.611101 pynecone-0.1.33a0/pynecone/components/forms/password.py
+-rw-r--r--   0        0        0     2670 2023-05-18 00:14:14.761619 pynecone-0.1.33a0/pynecone/components/forms/pininput.py
+-rw-r--r--   0        0        0     3043 2023-05-18 00:14:14.761823 pynecone-0.1.33a0/pynecone/components/forms/radio.py
+-rw-r--r--   0        0        0     2853 2023-05-18 00:14:14.761962 pynecone-0.1.33a0/pynecone/components/forms/rangeslider.py
+-rw-r--r--   0        0        0     3522 2023-06-03 03:13:18.320175 pynecone-0.1.33a0/pynecone/components/forms/select.py
+-rw-r--r--   0        0        0     3124 2023-05-18 00:14:14.762261 pynecone-0.1.33a0/pynecone/components/forms/slider.py
+-rw-r--r--   0        0        0     1552 2023-05-18 00:14:14.762398 pynecone-0.1.33a0/pynecone/components/forms/switch.py
+-rw-r--r--   0        0        0     1531 2023-05-18 00:14:14.762541 pynecone-0.1.33a0/pynecone/components/forms/textarea.py
+-rw-r--r--   0        0        0     2915 2023-05-18 00:14:14.762683 pynecone-0.1.33a0/pynecone/components/forms/upload.py
+-rw-r--r--   0        0        0      351 2023-01-24 02:43:48.879007 pynecone-0.1.33a0/pynecone/components/graphing/__init__.py
+-rw-r--r--   0        0        0     1357 2023-05-15 02:04:07.613685 pynecone-0.1.33a0/pynecone/components/graphing/plotly.py
+-rw-r--r--   0        0        0    17360 2023-05-15 02:04:07.613960 pynecone-0.1.33a0/pynecone/components/graphing/victory.py
+-rw-r--r--   0        0        0      872 2023-05-22 21:39:53.010163 pynecone-0.1.33a0/pynecone/components/layout/__init__.py
+-rw-r--r--   0        0        0      324 2023-05-15 02:04:07.614167 pynecone-0.1.33a0/pynecone/components/layout/aspect_ratio.py
+-rw-r--r--   0        0        0      769 2023-05-15 02:04:07.614311 pynecone-0.1.33a0/pynecone/components/layout/box.py
+-rw-r--r--   0        0        0     2859 2023-05-22 21:39:53.010378 pynecone-0.1.33a0/pynecone/components/layout/card.py
+-rw-r--r--   0        0        0      396 2022-12-07 23:08:48.792563 pynecone-0.1.33a0/pynecone/components/layout/center.py
+-rw-r--r--   0        0        0     3844 2023-05-18 00:14:14.762938 pynecone-0.1.33a0/pynecone/components/layout/cond.py
+-rw-r--r--   0        0        0      363 2023-05-15 02:04:07.614634 pynecone-0.1.33a0/pynecone/components/layout/container.py
+-rw-r--r--   0        0        0      656 2023-05-15 02:04:07.614740 pynecone-0.1.33a0/pynecone/components/layout/flex.py
+-rw-r--r--   0        0        0     3167 2023-05-26 18:45:47.408238 pynecone-0.1.33a0/pynecone/components/layout/foreach.py
+-rw-r--r--   0        0        0      314 2022-12-20 23:31:29.595612 pynecone-0.1.33a0/pynecone/components/layout/fragment.py
+-rw-r--r--   0        0        0     2418 2023-05-15 02:04:07.614987 pynecone-0.1.33a0/pynecone/components/layout/grid.py
+-rw-r--r--   0        0        0      979 2023-05-30 04:03:19.236282 pynecone-0.1.33a0/pynecone/components/layout/html.py
+-rw-r--r--   0        0        0     1900 2023-03-10 00:25:42.702272 pynecone-0.1.33a0/pynecone/components/layout/responsive.py
+-rw-r--r--   0        0        0      186 2022-12-07 23:08:48.793614 pynecone-0.1.33a0/pynecone/components/layout/spacer.py
+-rw-r--r--   0        0        0      995 2023-05-15 02:04:07.615111 pynecone-0.1.33a0/pynecone/components/layout/stack.py
+-rw-r--r--   0        0        0     1471 2023-05-15 02:04:07.615242 pynecone-0.1.33a0/pynecone/components/layout/wrap.py
+-rw-r--r--   0        0        0       33 2022-11-18 20:43:33.727543 pynecone-0.1.33a0/pynecone/components/libs/__init__.py
+-rw-r--r--   0        0        0      222 2022-11-18 20:43:33.727419 pynecone-0.1.33a0/pynecone/components/libs/chakra.py
+-rw-r--r--   0        0        0     1391 2023-06-01 03:15:26.564372 pynecone-0.1.33a0/pynecone/components/libs/react_player.py
+-rw-r--r--   0        0        0      240 2023-06-01 03:15:26.564561 pynecone-0.1.33a0/pynecone/components/media/__init__.py
+-rw-r--r--   0        0        0      197 2023-06-01 03:15:26.564687 pynecone-0.1.33a0/pynecone/components/media/audio.py
+-rw-r--r--   0        0        0     1524 2023-05-18 00:14:14.763360 pynecone-0.1.33a0/pynecone/components/media/avatar.py
+-rw-r--r--   0        0        0     2391 2023-03-16 23:52:12.745547 pynecone-0.1.33a0/pynecone/components/media/icon.py
+-rw-r--r--   0        0        0     1774 2023-06-01 03:15:26.564867 pynecone-0.1.33a0/pynecone/components/media/image.py
+-rw-r--r--   0        0        0      197 2023-06-01 03:15:26.564984 pynecone-0.1.33a0/pynecone/components/media/video.py
+-rw-r--r--   0        0        0      282 2023-01-24 02:43:48.884756 pynecone-0.1.33a0/pynecone/components/navigation/__init__.py
+-rw-r--r--   0        0        0     2023 2023-05-15 02:04:07.615856 pynecone-0.1.33a0/pynecone/components/navigation/breadcrumb.py
+-rw-r--r--   0        0        0     1082 2023-05-26 18:45:47.408434 pynecone-0.1.33a0/pynecone/components/navigation/link.py
+-rw-r--r--   0        0        0      530 2023-05-15 02:04:07.616129 pynecone-0.1.33a0/pynecone/components/navigation/linkoverlay.py
+-rw-r--r--   0        0        0      507 2023-05-15 02:04:07.616229 pynecone-0.1.33a0/pynecone/components/navigation/nextlink.py
+-rw-r--r--   0        0        0      887 2023-06-05 21:02:06.187867 pynecone-0.1.33a0/pynecone/components/overlay/__init__.py
+-rw-r--r--   0        0        0     5027 2023-05-18 00:14:14.763711 pynecone-0.1.33a0/pynecone/components/overlay/alertdialog.py
+-rw-r--r--   0        0        0     1016 2023-06-05 21:02:06.187998 pynecone-0.1.33a0/pynecone/components/overlay/banner.py
+-rw-r--r--   0        0        0     4681 2023-05-18 00:14:14.763867 pynecone-0.1.33a0/pynecone/components/overlay/drawer.py
+-rw-r--r--   0        0        0     5530 2023-05-18 00:14:14.764021 pynecone-0.1.33a0/pynecone/components/overlay/menu.py
+-rw-r--r--   0        0        0     4917 2023-05-18 00:14:14.764177 pynecone-0.1.33a0/pynecone/components/overlay/modal.py
+-rw-r--r--   0        0        0     5688 2023-05-18 00:14:14.764341 pynecone-0.1.33a0/pynecone/components/overlay/popover.py
+-rw-r--r--   0        0        0     1949 2023-05-18 00:14:14.764530 pynecone-0.1.33a0/pynecone/components/overlay/tooltip.py
+-rw-r--r--   0        0        0      120 2022-11-18 20:43:33.725191 pynecone-0.1.33a0/pynecone/components/tags/__init__.py
+-rw-r--r--   0        0        0      451 2023-05-15 02:04:07.617454 pynecone-0.1.33a0/pynecone/components/tags/cond_tag.py
+-rw-r--r--   0        0        0     2306 2023-05-15 02:04:07.617560 pynecone-0.1.33a0/pynecone/components/tags/iter_tag.py
+-rw-r--r--   0        0        0     5018 2023-05-18 00:14:14.764773 pynecone-0.1.33a0/pynecone/components/tags/tag.py
+-rw-r--r--   0        0        0      591 2023-03-16 23:52:12.746470 pynecone-0.1.33a0/pynecone/components/tags/tagless.py
+-rw-r--r--   0        0        0      304 2023-06-01 00:32:59.073257 pynecone-0.1.33a0/pynecone/components/typography/__init__.py
+-rw-r--r--   0        0        0      282 2023-05-15 02:04:07.617958 pynecone-0.1.33a0/pynecone/components/typography/heading.py
+-rw-r--r--   0        0        0      682 2023-06-01 00:32:59.073664 pynecone-0.1.33a0/pynecone/components/typography/highlight.py
+-rw-r--r--   0        0        0     3460 2023-06-03 03:13:18.321195 pynecone-0.1.33a0/pynecone/components/typography/markdown.py
+-rw-r--r--   0        0        0      337 2023-05-15 02:04:07.618372 pynecone-0.1.33a0/pynecone/components/typography/span.py
+-rw-r--r--   0        0        0      306 2023-05-15 02:04:07.618520 pynecone-0.1.33a0/pynecone/components/typography/text.py
+-rw-r--r--   0        0        0     6858 2023-06-05 03:00:53.231552 pynecone-0.1.33a0/pynecone/config.py
+-rw-r--r--   0        0        0    10169 2023-06-05 03:00:53.231706 pynecone-0.1.33a0/pynecone/constants.py
+-rw-r--r--   0        0        0       73 2023-04-27 02:06:35.757531 pynecone-0.1.33a0/pynecone/el/__init__.py
+-rw-r--r--   0        0        0      115 2023-04-27 02:06:35.757829 pynecone-0.1.33a0/pynecone/el/constants/__init__.py
+-rw-r--r--   0        0        0     7175 2023-04-27 02:06:35.758045 pynecone-0.1.33a0/pynecone/el/constants/html.py
+-rw-r--r--   0        0        0     1719 2023-04-27 02:06:35.758325 pynecone-0.1.33a0/pynecone/el/constants/pynecone.py
+-rw-r--r--   0        0        0    15554 2023-04-27 02:06:35.758673 pynecone-0.1.33a0/pynecone/el/constants/react.py
+-rw-r--r--   0        0        0     1283 2023-05-15 02:04:07.619213 pynecone-0.1.33a0/pynecone/el/element.py
+-rw-r--r--   0        0        0   108518 2023-05-15 02:04:07.619552 pynecone-0.1.33a0/pynecone/el/elements/__init__.py
+-rwxr-xr-x   0        0        0     2667 2023-05-15 02:04:07.619858 pynecone-0.1.33a0/pynecone/el/precompile.py
+-rw-r--r--   0        0        0    10977 2023-06-03 03:13:18.321601 pynecone-0.1.33a0/pynecone/event.py
+-rw-r--r--   0        0        0      113 2023-05-15 02:04:07.620772 pynecone-0.1.33a0/pynecone/middleware/__init__.py
+-rw-r--r--   0        0        0     1738 2023-05-15 02:04:07.621034 pynecone-0.1.33a0/pynecone/middleware/hydrate_middleware.py
+-rw-r--r--   0        0        0     1167 2023-05-15 02:04:07.621188 pynecone-0.1.33a0/pynecone/middleware/middleware.py
+-rw-r--r--   0        0        0     2085 2023-06-01 03:12:11.086155 pynecone-0.1.33a0/pynecone/model.py
+-rw-r--r--   0        0        0     8431 2023-06-01 03:12:42.958684 pynecone-0.1.33a0/pynecone/pc.py
+-rw-r--r--   0        0        0        0 2023-03-10 00:25:42.707141 pynecone-0.1.33a0/pynecone/py.typed
+-rw-r--r--   0        0        0     4108 2023-03-16 23:52:12.748303 pynecone-0.1.33a0/pynecone/route.py
+-rw-r--r--   0        0        0    30953 2023-06-05 18:43:43.583090 pynecone-0.1.33a0/pynecone/state.py
+-rw-r--r--   0        0        0     1060 2023-05-15 02:04:07.621889 pynecone-0.1.33a0/pynecone/style.py
+-rw-r--r--   0        0        0       26 2023-05-15 02:04:07.622076 pynecone-0.1.33a0/pynecone/utils/__init__.py
+-rw-r--r--   0        0        0     7451 2023-06-01 03:12:42.959046 pynecone-0.1.33a0/pynecone/utils/build.py
+-rw-r--r--   0        0        0     1759 2023-05-15 02:04:07.622587 pynecone-0.1.33a0/pynecone/utils/console.py
+-rw-r--r--   0        0        0     5229 2023-06-01 03:12:42.959181 pynecone-0.1.33a0/pynecone/utils/exec.py
+-rw-r--r--   0        0        0    11859 2023-06-01 03:15:26.565621 pynecone-0.1.33a0/pynecone/utils/format.py
+-rw-r--r--   0        0        0      587 2023-05-15 02:04:07.623144 pynecone-0.1.33a0/pynecone/utils/imports.py
+-rw-r--r--   0        0        0     2451 2023-03-16 23:52:12.757162 pynecone-0.1.33a0/pynecone/utils/path_ops.py
+-rw-r--r--   0        0        0    10033 2023-05-17 03:31:04.698132 pynecone-0.1.33a0/pynecone/utils/prerequisites.py
+-rw-r--r--   0        0        0     3021 2023-03-16 23:52:12.757337 pynecone-0.1.33a0/pynecone/utils/processes.py
+-rw-r--r--   0        0        0     2397 2023-05-15 02:04:07.623496 pynecone-0.1.33a0/pynecone/utils/telemetry.py
+-rw-r--r--   0        0        0     4806 2023-06-01 03:15:26.565774 pynecone-0.1.33a0/pynecone/utils/types.py
+-rw-r--r--   0        0        0     2634 2023-05-15 02:04:07.623722 pynecone-0.1.33a0/pynecone/utils/watch.py
+-rw-r--r--   0        0        0    30928 2023-05-18 00:14:14.766310 pynecone-0.1.33a0/pynecone/vars.py
+-rw-r--r--   0        0        0     1825 2023-06-05 21:02:13.244762 pynecone-0.1.33a0/pyproject.toml
+-rw-r--r--   0        0        0     9462 1970-01-01 00:00:00.000000 pynecone-0.1.33a0/PKG-INFO
```

### Comparing `pynecone-0.1.32a1/LICENSE` & `pynecone-0.1.33a0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/README.md` & `pynecone-0.1.33a0/README.md`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/.templates/apps/counter/counter.py` & `pynecone-0.1.33a0/pynecone/.templates/apps/counter/counter.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/.templates/apps/default/default.py` & `pynecone-0.1.33a0/pynecone/.templates/apps/default/default.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/.templates/assets/favicon.ico` & `pynecone-0.1.33a0/pynecone/.templates/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/.templates/jinja/web/pages/index.js.jinja2` & `pynecone-0.1.33a0/pynecone/.templates/jinja/web/pages/index.js.jinja2`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 {% endblock %}
 
 {% block export %}
 export default function Component() {
   const [{{state_name}}, {{state_name|react_setter}}] = useState({{initial_state|json_dumps}})
   const [{{const.result}}, {{const.result|react_setter}}] = useState({{const.initial_result|json_dumps}})
+  const [notConnected, setNotConnected] = useState(false)
   const {{const.router}} = useRouter()
   const {{const.socket}} = useRef(null)
   const { isReady } = {{const.router}}
   const { {{const.color_mode}}, {{const.toggle_color_mode}} } = {{const.use_color_mode}}()
   const focusRef = useRef();
   
   const Event = (events, _e) => {
@@ -31,27 +32,27 @@
   })
 
   useEffect(()=>{
     if(!isReady) {
       return;
     }
     if (!{{const.socket}}.current) {
-      connect({{const.socket}}, {{state_name}}, {{state_name|react_setter}}, {{const.result}}, {{const.result|react_setter}}, {{const.router}}, {{transports}})
+      connect({{const.socket}}, {{state_name}}, {{state_name|react_setter}}, {{const.result}}, {{const.result|react_setter}}, {{const.router}}, {{transports}}, setNotConnected)
     }
     const update = async () => {
       if ({{const.result}}.{{const.state}} != null){
         {{state_name|react_setter}}({
           ...{{const.result}}.{{const.state}},
           events: [...{{state_name}}.{{const.events}}, ...{{const.result}}.{{const.events}}],
         })
 
         {{const.result|react_setter}}({
           {{const.state}}: null,
           {{const.events}}: [],
-          {{const.processing}}: false,
+          {{const.processing}}: {{const.result}}.{{const.processing}},
         })
       }
 
       await updateState({{state_name}}, {{state_name|react_setter}}, {{const.result}}, {{const.result|react_setter}}, {{const.router}}, {{const.socket}}.current)
     }
     if (focusRef.current)
       focusRef.current.focus();
@@ -66,11 +67,16 @@
   }, [{{const.router}}])
 
   {% for hook in hooks %}
   {{ hook }}
   {% endfor %}
 
   return (
+  <Fragment>
+      {%- if err_comp -%}
+            {{ utils.render(err_comp, indent_width=1) }}
+       {%- endif -%}
     {{utils.render(render, indent_width=0)}}
+    </Fragment>
   )
 }
 {% endblock %}
```

### Comparing `pynecone-0.1.32a1/pynecone/.templates/jinja/web/pages/utils.js.jinja2` & `pynecone-0.1.33a0/pynecone/.templates/jinja/web/pages/utils.js.jinja2`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/.templates/web/bun.lockb` & `pynecone-0.1.33a0/pynecone/.templates/web/bun.lockb`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/.templates/web/package.json` & `pynecone-0.1.33a0/pynecone/.templates/web/package.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9938271604938271%*

 * *Differences: {"'dependencies'": "{'react-player': '^2.12.0'}"}*

```diff
@@ -14,14 +14,15 @@
         "json5": "^2.2.3",
         "next": "^13.3.1",
         "plotly.js": "^2.22.0",
         "react": "^18.2.0",
         "react-dom": "^18.2.0",
         "react-dropzone": "^14.2.3",
         "react-markdown": "^8.0.7",
+        "react-player": "^2.12.0",
         "react-plotly.js": "^2.6.0",
         "react-syntax-highlighter": "^15.5.0",
         "rehype-katex": "^6.0.3",
         "rehype-raw": "^6.1.1",
         "remark-gfm": "^3.0.1",
         "remark-math": "^5.1.1",
         "socket.io-client": "^4.6.1",
```

### Comparing `pynecone-0.1.32a1/pynecone/.templates/web/pages/_app.js` & `pynecone-0.1.33a0/pynecone/.templates/web/pages/_app.js`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/.templates/web/styles/code/prism.js` & `pynecone-0.1.33a0/pynecone/.templates/web/styles/code/prism.js`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/.templates/web/utils/state.js` & `pynecone-0.1.33a0/pynecone/.templates/web/utils/state.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -93,14 +93,21 @@
     }
 
     if (event.name == "_alert") {
         alert(event.payload.message);
         return false;
     }
 
+    if (event.name == "_set_focus") {
+        const ref =
+            event.payload.ref in refs ? refs[event.payload.ref] : event.payload.ref;
+        ref.current.focus();
+        return false;
+    }
+
     if (event.name == "_set_value") {
         const ref =
             event.payload.ref in refs ? refs[event.payload.ref] : event.payload.ref;
         ref.current.value = event.payload.value;
         return false;
     }
 
@@ -197,36 +204,42 @@
 export const connect = async (
     socket,
     state,
     setState,
     result,
     setResult,
     router,
-    transports
+    transports,
+    setNotConnected
 ) => {
     // Get backend URL object from the endpoint
     const endpoint_url = new URL(EVENTURL);
     // Create the socket.
     socket.current = io(EVENTURL, {
         path: endpoint_url["pathname"],
         transports: transports,
         autoUnref: false,
     });
 
     // Once the socket is open, hydrate the page.
     socket.current.on("connect", () => {
         updateState(state, setState, result, setResult, router, socket.current);
+        setNotConnected(false)
+    });
+
+    socket.current.on('connect_error', (error) => {
+        setNotConnected(true)
     });
 
     // On each received message, apply the delta and set the result.
     socket.current.on("event", function(update) {
         update = JSON5.parse(update);
         applyDelta(state, update.delta);
         setResult({
-            processing: true,
+            processing: update.processing,
             state: state,
             events: update.events,
         });
     });
 };
 
 /**
@@ -296,19 +309,19 @@
  * @returns True if the value is truthy, false otherwise.
  */
 export const isTrue = (val) => {
     return Array.isArray(val) ? val.length > 0 : !!val;
 };
 
 /**
- * Prevent the default event.
+ * Prevent the default event for form submission.
  * @param event
  */
 export const preventDefault = (event) => {
-    if (event && event.preventDefault) {
+    if (event && event.type == "submit") {
         event.preventDefault();
     }
 };
 
 /**
  * Get the value from a ref.
  * @param ref The ref to get the value from.
```

### Comparing `pynecone-0.1.32a1/pynecone/__init__.py` & `pynecone-0.1.33a0/pynecone/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from .constants import Env as Env
 from .constants import Transports as Transports
 from .event import EVENT_ARG as EVENT_ARG
 from .event import EventChain as EventChain
 from .event import FileUpload as upload_files
 from .event import console_log as console_log
 from .event import redirect as redirect
+from .event import set_focus as set_focus
 from .event import set_value as set_value
 from .event import window_alert as window_alert
 from .middleware import Middleware as Middleware
 from .model import Model as Model
 from .model import session as session
 from .route import route as route
 from .state import ComputedVar as var
```

### Comparing `pynecone-0.1.32a1/pynecone/app.py` & `pynecone-0.1.33a0/pynecone/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,34 @@
 """The main Pynecone app."""
 
 import asyncio
 import inspect
-from typing import Any, Callable, Coroutine, Dict, List, Optional, Tuple, Type, Union
+from typing import (
+    Any,
+    AsyncIterator,
+    Callable,
+    Coroutine,
+    Dict,
+    List,
+    Optional,
+    Tuple,
+    Type,
+    Union,
+)
 
 from fastapi import FastAPI, UploadFile
 from fastapi.middleware import cors
 from socketio import ASGIApp, AsyncNamespace, AsyncServer
 
 from pynecone import constants
 from pynecone.base import Base
 from pynecone.compiler import compiler
 from pynecone.compiler import utils as compiler_utils
 from pynecone.components.component import Component, ComponentStyle
+from pynecone.components.overlay.banner import ConnectionBanner
 from pynecone.config import get_config
 from pynecone.event import Event, EventHandler
 from pynecone.middleware import HydrateMiddleware, Middleware
 from pynecone.model import Model
 from pynecone.route import (
     DECORATED_ROUTES,
     catchall_in_route,
@@ -61,14 +73,17 @@
 
     # Middleware to add to the app.
     middleware: List[Middleware] = []
 
     # List of event handlers to trigger when a page loads.
     load_events: Dict[str, List[EventHandler]] = {}
 
+    # The component to render if there is a connection error to the server.
+    connect_error_component: Optional[Component] = ConnectionBanner.create()
+
     def __init__(self, *args, **kwargs):
         """Initialize the app.
 
         Args:
             *args: Args to initialize the app with.
             **kwargs: Kwargs to initialize the app with.
         """
@@ -84,23 +99,20 @@
         self.state_manager.setup(state=self.state)
 
         # Set up the API.
         self.api = FastAPI()
         self.add_cors()
         self.add_default_endpoints()
 
-        # Set up CORS options.
-        cors_allowed_origins = config.cors_allowed_origins
-        if config.cors_allowed_origins == [constants.CORS_ALLOWED_ORIGINS]:
-            cors_allowed_origins = "*"
-
         # Set up the Socket.IO AsyncServer.
         self.sio = AsyncServer(
             async_mode="asgi",
-            cors_allowed_origins=cors_allowed_origins,
+            cors_allowed_origins="*"
+            if config.cors_allowed_origins == constants.CORS_ALLOWED_ORIGINS
+            else config.cors_allowed_origins,
             cors_credentials=config.cors_credentials,
             max_http_buffer_size=config.polling_max_http_buffer_size,
             ping_interval=constants.PING_INTERVAL,
             ping_timeout=constants.PING_TIMEOUT,
         )
 
         # Create the socket app. Note event endpoint constant replaces the default 'socket.io' path.
@@ -399,36 +411,41 @@
         # Compile the theme.
         compiler.compile_theme(self.style)
 
         # Compile the pages.
         custom_components = set()
         for route, component in self.pages.items():
             component.add_style(self.style)
-            compiler.compile_page(route, component, self.state)
+            compiler.compile_page(
+                route,
+                component,
+                self.state,
+                self.connect_error_component,
+            )
 
             # Add the custom components from the page to the set.
             custom_components |= component.get_custom_components()
 
         # Compile the custom components.
         compiler.compile_components(custom_components)
 
 
 async def process(
     app: App, event: Event, sid: str, headers: Dict, client_ip: str
-) -> StateUpdate:
+) -> AsyncIterator[StateUpdate]:
     """Process an event.
 
     Args:
         app: The app to process the event for.
         event: The event to process.
         sid: The Socket.IO session id.
         headers: The client headers.
         client_ip: The client_ip.
 
-    Returns:
+    Yields:
         The state updates after processing the event.
     """
     # Get the state for the session.
     state = app.state_manager.get_state(event.token)
 
     # Add request data to the state.
     router_data = event.router_data
@@ -446,28 +463,31 @@
         # assignment will recurse into substates and force recalculation of
         # dependent ComputedVar (dynamic route variables)
         state.router_data = router_data
 
     # Preprocess the event.
     update = await app.preprocess(state, event)
 
+    # If there was an update, yield it.
+    if update is not None:
+        yield update
+
     # Only process the event if there is no update.
-    if update is None:
-        # Apply the event to the state.
-        update = await state._process(event)
+    else:
+        # Process the event.
+        async for update in state._process(event):
+            # Postprocess the event.
+            update = await app.postprocess(state, event, update)
 
-        # Postprocess the event.
-        update = await app.postprocess(state, event, update)
+            # Yield the update.
+            yield update
 
-    # Update the state.
+    # Set the state for the session.
     app.state_manager.set_state(event.token, state)
 
-    # Return the update.
-    return update
-
 
 async def ping() -> str:
     """Test API endpoint.
 
     Returns:
         The response.
     """
@@ -530,15 +550,16 @@
             )
 
         event = Event(
             token=token,
             name=handler,
             payload={handler_upload_param[0]: files},
         )
-        update = await state._process(event)
+        # TODO: refactor this to handle yields.
+        update = await state._process(event).__anext__()
         return update
 
     return upload_file
 
 
 class EventNamespace(AsyncNamespace):
     """The event namespace."""
@@ -594,18 +615,17 @@
             for (k, v) in environ["asgi.scope"]["headers"]
         }
 
         # Get the client IP
         client_ip = environ["REMOTE_ADDR"]
 
         # Process the events.
-        update = await process(self.app, event, sid, headers, client_ip)
-
-        # Emit the event.
-        await self.emit(str(constants.SocketEvent.EVENT), update.json(), to=sid)  # type: ignore
+        async for update in process(self.app, event, sid, headers, client_ip):
+            # Emit the event.
+            await self.emit(str(constants.SocketEvent.EVENT), update.json(), to=sid)  # type: ignore
 
     async def on_ping(self, sid):
         """Event for testing the API endpoint.
 
         Args:
             sid: The Socket.IO session id.
         """
```

### Comparing `pynecone-0.1.32a1/pynecone/base.py` & `pynecone-0.1.33a0/pynecone/base.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/compiler/compiler.py` & `pynecone-0.1.33a0/pynecone/compiler/compiler.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from pynecone.style import Style
 from pynecone.utils import imports
 from pynecone.vars import ImportVar
 
 # Imports to be included in every Pynecone app.
 DEFAULT_IMPORTS: imports.ImportDict = {
     "react": {
+        ImportVar(tag="Fragment"),
         ImportVar(tag="useEffect"),
         ImportVar(tag="useRef"),
         ImportVar(tag="useState"),
     },
     "next/router": {ImportVar(tag="useRouter")},
     f"/{constants.STATE_PATH}": {
         ImportVar(tag="connect"),
@@ -27,15 +28,19 @@
         ImportVar(tag="E"),
         ImportVar(tag="isTrue"),
         ImportVar(tag="preventDefault"),
         ImportVar(tag="refs"),
         ImportVar(tag="getRefValue"),
     },
     "": {ImportVar(tag="focus-visible/dist/focus-visible")},
-    "@chakra-ui/react": {ImportVar(tag=constants.USE_COLOR_MODE)},
+    "@chakra-ui/react": {
+        ImportVar(tag=constants.USE_COLOR_MODE),
+        ImportVar(tag="Box"),
+        ImportVar(tag="Text"),
+    },
 }
 
 
 def _compile_document_root(root: Component) -> str:
     """Compile the document root.
 
     Args:
@@ -58,20 +63,23 @@
 
     Returns:
         The compiled theme.
     """
     return templates.THEME.render(theme=theme)
 
 
-def _compile_page(component: Component, state: Type[State]) -> str:
+def _compile_page(
+    component: Component, state: Type[State], connect_error_component
+) -> str:
     """Compile the component given the app state.
 
     Args:
         component: The component to compile.
         state: The app state.
+        connect_error_component: The component to render on sever connection error.
 
     Returns:
         The compiled component.
     """
     # Merge the default imports with the app-specific imports.
     imports = utils.merge_imports(DEFAULT_IMPORTS, component.get_imports())
     imports = utils.compile_imports(imports)
@@ -81,14 +89,15 @@
         imports=imports,
         custom_codes=component.get_custom_code(),
         initial_state=utils.compile_state(state),
         state_name=state.get_name(),
         hooks=component.get_hooks(),
         render=component.render(),
         transports=constants.Transports.POLLING_WEBSOCKET.get_transports(),
+        err_comp=connect_error_component.render() if connect_error_component else None,
     )
 
 
 def _compile_components(components: Set[CustomComponent]) -> str:
     """Compile the components.
 
     Args:
@@ -184,31 +193,35 @@
     # Compile the theme.
     code = _compile_theme(theme)
     return output_path, code
 
 
 @write_output
 def compile_page(
-    path: str, component: Component, state: Type[State]
+    path: str,
+    component: Component,
+    state: Type[State],
+    connect_error_component: Component,
 ) -> Tuple[str, str]:
     """Compile a single page.
 
     Args:
         path: The path to compile the page to.
         component: The component to compile.
         state: The app state.
+        connect_error_component: The component to render on sever connection error.
 
     Returns:
         The path and code of the compiled page.
     """
     # Get the path for the output file.
     output_path = utils.get_page_path(path)
 
     # Add the style to the component.
-    code = _compile_page(component, state)
+    code = _compile_page(component, state, connect_error_component)
     return output_path, code
 
 
 @write_output
 def compile_components(components: Set[CustomComponent]):
     """Compile the custom components.
```

### Comparing `pynecone-0.1.32a1/pynecone/compiler/templates.py` & `pynecone-0.1.33a0/pynecone/compiler/templates.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/compiler/utils.py` & `pynecone-0.1.33a0/pynecone/compiler/utils.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/__init__.py` & `pynecone-0.1.33a0/pynecone/components/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
 # Add the convenience methods for all the components manually.
 # This is necessary for static type checking to work.
 component = Component.create
 badge = Badge.create
 code = Code.create
 code_block = CodeBlock.create
+connection_banner = ConnectionBanner.create
 data_table = DataTable.create
 divider = Divider.create
 list = List.create
 list_item = ListItem.create
 ordered_list = OrderedList.create
 unordered_list = UnorderedList.create
 stat = Stat.create
@@ -87,35 +88,40 @@
 skeleton_text = SkeletonText.create
 spinner = Spinner.create
 button = Button.create
 button_group = ButtonGroup.create
 checkbox = Checkbox.create
 checkbox_group = CheckboxGroup.create
 copy_to_clipboard = CopyToClipboard.create
+date_picker = DatePicker.create
+date_time_picker = DateTimePicker.create
 editable = Editable.create
 editable_input = EditableInput.create
 editable_preview = EditablePreview.create
 editable_textarea = EditableTextarea.create
 form = Form.create
 form_control = FormControl.create
 form_error_message = FormErrorMessage.create
 form_helper_text = FormHelperText.create
 form_label = FormLabel.create
 icon_button = IconButton.create
 input = Input.create
 input_group = InputGroup.create
 input_left_addon = InputLeftAddon.create
 input_right_addon = InputRightAddon.create
+multi_select = MultiSelect
+multi_select_option = MultiSelectOption
 number_decrement_stepper = NumberDecrementStepper.create
 number_increment_stepper = NumberIncrementStepper.create
 number_input = NumberInput.create
 number_input_field = NumberInputField.create
 number_input_stepper = NumberInputStepper.create
-option = Option
+option = Option.create
 password = Password.create
+email = Email.create
 pin_input = PinInput.create
 pin_input_field = PinInputField.create
 radio = Radio.create
 radio_group = RadioGroup.create
 range_slider = RangeSlider.create
 range_slider_filled_track = RangeSliderFilledTrack.create
 range_slider_thumb = RangeSliderThumb.create
@@ -163,14 +169,16 @@
 wrap = Wrap.create
 wrap_item = WrapItem.create
 avatar = Avatar.create
 avatar_badge = AvatarBadge.create
 avatar_group = AvatarGroup.create
 icon = Icon.create
 image = Image.create
+video = Video.create
+audio = Audio.create
 breadcrumb = Breadcrumb.create
 breadcrumb_item = BreadcrumbItem.create
 breadcrumb_link = BreadcrumbLink.create
 breadcrumb_separator = BreadcrumbSeparator.create
 link = Link.create
 link_box = LinkBox.create
 link_overlay = LinkOverlay.create
```

### Comparing `pynecone-0.1.32a1/pynecone/components/base/bare.py` & `pynecone-0.1.33a0/pynecone/components/base/bare.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/base/document.py` & `pynecone-0.1.33a0/pynecone/components/base/document.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/base/link.py` & `pynecone-0.1.33a0/pynecone/components/base/link.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/base/meta.py` & `pynecone-0.1.33a0/pynecone/components/base/meta.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/component.py` & `pynecone-0.1.33a0/pynecone/components/component.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/datadisplay/code.py` & `pynecone-0.1.33a0/pynecone/components/datadisplay/code.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/datadisplay/datatable.py` & `pynecone-0.1.33a0/pynecone/components/datadisplay/datatable.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/datadisplay/divider.py` & `pynecone-0.1.33a0/pynecone/components/datadisplay/divider.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/datadisplay/list.py` & `pynecone-0.1.33a0/pynecone/components/datadisplay/list.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/datadisplay/stat.py` & `pynecone-0.1.33a0/pynecone/components/datadisplay/stat.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/datadisplay/table.py` & `pynecone-0.1.33a0/pynecone/components/datadisplay/table.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/datadisplay/tag.py` & `pynecone-0.1.33a0/pynecone/components/datadisplay/tag.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/disclosure/accordion.py` & `pynecone-0.1.33a0/pynecone/components/disclosure/accordion.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/disclosure/tabs.py` & `pynecone-0.1.33a0/pynecone/components/disclosure/tabs.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/disclosure/transition.py` & `pynecone-0.1.33a0/pynecone/components/disclosure/transition.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/feedback/alert.py` & `pynecone-0.1.33a0/pynecone/components/feedback/alert.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/feedback/circularprogress.py` & `pynecone-0.1.33a0/pynecone/components/feedback/circularprogress.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/feedback/progress.py` & `pynecone-0.1.33a0/pynecone/components/feedback/progress.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/feedback/skeleton.py` & `pynecone-0.1.33a0/pynecone/components/feedback/skeleton.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/feedback/spinner.py` & `pynecone-0.1.33a0/pynecone/components/feedback/spinner.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/forms/button.py` & `pynecone-0.1.33a0/pynecone/components/forms/button.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/forms/checkbox.py` & `pynecone-0.1.33a0/pynecone/components/forms/checkbox.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/forms/copytoclipboard.py` & `pynecone-0.1.33a0/pynecone/components/forms/copytoclipboard.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/forms/editable.py` & `pynecone-0.1.33a0/pynecone/components/forms/editable.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/forms/form.py` & `pynecone-0.1.33a0/pynecone/components/forms/form.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/forms/iconbutton.py` & `pynecone-0.1.33a0/pynecone/components/forms/iconbutton.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/forms/input.py` & `pynecone-0.1.33a0/pynecone/components/forms/input.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/forms/numberinput.py` & `pynecone-0.1.33a0/pynecone/components/forms/numberinput.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/forms/pininput.py` & `pynecone-0.1.33a0/pynecone/components/forms/pininput.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/forms/radio.py` & `pynecone-0.1.33a0/pynecone/components/forms/radio.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/forms/rangeslider.py` & `pynecone-0.1.33a0/pynecone/components/forms/rangeslider.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/forms/select.py` & `pynecone-0.1.33a0/pynecone/components/forms/multiselect.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/forms/slider.py` & `pynecone-0.1.33a0/pynecone/components/forms/slider.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/forms/switch.py` & `pynecone-0.1.33a0/pynecone/components/forms/switch.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/forms/textarea.py` & `pynecone-0.1.33a0/pynecone/components/forms/textarea.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/forms/upload.py` & `pynecone-0.1.33a0/pynecone/components/forms/upload.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/graphing/plotly.py` & `pynecone-0.1.33a0/pynecone/components/graphing/plotly.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/graphing/victory.py` & `pynecone-0.1.33a0/pynecone/components/graphing/victory.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/layout/__init__.py` & `pynecone-0.1.33a0/pynecone/components/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/layout/box.py` & `pynecone-0.1.33a0/pynecone/components/layout/box.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/layout/card.py` & `pynecone-0.1.33a0/pynecone/components/layout/card.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/layout/cond.py` & `pynecone-0.1.33a0/pynecone/components/layout/cond.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/layout/flex.py` & `pynecone-0.1.33a0/pynecone/components/layout/flex.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/layout/foreach.py` & `pynecone-0.1.33a0/pynecone/components/layout/foreach.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/layout/grid.py` & `pynecone-0.1.33a0/pynecone/components/layout/grid.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/layout/html.py` & `pynecone-0.1.33a0/pynecone/components/layout/html.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/layout/responsive.py` & `pynecone-0.1.33a0/pynecone/components/layout/responsive.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/layout/stack.py` & `pynecone-0.1.33a0/pynecone/components/layout/stack.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/layout/wrap.py` & `pynecone-0.1.33a0/pynecone/components/layout/wrap.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/media/avatar.py` & `pynecone-0.1.33a0/pynecone/components/media/avatar.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/media/icon.py` & `pynecone-0.1.33a0/pynecone/components/media/icon.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/media/image.py` & `pynecone-0.1.33a0/pynecone/components/media/image.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """An image component."""
 from __future__ import annotations
 
-from typing import Optional, Set
+from typing import Any, Optional, Set
 
 from pynecone.components.component import Component
 from pynecone.components.libs.chakra import ChakraComponent
+from pynecone.components.tags import Tag
+from pynecone.utils import format, types
 from pynecone.vars import Var
 
 
 class Image(ChakraComponent):
     """Display an image."""
 
     tag = "Image"
@@ -34,19 +36,27 @@
     # If true, opt out of the fallbackSrc logic and use as img.
     ignore_fallback: Var[bool]
 
     # "eager" | "lazy"
     loading: Var[str]
 
     # The image src attribute.
-    src: Var[str]
+    src: Var[Any]
 
     # The image srcset attribute.
     src_set: Var[str]
 
     def get_triggers(self) -> Set[str]:
         """Get the event triggers for the component.
 
         Returns:
             The event triggers.
         """
         return super().get_triggers() | {"on_error", "on_load"}
+
+    def _render(self) -> Tag:
+        # If the src is an image, convert it to a base64 string.
+        if types.is_image(type(self.src)):
+            self.src = Var.create(format.format_image_data(self.src))  # type: ignore
+
+        # Render the table.
+        return super()._render()
```

### Comparing `pynecone-0.1.32a1/pynecone/components/navigation/breadcrumb.py` & `pynecone-0.1.33a0/pynecone/components/navigation/breadcrumb.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/navigation/link.py` & `pynecone-0.1.33a0/pynecone/components/navigation/link.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/navigation/linkoverlay.py` & `pynecone-0.1.33a0/pynecone/components/navigation/linkoverlay.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/overlay/__init__.py` & `pynecone-0.1.33a0/pynecone/components/overlay/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     AlertDialog,
     AlertDialogBody,
     AlertDialogContent,
     AlertDialogFooter,
     AlertDialogHeader,
     AlertDialogOverlay,
 )
+from .banner import ConnectionBanner
 from .drawer import (
     Drawer,
     DrawerBody,
     DrawerCloseButton,
     DrawerContent,
     DrawerFooter,
     DrawerHeader,
```

### Comparing `pynecone-0.1.32a1/pynecone/components/overlay/alertdialog.py` & `pynecone-0.1.33a0/pynecone/components/overlay/alertdialog.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/overlay/drawer.py` & `pynecone-0.1.33a0/pynecone/components/overlay/drawer.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/overlay/menu.py` & `pynecone-0.1.33a0/pynecone/components/overlay/menu.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/overlay/modal.py` & `pynecone-0.1.33a0/pynecone/components/overlay/modal.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/overlay/popover.py` & `pynecone-0.1.33a0/pynecone/components/overlay/popover.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/overlay/tooltip.py` & `pynecone-0.1.33a0/pynecone/components/overlay/tooltip.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/tags/iter_tag.py` & `pynecone-0.1.33a0/pynecone/components/tags/iter_tag.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/tags/tag.py` & `pynecone-0.1.33a0/pynecone/components/tags/tag.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/tags/tagless.py` & `pynecone-0.1.33a0/pynecone/components/tags/tagless.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/typography/highlight.py` & `pynecone-0.1.33a0/pynecone/components/typography/highlight.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/components/typography/markdown.py` & `pynecone-0.1.33a0/pynecone/components/typography/markdown.py`

 * *Files 8% similar despite different names*

```diff
@@ -62,14 +62,16 @@
             super()
             ._render()
             .add_props(
                 components={
                     "h1": "{({node, ...props}) => <Heading size='2xl' {...props} />}",
                     "h2": "{({node, ...props}) => <Heading size='xl' {...props} />}",
                     "h3": "{({node, ...props}) => <Heading size='lg' {...props} />}",
+                    "h4": "{({node, ...props}) => <Heading size='sm' {...props} />}",
+                    "h5": "{({node, ...props}) => <Heading size='xs' {...props} />}",
                     "ul": "{UnorderedList}",
                     "ol": "{OrderedList}",
                     "li": "{ListItem}",
                     "p": "{Text}",
                     "a": "{Link}",
                     "code": """{({node, inline, className, children, ...props}) =>
                     {
```

### Comparing `pynecone-0.1.32a1/pynecone/config.py` & `pynecone-0.1.33a0/pynecone/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """The Pynecone config."""
 
 from __future__ import annotations
 
+import importlib
 import os
 import sys
 import urllib.parse
 from typing import List, Optional
 
+from dotenv import load_dotenv
+
 from pynecone import constants
 from pynecone.base import Base
 
 
 class DBConfig(Base):
     """Database config."""
 
@@ -125,36 +128,36 @@
     # The name of the app.
     app_name: str
 
     # The username.
     username: Optional[str] = None
 
     # The frontend port.
-    port: str = constants.FRONTEND_PORT
+    frontend_port: str = constants.FRONTEND_PORT
 
-    # The frontend port.
+    # The backend port.
     backend_port: str = constants.BACKEND_PORT
 
     # The backend host.
     backend_host: str = constants.BACKEND_HOST
 
     # The backend API url.
     api_url: str = constants.API_URL
 
     # The deploy url.
-    deploy_url: Optional[str] = None
+    deploy_url: Optional[str] = constants.DEPLOY_URL
 
     # The database url.
     db_url: Optional[str] = constants.DB_URL
 
     # The database config.
     db_config: Optional[DBConfig] = None
 
     # The redis url.
-    redis_url: Optional[str] = None
+    redis_url: Optional[str] = constants.REDIS_URL
 
     # Telemetry opt-in.
     telemetry_enabled: bool = True
 
     # The pcdeploy url.
     pcdeploy_url: Optional[str] = None
 
@@ -172,43 +175,81 @@
 
     # Backend transport methods.
     backend_transports: Optional[
         constants.Transports
     ] = constants.Transports.WEBSOCKET_POLLING
 
     # List of origins that are allowed to connect to the backend API.
-    cors_allowed_origins: Optional[list] = [constants.CORS_ALLOWED_ORIGINS]
+    cors_allowed_origins: Optional[list] = constants.CORS_ALLOWED_ORIGINS
 
     # Whether credentials (cookies, authentication) are allowed in requests to the backend API.
     cors_credentials: Optional[bool] = True
 
     # The maximum size of a message when using the polling backend transport.
     polling_max_http_buffer_size: Optional[int] = constants.POLLING_MAX_HTTP_BUFFER_SIZE
 
+    # Dotenv file path
+    env_path: Optional[str] = constants.DOT_ENV_FILE
+
+    # Whether to override OS environment variables
+    override_os_envs: Optional[bool] = True
+
     def __init__(self, *args, **kwargs):
         """Initialize the config values.
 
         If db_url is not provided gets it from db_config.
 
         Args:
             *args: The args to pass to the Pydantic init method.
             **kwargs: The kwargs to pass to the Pydantic init method.
         """
         if "db_url" not in kwargs and "db_config" in kwargs:
             kwargs["db_url"] = kwargs["db_config"].get_url()
 
         super().__init__(*args, **kwargs)
 
+        # set overriden class attribute values as os env variables to avoid losing them
+        for key, value in dict(self).items():
+            key = key.upper()
+            if (
+                key.startswith("_")
+                or key in os.environ
+                or (value is None and key != "DB_URL")
+            ):
+                continue
+            os.environ[key] = str(value)
+
+        # Avoid overriding if env_path is not provided or does not exist
+        if self.env_path is not None and os.path.isfile(self.env_path):
+            load_dotenv(self.env_path, override=self.override_os_envs)  # type: ignore
+            # Recompute constants after loading env variables
+            importlib.reload(constants)
+            # Recompute instance attributes
+            self.recompute_field_values()
+
+    def recompute_field_values(self):
+        """Recompute instance field values to reflect new values after reloading
+        constant values.
+        """
+        for field in self.get_fields():
+            try:
+                if field.startswith("_"):
+                    continue
+                setattr(self, field, getattr(constants, f"{field.upper()}"))
+            except AttributeError:
+                pass
+
 
 def get_config() -> Config:
     """Get the app config.
 
     Returns:
         The app config.
     """
     from pynecone.config import Config
 
     sys.path.append(os.getcwd())
     try:
         return __import__(constants.CONFIG_MODULE).config
+
     except ImportError:
         return Config(app_name="")  # type: ignore
```

### Comparing `pynecone-0.1.32a1/pynecone/constants.py` & `pynecone-0.1.33a0/pynecone/constants.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,43 @@
 """Constants used throughout the package."""
 
 import os
 import re
 from enum import Enum
 from types import SimpleNamespace
+from typing import Any, Type
 
 import pkg_resources
 
+
+def get_value(key: str, default: Any = None, type_: Type = str) -> Type:
+    """Get the value for the constant.
+    Obtain os env value and cast non-string types into
+    their original types.
+
+    Args:
+        key: constant name.
+        default: default value if key doesn't exist.
+        type_: the type of the constant.
+
+    Returns:
+        the value of the constant in its designated type
+    """
+    value = os.getenv(key, default)
+    try:
+        if value and type_ != str:
+            value = eval(value)
+    except Exception:
+        pass
+    finally:
+        # Special case for db_url expects None to be a valid input when
+        # user explicitly overrides db_url as None
+        return value if value != "None" else None  # noqa B012
+
+
 # App names and versions.
 # The name of the Pynecone package.
 MODULE_NAME = "pynecone"
 # The current version of Pynecone.
 VERSION = pkg_resources.get_distribution(MODULE_NAME).version
 # Minimum version of Node.js required to run Pynecone.
 MIN_NODE_VERSION = "16.8.0"
@@ -57,28 +84,31 @@
 # The package lock file.
 PACKAGE_LOCK = "package-lock.json"
 # The pcversion app file.
 PCVERSION_APP_FILE = os.path.join(WEB_DIR, "pynecone.json")
 ENV_JSON = os.path.join(WEB_DIR, "env.json")
 
 # Commands to run the app.
+DOT_ENV_FILE = ".env"
 # The frontend default port.
-FRONTEND_PORT = "3000"
+FRONTEND_PORT = get_value("FRONTEND_PORT", "3000")
 # The backend default port.
-BACKEND_PORT = "8000"
+BACKEND_PORT = get_value("BACKEND_PORT", "8000")
 # The backend api url.
-API_URL = "http://localhost:8000"
+API_URL = get_value("API_URL", "http://localhost:8000")
+# The deploy url
+DEPLOY_URL = get_value("DEPLOY_URL")
 # bun root location
 BUN_ROOT_PATH = "$HOME/.bun"
 # The default path where bun is installed.
-BUN_PATH = f"{BUN_ROOT_PATH}/bin/bun"
+BUN_PATH = get_value("BUN_PATH", f"{BUN_ROOT_PATH}/bin/bun")
 # Command to install bun.
 INSTALL_BUN = f"curl -fsSL https://bun.sh/install | bash -s -- bun-v{MAX_BUN_VERSION}"
 # Default host in dev mode.
-BACKEND_HOST = "0.0.0.0"
+BACKEND_HOST = get_value("BACKEND_HOST", "0.0.0.0")
 # The default timeout when launching the gunicorn server.
 TIMEOUT = 120
 # The command to run the backend in production mode.
 RUN_BACKEND_PROD = f"gunicorn --worker-class uvicorn.workers.UvicornH11Worker --preload --timeout {TIMEOUT} --log-level critical".split()
 RUN_BACKEND_PROD_WINDOWS = f"uvicorn --timeout-keep-alive {TIMEOUT}".split()
 # Socket.IO web server
 PING_INTERVAL = 25
@@ -118,31 +148,32 @@
 # The prefix used to create setters for state vars.
 SETTER_PREFIX = "set_"
 # The name of the frontend zip during deployment.
 FRONTEND_ZIP = "frontend.zip"
 # The name of the backend zip during deployment.
 BACKEND_ZIP = "backend.zip"
 # The name of the sqlite database.
-DB_NAME = "pynecone.db"
+DB_NAME = os.getenv("DB_NAME", "pynecone.db")
 # The sqlite url.
-DB_URL = f"sqlite:///{DB_NAME}"
+DB_URL = get_value("DB_URL", f"sqlite:///{DB_NAME}")
+# The redis url
+REDIS_URL = get_value("REDIS_URL")
 # The default title to show for Pynecone apps.
 DEFAULT_TITLE = "Pynecone App"
 # The default description to show for Pynecone apps.
 DEFAULT_DESCRIPTION = "A Pynecone app."
 # The default image to show for Pynecone apps.
 DEFAULT_IMAGE = "favicon.ico"
 # The default meta list to show for Pynecone apps.
 DEFAULT_META_LIST = []
 
-
 # The gitignore file.
 GITIGNORE_FILE = ".gitignore"
 # Files to gitignore.
-DEFAULT_GITIGNORE = {WEB_DIR, DB_NAME}
+DEFAULT_GITIGNORE = {WEB_DIR, DB_NAME, "__pycache__/", "*.py[cod]"}
 # The name of the pynecone config module.
 CONFIG_MODULE = "pcconfig"
 # The python config file.
 CONFIG_FILE = f"{CONFIG_MODULE}{PY_EXT}"
 # The deployment URL.
 PRODUCTION_BACKEND_URL = "https://{username}-{app_name}.api.pynecone.app"
 # Token expiration time in seconds.
@@ -302,9 +333,9 @@
 
 # Color mode variables
 USE_COLOR_MODE = "useColorMode"
 COLOR_MODE = "colorMode"
 TOGGLE_COLOR_MODE = "toggleColorMode"
 
 # Server socket configuration variables
-CORS_ALLOWED_ORIGINS = "*"
+CORS_ALLOWED_ORIGINS = get_value("CORS_ALLOWED_ORIGINS", ["*"], list)
 POLLING_MAX_HTTP_BUFFER_SIZE = 1000 * 1000
```

### Comparing `pynecone-0.1.32a1/pynecone/el/constants/html.py` & `pynecone-0.1.33a0/pynecone/el/constants/html.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/el/constants/pynecone.py` & `pynecone-0.1.33a0/pynecone/el/constants/pynecone.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/el/constants/react.py` & `pynecone-0.1.33a0/pynecone/el/constants/react.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/el/element.py` & `pynecone-0.1.33a0/pynecone/el/element.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/el/elements/__init__.py` & `pynecone-0.1.33a0/pynecone/el/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/el/precompile.py` & `pynecone-0.1.33a0/pynecone/el/precompile.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/event.py` & `pynecone-0.1.33a0/pynecone/event.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     payload: Dict[str, Any] = {}
 
 
 class EventHandler(Base):
     """An event handler responds to an event to update the state."""
 
     # The function to call in response to the event.
-    fn: Callable
+    fn: Any
 
     class Config:
         """The Pydantic config."""
 
         # Needed to allow serialization of Callable.
         frozen = True
 
@@ -198,14 +198,30 @@
 
     Returns:
         An event to alert the message.
     """
     return server_side("_alert", get_fn_signature(window_alert), message=message)
 
 
+def set_focus(ref: str) -> EventSpec:
+    """Set focus to specified ref.
+
+    Args:
+        ref: The ref.
+
+    Returns:
+        An event to set focus on the ref
+    """
+    return server_side(
+        "_set_focus",
+        get_fn_signature(set_focus),
+        ref=Var.create_safe(format.format_ref(ref)),
+    )
+
+
 def set_value(ref: str, value: Any) -> EventSpec:
     """Set the value of a ref.
 
     Args:
         ref: The ref.
         value: The value to set.
```

### Comparing `pynecone-0.1.32a1/pynecone/middleware/hydrate_middleware.py` & `pynecone-0.1.33a0/pynecone/middleware/hydrate_middleware.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/middleware/middleware.py` & `pynecone-0.1.33a0/pynecone/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/model.py` & `pynecone-0.1.33a0/pynecone/model.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/pc.py` & `pynecone-0.1.33a0/pynecone/pc.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,25 +68,34 @@
     frontend: bool = typer.Option(
         False, "--frontend-only", help="Execute only frontend."
     ),
     backend: bool = typer.Option(False, "--backend-only", help="Execute only backend."),
     loglevel: constants.LogLevel = typer.Option(
         constants.LogLevel.ERROR, help="The log level to use."
     ),
-    port: str = typer.Option(None, help="Specify a different frontend port."),
+    frontend_port: str = typer.Option(None, help="Specify a different frontend port."),
     backend_port: str = typer.Option(None, help="Specify a different backend port."),
     backend_host: str = typer.Option(None, help="Specify the backend host."),
 ):
     """Run the app in the current directory."""
     if platform.system() == "Windows":
         console.print(
             "[yellow][WARNING] We strongly advise you to use Windows Subsystem for Linux (WSL) for optimal performance when using Pynecone. Due to compatibility issues with one of our dependencies, Bun, you may experience slower performance on Windows. By using WSL, you can expect to see a significant speed increase."
         )
+    # Set ports as os env variables to take precedence over config and
+    # .env variables(if override_os_envs flag in config is set to False).
+    build.set_os_env(
+        frontend_port=frontend_port,
+        backend_port=backend_port,
+        backend_host=backend_host,
+    )
 
-    frontend_port = get_config().port if port is None else port
+    frontend_port = (
+        get_config().frontend_port if frontend_port is None else frontend_port
+    )
     backend_port = get_config().backend_port if backend_port is None else backend_port
     backend_host = get_config().backend_host if backend_host is None else backend_host
 
     # If no --frontend-only and no --backend-only, then turn on frontend and backend both
     if not frontend and not backend:
         frontend = True
         backend = True
```

### Comparing `pynecone-0.1.32a1/pynecone/route.py` & `pynecone-0.1.33a0/pynecone/route.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/state.py` & `pynecone-0.1.33a0/pynecone/state.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 """Define the pynecone state specification."""
 from __future__ import annotations
 
 import asyncio
 import copy
 import functools
+import inspect
 import traceback
 from abc import ABC
 from collections import defaultdict
 from typing import (
     Any,
+    AsyncIterator,
     Callable,
     ClassVar,
     Dict,
     List,
     Optional,
     Sequence,
     Set,
+    Tuple,
     Type,
     Union,
 )
 
 import cloudpickle
 import pydantic
 from redis import Redis
 
 from pynecone import constants
 from pynecone.base import Base
-from pynecone.event import Event, EventHandler, fix_events, window_alert
+from pynecone.event import Event, EventHandler, EventSpec, fix_events, window_alert
 from pynecone.utils import format, prerequisites, types
 from pynecone.vars import BaseVar, ComputedVar, PCDict, PCList, Var
 
 Delta = Dict[str, Any]
 
 
 class State(Base, ABC, extra=pydantic.Extra.allow):
@@ -614,21 +617,21 @@
             if len(path) == 1:
                 return self
             path = path[1:]
         if path[0] not in self.substates:
             raise ValueError(f"Invalid path: {path}")
         return self.substates[path[0]].get_substate(path[1:])
 
-    async def _process(self, event: Event) -> StateUpdate:
+    async def _process(self, event: Event) -> AsyncIterator[StateUpdate]:
         """Obtain event info and process event.
 
         Args:
             event: The event to process.
 
-        Returns:
+        Yields:
             The state update after processing the event.
 
         Raises:
             ValueError: If the state value is None.
         """
         # Get the event handler.
         path = event.name.split(".")
@@ -637,60 +640,87 @@
         handler = substate.event_handlers[name]  # type: ignore
 
         if not substate:
             raise ValueError(
                 "The value of state cannot be None when processing an event."
             )
 
-        return await self._process_event(
+        # Get the event generator.
+        event_iter = self._process_event(
             handler=handler,
             state=substate,
             payload=event.payload,
-            token=event.token,
         )
 
+        # Clean the state before processing the event.
+        self.clean()
+
+        # Run the event generator and return state updates.
+        async for events, processing in event_iter:
+            # Fix the returned events.
+            events = fix_events(events, event.token)  # type: ignore
+
+            # Get the delta after processing the event.
+            delta = self.get_delta()
+
+            # Yield the state update.
+            yield StateUpdate(delta=delta, events=events, processing=processing)
+
+            # Clean the state to prepare for the next event.
+            self.clean()
+
     async def _process_event(
-        self, handler: EventHandler, state: State, payload: Dict, token: str
-    ) -> StateUpdate:
+        self, handler: EventHandler, state: State, payload: Dict
+    ) -> AsyncIterator[Tuple[Optional[List[EventSpec]], bool]]:
         """Process event.
 
         Args:
             handler: Eventhandler to process.
             state: State to process the handler.
             payload: The event payload.
-            token: Client token.
 
-        Returns:
-            The state update after processing the event.
+        Yields:
+            Tuple containing:
+                0: The state update after processing the event.
+                1: Whether the event is being processed.
         """
+        # Get the function to process the event.
         fn = functools.partial(handler.fn, state)
+
+        # Wrap the function in a try/except block.
         try:
+            # Handle async functions.
             if asyncio.iscoroutinefunction(fn.func):
                 events = await fn(**payload)
+
+            # Handle regular functions.
             else:
                 events = fn(**payload)
-        except Exception:
-            error = traceback.format_exc()
-            print(error)
-            events = fix_events(
-                [window_alert("An error occurred. See logs for details.")], token
-            )
-            return StateUpdate(events=events)
-
-        # Fix the returned events.
-        events = fix_events(events, token)
 
-        # Get the delta after processing the event.
-        delta = self.get_delta()
+            # Handle async generators.
+            if inspect.isasyncgen(events):
+                async for event in events:
+                    yield event, True
+                yield None, False
+
+            # Handle regular generators.
+            elif inspect.isgenerator(events):
+                for event in events:
+                    yield event, True
+                yield None, False
 
-        # Reset the dirty vars.
-        self.clean()
+            # Handle regular event chains.
+            else:
+                yield events, False
 
-        # Return the state update.
-        return StateUpdate(delta=delta, events=events)
+        # If an error occurs, throw a window alert.
+        except Exception:
+            error = traceback.format_exc()
+            print(error)
+            yield [window_alert("An error occurred. See logs for details.")], False
 
     def _always_dirty_computed_vars(self) -> Set[str]:
         """The set of ComputedVars that always need to be recalculated.
 
         Returns:
             Set of all ComputedVar in this state where cache=False
         """
@@ -847,14 +877,17 @@
 
     # The state delta.
     delta: Delta = {}
 
     # Events to be added to the event queue.
     events: List[Event] = []
 
+    # Whether the event is still processing.
+    processing: bool = False
+
 
 class StateManager(Base):
     """A class to manage many client states."""
 
     # The state class to use.
     state: Type[State] = DefaultState
```

### Comparing `pynecone-0.1.32a1/pynecone/style.py` & `pynecone-0.1.33a0/pynecone/style.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/utils/build.py` & `pynecone-0.1.33a0/pynecone/utils/build.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,14 +54,26 @@
             "uploadUrl": constants.Endpoint.UPLOAD.get_url(),
             "eventUrl": constants.Endpoint.EVENT.get_url(),
             "pingUrl": constants.Endpoint.PING.get_url(),
         },
     )
 
 
+def set_os_env(**kwargs):
+    """Set os environment variables.
+
+    Args:
+        kwargs: env key word args.
+    """
+    for key, value in kwargs.items():
+        if not value:
+            continue
+        os.environ[key.upper()] = value
+
+
 def generate_sitemap(deploy_url: str):
     """Generate the sitemap config file.
 
     Args:
         deploy_url: The URL of the deployed app.
     """
     # Import here to avoid circular imports.
```

### Comparing `pynecone-0.1.32a1/pynecone/utils/console.py` & `pynecone-0.1.33a0/pynecone/utils/console.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/utils/exec.py` & `pynecone-0.1.33a0/pynecone/utils/exec.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     setup_frontend(root)
 
     # Start watching asset folder.
     start_watching_assets_folder(root)
 
     # Run the frontend in development mode.
     console.rule("[bold green]App Running")
-    os.environ["PORT"] = get_config().port if port is None else port
+    os.environ["PORT"] = get_config().frontend_port if port is None else port
     run_process_and_launch_url(
         [prerequisites.get_package_manager(), "run", "dev"], root, loglevel
     )
 
 
 def run_frontend_prod(
     app: App,
@@ -119,15 +119,15 @@
     # Set up the frontend.
     setup_frontend(root)
 
     # Export the app.
     export_app(app, loglevel=loglevel)
 
     # Set the port.
-    os.environ["PORT"] = get_config().port if port is None else port
+    os.environ["PORT"] = get_config().frontend_port if port is None else port
 
     # Run the frontend in production mode.
     console.rule("[bold green]App Running")
     run_process_and_launch_url(
         [prerequisites.get_package_manager(), "run", "prod"], root, loglevel
     )
```

### Comparing `pynecone-0.1.32a1/pynecone/utils/format.py` & `pynecone-0.1.33a0/pynecone/utils/format.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Formatting operations."""
 
 from __future__ import annotations
 
+import base64
+import io
 import json
 import os
 import re
 import sys
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Type
 
 import plotly.graph_objects as go
@@ -355,14 +357,30 @@
         for d in data:
             element.append(str(d) if isinstance(d, (list, tuple)) else d)
         format_data.append(element)
 
     return format_data
 
 
+def format_image_data(value: Type) -> str:
+    """Format image data.
+
+    Args:
+        value: The value to format.
+
+    Returns:
+        Format data
+    """
+    buff = io.BytesIO()
+    value.save(buff, format="PNG")
+    image_bytes = buff.getvalue()
+    base64_image = base64.b64encode(image_bytes).decode("utf-8")
+    return f"data:image/png;base64,{base64_image}"
+
+
 def format_state(value: Any) -> Dict:
     """Recursively format values in the given state.
 
     Args:
         value: The state to format.
 
     Returns:
@@ -386,14 +404,18 @@
     # Convert pandas dataframes to JSON.
     if types.is_dataframe(type(value)):
         return {
             "columns": value.columns.tolist(),
             "data": format_dataframe_values(value),
         }
 
+    # Convert Image objects to base64.
+    if types.is_image(type(value)):
+        return format_image_data(value)  # type: ignore
+
     raise TypeError(
         "State vars must be primitive Python types, "
         "or subclasses of pc.Base. "
         f"Got var of type {type(value)}."
     )
```

### Comparing `pynecone-0.1.32a1/pynecone/utils/imports.py` & `pynecone-0.1.33a0/pynecone/utils/imports.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/utils/path_ops.py` & `pynecone-0.1.33a0/pynecone/utils/path_ops.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/utils/prerequisites.py` & `pynecone-0.1.33a0/pynecone/utils/prerequisites.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/utils/processes.py` & `pynecone-0.1.33a0/pynecone/utils/processes.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/utils/telemetry.py` & `pynecone-0.1.33a0/pynecone/utils/telemetry.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/utils/types.py` & `pynecone-0.1.33a0/pynecone/utils/types.py`

 * *Files 18% similar despite different names*

```diff
@@ -137,14 +137,28 @@
         Whether the value is a dataframe.
     """
     if is_generic_alias(value) or value == typing.Any:
         return False
     return value.__name__ == "DataFrame"
 
 
+def is_image(value: Type) -> bool:
+    """Check if the given value is a pillow image. By checking if the value subclasses PIL.
+
+    Args:
+        value: The value to check.
+
+    Returns:
+        Whether the value is a pillow image.
+    """
+    if is_generic_alias(value) or value == typing.Any:
+        return False
+    return "PIL" in value.__module__
+
+
 def is_figure(value: Type) -> bool:
     """Check if the given value is a figure.
 
     Args:
         value: The value to check.
 
     Returns:
@@ -158,15 +172,20 @@
 
     Args:
         var: The value to check.
 
     Returns:
         Whether the value is a valid prop type.
     """
-    return _issubclass(var, StateVar) or is_dataframe(var) or is_figure(var)
+    return (
+        _issubclass(var, StateVar)
+        or is_dataframe(var)
+        or is_figure(var)
+        or is_image(var)
+    )
 
 
 def is_backend_variable(name: str) -> bool:
     """Check if this variable name correspond to a backend variable.
 
     Args:
         name: The name of the variable to check
```

### Comparing `pynecone-0.1.32a1/pynecone/utils/watch.py` & `pynecone-0.1.33a0/pynecone/utils/watch.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pynecone/vars.py` & `pynecone-0.1.33a0/pynecone/vars.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.32a1/pyproject.toml` & `pynecone-0.1.33a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pynecone"
-version = "0.1.32a1"
+version = "0.1.33a0"
 description = "Web apps in pure Python."
 license = "Apache-2.0"
 authors = [
     "Nikhil Rao <nikhil@pynecone.io>",
     "Alek Petuskey <alek@pynecone.io>",
 ]
 readme = "README.md"
@@ -27,24 +27,25 @@
 cloudpickle = "^2.2.1"
 fastapi = "^0.92.0"
 gunicorn = "^20.1.0"
 httpx = "^0.23.0"
 jinja2 = "^3.1.2"
 plotly = "^5.13.0"
 psutil = "^5.9.4"
-pydantic = "1.10.2"
+pydantic = "^1.10.2"
 python-multipart = "^0.0.5"
 python-socketio = "^5.7.0"
 redis = "^4.3.5"
 rich = "^13.0.0"
 sqlmodel = "^0.0.8"
 typer = "0.4.2"
 uvicorn = "^0.20.0"
 watchdog = "^2.3.1"
 websockets = "^10.4"
+python-dotenv = "^0.13.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.2"
 pytest-mock = "^3.10.0"
 pyright = "^1.1.229"
 darglint = "^1.8.1"
 toml = "^0.10.2"
```

### Comparing `pynecone-0.1.32a1/PKG-INFO` & `pynecone-0.1.33a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynecone
-Version: 0.1.32a1
+Version: 0.1.33a0
 Summary: Web apps in pure Python.
 Home-page: https://pynecone.io
 License: Apache-2.0
 Keywords: web,framework
 Author: Nikhil Rao
 Author-email: nikhil@pynecone.io
 Requires-Python: >=3.7,<4.0
@@ -19,15 +19,16 @@
 Requires-Dist: cloudpickle (>=2.2.1,<3.0.0)
 Requires-Dist: fastapi (>=0.92.0,<0.93.0)
 Requires-Dist: gunicorn (>=20.1.0,<21.0.0)
 Requires-Dist: httpx (>=0.23.0,<0.24.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: plotly (>=5.13.0,<6.0.0)
 Requires-Dist: psutil (>=5.9.4,<6.0.0)
-Requires-Dist: pydantic (==1.10.2)
+Requires-Dist: pydantic (>=1.10.2,<2.0.0)
+Requires-Dist: python-dotenv (>=0.13.0,<0.14.0)
 Requires-Dist: python-multipart (>=0.0.5,<0.0.6)
 Requires-Dist: python-socketio (>=5.7.0,<6.0.0)
 Requires-Dist: redis (>=4.3.5,<5.0.0)
 Requires-Dist: rich (>=13.0.0,<14.0.0)
 Requires-Dist: sqlmodel (>=0.0.8,<0.0.9)
 Requires-Dist: typer (==0.4.2)
 Requires-Dist: uvicorn (>=0.20.0,<0.21.0)
```

