# Comparing `tmp/plotguy-1.1.tar.gz` & `tmp/plotguy-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plotguy-1.1.tar", last modified: Mon May 29 00:13:52 2023, max compression
+gzip compressed data, was "plotguy-1.1.2.tar", last modified: Mon Jun  5 01:05:10 2023, max compression
```

## Comparing `plotguy-1.1.tar` & `plotguy-1.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-05-29 00:13:52.058445 plotguy-1.1/
--rw-r--r--   0 cmw        (501) staff       (20)      351 2023-05-29 00:13:52.058188 plotguy-1.1/PKG-INFO
--rw-r--r--   0 cmw        (501) staff       (20)        9 2022-09-09 02:08:10.000000 plotguy-1.1/README.md
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-05-29 00:13:52.057246 plotguy-1.1/plotguy/
--rw-r--r--   0 cmw        (501) staff       (20)    25102 2023-05-29 00:11:51.000000 plotguy-1.1/plotguy/__init__.py
--rw-r--r--   0 cmw        (501) staff       (20)    16884 2023-05-22 09:16:53.000000 plotguy-1.1/plotguy/aggregate.py
--rw-r--r--   0 cmw        (501) staff       (20)    64059 2023-05-22 04:48:36.000000 plotguy-1.1/plotguy/components.py
--rw-r--r--   0 cmw        (501) staff       (20)    37762 2023-05-22 04:38:48.000000 plotguy-1.1/plotguy/equity_curves.py
--rw-r--r--   0 cmw        (501) staff       (20)    11123 2023-04-18 03:30:27.000000 plotguy-1.1/plotguy/signals.py
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-05-29 00:13:52.057999 plotguy-1.1/plotguy.egg-info/
--rw-r--r--   0 cmw        (501) staff       (20)      351 2023-05-29 00:13:51.000000 plotguy-1.1/plotguy.egg-info/PKG-INFO
--rw-r--r--   0 cmw        (501) staff       (20)      279 2023-05-29 00:13:51.000000 plotguy-1.1/plotguy.egg-info/SOURCES.txt
--rw-r--r--   0 cmw        (501) staff       (20)        1 2023-05-29 00:13:51.000000 plotguy-1.1/plotguy.egg-info/dependency_links.txt
--rw-r--r--   0 cmw        (501) staff       (20)      131 2023-05-29 00:13:51.000000 plotguy-1.1/plotguy.egg-info/requires.txt
--rw-r--r--   0 cmw        (501) staff       (20)        8 2023-05-29 00:13:51.000000 plotguy-1.1/plotguy.egg-info/top_level.txt
--rw-r--r--   0 cmw        (501) staff       (20)       38 2023-05-29 00:13:52.058492 plotguy-1.1/setup.cfg
--rw-r--r--   0 cmw        (501) staff       (20)      830 2023-05-29 00:13:02.000000 plotguy-1.1/setup.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-05 01:05:10.876574 plotguy-1.1.2/
+-rw-r--r--   0 cmw        (501) staff       (20)      353 2023-06-05 01:05:10.876405 plotguy-1.1.2/PKG-INFO
+-rw-r--r--   0 cmw        (501) staff       (20)        9 2022-09-09 02:08:10.000000 plotguy-1.1.2/README.md
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-05 01:05:10.875410 plotguy-1.1.2/plotguy/
+-rw-r--r--   0 cmw        (501) staff       (20)    25317 2023-06-05 00:25:28.000000 plotguy-1.1.2/plotguy/__init__.py
+-rw-r--r--   0 cmw        (501) staff       (20)    16884 2023-05-22 09:16:53.000000 plotguy-1.1.2/plotguy/aggregate.py
+-rw-r--r--   0 cmw        (501) staff       (20)    64265 2023-06-05 01:01:48.000000 plotguy-1.1.2/plotguy/components.py
+-rw-r--r--   0 cmw        (501) staff       (20)    37809 2023-06-05 00:51:56.000000 plotguy-1.1.2/plotguy/equity_curves.py
+-rw-r--r--   0 cmw        (501) staff       (20)    11123 2023-04-18 03:30:27.000000 plotguy-1.1.2/plotguy/signals.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-05 01:05:10.876182 plotguy-1.1.2/plotguy.egg-info/
+-rw-r--r--   0 cmw        (501) staff       (20)      353 2023-06-05 01:05:10.000000 plotguy-1.1.2/plotguy.egg-info/PKG-INFO
+-rw-r--r--   0 cmw        (501) staff       (20)      279 2023-06-05 01:05:10.000000 plotguy-1.1.2/plotguy.egg-info/SOURCES.txt
+-rw-r--r--   0 cmw        (501) staff       (20)        1 2023-06-05 01:05:10.000000 plotguy-1.1.2/plotguy.egg-info/dependency_links.txt
+-rw-r--r--   0 cmw        (501) staff       (20)      131 2023-06-05 01:05:10.000000 plotguy-1.1.2/plotguy.egg-info/requires.txt
+-rw-r--r--   0 cmw        (501) staff       (20)        8 2023-06-05 01:05:10.000000 plotguy-1.1.2/plotguy.egg-info/top_level.txt
+-rw-r--r--   0 cmw        (501) staff       (20)       38 2023-06-05 01:05:10.876628 plotguy-1.1.2/setup.cfg
+-rw-r--r--   0 cmw        (501) staff       (20)      832 2023-06-05 01:03:52.000000 plotguy-1.1.2/setup.py
```

### Comparing `plotguy-1.1/plotguy/__init__.py` & `plotguy-1.1.2/plotguy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,14 +90,15 @@
         if (date == open_date or date == close_date):
             # open_date and close_date may be the first
             # therefore, process open_date first, then close_date
 
             if date == open_date:
                 # Unrealized pnl on the open date, record on df_daily
                 df_daily.at[open_date, 'action'] = 'open'
+                df_daily.at[open_date, 'signal_value'] = df_daily.at[open_date, 'bah']  # Mark the open position for analysi chart
 
                 unrealized_pnl = num_of_share * multiplier * (now_close - open_price)#  - commission
                 unrealized_pnl = round(unrealized_pnl, 3)
                 df_daily.at[open_date, 'unrealized_pnl'] = unrealized_pnl
 
                 # print(open_date, 'Open!', open_price, now_close, num_of_share, unrealized_pnl)
 
@@ -445,23 +446,24 @@
           .with_columns(pl.col('datetime').alias('date'))
           .with_columns([
         (pl.col('close') * (initial_capital / df.head(1)['close'][0])).alias('bah'),
         pl.lit(None).alias('equity_value'),
         pl.lit(None).alias('action'),
         pl.lit(None).alias('realized_pnl'),
         pl.lit(None).alias('unrealized_pnl'),
+        pl.lit(None).alias('signal_value'),   # for the position of analysis chart
         pl.lit(None).alias('commission'),
     ])
           .collect()
           )
 
     df_daily = df.to_pandas()
     df_daily.index = pd.to_datetime(df_daily['datetime'], format='%Y-%m-%d')
 
-    # Apply apply_pnl on backtes here
+    # Apply apply_pnl on backtest here
     apply_pnl.last_realized_capital = last_realized_capital
     apply_pnl.multiplier = multiplier
     apply_pnl.df_daily = df_daily
 
     df_backtest.apply(apply_pnl, axis=1)
 
     df_daily = apply_pnl.df_daily
```

### Comparing `plotguy-1.1/plotguy/aggregate.py` & `plotguy-1.1.2/plotguy/aggregate.py`

 * *Files identical despite different names*

### Comparing `plotguy-1.1/plotguy/components.py` & `plotguy-1.1.2/plotguy/components.py`

 * *Files 0% similar despite different names*

```diff
@@ -490,16 +490,23 @@
 
         save_path = plotguy.generate_filepath(para_combination=para_combination)
         if file_format == 'parquet':
             df_signal_list = pd.read_parquet(save_path)  # Daraframe that may not be daily
         else:
             df_signal_list = pd.read_csv(save_path, index_col=0)
 
+
         df_signal_list['date'] = pd.to_datetime(df_signal_list['date'], format='%Y-%m-%d')
-        df_signal_list['datetime'] = pd.to_datetime(df_signal_list['datetime'], format='%Y-%m-%d %H:%M:%S')
+
+        try:
+            df_signal_list['datetime'] = pd.to_datetime(df_signal_list['datetime'], format='%Y-%m-%d %H:%M:%S')
+        except:
+            df_signal_list = df_signal_list.reset_index()
+            df_signal_list['datetime'] = pd.to_datetime(df_signal_list['datetime'], format='%Y-%m-%d %H:%M:%S')
+
         df_signal_list = df_signal_list.loc[
             (df_signal_list['date'] >= chart3_start) & (df_signal_list['date'] <= chart3_end)]
 
         df_open = df_signal_list.loc[df_signal_list['action'] == 'open']
         df_profit = df_signal_list.loc[df_signal_list['action'] == 'profit_target']
         df_stop_loss = df_signal_list.loc[df_signal_list['action'] == 'stop_loss']
         df_close = df_signal_list.loc[df_signal_list['action'] == 'close_logic']
```

### Comparing `plotguy-1.1/plotguy/equity_curves.py` & `plotguy-1.1.2/plotguy/equity_curves.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,18 +88,20 @@
         add_button_style = components.add_button_style
         add_button_style_disabled = components.add_button_style_disabled
 
 
 
         app = Dash(__name__, external_stylesheets=[dbc.themes.SUPERHERO], suppress_callback_exceptions=True)
 
-        my_css_data = """body {
+        my_css_data = """
+                body {
                   background-color: #1a2245;
                 }
-                        /* width */
+                
+                /* width */
                 ::-webkit-scrollbar {
                   width: 10px !important;
                   display: block !important;
                 }
 
                 /* Track */
                 ::-webkit-scrollbar-track {
@@ -110,14 +112,15 @@
 
 
                 /* Handle */
                 ::-webkit-scrollbar-thumb {
                   background: #154360;
                   border-radius: 10px;
                 }
+                
                 """
         innerHtmlText = "<style>%s</style>" % my_css_data
 
         app.layout = html.Div([
 
             dash_dangerously_set_inner_html.DangerouslySetInnerHTML(innerHtmlText),
 
@@ -202,15 +205,15 @@
                                  style={'padding': '5px', 'border-radius': '5px', 'background-color': chart_bg, 'display': 'none'}),
 
                         html.Div(id='chart3_dashboard',
                             children=[html.Div(style={'height': '5px', }),
                                   html.Div(children=dbc.Row([
                                                 dbc.Col(width=1),
                                                 dbc.Col(children=html.Div([
-                                                    html.Div(style={'height': '0.5px'}),
+                                                    html.Div(style={'height': '0.5px',}),
                                                     dcc.DatePickerRange(
                                                         id='chart3_date',
                                                         style={'margin-left':'15px'},
                                                         month_format='MMM Do, YY',
                                                         end_date_placeholder_text='MMM Do, YY',
                                                         start_date=datetime.date(self.start_date_datetime.year, self.start_date_datetime.month, self.start_date_datetime.day),
                                                         end_date=datetime.date(self.end_date_datetime.year, self.end_date_datetime.month, self.end_date_datetime.day),)
```

### Comparing `plotguy-1.1/plotguy/signals.py` & `plotguy-1.1.2/plotguy/signals.py`

 * *Files identical despite different names*

### Comparing `plotguy-1.1/setup.py` & `plotguy-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="plotguy",
-    version="1.1",
+    version="1.1.2",
     author="Plotguy Team",
     author_email="plotguy.info@gmail.com",
     description="Plotguy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[         
         'pandas>=1.5.2',
```

