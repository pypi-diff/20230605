# Comparing `tmp/fietsboek-0.7.0.tar.gz` & `tmp/fietsboek-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fietsboek-0.7.0.tar", max compression
+gzip compressed data, was "fietsboek-0.8.0.tar", max compression
```

## Comparing `fietsboek-0.7.0.tar` & `fietsboek-0.8.0.tar`

### file list

```diff
@@ -1,198 +1,202 @@
--rw-r--r--   0        0        0    34523 2022-07-04 18:57:32.078542 fietsboek-0.7.0/LICENSE.txt
--rw-r--r--   0        0        0     2711 2023-01-25 18:49:03.881246 fietsboek-0.7.0/README.md
--rw-r--r--   0        0        0     6287 2023-04-12 21:05:27.144201 fietsboek-0.7.0/fietsboek/__init__.py
--rw-r--r--   0        0        0     8093 2023-03-07 19:24:51.331839 fietsboek-0.7.0/fietsboek/actions.py
--rw-r--r--   0        0        0     1430 2022-12-13 21:14:10.387413 fietsboek-0.7.0/fietsboek/alembic/env.py
--rw-r--r--   0        0        0      492 2022-06-26 19:26:28.000000 fietsboek-0.7.0/fietsboek/alembic/script.py.mako
--rw-r--r--   0        0        0     7221 2022-12-29 14:02:02.600329 fietsboek-0.7.0/fietsboek/alembic/versions/20220702_1b4b1c179e5a.py
--rw-r--r--   0        0        0     1326 2022-12-29 14:02:02.598329 fietsboek-0.7.0/fietsboek/alembic/versions/20220706_c89d9bdbfa68.py
--rw-r--r--   0        0        0      910 2022-12-29 14:02:02.595329 fietsboek-0.7.0/fietsboek/alembic/versions/20220721_091ce24409fe.py
--rw-r--r--   0        0        0      541 2022-12-29 14:02:02.597329 fietsboek-0.7.0/fietsboek/alembic/versions/20220808_d085998b49ca.py
--rw-r--r--   0        0        0     1418 2022-12-29 14:02:02.596329 fietsboek-0.7.0/fietsboek/alembic/versions/20221214_c939800af428.py
--rw-r--r--   0        0        0      520 2023-03-07 19:07:52.859104 fietsboek-0.7.0/fietsboek/alembic/versions/20230203_3149aa2d0114.py
--rw-r--r--   0        0        0       33 2022-06-26 19:26:28.000000 fietsboek-0.7.0/fietsboek/alembic/versions/README.txt
--rw-r--r--   0        0        0     9886 2023-04-13 18:12:32.565708 fietsboek-0.7.0/fietsboek/config.py
--rw-r--r--   0        0        0    13873 2023-04-13 18:12:32.566708 fietsboek-0.7.0/fietsboek/data.py
--rw-r--r--   0        0        0     2330 2022-12-29 16:02:59.213304 fietsboek-0.7.0/fietsboek/email.py
--rw-r--r--   0        0        0     3809 2023-04-13 18:12:32.568709 fietsboek-0.7.0/fietsboek/hittekaart.py
--rw-r--r--   0        0        0     3698 2023-04-13 18:12:32.568709 fietsboek-0.7.0/fietsboek/jinja2.py
--rw-r--r--   0        0        0    13379 2023-04-24 18:24:31.964712 fietsboek-0.7.0/fietsboek/locale/de/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0    23161 2023-04-24 18:24:31.964712 fietsboek-0.7.0/fietsboek/locale/de/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0      484 2022-07-07 11:19:31.236253 fietsboek-0.7.0/fietsboek/locale/de/html/home.html
--rw-r--r--   0        0        0    12561 2023-04-24 18:24:31.964712 fietsboek-0.7.0/fietsboek/locale/en/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0    22314 2023-04-24 18:24:31.964712 fietsboek-0.7.0/fietsboek/locale/en/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0      439 2022-07-07 11:17:06.866340 fietsboek-0.7.0/fietsboek/locale/en/html/home.html
--rw-r--r--   0        0        0    18912 2023-04-24 18:24:31.964712 fietsboek-0.7.0/fietsboek/locale/fietslog.pot
--rw-r--r--   0        0        0     4991 2022-12-29 14:02:02.545329 fietsboek-0.7.0/fietsboek/models/__init__.py
--rw-r--r--   0        0        0     1643 2022-12-29 14:02:02.550329 fietsboek-0.7.0/fietsboek/models/badge.py
--rw-r--r--   0        0        0     1277 2022-12-29 14:02:02.552329 fietsboek-0.7.0/fietsboek/models/comment.py
--rw-r--r--   0        0        0     1954 2022-12-29 14:02:02.544329 fietsboek-0.7.0/fietsboek/models/image.py
--rw-r--r--   0        0        0      732 2023-03-07 19:07:19.490784 fietsboek-0.7.0/fietsboek/models/meta.py
--rw-r--r--   0        0        0    28311 2023-04-13 18:12:32.575709 fietsboek-0.7.0/fietsboek/models/track.py
--rw-r--r--   0        0        0    16106 2023-04-13 18:12:32.576709 fietsboek-0.7.0/fietsboek/models/user.py
--rw-r--r--   0        0        0     7386 2023-01-25 17:19:24.857216 fietsboek-0.7.0/fietsboek/pages.py
--rw-r--r--   0        0        0      462 2022-12-13 21:14:10.397413 fietsboek-0.7.0/fietsboek/pshell.py
--rw-r--r--   0        0        0     2780 2023-04-13 18:12:32.577709 fietsboek-0.7.0/fietsboek/routes.py
--rw-r--r--   0        0        0     1707 2023-04-12 21:05:27.149201 fietsboek-0.7.0/fietsboek/scripts/__init__.py
--rw-r--r--   0        0        0     5198 2023-04-24 18:24:31.964712 fietsboek-0.7.0/fietsboek/scripts/fietscron.py
--rw-r--r--   0        0        0     9555 2023-04-13 18:12:32.577709 fietsboek-0.7.0/fietsboek/scripts/fietsctl.py
--rw-r--r--   0        0        0     3663 2022-12-29 14:02:02.535329 fietsboek-0.7.0/fietsboek/security.py
--rw-r--r--   0        0        0     3033 2023-02-06 18:03:03.267372 fietsboek-0.7.0/fietsboek/static/GM_Utils/GPX2GM.css
--rw-r--r--   0        0        0   111993 2023-02-06 18:03:03.270372 fietsboek-0.7.0/fietsboek/static/GM_Utils/GPX2GM.js
--rw-r--r--   0        0        0    32768 2023-02-06 18:03:03.271372 fietsboek-0.7.0/fietsboek/static/GM_Utils/GPX2GM_Defs.js
--rw-r--r--   0        0        0      147 2023-02-06 18:03:03.276372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/Grau256x256.png
--rw-r--r--   0        0        0     7209 2023-02-06 18:03:03.277372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/Loading_icon.gif
--rw-r--r--   0        0        0    17490 2023-02-06 18:03:03.278372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/Loading_icon_V1.gif
--rw-r--r--   0        0        0     1775 2023-02-06 18:03:03.280372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/Loading_icon_V2.gif
--rw-r--r--   0        0        0      877 2023-02-06 18:03:03.284372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/airport.png
--rw-r--r--   0        0        0      698 2023-02-06 18:03:03.285372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/bar.png
--rw-r--r--   0        0        0      873 2023-02-06 18:03:03.285372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/boat.png
--rw-r--r--   0        0        0      624 2023-02-06 18:03:03.286372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/bridge.png
--rw-r--r--   0        0        0      715 2023-02-06 18:03:03.286372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/castle.png
--rw-r--r--   0        0        0      648 2023-02-06 18:03:03.287372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/church2.png
--rw-r--r--   0        0        0      428 2023-02-06 18:03:03.288372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/circle_green.svg
--rw-r--r--   0        0        0      421 2023-02-06 18:03:03.288372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/circle_red.svg
--rw-r--r--   0        0        0     1138 2023-02-06 18:03:03.289372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/cluster.png
--rw-r--r--   0        0        0      604 2023-02-06 18:03:03.290372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/cluster.svg
--rw-r--r--   0        0        0     1050 2023-02-06 18:03:03.291372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/current_location - Kopie.svg
--rw-r--r--   0        0        0     1050 2023-02-06 18:03:03.291372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/current_location.svg
--rw-r--r--   0        0        0     1270 2023-02-06 18:03:03.292372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/cycling.png
--rw-r--r--   0        0        0      780 2023-02-06 18:03:03.292372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/finish.png
--rw-r--r--   0        0        0      482 2023-02-06 18:03:03.293372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/flag.png
--rw-r--r--   0        0        0      428 2023-02-06 18:03:03.293372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/fullscreen_m.svg
--rw-r--r--   0        0        0      410 2023-02-06 18:03:03.295372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/fullscreen_p.svg
--rw-r--r--   0        0        0      710 2023-02-06 18:03:03.295372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/harbor.png
--rw-r--r--   0        0        0     1325 2023-02-06 18:03:03.296372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/hiking.png
--rw-r--r--   0        0        0      309 2023-02-06 18:03:03.296372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/hotel.png
--rw-r--r--   0        0        0      892 2023-02-06 18:03:03.297372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/hotel2.png
--rw-r--r--   0        0        0     3311 2023-02-06 18:03:03.298372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/kreis.png
--rw-r--r--   0        0        0      650 2023-02-06 18:03:03.298372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/library.png
--rw-r--r--   0        0        0      204 2023-02-06 18:03:03.299372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/lupe_m.png
--rw-r--r--   0        0        0      392 2023-02-06 18:03:03.299372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/lupe_m_32.png
--rw-r--r--   0        0        0      200 2023-02-06 18:03:03.300372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/lupe_p.png
--rw-r--r--   0        0        0      405 2023-02-06 18:03:03.300372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/lupe_p_32.png
--rw-r--r--   0        0        0      645 2023-02-06 18:03:03.301372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/marker-icon_bw.png
--rw-r--r--   0        0        0      495 2023-02-06 18:03:03.301372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/marker-icon_bw_41x25.png
--rw-r--r--   0        0        0      345 2023-02-06 18:03:03.302372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/marker-icon_bw_small.png
--rw-r--r--   0        0        0       77 2023-02-06 18:03:03.302372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/marker.gif
--rw-r--r--   0        0        0      699 2023-02-06 18:03:03.303372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/marker.svg
--rw-r--r--   0        0        0      849 2023-02-06 18:03:03.303372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/museum.png
--rw-r--r--   0        0        0     1390 2023-02-06 18:03:03.304372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/panorama.png
--rw-r--r--   0        0        0     1100 2023-02-06 18:03:03.304372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/park.png
--rw-r--r--   0        0        0      545 2023-02-06 18:03:03.305372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/peak.png
--rw-r--r--   0        0        0      720 2023-02-06 18:03:03.305372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/photo.png
--rw-r--r--   0        0        0      642 2023-02-06 18:03:03.306372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/pin_red.png
--rw-r--r--   0        0        0      650 2023-02-06 18:03:03.306372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/pin_red_shadow.png
--rw-r--r--   0        0        0     1003 2023-02-06 18:03:03.307372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/restaurant.png
--rw-r--r--   0        0        0      394 2023-02-06 18:03:03.308372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/scenic.png
--rw-r--r--   0        0        0      770 2023-02-06 18:03:03.308372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/shadow.png
--rw-r--r--   0        0        0      570 2023-02-06 18:03:03.308372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/shadow50.png
--rw-r--r--   0        0        0      643 2023-02-06 18:03:03.309372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/shoppingmall.png
--rw-r--r--   0        0        0      438 2023-02-06 18:03:03.309372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/square_green.svg
--rw-r--r--   0        0        0      431 2023-02-06 18:03:03.310372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/square_red.svg
--rw-r--r--   0        0        0      449 2023-02-06 18:03:03.310372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/start.png
--rw-r--r--   0        0        0      603 2023-02-06 18:03:03.310372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/streckenmarker - Kopie.svg
--rw-r--r--   0        0        0      603 2023-02-06 18:03:03.310372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/streckenmarker.svg
--rw-r--r--   0        0        0      795 2023-02-06 18:03:03.311372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/subway.png
--rw-r--r--   0        0        0      642 2023-02-06 18:03:03.311372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/tent.png
--rw-r--r--   0        0        0      947 2023-02-06 18:03:03.311372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/train.png
--rw-r--r--   0        0        0     1290 2023-02-06 18:03:03.312372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/video.png
--rw-r--r--   0        0        0      626 2023-02-06 18:03:03.312372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/villa.png
--rw-r--r--   0        0        0      657 2023-02-06 18:03:03.312372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/whereami.svg
--rw-r--r--   0        0        0     1121 2023-02-06 18:03:03.313372 fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/whereami_V1.svg
--rw-r--r--   0        0        0    37589 2023-02-06 18:03:03.314372 fietsboek-0.7.0/fietsboek/static/GM_Utils/gmutils.js
--rw-r--r--   0        0        0     3736 2023-02-06 18:03:03.314372 fietsboek-0.7.0/fietsboek/static/GM_Utils/gra_canvas.js
--rw-r--r--   0        0        0     6095 2023-02-06 18:03:03.314372 fietsboek-0.7.0/fietsboek/static/GM_Utils/gra_svg.js
--rw-r--r--   0        0        0     1259 2022-10-04 14:03:38.000000 fietsboek-0.7.0/fietsboek/static/GM_Utils/leaflet/images/layers-2x.png
--rw-r--r--   0        0        0      696 2022-10-04 14:03:38.000000 fietsboek-0.7.0/fietsboek/static/GM_Utils/leaflet/images/layers.png
--rw-r--r--   0        0        0     2464 2022-10-04 14:03:38.000000 fietsboek-0.7.0/fietsboek/static/GM_Utils/leaflet/images/marker-icon-2x.png
--rw-r--r--   0        0        0     1466 2022-10-04 14:03:38.000000 fietsboek-0.7.0/fietsboek/static/GM_Utils/leaflet/images/marker-icon.png
--rw-r--r--   0        0        0      618 2022-10-04 14:03:38.000000 fietsboek-0.7.0/fietsboek/static/GM_Utils/leaflet/images/marker-shadow.png
--rw-r--r--   0        0        0    14670 2022-10-04 14:03:38.000000 fietsboek-0.7.0/fietsboek/static/GM_Utils/leaflet/leaflet.css
--rw-r--r--   0        0        0   146315 2022-10-04 14:05:32.000000 fietsboek-0.7.0/fietsboek/static/GM_Utils/leaflet/leaflet.js
--rw-r--r--   0        0        0   223367 2022-10-04 14:05:32.000000 fietsboek-0.7.0/fietsboek/static/GM_Utils/leaflet/leaflet.js.map
--rw-r--r--   0        0        0    39191 2023-02-06 18:03:03.315372 fietsboek-0.7.0/fietsboek/static/GM_Utils/osmutils.js
--rw-r--r--   0        0        0    20687 2023-02-06 18:03:03.316372 fietsboek-0.7.0/fietsboek/static/GM_Utils/plot.js
--rw-r--r--   0        0        0     3594 2023-02-06 18:03:03.316372 fietsboek-0.7.0/fietsboek/static/GM_Utils/shimg.js
--rw-r--r--   0        0        0    93729 2023-04-24 18:24:31.965712 fietsboek-0.7.0/fietsboek/static/bootstrap-icons.css
--rw-r--r--   0        0        0    80420 2023-04-24 18:24:31.965712 fietsboek-0.7.0/fietsboek/static/bootstrap.bundle.min.js
--rw-r--r--   0        0        0   237950 2023-04-24 18:24:31.966712 fietsboek-0.7.0/fietsboek/static/bootstrap.css
--rw-r--r--   0        0        0    25053 2022-06-30 00:22:45.000000 fietsboek-0.7.0/fietsboek/static/favicon.png
--rw-r--r--   0        0        0    13219 2023-03-26 20:32:32.913787 fietsboek-0.7.0/fietsboek/static/fietsboek.js
--rw-r--r--   0        0        0    10999 2023-03-26 20:32:32.914788 fietsboek-0.7.0/fietsboek/static/fietsboek.js.map
--rw-r--r--   0        0        0   164360 2023-04-24 18:24:31.966712 fietsboek-0.7.0/fietsboek/static/fonts/bootstrap-icons.woff
--rw-r--r--   0        0        0   121340 2023-04-24 18:24:31.966712 fietsboek-0.7.0/fietsboek/static/fonts/bootstrap-icons.woff2
--rw-r--r--   0        0        0    20748 2022-07-04 18:57:32.170543 fietsboek-0.7.0/fietsboek/static/fonts/open-sans-v29-latin-300.woff
--rw-r--r--   0        0        0    16812 2022-07-04 18:57:32.170543 fietsboek-0.7.0/fietsboek/static/fonts/open-sans-v29-latin-300.woff2
--rw-r--r--   0        0        0    21928 2022-07-04 18:57:32.170543 fietsboek-0.7.0/fietsboek/static/fonts/open-sans-v29-latin-300italic.woff
--rw-r--r--   0        0        0    17828 2022-07-04 18:57:32.170543 fietsboek-0.7.0/fietsboek/static/fonts/open-sans-v29-latin-300italic.woff2
--rw-r--r--   0        0        0    20772 2022-07-04 18:57:32.171543 fietsboek-0.7.0/fietsboek/static/fonts/open-sans-v29-latin-500.woff
--rw-r--r--   0        0        0    16812 2022-07-04 18:57:32.171543 fietsboek-0.7.0/fietsboek/static/fonts/open-sans-v29-latin-500.woff2
--rw-r--r--   0        0        0    21868 2022-07-04 18:57:32.171543 fietsboek-0.7.0/fietsboek/static/fonts/open-sans-v29-latin-500italic.woff
--rw-r--r--   0        0        0    17896 2022-07-04 18:57:32.171543 fietsboek-0.7.0/fietsboek/static/fonts/open-sans-v29-latin-500italic.woff2
--rw-r--r--   0        0        0    20664 2022-07-04 18:57:32.172543 fietsboek-0.7.0/fietsboek/static/fonts/open-sans-v29-latin-600.woff
--rw-r--r--   0        0        0    16796 2022-07-04 18:57:32.172543 fietsboek-0.7.0/fietsboek/static/fonts/open-sans-v29-latin-600.woff2
--rw-r--r--   0        0        0    21812 2022-07-04 18:57:32.172543 fietsboek-0.7.0/fietsboek/static/fonts/open-sans-v29-latin-600italic.woff
--rw-r--r--   0        0        0    17836 2022-07-04 18:57:32.172543 fietsboek-0.7.0/fietsboek/static/fonts/open-sans-v29-latin-600italic.woff2
--rw-r--r--   0        0        0    20164 2022-07-04 18:57:32.173543 fietsboek-0.7.0/fietsboek/static/fonts/open-sans-v29-latin-700.woff
--rw-r--r--   0        0        0    16360 2022-07-04 18:57:32.173543 fietsboek-0.7.0/fietsboek/static/fonts/open-sans-v29-latin-700.woff2
--rw-r--r--   0        0        0    21244 2022-07-04 18:57:32.173543 fietsboek-0.7.0/fietsboek/static/fonts/open-sans-v29-latin-700italic.woff
--rw-r--r--   0        0        0    17396 2022-07-04 18:57:32.174543 fietsboek-0.7.0/fietsboek/static/fonts/open-sans-v29-latin-700italic.woff2
--rw-r--r--   0        0        0    20656 2022-07-04 18:57:32.174543 fietsboek-0.7.0/fietsboek/static/fonts/open-sans-v29-latin-800.woff
--rw-r--r--   0        0        0    16724 2022-07-04 18:57:32.174543 fietsboek-0.7.0/fietsboek/static/fonts/open-sans-v29-latin-800.woff2
--rw-r--r--   0        0        0    21520 2022-07-04 18:57:32.175543 fietsboek-0.7.0/fietsboek/static/fonts/open-sans-v29-latin-800italic.woff
--rw-r--r--   0        0        0    17704 2022-07-04 18:57:32.175543 fietsboek-0.7.0/fietsboek/static/fonts/open-sans-v29-latin-800italic.woff2
--rw-r--r--   0        0        0    21848 2022-07-04 18:57:32.175543 fietsboek-0.7.0/fietsboek/static/fonts/open-sans-v29-latin-italic.woff
--rw-r--r--   0        0        0    17816 2022-07-04 18:57:32.176543 fietsboek-0.7.0/fietsboek/static/fonts/open-sans-v29-latin-italic.woff2
--rw-r--r--   0        0        0    20704 2022-07-04 18:57:32.176543 fietsboek-0.7.0/fietsboek/static/fonts/open-sans-v29-latin-regular.woff
--rw-r--r--   0        0        0    16720 2022-07-04 18:57:32.176543 fietsboek-0.7.0/fietsboek/static/fonts/open-sans-v29-latin-regular.woff2
--rw-r--r--   0        0        0     4473 2022-07-04 18:57:32.169543 fietsboek-0.7.0/fietsboek/static/fonts.css
--rw-r--r--   0        0        0    14075 2022-12-13 21:14:10.403414 fietsboek-0.7.0/fietsboek/static/osm-monkeypatch.js
--rw-r--r--   0        0        0     2434 2023-03-26 20:32:32.914788 fietsboek-0.7.0/fietsboek/static/theme.css
--rw-r--r--   0        0        0      638 2023-03-26 20:32:32.914788 fietsboek-0.7.0/fietsboek/static/theme.css.map
--rw-r--r--   0        0        0     3700 2023-03-07 19:07:19.491784 fietsboek-0.7.0/fietsboek/summaries.py
--rw-r--r--   0        0        0      280 2022-06-26 19:26:28.000000 fietsboek-0.7.0/fietsboek/templates/404.jinja2
--rw-r--r--   0        0        0     2056 2022-07-14 14:18:13.964884 fietsboek-0.7.0/fietsboek/templates/admin.jinja2
--rw-r--r--   0        0        0     8831 2022-12-13 21:14:10.404414 fietsboek-0.7.0/fietsboek/templates/browse.jinja2
--rw-r--r--   0        0        0     2628 2022-12-13 21:14:10.405413 fietsboek-0.7.0/fietsboek/templates/create_account.jinja2
--rw-r--r--   0        0        0     8519 2023-03-07 19:07:52.862105 fietsboek-0.7.0/fietsboek/templates/details.jinja2
--rw-r--r--   0        0        0     1055 2022-12-13 21:14:10.410414 fietsboek-0.7.0/fietsboek/templates/edit.jinja2
--rw-r--r--   0        0        0     9803 2023-03-07 19:07:52.863104 fietsboek-0.7.0/fietsboek/templates/edit_form.jinja2
--rw-r--r--   0        0        0     1128 2022-12-13 21:14:10.411414 fietsboek-0.7.0/fietsboek/templates/finish_upload.jinja2
--rw-r--r--   0        0        0     2263 2023-04-24 18:24:31.966712 fietsboek-0.7.0/fietsboek/templates/home.jinja2
--rw-r--r--   0        0        0     6268 2023-04-13 18:12:32.578709 fietsboek-0.7.0/fietsboek/templates/layout.jinja2
--rw-r--r--   0        0        0     1812 2022-12-13 21:14:10.412414 fietsboek-0.7.0/fietsboek/templates/login.jinja2
--rw-r--r--   0        0        0     1479 2022-07-14 14:18:13.965884 fietsboek-0.7.0/fietsboek/templates/password_reset.jinja2
--rw-r--r--   0        0        0     5894 2023-04-13 18:12:32.578709 fietsboek-0.7.0/fietsboek/templates/profile.jinja2
--rw-r--r--   0        0        0      766 2022-07-14 14:18:13.966884 fietsboek-0.7.0/fietsboek/templates/request_password.jinja2
--rw-r--r--   0        0        0      171 2022-12-13 21:14:10.413414 fietsboek-0.7.0/fietsboek/templates/static-page.jinja2
--rw-r--r--   0        0        0      603 2022-07-14 14:18:13.966884 fietsboek-0.7.0/fietsboek/templates/upload.jinja2
--rw-r--r--   0        0        0     3832 2023-04-13 18:12:32.579709 fietsboek-0.7.0/fietsboek/templates/user_data.jinja2
--rw-r--r--   0        0        0      318 2022-07-14 14:18:13.966884 fietsboek-0.7.0/fietsboek/templates/util.jinja2
--rw-r--r--   0        0        0     7807 2023-04-24 18:24:31.971712 fietsboek-0.7.0/fietsboek/transformers/__init__.py
--rw-r--r--   0        0        0     4085 2023-04-24 18:24:31.971712 fietsboek-0.7.0/fietsboek/transformers/breaks.py
--rw-r--r--   0        0        0    15166 2023-04-12 21:05:27.159201 fietsboek-0.7.0/fietsboek/updater/__init__.py
--rw-r--r--   0        0        0     6574 2023-03-26 20:32:32.915788 fietsboek-0.7.0/fietsboek/updater/cli.py
--rw-r--r--   0        0        0     1087 2022-12-14 21:36:27.533733 fietsboek-0.7.0/fietsboek/updater/script.py
--rw-r--r--   0        0        0     2378 2023-01-10 20:57:15.559281 fietsboek-0.7.0/fietsboek/updater/scripts/upd_20230103_lu8w3rwlz4ddcpms.py
--rw-r--r--   0        0        0      475 2023-01-12 19:33:34.761460 fietsboek-0.7.0/fietsboek/updater/scripts/upd_20230112_v0.5.0.py
--rw-r--r--   0        0        0      465 2023-03-08 18:25:33.078353 fietsboek-0.7.0/fietsboek/updater/scripts/upd_20230308_v0.6.0.py
--rw-r--r--   0        0        0      465 2023-04-24 18:26:24.398858 fietsboek-0.7.0/fietsboek/updater/scripts/upd_20230424_v0.7.0.py
--rw-r--r--   0        0        0     2104 2022-12-29 14:02:02.591329 fietsboek-0.7.0/fietsboek/updater/scripts/upd_30ppwg8zi4ujb46f.py
--rw-r--r--   0        0        0      454 2022-12-13 21:14:10.416414 fietsboek-0.7.0/fietsboek/updater/scripts/upd_initial.py
--rw-r--r--   0        0        0      466 2022-12-13 21:14:10.417414 fietsboek-0.7.0/fietsboek/updater/scripts/upd_v0.4.0.py
--rw-r--r--   0        0        0    14161 2023-04-13 18:32:36.906301 fietsboek-0.7.0/fietsboek/util.py
--rw-r--r--   0        0        0        0 2022-06-26 19:26:27.000000 fietsboek-0.7.0/fietsboek/views/__init__.py
--rw-r--r--   0        0        0     2845 2022-12-29 14:02:02.561329 fietsboek-0.7.0/fietsboek/views/account.py
--rw-r--r--   0        0        0     2828 2022-12-29 14:02:02.572329 fietsboek-0.7.0/fietsboek/views/admin.py
--rw-r--r--   0        0        0    12981 2022-12-29 14:02:02.571329 fietsboek-0.7.0/fietsboek/views/browse.py
--rw-r--r--   0        0        0     8349 2023-04-20 19:43:46.582320 fietsboek-0.7.0/fietsboek/views/default.py
--rw-r--r--   0        0        0     6724 2023-04-13 18:12:32.581709 fietsboek-0.7.0/fietsboek/views/detail.py
--rw-r--r--   0        0        0     3553 2023-03-07 19:11:04.652006 fietsboek-0.7.0/fietsboek/views/edit.py
--rw-r--r--   0        0        0      404 2022-12-13 21:14:10.420414 fietsboek-0.7.0/fietsboek/views/notfound.py
--rw-r--r--   0        0        0     6420 2023-04-13 18:12:32.582709 fietsboek-0.7.0/fietsboek/views/profile.py
--rw-r--r--   0        0        0    14574 2023-03-08 18:45:52.332655 fietsboek-0.7.0/fietsboek/views/tileproxy.py
--rw-r--r--   0        0        0     7141 2023-04-13 18:12:32.583709 fietsboek-0.7.0/fietsboek/views/upload.py
--rw-r--r--   0        0        0     5737 2023-04-13 18:12:32.583709 fietsboek-0.7.0/fietsboek/views/user_data.py
--rw-r--r--   0        0        0     2284 2023-04-24 18:25:10.968106 fietsboek-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     4625 1970-01-01 00:00:00.000000 fietsboek-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2022-07-04 18:57:32.078542 fietsboek-0.8.0/LICENSE.txt
+-rw-r--r--   0        0        0     2711 2023-01-25 18:49:03.881246 fietsboek-0.8.0/README.md
+-rw-r--r--   0        0        0     6287 2023-04-12 21:05:27.144201 fietsboek-0.8.0/fietsboek/__init__.py
+-rw-r--r--   0        0        0     9706 2023-06-02 18:42:21.377174 fietsboek-0.8.0/fietsboek/actions.py
+-rw-r--r--   0        0        0     1430 2022-12-13 21:14:10.387413 fietsboek-0.8.0/fietsboek/alembic/env.py
+-rw-r--r--   0        0        0      492 2022-06-26 19:26:28.000000 fietsboek-0.8.0/fietsboek/alembic/script.py.mako
+-rw-r--r--   0        0        0     7221 2022-12-29 14:02:02.600329 fietsboek-0.8.0/fietsboek/alembic/versions/20220702_1b4b1c179e5a.py
+-rw-r--r--   0        0        0     1326 2022-12-29 14:02:02.598329 fietsboek-0.8.0/fietsboek/alembic/versions/20220706_c89d9bdbfa68.py
+-rw-r--r--   0        0        0      910 2022-12-29 14:02:02.595329 fietsboek-0.8.0/fietsboek/alembic/versions/20220721_091ce24409fe.py
+-rw-r--r--   0        0        0      541 2022-12-29 14:02:02.597329 fietsboek-0.8.0/fietsboek/alembic/versions/20220808_d085998b49ca.py
+-rw-r--r--   0        0        0     1418 2022-12-29 14:02:02.596329 fietsboek-0.8.0/fietsboek/alembic/versions/20221214_c939800af428.py
+-rw-r--r--   0        0        0      520 2023-03-07 19:07:52.859104 fietsboek-0.8.0/fietsboek/alembic/versions/20230203_3149aa2d0114.py
+-rw-r--r--   0        0        0       33 2022-06-26 19:26:28.000000 fietsboek-0.8.0/fietsboek/alembic/versions/README.txt
+-rw-r--r--   0        0        0    10094 2023-04-26 15:50:29.247401 fietsboek-0.8.0/fietsboek/config.py
+-rw-r--r--   0        0        0     1513 2023-05-31 19:17:03.317788 fietsboek-0.8.0/fietsboek/convert.py
+-rw-r--r--   0        0        0    14349 2023-06-02 18:37:35.903419 fietsboek-0.8.0/fietsboek/data.py
+-rw-r--r--   0        0        0     2330 2022-12-29 16:02:59.213304 fietsboek-0.8.0/fietsboek/email.py
+-rw-r--r--   0        0        0     4056 2023-06-02 18:32:17.215271 fietsboek-0.8.0/fietsboek/hittekaart.py
+-rw-r--r--   0        0        0     3698 2023-04-13 18:12:32.568709 fietsboek-0.8.0/fietsboek/jinja2.py
+-rw-r--r--   0        0        0    14476 2023-05-31 19:16:57.788790 fietsboek-0.8.0/fietsboek/locale/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    24955 2023-05-31 19:16:57.789790 fietsboek-0.8.0/fietsboek/locale/de/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0      484 2022-07-07 11:19:31.236253 fietsboek-0.8.0/fietsboek/locale/de/html/home.html
+-rw-r--r--   0        0        0    13505 2023-05-31 19:16:57.789790 fietsboek-0.8.0/fietsboek/locale/en/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    23949 2023-05-31 19:16:57.790790 fietsboek-0.8.0/fietsboek/locale/en/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0      439 2022-07-07 11:17:06.866340 fietsboek-0.8.0/fietsboek/locale/en/html/home.html
+-rw-r--r--   0        0        0    20222 2023-05-31 19:16:57.791790 fietsboek-0.8.0/fietsboek/locale/fietslog.pot
+-rw-r--r--   0        0        0     4991 2022-12-29 14:02:02.545329 fietsboek-0.8.0/fietsboek/models/__init__.py
+-rw-r--r--   0        0        0     1770 2023-06-02 17:51:09.655921 fietsboek-0.8.0/fietsboek/models/badge.py
+-rw-r--r--   0        0        0     1427 2023-06-02 17:48:17.227377 fietsboek-0.8.0/fietsboek/models/comment.py
+-rw-r--r--   0        0        0     2061 2023-06-02 17:48:00.727228 fietsboek-0.8.0/fietsboek/models/image.py
+-rw-r--r--   0        0        0      732 2023-03-07 19:07:19.490784 fietsboek-0.8.0/fietsboek/models/meta.py
+-rw-r--r--   0        0        0    29507 2023-06-02 18:40:04.354872 fietsboek-0.8.0/fietsboek/models/track.py
+-rw-r--r--   0        0        0    16939 2023-06-02 18:07:29.693912 fietsboek-0.8.0/fietsboek/models/user.py
+-rw-r--r--   0        0        0     7386 2023-01-25 17:19:24.857216 fietsboek-0.8.0/fietsboek/pages.py
+-rw-r--r--   0        0        0      462 2022-12-13 21:14:10.397413 fietsboek-0.8.0/fietsboek/pshell.py
+-rw-r--r--   0        0        0     2848 2023-05-31 19:16:57.792790 fietsboek-0.8.0/fietsboek/routes.py
+-rw-r--r--   0        0        0     1707 2023-04-12 21:05:27.149201 fietsboek-0.8.0/fietsboek/scripts/__init__.py
+-rw-r--r--   0        0        0     5873 2023-06-02 19:07:31.657561 fietsboek-0.8.0/fietsboek/scripts/fietscron.py
+-rw-r--r--   0        0        0    14808 2023-05-31 19:16:44.775795 fietsboek-0.8.0/fietsboek/scripts/fietsctl.py
+-rw-r--r--   0        0        0     3663 2022-12-29 14:02:02.535329 fietsboek-0.8.0/fietsboek/security.py
+-rw-r--r--   0        0        0     3033 2023-02-06 18:03:03.267372 fietsboek-0.8.0/fietsboek/static/GM_Utils/GPX2GM.css
+-rw-r--r--   0        0        0   111993 2023-02-06 18:03:03.270372 fietsboek-0.8.0/fietsboek/static/GM_Utils/GPX2GM.js
+-rw-r--r--   0        0        0    32768 2023-02-06 18:03:03.271372 fietsboek-0.8.0/fietsboek/static/GM_Utils/GPX2GM_Defs.js
+-rw-r--r--   0        0        0      147 2023-02-06 18:03:03.276372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/Grau256x256.png
+-rw-r--r--   0        0        0     7209 2023-02-06 18:03:03.277372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/Loading_icon.gif
+-rw-r--r--   0        0        0    17490 2023-02-06 18:03:03.278372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/Loading_icon_V1.gif
+-rw-r--r--   0        0        0     1775 2023-02-06 18:03:03.280372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/Loading_icon_V2.gif
+-rw-r--r--   0        0        0      877 2023-02-06 18:03:03.284372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/airport.png
+-rw-r--r--   0        0        0      698 2023-02-06 18:03:03.285372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/bar.png
+-rw-r--r--   0        0        0      873 2023-02-06 18:03:03.285372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/boat.png
+-rw-r--r--   0        0        0      624 2023-02-06 18:03:03.286372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/bridge.png
+-rw-r--r--   0        0        0      715 2023-02-06 18:03:03.286372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/castle.png
+-rw-r--r--   0        0        0      648 2023-02-06 18:03:03.287372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/church2.png
+-rw-r--r--   0        0        0      428 2023-02-06 18:03:03.288372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/circle_green.svg
+-rw-r--r--   0        0        0      421 2023-02-06 18:03:03.288372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/circle_red.svg
+-rw-r--r--   0        0        0     1138 2023-02-06 18:03:03.289372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/cluster.png
+-rw-r--r--   0        0        0      604 2023-02-06 18:03:03.290372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/cluster.svg
+-rw-r--r--   0        0        0     1050 2023-02-06 18:03:03.291372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/current_location - Kopie.svg
+-rw-r--r--   0        0        0     1050 2023-02-06 18:03:03.291372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/current_location.svg
+-rw-r--r--   0        0        0     1270 2023-02-06 18:03:03.292372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/cycling.png
+-rw-r--r--   0        0        0      780 2023-02-06 18:03:03.292372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/finish.png
+-rw-r--r--   0        0        0      482 2023-02-06 18:03:03.293372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/flag.png
+-rw-r--r--   0        0        0      428 2023-02-06 18:03:03.293372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/fullscreen_m.svg
+-rw-r--r--   0        0        0      410 2023-02-06 18:03:03.295372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/fullscreen_p.svg
+-rw-r--r--   0        0        0      710 2023-02-06 18:03:03.295372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/harbor.png
+-rw-r--r--   0        0        0     1325 2023-02-06 18:03:03.296372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/hiking.png
+-rw-r--r--   0        0        0      309 2023-02-06 18:03:03.296372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/hotel.png
+-rw-r--r--   0        0        0      892 2023-02-06 18:03:03.297372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/hotel2.png
+-rw-r--r--   0        0        0     3311 2023-02-06 18:03:03.298372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/kreis.png
+-rw-r--r--   0        0        0      650 2023-02-06 18:03:03.298372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/library.png
+-rw-r--r--   0        0        0      204 2023-02-06 18:03:03.299372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/lupe_m.png
+-rw-r--r--   0        0        0      392 2023-02-06 18:03:03.299372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/lupe_m_32.png
+-rw-r--r--   0        0        0      200 2023-02-06 18:03:03.300372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/lupe_p.png
+-rw-r--r--   0        0        0      405 2023-02-06 18:03:03.300372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/lupe_p_32.png
+-rw-r--r--   0        0        0      645 2023-02-06 18:03:03.301372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/marker-icon_bw.png
+-rw-r--r--   0        0        0      495 2023-02-06 18:03:03.301372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/marker-icon_bw_41x25.png
+-rw-r--r--   0        0        0      345 2023-02-06 18:03:03.302372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/marker-icon_bw_small.png
+-rw-r--r--   0        0        0       77 2023-02-06 18:03:03.302372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/marker.gif
+-rw-r--r--   0        0        0      699 2023-02-06 18:03:03.303372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/marker.svg
+-rw-r--r--   0        0        0      849 2023-02-06 18:03:03.303372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/museum.png
+-rw-r--r--   0        0        0     1390 2023-02-06 18:03:03.304372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/panorama.png
+-rw-r--r--   0        0        0     1100 2023-02-06 18:03:03.304372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/park.png
+-rw-r--r--   0        0        0      545 2023-02-06 18:03:03.305372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/peak.png
+-rw-r--r--   0        0        0      720 2023-02-06 18:03:03.305372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/photo.png
+-rw-r--r--   0        0        0      642 2023-02-06 18:03:03.306372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/pin_red.png
+-rw-r--r--   0        0        0      650 2023-02-06 18:03:03.306372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/pin_red_shadow.png
+-rw-r--r--   0        0        0     1003 2023-02-06 18:03:03.307372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/restaurant.png
+-rw-r--r--   0        0        0      394 2023-02-06 18:03:03.308372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/scenic.png
+-rw-r--r--   0        0        0      770 2023-02-06 18:03:03.308372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/shadow.png
+-rw-r--r--   0        0        0      570 2023-02-06 18:03:03.308372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/shadow50.png
+-rw-r--r--   0        0        0      643 2023-02-06 18:03:03.309372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/shoppingmall.png
+-rw-r--r--   0        0        0      438 2023-02-06 18:03:03.309372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/square_green.svg
+-rw-r--r--   0        0        0      431 2023-02-06 18:03:03.310372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/square_red.svg
+-rw-r--r--   0        0        0      449 2023-02-06 18:03:03.310372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/start.png
+-rw-r--r--   0        0        0      603 2023-02-06 18:03:03.310372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/streckenmarker - Kopie.svg
+-rw-r--r--   0        0        0      603 2023-02-06 18:03:03.310372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/streckenmarker.svg
+-rw-r--r--   0        0        0      795 2023-02-06 18:03:03.311372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/subway.png
+-rw-r--r--   0        0        0      642 2023-02-06 18:03:03.311372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/tent.png
+-rw-r--r--   0        0        0      947 2023-02-06 18:03:03.311372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/train.png
+-rw-r--r--   0        0        0     1290 2023-02-06 18:03:03.312372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/video.png
+-rw-r--r--   0        0        0      626 2023-02-06 18:03:03.312372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/villa.png
+-rw-r--r--   0        0        0      657 2023-02-06 18:03:03.312372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/whereami.svg
+-rw-r--r--   0        0        0     1121 2023-02-06 18:03:03.313372 fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/whereami_V1.svg
+-rw-r--r--   0        0        0    37589 2023-02-06 18:03:03.314372 fietsboek-0.8.0/fietsboek/static/GM_Utils/gmutils.js
+-rw-r--r--   0        0        0     3736 2023-02-06 18:03:03.314372 fietsboek-0.8.0/fietsboek/static/GM_Utils/gra_canvas.js
+-rw-r--r--   0        0        0     6095 2023-02-06 18:03:03.314372 fietsboek-0.8.0/fietsboek/static/GM_Utils/gra_svg.js
+-rw-r--r--   0        0        0     1259 2022-10-04 14:03:38.000000 fietsboek-0.8.0/fietsboek/static/GM_Utils/leaflet/images/layers-2x.png
+-rw-r--r--   0        0        0      696 2022-10-04 14:03:38.000000 fietsboek-0.8.0/fietsboek/static/GM_Utils/leaflet/images/layers.png
+-rw-r--r--   0        0        0     2464 2022-10-04 14:03:38.000000 fietsboek-0.8.0/fietsboek/static/GM_Utils/leaflet/images/marker-icon-2x.png
+-rw-r--r--   0        0        0     1466 2022-10-04 14:03:38.000000 fietsboek-0.8.0/fietsboek/static/GM_Utils/leaflet/images/marker-icon.png
+-rw-r--r--   0        0        0      618 2022-10-04 14:03:38.000000 fietsboek-0.8.0/fietsboek/static/GM_Utils/leaflet/images/marker-shadow.png
+-rw-r--r--   0        0        0    14670 2022-10-04 14:03:38.000000 fietsboek-0.8.0/fietsboek/static/GM_Utils/leaflet/leaflet.css
+-rw-r--r--   0        0        0   146315 2022-10-04 14:05:32.000000 fietsboek-0.8.0/fietsboek/static/GM_Utils/leaflet/leaflet.js
+-rw-r--r--   0        0        0   223367 2022-10-04 14:05:32.000000 fietsboek-0.8.0/fietsboek/static/GM_Utils/leaflet/leaflet.js.map
+-rw-r--r--   0        0        0    39191 2023-02-06 18:03:03.315372 fietsboek-0.8.0/fietsboek/static/GM_Utils/osmutils.js
+-rw-r--r--   0        0        0    20687 2023-02-06 18:03:03.316372 fietsboek-0.8.0/fietsboek/static/GM_Utils/plot.js
+-rw-r--r--   0        0        0     3594 2023-02-06 18:03:03.316372 fietsboek-0.8.0/fietsboek/static/GM_Utils/shimg.js
+-rw-r--r--   0        0        0    93729 2023-04-24 18:24:31.965712 fietsboek-0.8.0/fietsboek/static/bootstrap-icons.css
+-rw-r--r--   0        0        0    80420 2023-04-24 18:24:31.965712 fietsboek-0.8.0/fietsboek/static/bootstrap.bundle.min.js
+-rw-r--r--   0        0        0   237950 2023-04-24 18:24:31.966712 fietsboek-0.8.0/fietsboek/static/bootstrap.css
+-rw-r--r--   0        0        0    25053 2022-06-30 00:22:45.000000 fietsboek-0.8.0/fietsboek/static/favicon.png
+-rw-r--r--   0        0        0    13942 2023-05-15 18:19:43.117312 fietsboek-0.8.0/fietsboek/static/fietsboek.js
+-rw-r--r--   0        0        0    11482 2023-05-15 18:19:43.118312 fietsboek-0.8.0/fietsboek/static/fietsboek.js.map
+-rw-r--r--   0        0        0   164360 2023-04-24 18:24:31.966712 fietsboek-0.8.0/fietsboek/static/fonts/bootstrap-icons.woff
+-rw-r--r--   0        0        0   121340 2023-04-24 18:24:31.966712 fietsboek-0.8.0/fietsboek/static/fonts/bootstrap-icons.woff2
+-rw-r--r--   0        0        0    20748 2022-07-04 18:57:32.170543 fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-300.woff
+-rw-r--r--   0        0        0    16812 2022-07-04 18:57:32.170543 fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-300.woff2
+-rw-r--r--   0        0        0    21928 2022-07-04 18:57:32.170543 fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-300italic.woff
+-rw-r--r--   0        0        0    17828 2022-07-04 18:57:32.170543 fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-300italic.woff2
+-rw-r--r--   0        0        0    20772 2022-07-04 18:57:32.171543 fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-500.woff
+-rw-r--r--   0        0        0    16812 2022-07-04 18:57:32.171543 fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-500.woff2
+-rw-r--r--   0        0        0    21868 2022-07-04 18:57:32.171543 fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-500italic.woff
+-rw-r--r--   0        0        0    17896 2022-07-04 18:57:32.171543 fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-500italic.woff2
+-rw-r--r--   0        0        0    20664 2022-07-04 18:57:32.172543 fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-600.woff
+-rw-r--r--   0        0        0    16796 2022-07-04 18:57:32.172543 fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-600.woff2
+-rw-r--r--   0        0        0    21812 2022-07-04 18:57:32.172543 fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-600italic.woff
+-rw-r--r--   0        0        0    17836 2022-07-04 18:57:32.172543 fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-600italic.woff2
+-rw-r--r--   0        0        0    20164 2022-07-04 18:57:32.173543 fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-700.woff
+-rw-r--r--   0        0        0    16360 2022-07-04 18:57:32.173543 fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-700.woff2
+-rw-r--r--   0        0        0    21244 2022-07-04 18:57:32.173543 fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-700italic.woff
+-rw-r--r--   0        0        0    17396 2022-07-04 18:57:32.174543 fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-700italic.woff2
+-rw-r--r--   0        0        0    20656 2022-07-04 18:57:32.174543 fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-800.woff
+-rw-r--r--   0        0        0    16724 2022-07-04 18:57:32.174543 fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-800.woff2
+-rw-r--r--   0        0        0    21520 2022-07-04 18:57:32.175543 fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-800italic.woff
+-rw-r--r--   0        0        0    17704 2022-07-04 18:57:32.175543 fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-800italic.woff2
+-rw-r--r--   0        0        0    21848 2022-07-04 18:57:32.175543 fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-italic.woff
+-rw-r--r--   0        0        0    17816 2022-07-04 18:57:32.176543 fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-italic.woff2
+-rw-r--r--   0        0        0    20704 2022-07-04 18:57:32.176543 fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-regular.woff
+-rw-r--r--   0        0        0    16720 2022-07-04 18:57:32.176543 fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-regular.woff2
+-rw-r--r--   0        0        0     4473 2022-07-04 18:57:32.169543 fietsboek-0.8.0/fietsboek/static/fonts.css
+-rw-r--r--   0        0        0    14075 2022-12-13 21:14:10.403414 fietsboek-0.8.0/fietsboek/static/osm-monkeypatch.js
+-rw-r--r--   0        0        0     2476 2023-05-31 19:16:44.776795 fietsboek-0.8.0/fietsboek/static/theme.css
+-rw-r--r--   0        0        0      650 2023-05-31 19:16:44.776795 fietsboek-0.8.0/fietsboek/static/theme.css.map
+-rw-r--r--   0        0        0     4795 2023-06-02 18:35:40.418284 fietsboek-0.8.0/fietsboek/summaries.py
+-rw-r--r--   0        0        0      280 2022-06-26 19:26:28.000000 fietsboek-0.8.0/fietsboek/templates/404.jinja2
+-rw-r--r--   0        0        0     2056 2022-07-14 14:18:13.964884 fietsboek-0.8.0/fietsboek/templates/admin.jinja2
+-rw-r--r--   0        0        0     9969 2023-05-15 18:19:43.120312 fietsboek-0.8.0/fietsboek/templates/browse.jinja2
+-rw-r--r--   0        0        0     2628 2022-12-13 21:14:10.405413 fietsboek-0.8.0/fietsboek/templates/create_account.jinja2
+-rw-r--r--   0        0        0     8519 2023-03-07 19:07:52.862105 fietsboek-0.8.0/fietsboek/templates/details.jinja2
+-rw-r--r--   0        0        0     1055 2022-12-13 21:14:10.410414 fietsboek-0.8.0/fietsboek/templates/edit.jinja2
+-rw-r--r--   0        0        0     9803 2023-03-07 19:07:52.863104 fietsboek-0.8.0/fietsboek/templates/edit_form.jinja2
+-rw-r--r--   0        0        0     1128 2022-12-13 21:14:10.411414 fietsboek-0.8.0/fietsboek/templates/finish_upload.jinja2
+-rw-r--r--   0        0        0     2617 2023-05-31 19:16:44.777795 fietsboek-0.8.0/fietsboek/templates/home.jinja2
+-rw-r--r--   0        0        0     6362 2023-05-31 19:16:44.777795 fietsboek-0.8.0/fietsboek/templates/layout.jinja2
+-rw-r--r--   0        0        0     1938 2023-05-31 19:16:57.792790 fietsboek-0.8.0/fietsboek/templates/login.jinja2
+-rw-r--r--   0        0        0     1479 2022-07-14 14:18:13.965884 fietsboek-0.8.0/fietsboek/templates/password_reset.jinja2
+-rw-r--r--   0        0        0     5894 2023-04-13 18:12:32.578709 fietsboek-0.8.0/fietsboek/templates/profile.jinja2
+-rw-r--r--   0        0        0      766 2022-07-14 14:18:13.966884 fietsboek-0.8.0/fietsboek/templates/request_password.jinja2
+-rw-r--r--   0        0        0      780 2023-05-31 19:16:57.792790 fietsboek-0.8.0/fietsboek/templates/resend_verification.jinja2
+-rw-r--r--   0        0        0      171 2022-12-13 21:14:10.413414 fietsboek-0.8.0/fietsboek/templates/static-page.jinja2
+-rw-r--r--   0        0        0      603 2022-07-14 14:18:13.966884 fietsboek-0.8.0/fietsboek/templates/upload.jinja2
+-rw-r--r--   0        0        0     3832 2023-04-13 18:12:32.579709 fietsboek-0.8.0/fietsboek/templates/user_data.jinja2
+-rw-r--r--   0        0        0      318 2022-07-14 14:18:13.966884 fietsboek-0.8.0/fietsboek/templates/util.jinja2
+-rw-r--r--   0        0        0     4926 2023-05-22 20:39:44.459891 fietsboek-0.8.0/fietsboek/transformers/__init__.py
+-rw-r--r--   0        0        0     4085 2023-04-24 18:24:31.971712 fietsboek-0.8.0/fietsboek/transformers/breaks.py
+-rw-r--r--   0        0        0     4456 2023-05-22 20:39:44.460891 fietsboek-0.8.0/fietsboek/transformers/elevation.py
+-rw-r--r--   0        0        0    15166 2023-04-12 21:05:27.159201 fietsboek-0.8.0/fietsboek/updater/__init__.py
+-rw-r--r--   0        0        0     6574 2023-03-26 20:32:32.915788 fietsboek-0.8.0/fietsboek/updater/cli.py
+-rw-r--r--   0        0        0     1087 2022-12-14 21:36:27.533733 fietsboek-0.8.0/fietsboek/updater/script.py
+-rw-r--r--   0        0        0     2378 2023-01-10 20:57:15.559281 fietsboek-0.8.0/fietsboek/updater/scripts/upd_20230103_lu8w3rwlz4ddcpms.py
+-rw-r--r--   0        0        0      475 2023-01-12 19:33:34.761460 fietsboek-0.8.0/fietsboek/updater/scripts/upd_20230112_v0.5.0.py
+-rw-r--r--   0        0        0      465 2023-03-08 18:25:33.078353 fietsboek-0.8.0/fietsboek/updater/scripts/upd_20230308_v0.6.0.py
+-rw-r--r--   0        0        0      465 2023-04-24 18:26:24.398858 fietsboek-0.8.0/fietsboek/updater/scripts/upd_20230424_v0.7.0.py
+-rw-r--r--   0        0        0      465 2023-06-05 19:05:41.679195 fietsboek-0.8.0/fietsboek/updater/scripts/upd_20230605_v0.8.0.py
+-rw-r--r--   0        0        0     2104 2022-12-29 14:02:02.591329 fietsboek-0.8.0/fietsboek/updater/scripts/upd_30ppwg8zi4ujb46f.py
+-rw-r--r--   0        0        0      454 2022-12-13 21:14:10.416414 fietsboek-0.8.0/fietsboek/updater/scripts/upd_initial.py
+-rw-r--r--   0        0        0      466 2022-12-13 21:14:10.417414 fietsboek-0.8.0/fietsboek/updater/scripts/upd_v0.4.0.py
+-rw-r--r--   0        0        0    15418 2023-06-02 18:44:14.706240 fietsboek-0.8.0/fietsboek/util.py
+-rw-r--r--   0        0        0        0 2022-06-26 19:26:27.000000 fietsboek-0.8.0/fietsboek/views/__init__.py
+-rw-r--r--   0        0        0     2245 2023-05-31 19:16:57.793790 fietsboek-0.8.0/fietsboek/views/account.py
+-rw-r--r--   0        0        0     2828 2022-12-29 14:02:02.572329 fietsboek-0.8.0/fietsboek/views/admin.py
+-rw-r--r--   0        0        0    15572 2023-06-02 19:14:24.818521 fietsboek-0.8.0/fietsboek/views/browse.py
+-rw-r--r--   0        0        0     9500 2023-05-31 19:16:57.793790 fietsboek-0.8.0/fietsboek/views/default.py
+-rw-r--r--   0        0        0     7231 2023-05-31 19:16:44.779795 fietsboek-0.8.0/fietsboek/views/detail.py
+-rw-r--r--   0        0        0     3553 2023-03-07 19:11:04.652006 fietsboek-0.8.0/fietsboek/views/edit.py
+-rw-r--r--   0        0        0      404 2022-12-13 21:14:10.420414 fietsboek-0.8.0/fietsboek/views/notfound.py
+-rw-r--r--   0        0        0     7846 2023-05-31 19:16:44.780795 fietsboek-0.8.0/fietsboek/views/profile.py
+-rw-r--r--   0        0        0    14574 2023-03-08 18:45:52.332655 fietsboek-0.8.0/fietsboek/views/tileproxy.py
+-rw-r--r--   0        0        0     7258 2023-05-31 19:17:03.317788 fietsboek-0.8.0/fietsboek/views/upload.py
+-rw-r--r--   0        0        0     5737 2023-04-13 18:12:32.583709 fietsboek-0.8.0/fietsboek/views/user_data.py
+-rw-r--r--   0        0        0     2340 2023-06-05 18:56:38.304813 fietsboek-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     4677 1970-01-01 00:00:00.000000 fietsboek-0.8.0/PKG-INFO
```

### Comparing `fietsboek-0.7.0/LICENSE.txt` & `fietsboek-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/README.md` & `fietsboek-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/__init__.py` & `fietsboek-0.8.0/fietsboek/__init__.py`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/alembic/env.py` & `fietsboek-0.8.0/fietsboek/alembic/env.py`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/alembic/versions/20220702_1b4b1c179e5a.py` & `fietsboek-0.8.0/fietsboek/alembic/versions/20220702_1b4b1c179e5a.py`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/alembic/versions/20220706_c89d9bdbfa68.py` & `fietsboek-0.8.0/fietsboek/alembic/versions/20220706_c89d9bdbfa68.py`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/alembic/versions/20220721_091ce24409fe.py` & `fietsboek-0.8.0/fietsboek/alembic/versions/20220721_091ce24409fe.py`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/alembic/versions/20220808_d085998b49ca.py` & `fietsboek-0.8.0/fietsboek/alembic/versions/20220808_d085998b49ca.py`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/alembic/versions/20221214_c939800af428.py` & `fietsboek-0.8.0/fietsboek/alembic/versions/20221214_c939800af428.py`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/alembic/versions/20230203_3149aa2d0114.py` & `fietsboek-0.8.0/fietsboek/alembic/versions/20230203_3149aa2d0114.py`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/config.py` & `fietsboek-0.8.0/fietsboek/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,14 +197,20 @@
 
     hittekaart_bin: str = Field("", alias="hittekaart.bin")
     """Path to the hittekaart binary."""
 
     hittekaart_autogenerate: PyramidList = Field([], alias="hittekaart.autogenerate")
     """Overlay maps to automatically generate."""
 
+    hittekaart_threads: int = Field(0, alias="hittekaart.threads")
+    """Number of threads that hittekaart should use.
+
+    Defaults to 0, which makes it use as many threads as there are CPU cores.
+    """
+
     @validator("session_key")
     def _good_session_key(cls, value):
         """Ensures that the session key has been changed from its default
         value.
         """
         if value == "<EDIT THIS>":
             raise ValueError("You need to edit the default session key!")
```

### Comparing `fietsboek-0.7.0/fietsboek/data.py` & `fietsboek-0.8.0/fietsboek/data.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 """Data manager for fietsboek.
 
 Data are objects that belong to a track (such as images), but are not stored in
 the database itself. This module makes access to such data objects easier.
 """
 import datetime
 import logging
+import os
 import random
 import shutil
 import string
 import uuid
 from pathlib import Path
 from typing import BinaryIO, List, Literal, Optional
 
 import brotli
 import gpxpy
 from filelock import FileLock
 
-from .util import secure_filename
+from . import util
 
 LOGGER = logging.getLogger(__name__)
 
 
 def generate_filename(filename: Optional[str]) -> str:
     """Generates a safe-to-use filename for uploads.
 
     If possible, tries to keep parts of the original filename intact, such as
     the extension.
 
     :param filename: The original filename.
     :return: The generated filename.
     """
     if filename:
-        good_name = secure_filename(filename)
+        good_name = util.secure_filename(filename)
         if good_name:
             random_prefix = "".join(random.choice(string.ascii_lowercase) for _ in range(5))
             return f"{random_prefix}_{good_name}"
 
     return str(uuid.uuid4())
 
 
@@ -238,14 +239,24 @@
             if self.path.is_dir():
                 shutil.rmtree(self.path, ignore_errors=False, onerror=self._log_deletion_error)
         else:
             new_name = self.path.with_name("trash-" + self.path.name)
             shutil.move(self.path, new_name)
             self.journal.append(("purge", new_name))
 
+    def size(self) -> int:
+        """Returns the size of the data that this track entails.
+
+        :return: The size of bytes that this track consumes.
+        """
+        size = 0
+        for root, _, files in os.walk(self.path):
+            size += sum(os.path.getsize(os.path.join(root, fname)) for fname in files)
+        return size
+
     def gpx_path(self) -> Path:
         """Returns the path of the GPX file.
 
         This file contains the (brotli) compressed GPX data.
 
         :return: The path where the GPX is supposed to be.
         """
@@ -279,24 +290,27 @@
 
         :return: The saved GPX file, decompressed.
         """
         return brotli.decompress(self.gpx_path().read_bytes())
 
     def engrave_metadata(
         self,
-        title: str,
-        description: str,
-        author_name: str,
-        time: datetime.datetime,
+        title: Optional[str],
+        description: Optional[str],
+        author_name: Optional[str],
+        time: Optional[datetime.datetime],
         *,
         gpx: Optional[gpxpy.gpx.GPX] = None,
     ):
         """Engrave the given metadata into the GPX file.
 
-        Note that this will erase all existing metadata in the given fields.
+        Note that this will overwrite all existing metadata in the given
+        fields.
+
+        If ``None`` is given, it will erase that specific part of the metadata.
 
         :param title: The title of the track.
         :param description: The description of the track.
         :param creator: Name of the track's creator.
         :param time: Time of the track.
         :param gpx: The pre-parsed GPX track, to save time if it is already parsed.
         """
@@ -309,15 +323,15 @@
 
         # Now we add the new metadata
         gpx.author_name = author_name
         gpx.name = title
         gpx.description = description
         gpx.time = time
 
-        self.compress_gpx(gpx.to_xml().encode("utf-8"))
+        self.compress_gpx(util.encode_gpx(gpx))
 
     def backup(self):
         """Create a backup of the GPX file."""
         shutil.copy(self.gpx_path(), self.backup_path())
 
     def backup_path(self) -> Path:
         """Path of the GPX backup file.
@@ -341,15 +355,15 @@
     def image_path(self, image_id: str) -> Path:
         """Returns a path to a saved image.
 
         :raises FileNotFoundError: If the given image could not be found.
         :param image_id: ID of the image.
         :return: A path pointing to the requested image.
         """
-        image = self.path / "images" / secure_filename(image_id)
+        image = self.path / "images" / util.secure_filename(image_id)
         if not image.exists():
             raise FileNotFoundError("The requested image does not exist")
         return image
 
     def add_image(self, image: BinaryIO, filename: Optional[str] = None) -> str:
         """Saves an image to a track.
 
@@ -373,15 +387,15 @@
     def delete_image(self, image_id: str):
         """Deletes an image from a track.
 
         :raises FileNotFoundError: If the given image could not be found.
         :param image_id: ID of the image.
         """
         # Be sure to not delete anything else than the image file
-        image_id = secure_filename(image_id)
+        image_id = util.secure_filename(image_id)
         if "/" in image_id or "\\" in image_id:
             return
         path = self.image_path(image_id)
 
         if self.journal is not None:
             self.journal.append(("delete_image", path, path.read_bytes()))
```

### Comparing `fietsboek-0.7.0/fietsboek/email.py` & `fietsboek-0.8.0/fietsboek/email.py`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/hittekaart.py` & `fietsboek-0.8.0/fietsboek/hittekaart.py`

 * *Files 9% similar despite different names*

```diff
@@ -93,25 +93,32 @@
 
     This function automatically retrieves the user's tracks from the database
     and passes them to ``hittekaart``.
 
     The output is saved in the user's data directory using the
     ``data_manager``.
 
+    :raises ValueError: If the user does not have an ID and thus the map cannot
+        be saved.
     :param user: The user for which to generate the map.
     :param dbsession: The database session.
     :param data_manager: The data manager.
     :param mode: The mode of the heatmap.
     :param exe_path: See :meth:`generate`.
     :param threads: See :meth:`generate`.
     """
+    if user.id is None:
+        raise ValueError("User has no ID, cannot generate a heatmap yet")
+
     query = user.all_tracks_query()
     query = select(aliased(models.Track, query)).where(query.c.type == TrackType.ORGANIC)
     input_paths = []
     for track in dbsession.execute(query).scalars():
+        if track.id is None:
+            continue
         path = data_manager.open(track.id).gpx_path()
         input_paths.append(path)
 
     if not input_paths:
         return
 
     try:
```

### Comparing `fietsboek-0.7.0/fietsboek/jinja2.py` & `fietsboek-0.8.0/fietsboek/jinja2.py`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/locale/de/LC_MESSAGES/messages.mo` & `fietsboek-0.8.0/fietsboek/locale/de/LC_MESSAGES/messages.mo`

 * *Files 11% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,21 +1,21 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-04-23 10:47+0200\n"
+"POT-Creation-Date: 2023-05-31 20:46+0200\n"
 "PO-Revision-Date: 2022-07-02 17:35+0200\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: de\n"
 "Language-Team: de <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "email.verify.text"
 msgstr ""
 "Um Dein Fietsboek-Konto zu bestätigen, nutze diesen Link: {}\n"
 "\n"
 "Falls Du kein Konto angelegt hast, ignoriere diese E-Mail."
 
@@ -78,26 +78,35 @@
 
 msgid "flash.password_updated"
 msgstr "Passwort aktualisiert"
 
 msgid "flash.personal_data_updated"
 msgstr "Persönliche Daten wurden gespeichert"
 
+msgid "flash.resend_verification_email_fail"
+msgstr "Ungültige E-Mail-Adresse angegeben"
+
 msgid "flash.reset_invalid_email"
 msgstr "Ungültige E-Mail-Adresse angegeben"
 
+msgid "flash.token_expired"
+msgstr "Der Link ist nicht mehr gültig"
+
 msgid "flash.track_deleted"
 msgstr "Strecke gelöscht"
 
 msgid "flash.upload_cancelled"
 msgstr "Hochladen abgebrochen"
 
 msgid "flash.upload_success"
 msgstr "Hochladen erfolgreich"
 
+msgid "flash.verification_token_generated"
+msgstr "Ein Link zur Bestätigung Deines Kontos wurde versandt"
+
 msgid "page.admin.badge.delete_badge"
 msgstr "Löschen"
 
 msgid "page.admin.badge.edit"
 msgstr "Bearbeiten"
 
 msgid "page.admin.badges"
@@ -170,14 +179,23 @@
 msgstr ""
 "Es wurden keine Strecken gefunden, auf die Du Zugriff hast. Versuche, Dich "
 "anzumelden."
 
 msgid "page.browse.organic_tooltip"
 msgstr "Dies ist eine Aufnahme einer Strecke"
 
+msgid "page.browse.sort.date"
+msgstr "Nach Datum sortieren"
+
+msgid "page.browse.sort.duration"
+msgstr "Nach Dauer sortieren"
+
+msgid "page.browse.sort.length"
+msgstr "Nach Länge sortieren"
+
 msgid "page.browse.synthetic_tooltip"
 msgstr "Dies ist eine geplante Strecke"
 
 msgid "page.browse.title"
 msgstr "Stöbern"
 
 msgid "page.create_account.create"
@@ -334,14 +352,17 @@
 
 msgid "page.login.password"
 msgstr "Passwort"
 
 msgid "page.login.remember-me"
 msgstr "Eingeloggt bleiben"
 
+msgid "page.login.resend_verification"
+msgstr "Bestätigungsmail erneut senden"
+
 msgid "page.login.submit"
 msgstr "Anmelden"
 
 msgid "page.login.title"
 msgstr "Anmelden"
 
 msgid "page.my_profile.accept_friend"
@@ -504,14 +525,27 @@
 
 msgid "page.request_password.request"
 msgstr "Anfrage senden"
 
 msgid "page.request_password.title"
 msgstr "Passwortzurücksetzung Beantragen"
 
+msgid "page.resend_verification.email"
+msgstr "E-Mail-Adresse"
+
+msgid "page.resend_verification.info"
+msgstr ""
+"Hier kannst Du eine neue E-Mail zur Bestätigung Deines Kontos anfordern."
+
+msgid "page.resend_verification.request"
+msgstr "E-Mail anfordern"
+
+msgid "page.resend_verification.title"
+msgstr "Bestätigungsmail Erneut Senden"
+
 msgid "page.track.form.add_friend"
 msgstr "Freund suchen"
 
 msgid "page.track.form.add_tag"
 msgstr "Schlagwort hinzufügen"
 
 msgid "page.track.form.badges"
@@ -614,14 +648,22 @@
 
 msgid "tooltip.table.stopped_time"
 msgstr "Haltezeit"
 
 msgid "tooltip.table.uphill"
 msgstr "Bergauf"
 
+msgid "transformers.fix-elevation-jumps"
+msgstr "Höhensprünge beheben"
+
+msgid "transformers.fix-elevation-jumps.description"
+msgstr ""
+"Diese Transformation passt die Höhenangabe für Punkte an, bei denen die Höhe "
+"sprunghaft steigt oder fällt."
+
 msgid "transformers.fix-null-elevation.description"
 msgstr ""
 "Diese Transformation passt die Höhenangabe für Punkte an, bei denen die "
 "Höhenangabe fehlt."
 
 msgid "transformers.fix-null-elevation.title"
 msgstr "Nullhöhen beheben"
```

### Comparing `fietsboek-0.7.0/fietsboek/locale/de/LC_MESSAGES/messages.po` & `fietsboek-0.8.0/fietsboek/locale/de/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,30 +3,41 @@
 # This file is distributed under the same license as the Fietsboek project.
 # Daniel Schadt, 2022.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-04-23 10:47+0200\n"
+"POT-Creation-Date: 2023-05-31 20:46+0200\n"
 "PO-Revision-Date: 2022-07-02 17:35+0200\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: de\n"
 "Language-Team: de <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
-#: fietsboek/util.py:280
+#: fietsboek/actions.py:250
+msgid "email.verify_mail.subject"
+msgstr "Fietsboek Konto Bestätigung"
+
+#: fietsboek/actions.py:253
+msgid "email.verify.text"
+msgstr ""
+"Um Dein Fietsboek-Konto zu bestätigen, nutze diesen Link: {}\n"
+"\n"
+"Falls Du kein Konto angelegt hast, ignoriere diese E-Mail."
+
+#: fietsboek/util.py:304
 msgid "password_constraint.mismatch"
 msgstr "Passwörter stimmen nicht überein"
 
-#: fietsboek/util.py:282
+#: fietsboek/util.py:306
 msgid "password_constraint.length"
 msgstr "Passwort zu kurz"
 
 #: fietsboek/models/track.py:579
 msgid "tooltip.table.length"
 msgstr "Länge"
 
@@ -142,81 +153,93 @@
 msgid "page.browse.filters.clear_all"
 msgstr "Filter zurücksetzen"
 
 #: fietsboek/templates/browse.jinja2:105
 msgid "page.browse.filters.expand_advanced"
 msgstr "Erweitert"
 
-#: fietsboek/templates/browse.jinja2:122
+#: fietsboek/templates/browse.jinja2:110 fietsboek/templates/browse.jinja2:111
+msgid "page.browse.sort.date"
+msgstr "Nach Datum sortieren"
+
+#: fietsboek/templates/browse.jinja2:112 fietsboek/templates/browse.jinja2:113
+msgid "page.browse.sort.length"
+msgstr "Nach Länge sortieren"
+
+#: fietsboek/templates/browse.jinja2:114 fietsboek/templates/browse.jinja2:115
+msgid "page.browse.sort.duration"
+msgstr "Nach Dauer sortieren"
+
+#: fietsboek/templates/browse.jinja2:132
 msgid "page.browse.organic_tooltip"
 msgstr "Dies ist eine Aufnahme einer Strecke"
 
-#: fietsboek/templates/browse.jinja2:124
+#: fietsboek/templates/browse.jinja2:134
 msgid "page.browse.synthetic_tooltip"
 msgstr "Dies ist eine geplante Strecke"
 
-#: fietsboek/templates/browse.jinja2:132 fietsboek/templates/details.jinja2:90
+#: fietsboek/templates/browse.jinja2:142 fietsboek/templates/details.jinja2:90
 #: fietsboek/templates/profile.jinja2:15
 msgid "page.details.date"
 msgstr "Datum"
 
-#: fietsboek/templates/browse.jinja2:134 fietsboek/templates/details.jinja2:104
+#: fietsboek/templates/browse.jinja2:144 fietsboek/templates/details.jinja2:104
 #: fietsboek/templates/profile.jinja2:17
 msgid "page.details.length"
 msgstr "Länge"
 
-#: fietsboek/templates/browse.jinja2:139 fietsboek/templates/details.jinja2:95
+#: fietsboek/templates/browse.jinja2:149 fietsboek/templates/details.jinja2:95
 #: fietsboek/templates/profile.jinja2:21
 msgid "page.details.start_time"
 msgstr "Startzeit"
 
-#: fietsboek/templates/browse.jinja2:141 fietsboek/templates/details.jinja2:99
+#: fietsboek/templates/browse.jinja2:151 fietsboek/templates/details.jinja2:99
 #: fietsboek/templates/profile.jinja2:23
 msgid "page.details.end_time"
 msgstr "Endzeit"
 
-#: fietsboek/templates/browse.jinja2:146 fietsboek/templates/details.jinja2:108
+#: fietsboek/templates/browse.jinja2:156 fietsboek/templates/details.jinja2:108
 #: fietsboek/templates/profile.jinja2:27
 msgid "page.details.uphill"
 msgstr "Bergauf"
 
-#: fietsboek/templates/browse.jinja2:148 fietsboek/templates/details.jinja2:112
+#: fietsboek/templates/browse.jinja2:158 fietsboek/templates/details.jinja2:112
 #: fietsboek/templates/profile.jinja2:29
 msgid "page.details.downhill"
 msgstr "Bergab"
 
-#: fietsboek/templates/browse.jinja2:153 fietsboek/templates/details.jinja2:117
+#: fietsboek/templates/browse.jinja2:163 fietsboek/templates/details.jinja2:117
 #: fietsboek/templates/profile.jinja2:33
 msgid "page.details.moving_time"
 msgstr "Fahrzeit"
 
-#: fietsboek/templates/browse.jinja2:155 fietsboek/templates/details.jinja2:121
+#: fietsboek/templates/browse.jinja2:165 fietsboek/templates/details.jinja2:121
 #: fietsboek/templates/profile.jinja2:35
 msgid "page.details.stopped_time"
 msgstr "Haltezeit"
 
-#: fietsboek/templates/browse.jinja2:159 fietsboek/templates/details.jinja2:125
+#: fietsboek/templates/browse.jinja2:169 fietsboek/templates/details.jinja2:125
 #: fietsboek/templates/profile.jinja2:39
 msgid "page.details.max_speed"
 msgstr "maximale Geschwindigkeit"
 
-#: fietsboek/templates/browse.jinja2:161 fietsboek/templates/details.jinja2:129
+#: fietsboek/templates/browse.jinja2:171 fietsboek/templates/details.jinja2:129
 #: fietsboek/templates/profile.jinja2:41
 msgid "page.details.avg_speed"
 msgstr "durchschnittliche Geschwindigkeit"
 
-#: fietsboek/templates/browse.jinja2:179
+#: fietsboek/templates/browse.jinja2:189
 msgid "page.browse.download_multiple"
 msgstr "ausgewählte Herunterladen"
 
-#: fietsboek/templates/browse.jinja2:181
+#: fietsboek/templates/browse.jinja2:191
 msgid "page.browse.no_results"
 msgstr "Es wurden keine Strecken gefunden, die den Filtern entsprechen."
 
-#: fietsboek/templates/browse.jinja2:183
+#: fietsboek/templates/browse.jinja2:193
 msgid "page.browse.no_tracks"
 msgstr ""
 "Es wurden keine Strecken gefunden, auf die Du Zugriff hast. Versuche, "
 "Dich anzumelden."
 
 #: fietsboek/templates/create_account.jinja2:5
 msgid "page.create_account.title"
@@ -462,80 +485,80 @@
 msgid "page.upload.form.submit"
 msgstr "Absenden"
 
 #: fietsboek/templates/finish_upload.jinja2:17
 msgid "page.upload.form.cancel"
 msgstr "Abbrechen"
 
-#: fietsboek/templates/home.jinja2:5
+#: fietsboek/templates/home.jinja2:6
 msgid "page.home.title"
 msgstr "Startseite"
 
-#: fietsboek/templates/home.jinja2:8
+#: fietsboek/templates/home.jinja2:17
 msgid "page.home.unfinished_uploads"
 msgstr ""
 "Es sind noch nicht abgeschlossene Uploads vorhanden. Klicke auf die "
 "Links, um sie fortzusetzen:"
 
-#: fietsboek/templates/home.jinja2:22 fietsboek/templates/home.jinja2:29
-#: fietsboek/templates/home.jinja2:47
+#: fietsboek/templates/home.jinja2:31 fietsboek/templates/home.jinja2:38
+#: fietsboek/templates/home.jinja2:56
 msgid "page.home.summary.track"
 msgid_plural "page.home.summary.tracks"
 msgstr[0] "%(num)d Strecke"
 msgstr[1] "%(num)d Strecken"
 
-#: fietsboek/templates/home.jinja2:47
+#: fietsboek/templates/home.jinja2:56
 msgid "page.home.total"
 msgstr "Gesamt"
 
-#: fietsboek/templates/layout.jinja2:41
+#: fietsboek/templates/layout.jinja2:43
 msgid "page.navbar.toggle"
 msgstr "Navigation umschalten"
 
-#: fietsboek/templates/layout.jinja2:52
+#: fietsboek/templates/layout.jinja2:54
 msgid "page.navbar.home"
 msgstr "Startseite"
 
-#: fietsboek/templates/layout.jinja2:55
+#: fietsboek/templates/layout.jinja2:57
 msgid "page.navbar.browse"
 msgstr "Stöbern"
 
-#: fietsboek/templates/layout.jinja2:59
+#: fietsboek/templates/layout.jinja2:61
 msgid "page.navbar.upload"
 msgstr "Hochladen"
 
-#: fietsboek/templates/layout.jinja2:68
+#: fietsboek/templates/layout.jinja2:70
 msgid "page.navbar.user"
 msgstr "Nutzer"
 
-#: fietsboek/templates/layout.jinja2:72
+#: fietsboek/templates/layout.jinja2:74
 msgid "page.navbar.welcome_user"
 msgstr "Willkommen, {}!"
 
-#: fietsboek/templates/layout.jinja2:75
+#: fietsboek/templates/layout.jinja2:77
 msgid "page.navbar.logout"
 msgstr "Abmelden"
 
-#: fietsboek/templates/layout.jinja2:78
+#: fietsboek/templates/layout.jinja2:80
 msgid "page.navbar.profile"
 msgstr "Profil"
 
-#: fietsboek/templates/layout.jinja2:81
+#: fietsboek/templates/layout.jinja2:83
 msgid "page.navbar.user_data"
 msgstr "Persönliche Daten"
 
-#: fietsboek/templates/layout.jinja2:85
+#: fietsboek/templates/layout.jinja2:87
 msgid "page.navbar.admin"
 msgstr "Admin"
 
-#: fietsboek/templates/layout.jinja2:91
+#: fietsboek/templates/layout.jinja2:93
 msgid "page.navbar.login"
 msgstr "Anmelden"
 
-#: fietsboek/templates/layout.jinja2:95
+#: fietsboek/templates/layout.jinja2:97
 msgid "page.navbar.create_account"
 msgstr "Konto Erstellen"
 
 #: fietsboek/templates/login.jinja2:7
 msgid "page.login.title"
 msgstr "Anmelden"
 
@@ -555,14 +578,18 @@
 msgid "page.login.submit"
 msgstr "Anmelden"
 
 #: fietsboek/templates/login.jinja2:43
 msgid "page.login.forgot_password"
 msgstr "Passwort vergessen"
 
+#: fietsboek/templates/login.jinja2:45
+msgid "page.login.resend_verification"
+msgstr "Bestätigungsmail erneut senden"
+
 #: fietsboek/templates/password_reset.jinja2:5
 msgid "page.password_reset.title"
 msgstr "Passwort Zurücksetzen"
 
 #: fietsboek/templates/password_reset.jinja2:11
 msgid "page.password_reset.password"
 msgstr "Passwort"
@@ -653,14 +680,31 @@
 msgid "page.request_password.email"
 msgstr "E-Mail-Adresse"
 
 #: fietsboek/templates/request_password.jinja2:17
 msgid "page.request_password.request"
 msgstr "Anfrage senden"
 
+#: fietsboek/templates/resend_verification.jinja2:5
+msgid "page.resend_verification.title"
+msgstr "Bestätigungsmail Erneut Senden"
+
+#: fietsboek/templates/resend_verification.jinja2:6
+msgid "page.resend_verification.info"
+msgstr ""
+"Hier kannst Du eine neue E-Mail zur Bestätigung Deines Kontos anfordern."
+
+#: fietsboek/templates/resend_verification.jinja2:12
+msgid "page.resend_verification.email"
+msgstr "E-Mail-Adresse"
+
+#: fietsboek/templates/resend_verification.jinja2:17
+msgid "page.resend_verification.request"
+msgstr "E-Mail anfordern"
+
 #: fietsboek/templates/upload.jinja2:9
 msgid "page.upload.form.gpx"
 msgstr "GPX Datei"
 
 #: fietsboek/templates/user_data.jinja2:7
 msgid "page.my_profile.title"
 msgstr "Mein Profil"
@@ -709,53 +753,51 @@
 msgid "page.my_profile.friend_request_email"
 msgstr "E-Mail-Adresse des Freundes"
 
 #: fietsboek/templates/user_data.jinja2:77
 msgid "page.my_profile.send_friend_request"
 msgstr "Freundschaftsanfrage senden"
 
-#: fietsboek/transformers/__init__.py:140
+#: fietsboek/transformers/breaks.py:31
+msgid "transformers.remove-breaks.title"
+msgstr "Pausen entfernen"
+
+#: fietsboek/transformers/breaks.py:35
+msgid "transformers.remove-breaks.description"
+msgstr "Diese Transformation entfernt längere Pausen aus der Aufnahme."
+
+#: fietsboek/transformers/elevation.py:42
 msgid "transformers.fix-null-elevation.title"
 msgstr "Nullhöhen beheben"
 
-#: fietsboek/transformers/__init__.py:144
+#: fietsboek/transformers/elevation.py:46
 msgid "transformers.fix-null-elevation.description"
 msgstr ""
 "Diese Transformation passt die Höhenangabe für Punkte an, bei denen die "
 "Höhenangabe fehlt."
 
-#: fietsboek/transformers/breaks.py:31
-msgid "transformers.remove-breaks.title"
-msgstr "Pausen entfernen"
+#: fietsboek/transformers/elevation.py:115
+msgid "transformers.fix-elevation-jumps"
+msgstr "Höhensprünge beheben"
 
-#: fietsboek/transformers/breaks.py:35
-msgid "transformers.remove-breaks.description"
+#: fietsboek/transformers/elevation.py:119
+msgid "transformers.fix-elevation-jumps.description"
 msgstr ""
-"Diese Transformation entfernt längere Pausen aus der Aufnahme."
+"Diese Transformation passt die Höhenangabe für Punkte an, bei denen die "
+"Höhe sprunghaft steigt oder fällt."
 
-#: fietsboek/views/account.py:54
+#: fietsboek/views/account.py:53
 msgid "flash.invalid_name"
 msgstr "Ungültiger Name"
 
-#: fietsboek/views/account.py:59
+#: fietsboek/views/account.py:58
 msgid "flash.invalid_email"
 msgstr "Ungültige E-Mail-Adresse"
 
-#: fietsboek/views/account.py:72
-msgid "email.verify_mail.subject"
-msgstr "Fietsboek Konto Bestätigung"
-
-#: fietsboek/views/account.py:75
-msgid "email.verify.text"
-msgstr ""
-"Um Dein Fietsboek-Konto zu bestätigen, nutze diesen Link: {}\n"
-"\n"
-"Falls Du kein Konto angelegt hast, ignoriere diese E-Mail."
-
-#: fietsboek/views/account.py:86
+#: fietsboek/views/account.py:67
 msgid "flash.a_confirmation_link_has_been_sent"
 msgstr "Ein Bestätigungslink wurde versandt"
 
 #: fietsboek/views/admin.py:48
 msgid "flash.badge_added"
 msgstr "Wappen hinzugefügt"
 
@@ -763,59 +805,71 @@
 msgid "flash.badge_modified"
 msgstr "Wappen bearbeitet"
 
 #: fietsboek/views/admin.py:92
 msgid "flash.badge_deleted"
 msgstr "Wappen gelöscht"
 
-#: fietsboek/views/default.py:117
+#: fietsboek/views/default.py:115
 msgid "flash.invalid_credentials"
 msgstr "Ungültige Nutzerdaten"
 
-#: fietsboek/views/default.py:121
+#: fietsboek/views/default.py:119
 msgid "flash.account_not_verified"
 msgstr "Konto noch nicht bestätigt"
 
-#: fietsboek/views/default.py:124
+#: fietsboek/views/default.py:122
 msgid "flash.logged_in"
 msgstr "Du bist nun angemeldet"
 
-#: fietsboek/views/default.py:146
+#: fietsboek/views/default.py:142
 msgid "flash.logged_out"
 msgstr "Du bist nun abgemeldet"
 
-#: fietsboek/views/default.py:180
+#: fietsboek/views/default.py:172
 msgid "flash.reset_invalid_email"
 msgstr "Ungültige E-Mail-Adresse angegeben"
 
-#: fietsboek/views/default.py:185
+#: fietsboek/views/default.py:177
 msgid "flash.password_token_generated"
 msgstr "Ein Link zum Zurücksetzen des Passworts wurde versandt"
 
-#: fietsboek/views/default.py:190
+#: fietsboek/views/default.py:182
 msgid "page.password_reset.email.subject"
 msgstr "Fietsboek Passwortzurücksetzung"
 
-#: fietsboek/views/default.py:193
+#: fietsboek/views/default.py:185
 msgid "page.password_reset.email.body"
 msgstr ""
 "Du kannst Dein Fietsboek-Passwort hier zurücksetzen: {}\n"
 "\n"
 "Falls Du keine Passwortzurücksetzung beantragt hast, dann ignoriere diese"
 " E-Mail."
 
-#: fietsboek/views/default.py:226
+#: fietsboek/views/default.py:224
+msgid "flash.resend_verification_email_fail"
+msgstr "Ungültige E-Mail-Adresse angegeben"
+
+#: fietsboek/views/default.py:229
+msgid "flash.verification_token_generated"
+msgstr "Ein Link zur Bestätigung Deines Kontos wurde versandt"
+
+#: fietsboek/views/default.py:249
+msgid "flash.token_expired"
+msgstr "Der Link ist nicht mehr gültig"
+
+#: fietsboek/views/default.py:255
 msgid "flash.email_verified"
 msgstr "E-Mail-Adresse bestätigt"
 
-#: fietsboek/views/default.py:240
+#: fietsboek/views/default.py:269
 msgid "flash.password_updated"
 msgstr "Passwort aktualisiert"
 
-#: fietsboek/views/detail.py:140
+#: fietsboek/views/detail.py:155
 msgid "flash.track_deleted"
 msgstr "Strecke gelöscht"
 
 #: fietsboek/views/upload.py:52
 msgid "flash.no_file_selected"
 msgstr "Keine Datei ausgewählt"
```

### Comparing `fietsboek-0.7.0/fietsboek/locale/en/LC_MESSAGES/messages.mo` & `fietsboek-0.8.0/fietsboek/locale/en/LC_MESSAGES/messages.mo`

 * *Files 9% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,21 +1,21 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-04-23 10:47+0200\n"
+"POT-Creation-Date: 2023-05-31 20:46+0200\n"
 "PO-Revision-Date: 2023-04-03 20:42+0200\n"
 "Last-Translator: \n"
 "Language: en\n"
 "Language-Team: en <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "email.verify.text"
 msgstr ""
 "To verify your Fietsboek account, please use this link: {}\n"
 "\n"
 "If you did not create an account, ignore this email."
 
@@ -78,26 +78,35 @@
 
 msgid "flash.password_updated"
 msgstr "Password has been updated"
 
 msgid "flash.personal_data_updated"
 msgstr "Personal data has been updated"
 
+msgid "flash.resend_verification_email_fail"
+msgstr "Invalid email address provided"
+
 msgid "flash.reset_invalid_email"
 msgstr "Invalid email address provided"
 
+msgid "flash.token_expired"
+msgstr "The link has expired"
+
 msgid "flash.track_deleted"
 msgstr "Track has been deleted"
 
 msgid "flash.upload_cancelled"
 msgstr "Upload cancelled"
 
 msgid "flash.upload_success"
 msgstr "Upload successful"
 
+msgid "flash.verification_token_generated"
+msgstr "A verification email has been sent"
+
 msgid "page.admin.badge.delete_badge"
 msgstr "Delete badge"
 
 msgid "page.admin.badge.edit"
 msgstr "Edit"
 
 msgid "page.admin.badges"
@@ -168,14 +177,23 @@
 
 msgid "page.browse.no_tracks"
 msgstr "You currently do not have access to any tracks. Try logging in."
 
 msgid "page.browse.organic_tooltip"
 msgstr "This is a recording of a track"
 
+msgid "page.browse.sort.date"
+msgstr "Sort by date"
+
+msgid "page.browse.sort.duration"
+msgstr "Sort by duration"
+
+msgid "page.browse.sort.length"
+msgstr "Sort by length"
+
 msgid "page.browse.synthetic_tooltip"
 msgstr "This is a pre-planned track"
 
 msgid "page.browse.title"
 msgstr "Browse"
 
 msgid "page.create_account.create"
@@ -329,14 +347,17 @@
 
 msgid "page.login.password"
 msgstr "Password"
 
 msgid "page.login.remember-me"
 msgstr "Remember me"
 
+msgid "page.login.resend_verification"
+msgstr "Re-send verification mail"
+
 msgid "page.login.submit"
 msgstr "Login"
 
 msgid "page.login.title"
 msgstr "Login"
 
 msgid "page.my_profile.accept_friend"
@@ -496,14 +517,26 @@
 
 msgid "page.request_password.request"
 msgstr "Send request"
 
 msgid "page.request_password.title"
 msgstr "Request a Password Reset"
 
+msgid "page.resend_verification.email"
+msgstr "Email"
+
+msgid "page.resend_verification.info"
+msgstr "Here you can request a new mail to verify your account"
+
+msgid "page.resend_verification.request"
+msgstr "Send request"
+
+msgid "page.resend_verification.title"
+msgstr "Re-send Verification Mail"
+
 msgid "page.track.form.add_friend"
 msgstr "Search friends"
 
 msgid "page.track.form.add_tag"
 msgstr "Add Tag"
 
 msgid "page.track.form.badges"
@@ -606,14 +639,20 @@
 
 msgid "tooltip.table.stopped_time"
 msgstr "Stopped Time"
 
 msgid "tooltip.table.uphill"
 msgstr "Uphill"
 
+msgid "transformers.fix-elevation-jumps"
+msgstr "Fix elevation jumps"
+
+msgid "transformers.fix-elevation-jumps.description"
+msgstr "This transformer fixes abrupt jumps in the elevation value."
+
 msgid "transformers.fix-null-elevation.description"
 msgstr ""
 "This transformer fixes the elevation of points whose elevation is unset."
 
 msgid "transformers.fix-null-elevation.title"
 msgstr "Fix null elevation"
```

### Comparing `fietsboek-0.7.0/fietsboek/locale/en/LC_MESSAGES/messages.po` & `fietsboek-0.8.0/fietsboek/locale/en/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,30 +3,41 @@
 # This file is distributed under the same license as the Fietsboek project.
 # Daniel Schadt, 2022.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-04-23 10:47+0200\n"
+"POT-Creation-Date: 2023-05-31 20:46+0200\n"
 "PO-Revision-Date: 2023-04-03 20:42+0200\n"
 "Last-Translator: \n"
 "Language: en\n"
 "Language-Team: en <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
-#: fietsboek/util.py:280
+#: fietsboek/actions.py:250
+msgid "email.verify_mail.subject"
+msgstr "Fietsboek Account Verification"
+
+#: fietsboek/actions.py:253
+msgid "email.verify.text"
+msgstr ""
+"To verify your Fietsboek account, please use this link: {}\n"
+"\n"
+"If you did not create an account, ignore this email."
+
+#: fietsboek/util.py:304
 msgid "password_constraint.mismatch"
 msgstr "Passwords don't match"
 
-#: fietsboek/util.py:282
+#: fietsboek/util.py:306
 msgid "password_constraint.length"
 msgstr "Password not long enough"
 
 #: fietsboek/models/track.py:579
 msgid "tooltip.table.length"
 msgstr "Length"
 
@@ -142,81 +153,93 @@
 msgid "page.browse.filters.clear_all"
 msgstr "Remove filters"
 
 #: fietsboek/templates/browse.jinja2:105
 msgid "page.browse.filters.expand_advanced"
 msgstr "Advanced"
 
-#: fietsboek/templates/browse.jinja2:122
+#: fietsboek/templates/browse.jinja2:110 fietsboek/templates/browse.jinja2:111
+msgid "page.browse.sort.date"
+msgstr "Sort by date"
+
+#: fietsboek/templates/browse.jinja2:112 fietsboek/templates/browse.jinja2:113
+msgid "page.browse.sort.length"
+msgstr "Sort by length"
+
+#: fietsboek/templates/browse.jinja2:114 fietsboek/templates/browse.jinja2:115
+msgid "page.browse.sort.duration"
+msgstr "Sort by duration"
+
+#: fietsboek/templates/browse.jinja2:132
 msgid "page.browse.organic_tooltip"
 msgstr "This is a recording of a track"
 
-#: fietsboek/templates/browse.jinja2:124
+#: fietsboek/templates/browse.jinja2:134
 msgid "page.browse.synthetic_tooltip"
 msgstr "This is a pre-planned track"
 
-#: fietsboek/templates/browse.jinja2:132 fietsboek/templates/details.jinja2:90
+#: fietsboek/templates/browse.jinja2:142 fietsboek/templates/details.jinja2:90
 #: fietsboek/templates/profile.jinja2:15
 msgid "page.details.date"
 msgstr "Date"
 
-#: fietsboek/templates/browse.jinja2:134 fietsboek/templates/details.jinja2:104
+#: fietsboek/templates/browse.jinja2:144 fietsboek/templates/details.jinja2:104
 #: fietsboek/templates/profile.jinja2:17
 msgid "page.details.length"
 msgstr "Length"
 
-#: fietsboek/templates/browse.jinja2:139 fietsboek/templates/details.jinja2:95
+#: fietsboek/templates/browse.jinja2:149 fietsboek/templates/details.jinja2:95
 #: fietsboek/templates/profile.jinja2:21
 msgid "page.details.start_time"
 msgstr "Record Start"
 
-#: fietsboek/templates/browse.jinja2:141 fietsboek/templates/details.jinja2:99
+#: fietsboek/templates/browse.jinja2:151 fietsboek/templates/details.jinja2:99
 #: fietsboek/templates/profile.jinja2:23
 msgid "page.details.end_time"
 msgstr "Record End"
 
-#: fietsboek/templates/browse.jinja2:146 fietsboek/templates/details.jinja2:108
+#: fietsboek/templates/browse.jinja2:156 fietsboek/templates/details.jinja2:108
 #: fietsboek/templates/profile.jinja2:27
 msgid "page.details.uphill"
 msgstr "Uphill"
 
-#: fietsboek/templates/browse.jinja2:148 fietsboek/templates/details.jinja2:112
+#: fietsboek/templates/browse.jinja2:158 fietsboek/templates/details.jinja2:112
 #: fietsboek/templates/profile.jinja2:29
 msgid "page.details.downhill"
 msgstr "Downhill"
 
-#: fietsboek/templates/browse.jinja2:153 fietsboek/templates/details.jinja2:117
+#: fietsboek/templates/browse.jinja2:163 fietsboek/templates/details.jinja2:117
 #: fietsboek/templates/profile.jinja2:33
 msgid "page.details.moving_time"
 msgstr "Moving Time"
 
-#: fietsboek/templates/browse.jinja2:155 fietsboek/templates/details.jinja2:121
+#: fietsboek/templates/browse.jinja2:165 fietsboek/templates/details.jinja2:121
 #: fietsboek/templates/profile.jinja2:35
 msgid "page.details.stopped_time"
 msgstr "Stopped Time"
 
-#: fietsboek/templates/browse.jinja2:159 fietsboek/templates/details.jinja2:125
+#: fietsboek/templates/browse.jinja2:169 fietsboek/templates/details.jinja2:125
 #: fietsboek/templates/profile.jinja2:39
 msgid "page.details.max_speed"
 msgstr "Max Speed"
 
-#: fietsboek/templates/browse.jinja2:161 fietsboek/templates/details.jinja2:129
+#: fietsboek/templates/browse.jinja2:171 fietsboek/templates/details.jinja2:129
 #: fietsboek/templates/profile.jinja2:41
 msgid "page.details.avg_speed"
 msgstr "Average Speed"
 
-#: fietsboek/templates/browse.jinja2:179
+#: fietsboek/templates/browse.jinja2:189
 msgid "page.browse.download_multiple"
 msgstr "Download selected"
 
-#: fietsboek/templates/browse.jinja2:181
+#: fietsboek/templates/browse.jinja2:191
 msgid "page.browse.no_results"
 msgstr "No results matching the filters were found."
 
-#: fietsboek/templates/browse.jinja2:183
+#: fietsboek/templates/browse.jinja2:193
 msgid "page.browse.no_tracks"
 msgstr "You currently do not have access to any tracks. Try logging in."
 
 #: fietsboek/templates/create_account.jinja2:5
 msgid "page.create_account.title"
 msgstr "Create Account"
 
@@ -458,78 +481,78 @@
 msgid "page.upload.form.submit"
 msgstr "Upload"
 
 #: fietsboek/templates/finish_upload.jinja2:17
 msgid "page.upload.form.cancel"
 msgstr "Cancel"
 
-#: fietsboek/templates/home.jinja2:5
+#: fietsboek/templates/home.jinja2:6
 msgid "page.home.title"
 msgstr "Home"
 
-#: fietsboek/templates/home.jinja2:8
+#: fietsboek/templates/home.jinja2:17
 msgid "page.home.unfinished_uploads"
 msgstr "You have unfinished uploads. Click on the links below to resume them:"
 
-#: fietsboek/templates/home.jinja2:22 fietsboek/templates/home.jinja2:29
-#: fietsboek/templates/home.jinja2:47
+#: fietsboek/templates/home.jinja2:31 fietsboek/templates/home.jinja2:38
+#: fietsboek/templates/home.jinja2:56
 msgid "page.home.summary.track"
 msgid_plural "page.home.summary.tracks"
 msgstr[0] "%(num)d track"
 msgstr[1] "%(num)d tracks"
 
-#: fietsboek/templates/home.jinja2:47
+#: fietsboek/templates/home.jinja2:56
 msgid "page.home.total"
 msgstr "Total"
 
-#: fietsboek/templates/layout.jinja2:41
+#: fietsboek/templates/layout.jinja2:43
 msgid "page.navbar.toggle"
 msgstr "Toggle navigation"
 
-#: fietsboek/templates/layout.jinja2:52
+#: fietsboek/templates/layout.jinja2:54
 msgid "page.navbar.home"
 msgstr "Home"
 
-#: fietsboek/templates/layout.jinja2:55
+#: fietsboek/templates/layout.jinja2:57
 msgid "page.navbar.browse"
 msgstr "Browse"
 
-#: fietsboek/templates/layout.jinja2:59
+#: fietsboek/templates/layout.jinja2:61
 msgid "page.navbar.upload"
 msgstr "Upload"
 
-#: fietsboek/templates/layout.jinja2:68
+#: fietsboek/templates/layout.jinja2:70
 msgid "page.navbar.user"
 msgstr "User"
 
-#: fietsboek/templates/layout.jinja2:72
+#: fietsboek/templates/layout.jinja2:74
 msgid "page.navbar.welcome_user"
 msgstr "Welcome, {}!"
 
-#: fietsboek/templates/layout.jinja2:75
+#: fietsboek/templates/layout.jinja2:77
 msgid "page.navbar.logout"
 msgstr "Logout"
 
-#: fietsboek/templates/layout.jinja2:78
+#: fietsboek/templates/layout.jinja2:80
 msgid "page.navbar.profile"
 msgstr "Profile"
 
-#: fietsboek/templates/layout.jinja2:81
+#: fietsboek/templates/layout.jinja2:83
 msgid "page.navbar.user_data"
 msgstr "Personal Data"
 
-#: fietsboek/templates/layout.jinja2:85
+#: fietsboek/templates/layout.jinja2:87
 msgid "page.navbar.admin"
 msgstr "Admin"
 
-#: fietsboek/templates/layout.jinja2:91
+#: fietsboek/templates/layout.jinja2:93
 msgid "page.navbar.login"
 msgstr "Login"
 
-#: fietsboek/templates/layout.jinja2:95
+#: fietsboek/templates/layout.jinja2:97
 msgid "page.navbar.create_account"
 msgstr "Create Account"
 
 #: fietsboek/templates/login.jinja2:7
 msgid "page.login.title"
 msgstr "Login"
 
@@ -549,14 +572,18 @@
 msgid "page.login.submit"
 msgstr "Login"
 
 #: fietsboek/templates/login.jinja2:43
 msgid "page.login.forgot_password"
 msgstr "Forgot password"
 
+#: fietsboek/templates/login.jinja2:45
+msgid "page.login.resend_verification"
+msgstr "Re-send verification mail"
+
 #: fietsboek/templates/password_reset.jinja2:5
 msgid "page.password_reset.title"
 msgstr "Reset Your Password"
 
 #: fietsboek/templates/password_reset.jinja2:11
 msgid "page.password_reset.password"
 msgstr "Password"
@@ -647,14 +674,30 @@
 msgid "page.request_password.email"
 msgstr "Email"
 
 #: fietsboek/templates/request_password.jinja2:17
 msgid "page.request_password.request"
 msgstr "Send request"
 
+#: fietsboek/templates/resend_verification.jinja2:5
+msgid "page.resend_verification.title"
+msgstr "Re-send Verification Mail"
+
+#: fietsboek/templates/resend_verification.jinja2:6
+msgid "page.resend_verification.info"
+msgstr "Here you can request a new mail to verify your account"
+
+#: fietsboek/templates/resend_verification.jinja2:12
+msgid "page.resend_verification.email"
+msgstr "Email"
+
+#: fietsboek/templates/resend_verification.jinja2:17
+msgid "page.resend_verification.request"
+msgstr "Send request"
+
 #: fietsboek/templates/upload.jinja2:9
 msgid "page.upload.form.gpx"
 msgstr "GPX file"
 
 #: fietsboek/templates/user_data.jinja2:7
 msgid "page.my_profile.title"
 msgstr "My Profile"
@@ -703,50 +746,47 @@
 msgid "page.my_profile.friend_request_email"
 msgstr "Email of the friend"
 
 #: fietsboek/templates/user_data.jinja2:77
 msgid "page.my_profile.send_friend_request"
 msgstr "Send friend request"
 
-#: fietsboek/transformers/__init__.py:140
-msgid "transformers.fix-null-elevation.title"
-msgstr "Fix null elevation"
-
-#: fietsboek/transformers/__init__.py:144
-msgid "transformers.fix-null-elevation.description"
-msgstr "This transformer fixes the elevation of points whose elevation is unset."
-
 #: fietsboek/transformers/breaks.py:31
 msgid "transformers.remove-breaks.title"
 msgstr "Remove breaks"
 
 #: fietsboek/transformers/breaks.py:35
 msgid "transformers.remove-breaks.description"
 msgstr "This transformer removes long breaks from the recording"
 
-#: fietsboek/views/account.py:54
+#: fietsboek/transformers/elevation.py:42
+msgid "transformers.fix-null-elevation.title"
+msgstr "Fix null elevation"
+
+#: fietsboek/transformers/elevation.py:46
+msgid "transformers.fix-null-elevation.description"
+msgstr "This transformer fixes the elevation of points whose elevation is unset."
+
+#: fietsboek/transformers/elevation.py:115
+msgid "transformers.fix-elevation-jumps"
+msgstr "Fix elevation jumps"
+
+#: fietsboek/transformers/elevation.py:119
+msgid "transformers.fix-elevation-jumps.description"
+msgstr "This transformer fixes abrupt jumps in the elevation value."
+
+#: fietsboek/views/account.py:53
 msgid "flash.invalid_name"
 msgstr "Invalid name"
 
-#: fietsboek/views/account.py:59
+#: fietsboek/views/account.py:58
 msgid "flash.invalid_email"
 msgstr "Invalid email"
 
-#: fietsboek/views/account.py:72
-msgid "email.verify_mail.subject"
-msgstr "Fietsboek Account Verification"
-
-#: fietsboek/views/account.py:75
-msgid "email.verify.text"
-msgstr ""
-"To verify your Fietsboek account, please use this link: {}\n"
-"\n"
-"If you did not create an account, ignore this email."
-
-#: fietsboek/views/account.py:86
+#: fietsboek/views/account.py:67
 msgid "flash.a_confirmation_link_has_been_sent"
 msgstr "A confirmation link has been sent"
 
 #: fietsboek/views/admin.py:48
 msgid "flash.badge_added"
 msgstr "Badge has been added"
 
@@ -754,58 +794,70 @@
 msgid "flash.badge_modified"
 msgstr "Badge has been modified"
 
 #: fietsboek/views/admin.py:92
 msgid "flash.badge_deleted"
 msgstr "Badge has been deleted"
 
-#: fietsboek/views/default.py:117
+#: fietsboek/views/default.py:115
 msgid "flash.invalid_credentials"
 msgstr "Invalid login credentials"
 
-#: fietsboek/views/default.py:121
+#: fietsboek/views/default.py:119
 msgid "flash.account_not_verified"
 msgstr "Your account is not verified yet"
 
-#: fietsboek/views/default.py:124
+#: fietsboek/views/default.py:122
 msgid "flash.logged_in"
 msgstr "You are now logged in"
 
-#: fietsboek/views/default.py:146
+#: fietsboek/views/default.py:142
 msgid "flash.logged_out"
 msgstr "You have been logged out"
 
-#: fietsboek/views/default.py:180
+#: fietsboek/views/default.py:172
 msgid "flash.reset_invalid_email"
 msgstr "Invalid email address provided"
 
-#: fietsboek/views/default.py:185
+#: fietsboek/views/default.py:177
 msgid "flash.password_token_generated"
 msgstr "A password reset email has been sent"
 
-#: fietsboek/views/default.py:190
+#: fietsboek/views/default.py:182
 msgid "page.password_reset.email.subject"
 msgstr "Fietsboek Password Reset"
 
-#: fietsboek/views/default.py:193
+#: fietsboek/views/default.py:185
 msgid "page.password_reset.email.body"
 msgstr ""
 "You can reset your Fietsboek password here: {}\n"
 "\n"
 "If you did not request a password reset, ignore this email."
 
-#: fietsboek/views/default.py:226
+#: fietsboek/views/default.py:224
+msgid "flash.resend_verification_email_fail"
+msgstr "Invalid email address provided"
+
+#: fietsboek/views/default.py:229
+msgid "flash.verification_token_generated"
+msgstr "A verification email has been sent"
+
+#: fietsboek/views/default.py:249
+msgid "flash.token_expired"
+msgstr "The link has expired"
+
+#: fietsboek/views/default.py:255
 msgid "flash.email_verified"
 msgstr "Your email address has been verified"
 
-#: fietsboek/views/default.py:240
+#: fietsboek/views/default.py:269
 msgid "flash.password_updated"
 msgstr "Password has been updated"
 
-#: fietsboek/views/detail.py:140
+#: fietsboek/views/detail.py:155
 msgid "flash.track_deleted"
 msgstr "Track has been deleted"
 
 #: fietsboek/views/upload.py:52
 msgid "flash.no_file_selected"
 msgstr "No file selected"
```

### Comparing `fietsboek-0.7.0/fietsboek/locale/fietslog.pot` & `fietsboek-0.8.0/fietsboek/locale/fietslog.pot`

 * *Files 2% similar despite different names*

```diff
@@ -4,28 +4,36 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-04-23 10:47+0200\n"
+"POT-Creation-Date: 2023-05-31 20:46+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
-#: fietsboek/util.py:280
+#: fietsboek/actions.py:250
+msgid "email.verify_mail.subject"
+msgstr ""
+
+#: fietsboek/actions.py:253
+msgid "email.verify.text"
+msgstr ""
+
+#: fietsboek/util.py:304
 msgid "password_constraint.mismatch"
 msgstr ""
 
-#: fietsboek/util.py:282
+#: fietsboek/util.py:306
 msgid "password_constraint.length"
 msgstr ""
 
 #: fietsboek/models/track.py:579
 msgid "tooltip.table.length"
 msgstr ""
 
@@ -141,81 +149,93 @@
 msgid "page.browse.filters.clear_all"
 msgstr ""
 
 #: fietsboek/templates/browse.jinja2:105
 msgid "page.browse.filters.expand_advanced"
 msgstr ""
 
-#: fietsboek/templates/browse.jinja2:122
+#: fietsboek/templates/browse.jinja2:110 fietsboek/templates/browse.jinja2:111
+msgid "page.browse.sort.date"
+msgstr ""
+
+#: fietsboek/templates/browse.jinja2:112 fietsboek/templates/browse.jinja2:113
+msgid "page.browse.sort.length"
+msgstr ""
+
+#: fietsboek/templates/browse.jinja2:114 fietsboek/templates/browse.jinja2:115
+msgid "page.browse.sort.duration"
+msgstr ""
+
+#: fietsboek/templates/browse.jinja2:132
 msgid "page.browse.organic_tooltip"
 msgstr ""
 
-#: fietsboek/templates/browse.jinja2:124
+#: fietsboek/templates/browse.jinja2:134
 msgid "page.browse.synthetic_tooltip"
 msgstr ""
 
-#: fietsboek/templates/browse.jinja2:132 fietsboek/templates/details.jinja2:90
+#: fietsboek/templates/browse.jinja2:142 fietsboek/templates/details.jinja2:90
 #: fietsboek/templates/profile.jinja2:15
 msgid "page.details.date"
 msgstr ""
 
-#: fietsboek/templates/browse.jinja2:134 fietsboek/templates/details.jinja2:104
+#: fietsboek/templates/browse.jinja2:144 fietsboek/templates/details.jinja2:104
 #: fietsboek/templates/profile.jinja2:17
 msgid "page.details.length"
 msgstr ""
 
-#: fietsboek/templates/browse.jinja2:139 fietsboek/templates/details.jinja2:95
+#: fietsboek/templates/browse.jinja2:149 fietsboek/templates/details.jinja2:95
 #: fietsboek/templates/profile.jinja2:21
 msgid "page.details.start_time"
 msgstr ""
 
-#: fietsboek/templates/browse.jinja2:141 fietsboek/templates/details.jinja2:99
+#: fietsboek/templates/browse.jinja2:151 fietsboek/templates/details.jinja2:99
 #: fietsboek/templates/profile.jinja2:23
 msgid "page.details.end_time"
 msgstr ""
 
-#: fietsboek/templates/browse.jinja2:146 fietsboek/templates/details.jinja2:108
+#: fietsboek/templates/browse.jinja2:156 fietsboek/templates/details.jinja2:108
 #: fietsboek/templates/profile.jinja2:27
 msgid "page.details.uphill"
 msgstr ""
 
-#: fietsboek/templates/browse.jinja2:148 fietsboek/templates/details.jinja2:112
+#: fietsboek/templates/browse.jinja2:158 fietsboek/templates/details.jinja2:112
 #: fietsboek/templates/profile.jinja2:29
 msgid "page.details.downhill"
 msgstr ""
 
-#: fietsboek/templates/browse.jinja2:153 fietsboek/templates/details.jinja2:117
+#: fietsboek/templates/browse.jinja2:163 fietsboek/templates/details.jinja2:117
 #: fietsboek/templates/profile.jinja2:33
 msgid "page.details.moving_time"
 msgstr ""
 
-#: fietsboek/templates/browse.jinja2:155 fietsboek/templates/details.jinja2:121
+#: fietsboek/templates/browse.jinja2:165 fietsboek/templates/details.jinja2:121
 #: fietsboek/templates/profile.jinja2:35
 msgid "page.details.stopped_time"
 msgstr ""
 
-#: fietsboek/templates/browse.jinja2:159 fietsboek/templates/details.jinja2:125
+#: fietsboek/templates/browse.jinja2:169 fietsboek/templates/details.jinja2:125
 #: fietsboek/templates/profile.jinja2:39
 msgid "page.details.max_speed"
 msgstr ""
 
-#: fietsboek/templates/browse.jinja2:161 fietsboek/templates/details.jinja2:129
+#: fietsboek/templates/browse.jinja2:171 fietsboek/templates/details.jinja2:129
 #: fietsboek/templates/profile.jinja2:41
 msgid "page.details.avg_speed"
 msgstr ""
 
-#: fietsboek/templates/browse.jinja2:179
+#: fietsboek/templates/browse.jinja2:189
 msgid "page.browse.download_multiple"
 msgstr ""
 
-#: fietsboek/templates/browse.jinja2:181
+#: fietsboek/templates/browse.jinja2:191
 msgid "page.browse.no_results"
 msgstr ""
 
-#: fietsboek/templates/browse.jinja2:183
+#: fietsboek/templates/browse.jinja2:193
 msgid "page.browse.no_tracks"
 msgstr ""
 
 #: fietsboek/templates/create_account.jinja2:5
 msgid "page.create_account.title"
 msgstr ""
 
@@ -455,78 +475,78 @@
 msgid "page.upload.form.submit"
 msgstr ""
 
 #: fietsboek/templates/finish_upload.jinja2:17
 msgid "page.upload.form.cancel"
 msgstr ""
 
-#: fietsboek/templates/home.jinja2:5
+#: fietsboek/templates/home.jinja2:6
 msgid "page.home.title"
 msgstr ""
 
-#: fietsboek/templates/home.jinja2:8
+#: fietsboek/templates/home.jinja2:17
 msgid "page.home.unfinished_uploads"
 msgstr ""
 
-#: fietsboek/templates/home.jinja2:22 fietsboek/templates/home.jinja2:29
-#: fietsboek/templates/home.jinja2:47
+#: fietsboek/templates/home.jinja2:31 fietsboek/templates/home.jinja2:38
+#: fietsboek/templates/home.jinja2:56
 msgid "page.home.summary.track"
 msgid_plural "page.home.summary.tracks"
 msgstr[0] ""
 msgstr[1] ""
 
-#: fietsboek/templates/home.jinja2:47
+#: fietsboek/templates/home.jinja2:56
 msgid "page.home.total"
 msgstr ""
 
-#: fietsboek/templates/layout.jinja2:41
+#: fietsboek/templates/layout.jinja2:43
 msgid "page.navbar.toggle"
 msgstr ""
 
-#: fietsboek/templates/layout.jinja2:52
+#: fietsboek/templates/layout.jinja2:54
 msgid "page.navbar.home"
 msgstr ""
 
-#: fietsboek/templates/layout.jinja2:55
+#: fietsboek/templates/layout.jinja2:57
 msgid "page.navbar.browse"
 msgstr ""
 
-#: fietsboek/templates/layout.jinja2:59
+#: fietsboek/templates/layout.jinja2:61
 msgid "page.navbar.upload"
 msgstr ""
 
-#: fietsboek/templates/layout.jinja2:68
+#: fietsboek/templates/layout.jinja2:70
 msgid "page.navbar.user"
 msgstr ""
 
-#: fietsboek/templates/layout.jinja2:72
+#: fietsboek/templates/layout.jinja2:74
 msgid "page.navbar.welcome_user"
 msgstr ""
 
-#: fietsboek/templates/layout.jinja2:75
+#: fietsboek/templates/layout.jinja2:77
 msgid "page.navbar.logout"
 msgstr ""
 
-#: fietsboek/templates/layout.jinja2:78
+#: fietsboek/templates/layout.jinja2:80
 msgid "page.navbar.profile"
 msgstr ""
 
-#: fietsboek/templates/layout.jinja2:81
+#: fietsboek/templates/layout.jinja2:83
 msgid "page.navbar.user_data"
 msgstr ""
 
-#: fietsboek/templates/layout.jinja2:85
+#: fietsboek/templates/layout.jinja2:87
 msgid "page.navbar.admin"
 msgstr ""
 
-#: fietsboek/templates/layout.jinja2:91
+#: fietsboek/templates/layout.jinja2:93
 msgid "page.navbar.login"
 msgstr ""
 
-#: fietsboek/templates/layout.jinja2:95
+#: fietsboek/templates/layout.jinja2:97
 msgid "page.navbar.create_account"
 msgstr ""
 
 #: fietsboek/templates/login.jinja2:7
 msgid "page.login.title"
 msgstr ""
 
@@ -546,14 +566,18 @@
 msgid "page.login.submit"
 msgstr ""
 
 #: fietsboek/templates/login.jinja2:43
 msgid "page.login.forgot_password"
 msgstr ""
 
+#: fietsboek/templates/login.jinja2:45
+msgid "page.login.resend_verification"
+msgstr ""
+
 #: fietsboek/templates/password_reset.jinja2:5
 msgid "page.password_reset.title"
 msgstr ""
 
 #: fietsboek/templates/password_reset.jinja2:11
 msgid "page.password_reset.password"
 msgstr ""
@@ -642,14 +666,30 @@
 msgid "page.request_password.email"
 msgstr ""
 
 #: fietsboek/templates/request_password.jinja2:17
 msgid "page.request_password.request"
 msgstr ""
 
+#: fietsboek/templates/resend_verification.jinja2:5
+msgid "page.resend_verification.title"
+msgstr ""
+
+#: fietsboek/templates/resend_verification.jinja2:6
+msgid "page.resend_verification.info"
+msgstr ""
+
+#: fietsboek/templates/resend_verification.jinja2:12
+msgid "page.resend_verification.email"
+msgstr ""
+
+#: fietsboek/templates/resend_verification.jinja2:17
+msgid "page.resend_verification.request"
+msgstr ""
+
 #: fietsboek/templates/upload.jinja2:9
 msgid "page.upload.form.gpx"
 msgstr ""
 
 #: fietsboek/templates/user_data.jinja2:7
 msgid "page.my_profile.title"
 msgstr ""
@@ -698,47 +738,47 @@
 msgid "page.my_profile.friend_request_email"
 msgstr ""
 
 #: fietsboek/templates/user_data.jinja2:77
 msgid "page.my_profile.send_friend_request"
 msgstr ""
 
-#: fietsboek/transformers/__init__.py:140
-msgid "transformers.fix-null-elevation.title"
-msgstr ""
-
-#: fietsboek/transformers/__init__.py:144
-msgid "transformers.fix-null-elevation.description"
-msgstr ""
-
 #: fietsboek/transformers/breaks.py:31
 msgid "transformers.remove-breaks.title"
 msgstr ""
 
 #: fietsboek/transformers/breaks.py:35
 msgid "transformers.remove-breaks.description"
 msgstr ""
 
-#: fietsboek/views/account.py:54
-msgid "flash.invalid_name"
+#: fietsboek/transformers/elevation.py:42
+msgid "transformers.fix-null-elevation.title"
 msgstr ""
 
-#: fietsboek/views/account.py:59
-msgid "flash.invalid_email"
+#: fietsboek/transformers/elevation.py:46
+msgid "transformers.fix-null-elevation.description"
 msgstr ""
 
-#: fietsboek/views/account.py:72
-msgid "email.verify_mail.subject"
+#: fietsboek/transformers/elevation.py:115
+msgid "transformers.fix-elevation-jumps"
 msgstr ""
 
-#: fietsboek/views/account.py:75
-msgid "email.verify.text"
+#: fietsboek/transformers/elevation.py:119
+msgid "transformers.fix-elevation-jumps.description"
+msgstr ""
+
+#: fietsboek/views/account.py:53
+msgid "flash.invalid_name"
+msgstr ""
+
+#: fietsboek/views/account.py:58
+msgid "flash.invalid_email"
 msgstr ""
 
-#: fietsboek/views/account.py:86
+#: fietsboek/views/account.py:67
 msgid "flash.a_confirmation_link_has_been_sent"
 msgstr ""
 
 #: fietsboek/views/admin.py:48
 msgid "flash.badge_added"
 msgstr ""
 
@@ -746,55 +786,67 @@
 msgid "flash.badge_modified"
 msgstr ""
 
 #: fietsboek/views/admin.py:92
 msgid "flash.badge_deleted"
 msgstr ""
 
-#: fietsboek/views/default.py:117
+#: fietsboek/views/default.py:115
 msgid "flash.invalid_credentials"
 msgstr ""
 
-#: fietsboek/views/default.py:121
+#: fietsboek/views/default.py:119
 msgid "flash.account_not_verified"
 msgstr ""
 
-#: fietsboek/views/default.py:124
+#: fietsboek/views/default.py:122
 msgid "flash.logged_in"
 msgstr ""
 
-#: fietsboek/views/default.py:146
+#: fietsboek/views/default.py:142
 msgid "flash.logged_out"
 msgstr ""
 
-#: fietsboek/views/default.py:180
+#: fietsboek/views/default.py:172
 msgid "flash.reset_invalid_email"
 msgstr ""
 
-#: fietsboek/views/default.py:185
+#: fietsboek/views/default.py:177
 msgid "flash.password_token_generated"
 msgstr ""
 
-#: fietsboek/views/default.py:190
+#: fietsboek/views/default.py:182
 msgid "page.password_reset.email.subject"
 msgstr ""
 
-#: fietsboek/views/default.py:193
+#: fietsboek/views/default.py:185
 msgid "page.password_reset.email.body"
 msgstr ""
 
-#: fietsboek/views/default.py:226
+#: fietsboek/views/default.py:224
+msgid "flash.resend_verification_email_fail"
+msgstr ""
+
+#: fietsboek/views/default.py:229
+msgid "flash.verification_token_generated"
+msgstr ""
+
+#: fietsboek/views/default.py:249
+msgid "flash.token_expired"
+msgstr ""
+
+#: fietsboek/views/default.py:255
 msgid "flash.email_verified"
 msgstr ""
 
-#: fietsboek/views/default.py:240
+#: fietsboek/views/default.py:269
 msgid "flash.password_updated"
 msgstr ""
 
-#: fietsboek/views/detail.py:140
+#: fietsboek/views/detail.py:155
 msgid "flash.track_deleted"
 msgstr ""
 
 #: fietsboek/views/upload.py:52
 msgid "flash.no_file_selected"
 msgstr ""
```

### Comparing `fietsboek-0.7.0/fietsboek/models/__init__.py` & `fietsboek-0.8.0/fietsboek/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/models/badge.py` & `fietsboek-0.8.0/fietsboek/models/badge.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 """The Badge model."""
+from typing import TYPE_CHECKING
+
 from pyramid.httpexceptions import HTTPNotFound
 from sqlalchemy import Column, Integer, LargeBinary, Text, select
-from sqlalchemy.orm import relationship
+from sqlalchemy.orm import Mapped, relationship
 
 from .meta import Base
 
+if TYPE_CHECKING:
+    from .track import Track
+
 
 class Badge(Base):
     """Represents a badge.
 
     Badges have a title and an image and can be defined by the admin.
 
     :ivar id: Database ID.
@@ -23,15 +28,17 @@
 
     # pylint: disable=too-few-public-methods
     __tablename__ = "badges"
     id = Column(Integer, primary_key=True)
     title = Column(Text)
     image = Column(LargeBinary)
 
-    tracks = relationship("Track", secondary="track_badge_assoc", back_populates="badges")
+    tracks: Mapped[list["Track"]] = relationship(
+        "Track", secondary="track_badge_assoc", back_populates="badges"
+    )
 
     @classmethod
     def factory(cls, request):
         """Factory method to pass to a route definition.
 
         This factory retrieves the badge based on the ``badge_id`` matched
         route parameter, and returns the badge. If the badge is not found,
```

### Comparing `fietsboek-0.7.0/fietsboek/models/comment.py` & `fietsboek-0.8.0/fietsboek/models/comment.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 """Comment model."""
+from typing import TYPE_CHECKING
+
 from sqlalchemy import Column, DateTime, ForeignKey, Integer, Text
-from sqlalchemy.orm import relationship
+from sqlalchemy.orm import Mapped, relationship
 
 from .meta import Base
 
+if TYPE_CHECKING:
+    from .track import Track
+    from .user import User
+
 
 class Comment(Base):
     """Represents a comment on a track.
 
     :ivar id: Database ID.
     :vartype id: int
     :ivar author_id: ID of the comment's author.
@@ -31,9 +37,9 @@
     id = Column(Integer, primary_key=True)
     author_id = Column(Integer, ForeignKey("users.id"))
     track_id = Column(Integer, ForeignKey("tracks.id"))
     date = Column(DateTime)
     title = Column(Text)
     text = Column(Text)
 
-    author = relationship("User", back_populates="comments")
-    track = relationship("Track", back_populates="comments")
+    author: Mapped["User"] = relationship("User", back_populates="comments")
+    track: Mapped["Track"] = relationship("Track", back_populates="comments")
```

### Comparing `fietsboek-0.7.0/fietsboek/models/image.py` & `fietsboek-0.8.0/fietsboek/models/image.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 """Image metadata.
 
 The actual image data is saved on disk, we only store the metadata such as an
 image description here.
 """
+from typing import TYPE_CHECKING
+
 from sqlalchemy import Column, ForeignKey, Integer, Text, UniqueConstraint, select
-from sqlalchemy.orm import relationship
+from sqlalchemy.orm import Mapped, relationship
 
 from .meta import Base
 
+if TYPE_CHECKING:
+    from .track import Track
+
 
 class ImageMetadata(Base):
     """Represents metadata for an uploaded image.
 
     :ivar id: Database ID.
     :vartype id: int
     :ivar track_id: ID of the track that this image belongs to.
@@ -27,15 +32,15 @@
     # pylint: disable=too-few-public-methods
     __tablename__ = "image_metadata"
     id = Column(Integer, primary_key=True)
     track_id = Column(Integer, ForeignKey("tracks.id"), nullable=False)
     image_name = Column(Text, nullable=False)
     description = Column(Text)
 
-    track = relationship("Track", back_populates="images")
+    track: Mapped["Track"] = relationship("Track", back_populates="images")
 
     __table_args__ = (UniqueConstraint("track_id", "image_name"),)
 
     @classmethod
     def get_or_create(cls, dbsession, track, image_name):
         """Retrieves the image metadata for the given image, or creates a new
         one if it doesn't exist.
```

### Comparing `fietsboek-0.7.0/fietsboek/models/meta.py` & `fietsboek-0.8.0/fietsboek/models/meta.py`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/models/track.py` & `fietsboek-0.8.0/fietsboek/models/track.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     ForeignKey,
     Integer,
     LargeBinary,
     Table,
     Text,
     select,
 )
-from sqlalchemy.orm import relationship
+from sqlalchemy.orm import Mapped, relationship
 
 from .. import util
 from .meta import Base
 
 if TYPE_CHECKING:
     from .. import models
 
@@ -69,15 +69,15 @@
     """
 
     # pylint: disable=too-few-public-methods
     __tablename__ = "tags"
     track_id = Column(Integer, ForeignKey("tracks.id"), primary_key=True)
     tag = Column(Text, primary_key=True)
 
-    track = relationship("Track", back_populates="tags")
+    track: Mapped["Track"] = relationship("Track", back_populates="tags")
 
 
 class Visibility(enum.Enum):
     """An enum that represents the visibility of tracks.
 
     Note that the track is always visible to tagged people and via the sharing
     link.
@@ -200,25 +200,33 @@
     date_raw = Column(DateTime)
     date_tz = Column(Integer)
     visibility = Column(Enum(Visibility))
     link_secret = Column(Text)
     type = Column(Enum(TrackType))
     transformers = Column(JSON)
 
-    owner = relationship("User", back_populates="tracks")
-    cache = relationship(
+    owner: Mapped["models.User"] = relationship("User", back_populates="tracks")
+    cache: Mapped[Optional["TrackCache"]] = relationship(
         "TrackCache", back_populates="track", uselist=False, cascade="all, delete-orphan"
     )
-    tagged_people = relationship(
+    tagged_people: Mapped[list["models.User"]] = relationship(
         "User", secondary=track_people_assoc, back_populates="tagged_tracks"
     )
-    badges = relationship("Badge", secondary=track_badge_assoc, back_populates="tracks")
-    tags = relationship("Tag", back_populates="track", cascade="all, delete-orphan")
-    comments = relationship("Comment", back_populates="track", cascade="all, delete-orphan")
-    images = relationship("ImageMetadata", back_populates="track", cascade="all, delete-orphan")
+    badges: Mapped[list["models.Badge"]] = relationship(
+        "Badge", secondary=track_badge_assoc, back_populates="tracks"
+    )
+    tags: Mapped[list["Tag"]] = relationship(
+        "Tag", back_populates="track", cascade="all, delete-orphan"
+    )
+    comments: Mapped[list["models.Comment"]] = relationship(
+        "Comment", back_populates="track", cascade="all, delete-orphan"
+    )
+    images: Mapped[list["models.ImageMetadata"]] = relationship(
+        "ImageMetadata", back_populates="track", cascade="all, delete-orphan"
+    )
 
     @classmethod
     def factory(cls, request):
         """Factory method to pass to a route definition.
 
         This factory retrieves the track based on the ``track_id`` matched
         route parameter, and returns the track. If the track is not found,
@@ -281,14 +289,16 @@
 
         This combines the :attr:`date_raw` and :attr:`date_tz` values to
         provide a timezone aware :class:`~datetime.datetime`.
 
         :return: The aware datetime.
         :rtype: datetime.datetime
         """
+        if self.date_raw is None:
+            return datetime.datetime.utcfromtimestamp(0).replace(tzinfo=datetime.timezone.utc)
         if self.date_tz is None:
             timezone = datetime.timezone.utc
         else:
             timezone = datetime.timezone(datetime.timedelta(minutes=self.date_tz))
         return self.date_raw.replace(tzinfo=timezone)
 
     @date.setter
@@ -363,51 +373,51 @@
 
         If a tag with the text already exists, does nothing.
 
         :param text: The text of the tag.
         :type text: str
         """
         for tag in self.tags:
-            if tag.tag.lower() == text.lower():
+            if tag.tag and tag.tag.lower() == text.lower():
                 return
         self.tags.append(Tag(tag=text))
 
     def remove_tag(self, text):
         """Remove the tag with the given text.
 
         :param text: The text of the tag to remove.
         :type text: str
         """
         for i, tag in enumerate(self.tags):
-            if tag.tag.lower() == text.lower():
+            if tag.tag and tag.tag.lower() == text.lower():
                 break
         else:
             return
         del self.tags[i]
 
     def sync_tags(self, tags):
         """Syncs the track's tags with a given set of wanted tags.
 
         This adds and removes tags from the track as needed.
 
         :param tags: The wanted tags.
         :type tags: set[str]
         """
-        my_tags = {tag.tag.lower() for tag in self.tags}
+        my_tags = {tag.tag.lower() for tag in self.tags if tag.tag}
         lower_tags = {tag.lower() for tag in tags}
         # We cannot use the set difference methods because we want to keep the
         # capitalization of the original tags when adding them, but use the
         # lower-case version when comparing them.
         for to_add in tags:
             if to_add.lower() not in my_tags:
                 self.tags.append(Tag(tag=to_add))
 
         to_delete = []
         for i, tag in enumerate(self.tags):
-            if tag.tag.lower() not in lower_tags:
+            if tag.tag and tag.tag.lower() not in lower_tags:
                 to_delete.append(i)
         for i in to_delete[::-1]:
             del self.tags[i]
 
     def transformer_params_for(self, transformer_id: str) -> Optional[dict]:
         """Returns the transformer parameters for the given transformer.
 
@@ -454,103 +464,103 @@
 
     @property
     def length(self) -> float:
         """Returns the length of the track..
 
         :return: Length of the track in meters.
         """
-        if self.cache is None:
+        if self.cache is None or self.cache.length is None:
             return self._meta()["length"]
-        return self.cache.length
+        return float(self.cache.length)
 
     @property
     def downhill(self) -> float:
         """Returns the downhill of the track.
 
         :return: Downhill in meters.
         """
-        if self.cache is None:
+        if self.cache is None or self.cache.downhill is None:
             return self._meta()["downhill"]
-        return self.cache.downhill
+        return float(self.cache.downhill)
 
     @property
     def uphill(self) -> float:
         """Returns the uphill of the track.
 
         :return: Uphill in meters.
         """
-        if self.cache is None:
+        if self.cache is None or self.cache.uphill is None:
             return self._meta()["uphill"]
-        return self.cache.uphill
+        return float(self.cache.uphill)
 
     @property
     def moving_time(self) -> datetime.timedelta:
         """Returns the moving time.
 
         :return: Moving time in seconds.
         """
-        if self.cache is None:
+        if self.cache is None or self.cache.moving_time is None:
             value = self._meta()["moving_time"]
         else:
             value = self.cache.moving_time
         return datetime.timedelta(seconds=value)
 
     @property
     def stopped_time(self) -> datetime.timedelta:
         """Returns the stopped time.
 
         :return: Stopped time in seconds.
         """
-        if self.cache is None:
+        if self.cache is None or self.cache.stopped_time is None:
             value = self._meta()["stopped_time"]
         else:
             value = self.cache.stopped_time
         return datetime.timedelta(seconds=value)
 
     @property
     def max_speed(self) -> float:
         """Returns the maximum speed.
 
         :return: Maximum speed in meters/second.
         """
-        if self.cache is None:
+        if self.cache is None or self.cache.max_speed is None:
             return self._meta()["max_speed"]
-        return self.cache.max_speed
+        return float(self.cache.max_speed)
 
     @property
     def avg_speed(self) -> float:
         """Returns the average speed.
 
         :return: Average speed in meters/second.
         """
-        if self.cache is None:
+        if self.cache is None or self.cache.avg_speed is None:
             return self._meta()["avg_speed"]
-        return self.cache.avg_speed
+        return float(self.cache.avg_speed)
 
     @property
     def start_time(self) -> datetime.datetime:
         """Returns the start time.
 
         This is the time embedded in the GPX file, not the time in the ``date`` column.
 
         :return: Start time.
         """
-        if self.cache is None:
+        if self.cache is None or self.cache.start_time is None:
             return self._meta()["start_time"]
         return self.cache.start_time
 
     @property
     def end_time(self) -> datetime.datetime:
         """Returns the end time.
 
         This is the time embedded in the GPX file, not the time in the ``date`` column.
 
         :return: End time.
         """
-        if self.cache is None:
+        if self.cache is None or self.cache.end_time is None:
             return self._meta()["end_time"]
         return self.cache.end_time
 
     @property
     def duration(self) -> datetime.timedelta:
         """Returns the duration of this track.
 
@@ -594,45 +604,45 @@
             f"<tr><td>{localizer.translate(name)}</td><td>{value}</td></tr>"
             for (name, value) in rows
         ]
         return Markup(f'<table>{"".join(rows)}</table>')
 
     # Proxied properties
     @property
-    def id(self) -> int:
+    def id(self) -> Optional[int]:
         """ID of the underlying track."""
         return self.track.id
 
     @property
-    def title(self) -> str:
+    def title(self) -> Optional[str]:
         """Title of the underlying track."""
         return self.track.title
 
     @property
-    def description(self) -> str:
+    def description(self) -> Optional[str]:
         """Description of the underlying track."""
         return self.track.description
 
     @property
-    def date(self) -> datetime.datetime:
+    def date(self) -> Optional[datetime.datetime]:
         """Date of the underlying track."""
         return self.track.date
 
     @property
-    def visibility(self) -> Visibility:
+    def visibility(self) -> Optional[Visibility]:
         """Visibility of the underlying track."""
         return self.track.visibility
 
     @property
-    def link_secret(self) -> str:
+    def link_secret(self) -> Optional[str]:
         """Link secret of the underlying track."""
         return self.track.link_secret
 
     @property
-    def type(self) -> TrackType:
+    def type(self) -> Optional[TrackType]:
         """Type of the underlying track."""
         return self.track.type
 
     @property
     def owner(self) -> "models.User":
         """Owner of the undlerying track."""
         return self.track.owner
@@ -723,66 +733,70 @@
     max_speed = Column(Float)
     avg_speed = Column(Float)
     start_time_raw = Column(DateTime)
     start_time_tz = Column(Integer)
     end_time_raw = Column(DateTime)
     end_time_tz = Column(Integer)
 
-    track = relationship("Track", back_populates="cache")
+    track: Mapped["Track"] = relationship("Track", back_populates="cache")
 
     @property
-    def start_time(self):
+    def start_time(self) -> Optional[datetime.datetime]:
         """The time-zone-aware start time of this track.
 
         :return: The aware datetime.
-        :rtype: datetime.datetime
         """
+        if self.start_time_raw is None:
+            return None
         if self.start_time_tz is None:
             timezone = datetime.timezone.utc
         else:
             timezone = datetime.timezone(datetime.timedelta(minutes=self.start_time_tz))
         return self.start_time_raw.replace(tzinfo=timezone)
 
     @start_time.setter
-    def start_time(self, value):
+    def start_time(self, value: datetime.datetime):
         if value.tzinfo is None:
             LOGGER.debug(
                 "Non-aware datetime passed (cache_id=%d, value=%s), assuming offset=0",
-                self.id or -1,
+                self.track_id or -1,
                 value,
             )
             self.start_time_tz = 0
         else:
-            self.start_time_tz = value.tzinfo.utcoffset(value).total_seconds() // 60
+            utcoffset = value.tzinfo.utcoffset(value) or datetime.timedelta()
+            self.start_time_tz = int(utcoffset.total_seconds() // 60)
         self.start_time_raw = value.replace(tzinfo=None)
 
     @property
-    def end_time(self):
+    def end_time(self) -> Optional[datetime.datetime]:
         """The time-zone-aware end time of this track.
 
         :return: The aware datetime.
-        :rtype: datetime.datetime
         """
+        if self.end_time_raw is None:
+            return None
         if self.end_time_tz is None:
             timezone = datetime.timezone.utc
         else:
             timezone = datetime.timezone(datetime.timedelta(minutes=self.end_time_tz))
         return self.end_time_raw.replace(tzinfo=timezone)
 
     @end_time.setter
-    def end_time(self, value):
+    def end_time(self, value: datetime.datetime):
         if value.tzinfo is None:
             LOGGER.debug(
                 "Non-aware datetime passed (cache_id=%d, value=%s), assuming offset=0",
-                self.id or -1,
+                self.track_id or -1,
                 value,
             )
             self.end_time_tz = 0
         else:
-            self.end_time_tz = value.tzinfo.utcoffset(value).total_seconds() // 60
+            utcoffset = value.tzinfo.utcoffset(value) or datetime.timedelta()
+            self.end_time_tz = int(utcoffset.total_seconds() // 60)
         self.end_time_raw = value.replace(tzinfo=None)
 
 
 class Upload(Base):
     """A track that is currently being uploaded.
 
     Once a upload is done, the :class:`Upload` item is removed and a proper
@@ -803,15 +817,15 @@
     # pylint: disable=too-many-instance-attributes,too-few-public-methods
     __tablename__ = "uploads"
     id = Column(Integer, primary_key=True)
     uploaded_at = Column(DateTime)
     owner_id = Column(Integer, ForeignKey("users.id"))
     gpx = Column(LargeBinary)
 
-    owner = relationship("User", back_populates="uploads")
+    owner: Mapped["models.User"] = relationship("User", back_populates="uploads")
 
     @classmethod
     def factory(cls, request):
         """Factory method to pass to a route definition.
 
         This factory retrieves the upload based on the ``upload_id`` matched
         route parameter, and returns the upload. If the upload is not found,
@@ -834,12 +848,12 @@
             (Allow, "group:admins", ALL_PERMISSIONS),
             (Allow, f"user:{self.owner_id}", "upload.finish"),
         ]
 
     @property
     def gpx_data(self):
         """Access the decompressed gpx data."""
-        return gzip.decompress(self.gpx)
+        return gzip.decompress(self.gpx or b"")
 
     @gpx_data.setter
     def gpx_data(self, value):
         self.gpx = gzip.compress(value)
```

### Comparing `fietsboek-0.7.0/fietsboek/models/user.py` & `fietsboek-0.8.0/fietsboek/models/user.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """User models for fietsboek."""
 import datetime
 import enum
 import secrets
 import uuid
 from functools import reduce
+from typing import TYPE_CHECKING
 
 from cryptography.exceptions import InvalidKey
 from cryptography.hazmat.primitives.kdf.scrypt import Scrypt
 from pyramid.authorization import ALL_PERMISSIONS, Allow
 from pyramid.httpexceptions import HTTPNotFound
 from pyramid.request import Request
 from sqlalchemy import (
@@ -23,20 +24,24 @@
     Text,
     UniqueConstraint,
     delete,
     func,
     select,
     union,
 )
-from sqlalchemy.orm import relationship, with_parent
+from sqlalchemy.orm import Mapped, relationship, with_parent
 from sqlalchemy.orm.attributes import flag_dirty
 from sqlalchemy.orm.session import object_session
 
 from .meta import Base
 
+if TYPE_CHECKING:
+    from .comment import Comment
+    from .track import Track, Upload
+
 
 class PasswordMismatch(Exception):
     """Exception that is raised if the passwords mismatch.
 
     Using an exception forces the handling of the password mismatch and makes
     it impossible to accidentally ignore the return value of the password
     verification.
@@ -49,14 +54,17 @@
     "length": 32,
     "n": 2**14,
     "r": 8,
     "p": 1,
 }
 SALT_LENGTH = 32
 
+TOKEN_LIFETIME = datetime.timedelta(hours=24)
+"""Maximum validity time of a token."""
+
 
 friends_assoc = Table(
     "friends_assoc",
     Base.metadata,
     Column("user_1_id", ForeignKey("users.id"), primary_key=True),
     Column("user_2_id", ForeignKey("users.id"), primary_key=True),
 )
@@ -98,30 +106,38 @@
     name = Column(Text)
     password = Column(LargeBinary)
     salt = Column(LargeBinary)
     email = Column(Text)
     is_admin = Column(Boolean, default=False)
     is_verified = Column(Boolean, default=False)
 
-    tracks = relationship("Track", back_populates="owner", cascade="all, delete-orphan")
-    tagged_tracks = relationship(
+    tracks: Mapped[list["Track"]] = relationship(
+        "Track", back_populates="owner", cascade="all, delete-orphan"
+    )
+    tagged_tracks: Mapped[list["Track"]] = relationship(
         "Track", secondary="track_people_assoc", back_populates="tagged_people"
     )
-    uploads = relationship("Upload", back_populates="owner", cascade="all, delete-orphan")
-    tokens = relationship("Token", back_populates="user", cascade="all, delete-orphan")
-    comments = relationship("Comment", back_populates="author", cascade="all, delete-orphan")
+    uploads: Mapped[list["Upload"]] = relationship(
+        "Upload", back_populates="owner", cascade="all, delete-orphan"
+    )
+    tokens: Mapped[list["Token"]] = relationship(
+        "Token", back_populates="user", cascade="all, delete-orphan"
+    )
+    comments: Mapped[list["Comment"]] = relationship(
+        "Comment", back_populates="author", cascade="all, delete-orphan"
+    )
 
     # We don't use them, but include them to ensure our cascading works
-    friends_1 = relationship(
+    friends_1: Mapped[list["User"]] = relationship(
         "User",
         secondary="friends_assoc",
         back_populates="friends_2",
         foreign_keys=[friends_assoc.c.user_1_id],
     )
-    friends_2 = relationship(
+    friends_2: Mapped[list["User"]] = relationship(
         "User",
         secondary="friends_assoc",
         back_populates="friends_1",
         foreign_keys=[friends_assoc.c.user_2_id],
     )
 
     @classmethod
@@ -186,17 +202,17 @@
 
         :raises PasswordMismatch: When the password does not match the stored
             one.
         :param password: The password to check.
         :type password: str
         """
         password = password.encode("utf-8")
-        scrypt = Scrypt(salt=self.salt, **SCRYPT_PARAMETERS)
+        scrypt = Scrypt(salt=self.salt or b"", **SCRYPT_PARAMETERS)
         try:
-            scrypt.verify(password, self.password)
+            scrypt.verify(password, self.password or b"")
         except InvalidKey:
             raise PasswordMismatch from None
 
     def principals(self):
         """Returns all principals that this user fulfills.
 
         This does not include the ``Everyone`` and ``Authenticated``
@@ -318,39 +334,44 @@
 
         This is not a simple SQLAlchemy property because the friendship
         relation  is complex.
 
         :return: All friends of this user.
         :rtype: list[User]
         """
+        session = object_session(self)
+        assert session
         query = select(User).from_statement(self._friend_query())
-        yield from object_session(self).execute(query).scalars()
+        yield from session.execute(query).scalars()
 
     def remove_friend(self, friend):
         """Remove the friend relationship between two users.
 
         :param friend: The befriended user.
         :type friend: User
         """
         session = object_session(self)
+        assert session
         session.execute(delete(friends_assoc).filter_by(user_1_id=self.id, user_2_id=friend.id))
         session.execute(delete(friends_assoc).filter_by(user_1_id=friend.id, user_2_id=self.id))
         flag_dirty(self)
 
     def add_friend(self, friend):
         """Add the given user as a new friend.
 
         :param friend: The user to befriend.
         :type friend: User
         """
+        session = object_session(self)
+        assert session
         if self.id > friend.id:
             friend.add_friend(self)
             return
         stmt = friends_assoc.insert().values(user_1_id=self.id, user_2_id=friend.id)
-        object_session(self).execute(stmt)
+        session.execute(stmt)
 
     def autocomplete_tags(self):
         """Returns all tags the user has ever used, suitable for autocompletion
         lists.
 
         :return: All tags of the user.
         :rtype: ~collections.abc.Iterator[str]
@@ -381,18 +402,18 @@
     # pylint: disable=too-few-public-methods
     __tablename__ = "friend_requests"
     id = Column(Integer, primary_key=True)
     sender_id = Column(Integer, ForeignKey("users.id"))
     recipient_id = Column(Integer, ForeignKey("users.id"))
     date = Column(DateTime)
 
-    sender = relationship(
+    sender: Mapped["User"] = relationship(
         "User", primaryjoin="User.id == FriendRequest.sender_id", backref="outgoing_requests"
     )
-    recipient = relationship(
+    recipient: Mapped["User"] = relationship(
         "User", primaryjoin="User.id == FriendRequest.recipient_id", backref="incoming_requests"
     )
 
     __table_args__ = (UniqueConstraint("sender_id", "recipient_id"),)
 
 
 class TokenType(enum.Enum):
@@ -436,15 +457,15 @@
     __tablename__ = "tokens"
     id = Column(Integer, primary_key=True)
     user_id = Column(Integer, ForeignKey("users.id"))
     uuid = Column(Text)
     token_type = Column(Enum(TokenType))
     date = Column(DateTime)
 
-    user = relationship("User", back_populates="tokens")
+    user: Mapped["User"] = relationship("User", back_populates="tokens")
 
     @classmethod
     def generate(cls, user, token_type):
         """Generate a new token for the given user.
 
         :param user: The user which to generate the token for.
         :type user: User
@@ -453,9 +474,15 @@
         :return: The generated token.
         :rtype: Token
         """
         token_uuid = str(uuid.uuid4())
         now = datetime.datetime.utcnow()
         return cls(user=user, uuid=token_uuid, date=now, token_type=token_type)
 
+    def age(self) -> datetime.timedelta:
+        """Returns the age of the token."""
+        if self.date is None:
+            return datetime.timedelta()
+        return abs(datetime.datetime.utcnow() - self.date)
+
 
 Index("idx_token_uuid", Token.uuid, unique=True)
```

### Comparing `fietsboek-0.7.0/fietsboek/pages.py` & `fietsboek-0.8.0/fietsboek/pages.py`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/routes.py` & `fietsboek-0.8.0/fietsboek/routes.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     config.add_route("browse", "/track/")
 
     config.add_route("static-page", "/page/{slug}")
 
     config.add_route("track-archive", "/track/archive")
 
     config.add_route("password-reset", "/password-reset")
+    config.add_route("resend-verification", "/resend-verification")
     config.add_route("use-token", "/token/{uuid}")
     config.add_route("create-account", "/create-account")
 
     config.add_route("upload", "/upload")
     config.add_route(
         "preview", "/preview/{upload_id}.gpx", factory="fietsboek.models.Upload.factory"
     )
```

### Comparing `fietsboek-0.7.0/fietsboek/scripts/__init__.py` & `fietsboek-0.8.0/fietsboek/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/scripts/fietscron.py` & `fietsboek-0.8.0/fietsboek/scripts/fietscron.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from sqlalchemy.engine import Engine
 from sqlalchemy.orm import Session
 
 from .. import config as mod_config
 from .. import hittekaart, models
 from ..config import Config
 from ..data import DataManager
+from ..models.user import TOKEN_LIFETIME
 from . import config_option
 
 LOGGER = logging.getLogger(__name__)
 
 
 @click.command()
 @config_option
@@ -44,14 +45,15 @@
         LOGGER.info("Skipping cronjob tasks due to maintenance mode")
         return
 
     engine = create_engine(config.sqlalchemy_url)
 
     LOGGER.debug("Starting maintenance tasks")
     remove_old_uploads(engine)
+    remove_old_tokens(engine)
     rebuild_cache(engine, data_manager)
 
     if config.hittekaart_autogenerate:
         redis = mod_redis.from_url(config.redis_url)
         run_hittekaart(engine, data_manager, redis, config)
 
 
@@ -61,23 +63,34 @@
     limit = datetime.datetime.now() - datetime.timedelta(hours=24)
     session = Session(engine)
     stmt = delete(models.Upload).where(models.Upload.uploaded_at < limit)
     session.execute(stmt)
     session.commit()
 
 
+def remove_old_tokens(engine: Engine):
+    """Removes old tokens from the database."""
+    LOGGER.info("Deleting old tokens")
+    limit = datetime.datetime.utcnow() - TOKEN_LIFETIME
+    session = Session(engine)
+    stmt = delete(models.Token).where(models.Token.date < limit)
+    session.execute(stmt)
+    session.commit()
+
+
 def rebuild_cache(engine: Engine, data_manager: DataManager):
     """Rebuilds the cache entries that are currently missing."""
     LOGGER.debug("Rebuilding caches")
     session = Session(engine)
     needed_rebuilds = select(models.Track).where(
         not_(exists(select(models.TrackCache).where(models.TrackCache.track_id == models.Track.id)))
     )
     with session:
         for track in session.execute(needed_rebuilds).scalars():
+            assert track.id is not None
             LOGGER.info("Rebuilding cache for track %d", track.id)
             gpx_data = data_manager.open(track.id).decompress_gpx()
             track.ensure_cache(gpx_data)
             session.add(track)
         session.commit()
 
 
@@ -106,15 +119,22 @@
         user = session.execute(select(models.User).filter_by(id=int(item))).scalar()
         if user is None:
             LOGGER.debug("User %d had a high-priority queue entry but was not found", item)
             continue
 
         for mode in modes:
             LOGGER.info("Generating %s for user %d (high-priority)", mode.value, user.id)
-            hittekaart.generate_for(user, session, data_manager, mode, exe_path=exe_path)
+            hittekaart.generate_for(
+                user,
+                session,
+                data_manager,
+                mode,
+                exe_path=exe_path,
+                threads=config.hittekaart_threads,
+            )
 
     if had_hq_item:
         return
 
     # Low-priority queue
     item = redis.spop("hittekaart:queue:low")
     if item is None:
@@ -127,18 +147,21 @@
     user = session.execute(select(models.User).filter_by(id=int(item))).scalar()
     if user is None:
         LOGGER.debug("User %d had a low-priority queue entry but was not found", item)
         return
 
     for mode in modes:
         LOGGER.info("Generating %s for user %d (low-priority)", mode.value, user.id)
-        hittekaart.generate_for(user, session, data_manager, mode, exe_path=exe_path)
+        hittekaart.generate_for(
+            user, session, data_manager, mode, exe_path=exe_path, threads=config.hittekaart_threads
+        )
 
 
 def refill_queue(session: Session, redis: Redis):
     """Refills the low-priority hittekaart queue by adding all users to it."""
     LOGGER.debug("Refilling low-priority queue")
     for user in session.execute(select(models.User)).scalars():
+        assert user.id is not None
         redis.sadd("hittekaart:queue:low", user.id)
 
 
 __all__ = ["cli"]
```

### Comparing `fietsboek-0.7.0/fietsboek/security.py` & `fietsboek-0.8.0/fietsboek/security.py`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/GPX2GM.css` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/GPX2GM.css`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/GPX2GM.js` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/GPX2GM.js`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/GPX2GM_Defs.js` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/GPX2GM_Defs.js`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/Loading_icon.gif` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/Loading_icon.gif`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/Loading_icon_V1.gif` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/Loading_icon_V1.gif`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/Loading_icon_V2.gif` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/Loading_icon_V2.gif`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/airport.png` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/airport.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/bar.png` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/bar.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/boat.png` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/boat.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/bridge.png` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/bridge.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/castle.png` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/castle.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/church2.png` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/church2.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/cluster.png` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/cluster.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/cluster.svg` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/cluster.svg`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/current_location - Kopie.svg` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/current_location - Kopie.svg`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/current_location.svg` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/current_location.svg`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/cycling.png` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/cycling.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/finish.png` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/finish.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/harbor.png` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/harbor.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/hiking.png` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/hiking.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/hotel2.png` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/hotel2.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/kreis.png` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/kreis.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/library.png` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/library.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/marker-icon_bw.png` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/marker-icon_bw.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/marker.svg` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/marker.svg`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/museum.png` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/museum.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/panorama.png` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/panorama.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/park.png` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/park.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/peak.png` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/peak.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/photo.png` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/photo.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/pin_red.png` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/pin_red.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/pin_red_shadow.png` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/pin_red_shadow.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/restaurant.png` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/restaurant.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/shadow.png` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/shadow.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/shadow50.png` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/shadow50.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/shoppingmall.png` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/shoppingmall.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/streckenmarker - Kopie.svg` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/streckenmarker - Kopie.svg`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/streckenmarker.svg` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/streckenmarker.svg`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/subway.png` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/subway.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/tent.png` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/tent.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/train.png` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/train.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/video.png` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/video.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/villa.png` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/villa.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/whereami.svg` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/whereami.svg`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/Icons/whereami_V1.svg` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/Icons/whereami_V1.svg`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/gmutils.js` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/gmutils.js`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/gra_canvas.js` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/gra_canvas.js`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/gra_svg.js` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/gra_svg.js`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/leaflet/images/layers-2x.png` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/leaflet/images/layers-2x.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/leaflet/images/layers.png` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/leaflet/images/layers.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/leaflet/images/marker-icon-2x.png` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/leaflet/images/marker-icon-2x.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/leaflet/images/marker-icon.png` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/leaflet/images/marker-icon.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/leaflet/images/marker-shadow.png` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/leaflet/images/marker-shadow.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/leaflet/leaflet.css` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/leaflet/leaflet.css`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/leaflet/leaflet.js` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/leaflet/leaflet.js`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/leaflet/leaflet.js.map` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/leaflet/leaflet.js.map`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/osmutils.js` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/osmutils.js`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/plot.js` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/plot.js`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/GM_Utils/shimg.js` & `fietsboek-0.8.0/fietsboek/static/GM_Utils/shimg.js`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/bootstrap-icons.css` & `fietsboek-0.8.0/fietsboek/static/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/bootstrap.bundle.min.js` & `fietsboek-0.8.0/fietsboek/static/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/bootstrap.css` & `fietsboek-0.8.0/fietsboek/static/bootstrap.css`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/favicon.png` & `fietsboek-0.8.0/fietsboek/static/favicon.png`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/fietsboek.js` & `fietsboek-0.8.0/fietsboek/static/fietsboek.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -295,14 +295,31 @@
  */
 function clearInputButtonClicked(event) {
     const target = event.target;
     target.closest(".input-group").querySelectorAll("input").forEach((i) => i.value = "");
     target.closest(".input-group").querySelectorAll("select").forEach((i) => i.value = "");
 }
 addHandler(".button-clear-input", "click", clearInputButtonClicked);
+/**
+ * Handler to change the sorting of the home page.
+ *
+ * This basically sets the cookie to signal that the home page should be
+ * returned reversed, and then reloads the page.
+ *
+ * @param event - The triggering event.
+ */
+function changeHomeSorting(event) {
+    var _a, _b;
+    const currentSorting = (_b = (_a = document.cookie.split("; ")
+        .find((row) => row.startsWith("home_sorting="))) === null || _a === void 0 ? void 0 : _a.split("=")[1]) !== null && _b !== void 0 ? _b : "asc";
+    const newSorting = currentSorting == "asc" ? "desc" : "asc";
+    document.cookie = `home_sorting=${newSorting}; SameSite=Lax`;
+    window.location.reload();
+}
+addHandler("#changeHomeSorting", "click", changeHomeSorting);
 document.addEventListener('DOMContentLoaded', function() {
     window.fietsboekImageIndex = 0;
     /* Enable tooltips */
     const tooltipTriggerList = [].slice.call(document.querySelectorAll('[data-bs-toggle="tooltip"]'));
     tooltipTriggerList.map((tooltipTriggerEl) => {
         return new bootstrap.Tooltip(tooltipTriggerEl, {
             sanitize: false
```

### Comparing `fietsboek-0.7.0/fietsboek/static/fietsboek.js.map` & `fietsboek-0.8.0/fietsboek/static/fietsboek.js.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'mappings'": "';AAgBA,kDAAkD;AAClD,CAAC,CAAS,EAAE,EAAE,CAAC,IAAI,CAAC;AAOpB;;;;;;GAMG;AACH,SAAS,UAAU,CACf,QAAkB,EAClB,KAAQ,EACR,OAAoD;IAEpD,QAAQ,CAAC,gBAAgB,CAAC,QAAQ,CAAC;QAC/B,OAAO,CAAC,CAAC,GAAG,EAAE,EAAE,CAAC,GAAG,CAAC,gBAAgB,CAAC,KAAK,EAAE,OAAwB,CAAC,CAAC,CAAC;AAChF,CAAC;AAED;;;;GAIG;AACH,SAAS,UAAU,CAAC,KAAiB;IACjC,MAAM,IAAI,GAAI,KAAK,CAAC,MAAsB,CAAC,OAAO,CAAC,MAAM,CAAE,CAAC;IAC5D,IAAI,CAAC,UAAW,CAAC,WAAW,CAAC,IAAI,CAAC,CAAC;AACvC,CAAC;AAED,UAAU,CAAC,YAAY,EAAE,OAAO,EAAE,UAAU,CAAC,CAAC;AAE9C;;GAEG;AAC […]*

```diff
@@ -1,10 +1,10 @@
 {
     "file": "fietsboek.js",
-    "mappings": ";AAgBA,kDAAkD;AAClD,CAAC,CAAS,EAAE,EAAE,CAAC,IAAI,CAAC;AAOpB;;;;;;GAMG;AACH,SAAS,UAAU,CACf,QAAkB,EAClB,KAAQ,EACR,OAAoD;IAEpD,QAAQ,CAAC,gBAAgB,CAAC,QAAQ,CAAC;QAC/B,OAAO,CAAC,CAAC,GAAG,EAAE,EAAE,CAAC,GAAG,CAAC,gBAAgB,CAAC,KAAK,EAAE,OAAwB,CAAC,CAAC,CAAC;AAChF,CAAC;AAED;;;;GAIG;AACH,SAAS,UAAU,CAAC,KAAiB;IACjC,MAAM,IAAI,GAAI,KAAK,CAAC,MAAsB,CAAC,OAAO,CAAC,MAAM,CAAE,CAAC;IAC5D,IAAI,CAAC,UAAW,CAAC,WAAW,CAAC,IAAI,CAAC,CAAC;AACvC,CAAC;AAED,UAAU,CAAC,YAAY,EAAE,OAAO,EAAE,UAAU,CAAC,CAAC;AAE9C;;GAEG;AACH,SAAS,MAAM;;IACX,MAAM,MAAM,GAAG,QAAQ,CAAC,aAAa,CAAC,UAAU,CAAqB,CAAC;IACtE,IAAI,MAAM,CAAC,KAAK,KAAK,EAAE,EAAE;QACrB,OAAO;KACV;IACD,MAAM,IAAI,GAAG,QAAQ,CAAC,aAAa,CAAC,MAAM,CAAC,CAAC;IAC5C,IAAI,CAAC,SAAS,CAAC,GAAG,CAAC,WAAW,CAAC,CAAC;IAChC,IAAI,CAAC,SAAS,CAAC,GAAG,CAAC,OAAO,CAAC,CAAC;IAC5B,IAAI,CAAC,SAAS,CAAC,GAAG,CAAC,cAAc,CAAC,CAAC;IACnC,IAAI,CAAC,SAAS,CAAC,GAAG,CAAC,SAAS,CAAC,CAAC;IAC9B,IAAI,CAAC,SAAS,CAAC,GAAG,CAAC,WAAW,CAAC,CAAC;IAChC,IAAI,CAAC,gBAAgB,CAAC,OAAO,EAAE,UAAU,CAAC,CAAC;IAC3C,MAAM,IAAI,GAAG,QAAQ,CAAC,cAAc,CAAC,MAAM,CAAC,KAAK,CAAC,CAAC;IACnD,IAAI,CAAC,WAAW,CAAC,IAAI,CAAC,CAAC;IACvB,MAAM,IAAI,GAAG,QAAQ,CAAC,aAAa,CAAC,GAAG,CAAC,CAAC;IACzC,IAAI,CAAC,SAAS,CAAC,GAAG,CAAC,IAAI,CAAC,CAAC;IACzB,IAAI,CAAC,SAAS,CAAC,GAAG,CAAC,MAAM,CAAC,CAAC;IAC3B,IAAI,CAAC,WAAW,CAAC,IAAI,CAAC,CAAC;IACvB,MAAM,KAAK,GAAG,QAAQ,CAAC,aAAa,CAAC,OAAO,CAAC,CAAC;IAC9C,KAAK,CAAC,MAAM,GAAG,IAAI,CAAC;IACpB,KAAK,CAAC,IAAI,GAAG,OAAO,CAAC;IACrB,KAAK,CAAC,KAAK,GAAG,MAAM,CAAC,KAAK,CAAC;IAC3B,IAAI,CAAC,WAAW,CAAC,KAAK,CAAC,CAAC;IACxB,MAAA,QAAQ,CAAC,aAAa,CAAC,WAAW,CAAC,0CAAE,WAAW,CAAC,IAAI,CAAC,CAAC;IACvD,MAAM,KAAK,GAAG,QAAQ,CAAC,cAAc,CAAC,GAAG,CAAC,CAAC;IAC3C,MAAA,QAAQ,CAAC,aAAa,CAAC,WAAW,CAAC,0CAAE,WAAW,CAAC,KAAK,CAAC,CAAC;IACxD,MAAM,CAAC,KAAK,GAAG,EAAE,CAAC;AACtB,CAAC;AAED,UAAU,CAAC,cAAc,EAAE,OAAO,EAAE,MAAM,CAAC,CAAC;AAC5C,uCAAuC;AACvC,UAAU,CAAC,UAAU,EAAE,UAAU,EAAE,CAAC,KAAK,EAAE,EAAE;IACzC,IAAI,KAAK,CAAC,IAAI,IAAI,OAAO,EAAE;QACvB,KAAK,CAAC,cAAc,EAAE,CAAC;QACvB,MAAM,EAAE,CAAC;KACZ;AACL,CAAC,CAAC,CAAC;AAEH;;;;;GAKG;AACH,SAAS,qBAAqB,CAAC,IAAc,EAAE,MAAgB;IAC3D,MAAM,YAAY,GAAG,QAAQ,CAAC,aAAa,CAAC,IAAI,CAAqB,CAAC;IACtE,MAAM,cAAc,GAAG,QAAQ,CAAC,aAAa,CAAC,MAAM,CAAqB,CAAC;IAE1E,MAAM,IAAI,GAAG,YAAY,CAAC,OAAO,CAAC,MAAM,CAAE,CAAC;IAC3C,IAAI,CAAC,SAAS,CAAC,MAAM,CAAC,eAAe,CAAC,CAAC;IAEvC,sEAAsE;IACtE,sEAAsE;IACtE,IAAI,YAAY,CAAC,KAAK,CAAC,MAAM,IAAI,CAAC,IAAI,YAAY,CAAC,KAAK,CAAC,MAAM,GAAG,CAAC,EAAE;QACjE,YAAY,CAAC,iBAAiB,CAAC,WAAW,CAAC,CAAC;KAC/C;SAAM;QACH,YAAY,CAAC,iBAAiB,CAAC,EAAE,CAAC,CAAC;KACtC;IAED,IAAI,YAAY,CAAC,KAAK,IAAI,cAAc,CAAC,KAAK,EAAE;QAC5C,cAAc,CAAC,iBAAiB,CAAC,gBAAgB,CAAC,CAAC;KACtD;SAAM;QACH,cAAc,CAAC,iBAAiB,CAAC,EAAE,CAAC,CAAC;KACxC;AACL,CAAC;AAED,2EAA2E;AAC3E,qBAAqB,CAAC;AAEtB;;;;GAIG;AACH,SAAS,iBAAiB,CAAC,IAAc;IACrC,MAAM,SAAS,GAAG,QAAQ,CAAC,aAAa,CAAC,IAAI,CAAqB,CAAC;IACnE,IAAI,SAAS,CAAC,KAAK,CAAC,MAAM,IAAI,CAAC,EAAE;QAC7B,SAAS,CAAC,iBAAiB,CAAC,cAAc,CAAC,CAAC;KAC/C;AACL,CAAC;AAED,2EAA2E;AAC3E,iBAAiB,CAAC;AAElB;;;GAGG;AACH,SAAS,aAAa;IAClB,MAAM,aAAa,GAAI,QAAQ,CAAC,aAAa,CAAC,oBAAoB,CAAsB;QACpF,KAAK,CAAC,WAAW,EAAE,CAAC;IACxB,MAAM,YAAY,GAAG,QAAQ,CAAC,aAAa,CAAC,eAAe,CAAE,CAAC;IAC9D,YAAY,CAAC,SAAS,GAAG,EAAE,CAAC;IAC5B,KAAK,CAAC,WAAW,CAAC;SACb,IAAI,CAAC,CAAC,QAAQ,EAAE,EAAE,CAAC,QAAQ,CAAC,IAAI,EAAE,CAAC;SACnC,IAAI,CAAC,CAAC,QAAsB,EAAE,EAAE;QAC7B,MAAM,SAAS,GAAG,QAAQ,CAAC,aAAa,CAAC,wBAAwB,CAAkB,CAAC;QAEpF,yCAAyC;QACzC,MAAM,OAAO,GAAG,QAAQ,CAAC,MAAM,CAC3B,CAAC,GAAG,EAAE,EAAE,CAAC,GAAG,CAAC,IAAI,CAAC,WAAW,EAAE,CAAC,OAAO,CAAC,aAAa,CAAC,IAAI,CAAC,CAAC,CAC/D,CAAC;QAEF,OAAO,CAAC,OAAO,CAAC,CAAC,MAAM,EAAE,EAAE;;YACvB,MAAM,IAAI,GAAG,SAAS,CAAC,SAAS,CAAC,IAAI,CAAkB,CAAC;YACxD,IAAI,CAAC,eAAe,CAAC,IAAI,CAAC,CAAC;YAC1B,IAAI,CAAC,aAAa,CAAC,cAAc,CAAqB,CAAC,WAAW,GAAG,MAAM,CAAC,IAAI,CAAC;YAClF,MAAA,IAAI,CAAC,aAAa,CAAC,QAAQ,CAAC,0CAAE,gBAAgB,CAAC,OAAO,EAAE,CAAC,KAAiB,EAAE,EAAE;gBAC1E,MAAM,MAAM,GAAI,KAAK,CAAC,MAAsB,CAAC,OAAO,CAAC,QAAQ,CAAE,CAAC;gBAChE,MAAM,CAAC,UAAW,CAAC,UAAW,CAAC,WAAW,CAAC,MAAM,CAAC,UAAW,CAAC,CAAC;gBAE/D,MAAM,KAAK,GAAG,QAAQ,CAAC,aAAa,CAAC,uBAAuB,CAAE;oBAC1D,SAAS,CAAC,IAAI,CAAkB,CAAC;gBACrC,KAAK,CAAC,eAAe,CAAC,IAAI,CAAC,CAAC;gBAC3B,KAAK,CAAC,aAAa,CAAC,cAAc,CAAqB;oBACpD,WAAW,GAAG,MAAM,CAAC,IAAI,CAAC;gBAC9B,KAAK,CAAC,aAAa,CAAC,OAAO,CAAE,CAAC,KAAK,GAAG,MAAM,CAAC,EAAE,CAAC,QAAQ,EAAE,CAAC;gBAC3D,KAAK,CAAC,aAAa,CAAC,OAAO,CAAE,CAAC,eAAe,CAAC,UAAU,CAAC,CAAC;gBAC1D,KAAK,CAAC,aAAa,CAAC,QAAQ,CAAE,CAAC,gBAAgB,CAAC,OAAO,EAAE,mBAAmB,CAAC,CAAC;gBAC9E,QAAQ,CAAC,aAAa,CAAC,gBAAgB,CAAE,CAAC,WAAW,CAAC,KAAK,CAAC,CAAC;YACjE,CAAC,CAAC,CAAC;YACH,YAAY,CAAC,WAAW,CAAC,IAAI,CAAC,CAAC;QACnC,CAAC,CAAC,CAAC;IACP,CAAC,CAAC,CAAC;AACX,CAAC;AAED,UAAU,CAAC,iBAAiB,EAAE,OAAO,EAAE,GAAG,EAAE,CAAC,aAAa,EAAE,CAAC,CAAC;AAC9D,4CAA4C;AAC5C,UAAU,CAAC,oBAAoB,EAAE,UAAU,EAAE,CAAC,KAAK,EAAE,EAAE;IACnD,IAAI,KAAK,CAAC,IAAI,IAAI,OAAO,EAAE;QACvB,KAAK,CAAC,cAAc,EAAE,CAAC;QACvB,aAAa,EAAE,CAAC;KACnB;AACL,CAAC,CAAC,CAAC;AAEH;;;;GAIG;AACH,SAAS,mBAAmB,CAAC,KAAiB;IAC1C,MAAM,MAAM,GAAI,KAAK,CAAC,MAAsB,CAAC,OAAO,CAAC,QAAQ,CAAE,CAAC;IAChE,MAAM,CAAC,UAAW,CAAC,UAAW,CAAC,WAAW,CAAC,MAAM,CAAC,UAAW,CAAC,CAAC;AACnE,CAAC;AAED,UAAU,CAAC,uBAAuB,EAAE,OAAO,EAAE,mBAAmB,CAAC,CAAC;AAElE;;;;;;;;GAQG;AACH,SAAS,oBAAoB,CAAC,KAAY;;IACtC,OAAO,CAAC,GAAG,CAAC,KAAK,CAAC,CAAC;IACnB,MAAM,MAAM,GAAG,KAAK,CAAC,MAA0B,CAAC;IAChD,KAAK,MAAM,IAAI,IAAI,KAAK,CAAC,IAAI,CAAC,MAAA,MAAM,CAAC,KAAK,mCAAI,EAAE,CAAC,EAAE;QAC/C,MAAM,CAAC,mBAAmB,EAAE,CAAC;QAE7B,MAAM,KAAK,GAAG,QAAQ,CAAC,aAAa,CAAC,OAAO,CAAC,CAAC;QAC9C,KAAK,CAAC,IAAI,GAAG,MAAM,CAAC;QACpB,KAAK,CAAC,MAAM,GAAG,IAAI,CAAC;QACpB,KAAK,CAAC,IAAI,GAAG,SAAS,MAAM,CAAC,mBAAmB,GAAG,CAAC;QAEpD,MAAM,QAAQ,GAAG,IAAI,YAAY,EAAE,CAAC;QACpC,QAAQ,CAAC,KAAK,CAAC,GAAG,CAAC,IAAI,CAAC,CAAC;QACzB,KAAK,CAAC,KAAK,GAAG,QAAQ,CAAC,KAAK,CAAC;QAE7B,MAAM,OAAO,GAAG,QAAQ,CAAC,aAAa,CAAC,6BAA6B,CAAE;YAClE,SAAS,CAAC,IAAI,CAAmB,CAAC;QACtC,OAAO,CAAC,eAAe,CAAC,IAAI,CAAC,CAAC;QAC9B,OAAO,CAAC,aAAa,CAAC,KAAK,CAAE,CAAC,GAAG,GAAG,GAAG,CAAC,eAAe,CAAC,IAAI,CAAC,CAAC;QAC9D,OAAO,CAAC,aAAa,CAAC,qBAAqB,CAAE;YACzC,gBAAgB,CAAC,OAAO,EAAE,wBAAyC,CAAC,CAAC;QACzE,OAAO,CAAC,aAAa,CAAC,+BAA+B,CAAE;YACnD,gBAAgB,CAAC,OAAO,EAAE,2BAA4C,CAAC,CAAC;QAC3E,OAAO,CAAC,aAAa,CAAC,+BAA+B,CAAsB;YACxE,IAAI,GAAG,qBAAqB,MAAM,CAAC,mBAAmB,GAAG,CAAC;QAC9D,OAAO,CAAC,WAAW,CAAC,KAAK,CAAC,CAAC;QAE3B,QAAQ,CAAC,aAAa,CAAC,iBAAiB,CAAE,CAAC,WAAW,CAAC,OAAO,CAAC,CAAC;KACnE;IAED,MAAM,CAAC,KAAK,GAAG,EAAE,CAAC;AACtB,CAAC;AAED,UAAU,CAAC,gBAAgB,EAAE,QAAQ,EAAE,oBAAoB,CAAC,CAAC;AAE7D;;;;GAIG;AACH,SAAS,wBAAwB,CAAC,KAAiB;IAC/C,MAAM,OAAO,GAAI,KAAK,CAAC,MAAsB,CAAC,OAAO,CAAC,yBAAyB,CAAE,CAAC;IAClF,8DAA8D;IAC9D,MAAM,KAAK,GAAG,OAAO,CAAC,aAAa,CAAC,kBAAkB,CAAC,CAAC;IACxD,IAAI,KAAK,EAAE;QACP,OAAO,CAAC,UAAW,CAAC,WAAW,CAAC,OAAO,CAAC,CAAC;QACzC,OAAO;KACV;IAED,4EAA4E;IAC5E,MAAM,OAAO,GAAG,OAAO,CAAC,aAAa,CAAC,2BAA2B,CAAE,CAAC;IACpE,OAAO,CAAC,eAAe,CAAC,UAAU,CAAC,CAAC;IACpC,OAAO,CAAC,WAAW,CAAC,OAAO,CAAC,CAAC;IAC7B,OAAO,CAAC,UAAW,CAAC,WAAW,CAAC,OAAO,CAAC,CAAC;IACzC,OAAO,CAAC,UAAW,CAAC,WAAW,CAAC,OAAO,CAAC,CAAC;AAC7C,CAAC;AAED,UAAU,CAAC,qBAAqB,EAAE,OAAO,EAAE,wBAAwB,CAAC,CAAC;AAErE;;;;GAIG;AACH,SAAS,2BAA2B,CAAC,KAAiB;IAClD,MAAM,CAAC,qBAAqB,GAAI,KAAK,CAAC,MAAsB,CAAC,OAAO,CAAC,KAAK,CAAE,CAAC;IAE7E,MAAM,UAAU,GAEZ,MAAM,CAAC,qBAAqB,CAAC,aAAa,CAAC,+BAA+B,CAC7E,CAAC;IACF,MAAM,kBAAkB,GAAG,UAAU,CAAC,KAAK,CAAC;IAC5C,MAAM,QAAQ,GAAG,QAAQ,CAAC,cAAc,CAAC,uBAAuB,CAAE,CAAC;IACnE,QAAQ,CAAC,aAAa,CAAC,UAAU,CAAE,CAAC,KAAK,GAAG,kBAAkB,CAAC;IAE/D,MAAM,KAAK,GAAG,SAAS,CAAC,KAAK,CAAC,mBAAmB,CAAC,QAAQ,EAAE,EAAE,CAAC,CAAC;IAChE,KAAK,CAAC,IAAI,EAAE,CAAC;AACjB,CAAC;AAED,UAAU,CAAC,+BAA+B,EAAE,OAAO,EAAE,2BAA2B,CAAC,CAAC;AAElF;;;;GAIG;AACH,SAAS,2BAA2B,CAAC,MAAkB;IACnD,MAAM,QAAQ,GAAG,QAAQ,CAAC,cAAc,CAAC,uBAAuB,CAAE,CAAC;IACnE,MAAM,iBAAiB,GAAG,QAAQ,CAAC,aAAa,CAAC,UAAU,CAAE,CAAC,KAAK,CAAC;IACnE,MAAM,CAAC,qBAAsB;QAC1B,aAAa,CAAC,+BAA+B,CAAsB;QACnE,KAAK,GAAG,iBAAiB,CAAC;IAC9B,MAAM,CAAC,qBAAsB;QACzB,aAAa,CAAC,KAAK,CAAE,CAAC,KAAK,GAAG,iBAAiB,CAAC;IAEpD,MAAM,KAAK,GAAG,SAAS,CAAC,KAAK,CAAC,mBAAmB,CAAC,QAAQ,EAAE,EAAE,CAAC,CAAC;IAChE,KAAK,CAAC,IAAI,EAAE,CAAC;IAEb,MAAM,CAAC,qBAAqB,GAAG,IAAI,CAAC;AACxC,CAAC;AAED,UAAU,CAAC,2CAA2C,EAAE,OAAO,EAAE,2BAA2B,CAAC,CAAC;AAE9F;;;;GAIG;AACH,SAAS,aAAa,CAAC,KAAiB;IACpC,MAAM,OAAO,GAAG,KAAK,CAAC,MAAqB,CAAC;IAC5C,MAAM,UAAU,GAAG,OAAO,CAAC,OAAO,CAAC,GAAG,CAAE,CAAC;IACzC,MAAM,OAAO,GAAG,UAAU,CAAC,kBAAmB,CAAC;IAC/C,SAAS,CAAC,QAAQ,CAAC,mBAAmB,CAAC,OAAO,CAAC,CAAC,MAAM,EAAE,CAAC;IACzD,IAAI,OAAO,CAAC,SAAS,CAAC,QAAQ,CAAC,iBAAiB,CAAC,EAAE;QAC/C,OAAO,CAAC,SAAS,CAAC,MAAM,CAAC,iBAAiB,CAAC,CAAC;QAC5C,OAAO,CAAC,SAAS,CAAC,GAAG,CAAC,kBAAkB,CAAC,CAAC;KAC7C;SAAM;QACH,OAAO,CAAC,SAAS,CAAC,MAAM,CAAC,kBAAkB,CAAC,CAAC;QAC7C,OAAO,CAAC,SAAS,CAAC,GAAG,CAAC,iBAAiB,CAAC,CAAC;KAC5C;AACL,CAAC;AAED,UAAU,CAAC,kBAAkB,EAAE,OAAO,EAAE,aAAa,CAAC,CAAC;AAEvD;;GAEG;AACH,UAAU,CAAC,wBAAwB,EAAE,OAAO,EAAE,GAAG,EAAE;IAC/C,MAAM,OAAO,GAAG,QAAQ,CAAC,gBAAgB,CAAC,2BAA2B,CAAC,CAAC;IACvE,MAAM,GAAG,GAAG,IAAI,GAAG,CAAC,gBAAgB,EAAE,MAAM,CAAC,QAAQ,CAAC,IAAI,CAAC,CAAC;IAC5D,OAAO,CAAC,OAAO,CAAC,CAAC,CAAC,EAAE,EAAE;QAClB,GAAG,CAAC,YAAY,CAAC,MAAM,CAAC,YAAY,EAAG,CAAsB,CAAC,KAAK,CAAC,CAAC;IACzE,CAAC,CAAC,CAAC;IACH,MAAM,CAAC,QAAQ,CAAC,MAAM,CAAC,GAAG,CAAC,CAAC;AAChC,CAAC,CAAC,CAAC;AACH;;GAEG;AACH,UAAU,CAAC,mBAAmB,EAAE,QAAQ,EAAE,GAAG,EAAE;IAC3C,MAAM,OAAO,GAAG,QAAQ,CAAC,gBAAgB,CAAC,2BAA2B,CAAC,CAAC;IACvE,MAAM,cAAc,GAAG,QAAQ,CAAC,aAAa,CAAC,wBAAwB,CAAsB,CAAC;IAC7F,cAAc,CAAC,QAAQ,GAAG,CAAC,OAAO,CAAC,MAAM,IAAI,CAAC,CAAC,CAAC;AACpD,CAAC,CAAC,CAAC;AAEH;;;;;;GAMG;AACH,SAAS,uBAAuB,CAAC,KAAiB;IAC9C,MAAM,MAAM,GAAG,KAAK,CAAC,MAAqB,CAAC;IAC3C,MAAM,CAAC,OAAO,CAAC,cAAc,CAAE,CAAC,gBAAgB,CAAC,OAAO,CAAC,CAAC,OAAO,CAAC,CAAC,CAAC,EAAE,EAAE,CAAC,CAAC,CAAC,KAAK,GAAG,EAAE,CAAC,CAAC;IACvF,MAAM,CAAC,OAAO,CAAC,cAAc,CAAE,CAAC,gBAAgB,CAAC,QAAQ,CAAC,CAAC,OAAO,CAAC,CAAC,CAAC,EAAE,EAAE,CAAC,CAAC,CAAC,KAAK,GAAG,EAAE,CAAC,CAAC;AAC5F,CAAC;AAED,UAAU,CAAC,qBAAqB,EAAE,OAAO,EAAE,uBAAuB,CAAC,CAAC;AAGpE,QAAQ,CAAC,gBAAgB,CAAC,kBAAkB,EAAE;IAC1C,MAAM,CAAC,mBAAmB,GAAG,CAAC,CAAC;IAE/B,qBAAqB;IACrB,MAAM,kBAAkB,GAAG,EAAE,CAAC,KAAK,CAAC,IAAI,CACpC,QAAQ,CAAC,gBAAgB,CAAC,4BAA4B,CAAC,CAC1D,CAAC;IACF,kBAAkB,CAAC,GAAG,CAAC,CAAC,gBAAgB,EAAE,EAAE;QACxC,OAAO,IAAI,SAAS,CAAC,OAAO,CAAC,gBAAgB,EAAE,EAAE,QAAQ,EAAE,KAAK,EAAE,CAAC,CAAC;IACxE,CAAC,CAAC,CAAC;IAEH,sCAAsC;IACtC,MAAM,KAAK,GAAG,QAAQ,CAAC,gBAAgB,CAAC,mBAAmB,CAAC,CAAC;IAC7D,KAAK,CAAC,IAAI,CAAC,KAAK,CAAC,CAAC,OAAO,CAAC,CAAC,IAAI,EAAE,EAAE;QAC/B,IAAI,CAAC,gBAAgB,CAAC,QAAQ,EAAE,CAAC,KAAK,EAAE,EAAE;YACtC,IAAI,CAAE,IAAwB,CAAC,aAAa,EAAE,EAAE;gBAC5C,KAAK,CAAC,cAAc,EAAE,CAAC;gBACvB,KAAK,CAAC,eAAe,EAAE,CAAC;aAC3B;YAED,IAAI,CAAC,SAAS,CAAC,GAAG,CAAC,eAAe,CAAC,CAAC;QACxC,CAAC,EAAE,KAAK,CAAC,CAAC;IACd,CAAC,CAAC,CAAC;IAEH,gDAAgD;IAChD,QAAQ,CAAC,gBAAgB,CAAC,2BAA2B,CAAC,CAAC,OAAO,CAAC,CAAC,GAAG,EAAE,EAAE;QACnE,MAAM,SAAS,GAAG,UAAU,CAAC,GAAG,CAAC,UAAU,CAAC,YAAY,CAAC,oBAAoB,CAAE,CAAC,KAAK,CAAC,CAAC;QACvF,MAAM,IAAI,GAAG,IAAI,IAAI,CAAC,SAAS,GAAG,IAAI,CAAC,CAAC;QACxC,uEAAuE;QACvE,sCAAsC;QACtC,MAAM,IAAI,GAAG,IAAI,IAAI,CAAC,cAAc,CAAC,MAAM,EAAE;YACzC,SAAS,EAAE,QAAQ;YACnB,SAAS,EAAE,QAAQ;SACf,CAAC,CAAC;QACV,GAAG,CAAC,SAAS,GAAG,IAAI,CAAC,MAAM,CAAC,IAAI,CAAC,CAAC;IACtC,CAAC,CAAC,CAAC;AACP,CAAC,CAAC,CAAC",
+    "mappings": "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",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "../../asset-sources/fietsboek.ts"
     ],
     "version": 3
 }
```

### Comparing `fietsboek-0.7.0/fietsboek/static/fonts/bootstrap-icons.woff` & `fietsboek-0.8.0/fietsboek/static/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/fonts/bootstrap-icons.woff2` & `fietsboek-0.8.0/fietsboek/static/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/fonts/open-sans-v29-latin-300.woff` & `fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-300.woff`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/fonts/open-sans-v29-latin-300.woff2` & `fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-300.woff2`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/fonts/open-sans-v29-latin-300italic.woff` & `fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-300italic.woff`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/fonts/open-sans-v29-latin-300italic.woff2` & `fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-300italic.woff2`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/fonts/open-sans-v29-latin-500.woff` & `fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-500.woff`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/fonts/open-sans-v29-latin-500.woff2` & `fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-500.woff2`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/fonts/open-sans-v29-latin-500italic.woff` & `fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-500italic.woff`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/fonts/open-sans-v29-latin-500italic.woff2` & `fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-500italic.woff2`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/fonts/open-sans-v29-latin-600.woff` & `fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-600.woff`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/fonts/open-sans-v29-latin-600.woff2` & `fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-600.woff2`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/fonts/open-sans-v29-latin-600italic.woff` & `fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-600italic.woff`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/fonts/open-sans-v29-latin-600italic.woff2` & `fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-600italic.woff2`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/fonts/open-sans-v29-latin-700.woff` & `fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-700.woff`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/fonts/open-sans-v29-latin-700.woff2` & `fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-700.woff2`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/fonts/open-sans-v29-latin-700italic.woff` & `fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-700italic.woff`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/fonts/open-sans-v29-latin-700italic.woff2` & `fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-700italic.woff2`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/fonts/open-sans-v29-latin-800.woff` & `fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-800.woff`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/fonts/open-sans-v29-latin-800.woff2` & `fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-800.woff2`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/fonts/open-sans-v29-latin-800italic.woff` & `fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-800italic.woff`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/fonts/open-sans-v29-latin-800italic.woff2` & `fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-800italic.woff2`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/fonts/open-sans-v29-latin-italic.woff` & `fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-italic.woff`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/fonts/open-sans-v29-latin-italic.woff2` & `fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-italic.woff2`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/fonts/open-sans-v29-latin-regular.woff` & `fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-regular.woff`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/fonts/open-sans-v29-latin-regular.woff2` & `fietsboek-0.8.0/fietsboek/static/fonts/open-sans-v29-latin-regular.woff2`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/fonts.css` & `fietsboek-0.8.0/fietsboek/static/fonts.css`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/osm-monkeypatch.js` & `fietsboek-0.8.0/fietsboek/static/osm-monkeypatch.js`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/static/theme.css` & `fietsboek-0.8.0/fietsboek/static/theme.css`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,18 @@
   background: #efefef;
 }
 
 strong {
   font-weight: 700;
 }
 
+.brand-link {
+  text-decoration: none;
+}
+
 .badge-container {
   width: 50px;
   height: 50px;
   border: 1px solid #dee2e6;
   display: flex;
   justify-content: center;
   align-items: center;
```

### Comparing `fietsboek-0.7.0/fietsboek/static/theme.css.map` & `fietsboek-0.8.0/fietsboek/static/theme.css.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'mappings'": "'AAAA;EACE;EACA;EACA;EACA;;;AAGF;EACE;;;AAGF;EACE;;;AAGF;EACE;EACA;EACA;EACA;EACA;EACA;;;AAGF;EACE;EACA;;;AAGF;EACE;;;AAGF;EACE;EACA;;;AAGF;EAqCE;EACA;EACA;EACA;EACA;EACA;;AAzCA;EACE;EACA;EACA;EACA;;AAGF;EACE;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;;AAGF;EACE;EACA;;AAGF;EACE;EACA;EACA;EACA;EACA;EACA;;;AAWJ;EACI;;;AAGJ;EACE;;;AAGF;EACE;EACA;;;AAGF;EACE;EACA;;;AAGF;EACE;;;AAGF;EACE;EACA;EACA;;AAEA;EACE;EACA;;AAGF;EACE;;;AAIJ;AACA;EACE;;;AAGF;EACE;EACA;;;AAGF;EACE;;;AAGF;EACE;EAC […]*

```diff
@@ -1,10 +1,10 @@
 {
     "file": "theme.css",
-    "mappings": "AAAA;EACE;EACA;EACA;EACA;;;AAGF;EACE;;;AAGF;EACE;EACA;EACA;EACA;EACA;EACA;;;AAGF;EACE;EACA;;;AAGF;EACE;;;AAGF;EACE;EACA;;;AAGF;EAqCE;EACA;EACA;EACA;EACA;EACA;;AAzCA;EACE;EACA;EACA;EACA;;AAGF;EACE;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;;AAGF;EACE;EACA;;AAGF;EACE;EACA;EACA;EACA;EACA;EACA;;;AAWJ;EACI;;;AAGJ;EACE;;;AAGF;EACE;EACA;;;AAGF;EACE;EACA;;;AAGF;EACE;;;AAGF;EACE;EACA;EACA;;AAEA;EACE;EACA;;AAGF;EACE;;;AAIJ;AACA;EACE;;;AAGF;EACE;EACA;;;AAGF;EACE;;;AAGF;EACE;EACA;;;AAGF;EACE;;;AAGF;EACE;;;AAGF;EACE",
+    "mappings": "AAAA;EACE;EACA;EACA;EACA;;;AAGF;EACE;;;AAGF;EACE;;;AAGF;EACE;EACA;EACA;EACA;EACA;EACA;;;AAGF;EACE;EACA;;;AAGF;EACE;;;AAGF;EACE;EACA;;;AAGF;EAqCE;EACA;EACA;EACA;EACA;EACA;;AAzCA;EACE;EACA;EACA;EACA;;AAGF;EACE;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;;AAGF;EACE;EACA;;AAGF;EACE;EACA;EACA;EACA;EACA;EACA;;;AAWJ;EACI;;;AAGJ;EACE;;;AAGF;EACE;EACA;;;AAGF;EACE;EACA;;;AAGF;EACE;;;AAGF;EACE;EACA;EACA;;AAEA;EACE;EACA;;AAGF;EACE;;;AAIJ;AACA;EACE;;;AAGF;EACE;EACA;;;AAGF;EACE;;;AAGF;EACE;EACA;;;AAGF;EACE;;;AAGF;EACE;;;AAGF;EACE",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "../../asset-sources/theme.scss"
     ],
     "version": 3
 }
```

### Comparing `fietsboek-0.7.0/fietsboek/summaries.py` & `fietsboek-0.8.0/fietsboek/summaries.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,22 +5,26 @@
 
 
 class Summary:
     """A summary of a user's tracks.
 
     :ivar years: Mapping of year to :class:`YearSummary`.
     :vartype years: dict[int, YearSummary]
+    :ivar ascending: If ``True``, years will be sorted from old-to-new,
+        otherwise they will be sorted new-to-old.
+    :vartype ascending: bool
     """
 
-    def __init__(self):
+    def __init__(self, ascending: bool = True):
         self.years: Dict[int, YearSummary] = {}
+        self.ascending = ascending
 
     def __iter__(self):
         items = list(self.years.values())
-        items.sort(key=lambda y: y.year)
+        items.sort(key=lambda y: y.year, reverse=not self.ascending)
         return iter(items)
 
     def __len__(self) -> int:
         return len(self.all_tracks())
 
     def all_tracks(self) -> List[TrackWithMetadata]:
         """Returns all tracks of the summary.
@@ -30,19 +34,22 @@
         return [track for year in self for month in year for track in month.all_tracks()]
 
     def add(self, track: TrackWithMetadata):
         """Add a track to the summary.
 
         This automatically inserts the track into the right yearly summary.
 
+        :raises ValueError: If the given track has no date set.
         :param track: The track to insert.
         :type track: fietsboek.model.track.Track
         """
+        if track.date is None:
+            raise ValueError("Cannot add a track without date")
         year = track.date.year
-        self.years.setdefault(year, YearSummary(year)).add(track)
+        self.years.setdefault(year, YearSummary(year, self.ascending)).add(track)
 
     @property
     def total_length(self) -> float:
         """Returns the total length of all tracks in this summary.
 
         :return: The total length in meters.
         """
@@ -50,23 +57,27 @@
 
 
 class YearSummary:
     """A summary over a single year.
 
     :ivar year: Year number.
     :ivar months: Mapping of month to :class:`MonthSummary`.
+    :ivar ascending: If ``True``, months will be sorted from old-to-new,
+        otherwise they will be sorted new-to-old.
+    :vartype ascending: bool
     """
 
-    def __init__(self, year):
+    def __init__(self, year: int, ascending: bool = True):
         self.year: int = year
         self.months: Dict[int, MonthSummary] = {}
+        self.ascending = ascending
 
     def __iter__(self):
         items = list(self.months.values())
-        items.sort(key=lambda x: x.month)
+        items.sort(key=lambda x: x.month, reverse=not self.ascending)
         return iter(items)
 
     def __len__(self) -> int:
         return len(self.all_tracks())
 
     def all_tracks(self) -> List[TrackWithMetadata]:
         """Returns all tracks of the summary.
@@ -76,16 +87,19 @@
         return [track for month in self for track in month]
 
     def add(self, track: TrackWithMetadata):
         """Add a track to the summary.
 
         This automatically inserts the track into the right monthly summary.
 
+        :raises ValueError: If the given track has no date set.
         :param track: The track to insert.
         """
+        if track.date is None:
+            raise ValueError("Cannot add a track without date")
         month = track.date.month
         self.months.setdefault(month, MonthSummary(month)).add(track)
 
     @property
     def total_length(self) -> float:
         """Returns the total length of all tracks in this summary.
 
@@ -103,15 +117,17 @@
 
     def __init__(self, month):
         self.month: int = month
         self.tracks: List[TrackWithMetadata] = []
 
     def __iter__(self):
         items = self.tracks[:]
-        items.sort(key=lambda t: t.date)
+        # We know that sorting by date works, we even assert that all tracks
+        # have a date set.
+        items.sort(key=lambda t: t.date)  # type: ignore
         return iter(items)
 
     def __len__(self) -> int:
         return len(self.all_tracks())
 
     def all_tracks(self) -> List[TrackWithMetadata]:
         """Returns all tracks of the summary.
@@ -119,16 +135,19 @@
         :return: All tracks.
         """
         return self.tracks[:]
 
     def add(self, track: TrackWithMetadata):
         """Add a track to the summary.
 
+        :raises ValueError: If the given track has no date set.
         :param track: The track to insert.
         """
+        if track.date is None:
+            raise ValueError("Cannot add a track without date")
         self.tracks.append(track)
 
     @property
     def total_length(self) -> float:
         """Returns the total length of all tracks in this summary.
 
         :return: The total length in meters.
```

### Comparing `fietsboek-0.7.0/fietsboek/templates/admin.jinja2` & `fietsboek-0.8.0/fietsboek/templates/admin.jinja2`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/templates/browse.jinja2` & `fietsboek-0.8.0/fietsboek/templates/browse.jinja2`

 * *Files 13% similar despite different names*

```diff
@@ -101,14 +101,24 @@
             <i class="bi bi-x-octagon"></i>
             {{ _("page.browse.filters.clear_all") }}
           </a>
           <button class="btn btn-secondary" type="button" data-bs-toggle="collapse" data-bs-target="#advancedSearch" aria-expanded="false" aria-controls="advancedSearch">
             {{ _("page.browse.filters.expand_advanced") }}
           </button>
         </div>
+        <div class="col">
+          <select class="form-select" name="sort">
+            <option value="DATE_DESC" {% if request.params.get("sort") == "DATE_DESC" %}selected{% endif %}>{{ _("page.browse.sort.date") }} &ShortDownArrow;</option>
+            <option value="DATE_ASC" {% if request.params.get("sort") == "DATE_ASC" %}selected{% endif %}>{{ _("page.browse.sort.date") }} &ShortUpArrow;</option>
+            <option value="LENGTH_DESC" {% if request.params.get("sort") == "LENGTH_DESC" %}selected{% endif %}>{{ _("page.browse.sort.length") }} &ShortDownArrow;</option>
+            <option value="LENGTH_ASC" {% if request.params.get("sort") == "LENGTH_ASC" %}selected{% endif %}>{{ _("page.browse.sort.length") }} &ShortUpArrow;</option>
+            <option value="DURATION_DESC" {% if request.params.get("sort") == "DURATION_DESC" %}selected{% endif %}>{{ _("page.browse.sort.duration") }} &ShortDownArrow;</option>
+            <option value="DURATION_ASC" {% if request.params.get("sort") == "DURATION_ASC" %}selected{% endif %}>{{ _("page.browse.sort.duration") }} &ShortUpArrow;</option>
+          </select>
+        </div>
       </div>
     </form>
   </div>
   {% if tracks %}
   {% for track in tracks %}
   <div class="card mb-3">
     <h5 class="card-header">
```

### Comparing `fietsboek-0.7.0/fietsboek/templates/create_account.jinja2` & `fietsboek-0.8.0/fietsboek/templates/create_account.jinja2`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/templates/details.jinja2` & `fietsboek-0.8.0/fietsboek/templates/details.jinja2`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/templates/edit.jinja2` & `fietsboek-0.8.0/fietsboek/templates/edit.jinja2`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/templates/edit_form.jinja2` & `fietsboek-0.8.0/fietsboek/templates/edit_form.jinja2`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/templates/finish_upload.jinja2` & `fietsboek-0.8.0/fietsboek/templates/finish_upload.jinja2`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/templates/home.jinja2` & `fietsboek-0.8.0/fietsboek/templates/home.jinja2`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 {% extends "layout.jinja2" %}
 
 {% block content %}
 <div class="container">
-  <h1>{{ _("page.home.title") }}</h1>
+  <div class="clearfix">
+    <h1 class="float-start">{{ _("page.home.title") }}</h1>
+    {% if summary %}
+    <div class="float-end mb-2 mt-2">
+      <button type="button" class="btn btn-outline-dark" id="changeHomeSorting">
+        {% if sorted_ascending %}<i class="bi bi-sort-down"></i>{% else %}<i class="bi bi-sort-up"></i>{% endif %}
+      </button>
+    </div>
+    {% endif %}
+  </div>
   {% if unfinished_uploads %}
   <div class="alert alert-warning">
     {{ _("page.home.unfinished_uploads") }}
     <ul class="mb-0">
       {% for upload in unfinished_uploads %}
       <li><a href="{{ request.route_url("finish-upload", upload_id=upload.id) }}">{{ upload.uploaded_at | local_datetime }}</a></li>
       {% endfor %}
```

#### html2text {}

```diff
@@ -1,9 +1,12 @@
 {% extends "layout.jinja2" %} {% block content %}
 ****** {{ _("page.home.title") }} ******
+{% if summary %}
+ {% if sorted_ascending %}{% else %}{% endif %}
+{% endif %}
 {% if unfinished_uploads %}
 {{ _("page.home.unfinished_uploads") }}
     * {% for upload in unfinished_uploads %}
     * , upload_id=upload.id) }}">{{ upload.uploaded_at | local_datetime }}
 {% endfor %}
 {% endif %} {% if summary %}
 {% for year in summary %}
```

### Comparing `fietsboek-0.7.0/fietsboek/templates/layout.jinja2` & `fietsboek-0.8.0/fietsboek/templates/layout.jinja2`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,17 @@
     </script>
 
   </head>
 
   <body>
     <nav class="navbar navbar-dark bg-dark navbar-expand-lg">
       <div class="container-fluid">
-        <span class="navbar-brand mb-0 h1"><i class="bi bi-bicycle"></i> Fietsboek</span>
+        <a href="{{ request.route_url('home') }}" class="brand-link">
+          <span class="navbar-brand mb-0 h1"><i class="bi bi-bicycle"></i> Fietsboek</span>
+        </a>
         <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbar" aria-controls="navbar" aria-expanded="false" aria-label="{{ _('page.navbar.toggle') }}">
           <span class="navbar-toggler-icon"></span>
         </button>
         <div class="collapse navbar-collapse" id="navbar">
           <ul class="navbar-nav w-100 mb-2 mb-lg-0">
             {% for page in request.pages.pre_menu_items(request) %}
             <li class="nav-item">
@@ -113,15 +115,15 @@
     {% block content %}
     {% endblock %}
     <!-- Bootstrap core JavaScript
     ================================================== -->
     <!-- Placed at the end of the document so the pages load faster -->
     <script src="{{request.static_url('fietsboek:static/bootstrap.bundle.min.js')}}"></script>
     <!-- Pre-load leaflet Javascript. This lets us use Leaflet on any page, without relying on GPXViewer to load it -->
-    <script src="{{request.static_url('fietsboek:static/GM_Utils/leaflet/leaflet.js')}}">
+    <script src="{{request.static_url('fietsboek:static/GM_Utils/leaflet/leaflet.js')}}"></script>
     <!-- Our patch to the GPX viewer, load before the actual GPX viewer -->
     <script src="{{request.static_url('fietsboek:static/osm-monkeypatch.js')}}"></script>
     <!-- Jürgen Berkemeier's GPX viewer -->
     <script src="{{request.static_url('fietsboek:static/GM_Utils/GPX2GM.js')}}"></script>
     <script src="{{request.static_url('fietsboek:static/fietsboek.js')}}"></script>
     {% block latescripts %}
     {% endblock %}
```

#### html2text {}

```diff
@@ -4,14 +4,15 @@
 
 
 
 
 
 
  Fietsboek
+
     * {% for page in request.pages.pre_menu_items(request) %}
     * {{_page.link_name_}}
     * {% endfor %}
     * {{__("page.navbar.home")_}}
     * {{__("page.navbar.browse")_}}
     * {% if request.identity is not none %}
     * {{__("page.navbar.upload")_}}
@@ -34,8 +35,9 @@
           o {{__("page.navbar.create_account")_}}
           o {% endif %} {% endif %}
  {% for message in request.session.pop_flash() %}
 {{message}}
 {% endfor %} {% block content %} {% endblock %}
 
 
+
  {% block latescripts %} {% endblock %}
```

### Comparing `fietsboek-0.7.0/fietsboek/templates/login.jinja2` & `fietsboek-0.8.0/fietsboek/templates/login.jinja2`

 * *Files 6% similar despite different names*

```diff
@@ -37,12 +37,14 @@
       <div class="col-auto mb-3">
         <button type="submit" class="btn btn-primary"><i class="bi bi-door-open"></i> {{ _("page.login.submit") }}</button>
       </div>
     </div>
     <div class="row justify-content-center">
       <div class="col-auto mb-3">
         <a href="{{ request.route_url("password-reset") }}">{{ _("page.login.forgot_password") }}</a>
+        &bull;
+        <a href="{{ request.route_url("resend-verification") }}">{{ _("page.login.resend_verification") }}</a>
       </div>
     </div>
   </form>
 </div>
 {% endblock content %}
```

#### html2text {}

```diff
@@ -3,8 +3,10 @@
 ****** {{ _("page.login.title") }} ******
 [Unknown INPUT type] {{ _("page.login.email") }}
 [********************] {{ _("page.login.password") }}
 ⁰  {{ _("page.login.remember-me") }}
 {{ util.hidden_csrf_input() }}
  {{ _("page.login.submit") }}
 ) }}">{{ _("page.login.forgot_password") }}
+ •
+) }}">{{ _("page.login.resend_verification") }}
 {% endblock content %}
```

### Comparing `fietsboek-0.7.0/fietsboek/templates/password_reset.jinja2` & `fietsboek-0.8.0/fietsboek/templates/password_reset.jinja2`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/templates/profile.jinja2` & `fietsboek-0.8.0/fietsboek/templates/profile.jinja2`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/templates/request_password.jinja2` & `fietsboek-0.8.0/fietsboek/templates/request_password.jinja2`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/templates/upload.jinja2` & `fietsboek-0.8.0/fietsboek/templates/upload.jinja2`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/templates/user_data.jinja2` & `fietsboek-0.8.0/fietsboek/templates/user_data.jinja2`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/transformers/breaks.py` & `fietsboek-0.8.0/fietsboek/transformers/breaks.py`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/updater/__init__.py` & `fietsboek-0.8.0/fietsboek/updater/__init__.py`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/updater/cli.py` & `fietsboek-0.8.0/fietsboek/updater/cli.py`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/updater/script.py` & `fietsboek-0.8.0/fietsboek/updater/script.py`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/updater/scripts/upd_20230103_lu8w3rwlz4ddcpms.py` & `fietsboek-0.8.0/fietsboek/updater/scripts/upd_20230103_lu8w3rwlz4ddcpms.py`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/updater/scripts/upd_30ppwg8zi4ujb46f.py` & `fietsboek-0.8.0/fietsboek/updater/scripts/upd_30ppwg8zi4ujb46f.py`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/util.py` & `fietsboek-0.8.0/fietsboek/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 """Various utility functions."""
 import datetime
+import html
 import importlib.resources
 import os
 import re
 import secrets
 import unicodedata
-from typing import List, Optional, Union
+from typing import List, Optional, TypeVar, Union
 
 import babel
 import gpxpy
 import markdown
 import nh3
 import sqlalchemy
 import webob
 from markupsafe import Markup
 from pyramid.httpexceptions import HTTPBadRequest
 from pyramid.i18n import TranslationString as _
 from pyramid.request import Request
 from sqlalchemy import select
 
+T = TypeVar("T")
+
 ALLOWED_TAGS = (
     # Those were the bleach defaults, they worked fine
     {"a", "abbr", "acronym", "b", "blockquote", "code", "em", "i", "li", "ol", "strong", "ul"}
     # Allow headings
     .union({"h1", "h2", "h3", "h4", "h5", "h6"})
     .union({"p"})
     .union({"img"})
@@ -61,17 +64,17 @@
 
     This uses ``markdown`` to first parse the markdown source into HTML, and
     then ``bleach`` to strip any disallowed HTML tags.
 
     :param md_source: The markdown source.
     :return: The safe HTML transformed version.
     """
-    html = markdown.markdown(md_source, output_format="html")
-    html = nh3.clean(html, tags=ALLOWED_TAGS, attributes=ALLOWED_ATTRIBUTES)
-    return Markup(html)
+    converted = markdown.markdown(md_source, output_format="html")
+    converted = nh3.clean(converted, tags=ALLOWED_TAGS, attributes=ALLOWED_ATTRIBUTES)
+    return Markup(converted)
 
 
 def fix_iso_timestamp(timestamp: str) -> str:
     """Fixes an ISO timestamp to make it parseable by
     :meth:`datetime.datetime.fromisoformat`.
 
     This removes an 'Z' if it exists at the end of the timestamp, and replaces
@@ -198,14 +201,37 @@
 
     :param mps: Input meters/second.
     :return: The converted km/h value.
     """
     return mps / 1000 * 60 * 60
 
 
+def human_size(num_bytes: int) -> str:
+    """Formats the amount of bytes for human consumption.
+
+    :param num_bytes: The amount of bytes.
+    :return: The formatted amount.
+    """
+    num_bytes = float(num_bytes)
+    suffixes = ["B", "KiB", "MiB", "GiB"]
+    prefix = ""
+    if num_bytes < 0:
+        prefix = "-"
+        num_bytes = -num_bytes
+    for suffix in suffixes:
+        if num_bytes < 1024 or suffix == suffixes[-1]:
+            if suffix == "B":
+                # Don't do the decimal point for bytes
+                return f"{prefix}{int(num_bytes)} {suffix}"
+            return f"{prefix}{num_bytes:.1f} {suffix}"
+        num_bytes /= 1024
+    # Unreachable:
+    return ""
+
+
 def month_name(request: Request, month: int) -> str:
     """Returns the localized name for the month with the given number.
 
     :param request: The pyramid request.
     :param month: Number of the month, 1 = January.
     :return: The localized month name.
     """
@@ -223,18 +249,18 @@
     :return: A randomly drawn string.
     """
     return secrets.token_urlsafe(nbytes)
 
 
 def retrieve_multiple(
     dbsession: "sqlalchemy.orm.session.Session",
-    model: type,
+    model: type[T],
     params: "webob.multidict.NestedMultiDict",
     name: str,
-) -> list:
+) -> list[T]:
     """Parses a reply to retrieve multiple database objects.
 
     This is usable for arrays sent by HTML forms, for example to retrieve all
     badges or all tagged friends.
 
     If an object could not be found, this raises a
     :class:`~pyramid.httpexceptions.HTTPBadRequest`.
@@ -350,14 +376,30 @@
     kwargs["x"] = "__x__"
     kwargs["y"] = "__y__"
     kwargs["z"] = "__z__"
     route = request.route_url(route_name, **kwargs)
     return route.replace("__x__", "{x}").replace("__y__", "{y}").replace("__z__", "{z}")
 
 
+def encode_gpx(gpx: gpxpy.gpx.GPX) -> bytes:
+    """Encodes a GPX in-memory representation to the XML representation.
+
+    This ensures that the resulting XML file is valid.
+
+    Returns the contents of the XML as bytes, ready to be written to disk.
+
+    :param gpx: The GPX file to encode. Might be modified!
+    :return: The encoded GPX content.
+    """
+    for track in gpx.tracks:
+        if track.link:
+            track.link = html.escape(track.link)
+    return gpx.to_xml().encode("utf-8")
+
+
 def secure_filename(filename: str) -> str:
     r"""Pass it a filename and it will return a secure version of it.  This
     filename can then safely be stored on a regular file system and passed
     to :func:`os.path.join`.  The filename returned is an ASCII only string
     for maximum portability.
     On windows systems the function also makes sure that the file is not
     named after one of the special device files.
```

### Comparing `fietsboek-0.7.0/fietsboek/views/account.py` & `fietsboek-0.8.0/fietsboek/views/account.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Account related endpoints."""
 from pyramid.httpexceptions import HTTPForbidden, HTTPFound
 from pyramid.i18n import TranslationString as _
 from pyramid.view import view_config
 
-from .. import email, models, util
-from ..models.user import TokenType
+from .. import actions, models, util
 
 
 @view_config(
     route_name="create-account",
     renderer="fietsboek:templates/create_account.jinja2",
     request_method="GET",
 )
@@ -59,29 +58,11 @@
         request.session.flash(request.localizer.translate(_("flash.invalid_email")))
         return HTTPFound(request.route_url("create-account"))
 
     user = models.User(name=name, email=email_addr)
     user.set_password(password)
     request.dbsession.add(user)
 
-    token = models.Token.generate(user, TokenType.VERIFY_EMAIL)
-    request.dbsession.add(token)
-
-    message = email.prepare_message(
-        request.config.email_from,
-        user.email,
-        request.localizer.translate(_("email.verify_mail.subject")),
-    )
-    message.set_content(
-        request.localizer.translate(_("email.verify.text")).format(
-            request.route_url("use-token", uuid=token.uuid)
-        )
-    )
-    email.send_message(
-        request.config.email_smtp_url,
-        request.config.email_username,
-        request.config.email_password.get_secret_value(),
-        message,
-    )
+    actions.send_verification_token(request, user)
 
     request.session.flash(request.localizer.translate(_("flash.a_confirmation_link_has_been_sent")))
     return HTTPFound(request.route_url("login"))
```

### Comparing `fietsboek-0.7.0/fietsboek/views/admin.py` & `fietsboek-0.8.0/fietsboek/views/admin.py`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/views/default.py` & `fietsboek-0.8.0/fietsboek/views/default.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 """Home views."""
 from markupsafe import Markup
 from pyramid.httpexceptions import HTTPFound, HTTPNotFound
 from pyramid.i18n import TranslationString as _
 from pyramid.interfaces import ISecurityPolicy
 from pyramid.renderers import render_to_response
+from pyramid.request import Request
+from pyramid.response import Response
 from pyramid.security import forget, remember
 from pyramid.view import view_config
 from sqlalchemy import select
 from sqlalchemy.exc import NoResultFound
 from sqlalchemy.orm import aliased
 
-from .. import email, models, summaries, util
+from .. import actions, email, models, summaries, util
 from ..models.track import TrackType, TrackWithMetadata
-from ..models.user import PasswordMismatch, TokenType
+from ..models.user import TOKEN_LIFETIME, PasswordMismatch, TokenType
 
 
 @view_config(route_name="home", renderer="fietsboek:templates/home.jinja2")
-def home(request):
+def home(request: Request) -> Response:
     """Renders the home page.
 
     :param request: The Pyramid request.
-    :type request: pyramid.request.Request
     :return: The HTTP response.
-    :rtype: pyramid.response.Response
     """
     if not request.identity:
         # See if the admin set a custom home page
         page = request.pages.find("/", request)
         if page is not None:
             return render_to_response(
                 "fietsboek:templates/static-page.jinja2",
@@ -44,74 +44,72 @@
             "html/home.html",
             locale_packages=request.config.language_packs,
         )
         return {
             "home_content": content,
         }
 
+    sorting = request.cookies.get("home_sorting", "asc")
+    ascending = sorting == "asc"
+
     query = request.identity.all_tracks_query()
     query = select(aliased(models.Track, query)).where(query.c.type == TrackType.ORGANIC)
-    summary = summaries.Summary()
+    summary = summaries.Summary(ascending=ascending)
 
     for track in request.dbsession.execute(query).scalars():
         if track.cache is None:
             gpx_data = request.data_manager.open(track.id).decompress_gpx()
             track.ensure_cache(gpx_data)
             request.dbsession.add(track.cache)
         summary.add(TrackWithMetadata(track, request.data_manager))
 
     unfinished_uploads = request.identity.uploads
 
     return {
         "summary": summary,
         "month_name": util.month_name,
         "unfinished_uploads": unfinished_uploads,
+        "sorted_ascending": ascending,
     }
 
 
 @view_config(route_name="static-page", renderer="fietsboek:templates/static-page.jinja2")
-def static_page(request):
+def static_page(request: Request) -> Response:
     """Renders a static page.
 
     :param request: The Pyramid request.
-    :type request: pyramid.request.Request
     :return: The HTTP response.
-    :rtype: pyramid.response.Response
     """
     page = request.pages.find(request.matchdict["slug"], request)
     if page is None:
         return HTTPNotFound()
 
     return {
         "title": page.title,
         "content": Markup(page.content),
     }
 
 
 @view_config(route_name="login", renderer="fietsboek:templates/login.jinja2", request_method="GET")
-def login(request):
+def login(request: Request) -> Response:
     """Renders the login page.
 
     :param request: The Pyramid request.
-    :type request: pyramid.request.Request
     :return: The HTTP response.
-    :rtype: pyramid.response.Response
     """
     # pylint: disable=unused-argument
     return {}
 
 
 @view_config(route_name="login", request_method="POST")
-def do_login(request):
+def do_login(request: Request) -> Response:
     """Endpoint for the login form.
 
     :param request: The Pyramid request.
-    :type request: pyramid.request.Request
     :return: The HTTP response.
-    :rtype: pyramid.response.Response
     """
     query = models.User.query_by_email(request.params["email"])
     try:
         user = request.dbsession.execute(query).scalar_one()
         user.check_password(request.params["password"])
     except (NoResultFound, PasswordMismatch):
         request.session.flash(request.localizer.translate(_("flash.invalid_credentials")))
@@ -131,52 +129,46 @@
         headers += policy.remember_cookie(request, str(user.id))
 
     response = HTTPFound("/", headers=headers)
     return response
 
 
 @view_config(route_name="logout")
-def logout(request):
+def logout(request: Request) -> Response:
     """Logs the user out.
 
     :param request: The Pyramid request.
-    :type request: pyramid.request.Request
     :return: The HTTP response.
-    :rtype: pyramid.response.Response
     """
     request.session.flash(request.localizer.translate(_("flash.logged_out")))
     headers = forget(request)
     return HTTPFound("/", headers=headers)
 
 
 @view_config(
     route_name="password-reset",
     request_method="GET",
     renderer="fietsboek:templates/request_password.jinja2",
 )
-def password_reset(request):
+def password_reset(request: Request) -> Response:
     """Form to request a new password.
 
     :param request: The Pyramid request.
-    :type request: pyramid.request.Request
     :return: The HTTP response.
-    :rtype: pyramid.response.Response
     """
     # pylint: disable=unused-argument
     return {}
 
 
 @view_config(route_name="password-reset", request_method="POST")
-def do_password_reset(request):
+def do_password_reset(request: Request) -> Response:
     """Endpoint for the password request form.
 
     :param request: The Pyramid request.
-    :type request: pyramid.request.Request
     :return: The HTTP response.
-    :rtype: pyramid.response.Response
     """
     query = models.User.query_by_email(request.params["email"])
     user = request.dbsession.execute(query).scalar_one_or_none()
     if user is None:
         request.session.flash(request.localizer.translate(_("flash.reset_invalid_email")))
         return HTTPFound(request.route_url("password-reset"))
 
@@ -200,30 +192,67 @@
         request.config.email_password.get_secret_value(),
         mail,
     )
 
     return HTTPFound(request.route_url("password-reset"))
 
 
+@view_config(
+    route_name="resend-verification",
+    request_method="GET",
+    renderer="fietsboek:templates/resend_verification.jinja2",
+)
+def resend_verification(_request: Request) -> Response:
+    """Form to request a new verification mail.
+
+    :param request: The Pyramid request.
+    :return: The HTTP response.
+    """
+    return {}
+
+
+@view_config(route_name="resend-verification", request_method="POST")
+def do_resend_verification(request: Request) -> Response:
+    """Endpoint for the verification resend form.
+
+    :param request: The Pyramid request.
+    :return: The HTTP response.
+    """
+    query = models.User.query_by_email(request.params["email"])
+    user = request.dbsession.execute(query).scalar_one_or_none()
+    if user is None or user.is_verified:
+        request.session.flash(
+            request.localizer.translate(_("flash.resend_verification_email_fail"))
+        )
+        return HTTPFound(request.route_url("resend-verification"))
+
+    actions.send_verification_token(request, user)
+    request.session.flash(request.localizer.translate(_("flash.verification_token_generated")))
+
+    return HTTPFound(request.route_url("login"))
+
+
 @view_config(route_name="use-token")
-def use_token(request):
+def use_token(request: Request) -> Response:
     """Endpoint with which a user can use a token for a password reset or email
     verification.
 
     :param request: The Pyramid request.
-    :type request: pyramid.request.Request
     :return: The HTTP response.
-    :rtype: pyramid.response.Response
     """
     token = request.dbsession.execute(
         select(models.Token).filter_by(uuid=request.matchdict["uuid"])
     ).scalar_one_or_none()
     if token is None:
         return HTTPNotFound()
 
+    if token.age() > TOKEN_LIFETIME:
+        request.session.flash(request.localizer.translate(_("flash.token_expired")))
+        return HTTPFound(request.route_url("home"))
+
     if token.token_type == TokenType.VERIFY_EMAIL:
         token.user.is_verified = True
         request.dbsession.delete(token)
         request.session.flash(request.localizer.translate(_("flash.email_verified")))
         return HTTPFound(request.route_url("login"))
     if request.method == "GET" and token.token_type == TokenType.RESET_PASSWORD:
         return render_to_response("fietsboek:templates/password_reset.jinja2", {}, request)
@@ -235,8 +264,8 @@
             request.session.flash(request.localizer.translate(exc.args[0]))
             return HTTPFound(request.route_url("use-token", uuid=token.uuid))
 
         token.user.set_password(password)
         request.dbsession.delete(token)
         request.session.flash(request.localizer.translate(_("flash.password_updated")))
         return HTTPFound(request.route_url("login"))
-    return None
+    raise NotImplementedError("No matching action found")
```

### Comparing `fietsboek-0.7.0/fietsboek/views/detail.py` & `fietsboek-0.8.0/fietsboek/views/detail.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,25 @@
 
 from .. import models, util
 from ..models.track import TrackWithMetadata
 
 LOGGER = logging.getLogger(__name__)
 
 
+def _sort_key(image_name: str) -> str:
+    """Returns the "key" by which the image should be sorted.
+
+    :param image_name: Name of the image (on disk).
+    :return: The value that should be used to sort the image.
+    """
+    if "_" not in image_name:
+        return image_name
+    return image_name.split("_", 1)[1]
+
+
 @view_config(
     route_name="details", renderer="fietsboek:templates/details.jinja2", permission="track.view"
 )
 def details(request):
     """Renders the detail page for a given track.
 
     :param request: The Pyramid request.
@@ -47,17 +58,21 @@
         query = []
         if "secret" in request.GET:
             query.append(("secret", request.GET["secret"]))
         img_src = request.route_url("image", track_id=track.id, image_name=image_name, _query=query)
         query = select(models.ImageMetadata).filter_by(track=track, image_name=image_name)
         image_metadata = request.dbsession.execute(query).scalar_one_or_none()
         if image_metadata:
-            images.append((img_src, image_metadata.description))
+            images.append((_sort_key(image_name), img_src, image_metadata.description))
         else:
-            images.append((img_src, ""))
+            images.append((_sort_key(image_name), img_src, ""))
+
+    images.sort(key=lambda element: element[0])
+    # Strip off the sort key again
+    images = [(image[1], image[2]) for image in images]
 
     with_meta = TrackWithMetadata(track, request.data_manager)
     return {
         "track": with_meta,
         "show_organic": track.show_organic_data(),
         "show_edit_link": show_edit_link,
         "mps_to_kph": util.mps_to_kph,
```

### Comparing `fietsboek-0.7.0/fietsboek/views/edit.py` & `fietsboek-0.8.0/fietsboek/views/edit.py`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/views/profile.py` & `fietsboek-0.8.0/fietsboek/views/profile.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,14 +12,39 @@
 from sqlalchemy import select
 from sqlalchemy.orm import aliased
 
 from .. import models, util
 from ..data import UserDataDir
 from ..models.track import TrackType, TrackWithMetadata
 
+# A well-made transparent tile is actually pretty small (only 116 bytes), which
+# is even smaller than our HTTP 404 page. So not only is it more efficient
+# (bandwidth-wise) to transfer the transparent PNG, it also means that we can
+# set cache headers, which the client will honor.
+#
+# Since the tile is so small, we've embedded it right here in the source.
+#
+# The tile is taken and adapted from hittekaart, which in turn took inspiration
+# from https://www.mjt.me.uk/posts/smallest-png/ and
+# http://www.libpng.org/pub/png/spec/1.2/PNG-Contents.html
+# fmt: off
+EMPTY_TILE = bytes([
+    0x89, 0x50, 0x4e, 0x47, 0x0d, 0x0a, 0x1a, 0x0a, 0x00, 0x00, 0x00, 0x0d,
+    0x49, 0x48, 0x44, 0x52, 0x00, 0x00, 0x01, 0x00, 0x00, 0x00, 0x01, 0x00,
+    0x01, 0x03, 0x00, 0x00, 0x00, 0x66, 0xbc, 0x3a, 0x25, 0x00, 0x00, 0x00,
+    0x03, 0x50, 0x4c, 0x54, 0x45, 0x00, 0xff, 0x00, 0x34, 0x5e, 0xc0, 0xa8,
+    0x00, 0x00, 0x00, 0x01, 0x74, 0x52, 0x4e, 0x53, 0x00, 0x40, 0xe6, 0xd8,
+    0x66, 0x00, 0x00, 0x00, 0x1f, 0x49, 0x44, 0x41, 0x54, 0x68, 0x81, 0xed,
+    0xc1, 0x01, 0x0d, 0x00, 0x00, 0x00, 0xc2, 0xa0, 0xf7, 0x4f, 0x6d, 0x0e,
+    0x37, 0xa0, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0xbe, 0x0d,
+    0x21, 0x00, 0x00, 0x01, 0x9a, 0x60, 0xe1, 0xd5, 0x00, 0x00, 0x00, 0x00,
+    0x49, 0x45, 0x4e, 0x44, 0xae, 0x42, 0x60, 0x82,
+])
+# fmt: on
+
 
 @dataclass
 class CumulativeStats:
     """Cumulative user stats.
 
     The values start out with default values, and tracks can be merged in via
     :meth:`add`.
@@ -153,15 +178,20 @@
         "total": total,
         "mps_to_kph": util.mps_to_kph,
         "heatmap_url": heatmap_url,
         "tilehunt_url": tilehunt_url,
     }
 
 
-@view_config(route_name="user-tile", request_method="GET", permission="profile.view")
+@view_config(
+    route_name="user-tile",
+    request_method="GET",
+    permission="profile.view",
+    http_cache=datetime.timedelta(hours=1),
+)
 def user_tile(request: Request) -> Response:
     """Returns a single tile from the user's own overlay maps.
 
     :param request: The pyramid request.
     :return: The response, with the tile content (or an error).
     """
     try:
@@ -190,13 +220,13 @@
     cursor = connection.cursor()
     result = cursor.execute(
         "SELECT data FROM tiles WHERE zoom = ? AND x = ? AND y = ?;",
         (int(request.matchdict["z"]), int(request.matchdict["x"]), int(request.matchdict["y"])),
     )
     result = result.fetchone()
     if result is None:
-        return HTTPNotFound()
+        return Response(EMPTY_TILE, content_type="image/png")
 
     return Response(result[0], content_type="image/png")
 
 
 __all__ = ["profile", "user_tile"]
```

### Comparing `fietsboek-0.7.0/fietsboek/views/tileproxy.py` & `fietsboek-0.8.0/fietsboek/views/tileproxy.py`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/fietsboek/views/upload.py` & `fietsboek-0.8.0/fietsboek/views/upload.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import gpxpy
 from pyramid.httpexceptions import HTTPBadRequest, HTTPFound
 from pyramid.i18n import TranslationString as _
 from pyramid.response import Response
 from pyramid.view import view_config
 from sqlalchemy import select
 
-from .. import actions, models, transformers, util
+from .. import actions, convert, models, transformers, util
 from ..models.track import TrackType, Visibility
 
 LOGGER = logging.getLogger(__name__)
 
 
 @view_config(
     route_name="upload",
@@ -48,14 +48,17 @@
     """
     try:
         gpx = request.POST["gpx"].file.read()
     except AttributeError:
         request.session.flash(request.localizer.translate(_("flash.no_file_selected")))
         return HTTPFound(request.route_url("upload"))
 
+    if len(gpx) > 11 and gpx[9:12] == b"FIT":
+        gpx = convert.from_fit(gpx).to_xml().encode("utf-8")
+
     # Before we do anything, we check if we can parse the file.
     # gpxpy might throw different exceptions, so we simply catch `Exception`
     # here - if we can't parse it, we don't care too much why at this point.
     # pylint: disable=broad-except
     try:
         gpxpy.parse(gpx)
     except Exception as exc:
```

### Comparing `fietsboek-0.7.0/fietsboek/views/user_data.py` & `fietsboek-0.8.0/fietsboek/views/user_data.py`

 * *Files identical despite different names*

### Comparing `fietsboek-0.7.0/pyproject.toml` & `fietsboek-0.8.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "fietsboek"
 description = "GPX file sharing website"
-version = "0.7.0"
+version = "0.8.0"
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 authors = [
     "Daniel Schadt <fietsboek@kingdread.de>",
 ]
 classifiers = [
     'Development Status :: 3 - Alpha',
@@ -30,39 +30,40 @@
 pyramid = "^2"
 pyramid_jinja2 = "^2.10"
 pyramid_debugtoolbar = "^4.9"
 pyramid_retry = "^2.1"
 pyramid_tm = "^2.5"
 waitress = "^2.1"
 
-SQLAlchemy = "^1.4"
+SQLAlchemy = { version = "^2.0.15", extras = ["mypy"] }
 alembic = "^1.8"
 transaction = "^3"
-"zope.sqlalchemy" = "^2.0"
+"zope.sqlalchemy" = "^3.0"
 redis = "^4.3.4"
 
 Babel = "^2.11"
-cryptography = "^40.0.2"
+cryptography = "^41.0.1"
 gpxpy = "^1.5"
 markdown = "^3.4"
 nh3 = "^0.2.9"
 Click = "^8.1"
 requests = "^2.28.1"
 
 pydantic = "^1.10.2"
 termcolor = "^2.1.1"
 filelock = "^3.8.2"
 brotli = "^1.0.9"
 click-option-group = "^0.5.5"
+fitparse = "^1.2.0"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
-Sphinx = "^6.1"
+Sphinx = "^7.0"
 sphinx-autodoc-typehints = "^1.19.5"
 
 [tool.poetry.group.testing]
 optional = true
 
 [tool.poetry.group.testing.dependencies]
 pytest = "^7.2.0"
```

### Comparing `fietsboek-0.7.0/PKG-INFO` & `fietsboek-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fietsboek
-Version: 0.7.0
+Version: 0.8.0
 Summary: GPX file sharing website
 Home-page: https://fietsboek.org/
 License: AGPL-3.0-or-later
 Keywords: web,gpx
 Author: Daniel Schadt
 Author-email: fietsboek@kingdread.de
 Requires-Python: >=3.9,<4.0
@@ -17,35 +17,36 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Requires-Dist: Babel (>=2.11,<3.0)
 Requires-Dist: Click (>=8.1,<9.0)
-Requires-Dist: SQLAlchemy (>=1.4,<2.0)
+Requires-Dist: SQLAlchemy[mypy] (>=2.0.15,<3.0.0)
 Requires-Dist: alembic (>=1.8,<2.0)
 Requires-Dist: brotli (>=1.0.9,<2.0.0)
 Requires-Dist: click-option-group (>=0.5.5,<0.6.0)
-Requires-Dist: cryptography (>=40.0.2,<41.0.0)
+Requires-Dist: cryptography (>=41.0.1,<42.0.0)
 Requires-Dist: filelock (>=3.8.2,<4.0.0)
+Requires-Dist: fitparse (>=1.2.0,<2.0.0)
 Requires-Dist: gpxpy (>=1.5,<2.0)
 Requires-Dist: markdown (>=3.4,<4.0)
 Requires-Dist: nh3 (>=0.2.9,<0.3.0)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: pyramid (>=2,<3)
 Requires-Dist: pyramid_debugtoolbar (>=4.9,<5.0)
 Requires-Dist: pyramid_jinja2 (>=2.10,<3.0)
 Requires-Dist: pyramid_retry (>=2.1,<3.0)
 Requires-Dist: pyramid_tm (>=2.5,<3.0)
 Requires-Dist: redis (>=4.3.4,<5.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: termcolor (>=2.1.1,<3.0.0)
 Requires-Dist: transaction (>=3,<4)
 Requires-Dist: waitress (>=2.1,<3.0)
-Requires-Dist: zope.sqlalchemy (>=2.0,<3.0)
+Requires-Dist: zope.sqlalchemy (>=3.0,<4.0)
 Project-URL: Documentation, https://docs.fietsboek.org/
 Project-URL: Repository, https://gitlab.com/dunj3/fietsboek
 Description-Content-Type: text/markdown
 
 Fietsboek
 =========
```

#### html2text {}

```diff
@@ -1,49 +1,49 @@
-Metadata-Version: 2.1 Name: fietsboek Version: 0.7.0 Summary: GPX file sharing
+Metadata-Version: 2.1 Name: fietsboek Version: 0.8.0 Summary: GPX file sharing
 website Home-page: https://fietsboek.org/ License: AGPL-3.0-or-later Keywords:
 web,gpx Author: Daniel Schadt Author-email: fietsboek@kingdread.de Requires-
 Python: >=3.9,<4.0 Classifier: Development Status :: 3 - Alpha Classifier:
 Framework :: Pyramid Classifier: License :: OSI Approved :: GNU Affero General
 Public License v3 or later (AGPLv3+) Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
 Internet :: WWW/HTTP Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic
 Content Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Requires-Dist: Babel (>=2.11,<3.0) Requires-Dist: Click (>=8.1,<9.0) Requires-
-Dist: SQLAlchemy (>=1.4,<2.0) Requires-Dist: alembic (>=1.8,<2.0) Requires-
-Dist: brotli (>=1.0.9,<2.0.0) Requires-Dist: click-option-group
-(>=0.5.5,<0.6.0) Requires-Dist: cryptography (>=40.0.2,<41.0.0) Requires-Dist:
-filelock (>=3.8.2,<4.0.0) Requires-Dist: gpxpy (>=1.5,<2.0) Requires-Dist:
-markdown (>=3.4,<4.0) Requires-Dist: nh3 (>=0.2.9,<0.3.0) Requires-Dist:
-pydantic (>=1.10.2,<2.0.0) Requires-Dist: pyramid (>=2,<3) Requires-Dist:
-pyramid_debugtoolbar (>=4.9,<5.0) Requires-Dist: pyramid_jinja2 (>=2.10,<3.0)
-Requires-Dist: pyramid_retry (>=2.1,<3.0) Requires-Dist: pyramid_tm
-(>=2.5,<3.0) Requires-Dist: redis (>=4.3.4,<5.0.0) Requires-Dist: requests
-(>=2.28.1,<3.0.0) Requires-Dist: termcolor (>=2.1.1,<3.0.0) Requires-Dist:
-transaction (>=3,<4) Requires-Dist: waitress (>=2.1,<3.0) Requires-Dist:
-zope.sqlalchemy (>=2.0,<3.0) Project-URL: Documentation, https://
-docs.fietsboek.org/ Project-URL: Repository, https://gitlab.com/dunj3/fietsboek
-Description-Content-Type: text/markdown Fietsboek ========= [Pipeline_status]
-[Documentation_status] [PyPI_version] [License] [Python_versions] [Website]
-(https://fietsboek.org) â [Documentation](https://docs.fietsboek.org)
-Fietsboek is a self-hostable sharing site for GPX track recordings with social
-features. The goal is to have an application like [MyTourbook][MyTourbook] that
-runs as a web-service and allows sharing and discovering of new tracks. Note
-that Fietsboek is early in development and a hobby project, as such many
-features are still lacking. [MyTourbook]: https://mytourbook.sourceforge.io/
-mytourbook/ Installation ------------ Setup instructions are in the
-[documentation](https://docs.fietsboek.org/administration/installation.html) (
-[mirror](https://fietsboek.readthedocs.io/en/latest/administration/
-installation.html)). Development ----------- - Setup the environment:
-virtualenv .venv .venv/bin/pip install poetry .venv/bin/poetry install - Adjust
-`development.ini` to your needs. Explanations of the configuration options are
-in the [documentation](https://docs.fietsboek.org/administration/
-configuration.html). - Initialize the database: .venv/bin/alembic -
-c development.ini upgrade head - Serve the code: .venv/bin/pserve
+Dist: SQLAlchemy[mypy] (>=2.0.15,<3.0.0) Requires-Dist: alembic (>=1.8,<2.0)
+Requires-Dist: brotli (>=1.0.9,<2.0.0) Requires-Dist: click-option-group
+(>=0.5.5,<0.6.0) Requires-Dist: cryptography (>=41.0.1,<42.0.0) Requires-Dist:
+filelock (>=3.8.2,<4.0.0) Requires-Dist: fitparse (>=1.2.0,<2.0.0) Requires-
+Dist: gpxpy (>=1.5,<2.0) Requires-Dist: markdown (>=3.4,<4.0) Requires-Dist:
+nh3 (>=0.2.9,<0.3.0) Requires-Dist: pydantic (>=1.10.2,<2.0.0) Requires-Dist:
+pyramid (>=2,<3) Requires-Dist: pyramid_debugtoolbar (>=4.9,<5.0) Requires-
+Dist: pyramid_jinja2 (>=2.10,<3.0) Requires-Dist: pyramid_retry (>=2.1,<3.0)
+Requires-Dist: pyramid_tm (>=2.5,<3.0) Requires-Dist: redis (>=4.3.4,<5.0.0)
+Requires-Dist: requests (>=2.28.1,<3.0.0) Requires-Dist: termcolor
+(>=2.1.1,<3.0.0) Requires-Dist: transaction (>=3,<4) Requires-Dist: waitress
+(>=2.1,<3.0) Requires-Dist: zope.sqlalchemy (>=3.0,<4.0) Project-URL:
+Documentation, https://docs.fietsboek.org/ Project-URL: Repository, https://
+gitlab.com/dunj3/fietsboek Description-Content-Type: text/markdown Fietsboek
+========= [Pipeline_status] [Documentation_status] [PyPI_version] [License]
+[Python_versions] [Website](https://fietsboek.org) â [Documentation](https://
+docs.fietsboek.org) Fietsboek is a self-hostable sharing site for GPX track
+recordings with social features. The goal is to have an application like
+[MyTourbook][MyTourbook] that runs as a web-service and allows sharing and
+discovering of new tracks. Note that Fietsboek is early in development and a
+hobby project, as such many features are still lacking. [MyTourbook]: https://
+mytourbook.sourceforge.io/mytourbook/ Installation ------------ Setup
+instructions are in the [documentation](https://docs.fietsboek.org/
+administration/installation.html) ([mirror](https://fietsboek.readthedocs.io/
+en/latest/administration/installation.html)). Development ----------- - Setup
+the environment: virtualenv .venv .venv/bin/pip install poetry .venv/bin/poetry
+install - Adjust `development.ini` to your needs. Explanations of the
+configuration options are in the [documentation](https://docs.fietsboek.org/
+administration/configuration.html). - Initialize the database: .venv/bin/
+alembic -c development.ini upgrade head - Serve the code: .venv/bin/pserve
 development.ini --reload - Hack away! License ------- Fietsboek, the GPX web
 sharing project Copyright (C) 2022 Daniel Schadt This program is free software:
 you can redistribute it and/or modify it under the terms of the GNU Affero
 General Public License as published by the Free Software Foundation, either
 version 3 of the License, or (at your option) any later version. This program
 is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
```

