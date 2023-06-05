# Comparing `tmp/keras-cortex-0.0.7.tar.gz` & `tmp/keras-cortex-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras-cortex-0.0.7.tar", last modified: Fri Mar 17 11:21:30 2023, max compression
+gzip compressed data, was "keras-cortex-0.0.8.tar", last modified: Mon Jun  5 11:37:41 2023, max compression
```

## Comparing `keras-cortex-0.0.7.tar` & `keras-cortex-0.0.8.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-03-17 11:21:30.416798 keras-cortex-0.0.7/
--rw-rw-r--   0 weidler   (1000) weidler   (1000)    11357 2022-09-16 08:55:55.000000 keras-cortex-0.0.7/LICENSE
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     1562 2023-03-17 11:21:30.416798 keras-cortex-0.0.7/PKG-INFO
--rw-rw-r--   0 weidler   (1000) weidler   (1000)      767 2022-09-16 12:24:13.000000 keras-cortex-0.0.7/README.md
-drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-03-17 11:21:30.416798 keras-cortex-0.0.7/keras_cortex/
--rw-rw-r--   0 weidler   (1000) weidler   (1000)       27 2022-09-16 13:04:20.000000 keras-cortex-0.0.7/keras_cortex/__init__.py
-drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-03-17 11:21:30.416798 keras-cortex-0.0.7/keras_cortex/cornet/
--rw-rw-r--   0 weidler   (1000) weidler   (1000)      120 2022-10-10 15:54:44.000000 keras-cortex-0.0.7/keras_cortex/cornet/__init__.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     4260 2023-03-15 08:24:23.000000 keras-cortex-0.0.7/keras_cortex/cornet/cornet_s.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     3550 2023-03-17 10:26:25.000000 keras-cortex-0.0.7/keras_cortex/cornet/cornet_z.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)      273 2022-10-11 09:42:24.000000 keras-cortex-0.0.7/keras_cortex/cornet/util.py
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     1602 2023-03-17 11:12:40.000000 keras-cortex-0.0.7/keras_cortex/layers.py
-drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-03-17 11:21:30.416798 keras-cortex-0.0.7/keras_cortex.egg-info/
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     1562 2023-03-17 11:21:30.000000 keras-cortex-0.0.7/keras_cortex.egg-info/PKG-INFO
--rw-rw-r--   0 weidler   (1000) weidler   (1000)      397 2023-03-17 11:21:30.000000 keras-cortex-0.0.7/keras_cortex.egg-info/SOURCES.txt
--rw-rw-r--   0 weidler   (1000) weidler   (1000)        1 2023-03-17 11:21:30.000000 keras-cortex-0.0.7/keras_cortex.egg-info/dependency_links.txt
--rw-rw-r--   0 weidler   (1000) weidler   (1000)       18 2023-03-17 11:21:30.000000 keras-cortex-0.0.7/keras_cortex.egg-info/requires.txt
--rw-rw-r--   0 weidler   (1000) weidler   (1000)       13 2023-03-17 11:21:30.000000 keras-cortex-0.0.7/keras_cortex.egg-info/top_level.txt
--rw-rw-r--   0 weidler   (1000) weidler   (1000)       38 2023-03-17 11:21:30.416798 keras-cortex-0.0.7/setup.cfg
--rw-rw-r--   0 weidler   (1000) weidler   (1000)     1158 2023-03-17 11:18:42.000000 keras-cortex-0.0.7/setup.py
-drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-03-17 11:21:30.416798 keras-cortex-0.0.7/test/
--rw-rw-r--   0 weidler   (1000) weidler   (1000)      377 2022-09-16 09:02:40.000000 keras-cortex-0.0.7/test/test_cornet.py
+drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-06-05 11:37:41.807950 keras-cortex-0.0.8/
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)    11357 2022-09-16 08:55:55.000000 keras-cortex-0.0.8/LICENSE
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     1562 2023-06-05 11:37:41.807950 keras-cortex-0.0.8/PKG-INFO
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)      767 2022-09-16 12:24:13.000000 keras-cortex-0.0.8/README.md
+drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-06-05 11:37:41.807950 keras-cortex-0.0.8/keras_cortex/
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)       27 2022-09-16 13:04:20.000000 keras-cortex-0.0.8/keras_cortex/__init__.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)        0 2023-03-21 18:22:36.000000 keras-cortex-0.0.8/keras_cortex/activations.py
+drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-06-05 11:37:41.807950 keras-cortex-0.0.8/keras_cortex/cornet/
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)      120 2022-10-10 15:54:44.000000 keras-cortex-0.0.8/keras_cortex/cornet/__init__.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     4262 2023-05-23 14:23:56.000000 keras-cortex-0.0.8/keras_cortex/cornet/cornet_s.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     6011 2023-03-21 18:35:11.000000 keras-cortex-0.0.8/keras_cortex/cornet/cornet_z.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)      273 2022-10-11 09:42:24.000000 keras-cortex-0.0.8/keras_cortex/cornet/util.py
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     1822 2023-05-23 13:08:02.000000 keras-cortex-0.0.8/keras_cortex/layers.py
+drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-06-05 11:37:41.807950 keras-cortex-0.0.8/keras_cortex.egg-info/
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     1562 2023-06-05 11:37:41.000000 keras-cortex-0.0.8/keras_cortex.egg-info/PKG-INFO
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)      425 2023-06-05 11:37:41.000000 keras-cortex-0.0.8/keras_cortex.egg-info/SOURCES.txt
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)        1 2023-06-05 11:37:41.000000 keras-cortex-0.0.8/keras_cortex.egg-info/dependency_links.txt
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)       11 2023-06-05 11:37:41.000000 keras-cortex-0.0.8/keras_cortex.egg-info/requires.txt
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)       13 2023-06-05 11:37:41.000000 keras-cortex-0.0.8/keras_cortex.egg-info/top_level.txt
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)       38 2023-06-05 11:37:41.807950 keras-cortex-0.0.8/setup.cfg
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)     1151 2023-06-05 11:36:31.000000 keras-cortex-0.0.8/setup.py
+drwxrwxr-x   0 weidler   (1000) weidler   (1000)        0 2023-06-05 11:37:41.807950 keras-cortex-0.0.8/test/
+-rw-rw-r--   0 weidler   (1000) weidler   (1000)      377 2022-09-16 09:02:40.000000 keras-cortex-0.0.8/test/test_cornet.py
```

### Comparing `keras-cortex-0.0.7/LICENSE` & `keras-cortex-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `keras-cortex-0.0.7/PKG-INFO` & `keras-cortex-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-cortex
-Version: 0.0.7
+Version: 0.0.8
 Summary: Keras Implementations of Goal-driven models of (parts of) cortex
 Home-page: https://github.com/weidler/keras-cortex
 Author: Tonio Weidler
 Author-email: research@tonioweidler.de
 License: Apache-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `keras-cortex-0.0.7/README.md` & `keras-cortex-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `keras-cortex-0.0.7/keras_cortex/cornet/cornet_s.py` & `keras-cortex-0.0.8/keras_cortex/cornet/cornet_s.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
             tf.keras.layers.ReLU(name='nonlin2'),
             Identity(name='output')
         ], name='V1'),
         CORBlockS(64, 128, times=2, name='V2'),
         CORBlockS(128, 256, times=4, name='V4'),
         CORBlockS(256, 512, times=2, name='IT'),
         tf.keras.Sequential([
-            keras_cortex.layers.SpatialSoftmax(),
+            # keras_cortex.layers.SpatialSoftmax(),
             tf.keras.layers.Flatten(name='flatten'),
             tf.keras.layers.Dense(output_dim, name='linear'),
             Identity(name="output")
         ], name='decoder')
     ])
 
     return model
```

### Comparing `keras-cortex-0.0.7/keras_cortex/cornet/cornet_z.py` & `keras-cortex-0.0.8/keras_cortex/cornet/cornet_z.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,20 +14,20 @@
         self.conv = tf.keras.layers.Conv2D(out_channels, kernel_size=kernel_size, strides=stride,
                                            kernel_initializer=tf.keras.initializers.GlorotUniform(),
                                            bias_initializer=tf.keras.initializers.Constant(0),
                                            kernel_regularizer=tf.keras.regularizers.L2(0.001),
                                            bias_regularizer=tf.keras.regularizers.L2(0.001))
         self.nonlin = tf.keras.layers.ReLU()
         self.pad2 = tf.keras.layers.ZeroPadding2D((1, 1))
-        # self.pool = tf.keras.layers.MaxPool2D(pool_size=3, strides=2)
-        self.pool = tf.keras.layers.Conv2D(out_channels, kernel_size=3, strides=2,
-                                           kernel_initializer=tf.keras.initializers.GlorotUniform(),
-                                           bias_initializer=tf.keras.initializers.Constant(0),
-                                           kernel_regularizer=tf.keras.regularizers.L2(0.001),
-                                           bias_regularizer=tf.keras.regularizers.L2(0.001))
+        self.pool = tf.keras.layers.MaxPool2D(pool_size=3, strides=2)
+        # self.pool = tf.keras.layers.Conv2D(out_channels, kernel_size=3, strides=2,
+        #                                    kernel_initializer=tf.keras.initializers.GlorotUniform(),
+        #                                    bias_initializer=tf.keras.initializers.Constant(0),
+        #                                    kernel_regularizer=tf.keras.regularizers.L2(0.001),
+        #                                    bias_regularizer=tf.keras.regularizers.L2(0.001))
         self.out = Identity()  # for an easy access to this block's output
 
     def call(self, x, **kwargs):
         x = self.pad1(x)
         x = self.conv(x)
         x = self.nonlin(x)
         x = self.pad2(x)
@@ -57,23 +57,76 @@
 
     return tf.keras.Sequential([
         CORBlockZ(3, 64, kernel_size=7, stride=2, name='V1'),
         CORBlockZ(64, 128, name='V2'),
         CORBlockZ(128, 256, name='V4'),
         CORBlockZ(256, 512, name='IT'),
         tf.keras.Sequential([
-            keras_cortex.layers.SpatialSoftmax(),
             tf.keras.layers.Flatten(),
             tf.keras.layers.Dense(output_dim,
                                   kernel_initializer=tf.keras.initializers.GlorotUniform(),
                                   bias_initializer=tf.keras.initializers.Constant(0),
                                   kernel_regularizer=tf.keras.regularizers.L2(0.001),
                                   bias_regularizer=tf.keras.regularizers.L2(0.001),
                                   name="output"),
         ], name='decoder')
     ], name=name)
 
 
+def PoseCORNetZ(output_dim: int = 10, name="CORNetZ"):
+    """CORNet Z architecture. Smaller than S, but still efficient."""
+    inputs = tf.keras.layers.Input((128, 128, 3))
+    convoluted = tf.keras.Sequential([
+        CORBlockZ(3, 64, kernel_size=7, stride=2, name='V1'),
+        CORBlockZ(64, 64, name='V2'),
+        CORBlockZ(64, 64, name='V4'),
+        CORBlockZ(64, 64, name='IT')
+    ])(inputs)
+
+    x = keras_cortex.layers.SpatialSoftmax()(convoluted)
+    x = tf.keras.layers.Flatten()(x)
+    x = tf.keras.layers.Dense(64, kernel_initializer=tf.keras.initializers.GlorotUniform(),
+                                  bias_initializer=tf.keras.initializers.Constant(0),
+                                  kernel_regularizer=tf.keras.regularizers.L2(0.001),
+                                  bias_regularizer=tf.keras.regularizers.L2(0.001))(x)
+
+    pos = tf.keras.layers.Dense(3, kernel_initializer=tf.keras.initializers.GlorotUniform(),
+                                  bias_initializer=tf.keras.initializers.Constant(0),
+                                  kernel_regularizer=tf.keras.regularizers.L2(0.001),
+                                  bias_regularizer=tf.keras.regularizers.L2(0.001))(x)
+    rot = tf.keras.layers.Dense(4, kernel_initializer=tf.keras.initializers.GlorotUniform(),
+                                  bias_initializer=tf.keras.initializers.Constant(0),
+                                  kernel_regularizer=tf.keras.regularizers.L2(0.001),
+                                  bias_regularizer=tf.keras.regularizers.L2(0.001))(x)
+    rot = tf.math.l2_normalize(rot, axis=-1)  # ensure quaternions are quaternions
+
+    outputs = tf.concat([pos, rot], axis=-1)
+
+    return tf.keras.Model(inputs=inputs, outputs=outputs, name=name)
+
+
+class BinocularVisualComponent(tf.keras.Model):
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        self.conv_path = keras_cortex.cornet.CORNetZ(output_dim=32)
+        self.latent_fcn = tf.keras.layers.Dense(128)
+        self.output_fcn = tf.keras.layers.Dense(7)
+
+    def call(self, inputs, training=None, mask=None):
+        first_eye, second_eye = inputs
+
+        first_eye_latent = self.conv_path(first_eye)
+        second_eye_latent = self.conv_path(second_eye)
+
+        latent = tf.keras.layers.concatenate([first_eye_latent, second_eye_latent])
+        latent = self.latent_fcn(latent)
+        out = self.output_fcn(latent)
+
+        return out
+
+
 if __name__ == '__main__':
     network = CORNetZ(output_dim=15)
     output = network(tf.random.normal((128, 128, 128, 3)))
     print(output.shape)
```

### Comparing `keras-cortex-0.0.7/keras_cortex/layers.py` & `keras-cortex-0.0.8/keras_cortex/layers.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 class SpatialSoftmax(tf.keras.layers.Layer):
     """Deep Spatial Autoencoders for Visuomotor Learning (Finn et al., 2015)"""
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
     def build(self, input_shape):
+        print(input_shape)
         N, H, W, C = list(input_shape)
 
         self.alpha = self.add_weight(
             "alpha",
             shape=(1,),
             initializer=tf.keras.initializers.RandomNormal(stddev=0.01),
             trainable=True
@@ -24,23 +25,26 @@
         self.image_coords = self.add_weight(
             "image_coords",
             initializer=tf.keras.initializers.constant(image_coords),
             shape=image_coords.shape,
             trainable=False)
 
     def call(self, inputs, **kwargs):
+        print(inputs.shape)
         N, H, W, C = list(inputs.shape)
 
         if N is None:
             N = -1
 
         # per filter softmax
-        features = tf.reshape(tf.transpose(inputs / self.alpha, perm=[0, 3, 1, 2]), [-1, H * W])
+        features = tf.reshape(tf.transpose(inputs / self.alpha, 
+                                           perm=[0, 3, 1, 2]), 
+                              [-1, H * W if not H is None and not W is None else 1])
         softmax = tf.nn.softmax(features)
-        softmax = tf.transpose(tf.reshape(softmax, [N, C, H, W]), [0, 2, 3, 1])
+        softmax = tf.transpose(tf.reshape(softmax, [N, C, H if H is not None else 1, W if W is not None else 1]), [0, 2, 3, 1])
 
         # expected position
         softmax = tf.expand_dims(softmax, -1)
         image_coords = tf.expand_dims(self.image_coords, 2)
         spatial_soft_argmax = tf.reduce_sum(softmax * image_coords, axis=[1, 2])
 
         return spatial_soft_argmax
```

### Comparing `keras-cortex-0.0.7/keras_cortex.egg-info/PKG-INFO` & `keras-cortex-0.0.8/keras_cortex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-cortex
-Version: 0.0.7
+Version: 0.0.8
 Summary: Keras Implementations of Goal-driven models of (parts of) cortex
 Home-page: https://github.com/weidler/keras-cortex
 Author: Tonio Weidler
 Author-email: research@tonioweidler.de
 License: Apache-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `keras-cortex-0.0.7/setup.py` & `keras-cortex-0.0.8/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='keras-cortex',
-    version='0.0.7',
+    version='0.0.8',
     description='Keras Implementations of Goal-driven models of (parts of) cortex',
     long_description_content_type='text/markdown',
     long_description=long_description,
     url='https://github.com/weidler/keras-cortex',
     author='Tonio Weidler',
     author_email='research@tonioweidler.de',
     license='Apache-2.0',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
-        "tensorflow==2.4.2",
+        "tensorflow",
     ],
 
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Operating System :: POSIX :: Linux',
```

