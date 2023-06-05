# Comparing `tmp/neuroimager-0.0.2.tar.gz` & `tmp/neuroimager-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuroimager-0.0.2.tar", last modified: Mon Jun  5 10:21:58 2023, max compression
+gzip compressed data, was "neuroimager-0.0.3.tar", last modified: Mon Jun  5 13:23:18 2023, max compression
```

## Comparing `neuroimager-0.0.2.tar` & `neuroimager-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 nij       (1000) nij       (1000)        0 2023-06-05 10:21:58.453227 neuroimager-0.0.2/
--rw-r--r--   0 nij       (1000) nij       (1000)      520 2023-06-05 10:21:58.453227 neuroimager-0.0.2/PKG-INFO
--rw-r--r--   0 nij       (1000) nij       (1000)       14 2023-06-05 09:20:11.000000 neuroimager-0.0.2/README.md
-drwxr-xr-x   0 nij       (1000) nij       (1000)        0 2023-06-05 10:21:58.452227 neuroimager-0.0.2/neuroimager.egg-info/
--rw-r--r--   0 nij       (1000) nij       (1000)      520 2023-06-05 10:21:58.000000 neuroimager-0.0.2/neuroimager.egg-info/PKG-INFO
--rw-r--r--   0 nij       (1000) nij       (1000)      324 2023-06-05 10:21:58.000000 neuroimager-0.0.2/neuroimager.egg-info/SOURCES.txt
--rw-r--r--   0 nij       (1000) nij       (1000)        1 2023-06-05 10:21:58.000000 neuroimager-0.0.2/neuroimager.egg-info/dependency_links.txt
--rw-r--r--   0 nij       (1000) nij       (1000)       46 2023-06-05 10:21:58.000000 neuroimager-0.0.2/neuroimager.egg-info/requires.txt
--rw-r--r--   0 nij       (1000) nij       (1000)       21 2023-06-05 10:21:58.000000 neuroimager-0.0.2/neuroimager.egg-info/top_level.txt
-drwxr-xr-x   0 nij       (1000) nij       (1000)        0 2023-06-05 10:21:58.453227 neuroimager-0.0.2/pipes/
--rw-r--r--   0 nij       (1000) nij       (1000)        1 2023-06-05 10:04:05.000000 neuroimager-0.0.2/pipes/__init__.py
--rw-r--r--   0 nij       (1000) nij       (1000)     1173 2023-06-03 12:41:44.000000 neuroimager-0.0.2/pipes/brainage.py
--rw-r--r--   0 nij       (1000) nij       (1000)     6684 2023-06-04 11:19:58.000000 neuroimager-0.0.2/pipes/cca.py
-drwxr-xr-x   0 nij       (1000) nij       (1000)        0 2023-06-05 10:21:58.453227 neuroimager-0.0.2/plotting/
--rw-r--r--   0 nij       (1000) nij       (1000)        1 2023-06-05 10:04:05.000000 neuroimager-0.0.2/plotting/__init__.py
--rw-r--r--   0 nij       (1000) nij       (1000)     1022 2023-06-04 11:09:38.000000 neuroimager-0.0.2/plotting/plot.py
--rw-r--r--   0 nij       (1000) nij       (1000)       38 2023-06-05 10:21:58.453227 neuroimager-0.0.2/setup.cfg
--rw-r--r--   0 nij       (1000) nij       (1000)      777 2023-06-05 10:21:53.000000 neuroimager-0.0.2/setup.py
-drwxr-xr-x   0 nij       (1000) nij       (1000)        0 2023-06-05 10:21:58.453227 neuroimager-0.0.2/utils/
--rw-r--r--   0 nij       (1000) nij       (1000)        1 2023-06-05 10:04:31.000000 neuroimager-0.0.2/utils/__init__.py
--rw-r--r--   0 nij       (1000) nij       (1000)     1080 2023-06-04 07:27:48.000000 neuroimager-0.0.2/utils/atlas.py
--rw-r--r--   0 nij       (1000) nij       (1000)     4161 2023-06-04 11:49:18.000000 neuroimager-0.0.2/utils/fc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:23:18.334555 neuroimager-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-05 13:23:18.334555 neuroimager-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-05 13:23:04.000000 neuroimager-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:23:18.330555 neuroimager-0.0.3/neuroimager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-05 13:23:18.000000 neuroimager-0.0.3/neuroimager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-05 13:23:18.000000 neuroimager-0.0.3/neuroimager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 13:23:18.000000 neuroimager-0.0.3/neuroimager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-05 13:23:18.000000 neuroimager-0.0.3/neuroimager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-05 13:23:18.000000 neuroimager-0.0.3/neuroimager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:23:18.334555 neuroimager-0.0.3/pipes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 13:23:04.000000 neuroimager-0.0.3/pipes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-05 13:23:04.000000 neuroimager-0.0.3/pipes/brainage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7085 2023-06-05 13:23:04.000000 neuroimager-0.0.3/pipes/cca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:23:18.334555 neuroimager-0.0.3/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-05 13:23:04.000000 neuroimager-0.0.3/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-05 13:23:04.000000 neuroimager-0.0.3/plotting/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 13:23:18.334555 neuroimager-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-05 13:23:04.000000 neuroimager-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:23:18.334555 neuroimager-0.0.3/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-05 13:23:04.000000 neuroimager-0.0.3/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-05 13:23:04.000000 neuroimager-0.0.3/utils/atlas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-06-05 13:23:04.000000 neuroimager-0.0.3/utils/fc.py
```

### Comparing `neuroimager-0.0.2/PKG-INFO` & `neuroimager-0.0.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 Metadata-Version: 2.1
 Name: neuroimager
-Version: 0.0.2
+Version: 0.0.3
 Summary: A collection of utilities used for MRI data analysis
-Author: Wetiqe@GitHub
+Author: Wetiqe
 Author-email: jzni132134@gmail.com
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
+
+# neuroimager
+
+A collection of utilities used for MRI data analysis
```

### Comparing `neuroimager-0.0.2/neuroimager.egg-info/PKG-INFO` & `neuroimager-0.0.3/neuroimager.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 Metadata-Version: 2.1
 Name: neuroimager
-Version: 0.0.2
+Version: 0.0.3
 Summary: A collection of utilities used for MRI data analysis
-Author: Wetiqe@GitHub
+Author: Wetiqe
 Author-email: jzni132134@gmail.com
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
+
+# neuroimager
+
+A collection of utilities used for MRI data analysis
```

### Comparing `neuroimager-0.0.2/pipes/brainage.py` & `neuroimager-0.0.3/pipes/brainage.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,33 @@
+import numpy as np
 from sklearn.linear_model import LinearRegression
 from sklearn.preprocessing import PolynomialFeatures
 
+
 def BAG(train_pred, test_pred, train_y, test_y):
-    '''
+    """
     Brain Age Gap Correction
 
     Parameters:
     train_pred (numpy array): Predicted age on the training set.
     test_pred (numpy array): Predicted age on the test set.
     train_y (numpy array): Actual age in the training set.
     test_y (numpy array): Actual age in the test set.
 
     Returns:
     corrected_age (numpy array): Corrected predicted age on the test set.
     train_delta_age (numpy array): Difference between predicted and actual age on the training set.
     line_reg (LinearRegression object): Trained regression model.
-    '''
+    """
 
     line_reg = LinearRegression()
     poly = PolynomialFeatures(degree=1, include_bias=True)
-    line_reg_features = poly.fit_transform(train_y.reshape(-1,1))
-    line_reg.fit(line_reg_features, train_pred.reshape(-1,1))
+    line_reg_features = poly.fit_transform(train_y.reshape(-1, 1))
+    line_reg.fit(line_reg_features, train_pred.reshape(-1, 1))
 
-    test_features = poly.transform(test_y.reshape(-1,1))
-    corrected_delta_age = test_pred - np.array(line_reg.predict(test_features)).flatten()
+    test_features = poly.transform(test_y.reshape(-1, 1))
+    corrected_delta_age = (
+        test_pred - np.array(line_reg.predict(test_features)).flatten()
+    )
     corrected_age = test_y + corrected_delta_age
 
     return corrected_age, corrected_delta_age
```

### Comparing `neuroimager-0.0.2/pipes/cca.py` & `neuroimager-0.0.3/pipes/cca.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import numpy as np
 import pandas as pd
 from sklearn.cross_decomposition import CCA
 import seaborn as sns
 from matplotlib import pyplot as plt
-
+from scipy.stats import pearsonr
+from plotting import density_scatter
 
 
 def permutation_test_cca(X, Y, n_components=1, n_permutations=1000, random_state=None):
     """
     Perform a permutation test for Canonical Correlation Analysis (CCA) to assess the significance
     of the correlation between two sets of features.
 
@@ -38,142 +39,184 @@
     np.random.seed(random_state)
 
     # Fit the CCA model
     cca = CCA(n_components=n_components)
     X_c, Y_c = cca.fit_transform(X, Y)
 
     # Compute the original correlations
-    original_correlations = [pearsonr(X_c[:, i], Y_c[:, i])[0] for i in range(n_components)]
+    original_correlations = [
+        pearsonr(X_c[:, i], Y_c[:, i])[0] for i in range(n_components)
+    ]
 
     # Perform the permutation test
     count_better_correlations = [0] * n_components
-    seeds=np.random.randint(0,100000,n_permutations)
-    rs = []; p_values = []
+    seeds = np.random.randint(0, 100000, n_permutations)
+    rs = []
+    p_values = []
     for i, seed in enumerate(seeds):
         np.random.seed(seed)
-        
+
         ids = np.random.permutation(X.shape[0])
-        x_perm = X[ids,:]
+        x_perm = X[ids, :]
         cca_perm = CCA(n_components=n_components)
         X_perm, Y_perm = cca_perm.fit_transform(x_perm, Y)
         rs.append(pd.DataFrame(X_perm).corrwith(pd.DataFrame(Y_perm)))
     r_permuted_values = pd.DataFrame(rs)
     for i in range(n_components):
-        p_value = (abs(r_permuted_values.iloc[:,i]) > abs(original_correlations[i])).sum() / r_permuted_values.shape[0]
+        p_value = (
+            abs(r_permuted_values.iloc[:, i]) > abs(original_correlations[i])
+        ).sum() / r_permuted_values.shape[0]
         p_values.append(p_value)
 
     return cca, X_c, Y_c, original_correlations, p_values
-    
+
 
 def plot_cca_scatter(transformed_X, transformed_Y, n_components=1, **kwargs):
     """
     Plots Canonical Correlation Analysis (CCA) scatter plot.
 
     Parameters:
     transformed_X (array-like): Transformed X data from CCA.
     transformed_Y (array-like): Transformed Y data from CCA.
     n_components (int): Number of components to plot.
 
     Returns:
     None
     """
-    fig_size = kwargs.get('fig_size', (10, 10))
-    marker = kwargs.get('marker', 'o')
-    color = kwargs.get('color', 'b')
-    xlabel = kwargs.get('xlabel', None)
-    ylabel = kwargs.get('ylabel', None)
-    title_prefix = kwargs.get('title_prefix', 'Scatter plot of CCA components')
-    layout = kwargs.get('layout', 'tight')
-    p_values = kwargs.get('p_values', None)
+    fig_size = kwargs.get("fig_size", (10, 10))
+    marker = kwargs.get("marker", "o")
+    color = kwargs.get("color", "b")
+    xlabel = kwargs.get("xlabel", None)
+    ylabel = kwargs.get("ylabel", None)
+    title_prefix = kwargs.get("title_prefix", "Scatter plot of CCA components")
+    layout = kwargs.get("layout", "tight")
+    p_values = kwargs.get("p_values", None)
     for i in range(n_components):
         # plt.scatter(transformed_X[:, i], transformed_Y[:, i], marker=marker, color=color, label=f'Component {i+1}')
-        desity_scatter(transformed_X[:, i], transformed_Y[:, i],display=False)
+        density_scatter(transformed_X[:, i], transformed_Y[:, i], display=False)
         corr_coef = np.corrcoef(transformed_X[:, i], transformed_Y[:, i])[0, 1]
-        if kwargs.get('xlabel', False) & kwargs.get('ylabel', False):
-            title = f"{title_prefix}: {xlabel} vs {ylabel} pearson r = {corr_coef}" 
+        if kwargs.get("xlabel", False) & kwargs.get("ylabel", False):
+            title = f"{title_prefix}: {xlabel} vs {ylabel} pearson r = {corr_coef}"
             if p_values:
-                title += f" p = {p_values[i]}" 
+                title += f" p = {p_values[i]}"
             plt.title(title)
         else:
-            title = f'Component {i + 1}: pearson r = {corr_coef}'
+            title = f"Component {i + 1}: pearson r = {corr_coef}"
             if p_values:
-                title += f" p = {p_values[i]}" 
+                title += f" p = {p_values[i]}"
             plt.title(title)
         if not xlabel:
-            xlabel = 'X Component {}'.format(i + 1) 
+            xlabel = "X Component {}".format(i + 1)
         if not ylabel:
-            ylabel = 'Y Component {}'.format(i + 1)
+            ylabel = "Y Component {}".format(i + 1)
         plt.xlabel(xlabel)
         plt.ylabel(ylabel)
         plt.tight_layout()
         plt.show()
-        
-        
 
-def plot_cca_weights(weights, labels, ax=False,display_thresh=0.2, show=False, min_font_size=6, scaling_factor=50, **kwargs):
-    xlim = kwargs.get("xlim",(-1,1))
-    xlabel = kwargs.get("xlabel","")
-    title = kwargs.get("title","")
+
+def plot_cca_weights(
+    weights,
+    labels,
+    ax=False,
+    display_thresh=0.2,
+    show=False,
+    min_font_size=6,
+    scaling_factor=50,
+    **kwargs,
+):
+    xlim = kwargs.get("xlim", (-1, 1))
+    xlabel = kwargs.get("xlabel", "")
+    title = kwargs.get("title", "")
     if not ax:
         fig, ax = plt.subplots(figsize=(8, 5))
     weights = weights.flatten()
     # Sort weights and labels for X features
     sorted_indices = np.argsort(weights)
     sorted_weights = weights[sorted_indices]
     if labels is not None:
         sorted_labels = [labels[idx] for idx in sorted_indices]
-        
+
     # Plot X feature weights
-    ax.set_ylabel('Weights')
-    ax.set_xlim(xlim[0],xlim[1])
+    ax.set_ylabel("Weights")
+    ax.set_xlim(xlim[0], xlim[1])
     ax.set_ylim(-0.5, len(weights) + 0.5)
     ax.set_xlabel(xlabel)
     ax.set_title(title)
 
     texts = []
     for i, label in enumerate(sorted_labels):
-        if abs(sorted_weights[i])<display_thresh:
+        if abs(sorted_weights[i]) < display_thresh:
             continue
         font_size = max(min_font_size, abs(sorted_weights[i]) * scaling_factor)
-        ax.text(0, i, label + f'  weights {round(sorted_weights[i],2)}', ha='center', va='center', fontsize=font_size)
+        ax.text(
+            0,
+            i,
+            label + f"  weights {round(sorted_weights[i],2)}",
+            ha="center",
+            va="center",
+            fontsize=font_size,
+        )
 
     # adjust_text(texts,only_move={ 'text':'X'})
-    ax.spines['top'].set_visible(False)
-    ax.spines['left'].set_visible(False)
-    ax.spines['right'].set_visible(False)
-    ax.spines['bottom'].set_visible(False)
+    ax.spines["top"].set_visible(False)
+    ax.spines["left"].set_visible(False)
+    ax.spines["right"].set_visible(False)
+    ax.spines["bottom"].set_visible(False)
     ax.set_xticks([])
     ax.set_yticks([])
 
     if show:
         plt.show()
-    
-    return ax
 
+    return ax
 
 
-def plot_paired_cca_weights(weights_X, weights_Y,display_thresh=0.2, scaling_factor=30, x_labels=None, y_labels=None, **kwargs):
+def plot_paired_cca_weights(
+    weights_X,
+    weights_Y,
+    display_thresh=0.2,
+    scaling_factor=30,
+    x_labels=None,
+    y_labels=None,
+    **kwargs,
+):
     """
     Plots Canonical Correlation Analysis (CCA) feature weights.
 
     Parameters:
     weights_X (array-like): Weights for X features.
     weights_Y (array-like): Weights for Y features.
     x_labels (list, optional): Labels for X features. Defaults to None.
     y_labels (list, optional): Labels for Y features. Defaults to None.
 
     Returns:
     None
     """
-    figsize=kwargs.get("fig_size", (10,5))
+    figsize = kwargs.get("fig_size", (10, 5))
     n_components = weights_X.shape[1]
-    
+
     for i in range(n_components):
         fig, (ax1, ax2) = plt.subplots(1, 2, figsize=figsize)
-        plot_cca_weights(weights_X[:, i], x_labels, ax=ax1, display_thresh=display_thresh, min_font_size=6, scaling_factor=scaling_factor,\
-                         xlim=(-1,1),xlabel='X Features', title='Component {} X feature weights'.format(i + 1))
-        plot_cca_weights(weights_Y[:, i], y_labels, ax=ax2, display_thresh=display_thresh, min_font_size=6, scaling_factor=scaling_factor,\
-                         xlabel='Y Features', title='Component {} Y feature weights'.format(i + 1))
+        plot_cca_weights(
+            weights_X[:, i],
+            x_labels,
+            ax=ax1,
+            display_thresh=display_thresh,
+            min_font_size=6,
+            scaling_factor=scaling_factor,
+            xlim=(-1, 1),
+            xlabel="X Features",
+            title="Component {} X feature weights".format(i + 1),
+        )
+        plot_cca_weights(
+            weights_Y[:, i],
+            y_labels,
+            ax=ax2,
+            display_thresh=display_thresh,
+            min_font_size=6,
+            scaling_factor=scaling_factor,
+            xlabel="Y Features",
+            title="Component {} Y feature weights".format(i + 1),
+        )
         plt.tight_layout()
         plt.show()
-
-
```

### Comparing `neuroimager-0.0.2/plotting/plot.py` & `neuroimager-0.0.3/plotting/plot.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 import numpy as np
 from matplotlib import pyplot as plt
 import seaborn as sns
 from scipy.stats import gaussian_kde
 
 
-def desity_scatter(x,y, reg=True, gaussian_density=True,figsize=(10,10), display=True, **kwargs):
+def density_scatter(
+    x, y, reg=True, gaussian_density=True, figsize=(10, 10), display=True, **kwargs
+):
     xy = np.vstack([x, y])
     if gaussian_density:
         z = gaussian_kde(xy)(xy)
     else:
         H, x_edges, y_edges = np.histogram2d(x, y)
         x_centers = (x_edges[:-1] + x_edges[1:]) / 2
         y_centers = (y_edges[:-1] + y_edges[1:]) / 2
-        
+
         # Convert the histogram to a 2D array of densities
         dx = x_centers[1] - x_centers[0]
         dy = y_centers[1] - y_centers[0]
         z = H / (dx * dy)
     # Create the scatter plot with density-based coloring
     fig, ax = plt.subplots(figsize=figsize)
     sc = ax.scatter(x=x, y=y, c=z, cmap="viridis", **kwargs)
-    sns.regplot(x=x, y=y, scatter=False, ax=ax, color='black')
+    sns.regplot(x=x, y=y, scatter=False, ax=ax, color="black")
 
     # Add a colorbar to the figure
     cbar = plt.colorbar(sc)
-    cbar.set_label('Density')
+    cbar.set_label("Density")
     if display:
         plt.show()
-    
+
     return fig, ax
```

### Comparing `neuroimager-0.0.2/utils/atlas.py` & `neuroimager-0.0.3/utils/atlas.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 import re
 import pandas as pd
 
 
 def split_schafer_names(file_path):
-	"""
-	This function reads a CSV file containing Schafer parcellation data and extracts the hemisphere, network, and subregion
-	information from the ROI names. The extracted information is added as new columns to the DataFrame and the updated
-	DataFrame is returned.
-
-	Args:
-		file_path (str): The path to the CSV file containing Schafer parcellation data.
-
-	Returns:
-		pd.DataFrame: A DataFrame containing the original Schafer parcellation data with additional columns for
-		              'Hemisphere', 'Network', and 'Subregion' extracted from the ROI names.
-	"""
+    """
+    This function reads a CSV file containing Schafer parcellation data and extracts the hemisphere, network, and subregion
+    information from the ROI names. The extracted information is added as new columns to the DataFrame and the updated
+    DataFrame is returned.
+
+    Args:
+        file_path (str): The path to the CSV file containing Schafer parcellation data.
+
+    Returns:
+        pd.DataFrame: A DataFrame containing the original Schafer parcellation data with additional columns for
+                      'Hemisphere', 'Network', and 'Subregion' extracted from the ROI names.
+    """
     schafer = pd.read_csv(file_path)
-    regex_pattern = r'(RH|LH)_([A-Za-z]+)(?:_([A-Za-z]+))?(?:_[A-Za-z]+)*'
+    regex_pattern = r"(RH|LH)_([A-Za-z]+)(?:_([A-Za-z]+))?(?:_[A-Za-z]+)*"
+
     def parse_roi_name(roi_name):
         match = re.search(regex_pattern, roi_name)
         if match:
             return match.group(1), match.group(2), match.group(3)
         return None, None, None
 
-    schafer[['Hemisphere', 'Network', 'Subregion']] = schafer['ROI Name'].apply(parse_roi_name).apply(pd.Series)
+    schafer[["Hemisphere", "Network", "Subregion"]] = (
+        schafer["ROI Name"].apply(parse_roi_name).apply(pd.Series)
+    )
 
     return schafer
```

### Comparing `neuroimager-0.0.2/utils/fc.py` & `neuroimager-0.0.3/utils/fc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import numpy as np
-import pandas as pd
 import math
 
 
-def filt_fcs(fcs, coords, network_col='Network', excludes: list = None, includes: list = None):
-    '''Filter FC matrix based on network labels
+def filt_fcs(
+    fcs, coords, network_col="Network", excludes: list = None, includes: list = None
+):
+    """Filter FC matrix based on network labels
     :param fcs: A numpy matrix shaped (n_subjs, n_nodes, n_nodes) representing the functional connectivity data.
     :param coords: A DataFrame containing the coordinates and network labels for each node.
     :param network_col: A string representing the column name in the coords DataFrame that contains the network labels. Default is 'Network'.
     :param excludes: A list of network labels to exclude from the filtered FC matrix. Default is None.
     :param includes: A list of network labels to include in the filtered FC matrix. Default is None.
     :return: A filtered numpy matrix containing only the desired network labels.
 
     This function filters the input functional connectivity matrix based on the specified network labels.
     It can be used to include or exclude specific networks from the analysis.
-    '''
+    """
     if includes is not None and excludes is not None:
         raise ValueError("Only one of 'includes' and 'excludes' can be specified.")
     elif excludes is None:
         excludes = []
     elif includes is None:
         includes = []
 
@@ -29,18 +30,18 @@
         ind = get_coords_index(coords, network_col, includes)
         indexer = np.ix_(np.arange(fcs.shape[0]), ind, ind)
         fcs = fcs[indexer]
     elif excludes:
         ind = get_coords_index(coords, network_col, excludes)
         fcs = np.delete(fcs, ind, axis=1)
         fcs = np.delete(fcs, ind, axis=2)
-    
+
     return fcs
-    
-    
+
+
 def flatten_lower_triangular(matrix):
     """
     This function takes a 2D or 3D numpy array representing one or multiple square matrices as input and returns a 2D numpy array
     where each row corresponds to the flattened lower triangular part of a matrix in the input. The diagonal and upper triangular
     elements of each input matrix are excluded from the output.
 
     Parameters:
@@ -51,15 +52,17 @@
     with diagonal and upper triangular elements excluded.
     """
     if len(matrix.shape) == 2:
         matrix = np.array([matrix])
     elif len(matrix.shape) != 3:
         raise ValueError("Input matrix must be 2D or 3D")
 
-    tril_matrices = np.array([np.tril(fc, k=-1) for fc in matrix]).reshape(matrix.shape[0], -1)
+    tril_matrices = np.array([np.tril(fc, k=-1) for fc in matrix]).reshape(
+        matrix.shape[0], -1
+    )
     flat_matrices = tril_matrices[:, ~np.all(tril_matrices == 0, axis=0)]
 
     return flat_matrices
 
 
 def unflatten_lower_triangular(flat_matrices, n):
     """
@@ -85,14 +88,15 @@
         discriminant = 1 + 8 * n
         if discriminant < 0:
             raise ValueError("No real solution for n")
         else:
             n1 = (1 + math.sqrt(discriminant)) / 2
             n2 = (1 - math.sqrt(discriminant)) / 2
             return n1, n2
+
     n = int(calculate_orig_n(n)[0])
     tril_indices = np.tril_indices(n, k=-1)
     original_shape_matrices = np.zeros((m, n, n))
 
     for i in range(m):
         original_shape_matrices[i][tril_indices] = flat_matrices[i, :]
```

