# Comparing `tmp/ckanext-dcat_usmetadata-0.4.0.tar.gz` & `tmp/ckanext-dcat_usmetadata-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-dcat_usmetadata-0.4.0.tar", last modified: Thu Sep 15 14:38:23 2022, max compression
+gzip compressed data, was "ckanext-dcat_usmetadata-0.4.1.tar", last modified: Mon Jun  5 18:55:07 2023, max compression
```

## Comparing `ckanext-dcat_usmetadata-0.4.0.tar` & `ckanext-dcat_usmetadata-0.4.1.tar`

### file list

```diff
@@ -1,196 +1,196 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 14:38:23.004873 ckanext-dcat_usmetadata-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (121)    34499 2022-09-15 14:36:18.000000 ckanext-dcat_usmetadata-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      202 2022-09-15 14:36:18.000000 ckanext-dcat_usmetadata-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    12105 2022-09-15 14:38:23.004873 ckanext-dcat_usmetadata-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9623 2022-09-15 14:36:18.000000 ckanext-dcat_usmetadata-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 14:38:22.972873 ckanext-dcat_usmetadata-0.4.0/ckanext/
--rw-r--r--   0 runner    (1001) docker     (121)      219 2022-09-15 14:36:18.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 14:38:22.972873 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-15 14:36:18.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2371 2022-09-15 14:36:18.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/blueprint.py
--rw-r--r--   0 runner    (1001) docker     (121)     2247 2022-09-15 14:36:18.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     1492 2022-09-15 14:36:18.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/db_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 14:38:22.972873 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/fanstatic/
--rw-r--r--   0 runner    (1001) docker     (121)      127 2022-09-15 14:36:18.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/fanstatic/custom.css
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-09-15 14:36:18.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/fanstatic/webassets.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1158 2022-09-15 14:36:18.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 14:38:22.972873 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 14:38:22.972873 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 14:38:23.000873 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/
--rw-r--r--   0 runner    (1001) docker     (121)    25896 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Bitter-Bold.21c58d74.ttf
--rw-r--r--   0 runner    (1001) docker     (121)    23344 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Bitter-Bold.9efe74f3.eot
--rw-r--r--   0 runner    (1001) docker     (121)    15644 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Bitter-Bold.b786d169.woff
--rw-r--r--   0 runner    (1001) docker     (121)    11496 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Bitter-Bold.fc1844c7.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    25880 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Bitter-Italic.18853b8c.eot
--rw-r--r--   0 runner    (1001) docker     (121)    39420 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Bitter-Italic.58093e86.ttf
--rw-r--r--   0 runner    (1001) docker     (121)    14296 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Bitter-Italic.75fb25c1.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    20216 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Bitter-Italic.f09ccd61.woff
--rw-r--r--   0 runner    (1001) docker     (121)    33984 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Bitter-Regular.0078d318.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    24320 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Bitter-Regular.12b71a42.eot
--rw-r--r--   0 runner    (1001) docker     (121)    22436 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Bitter-Regular.22c8272f.woff
--rw-r--r--   0 runner    (1001) docker     (121)    90628 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Bitter-Regular.c99f7ae5.ttf
--rw-r--r--   0 runner    (1001) docker     (121)    21308 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-Bold.115f5a1d.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    47228 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-Bold.46eab112.ttf
--rw-r--r--   0 runner    (1001) docker     (121)    26892 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-Bold.704b3917.woff
--rw-r--r--   0 runner    (1001) docker     (121)    19568 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-BoldItalic.2750a1e9.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    24464 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-BoldItalic.69debb55.woff
--rw-r--r--   0 runner    (1001) docker     (121)    40472 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-BoldItalic.9bce1501.ttf
--rw-r--r--   0 runner    (1001) docker     (121)    19252 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-Italic.2412c72a.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    39480 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-Italic.3ee014ee.ttf
--rw-r--r--   0 runner    (1001) docker     (121)    24152 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-Italic.b85b8ae5.woff
--rw-r--r--   0 runner    (1001) docker     (121)    21260 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-Light.4f0fb504.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    26988 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-Light.ddae281a.woff
--rw-r--r--   0 runner    (1001) docker     (121)    49164 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-Light.e6dc7e59.ttf
--rw-r--r--   0 runner    (1001) docker     (121)    18976 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-LightItalic.08acae9c.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    23808 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-LightItalic.af8e7e14.woff
--rw-r--r--   0 runner    (1001) docker     (121)    39456 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-LightItalic.efbd9a2b.ttf
--rw-r--r--   0 runner    (1001) docker     (121)    27512 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-Regular.73c28f4e.woff
--rw-r--r--   0 runner    (1001) docker     (121)    49484 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-Regular.efc70b44.ttf
--rw-r--r--   0 runner    (1001) docker     (121)    21692 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-Regular.fa9b615a.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    11584 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Bold-webfont.3c4dc405.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    15440 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Bold-webfont.6a13b444.woff
--rw-r--r--   0 runner    (1001) docker     (121)    23602 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Bold-webfont.8bb31d27.eot
--rw-r--r--   0 runner    (1001) docker     (121)    23424 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Bold-webfont.bf0b1c03.ttf
--rw-r--r--   0 runner    (1001) docker     (121)    13048 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Italic-webfont.318b4f41.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    25792 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Italic-webfont.346b43cf.ttf
--rw-r--r--   0 runner    (1001) docker     (121)    25978 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Italic-webfont.9487423d.eot
--rw-r--r--   0 runner    (1001) docker     (121)    17204 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Italic-webfont.c0de58fc.woff
--rw-r--r--   0 runner    (1001) docker     (121)    22902 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Regular-webfont.33ec9bca.eot
--rw-r--r--   0 runner    (1001) docker     (121)    15284 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Regular-webfont.467063b1.woff
--rw-r--r--   0 runner    (1001) docker     (121)    22712 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Regular-webfont.cb95bc69.ttf
--rw-r--r--   0 runner    (1001) docker     (121)    11472 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Regular-webfont.e3b01381.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    23032 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Semibold-webfont.80744a04.ttf
--rw-r--r--   0 runner    (1001) docker     (121)    15364 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Semibold-webfont.8e80acc0.woff
--rw-r--r--   0 runner    (1001) docker     (121)    11536 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Semibold-webfont.aebd17d5.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    23226 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Semibold-webfont.d543421f.eot
--rw-r--r--   0 runner    (1001) docker     (121)      173 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/add.0e3e08bc.svg
--rw-r--r--   0 runner    (1001) docker     (121)      552 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/angle-arrow-down-primary.51295a10.svg
--rw-r--r--   0 runner    (1001) docker     (121)      544 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/angle-arrow-down.8e2c6296.svg
--rw-r--r--   0 runner    (1001) docker     (121)      542 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/angle-arrow-right.0f46e09b.svg
--rw-r--r--   0 runner    (1001) docker     (121)      551 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/angle-arrow-up-white.e60b3e19.svg
--rw-r--r--   0 runner    (1001) docker     (121)      625 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/angle-double-left-solid.a1c42657.svg
--rw-r--r--   0 runner    (1001) docker     (121)      629 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/angle-double-right-solid.9addc335.svg
--rw-r--r--   0 runner    (1001) docker     (121)      422 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/angle-left-solid.247b735a.svg
--rw-r--r--   0 runner    (1001) docker     (121)      425 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/angle-right-solid.fe82c509.svg
--rw-r--r--   0 runner    (1001) docker     (121)      558 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/arrow-both.0bfe2193.svg
--rw-r--r--   0 runner    (1001) docker     (121)      338 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/arrow-both.50893060.svg
--rw-r--r--   0 runner    (1001) docker     (121)      566 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/arrow-down-gray-60.9b52f832.svg
--rw-r--r--   0 runner    (1001) docker     (121)      551 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/arrow-down.6c056294.svg
--rw-r--r--   0 runner    (1001) docker     (121)      404 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/arrow-down.cb9919ed.svg
--rw-r--r--   0 runner    (1001) docker     (121)      665 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/arrow-left.ffd0d3ac.svg
--rw-r--r--   0 runner    (1001) docker     (121)      553 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/arrow-right.750bd27b.svg
--rw-r--r--   0 runner    (1001) docker     (121)      407 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/arrow-up.7fa2607f.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1063 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/calendar-alt-solid.95c20e20.svg
--rw-r--r--   0 runner    (1001) docker     (121)      255 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/check_circle.90deb06e.svg
--rw-r--r--   0 runner    (1001) docker     (121)      550 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/checkbox-check-print.fdb58020.svg
--rw-r--r--   0 runner    (1001) docker     (121)      332 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/checkmark-green.142e6c1d.svg
--rw-r--r--   0 runner    (1001) docker     (121)      532 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/chevron.f15c792a.svg
--rw-r--r--   0 runner    (1001) docker     (121)      661 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/close--primary-darker.05ee67ed.svg
--rw-r--r--   0 runner    (1001) docker     (121)      661 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/close--primary.c716dc4c.svg
--rw-r--r--   0 runner    (1001) docker     (121)      251 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/close-alt.659d1890.svg
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/close-alt.8e9b0025.svg
--rw-r--r--   0 runner    (1001) docker     (121)      495 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/close-gray-60.7e82cc30.svg
--rw-r--r--   0 runner    (1001) docker     (121)      626 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/close.fe903f4b.svg
--rw-r--r--   0 runner    (1001) docker     (121)      600 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/correct8.1c696dec.svg
--rw-r--r--   0 runner    (1001) docker     (121)      615 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/correct9.1730d813.svg
--rw-r--r--   0 runner    (1001) docker     (121)      367 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/download.381b359a.svg
--rw-r--r--   0 runner    (1001) docker     (121)      250 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/error-white.6252fbdb.svg
--rw-r--r--   0 runner    (1001) docker     (121)      234 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/error.62d23dd4.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1094 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/error.e73ca64b.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1174 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/external-link-alt-hover.74ba81d1.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1171 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/external-link-alt.4b6aa08a.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1173 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/external-link-hover.73f16cba.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1167 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/external-link.18ea418e.svg
--rw-r--r--   0 runner    (1001) docker     (121)      415 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/facebook25.754f3a1c.svg
--rw-r--r--   0 runner    (1001) docker     (121)      658 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/file-excel.f208070c.svg
--rw-r--r--   0 runner    (1001) docker     (121)      904 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/file-pdf.080ccfc5.svg
--rw-r--r--   0 runner    (1001) docker     (121)      574 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/file-video.15c2687c.svg
--rw-r--r--   0 runner    (1001) docker     (121)      760 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/file-word.2fc990ab.svg
--rw-r--r--   0 runner    (1001) docker     (121)      283 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/file.eb89414b.svg
--rw-r--r--   0 runner    (1001) docker     (121)   689079 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/hero.544cee01.png
--rw-r--r--   0 runner    (1001) docker     (121)      276 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/image.45732aef.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1890 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/info.157ac1b1.svg
--rw-r--r--   0 runner    (1001) docker     (121)      234 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/info.e24db876.svg
--rw-r--r--   0 runner    (1001) docker     (121)      428 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/information-new-hover.2d7be265.svg
--rw-r--r--   0 runner    (1001) docker     (121)      264 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/information-new.3ff7655b.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1298 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/information.61116626.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1713 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/loader.c04c3ed0.svg
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/next.872082d4.svg
--rw-r--r--   0 runner    (1001) docker     (121)      988 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/pdf.f6d71f14.svg
--rw-r--r--   0 runner    (1001) docker     (121)      155 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/remove.d788b81e.svg
--rw-r--r--   0 runner    (1001) docker     (121)    32160 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-300.287fb5bc.ttf
--rw-r--r--   0 runner    (1001) docker     (121)    19884 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-300.4f691391.woff
--rw-r--r--   0 runner    (1001) docker     (121)    16380 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-300.db95b37e.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    17340 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-300italic.18357dda.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    21052 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-300italic.8debb2d5.woff
--rw-r--r--   0 runner    (1001) docker     (121)    32596 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-300italic.c24ee49d.ttf
--rw-r--r--   0 runner    (1001) docker     (121)    31092 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-700.0017dad2.ttf
--rw-r--r--   0 runner    (1001) docker     (121)    15956 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-700.4bc0bd04.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    19564 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-700.f61e5a8d.woff
--rw-r--r--   0 runner    (1001) docker     (121)    32564 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-700italic.27139953.ttf
--rw-r--r--   0 runner    (1001) docker     (121)    17336 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-700italic.5eca10b5.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    21132 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-700italic.7324e30e.woff
--rw-r--r--   0 runner    (1001) docker     (121)    17312 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-italic.55befc28.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    21096 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-italic.5711b84f.woff
--rw-r--r--   0 runner    (1001) docker     (121)    32336 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-italic.e3c56211.ttf
--rw-r--r--   0 runner    (1001) docker     (121)    19576 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-regular.1db1469b.woff
--rw-r--r--   0 runner    (1001) docker     (121)    31052 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-regular.c03588a7.ttf
--rw-r--r--   0 runner    (1001) docker     (121)    16028 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-regular.e92cc0fb.woff2
--rw-r--r--   0 runner    (1001) docker     (121)     1484 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/rss25.13c4042b.svg
--rw-r--r--   0 runner    (1001) docker     (121)      387 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/search--white.cebf50fe.svg
--rw-r--r--   0 runner    (1001) docker     (121)    26040 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-bold-webfont.738b5fd5.woff
--rw-r--r--   0 runner    (1001) docker     (121)    54340 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-bold-webfont.ab04959e.ttf
--rw-r--r--   0 runner    (1001) docker     (121)    20368 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-bold-webfont.f12f6a2f.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    38760 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-bolditalic-webfont.00a1cd13.ttf
--rw-r--r--   0 runner    (1001) docker     (121)    20164 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-bolditalic-webfont.60573f53.woff
--rw-r--r--   0 runner    (1001) docker     (121)    16416 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-bolditalic-webfont.dae8945d.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    20204 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-italic-webfont.12c96d9d.woff
--rw-r--r--   0 runner    (1001) docker     (121)    16372 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-italic-webfont.8740838d.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    38848 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-italic-webfont.bf26dc0f.ttf
--rw-r--r--   0 runner    (1001) docker     (121)    20412 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-light-webfont.4572c51e.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    25956 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-light-webfont.9cf8ece9.woff
--rw-r--r--   0 runner    (1001) docker     (121)    54504 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-light-webfont.fb881861.ttf
--rw-r--r--   0 runner    (1001) docker     (121)    39144 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-lightitalic-webfont.03f9a24f.ttf
--rw-r--r--   0 runner    (1001) docker     (121)    20256 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-lightitalic-webfont.3fa6ebb8.woff
--rw-r--r--   0 runner    (1001) docker     (121)    16316 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-lightitalic-webfont.ffb6369e.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    26140 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-regular-webfont.34197df8.woff
--rw-r--r--   0 runner    (1001) docker     (121)    54432 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-regular-webfont.998d95f8.ttf
--rw-r--r--   0 runner    (1001) docker     (121)    20540 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-regular-webfont.d67b548b.woff2
--rw-r--r--   0 runner    (1001) docker     (121)      205 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/star-filled.b51af7f7.svg
--rw-r--r--   0 runner    (1001) docker     (121)      235 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/star.85ebfc24.svg
--rw-r--r--   0 runner    (1001) docker     (121)      957 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/success-fill.8a5df9fd.svg
--rw-r--r--   0 runner    (1001) docker     (121)      515 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/success.7144d784.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1126 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/twitter16.60eb977c.svg
--rw-r--r--   0 runner    (1001) docker     (121)      992 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/warning.2e405b2b.svg
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/warning.62d335b7.svg
--rw-r--r--   0 runner    (1001) docker     (121)     2688 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/youtube15.9d356b3b.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 14:38:23.000873 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/css/
--rw-r--r--   0 runner    (1001) docker     (121)   434115 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/css/2.chunk.css
--rw-r--r--   0 runner    (1001) docker     (121)     7043 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/css/main.chunk.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 14:38:23.004873 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/js/
--rw-r--r--   0 runner    (1001) docker     (121)   482374 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/js/2.chunk.js
--rw-r--r--   0 runner    (1001) docker     (121)    81776 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/js/main.chunk.js
--rw-r--r--   0 runner    (1001) docker     (121)     1584 2022-09-15 14:38:21.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/js/runtime-main.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 14:38:23.004873 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/templates/
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-09-15 14:36:18.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (121)      404 2022-09-15 14:36:18.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/templates/new-metadata.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 14:38:23.004873 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/templates/organization/
--rw-r--r--   0 runner    (1001) docker     (121)      322 2022-09-15 14:36:18.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/templates/organization/read.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 14:38:23.004873 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/templates/package/
--rw-r--r--   0 runner    (1001) docker     (121)      624 2022-09-15 14:36:18.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/templates/package/read_base.html
--rw-r--r--   0 runner    (1001) docker     (121)     2884 2022-09-15 14:36:18.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/templates/package/search.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 14:38:23.004873 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/templates/snippets/
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-09-15 14:36:18.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/templates/snippets/add_dataset.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 14:38:23.004873 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-15 14:36:18.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3668 2022-09-15 14:36:18.000000 ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/tests/test_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 14:38:23.004873 ckanext-dcat_usmetadata-0.4.0/ckanext_dcat_usmetadata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    12105 2022-09-15 14:38:22.000000 ckanext-dcat_usmetadata-0.4.0/ckanext_dcat_usmetadata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    12632 2022-09-15 14:38:22.000000 ckanext-dcat_usmetadata-0.4.0/ckanext_dcat_usmetadata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-15 14:38:22.000000 ckanext-dcat_usmetadata-0.4.0/ckanext_dcat_usmetadata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-09-15 14:38:22.000000 ckanext-dcat_usmetadata-0.4.0/ckanext_dcat_usmetadata.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-09-15 14:38:22.000000 ckanext-dcat_usmetadata-0.4.0/ckanext_dcat_usmetadata.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-09-15 14:38:22.000000 ckanext-dcat_usmetadata-0.4.0/ckanext_dcat_usmetadata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      677 2022-09-15 14:36:18.000000 ckanext-dcat_usmetadata-0.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      763 2022-09-15 14:38:23.008873 ckanext-dcat_usmetadata-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3741 2022-09-15 14:38:22.000000 ckanext-dcat_usmetadata-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:55:07.236062 ckanext-dcat_usmetadata-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34499 2023-06-05 18:53:05.000000 ckanext-dcat_usmetadata-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-05 18:53:05.000000 ckanext-dcat_usmetadata-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9876 2023-06-05 18:55:07.236062 ckanext-dcat_usmetadata-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9359 2023-06-05 18:53:05.000000 ckanext-dcat_usmetadata-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:55:07.200062 ckanext-dcat_usmetadata-0.4.1/ckanext/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-05 18:53:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:55:07.200062 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 18:53:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-05 18:53:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-06-05 18:53:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-05 18:53:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/db_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:55:07.200062 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/fanstatic/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-05 18:53:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/fanstatic/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-05 18:53:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/fanstatic/webassets.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-05 18:53:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:55:07.196062 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:55:07.196062 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:55:07.232062 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/
+-rw-r--r--   0 runner    (1001) docker     (123)    25896 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Bitter-Bold.21c58d74.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    23344 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Bitter-Bold.9efe74f3.eot
+-rw-r--r--   0 runner    (1001) docker     (123)    15644 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Bitter-Bold.b786d169.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    11496 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Bitter-Bold.fc1844c7.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    25880 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Bitter-Italic.18853b8c.eot
+-rw-r--r--   0 runner    (1001) docker     (123)    39420 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Bitter-Italic.58093e86.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    14296 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Bitter-Italic.75fb25c1.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    20216 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Bitter-Italic.f09ccd61.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    33984 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Bitter-Regular.0078d318.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    24320 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Bitter-Regular.12b71a42.eot
+-rw-r--r--   0 runner    (1001) docker     (123)    22436 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Bitter-Regular.22c8272f.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    90628 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Bitter-Regular.c99f7ae5.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    21308 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-Bold.115f5a1d.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    47228 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-Bold.46eab112.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    26892 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-Bold.704b3917.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    19568 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-BoldItalic.2750a1e9.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    24464 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-BoldItalic.69debb55.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    40472 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-BoldItalic.9bce1501.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    19252 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-Italic.2412c72a.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    39480 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-Italic.3ee014ee.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    24152 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-Italic.b85b8ae5.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    21260 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-Light.4f0fb504.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    26988 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-Light.ddae281a.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    49164 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-Light.e6dc7e59.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    18976 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-LightItalic.08acae9c.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    23808 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-LightItalic.af8e7e14.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    39456 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-LightItalic.efbd9a2b.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    27512 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-Regular.73c28f4e.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    49484 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-Regular.efc70b44.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    21692 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-Regular.fa9b615a.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    11584 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Bold-webfont.3c4dc405.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    15440 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Bold-webfont.6a13b444.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    23602 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Bold-webfont.8bb31d27.eot
+-rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Bold-webfont.bf0b1c03.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    13048 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Italic-webfont.318b4f41.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    25792 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Italic-webfont.346b43cf.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    25978 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Italic-webfont.9487423d.eot
+-rw-r--r--   0 runner    (1001) docker     (123)    17204 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Italic-webfont.c0de58fc.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    22902 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Regular-webfont.33ec9bca.eot
+-rw-r--r--   0 runner    (1001) docker     (123)    15284 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Regular-webfont.467063b1.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    22712 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Regular-webfont.cb95bc69.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    11472 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Regular-webfont.e3b01381.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    23032 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Semibold-webfont.80744a04.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    15364 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Semibold-webfont.8e80acc0.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    11536 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Semibold-webfont.aebd17d5.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    23226 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Semibold-webfont.d543421f.eot
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/add.0e3e08bc.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/angle-arrow-down-primary.51295a10.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/angle-arrow-down.8e2c6296.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/angle-arrow-right.0f46e09b.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/angle-arrow-up-white.e60b3e19.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/angle-double-left-solid.a1c42657.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/angle-double-right-solid.9addc335.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/angle-left-solid.247b735a.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/angle-right-solid.fe82c509.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/arrow-both.0bfe2193.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/arrow-both.50893060.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/arrow-down-gray-60.9b52f832.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/arrow-down.6c056294.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/arrow-down.cb9919ed.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/arrow-left.ffd0d3ac.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/arrow-right.750bd27b.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/arrow-up.7fa2607f.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/calendar-alt-solid.95c20e20.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/check_circle.90deb06e.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/checkbox-check-print.fdb58020.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/checkmark-green.142e6c1d.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/chevron.f15c792a.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/close--primary-darker.05ee67ed.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/close--primary.c716dc4c.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/close-alt.659d1890.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/close-alt.8e9b0025.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/close-gray-60.7e82cc30.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/close.fe903f4b.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/correct8.1c696dec.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/correct9.1730d813.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/download.381b359a.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/error-white.6252fbdb.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/error.62d23dd4.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/error.e73ca64b.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/external-link-alt-hover.74ba81d1.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/external-link-alt.4b6aa08a.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/external-link-hover.73f16cba.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/external-link.18ea418e.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/facebook25.754f3a1c.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/file-excel.f208070c.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/file-pdf.080ccfc5.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/file-video.15c2687c.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/file-word.2fc990ab.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/file.eb89414b.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   689079 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/hero.544cee01.png
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/image.45732aef.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/info.157ac1b1.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/info.e24db876.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/information-new-hover.2d7be265.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/information-new.3ff7655b.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/information.61116626.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/loader.c04c3ed0.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/next.872082d4.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/pdf.f6d71f14.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/remove.d788b81e.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    32160 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-300.287fb5bc.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    19884 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-300.4f691391.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    16380 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-300.db95b37e.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    17340 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-300italic.18357dda.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    21052 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-300italic.8debb2d5.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    32596 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-300italic.c24ee49d.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    31092 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-700.0017dad2.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    15956 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-700.4bc0bd04.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    19564 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-700.f61e5a8d.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    32564 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-700italic.27139953.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    17336 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-700italic.5eca10b5.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    21132 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-700italic.7324e30e.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    17312 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-italic.55befc28.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    21096 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-italic.5711b84f.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    32336 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-italic.e3c56211.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    19576 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-regular.1db1469b.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    31052 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-regular.c03588a7.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    16028 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-regular.e92cc0fb.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/rss25.13c4042b.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/search--white.cebf50fe.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    26040 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-bold-webfont.738b5fd5.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    54340 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-bold-webfont.ab04959e.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    20368 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-bold-webfont.f12f6a2f.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    38760 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-bolditalic-webfont.00a1cd13.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    20164 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-bolditalic-webfont.60573f53.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    16416 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-bolditalic-webfont.dae8945d.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    20204 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-italic-webfont.12c96d9d.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    16372 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-italic-webfont.8740838d.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    38848 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-italic-webfont.bf26dc0f.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    20412 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-light-webfont.4572c51e.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    25956 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-light-webfont.9cf8ece9.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    54504 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-light-webfont.fb881861.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    39144 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-lightitalic-webfont.03f9a24f.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    20256 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-lightitalic-webfont.3fa6ebb8.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    16316 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-lightitalic-webfont.ffb6369e.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    26140 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-regular-webfont.34197df8.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    54432 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-regular-webfont.998d95f8.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    20540 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-regular-webfont.d67b548b.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/star-filled.b51af7f7.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/star.85ebfc24.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/success-fill.8a5df9fd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/success.7144d784.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/twitter16.60eb977c.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/warning.2e405b2b.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/warning.62d335b7.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/youtube15.9d356b3b.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:55:07.232062 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   434115 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/css/2.chunk.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7043 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/css/main.chunk.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:55:07.232062 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   482374 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/js/2.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (123)    82372 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/js/main.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-05 18:55:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/js/runtime-main.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:55:07.236062 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-05 18:53:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-05 18:53:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/templates/new-metadata.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:55:07.236062 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/templates/organization/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-05 18:53:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/templates/organization/read.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:55:07.236062 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/templates/package/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-05 18:53:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/templates/package/read_base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-05 18:53:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/templates/package/search.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:55:07.236062 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/templates/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-05 18:53:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/templates/snippets/add_dataset.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:55:07.236062 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 18:53:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-06-05 18:53:05.000000 ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/tests/test_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:55:07.236062 ckanext-dcat_usmetadata-0.4.1/ckanext_dcat_usmetadata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9876 2023-06-05 18:55:07.000000 ckanext-dcat_usmetadata-0.4.1/ckanext_dcat_usmetadata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12632 2023-06-05 18:55:07.000000 ckanext-dcat_usmetadata-0.4.1/ckanext_dcat_usmetadata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 18:55:07.000000 ckanext-dcat_usmetadata-0.4.1/ckanext_dcat_usmetadata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-05 18:55:07.000000 ckanext-dcat_usmetadata-0.4.1/ckanext_dcat_usmetadata.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-05 18:55:07.000000 ckanext-dcat_usmetadata-0.4.1/ckanext_dcat_usmetadata.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-05 18:55:07.000000 ckanext-dcat_usmetadata-0.4.1/ckanext_dcat_usmetadata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-05 18:53:05.000000 ckanext-dcat_usmetadata-0.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-05 18:55:07.236062 ckanext-dcat_usmetadata-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-06-05 18:55:06.000000 ckanext-dcat_usmetadata-0.4.1/setup.py
```

### Comparing `ckanext-dcat_usmetadata-0.4.0/LICENSE` & `ckanext-dcat_usmetadata-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/README.md` & `ckanext-dcat_usmetadata-0.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: ckanext-dcat_usmetadata
+Version: 0.4.1
+Summary: DCAT USMetadata Form App for CKAN
+Home-page: https://github.com/GSA/ckanext-dcat_usmetadata
+Author: Data.gov
+Author-email: datagovhelp@gsa.gov
+License: AGPL
+Keywords: CKAN
+Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![Github Actions](https://github.com/GSA/ckanext-dcat_usmetadata/actions/workflows/test.yml/badge.svg)](https://github.com/GSA/ckanext-dcat_usmetadata/actions)
 [![PyPI version](https://badge.fury.io/py/ckanext-dcat_usmetadata.svg)](https://badge.fury.io/py/ckanext-dcat_usmetadata)
 
 # ckanext-dcat_usmetadata
 
 This extension provides a new dataset form for [inventory.data.gov](https://inventory.data.gov/). The form is tailored to managing metadata meeting the [DCAT-US Schema](https://resources.data.gov/resources/dcat-us/).
 
@@ -99,20 +115,19 @@
 yarn up
 ```
 
 ## Testing
 
 There are several levels of testing:
 
-| Suite                     | Description                         | Command                  |
-| ------------------------- | ----------------------------------- | ------------------------ |
-| Unit tests for the JS app | Tests for the React app.            | `yarn test:metadata-app` |
-| CKAN extension tests      | Python tests using Nosetests        | `yarn test`              |
-| End to end tests          | Cypress tests against inventory app | `yarn e2e`               |
-| End to end tests (local)  | Cypress tests against inventory app | `yarn front-end`         |
+| Suite                     | Description                  | Command                  |
+| ------------------------- | ---------------------------- | ------------------------ |
+| Unit tests for the JS app | Tests for the React app.     | `yarn test:metadata-app` |
+| CKAN extension tests      | Python tests using Nosetests | `yarn test`              |
+| End to end tests          | Cypress tests                | `yarn e2e`               |
 
 ## Linting
 
 Lint the python code.
 
 ```bash
 yarn lint:python
@@ -158,29 +173,27 @@
 
 ```bash
 yarn test:metadata-app --updateSnapshot
 ```
 
 ## Local development and end-to-end testing
 
-We use the [inventory app](https://github.com/GSA/inventory-app) locally for development and end-to-end (e2e) testing.
-
 To build the latest JS code and update assets in the CKAN extension, you can run the following command from the root directory of this project:
 
 ```
 yarn build
 ```
 
 For convenience, we have prepared a single script that you can run to perform end-to-end tests locally. Don't forget to `yarn build` prior to running e2e tests, otherwise, the tests could run against older builds:
 
 ```bash
 yarn e2e
 ```
 
-Note, it may be necessary to remove cached images when rebuilding the inventory app docker container, in order to ensure that the new usmetadata-app template is included in the build. If you want to make sure that you aren't using cached builds, you can try:
+Note, it may be necessary to remove cached images when rebuilding the docker container, in order to ensure that the new usmetadata-app template is included in the build. If you want to make sure that you aren't using cached builds, you can try:
 
 ```bash
 docker-compose build --no-cache --pull ckanext-dcat_usmetadata_app
 ```
 
 To run e2e tests interactively use:
 
@@ -241,7 +254,9 @@
 Issues labeled [help wanted](https://github.com/GSA/data.gov/labels/help%20wanted) make it easy for you to find ways you can contribute today.
 
 ## Public Domain
 
 This project constitutes a work of the United States Government and is not subject to domestic copyright protection under 17 USC § 105. Additionally, we waive copyright and related rights in the work worldwide through the CC0 1.0 [Universal public domain dedication](https://creativecommons.org/publicdomain/zero/1.0/).
 
 All contributions to this project will be released under the CC0 dedication. By submitting a pull request, you are agreeing to comply with this waiver of copyright interest.
+
+
```

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/blueprint.py` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/blueprint.py`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/cli.py` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/cli.py`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/db_utils.py` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/db_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,10 +34,10 @@
                 "and package.id = package_extra.package_id " \
                 "and package.state = 'active' " \
                 "and package.owner_org in " + str(tuple(ids))
 
     connection = model.Session.connection()
     res = connection.execute(query).fetchall()
     for result in res:
-        items[result._row[0]] = result._row[1]
+        items[result[0]] = result[1]
 
     return items
```

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/plugin.py` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Bitter-Bold.21c58d74.ttf` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Bitter-Bold.21c58d74.ttf`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Bitter-Bold.9efe74f3.eot` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Bitter-Bold.9efe74f3.eot`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Bitter-Bold.b786d169.woff` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Bitter-Bold.b786d169.woff`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Bitter-Bold.fc1844c7.woff2` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Bitter-Bold.fc1844c7.woff2`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Bitter-Italic.18853b8c.eot` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Bitter-Italic.18853b8c.eot`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Bitter-Italic.58093e86.ttf` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Bitter-Italic.58093e86.ttf`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Bitter-Italic.75fb25c1.woff2` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Bitter-Italic.75fb25c1.woff2`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Bitter-Italic.f09ccd61.woff` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Bitter-Italic.f09ccd61.woff`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Bitter-Regular.0078d318.woff2` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Bitter-Regular.0078d318.woff2`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Bitter-Regular.12b71a42.eot` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Bitter-Regular.12b71a42.eot`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Bitter-Regular.22c8272f.woff` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Bitter-Regular.22c8272f.woff`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Bitter-Regular.c99f7ae5.ttf` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Bitter-Regular.c99f7ae5.ttf`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-Bold.115f5a1d.woff2` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-Bold.115f5a1d.woff2`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-Bold.46eab112.ttf` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-Bold.46eab112.ttf`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-Bold.704b3917.woff` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-Bold.704b3917.woff`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-BoldItalic.2750a1e9.woff2` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-BoldItalic.2750a1e9.woff2`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-BoldItalic.69debb55.woff` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-BoldItalic.69debb55.woff`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-BoldItalic.9bce1501.ttf` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-BoldItalic.9bce1501.ttf`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-Italic.2412c72a.woff2` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-Italic.2412c72a.woff2`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-Italic.3ee014ee.ttf` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-Italic.3ee014ee.ttf`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-Italic.b85b8ae5.woff` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-Italic.b85b8ae5.woff`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-Light.4f0fb504.woff2` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-Light.4f0fb504.woff2`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-Light.ddae281a.woff` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-Light.ddae281a.woff`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-Light.e6dc7e59.ttf` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-Light.e6dc7e59.ttf`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-LightItalic.08acae9c.woff2` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-LightItalic.08acae9c.woff2`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-LightItalic.af8e7e14.woff` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-LightItalic.af8e7e14.woff`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-LightItalic.efbd9a2b.ttf` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-LightItalic.efbd9a2b.ttf`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-Regular.73c28f4e.woff` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-Regular.73c28f4e.woff`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-Regular.efc70b44.ttf` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-Regular.efc70b44.ttf`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-Regular.fa9b615a.woff2` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/Latin-Merriweather-Regular.fa9b615a.woff2`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Bold-webfont.3c4dc405.woff2` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Bold-webfont.3c4dc405.woff2`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Bold-webfont.6a13b444.woff` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Bold-webfont.6a13b444.woff`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Bold-webfont.8bb31d27.eot` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Bold-webfont.8bb31d27.eot`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Bold-webfont.bf0b1c03.ttf` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Bold-webfont.bf0b1c03.ttf`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Italic-webfont.318b4f41.woff2` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Italic-webfont.318b4f41.woff2`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Italic-webfont.346b43cf.ttf` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Italic-webfont.346b43cf.ttf`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Italic-webfont.9487423d.eot` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Italic-webfont.9487423d.eot`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Italic-webfont.c0de58fc.woff` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Italic-webfont.c0de58fc.woff`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Regular-webfont.33ec9bca.eot` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Regular-webfont.33ec9bca.eot`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Regular-webfont.467063b1.woff` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Regular-webfont.467063b1.woff`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Regular-webfont.cb95bc69.ttf` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Regular-webfont.cb95bc69.ttf`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Regular-webfont.e3b01381.woff2` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Regular-webfont.e3b01381.woff2`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Semibold-webfont.80744a04.ttf` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Semibold-webfont.80744a04.ttf`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Semibold-webfont.8e80acc0.woff` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Semibold-webfont.8e80acc0.woff`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Semibold-webfont.aebd17d5.woff2` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Semibold-webfont.aebd17d5.woff2`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Semibold-webfont.d543421f.eot` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/OpenSans-Semibold-webfont.d543421f.eot`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/angle-arrow-down-primary.51295a10.svg` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/angle-arrow-down-primary.51295a10.svg`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/angle-arrow-down.8e2c6296.svg` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/angle-arrow-down.8e2c6296.svg`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/angle-arrow-right.0f46e09b.svg` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/angle-arrow-right.0f46e09b.svg`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/angle-arrow-up-white.e60b3e19.svg` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/angle-arrow-up-white.e60b3e19.svg`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/angle-double-left-solid.a1c42657.svg` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/angle-double-left-solid.a1c42657.svg`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/angle-double-right-solid.9addc335.svg` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/angle-double-right-solid.9addc335.svg`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/arrow-both.0bfe2193.svg` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/arrow-both.0bfe2193.svg`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/arrow-down-gray-60.9b52f832.svg` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/arrow-down-gray-60.9b52f832.svg`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/arrow-down.6c056294.svg` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/arrow-down.6c056294.svg`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/arrow-left.ffd0d3ac.svg` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/arrow-left.ffd0d3ac.svg`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/arrow-right.750bd27b.svg` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/arrow-right.750bd27b.svg`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/calendar-alt-solid.95c20e20.svg` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/calendar-alt-solid.95c20e20.svg`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/checkbox-check-print.fdb58020.svg` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/checkbox-check-print.fdb58020.svg`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/chevron.f15c792a.svg` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/chevron.f15c792a.svg`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/close--primary-darker.05ee67ed.svg` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/close--primary-darker.05ee67ed.svg`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/close--primary.c716dc4c.svg` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/close--primary.c716dc4c.svg`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/close.fe903f4b.svg` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/close.fe903f4b.svg`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/correct8.1c696dec.svg` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/correct8.1c696dec.svg`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/correct9.1730d813.svg` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/correct9.1730d813.svg`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/error.e73ca64b.svg` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/error.e73ca64b.svg`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/external-link-alt-hover.74ba81d1.svg` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/external-link-alt-hover.74ba81d1.svg`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/external-link-alt.4b6aa08a.svg` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/external-link-alt.4b6aa08a.svg`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/external-link-hover.73f16cba.svg` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/external-link-hover.73f16cba.svg`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/external-link.18ea418e.svg` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/external-link.18ea418e.svg`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/file-excel.f208070c.svg` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/file-excel.f208070c.svg`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/file-pdf.080ccfc5.svg` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/file-pdf.080ccfc5.svg`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/file-video.15c2687c.svg` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/file-video.15c2687c.svg`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/file-word.2fc990ab.svg` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/file-word.2fc990ab.svg`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/hero.544cee01.png` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/hero.544cee01.png`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/info.157ac1b1.svg` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/info.157ac1b1.svg`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/information.61116626.svg` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/information.61116626.svg`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/loader.c04c3ed0.svg` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/loader.c04c3ed0.svg`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/pdf.f6d71f14.svg` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/pdf.f6d71f14.svg`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-300.287fb5bc.ttf` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-300.287fb5bc.ttf`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-300.4f691391.woff` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-300.4f691391.woff`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-300.db95b37e.woff2` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-300.db95b37e.woff2`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-300italic.18357dda.woff2` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-300italic.18357dda.woff2`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-300italic.8debb2d5.woff` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-300italic.8debb2d5.woff`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-300italic.c24ee49d.ttf` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-300italic.c24ee49d.ttf`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-700.0017dad2.ttf` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-700.0017dad2.ttf`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-700.4bc0bd04.woff2` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-700.4bc0bd04.woff2`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-700.f61e5a8d.woff` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-700.f61e5a8d.woff`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-700italic.27139953.ttf` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-700italic.27139953.ttf`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-700italic.5eca10b5.woff2` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-700italic.5eca10b5.woff2`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-700italic.7324e30e.woff` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-700italic.7324e30e.woff`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-italic.55befc28.woff2` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-italic.55befc28.woff2`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-italic.5711b84f.woff` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-italic.5711b84f.woff`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-italic.e3c56211.ttf` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-italic.e3c56211.ttf`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-regular.1db1469b.woff` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-regular.1db1469b.woff`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-regular.c03588a7.ttf` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-regular.c03588a7.ttf`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-regular.e92cc0fb.woff2` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/roboto-mono-v5-latin-regular.e92cc0fb.woff2`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/rss25.13c4042b.svg` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/rss25.13c4042b.svg`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-bold-webfont.738b5fd5.woff` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-bold-webfont.738b5fd5.woff`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-bold-webfont.ab04959e.ttf` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-bold-webfont.ab04959e.ttf`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-bold-webfont.f12f6a2f.woff2` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-bold-webfont.f12f6a2f.woff2`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-bolditalic-webfont.00a1cd13.ttf` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-bolditalic-webfont.00a1cd13.ttf`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-bolditalic-webfont.60573f53.woff` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-bolditalic-webfont.60573f53.woff`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-bolditalic-webfont.dae8945d.woff2` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-bolditalic-webfont.dae8945d.woff2`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-italic-webfont.12c96d9d.woff` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-italic-webfont.12c96d9d.woff`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-italic-webfont.8740838d.woff2` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-italic-webfont.8740838d.woff2`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-italic-webfont.bf26dc0f.ttf` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-italic-webfont.bf26dc0f.ttf`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-light-webfont.4572c51e.woff2` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-light-webfont.4572c51e.woff2`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-light-webfont.9cf8ece9.woff` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-light-webfont.9cf8ece9.woff`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-light-webfont.fb881861.ttf` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-light-webfont.fb881861.ttf`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-lightitalic-webfont.03f9a24f.ttf` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-lightitalic-webfont.03f9a24f.ttf`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-lightitalic-webfont.3fa6ebb8.woff` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-lightitalic-webfont.3fa6ebb8.woff`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-lightitalic-webfont.ffb6369e.woff2` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-lightitalic-webfont.ffb6369e.woff2`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-regular-webfont.34197df8.woff` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-regular-webfont.34197df8.woff`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-regular-webfont.998d95f8.ttf` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-regular-webfont.998d95f8.ttf`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-regular-webfont.d67b548b.woff2` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/sourcesanspro-regular-webfont.d67b548b.woff2`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/success-fill.8a5df9fd.svg` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/success-fill.8a5df9fd.svg`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/success.7144d784.svg` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/success.7144d784.svg`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/twitter16.60eb977c.svg` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/twitter16.60eb977c.svg`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/warning.2e405b2b.svg` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/warning.2e405b2b.svg`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/assets/media/youtube15.9d356b3b.svg` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/assets/media/youtube15.9d356b3b.svg`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/css/2.chunk.css` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/css/2.chunk.css`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/css/main.chunk.css` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/css/main.chunk.css`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/js/2.chunk.js` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/js/2.chunk.js`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/js/main.chunk.js` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/js/main.chunk.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -31,17 +31,17 @@
                 n = t(149),
                 i = t.n(n),
                 s = (t(457), t(6)),
                 c = t.n(s),
                 o = t(15),
                 u = t(56),
                 d = t(7),
-                p = t(19),
-                m = t(87),
-                v = t.n(m),
+                m = t(19),
+                p = t(87),
+                v = t.n(p),
                 b = t(259),
                 g = t(252),
                 f = function(e) {
                     var a = e.children,
                         t = Object(l.useRef)(null),
                         n = Object(l.useRef)(null),
                         i = Object(l.useState)(!1),
@@ -100,18 +100,18 @@
                         n = e.children,
                         i = e.helptext,
                         s = (e.required, e.id),
                         c = e.errors,
                         o = e.disabled,
                         u = e.infoText,
                         d = e.onClick,
-                        m = (e.onSelect, Object(b.a)(e, ["value", "name", "label", "children", "helptext", "required", "id", "errors", "disabled", "infoText", "onClick", "onSelect"])),
+                        p = (e.onSelect, Object(b.a)(e, ["value", "name", "label", "children", "helptext", "required", "id", "errors", "disabled", "infoText", "onClick", "onSelect"])),
                         v = c || {},
-                        g = m.choices || [],
-                        h = m.type || "string",
+                        g = p.choices || [],
+                        h = p.type || "string",
                         y = "";
                     return y = o ? "disabled" : "", r.a.createElement("div", {
                         className: "wrapper"
                     }, r.a.createElement("label", {
                         className: "usa-label",
                         htmlFor: s
                     }, l, u && r.a.createElement(f, null, r.a.createElement("h3", null, l), r.a.createElement("p", null, u))), v[t] && r.a.createElement("span", {
@@ -120,27 +120,27 @@
                         className: "usa-helptext ".concat(y)
                     }, i), d ? r.a.createElement("button", {
                         className: "clear-button usa-button usa-button--secondary",
                         onClick: d,
                         type: "button"
                     }, "Remove") : "", {
                         label: r.a.createElement("div", null, a),
-                        string: r.a.createElement(p.a, Object.assign({
+                        string: r.a.createElement(m.a, Object.assign({
                             className: "usa-input ".concat(y, " ") + "".concat(v[t] && "field-error", " ") + "".concat(d && "has-clear-button"),
                             disabled: o,
                             id: s,
                             name: t
-                        }, m)),
-                        url: r.a.createElement(p.a, Object.assign({
+                        }, p)),
+                        url: r.a.createElement(m.a, Object.assign({
                             className: "usa-input ".concat(y, " ").concat((v[t] || v.resource) && "field-error", " ").concat(d && "has-clear-button"),
                             disabled: o,
                             id: s,
                             name: t
-                        }, m)),
-                        select: r.a.createElement(p.a, Object.assign({}, m, {
+                        }, p)),
+                        select: r.a.createElement(m.a, Object.assign({}, p, {
                             as: "select",
                             id: s,
                             name: t,
                             disabled: o,
                             className: "usa-select ".concat(y, " ").concat(v[t] ? "field-error" : ""),
                             component: "select"
                         }), r.a.createElement("option", {
@@ -149,24 +149,24 @@
                             var t = e.value || e.id || e,
                                 l = e.label || e.title || e.name || e;
                             return r.a.createElement("option", {
                                 value: t,
                                 key: t + a
                             }, l)
                         }))),
-                        radio: r.a.createElement("div", null, r.a.createElement(p.a, Object.assign({}, m, {
+                        radio: r.a.createElement("div", null, r.a.createElement(m.a, Object.assign({}, p, {
                             id: s,
                             name: t,
                             className: "usa-radio__input",
                             component: "radio"
                         })), r.a.createElement("label", {
                             className: "usa-radio__label",
                             htmlFor: s
                         }, l)),
-                        date: r.a.createElement("div", null, r.a.createElement(p.a, {
+                        date: r.a.createElement("div", null, r.a.createElement(m.a, {
                             type: "date",
                             id: s,
                             name: t,
                             className: "usa-input ".concat(y),
                             disabled: o
                         }))
                     } [h], n)
@@ -265,25 +265,25 @@
                     } else e.spatial_location_desc && (a.spatial = e.spatial_location_desc, delete a.spatial_location_desc);
                     if ("true" === e.temporal) {
                         var u = C(e.temporal_start_date),
                             d = C(e.temporal_end_date);
                         a.temporal = "".concat(u, "/").concat(d), delete a.temporal_start_date, delete a.temporal_end_date
                     } else {
                         delete a.temporal, delete a.temporal_start_date, delete a.temporal_end_date;
-                        var p = a.extras.findIndex((function(e) {
+                        var m = a.extras.findIndex((function(e) {
                             return "temporal" === e.key
                         }));
-                        p > -1 && a.extras.splice(p, 1)
+                        m > -1 && a.extras.splice(m, 1)
                     }
                     if (e.dataQuality) {
                         a.data_quality = "Yes" === e.dataQuality;
-                        var m = a.extras.findIndex((function(e) {
+                        var p = a.extras.findIndex((function(e) {
                             return "data_quality" === e.key
                         }));
-                        m > -1 && (a.extras[m].value = a.data_quality)
+                        p > -1 && (a.extras[p].value = a.data_quality)
                     }
                     var v = a.extras.findIndex((function(e) {
                         return "category" === e.key
                     }));
                     e.category ? v > -1 && (a.extras[v].value = e.category) : v > -1 && a.extras.splice(v, 1);
                     var b = a.extras.findIndex((function(e) {
                         return "data_dictionary" === e.key
@@ -385,40 +385,40 @@
                     var i = {};
                     return (e.extras || []).map((function(e) {
                         var a = e.key,
                             t = e.value;
                         k.includes(a) && (i[a] = t)
                     })), a.publisher = T(i), a
                 },
-                B = function(e) {
+                G = function(e) {
                     for (var a = I(e), t = [], l = ["publisher", "contact_name", "contact_email", "unique_id", "modified", "public_access_level", "bureau_code", "program_code", "release_date", "accrual_periodicity", "language", "data_quality", "publishing_status", "is_parent", "parent_dataset", "category", "related_documents", "conforms_to", "homepage_url", "system_of_records", "primary_it_investment_uii", "publisher_1", "publisher_2", "publisher_3", "publisher_4", "publisher_5"], r = 0; r < l.length; r += 1) l[r] in e && (t.push({
                         key: l[r],
                         value: e[l[r]]
                     }), delete a[l[r]]);
                     for (var n = {}, i = 0; i < t.length; i += 1) n[t[i].key] = t[i].value;
                     return a.common_core = n, a.extras = t, a
                 },
-                G = {
+                B = {
                     createDataset: function(e, a, t) {
                         var l = L(e);
                         return l.name = e.url ? e.url.split("/").pop() : v()(e.title, {
                             lower: !0,
                             remove: /[*+~.()'"!:@]/g
-                        }), l.notes = l.notes || "", delete l.url, l.bureau_code = "015:11", l.program_code = "015:001", _.a.post("".concat(a, "package_create"), R(B(l)), {
+                        }), l.notes = l.notes || "", delete l.url, l.bureau_code = "015:11", l.program_code = "015:001", _.a.post("".concat(a, "package_create"), R(G(l)), {
                             headers: {
                                 "X-CKAN-API-Key": t
                             }
                         }).then((function(e) {
                             var a = e.data.result;
                             return U(F(a))
                         }))
                     },
                     updateDataset: function(e, a, t, l) {
                         var r = L(a);
-                        return r.id = e, r.name = a.url ? a.url.split("/").pop() : r.name, delete r.url, r.bureau_code = "015:11", r.program_code = "015:001", _.a.post("".concat(t, "package_update"), R(B(r)), {
+                        return r.id = e, r.name = a.url ? a.url.split("/").pop() : r.name, delete r.url, r.bureau_code = "015:11", r.program_code = "015:001", _.a.post("".concat(t, "package_update"), R(G(r)), {
                             headers: {
                                 "X-CKAN-API-Key": l
                             }
                         }).then((function(e) {
                             var a = e.data.result;
                             return U(F(a))
                         }))
@@ -652,30 +652,30 @@
                 z = (t(480), function(e) {
                     var a = e.tags,
                         t = e.name,
                         n = e.helptext,
                         i = e.placeholder,
                         s = e.apiUrl,
                         u = e.apiKey,
-                        m = e.errors,
+                        p = e.errors,
                         v = e.fetchOpts,
                         b = e.type,
                         g = Object(l.useState)([]),
                         f = Object(d.a)(g, 2),
                         h = f[0],
                         y = f[1],
-                        E = Object(p.e)(t),
+                        E = Object(m.e)(t),
                         _ = Object(d.a)(E, 3),
                         x = (_[0], _[1], _[2].setValue);
                     if ("string" === b) {
                         var S = e.value ? [{
                             name: e.value
                         }] : [];
                         return r.a.createElement("div", {
-                            className: "react-tags-input grid-col-12 ".concat(m && m[t] && "field-error")
+                            className: "react-tags-input grid-col-12 ".concat(p && p[t] && "field-error")
                         }, r.a.createElement("div", {
                             className: "usa-helptext"
                         }, n), r.a.createElement(K.a, {
                             tags: S,
                             suggestions: h,
                             allowNew: !0,
                             addOnBlur: !0,
@@ -710,22 +710,22 @@
                                 })));
                                 return function(a) {
                                     return e.apply(this, arguments)
                                 }
                             }()
                         }))
                     }
-                    return r.a.createElement(p.b, {
+                    return r.a.createElement(m.b, {
                         name: t,
                         render: function(e) {
                             return r.a.createElement("div", {
-                                className: "react-tags-input grid-col-12 ".concat(m && m[t] && "field-error")
-                            }, m && m[t] && r.a.createElement("span", {
+                                className: "react-tags-input grid-col-12 ".concat(p && p[t] && "field-error")
+                            }, p && p[t] && r.a.createElement("span", {
                                 className: "error-msg"
-                            }, "String" === m[t].constructor.name ? m[t] : JSON.stringify(m[t]), r.a.createElement("br", null)), n, r.a.createElement(K.a, {
+                            }, "String" === p[t].constructor.name ? p[t] : JSON.stringify(p[t]), r.a.createElement("br", null)), n, r.a.createElement(K.a, {
                                 tags: a,
                                 suggestions: h,
                                 allowNew: !0,
                                 addOnBlur: !0,
                                 ref: r.a.createRef(),
                                 onAddition: e.push,
                                 onDelete: e.remove,
@@ -773,26 +773,26 @@
                 W = function(e) {
                     var a = e.name,
                         t = e.helptext,
                         n = e.inputValue,
                         i = e.value,
                         s = e.placeholder,
                         u = e.apiUrl,
-                        m = e.apiKey,
+                        p = e.apiKey,
                         v = e.errors,
                         b = e.fetchOpts,
                         g = Object(l.useState)([]),
                         f = Object(d.a)(g, 2),
                         h = f[0],
                         y = f[1],
                         E = Object(l.useState)(null),
                         _ = Object(d.a)(E, 2),
                         x = _[0],
                         S = _[1],
-                        w = Object(p.e)(a),
+                        w = Object(m.e)(a),
                         N = Object(d.a)(w, 3),
                         O = (N[0], N[1], N[2].setValue),
                         D = Object(l.useState)(""),
                         P = Object(d.a)(D, 2),
                         k = P[0],
                         T = P[1];
                     Object(l.useEffect)((function() {
@@ -809,15 +809,15 @@
                                         case 0:
                                             if (t = (a || "").trim().toLowerCase(), 0 !== (l = t.length)) {
                                                 e.next = 4;
                                                 break
                                             }
                                             return e.abrupt("return", []);
                                         case 4:
-                                            return e.prev = 4, e.next = 7, b(t, u, m);
+                                            return e.prev = 4, e.next = 7, b(t, u, p);
                                         case 7:
                                             return e.abrupt("return", e.sent.filter((function(e) {
                                                 return e.name.toLowerCase().slice(0, l) === t
                                             })));
                                         case 10:
                                             return e.prev = 10, e.t0 = e.catch(4), console.warn("Unable to fetch autocomplete options", e.t0), e.abrupt("return", []);
                                         case 14:
@@ -906,15 +906,15 @@
                     var a = e.label,
                         t = e.value,
                         l = e.styleClass,
                         n = e.id,
                         i = e.name;
                     return r.a.createElement("div", {
                         className: "form-group ".concat(l)
-                    }, r.a.createElement(p.a, {
+                    }, r.a.createElement(m.a, {
                         type: "radio",
                         className: "usa-radio__input",
                         value: t,
                         name: i,
                         id: n
                     }), r.a.createElement("label", {
                         className: "usa-radio__label",
@@ -946,26 +946,26 @@
                 te = function(e) {
                     var a = e.values,
                         t = e.errors,
                         n = e.apiUrl,
                         i = e.apiKey,
                         s = e.draftSaved,
                         u = e.setFieldValue,
-                        p = e.submitForm,
-                        m = e.handleChange,
+                        m = e.submitForm,
+                        p = e.handleChange,
                         b = Object(l.useState)([]),
                         g = Object(d.a)(b, 2),
                         y = g[0],
                         E = g[1],
                         _ = Object(l.useState)([]),
                         x = Object(d.a)(_, 2),
                         S = x[0],
                         w = x[1];
                     Object(l.useEffect)((function() {
-                        G.fetchOrganizationsForUser(n, i).then((function(e) {
+                        B.fetchOrganizationsForUser(n, i).then((function(e) {
                             var a = new URLSearchParams(window.location.search).get("group");
                             a && u("owner_org", a), 1 === e.length && u("owner_org", e[0].id), E(e)
                         }))
                     }), []);
                     var N = Object(l.useState)(!0),
                         O = Object(d.a)(N, 2),
                         D = O[0],
@@ -982,15 +982,15 @@
                         },
                         C = function() {
                             var e = Object(o.a)(c.a.mark((function e() {
                                 var t;
                                 return c.a.wrap((function(e) {
                                     for (;;) switch (e.prev = e.next) {
                                         case 0:
-                                            return e.next = 2, G.fetchPublishers(a.owner_org, n, i);
+                                            return e.next = 2, B.fetchPublishers(a.owner_org, n, i);
                                         case 2:
                                             return t = e.sent, w(t), e.abrupt("return", t);
                                         case 5:
                                         case "end":
                                             return e.stop()
                                     }
                                 }), e)
@@ -1087,15 +1087,15 @@
                     }, r.a.createElement("span", {
                         className: "usa-label"
                     }, "Tags"), r.a.createElement(z, {
                         id: "tags-autocomplete-input",
                         tags: a.tags,
                         apiUrl: n,
                         apiKey: i,
-                        fetchOpts: G.fetchTags,
+                        fetchOpts: B.fetchTags,
                         name: "tags",
                         titleField: "name",
                         required: !0,
                         placeholder: "Start typing to search",
                         errors: t,
                         helptext: k("Use both technical and non-technical terms to help users find your dataset. Press tab or enter to add each new tag.")
                     })), r.a.createElement("div", {
@@ -1103,15 +1103,15 @@
                     }, r.a.createElement(h, {
                         label: "Organization",
                         name: "owner_org",
                         type: "select",
                         value: a.owner_org,
                         choices: y,
                         onChange: function(e) {
-                            m(e), u("publisher", ""), u("selectedPublisher", null)
+                            p(e), u("publisher", ""), u("selectedPublisher", null)
                         },
                         required: !0,
                         className: "error-msg",
                         errors: t
                     })), r.a.createElement("div", {
                         className: "grid-row margin-top-3"
                     }, r.a.createElement("div", {
@@ -1295,15 +1295,15 @@
                         type: "button",
                         onClick: Object(o.a)(c.a.mark((function e() {
                             return c.a.wrap((function(e) {
                                 for (;;) switch (e.prev = e.next) {
                                     case 0:
                                         return e.next = 2, u("saveDraft", !0);
                                     case 2:
-                                        p();
+                                        m();
                                     case 3:
                                     case "end":
                                         return e.stop()
                                 }
                             }), e)
                         })))
                     }, "Save draft"), r.a.createElement("button", {
@@ -1311,15 +1311,15 @@
                         type: "button",
                         onClick: Object(o.a)(c.a.mark((function e() {
                             return c.a.wrap((function(e) {
                                 for (;;) switch (e.prev = e.next) {
                                     case 0:
                                         return e.next = 2, u("saveDraft", !1);
                                     case 2:
-                                        p();
+                                        m();
                                     case 3:
                                     case "end":
                                         return e.stop()
                                 }
                             }), e)
                         })))
                     }, "Save and Continue")), s && r.a.createElement("div", {
@@ -1440,23 +1440,23 @@
                     references: r.a.createElement(Z, null, "Related documents such as technical information about a dataset, developer documentation, etc. Format for entry is: https://www.agency.gov/fruits/fruits.csv, https://www.agency.gov/legumes/legumes"),
                     systemOfRecordsUSG: r.a.createElement(Z, null, "If the dataset is a designated System of Records under the Privacy Act of 1974, provide the URL for the System of Records Notice"),
                     accrualPeriodicity: r.a.createElement(Z, null, "If you selected \u201cOther, please specify a valid", " ", r.a.createElement(ee, {
                         target: "_blank",
                         href: "https://en.wikipedia.org/wiki/ISO_8601"
                     }, "ISO 8601"), " ", "timestamp")
                 },
-                pe = function(e) {
+                me = function(e) {
                     var a, t = e.values,
                         l = e.apiUrl,
                         n = e.errors,
                         i = e.apiKey,
                         s = e.draftSaved,
                         u = e.setFieldValue,
                         d = e.submitForm,
-                        p = e.handleSteps;
+                        m = e.handleSteps;
                     return r.a.createElement("div", {
                         className: "usa-form-custom"
                     }, r.a.createElement("section", {
                         id: "section-basic-mega-menu",
                         className: "site-component-section"
                     }, r.a.createElement("p", {
                         className: "site-text-intro"
@@ -1624,15 +1624,15 @@
                         label: "Select Parent Dataset",
                         name: "parentDataset",
                         type: "string",
                         value: t.parentDataset,
                         inputValue: t.parentDatasetTitle,
                         placeholder: "Select parent dataset",
                         helptext: "Start typing to see list of matching datasets by title",
-                        fetchOpts: G.fetchParentDatasets,
+                        fetchOpts: B.fetchParentDatasets,
                         apiUrl: l,
                         apiKey: i
                     }))), r.a.createElement("div", {
                         className: "margin-top-6 clearfix"
                     }, "Published" === t.publishing_status ? "" : r.a.createElement("button", {
                         className: "usa-button usa-button--outline",
                         type: "button",
@@ -1651,18 +1651,18 @@
                         })))
                     }, "Save draft"), r.a.createElement("div", {
                         className: "float-right"
                     }, r.a.createElement("button", {
                         className: "usa-button usa-button--outline",
                         type: "button",
                         onClick: function() {
-                            return p(0)
+                            return m(0)
                         },
                         onKeyUp: function(e) {
-                            13 === e.keyCode && p(0)
+                            13 === e.keyCode && m(0)
                         }
                     }, "Back to previous page"), r.a.createElement("button", {
                         className: "usa-button margin-right-0",
                         type: "button",
                         onClick: Object(o.a)(c.a.mark((function e() {
                             return c.a.wrap((function(e) {
                                 for (;;) switch (e.prev = e.next) {
@@ -1680,69 +1680,76 @@
                         style: {
                             marginTop: "1rem"
                         }
                     }, r.a.createElement("div", {
                         className: "col-md-12 text-mint"
                     }, r.a.createElement("i", null, "Draft saved:", r.a.createElement("br", null), "[", s, "]"))))
                 },
-                me = /^P(?:(\d+(?:[\.,]\d+)?)Y)?(?:(\d+(?:[\.,]\d+)?)M)?(?:(\d+(?:[\.,]\d+)?)D)?(?:T(?:(\d+(?:[\.,]\d+)?)H)?(?:(\d+(?:[\.,]\d+)?)M)?(?:(\d+(?:[\.,]\d+)?)S)?)?$/,
+                pe = /^P(?:(\d+(?:[\.,]\d+)?)Y)?(?:(\d+(?:[\.,]\d+)?)M)?(?:(\d+(?:[\.,]\d+)?)D)?(?:T(?:(\d+(?:[\.,]\d+)?)H)?(?:(\d+(?:[\.,]\d+)?)M)?(?:(\d+(?:[\.,]\d+)?)S)?)?$/,
                 ve = le.e().shape({
                     dataQuality: le.f(),
                     category: le.f(),
                     data_dictionary: le.f().url(),
                     data_dictionary_type: le.f(),
                     primary_it_investment_uii: le.f().trim().matches(/^[0-9]{3}-[0-9]{9}$/, "uii should match format: 000-000000000"),
                     homepage_url: le.f().url(),
                     related_documents: le.f(),
                     deribed_by: le.f().url(),
                     described_by_type: le.f(),
                     system_of_records: le.f(),
                     release_date: le.c().typeError("Please specify a valid release date"),
                     accrualPeriodicityOther: le.f().test("accrual-periodicity-other", "Data Publishing Frequency should be formatted as a proper ISO 8601 timestamp", (function(e) {
-                        return e && me.test(e.replace("R/", ""))
+                        return e && pe.test(e.replace("R/", ""))
                     })).when("accrualPeriodicity", (function(e, a) {
                         return "other" === e ? a : le.f()
                     }))
                 }),
                 be = t(600),
                 ge = t(257),
                 fe = (t(591), ge.sort((function(e, a) {
                     var t = e.label.toUpperCase(),
                         l = a.label.toUpperCase();
                     return t < l ? -1 : t > l ? 1 : 0
                 }))),
-                he = function(e) {
+                he = {
+                    conformsTo: r.a.createElement(Z, null, "Refer to documentation here for", " ", r.a.createElement(ee, {
+                        target: "_blank",
+                        href: "https://github.com/GSA/ckanext-datajson/tree/main/ckanext/datajson/tests/datajson-samples#datajson-examples"
+                    }, "geospatial datasets"), " ")
+                },
+                ye = function(e) {
                     var a = e.values,
                         t = e.errors,
                         n = e.setFieldValue,
                         i = e.submitForm,
                         s = e.draftSaved,
                         u = e.isSubmitting,
-                        p = e.handleSteps,
-                        m = a.resourceAction,
+                        m = e.handleSteps,
+                        p = a.resourceAction,
                         v = a.resource || {},
                         b = a.resources || [],
                         g = v.url,
                         f = v.name,
                         y = v.description,
                         E = v.mimetype,
-                        _ = v.format,
-                        x = Object(l.useState)(!1),
-                        S = Object(d.a)(x, 2),
-                        w = S[0],
-                        k = S[1],
-                        T = Object(l.useState)(!1),
-                        I = Object(d.a)(T, 2),
-                        C = I[0],
-                        A = I[1];
+                        _ = v.conformsTo,
+                        x = v.format,
+                        S = Object(l.useState)(!1),
+                        w = Object(d.a)(S, 2),
+                        k = w[0],
+                        T = w[1],
+                        I = Object(l.useState)(!1),
+                        C = Object(d.a)(I, 2),
+                        A = C[0],
+                        F = C[1];
                     Object(l.useEffect)((function() {
                         v.format || v.urlType !== D || n("resource.format", "API")
                     }), [v.urlType]);
-                    var F = function() {
-                        A(!1)
+                    var R = function() {
+                        F(!1)
                     };
                     return r.a.createElement("div", {
                         className: "usa-form-custom",
                         id: "resource-upload"
                     }, r.a.createElement("section", {
                         id: "section-basic-mega-menu",
                         className: "site-component-section"
@@ -1767,52 +1774,52 @@
                         }, r.a.createElement("div", {
                             className: "grid-col-12 bg-base-lightest padding-x-1"
                         }, r.a.createElement("div", {
                             className: "resource-item-name"
                         }, e.name), r.a.createElement("button", {
                             id: "delete-".concat(e.name),
                             onClick: function() {
-                                return a = e.name, void A(a);
+                                return a = e.name, void F(a);
                                 var a
                             },
                             type: "button",
                             className: "usa-button--unstyled resource-action-button"
-                        }, "Delete"), C === e.name && r.a.createElement(be.a, {
+                        }, "Delete"), A === e.name && r.a.createElement(be.a, {
                             onExit: function() {
-                                return F()
+                                return R()
                             },
                             getApplicationNode: function() {
                                 return document.getElementById("resource-upload")
                             },
                             heading: "Please Confirm Action",
                             underlayClickExits: !0,
                             actions: [r.a.createElement("button", {
                                 type: "button",
                                 className: "ds-c-button ds-c-button--primary",
                                 key: "primary",
                                 onClick: function() {
                                     ! function(e) {
                                         n("resource", {
                                             id: e.id
-                                        }), n("resourceAction", "delete"), n("publish", !1), n("saveDraft", !1), k(!1), i()
-                                    }(e), F()
+                                        }), n("resourceAction", "delete"), n("publish", !1), n("saveDraft", !1), T(!1), i()
+                                    }(e), R()
                                 }
                             }, "Delete"), r.a.createElement("button", {
                                 type: "button",
                                 className: "ds-c-button ds-c-button--transparent",
                                 key: "cancel",
                                 onClick: function() {
-                                    return F()
+                                    return R()
                                 }
                             }, "Cancel")]
                         }, "Are you sure you want to delete this resource?"), r.a.createElement("button", {
                             id: "edit-".concat(e.name),
                             onClick: function() {
                                 ! function(e) {
-                                    n("resourceAction", "edit"), k(!1), n("resource", e), n("resource.size", ""), n("resource.webstore_last_updated", ""), n("resource.cache_last_updated", "")
+                                    n("resourceAction", "edit"), T(!1), n("resource", e), n("resource.size", ""), n("resource.webstore_last_updated", ""), n("resource.cache_last_updated", "")
                                 }(e)
                             },
                             type: "button",
                             className: "usa-button--unstyled resource-action-button"
                         }, "Edit")))
                     }))) : "", r.a.createElement("div", {
                         className: "grid-row margin-top-3"
@@ -1851,34 +1858,34 @@
                         name: "resource.url",
                         type: "url",
                         value: g,
                         onClick: function() {
                             n("resource.url", "")
                         },
                         errors: t
-                    })) : w ? r.a.createElement(h, {
+                    })) : k ? r.a.createElement(h, {
                         name: "resource.fileName",
                         type: "label",
                         value: v.fileName,
                         onClick: function() {
-                            n("resource.upload", null), n("resource.fileName", ""), n("resource.name", ""), n("resource.description", ""), n("resource.format", ""), n("resource.mimetype", ""), k(!1)
+                            n("resource.upload", null), n("resource.fileName", ""), n("resource.name", ""), n("resource.description", ""), n("resource.mimetype", ""), n("resource.conformsTo", ""), n("resource.format", ""), T(!1)
                         }
                     }) : v.urlType === O && r.a.createElement(r.a.Fragment, null, r.a.createElement("br", null), r.a.createElement("label", {
                         tabIndex: "0",
                         htmlFor: "upload",
                         className: "usa-button usa-button--base"
                     }, r.a.createElement("i", {
                         className: "fa fa-cloud-upload",
                         "aria-hidden": "true"
                     }), " Upload data"), r.a.createElement("input", {
                         id: "upload",
                         name: "resource.upload",
                         type: "file",
                         onChange: function(e) {
-                            if (k(!w), n("resource.fileName", e.currentTarget.files[0].name), f || n("resource.name", e.currentTarget.files[0].name), E || n("resource.mimetype", e.currentTarget.files[0].type), !_) {
+                            if (T(!k), n("resource.fileName", e.currentTarget.files[0].name), f || n("resource.name", e.currentTarget.files[0].name), E || n("resource.mimetype", e.currentTarget.files[0].type), !x) {
                                 var a = e.currentTarget.files[0].name && e.currentTarget.files[0].name.split(".").slice(-1)[0];
                                 n("resource.format", a || "")
                             }
                             n("resource.upload", e.currentTarget.files[0])
                         }
                     }), r.a.createElement("p", {
                         className: "usa-helptext"
@@ -1916,31 +1923,42 @@
                         choices: fe,
                         value: E
                     }))), r.a.createElement("div", {
                         className: "grid-row margin-top-3"
                     }, r.a.createElement("div", {
                         className: "grid-col-12"
                     }, r.a.createElement(h, {
+                        label: "Conforms To",
+                        name: "resource.conformsTo",
+                        type: "string",
+                        helptext: "Please ensure this is a resolvable URL.",
+                        infoText: he.conformsTo,
+                        value: _
+                    }))), r.a.createElement("div", {
+                        className: "grid-row margin-top-3"
+                    }, r.a.createElement("div", {
+                        className: "grid-col-12"
+                    }, r.a.createElement(h, {
                         label: "Format",
                         name: "resource.format",
                         type: "string",
                         helptext: "Examples include: csv, xml, json.  This will be guessed automatically.  Leave blank if you wish.",
-                        value: _
+                        value: x
                     }))), r.a.createElement("div", {
                         className: "grid-row margin-top-3"
                     }, r.a.createElement("div", {
                         className: "grid-col-12"
                     }, r.a.createElement("button", {
                         type: "button",
                         className: "usa-button usa-button--outline",
                         onClick: function() {
-                            n("publish", !1), n("saveDraft", !1), k(!1), i()
+                            n("publish", !1), n("saveDraft", !1), T(!1), i()
                         },
                         disabled: u
-                    }, "edit" === m ? "Save" : "Save and add another resource"))), a.lastSavedResource && b.length ? r.a.createElement("div", {
+                    }, "edit" === p ? "Save" : "Save and add another resource"))), a.lastSavedResource && b.length ? r.a.createElement("div", {
                         className: "grid-row margin-top-3"
                     }, r.a.createElement("div", {
                         className: "grid-col-12"
                     }, r.a.createElement("div", {
                         className: "usa-alert usa-alert--success usa-alert--slim usa-alert--no-icon"
                     }, r.a.createElement("div", {
                         className: "usa-alert__body"
@@ -1974,18 +1992,18 @@
                         })))
                     }, "Save draft"), r.a.createElement("div", {
                         className: "float-right"
                     }, r.a.createElement("button", {
                         className: "usa-button usa-button--outline",
                         type: "button",
                         onClick: function() {
-                            return p(1)
+                            return m(1)
                         },
                         onKeyUp: function(e) {
-                            13 === e.keyCode && p(1)
+                            13 === e.keyCode && m(1)
                         }
                     }, "Back to previous page"), r.a.createElement("button", {
                         className: "usa-button margin-right-0",
                         type: "button",
                         onClick: function() {
                             n("publish", !0), i()
                         },
@@ -1994,33 +2012,34 @@
                         style: {
                             marginTop: "1rem"
                         }
                     }, r.a.createElement("div", {
                         className: "grid-col-12 text-custom-green"
                     }, r.a.createElement("i", null, "Draft saved:", r.a.createElement("br", null), "[", s, "]"))))
                 },
-                ye = le.e().shape({
+                Ee = le.e().shape({
                     resource: le.e().shape({
                         name: le.f(),
                         description: le.f(),
                         mimetype: le.f(),
                         format: le.f(),
                         url: le.f().url('If you are linking to a dataset, please include "https://" at the beginning of your URL.'),
                         upload: le.d()
                     })
                 }),
-                Ee = {
+                _e = {
                     name: "",
                     description: "",
                     url: "",
                     format: "",
                     mimetype: "",
+                    conformsTo: "",
                     upload: null
                 },
-                _e = function(e) {
+                xe = function(e) {
                     var a = e.currentStep,
                         t = e.handleSteps;
                     return r.a.createElement("div", {
                         className: "app_navigation",
                         id: "app_navigation"
                     }, r.a.createElement("div", {
                         tabIndex: "0",
@@ -2051,15 +2070,15 @@
                             13 === e.keyCode && t(2)
                         },
                         onClick: function() {
                             t(2)
                         }
                     }, r.a.createElement("span", null, "Resource Upload")))
                 },
-                xe = function(e) {
+                Se = function(e) {
                     Object(l.useEffect)((function() {
                         window.scrollTo(0, 0)
                     }), []);
                     var a = e.type,
                         t = e.errors,
                         n = e.message,
                         i = e.heading,
@@ -2097,45 +2116,45 @@
                         className: "usa-alert__text"
                     }, "string" === typeof n && n, "object" === typeof n && n.map((function(e) {
                         return r.a.createElement("p", {
                             key: e
                         }, e)
                     })), c)))))
                 },
-                Se = (t(597), function(e) {
+                we = (t(597), function(e) {
                     return Object.keys(e).map((function(a) {
                         return {
                             name: a,
                             label: ne[a],
                             message: e[a]
                         }
                     }))
                 }),
-                we = function(e) {
+                Ne = function(e) {
                     return "".concat(["0".concat(e.getHours()).slice(-2), "0".concat(e.getMinutes()).slice(-2)].join(":"), ", ").concat(["0".concat(e.getMonth() + 1).slice(-2), "0".concat(e.getDate()).slice(-2), e.getFullYear().toString().slice(-2)].join("-"))
                 },
-                Ne = function(e) {
+                Oe = function(e) {
                     var a = e.currentStep;
                     return 0 === a ? r.a.createElement("h1", {
                         className: "usite-page-title",
                         id: "basic-mega-menu"
                     }, "Required Metadata") : 1 === a ? r.a.createElement("h1", {
                         className: "usite-page-title",
                         id: "basic-mega-menu"
                     }, "Additional Metadata") : ""
                 },
-                Oe = function(e) {
+                De = function(e) {
                     var a = e.apiUrl,
                         t = e.apiKey,
                         n = e.ownerOrg,
                         i = e.datasetId,
                         s = Object(l.useState)(!0),
-                        m = Object(d.a)(s, 2),
-                        v = m[0],
-                        b = m[1],
+                        p = Object(d.a)(s, 2),
+                        v = p[0],
+                        b = p[1],
                         g = Object(l.useState)(i),
                         f = Object(d.a)(g, 2),
                         h = f[0],
                         y = f[1],
                         E = Object(l.useState)(Object(u.a)(Object(u.a)(Object(u.a)({}, ie), se), {}, {
                             publishing_status: "Draft",
                             private: !0,
@@ -2156,66 +2175,66 @@
                         A = Object(d.a)(C, 2),
                         F = A[0],
                         R = A[1],
                         j = Object(l.useState)(),
                         M = Object(d.a)(j, 2),
                         L = M[0],
                         U = M[1],
-                        B = Object(l.useState)("/dataset"),
-                        q = Object(d.a)(B, 2),
+                        G = Object(l.useState)("/dataset"),
+                        q = Object(d.a)(G, 2),
                         K = q[0],
                         z = q[1];
                     Object(l.useEffect)((function() {
                         S(Object(u.a)(Object(u.a)({}, x), {}, {
                             resources: O || x.resources
                         }))
                     }), [T]);
                     var X = function(e) {
                         var a = [];
                         a = e.response ? e.response.data && e.response.data.error ? Object.keys(e.response.data.error).map((function(a) {
                             return "object" === typeof e.response.data.error[a] ? e.response.data.error[a].join("; ") : e.response.data.error[a]
-                        })) : "Something has failed. Please, try again later or contact site administrator." : e.request ? "Please, check your connection or try again later. If the issue persists, contact site administrator." : "Something has failed. Please, try again later or contact site administrator.", R(r.a.createElement(xe, {
+                        })) : "Something has failed. Please, try again later or contact site administrator." : e.request ? "Please, check your connection or try again later. If the issue persists, contact site administrator." : "Something has failed. Please, try again later or contact site administrator.", R(r.a.createElement(Se, {
                             type: "error",
                             heading: "Error saving metadata",
                             message: a
                         })), window.scrollTo(0, 0)
                     };
-                    return h && v && (b(!1), G.fetchDataset(h, a, t).then((function(e) {
+                    return h && v && (b(!1), B.fetchDataset(h, a, t).then((function(e) {
                         var l = Object.assign({}, e);
-                        l.description = e.notes, y(l.id), l.parentDataset ? G.fetchDataset(l.parentDataset, a, t).then((function(e) {
+                        l.description = e.notes, y(l.id), l.parentDataset ? B.fetchDataset(l.parentDataset, a, t).then((function(e) {
                             S(Object.assign({}, x, l, {
                                 parentDatasetTitle: e.title
                             }))
                         })).catch(X) : S(Object.assign({}, x, l))
                     })).catch(X)), Object(l.useEffect)((function() {
                         var e = new URLSearchParams(window.location.search).get("group");
                         e && z("/organization/".concat(e))
                     }), []), r.a.createElement("div", {
                         className: "grid-container"
-                    }, r.a.createElement(_e, {
+                    }, r.a.createElement(xe, {
                         currentStep: T,
                         handleSteps: I
                     }), r.a.createElement("a", {
                         href: K
-                    }, "< Back to dashboard"), r.a.createElement(Ne, {
+                    }, "< Back to dashboard"), r.a.createElement(Oe, {
                         currentStep: T
-                    }), F, 0 === T && r.a.createElement(p.d, {
+                    }), F, 0 === T && r.a.createElement(m.d, {
                         initialValues: x,
                         enableReinitialize: !0,
                         validateOnChange: !1,
                         validateOnBlur: !1,
                         validateOnMount: !1,
                         onSubmit: function(e) {
-                            R(), h ? G.updateDataset(h, e, a, t).then((function() {
-                                S(Object.assign({}, e)), e.saveDraft ? U(new Date) : (R(r.a.createElement(xe, {
+                            R(), h ? B.updateDataset(h, e, a, t).then((function() {
+                                S(Object.assign({}, e)), e.saveDraft ? U(new Date) : (R(r.a.createElement(Se, {
                                     type: "success",
                                     heading: "Dataset saved successfully"
                                 })), I(1), window.scrollTo(0, 0))
-                            })).catch(X) : G.createDataset(e, a, t).then((function(a) {
-                                S(Object.assign({}, e)), y(a.id), e.saveDraft ? U(new Date) : (R(r.a.createElement(xe, {
+                            })).catch(X) : B.createDataset(e, a, t).then((function(a) {
+                                S(Object.assign({}, e)), y(a.id), e.saveDraft ? U(new Date) : (R(r.a.createElement(Se, {
                                     type: "success",
                                     heading: "Dataset saved successfully"
                                 })), I(1), window.scrollTo(0, 0))
                             })).catch(X)
                         },
                         validate: function() {
                             R()
@@ -2224,47 +2243,47 @@
                     }, (function(e) {
                         var l = e.values,
                             i = e.handleSubmit,
                             s = e.errors,
                             c = e.setFieldValue,
                             o = e.submitForm,
                             u = e.handleChange;
-                        return r.a.createElement("div", null, s && Object.keys(s).length > 0 && r.a.createElement("div", null, r.a.createElement(xe, {
+                        return r.a.createElement("div", null, s && Object.keys(s).length > 0 && r.a.createElement("div", null, r.a.createElement(Se, {
                             type: "error",
                             heading: "This form contains invalid entries",
-                            errors: Se(s)
-                        })), r.a.createElement(p.c, {
+                            errors: we(s)
+                        })), r.a.createElement(m.c, {
                             onSubmit: i
                         }, r.a.createElement("div", null, r.a.createElement(te, {
                             apiKey: t,
                             apiUrl: a,
                             ownerOrg: n,
                             currentStep: 0,
                             fetchDatasetsOpts: "false",
                             values: l || {},
                             errors: s,
-                            draftSaved: L ? we(L) : void 0,
+                            draftSaved: L ? Ne(L) : void 0,
                             setFieldValue: c,
                             submitForm: o,
                             handleChange: u
                         }))))
-                    })), 1 === T && r.a.createElement(p.d, {
+                    })), 1 === T && r.a.createElement(m.d, {
                         initialValues: x,
                         enableReinitialize: !0,
                         validateOnChange: !1,
                         validateOnBlur: !1,
                         onSubmit: function(e) {
                             R();
                             var l = x && x.id;
-                            S(Object.assign({}, x, e)), l ? G.updateDataset(l, e, a, t).then((function() {
-                                e.saveDraft ? U(new Date) : (R(r.a.createElement(xe, {
+                            S(Object.assign({}, x, e)), l ? B.updateDataset(l, e, a, t).then((function() {
+                                e.saveDraft ? U(new Date) : (R(r.a.createElement(Se, {
                                     type: "success",
                                     heading: "Dataset saved successfully"
                                 })), I(2), window.scrollTo(0, 0))
-                            })).catch(X) : (R(r.a.createElement(xe, {
+                            })).catch(X) : (R(r.a.createElement(Se, {
                                 type: "error",
                                 heading: "No valid metadata saved in step 1.",
                                 message: "Please complete complete step one before submitting step 2."
                             })), window.scrollTo(0, 0))
                         },
                         validate: function() {
                             R()
@@ -2272,63 +2291,63 @@
                         validationSchema: ve
                     }, (function(e) {
                         var l = e.values,
                             i = e.handleSubmit,
                             s = e.errors,
                             c = e.setFieldValue,
                             o = e.submitForm;
-                        return r.a.createElement("div", null, s && Object.keys(s).length > 0 && r.a.createElement("div", null, r.a.createElement(xe, {
+                        return r.a.createElement("div", null, s && Object.keys(s).length > 0 && r.a.createElement("div", null, r.a.createElement(Se, {
                             type: "error",
                             heading: "This form contains invalid entries",
-                            errors: Se(s)
-                        })), r.a.createElement(p.c, {
+                            errors: we(s)
+                        })), r.a.createElement(m.c, {
                             onSubmit: i
-                        }, r.a.createElement("div", null, r.a.createElement(pe, {
+                        }, r.a.createElement("div", null, r.a.createElement(me, {
                             apiKey: t,
                             apiUrl: a,
                             ownerOrg: n,
                             currentStep: 1,
                             fetchDatasetsOpts: "false",
                             values: l || {},
                             errors: s,
-                            draftSaved: L ? we(L) : void 0,
+                            draftSaved: L ? Ne(L) : void 0,
                             setFieldValue: c,
                             submitForm: o,
                             handleSteps: I
                         }))))
-                    })), 2 === T && r.a.createElement(p.d, {
+                    })), 2 === T && r.a.createElement(m.d, {
                         initialValues: {
-                            resource: JSON.parse(JSON.stringify(Ee)),
+                            resource: JSON.parse(JSON.stringify(_e)),
                             resources: x.resources,
                             publish: !0,
                             savedResources: 0,
                             lastSavedResource: null,
                             saveDraft: !1,
                             publishing_status: x.publishing_status
                         },
                         enableReinitialize: !0,
                         validateOnChange: !1,
                         validateOnBlur: !1,
                         onSubmit: function(e, l) {
                             var n = l.setFieldValue,
                                 i = l.setSubmitting;
                             R();
-                            var s = JSON.stringify(Ee) !== JSON.stringify(e.resource);
+                            var s = JSON.stringify(_e) !== JSON.stringify(e.resource);
                             if (h) {
                                 var u, d = new URL(a),
-                                    p = "".concat(d.origin, "/dataset/").concat(h);
+                                    m = "".concat(d.origin, "/dataset/").concat(h);
                                 switch (e.resourceAction) {
                                     case "edit":
-                                        u = G.updateResource(e.resource, a, t);
+                                        u = B.updateResource(e.resource, a, t);
                                         break;
                                     case "delete":
-                                        u = G.deleteResource(e.resource.id, a, t);
+                                        u = B.deleteResource(e.resource.id, a, t);
                                         break;
                                     default:
-                                        s && (u = G.createResource(h, e.resource, a, t))
+                                        s && (u = B.createResource(h, e.resource, a, t))
                                 }
                                 u ? u.then(function() {
                                     var l = Object(o.a)(c.a.mark((function l(r) {
                                         var s;
                                         return c.a.wrap((function(l) {
                                             for (;;) switch (l.prev = l.next) {
                                                 case 0:
@@ -2336,107 +2355,107 @@
                                                         l.next = 5;
                                                         break
                                                     }
                                                     if (!e.resource.upload) {
                                                         l.next = 4;
                                                         break
                                                     }
-                                                    return l.next = 4, G.patchDataset(h, {
+                                                    return l.next = 4, B.patchDataset(h, {
                                                         private: !1
                                                     }, a, t);
                                                 case 4:
-                                                    e.publish ? G.patchDataset(h, {
+                                                    e.publish ? B.patchDataset(h, {
                                                         publishing_status: "Published"
                                                     }, a, t).then((function(e) {
-                                                        200 === e.status && window.location.replace(p)
+                                                        200 === e.status && window.location.replace(m)
                                                     })) : e.saveDraft ? (U(new Date), i(!1)) : (U(new Date), s = e.resources.filter((function(a) {
                                                         return a.id !== e.resource.id
-                                                    })), "delete" !== e.resourceAction && (s.push(r.data.result), n("savedResources", e.savedResources + 1), n("lastSavedResource", e.resource.name || e.resource.url)), n("resources", s), D(s), n("resource", JSON.parse(JSON.stringify(Ee))), i(!1));
+                                                    })), "delete" !== e.resourceAction && (s.push(r.data.result), n("savedResources", e.savedResources + 1), n("lastSavedResource", e.resource.name || e.resource.url)), n("resources", s), D(s), n("resource", JSON.parse(JSON.stringify(_e))), i(!1));
                                                 case 5:
                                                     n("resourceAction", void 0);
                                                 case 6:
                                                 case "end":
                                                     return l.stop()
                                             }
                                         }), l)
                                     })));
                                     return function(e) {
                                         return l.apply(this, arguments)
                                     }
                                 }()).catch((function(e) {
                                     X(e), i(!1)
-                                })) : e.publish ? G.patchDataset(h, {
+                                })) : e.publish ? B.patchDataset(h, {
                                     publishing_status: "Published"
                                 }, a, t).then((function(e) {
-                                    200 === e.status && window.location.replace(p)
+                                    200 === e.status && window.location.replace(m)
                                 })).catch((function(e) {
                                     X(e), i(!1)
                                 })) : e.saveDraft ? (U(new Date), i(!1)) : i(!1)
-                            } else R(r.a.createElement(xe, {
+                            } else R(r.a.createElement(Se, {
                                 type: "error",
                                 heading: "No valid metadata saved in previous steps.",
                                 message: "Please complete previous steps before submitting resource(s)."
                             }))
                         },
                         validate: function() {
                             R()
                         },
-                        validationSchema: ye,
+                        validationSchema: Ee,
                         render: function(e) {
                             var a = e.values,
                                 t = e.errors,
                                 l = e.handleSubmit,
                                 n = e.setFieldValue,
                                 i = e.submitForm,
                                 s = e.isSubmitting;
                             return r.a.createElement("div", {
                                 className: ""
-                            }, t && Object.keys(t).length > 0 && r.a.createElement("div", null, r.a.createElement(xe, {
+                            }, t && Object.keys(t).length > 0 && r.a.createElement("div", null, r.a.createElement(Se, {
                                 type: "error",
                                 heading: "This form contains invalid entries",
-                                errors: Se(t)
-                            })), r.a.createElement(p.c, {
+                                errors: we(t)
+                            })), r.a.createElement(m.c, {
                                 onSubmit: l
-                            }, r.a.createElement(he, {
+                            }, r.a.createElement(ye, {
                                 values: a,
                                 errors: t,
-                                draftSaved: L ? we(L) : void 0,
+                                draftSaved: L ? Ne(L) : void 0,
                                 setFieldValue: n,
                                 submitForm: i,
                                 isSubmitting: s,
                                 handleSteps: I
                             })))
                         }
                     }))
                 },
-                De = function(e) {
+                Pe = function(e) {
                     var a = e.apiUrl,
                         t = e.apiKey,
                         l = e.ownerOrg,
                         n = e.datasetId;
                     return r.a.createElement("div", {
                         className: "App"
-                    }, r.a.createElement(Oe, {
+                    }, r.a.createElement(De, {
                         apiUrl: a,
                         apiKey: t,
                         ownerOrg: l,
                         datasetId: n
                     }))
                 };
             Boolean("localhost" === window.location.hostname || "[::1]" === window.location.hostname || window.location.hostname.match(/^127(?:\.(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)){3}$/));
-            var Pe = document.getElementById("root"),
-                ke = Pe.getAttribute("data-apiUrl"),
-                Te = Pe.getAttribute("data-apiKey"),
-                Ie = Pe.getAttribute("data-ownerOrg"),
-                Ce = Pe.getAttribute("data-datasetId");
-            i.a.render(r.a.createElement(r.a.StrictMode, null, r.a.createElement(De, {
-                apiUrl: ke,
-                apiKey: Te,
-                ownerOrg: Ie,
-                datasetId: Ce
+            var ke = document.getElementById("root"),
+                Te = ke.getAttribute("data-apiUrl"),
+                Ie = ke.getAttribute("data-apiKey"),
+                Ce = ke.getAttribute("data-ownerOrg"),
+                Ae = ke.getAttribute("data-datasetId");
+            i.a.render(r.a.createElement(r.a.StrictMode, null, r.a.createElement(Pe, {
+                apiUrl: Te,
+                apiKey: Ie,
+                ownerOrg: Ce,
+                datasetId: Ae
             })), document.getElementById("root")), "serviceWorker" in navigator && navigator.serviceWorker.ready.then((function(e) {
                 e.unregister()
             })).catch((function(e) {
                 console.error(e.message)
             }))
         }
     },
```

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/public/js/runtime-main.js` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/public/js/runtime-main.js`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/templates/package/read_base.html` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/templates/package/read_base.html`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext/dcat_usmetadata/templates/package/search.html` & `ckanext-dcat_usmetadata-0.4.1/ckanext/dcat_usmetadata/templates/package/search.html`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/ckanext_dcat_usmetadata.egg-info/SOURCES.txt` & `ckanext-dcat_usmetadata-0.4.1/ckanext_dcat_usmetadata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/requirements.txt` & `ckanext-dcat_usmetadata-0.4.1/requirements.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 -e git+https://github.com/ckan/ckanext-harvest.git@master#egg=ckanext_harvest
 git+https://github.com/keitaroinc/ckanext-saml2auth@main#egg=ckanext-saml2auth
 
 ckanext-datajson
 ckanext-googleanalyticsbasic
-ckanext-usmetadata
+# ckanext-usmetadata
+-e git+https://github.com/GSA/ckanext-usmetadata.git@ckan-2.10#egg=ckanext-usmetadata
 
 repoze.lru==0.7
 repoze.who==2.4
 webob
 
 # ckanext-saml2 dependencies
 M2Crypto==0.36.0
```

### Comparing `ckanext-dcat_usmetadata-0.4.0/setup.cfg` & `ckanext-dcat_usmetadata-0.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `ckanext-dcat_usmetadata-0.4.0/setup.py` & `ckanext-dcat_usmetadata-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 setup(
     name='''ckanext-dcat_usmetadata''',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # http://packaging.python.org/en/latest/tutorial.html#version
-    version='0.4.0',
+    version='0.4.1',
 
     description='''DCAT USMetadata Form App for CKAN''',
     long_description=long_description,
     long_description_content_type='text/markdown',
 
     # The project's main homepage.
     url='https://github.com/GSA/ckanext-dcat_usmetadata',
```

