# Comparing `tmp/hvplot-0.8.3rc2.tar.gz` & `tmp/hvplot-0.8.4a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hvplot-0.8.3rc2.tar", last modified: Fri Mar 17 07:28:11 2023, max compression
+gzip compressed data, was "dist/hvplot-0.8.4a1.tar", last modified: Mon Jun  5 17:06:56 2023, max compression
```

## Comparing `hvplot-0.8.3rc2.tar` & `hvplot-0.8.4a1.tar`

### file list

```diff
@@ -1,203 +1,203 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 07:28:11.000000 hvplot-0.8.3rc2/
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11124 2023-03-17 07:28:11.000000 hvplot-0.8.3rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 07:28:11.000000 hvplot-0.8.3rc2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 07:28:11.000000 hvplot-0.8.3rc2/examples/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   359182 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/assets/console.png
--rw-r--r--   0 runner    (1001) docker     (123)  1080507 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/assets/console_server.gif
--rw-r--r--   0 runner    (1001) docker     (123)   160622 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/assets/diagram.png
--rw-r--r--   0 runner    (1001) docker     (123)   633920 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/assets/diagram.svg
--rw-r--r--   0 runner    (1001) docker     (123)    16120 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/assets/hvplot-wm.png
--rw-r--r--   0 runner    (1001) docker     (123)  1007817 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/assets/streamz_demo.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 07:28:11.000000 hvplot-0.8.3rc2/examples/data/
--rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/data/crime.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/datasets.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 07:28:11.000000 hvplot-0.8.3rc2/examples/getting_started/
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/getting_started/explorer.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    10052 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/getting_started/hvplot.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/getting_started/interactive.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 07:28:11.000000 hvplot-0.8.3rc2/examples/reference/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 07:28:11.000000 hvplot-0.8.3rc2/examples/reference/geopandas/
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/reference/geopandas/points.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/reference/geopandas/polygons.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 07:28:11.000000 hvplot-0.8.3rc2/examples/reference/pandas/
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/reference/pandas/andrewscurves.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/reference/pandas/area.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6473 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/reference/pandas/bar.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/reference/pandas/barh.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/reference/pandas/bivariate.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/reference/pandas/box.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/reference/pandas/errorbars.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/reference/pandas/heatmap.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/reference/pandas/hexbin.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/reference/pandas/hist.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/reference/pandas/kde.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/reference/pandas/labels.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/reference/pandas/lagplot.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/reference/pandas/line.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/reference/pandas/ohlc.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/reference/pandas/parallelcoordinates.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/reference/pandas/scatter.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/reference/pandas/scattermatrix.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/reference/pandas/step.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/reference/pandas/table.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/reference/pandas/violin.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 07:28:11.000000 hvplot-0.8.3rc2/examples/reference/xarray/
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/reference/xarray/contour.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/reference/xarray/contourf.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/reference/xarray/image.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/reference/xarray/quadmesh.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/reference/xarray/rgb.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/reference/xarray/vectorfield.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 07:28:11.000000 hvplot-0.8.3rc2/examples/user_guide/
--rw-r--r--   0 runner    (1001) docker     (123)    11280 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/user_guide/Customization.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/user_guide/Explorer.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11740 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/user_guide/Geographic_Data.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8635 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/user_guide/Gridded_Data.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    13494 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/user_guide/Interactive.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/user_guide/Introduction.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    25828 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/user_guide/NetworkX.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    31612 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/user_guide/Pandas_API.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    22061 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/user_guide/Plotting.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/user_guide/Plotting_Extensions.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    23435 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/user_guide/Plotting_with_Matplotlib.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    23004 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/user_guide/Plotting_with_Plotly.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/user_guide/Statistical_Plots.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/user_guide/Streaming.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/user_guide/Subplots.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/user_guide/Timeseries_Data.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/user_guide/Viewing.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/user_guide/Widgets.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 07:28:11.000000 hvplot-0.8.3rc2/examples/user_guide/images/
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/examples/user_guide/images/simple.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 07:28:11.000000 hvplot-0.8.3rc2/hvplot/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-17 07:28:11.000000 hvplot-0.8.3rc2/hvplot/.version
--rw-r--r--   0 runner    (1001) docker     (123)     9441 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10844 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/backend_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    97201 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/cudf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/dask.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 07:28:11.000000 hvplot-0.8.3rc2/hvplot/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 07:28:11.000000 hvplot-0.8.3rc2/hvplot/examples/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   359182 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/assets/console.png
--rw-r--r--   0 runner    (1001) docker     (123)  1080507 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/assets/console_server.gif
--rw-r--r--   0 runner    (1001) docker     (123)   160622 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/assets/diagram.png
--rw-r--r--   0 runner    (1001) docker     (123)   633920 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/assets/diagram.svg
--rw-r--r--   0 runner    (1001) docker     (123)    16120 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/assets/hvplot-wm.png
--rw-r--r--   0 runner    (1001) docker     (123)  1007817 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/assets/streamz_demo.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 07:28:11.000000 hvplot-0.8.3rc2/hvplot/examples/data/
--rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/data/crime.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/datasets.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 07:28:11.000000 hvplot-0.8.3rc2/hvplot/examples/getting_started/
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/getting_started/explorer.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    10052 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/getting_started/hvplot.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/getting_started/interactive.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 07:28:11.000000 hvplot-0.8.3rc2/hvplot/examples/reference/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 07:28:11.000000 hvplot-0.8.3rc2/hvplot/examples/reference/geopandas/
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/reference/geopandas/points.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/reference/geopandas/polygons.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 07:28:11.000000 hvplot-0.8.3rc2/hvplot/examples/reference/pandas/
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/reference/pandas/andrewscurves.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/reference/pandas/area.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6473 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/reference/pandas/bar.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/reference/pandas/barh.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/reference/pandas/bivariate.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/reference/pandas/box.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/reference/pandas/errorbars.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/reference/pandas/heatmap.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/reference/pandas/hexbin.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/reference/pandas/hist.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/reference/pandas/kde.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/reference/pandas/labels.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/reference/pandas/lagplot.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/reference/pandas/line.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/reference/pandas/ohlc.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/reference/pandas/parallelcoordinates.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/reference/pandas/scatter.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/reference/pandas/scattermatrix.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/reference/pandas/step.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/reference/pandas/table.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/reference/pandas/violin.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 07:28:11.000000 hvplot-0.8.3rc2/hvplot/examples/reference/xarray/
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/reference/xarray/contour.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/reference/xarray/contourf.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/reference/xarray/image.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/reference/xarray/quadmesh.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/reference/xarray/rgb.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/reference/xarray/vectorfield.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 07:28:11.000000 hvplot-0.8.3rc2/hvplot/examples/user_guide/
--rw-r--r--   0 runner    (1001) docker     (123)    11280 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/user_guide/Customization.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/user_guide/Explorer.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11740 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/user_guide/Geographic_Data.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8635 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/user_guide/Gridded_Data.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    13494 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/user_guide/Interactive.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/user_guide/Introduction.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    25828 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/user_guide/NetworkX.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    31612 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/user_guide/Pandas_API.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    22061 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/user_guide/Plotting.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/user_guide/Plotting_Extensions.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    23435 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/user_guide/Plotting_with_Matplotlib.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    23004 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/user_guide/Plotting_with_Plotly.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/user_guide/Statistical_Plots.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/user_guide/Streaming.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/user_guide/Subplots.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/user_guide/Timeseries_Data.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/user_guide/Viewing.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/user_guide/Widgets.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 07:28:11.000000 hvplot-0.8.3rc2/hvplot/examples/user_guide/images/
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/examples/user_guide/images/simple.svg
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/ibis.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/intake.py
--rw-r--r--   0 runner    (1001) docker     (123)    34864 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)    21358 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/networkx.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 07:28:11.000000 hvplot-0.8.3rc2/hvplot/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/plotting/andrews_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)    77095 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/plotting/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/plotting/lag_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/plotting/parallel_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     8739 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/plotting/scatter_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/sample_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/streamz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 07:28:11.000000 hvplot-0.8.3rc2/hvplot/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 07:28:11.000000 hvplot-0.8.3rc2/hvplot/tests/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/tests/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/tests/plotting/testcore.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/tests/plotting/testscattermatrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/tests/test_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/tests/testbackend_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    17267 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/tests/testcharts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/tests/testgeo.py
--rw-r--r--   0 runner    (1001) docker     (123)    11575 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/tests/testgridplots.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/tests/testhelp.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/tests/testibis.py
--rw-r--r--   0 runner    (1001) docker     (123)    40872 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/tests/testinteractive.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/tests/testnetworkx.py
--rw-r--r--   0 runner    (1001) docker     (123)    10934 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/tests/testoperations.py
--rw-r--r--   0 runner    (1001) docker     (123)    22822 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/tests/testoptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/tests/testoverrides.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/tests/testpanel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/tests/testpatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/tests/testplotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/tests/teststreaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/tests/testtransforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/tests/testui.py
--rw-r--r--   0 runner    (1001) docker     (123)     9789 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/tests/testutil.py
--rw-r--r--   0 runner    (1001) docker     (123)    23363 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)    17520 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/hvplot/xarray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 07:28:11.000000 hvplot-0.8.3rc2/hvplot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11124 2023-03-17 07:28:11.000000 hvplot-0.8.3rc2/hvplot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-03-17 07:28:11.000000 hvplot-0.8.3rc2/hvplot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 07:28:11.000000 hvplot-0.8.3rc2/hvplot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-17 07:28:11.000000 hvplot-0.8.3rc2/hvplot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-03-17 07:28:11.000000 hvplot-0.8.3rc2/hvplot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-17 07:28:11.000000 hvplot-0.8.3rc2/hvplot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-17 07:28:11.000000 hvplot-0.8.3rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-03-17 07:20:37.000000 hvplot-0.8.3rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11123 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/examples/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   359182 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/assets/console.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1080507 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/assets/console_server.gif
+-rw-r--r--   0 runner    (1001) docker     (123)   160622 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/assets/diagram.png
+-rw-r--r--   0 runner    (1001) docker     (123)   633920 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/assets/diagram.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    16120 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/assets/hvplot-wm.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1007817 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/assets/streamz_demo.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/data/crime.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/datasets.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/examples/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/getting_started/explorer.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10052 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/getting_started/hvplot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/getting_started/interactive.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/examples/reference/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/examples/reference/geopandas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/geopandas/points.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/geopandas/polygons.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/examples/reference/pandas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/pandas/andrewscurves.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/pandas/area.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6473 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/pandas/bar.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/pandas/barh.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/pandas/bivariate.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/pandas/box.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/pandas/errorbars.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/pandas/heatmap.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/pandas/hexbin.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/pandas/hist.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/pandas/kde.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/pandas/labels.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/pandas/lagplot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/pandas/line.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/pandas/ohlc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/pandas/parallelcoordinates.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/pandas/scatter.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/pandas/scattermatrix.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/pandas/step.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/pandas/table.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/pandas/violin.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/examples/reference/xarray/
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/xarray/contour.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/xarray/contourf.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/xarray/image.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/xarray/quadmesh.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/xarray/rgb.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/xarray/vectorfield.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/examples/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)    11280 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/user_guide/Customization.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/user_guide/Explorer.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11740 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/user_guide/Geographic_Data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8635 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/user_guide/Gridded_Data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    13494 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/user_guide/Interactive.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/user_guide/Introduction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    25828 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/user_guide/NetworkX.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    31612 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/user_guide/Pandas_API.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    22061 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/user_guide/Plotting.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/user_guide/Plotting_Extensions.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    23435 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/user_guide/Plotting_with_Matplotlib.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    23004 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/user_guide/Plotting_with_Plotly.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/user_guide/Statistical_Plots.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/user_guide/Streaming.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/user_guide/Subplots.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/user_guide/Timeseries_Data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/user_guide/Viewing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/user_guide/Widgets.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/examples/user_guide/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/user_guide/images/simple.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/hvplot/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/hvplot/.version
+-rw-r--r--   0 runner    (1001) docker     (123)     9441 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10844 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/backend_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98207 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/cudf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/dask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/hvplot/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/hvplot/examples/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   359182 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/assets/console.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1080507 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/assets/console_server.gif
+-rw-r--r--   0 runner    (1001) docker     (123)   160622 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/assets/diagram.png
+-rw-r--r--   0 runner    (1001) docker     (123)   633920 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/assets/diagram.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    16120 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/assets/hvplot-wm.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1007817 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/assets/streamz_demo.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/hvplot/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/data/crime.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/datasets.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/hvplot/examples/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/getting_started/explorer.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10052 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/getting_started/hvplot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/getting_started/interactive.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/hvplot/examples/reference/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/hvplot/examples/reference/geopandas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/geopandas/points.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/geopandas/polygons.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/hvplot/examples/reference/pandas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/pandas/andrewscurves.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/pandas/area.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6473 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/pandas/bar.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/pandas/barh.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/pandas/bivariate.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/pandas/box.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/pandas/errorbars.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/pandas/heatmap.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/pandas/hexbin.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/pandas/hist.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/pandas/kde.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/pandas/labels.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/pandas/lagplot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/pandas/line.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/pandas/ohlc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/pandas/parallelcoordinates.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/pandas/scatter.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/pandas/scattermatrix.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/pandas/step.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/pandas/table.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/pandas/violin.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/hvplot/examples/reference/xarray/
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/xarray/contour.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/xarray/contourf.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/xarray/image.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/xarray/quadmesh.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/xarray/rgb.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/xarray/vectorfield.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/hvplot/examples/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)    11280 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/user_guide/Customization.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/user_guide/Explorer.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11740 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/user_guide/Geographic_Data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8635 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/user_guide/Gridded_Data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    13494 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/user_guide/Interactive.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/user_guide/Introduction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    25828 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/user_guide/NetworkX.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    31612 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/user_guide/Pandas_API.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    22061 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/user_guide/Plotting.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/user_guide/Plotting_Extensions.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    23435 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/user_guide/Plotting_with_Matplotlib.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    23004 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/user_guide/Plotting_with_Plotly.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/user_guide/Statistical_Plots.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/user_guide/Streaming.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/user_guide/Subplots.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/user_guide/Timeseries_Data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/user_guide/Viewing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/user_guide/Widgets.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/hvplot/examples/user_guide/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/user_guide/images/simple.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/ibis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/intake.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36819 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21358 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/networkx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/hvplot/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/plotting/andrews_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77101 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/plotting/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/plotting/lag_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/plotting/parallel_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8739 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/plotting/scatter_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/streamz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/hvplot/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/hvplot/tests/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/tests/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/tests/plotting/testcore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/tests/plotting/testscattermatrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/tests/test_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/tests/testbackend_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17267 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/tests/testcharts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11812 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/tests/testgeo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11575 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/tests/testgridplots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/tests/testhelp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/tests/testibis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41686 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/tests/testinteractive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/tests/testnetworkx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10934 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/tests/testoperations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22822 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/tests/testoptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/tests/testoverrides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/tests/testpanel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/tests/testpatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/tests/testplotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/tests/teststreaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/tests/testtransforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/tests/testui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9789 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/tests/testutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23363 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17806 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/xarray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/hvplot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11123 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/hvplot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/hvplot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/hvplot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/hvplot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/hvplot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/hvplot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5137 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/setup.py
```

### Comparing `hvplot-0.8.3rc2/LICENSE` & `hvplot-0.8.4a1/LICENSE`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/PKG-INFO` & `hvplot-0.8.4a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hvplot
-Version: 0.8.3rc2
+Version: 0.8.4a1
 Summary: A high-level plotting API for the PyData ecosystem built on HoloViews.
 Home-page: https://hvplot.pyviz.org
 Author: Philipp Rudiger
 Author-email: developers@pyviz.org
 Maintainer: HoloViz developers
 Maintainer-email: developers@pyviz.org
 License: BSD
```

### Comparing `hvplot-0.8.3rc2/README.md` & `hvplot-0.8.4a1/README.md`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/assets/console.png` & `hvplot-0.8.4a1/examples/assets/console.png`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/assets/console_server.gif` & `hvplot-0.8.4a1/examples/assets/console_server.gif`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/assets/diagram.png` & `hvplot-0.8.4a1/examples/assets/diagram.png`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/assets/diagram.svg` & `hvplot-0.8.4a1/examples/assets/diagram.svg`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/assets/hvplot-wm.png` & `hvplot-0.8.4a1/examples/assets/hvplot-wm.png`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/assets/streamz_demo.gif` & `hvplot-0.8.4a1/examples/assets/streamz_demo.gif`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/data/crime.csv` & `hvplot-0.8.4a1/examples/data/crime.csv`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/datasets.yaml` & `hvplot-0.8.4a1/examples/datasets.yaml`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/getting_started/explorer.ipynb` & `hvplot-0.8.4a1/examples/getting_started/explorer.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/getting_started/hvplot.ipynb` & `hvplot-0.8.4a1/examples/getting_started/hvplot.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/getting_started/interactive.ipynb` & `hvplot-0.8.4a1/examples/getting_started/interactive.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/reference/geopandas/points.ipynb` & `hvplot-0.8.4a1/examples/reference/geopandas/points.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/reference/geopandas/polygons.ipynb` & `hvplot-0.8.4a1/examples/reference/geopandas/polygons.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/reference/pandas/andrewscurves.ipynb` & `hvplot-0.8.4a1/examples/reference/pandas/andrewscurves.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/reference/pandas/area.ipynb` & `hvplot-0.8.4a1/examples/reference/pandas/area.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/reference/pandas/bar.ipynb` & `hvplot-0.8.4a1/examples/reference/pandas/bar.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/reference/pandas/barh.ipynb` & `hvplot-0.8.4a1/examples/reference/pandas/barh.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/reference/pandas/bivariate.ipynb` & `hvplot-0.8.4a1/examples/reference/pandas/bivariate.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/reference/pandas/box.ipynb` & `hvplot-0.8.4a1/examples/reference/pandas/box.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/reference/pandas/errorbars.ipynb` & `hvplot-0.8.4a1/examples/reference/pandas/errorbars.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/reference/pandas/heatmap.ipynb` & `hvplot-0.8.4a1/examples/reference/pandas/heatmap.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/reference/pandas/hexbin.ipynb` & `hvplot-0.8.4a1/examples/reference/pandas/hexbin.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/reference/pandas/hist.ipynb` & `hvplot-0.8.4a1/examples/reference/pandas/hist.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/reference/pandas/kde.ipynb` & `hvplot-0.8.4a1/examples/reference/pandas/kde.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/reference/pandas/labels.ipynb` & `hvplot-0.8.4a1/examples/reference/pandas/labels.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/reference/pandas/lagplot.ipynb` & `hvplot-0.8.4a1/examples/reference/pandas/lagplot.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/reference/pandas/line.ipynb` & `hvplot-0.8.4a1/examples/reference/pandas/line.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/reference/pandas/ohlc.ipynb` & `hvplot-0.8.4a1/examples/reference/pandas/ohlc.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/reference/pandas/parallelcoordinates.ipynb` & `hvplot-0.8.4a1/examples/reference/pandas/parallelcoordinates.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/reference/pandas/scatter.ipynb` & `hvplot-0.8.4a1/examples/reference/pandas/scatter.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/reference/pandas/scattermatrix.ipynb` & `hvplot-0.8.4a1/examples/reference/pandas/scattermatrix.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/reference/pandas/step.ipynb` & `hvplot-0.8.4a1/examples/reference/pandas/step.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/reference/pandas/table.ipynb` & `hvplot-0.8.4a1/examples/reference/pandas/table.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/reference/pandas/violin.ipynb` & `hvplot-0.8.4a1/examples/reference/pandas/violin.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/reference/xarray/contour.ipynb` & `hvplot-0.8.4a1/examples/reference/xarray/contour.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/reference/xarray/contourf.ipynb` & `hvplot-0.8.4a1/examples/reference/xarray/contourf.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/reference/xarray/image.ipynb` & `hvplot-0.8.4a1/examples/reference/xarray/image.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/reference/xarray/quadmesh.ipynb` & `hvplot-0.8.4a1/examples/reference/xarray/quadmesh.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/reference/xarray/rgb.ipynb` & `hvplot-0.8.4a1/examples/reference/xarray/rgb.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/reference/xarray/vectorfield.ipynb` & `hvplot-0.8.4a1/examples/reference/xarray/vectorfield.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/user_guide/Customization.ipynb` & `hvplot-0.8.4a1/examples/user_guide/Customization.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/user_guide/Explorer.ipynb` & `hvplot-0.8.4a1/examples/user_guide/Explorer.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/user_guide/Geographic_Data.ipynb` & `hvplot-0.8.4a1/examples/user_guide/Geographic_Data.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/user_guide/Gridded_Data.ipynb` & `hvplot-0.8.4a1/examples/user_guide/Gridded_Data.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/user_guide/Interactive.ipynb` & `hvplot-0.8.4a1/examples/user_guide/Interactive.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/user_guide/Introduction.ipynb` & `hvplot-0.8.4a1/examples/user_guide/Introduction.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/user_guide/NetworkX.ipynb` & `hvplot-0.8.4a1/examples/user_guide/NetworkX.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/user_guide/Pandas_API.ipynb` & `hvplot-0.8.4a1/examples/user_guide/Pandas_API.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/user_guide/Plotting.ipynb` & `hvplot-0.8.4a1/examples/user_guide/Plotting.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/user_guide/Plotting_Extensions.ipynb` & `hvplot-0.8.4a1/examples/user_guide/Plotting_Extensions.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/user_guide/Plotting_with_Matplotlib.ipynb` & `hvplot-0.8.4a1/examples/user_guide/Plotting_with_Matplotlib.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/user_guide/Plotting_with_Plotly.ipynb` & `hvplot-0.8.4a1/examples/user_guide/Plotting_with_Plotly.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/user_guide/Statistical_Plots.ipynb` & `hvplot-0.8.4a1/examples/user_guide/Statistical_Plots.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/user_guide/Streaming.ipynb` & `hvplot-0.8.4a1/examples/user_guide/Streaming.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/user_guide/Subplots.ipynb` & `hvplot-0.8.4a1/examples/user_guide/Subplots.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/user_guide/Timeseries_Data.ipynb` & `hvplot-0.8.4a1/examples/user_guide/Timeseries_Data.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/user_guide/Viewing.ipynb` & `hvplot-0.8.4a1/examples/user_guide/Viewing.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/user_guide/Widgets.ipynb` & `hvplot-0.8.4a1/examples/user_guide/Widgets.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/examples/user_guide/images/simple.svg` & `hvplot-0.8.4a1/examples/user_guide/images/simple.svg`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/__init__.py` & `hvplot-0.8.4a1/hvplot/__init__.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/backend_transforms.py` & `hvplot-0.8.4a1/hvplot/backend_transforms.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/converter.py` & `hvplot-0.8.4a1/hvplot/converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -226,14 +226,17 @@
         PlateCarree, i.e. lat/lon coordinates).
     global_extent (default=False):
         Whether to expand the plot extent to span the whole globe.
     project (default=False):
         Whether to project the data before plotting (adds initial
         overhead but avoids projecting data when plot is dynamically
         updated).
+    projection (default=None): str or Cartopy CRS
+        Coordinate reference system of the plot specified as Cartopy
+        CRS object or class name.
     tiles (default=False):
         Whether to overlay the plot on a tile source. Tiles sources
         can be selected by name or a tiles object or class can be passed,
         the default is 'Wikipedia'.
     """
 
     _gridded_types = [
@@ -251,15 +254,16 @@
     _data_options = [
         'x', 'y', 'kind', 'by', 'use_index', 'use_dask', 'dynamic',
         'crs', 'value_label', 'group_label', 'backlog', 'persist',
         'sort_date'
     ]
 
     _geo_options = [
-        'geo', 'crs', 'features', 'project', 'coastline', 'tiles'
+        'geo', 'crs', 'features', 'project', 'coastline', 'tiles',
+        'projection', 'global_extents'
     ]
 
     _axis_options = [
         'width', 'height', 'shared_axes', 'grid', 'legend',
         'rot', 'xlim', 'ylim', 'xticks', 'yticks', 'colorbar',
         'invert', 'title', 'logx', 'logy', 'loglog', 'xaxis',
         'yaxis', 'xformatter', 'yformatter', 'xlabel', 'ylabel',
@@ -389,15 +393,15 @@
         self._process_data(
             kind, data, x, y, by, groupby, row, col, use_dask,
             persist, backlog, label, group_label, value_label,
             hover_cols, attr_labels, transforms, stream, kwds
         )
 
         self.dynamic = dynamic
-        self.geo = any([geo, crs, global_extent, projection, project, coastline, features])
+        self.geo = any([geo, crs, global_extent, projection, project, coastline, features, tiles])
         self.crs = self._process_crs(data, crs) if self.geo else None
         self.project = project
         self.coastline = coastline
         self.features = features
         self.tiles = tiles
         self.sort_date = sort_date
 
@@ -408,15 +412,15 @@
             except ImportError:
                 raise ImportError('In order to use geo-related features '
                                   'the geoviews library must be available. '
                                   'It can be installed with:\n  conda '
                                   'install -c pyviz geoviews')
         if self.geo:
             if self.kind not in self._geo_types:
-                param.main.warning(
+                param.main.param.warning(
                     "geo option cannot be used with kind=%r plot "
                     "type. Geographic plots are only supported for "
                     "following plot types: %r" % (self.kind, self._geo_types))
             from cartopy import crs as ccrs
             from geoviews.util import project_extents
 
             if isinstance(projection, str):
@@ -430,21 +434,28 @@
                 elif projection == 'GOOGLE_MERCATOR':
                     projection = getattr(ccrs, projection)
                 else:
                     raise ValueError(
                         "Projection must be defined as cartopy CRS or "
                         "one of the following CRS string:\n {}".format(all_crs))
 
-            proj_crs = projection or ccrs.GOOGLE_MERCATOR
-            if self.crs != proj_crs:
+            projection = projection or (ccrs.GOOGLE_MERCATOR if tiles else self.crs)
+            if tiles and projection != ccrs.GOOGLE_MERCATOR:
+                raise ValueError(
+                    "Tiles can only be used with output projection of "
+                    "`cartopy.crs.GOOGLE_MERCATOR`. To get rid of this error "
+                    "remove `projection=` or `tiles=`"
+                )
+
+            if self.crs != projection:
                 px0, py0, px1, py1 = ccrs.GOOGLE_MERCATOR.boundary.bounds
                 x0, x1 = xlim or (px0, px1)
                 y0, y1 = ylim or (py0, py1)
                 extents = (x0, y0, x1, y1)
-                x0, y0, x1, y1 = project_extents(extents, self.crs, proj_crs)
+                x0, y0, x1, y1 = project_extents(extents, self.crs, projection)
                 if xlim:
                     xlim = (x0, x1)
                 if ylim:
                     ylim = (y0, y1)
 
         # Operations
         self.datashade = datashade
@@ -602,15 +613,15 @@
         self._dim_ranges = {'c': clim or (None, None)}
 
         # High-level options
         self._validate_kwds(kwds)
         if debug:
             kwds = dict(x=self.x, y=self.y, by=self.by, kind=self.kind,
                         groupby=self.groupby, grid=self.grid)
-            param.main.warning('Plotting {kind} plot with parameters x: {x}, '
+            param.main.param.warning('Plotting {kind} plot with parameters x: {x}, '
                                'y: {y}, by: {by}, groupby: {groupby}, row/col: {grid}'.format(**kwds))
 
     def _process_symmetric(self, symmetric, clim, check_symmetric_max):
         if symmetric is not None or clim is not None:
             return symmetric
 
         if is_xarray(self.data):
@@ -702,14 +713,18 @@
                 geom_type = list(geom_types)[0]
                 if geom_type == 'Point':
                     kind = 'points'
                 elif geom_type == 'Polygon':
                     kind = 'polygons'
                 elif geom_type in ('LineString', 'LineRing', 'Line'):
                     kind = 'paths'
+            # if only one arg is provided, treat it like color
+            if x is not None and y is None:
+                kwds['color'] = kwds.pop('color', kwds.pop('c', x))
+                x = None
         elif isinstance(data, pd.DataFrame):
             datatype = 'pandas'
             self.data = data
         elif is_dask(data):
             datatype = 'dask'
             self.data = data.persist() if persist else data
         elif is_cudf(data):
@@ -2228,17 +2243,20 @@
         if self.gridded_data:
             vdims = Dataset(data).vdims
         element = self._get_element(kind)
         cur_opts, compat_opts = self._get_compat_opts(element.name)
         for opts_ in [cur_opts, compat_opts]:
             if 'color' in opts_ and opts_['color'] in vdims:
                 opts_['color'] = hv.dim(opts_['color'])
+            # if there is nothing to put in hover, turn it off
+            if 'tools' in opts_ and kind in ["polygons", "paths"] and not vdims:
+                opts_["tools"] = [t for t in opts_["tools"] if t != "hover"]
         if self.geo: params['crs'] = self.crs
         if self.by:
-            obj = Dataset(data).to(element, kdims, vdims, self.by, **params)
+            obj = Dataset(data, self.by+kdims, vdims).to(element, kdims, vdims, self.by, **params)
             if self.subplots:
                 obj = obj.layout(sort=False)
             else:
                 obj = obj.overlay(sort=False)
         else:
             obj = element(data, kdims, vdims, **params)
```

### Comparing `hvplot-0.8.3rc2/hvplot/cudf.py` & `hvplot-0.8.4a1/hvplot/cudf.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/dask.py` & `hvplot-0.8.4a1/hvplot/dask.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/assets/console.png` & `hvplot-0.8.4a1/hvplot/examples/assets/console.png`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/assets/console_server.gif` & `hvplot-0.8.4a1/hvplot/examples/assets/console_server.gif`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/assets/diagram.png` & `hvplot-0.8.4a1/hvplot/examples/assets/diagram.png`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/assets/diagram.svg` & `hvplot-0.8.4a1/hvplot/examples/assets/diagram.svg`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/assets/hvplot-wm.png` & `hvplot-0.8.4a1/hvplot/examples/assets/hvplot-wm.png`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/assets/streamz_demo.gif` & `hvplot-0.8.4a1/hvplot/examples/assets/streamz_demo.gif`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/data/crime.csv` & `hvplot-0.8.4a1/hvplot/examples/data/crime.csv`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/datasets.yaml` & `hvplot-0.8.4a1/hvplot/examples/datasets.yaml`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/getting_started/explorer.ipynb` & `hvplot-0.8.4a1/hvplot/examples/getting_started/explorer.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/getting_started/hvplot.ipynb` & `hvplot-0.8.4a1/hvplot/examples/getting_started/hvplot.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/getting_started/interactive.ipynb` & `hvplot-0.8.4a1/hvplot/examples/getting_started/interactive.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/reference/geopandas/points.ipynb` & `hvplot-0.8.4a1/hvplot/examples/reference/geopandas/points.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/reference/geopandas/polygons.ipynb` & `hvplot-0.8.4a1/hvplot/examples/reference/geopandas/polygons.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/reference/pandas/andrewscurves.ipynb` & `hvplot-0.8.4a1/hvplot/examples/reference/pandas/andrewscurves.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/reference/pandas/area.ipynb` & `hvplot-0.8.4a1/hvplot/examples/reference/pandas/area.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/reference/pandas/bar.ipynb` & `hvplot-0.8.4a1/hvplot/examples/reference/pandas/bar.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/reference/pandas/barh.ipynb` & `hvplot-0.8.4a1/hvplot/examples/reference/pandas/barh.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/reference/pandas/bivariate.ipynb` & `hvplot-0.8.4a1/hvplot/examples/reference/pandas/bivariate.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/reference/pandas/box.ipynb` & `hvplot-0.8.4a1/hvplot/examples/reference/pandas/box.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/reference/pandas/errorbars.ipynb` & `hvplot-0.8.4a1/hvplot/examples/reference/pandas/errorbars.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/reference/pandas/heatmap.ipynb` & `hvplot-0.8.4a1/hvplot/examples/reference/pandas/heatmap.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/reference/pandas/hexbin.ipynb` & `hvplot-0.8.4a1/hvplot/examples/reference/pandas/hexbin.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/reference/pandas/hist.ipynb` & `hvplot-0.8.4a1/hvplot/examples/reference/pandas/hist.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/reference/pandas/kde.ipynb` & `hvplot-0.8.4a1/hvplot/examples/reference/pandas/kde.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/reference/pandas/labels.ipynb` & `hvplot-0.8.4a1/hvplot/examples/reference/pandas/labels.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/reference/pandas/lagplot.ipynb` & `hvplot-0.8.4a1/hvplot/examples/reference/pandas/lagplot.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/reference/pandas/line.ipynb` & `hvplot-0.8.4a1/hvplot/examples/reference/pandas/line.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/reference/pandas/ohlc.ipynb` & `hvplot-0.8.4a1/hvplot/examples/reference/pandas/ohlc.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/reference/pandas/parallelcoordinates.ipynb` & `hvplot-0.8.4a1/hvplot/examples/reference/pandas/parallelcoordinates.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/reference/pandas/scatter.ipynb` & `hvplot-0.8.4a1/hvplot/examples/reference/pandas/scatter.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/reference/pandas/scattermatrix.ipynb` & `hvplot-0.8.4a1/hvplot/examples/reference/pandas/scattermatrix.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/reference/pandas/step.ipynb` & `hvplot-0.8.4a1/hvplot/examples/reference/pandas/step.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/reference/pandas/table.ipynb` & `hvplot-0.8.4a1/hvplot/examples/reference/pandas/table.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/reference/pandas/violin.ipynb` & `hvplot-0.8.4a1/hvplot/examples/reference/pandas/violin.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/reference/xarray/contour.ipynb` & `hvplot-0.8.4a1/hvplot/examples/reference/xarray/contour.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/reference/xarray/contourf.ipynb` & `hvplot-0.8.4a1/hvplot/examples/reference/xarray/contourf.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/reference/xarray/image.ipynb` & `hvplot-0.8.4a1/hvplot/examples/reference/xarray/image.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/reference/xarray/quadmesh.ipynb` & `hvplot-0.8.4a1/hvplot/examples/reference/xarray/quadmesh.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/reference/xarray/rgb.ipynb` & `hvplot-0.8.4a1/hvplot/examples/reference/xarray/rgb.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/reference/xarray/vectorfield.ipynb` & `hvplot-0.8.4a1/hvplot/examples/reference/xarray/vectorfield.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/user_guide/Customization.ipynb` & `hvplot-0.8.4a1/hvplot/examples/user_guide/Customization.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/user_guide/Explorer.ipynb` & `hvplot-0.8.4a1/hvplot/examples/user_guide/Explorer.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/user_guide/Geographic_Data.ipynb` & `hvplot-0.8.4a1/hvplot/examples/user_guide/Geographic_Data.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/user_guide/Gridded_Data.ipynb` & `hvplot-0.8.4a1/hvplot/examples/user_guide/Gridded_Data.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/user_guide/Interactive.ipynb` & `hvplot-0.8.4a1/hvplot/examples/user_guide/Interactive.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/user_guide/Introduction.ipynb` & `hvplot-0.8.4a1/hvplot/examples/user_guide/Introduction.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/user_guide/NetworkX.ipynb` & `hvplot-0.8.4a1/hvplot/examples/user_guide/NetworkX.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/user_guide/Pandas_API.ipynb` & `hvplot-0.8.4a1/hvplot/examples/user_guide/Pandas_API.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/user_guide/Plotting.ipynb` & `hvplot-0.8.4a1/hvplot/examples/user_guide/Plotting.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/user_guide/Plotting_Extensions.ipynb` & `hvplot-0.8.4a1/hvplot/examples/user_guide/Plotting_Extensions.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/user_guide/Plotting_with_Matplotlib.ipynb` & `hvplot-0.8.4a1/hvplot/examples/user_guide/Plotting_with_Matplotlib.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/user_guide/Plotting_with_Plotly.ipynb` & `hvplot-0.8.4a1/hvplot/examples/user_guide/Plotting_with_Plotly.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/user_guide/Statistical_Plots.ipynb` & `hvplot-0.8.4a1/hvplot/examples/user_guide/Statistical_Plots.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/user_guide/Streaming.ipynb` & `hvplot-0.8.4a1/hvplot/examples/user_guide/Streaming.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/user_guide/Subplots.ipynb` & `hvplot-0.8.4a1/hvplot/examples/user_guide/Subplots.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/user_guide/Timeseries_Data.ipynb` & `hvplot-0.8.4a1/hvplot/examples/user_guide/Timeseries_Data.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/user_guide/Viewing.ipynb` & `hvplot-0.8.4a1/hvplot/examples/user_guide/Viewing.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/user_guide/Widgets.ipynb` & `hvplot-0.8.4a1/hvplot/examples/user_guide/Widgets.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/examples/user_guide/images/simple.svg` & `hvplot-0.8.4a1/hvplot/examples/user_guide/images/simple.svg`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/intake.py` & `hvplot-0.8.4a1/hvplot/intake.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/interactive.py` & `hvplot-0.8.4a1/hvplot/interactive.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 
 from panel.layout import Column, Row, VSpacer, HSpacer
 from panel.util import get_method_owner, full_groupby
 from panel.widgets.base import Widget
 
 from .converter import HoloViewsConverter
 from .util import (
-    _flatten, is_tabular, is_xarray, is_xarray_dataarray,
+    _flatten, bokeh3, is_tabular, is_xarray, is_xarray_dataarray,
     _convert_col_names_to_str,
 )
 
 
 def _find_widgets(op):
     widgets = []
     op_args = list(op['args']) + list(op['kwargs'].values())
@@ -705,14 +705,19 @@
 
     def layout(self, **kwargs):
         """
         Returns a layout of the widgets and output arranged according
         to the center and widget location specified in the
         interactive call.
         """
+        if bokeh3:
+            return self._layout_bk3(**kwargs)
+        return self._layout_bk2(**kwargs)
+
+    def _layout_bk2(self, **kwargs):
         widget_box = self.widgets()
         panel = self.output()
         loc = self._loc
         if loc in ('left', 'right'):
             widgets = Column(VSpacer(), widget_box, VSpacer())
         elif loc in ('top', 'bottom'):
             widgets = Row(HSpacer(), widget_box, HSpacer())
@@ -747,14 +752,57 @@
                 components = [panel, widgets]
             elif loc.startswith('top'):
                 components = [Column(widgets, panel)]
             elif loc.startswith('bottom'):
                 components = [Column(panel, widgets)]
         return Row(*components, **kwargs)
 
+    def _layout_bk3(self, **kwargs):
+        widget_box = self.widgets()
+        panel = self.output()
+        loc = self._loc
+        center = self._center
+        alignments = {
+            'left': (Row, ('start', 'center'), True),
+            'right': (Row, ('end', 'center'), False),
+            'top': (Column, ('center', 'start'), True),
+            'bottom': (Column, ('center', 'end'), False),
+            'top_left': (Column, 'start', True),
+            'top_right': (Column, ('end', 'start'), True),
+            'bottom_left': (Column, ('start', 'end'), False),
+            'bottom_right': (Column, 'end', False),
+            'left_top': (Row, 'start', True),
+            'left_bottom': (Row, ('start', 'end'), True),
+            'right_top': (Row, ('end', 'start'), False),
+            'right_bottom': (Row, 'end', False)
+        }
+        layout, align, widget_first = alignments[loc]
+        widget_box.align = align
+        if not len(widget_box):
+            if center:
+                components = [HSpacer(), panel, HSpacer()]
+            else:
+                components = [panel]
+            return Row(*components, **kwargs)
+
+        items = (widget_box, panel) if widget_first else (panel, widget_box)
+        sizing_mode = kwargs.get('sizing_mode')
+        if not center:
+            if layout is Row:
+                components = list(items)
+            else:
+                components = [layout(*items, sizing_mode=sizing_mode)]
+        elif layout is Column:
+            components = [HSpacer(), layout(*items, sizing_mode=sizing_mode), HSpacer()]
+        elif loc.startswith('left'):
+            components = [widget_box, HSpacer(), panel, HSpacer()]
+        else:
+            components = [HSpacer(), panel, HSpacer(), widget_box]
+        return Row(*components, **kwargs)
+
     def holoviews(self):
         """
         Returns a HoloViews object to render the output of this
         pipeline. Only works if the output of this pipeline is a
         HoloViews object, e.g. from an .hvplot call.
         """
         return hv.DynamicMap(self._callback)
```

### Comparing `hvplot-0.8.3rc2/hvplot/networkx.py` & `hvplot-0.8.4a1/hvplot/networkx.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/pandas.py` & `hvplot-0.8.4a1/hvplot/pandas.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/plotting/__init__.py` & `hvplot-0.8.4a1/hvplot/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/plotting/andrews_curves.py` & `hvplot-0.8.4a1/hvplot/plotting/andrews_curves.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/plotting/core.py` & `hvplot-0.8.4a1/hvplot/plotting/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
         """
         Custom getattribute to expose user defined subplots.
         """
         plots = object.__getattribute__(self, "_plots")
         if name in plots:
             plot_opts = plots[name]
             if "kind" in plot_opts and name in HoloViewsConverter._kind_mapping:
-                param.main.warning(
+                param.main.param.warning(
                     "Custom options for existing plot types should not "
                     "declare the 'kind' argument. The .%s plot method "
                     "was unexpectedly customized with kind=%r." % (plot_opts["kind"], name)
                 )
                 plot_opts["kind"] = name
             return hvPlotBase(self._data, **dict(self._metadata, **plot_opts))
         return super().__getattribute__(name)
```

### Comparing `hvplot-0.8.3rc2/hvplot/plotting/lag_plot.py` & `hvplot-0.8.4a1/hvplot/plotting/lag_plot.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/plotting/parallel_coordinates.py` & `hvplot-0.8.4a1/hvplot/plotting/parallel_coordinates.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/plotting/scatter_matrix.py` & `hvplot-0.8.4a1/hvplot/plotting/scatter_matrix.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/sample_data.py` & `hvplot-0.8.4a1/hvplot/sample_data.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/streamz.py` & `hvplot-0.8.4a1/hvplot/streamz.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/tests/plotting/testcore.py` & `hvplot-0.8.4a1/hvplot/tests/plotting/testcore.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/tests/plotting/testscattermatrix.py` & `hvplot-0.8.4a1/hvplot/tests/plotting/testscattermatrix.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/tests/test_links.py` & `hvplot-0.8.4a1/hvplot/tests/test_links.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/tests/testbackend_transforms.py` & `hvplot-0.8.4a1/hvplot/tests/testbackend_transforms.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/tests/testcharts.py` & `hvplot-0.8.4a1/hvplot/tests/testcharts.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/tests/testgeo.py` & `hvplot-0.8.4a1/hvplot/tests/testgeo.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 from unittest import TestCase, SkipTest
 
 from packaging.version import Version
 import numpy as np
 import pandas as pd
 import holoviews as hv
-import pytest
 
 from hvplot.util import proj_to_cartopy
 
 
 class TestGeo(TestCase):
 
     def setUp(self):
@@ -103,14 +102,19 @@
         plot = da.hvplot.image('x', 'y', crs=self.crs, projection='GOOGLE_MERCATOR')
         self.assert_projection(plot, 'merc')
 
     def test_plot_with_projection_as_invalid_string(self):
         with self.assertRaisesRegex(ValueError, "Projection must be defined"):
             self.da.hvplot.image('x', 'y', projection='foo')
 
+    def test_plot_with_projection_raises_an_error_when_tiles_set(self):
+        da = self.da.copy()
+        with self.assertRaisesRegex(ValueError, "Tiles can only be used with output projection"):
+            da.hvplot.image('x', 'y', crs=self.crs, projection='Robinson', tiles=True)
+
 
 class TestGeoAnnotation(TestCase):
 
     def setUp(self):
         try:
             import geoviews  # noqa
             import cartopy.crs as ccrs # noqa
@@ -257,27 +261,44 @@
         assert points.vdims == ['name']
 
     def test_points_hover_cols_index_in_list(self):
         points = self.cities.hvplot(y='y', hover_cols=['index'])
         assert points.kdims == ['x', 'y']
         assert points.vdims == ['index']
 
+    def test_points_hover_cols_positional_arg_sets_color(self):
+        points = self.cities.hvplot('name')
+        assert points.kdims == ['x', 'y']
+        assert points.vdims == ['name']
+        opts = hv.Store.lookup_options('bokeh', points, 'style').kwargs
+        assert opts['color'] == 'name'
+
     def test_points_hover_cols_with_c_set_to_name(self):
         points = self.cities.hvplot(c='name')
         assert points.kdims == ['x', 'y']
         assert points.vdims == ['name']
         opts = hv.Store.lookup_options('bokeh', points, 'style').kwargs
         assert opts['color'] == 'name'
 
-    @pytest.mark.xfail
     def test_points_hover_cols_with_by_set_to_name(self):
         points = self.cities.hvplot(by='name')
-        assert points.kdims == ['x', 'y']
-        assert points.vdims == ['name']
+        assert isinstance(points, hv.core.overlay.NdOverlay)
+        assert points.kdims == ['name']
+        assert points.vdims == []
+        for element in points.values():
+            assert element.kdims == ['x', 'y']
+            assert element.vdims == []
+
+    def test_points_project_xlim_and_ylim(self):
+        points = self.cities.hvplot(geo=True, xlim=(-10, 10), ylim=(-20, -10))
+        opts = hv.Store.lookup_options('bokeh', points, 'plot').options
+        assert opts['xlim'] == (-10, 10)
+        assert opts['ylim'] == (-20, -10)
 
-    @pytest.mark.xfail(
-        reason='Waiting for upstream fix https://github.com/holoviz/holoviews/pull/5325',
-        raises=KeyError,
-    )
     def test_polygons_by_subplots(self):
         polygons = self.polygons.hvplot(geo=True, by="name", subplots=True)
         assert isinstance(polygons, hv.core.layout.NdLayout)
+
+    def test_polygons_turns_off_hover_when_there_are_no_fields_to_include(self):
+        polygons = self.polygons.hvplot(geo=True)
+        opts = hv.Store.lookup_options('bokeh', polygons, 'plot').kwargs
+        assert 'hover' not in opts.get('tools')
```

### Comparing `hvplot-0.8.3rc2/hvplot/tests/testgridplots.py` & `hvplot-0.8.4a1/hvplot/tests/testgridplots.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/tests/testhelp.py` & `hvplot-0.8.4a1/hvplot/tests/testhelp.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/tests/testinteractive.py` & `hvplot-0.8.4a1/hvplot/tests/testinteractive.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 import pytest
 import xarray as xr
 
 from holoviews.util.transform import dim
 from hvplot import bind
 from hvplot.interactive import Interactive
 from hvplot.xarray import XArrayInteractive
+from hvplot.util import bokeh3
+
+is_bokeh2 = pytest.mark.skipif(bokeh3, reason="requires bokeh 2.x")
+is_bokeh3 = pytest.mark.skipif(not bokeh3, reason="requires bokeh 3.x")
 
 
 @pytest.fixture(scope='module')
 def series():
     return pd.Series(np.arange(5.0), name='A')
 
 
@@ -661,15 +665,15 @@
 
     assert isinstance(widgets, pn.Column)
     assert len(widgets) == 1
     assert widgets[0] is select
 
 
 def test_interactive_pandas_frame_bind_operator_out_widgets(df):
-    select = pn.widgets.Select(default='A', options=list(df.columns))
+    select = pn.widgets.Select(value='A', options=list(df.columns))
 
     def sel_col(col):
         return df[col]
 
     dfi = Interactive(bind(sel_col, select))
 
     w = pn.widgets.FloatSlider(value=2., start=1., end=5.)
@@ -1243,14 +1247,15 @@
 
     layout = dfi.layout(width=200)
 
     assert isinstance(layout, pn.Row)
     assert layout.width == 200
 
 
+@is_bokeh2
 def test_interactive_pandas_layout_default_with_widgets(df):
     w = pn.widgets.IntSlider(value=2, start=1, end=5)
     dfi = Interactive(df)
     dfi = dfi.head(w)
 
     assert dfi._center is False
     assert dfi._loc == 'top_left'
@@ -1266,14 +1271,35 @@
     assert len(layout[0][0]) == 2
     assert isinstance(layout[0][0][0], pn.Column)
     assert len(layout[0][0][0]) == 1
     assert isinstance(layout[0][0][0][0], pn.widgets.Widget)
     assert isinstance(layout[0][0][1], pn.layout.HSpacer)
 
 
+@is_bokeh3
+def test_interactive_pandas_layout_default_with_widgets_bk3(df):
+    w = pn.widgets.IntSlider(value=2, start=1, end=5)
+    dfi = Interactive(df)
+    dfi = dfi.head(w)
+
+    assert dfi._center is False
+    assert dfi._loc == 'top_left'
+
+    layout = dfi.layout()
+
+    assert isinstance(layout, pn.Row)
+    assert len(layout) == 1
+    assert isinstance(layout[0], pn.Column)
+    assert len(layout[0]) == 2
+    assert isinstance(layout[0][0], pn.Column)
+    assert isinstance(layout[0][1], pn.pane.PaneBase)
+    assert len(layout[0][0]) == 1
+    assert isinstance(layout[0][0][0], pn.widgets.IntSlider)
+
+@is_bokeh2
 def test_interactive_pandas_layout_center_with_widgets(df):
     w = pn.widgets.IntSlider(value=2, start=1, end=5)
     dfi = df.interactive(center=True)
     dfi = dfi.head(w)
 
     assert dfi._center is True
     assert dfi._loc == 'top_left'
@@ -1294,14 +1320,15 @@
     assert len(layout[1][0][0]) == 1
     assert isinstance(layout[1][0][0][0], pn.widgets.Widget)
     assert isinstance(layout[1][1][0], pn.layout.HSpacer)
     assert isinstance(layout[1][1][1], pn.pane.PaneBase)
     assert isinstance(layout[1][1][2], pn.layout.HSpacer)
 
 
+@is_bokeh2
 def test_interactive_pandas_layout_loc_with_widgets(df):
     w = pn.widgets.IntSlider(value=2, start=1, end=5)
     dfi = df.interactive(loc='top_right')
     dfi = dfi.head(w)
 
     assert dfi._center is False
     assert dfi._loc == 'top_right'
```

### Comparing `hvplot-0.8.3rc2/hvplot/tests/testnetworkx.py` & `hvplot-0.8.4a1/hvplot/tests/testnetworkx.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/tests/testoperations.py` & `hvplot-0.8.4a1/hvplot/tests/testoperations.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/tests/testoptions.py` & `hvplot-0.8.4a1/hvplot/tests/testoptions.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/tests/testoverrides.py` & `hvplot-0.8.4a1/hvplot/tests/testoverrides.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/tests/testpanel.py` & `hvplot-0.8.4a1/hvplot/tests/testpanel.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/tests/testpatch.py` & `hvplot-0.8.4a1/hvplot/tests/testpatch.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/tests/testplotting.py` & `hvplot-0.8.4a1/hvplot/tests/testplotting.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/tests/teststreaming.py` & `hvplot-0.8.4a1/hvplot/tests/teststreaming.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/tests/testtransforms.py` & `hvplot-0.8.4a1/hvplot/tests/testtransforms.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/tests/testui.py` & `hvplot-0.8.4a1/hvplot/tests/testui.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/tests/testutil.py` & `hvplot-0.8.4a1/hvplot/tests/testutil.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/ui.py` & `hvplot-0.8.4a1/hvplot/ui.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/util.py` & `hvplot-0.8.4a1/hvplot/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,25 +6,28 @@
 
 from collections.abc import Hashable
 
 from functools import wraps
 from packaging.version import Version
 from types import FunctionType
 
+import bokeh
 import numpy as np
 import pandas as pd
 import param
 import holoviews as hv
 try:
     import panel as pn
     panel_available = True
 except:
     panel_available = False
 
 hv_version = Version(hv.__version__)
+bokeh_version = Version(bokeh.__version__)
+bokeh3 = bokeh_version >= Version("3.0")
 
 
 def with_hv_extension(func, extension='bokeh', logo=False):
     """If hv.extension is not loaded, load before calling function"""
     @wraps(func)
     def wrapper(*args, **kwargs):
         if extension and not getattr(hv.extension, '_loaded', False):
@@ -224,20 +227,29 @@
     Parses cartopy CRS definitions defined in one of a few formats:
 
       1. EPSG codes:   Defined as string of the form "EPSG: {code}" or an integer
       2. proj.4 string: Defined as string of the form "{proj.4 string}"
       3. cartopy.crs.CRS instance
       4. None defaults to crs.PlateCaree
     """
+    missing = []
     try:
         import cartopy.crs as ccrs
+    except ImportError:
+        missing.append('cartopy')
+    try:
         import geoviews as gv # noqa
+    except ImportError:
+        missing.append('geoviews')
+    try:
         import pyproj
     except ImportError:
-        raise ImportError('Geographic projection support requires geoviews, pyproj and cartopy.')
+        missing.append('pyproj')
+    if missing:
+        raise ImportError(f'Geographic projection support requires: {", ".join(missing)}.')
 
     if crs is None:
         return ccrs.PlateCarree()
 
     errors = []
     if isinstance(crs, str) and crs.lower().startswith('epsg'):
         try:
@@ -316,15 +328,15 @@
 def is_dask(data):
     if not check_library(data, 'dask'):
         return False
     import dask.dataframe as dd
     return isinstance(data, (dd.DataFrame, dd.Series))
 
 def is_intake(data):
-    if not check_library(data, 'intake'):
+    if "intake" not in sys.modules:
         return False
     from intake.source.base import DataSource
     return isinstance(data, DataSource)
 
 def is_ibis(data):
     if not check_library(data, 'ibis'):
         return False
```

### Comparing `hvplot-0.8.3rc2/hvplot/utilities.py` & `hvplot-0.8.4a1/hvplot/utilities.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot/xarray.py` & `hvplot-0.8.4a1/hvplot/xarray.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot.egg-info/PKG-INFO` & `hvplot-0.8.4a1/hvplot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hvplot
-Version: 0.8.3rc2
+Version: 0.8.4a1
 Summary: A high-level plotting API for the PyData ecosystem built on HoloViews.
 Home-page: https://hvplot.pyviz.org
 Author: Philipp Rudiger
 Author-email: developers@pyviz.org
 Maintainer: HoloViz developers
 Maintainer-email: developers@pyviz.org
 License: BSD
```

### Comparing `hvplot-0.8.3rc2/hvplot.egg-info/SOURCES.txt` & `hvplot-0.8.4a1/hvplot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.3rc2/hvplot.egg-info/requires.txt` & `hvplot-0.8.4a1/hvplot.egg-info/requires.txt`

 * *Files 7% similar despite different names*

```diff
@@ -18,29 +18,28 @@
 geoviews>=1.9.0
 intake>=0.6.5
 intake-parquet>=0.2.3
 intake-xarray>=0.5.0
 ipykernel<6.18.0
 ipywidgets
 matplotlib
-nbsite>=0.7.2rc2
+nbsite>=0.8.0rc33
 nbval
 networkx>=2.6.3
 notebook>=5.4
 numba>=0.51.0
 numpy<1.24
 param>=1.7.0
 parameterized
 pillow>=8.2.0
 plotly
 pooch
 pooch>=1.6.0
 pre-commit
 pyct>=0.4.4
-pydata-sphinx-theme<0.10
 pyepsg
 pygraphviz
 pyproj
 pytest
 pytest-cov
 pytest-xdist
 python-snappy>=0.6.0
@@ -49,16 +48,14 @@
 s3fs>=2022.1.0
 scikit-image>=0.17.2
 scipy
 scipy>=1.5.3
 selenium>=3.141.0
 setuptools>=30.3.0
 spatialpandas>=0.4.3
-sphinx-copybutton
-sphinx-design
 streamz>=0.3.0
 xarray
 xarray>=0.18.2
 
 [build]
 param>=1.7.0
 pyct>=0.4.4
@@ -89,21 +86,19 @@
 rioxarray
 pyepsg
 matplotlib
 plotly
 pygraphviz
 ipykernel<6.18.0
 numpy<1.24
+ipywidgets
 numba>=0.51.0
 datashader>=0.6.5
 spatialpandas>=0.4.3
-nbsite>=0.7.2rc2
-pydata-sphinx-theme<0.10
-sphinx-copybutton
-sphinx-design
+nbsite>=0.8.0rc33
 
 [examples]
 geoviews>=1.9.0
 geopandas
 xarray>=0.18.2
 networkx>=2.6.3
 streamz>=0.3.0
@@ -126,14 +121,15 @@
 rioxarray
 pyepsg
 matplotlib
 plotly
 pygraphviz
 ipykernel<6.18.0
 numpy<1.24
+ipywidgets
 numba>=0.51.0
 datashader>=0.6.5
 spatialpandas>=0.4.3
 
 [examples_tests]
 geoviews>=1.9.0
 geopandas
@@ -159,14 +155,15 @@
 rioxarray
 pyepsg
 matplotlib
 plotly
 pygraphviz
 ipykernel<6.18.0
 numpy<1.24
+ipywidgets
 numba>=0.51.0
 datashader>=0.6.5
 spatialpandas>=0.4.3
 pytest-xdist
 nbval
 
 [tests]
```

### Comparing `hvplot-0.8.3rc2/setup.py` & `hvplot-0.8.4a1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,15 +56,14 @@
     'pytest-cov',
     'matplotlib',
     'plotly',
     'xarray',
     'pooch',
     'scipy',
     'ipywidgets',
-
 ]
 
 # Dependencies required to run the notebooks
 extras_require['examples'] = [
     'geoviews >=1.9.0',
     'geopandas',
     'xarray >=0.18.2',
@@ -90,14 +89,15 @@
     # Extra dependency of cartopy on Python 3.6 only
     'pyepsg',
     'matplotlib',
     'plotly',
     'pygraphviz',
     'ipykernel <6.18.0',  # temporary
     'numpy < 1.24', # temporary, for a numba error
+    'ipywidgets',
 ]
 
 # Packages not working on python 3.11 because of numba
 if sys.version_info < (3, 11):
     extras_require['examples'] += [
         'numba >=0.51.0',
         'datashader >=0.6.5',
@@ -105,18 +105,15 @@
     ]
 
 # Run the example tests by installing examples_tests together with tests
 extras_require["examples_tests"] = extras_require["examples"] + extras_require['tests_nb']
 
 # Additional packages required to build the docs
 extras_require['doc'] = extras_require['examples'] + [
-    'nbsite >=0.7.2rc2',
-    'pydata-sphinx-theme <0.10',
-    'sphinx-copybutton',
-    'sphinx-design',
+    'nbsite >=0.8.0rc33',
 ]
 
 # until pyproject.toml/equivalent is widely supported (setup_requires
 # doesn't work well with pip)
 extras_require['build'] = [
     'param >=1.7.0',
     'pyct >=0.4.4',
```

