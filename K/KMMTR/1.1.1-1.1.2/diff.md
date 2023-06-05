# Comparing `tmp/KMMTR-1.1.1.tar.gz` & `tmp/KMMTR-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KMMTR-1.1.1.tar", last modified: Mon May 22 00:15:06 2023, max compression
+gzip compressed data, was "KMMTR-1.1.2.tar", last modified: Mon Jun  5 10:25:24 2023, max compression
```

## Comparing `KMMTR-1.1.1.tar` & `KMMTR-1.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-22 00:15:06.228455 KMMTR-1.1.1/
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-22 00:15:06.227547 KMMTR-1.1.1/KMMTR/
--rwxr-xr-x   0 jacob      (501) staff       (20)     6821 2023-05-22 00:14:25.000000 KMMTR-1.1.1/KMMTR/KMM.py
--rwxr-xr-x   0 jacob      (501) staff       (20)     6660 2023-05-21 00:08:25.000000 KMMTR-1.1.1/KMMTR/KMMTR.py
--rwxr-xr-x   0 jacob      (501) staff       (20)      386 2023-04-19 10:18:26.000000 KMMTR-1.1.1/KMMTR/__init__.py
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-22 00:15:06.228146 KMMTR-1.1.1/KMMTR.egg-info/
--rw-r--r--   0 jacob      (501) staff       (20)     1453 2023-05-22 00:15:06.000000 KMMTR-1.1.1/KMMTR.egg-info/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)      208 2023-05-22 00:15:06.000000 KMMTR-1.1.1/KMMTR.egg-info/SOURCES.txt
--rw-r--r--   0 jacob      (501) staff       (20)        1 2023-05-22 00:15:06.000000 KMMTR-1.1.1/KMMTR.egg-info/dependency_links.txt
--rw-r--r--   0 jacob      (501) staff       (20)       33 2023-05-22 00:15:06.000000 KMMTR-1.1.1/KMMTR.egg-info/requires.txt
--rw-r--r--   0 jacob      (501) staff       (20)        6 2023-05-22 00:15:06.000000 KMMTR-1.1.1/KMMTR.egg-info/top_level.txt
--rw-r--r--   0 jacob      (501) staff       (20)     1453 2023-05-22 00:15:06.228316 KMMTR-1.1.1/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)      859 2023-04-20 09:04:07.000000 KMMTR-1.1.1/README.md
--rw-r--r--   0 jacob      (501) staff       (20)       38 2023-05-22 00:15:06.228495 KMMTR-1.1.1/setup.cfg
--rw-r--r--   0 jacob      (501) staff       (20)     1381 2023-05-22 00:14:40.000000 KMMTR-1.1.1/setup.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-06-05 10:25:24.843181 KMMTR-1.1.2/
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-06-05 10:25:24.842284 KMMTR-1.1.2/KMMTR/
+-rwxr-xr-x   0 jacob      (501) staff       (20)     6888 2023-06-05 08:58:37.000000 KMMTR-1.1.2/KMMTR/KMM.py
+-rwxr-xr-x   0 jacob      (501) staff       (20)     6782 2023-06-05 09:01:20.000000 KMMTR-1.1.2/KMMTR/KMMTR.py
+-rwxr-xr-x   0 jacob      (501) staff       (20)      386 2023-04-19 10:18:26.000000 KMMTR-1.1.2/KMMTR/__init__.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-06-05 10:25:24.842876 KMMTR-1.1.2/KMMTR.egg-info/
+-rw-r--r--   0 jacob      (501) staff       (20)     1453 2023-06-05 10:25:24.000000 KMMTR-1.1.2/KMMTR.egg-info/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)      208 2023-06-05 10:25:24.000000 KMMTR-1.1.2/KMMTR.egg-info/SOURCES.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        1 2023-06-05 10:25:24.000000 KMMTR-1.1.2/KMMTR.egg-info/dependency_links.txt
+-rw-r--r--   0 jacob      (501) staff       (20)       33 2023-06-05 10:25:24.000000 KMMTR-1.1.2/KMMTR.egg-info/requires.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        6 2023-06-05 10:25:24.000000 KMMTR-1.1.2/KMMTR.egg-info/top_level.txt
+-rw-r--r--   0 jacob      (501) staff       (20)     1453 2023-06-05 10:25:24.843049 KMMTR-1.1.2/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)      859 2023-04-20 09:04:07.000000 KMMTR-1.1.2/README.md
+-rw-r--r--   0 jacob      (501) staff       (20)       38 2023-06-05 10:25:24.843220 KMMTR-1.1.2/setup.cfg
+-rw-r--r--   0 jacob      (501) staff       (20)     1381 2023-06-05 10:24:35.000000 KMMTR-1.1.2/setup.py
```

### Comparing `KMMTR-1.1.1/KMMTR/KMM.py` & `KMMTR-1.1.2/KMMTR/KMM.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import warnings
 from cvxopt import solvers, matrix 
 from sklearn.gaussian_process import GaussianProcessRegressor as GPR
 from sklearn.gaussian_process.kernels import DotProduct, WhiteKernel, RBF, Matern 
 
 
 class KernelMeanMatching():
-    def __init__(self,kernel,source_data,target_data,target_response):
+    def __init__(self,kernel,source_data,target_data,target_response,powder = 2):
         """
         Constructor for KernelMeanMatching class.
         
         Args:
             kernel (str): Name of the kernel function to use.
             source_data (numpy array): n x d numpy array containing the source data features.
             target_data (numpy array): m x d numpy array containing the target data features.
@@ -19,44 +19,45 @@
         """
         self.kernel = kernel
         # n data points
         self.source_data = source_data
         # m data points
         self.target_data = target_data
         self.target_response = target_response
+        self.powder = powder
         warnings.filterwarnings('ignore')
 
-    def call_kernel(self,para = None):
+    def call_kernel(self, para = None):
         """
         Helper function to call the kernel function specified by the user.
         
         Args:
             para (numpy array): Parameters to use when instantiating the kernel function. Defaults to None.
         
         Returns:
             A kernel function object based on the user-specified kernel function and parameters.
         """
         if para is None :
             if self.kernel == 'RBF':
                 kernel = RBF(length_scale_bounds=(0.01,100))  
             elif self.kernel == 'DotProduct':
-                kernel = DotProduct(sigma_0_bounds=(0.01,100))
+                kernel = DotProduct(sigma_0_bounds=(0.01,100))**self.powder
             elif self.kernel == 'WhiteKernel':
                 kernel = WhiteKernel(noise_level_bounds=(0.01,100))
             elif self.kernel == 'Matern':
                 kernel = Matern(length_scale_bounds=(0.01,100))
             else:
                 print("Unknown kernel !")
                 print('Only the following kernel functions are legal')
                 print('RBF | DotProduct | WhiteKernel | Matern')
         else :
             if self.kernel == 'RBF':
                 kernel = RBF(para,"fixed")
             elif self.kernel == 'DotProduct':
-                kernel = DotProduct(para,"fixed")
+                kernel = DotProduct(para,"fixed")**self.powder
             elif self.kernel == 'WhiteKernel':
                 kernel = WhiteKernel(para,"fixed")
             elif self.kernel == 'Matern':
                 kernel = Matern(para,"fixed")
             else:
                 print("Unknown kernel !")
                 print('Only the following kernel functions are legal')
```

### Comparing `KMMTR-1.1.1/KMMTR/KMMTR.py` & `KMMTR-1.1.2/KMMTR/KMMTR.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         self.UpBound = UpBound
         self.kernel = kernel
         self.S_expt = S_expt
         self.Targets = Targets
         warnings.filterwarnings('ignore')
 
 
-    def fit(self,source_dataset,target_dataset,test_data,tao=None):
+    def fit(self,source_dataset,target_dataset,test_data,tao=None,powder=2):
         """
         Fit the transfer model on source and target datasets and return the predictions
         on the test data along with beta coefficients.
 
         Parameters
         ----------
         source_dataset : array-like of shape (n_samples, n_features)
@@ -82,27 +82,29 @@
             is the number of features including the target variable(s).
         test_data : array-like of shape (n_samples, n_features - Targets)
             The test dataset, where n_samples is the number of samples and n_features
             is the number of features excluding the target variable(s).
         tao : float, default=None
             used in KMM : 1-tao <= sum(beta_i) <= 1+tao , E(beta) = 1 , E is expectation 
             if tao == None, tao =  B/np.sqrt(n), n is the number of source domain data.
+        powder : int, default=2
+            the powder of ploynormal kernel ( viz., DotProduct ** powder)
         Returns
         -------
         predictions : array-like of shape (n_samples,)
             The predicted values for the test data.
         beta : array-like of shape (n_samples,)
             The beta coefficients derived by the KMM weighting scheme.
         """
         source_data = np.array(source_dataset)[:, :-self.Targets]
         source_response = np.array(source_dataset)[:, -self.Targets:]
         target_data = np.array(target_dataset)[:, :-self.Targets]
         target_response = np.array(target_dataset)[:, -self.Targets:]
 
-        KMM = KernelMeanMatching(self.kernel,source_data,target_data,target_response)
+        KMM = KernelMeanMatching(self.kernel,source_data,target_data,target_response,powder)
         beta = KMM.cal_beta(B = self.UpBound,S_expt=self.S_expt,tao=tao)
 
         X = np.concatenate((source_data, target_data), axis=0)
         Y = np.concatenate((source_response, target_response), axis=0)
 
         # test the Regressor
         attribute_list = ['fit', 'predict',]
```

### Comparing `KMMTR-1.1.1/KMMTR.egg-info/PKG-INFO` & `KMMTR-1.1.2/KMMTR.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KMMTR
-Version: 1.1.1
+Version: 1.1.2
 Summary: a transfer learning regression model based on Kernel Mean Matching (KMM) algorithm
 Home-page: https://github.com/Bin-Cao/KMMTransferRegressor
 Author: CaoBin
 Author-email: bcao@shu.edu.com
 Maintainer: CaoBin
 Maintainer-email: binjacobcao@gmail.com
 License: MIT License
```

### Comparing `KMMTR-1.1.1/PKG-INFO` & `KMMTR-1.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KMMTR
-Version: 1.1.1
+Version: 1.1.2
 Summary: a transfer learning regression model based on Kernel Mean Matching (KMM) algorithm
 Home-page: https://github.com/Bin-Cao/KMMTransferRegressor
 Author: CaoBin
 Author-email: bcao@shu.edu.com
 Maintainer: CaoBin
 Maintainer-email: binjacobcao@gmail.com
 License: MIT License
```

### Comparing `KMMTR-1.1.1/README.md` & `KMMTR-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `KMMTR-1.1.1/setup.py` & `KMMTR-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='KMMTR',  # 包名
-    version='1.1.1',  # 版本
+    version='1.1.2',  # 版本
     description="a transfer learning regression model based on Kernel Mean Matching (KMM) algorithm",  # 包简介
     long_description=open('README.md',encoding='utf-8').read(),  # 读取文件中介绍包的详细内容
     include_package_data=True,  # 是否允许上传资源文件
     author='CaoBin',  # 作者
     author_email='bcao@shu.edu.com',  # 作者邮件
     maintainer='CaoBin',  # 维护者
     maintainer_email='binjacobcao@gmail.com',  # 维护者邮件
```

