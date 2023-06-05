# Comparing `tmp/kboxx-1.0.2.tar.gz` & `tmp/kboxx-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\kboxx-1.0.2.tar", last modified: Sat May 13 16:34:32 2023, max compression
+gzip compressed data, was "dist\kboxx-1.0.3.tar", last modified: Mon Jun  5 10:53:20 2023, max compression
```

## Comparing `kboxx-1.0.2.tar` & `kboxx-1.0.3.tar`

### file list

```diff
@@ -1,36 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 16:34:32.000000 kboxx-1.0.2/
--rw-rw-rw-   0        0        0      934 2023-05-13 16:34:32.000000 kboxx-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      369 2023-05-11 08:56:42.000000 kboxx-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-13 16:34:32.000000 kboxx-1.0.2/kboxx/
--rw-rw-rw-   0        0        0       23 2023-05-13 16:34:00.000000 kboxx-1.0.2/kboxx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-13 16:34:32.000000 kboxx-1.0.2/kboxx/transformer/
--rw-rw-rw-   0        0        0      129 2023-05-13 05:18:39.000000 kboxx-1.0.2/kboxx/transformer/__init__.py
--rw-rw-rw-   0        0        0        2 2023-01-20 13:12:54.000000 kboxx-1.0.2/kboxx/transformer/config.py
-drwxrwxrwx   0        0        0        0 2023-05-13 16:34:32.000000 kboxx-1.0.2/kboxx/transformer/layers/
--rw-rw-rw-   0        0        0      481 2023-05-13 12:15:05.000000 kboxx-1.0.2/kboxx/transformer/layers/__init__.py
--rw-rw-rw-   0        0        0     8334 2023-05-13 12:15:05.000000 kboxx-1.0.2/kboxx/transformer/layers/layers.py
-drwxrwxrwx   0        0        0        0 2023-05-13 16:34:32.000000 kboxx-1.0.2/kboxx/transformer/models/
--rw-rw-rw-   0        0        0       55 2023-05-12 14:07:03.000000 kboxx-1.0.2/kboxx/transformer/models/__init__.py
--rw-rw-rw-   0        0        0     4878 2023-05-13 12:29:03.000000 kboxx-1.0.2/kboxx/transformer/models/models.py
-drwxrwxrwx   0        0        0        0 2023-05-13 16:34:32.000000 kboxx-1.0.2/kboxx/transformer/utils/
--rw-rw-rw-   0        0        0      188 2023-05-13 06:07:51.000000 kboxx-1.0.2/kboxx/transformer/utils/__init__.py
--rw-rw-rw-   0        0        0     1959 2023-05-13 06:36:44.000000 kboxx-1.0.2/kboxx/transformer/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-13 16:34:32.000000 kboxx-1.0.2/kboxx/vit/
--rw-rw-rw-   0        0        0      247 2023-05-11 08:53:13.000000 kboxx-1.0.2/kboxx/vit/__init__.py
--rw-rw-rw-   0        0        0     1295 2023-05-10 08:39:18.000000 kboxx-1.0.2/kboxx/vit/config.py
-drwxrwxrwx   0        0        0        0 2023-05-13 16:34:32.000000 kboxx-1.0.2/kboxx/vit/layers/
--rw-rw-rw-   0        0        0      317 2023-05-11 08:55:27.000000 kboxx-1.0.2/kboxx/vit/layers/__init__.py
--rw-rw-rw-   0        0        0     4960 2023-05-10 06:29:39.000000 kboxx-1.0.2/kboxx/vit/layers/layers.py
-drwxrwxrwx   0        0        0        0 2023-05-13 16:34:32.000000 kboxx-1.0.2/kboxx/vit/models/
--rw-rw-rw-   0        0        0      221 2023-05-11 08:55:15.000000 kboxx-1.0.2/kboxx/vit/models/__init__.py
--rw-rw-rw-   0        0        0    15472 2023-05-11 08:03:14.000000 kboxx-1.0.2/kboxx/vit/models/models.py
-drwxrwxrwx   0        0        0        0 2023-05-13 16:34:32.000000 kboxx-1.0.2/kboxx/vit/utils/
--rw-rw-rw-   0        0        0      115 2023-05-11 08:53:26.000000 kboxx-1.0.2/kboxx/vit/utils/__init__.py
--rw-rw-rw-   0        0        0     5425 2023-05-11 08:24:56.000000 kboxx-1.0.2/kboxx/vit/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-13 16:34:32.000000 kboxx-1.0.2/kboxx.egg-info/
--rw-rw-rw-   0        0        0      934 2023-05-13 16:34:32.000000 kboxx-1.0.2/kboxx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      630 2023-05-13 16:34:32.000000 kboxx-1.0.2/kboxx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 16:34:32.000000 kboxx-1.0.2/kboxx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-13 16:34:32.000000 kboxx-1.0.2/kboxx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-13 16:34:32.000000 kboxx-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      694 2023-05-13 16:33:42.000000 kboxx-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 10:53:20.000000 kboxx-1.0.3/
+-rw-rw-rw-   0        0        0      934 2023-06-05 10:53:20.000000 kboxx-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      369 2023-05-11 08:56:42.000000 kboxx-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 10:53:20.000000 kboxx-1.0.3/kboxx/
+-rw-rw-rw-   0        0        0       23 2023-06-05 10:51:50.000000 kboxx-1.0.3/kboxx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 10:53:20.000000 kboxx-1.0.3/kboxx/transformer/
+-rw-rw-rw-   0        0        0      214 2023-06-05 10:12:04.000000 kboxx-1.0.3/kboxx/transformer/__init__.py
+-rw-rw-rw-   0        0        0      603 2023-06-05 10:01:37.000000 kboxx-1.0.3/kboxx/transformer/config.py
+drwxrwxrwx   0        0        0        0 2023-06-05 10:53:20.000000 kboxx-1.0.3/kboxx/transformer/layers/
+-rw-rw-rw-   0        0        0      535 2023-05-16 15:16:05.000000 kboxx-1.0.3/kboxx/transformer/layers/__init__.py
+-rw-rw-rw-   0        0        0     8321 2023-06-05 08:17:59.000000 kboxx-1.0.3/kboxx/transformer/layers/layers.py
+drwxrwxrwx   0        0        0        0 2023-06-05 10:53:20.000000 kboxx-1.0.3/kboxx/transformer/models/
+-rw-rw-rw-   0        0        0      115 2023-06-05 09:58:36.000000 kboxx-1.0.3/kboxx/transformer/models/__init__.py
+-rw-rw-rw-   0        0        0     3441 2023-06-05 10:48:08.000000 kboxx-1.0.3/kboxx/transformer/models/models.py
+drwxrwxrwx   0        0        0        0 2023-06-05 10:53:20.000000 kboxx-1.0.3/kboxx/transformer/utils/
+-rw-rw-rw-   0        0        0      312 2023-06-05 10:10:34.000000 kboxx-1.0.3/kboxx/transformer/utils/__init__.py
+-rw-rw-rw-   0        0        0     3118 2023-06-05 10:43:13.000000 kboxx-1.0.3/kboxx/transformer/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-05 10:53:20.000000 kboxx-1.0.3/kboxx/utils/
+-rw-rw-rw-   0        0        0       47 2023-06-05 10:34:16.000000 kboxx-1.0.3/kboxx/utils/__init__.py
+-rw-rw-rw-   0        0        0     8000 2023-05-31 18:25:10.000000 kboxx-1.0.3/kboxx/utils/tokenize.py
+drwxrwxrwx   0        0        0        0 2023-06-05 10:53:20.000000 kboxx-1.0.3/kboxx/vit/
+-rw-rw-rw-   0        0        0      275 2023-06-05 08:51:13.000000 kboxx-1.0.3/kboxx/vit/__init__.py
+-rw-rw-rw-   0        0        0     1295 2023-05-13 16:38:11.000000 kboxx-1.0.3/kboxx/vit/config.py
+drwxrwxrwx   0        0        0        0 2023-06-05 10:53:20.000000 kboxx-1.0.3/kboxx/vit/layers/
+-rw-rw-rw-   0        0        0      317 2023-05-13 16:38:11.000000 kboxx-1.0.3/kboxx/vit/layers/__init__.py
+-rw-rw-rw-   0        0        0     4960 2023-05-13 16:38:11.000000 kboxx-1.0.3/kboxx/vit/layers/layers.py
+drwxrwxrwx   0        0        0        0 2023-06-05 10:53:20.000000 kboxx-1.0.3/kboxx/vit/models/
+-rw-rw-rw-   0        0        0      221 2023-05-13 16:38:11.000000 kboxx-1.0.3/kboxx/vit/models/__init__.py
+-rw-rw-rw-   0        0        0    15472 2023-05-13 16:38:11.000000 kboxx-1.0.3/kboxx/vit/models/models.py
+drwxrwxrwx   0        0        0        0 2023-06-05 10:53:20.000000 kboxx-1.0.3/kboxx/vit/utils/
+-rw-rw-rw-   0        0        0      115 2023-05-13 16:38:11.000000 kboxx-1.0.3/kboxx/vit/utils/__init__.py
+-rw-rw-rw-   0        0        0     5425 2023-05-13 16:38:11.000000 kboxx-1.0.3/kboxx/vit/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-05 10:53:20.000000 kboxx-1.0.3/kboxx.egg-info/
+-rw-rw-rw-   0        0        0      934 2023-06-05 10:53:20.000000 kboxx-1.0.3/kboxx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      678 2023-06-05 10:53:20.000000 kboxx-1.0.3/kboxx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 10:53:20.000000 kboxx-1.0.3/kboxx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-05 10:53:20.000000 kboxx-1.0.3/kboxx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 10:53:20.000000 kboxx-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      694 2023-06-05 10:51:13.000000 kboxx-1.0.3/setup.py
```

### Comparing `kboxx-1.0.2/PKG-INFO` & `kboxx-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kboxx
-Version: 1.0.2
+Version: 1.0.3
 Summary: Implementation of pre-trained model based on Keras
 Home-page: https://github.com/djsaber/Keras-ViT
 Author: djsaber
 Author-email: 479719615@qq.com
 License: UNKNOWN
 Description: # kboxx
```

### Comparing `kboxx-1.0.2/kboxx/transformer/layers/layers.py` & `kboxx-1.0.3/kboxx/transformer/layers/layers.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,63 +1,64 @@
 from keras import layers
 from keras import activations
 from .. import utils
 
 
 class Embedding(layers.Layer):
+    """Input embedding.
+    args:
+        - size: the size of the vocabulary
+        - dim: embedding dimension for each word
+    """
     def __init__(self, size, dim, **kwargs):
         super().__init__(**kwargs)
-        self.size = size
-        self.dim = dim
-        
-    def build(self, input_shape):
-        self.embedding=layers.Embedding(self.size, self.dim)
-        return super().build(input_shape)
+        self.embedding=layers.Embedding(size, dim)
 
     def call(self, inputs):
         return self.embedding(inputs)
 
 
 class PositionalEncoding(layers.Layer):
-    """Positional encoding.
+    """Add Positional encoding to inputs.
     args:
-        - trainable=False: Can the weight parameters of position encoding be learned
+        - pos: position length
+        - dim: encoding length for each position
     """
-    def __init__(self, trainable=False, **kwargs):
+    def __init__(self, **kwargs):
         super().__init__(**kwargs)
-        self.trainable = trainable
-
+        
     def build(self, input_shape):
-        if self.trainable:
-            self.pe = self.add_weight(
-                shape=(1,*input_shape[1:]),
-                trainable=self.trainable
-                )
-        else:
-            self.pe = utils.get_positional_encoding(
-                pos=input_shape[1], 
-                dim=input_shape[2]
-                )
+        pos, dim = input_shape[1:]    
+        self.pe = utils.get_positional_encoding(pos, dim)
         return super().build(input_shape)
 
-    def call(self, _):
-        return self.pe
+    def call(self, inputs):
+        return inputs + self.pe
+
+
+class GetMasks(layers.Layer):
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+
+    def call(self, encoder_inputs, decoder_inputs, padding_value):
+        masks = utils.get_transformer_masks(encoder_inputs, decoder_inputs, padding_value)
+        return masks
 
 
 class MultiHeadAttention(layers.Layer):
-    """MultiHeadAttention layer
+    """MultiHeadAttention layer.
     args:
-        - num_heads: Number of heads in a multi head attention layer
-        - hiddem_dim: Dimensions of queries, keys, and values for each attention head 
-        - dropout: Dropout probability
-    callargs:
-        - query, shape like (B, T, dim)
-        - value, shape like (B, S, dim)
-        - key=None, shape like (B, S, dim)
-        - attention_mask=None, shape like (B, T, S)
+        - num_heads: number of heads in a multi head attention layer
+        - hiddem_dim: dimensions of queries, keys, and values for each attention head
+        - dropout: dropout probability
+    call arguments:
+        - query, shape-->(B, T, dim)
+        - value, shape-->(B, S, dim)
+        - key=None, shape-->(B, S, dim)
+        - mask=None, shape-->(B, T, S)
     """
     def __init__(
         self, 
         num_heads, 
         hiddem_dim, 
         dropout,
         **kwargs):
@@ -66,71 +67,73 @@
         self.hiddem_dim = hiddem_dim
         self.dropout = dropout
 
     def build(self, input_shape):
         self.multi_head_attetion = layers.MultiHeadAttention(
             key_dim=self.hiddem_dim,
             num_heads=self.num_heads, 
-            dropout=0.2,
+            dropout=self.dropout,
             )
         return super().build(input_shape)
 
-    def call(self, query, value, key=None, attention_mask=None):
-        return self.multi_head_attetion(query, value, key=key, attention_mask=attention_mask)
+    def call(self, query, value, key=None, mask=None):
+        return self.multi_head_attetion(query, value, key=key, attention_mask=mask)
 
 
 class AddNorm(layers.Layer):
-    """Add and Norm"""
+    """Add and Norm, Layer Normalize x first, then add y.
+    call arguments:
+        - x: inputs 1
+        - y: inputs 2
+    """
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
-
-    def build(self, input_shape):
         self.layer_norm = layers.LayerNormalization(epsilon=1e-6)
-        return super().build(input_shape)
 
-    def call(self, inputs_a, inputs_b):
-        return self.layer_norm(inputs_a + inputs_b)
+    def call(self, x, y):
+        return y + self.layer_norm(x)
 
 
 class FeedForward(layers.Layer):
     """FeedForward layer for encoder and decoder.
     args:
-        - linear_dim: Dimension of the first linear projection
-        - output_dim=None: The Dimension of the Second Linear Projection
-        - activation=None: Activation function of the first linear projection
+        - linear_dim: dimension of the linear projection
+        - dropout: dropout probability
+        - activation=None: activation function of the first linear projection
     """
     def __init__(
         self, 
-        linear_dim, 
-        output_dim=None, 
+        linear_dim,
+        dropout,
         activation=None,
         **kwargs):
         super().__init__(**kwargs)
         self.linear_dim = linear_dim
-        self.output_dim = output_dim
+        self.dropout = dropout
         self.activation = activations.get(activation)
 
     def build(self, input_shape):
-        if self.output_dim is None:
-            self.output_dim = input_shape[-1]
+        output_dim = self.output_dim = input_shape[-1]
         self.linear_1 = layers.Dense(self.linear_dim, self.activation)
-        self.linear_2 = layers.Dense(self.output_dim)
+        self.linear_2 = layers.Dense(output_dim)
+        self.dropout_layer = layers.Dropout(self.dropout)
         return super().build(input_shape)
 
     def call(self, inputs):
         x = self.linear_1(inputs)
+        x = self.dropout_layer(x)
         x = self.linear_2(x)
         return x
 
 
 class Linear(layers.Layer):
-    """linear projection
+    """linear projection.
     args:
-        - output_dim: Linear projection output dimension
-        - use_bias=False: Whether to use bias
+        - output_dim: linear projection output dimension
+        - use_bias=False: whether to use bias
     """
     def __init__(self, output_dim, use_bias=False, **kwargs):
         super().__init__(**kwargs)
         self.output_dim = output_dim
         self.use_bias = use_bias
 
     def build(self, input_shape):
@@ -140,30 +143,30 @@
     def call(self, inputs):
         return self.linear(inputs)
 
 
 class TransformerEncoderBlock(layers.Layer):
     """Classic Transformer Encoder Block.
     args:
-        - num_heads: The number of heads in a multi head attention layer
-        - hidden_dim: Dimensions of queries, keys, and values for each attention head 
-        - linear_dim: The linear projection dimension of feedforward
-        - dropout: Default to 0.1
-        - activation: Activation function of feedforward layer
-    call args:
-        - inputs, shape like (B, T, dim)
-        - padding_mask=None, shape like (B, T, T)
+        - num_heads: the number of heads in a multi head attention layer
+        - hidden_dim: dimensions of queries, keys, and values for each attention head 
+        - linear_dim: the linear projection dimension of feedforward
+        - dropout: dropout probability
+        - activation: activation function of feedforward layer
+    call arguments:
+        - inputs, shape-->(B, S, dim)
+        - padding_mask=None, shape-->(B, S, S)
     """
     def __init__(
         self, 
         num_heads,
         hidden_dim,
         linear_dim,
-        dropout=0.1,
-        activation="leaky_relu",
+        dropout,
+        activation,
         **kwargs
         ):
         super().__init__(**kwargs)
         self.num_heads = num_heads
         self.hidden_dim = hidden_dim
         self.linear_dim = linear_dim
         self.dropout = dropout
@@ -171,51 +174,52 @@
         
     def build(self, input_shape):
         self.multi_head_attention = MultiHeadAttention(
             num_heads=self.num_heads,
             hiddem_dim=self.hidden_dim, 
             dropout=self.dropout,
             )
-        self.add_and_norm_1 = AddNorm()
+        self.add_norm_1 = AddNorm()
         self.feed_forward = FeedForward(
             linear_dim=self.linear_dim,
+            dropout = self.dropout,
             activation=self.activation
             )
-        self.add_and_norm_2 = AddNorm()
+        self.add_norm_2 = AddNorm()
         super().build(input_shape)
 
-    def call(self, inputs, padding_mask):
-        x = self.multi_head_attention(inputs, inputs, attention_mask=padding_mask)
-        x = self.add_and_norm_1(x, inputs)
+    def call(self, inputs, padding_mask=None):
+        x = self.multi_head_attention(inputs, inputs, mask=padding_mask)
+        x = self.add_norm_1(x, inputs)
         y = self.feed_forward(x)
-        y = self.add_and_norm_2(x, y)
+        y = self.add_norm_2(y, x)
         return y
 
 
 class TransformerDecoderBlock(layers.Layer):
     """Classic Transformer Decoder Block.
     args:
-        - num_heads: The number of heads in a multi head attention layer
-        - hidden_dim: Dimensions of queries, keys, and values for each attention head 
-        - linear_dim: The linear projection dimension of feedforward
-        - dropout: Default to 0.1
-        - activation: Activation function of feedforward layer
-    call args:
-        - decoder_inputs, shape like (B, T, dim)
-        - encoder_outputs, shape like (B, T, dim)
-        - sequence_mask, shape like (B, T, T)
-        - padding_mask, shape like (B, T, T)
+        - num_heads: the number of heads in a multi head attention layer
+        - hidden_dim: dimensions of queries, keys, and values for each attention head 
+        - linear_dim: the linear projection dimension of feedforward
+        - dropout: dropout probability
+        - activation: activation function of feedforward layer
+    call arguments:
+        - decoder_inputs, shape-->(B, T, dim)
+        - encoder_outputs, shape-->(B, S, dim)
+        - sequence_mask, shape-->(B, T, T)
+        - padding_mask, shape-->(B, T, S)
     """
     def __init__(
         self, 
         num_heads,
         hidden_dim,
         linear_dim,
-        dropout=0.1,
-        activation="leaky_relu",
+        dropout,
+        activation,
         **kwargs
         ):
         super().__init__(**kwargs)     
         self.num_heads = num_heads
         self.hidden_dim = hidden_dim
         self.linear_dim = linear_dim
         self.dropout = dropout
@@ -223,29 +227,30 @@
 
     def build(self, input_shape):
         self.masked_multi_head_attention = MultiHeadAttention(
             num_heads=self.num_heads,
             hiddem_dim=self.hidden_dim, 
             dropout=self.dropout,
             )
-        self.add_and_norm_1 = AddNorm()
+        self.add_norm_1 = AddNorm()
         self.multi_head_attention = MultiHeadAttention(
             num_heads=self.num_heads,
             hiddem_dim=self.hidden_dim, 
             dropout=self.dropout,
             )
-        self.add_and_norm_2 = AddNorm()
+        self.add_norm_2 = AddNorm()
         self.feed_forward = FeedForward(
             linear_dim=self.linear_dim,
+            dropout=self.dropout,
             activation=self.activation
             )
-        self.add_and_norm_3 = AddNorm()
+        self.add_norm_3 = AddNorm()
         super().build(input_shape)
 
-    def call(self, decoder_inputs, encoder_outputs, sequence_mask, padding_mask):
-        x = self.masked_multi_head_attention(decoder_inputs, decoder_inputs, attention_mask=sequence_mask)
-        x = self.add_and_norm_1(x, decoder_inputs)
-        y = self.multi_head_attention(x, encoder_outputs, attention_mask=padding_mask)
-        y = self.add_and_norm_2(x, y)
+    def call(self, decoder_inputs, encoder_outputs, sequence_mask=None, padding_mask=None):
+        x = self.masked_multi_head_attention(decoder_inputs, decoder_inputs, mask=sequence_mask)
+        x = self.add_norm_1(x, decoder_inputs)
+        y = self.multi_head_attention(x, encoder_outputs, mask=padding_mask)
+        y = self.add_norm_2(y, x)
         z = self.feed_forward(y)
-        z = self.add_and_norm_3(y, z)
+        z = self.add_norm_3(z, y)
         return z
```

### Comparing `kboxx-1.0.2/kboxx/vit/config.py` & `kboxx-1.0.3/kboxx/vit/config.py`

 * *Files identical despite different names*

### Comparing `kboxx-1.0.2/kboxx/vit/layers/layers.py` & `kboxx-1.0.3/kboxx/vit/layers/layers.py`

 * *Files identical despite different names*

### Comparing `kboxx-1.0.2/kboxx/vit/models/models.py` & `kboxx-1.0.3/kboxx/vit/models/models.py`

 * *Files identical despite different names*

### Comparing `kboxx-1.0.2/kboxx/vit/utils/utils.py` & `kboxx-1.0.3/kboxx/vit/utils/utils.py`

 * *Files identical despite different names*

### Comparing `kboxx-1.0.2/kboxx.egg-info/PKG-INFO` & `kboxx-1.0.3/kboxx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kboxx
-Version: 1.0.2
+Version: 1.0.3
 Summary: Implementation of pre-trained model based on Keras
 Home-page: https://github.com/djsaber/Keras-ViT
 Author: djsaber
 Author-email: 479719615@qq.com
 License: UNKNOWN
 Description: # kboxx
```

### Comparing `kboxx-1.0.2/kboxx.egg-info/SOURCES.txt` & `kboxx-1.0.3/kboxx.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 kboxx/transformer/config.py
 kboxx/transformer/layers/__init__.py
 kboxx/transformer/layers/layers.py
 kboxx/transformer/models/__init__.py
 kboxx/transformer/models/models.py
 kboxx/transformer/utils/__init__.py
 kboxx/transformer/utils/utils.py
+kboxx/utils/__init__.py
+kboxx/utils/tokenize.py
 kboxx/vit/__init__.py
 kboxx/vit/config.py
 kboxx/vit/layers/__init__.py
 kboxx/vit/layers/layers.py
 kboxx/vit/models/__init__.py
 kboxx/vit/models/models.py
 kboxx/vit/utils/__init__.py
```

### Comparing `kboxx-1.0.2/setup.py` & `kboxx-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
  
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
  
 setuptools.setup(
     name="kboxx",
-    version="1.0.2",
+    version="1.0.3",
     author="djsaber",
     author_email="479719615@qq.com",
     description="Implementation of pre-trained model based on Keras",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/djsaber/Keras-ViT",
     packages=setuptools.find_packages(),
```

