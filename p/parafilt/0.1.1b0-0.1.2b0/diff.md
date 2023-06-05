# Comparing `tmp/parafilt-0.1.1b0.tar.gz` & `tmp/parafilt-0.1.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parafilt-0.1.1b0.tar", last modified: Sun Jun  4 19:54:24 2023, max compression
+gzip compressed data, was "parafilt-0.1.2b0.tar", last modified: Mon Jun  5 04:57:03 2023, max compression
```

## Comparing `parafilt-0.1.1b0.tar` & `parafilt-0.1.2b0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 19:54:24.403200 parafilt-0.1.1b0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-04 19:54:14.000000 parafilt-0.1.1b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-06-04 19:54:24.403200 parafilt-0.1.1b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-06-04 19:54:14.000000 parafilt-0.1.1b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 19:54:24.403200 parafilt-0.1.1b0/parafilt/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-04 19:54:14.000000 parafilt-0.1.1b0/parafilt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-06-04 19:54:14.000000 parafilt-0.1.1b0/parafilt/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6444 2023-06-04 19:54:14.000000 parafilt-0.1.1b0/parafilt/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-04 19:54:14.000000 parafilt-0.1.1b0/parafilt/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 19:54:24.403200 parafilt-0.1.1b0/parafilt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-06-04 19:54:24.000000 parafilt-0.1.1b0/parafilt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-04 19:54:24.000000 parafilt-0.1.1b0/parafilt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 19:54:24.000000 parafilt-0.1.1b0/parafilt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-04 19:54:24.000000 parafilt-0.1.1b0/parafilt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-04 19:54:24.000000 parafilt-0.1.1b0/parafilt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 19:54:24.403200 parafilt-0.1.1b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-04 19:54:14.000000 parafilt-0.1.1b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 04:57:03.027668 parafilt-0.1.2b0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-05 04:56:50.000000 parafilt-0.1.2b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-06-05 04:57:03.027668 parafilt-0.1.2b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-06-05 04:56:50.000000 parafilt-0.1.2b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 04:57:03.023668 parafilt-0.1.2b0/parafilt/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-05 04:56:50.000000 parafilt-0.1.2b0/parafilt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-06-05 04:56:50.000000 parafilt-0.1.2b0/parafilt/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-06-05 04:56:50.000000 parafilt-0.1.2b0/parafilt/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-05 04:56:50.000000 parafilt-0.1.2b0/parafilt/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 04:57:03.027668 parafilt-0.1.2b0/parafilt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-06-05 04:57:03.000000 parafilt-0.1.2b0/parafilt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-05 04:57:03.000000 parafilt-0.1.2b0/parafilt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 04:57:03.000000 parafilt-0.1.2b0/parafilt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-05 04:57:03.000000 parafilt-0.1.2b0/parafilt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-05 04:57:03.000000 parafilt-0.1.2b0/parafilt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 04:57:03.027668 parafilt-0.1.2b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-05 04:56:50.000000 parafilt-0.1.2b0/setup.py
```

### Comparing `parafilt-0.1.1b0/LICENSE` & `parafilt-0.1.2b0/LICENSE`

 * *Files identical despite different names*

### Comparing `parafilt-0.1.1b0/PKG-INFO` & `parafilt-0.1.2b0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parafilt
-Version: 0.1.1b0
+Version: 0.1.2b0
 Summary: ParaFilt is a Python package that provides a collection of parallel adaptive filter implementations for efficient signal processing applications.
 Home-page: https://github.com/nuniz/ParaFilt
 Author: Asaf Zorea
 Author-email: zoreasaf@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -25,16 +25,27 @@
 ## Installation
 To install ParaFilt, you can use `pip`:
 ```
 pip install parafilt
 ```
 
 ## Usage
-Here's an example of how to use the package to create and apply the LMS filter:
+Inputs:
+
+    desired_signal: (batch_size, samples) - Desired signal tensor.
+    input_signal: (samples) - Input tensor.
+
+Returns:
+
+    Tuple containing the estimated output and the error signal (d_est, e).
+	d_est: (batch_size, samples) - Estimated output tensor.
+    e: (batch_size, samples) - Error signal tensor.
 
+
+Here's an example of how to use the package to create and apply the LMS filter:
 ```python
 import parafilt
 
 # Create an instance of the LMS filter
 lms_filter = parafilt.LMS(hop=1024, framelen=4096, filterlen=1024).cuda()
 
 # Perform parallel filter iteration
@@ -60,59 +71,64 @@
 To leverage the parallel algorithm framework, researchers can extend the base classes provided by Parafilt and utilize the parallel computation capabilities provided by PyTorch.
 
 Here's an example of how to use the package to create your own filter:
 ```python
 from parafilt import BaseFilter
 
 class TemplateFilter(BaseFilter):
-    def __init__(self, hop: int, framelen: int, filterlen: int = 1024, weights_delay: Optional[int] = None,
-                 weights_range: (float, float) = (-65535, 65535)):
+    def __init__(self, hop: int, framelen: int, filterlen: int = 1024, weights_delay: Optional[int] = None, 
+	weights_range: (float, float) = (-65535, 65535)):
         '''
         Template filter class that extends the BaseFilter class.
         :param hop: Hop size for frame processing.
         :param framelen: Length of each frame.
         :param filterlen: Length of the filter.
-        :param weights_delay: Delay for the weights, If None, it is set to framelen/2 (default: None).
+        :param weights_delay: Delay for the weights, If None, it is set to framelen-1 (default: None).
         :param weights_range: Range for the filter weights (default: (-65535, 65535)).
         '''
         super().__init__(hop=hop, framelen=framelen, filterlen=filterlen, weights_delay=weights_delay,
                          weights_range=weights_range)
 
     @torch.no_grad()
     def forward_settings(self, d: torch.Tensor, x: torch.Tensor):
         '''
         Placeholder for the settings during forward.
         :param d: Desired signal tensor.
+            Shape: (batch_size, frame_length)
         :param x: Input tensor.
+            Shape: (1, frame_length, filter_length)
         '''
         return
 
     @torch.no_grad()
     def iterate(self, d: torch.Tensor, x: torch.Tensor) -> (torch.Tensor, torch.Tensor):
         '''
         Placeholder for the filter iteration.
         :param d: Desired signal tensor.
             Shape: (batch_size, frame_length)
         :param x: Input tensor.
-            Shape: (batch_size, frame_length, filter_length)
+            Shape: (1, frame_length, filter_length)
         :return:
             torch.Tensor: Estimated output tensor.
                 Shape: (batch_size, frame_length)
             torch.Tensor: Error tensor.
                 Shape: (batch_size, frame_length)
         '''
         raise NotImplementedError
 ```
 
+## Future Work
+- Implementation of CUDA code for the parallel frameworks and filter algorithms to achieve even faster computations.
+- Addition of an option for zero-padding, enabling the output size to match the input size without discarding any samples during the frame decomposition and reconstruction process after performing the filter.
+
+## Citation
+TBD.
 
 ## Contributing
 Contributions are welcome! If you find any issues or have suggestions for improvement, please open an issue or submit a pull request on the GitHub repository.
 
 ## License
-This project is licensed under the MIT License. See the LICENSE file for more information.
-
-## Citation
-TBD.
+This project is licensed under the MIT License. See the [LICENSE file](https://github.com/nuniz/ParaFilt/blob/main/LICENSE) for more information.
 
 ## Contact
 For any inquiries or questions, please contact zoreasaf@gmail.com.
```

### Comparing `parafilt-0.1.1b0/README.md` & `parafilt-0.1.2b0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -10,16 +10,27 @@
 ## Installation
 To install ParaFilt, you can use `pip`:
 ```
 pip install parafilt
 ```
 
 ## Usage
-Here's an example of how to use the package to create and apply the LMS filter:
+Inputs:
+
+    desired_signal: (batch_size, samples) - Desired signal tensor.
+    input_signal: (samples) - Input tensor.
+
+Returns:
+
+    Tuple containing the estimated output and the error signal (d_est, e).
+	d_est: (batch_size, samples) - Estimated output tensor.
+    e: (batch_size, samples) - Error signal tensor.
 
+
+Here's an example of how to use the package to create and apply the LMS filter:
 ```python
 import parafilt
 
 # Create an instance of the LMS filter
 lms_filter = parafilt.LMS(hop=1024, framelen=4096, filterlen=1024).cuda()
 
 # Perform parallel filter iteration
@@ -45,59 +56,64 @@
 To leverage the parallel algorithm framework, researchers can extend the base classes provided by Parafilt and utilize the parallel computation capabilities provided by PyTorch.
 
 Here's an example of how to use the package to create your own filter:
 ```python
 from parafilt import BaseFilter
 
 class TemplateFilter(BaseFilter):
-    def __init__(self, hop: int, framelen: int, filterlen: int = 1024, weights_delay: Optional[int] = None,
-                 weights_range: (float, float) = (-65535, 65535)):
+    def __init__(self, hop: int, framelen: int, filterlen: int = 1024, weights_delay: Optional[int] = None, 
+	weights_range: (float, float) = (-65535, 65535)):
         '''
         Template filter class that extends the BaseFilter class.
         :param hop: Hop size for frame processing.
         :param framelen: Length of each frame.
         :param filterlen: Length of the filter.
-        :param weights_delay: Delay for the weights, If None, it is set to framelen/2 (default: None).
+        :param weights_delay: Delay for the weights, If None, it is set to framelen-1 (default: None).
         :param weights_range: Range for the filter weights (default: (-65535, 65535)).
         '''
         super().__init__(hop=hop, framelen=framelen, filterlen=filterlen, weights_delay=weights_delay,
                          weights_range=weights_range)
 
     @torch.no_grad()
     def forward_settings(self, d: torch.Tensor, x: torch.Tensor):
         '''
         Placeholder for the settings during forward.
         :param d: Desired signal tensor.
+            Shape: (batch_size, frame_length)
         :param x: Input tensor.
+            Shape: (1, frame_length, filter_length)
         '''
         return
 
     @torch.no_grad()
     def iterate(self, d: torch.Tensor, x: torch.Tensor) -> (torch.Tensor, torch.Tensor):
         '''
         Placeholder for the filter iteration.
         :param d: Desired signal tensor.
             Shape: (batch_size, frame_length)
         :param x: Input tensor.
-            Shape: (batch_size, frame_length, filter_length)
+            Shape: (1, frame_length, filter_length)
         :return:
             torch.Tensor: Estimated output tensor.
                 Shape: (batch_size, frame_length)
             torch.Tensor: Error tensor.
                 Shape: (batch_size, frame_length)
         '''
         raise NotImplementedError
 ```
 
+## Future Work
+- Implementation of CUDA code for the parallel frameworks and filter algorithms to achieve even faster computations.
+- Addition of an option for zero-padding, enabling the output size to match the input size without discarding any samples during the frame decomposition and reconstruction process after performing the filter.
+
+## Citation
+TBD.
 
 ## Contributing
 Contributions are welcome! If you find any issues or have suggestions for improvement, please open an issue or submit a pull request on the GitHub repository.
 
 ## License
-This project is licensed under the MIT License. See the LICENSE file for more information.
-
-## Citation
-TBD.
+This project is licensed under the MIT License. See the [LICENSE file](https://github.com/nuniz/ParaFilt/blob/main/LICENSE) for more information.
 
 ## Contact
 For any inquiries or questions, please contact zoreasaf@gmail.com.
```

### Comparing `parafilt-0.1.1b0/parafilt/base.py` & `parafilt-0.1.2b0/parafilt/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,50 +43,55 @@
         self.w *= 0
 
     @torch.no_grad()
     def run_filter(self, x: torch.Tensor) -> torch.Tensor:
         '''
         Apply the filter to the input tensor.
         :param x: Input tensor.
+            Shape: (1, frame_length, filter_length)
         :return:
             torch.Tensor: Filtered output tensor.
         '''
         return torch.einsum('ijk, pjk->ij', self.w, x)
 
     @torch.no_grad()
     def iterate(self, d: torch.Tensor, x: torch.Tensor) -> (torch.Tensor, torch.Tensor):
         '''
         Placeholder for the filter iteration.
         :param d: Desired signal tensor.
             Shape: (batch_size, frame_length)
         :param x: Input tensor.
-            Shape: (batch_size, frame_length, filter_length)
+            Shape: (1, frame_length, filter_length)
         :return:
             torch.Tensor: Estimated output tensor.
                 Shape: (batch_size, frame_length)
             torch.Tensor: Error tensor.
                 Shape: (batch_size, frame_length)
         '''
         raise NotImplementedError
 
     @torch.no_grad()
     def forward_settings(self, d: torch.Tensor, x: torch.Tensor):
         '''
         Placeholder for the settings during forward.
         :param d: Desired signal tensor.
+            Shape: (batch_size, frame_length)
         :param x: Input tensor.
+            Shape: (1, frame_length, filter_length)
         '''
         return
 
     @torch.no_grad()
     def forward(self, d: torch.Tensor, x: torch.Tensor) -> (torch.Tensor, torch.Tensor):
         '''
         Apply the filter to the input signals.
         :param d: Desired signal tensor.
+            Shape: (batch_size, signal_samples)
         :param x: Input tensor.
+            Shape: (signal_samples)
         :return:
             torch.Tensor: Estimated output tensor.
             torch.Tensor: Error tensor.
         '''
         self.reset()
 
         # Input validation
```

### Comparing `parafilt-0.1.1b0/parafilt/filters.py` & `parafilt-0.1.2b0/parafilt/filters.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,37 +7,39 @@
     def __init__(self, hop: int, framelen: int, filterlen: int = 1024, weights_delay: Optional[int] = None,
                  weights_range: (float, float) = (-65535, 65535)):
         '''
         Template filter class that extends the BaseFilter class.
         :param hop: Hop size for frame processing.
         :param framelen: Length of each frame.
         :param filterlen: Length of the filter.
-        :param weights_delay: Delay for the weights, If None, it is set to framelen/2 (default: None).
+        :param weights_delay: Delay for the weights, If None, it is set to framelen-1 (default: None).
         :param weights_range: Range for the filter weights (default: (-65535, 65535)).
         '''
         super().__init__(hop=hop, framelen=framelen, filterlen=filterlen, weights_delay=weights_delay,
                          weights_range=weights_range)
 
     @torch.no_grad()
     def forward_settings(self, d: torch.Tensor, x: torch.Tensor):
         '''
         Placeholder for the settings during forward.
         :param d: Desired signal tensor.
+            Shape: (batch_size, frame_length)
         :param x: Input tensor.
+            Shape: (1, frame_length, filter_length)
         '''
         return
 
     @torch.no_grad()
     def iterate(self, d: torch.Tensor, x: torch.Tensor) -> (torch.Tensor, torch.Tensor):
         '''
         Placeholder for the filter iteration.
         :param d: Desired signal tensor.
             Shape: (batch_size, frame_length)
         :param x: Input tensor.
-            Shape: (batch_size, frame_length, filter_length)
+            Shape: (1, frame_length, filter_length)
         :return:
             torch.Tensor: Estimated output tensor.
                 Shape: (batch_size, frame_length)
             torch.Tensor: Error tensor.
                 Shape: (batch_size, frame_length)
         '''
         raise NotImplementedError
@@ -47,29 +49,31 @@
     def __init__(self, hop: int, framelen: int, filterlen: int = 1024, weights_delay: Optional[int] = None,
                  weights_range: (float, float) = (-65535, 65535), learning_rate: float = 0.01, normalized: bool = True):
         '''
         LMS filter class that extends the BaseFilter class.
         :param hop: Hop size for frame processing.
         :param framelen: Length of each frame.
         :param filterlen: Length of the filter (default: 1024).
-        :param weights_delay: Delay for the weights, If None, it is set to framelen/2 (default: None).
+        :param weights_delay: Delay for the weights, If None, it is set to framelen-1 (default: None).
         :param learning_rate: Learning rate for the LMS algorithm (default: 0.01).
         :param normalized: Flag indicating whether to normalize the input energy (default: True).
         '''
         super().__init__(hop=hop, framelen=framelen, filterlen=filterlen, weights_delay=weights_delay,
                          weights_range=weights_range)
         self.learning_rate = learning_rate
         self.normalized = normalized
 
     @torch.no_grad()
     def iterate(self, d: torch.Tensor, x: torch.Tensor) -> (torch.Tensor, torch.Tensor):
         '''
         Performs one iteration of the LMS algorithm.
         :param d: Desired signal tensor.
+            Shape: (batch_size, frame_length)
         :param x: Input tensor.
+            Shape: (1, frame_length, filter_length)
         :return:
             (torch.Tensor, torch.Tensor): Tuple containing the estimated output and the error signal.
         '''
         d_est = self.run_filter(x)  # Estimated output using the current filter weights
         e = d - d_est  # Compute the error signal
 
         # Update the filter weights using the LMS update rule
@@ -83,15 +87,15 @@
     def __init__(self, hop: int, framelen: int, filterlen: int = 20, weights_delay: Optional[int] = None,
                  weights_range: (float, float) = (-65535, 65535), delta: float = 0.1, lmbd: float = 0.999):
         '''
         RLS filter class that extends the BaseFilter class.
         :param hop: Hop size for frame processing.
         :param framelen: Length of each frame.
         :param filterlen: Length of the filter (default: 20).
-        :param weights_delay: Delay for the weights, If None, it is set to framelen/2 (default: None).
+        :param weights_delay: Delay for the weights, If None, it is set to framelen-1 (default: None).
         :param delta: Forgetting factor delta for the RLS algorithm (default: 0.1).
         :param lmbd: Lambda parameter for the RLS algorithm (default: 0.999).
         '''
         super().__init__(hop=hop, framelen=framelen, filterlen=filterlen, weights_delay=weights_delay,
                          weights_range=weights_range)
         self.delta = delta
         self.lmbd = lmbd
@@ -107,15 +111,17 @@
             self.inverse_correlation.device)
 
     @torch.no_grad()
     def iterate(self, d: torch.Tensor, x: torch.Tensor) -> (torch.Tensor, torch.Tensor):
         '''
         Perform a single iteration of the RLS algorithm.
         :param d: Desired signal tensor.
-        :param x: Input signal tensor.
+            Shape: (batch_size, frame_length)
+        :param x: Input tensor.
+            Shape: (1, frame_length, filter_length)
         :return:
             (torch.Tensor, torch.Tensor): Tuple containing the estimated output and the error signal.
         '''
         d_est = self.run_filter(x)  # Estimated output using the current filter weights
         e = d - d_est  # Compute the error signal
 
         # Update the filter weights using the RLS update rule
@@ -130,11 +136,13 @@
         return d_est, e
 
     @torch.no_grad()
     def forward_settings(self, d: torch.Tensor, x: torch.Tensor):
         '''
         Set the forward settings for the RLS filter.
         :param d: Desired signal tensor.
-        :param x: Input signal tensor.
+            Shape: (batch_size, frame_length)
+        :param x: Input tensor.
+            Shape: (1, frame_length, filter_length)
         '''
         # Repeat inverse_correlation buffer along batch dimension
         self.inverse_correlation = self.inverse_correlation.repeat(d.shape[0], d.shape[1], 1, 1)
```

### Comparing `parafilt-0.1.1b0/parafilt.egg-info/PKG-INFO` & `parafilt-0.1.2b0/parafilt.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parafilt
-Version: 0.1.1b0
+Version: 0.1.2b0
 Summary: ParaFilt is a Python package that provides a collection of parallel adaptive filter implementations for efficient signal processing applications.
 Home-page: https://github.com/nuniz/ParaFilt
 Author: Asaf Zorea
 Author-email: zoreasaf@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -25,16 +25,27 @@
 ## Installation
 To install ParaFilt, you can use `pip`:
 ```
 pip install parafilt
 ```
 
 ## Usage
-Here's an example of how to use the package to create and apply the LMS filter:
+Inputs:
+
+    desired_signal: (batch_size, samples) - Desired signal tensor.
+    input_signal: (samples) - Input tensor.
+
+Returns:
+
+    Tuple containing the estimated output and the error signal (d_est, e).
+	d_est: (batch_size, samples) - Estimated output tensor.
+    e: (batch_size, samples) - Error signal tensor.
 
+
+Here's an example of how to use the package to create and apply the LMS filter:
 ```python
 import parafilt
 
 # Create an instance of the LMS filter
 lms_filter = parafilt.LMS(hop=1024, framelen=4096, filterlen=1024).cuda()
 
 # Perform parallel filter iteration
@@ -60,59 +71,64 @@
 To leverage the parallel algorithm framework, researchers can extend the base classes provided by Parafilt and utilize the parallel computation capabilities provided by PyTorch.
 
 Here's an example of how to use the package to create your own filter:
 ```python
 from parafilt import BaseFilter
 
 class TemplateFilter(BaseFilter):
-    def __init__(self, hop: int, framelen: int, filterlen: int = 1024, weights_delay: Optional[int] = None,
-                 weights_range: (float, float) = (-65535, 65535)):
+    def __init__(self, hop: int, framelen: int, filterlen: int = 1024, weights_delay: Optional[int] = None, 
+	weights_range: (float, float) = (-65535, 65535)):
         '''
         Template filter class that extends the BaseFilter class.
         :param hop: Hop size for frame processing.
         :param framelen: Length of each frame.
         :param filterlen: Length of the filter.
-        :param weights_delay: Delay for the weights, If None, it is set to framelen/2 (default: None).
+        :param weights_delay: Delay for the weights, If None, it is set to framelen-1 (default: None).
         :param weights_range: Range for the filter weights (default: (-65535, 65535)).
         '''
         super().__init__(hop=hop, framelen=framelen, filterlen=filterlen, weights_delay=weights_delay,
                          weights_range=weights_range)
 
     @torch.no_grad()
     def forward_settings(self, d: torch.Tensor, x: torch.Tensor):
         '''
         Placeholder for the settings during forward.
         :param d: Desired signal tensor.
+            Shape: (batch_size, frame_length)
         :param x: Input tensor.
+            Shape: (1, frame_length, filter_length)
         '''
         return
 
     @torch.no_grad()
     def iterate(self, d: torch.Tensor, x: torch.Tensor) -> (torch.Tensor, torch.Tensor):
         '''
         Placeholder for the filter iteration.
         :param d: Desired signal tensor.
             Shape: (batch_size, frame_length)
         :param x: Input tensor.
-            Shape: (batch_size, frame_length, filter_length)
+            Shape: (1, frame_length, filter_length)
         :return:
             torch.Tensor: Estimated output tensor.
                 Shape: (batch_size, frame_length)
             torch.Tensor: Error tensor.
                 Shape: (batch_size, frame_length)
         '''
         raise NotImplementedError
 ```
 
+## Future Work
+- Implementation of CUDA code for the parallel frameworks and filter algorithms to achieve even faster computations.
+- Addition of an option for zero-padding, enabling the output size to match the input size without discarding any samples during the frame decomposition and reconstruction process after performing the filter.
+
+## Citation
+TBD.
 
 ## Contributing
 Contributions are welcome! If you find any issues or have suggestions for improvement, please open an issue or submit a pull request on the GitHub repository.
 
 ## License
-This project is licensed under the MIT License. See the LICENSE file for more information.
-
-## Citation
-TBD.
+This project is licensed under the MIT License. See the [LICENSE file](https://github.com/nuniz/ParaFilt/blob/main/LICENSE) for more information.
 
 ## Contact
 For any inquiries or questions, please contact zoreasaf@gmail.com.
```

### Comparing `parafilt-0.1.1b0/setup.py` & `parafilt-0.1.2b0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="parafilt",
-    version="0.1.1-beta",
+    version="0.1.2-beta",
     author="Asaf Zorea",
     author_email="zoreasaf@gmail.com",
     description="ParaFilt is a Python package that provides a collection of parallel adaptive filter "
                 "implementations for efficient signal processing applications.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
```

