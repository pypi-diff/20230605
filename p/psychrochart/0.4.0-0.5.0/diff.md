# Comparing `tmp/psychrochart-0.4.0.tar.gz` & `tmp/psychrochart-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psychrochart-0.4.0.tar", max compression
+gzip compressed data, was "psychrochart-0.5.0.tar", max compression
```

## Comparing `psychrochart-0.4.0.tar` & `psychrochart-0.5.0.tar`

### file list

```diff
@@ -1,18 +1,26 @@
--rw-r--r--   0        0        0     3758 2023-06-02 06:57:29.062189 psychrochart-0.4.0/CHANGELOG.md
--rw-r--r--   0        0        0     1074 2023-06-02 06:57:29.062189 psychrochart-0.4.0/LICENSE
--rw-r--r--   0        0        0     5844 2023-06-02 06:57:29.062189 psychrochart-0.4.0/README.md
--rw-r--r--   0        0        0      344 2023-06-02 06:57:29.146189 psychrochart-0.4.0/psychrochart/__init__.py
--rw-r--r--   0        0        0      353 2023-06-02 06:57:29.146189 psychrochart-0.4.0/psychrochart/__main__.py
--rw-r--r--   0        0        0      278 2023-06-02 06:57:29.146189 psychrochart-0.4.0/psychrochart/agg.py
--rw-r--r--   0        0        0    26781 2023-06-02 06:57:29.146189 psychrochart-0.4.0/psychrochart/chart.py
--rw-r--r--   0        0        0     2157 2023-06-02 06:57:29.146189 psychrochart-0.4.0/psychrochart/chart_styles/ashrae_chart_style.json
--rw-r--r--   0        0        0     2380 2023-06-02 06:57:29.146189 psychrochart-0.4.0/psychrochart/chart_styles/ashrae_ip_chart_style.json
--rw-r--r--   0        0        0     3044 2023-06-02 06:57:29.146189 psychrochart-0.4.0/psychrochart/chart_styles/default_chart_config.json
--rw-r--r--   0        0        0      585 2023-06-02 06:57:29.146189 psychrochart-0.4.0/psychrochart/chart_styles/default_comfort_zones.json
--rw-r--r--   0        0        0     2436 2023-06-02 06:57:29.146189 psychrochart-0.4.0/psychrochart/chart_styles/interior_chart_style.json
--rw-r--r--   0        0        0     2490 2023-06-02 06:57:29.146189 psychrochart-0.4.0/psychrochart/chart_styles/minimal_chart_style.json
--rw-r--r--   0        0        0    14037 2023-06-02 06:57:29.146189 psychrochart-0.4.0/psychrochart/chartdata.py
--rw-r--r--   0        0        0     9199 2023-06-02 06:57:29.146189 psychrochart-0.4.0/psychrochart/psychrocurves.py
--rw-r--r--   0        0        0     7460 2023-06-02 06:57:29.146189 psychrochart-0.4.0/psychrochart/util.py
--rw-r--r--   0        0        0     2182 2023-06-02 06:57:29.146189 psychrochart-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     7101 1970-01-01 00:00:00.000000 psychrochart-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     6055 2023-06-05 11:57:37.165362 psychrochart-0.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1074 2023-06-05 11:57:37.165362 psychrochart-0.5.0/LICENSE
+-rw-r--r--   0        0        0     6746 2023-06-05 11:57:37.165362 psychrochart-0.5.0/README.md
+-rw-r--r--   0        0        0      711 2023-06-05 11:57:37.265361 psychrochart-0.5.0/psychrochart/__init__.py
+-rw-r--r--   0        0        0      336 2023-06-05 11:57:37.265361 psychrochart-0.5.0/psychrochart/__main__.py
+-rw-r--r--   0        0        0      254 2023-06-05 11:57:37.265361 psychrochart-0.5.0/psychrochart/agg.py
+-rw-r--r--   0        0        0    11817 2023-06-05 11:57:37.265361 psychrochart-0.5.0/psychrochart/chart.py
+-rw-r--r--   0        0        0     2157 2023-06-05 11:57:37.265361 psychrochart-0.5.0/psychrochart/chart_styles/ashrae_chart_style.json
+-rw-r--r--   0        0        0     2380 2023-06-05 11:57:37.265361 psychrochart-0.5.0/psychrochart/chart_styles/ashrae_ip_chart_style.json
+-rw-r--r--   0        0        0     3064 2023-06-05 11:57:37.265361 psychrochart-0.5.0/psychrochart/chart_styles/default_chart_config.json
+-rw-r--r--   0        0        0      585 2023-06-05 11:57:37.265361 psychrochart-0.5.0/psychrochart/chart_styles/default_comfort_zones.json
+-rw-r--r--   0        0        0     2436 2023-06-05 11:57:37.265361 psychrochart-0.5.0/psychrochart/chart_styles/interior_chart_style.json
+-rw-r--r--   0        0        0     2490 2023-06-05 11:57:37.265361 psychrochart-0.5.0/psychrochart/chart_styles/minimal_chart_style.json
+-rw-r--r--   0        0        0    14520 2023-06-05 11:57:37.265361 psychrochart-0.5.0/psychrochart/chartdata.py
+-rw-r--r--   0        0        0        0 2023-06-05 11:57:37.265361 psychrochart-0.5.0/psychrochart/models/__init__.py
+-rw-r--r--   0        0        0     4427 2023-06-05 11:57:37.265361 psychrochart-0.5.0/psychrochart/models/annots.py
+-rw-r--r--   0        0        0     6671 2023-06-05 11:57:37.265361 psychrochart-0.5.0/psychrochart/models/config.py
+-rw-r--r--   0        0        0     9239 2023-06-05 11:57:37.265361 psychrochart-0.5.0/psychrochart/models/curves.py
+-rw-r--r--   0        0        0     5852 2023-06-05 11:57:37.265361 psychrochart-0.5.0/psychrochart/models/parsers.py
+-rw-r--r--   0        0        0     1868 2023-06-05 11:57:37.265361 psychrochart-0.5.0/psychrochart/models/styles.py
+-rw-r--r--   0        0        0     1742 2023-06-05 11:57:37.265361 psychrochart-0.5.0/psychrochart/models/validators.py
+-rw-r--r--   0        0        0     7361 2023-06-05 11:57:37.265361 psychrochart-0.5.0/psychrochart/plot_logic.py
+-rw-r--r--   0        0        0     6268 2023-06-05 11:57:37.269361 psychrochart-0.5.0/psychrochart/process_logic.py
+-rw-r--r--   0        0        0     3898 2023-06-05 11:57:37.269361 psychrochart-0.5.0/psychrochart/util.py
+-rw-r--r--   0        0        0     2222 2023-06-05 11:57:37.269361 psychrochart-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     8035 1970-01-01 00:00:00.000000 psychrochart-0.5.0/PKG-INFO
```

### Comparing `psychrochart-0.4.0/LICENSE` & `psychrochart-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `psychrochart-0.4.0/README.md` & `psychrochart-0.5.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -15,84 +15,103 @@
 
 A python 3 library to make **[psychrometric charts](https://en.wikipedia.org/wiki/Psychrometrics)** and overlay information on them.
 
 It implements a useful collection of psychrometric equations for moisture and humid air calculations, and the generation of beautiful and high customizable **psychrometric charts in SVG** with [`matplotlib`](https://matplotlib.org).
 
 **Psychrometric calculations to make the chart data are done with [`PsychroLib`](https://github.com/psychrometrics/psychrolib)** (summary paper in https://doi.org/10.21105/joss.01137).
 
-<img src="https://rawgit.com/azogue/psychrochart/master/tests/charts/chart_overlay_style_minimal.svg" width="100%" height="100%">
+<img src="./tests/example-charts/chart_overlay_style_minimal.svg" width="100%" height="100%">
 
 ## Install
 
 Get it **[from pypi](https://pypi.python.org/pypi?:action=display&name=psychrochart)** or **[clone it](https://github.com/azogue/psychrochart.git)** if you want to run the tests.
 
-```bash
+```shell
 pip install psychrochart
 ```
 
 ## Features
 
 - **SI** units (with temperatures in celsius for better readability).
-- Easy style customization with a **JSON template** (colors, line styles and line widths).
+- Easy style customization based on [**pydantic**](https://docs.pydantic.dev/latest/) models and config presets for full customization of colors, line styles, line widths, etc..
 - Psychrometric charts within temperature and humidity ratio ranges, for any pressure\*, with:
   - **Saturation line**
   - **Constant RH lines**
   - **Constant enthalpy lines**
   - **Constant wet-bulb temperature lines**
   - **Constant specific volume lines**
   - **Constant dry-bulb temperature lines** (internal orthogonal grid, vertical)
   - **Constant humidity ratio lines** (internal orthogonal grid, horizontal)
 - Plot legend for each family of lines
 - Specify labels for each family of lines
-- **Overlay points, zones, arrows...**
+- **Overlay points, zones, convex hulls, and arrows**
 - **Export SVG, PNG files**
 
-\* The ranges of temperature, humidity and pressure where this library should provide good results are within the normal environments for people to live in. Don't expect right results if doing other type of thermodynamic calculations. Over saturated water vapor states are not implemented.
+> NOTE: The ranges of temperature, humidity and pressure where this library should provide good results are within the normal environments for people to live in.
+>
+> Don't expect right results if doing other type of thermodynamic calculations.
+>
+> ⚠️ **Over saturated water vapor states are not implemented**. This library is intended for HVAC applications only ⚠️
 
 ## Usage
 
 ```python
 from psychrochart import PsychroChart
 
 # Load default style:
-chart_default = PsychroChart()
+chart_default = PsychroChart.create()
 axes = chart_default.plot()
 axes.get_figure()
 ```
 
-Called from a terminal (`python psychrochart`), it plots and shows the default chart using the default matplotlib backend, equivalent to this python script:
+Called from the terminal (`python psychrochart`), it plots and shows the default chart using the default matplotlib backend, equivalent to this python script:
 
 ```python
 from psychrochart import PsychroChart
 import matplotlib.pyplot as plt
 
-PsychroChart().plot(ax=plt.gca())
+PsychroChart.create().plot(ax=plt.gca())
 plt.show()
 ```
 
 ### Chart customization
 
 The default styling for charts is defined in JSON files that you can change, or you can pass a path of a file in JSON, or a dict, when you create the psychrometric chart object.
 Included styles are: `default`, `ashrae`, `interior` and `minimal`.
 
 ```python
+from pathlib import Path
 from psychrochart import load_config, PsychroChart
 
 # Load preconfigured styles:
-chart_ashrae_style = PsychroChart('ashrae')
+chart_ashrae_style = PsychroChart.create('ashrae')
 chart_ashrae_style.plot()
 
-chart_minimal = PsychroChart('minimal')
+chart_minimal = PsychroChart.create('minimal')
 chart_minimal.plot()
 
-# Get a preconfigured style dict
-dict_config = load_config('interior')
+# Get a preconfigured style model and customize it
+chart_config = load_config('interior')
+chart_config.limits.range_temp_c = (18.0, 32.0)
+chart_config.limits.range_humidity_g_kg = (1.0, 40.0)
+chart_config.limits.altitude_m = 3000
+
+custom_chart = PsychroChart.create(chart_config)
+custom_chart.save("custom-chart.svg")
+
+# serialize the config for future uses
+assert chart_config.json() == custom_chart.config.json()
+Path('path/to/chart_config_file.json').write_text(chart_config.json())
+custom_chart_bis = PsychroChart.create('path/to/chart_config_file.json')
+# or even the full psychrochart
+Path('path/to/chart_file.json').write_text(custom_chart.json())
+custom_chart_bis_2 = PsychroChart.parse_file('path/to/chart_file.json')
 
 # Specify the styles JSON file:
-chart_custom = PsychroChart('/path/to/json_file.json')
+chart_custom = PsychroChart.create('/path/to/json_file.json')
 chart_custom.plot()
 
 # Pass a dict with the changes wanted:
 custom_style = {
     "figure": {
         "figsize": [12, 8],
         "base_fontsize": 12,
@@ -117,40 +136,42 @@
         "with_constant_v": False,
         "with_constant_h": False,
         "with_constant_wet_temp": False,
         "with_zones": False
     }
 }
 
-chart_custom_2 = PsychroChart(custom_style)
+chart_custom_2 = PsychroChart.create(custom_style)
 chart_custom_2.plot()
 ```
 
 The custom configuration does not need to include all fields, but only the fields you want to change.
 
 To play with it and see the results, look at this **[notebook with usage examples](https://github.com/azogue/psychrochart/blob/master/notebooks/Usage%20example%20of%20psychrochart.ipynb)**.
 
-## Tests
+## Development and testing
 
 To run the tests, clone the repository, `poetry install` it, and run `poetry run pytest`.
 
+Run `poetry run pre-commit run --all-files` to apply linters for changes in the code 😜.
+
 ## License
 
 [MIT license](https://github.com/azogue/psychrochart/blob/master/LICENSE), so do with it as you like ;-)
 
 ## Included styling examples
 
 **Default style**:
 
-<img src="https://rawgit.com/azogue/psychrochart/master/tests/charts/test_default_psychrochart.svg" width="100%" height="100%">
+<img src="./tests/example-charts/test_default_psychrochart.svg" width="100%" height="100%">
 
-**ASHRAE Handbook black and white style**:
+**ASHRAE Handbook black and white style**: (preset: `ashrae`)
 
-<img src="https://rawgit.com/azogue/psychrochart/master/tests/charts/test_ashrae_psychrochart.svg" width="100%" height="100%">
+<img src="./tests/example-charts/test_ashrae_psychrochart.svg" width="100%" height="100%">
 
-**ASHRAE Handbook black and white style (IP units)**:
+**ASHRAE Handbook black and white style (IP units)**: (preset: `ashrae_ip`)
 
-<img src="https://rawgit.com/azogue/psychrochart/master/tests/charts/test_ashrae_psychrochart_ip.svg" width="100%" height="100%">
+<img src="./tests/example-charts/test_ashrae_psychrochart_ip.svg" width="100%" height="100%">
 
-**Minimal style**:
+**Minimal style**: (preset: `minimal`)
 
-<img src="https://rawgit.com/azogue/psychrochart/master/tests/charts/test_minimal_psychrochart.svg" width="100%" height="100%">
+<img src="./tests/example-charts/test_minimal_psychrochart.svg" width="100%" height="100%">
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `psychrochart-0.4.0/psychrochart/chart_styles/ashrae_chart_style.json` & `psychrochart-0.5.0/psychrochart/chart_styles/ashrae_chart_style.json`

 * *Files identical despite different names*

### Comparing `psychrochart-0.4.0/psychrochart/chart_styles/ashrae_ip_chart_style.json` & `psychrochart-0.5.0/psychrochart/chart_styles/ashrae_ip_chart_style.json`

 * *Files identical despite different names*

### Comparing `psychrochart-0.4.0/psychrochart/chart_styles/default_chart_config.json` & `psychrochart-0.5.0/psychrochart/chart_styles/default_chart_config.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9961538461538462%*

 * *Differences: {"'figure'": "{'fontsize': 10}"}*

```diff
@@ -139,14 +139,15 @@
         "linewidth": 1
     },
     "figure": {
         "figsize": [
             16,
             9
         ],
+        "fontsize": 10,
         "partial_axis": true,
         "position": [
             0.025,
             0.075,
             0.925,
             0.875
         ],
```

### Comparing `psychrochart-0.4.0/psychrochart/chart_styles/default_comfort_zones.json` & `psychrochart-0.5.0/psychrochart/chart_styles/default_comfort_zones.json`

 * *Files identical despite different names*

### Comparing `psychrochart-0.4.0/psychrochart/chart_styles/interior_chart_style.json` & `psychrochart-0.5.0/psychrochart/chart_styles/interior_chart_style.json`

 * *Files identical despite different names*

### Comparing `psychrochart-0.4.0/psychrochart/chart_styles/minimal_chart_style.json` & `psychrochart-0.5.0/psychrochart/chart_styles/minimal_chart_style.json`

 * *Files identical despite different names*

### Comparing `psychrochart-0.4.0/psychrochart/chartdata.py` & `psychrochart-0.5.0/psychrochart/chartdata.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# -*- coding: utf-8 -*-
 """A library to make psychrometric charts and overlay information in them."""
-from typing import Any, Callable, Iterable
+from typing import Callable, Iterable
 
 import numpy as np
 from psychrolib import (
     GetHumRatioFromVapPres,
     GetMoistAirEnthalpy,
     GetMoistAirVolume,
     GetRelHumFromTWetBulb,
@@ -13,16 +12,18 @@
     GetTDryBulbFromEnthalpyAndHumRatio,
     GetTDryBulbFromMoistAirVolumeAndHumRatio,
     GetVapPresFromHumRatio,
     isIP,
 )
 from scipy.interpolate import interp1d
 
-from .psychrocurves import PsychroCurve, PsychroCurves
-from .util import solve_curves_with_iteration
+from psychrochart.models.annots import ChartZone
+from psychrochart.models.curves import PsychroCurve, PsychroCurves
+from psychrochart.models.styles import CurveStyle, ZoneStyle
+from psychrochart.util import solve_curves_with_iteration
 
 f_vec_hum_ratio_from_vap_press = np.vectorize(GetHumRatioFromVapPres)
 f_vec_moist_air_enthalpy = np.vectorize(GetMoistAirEnthalpy)
 f_vec_moist_air_volume = np.vectorize(GetMoistAirVolume)
 f_vec_dew_point_from_vap_press = np.vectorize(GetTDewPointFromVapPres)
 f_vec_dry_temp_from_enthalpy = np.vectorize(GetTDryBulbFromEnthalpyAndHumRatio)
 f_vec_dry_temp_from_spec_vol = np.vectorize(
@@ -100,33 +101,33 @@
 def make_constant_relative_humidity_lines(
     dbt_min: float,
     dbt_max: float,
     temp_step: float,
     pressure: float,
     rh_perc_values: Iterable[float],
     rh_label_values: Iterable[float],
-    style: dict[str, Any],
+    style: CurveStyle,
     label_loc: float,
-    family_label: str,
+    family_label: str | None,
 ) -> PsychroCurves:
     """Generate curves of constant relative humidity for the chart."""
     temps_ct_rh, curves_ct_rh = _gen_list_curves_range_temps(
         gen_points_in_constant_relative_humidity,
         rh_perc_values,
         dbt_min,
         dbt_max,
         temp_step,
         pressure,
     )
     return PsychroCurves(
-        [
+        curves=[
             PsychroCurve(
-                temps_ct_rh,
-                curve_ct_rh,
-                style,
+                x_data=temps_ct_rh,
+                y_data=curve_ct_rh,
+                style=style,
                 type_curve="constant_rh_data",
                 label_loc=label_loc,
                 label=(
                     f"RH {rh:g} %" if round(rh, 1) in rh_label_values else None
                 ),
             )
             for rh, curve_ct_rh in zip(rh_perc_values, curves_ct_rh)
@@ -135,104 +136,112 @@
     )
 
 
 def make_constant_dry_bulb_v_line(
     w_humidity_ratio_min: float,
     temp: float,
     pressure: float,
-    style: dict[str, Any],
+    style: CurveStyle,
     type_curve: str | None = None,
     reverse: bool = False,
 ) -> PsychroCurve:
     """Generate vertical line (constant dry bulb temp) up to saturation."""
     w_max = _factor_out_w() * GetHumRatioFromVapPres(
         GetSatVapPres(temp), pressure
     )
     if reverse:
         path_y = [w_max, w_humidity_ratio_min]
     else:
         path_y = [w_humidity_ratio_min, w_max]
     return PsychroCurve(
-        np.array([temp, temp]), np.array(path_y), style, type_curve=type_curve
+        x_data=np.array([temp, temp]),
+        y_data=np.array(path_y),
+        style=style,
+        type_curve=type_curve,
     )
 
 
 def make_constant_dry_bulb_v_lines(
     w_humidity_ratio_min: float,
     pressure: float,
     temps_vl: np.ndarray,
-    style: dict[str, Any],
-    family_label: str,
+    style: CurveStyle,
+    family_label: str | None,
 ) -> PsychroCurves:
     """Generate curves of constant dry bulb temperature (vertical)."""
     w_max_vec = _get_humid_ratio_in_saturation(temps_vl, pressure)
     return PsychroCurves(
-        [
+        curves=[
             PsychroCurve(
-                np.array([temp, temp]),
-                np.array([w_humidity_ratio_min, w_max]),
+                x_data=np.array([temp, temp]),
+                y_data=np.array([w_humidity_ratio_min, w_max]),
                 style=style,
                 type_curve="constant_dry_temp_data",
             )
             for temp, w_max in zip(temps_vl, w_max_vec)
         ],
         family_label=family_label,
     )
 
 
 def make_constant_humidity_ratio_h_lines(
     dbt_max: float,
     pressure: float,
     ws_hl: Iterable[float],
-    style: dict[str, Any],
-    family_label: str,
+    style: CurveStyle,
+    family_label: str | None,
 ) -> PsychroCurves:
     """Generate curves of constant absolute humidity (horizontal)."""
     arr_hum_ratios = np.array(ws_hl) / _factor_out_w()
     dew_points = f_vec_dew_point_from_vap_press(
         dbt_max, f_vec_vap_press_from_hum_ratio(arr_hum_ratios, pressure)
     )
     return PsychroCurves(
-        [
+        curves=[
             PsychroCurve(
-                np.array([t_dp, dbt_max]),
-                np.array([w, w]),
-                style,
+                x_data=np.array([t_dp, dbt_max]),
+                y_data=np.array([w, w]),
+                style=style,
                 type_curve="constant_humidity_data",
             )
             for w, t_dp in zip(ws_hl, dew_points)
         ],
         family_label=family_label,
     )
 
 
 def make_saturation_line(
     dbt_min: float,
     dbt_max: float,
     temp_step: float,
     pressure: float,
-    style: dict[str, Any],
+    style: CurveStyle,
 ) -> PsychroCurves:
     """Generate line of saturation for the psychrochart."""
     temps_sat_line = np.arange(dbt_min, dbt_max + temp_step, temp_step)
     w_sat = gen_points_in_constant_relative_humidity(
         temps_sat_line, 100.0, pressure
     )
-    sat_c = PsychroCurve(temps_sat_line, w_sat, style, type_curve="saturation")
-    return PsychroCurves([sat_c])
+    sat_c = PsychroCurve(
+        x_data=temps_sat_line,
+        y_data=w_sat,
+        style=style,
+        type_curve="saturation",
+    )
+    return PsychroCurves(curves=[sat_c])
 
 
 def make_constant_enthalpy_lines(
     w_humidity_ratio_min: float,
     pressure: float,
     enthalpy_values: Iterable[float],
     h_label_values: Iterable[float],
-    style: dict[str, Any],
+    style: CurveStyle,
     label_loc: float,
-    family_label: str,
+    family_label: str | None,
     saturation_curve: PsychroCurve,
 ) -> PsychroCurves:
     """Generate curves of constant enthalpy for the chart."""
     enthalpy_objective = np.array(enthalpy_values)
     temps_max_constant_h = f_vec_dry_temp_from_enthalpy(
         enthalpy_objective * _factor_out_h(),
         w_humidity_ratio_min / _factor_out_w(),
@@ -257,19 +266,19 @@
             x, GetHumRatioFromVapPres(GetSatVapPres(x), pressure)
         )
         / _factor_out_h(),
     )
     w_in_sat = _get_humid_ratio_in_saturation(t_sat_points, pressure)
 
     return PsychroCurves(
-        [
+        curves=[
             PsychroCurve(
-                np.array([t_sat, t_max]),
-                np.array([w_sat, w_humidity_ratio_min]),
-                style,
+                x_data=np.array([t_sat, t_max]),
+                y_data=np.array([w_sat, w_humidity_ratio_min]),
+                style=style,
                 type_curve="constant_h_data",
                 label_loc=label_loc,
                 label=(
                     _make_enthalpy_label(h)
                     if round(h, 3) in h_label_values
                     else None
                 ),
@@ -283,17 +292,17 @@
 
 
 def make_constant_specific_volume_lines(
     w_humidity_ratio_min: float,
     pressure: float,
     vol_values: np.ndarray,
     v_label_values: Iterable[float],
-    style: dict[str, Any],
+    style: CurveStyle,
     label_loc: float,
-    family_label: str,
+    family_label: str | None,
     saturation_curve: PsychroCurve,
 ) -> PsychroCurves:
     """Generate curves of constant specific volume for the chart."""
     temps_max_constant_v = f_vec_dry_temp_from_spec_vol(
         np.array(vol_values), w_humidity_ratio_min / _factor_out_w(), pressure
     )
     v_in_sat = f_vec_moist_air_volume(
@@ -314,19 +323,19 @@
         lambda x: GetMoistAirVolume(
             x, GetHumRatioFromVapPres(GetSatVapPres(x), pressure), pressure
         ),
     )
     w_in_sat = _get_humid_ratio_in_saturation(t_sat_points, pressure)
 
     return PsychroCurves(
-        [
+        curves=[
             PsychroCurve(
-                np.array([t_sat, t_max]),
-                np.array([w_sat, w_humidity_ratio_min]),
-                style,
+                x_data=np.array([t_sat, t_max]),
+                y_data=np.array([w_sat, w_humidity_ratio_min]),
+                style=style,
                 type_curve="constant_v_data",
                 label_loc=label_loc,
                 label=(
                     _make_vol_label(vol)
                     if round(vol, 3) in v_label_values
                     else None
                 ),
@@ -340,17 +349,17 @@
 
 
 def make_constant_wet_bulb_temperature_lines(
     dry_bulb_temp_max: float,
     pressure: float,
     wbt_values: np.ndarray,
     wbt_label_values: Iterable[float],
-    style: dict[str, Any],
+    style: CurveStyle,
     label_loc: float,
-    family_label: str,
+    family_label: str | None,
 ) -> PsychroCurves:
     """Generate curves of constant wet bulb temperature for the chart."""
     w_max_constant_wbt = f_vec_hum_ratio_from_vap_press(
         f_vec_sat_press(np.array(wbt_values)), pressure
     )
 
     def _hum_ratio_for_constant_wet_temp_at_dry_temp(db_t, wb_t, p_atm):
@@ -379,34 +388,34 @@
                 slope = (pair_t[1] - pair_t[0]) / (pair_w[1] - pair_w[0])
                 new_dbt = wbt - slope * pair_w[0]
                 pair_t[1] = new_dbt
                 pair_w[1] = 0.0
                 break
 
         c = PsychroCurve(
-            np.array(pair_t),
-            np.array(pair_w),
-            style,
+            x_data=np.array(pair_t),
+            y_data=np.array(pair_w),
+            style=style,
             type_curve="constant_wbt_data",
             label_loc=label_loc,
             label=(_make_temp_label(wbt) if wbt in wbt_label_values else None),
         )
         curves.append(c)
 
-    return PsychroCurves(curves, family_label=family_label)
+    return PsychroCurves(curves=curves, family_label=family_label)
 
 
 def _make_zone_dbt_rh(
     t_min: float,
     t_max: float,
     increment: float,
     rh_min: float,
     rh_max: float,
     pressure: float,
-    style: dict[str, Any] | None = None,
+    style: ZoneStyle,
     label: str | None = None,
 ) -> PsychroCurve:
     """Generate points for zone between constant dry bulb temps and RH."""
     temps = np.arange(t_min, t_max + increment, increment)
     curve_rh_up = gen_points_in_constant_relative_humidity(
         temps, rh_max, pressure
     )
@@ -414,42 +423,45 @@
         temps, rh_min, pressure
     )
     abs_humid: list[float] = (
         list(curve_rh_up) + list(curve_rh_down)[::-1] + [curve_rh_up[0]]
     )
     temps_zone: list[float] = list(temps) + list(temps)[::-1] + [temps[0]]
     return PsychroCurve(
-        np.array(temps_zone),
-        np.array(abs_humid),
-        style,
+        x_data=np.array(temps_zone),
+        y_data=np.array(abs_humid),
+        style=style,
         type_curve="constant_rh_data",
         label=label,
     )
 
 
 def make_zone_curve(
-    zone_conf: dict[str, Any], increment: float, pressure: float
+    zone_conf: ChartZone, increment: float, pressure: float
 ) -> PsychroCurve:
     """Generate points for zone between constant dry bulb temps and RH."""
     # TODO make conversion rh -> w and new zone_type: "dbt-rh-points"
-    if zone_conf["zone_type"] == "dbt-rh":
-        t_min, t_max = zone_conf["points_x"]
-        rh_min, rh_max = zone_conf["points_y"]
+    assert isinstance(zone_conf.style, ZoneStyle)
+    if zone_conf.zone_type == "dbt-rh":
+        t_min = zone_conf.points_x[0]
+        t_max = zone_conf.points_x[-1]
+        rh_min = zone_conf.points_y[0]
+        rh_max = zone_conf.points_y[-1]
         return _make_zone_dbt_rh(
             t_min,
             t_max,
             increment,
             rh_min,
             rh_max,
             pressure,
-            zone_conf["style"],
-            label=zone_conf.get("label"),
+            zone_conf.style,
+            label=zone_conf.label,
         )
     else:
         # zone_type: 'xy-points'
         return PsychroCurve(
-            zone_conf["points_x"],
-            zone_conf["points_y"],
-            zone_conf["style"],
+            x_data=zone_conf.points_x,
+            y_data=zone_conf.points_y,
+            style=zone_conf.style,
             type_curve="custom path",
-            label=zone_conf.get("label"),
+            label=zone_conf.label,
         )
```

### Comparing `psychrochart-0.4.0/psychrochart/psychrocurves.py` & `psychrochart-0.5.0/psychrochart/models/curves.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# -*- coding: utf-8 -*-
-"""A library to make psychrometric charts and overlay information in them."""
-import json
 import logging
 from math import atan2, degrees
-from typing import Any, AnyStr
+from typing import AbstractSet, Any, AnyStr, Mapping
 
 from matplotlib import patches
 from matplotlib.axes import Axes
 from matplotlib.path import Path
 import numpy as np
+from pydantic import BaseModel, Field, root_validator
 
-from .util import mod_color
+from psychrochart.models.styles import CurveStyle, ZoneStyle
+from psychrochart.models.validators import parse_curve_arrays
+from psychrochart.util import mod_color
 
 
 def _between_limits(
     x_data: np.ndarray,
     y_data: np.ndarray,
     xmin: float,
     xmax: float,
@@ -31,162 +31,161 @@
         or (data_ymin > ymax)
         or (data_xmin > xmax)
     ):
         return False
     return True
 
 
-class PsychroCurve:
-    """Object to store a psychrometric curve for plotting."""
+def _annotate_label(
+    ax: Axes,
+    label: AnyStr,
+    text_x: float,
+    text_y: float,
+    rotation: float,
+    text_style: dict[str, Any],
+) -> None:
+    if abs(rotation) > 0:
+        text_loc = np.array((text_x, text_y))
+        text_style["rotation"] = ax.transData.transform_angles(
+            np.array((rotation,)), text_loc.reshape((1, 2))
+        )[0]
+        text_style["rotation_mode"] = "anchor"
+    ax.annotate(label, (text_x, text_y), **text_style)
+
+
+class PsychroCurve(BaseModel):
+    """Pydantic model to store a psychrometric curve for plotting."""
+
+    x_data: np.ndarray
+    y_data: np.ndarray
+    style: ZoneStyle | CurveStyle
+    type_curve: str | None = None
+    label: str | None = None
+    label_loc: float = 0.75
+
+    class Config:
+        arbitrary_types_allowed = True
+        json_encoders = {np.ndarray: lambda x: x.tolist()}
+
+    @root_validator(pre=True)
+    def _parse_curve_data(cls, values):
+        return parse_curve_arrays(values)
 
-    def __init__(
+    def dict(
         self,
-        x_data: np.ndarray | None = None,
-        y_data: np.ndarray | None = None,
-        style: dict[str, Any] | None = None,
-        type_curve: str | None = None,
-        limits: dict[str, Any] | None = None,
-        label: str | None = None,
-        label_loc: float = 0.75,
-    ) -> None:
-        """Create the Psychrocurve object."""
-        self.x_data = np.array(x_data if x_data is not None else [])
-        self.y_data = np.array(y_data if y_data is not None else [])
-        self.style: dict[str, Any] = style or {}
-        self._type_curve = type_curve
-        self._label = label
-        self._label_loc = label_loc
-        self._limits = limits
-        self._is_patch: bool = style is not None and "facecolor" in style
-
-    def __bool__(self) -> bool:
-        """Return the valid existence of the curve."""
-        if (
-            self.x_data is not None
-            and len(self.x_data) > 1
-            and self.y_data is not None
-            and len(self.y_data) > 1
-        ):
-            return True
-        return False
+        *,
+        include: AbstractSet[int | str]
+        | Mapping[int | str, Any]
+        | None = None,
+        exclude: AbstractSet[int | str]
+        | Mapping[int | str, Any]
+        | None = None,
+        by_alias: bool = False,
+        skip_defaults: bool | None = None,
+        exclude_unset: bool = False,
+        exclude_defaults: bool = False,
+        exclude_none: bool = False,
+    ) -> dict[str, Any]:
+        """Override pydantic.BaseModel.dict() to export arrays as list."""
+        plain_dict = super().dict(
+            include=include,
+            exclude=exclude,
+            by_alias=by_alias,
+            skip_defaults=skip_defaults,
+            exclude_unset=exclude_unset,
+            exclude_defaults=exclude_defaults,
+            exclude_none=exclude_none,
+        )
+        plain_dict["x_data"] = plain_dict["x_data"].tolist()
+        plain_dict["y_data"] = plain_dict["y_data"].tolist()
+        return plain_dict
 
     def __repr__(self) -> str:
         """Object string representation."""
-        name = "PsychroZone" if self._is_patch else "PsychroCurve"
-        if self and self.x_data is not None:
-            return f"<{name} {len(self.x_data)} values (label: {self._label})>"
-        else:
-            return f"<Empty {name} (label: {self._label})>"
-
-    def to_dict(self) -> dict[str, Any]:
-        """Return the curve as a dict."""
-        if len(self.x_data) == 0 or len(self.y_data) == 0:
-            return {}
-        return {
-            "x_data": self.x_data.tolist(),
-            "y_data": self.y_data.tolist(),
-            "style": self.style,
-            "label": self._label,
-        }
-
-    def to_json(self) -> str:
-        """Return the curve as a JSON string."""
-        return json.dumps(self.to_dict())
-
-    def from_json(self, json_str: AnyStr):
-        """Load a curve from a JSON string."""
-        data = json.loads(json_str)
-        self.x_data = np.array(data["x_data"])
-        self.y_data = np.array(data["y_data"])
-        self.style = data.get("style")
-        self._label = data.get("label")
-        return self
-
-    @staticmethod
-    def _annotate_label(
-        ax: Axes,
-        label: AnyStr,
-        text_x: float,
-        text_y: float,
-        rotation: float,
-        text_style: dict[str, Any],
-    ):
-        if abs(rotation) > 0:
-            text_loc = np.array((text_x, text_y))
-            text_style["rotation"] = ax.transData.transform_angles(
-                np.array((rotation,)), text_loc.reshape((1, 2))
-            )[0]
-            text_style["rotation_mode"] = "anchor"
-        ax.annotate(label, (text_x, text_y), **text_style)
+        name = (
+            "PsychroZone"
+            if isinstance(self.style, ZoneStyle)
+            else "PsychroCurve"
+        )
+        extra = f" (label: {self.label})" if self.label else ""
+        return f"<{name} {len(self.x_data)} values{extra}>"
 
-    def plot(self, ax: Axes) -> Axes:
-        """Plot the curve."""
+    def plot_curve(self, ax: Axes) -> bool:
+        """Plot the curve, if it's between chart limits."""
         xmin, xmax = ax.get_xlim()
         ymin, ymax = ax.get_ylim()
         if (
             self.x_data is None
             or self.y_data is None
             or not _between_limits(
                 self.x_data, self.y_data, xmin, xmax, ymin, ymax
             )
         ):
-            logging.info(
-                f"{self._type_curve} (label:{self._label}) Not between limits "
-                f"([{xmin}, {xmax}, {ymin}, {ymax}]) "
-                f"-> x:{self.x_data}, y:{self.y_data}"
+            logging.debug(
+                "%s (label:%s) Not between limits ([%.2g, %.2g, %.2g, %.2g]) "
+                "-> x:%s, y:%s",
+                self.type_curve,
+                self.label or "unnamed",
+                xmin,
+                xmax,
+                ymin,
+                ymax,
+                self.x_data,
+                self.y_data,
             )
-            return ax
+            return False
 
-        if self._is_patch and self.y_data is not None:
+        if isinstance(self.style, ZoneStyle):
             assert len(self.y_data) > 2
             verts = list(zip(self.x_data, self.y_data))
             codes = (
                 [Path.MOVETO]
                 + [Path.LINETO] * (len(self.y_data) - 2)
                 + [Path.CLOSEPOLY]
             )
             path = Path(verts, codes)
-            patch = patches.PathPatch(path, **self.style)
+            patch = patches.PathPatch(path, **self.style.dict())
             ax.add_patch(patch)
 
-            if self._label is not None:
+            if self.label is not None:
                 bbox_p = path.get_extents()
                 text_x = 0.5 * (bbox_p.x0 + bbox_p.x1)
                 text_y = 0.5 * (bbox_p.y0 + bbox_p.y1)
-                style = {
+                style_params = {
                     "ha": "center",
                     "va": "center",
                     "backgroundcolor": [1, 1, 1, 0.4],
                 }
-                if "edgecolor" in self.style:
-                    style["color"] = mod_color(self.style["edgecolor"], -25)
-                self._annotate_label(ax, self._label, text_x, text_y, 0, style)
+                assert isinstance(self.style, ZoneStyle)
+                style_params["color"] = mod_color(self.style.edgecolor, -25)
+                _annotate_label(
+                    ax, self.label, text_x, text_y, 0, style_params
+                )
         else:
-            ax.plot(self.x_data, self.y_data, **self.style)
-            if self._label is not None:
+            ax.plot(self.x_data, self.y_data, **self.style.dict())
+            if self.label is not None:
                 self.add_label(ax)
-
-        return ax
+        return True
 
     def add_label(
         self,
         ax: Axes,
         text_label: str | None = None,
         va: str | None = None,
         ha: str | None = None,
         loc: float | None = None,
         **params,
     ) -> Axes:
         """Annotate the curve with its label."""
         num_samples = len(self.x_data)
         assert num_samples > 1
         text_style = {"va": "bottom", "ha": "left", "color": [0.0, 0.0, 0.0]}
-        loc_f: float = self._label_loc if loc is None else loc
+        loc_f: float = self.label_loc if loc is None else loc
         label: str = (
-            (self._label if self._label is not None else "")
+            (self.label if self.label is not None else "")
             if text_label is None
             else text_label
         )
 
         def _tilt_params(x_data, y_data, idx_0, idx_f):
             delta_x = x_data[idx_f] - self.x_data[idx_0]
             delta_y = y_data[idx_f] - self.y_data[idx_0]
@@ -222,57 +221,64 @@
             idx = min(num_samples - 2, int(num_samples * loc_f))
             rotation, tilt = _tilt_params(
                 self.x_data, self.y_data, idx, idx + 1
             )
             text_x, text_y = self.x_data[idx], self.y_data[idx]
             text_style["ha"] = "center"
 
-        if "color" in self.style:
-            text_style["color"] = mod_color(self.style["color"], -25)
+        text_style["color"] = mod_color(self.style.color, -25)
         if ha is not None:
             text_style["ha"] = ha
         if va is not None:
             text_style["va"] = va
         if params:
             text_style.update(params)
 
-        self._annotate_label(ax, label, text_x, text_y, rotation, text_style)
+        _annotate_label(ax, label, text_x, text_y, rotation, text_style)
 
         return ax
 
 
-class PsychroCurves:
-    """Object to store a list of psychrometric curves for plotting."""
+class PsychroCurves(BaseModel):
+    """Pydantic model to store a list of psychrometric curves for plotting."""
 
-    def __init__(
-        self, curves: list[PsychroCurve], family_label: str | None = None
-    ) -> None:
-        """Create the Psychrocurves array object."""
-        self.curves: list[PsychroCurve] = curves
-        self.size: int = len(self.curves)
-        self.family_label: str | None = family_label
-
-    def __getitem__(self, item) -> PsychroCurve:
-        """Get item from the PsychroCurve list."""
-        return self.curves[item]
+    curves: list[PsychroCurve] = Field(min_items=1)
+    family_label: str | None = None
 
     def __repr__(self) -> str:
         """Object string representation."""
-        return f"<{self.size} PsychroCurves (label: {self.family_label})>"
+        extra = f" (label: {self.family_label})" if self.family_label else ""
+        return f"<{len(self.curves)} PsychroCurves{extra}>"
 
     def plot(self, ax: Axes) -> Axes:
         """Plot the family curves."""
-        [curve.plot(ax) for curve in self.curves]
+        [curve.plot_curve(ax) for curve in self.curves]
 
         # Curves family labelling
         if self.curves and self.family_label is not None:
-            style = self.curves[0].style or {}
             ax.plot(
                 [-1],
                 [-1],
                 label=self.family_label,
                 marker="D",
                 markersize=10,
-                **style,
+                **self.curves[0].style.dict(),
             )
 
         return ax
+
+
+class PsychroChartModel(BaseModel):
+    """Pydantic model to store all psychrometric curves for PsychroChart."""
+
+    unit_system_si: bool
+    altitude_m: int
+    pressure: float
+
+    saturation: PsychroCurves
+    constant_dry_temp_data: PsychroCurves | None = None
+    constant_humidity_data: PsychroCurves | None = None
+    constant_rh_data: PsychroCurves | None = None
+    constant_h_data: PsychroCurves | None = None
+    constant_v_data: PsychroCurves | None = None
+    constant_wbt_data: PsychroCurves | None = None
+    zones: list[PsychroCurves] = Field(default_factory=list)
```

### Comparing `psychrochart-0.4.0/pyproject.toml` & `psychrochart-0.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -33,20 +33,21 @@
 ]
 
 [tool.pytest.ini_options]
 minversion = 6.0
 testpaths = "tests"
 addopts = "-vv -s --cov psychrochart --cov-report term --cov-report html"
 log_level = "INFO"
+log_cli = true
 log_format = "%(asctime)s %(levelname)s: (%(filename)s:%(lineno)s): %(message)s"
 log_date_format = "%Y-%m-%d %H:%M:%S"
 
 [tool.poetry]
 name = "psychrochart"
-version = "0.4.0"
+version = "0.5.0"
 description = "A python 3 library to make psychrometric charts and overlay information on them"
 authors = ["Eugenio Panadero <eugenio.panadero@gmail.com>"]
 packages = [
     { include = "psychrochart" }
 ]
 license = "MIT"
 readme = "README.md"
@@ -69,16 +70,17 @@
 include = ["CHANGELOG.md"]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
 matplotlib = ">=3.7"
 scipy = ">=1.10"
 psychrolib = ">=2.5"
+pydantic = ">=1.8"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 pre-commit = ">=2.10.0"
 pytest = "*"
 pytest-cov = "*"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `psychrochart-0.4.0/PKG-INFO` & `psychrochart-0.5.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psychrochart
-Version: 0.4.0
+Version: 0.5.0
 Summary: A python 3 library to make psychrometric charts and overlay information on them
 Home-page: https://github.com/azogue/psychrochart
 License: MIT
 Keywords: psychrometrics,moist,humid air,climate control,matplotlib
 Author: Eugenio Panadero
 Author-email: eugenio.panadero@gmail.com
 Requires-Python: >=3.10,<3.12
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Requires-Dist: matplotlib (>=3.7)
 Requires-Dist: psychrolib (>=2.5)
+Requires-Dist: pydantic (>=1.8)
 Requires-Dist: scipy (>=1.10)
 Project-URL: Repository, https://github.com/azogue/psychrochart
 Description-Content-Type: text/markdown
 
 [![pre-commit.ci Status][pre-commit-ci-image]][pre-commit-ci-url]
 [![Build Status][build-image]][build-url]
 [![PyPI Version][pypi-image]][pypi-url]
@@ -44,84 +45,103 @@
 
 A python 3 library to make **[psychrometric charts](https://en.wikipedia.org/wiki/Psychrometrics)** and overlay information on them.
 
 It implements a useful collection of psychrometric equations for moisture and humid air calculations, and the generation of beautiful and high customizable **psychrometric charts in SVG** with [`matplotlib`](https://matplotlib.org).
 
 **Psychrometric calculations to make the chart data are done with [`PsychroLib`](https://github.com/psychrometrics/psychrolib)** (summary paper in https://doi.org/10.21105/joss.01137).
 
-<img src="https://rawgit.com/azogue/psychrochart/master/tests/charts/chart_overlay_style_minimal.svg" width="100%" height="100%">
+<img src="./tests/example-charts/chart_overlay_style_minimal.svg" width="100%" height="100%">
 
 ## Install
 
 Get it **[from pypi](https://pypi.python.org/pypi?:action=display&name=psychrochart)** or **[clone it](https://github.com/azogue/psychrochart.git)** if you want to run the tests.
 
-```bash
+```shell
 pip install psychrochart
 ```
 
 ## Features
 
 - **SI** units (with temperatures in celsius for better readability).
-- Easy style customization with a **JSON template** (colors, line styles and line widths).
+- Easy style customization based on [**pydantic**](https://docs.pydantic.dev/latest/) models and config presets for full customization of colors, line styles, line widths, etc..
 - Psychrometric charts within temperature and humidity ratio ranges, for any pressure\*, with:
   - **Saturation line**
   - **Constant RH lines**
   - **Constant enthalpy lines**
   - **Constant wet-bulb temperature lines**
   - **Constant specific volume lines**
   - **Constant dry-bulb temperature lines** (internal orthogonal grid, vertical)
   - **Constant humidity ratio lines** (internal orthogonal grid, horizontal)
 - Plot legend for each family of lines
 - Specify labels for each family of lines
-- **Overlay points, zones, arrows...**
+- **Overlay points, zones, convex hulls, and arrows**
 - **Export SVG, PNG files**
 
-\* The ranges of temperature, humidity and pressure where this library should provide good results are within the normal environments for people to live in. Don't expect right results if doing other type of thermodynamic calculations. Over saturated water vapor states are not implemented.
+> NOTE: The ranges of temperature, humidity and pressure where this library should provide good results are within the normal environments for people to live in.
+>
+> Don't expect right results if doing other type of thermodynamic calculations.
+>
+> ⚠️ **Over saturated water vapor states are not implemented**. This library is intended for HVAC applications only ⚠️
 
 ## Usage
 
 ```python
 from psychrochart import PsychroChart
 
 # Load default style:
-chart_default = PsychroChart()
+chart_default = PsychroChart.create()
 axes = chart_default.plot()
 axes.get_figure()
 ```
 
-Called from a terminal (`python psychrochart`), it plots and shows the default chart using the default matplotlib backend, equivalent to this python script:
+Called from the terminal (`python psychrochart`), it plots and shows the default chart using the default matplotlib backend, equivalent to this python script:
 
 ```python
 from psychrochart import PsychroChart
 import matplotlib.pyplot as plt
 
-PsychroChart().plot(ax=plt.gca())
+PsychroChart.create().plot(ax=plt.gca())
 plt.show()
 ```
 
 ### Chart customization
 
 The default styling for charts is defined in JSON files that you can change, or you can pass a path of a file in JSON, or a dict, when you create the psychrometric chart object.
 Included styles are: `default`, `ashrae`, `interior` and `minimal`.
 
 ```python
+from pathlib import Path
 from psychrochart import load_config, PsychroChart
 
 # Load preconfigured styles:
-chart_ashrae_style = PsychroChart('ashrae')
+chart_ashrae_style = PsychroChart.create('ashrae')
 chart_ashrae_style.plot()
 
-chart_minimal = PsychroChart('minimal')
+chart_minimal = PsychroChart.create('minimal')
 chart_minimal.plot()
 
-# Get a preconfigured style dict
-dict_config = load_config('interior')
+# Get a preconfigured style model and customize it
+chart_config = load_config('interior')
+chart_config.limits.range_temp_c = (18.0, 32.0)
+chart_config.limits.range_humidity_g_kg = (1.0, 40.0)
+chart_config.limits.altitude_m = 3000
+
+custom_chart = PsychroChart.create(chart_config)
+custom_chart.save("custom-chart.svg")
+
+# serialize the config for future uses
+assert chart_config.json() == custom_chart.config.json()
+Path('path/to/chart_config_file.json').write_text(chart_config.json())
+custom_chart_bis = PsychroChart.create('path/to/chart_config_file.json')
+# or even the full psychrochart
+Path('path/to/chart_file.json').write_text(custom_chart.json())
+custom_chart_bis_2 = PsychroChart.parse_file('path/to/chart_file.json')
 
 # Specify the styles JSON file:
-chart_custom = PsychroChart('/path/to/json_file.json')
+chart_custom = PsychroChart.create('/path/to/json_file.json')
 chart_custom.plot()
 
 # Pass a dict with the changes wanted:
 custom_style = {
     "figure": {
         "figsize": [12, 8],
         "base_fontsize": 12,
@@ -146,41 +166,43 @@
         "with_constant_v": False,
         "with_constant_h": False,
         "with_constant_wet_temp": False,
         "with_zones": False
     }
 }
 
-chart_custom_2 = PsychroChart(custom_style)
+chart_custom_2 = PsychroChart.create(custom_style)
 chart_custom_2.plot()
 ```
 
 The custom configuration does not need to include all fields, but only the fields you want to change.
 
 To play with it and see the results, look at this **[notebook with usage examples](https://github.com/azogue/psychrochart/blob/master/notebooks/Usage%20example%20of%20psychrochart.ipynb)**.
 
-## Tests
+## Development and testing
 
 To run the tests, clone the repository, `poetry install` it, and run `poetry run pytest`.
 
+Run `poetry run pre-commit run --all-files` to apply linters for changes in the code 😜.
+
 ## License
 
 [MIT license](https://github.com/azogue/psychrochart/blob/master/LICENSE), so do with it as you like ;-)
 
 ## Included styling examples
 
 **Default style**:
 
-<img src="https://rawgit.com/azogue/psychrochart/master/tests/charts/test_default_psychrochart.svg" width="100%" height="100%">
+<img src="./tests/example-charts/test_default_psychrochart.svg" width="100%" height="100%">
 
-**ASHRAE Handbook black and white style**:
+**ASHRAE Handbook black and white style**: (preset: `ashrae`)
 
-<img src="https://rawgit.com/azogue/psychrochart/master/tests/charts/test_ashrae_psychrochart.svg" width="100%" height="100%">
+<img src="./tests/example-charts/test_ashrae_psychrochart.svg" width="100%" height="100%">
 
-**ASHRAE Handbook black and white style (IP units)**:
+**ASHRAE Handbook black and white style (IP units)**: (preset: `ashrae_ip`)
 
-<img src="https://rawgit.com/azogue/psychrochart/master/tests/charts/test_ashrae_psychrochart_ip.svg" width="100%" height="100%">
+<img src="./tests/example-charts/test_ashrae_psychrochart_ip.svg" width="100%" height="100%">
 
-**Minimal style**:
+**Minimal style**: (preset: `minimal`)
 
-<img src="https://rawgit.com/azogue/psychrochart/master/tests/charts/test_minimal_psychrochart.svg" width="100%" height="100%">
+<img src="./tests/example-charts/test_minimal_psychrochart.svg" width="100%" height="100%">
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

