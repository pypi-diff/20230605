# Comparing `tmp/mapchete-2023.4.1.tar.gz` & `tmp/mapchete-2023.6.0.tar.gz`

## Comparing `mapchete-2023.4.1.tar` & `mapchete-2023.6.0.tar`

### file list

```diff
@@ -1,80 +1,82 @@
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/__init__.py
--rw-r--r--   0        0        0    28539 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/_core.py
--rw-r--r--   0        0        0    26312 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/_executor.py
--rw-r--r--   0        0        0    32289 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/_processing.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/_registered.py
--rw-r--r--   0        0        0    16735 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/_tasks.py
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/_timer.py
--rw-r--r--   0        0        0     5183 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/_user_process.py
--rw-r--r--   0        0        0    48250 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/config.py
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/errors.py
--rw-r--r--   0        0        0    17249 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/index.py
--rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/log.py
--rw-r--r--   0        0        0    17536 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/stac.py
--rw-r--r--   0        0        0     3859 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/testing.py
--rw-r--r--   0        0        0    15520 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/tile.py
--rw-r--r--   0        0        0     8449 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/types.py
--rw-r--r--   0        0        0     4853 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/validate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/cli/__init__.py
--rwxr-xr-x   0        0        0      308 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/cli/main.py
--rw-r--r--   0        0        0    11120 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/cli/options.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/cli/default/__init__.py
--rw-r--r--   0        0        0     3962 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/cli/default/convert.py
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/cli/default/cp.py
--rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/cli/default/create.py
--rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/cli/default/execute.py
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/cli/default/formats.py
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/cli/default/index.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/cli/default/processes.py
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/cli/default/rm.py
--rwxr-xr-x   0        0        0     4936 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/cli/default/serve.py
--rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/cli/default/stac.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/commands/__init__.py
--rw-r--r--   0        0        0    15925 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/commands/_convert.py
--rw-r--r--   0        0        0     8477 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/commands/_cp.py
--rw-r--r--   0        0        0     8548 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/commands/_execute.py
--rw-r--r--   0        0        0     4721 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/commands/_index.py
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/commands/_rm.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/commons/__init__.py
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/commons/clip.py
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/commons/contours.py
--rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/commons/hillshade.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/formats/__init__.py
--rw-r--r--   0        0        0    20950 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/formats/base.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/formats/drivers.py
--rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/formats/loaders.py
--rw-r--r--   0        0        0    12511 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/formats/tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/formats/default/__init__.py
--rw-r--r--   0        0        0     6721 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/formats/default/_fiona_base.py
--rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/formats/default/flatgeobuf.py
--rw-r--r--   0        0        0     5054 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/formats/default/geobuf.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/formats/default/geojson.py
--rw-r--r--   0        0        0    22206 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/formats/default/gtiff.py
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/formats/default/mapchete_input.py
--rw-r--r--   0        0        0     6916 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/formats/default/png.py
--rw-r--r--   0        0        0     6341 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/formats/default/png_hillshade.py
--rw-r--r--   0        0        0    11148 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/formats/default/raster_file.py
--rw-r--r--   0        0        0    15375 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/formats/default/tile_directory.py
--rw-r--r--   0        0        0     9272 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/formats/default/vector_file.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/io/__init__.py
--rw-r--r--   0        0        0    12037 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/io/_geometry_operations.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/io/_json.py
--rw-r--r--   0        0        0     8048 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/io/_misc.py
--rw-r--r--   0        0        0     9515 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/io/_path.py
--rw-r--r--   0        0        0    43386 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/io/raster.py
--rw-r--r--   0        0        0    17903 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/io/vector.py
--rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/processes/__init__.py
--rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/processes/contours.py
--rw-r--r--   0        0        0     4895 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/processes/convert.py
--rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/processes/hillshade.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/processes/examples/__init__.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/processes/examples/example_process.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/static/__init__.py
--rw-r--r--   0        0        0     7217 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/static/index.html
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/static/mapchete_template.mapchete
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 mapchete-2023.4.1/mapchete/static/process_template.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 mapchete-2023.4.1/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 mapchete-2023.4.1/LICENSE
--rw-r--r--   0        0        0     6140 2020-02-02 00:00:00.000000 mapchete-2023.4.1/README.rst
--rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 mapchete-2023.4.1/pyproject.toml
--rw-r--r--   0        0        0     8954 2020-02-02 00:00:00.000000 mapchete-2023.4.1/PKG-INFO
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/__init__.py
+-rw-r--r--   0        0        0    29098 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/_core.py
+-rw-r--r--   0        0        0    26311 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/_executor.py
+-rw-r--r--   0        0        0    32289 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/_processing.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/_registered.py
+-rw-r--r--   0        0        0    16735 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/_tasks.py
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/_timer.py
+-rw-r--r--   0        0        0     5183 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/_user_process.py
+-rw-r--r--   0        0        0    48597 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/config.py
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/errors.py
+-rw-r--r--   0        0        0    17748 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/index.py
+-rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/log.py
+-rw-r--r--   0        0        0    24446 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/path.py
+-rw-r--r--   0        0        0    17498 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/stac.py
+-rw-r--r--   0        0        0     5981 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/testing.py
+-rw-r--r--   0        0        0    15519 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/tile.py
+-rw-r--r--   0        0        0     8449 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/types.py
+-rw-r--r--   0        0        0     4854 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/validate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/cli/__init__.py
+-rwxr-xr-x   0        0        0      308 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/cli/main.py
+-rw-r--r--   0        0        0    11007 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/cli/options.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/cli/default/__init__.py
+-rw-r--r--   0        0        0     3962 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/cli/default/convert.py
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/cli/default/cp.py
+-rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/cli/default/create.py
+-rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/cli/default/execute.py
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/cli/default/formats.py
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/cli/default/index.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/cli/default/processes.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/cli/default/rm.py
+-rwxr-xr-x   0        0        0     4995 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/cli/default/serve.py
+-rw-r--r--   0        0        0     3918 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/cli/default/stac.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/commands/__init__.py
+-rw-r--r--   0        0        0    15954 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/commands/_convert.py
+-rw-r--r--   0        0        0     8538 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/commands/_cp.py
+-rw-r--r--   0        0        0     8548 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/commands/_execute.py
+-rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/commands/_index.py
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/commands/_rm.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/commons/__init__.py
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/commons/clip.py
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/commons/contours.py
+-rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/commons/hillshade.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/formats/__init__.py
+-rw-r--r--   0        0        0    20802 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/formats/base.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/formats/drivers.py
+-rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/formats/loaders.py
+-rw-r--r--   0        0        0    12520 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/formats/tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/formats/default/__init__.py
+-rw-r--r--   0        0        0     6783 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/formats/default/_fiona_base.py
+-rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/formats/default/flatgeobuf.py
+-rw-r--r--   0        0        0     5070 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/formats/default/geobuf.py
+-rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/formats/default/geojson.py
+-rw-r--r--   0        0        0    22226 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/formats/default/gtiff.py
+-rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/formats/default/mapchete_input.py
+-rw-r--r--   0        0        0     6935 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/formats/default/png.py
+-rw-r--r--   0        0        0     6379 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/formats/default/png_hillshade.py
+-rw-r--r--   0        0        0    11232 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/formats/default/raster_file.py
+-rw-r--r--   0        0        0    15914 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/formats/default/tile_directory.py
+-rw-r--r--   0        0        0     9451 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/formats/default/vector_file.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/io/__init__.py
+-rw-r--r--   0        0        0    12038 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/io/_geometry_operations.py
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/io/_json.py
+-rw-r--r--   0        0        0     7098 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/io/_misc.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/io/_path.py
+-rw-r--r--   0        0        0    44018 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/io/raster.py
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/io/settings.py
+-rw-r--r--   0        0        0    21813 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/io/vector.py
+-rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/processes/__init__.py
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/processes/contours.py
+-rw-r--r--   0        0        0     4896 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/processes/convert.py
+-rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/processes/hillshade.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/processes/examples/__init__.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/processes/examples/example_process.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/static/__init__.py
+-rw-r--r--   0        0        0     8416 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/static/index.html
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/static/mapchete_template.mapchete
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 mapchete-2023.6.0/mapchete/static/process_template.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 mapchete-2023.6.0/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 mapchete-2023.6.0/LICENSE
+-rw-r--r--   0        0        0     6140 2020-02-02 00:00:00.000000 mapchete-2023.6.0/README.rst
+-rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 mapchete-2023.6.0/pyproject.toml
+-rw-r--r--   0        0        0     9061 2020-02-02 00:00:00.000000 mapchete-2023.6.0/PKG-INFO
```

### Comparing `mapchete-2023.4.1/mapchete/__init__.py` & `mapchete-2023.6.0/mapchete/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 import logging
 
-from mapchete._core import open, Mapchete
+from mapchete._core import Mapchete, open
 from mapchete._executor import Executor, FakeFuture, SkippedFuture
 from mapchete._processing import Job, ProcessInfo
+from mapchete._timer import Timer
 from mapchete._user_process import MapcheteProcess
 from mapchete.tile import count_tiles
-from mapchete._timer import Timer
-
 
 __all__ = [
     "open",
     "count_tiles",
     "Mapchete",
     "MapcheteProcess",
     "ProcessInfo",
     "Timer",
     "Executor",
     "FakeFuture",
     "SkippedFuture",
     "Job",
 ]
-__version__ = "2023.4.1"
+__version__ = "2023.6.0"
 
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.NullHandler())
```

### Comparing `mapchete-2023.4.1/mapchete/_core.py` & `mapchete-2023.6.0/mapchete/_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 """Main module managing processes."""
 
-from cachetools import LRUCache
 import json
 import logging
 import multiprocessing
 import os
 import threading
 import warnings
 
-from mapchete.config import MapcheteConfig, MULTIPROCESSING_DEFAULT_START_METHOD
-from mapchete.errors import MapcheteNodataTile, ReprojectionFailed
-from mapchete.formats import read_output_metadata
-from mapchete.io import fs_from_path, tiles_exist, read_json, makedirs
+from cachetools import LRUCache
+
 from mapchete._processing import (
-    compute,
-    _run_on_single_tile,
-    _run_area,
-    _preprocess,
     ProcessInfo,
+    _preprocess,
+    _run_area,
+    _run_on_single_tile,
+    compute,
     task_batches,
 )
-from mapchete.stac import update_tile_directory_stac_item
 from mapchete._tasks import TileTask
-from mapchete.tile import count_tiles
 from mapchete._timer import Timer
+from mapchete.config import MULTIPROCESSING_DEFAULT_START_METHOD, MapcheteConfig
+from mapchete.errors import MapcheteNodataTile, ReprojectionFailed
+from mapchete.formats import read_output_metadata
+from mapchete.io import MPath, fs_from_path, tiles_exist
+from mapchete.stac import update_tile_directory_stac_item
+from mapchete.tile import count_tiles
 from mapchete.validate import validate_tile, validate_zooms
 
 logger = logging.getLogger(__name__)
 
 
 def open(some_input, with_cache=False, fs=None, fs_kwargs=None, **kwargs):
     """
@@ -58,17 +59,21 @@
         Special configuration parameters if FileSystem object has to be created.
 
     Returns
     -------
     Mapchete
         a Mapchete process object
     """
-    if isinstance(some_input, str) and not some_input.endswith(".mapchete"):
+    # convert to MPath object if possible
+    if isinstance(some_input, str):
+        some_input = MPath(some_input)
+    # for TileDirectory inputs
+    if isinstance(some_input, MPath) and some_input.suffix == "":
         logger.debug("assuming TileDirectory")
-        metadata_json = os.path.join(some_input, "metadata.json")
+        metadata_json = MPath(some_input).joinpath("metadata.json")
         fs_kwargs = fs_kwargs or {}
         fs = fs or fs_from_path(metadata_json, **fs_kwargs)
         logger.debug("read metadata.json")
         metadata = read_output_metadata(metadata_json, fs=fs)
         config = dict(
             process=None,
             input=None,
@@ -85,16 +90,27 @@
                 **kwargs,
             ),
             config_dir=os.getcwd(),
             zoom_levels=kwargs.get("zoom"),
         )
         kwargs.update(mode="readonly")
         return Mapchete(MapcheteConfig(config, **kwargs))
-
-    return Mapchete(MapcheteConfig(some_input, **kwargs), with_cache=with_cache)
+    # for dicts, .mapchete file paths or MpacheteConfig objects
+    elif (
+        isinstance(some_input, dict)
+        or isinstance(some_input, MPath)
+        and some_input.suffix == ".mapchete"
+        or isinstance(some_input, MapcheteConfig)
+    ):
+        return Mapchete(MapcheteConfig(some_input, **kwargs), with_cache=with_cache)
+    else:  # pragma: no cover
+        raise TypeError(
+            "can only open input in form of a mapchete file path, a TileDirectory path, "
+            f"a dictionary or a MapcheteConfig object, not {type(some_input)}"
+        )
 
 
 class Mapchete(object):
     """
     Main entry point to every processing job.
 
     From here, the process tiles can be determined and executed.
@@ -669,36 +685,34 @@
             return
 
         if not self.config.output.use_stac or self.config.mode in [
             "readonly",
             "memory",
         ]:
             return
-
         # read existing STAC file
         try:
-            with self.config.output.fs.open(self.config.output.stac_path, "r") as src:
+            with self.config.output.stac_path.open("r") as src:
                 item = pystac.read_dict(json.loads(src.read()))
         except FileNotFoundError:
             item = None
-
         try:
             item = update_tile_directory_stac_item(
                 item=item,
-                item_path=self.config.output.stac_path,
+                item_path=str(self.config.output.stac_path),
                 item_id=self.config.output.stac_item_id,
                 zoom_levels=self.config.init_zoom_levels,
                 bounds=self.config.effective_bounds,
                 item_metadata=self.config.output.stac_item_metadata,
                 tile_pyramid=self.config.output_pyramid,
                 bands_type=self.config.output.stac_asset_type,
             )
             logger.debug("write STAC item JSON to %s", self.config.output.stac_path)
-            makedirs(os.path.dirname(self.config.output.stac_path))
-            with self.config.output.fs.open(self.config.output.stac_path, "w") as dst:
+            self.config.output.stac_path.makedirs()
+            with self.config.output.stac_path.open("w") as dst:
                 dst.write(json.dumps(item.to_dict(), indent=indent))
         except ReprojectionFailed:
             logger.warning(
                 "cannot create STAC item because footprint cannot be reprojected into EPSG:4326"
             )
         except Exception as exc:  # pragma: no cover
             logger.warning("cannot create or update STAC item: %s", str(exc))
```

### Comparing `mapchete-2023.4.1/mapchete/_executor.py` & `mapchete-2023.6.0/mapchete/_executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """Abstraction classes for multiprocessing and distributed processing."""
 
 import concurrent.futures
-from concurrent.futures._base import CancelledError
-from functools import partial
 import logging
 import multiprocessing
 import os
 import sys
 import warnings
+from concurrent.futures._base import CancelledError
+from functools import partial
 
 from cached_property import cached_property
 
+from mapchete._timer import Timer
 from mapchete.errors import JobCancelledError, MapcheteTaskFailed
 from mapchete.log import set_log_level
-from mapchete._timer import Timer
 
 MULTIPROCESSING_DEFAULT_START_METHOD = "spawn"
 FUTURE_TIMEOUT = float(os.environ.get("MP_FUTURE_TIMEOUT", 10))
 
 logger = logging.getLogger(__name__)
 
 
@@ -224,15 +224,15 @@
         self,
         *args,
         dask_scheduler=None,
         dask_client=None,
         max_workers=None,
         **kwargs,
     ):
-        from dask.distributed import as_completed, Client, LocalCluster
+        from dask.distributed import Client, LocalCluster, as_completed
 
         self._executor_client = dask_client
         self._local_cluster = None
         if self._executor_client:  # pragma: no cover
             logger.debug("using existing dask client: %s", dask_client)
         else:
             local_cluster_kwargs = dict(
@@ -311,15 +311,14 @@
         chunksize = chunksize or 100
 
         try:
             fargs = fargs or ()
             fkwargs = fkwargs or {}
             chunk = []
             for item in iterable:
-
                 # abort if execution is cancelled
                 if self.cancelled:  # pragma: no cover
                     logger.debug("executor cancelled")
                     return
 
                 # skip task submission if option is activated
                 if item_skip_bool:
```

### Comparing `mapchete-2023.4.1/mapchete/_processing.py` & `mapchete-2023.6.0/mapchete/_processing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 """Internal processing classes and functions."""
 
-from collections import namedtuple
-from contextlib import ExitStack
 import logging
 import multiprocessing
 import os
-from shapely.geometry import mapping
+from collections import namedtuple
+from contextlib import ExitStack
 from typing import Generator
 
-from mapchete.config import get_process_func
+from shapely.geometry import mapping
+
 from mapchete._executor import (
     DaskExecutor,
     Executor,
-    SkippedFuture,
     FinishedFuture,
+    SkippedFuture,
     future_raise_exception,
 )
-from mapchete.errors import MapcheteNodataTile, MapcheteTaskFailed
-from mapchete._tasks import to_dask_collection, TileTaskBatch, TileTask, TaskBatch
+from mapchete._tasks import TaskBatch, TileTask, TileTaskBatch, to_dask_collection
 from mapchete._timer import Timer
+from mapchete.config import get_process_func
+from mapchete.errors import MapcheteNodataTile, MapcheteTaskFailed
 from mapchete.types import Bounds, ZoomLevels
 
 FUTURE_TIMEOUT = float(os.environ.get("MP_FUTURE_TIMEOUT", 10))
 
 
 logger = logging.getLogger(__name__)
 
@@ -700,15 +701,14 @@
     write_in_parent_process=None,
 ):
     # here we store the parents of processed tiles so we can update overviews
     # also in "continue" mode in case there were updates at the baselevel
     overview_parents = set()
 
     for i, zoom in enumerate(zoom_levels.descending()):
-
         logger.debug("sending tasks to executor %s...", executor)
         # get generator list of tiles, whether they are to be skipped and skip_info
         # from _filter_skipable and pass on to executor
         for future in executor.as_completed(
             func=func,
             iterable=(
                 (
```

### Comparing `mapchete-2023.4.1/mapchete/_registered.py` & `mapchete-2023.6.0/mapchete/_registered.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.4.1/mapchete/_tasks.py` & `mapchete-2023.6.0/mapchete/_tasks.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
+import logging
 from collections import namedtuple
 from itertools import chain
-import logging
-from shapely.geometry import box, mapping
 from traceback import format_exc
 from uuid import uuid4
 
+from shapely.geometry import box, mapping
+
 from mapchete._timer import Timer
+from mapchete._user_process import MapcheteProcess
 from mapchete.config import get_process_func
 from mapchete.errors import (
     MapcheteNodataTile,
-    NoTaskGeometry,
     MapcheteProcessException,
     MapcheteProcessOutputError,
+    NoTaskGeometry,
 )
 from mapchete.io import raster
 from mapchete.io._geometry_operations import to_shape
 from mapchete.io.vector import IndexedFeatures
 from mapchete.validate import validate_bounds
-from mapchete._user_process import MapcheteProcess
-
 
 logger = logging.getLogger(__name__)
 
 
 TaskResult = namedtuple(
     "TaskResult",
     "task_id tile processed process_msg result",
```

### Comparing `mapchete-2023.4.1/mapchete/_timer.py` & `mapchete-2023.6.0/mapchete/_timer.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.4.1/mapchete/_user_process.py` & `mapchete-2023.6.0/mapchete/_user_process.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.4.1/mapchete/config.py` & `mapchete-2023.6.0/mapchete/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,67 +6,66 @@
 Upon creation, all parameters are validated and the InputData objects are
 created which are then exposed to the user process.
 
 An invalid process configuration or an invalid process file cause an Exception
 when initializing the configuration.
 """
 
-from cached_property import cached_property
-from collections import OrderedDict
-from copy import deepcopy
-import fiona
-import fsspec
 import hashlib
 import importlib
 import inspect
 import logging
 import operator
 import os
-import oyaml as yaml
 import py_compile
+import sys
+import warnings
+from collections import OrderedDict
+from copy import deepcopy
+from tempfile import NamedTemporaryFile
+
+import fsspec
+import oyaml as yaml
+from cached_property import cached_property
 from shapely import wkt
-from shapely.geometry import box, Point, shape
+from shapely.geometry import Point, box, shape
 from shapely.geometry.base import BaseGeometry
 from shapely.ops import unary_union
-import sys
-from tempfile import NamedTemporaryFile
-import warnings
 
-from mapchete.validate import (
-    validate_bounds,
-    validate_zooms,
-    validate_values,
-    validate_bufferedtilepyramid,
-)
+from mapchete._executor import MULTIPROCESSING_DEFAULT_START_METHOD
 from mapchete.errors import (
+    GeometryTypeError,
     MapcheteConfigError,
-    MapcheteProcessSyntaxError,
-    MapcheteProcessImportError,
     MapcheteDriverError,
-    GeometryTypeError,
+    MapcheteProcessImportError,
+    MapcheteProcessSyntaxError,
 )
-from mapchete._executor import MULTIPROCESSING_DEFAULT_START_METHOD
 from mapchete.formats import (
-    load_output_reader,
-    load_output_writer,
     available_output_formats,
     load_input_reader,
+    load_output_reader,
+    load_output_writer,
 )
-from mapchete.io import absolute_path
+from mapchete.io import MPath, absolute_path, fiona_open
 from mapchete.io.vector import clean_geometry_type, reproject_geometry
 from mapchete.log import add_module_logger
 from mapchete.tile import BufferedTilePyramid
 from mapchete.types import Bounds
-
+from mapchete.validate import (
+    validate_bounds,
+    validate_bufferedtilepyramid,
+    validate_values,
+    validate_zooms,
+)
 
 logger = logging.getLogger(__name__)
 
 # parameters which have to be provided in the configuration and their types
 _MANDATORY_PARAMETERS = [
-    ("process", (str, list, type(None))),  # path to .py file or module path
+    ("process", (str, list, type(None), MPath)),  # path to .py file or module path
     ("pyramid", dict),  # process pyramid definition
     ("input", (dict, type(None))),  # files & other types
     ("output", dict),  # process output parameters
     ("zoom_levels", (int, dict, list)),  # process zoom levels
 ]
 
 # parameters with special functions which cannot be used for user parameters
@@ -424,15 +423,17 @@
             pixelbuffer=self.output_pyramid.pixelbuffer,
             metatiling=self.output_pyramid.metatiling,
             delimiters=self._delimiters,
             mode=self.mode,
         )
         if "path" in output_params:
             output_params.update(
-                path=absolute_path(path=output_params["path"], base_dir=self.config_dir)
+                path=MPath.from_dict(output_params).absolute_path(
+                    base_dir=self.config_dir
+                )
             )
 
         if "format" not in output_params:
             raise MapcheteConfigError("output format not specified")
 
         if output_params["format"] not in available_output_formats():
             raise MapcheteConfigError(
@@ -779,43 +780,31 @@
 
     @cached_property
     def inputs(self):
         """Deprecated."""
         warnings.warn(DeprecationWarning("self.inputs renamed to self.input."))
         return self.input
 
-    @cached_property
-    def process_file(self):
-        """Deprecated."""
-        warnings.warn(DeprecationWarning("'self.process_file' is deprecated"))
-        return os.path.join(self._raw["config_dir"], self._raw["process"])
-
     def at_zoom(self, zoom):
         """Deprecated."""
         warnings.warn(
             DeprecationWarning("Method renamed to self.params_at_zoom(zoom).")
         )
         return self.params_at_zoom(zoom)
 
-    def process_area(self, zoom=None):
-        """Deprecated."""
-        warnings.warn(DeprecationWarning("Method renamed to self.area_at_zoom(zoom)."))
-        return self.area_at_zoom(zoom)
-
-    def process_bounds(self, zoom=None):
-        """Deprecated."""
-        warnings.warn(
-            DeprecationWarning("Method renamed to self.bounds_at_zoom(zoom).")
-        )
-        return self.bounds_at_zoom(zoom)
-
 
 def get_hash(x, length=16):
     """Return hash of x."""
-    return hashlib.sha224(yaml.dump(dict(key=x)).encode()).hexdigest()[:length]
+    if isinstance(x, MPath):
+        x = str(x)
+    try:
+        return hashlib.sha224(yaml.dump(dict(key=x)).encode()).hexdigest()[:length]
+    except TypeError:  # pragma: no cover
+        # in case yaml.dump fails, we just try to get a string representation of object
+        return hashlib.sha224(str(x).encode()).hexdigest()[:length]
 
 
 def get_zoom_levels(process_zoom_levels=None, init_zoom_levels=None):
     """Validate and return zoom levels."""
     process_zoom_levels = validate_zooms(process_zoom_levels)
     if init_zoom_levels is None:
         return process_zoom_levels
@@ -1025,40 +1014,43 @@
     pyramid=None,
     delimiters=None,
     readonly=False,
 ):
     initalized_inputs = OrderedDict()
     for k, v in raw_inputs.items():
         # for files and tile directories
-        if isinstance(v, str):
+        if isinstance(v, (str, MPath)):
             logger.debug("load input reader for simple input %s", v)
             try:
                 reader = load_input_reader(
                     dict(
                         path=absolute_path(path=v, base_dir=config_dir),
                         pyramid=pyramid,
                         pixelbuffer=pyramid.pixelbuffer,
                         delimiters=delimiters,
                     ),
                     readonly=readonly,
                     input_key=k,
                 )
             except Exception as e:
                 logger.exception(e)
-                raise MapcheteDriverError("error when loading input %s: %s" % (v, e))
+                raise MapcheteDriverError(
+                    "error when loading input %s: %s" % (v, e)
+                ) from e
             logger.debug("input reader for simple input %s is %s", v, reader)
 
         # for abstract inputs
         elif isinstance(v, dict):
             logger.debug("load input reader for abstract input %s", v)
             try:
                 abstract = deepcopy(v)
+                # make path absolute and add filesystem options
                 if "path" in abstract:
                     abstract.update(
-                        path=absolute_path(path=abstract["path"], base_dir=config_dir)
+                        path=MPath.from_dict(abstract).absolute_path(config_dir)
                     )
                 reader = load_input_reader(
                     dict(
                         abstract=abstract,
                         pyramid=pyramid,
                         pixelbuffer=pyramid.pixelbuffer,
                         delimiters=delimiters,
@@ -1082,45 +1074,48 @@
         initalized_inputs.keys(),
     )
     return initalized_inputs
 
 
 def _load_process_module(process=None, config_dir=None, run_compile=False):
     tmpfile = None
+    process = MPath(process) if isinstance(process, str) else process
     try:
         if isinstance(process, list):
             tmpfile = NamedTemporaryFile(suffix=".py")
             logger.debug(f"writing process code to temporary file {tmpfile.name}")
             with open(tmpfile.name, "w") as dst:
                 for line in process:
                     dst.write(line + "\n")
-            process = tmpfile.name
-        if process.endswith(".py"):
+            process = MPath(tmpfile.name)
+        if process.suffix == ".py":
             module_path = absolute_path(path=process, base_dir=config_dir)
-            if not os.path.isfile(module_path):
+            if not module_path.exists():
                 raise MapcheteConfigError(f"{module_path} is not available")
             try:
                 if run_compile:
                     py_compile.compile(module_path, doraise=True)
-                module_name = os.path.splitext(os.path.basename(module_path))[0]
+                module_name = module_path.stem
                 # load module
-                spec = importlib.util.spec_from_file_location(module_name, module_path)
+                spec = importlib.util.spec_from_file_location(
+                    module_name, str(module_path)
+                )
                 module = importlib.util.module_from_spec(spec)
                 spec.loader.exec_module(module)
                 # required to make imported module available using multiprocessing
                 sys.modules[module_name] = module
                 # configure process file logger
                 add_module_logger(module.__name__)
             except py_compile.PyCompileError as e:
                 raise MapcheteProcessSyntaxError(e)
             except ImportError as e:
                 raise MapcheteProcessImportError(e)
         else:
             try:
-                module = importlib.import_module(process)
+                module = importlib.import_module(str(process))
             except ImportError as e:
                 raise MapcheteProcessImportError(e)
         logger.debug(f"return process func: {module}")
     finally:
         if tmpfile:
             logger.debug(f"removing {tmpfile.name}")
             tmpfile.close()
@@ -1137,30 +1132,45 @@
             yield (k, v.open(tile))
 
 
 def _config_to_dict(input_config):
     if isinstance(input_config, dict):
         if "config_dir" not in input_config:
             raise MapcheteConfigError("config_dir parameter missing")
-        return OrderedDict(input_config, mapchete_file=None)
+        return OrderedDict(_include_env(input_config), mapchete_file=None)
     # from Mapchete file
-    elif os.path.splitext(input_config)[1] == ".mapchete":
-        with fsspec.open(input_config, "r") as config_file:
-            return OrderedDict(
-                yaml.safe_load(config_file.read()),
-                config_dir=os.path.dirname(os.path.realpath(input_config)),
-                mapchete_file=input_config,
-            )
+    elif input_config.suffix == ".mapchete":
+        config_dict = _include_env(yaml.safe_load(input_config.read_text()))
+        return OrderedDict(
+            config_dict,
+            config_dir=config_dict.get(
+                "config_dir", input_config.absolute_path().dirname or os.getcwd()
+            ),
+            mapchete_file=input_config,
+        )
     # throw error if unknown object
     else:  # pragma: no cover
         raise MapcheteConfigError(
             "Configuration has to be a dictionary or a .mapchete file."
         )
 
 
+def _include_env(d):
+    out = OrderedDict()
+    for k, v in d.items():
+        if isinstance(v, dict):
+            out[k] = _include_env(v)
+        elif isinstance(v, str) and v.startswith("${") and v.endswith("}"):
+            envvar = v.lstrip("${").rstrip("}")
+            out[k] = os.environ.get(envvar)
+        else:
+            out[k] = v
+    return out
+
+
 def _raw_at_zoom(config, zooms):
     """Return parameter dictionary per zoom level."""
     params_per_zoom = OrderedDict()
     for zoom in zooms:
         params = OrderedDict()
         for name, element in config.items():
             if name not in _RESERVED_PARAMETERS:
@@ -1359,21 +1369,23 @@
     - a WKT string
     - a GeoJSON mapping
     - a shapely geometry
     - a path to a Fiona-readable file
     """
     crs = None
     # WKT or path:
-    if isinstance(i, str):
-        if i.upper().startswith(("POLYGON ", "MULTIPOLYGON ")):
+    if isinstance(i, (str, MPath)):
+        if str(i).upper().startswith(("POLYGON ", "MULTIPOLYGON ")):
             geom = wkt.loads(i)
         else:
-            with fiona.open(absolute_path(path=i, base_dir=base_dir)) as src:
-                geom = unary_union([shape(f["geometry"]) for f in src])
-                crs = src.crs
+            path = MPath(i)
+            with path.fio_env():
+                with fiona_open(str(path.absolute_path(base_dir))) as src:
+                    geom = unary_union([shape(f["geometry"]) for f in src])
+                    crs = src.crs
     # GeoJSON mapping
     elif isinstance(i, dict):
         geom = shape(i)
     # shapely geometry
     elif isinstance(i, BaseGeometry):
         geom = i
     else:
```

### Comparing `mapchete-2023.4.1/mapchete/errors.py` & `mapchete-2023.6.0/mapchete/errors.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.4.1/mapchete/index.py` & `mapchete-2023.6.0/mapchete/index.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,33 +15,35 @@
   all GeoTIFF files from a certain zoom level.
 
 All index types are generated once per zoom level. For example GeoPackage will
 generate GPKG files 3.gpkg, 4.gpkg and 5.gpkg for zoom levels 3, 4 and 5.
 
 """
 
+import logging
+import operator
+import xml.etree.ElementTree as ET
 from contextlib import ExitStack
 from copy import deepcopy
+from xml.dom import minidom
+
 import fiona
-import logging
-import operator
-import os
 from rasterio.dtypes import _gdal_typename
 from shapely.geometry import mapping
-import xml.etree.ElementTree as ET
-from xml.dom import minidom
 
 from mapchete.config import get_zoom_levels
 from mapchete.io import (
+    MPath,
+    fiona_open,
     fs_from_path,
     path_exists,
-    path_is_remote,
     raster,
     relative_path,
     tiles_exist,
+    vector,
 )
 
 logger = logging.getLogger(__name__)
 
 spatial_schema = {
     "geometry": "Polygon",
     "properties": {"tile_id": "str:254", "zoom": "int", "row": "int", "col": "int"},
@@ -160,15 +162,14 @@
                 output_tiles_batches = mp.config.output_pyramid.tiles_from_geom(
                     mp.config.area_at_zoom(zoom), zoom, batch_by="row", exact=True
                 )
 
             for output_tile, exists in tiles_exist(
                 mp.config, output_tiles_batches=output_tiles_batches
             ):
-
                 tile_path = _tile_path(
                     orig_path=mp.config.output.get_path(output_tile),
                     basepath=basepath,
                     for_gdal=for_gdal,
                 )
                 # get indexes where tile entry does not exist
                 indexes = [
@@ -184,76 +185,93 @@
                         index.write(output_tile, tile_path)
 
                 # yield tile for progress information
                 yield output_tile
 
 
 def _index_file_path(out_dir, zoom, ext):
-    return os.path.join(out_dir, str(zoom) + "." + ext)
+    return MPath(out_dir) / f"{str(zoom)}.{ext}"
 
 
 def _tile_path(orig_path=None, basepath=None, for_gdal=True):
     path = (
-        os.path.join(basepath, "/".join(orig_path.split("/")[-3:]))
+        MPath(basepath).joinpath(*orig_path.elements[-3:])
         if basepath
-        else orig_path
+        else MPath(orig_path)
     )
-    if for_gdal and path.startswith(("http://", "https://")):
-        return "/vsicurl/" + path
-    elif for_gdal and path.startswith("s3://"):
-        return path.replace("s3://", "/vsis3/")
+    if for_gdal:
+        return path.as_gdal_str()
     else:
-        return path
+        return str(path)
 
 
 class VectorFileWriter:
     """Writes GeoJSON or GeoPackage files."""
 
     def __init__(self, out_path=None, crs=None, fieldname=None, driver=None):
-        self._append = "a" in fiona.supported_drivers[driver]
+        self.path = MPath(out_path)
+        self._append = (
+            "a" in fiona.supported_drivers[driver] and not self.path.is_remote()
+        )
         logger.debug("initialize %s writer with append %s", driver, self._append)
-        self.path = out_path
         self.driver = driver
         self.fieldname = fieldname
         self.new_entries = 0
-        schema = deepcopy(spatial_schema)
-        schema["properties"][fieldname] = "str:254"
+        self.schema = deepcopy(spatial_schema)
+        self.schema["properties"][fieldname] = "str:254"
+        self.crs = crs
 
+    def __repr__(self):
+        return "VectorFileWriter(%s)" % self.path
+
+    def __enter__(self):
+        self.es = ExitStack().__enter__()
         if self._append:
-            if os.path.isfile(self.path):
+            if self.path.exists():
                 logger.debug("read existing entries")
-                with fiona.open(self.path, "r") as src:
+                with fiona_open(self.path, "r") as src:
                     self._existing = {f["properties"]["tile_id"]: f for f in src}
-                self.sink = fiona.open(self.path, "a")
+                self.sink = self.es.enter_context(vector.fiona_write(self.path, "a"))
             else:
-                self.sink = fiona.open(
-                    self.path, "w", driver=self.driver, crs=crs.to_dict(), schema=schema
+                self.sink = self.es.enter_context(
+                    vector.fiona_write(
+                        self.path,
+                        "w",
+                        driver=self.driver,
+                        crs=self.crs.to_dict(),
+                        schema=self.schema,
+                    )
                 )
                 self._existing = {}
         else:  # pragma: no cover
-            if os.path.isfile(self.path):
+            if self.path.exists():
                 logger.debug("read existing entries")
-                with fiona.open(self.path, "r") as src:
+                with fiona_open(self.path, "r") as src:
                     self._existing = {f["properties"]["tile_id"]: f for f in src}
-                fiona.remove(self.path, driver=driver)
+                if not self.path.is_remote():
+                    fiona.remove(str(self.path), driver=self.driver)
             else:
                 self._existing = {}
-            self.sink = fiona.open(
-                self.path, "w", driver=self.driver, crs=crs, schema=schema
+            self.sink = self.es.enter_context(
+                vector.fiona_write(
+                    self.path,
+                    "w",
+                    driver=self.driver,
+                    crs=self.crs,
+                    schema=self.schema,
+                )
             )
             self.sink.writerecords(self._existing.values())
-
-    def __repr__(self):
-        return "VectorFileWriter(%s)" % self.path
-
-    def __enter__(self):
         return self
 
-    def __exit__(self, *args):
-        self.close()
+    def __exit__(self, exc_type, exc_value, exc_traceback):
+        try:
+            self.es.__exit__(exc_type, exc_value, exc_traceback)
+        finally:
+            self.close()
 
     def write(self, tile, path):
         if not self.entry_exists(tile=tile):
             logger.debug("write %s to %s", path, self)
             self.sink.write(
                 {
                     "geometry": mapping(tile.bbox),
@@ -333,15 +351,17 @@
         self.path = out_path
         self._tp = out_pyramid
         self._output = output
         self.fs = fs_from_path(out_path)
         logger.debug("initialize VRT writer for %s", self.path)
         if path_exists(self.path):
             with self.fs.open(self.path) as src:
-                self._existing = {k: v for k, v in self._xml_to_entries(src.read())}
+                self._existing = {
+                    k: MPath(v) for k, v in self._xml_to_entries(src.read())
+                }
         else:
             self._existing = {}
         logger.debug("%s existing entries", len(self._existing))
         self.new_entries = 0
         self._new = {}
 
     def __repr__(self):
@@ -350,18 +370,18 @@
     def __enter__(self):
         return self
 
     def __exit__(self, *args):
         self.close()
 
     def _path_to_tile(self, path):
-        return self._tp.tile(*map(int, os.path.splitext(path)[0].split("/")[-3:]))
+        return self._tp.tile(*map(int, MPath(path).without_suffix().elements[-3:]))
 
     def _add_entry(self, tile=None, path=None):
-        self._new[tile] = path
+        self._new[tile] = MPath(path)
 
     def _xml_to_entries(self, xml_string):
         for entry in next(
             ET.ElementTree(ET.fromstring(xml_string)).getroot().iter("VRTRasterBand")
         ).iter("ComplexSource"):
             path = next(entry.iter("SourceFilename")).text
             yield (self._path_to_tile(path), path)
@@ -369,15 +389,15 @@
     def write(self, tile, path):
         if not self.entry_exists(tile=tile, path=path):
             logger.debug("write %s to %s", path, self)
             self._add_entry(tile=tile, path=path)
             self.new_entries += 1
 
     def entry_exists(self, tile=None, path=None):
-        path = relative_path(path=path, base_dir=os.path.split(self.path)[0])
+        path = relative_path(path=path, base_dir=self.path.dirname)
         exists = path in self._existing
         logger.debug("tile %s with path %s exists: %s", tile, path, exists)
         return exists
 
     def close(self):
         from lxml.builder import ElementMaker
 
@@ -404,19 +424,17 @@
                 E.VRTRasterBand(
                     E.NoDataValue(str(vrt_nodata)),
                     E.ColorInterp("Gray"),
                     *[
                         E.ComplexSource(
                             E.SourceFilename(
                                 _tile_path(orig_path=path, for_gdal=True)
-                                if path_is_remote(path)
-                                else relative_path(
-                                    path=path, base_dir=os.path.split(self.path)[0]
-                                ),
-                                relativeToVRT="0" if path_is_remote(path) else "1",
+                                if path.is_remote()
+                                else str(path.relative_path(start=self.path.dirname)),
+                                relativeToVRT="0" if path.is_remote() else "1",
                             ),
                             E.SourceBand(str(b_idx)),
                             E.SourceProperties(
                                 RasterXSize=str(tile.shape.width),
                                 RasterYSize=str(tile.shape.height),
                                 DataType=vrt_dtype,
                                 BlockXSize=str(
```

### Comparing `mapchete-2023.4.1/mapchete/log.py` & `mapchete-2023.6.0/mapchete/log.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 Custom loggers for external code such as user processes & drivers.
 
 This is necessary because if using the logging module directly, the namespace
 is not assigned properly and log levels & log handlers cannot be assigned
 correctly.
 """
-from itertools import chain
 import logging
 import sys
 import warnings
+from itertools import chain
 
 from mapchete._registered import drivers, processes
 
 all_mapchete_packages = set(v.value.split(".")[0] for v in chain(drivers, processes))
 
 key_value_replace_patterns = {
     "AWS_ACCESS_KEY_ID": "***",
```

### Comparing `mapchete-2023.4.1/mapchete/stac.py` & `mapchete-2023.6.0/mapchete/stac.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-from collections import OrderedDict
 import datetime
 import logging
+from collections import OrderedDict
+
 import numpy as np
 import numpy.ma as ma
-import os
 from pyproj import CRS
 from shapely.geometry import box, mapping
 
 from mapchete.errors import ReprojectionFailed
-from mapchete.io import makedirs
+from mapchete.io import MPath
 from mapchete.io.raster import write_raster_window
 from mapchete.io.vector import reproject_geometry
 from mapchete.tile import BufferedTilePyramid
 from mapchete.types import Bounds
 
-
 logger = logging.getLogger(__name__)
 
 OUT_PIXEL_SIZE = 0.28e-3
 UNIT_TO_METER = {"mercator": 1, "geodetic": 111319.4907932732}
 KNOWN_MATRIX_PROPERTIES = {
     "geodetic": {
         "name": "WorldCRS84Quad",
@@ -98,32 +97,33 @@
     if item_id is None:
         raise ValueError("item_id must be set")
     if zoom_levels is None:
         raise ValueError("zoom_levels must be set")
     if tile_pyramid is None:
         raise ValueError("tile_pyramid must be set")
 
+    asset_basepath = MPath(asset_basepath) if asset_basepath else None
+    item_path = MPath(item_path) if item_path else None
+
     item_metadata = _cleanup_datetime(item_metadata or {})
     timestamp = (
         item_metadata.get("properties", {}).get("start_datetime")
         or item_metadata.get("properties", {}).get("end_datetime")
         or str(datetime.datetime.utcnow())
     )
     tp_grid = tile_pyramid.grid.type
     bands_schema = "{TileMatrix}/{TileRow}/{TileCol}.tif"
     # thumbnail_href = thumbnail_href or "0/0/0.tif"
     # thumbnail_type = thumbnail_type or "image/tiff; application=geotiff"
     if asset_basepath:
-        bands_schema = os.path.join(asset_basepath, bands_schema)
-        # thumbnail_href = os.path.join(asset_basepath, thumbnail_href)
+        bands_schema = asset_basepath / bands_schema
     elif not relative_paths:
         if item_path is None:
             raise ValueError("either alternative_basepath or item_path must be set")
-        bands_schema = os.path.join(os.path.dirname(item_path), bands_schema)
-        # thumbnail_href = os.path.join(os.path.dirname(item_path), thumbnail_href)
+        bands_schema = item_path.parent / bands_schema
 
     # use bounds provided or fall back to tile pyramid bounds
     bounds = bounds or tile_pyramid.bounds
     bounds_crs = bounds_crs or tile_pyramid.crs
 
     # bounds in tilepyramid CRS
     tp_bbox = reproject_geometry(
@@ -240,29 +240,29 @@
         "properties": {
             **item_metadata.get("properties", {}),
             "datetime": timestamp,
             "collection": item_id,
             "tiles:tile_matrix_links": {tile_matrix_set_identifier: tile_matrix_links},
             "tiles:tile_matrix_sets": {tile_matrix_set_identifier: tile_matrix_set},
         },
-        "asset_templates": {"bands": {"href": bands_schema, "type": bands_type}},
+        "asset_templates": {"bands": {"href": str(bands_schema), "type": bands_type}},
         "assets": {
             # "thumbnail": {
             #     "href": thumbnail_href,
             #     "title": "Overview of the whole tiled dataset.",
             #     "type": thumbnail_type,
             # }
         },
     }
     if "eo:bands" in item_metadata:
         out["asset_templates"]["bands"]["eo:bands"] = item_metadata["eo:bands"]
         # out["assets"]["thumbnail"]["eo:bands"] = item_metadata["eo:bands"]
     out["links"] = item_metadata.get("links", [])
     if item_path:
-        out["links"].extend([{"rel": "self", "href": item_path}])
+        out["links"].extend([{"rel": "self", "href": str(item_path)}])
 
     return pystac.read_dict(out)
 
 
 def _scale(grid, pixel_x_size, default_unit_to_meter=1):
     return (
         UNIT_TO_METER.get(grid, default_unit_to_meter) * pixel_x_size / OUT_PIXEL_SIZE
@@ -325,14 +325,15 @@
     crs_unit_to_meter : int or float
         Factor to convert CRS units to meter if tile pyramid grid is not "geodetic" or "mercator". (default: 1)
 
     Returns
     -------
     pystac.Item
     """
+    item_path = MPath(item_path) if item_path else None
     # from existing item
     if item is not None:
         zoom_levels = zoom_levels or []
         zoom_levels = sorted(list(set(zoom_levels + zoom_levels_from_item(item))))
         existing_tile_pyramid = tile_pyramid_from_item(item)
         if tile_pyramid and tile_pyramid != existing_tile_pyramid:
             raise TypeError(
@@ -356,27 +357,26 @@
         item_id = item_id or item.id
 
     return tile_directory_stac_item(
         item_id=item_id,
         tile_pyramid=tile_pyramid,
         zoom_levels=zoom_levels,
         item_path=item_path,
-        asset_basepath=os.path.dirname(item_path) if item_path else None,
+        asset_basepath=item_path.parent if item_path else None,
         relative_paths=True,
         item_metadata=item_metadata,
         bounds=bounds,
         bands_type=bands_type,
         crs_unit_to_meter=crs_unit_to_meter,
     )
 
 
 def tile_pyramid_from_item(item):
     matrix_sets = item.properties.get("tiles:tile_matrix_sets")
     if matrix_sets:
-
         # find out grid
         wkss = next(iter(matrix_sets.keys()))
         for grid, properties in KNOWN_MATRIX_PROPERTIES.items():
             if properties["name"] == wkss:
                 break
         else:
             raise ValueError(f"STAC tiled-assets WKSS not known: {wkss}")
@@ -450,15 +450,15 @@
         if mp.config.output.tiles_exist(output_tile=prototype_tile):
             logger.debug("prototype tile %s already exists", tile_path)
             pass
         # if not, write empty tile
         else:
             logger.debug("creating prototype tile %s", tile_path)
             out_profile = mp.config.output.profile(prototype_tile)
-            makedirs(os.path.dirname(tile_path))
+            tile_path.makedirs()
             write_raster_window(
                 in_tile=prototype_tile,
                 in_data=ma.masked_array(
                     data=np.full(
                         (out_profile["count"],) + prototype_tile.shape,
                         out_profile["nodata"],
                         dtype=out_profile["dtype"],
```

### Comparing `mapchete-2023.4.1/mapchete/testing.py` & `mapchete-2023.6.0/mapchete/testing.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,74 +1,132 @@
 """
 Useful tools to facilitate testing.
 """
-from collections import OrderedDict
 import logging
-import os
+import uuid
+from collections import OrderedDict
+
 import oyaml as yaml
 from shapely.ops import unary_union
-import uuid
 
 import mapchete
 from mapchete.config import initialize_inputs, open_inputs
 from mapchete.io import fs_from_path
-from mapchete.tile import BufferedTile, BufferedTilePyramid
-
+from mapchete.path import MPath
+from mapchete.tile import BufferedTilePyramid
 
 logger = logging.getLogger(__name__)
 
 
 # helper functions
 def dict_from_mapchete(path):
     """
     Read mapchete configuration from file and return as dictionary.
     """
-    with open(path) as src:
-        return dict(yaml.safe_load(src.read()), config_dir=os.path.dirname(path))
+    path = MPath(path)
+    with path.open() as src:
+        out = dict(yaml.safe_load(src.read()), config_dir=path.dirname)
+        if "config_dir" in out:
+            out["config_dir"] = MPath(out["config_dir"])
+        elif "path" in out.get("output", {}):  # pragma: no cover
+            out["output"]["path"] = MPath.from_dict(out["output"])
+    return out
+
+
+def dict_to_yaml(dictionary):
+    def _convert(vv):
+        out = OrderedDict()
+        for k, v in vv.items():
+            if isinstance(v, MPath):
+                v = str(v)
+            elif isinstance(v, dict):
+                v = _convert(v)
+            out[k] = v
+        return out
+
+    return yaml.dump(_convert(dictionary))
 
 
 class ProcessFixture:
-    def __init__(self, path=None, output_tempdir=None, output_suffix=""):
-        self.path = path
+    def __init__(
+        self,
+        path=None,
+        tempdir=None,
+        inp_cache_tempdir=None,
+        output_suffix="",
+        **kwargs,
+    ):
+        self.path = MPath(path)
+        self.basepath = MPath.parent
+        self.output_path = None
         self.dict = None
-        if output_tempdir:
-            self._output_tempdir = (
-                os.path.join(output_tempdir, uuid.uuid4().hex) + output_suffix
-            )
+        tempdir = tempdir or kwargs.get("output_tempdir")
+        if tempdir:
+            self._tempdir = MPath(tempdir) / uuid.uuid4().hex
+        else:  # pragma: no cover
+            self._tempdir = None
+        if inp_cache_tempdir:
+            self._inp_cache_tempdir = inp_cache_tempdir / uuid.uuid4().hex
         else:
-            self._output_tempdir = None
+            self._inp_cache_tempdir = None
         self._out_fs = None
         self._mp = None
 
     def __enter__(self, *args):
         self.dict = dict_from_mapchete(self.path)
-        if self._output_tempdir:
+
+        # move all input/foo/cache/path paths to inp_cache_tempdir
+        if self._inp_cache_tempdir:
+            for key, val in self.dict.get("input", {}).items():
+                if isinstance(val, dict):
+                    if "cache" in val:
+                        if "path" in val["cache"]:
+                            path = MPath.from_dict(val["cache"])
+                            temp_path = (
+                                self._inp_cache_tempdir / key / "cache" / path.name
+                            )
+                            temp_path.makedirs()
+                            val["cache"]["path"] = temp_path
+        # replace output path with temporary path
+        if self._tempdir:
             # set output directory
-            self.dict["output"]["path"] = self._output_tempdir
+            current_output_path = MPath.from_dict(self.dict["output"])
+            if current_output_path.suffix:
+                self.dict["output"]["path"] = self._tempdir / current_output_path.name
+            else:
+                self.dict["output"]["path"] = self._tempdir / "out"
+
+            self.path = self._tempdir / self.path.name
+
+            # dump modified mapchete config to temporary directory
+            self.path.makedirs()
+            with self.path.open("w") as dst:
+                dst.write(dict_to_yaml(self.dict))
 
+        # shortcut to output path
+        self.output_path = self.dict["output"]["path"]
         return self
 
     def __exit__(self, *args):
         # properly close mapchete
         try:
             if self._mp:
                 self._mp.__exit__(*args)
         finally:
             self.clear_output()
+        if self._tempdir:
+            self._tempdir.rm(recursive=True, ignore_errors=True)
 
     def clear_output(self):
         # delete written output if any
-        if self._output_tempdir:
-            out_dir = self._output_tempdir
-        else:
-            out_dir = os.path.join(self.dict["config_dir"], self.dict["output"]["path"])
-        try:
-            fs_from_path(out_dir).rm(out_dir, recursive=True)
-        except FileNotFoundError:
-            pass
+        out_dir = (
+            self._tempdir
+            or MPath(self.dict["config_dir"]) / self.dict["output"]["path"]
+        )
+        out_dir.rm(recursive=True, ignore_errors=True)
 
     def process_mp(self, tile=None, tile_zoom=None, batch_preprocess=True):
         """
         Return MapcheteProcess object used to test processes.
         """
         mp = self.mp(batch_preprocess=batch_preprocess)
         if tile:
```

### Comparing `mapchete-2023.4.1/mapchete/tile.py` & `mapchete-2023.6.0/mapchete/tile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 """Mapchtete handling tiles."""
-from itertools import product
 import logging
+from itertools import product
 
+import numpy as np
 from affine import Affine
 from cached_property import cached_property
-import numpy as np
 from rasterio.enums import Resampling
 from rasterio.features import rasterize
 from rasterio.warp import reproject
 from shapely.geometry import box
 from tilematrix import Tile, TilePyramid
 from tilematrix._conf import ROUND
 
-
 logger = logging.getLogger(__name__)
 
 
 class BufferedTilePyramid(TilePyramid):
     """
     A special tile pyramid with fixed pixelbuffer and metatiling.
```

### Comparing `mapchete-2023.4.1/mapchete/types.py` & `mapchete-2023.6.0/mapchete/types.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.4.1/mapchete/validate.py` & `mapchete-2023.6.0/mapchete/validate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Convenience validator functions for core and extension packages."""
 
 
+import warnings
 from collections.abc import Iterable
+from typing import Dict, List, Union
+
 import numpy.ma as ma
 from rasterio.crs import CRS
-from typing import Union, List, Dict
-import warnings
 
 from mapchete.tile import BufferedTile, BufferedTilePyramid
 from mapchete.types import Bounds, ZoomLevels
 
 ########################
 # validator functionrs #
 ########################
```

### Comparing `mapchete-2023.4.1/mapchete/cli/options.py` & `mapchete-2023.6.0/mapchete/cli/options.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,21 @@
-import click
-import click_spinner
 import logging
-from multiprocessing import cpu_count, get_all_start_methods
 import os
-from rasterio.enums import Resampling
+from multiprocessing import cpu_count, get_all_start_methods
+
+import click
 import tilematrix
-import tqdm
+from rasterio.enums import Resampling
 
-import mapchete
-from mapchete.config import (
-    raw_conf,
-    bounds_from_opts,
-    MULTIPROCESSING_DEFAULT_START_METHOD,
-)
+from mapchete.config import MULTIPROCESSING_DEFAULT_START_METHOD
 from mapchete.formats import available_output_formats
-from mapchete.index import zoom_index_gen
+from mapchete.io import MPath
 from mapchete.log import set_log_level, setup_logfile
 from mapchete.validate import validate_bounds, validate_crs, validate_zooms
 
-
 logger = logging.getLogger(__name__)
 
 
 MULTIPROCESSING_START_METHODS = get_all_start_methods()
 
 
 # click callbacks #
@@ -64,15 +57,14 @@
 def _setup_logfile(ctx, param, logfile):
     if logfile:
         setup_logfile(logfile)
     return logfile
 
 
 def _cb_key_val(ctx, param, value):
-
     """
     from: https://github.com/mapbox/rasterio/blob/69305c72b58b15a96330d371ad90ef31c209e981/rasterio/rio/options.py
 
     click callback to validate `--opt KEY1=VAL1 --opt KEY2=VAL2` and collect
     in a dictionary like the one below, which is what the CLI function receives.
     If no value or `None` is received then an empty dictionary is returned.
         {
@@ -139,15 +131,15 @@
 
 
 # click options #
 #################
 opt_out_path = click.option(
     "--out-path",
     type=click.Path(),
-    default=os.path.join(os.getcwd(), "output"),
+    default=MPath(os.getcwd()) / "output",
     help="Output path.",
 )
 opt_idx_out_dir = click.option(
     "--idx-out-dir", type=click.Path(), help="Index output directory."
 )
 opt_input_file = click.option(
     "--input-file",
```

### Comparing `mapchete-2023.4.1/mapchete/cli/default/convert.py` & `mapchete-2023.6.0/mapchete/cli/default/convert.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import click
+import tilematrix
+import tqdm
 from rasterio.dtypes import dtype_ranges
 from rasterio.enums import Resampling
 from rasterio.rio.options import creation_options
-import tilematrix
-import tqdm
 
 import mapchete
 from mapchete import commands
 from mapchete.cli import options
 from mapchete.formats import available_output_formats
 
 OUTPUT_FORMATS = available_output_formats()
```

### Comparing `mapchete-2023.4.1/mapchete/cli/default/cp.py` & `mapchete-2023.6.0/mapchete/cli/default/cp.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.4.1/mapchete/cli/default/create.py` & `mapchete-2023.6.0/mapchete/cli/default/create.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """Create dummy Mapchete and python process files."""
 
-import click
-from importlib_resources import files
 import os
-from string import Template
 from shutil import copyfile
+from string import Template
+
+import click
+from importlib_resources import files
 from oyaml import dump
 
 from mapchete.cli import options
+from mapchete.io import MPath
 
 FORMAT_MANDATORY = {
     "GTiff": {"bands": None, "dtype": None},
     "PNG": {"bands": None, "dtype": None},
     "PNG_hillshade": {"bands": 4, "dtype": "uint8"},
     "GeoJSON": {"schema": {}},
     "PostGIS": {
@@ -40,39 +42,41 @@
     process_file,
     out_format,
     out_path=None,
     pyramid_type=None,
     force=False,
 ):
     """Create an empty Mapchete and process file in a given directory."""
-    if os.path.isfile(process_file) or os.path.isfile(mapchete_file):
+    process_file = MPath(process_file)
+    mapchete_file = MPath(mapchete_file)
+    if process_file.exists() or mapchete_file.exists():
         if not force:
             raise IOError("file(s) already exists")
 
-    out_path = out_path if out_path else os.path.join(os.getcwd(), "output")
+    out_path = out_path if out_path else MPath(os.getcwd()) / "output"
 
     # copy file template to target directory
     # Reads contents with UTF-8 encoding and returns str.
     process_template = str(files("mapchete.static").joinpath("process_template.py"))
-    process_file = os.path.join(os.getcwd(), process_file)
+    process_file = MPath(os.getcwd()) / process_file
     copyfile(process_template, process_file)
 
     # modify and copy mapchete file template to target directory
     mapchete_template = str(
         files("mapchete.static").joinpath("mapchete_template.mapchete")
     )
 
     output_options = dict(
-        format=out_format, path=out_path, **FORMAT_MANDATORY[out_format]
+        format=out_format, path=str(out_path), **FORMAT_MANDATORY[out_format]
     )
 
     pyramid_options = {"grid": pyramid_type}
 
     substitute_elements = {
-        "process_file": process_file,
+        "process_file": str(process_file),
         "output": dump({"output": output_options}, default_flow_style=False),
         "pyramid": dump({"pyramid": pyramid_options}, default_flow_style=False),
     }
     with open(mapchete_template, "r") as config_template:
         config = Template(config_template.read())
         customized_config = config.substitute(substitute_elements)
     with open(mapchete_file, "w") as target_config:
```

### Comparing `mapchete-2023.4.1/mapchete/cli/default/execute.py` & `mapchete-2023.6.0/mapchete/cli/default/execute.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.4.1/mapchete/cli/default/formats.py` & `mapchete-2023.6.0/mapchete/cli/default/formats.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.4.1/mapchete/cli/default/index.py` & `mapchete-2023.6.0/mapchete/cli/default/index.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """Create index for process output."""
 
-import click
-import click_spinner
 import logging
 import os
 import sys
+
+import click
+import click_spinner
 import tqdm
 
 import mapchete
-from mapchete.cli import options
 from mapchete import commands
-
+from mapchete.cli import options
 
 # workaround for https://github.com/tqdm/tqdm/issues/481
 tqdm.monitor_interval = 0
 
 logger = logging.getLogger(__name__)
```

### Comparing `mapchete-2023.4.1/mapchete/cli/default/processes.py` & `mapchete-2023.6.0/mapchete/cli/default/processes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """CLI to list processes."""
 
-import click
 import logging
 
+import click
+
 from mapchete.cli import options
 from mapchete.processes import process_names_docstrings
 
 logger = logging.getLogger(__name__)
 
 
 @click.command(help="List available processes.")
```

### Comparing `mapchete-2023.4.1/mapchete/cli/default/rm.py` & `mapchete-2023.6.0/mapchete/cli/default/rm.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.4.1/mapchete/cli/default/serve.py` & `mapchete-2023.6.0/mapchete/cli/default/serve.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 #!/usr/bin/env python
 """Command line utility to serve a Mapchete process."""
 
-import click
 import logging
 import logging.config
 import os
 import pkgutil
+
+import click
 from rasterio.io import MemoryFile
 
 import mapchete
 from mapchete.cli import options
+from mapchete.io import MPath
 from mapchete.tile import BufferedTilePyramid
 
 logger = logging.getLogger(__name__)
 
 
 @click.command(help="Serve a process on localhost.")
 @options.arg_mapchete_files
@@ -75,15 +77,15 @@
     debug=None,
 ):
     """Configure and create Flask app."""
     from flask import Flask, render_template_string
 
     app = Flask(__name__)
     mapchete_processes = {
-        os.path.splitext(os.path.basename(mapchete_file))[0]: mapchete.open(
+        str(MPath(MPath(mapchete_file).name).without_suffix()): mapchete.open(
             mapchete_file,
             zoom=zoom,
             bounds=bounds,
             single_input_file=single_input_file,
             mode=mode,
             with_cache=True,
             debug=debug,
@@ -160,20 +162,21 @@
         else:
             from flask import abort
 
             abort(500)
 
 
 def _valid_tile_response(mp, data):
-    from flask import send_file, make_response, jsonify
+    from flask import make_response, jsonify
+    from flask_rangerequest import RangeRequest
 
     out_data, mime_type = mp.config.output.for_web(data)
     logger.debug("create tile response %s", mime_type)
     if isinstance(out_data, MemoryFile):
-        response = make_response(send_file(out_data, mime_type))
+        return RangeRequest(out_data).make_response()
     elif isinstance(out_data, list):
         response = make_response(jsonify(data))
     else:
         response = make_response(out_data)
     response.headers["Content-Type"] = mime_type
     response.cache_control.no_write = True
     return response
```

### Comparing `mapchete-2023.4.1/mapchete/cli/default/stac.py` & `mapchete-2023.6.0/mapchete/cli/default/stac.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-import click
-import fsspec
-import logging
 import json
+import logging
 import os
+
+import click
+import fsspec
 import oyaml as yaml
 
 import mapchete
 from mapchete.cli import options
 from mapchete.config import raw_conf, raw_conf_output_pyramid
 from mapchete.formats import read_output_metadata
-from mapchete.stac import tile_directory_stac_item, create_prototype_files
+from mapchete.io import MPath
+from mapchete.stac import create_prototype_files, tile_directory_stac_item
 from mapchete.validate import validate_zooms
 
-
 logger = logging.getLogger(__name__)
 
 
 @click.group(help="Tools to handle STAC metadata.")
 def stac():
     pass
 
@@ -79,15 +80,15 @@
         with fsspec.open(item_metadata) as src:
             metadata = yaml.safe_load(src.read())
     else:
         metadata = default_item_metadata or {}
 
     item_id = item_id or metadata.get("id", default_id)
     logger.debug("use item ID %s", item_id)
-    item_path = item_path or os.path.join(default_basepath, f"{item_id}.json")
+    item_path = item_path or MPath(default_basepath) / f"{item_id}.json"
     item = tile_directory_stac_item(
         item_id=item_id,
         item_metadata=metadata,
         tile_pyramid=tile_pyramid,
         zoom_levels=zoom,
         bounds=bounds or default_bounds,
         bounds_crs=bounds_crs or default_bounds_crs,
@@ -102,32 +103,32 @@
     click.echo(item_json)
     if force or click.confirm(f"Write output to {item_path}?", abort=True):
         with fsspec.open(item_path, "w") as dst:
             dst.write(item_json)
 
 
 def output_info(inp):
-    if inp.endswith(".mapchete"):
-        conf = raw_conf(inp)
-        default_basepath = os.path.dirname(conf["output"]["path"].strip("/") + "/")
+    path = MPath(inp)
+    if path.suffix == ".mapchete":
+        conf = raw_conf(path)
+        default_basepath = MPath.from_dict(conf["output"])
         return (
             raw_conf_output_pyramid(conf),
             default_basepath,
-            os.path.basename(default_basepath),
+            default_basepath.name,
             conf.get("bounds"),
             conf.get("bounds_crs"),
             conf.get("zoom_levels"),
             conf["output"].get("stac"),
         )
 
-    default_basepath = inp.strip("/")
     return (
-        read_output_metadata(os.path.join(inp, "metadata.json"))["pyramid"],
-        default_basepath,
-        os.path.basename(default_basepath),
+        read_output_metadata(path / "metadata.json")["pyramid"],
+        path,
+        path.name,
         None,
         None,
         None,
         None,
     )
```

### Comparing `mapchete-2023.4.1/mapchete/commands/_convert.py` & `mapchete-2023.6.0/mapchete/commands/_convert.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,41 @@
-import fiona
-import logging
 import json
-from multiprocessing import cpu_count
+import logging
 import os
+import warnings
+from multiprocessing import cpu_count
 from pprint import pformat
-import rasterio
+from typing import Callable, List, Tuple, Union
+
+import tilematrix
 from rasterio.crs import CRS
 from rasterio.vrt import WarpedVRT
 from shapely.geometry import box
 from shapely.geometry.base import BaseGeometry
-import tilematrix
-from typing import Callable, List, Tuple, Union
-import warnings
 
 import mapchete
 from mapchete.commands._execute import execute
 from mapchete.config import raw_conf, raw_conf_output_pyramid
 from mapchete.formats import (
-    driver_from_file,
-    available_output_formats,
     available_input_formats,
+    available_output_formats,
+    driver_from_file,
 )
-from mapchete.io import read_json, get_best_zoom_level, fs_from_path
+from mapchete.io import MPath, fiona_open, get_best_zoom_level, rasterio_open, read_json
 from mapchete.io.vector import reproject_geometry
 from mapchete.tile import BufferedTilePyramid
 from mapchete.validate import validate_zooms
 
 logger = logging.getLogger(__name__)
 OUTPUT_FORMATS = available_output_formats()
 
 
 def convert(
-    tiledir: Union[str, dict],
-    output: str,
+    tiledir: Union[str, dict, MPath],
+    output: Union[str, MPath],
     zoom: Union[int, List[int]] = None,
     area: Union[BaseGeometry, str, dict] = None,
     area_crs: Union[CRS, str] = None,
     bounds: Tuple[float] = None,
     bounds_crs: Union[CRS, str] = None,
     point: Tuple[float, float] = None,
     point_crs: Tuple[float, float] = None,
@@ -173,28 +172,29 @@
 
     msg_callback = msg_callback or _empty_callback
     if multi is not None:  # pragma: no cover
         warnings.warn("The 'multi' parameter is deprecated and is now named 'workers'")
     workers = workers or multi or cpu_count()
     creation_options = creation_options or {}
     bidx = [bidx] if isinstance(bidx, int) else bidx
+    tiledir = MPath(tiledir) if isinstance(tiledir, str) else tiledir
+    output = MPath(output)
     try:
         input_info = _get_input_info(tiledir)
         logger.debug("input params: %s", input_info)
         output_info = _get_output_info(output)
         logger.debug("output params: %s", output_info)
     except Exception as e:
         raise ValueError(e)
 
     if (
-        isinstance(output_pyramid, str)
+        isinstance(output_pyramid, (str, MPath))
         and output_pyramid not in tilematrix._conf.PYRAMID_PARAMS.keys()
     ):
-        with fs_from_path(output_pyramid).open(output_pyramid) as src:
-            output_pyramid = json.loads(src.read())
+        output_pyramid = json.loads(MPath(output_pyramid).read_text())
 
     # collect mapchete configuration
     mapchete_config = dict(
         process="mapchete.processes.convert",
         input=dict(inp=tiledir, clip=clip_geometry),
         pyramid=(
             dict(
@@ -325,22 +325,21 @@
         workers=workers,
         as_iterator=as_iterator,
         msg_callback=msg_callback,
     )
 
 
 def _clip_bbox(clip_geometry, dst_crs=None):
-    with fiona.open(clip_geometry) as src:
+    with fiona_open(clip_geometry) as src:
         return reproject_geometry(box(*src.bounds), src_crs=src.crs, dst_crs=dst_crs)
 
 
 def _get_input_info(inp):
-
     # assuming single file if path has a file extension
-    if os.path.splitext(inp)[1]:
+    if inp.suffix:
         logger.debug("assuming single file")
         driver = driver_from_file(inp)
 
         # single file input can be a mapchete file or a rasterio/fiona file
         if driver == "Mapchete":
             logger.debug("input is mapchete file")
             input_info = _input_mapchete_info(inp)
@@ -376,15 +375,15 @@
         pixel_size=None,
         input_type=OUTPUT_FORMATS[output_params["format"]]["data_type"],
         bounds=conf.get("bounds"),
     )
 
 
 def _input_rasterio_info(inp):
-    with rasterio.open(inp) as src:
+    with rasterio_open(inp) as src:
         if src.transform.is_identity:
             if src.gcps[1] is not None:
                 with WarpedVRT(src) as dst:
                     bounds = dst.bounds
                     crs = src.gcps[1]
             elif src.rpcs:  # pragma: no cover
                 with WarpedVRT(src) as dst:
@@ -407,43 +406,42 @@
             pixel_size=src.transform[0],
             input_type="raster",
             bounds=bounds,
         )
 
 
 def _input_fiona_info(inp):
-    with fiona.open(inp) as src:
+    with fiona_open(inp) as src:
         return dict(
             output_params=dict(
                 schema=src.schema,
                 format=src.driver if src.driver in available_input_formats() else None,
             ),
             pyramid=None,
             crs=src.crs,
             zoom_levels=None,
             input_type="vector",
             bounds=src.bounds if len(src) else None,
         )
 
 
-def _input_tile_directory_info(inp):
-    conf = read_json(os.path.join(inp, "metadata.json"))
+def _input_tile_directory_info(tiledir_path):
+    conf = read_json(tiledir_path / "metadata.json")
     pyramid = BufferedTilePyramid.from_dict(conf["pyramid"])
     return dict(
         output_params=conf["driver"],
         pyramid=pyramid.to_dict(),
         crs=pyramid.crs,
         zoom_levels=None,
         pixel_size=None,
         input_type=OUTPUT_FORMATS[conf["driver"]["format"]]["data_type"],
         bounds=None,
     )
 
 
 def _get_output_info(output):
-    _, file_ext = os.path.splitext(output)
-    if not file_ext:
+    if not output.suffix:
         return dict(type="TileDirectory", driver=None)
-    elif file_ext == ".tif":
+    elif output.suffix == ".tif":
         return dict(type="SingleFile", driver="GTiff")
     else:
-        raise TypeError(f"Could not determine output from extension: {file_ext}")
+        raise TypeError(f"Could not determine output from extension: {output.suffix}")
```

### Comparing `mapchete-2023.4.1/mapchete/commands/_cp.py` & `mapchete-2023.6.0/mapchete/commands/_cp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 """Copy tiles between Tile Directories."""
 
 import logging
-from multiprocessing import cpu_count
 import os
-from typing import Callable, List, Tuple, Union
 import warnings
+from multiprocessing import cpu_count
+from typing import Callable, List, Tuple, Union
 
 from rasterio.crs import CRS
 from shapely.geometry import Point
 from shapely.geometry.base import BaseGeometry
 
 import mapchete
-from mapchete.io import fs_from_path, tiles_exist, copy
+from mapchete.io import MPath, copy, fs_from_path, tiles_exist
 from mapchete.io.vector import reproject_geometry
 
 logger = logging.getLogger(__name__)
 
 
 def cp(
-    src_tiledir: str,
-    dst_tiledir: str,
+    src_tiledir: Union[str, MPath],
+    dst_tiledir: Union[str, MPath],
     zoom: Union[int, List[int]] = None,
     area: Union[BaseGeometry, str, dict] = None,
     area_crs: Union[CRS, str] = None,
     bounds: Tuple[float] = None,
     bounds_crs: Union[CRS, str] = None,
     point: Tuple[float, float] = None,
     point_crs: Tuple[float, float] = None,
@@ -109,16 +109,18 @@
         warnings.warn("The 'multi' parameter is deprecated and is now named 'workers'")
     workers = workers or multi or cpu_count()
     src_fs_opts = src_fs_opts or {}
     dst_fs_opts = dst_fs_opts or {}
     if zoom is None:  # pragma: no cover
         raise ValueError("zoom level(s) required")
 
-    src_fs = fs_from_path(src_tiledir, **src_fs_opts)
-    dst_fs = fs_from_path(dst_tiledir, **dst_fs_opts)
+    src_tiledir = MPath(src_tiledir, **src_fs_opts)
+    dst_tiledir = MPath(dst_tiledir, **dst_fs_opts)
+    src_fs = src_tiledir.fs
+    dst_fs = dst_tiledir.fs
 
     # open source tile directory
     with mapchete.open(
         src_tiledir,
         zoom=zoom,
         area=area,
         area_crs=area_crs,
@@ -127,16 +129,16 @@
         fs=src_fs,
         fs_kwargs=src_fs_opts,
         mode="readonly",
     ) as src_mp:
         tp = src_mp.config.output_pyramid
 
         # copy metadata to destination if necessary
-        src_metadata = os.path.join(src_tiledir, "metadata.json")
-        dst_metadata = os.path.join(dst_tiledir, "metadata.json")
+        src_metadata = src_tiledir / "metadata.json"
+        dst_metadata = dst_tiledir / "metadata.json"
         if not dst_fs.exists(dst_metadata):
             msg = f"copy {src_metadata} to {dst_metadata}"
             logger.debug(msg)
             msg_callback(msg)
             copy(
                 src_metadata,
                 dst_metadata,
```

### Comparing `mapchete-2023.4.1/mapchete/commands/_execute.py` & `mapchete-2023.6.0/mapchete/commands/_execute.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Execute a process."""
 
 import logging
-from multiprocessing import cpu_count
 import traceback
-from typing import Callable, List, Tuple, Union
 import warnings
+from multiprocessing import cpu_count
+from typing import Callable, List, Tuple, Union
 
 from rasterio.crs import CRS
 from shapely.geometry.base import BaseGeometry
 
 import mapchete
-from mapchete.config import bounds_from_opts, raw_conf, raw_conf_process_pyramid
 from mapchete._processing import PreprocessingProcessInfo, TileProcessInfo
+from mapchete.config import bounds_from_opts, raw_conf, raw_conf_process_pyramid
 
 logger = logging.getLogger(__name__)
 
 
 def execute(
     mapchete_config: Union[str, dict],
     zoom: Union[int, List[int]] = None,
```

### Comparing `mapchete-2023.4.1/mapchete/commands/_index.py` & `mapchete-2023.6.0/mapchete/commands/_index.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,14 @@
         point=point,
         point_crs=point_crs,
         bounds=bounds,
         bounds_crs=bounds_crs,
         area=area,
         area_crs=area_crs,
     ) as mp:
-
         return mapchete.Job(
             zoom_index_gen,
             fkwargs=dict(
                 mp=mp,
                 zoom=None if tile else mp.config.init_zoom_levels,
                 tile=tile,
                 out_dir=idx_out_dir if idx_out_dir else mp.config.output.path,
```

### Comparing `mapchete-2023.4.1/mapchete/commands/_rm.py` & `mapchete-2023.6.0/mapchete/commands/_rm.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.4.1/mapchete/commons/clip.py` & `mapchete-2023.6.0/mapchete/commons/clip.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Clip array using vector data."""
 import numpy as np
 import numpy.ma as ma
-from shapely.ops import unary_union
 from rasterio.features import geometry_mask
+from shapely.ops import unary_union
 
 from mapchete.io.vector import to_shape
 
 
 def clip_array_with_vector(
     array, array_affine, geometries, inverted=False, clip_buffer=0
 ):
```

### Comparing `mapchete-2023.4.1/mapchete/commons/contours.py` & `mapchete-2023.6.0/mapchete/commons/contours.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.4.1/mapchete/commons/hillshade.py` & `mapchete-2023.6.0/mapchete/commons/hillshade.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,18 +29,19 @@
 FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """
+import math
+from itertools import product
+
 import numpy as np
 import numpy.ma as ma
-from itertools import product
-import math
 
 
 def calculate_slope_aspect(elevation, xres, yres, z=1.0, scale=1.0):
     """
     Calculate slope and aspect map.
 
     Return a pair of arrays 2 pixels smaller than the input elevation array.
```

### Comparing `mapchete-2023.4.1/mapchete/formats/__init__.py` & `mapchete-2023.6.0/mapchete/formats/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -2,23 +2,23 @@
     load_input_reader,
     load_output_reader,
     load_output_writer,
 )
 from mapchete.formats.tools import (
     available_input_formats,
     available_output_formats,
-    driver_metadata,
+    compare_metadata_params,
+    data_type_from_extension,
     driver_from_extension,
     driver_from_file,
-    data_type_from_extension,
+    driver_metadata,
     dump_metadata,
     load_metadata,
     read_output_metadata,
     write_output_metadata,
-    compare_metadata_params,
 )
 
 __all__ = [
     "available_input_formats",
     "available_output_formats",
     "load_input_reader",
     "load_output_reader",
```

### Comparing `mapchete-2023.4.1/mapchete/formats/base.py` & `mapchete-2023.6.0/mapchete/formats/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 """
 Main base classes for input and output formats.
 
 When writing a new driver, please inherit from these classes and implement the
 respective interfaces.
 """
 
-from itertools import chain
 import logging
-import numpy as np
-import numpy.ma as ma
 import os
-from shapely.geometry import shape
 import types
 import warnings
+from itertools import chain
 
+import numpy as np
+import numpy.ma as ma
+from shapely.geometry import shape
+
+from mapchete._tasks import Task
 from mapchete.config import get_hash
-from mapchete.errors import MapcheteProcessOutputError, MapcheteNodataTile
+from mapchete.errors import MapcheteNodataTile, MapcheteProcessOutputError
 from mapchete.formats import write_output_metadata
-from mapchete.io import makedirs, path_exists, fs_from_path
+from mapchete.io import fs_from_path, makedirs, path_exists
 from mapchete.io.raster import (
     create_mosaic,
     extract_from_array,
     prepare_array,
     read_raster_window,
 )
-from mapchete._tasks import Task
 from mapchete.io.vector import read_vector_window
 from mapchete.tile import BufferedTilePyramid
 
 logger = logging.getLogger(__name__)
 
 
 class InputData(object):
@@ -58,14 +59,17 @@
         self.pyramid = input_params.get("pyramid")
         self.pixelbuffer = input_params.get("pixelbuffer")
         self.crs = self.pyramid.crs if self.pyramid else None
         # collect preprocessing tasks to be run by the Executor
         self.preprocessing_tasks = {}
         # storage location of all preprocessing tasks
         self.preprocessing_tasks_results = {}
+        self.storage_options = input_params.get("abstract", {}).get(
+            "storage_options", {}
+        )
 
     def open(self, tile, **kwargs):
         """
         Return InputTile object.
 
         Parameters
         ----------
@@ -226,15 +230,14 @@
 
     def __exit__(self, t, v, tb):
         """Clean up."""
         pass
 
 
 class OutputDataBaseFunctions:
-
     write_in_parent_process = False
 
     def __init__(self, output_params, readonly=False, **kwargs):
         """Initialize."""
         self.pixelbuffer = output_params["pixelbuffer"]
         if "type" in output_params:  # pragma: no cover
             warnings.warn(
@@ -244,37 +247,33 @@
                 output_params["grid"] = output_params.pop("type")
         self.pyramid = BufferedTilePyramid(
             grid=output_params["grid"],
             metatiling=output_params["metatiling"],
             pixelbuffer=output_params["pixelbuffer"],
         )
         self.crs = self.pyramid.crs
-        self._bucket = None
+        self.storage_options = output_params.get("storage_options")
         self.fs = self._fs = output_params.get(
             "fs", fs_from_path(output_params.get("path", ""))
         )
         self.fs_kwargs = self._fs_kwargs = output_params.get("fs_kwargs") or {}
 
     @property
     def stac_path(self):
         """Return path to STAC JSON file."""
-        default_basepath = os.path.dirname(self.path.rstrip("/") + "/")
-        return os.path.join(default_basepath, f"{self.stac_item_id}.json")
+        return self.path.joinpath(f"{self.stac_item_id}.json")
 
     @property
     def stac_item_id(self):
         """
         Return STAC item ID according to configuration.
 
         Defaults to path basename.
         """
-        default_basepath = os.path.dirname(self.path.rstrip("/") + "/")
-        return self.output_params.get("stac", {}).get("id") or os.path.basename(
-            default_basepath
-        )
+        return self.output_params.get("stac", {}).get("id") or self.path.stem
 
     @property
     def stac_item_metadata(self):
         """Custom STAC metadata."""
         return self.output_params.get("stac", {})
 
     @property
@@ -306,21 +305,16 @@
         tile : ``BufferedTile``
             must be member of output ``TilePyramid``
 
         Returns
         -------
         path : string
         """
-        return os.path.join(
-            *[
-                self.path,
-                str(tile.zoom),
-                str(tile.row),
-                str(tile.col) + self.file_extension,
-            ]
+        return self.path.joinpath(
+            str(tile.zoom), str(tile.row), str(tile.col) + self.file_extension
         )
 
     def extract_subset(self, input_data_tiles=None, out_tile=None):
         """
         Extract subset from multiple tiles.
         input_data_tiles : list of (``Tile``, process data) tuples
         out_tile : ``Tile``
@@ -449,15 +443,15 @@
         Create directory and subdirectory if necessary.
 
         Parameters
         ----------
         tile : ``BufferedTile``
             must be member of output ``TilePyramid``
         """
-        makedirs(os.path.dirname(self.get_path(tile)))
+        self.get_path(tile).makedirs()
 
     def output_is_valid(self, process_data):
         """
         Check whether process output is allowed with output driver.
 
         Parameters
         ----------
```

### Comparing `mapchete-2023.4.1/mapchete/formats/loaders.py` & `mapchete-2023.6.0/mapchete/formats/loaders.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 import logging
-import os
-from typing import Dict, Optional, TYPE_CHECKING
+from typing import Dict, Optional
 
-# from mapchete.formats.base import OutputDataReader, OutputDataWriter, InputData
-from mapchete.formats.tools import driver_from_file
-from mapchete.errors import MapcheteDriverError
 from mapchete._registered import drivers
-
+from mapchete.errors import MapcheteDriverError
+from mapchete.formats.tools import driver_from_file
 
 logger = logging.getLogger(__name__)
 
 
 def load_output_reader(output_params: Dict) -> "OutputDataReader":
     """
     Return OutputReader class of driver.
@@ -92,15 +89,15 @@
         raise TypeError("input_params must be a dictionary")
 
     # find out driver name
     if "abstract" in input_params:
         driver_name = input_params["abstract"]["format"]
     elif "path" in input_params:
         # if path has a file extension it is considered a single file
-        if os.path.splitext(input_params["path"])[1]:
+        if input_params["path"].suffix:
             input_file = input_params["path"]
             driver_name = driver_from_file(input_file)
         # else a TileDirectory is assumed
         else:
             logger.debug("%s is a directory", input_params["path"])
             driver_name = "TileDirectory"
     else:
```

### Comparing `mapchete-2023.4.1/mapchete/formats/tools.py` & `mapchete-2023.6.0/mapchete/formats/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 """
 Functions handling output formats.
 
 This module deserves a cleaner rewrite some day.
 """
 
 import datetime
-import dateutil.parser
-import fiona
 import logging
-import os
+import warnings
 from pprint import pformat
-import rasterio
+from typing import Dict
+
+import dateutil.parser
 from rasterio.crs import CRS
-from typing import Dict, Type
-import warnings
 
-from mapchete.errors import MapcheteConfigError, MapcheteDriverError
-from mapchete.io import read_json, write_json, path_exists
 from mapchete._registered import drivers
+from mapchete.errors import MapcheteConfigError, MapcheteDriverError
+from mapchete.io import MPath, fiona_open, rasterio_open, read_json, write_json
 from mapchete.tile import BufferedTilePyramid
 
-
 logger = logging.getLogger(__name__)
 
 
 def available_output_formats() -> Dict:
     """
     Return all available output formats.
 
@@ -95,39 +92,39 @@
         fiona and rasterio. (default: True)
 
     Returns
     -------
     driver : string
         driver name
     """
-    file_ext = os.path.splitext(input_file)[1].split(".")[1]
+    input_file = MPath(input_file)
 
     # mapchete files can immediately be returned:
-    if file_ext == "mapchete":
+    if input_file.suffix == ".mapchete":
         return "Mapchete"
 
     # use the most common file extensions to quickly determine input driver for file:
     if quick:
         try:
-            return driver_from_extension(file_ext)
+            return driver_from_extension(input_file.suffix)
         except ValueError:
             pass
 
     # brute force by trying to open file with rasterio and fiona:
     try:
         logger.debug("try to open %s with rasterio...", input_file)
-        with rasterio.open(input_file):  # pragma: no cover
+        with rasterio_open(input_file):  # pragma: no cover
             return "raster_file"
     except Exception as rio_exception:
         try:
             logger.debug("try to open %s with fiona...", input_file)
-            with fiona.open(input_file):  # pragma: no cover
+            with fiona_open(input_file):  # pragma: no cover
                 return "vector_file"
         except Exception as fio_exception:
-            if path_exists(input_file):
+            if input_file.exists():
                 logger.exception(f"fiona error: {fio_exception}")
                 logger.exception(f"rasterio error: {rio_exception}")
                 raise MapcheteDriverError(
                     "%s has an unknown file extension and could not be opened by neither "
                     "rasterio nor fiona." % input_file
                 )
             else:
@@ -144,14 +141,15 @@
         File extension to look for.
 
     Returns
     -------
     driver : string
         driver name
     """
+    file_extension = file_extension.lstrip(".")
     all_drivers_extensions = {}
     for v in drivers:
         driver = v.load()
         try:
             driver_extensions = driver.METADATA.get("file_extensions", []).copy()
             all_drivers_extensions[driver.METADATA["driver_name"]] = driver_extensions
             if driver_extensions and file_extension in driver_extensions:
@@ -311,15 +309,15 @@
 
     Parameters
     ----------
     output_params : dict
         Output parameters
     """
     if "path" in output_params:
-        metadata_path = os.path.join(output_params["path"], "metadata.json")
+        metadata_path = MPath.from_dict(output_params) / "metadata.json"
         logger.debug("check for output %s", metadata_path)
         try:
             existing_params = read_output_metadata(metadata_path)
             logger.debug("%s exists", metadata_path)
             logger.debug("existing output parameters: %s", pformat(existing_params))
             current_params = dump_metadata(output_params)
             logger.debug("current output parameters: %s", pformat(current_params))
```

### Comparing `mapchete-2023.4.1/mapchete/formats/default/_fiona_base.py` & `mapchete-2023.6.0/mapchete/formats/default/_fiona_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """
 Baseclasses for all drivers using fiona for reading and writing data.
 """
 
-import fiona
-from fiona.errors import DriverError
 import logging
 import types
 
+from fiona.errors import DriverError
+
 from mapchete.config import validate_values
 from mapchete.formats import base
+from mapchete.io import MPath, fiona_open
 from mapchete.io.vector import write_vector_window
 from mapchete.tile import BufferedTile
 
-
 logger = logging.getLogger(__name__)
 
 
 class OutputDataReader(base.TileDirectoryOutputReader):
     """
     Output reader base class for vector drivers.
 
@@ -53,15 +53,16 @@
             must be member of output ``TilePyramid``
 
         Returns
         -------
         process output : list
         """
         try:
-            with fiona.open(self.get_path(output_tile), "r") as src:
+            path = self.get_path(output_tile)
+            with fiona_open(path, "r") as src:
                 return list(src)
         except DriverError as e:
             for i in (
                 "does not exist in the file system",
                 "No such file or directory",
                 "specified key does not exist.",
             ):
@@ -79,15 +80,15 @@
         config : dictionary
             output configuration parameters
 
         Returns
         -------
         is_valid : bool
         """
-        validate_values(config, [("schema", dict), ("path", str)])
+        validate_values(config, [("schema", dict), ("path", (str, MPath))])
         validate_values(config["schema"], [("properties", dict), ("geometry", str)])
         if config["schema"]["geometry"] not in [
             "Geometry",
             "Point",
             "MultiPoint",
             "Line",
             "LineString",
```

### Comparing `mapchete-2023.4.1/mapchete/formats/default/flatgeobuf.py` & `mapchete-2023.6.0/mapchete/formats/default/flatgeobuf.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     Polygon, MultiPolygon)
 """
 
 import warnings
 
 from mapchete.formats.default import _fiona_base
 
-
 METADATA = {"driver_name": "FlatGeobuf", "data_type": "vector", "mode": "rw"}
 
 
 class OutputDataReader(_fiona_base.OutputDataReader):
     """
     Output reader class for FlatGeobuf.
 
@@ -69,21 +68,17 @@
                         f"""'{k}' field has type '{v}' which is not allowed by FlatGeobuf """
                         """and will be changed to 'string'"""
                     )
                 )
                 output_params["schema"]["properties"][k] = "str"
 
         self.output_params = output_params
-        self._bucket = (
-            self.path.split("/")[2] if self.path.startswith("s3://") else None
-        )
 
 
 class OutputDataWriter(_fiona_base.OutputDataWriter, OutputDataReader):
-
     METADATA = METADATA
 
 
 class InputTile(_fiona_base.InputTile):
     """
     Target Tile representation of input data.
```

### Comparing `mapchete-2023.4.1/mapchete/formats/default/geobuf.py` & `mapchete-2023.6.0/mapchete/formats/default/geobuf.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,22 +15,22 @@
     the schema is passed on to fiona
     - properties: key-value pairs (fields and field types, like "id: int" etc.)
     - geometry: output geometry type (Geometry, Point, MultiPoint, Line, MultiLine,
     Polygon, MultiPolygon)
 """
 
 import logging
+
 from shapely.geometry import mapping, shape
 
 from mapchete.config import validate_values
 from mapchete.formats.default import geojson
-from mapchete.io import fs_from_path
+from mapchete.io import MPath, fs_from_path
 from mapchete.io._geometry_operations import _repair, reproject_geometry
 
-
 logger = logging.getLogger(__name__)
 METADATA = {"driver_name": "Geobuf", "data_type": "vector", "mode": "rw"}
 
 
 class OutputDataReader(geojson.OutputDataReader):
     """
     Output reader class for Geobuf Tile Directory.
@@ -99,15 +99,15 @@
         config : dictionary
             output configuration parameters
 
         Returns
         -------
         is_valid : bool
         """
-        validate_values(config, [("schema", dict), ("path", str)])
+        validate_values(config, [("schema", dict), ("path", (str, MPath))])
         validate_values(config["schema"], [("properties", dict), ("geometry", str)])
         if config["schema"]["geometry"] not in [
             "Geometry",
             "Point",
             "MultiPoint",
             "Line",
             "MultiLine",
```

### Comparing `mapchete-2023.4.1/mapchete/formats/default/geojson.py` & `mapchete-2023.6.0/mapchete/formats/default/geojson.py`

 * *Files 11% similar despite different names*

```diff
@@ -57,21 +57,17 @@
 
     def __init__(self, output_params, **kwargs):
         """Initialize."""
         super().__init__(output_params)
         self.path = output_params["path"]
         self.file_extension = ".geojson"
         self.output_params = output_params
-        self._bucket = (
-            self.path.split("/")[2] if self.path.startswith("s3://") else None
-        )
 
 
 class OutputDataWriter(_fiona_base.OutputDataWriter, OutputDataReader):
-
     METADATA = METADATA
 
 
 class InputTile(_fiona_base.InputTile):
     """
     Target Tile representation of input data.
```

### Comparing `mapchete-2023.4.1/mapchete/formats/default/gtiff.py` & `mapchete-2023.6.0/mapchete/formats/default/gtiff.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,46 +26,45 @@
 nodata: integer or float
     nodata value used for writing
 compress: string
     compression method (default: lzw): lzw, jpeg, packbits, deflate, CCITTRLE,
     CCITTFAX3, CCITTFAX4, lzma
 """
 
-from contextlib import ExitStack
 import logging
 import math
 import os
 import warnings
+from contextlib import ExitStack
 
-from affine import Affine
 import numpy as np
+from affine import Affine
 from numpy import ma
 from rasterio.enums import Resampling
 from rasterio.profiles import Profile
 from rasterio.rio.overview import get_maximum_overview_level
 from rasterio.windows import from_bounds
 from shapely.geometry import box
 from tilematrix import Bounds
 
-from mapchete.config import validate_values, snap_bounds, _OUTPUT_PARAMETERS
+from mapchete.config import _OUTPUT_PARAMETERS, snap_bounds, validate_values
 from mapchete.errors import MapcheteConfigError
 from mapchete.formats import base
-from mapchete.io import makedirs, path_exists, path_is_remote
+from mapchete.io import MPath, makedirs, path_exists, path_is_remote
 from mapchete.io.raster import (
-    write_raster_window,
-    prepare_array,
-    memory_file,
-    read_raster_no_crs,
     extract_from_array,
+    memory_file,
+    prepare_array,
     rasterio_write,
+    read_raster_no_crs,
+    write_raster_window,
 )
 from mapchete.tile import BufferedTile
 from mapchete.validate import deprecated_kwargs
 
-
 logger = logging.getLogger(__name__)
 
 
 class DefaultGTiffProfile(Profile):
     """Tiled, band-interleaved, DEFLATE-compressed, 8-bit GTiff."""
 
     defaults = {
@@ -150,15 +149,15 @@
         spatial reference ID of CRS (e.g. "{'init': 'epsg:4326'}")
     """
 
     def __new__(self, output_params, **kwargs):
         """Initialize."""
         self.path = output_params["path"]
         self.file_extension = ".tif"
-        if self.path.endswith(self.file_extension):
+        if self.path.suffix == self.file_extension:
             return GTiffSingleFileOutputWriter(output_params, **kwargs)
         else:
             return GTiffTileDirectoryOutputWriter(output_params, **kwargs)
 
 
 class GTiffOutputReaderFunctions:
     """Common functions."""
@@ -236,15 +235,17 @@
         config : dictionary
             output configuration parameters
 
         Returns
         -------
         is_valid : bool
         """
-        return validate_values(config, [("bands", int), ("path", str), ("dtype", str)])
+        return validate_values(
+            config, [("bands", int), ("path", (str, MPath)), ("dtype", str)]
+        )
 
     def _set_attributes(self, output_params):
         self.path = output_params["path"]
         self.file_extension = ".tif"
         self.output_params = dict(
             output_params,
             nodata=output_params.get("nodata", GTIFF_DEFAULT_PROFILE["nodata"]),
@@ -397,15 +398,14 @@
         """GeoTIFF media type."""
         return "image/tiff; application=geotiff"
 
 
 class GTiffSingleFileOutputWriter(
     GTiffOutputReaderFunctions, base.SingleFileOutputWriter
 ):
-
     write_in_parent_process = True
 
     def __init__(self, output_params, **kwargs):
         """Initialize."""
         logger.debug("output is single file")
         self.dst = None
         super().__init__(output_params, **kwargs)
@@ -503,15 +503,15 @@
                 raise MapcheteConfigError(
                     "single GTiff file already exists, use overwrite mode to replace"
                 )
             elif not path_is_remote(self.path):
                 logger.debug("remove existing file: %s", self.path)
                 os.remove(self.path)
         # create output directory if necessary
-        makedirs(os.path.dirname(self.path))
+        self.path.makedirs()
         logger.debug("open output file: %s", self.path)
         self._ctx = ExitStack()
         self.dst = self._ctx.enter_context(
             rasterio_write(self.path, "w+", **self._profile)
         )
 
     def read(self, output_tile, **kwargs):
```

### Comparing `mapchete-2023.4.1/mapchete/formats/default/mapchete_input.py` & `mapchete-2023.6.0/mapchete/formats/default/mapchete_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Use another Mapchete process as input."""
 
 from mapchete import Mapchete
 from mapchete.config import MapcheteConfig
 from mapchete.formats import base
 from mapchete.io.vector import reproject_geometry
 
-
 METADATA = {
     "driver_name": "Mapchete",
     "data_type": None,
     "mode": "r",
     "file_extensions": ["mapchete"],
 }
```

### Comparing `mapchete-2023.4.1/mapchete/formats/default/png.py` & `mapchete-2023.6.0/mapchete/formats/default/png.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,28 +16,29 @@
 ~~~~~~~~
 
 nodata: integer or float
     nodata value used for writing
 """
 
 import logging
+
 import numpy as np
 import numpy.ma as ma
 
 from mapchete.config import validate_values
 from mapchete.formats import base
 from mapchete.io.raster import (
-    write_raster_window,
-    prepare_array,
+    MPath,
     memory_file,
+    prepare_array,
     read_raster_no_crs,
+    write_raster_window,
 )
 from mapchete.tile import BufferedTile
 
-
 logger = logging.getLogger(__name__)
 METADATA = {"driver_name": "PNG", "data_type": "raster", "mode": "w"}
 PNG_DEFAULT_PROFILE = {"dtype": "uint8", "driver": "PNG", "count": 4, "nodata": 0}
 
 
 class OutputDataReader(base.TileDirectoryOutputReader):
     """
@@ -108,15 +109,15 @@
         config : dictionary
             output configuration parameters
 
         Returns
         -------
         is_valid : bool
         """
-        return validate_values(config, [("path", str)])
+        return validate_values(config, [("path", (str, MPath))])
 
     def profile(self, tile=None):
         """
         Create a metadata dictionary for rasterio.
 
         Parameters
         ----------
@@ -211,15 +212,14 @@
             rgba = np.array(data).astype("uint8", copy=False)
         else:
             raise TypeError("invalid number of bands: %s" % len(data))
         return rgba
 
 
 class OutputDataWriter(base.OutputDataWriter, OutputDataReader):
-
     METADATA = METADATA
 
     def write(self, process_tile, data):
         """
         Write data from one or more process tiles.
 
         Parameters
```

### Comparing `mapchete-2023.4.1/mapchete/formats/default/png_hillshade.py` & `mapchete-2023.6.0/mapchete/formats/default/png_hillshade.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,28 +17,29 @@
 ~~~~~~~~
 
 nodata: integer or float
     nodata value used for writing
 """
 
 import logging
+
 import numpy as np
 import numpy.ma as ma
 
 from mapchete.config import validate_values
 from mapchete.formats import base
+from mapchete.io import MPath
 from mapchete.io.raster import (
-    write_raster_window,
-    prepare_array,
     memory_file,
+    prepare_array,
     read_raster_no_crs,
+    write_raster_window,
 )
 from mapchete.tile import BufferedTile
 
-
 logger = logging.getLogger(__name__)
 METADATA = {"driver_name": "PNG_hillshade", "data_type": "raster", "mode": "w"}
 PNG_DEFAULT_PROFILE = {"dtype": "uint8", "driver": "PNG", "count": 2, "nodata": 255}
 
 
 class OutputDataReader(base.TileDirectoryOutputReader):
     """
@@ -122,15 +123,15 @@
         config : dictionary
             output configuration parameters
 
         Returns
         -------
         is_valid : bool
         """
-        return validate_values(config, [("path", str)])
+        return validate_values(config, [("path", (str, MPath))])
 
     def profile(self, tile=None):
         """
         Create a metadata dictionary for rasterio.
 
         Parameters
         ----------
@@ -193,15 +194,14 @@
             data = np.stack([zeros, zeros, zeros, data])
         else:
             data = np.stack([zeros, data])
         return prepare_array(data, dtype="uint8", masked=True, nodata=255)
 
 
 class OutputDataWriter(base.OutputDataWriter, OutputDataReader):
-
     METADATA = METADATA
 
     def write(self, process_tile, data):
         """
         Write data from process tiles into PNG file(s).
 
         Parameters
```

### Comparing `mapchete-2023.4.1/mapchete/formats/default/raster_file.py` & `mapchete-2023.6.0/mapchete/formats/default/raster_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 """
 Raster file input which can be read by rasterio.
 
 Currently limited by extensions .tif, .vrt., .png and .jp2 but could be
 extended easily.
 """
 
-from cached_property import cached_property
-from copy import deepcopy
 import logging
+import warnings
+from copy import deepcopy
+
 import numpy.ma as ma
-import os
-import rasterio
 from rasterio.crs import CRS
 from rasterio.vrt import WarpedVRT
 from shapely.geometry import box
-import warnings
 
+from mapchete import io
 from mapchete.formats import base
-from mapchete.io.vector import reproject_geometry, segmentize_geometry
 from mapchete.io.raster import (
-    read_raster_window,
     convert_raster,
+    rasterio_open,
     read_raster,
+    read_raster_window,
     resample_from_array,
 )
-from mapchete import io
-
+from mapchete.io.vector import reproject_geometry, segmentize_geometry
+from mapchete.path import MPath
 
 logger = logging.getLogger(__name__)
 
 METADATA = {
     "driver_name": "raster_file",
     "data_type": "raster",
     "mode": "r",
@@ -76,15 +75,15 @@
         """Initialize."""
         super().__init__(input_params, **kwargs)
         self.path = (
             input_params["abstract"]["path"]
             if "abstract" in input_params
             else input_params["path"]
         )
-        with rasterio.open(self.path, "r") as src:
+        with rasterio_open(self.path, "r") as src:
             self.profile = deepcopy(src.meta)
             # determine bounding box
             if src.transform.is_identity:
                 if src.gcps[1] is not None:
                     with WarpedVRT(src) as dst:
                         self._src_bounds = dst.bounds
                         self._src_crs = src.gcps[1]
@@ -102,18 +101,21 @@
                 self._src_transform = src.transform
             self._src_bbox = box(*self._src_bounds)
 
         self._cache_task = f"cache_{self.path}"
         if "abstract" in input_params and "cache" in input_params["abstract"]:
             if isinstance(input_params["abstract"]["cache"], dict):
                 if "path" in input_params["abstract"]["cache"]:
-                    self._cached_path = io.absolute_path(
-                        path=input_params["abstract"]["cache"]["path"],
-                        base_dir=input_params["conf_dir"],
-                    )
+                    cached_path = MPath.from_dict(input_params["abstract"]["cache"])
+                    if cached_path.is_absolute():
+                        self._cached_path = cached_path
+                    else:  # pragma: no cover
+                        self._cached_path = cached_path.absolute_path(
+                            base_dir=input_params["conf_dir"],
+                        )
                 else:  # pragma: no cover
                     raise ValueError("please provide a cache path")
                 # add preprocessing task to cache data
                 self.add_preprocessing_task(
                     convert_raster,
                     key=self._cache_task,
                     fkwargs=dict(
@@ -201,24 +203,21 @@
         """
         Check if data or file even exists.
 
         Returns
         -------
         file exists : bool
         """
-        return os.path.isfile(self.path)  # pragma: no cover
+        return self.path.exists()  # pragma: no cover
 
     def cleanup(self):
         """Cleanup when mapchete closes."""
-        if self._cached_path and not self._cache_keep:
+        if self._cached_path and not self._cache_keep:  # pragma: no cover
             logger.debug("remove cached file %s", self._cached_path)
-            try:
-                io.fs_from_path(self._cached_path).rm(self._cached_path)
-            except FileNotFoundError:
-                pass
+            self._cached_path.rm(ignore_errors=True)
 
 
 class InputTile(base.InputTile):
     """
     Target Tile representation of input data.
 
     Parameters
```

### Comparing `mapchete-2023.4.1/mapchete/formats/default/tile_directory.py` & `mapchete-2023.6.0/mapchete/formats/default/tile_directory.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 """Use a directory of zoom/row/column tiles as input."""
 
 import logging
-import os
+from functools import cached_property
+
 from shapely.geometry import box
 
 from mapchete.config import validate_values
 from mapchete.errors import MapcheteConfigError
 from mapchete.formats import (
     base,
     data_type_from_extension,
+    driver_from_extension,
     driver_metadata,
     load_output_writer,
     read_output_metadata,
 )
-from mapchete.io import path_exists, absolute_path, tile_to_zoom_level
+from mapchete.io import MPath, tile_to_zoom_level
 from mapchete.io.vector import reproject_geometry
 from mapchete.tile import BufferedTilePyramid
 
-
 logger = logging.getLogger(__name__)
 METADATA = {
     "driver_name": "TileDirectory",
     "data_type": None,
     "mode": "r",
     "file_extensions": None,
 }
@@ -51,106 +52,121 @@
     """
 
     METADATA = METADATA
 
     def __init__(self, input_params, **kwargs):
         """Initialize."""
         super().__init__(input_params, **kwargs)
+        self._read_as_tiledir_func = None
+        logger.debug("InputData params: %s", input_params)
+        # populate internal parameters initially depending on whether this input was
+        # defined as simple or abstract input
+        self._params = input_params.get("abstract") or dict(path=input_params["path"])
+        # construct path and append optional filesystem options
+        self.path = MPath.from_dict(self._params).absolute_path(
+            input_params.get("conf_dir")
+        )
         if "abstract" in input_params:
-            self._params = input_params["abstract"]
-            self.path = absolute_path(
-                path=self._params["path"], base_dir=input_params["conf_dir"]
-            )
-            logger.debug("InputData params: %s", input_params)
-            # define pyramid
-            self.td_pyramid = BufferedTilePyramid(
-                self._params["grid"],
-                metatiling=self._params.get("metatiling", 1),
-                tile_size=self._params.get("tile_size", 256),
-                pixelbuffer=self._params.get("pixelbuffer", 0),
-            )
-            self._read_as_tiledir_func = base._read_as_tiledir
-            try:
-                self._tiledir_metadata_json = read_output_metadata(
-                    os.path.join(self.path, "metadata.json")
+            # define pyramid either by hardcoded given values or by existing metadata.json
+            if "grid" in self._params:
+                self.td_pyramid = BufferedTilePyramid(
+                    self._params["grid"],
+                    metatiling=self._params.get("metatiling", 1),
+                    tile_size=self._params.get("tile_size", 256),
+                    pixelbuffer=self._params.get("pixelbuffer", 0),
                 )
+            else:
                 try:
-                    self._data_type = self._tiledir_metadata_json["driver"]["data_type"]
-                except KeyError:
-                    self._data_type = driver_metadata(
-                        self._tiledir_metadata_json["driver"]["format"]
-                    )["data_type"]
-            except FileNotFoundError:
-                # in case no metadata.json is available, try to guess data type via the
-                # format file extension
+                    self.td_pyramid = self._tiledir_metadata_json["pyramid"]
+                except FileNotFoundError:
+                    raise MapcheteConfigError(
+                        f"Pyramid not defined and cannot find metadata.json in {self.path}"
+                    )
+            self._read_as_tiledir_func = base._read_as_tiledir
+            if "extension" in self._params:
                 self._data_type = data_type_from_extension(self._params["extension"])
+            else:
+                try:
+                    self._data_type = self._tiledir_metadata_json["driver"].get(
+                        "data_type",
+                        driver_metadata(
+                            self._tiledir_metadata_json["driver"]["format"]
+                        )["data_type"],
+                    )
+                except FileNotFoundError:
+                    # in case no metadata.json is available, try to guess data type via the
+                    # format file extension
+                    raise MapcheteConfigError(
+                        f"data type not defined and cannot find metadata.json in {self.path}"
+                    )
 
         elif "path" in input_params:
-            self.path = absolute_path(
-                path=input_params["path"], base_dir=input_params.get("conf_dir")
-            )
-            try:
-                self._tiledir_metadata_json = read_output_metadata(
-                    os.path.join(self.path, "metadata.json")
-                )
-            except FileNotFoundError:
-                raise MapcheteConfigError(f"Cannot find metadata.json in {self.path}")
             # define pyramid
             self.td_pyramid = self._tiledir_metadata_json["pyramid"]
+            self._data_type = driver_metadata(
+                self._tiledir_metadata_json["driver"]["format"]
+            )["data_type"]
+
+        try:
             self.output_data = load_output_writer(
                 dict(
                     self._tiledir_metadata_json["driver"],
                     metatiling=self.td_pyramid.metatiling,
                     pixelbuffer=self.td_pyramid.pixelbuffer,
                     pyramid=self.td_pyramid,
                     grid=self.td_pyramid.grid,
                     path=self.path,
                 ),
                 readonly=True,
             )
-            self._params = dict(
-                path=self.path,
-                grid=self.td_pyramid.grid.to_dict(),
-                metatiling=self.td_pyramid.metatiling,
-                pixelbuffer=self.td_pyramid.pixelbuffer,
-                tile_size=self.td_pyramid.tile_size,
+            self._read_as_tiledir_func = self.output_data._read_as_tiledir
+            self._params.update(
                 extension=self.output_data.file_extension.split(".")[-1],
                 **self._tiledir_metadata_json["driver"],
             )
-            self._read_as_tiledir_func = self.output_data._read_as_tiledir
-            self._data_type = driver_metadata(
-                self._tiledir_metadata_json["driver"]["format"]
-            )["data_type"]
-
+        except FileNotFoundError:
+            self.output_data = None
+            self._read_as_tiledir_func = self._read_as_tiledir_func
+        self._params.update(
+            grid=self.td_pyramid.grid.to_dict(),
+            metatiling=self.td_pyramid.metatiling,
+            pixelbuffer=self.td_pyramid.pixelbuffer,
+            tile_size=self.td_pyramid.tile_size,
+        )
         # validate parameters
         validate_values(
-            self._params, [("path", str), ("grid", (str, dict)), ("extension", str)]
+            self._params,
+            [("path", (str, MPath)), ("grid", (str, dict)), ("extension", str)],
         )
         self._ext = self._params["extension"]
 
         # additional params
         self._bounds = self._params.get("bounds", self.td_pyramid.bounds)
         self._metadata = dict(
             self.METADATA,
             data_type=self._data_type,
-            file_extensions=[self._params["extension"]],
+            file_extensions=[self._ext],
         )
         if self._metadata.get("data_type") == "raster":
             self._params["count"] = self._params.get(
                 "count", self._params.get("bands", None)
             )
             validate_values(self._params, [("dtype", str), ("count", int)])
             self._profile = {
                 "nodata": self._params.get("nodata", 0),
                 "dtype": self._params["dtype"],
                 "count": self._params["count"],
             }
         else:
             self._profile = None
 
+    @cached_property
+    def _tiledir_metadata_json(self):
+        return read_output_metadata(self.path.joinpath("metadata.json"))
+
     def open(self, tile, **kwargs):
         """
         Return InputTile object.
 
         Parameters
         ----------
         tile : ``Tile``
@@ -195,25 +211,18 @@
 
 def _get_tiles_paths(
     basepath=None, ext=None, pyramid=None, bounds=None, zoom=None, exists_check=False
 ):
     return [
         (_tile, _path)
         for _tile, _path in [
-            (
-                t,
-                "%s.%s"
-                % (
-                    os.path.join(*([basepath, str(t.zoom), str(t.row), str(t.col)])),
-                    ext,
-                ),
-            )
+            (t, basepath.joinpath(str(t.zoom), str(t.row), str(t.col)).with_suffix(ext))
             for t in pyramid.tiles_from_bounds(bounds, zoom)
         ]
-        if not exists_check or (exists_check and path_exists(_path))
+        if not exists_check or (exists_check and _path.exists())
     ]
 
 
 class InputTile(base.InputTile):
     """
     Target Tile representation of input data.
 
@@ -425,9 +434,8 @@
                 basepath=self._basepath,
                 ext=self._ext,
                 pyramid=self._td_pyramid,
                 bounds=td_bounds,
                 zoom=zoom,
             )
             logger.debug("%s potential tiles at zoom %s", len(tiles_paths), zoom)
-
         return tiles_paths
```

### Comparing `mapchete-2023.4.1/mapchete/formats/default/vector_file.py` & `mapchete-2023.6.0/mapchete/formats/default/vector_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 """
 Vector file input which can be read by fiona.
 
 Currently limited by extensions .shp and .geojson but could be extended easily.
 """
 
-from cached_property import cached_property
-import fiona
 import logging
-from shapely.geometry import box, Point
+
+from cached_property import cached_property
 from rasterio.crs import CRS
+from shapely.geometry import Point, box
 
 from mapchete.formats import base
+from mapchete.io import fiona_open
 from mapchete.io.vector import (
-    reproject_geometry,
-    read_vector_window,
+    IndexedFeatures,
     convert_vector,
     read_vector,
-    IndexedFeatures,
+    read_vector_window,
+    reproject_geometry,
 )
-from mapchete.io import fs_from_path, absolute_path
-
+from mapchete.path import MPath
 
 logger = logging.getLogger(__name__)
 
 
 METADATA = {
     "driver_name": "vector_file",
     "data_type": "vector",
@@ -74,18 +74,21 @@
             if "abstract" in input_params
             else input_params["path"]
         )
         self._cache_task = f"cache_{self.path}"
         if "abstract" in input_params and "cache" in input_params["abstract"]:
             if isinstance(input_params["abstract"]["cache"], dict):
                 if "path" in input_params["abstract"]["cache"]:
-                    self._cached_path = absolute_path(
-                        path=input_params["abstract"]["cache"]["path"],
-                        base_dir=input_params["conf_dir"],
-                    )
+                    cached_path = MPath.from_dict(input_params["abstract"]["cache"])
+                    if cached_path.is_absolute():
+                        self._cached_path = cached_path
+                    else:  # pragma: no cover
+                        self._cached_path = cached_path.absolute_path(
+                            base_dir=input_params["conf_dir"],
+                        )
                 else:  # pragma: no cover
                     raise ValueError("please provide a cache path")
                 # add preprocessing task to cache data
                 self.add_preprocessing_task(
                     convert_vector,
                     key=f"cache_{self.path}",
                     fkwargs=dict(
@@ -168,33 +171,33 @@
         Returns
         -------
         bounding box : geometry
             Shapely geometry object
         """
         out_crs = self.pyramid.crs if out_crs is None else out_crs
         if self._bbox_cache is None:
-            with fiona.open(self.path) as inp:
-                self._bbox_cache = CRS(inp.crs), tuple(inp.bounds) if len(inp) else None
+            with fiona_open(self.path) as inp:
+                self._bbox_cache = (
+                    CRS(inp.crs),
+                    tuple(inp.bounds) if len(inp) else None,
+                )
         inp_crs, bounds = self._bbox_cache
         if bounds is None:
             # this creates an empty GeometryCollection object
             return Point()
         # TODO find a way to get a good segmentize value in bbox source CRS
         return reproject_geometry(
             box(*bounds), src_crs=inp_crs, dst_crs=out_crs, clip_to_crs_bounds=False
         )
 
     def cleanup(self):
         """Cleanup when mapchete closes."""
-        if self._cached_path and not self._cache_keep:
+        if self._cached_path and not self._cache_keep:  # pragma: no cover
             logger.debug("remove cached file %s", self._cached_path)
-            try:
-                fs_from_path(self._cached_path).rm(self._cached_path)
-            except FileNotFoundError:
-                pass
+            self._cached_path.rm(ignore_errors=True)
 
 
 class InputTile(base.InputTile):
     """
     Target Tile representation of input data.
 
     Parameters
```

### Comparing `mapchete-2023.4.1/mapchete/io/_geometry_operations.py` & `mapchete-2023.6.0/mapchete/io/_geometry_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-import fiona
-from fiona.transform import transform_geom
 import logging
+
+import fiona
 import pyproj
+from fiona.transform import transform_geom
 from rasterio.crs import CRS
 from shapely.errors import TopologicalError
 from shapely.geometry import (
-    box,
     GeometryCollection,
-    shape,
-    mapping,
-    MultiPoint,
+    LinearRing,
+    LineString,
     MultiLineString,
+    MultiPoint,
     MultiPolygon,
     Polygon,
-    LinearRing,
-    LineString,
     base,
+    box,
+    mapping,
+    shape,
 )
 from shapely.validation import explain_validity
 
 from mapchete.errors import GeometryTypeError, ReprojectionFailed
 from mapchete.validate import validate_crs
 
 logger = logging.getLogger(__name__)
```

### Comparing `mapchete-2023.4.1/mapchete/io/_misc.py` & `mapchete-2023.6.0/mapchete/io/_misc.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,42 +1,21 @@
 import logging
-import os
+
 import rasterio
 from rasterio.warp import calculate_default_transform
 from shapely.errors import TopologicalError
 from shapely.geometry import box
 
 from mapchete.io._geometry_operations import reproject_geometry, segmentize_geometry
+from mapchete.path import MPath
 from mapchete.tile import BufferedTilePyramid
 
-
 logger = logging.getLogger(__name__)
 
 
-GDAL_HTTP_OPTS = dict(
-    GDAL_DISABLE_READDIR_ON_OPEN=os.environ.get(
-        "GDAL_DISABLE_READDIR_ON_OPEN", "TRUE"
-    ).upper()
-    == "TRUE",
-    CPL_VSIL_CURL_ALLOWED_EXTENSIONS=".tif, .ovr, .jp2, .png, .xml, .rpc",
-    GDAL_HTTP_TIMEOUT=int(os.environ.get("GDAL_HTTP_TIMEOUT", "30")),
-    GDAL_HTTP_MAX_RETRY=int(os.environ.get("GDAL_HTTP_MAX_RETRY", "3")),
-    GDAL_HTTP_MERGE_CONSECUTIVE_RANGES=os.environ.get(
-        "GDAL_HTTP_MERGE_CONSECUTIVE_RANGES", "TRUE"
-    ).upper()
-    == "TRUE",
-    GDAL_HTTP_RETRY_DELAY=int(os.environ.get("GDAL_HTTP_RETRY_DELAY", "5")),
-)
-MAPCHETE_IO_RETRY_SETTINGS = {
-    "tries": int(os.environ.get("MAPCHETE_IO_RETRY_TRIES", "3")),
-    "delay": float(os.environ.get("MAPCHETE_IO_RETRY_DELAY", "1")),
-    "backoff": float(os.environ.get("MAPCHETE_IO_RETRY_BACKOFF", "1")),
-}
-
-
 def get_best_zoom_level(input_file, tile_pyramid_type):
     """
     Determine the best base zoom level for a raster.
 
     "Best" means the maximum zoom level where no oversampling has to be done.
 
     Parameters
@@ -191,34 +170,25 @@
 
 
 def get_boto3_bucket(bucket_name):  # pragma: no cover
     """Return boto3.Bucket object from bucket name."""
     raise DeprecationWarning("get_boto3_bucket() is deprecated")
 
 
-def get_gdal_options(opts, is_remote=False, allowed_remote_extensions=[]):
-    """
-    Return a merged set of custom and default GDAL/rasterio Env options.
-
-    If is_remote is set to True, the default GDAL_HTTP_OPTS are appended.
-
-    Parameters
-    ----------
-    opts : dict or None
-        Explicit GDAL options.
-    is_remote : bool
-        Indicate whether Env is for a remote file.
-
-    Returns
-    -------
-    dictionary
-    """
-    user_opts = {} if opts is None else dict(**opts)
-    if is_remote:
-        gdal_opts = dict(GDAL_HTTP_OPTS)
-        if allowed_remote_extensions:
-            gdal_opts.update(CPL_VSIL_CURL_ALLOWED_EXTENSIONS=allowed_remote_extensions)
-        gdal_opts.update(user_opts)
+def copy(src_path, dst_path, src_fs=None, dst_fs=None, overwrite=False):
+    """Copy path from one place to the other."""
+    src_path = MPath(src_path, fs=src_fs)
+    dst_path = MPath(dst_path, fs=dst_fs)
+
+    if not overwrite and dst_path.fs.exists(dst_path):
+        raise IOError(f"{dst_path} already exists")
+
+    # create parent directories on local filesystems
+    dst_path.makedirs()
+
+    # copy either within a filesystem or between filesystems
+    if src_path.fs == dst_path.fs:
+        src_path.fs.copy(str(src_path), str(dst_path))
     else:
-        gdal_opts = user_opts
-    logger.debug("using GDAL options: %s", gdal_opts)
-    return gdal_opts
+        with src_path.open("rb") as src:
+            with dst_path.open("wb") as dst:
+                dst.write(src.read())
```

### Comparing `mapchete-2023.4.1/mapchete/io/raster.py` & `mapchete-2023.6.0/mapchete/io/raster.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,49 +1,109 @@
 """Wrapper functions around rasterio and useful raster functions."""
 
-from affine import Affine
 import itertools
 import logging
+import warnings
+from contextlib import contextmanager
+from tempfile import NamedTemporaryFile
+from types import GeneratorType
+from typing import List, Tuple, Union
+
 import numpy as np
 import numpy.ma as ma
-import os
-from retry import retry
 import rasterio
+from affine import Affine
 from rasterio.enums import Resampling
 from rasterio.errors import RasterioIOError
 from rasterio.io import MemoryFile
 from rasterio.transform import from_bounds as affine_from_bounds
 from rasterio.vrt import WarpedVRT
 from rasterio.warp import reproject
 from rasterio.windows import from_bounds
+from retry import retry
 from shapely.geometry import box, mapping
-from tempfile import NamedTemporaryFile
-from tilematrix import clip_geometry_to_srs_bounds, Shape, Bounds
-from types import GeneratorType
-from typing import List, Tuple, Union
-import warnings
+from tilematrix import Bounds, Shape, clip_geometry_to_srs_bounds
 
+from mapchete._timer import Timer
 from mapchete.errors import MapcheteIOError
-from mapchete.io import (
-    path_is_remote,
-    get_gdal_options,
-    path_exists,
-    fs_from_path,
-    copy,
-    makedirs,
-)
-from mapchete.io._misc import MAPCHETE_IO_RETRY_SETTINGS
+from mapchete.io import copy
+from mapchete.io.settings import MAPCHETE_IO_RETRY_SETTINGS
+from mapchete.path import MPath, fs_from_path
 from mapchete.tile import BufferedTile
-from mapchete._timer import Timer
 from mapchete.validate import validate_write_window_params
 
-
 logger = logging.getLogger(__name__)
 
 
+@contextmanager
+def rasterio_open(path, mode="r", **kwargs):
+    """Call rasterio.open but set environment correctly and return custom writer if needed."""
+    path = MPath(path)
+
+    if "w" in mode:
+        with rasterio_write(path, mode=mode, **kwargs) as dst:
+            yield dst
+
+    else:
+        with rasterio_read(path, mode=mode, **kwargs) as src:
+            yield src
+
+
+@contextmanager
+def rasterio_read(path, mode="r", **kwargs):
+    """
+    Wrapper around rasterio.open but rasterio.Env is set according to path properties.
+    """
+    with path.rio_env() as env:
+        logger.debug("reading %s with GDAL options %s", str(path), env.options)
+        with rasterio.open(path, mode=mode, **kwargs) as src:
+            yield src
+
+
+@contextmanager
+def rasterio_write(path, mode="w", fs=None, in_memory=True, *args, **kwargs):
+    """
+    Wrap rasterio.open() but handle bucket upload if path is remote.
+
+    Parameters
+    ----------
+    path : str
+        Path to write to.
+    mode : str
+        One of the rasterio.open() modes.
+    fs : fsspec.FileSystem
+        Target filesystem.
+    in_memory : bool
+        On remote output store an in-memory file instead of writing to a tempfile.
+    args : list
+        Arguments to be passed on to rasterio.open()
+    kwargs : dict
+        Keyword arguments to be passed on to rasterio.open()
+
+    Returns
+    -------
+    RasterioRemoteWriter if target is remote, otherwise return rasterio.open().
+    """
+    if path.is_remote():
+        if "s3" in path.protocols:  # pragma: no cover
+            try:
+                import boto3
+            except ImportError:
+                raise ImportError("please install [s3] extra to write remote files")
+        with RasterioRemoteWriter(
+            path, fs=fs, in_memory=in_memory, *args, **kwargs
+        ) as dst:
+            yield dst
+    else:
+        with path.rio_env() as env:
+            logger.debug("reading %s with GDAL options %s", str(path), env.options)
+            with rasterio.open(path, mode=mode, *args, **kwargs) as dst:
+                yield dst
+
+
 class ReferencedRaster:
     """
     A loose in-memory representation of a rasterio dataset.
 
     Useful to ship cached raster files between worker nodes.
     """
 
@@ -140,15 +200,15 @@
             transform=src.transform,
             bounds=src.bounds,
             crs=src.crs,
         )
 
     @staticmethod
     def from_file(path, masked: bool = True) -> "ReferencedRaster":
-        with rasterio.open(path) as src:
+        with rasterio_open(path) as src:
             return ReferencedRaster.from_rasterio(src, masked=masked)
 
 
 def read_raster_window(
     input_files,
     tile,
     indexes=None,
@@ -187,23 +247,24 @@
     gdal_opts : dict
         GDAL options passed on to rasterio.Env()
 
     Returns
     -------
     raster : MaskedArray
     """
-    input_files = input_files if isinstance(input_files, list) else [input_files]
+    input_files = [
+        MPath(input_file)
+        for input_file in (
+            input_files if isinstance(input_files, list) else [input_files]
+        )
+    ]
     if len(input_files) == 0:  # pragma: no cover
         raise ValueError("no input given")
     try:
-        with rasterio.Env(
-            **get_gdal_options(
-                gdal_opts, is_remote=path_is_remote(input_files[0], s3=True)
-            )
-        ) as env:
+        with input_files[0].rio_env(gdal_opts) as env:
             logger.debug(
                 "reading %s file(s) with GDAL options %s", len(input_files), env.options
             )
             return _read_raster_window(
                 input_files,
                 tile,
                 indexes=indexes,
@@ -212,14 +273,15 @@
                 dst_nodata=dst_nodata,
                 dst_dtype=dst_dtype,
                 skip_missing_files=skip_missing_files,
             )
     except FileNotFoundError:  # pragma: no cover
         raise
     except Exception as e:  # pragma: no cover
+        logger.exception(e)
         raise MapcheteIOError(e)
 
 
 def _read_raster_window(
     input_files,
     tile,
     indexes=None,
@@ -477,15 +539,15 @@
                         out_shape=dst_shape,
                         indexes=indexes,
                         masked=True,
                     )
 
     try:
         with Timer() as t:
-            with rasterio.open(input_file, "r") as src:
+            with rasterio_open(input_file, "r") as src:
                 logger.debug("read from %s...", input_file)
                 out = _read(
                     src,
                     indexes,
                     dst_bounds,
                     dst_shape,
                     dst_crs,
@@ -522,26 +584,16 @@
     """
 
     @retry(logger=logger, exceptions=RasterioIOError, **MAPCHETE_IO_RETRY_SETTINGS)
     def _read():
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             try:
-                with rasterio.Env(
-                    **get_gdal_options(
-                        gdal_opts,
-                        is_remote=path_is_remote(input_file, s3=True),
-                        allowed_remote_extensions=os.path.splitext(input_file)[1],
-                    ),
-                ) as env:
-                    logger.debug(
-                        "reading %s with GDAL options %s", input_file, env.options
-                    )
-                    with rasterio.open(input_file, "r") as src:
-                        return src.read(indexes=indexes, masked=True)
+                with rasterio_open(input_file, "r") as src:
+                    return src.read(indexes=indexes, masked=True)
             except RasterioIOError as rio_exc:
                 _extract_filenotfound_exception(rio_exc, input_file)
 
     try:
         return _read()
     except Exception as exc:
         if isinstance(exc, FileNotFoundError):
@@ -550,27 +602,29 @@
             raise MapcheteIOError(exc)
 
 
 def _extract_filenotfound_exception(rio_exc, path):
     """
     Extracts and raises FileNotFoundError from RasterioIOError if applicable.
     """
-    filenotfound_msg = f"{path} not found and cannot be opened with rasterio"
+    filenotfound_msg = (
+        f"{str(path)} not found and cannot be opened with rasterio: {str(rio_exc)}"
+    )
     # rasterio errors which indicate file does not exist
     for i in (
         "does not exist in the file system",
         "No such file or directory",
         "The specified key does not exist",
     ):
         if i in str(rio_exc):
             raise FileNotFoundError(filenotfound_msg)
     else:
         try:
             # NOTE: this can cause addional S3 requests
-            exists = path_exists(path)
+            exists = path.exists()
         except Exception:  # pragma: no cover
             # in order not to mask the original rasterio exception, raise it as is
             raise rio_exc
         if exists:
             # raise original rasterio exception
             raise rio_exc
         else:  # pragma: no cover
@@ -632,15 +686,15 @@
         metadata dictionary for rasterio
     out_tile : ``Tile``
         provides output boundaries; if None, in_tile is used
     out_path : string
         output path to write to
     tags : optional tags to be added to GeoTIFF file
     """
-    if not isinstance(out_path, str):
+    if not isinstance(out_path, (str, MPath)):
         raise TypeError("out_path must be a string")
     logger.debug("write %s", out_path)
     if out_path == "memoryfile":
         raise DeprecationWarning(
             "Writing to memoryfile with write_raster_window() is deprecated. "
             "Please use RasterWindowMemoryFile."
         )
@@ -658,17 +712,16 @@
 
     # use transform instead of affine
     if "affine" in out_profile:
         out_profile["transform"] = out_profile.pop("affine")
 
     # write if there is any band with non-masked data
     if write_empty or (window_data.all() is not ma.masked):
-
         try:
-            with rasterio_write(out_path, "w", fs=fs, **out_profile) as dst:
+            with rasterio_open(out_path, "w", fs=fs, **out_profile) as dst:
                 logger.debug((out_tile.id, "write tile", out_path))
                 dst.write(window_data.astype(out_profile["dtype"], copy=False))
                 _write_tags(dst, tags)
         except Exception as e:
             logger.exception("error while writing file %s: %s", out_path, e)
             raise
     else:
@@ -682,47 +735,14 @@
             if isinstance(k, int):
                 dst.update_tags(k, **v)
             # for filewide tags
             else:
                 dst.update_tags(**{k: v})
 
 
-def rasterio_write(path, mode=None, fs=None, in_memory=True, *args, **kwargs):
-    """
-    Wrap rasterio.open() but handle bucket upload if path is remote.
-
-    Parameters
-    ----------
-    path : str
-        Path to write to.
-    mode : str
-        One of the rasterio.open() modes.
-    fs : fsspec.FileSystem
-        Target filesystem.
-    in_memory : bool
-        On remote output store an in-memory file instead of writing to a tempfile.
-    args : list
-        Arguments to be passed on to rasterio.open()
-    kwargs : dict
-        Keyword arguments to be passed on to rasterio.open()
-
-    Returns
-    -------
-    RasterioRemoteWriter if target is remote, otherwise return rasterio.open().
-    """
-    if path.startswith("s3://"):
-        try:  # pragma: no cover
-            import boto3
-        except ImportError:  # pragma: no cover
-            raise ImportError("please install [s3] extra to write remote files")
-        return RasterioRemoteWriter(path, fs=fs, in_memory=in_memory, *args, **kwargs)
-    else:
-        return rasterio.open(path, mode=mode, *args, **kwargs)
-
-
 class RasterioRemoteMemoryWriter:
     def __init__(self, path, *args, fs=None, **kwargs):
         logger.debug("open RasterioRemoteMemoryWriter for path %s", path)
         self.path = path
         self.fs = fs
         self._dst = MemoryFile()
         self._open_args = args
@@ -746,15 +766,15 @@
 
 
 class RasterioRemoteTempFileWriter:
     def __init__(self, path, *args, fs=None, **kwargs):
         logger.debug("open RasterioTempFileWriter for path %s", path)
         self.path = path
         self.fs = fs
-        self._dst = NamedTemporaryFile(suffix=".tif")
+        self._dst = NamedTemporaryFile(suffix=self.path.suffix)
         self._open_args = args
         self._open_kwargs = kwargs
         self._sink = None
 
     def __enter__(self):
         self._sink = rasterio.open(
             self._dst.name, "w+", *self._open_args, **self._open_kwargs
@@ -1247,34 +1267,38 @@
     overwrite : bool
         Overwrite output file. (default: False)
     skip_exists : bool
         Skip conversion if outpu already exists. (default: True)
     kwargs : mapping
         Creation parameters passed on to output file.
     """
-    if path_exists(out):
+    inp = MPath(inp)
+    out = MPath(out)
+    if out.exists():
         if not exists_ok:
-            raise OSError(f"{out} already exists")
+            raise OSError(f"{str(out)} already exists")
         elif not overwrite:
             logger.debug("output %s already exists and will not be overwritten")
             return
     kwargs = kwargs or {}
     if kwargs:
         logger.debug("convert raster file %s to %s using %s", inp, out, kwargs)
-        with rasterio.open(inp, "r") as src:
-            makedirs(os.path.dirname(out))
-            with rasterio_write(out, mode="w", **{**src.meta, **kwargs}) as dst:
+        with rasterio_open(inp, "r") as src:
+            out.makedirs()
+            with rasterio_open(out, mode="w", **{**src.meta, **kwargs}) as dst:
                 dst.write(src.read())
     else:
-        logger.debug("copy %s to %s", inp, out)
+        logger.debug("copy %s to %s", inp, (out))
+        out.makedirs()
         copy(inp, out, overwrite=overwrite)
 
 
 def read_raster(inp, **kwargs):
-    logger.debug("reading {inp} into memory")
-    with rasterio.open(inp, "r") as src:
+    inp = MPath(inp)
+    logger.debug(f"reading {str(inp)} into memory")
+    with rasterio_open(inp, "r") as src:
         return ReferencedRaster(
             data=src.read(masked=True),
             affine=src.transform,
             bounds=src.bounds,
             crs=src.crs,
         )
```

### Comparing `mapchete-2023.4.1/mapchete/io/vector.py` & `mapchete-2023.6.0/mapchete/io/vector.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,116 @@
 """Functions handling vector data."""
 
-from contextlib import ExitStack
-import os
 import logging
+import warnings
+from contextlib import ExitStack, contextmanager
+from itertools import chain
+from tempfile import NamedTemporaryFile
+
 import fiona
 from fiona.errors import DriverError, FionaError, FionaValueError
 from fiona.io import MemoryFile
-from retry import retry
 from rasterio.crs import CRS
-from shapely.geometry import base, box, mapping
+from retry import retry
 from shapely.errors import TopologicalError
+from shapely.geometry import base, box, mapping
 from tilematrix import clip_geometry_to_srs_bounds
-from itertools import chain
-import warnings
 
-from mapchete.errors import NoGeoError, MapcheteIOError
-from mapchete.io._misc import MAPCHETE_IO_RETRY_SETTINGS
-from mapchete.io._path import fs_from_path, path_exists, makedirs, copy
+from mapchete.errors import MapcheteIOError, NoGeoError
+from mapchete.io import copy
 from mapchete.io._geometry_operations import (
+    _repair,
+    clean_geometry_type,
+    multipart_to_singleparts,
     reproject_geometry,
     segmentize_geometry,
     to_shape,
-    multipart_to_singleparts,
-    clean_geometry_type,
-    _repair,
 )
+from mapchete.io.settings import MAPCHETE_IO_RETRY_SETTINGS
+from mapchete.path import MPath, fs_from_path, path_exists
 from mapchete.types import Bounds
 from mapchete.validate import validate_bounds
 
 __all__ = [
     "reproject_geometry",
     "segmentize_geometry",
     "to_shape",
     "multipart_to_singleparts",
     "clean_geometry_type",
 ]
 
 logger = logging.getLogger(__name__)
 
 
+@contextmanager
+def fiona_open(path, mode="r", **kwargs):
+    """Call fiona.open but set environment correctly and return custom writer if needed."""
+    path = MPath(path)
+
+    if "w" in mode:
+        with fiona_write(path, mode=mode, **kwargs) as dst:
+            yield dst
+
+    else:
+        with fiona_read(path, mode=mode, **kwargs) as src:
+            yield src
+
+
+@contextmanager
+def fiona_read(path, mode="r", **kwargs):
+    """
+    Wrapper around fiona.open but fiona.Env is set according to path properties.
+    """
+    with path.fio_env() as env:
+        logger.debug("reading %s with GDAL options %s", str(path), env.options)
+        with fiona.open(str(path), mode=mode, **kwargs) as src:
+            yield src
+
+
+@contextmanager
+def fiona_write(path, mode="w", fs=None, in_memory=True, *args, **kwargs):
+    """
+    Wrap fiona.open() but handle bucket upload if path is remote.
+
+    Parameters
+    ----------
+    path : str or MPath
+        Path to write to.
+    mode : str
+        One of the fiona.open() modes.
+    fs : fsspec.FileSystem
+        Target filesystem.
+    in_memory : bool
+        On remote output store an in-memory file instead of writing to a tempfile.
+    args : list
+        Arguments to be passed on to fiona.open()
+    kwargs : dict
+        Keyword arguments to be passed on to fiona.open()
+
+    Returns
+    -------
+    FionaRemoteWriter if target is remote, otherwise return fiona.open().
+    """
+    path = MPath(path)
+    if path.is_remote():
+        if "s3" in path.protocols:  # pragma: no cover
+            try:
+                import boto3
+            except ImportError:
+                raise ImportError("please install [s3] extra to write remote files")
+        with FionaRemoteWriter(
+            path, fs=fs, in_memory=in_memory, *args, **kwargs
+        ) as dst:
+            yield dst
+    else:
+        with path.fio_env():
+            with fiona.open(str(path), mode=mode, *args, **kwargs) as dst:
+                yield dst
+
+
 def read_vector_window(
     inp, tile, validity_check=True, clip_to_crs_bounds=False, skip_missing_files=False
 ):
     """
     Read a window of an input vector dataset.
 
     Also clips geometry.
@@ -141,19 +209,16 @@
         output schema for fiona
     out_tile : ``BufferedTile``
         tile used for output extent
     out_path : string
         output path for file
     """
     # Delete existing file.
-    try:
-        os.remove(out_path)
-    except OSError:
-        pass
-
+    out_path = MPath(out_path)
+    out_path.rm(ignore_errors=True)
     out_features = []
     for feature in in_data:
         try:
             # clip feature geometry to tile bounding box and append for writing
             clipped = clean_geometry_type(
                 to_shape(feature["geometry"]).intersection(out_tile.bbox),
                 out_schema["geometry"],
@@ -181,21 +246,18 @@
                 with VectorWindowMemoryFile(
                     tile=out_tile,
                     features=out_features,
                     schema=out_schema,
                     driver=out_driver,
                 ) as memfile:
                     logger.debug((out_tile.id, "write tile", out_path))
-                    with fs_from_path(out_path).open(out_path, "wb") as dst:
+                    with out_path.open("wb") as dst:
                         dst.write(memfile)
             else:  # pragma: no cover
-                # write data to local file
-                # this part is not covered by tests as we now try to let fiona directly
-                # write to S3
-                with fiona.open(
+                with fiona_open(
                     out_path,
                     "w",
                     schema=out_schema,
                     driver=out_driver,
                     crs=out_tile.crs.to_dict(),
                 ) as dst:
                     logger.debug((out_tile.id, "write tile", out_path))
@@ -257,17 +319,17 @@
     dst_bounds=None,
     dst_crs=None,
     validity_check=False,
     clip_to_crs_bounds=False,
 ):
     logger.debug("reading %s", inp)
     with ExitStack() as exit_stack:
-        if isinstance(inp, str):
+        if isinstance(inp, (str, MPath)):
             try:
-                src = exit_stack.enter_context(fiona.open(inp, "r"))
+                src = exit_stack.enter_context(fiona_open(inp, "r"))
                 src_crs = CRS(src.crs)
             except Exception as e:
                 # fiona errors which indicate file does not exist
                 for i in (
                     "does not exist in the file system",
                     "No such file or directory",
                     "The specified key does not exist",
@@ -301,15 +363,14 @@
             dst_bbox = reproject_geometry(
                 box(*dst_bounds),
                 src_crs=dst_crs,
                 dst_crs=src_crs,
                 validity_check=True,
             )
         for feature in src.filter(bbox=dst_bbox.bounds):
-
             try:
                 # check validity
                 original_geom = _repair(to_shape(feature["geometry"]))
 
                 # clip with bounds and omit if clipped geometry is empty
                 clipped_geom = original_geom.intersection(dst_bbox)
 
@@ -523,30 +584,92 @@
     overwrite : bool
         Overwrite output file. (default: False)
     skip_exists : bool
         Skip conversion if outpu already exists. (default: True)
     kwargs : mapping
         Creation parameters passed on to output file.
     """
-    if path_exists(out):
+    inp = MPath(inp)
+    out = MPath(out)
+    if out.exists():
         if not exists_ok:
             raise IOError(f"{out} already exists")
         elif not overwrite:
             logger.debug("output %s already exists and will not be overwritten")
             return
         else:
             fs_from_path(out).rm(out)
     kwargs = kwargs or {}
     if kwargs:
-        logger.debug("convert raster file %s to %s using %s", inp, out, kwargs)
-        with fiona.open(inp, "r") as src:
-            makedirs(os.path.dirname(out))
-            with fiona.open(out, mode="w", **{**src.meta, **kwargs}) as dst:
+        logger.debug("convert vector file %s to %s using %s", str(inp), out, kwargs)
+        with fiona_open(inp, "r") as src:
+            out.makedirs()
+            with fiona_open(out, mode="w", **{**src.meta, **kwargs}) as dst:
                 dst.writerecords(src)
     else:
-        logger.debug("copy %s to %s", inp, out)
+        logger.debug("copy %s to %s", str(inp), str(out))
+        out.makedirs()
         copy(inp, out, overwrite=overwrite)
 
 
 def read_vector(inp, index="rtree"):
-    with fiona.open(inp, "r") as src:
+    with fiona_open(inp, "r") as src:
         return IndexedFeatures(src, index=index)
+
+
+class FionaRemoteMemoryWriter:
+    def __init__(self, path, *args, **kwargs):
+        logger.debug("open FionaRemoteMemoryWriter for path %s", path)
+        self.path = path
+        self._dst = MemoryFile()
+        self._open_args = args
+        self._open_kwargs = kwargs
+        self._sink = None
+
+    def __enter__(self):
+        self._sink = self._dst.open(*self._open_args, **self._open_kwargs)
+        return self._sink
+
+    def __exit__(self, exc_type, exc_value, exc_traceback):
+        try:
+            self._sink.close()
+            if exc_value is None:
+                logger.debug("upload fiona MemoryFile to %s", self.path)
+                with self.path.open("wb") as dst:
+                    dst.write(self._dst.getbuffer())
+        finally:
+            logger.debug("close fiona MemoryFile")
+            self._dst.close()
+
+
+class FionaRemoteTempFileWriter:
+    def __init__(self, path, *args, **kwargs):
+        logger.debug("open FionaRemoteTempFileWriter for path %s", path)
+        self.path = path
+        self._dst = NamedTemporaryFile(suffix=self.path.suffix)
+        self._open_args = args
+        self._open_kwargs = kwargs
+        self._sink = None
+
+    def __enter__(self):
+        self._sink = fiona.open(
+            self._dst.name, "w", *self._open_args, **self._open_kwargs
+        )
+        return self._sink
+
+    def __exit__(self, exc_type, exc_value, exc_traceback):
+        try:
+            self._sink.close()
+            if exc_value is None:
+                logger.debug("upload TempFile %s to %s", self._dst.name, self.path)
+                self.path.fs.put_file(self._dst.name, self.path)
+        finally:
+            logger.debug("close and remove tempfile")
+            self._dst.close()
+
+
+class FionaRemoteWriter:
+    def __new__(self, path, *args, in_memory=True, **kwargs):
+        if in_memory:
+            return FionaRemoteMemoryWriter(path, *args, **kwargs)
+        else:
+            return FionaRemoteTempFileWriter(path, *args, **kwargs)
```

### Comparing `mapchete-2023.4.1/mapchete/processes/__init__.py` & `mapchete-2023.6.0/mapchete/processes/__init__.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.4.1/mapchete/processes/contours.py` & `mapchete-2023.6.0/mapchete/processes/contours.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+
 from shapely.geometry import mapping, shape
 from shapely.ops import unary_union
 
 logger = logging.getLogger(__name__)
 
 
 def execute(
```

### Comparing `mapchete-2023.4.1/mapchete/processes/convert.py` & `mapchete-2023.6.0/mapchete/processes/convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
+import warnings
+
 import numpy as np
 from rasterio.dtypes import dtype_ranges
-import warnings
 
 logger = logging.getLogger(__name__)
 
 
 def execute(
     mp,
     resampling="nearest",
```

### Comparing `mapchete-2023.4.1/mapchete/processes/hillshade.py` & `mapchete-2023.6.0/mapchete/processes/hillshade.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.4.1/mapchete/processes/examples/example_process.py` & `mapchete-2023.6.0/mapchete/processes/examples/example_process.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.4.1/mapchete/static/index.html` & `mapchete-2023.6.0/mapchete/static/index.html`

 * *Files 14% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         padding: 0px;
     }
     .olImageLoadError {
         /* when OL encounters a 404, don't display the pink image */
         display: none !important;
     }
     </style>
-    <script src="http://www.openlayers.org/api/OpenLayers.js"></script>
+    <script src="https://www.openlayers.org/api/OpenLayers.js"></script>
     <script type="text/javascript">
         function extend(a, b){
             for(var key in b)
                 if(b.hasOwnProperty(key))
                     a[key] = b[key];
             return a;
         }
@@ -61,104 +61,134 @@
                 units: "dd",
                 projection: new OpenLayers.Projection("EPSG:{{srid}}".toUpperCase()),
                 wrapDateLine: true
             }
 
             // Terrain light
             var options = extend(defaults, {
-                url: "http://tiles.maps.eox.at/wmts/",
+                url: "https://s2maps-tiles.eu/wmts/",
                 name: "EOX::Maps Terrain Light",
                 {% if is_mercator %}
                 layer: 'terrain-light_3857',
                 {% else %}
                 layer: 'terrain-light',
                 {% endif %}
                 format: 'image/jpeg',
-                isBaseLayer:true,
+                isBaseLayer: true,
             });
             var terrain_light_wmts_layer = new OpenLayers.Layer.WMTS(options);
             map.addLayer(terrain_light_wmts_layer);
 
+            // Sentinel-2 Cloudless 2021
+            var options = extend(defaults, {
+                url: "https://s2maps-tiles.eu/wmts/",
+                name: "Sentinel-2 Cloudless 2021",
+                {% if is_mercator %}
+                layer: 's2cloudless-2021_3857',
+                {% else %}
+                layer: 's2cloudless-2021',
+                {% endif %}
+                format: 'image/jpeg',
+                isBaseLayer: true,
+            });
+            var s2cloudless2021_wmts_layer = new OpenLayers.Layer.WMTS(options);
+            map.addLayer(s2cloudless2021_wmts_layer);
+
+            // Sentinel-2 Cloudless 2020
+            var options = extend(defaults, {
+                url: "https://s2maps-tiles.eu/wmts/",
+                name: "Sentinel-2 Cloudless 2020",
+                {% if is_mercator %}
+                layer: 's2cloudless-2020_3857',
+                {% else %}
+                layer: 's2cloudless-2020',
+                {% endif %}
+                format: 'image/jpeg',
+                isBaseLayer: true,
+            });
+            var s2cloudless2020_wmts_layer = new OpenLayers.Layer.WMTS(options);
+            map.addLayer(s2cloudless2020_wmts_layer);
+
             // Sentinel-2 Cloudless 2019
             var options = extend(defaults, {
-                url: "http://tiles.maps.eox.at/wmts/",
+                url: "https://s2maps-tiles.eu/wmts/",
                 name: "Sentinel-2 Cloudless 2019",
                 {% if is_mercator %}
                 layer: 's2cloudless-2019_3857',
                 {% else %}
                 layer: 's2cloudless-2019',
                 {% endif %}
                 format: 'image/jpeg',
-                isBaseLayer:true,
+                isBaseLayer: true,
             });
             var s2cloudless2019_wmts_layer = new OpenLayers.Layer.WMTS(options);
             map.addLayer(s2cloudless2019_wmts_layer);
 
             // Sentinel-2 Cloudless 2018
             var options = extend(defaults, {
-                url: "http://tiles.maps.eox.at/wmts/",
+                url: "https://s2maps-tiles.eu/wmts/",
                 name: "Sentinel-2 Cloudless 2018",
                 {% if is_mercator %}
                 layer: 's2cloudless-2018_3857',
                 {% else %}
                 layer: 's2cloudless-2018',
                 {% endif %}
                 format: 'image/jpeg',
-                isBaseLayer:true,
+                isBaseLayer: true,
             });
             var s2cloudless2018_wmts_layer = new OpenLayers.Layer.WMTS(options);
             map.addLayer(s2cloudless2018_wmts_layer);
 
             // OSM
             var options = extend(defaults, {
-                url: "http://tiles.maps.eox.at/wmts/",
+                url: "https://s2maps-tiles.eu/wmts/",
                 name: "OpenStreetMap",
                 {% if is_mercator %}
                 layer: 'osm_3857',
                 {% else %}
                 layer: 'osm',
                 {% endif %}
                 format: 'image/jpeg',
-                isBaseLayer:true,
+                isBaseLayer: true,
             });
             var osm_wmts_layer = new OpenLayers.Layer.WMTS(options);
             map.addLayer(osm_wmts_layer);
 
             // Coastline
             var options = extend(defaults, {
-                url: "http://tiles.maps.eox.at/wmts/",
+                url: "https://s2maps-tiles.eu/wmts/",
                 name: "EOX::Maps Coastline",
                 {% if is_mercator %}
                 layer: 'coastline_3857',
                 {% else %}
                 layer: 'coastline',
                 {% endif %}
                 format: 'image/png',
-                isBaseLayer:true,
+                isBaseLayer: true,
             });
             var coastline_wmts_layer = new OpenLayers.Layer.WMTS(options);
             map.addLayer(coastline_wmts_layer);
 
             // processes
             {% for process_name in process_names -%}
                 var options = extend(defaults, {
                     url: "/wmts_simple",
                     name: "{{process_name}}",
                     layer: "{{process_name}}",
                     format: 'image/png',
                     requestEncoding: 'REST',
-                    isBaseLayer:false,
+                    isBaseLayer: false,
                 });
                 var {{process_name}}_layer = new OpenLayers.Layer.WMTS(options);
                 map.addLayer({{process_name}}_layer);
                 {%- endfor %}
 
             // Overlay
             var options = extend(defaults, {
-                url: "http://tiles.maps.eox.at/wmts/",
+                url: "https://s2maps-tiles.eu/wmts/",
                 name: "EOX::Maps Base Overlay",
                 {% if is_mercator %}
                 layer: 'overlay_base_3857',
                 {% else %}
                 layer: 'overlay_base',
                 {% endif %}
                 format: 'image/png',
```

### Comparing `mapchete-2023.4.1/mapchete/static/process_template.py` & `mapchete-2023.6.0/mapchete/static/process_template.py`

 * *Files identical despite different names*

### Comparing `mapchete-2023.4.1/LICENSE` & `mapchete-2023.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mapchete-2023.4.1/README.rst` & `mapchete-2023.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `mapchete-2023.4.1/pyproject.toml` & `mapchete-2023.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,16 @@
 [project.optional-dependencies]
 complete = [
     "aiohttp",
     "aiobotocore>=1.1.2",
     "boto3>=1.14.44",
     "dask",
     "distributed",
-    "flask",
+    "Flask",
+    "Flask-RangeRequest",
     "fsspec[http]",
     "fsspec[s3]",
     "geobuf",
     "lxml",
     "matplotlib",
     "protobuf<=3.20.1",
     "pystac",
@@ -78,15 +79,16 @@
 ]
 s3 = [
     "aiobotocore>=1.1.2",
     "boto3>=1.14.44",
     "fsspec[s3]",
 ]
 serve = [
-    "flask",
+    "Flask",
+    "Flask-RangeRequest",
     "werkzeug>=0.15",
 ]
 spatial-index = [
     "rtree",
 ]
 stac = [
     "pystac",
```

### Comparing `mapchete-2023.4.1/PKG-INFO` & `mapchete-2023.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapchete
-Version: 2023.4.1
+Version: 2023.6.0
 Summary: Tile-based geodata processing using rasterio & Fiona
 Project-URL: Homepage, https://github.com/ungarj/mapchete
 Author-email: Joachim Ungar <joachim.ungar@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -34,14 +34,15 @@
 Provides-Extra: complete
 Requires-Dist: aiobotocore>=1.1.2; extra == 'complete'
 Requires-Dist: aiohttp; extra == 'complete'
 Requires-Dist: boto3>=1.14.44; extra == 'complete'
 Requires-Dist: dask; extra == 'complete'
 Requires-Dist: distributed; extra == 'complete'
 Requires-Dist: flask; extra == 'complete'
+Requires-Dist: flask-rangerequest; extra == 'complete'
 Requires-Dist: fsspec[http]; extra == 'complete'
 Requires-Dist: fsspec[s3]; extra == 'complete'
 Requires-Dist: geobuf; extra == 'complete'
 Requires-Dist: lxml; extra == 'complete'
 Requires-Dist: matplotlib; extra == 'complete'
 Requires-Dist: protobuf<=3.20.1; extra == 'complete'
 Requires-Dist: pystac; extra == 'complete'
@@ -62,14 +63,15 @@
 Requires-Dist: requests; extra == 'http'
 Provides-Extra: s3
 Requires-Dist: aiobotocore>=1.1.2; extra == 's3'
 Requires-Dist: boto3>=1.14.44; extra == 's3'
 Requires-Dist: fsspec[s3]; extra == 's3'
 Provides-Extra: serve
 Requires-Dist: flask; extra == 'serve'
+Requires-Dist: flask-rangerequest; extra == 'serve'
 Requires-Dist: werkzeug>=0.15; extra == 'serve'
 Provides-Extra: spatial-index
 Requires-Dist: rtree; extra == 'spatial-index'
 Provides-Extra: stac
 Requires-Dist: pystac; extra == 'stac'
 Provides-Extra: vrt
 Requires-Dist: lxml; extra == 'vrt'
```

