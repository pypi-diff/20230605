# Comparing `tmp/deepfilternet-0.4.0.tar.gz` & `tmp/deepfilternet-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepfilternet-0.4.0.tar", max compression
+gzip compressed data, was "deepfilternet-0.5.0.tar", max compression
```

## Comparing `deepfilternet-0.4.0.tar` & `deepfilternet-0.5.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0      495 2022-12-13 08:27:14.051424 deepfilternet-0.4.0/LICENSE
--rw-r--r--   0        0        0    10837 2022-12-13 08:27:14.051424 deepfilternet-0.4.0/LICENSE-APACHE
--rw-r--r--   0        0        0     1083 2022-12-13 08:27:14.051424 deepfilternet-0.4.0/LICENSE-MIT
--rw-r--r--   0        0        0      111 2022-12-13 08:27:14.051424 deepfilternet-0.4.0/df/__init__.py
--rw-r--r--   0        0        0     7976 2022-12-13 08:27:14.051424 deepfilternet-0.4.0/df/checkpoint.py
--rw-r--r--   0        0        0    11708 2022-12-13 08:27:14.051424 deepfilternet-0.4.0/df/config.py
--rw-r--r--   0        0        0    11383 2022-12-13 08:27:14.051424 deepfilternet-0.4.0/df/deepfilternet.py
--rw-r--r--   0        0        0    19236 2022-12-13 08:27:14.051424 deepfilternet-0.4.0/df/deepfilternet2.py
--rw-r--r--   0        0        0    15163 2022-12-13 08:27:14.051424 deepfilternet-0.4.0/df/deepfilternet3.py
--rw-r--r--   0        0        0    15869 2022-12-13 08:27:14.051424 deepfilternet-0.4.0/df/deepfilternetmf.py
--rw-r--r--   0        0        0    11766 2022-12-13 08:27:14.051424 deepfilternet-0.4.0/df/enhance.py
--rw-r--r--   0        0        0    23641 2022-12-13 08:27:14.051424 deepfilternet-0.4.0/df/evaluation_utils.py
--rw-r--r--   0        0        0     4098 2022-12-13 08:27:14.051424 deepfilternet-0.4.0/df/io.py
--rw-r--r--   0        0        0     7192 2022-12-13 08:27:14.051424 deepfilternet-0.4.0/df/logger.py
--rw-r--r--   0        0        0    24589 2022-12-13 08:27:14.051424 deepfilternet-0.4.0/df/loss.py
--rw-r--r--   0        0        0     1920 2022-12-13 08:27:14.051424 deepfilternet-0.4.0/df/lr.py
--rw-r--r--   0        0        0      779 2022-12-13 08:27:14.051424 deepfilternet-0.4.0/df/model.py
--rw-r--r--   0        0        0    36938 2022-12-13 08:27:14.051424 deepfilternet-0.4.0/df/modules.py
--rw-r--r--   0        0        0    24472 2022-12-13 08:27:14.051424 deepfilternet-0.4.0/df/multiframe.py
--rw-r--r--   0        0        0     8012 2022-12-13 08:27:14.051424 deepfilternet-0.4.0/df/scripts/dnsmos.py
--rw-r--r--   0        0        0     3528 2022-12-13 08:27:14.051424 deepfilternet-0.4.0/df/scripts/dnsmos_v2.py
--rw-r--r--   0        0        0    10472 2022-12-13 08:27:14.051424 deepfilternet-0.4.0/df/scripts/export.py
--rw-r--r--   0        0        0     4382 2022-12-13 08:27:14.055424 deepfilternet-0.4.0/df/scripts/filter_dnsmos.py
--rw-r--r--   0        0        0     2267 2022-12-13 08:27:14.055424 deepfilternet-0.4.0/df/scripts/fix_n_samples_hdf5.py
--rw-r--r--   0        0        0      519 2022-12-13 08:27:14.055424 deepfilternet-0.4.0/df/scripts/list_attrs_in_hdf5.py
--rw-r--r--   0        0        0     1959 2022-12-13 08:27:14.055424 deepfilternet-0.4.0/df/scripts/model_summary.py
--rw-r--r--   0        0        0     2211 2022-12-13 08:27:14.055424 deepfilternet-0.4.0/df/scripts/plot_lrs.py
--rw-r--r--   0        0        0      636 2022-12-13 08:27:14.055424 deepfilternet-0.4.0/df/scripts/plot_spec.py
--rw-r--r--   0        0        0     4194 2022-12-13 08:27:14.055424 deepfilternet-0.4.0/df/scripts/plot_summaries.py
--rwxr-xr-x   0        0        0     8762 2022-12-13 08:27:14.055424 deepfilternet-0.4.0/df/scripts/prepare_data.py
--rw-r--r--   0        0        0      355 2022-12-13 08:27:14.055424 deepfilternet-0.4.0/df/scripts/print_model.py
--rw-r--r--   0        0        0     2423 2022-12-13 08:27:14.055424 deepfilternet-0.4.0/df/scripts/sample_from_hdf5.py
--rw-r--r--   0        0        0     2393 2022-12-13 08:27:14.055424 deepfilternet-0.4.0/df/scripts/split_hdf5.py
--rwxr-xr-x   0        0        0     4154 2022-12-13 08:27:14.055424 deepfilternet-0.4.0/df/scripts/test_df.py
--rw-r--r--   0        0        0     2535 2022-12-13 08:27:14.055424 deepfilternet-0.4.0/df/scripts/test_dns_2020.py
--rw-r--r--   0        0        0     2312 2022-12-13 08:27:14.055424 deepfilternet-0.4.0/df/scripts/test_noisy_dnsmos.py
--rw-r--r--   0        0        0     2473 2022-12-13 08:27:14.055424 deepfilternet-0.4.0/df/scripts/test_voicebank_demand.py
--rw-r--r--   0        0        0     1849 2022-12-13 08:27:14.055424 deepfilternet-0.4.0/df/scripts/trim_silence_hdf5.py
--rw-r--r--   0        0        0    17443 2022-12-13 08:27:14.055424 deepfilternet-0.4.0/df/sepm.py
--rw-r--r--   0        0        0     9474 2022-12-13 08:27:14.055424 deepfilternet-0.4.0/df/stoi.py
--rw-r--r--   0        0        0    23872 2022-12-13 08:27:14.055424 deepfilternet-0.4.0/df/train.py
--rw-r--r--   0        0        0     7464 2022-12-13 08:27:14.055424 deepfilternet-0.4.0/df/utils.py
--rw-r--r--   0        0        0      884 2022-12-13 08:27:14.055424 deepfilternet-0.4.0/df/version.py
--rw-r--r--   0        0        0     3491 2022-12-13 08:27:14.055424 deepfilternet-0.4.0/df/visualization.py
--rw-r--r--   0        0        0     2264 2022-12-13 08:27:14.055424 deepfilternet-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1187 1970-01-01 00:00:00.000000 deepfilternet-0.4.0/setup.py
--rw-r--r--   0        0        0     1638 1970-01-01 00:00:00.000000 deepfilternet-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      495 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/LICENSE
+-rw-r--r--   0        0        0    10837 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/LICENSE-APACHE
+-rw-r--r--   0        0        0     1083 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/LICENSE-MIT
+-rw-r--r--   0        0        0      171 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/__init__.py
+-rw-r--r--   0        0        0     7976 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/checkpoint.py
+-rw-r--r--   0        0        0    10763 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/config.py
+-rw-r--r--   0        0        0    11383 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/deepfilternet.py
+-rw-r--r--   0        0        0    19236 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/deepfilternet2.py
+-rw-r--r--   0        0        0    16199 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/deepfilternet3.py
+-rw-r--r--   0        0        0    15869 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/deepfilternetmf.py
+-rw-r--r--   0        0        0    13645 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/enhance.py
+-rw-r--r--   0        0        0    23763 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/evaluation_utils.py
+-rw-r--r--   0        0        0     4105 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/io.py
+-rw-r--r--   0        0        0     7192 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/logger.py
+-rw-r--r--   0        0        0    33521 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/loss.py
+-rw-r--r--   0        0        0     1920 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/lr.py
+-rw-r--r--   0        0        0      779 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/model.py
+-rw-r--r--   0        0        0    36996 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/modules.py
+-rw-r--r--   0        0        0    24438 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/multiframe.py
+-rw-r--r--   0        0        0     8108 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/scripts/dnsmos.py
+-rw-r--r--   0        0        0     9489 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/scripts/dnsmos_dns5.py
+-rw-r--r--   0        0        0     3528 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/scripts/dnsmos_v2.py
+-rw-r--r--   0        0        0    10613 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/scripts/export.py
+-rw-r--r--   0        0        0     4376 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/scripts/filter_dnsmos.py
+-rw-r--r--   0        0        0     2267 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/scripts/fix_n_samples_hdf5.py
+-rw-r--r--   0        0        0      519 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/scripts/list_attrs_in_hdf5.py
+-rw-r--r--   0        0        0     1959 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/scripts/model_summary.py
+-rw-r--r--   0        0        0     2211 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/scripts/plot_lrs.py
+-rw-r--r--   0        0        0      636 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/scripts/plot_spec.py
+-rw-r--r--   0        0        0     4194 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/scripts/plot_summaries.py
+-rwxr-xr-x   0        0        0     8762 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/scripts/prepare_data.py
+-rw-r--r--   0        0        0      355 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/scripts/print_model.py
+-rw-r--r--   0        0        0     2423 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/scripts/sample_from_hdf5.py
+-rw-r--r--   0        0        0     2393 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/scripts/split_hdf5.py
+-rwxr-xr-x   0        0        0     4608 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/scripts/test_df.py
+-rw-r--r--   0        0        0     2535 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/scripts/test_dns_2020.py
+-rw-r--r--   0        0        0     2312 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/scripts/test_noisy_dnsmos.py
+-rw-r--r--   0        0        0     2592 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/scripts/test_voicebank_demand.py
+-rw-r--r--   0        0        0     3109 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/scripts/trim_silence_hdf5.py
+-rw-r--r--   0        0        0    17442 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/sepm.py
+-rw-r--r--   0        0        0     9474 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/stoi.py
+-rw-r--r--   0        0        0    23584 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/train.py
+-rw-r--r--   0        0        0     7430 2023-06-05 11:47:27.017806 deepfilternet-0.5.0/df/utils.py
+-rw-r--r--   0        0        0      884 2023-06-05 11:47:27.021806 deepfilternet-0.5.0/df/version.py
+-rw-r--r--   0        0        0     3566 2023-06-05 11:47:27.021806 deepfilternet-0.5.0/df/visualization.py
+-rw-r--r--   0        0        0     2450 2023-06-05 11:47:27.021806 deepfilternet-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1707 1970-01-01 00:00:00.000000 deepfilternet-0.5.0/PKG-INFO
```

### Comparing `deepfilternet-0.4.0/LICENSE-APACHE` & `deepfilternet-0.5.0/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.4.0/LICENSE-MIT` & `deepfilternet-0.5.0/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.4.0/df/checkpoint.py` & `deepfilternet-0.5.0/df/checkpoint.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.4.0/df/config.py` & `deepfilternet-0.5.0/df/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -117,23 +117,23 @@
         if not self.parser.has_section(section.lower()):
             self.parser.add_section(section.lower())
         if option.upper() in os.environ:
             value = os.environ[option.upper()]
             if save:
                 self.parser.set(section, option, self.tostr(value, cast))
         elif self.parser.has_option(section, option):
-            value = self.read_from_section(section, option, default, cast=cast, save=save)
+            value = self.parser.get(section, option)
         elif self.parser.has_option(section.lower(), option):
-            value = self.read_from_section(section.lower(), option, default, cast=cast, save=save)
+            value = self.parser.get(section.lower(), option)
         elif self.parser.has_option(self.DEFAULT_SECTION, option):
             logger.warning(
                 f"Couldn't find option {option} in section {section}. "
                 "Falling back to default settings section."
             )
-            value = self.read_from_section(self.DEFAULT_SECTION, option, cast=cast, save=save)
+            value = self.parser.get(self.DEFAULT_SECTION, option)
         elif default is None:
             raise ValueError("Value {} not found.".format(option))
         elif not self.allow_defaults and save:
             raise ValueError(f"Value '{option}' not found in config (defaults not allowed).")
         else:
             value = default
             if save:
@@ -155,32 +155,14 @@
         section = self.DEFAULT_SECTION if section is None else section
         if not self.parser.has_section(section):
             raise KeyError(section)
         if not self.parser.has_option(section, option):
             raise KeyError(option)
         return self.cast(self.parser.get(section, option), cast)
 
-    def read_from_section(
-        self, section: str, option: str, default: Any = None, cast: Type = str, save: bool = True
-    ) -> str:
-        value = self.parser.get(section, option)
-        if not save:
-            # Set to default or remove to not read it at trainig start again
-            if default is None:
-                self.parser.remove_option(section, option)
-            elif not self.allow_defaults:
-                raise ValueError(f"Value '{option}' not found in config (defaults not allowed).")
-            else:
-                self.parser.set(section, option, self.tostr(default, cast))
-        elif section.lower() != section:
-            self.parser.set(section.lower(), option, self.tostr(value, cast))
-            self.parser.remove_option(section, option)
-            self.modified = True
-        return value
-
     def overwrite(self, section: str, option: str, value: Any):
         if not self.parser.has_section(section):
             return ValueError(f"Section not found: '{section}'")
         if not self.parser.has_option(section, option):
             return ValueError(f"Option not found '{option}' in section '{section}'")
         self.modified = True
         cast = type(value)
```

### Comparing `deepfilternet-0.4.0/df/deepfilternet.py` & `deepfilternet-0.5.0/df/deepfilternet.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.4.0/df/deepfilternet2.py` & `deepfilternet-0.5.0/df/deepfilternet2.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.4.0/df/deepfilternet3.py` & `deepfilternet-0.5.0/df/deepfilternet3.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,17 @@
         )
         self.convt_depthwise: bool = config(
             "CONVT_DEPTHWISE", cast=bool, default=True, section=self.section
         )
         self.conv_kernel: List[int] = config(
             "CONV_KERNEL", cast=Csv(int), default=(1, 3), section=self.section  # type: ignore
         )
+        self.convt_kernel: List[int] = config(
+            "CONVT_KERNEL", cast=Csv(int), default=(1, 3), section=self.section  # type: ignore
+        )
         self.conv_kernel_inp: List[int] = config(
             "CONV_KERNEL_INP", cast=Csv(int), default=(3, 3), section=self.section  # type: ignore
         )
         self.emb_hidden_dim: int = config(
             "EMB_HIDDEN_DIM", cast=int, default=256, section=self.section
         )
         self.emb_num_layers: int = config(
@@ -58,14 +61,17 @@
         self.df_num_layers: int = config("DF_NUM_LAYERS", cast=int, default=3, section=self.section)
         self.df_n_iter: int = config("DF_N_ITER", cast=int, default=1, section=self.section)
         self.lin_groups: int = config("LINEAR_GROUPS", cast=int, default=1, section=self.section)
         self.enc_lin_groups: int = config(
             "ENC_LINEAR_GROUPS", cast=int, default=16, section=self.section
         )
         self.mask_pf: bool = config("MASK_PF", cast=bool, default=False, section=self.section)
+        self.lsnr_dropout: bool = config(
+            "LSNR_DROPOUT", cast=bool, default=False, section=self.section
+        )
 
 
 def init_model(df_state: Optional[DF] = None, run_df: bool = True, train_mask: bool = True):
     p = ModelParams()
     if df_state is None:
         df_state = DF(sr=p.sr, fft_size=p.fft_size, hop_size=p.hop_size, nb_bands=p.nb_erb)
     erb = erb_fb(df_state.erb_widths(), p.sr, inverse=False)
@@ -188,19 +194,17 @@
             output_size=self.emb_out_dim,
             num_layers=p.emb_num_layers - 1,
             batch_first=True,
             gru_skip_op=skip_op,
             linear_groups=p.lin_groups,
             linear_act_layer=partial(nn.ReLU, inplace=True),
         )
-        t_conv_kernel = list(p.conv_kernel)
-        t_conv_kernel[0] = 1
         tconv_layer = partial(
             ConvTranspose2dNormAct,
-            kernel_size=t_conv_kernel,
+            kernel_size=p.convt_kernel,
             bias=False,
             separable=True,
         )
         conv_layer = partial(
             Conv2dNormAct,
             bias=False,
             separable=True,
@@ -305,14 +309,16 @@
         c = self.df_out(c)  # [B, T, F*O*2], O: df_order
         c = c.view(b, t, self.df_bins, self.df_out_ch) + c0  # [B, T, F, O*2]
         return c, alpha
 
 
 class DfNet(nn.Module):
     run_df: Final[bool]
+    run_erb: Final[bool]
+    lsnr_droput: Final[bool]
 
     def __init__(
         self,
         erb_fb: Tensor,
         erb_inv_fb: Tensor,
         run_df: bool = True,
         train_mask: bool = True,
@@ -348,14 +354,15 @@
         self.run_erb = p.nb_df + 1 < self.freq_bins
         if not self.run_erb:
             logger.warning("Running without ERB stage")
         self.run_df = run_df
         if not run_df:
             logger.warning("Running without DF stage")
         self.train_mask = train_mask
+        self.lsnr_droput = p.lsnr_dropout
         assert p.df_n_iter == 1
 
     def forward(
         self,
         spec: Tensor,
         feat_erb: Tensor,
         feat_spec: Tensor,  # Not used, take spec modified by mask instead
@@ -373,23 +380,43 @@
             lsnr (Tensor): Local SNR estimate of shape [B, T, 1]
         """
         feat_spec = feat_spec.squeeze(1).permute(0, 3, 1, 2)
 
         feat_erb = self.pad_feat(feat_erb)
         feat_spec = self.pad_feat(feat_spec)
         e0, e1, e2, e3, emb, c0, lsnr = self.enc(feat_erb, feat_spec)
+
+        if self.lsnr_droput:
+            idcs = lsnr.squeeze() > -10.0
+            b, t = (spec.shape[0], spec.shape[2])
+            m = torch.zeros((b, 1, t, self.erb_bins), device=spec.device)
+            df_coefs = torch.zeros((b, t, self.nb_df, self.df_order * 2))
+            spec_m = spec.clone()
+            emb = emb[:, idcs]
+            e0 = e0[:, :, idcs]
+            e1 = e1[:, :, idcs]
+            e2 = e2[:, :, idcs]
+            e3 = e3[:, :, idcs]
+            c0 = c0[:, :, idcs]
+
         if self.run_erb:
-            m = self.erb_dec(emb, e3, e2, e1, e0)
+            if self.lsnr_droput:
+                m[:, :, idcs] = self.erb_dec(emb, e3, e2, e1, e0)
+            else:
+                m = self.erb_dec(emb, e3, e2, e1, e0)
             spec_m = self.mask(spec, m)
         else:
             m = torch.zeros((), device=spec.device)
             spec_m = torch.zeros_like(spec)
 
         if self.run_df:
-            df_coefs, _ = self.df_dec(emb, c0)
+            if self.lsnr_droput:
+                df_coefs[:, idcs] = self.df_dec(emb, c0)[0]
+            else:
+                df_coefs = self.df_dec(emb, c0)[0]
             df_coefs = self.df_out_transform(df_coefs)
             spec = self.df_op(spec, df_coefs)
             spec[..., self.nb_df :, :] = spec_m[..., self.nb_df :, :]
         else:
             df_coefs = torch.zeros((), device=spec.device)
             spec = spec_m
```

### Comparing `deepfilternet-0.4.0/df/deepfilternetmf.py` & `deepfilternet-0.5.0/df/deepfilternetmf.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.4.0/df/enhance.py` & `deepfilternet-0.5.0/df/enhance.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,63 +1,95 @@
 import argparse
+import glob
 import os
 import time
 import warnings
-from typing import Optional, Tuple, Union
+from typing import List, Optional, Tuple, Union
 
 import torch
 from loguru import logger
 from torch import Tensor, nn
 from torch.nn import functional as F
+from torch.utils.data import DataLoader, Dataset
 
-from df import __version__, config
 from df.checkpoint import load_model as load_model_cp
+from df.config import config
 from df.io import load_audio, resample, save_audio
 from df.logger import init_logger
 from df.model import ModelParams
 from df.modules import get_device
 from df.utils import as_complex, as_real, download_file, get_cache_dir, get_norm_alpha
+from df.version import version
 from libdf import DF, erb, erb_norm, unit_norm
 
-PRETRAINED_MODELS = ("DeepFilterNet", "DeepFilterNet2")
-DEFAULT_MODEL = "DeepFilterNet2"
+PRETRAINED_MODELS = ("DeepFilterNet", "DeepFilterNet2", "DeepFilterNet3")
+DEFAULT_MODEL = "DeepFilterNet3"
+
+
+class AudioDataset(Dataset):
+    def __init__(self, files: List[str], sr: int) -> None:
+        super().__init__()
+        self.files = []
+        for file in files:
+            if not os.path.isfile(file):
+                logger.warning(f"File not found: {file}. Skipping...")
+            self.files.append(file)
+        self.sr = sr
+
+    def __getitem__(self, index) -> Tuple[str, Tensor, int]:
+        fn = self.files[index]
+        audio, meta = load_audio(fn, self.sr, "cpu")
+        return fn, audio, meta.sample_rate
+
+    def __len__(self):
+        return len(self.files)
 
 
 def main(args):
     model, df_state, suffix = init_df(
         args.model_base_dir,
         post_filter=args.pf,
         log_level=args.log_level,
         config_allow_defaults=True,
         epoch=args.epoch,
     )
+    suffix = suffix if args.suffix else None
     if args.output_dir is None:
         args.output_dir = "."
     elif not os.path.isdir(args.output_dir):
         os.mkdir(args.output_dir)
     df_sr = ModelParams().sr
-    n_samples = len(args.noisy_audio_files)
-    for i, file in enumerate(args.noisy_audio_files):
+    if args.noisy_dir is not None:
+        if len(args.noisy_audio_files) > 0:
+            logger.error("Only one of `noisy_audio_files` or `noisy_dir` arguments are supported.")
+            exit(1)
+        input_files = glob.glob(args.noisy_dir + "/*")
+    else:
+        assert len(args.noisy_audio_files) > 0, "No audio files provided"
+        input_files = args.noisy_audio_files
+    ds = AudioDataset(input_files, df_sr)
+    loader = DataLoader(ds, num_workers=2, pin_memory=True)
+    n_samples = len(ds)
+    for i, (file, audio, audio_sr) in enumerate(loader):
+        file = file[0]
+        audio = audio.squeeze(0)
         progress = (i + 1) / n_samples * 100
-        audio, meta = load_audio(file, df_sr)
         t0 = time.time()
         audio = enhance(
             model, df_state, audio, pad=args.compensate_delay, atten_lim_db=args.atten_lim
         )
         t1 = time.time()
         t_audio = audio.shape[-1] / df_sr
         t = t1 - t0
         rtf = t / t_audio
         fn = os.path.basename(file)
         p_str = f"{progress:2.0f}% | " if n_samples > 1 else ""
         logger.info(f"{p_str}Enhanced noisy audio file '{fn}' in {t:.1f}s (RT factor: {rtf:.3f})")
-        audio = resample(audio, df_sr, meta.sample_rate)
-        save_audio(
-            file, audio, sr=meta.sample_rate, output_dir=args.output_dir, suffix=suffix, log=False
-        )
+        audio = resample(audio.to("cpu"), df_sr, audio_sr)
+        save_audio(file, audio, sr=audio_sr, output_dir=args.output_dir, suffix=suffix, log=False)
 
 
 def get_model_basedir(m: Optional[str]) -> str:
     if m is None:
         m = DEFAULT_MODEL
     is_default_model = m in PRETRAINED_MODELS
     if is_default_model:
@@ -235,14 +267,29 @@
     try:
         return int(value)
     except ValueError:
         assert value in ("best", "latest")
         return value
 
 
+class PrintVersion(argparse.Action):
+    def __init__(self, option_strings, dest):
+        super().__init__(
+            option_strings=option_strings,
+            dest=dest,
+            nargs=0,
+            required=False,
+            help="Print DeepFilterNet version information",
+        )
+
+    def __call__(self, *args):
+        print("DeepFilterNet", version)
+        exit(0)
+
+
 def setup_df_argument_parser(default_log_level: str = "INFO") -> argparse.ArgumentParser:
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "--model-base-dir",
         "-m",
         type=str,
         default=None,
@@ -272,15 +319,15 @@
     parser.add_argument(
         "--epoch",
         "-e",
         default="best",
         type=parse_epoch_type,
         help="Epoch for checkpoint loading. Can be one of ['best', 'latest', <int>].",
     )
-    parser.add_argument("--version", action="store_true")
+    parser.add_argument("-v", "--version", action=PrintVersion)
     return parser
 
 
 def run():
     parser = setup_df_argument_parser()
     parser.add_argument(
         "--compensate-delay",
@@ -294,19 +341,29 @@
         type=int,
         default=None,
         help="Attenuation limit in dB by mixing the enhanced signal with the noisy signal.",
     )
     parser.add_argument(
         "noisy_audio_files",
         type=str,
-        nargs="+",
+        nargs="*",
         help="List of noise files to mix with the clean speech file.",
     )
+    parser.add_argument(
+        "--noisy-dir",
+        "-i",
+        type=str,
+        default=None,
+        help="Input directory containing noisy audio files. Use instead of `noisy_audio_files`.",
+    )
+    parser.add_argument(
+        "--no-suffix",
+        action="store_false",
+        dest="suffix",
+        help="Don't add the model suffix to the enhanced audio files",
+    )
     args = parser.parse_args()
-    if args.version:
-        print("DeepFilterNet", __version__)
-        exit(0)
     main(args)
 
 
 if __name__ == "__main__":
     run()
```

### Comparing `deepfilternet-0.4.0/df/evaluation_utils.py` & `deepfilternet-0.5.0/df/evaluation_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,14 +91,15 @@
     noisy_files: List[str],
     metrics: List[str] = ["stoi", "composite", "sisdr"],  # type: ignore
     save_audio_callback: Optional[Callable[[str, Tensor], None]] = None,
     n_workers: int = 4,
     log_percent: int = 25,
     csv_path_enh: Optional[str] = None,
     csv_path_noisy: Optional[str] = None,
+    noisy_metric: bool = False,
     sleep_ms=0,
 ) -> Dict[str, float]:
     sr = df_state.sr()
     if n_workers >= 1:
         ctx = mp.get_context("spawn")
         pool_fn = ctx.Pool
     else:
@@ -110,15 +111,18 @@
             zip(noisy_files, clean_files), len(noisy_files), log_percent
         ):
             noisy, _ = load_audio(noisyfn, sr, method=RESAMPLE_METHOD)
             clean, _ = load_audio(cleanfn, sr, method=RESAMPLE_METHOD)
             logger.debug(f"Processing {os.path.basename(noisyfn)}, {os.path.basename(cleanfn)}")
             enh = enhance(model, df_state, noisy)[0]
             clean = df_state.synthesis(df_state.analysis(clean.numpy()))[0]
-            noisy = df_state.synthesis(df_state.analysis(noisy.numpy()))[0]
+            if noisy_metric:
+                noisy = df_state.synthesis(df_state.analysis(noisy.numpy()))[0]
+            else:
+                noisy = None
             for m in metrics:
                 m.add(clean=clean, enhanced=enh, noisy=noisy, fn=os.path.basename(noisyfn))
             if save_audio_callback is not None:
                 enh = torch.as_tensor(enh).to(torch.float32).view(1, -1)
                 save_audio_callback(cleanfn, enh)
             if sleep_ms > 0:
                 time.sleep(sleep_ms / 1000)
@@ -306,15 +310,15 @@
             self.noisy_values[k].append((fn, v))
 
     def maybe_resample(self, x) -> Tensor:
         if self.resampler is not None:
             x = self.resampler.forward(torch.as_tensor(x).clone())
         return x
 
-    def add(self, clean, enhanced, noisy, fn: Optional[str] = None):
+    def add(self, clean, enhanced, noisy=None, fn: Optional[str] = None):
         assert clean.shape == enhanced.shape, f"{clean.shape}, {enhanced.shape}, {fn}"
         clean = self.maybe_resample(clean).squeeze(0)
         enhanced = self.maybe_resample(enhanced).squeeze(0)
         values_enh = self.compute_metric(clean=clean, degraded=enhanced)
         self._add_values_enh(values_enh, fn)
         if noisy is not None:
             assert clean.shape == noisy.shape, f"{clean.shape}, {noisy.shape}, {fn}"
@@ -356,15 +360,15 @@
         target_sr: Optional[int] = None,
     ):
         super().__init__(name, source_sr=source_sr, target_sr=target_sr)
         self.pool = pool
         self.worker_results = deque()
         self.is_joined = False
 
-    def add(self, clean, enhanced, noisy, fn: Optional[str] = None):
+    def add(self, clean, enhanced, noisy=None, fn: Optional[str] = None):
         assert clean.shape == enhanced.shape, f"{clean.shape}, {enhanced.shape}, {fn}"
         if noisy is not None:
             assert clean.shape == noisy.shape, f"{clean.shape}, {noisy.shape}, {fn}"
         clean = self.maybe_resample(torch.as_tensor(clean)).squeeze(0)
         enhanced = self.maybe_resample(torch.as_tensor(enhanced)).squeeze(0)
         h = self.pool.apply_async(
             self.compute_metric,
```

### Comparing `deepfilternet-0.4.0/df/io.py` & `deepfilternet-0.5.0/df/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from torchaudio.backend.common import AudioMetaData
 
 from df.logger import warn_once
 from df.utils import download_file, get_cache_dir, get_git_root
 
 
 def load_audio(
-    file: str, sr: Optional[int], verbose=True, **kwargs
+    file: str, sr: Optional[int] = None, verbose=True, **kwargs
 ) -> Tuple[Tensor, AudioMetaData]:
     """Loads an audio file using torchaudio.
 
     Args:
         file (str): Path to an audio file.
         sr (int): Optionally resample audio to specified target sampling rate.
         **kwargs: Passed to torchaudio.load(). Depends on the backend. The resample method
```

### Comparing `deepfilternet-0.4.0/df/logger.py` & `deepfilternet-0.5.0/df/logger.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.4.0/df/loss.py` & `deepfilternet-0.5.0/df/loss.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import warnings
 from collections import defaultdict
-from typing import Dict, Final, Iterable, List, Optional, Union
+from typing import Dict, Final, Iterable, List, Literal, Optional, Tuple, Union
 
 import torch
 import torch.nn.functional as F
 from torch import Tensor, nn
 
 from df.config import Csv, config
+from df.io import resample
 from df.model import ModelParams
-from df.modules import LocalSnrTarget, erb_fb
+from df.modules import LocalSnrTarget, Mask, erb_fb
 from df.stoi import stoi
 from df.utils import angle, as_complex, get_device
 from libdf import DF
 
 
 def wg(S: Tensor, X: Tensor, eps: float = 1e-10) -> Tensor:
     N = X - S
@@ -255,26 +256,37 @@
         else:
             g_t = self.erb(clean.abs()).pow(self.gamma)  # We use directly the clean spectrum
             g_p = (self.erb(noisy.abs()) * input).pow(self.gamma_pred)
         loss = torch.zeros((), device=input.device)
         tmp = g_t.sub(g_p).pow(2)
         if self.f_under != 1:
             # Weighting if gains are too low
-            tmp *= torch.where(g_p < g_t, self.f_under, 1.0)
+            tmp = tmp * torch.where(g_p < g_t, self.f_under, 1.0)
         if max_bin is not None:
             m = torch.ones((b, 1, 1, f), device=input.device)
             for i, mb in enumerate(max_bin):
                 m[i, ..., mb:] = 0
             tmp = tmp * m
         for power, factor in zip(self.powers, self.factors):
             # Reduce the 2 from .pow(2) above
             loss += tmp.clamp_min(1e-13).pow(power // 2).mean().mul(factor) * self.factor
         return loss.mean()
 
 
+class MaskSpecLoss(nn.Module):
+    def __init__(self, df_state: DF, factor=1, gamma: float = 0.6):
+        super().__init__()
+        self.apply_mask = Mask(erb_fb(df_state.erb_widths(), ModelParams().sr, inverse=True))
+        self.loss = SpectralLoss(factor_magnitude=factor, gamma=gamma)
+
+    def forward(self, input: Tensor, clean: Tensor, noisy: Tensor) -> Tensor:
+        enh = self.apply_mask(noisy, input)
+        return self.loss(enh, clean)
+
+
 class DfAlphaLoss(nn.Module):
     """Add a penalty to use DF for very noisy segments.
 
     Starting from lsnr_thresh, the penalty is increased and has its maximum at lsnr_min.
     """
 
     factor: Final[float]
@@ -389,14 +401,246 @@
 
     def forward(self, input: Tensor, target_lsnr: Tensor):
         # input (freq-domain): [B, T, 1]
         input = input.squeeze(-1)
         return F.mse_loss(input, target_lsnr) * self.factor
 
 
+class ASRLoss(nn.Module):
+    target_sr = 16000
+    n_fft = 400
+    hop = 160
+    beam_size = 20
+    lang = "en"
+    task = "transcribe"
+    max_ctx = 25
+
+    def __init__(
+        self,
+        sr: int,
+        factor: float = 1,
+        factor_lm: float = 1,
+        loss_lm: Literal["CTC", "CrossEntropy"] = "CrossEntropy",
+        model: str = "base.en",
+    ) -> None:
+        super().__init__()
+        import whisper
+
+        self.sr = sr
+        self.factor = factor
+        self.factor_lm = factor_lm
+        self.model = whisper.load_model(model)
+        self.model.requires_grad_(False)
+        self.options = whisper.DecodingOptions(
+            task=self.task, language=self.lang, without_timestamps=True, sample_len=self.max_ctx
+        )
+        self.mel_filters: Tensor
+        self.register_buffer(
+            "mel_filters", torch.from_numpy(self.get_mel_filters(self.target_sr, 400, 80))
+        )
+        self.tokenizer = whisper.tokenizer.get_tokenizer(
+            self.model.is_multilingual, language=self.lang, task=self.options.task
+        )
+        self.decoder = whisper.decoding.GreedyDecoder(0.0, self.tokenizer.eot)
+        # self.decoder = whisper.decoding.BeamSearchDecoder(self.beam_size, self.tokenizer.eot, , 1.)
+        self.sot_sequence = self.tokenizer.sot_sequence_including_notimestamps
+        self.n_ctx: int = self.model.dims.n_text_ctx
+        self.initial_tokens = self._get_initial_tokens()
+        self.sot_index: int = self.initial_tokens.index(self.tokenizer.sot)
+        self.sample_begin: int = len(self.initial_tokens)
+        self.sample_len: int = self.options.sample_len or self.model.dims.n_text_ctx // 2
+        self.blank = self.tokenizer.encode(" ")[0]
+        self.eot = self.tokenizer.eot
+        self.loss_lm = loss_lm
+
+    def forward(self, input: Tensor, target: Tensor) -> Tensor:
+        features_i = self.model.embed_audio(self.preprocess(input))
+        features_t = self.model.embed_audio(self.preprocess(target))
+        # Loss based on the audio encoding:
+        loss = 0
+        if self.factor > 0:
+            loss = F.mse_loss(features_i[0], features_t[0]) * self.factor
+        if self.factor_lm > 0:
+            _, tokens_t = self.decode_tokens(features_t)  # [N, S]
+            logits_i, tokens_i = self.decode_tokens(features_i)  # [N, T, C]
+            log_probs_i = F.log_softmax(logits_i, dim=-1)
+
+            # Loss based on the logits:
+            if self.factor_lm > 0:
+                if self.loss_lm == "CTC":
+                    input_lengths = torch.as_tensor(
+                        [torch.argwhere(t == self.eot)[0] for t in tokens_i],
+                        device=input.device,
+                        dtype=torch.long,
+                    )
+                    target_lengths = torch.as_tensor(
+                        [torch.argwhere(t == self.eot)[0] for t in tokens_t],
+                        device=input.device,
+                        dtype=torch.long,
+                    )
+                    ctc_loss = F.ctc_loss(
+                        log_probs=log_probs_i[:, : input_lengths.max()].transpose(0, 1),
+                        targets=tokens_t[:, : target_lengths.max()].to(torch.long),
+                        input_lengths=input_lengths,
+                        target_lengths=target_lengths,
+                        blank=self.blank,
+                        zero_infinity=True,
+                    )
+                    loss += ctc_loss * self.factor_lm
+                else:
+                    delta = log_probs_i.shape[1] - tokens_t.shape[1]
+                    if delta > 0:
+                        tokens_t = torch.cat(
+                            (
+                                tokens_t,
+                                torch.full(
+                                    (tokens_t.shape[0], delta),
+                                    self.eot,
+                                    device=tokens_t.device,
+                                    dtype=tokens_t.dtype,
+                                ),
+                            ),
+                            dim=1,
+                        )
+                    # if tokens_t.shape[1] != log_probs_i.shape[1]:
+                    #     ic(tokens_t.shape, log_probs_i.shape)
+                    #     for i in range(tokens_t.shape[0]):
+                    #         ic(tokens_t[i])
+                    #         ic(log_probs_i[i].argmax(dim=-1))
+                    ce_loss = F.nll_loss(
+                        log_probs_i.flatten(0, 1),
+                        tokens_t[:, : tokens_i.shape[1]].flatten(0, 1),
+                    )
+                    loss += ce_loss * self.factor_lm
+        return loss
+
+    def decode_text(self, tokens: Tensor) -> List[str]:
+        tokens = [t[: torch.argwhere(t == self.eot)[0]] for t in tokens]
+        return [self.tokenizer.decode(t).strip() for t in tokens]
+
+    def decode_tokens(
+        self,
+        features: Tensor,
+        start_tokens: Optional[Tensor] = None,
+    ) -> Tuple[Tensor, Tensor]:
+        n = features.shape[0]
+        sum_logprobs: Tensor = torch.zeros(n, device=features.device)
+        tokens: Tensor = start_tokens or torch.tensor(
+            [self.initial_tokens], device=features.device
+        ).repeat(n, 1)
+        logits: List[Tensor] = []
+        for i in range(self.sample_len):
+            # we don't need no_speech_probs, only use last index (-1)
+            logits.append(self.model.logits(tokens, features)[:, -1])
+            tokens, completed = self.decoder.update(tokens, logits[-1], sum_logprobs)
+            if completed or tokens.shape[-1] > self.n_ctx:
+                break
+        tokens, _ = self.decoder.finalize(tokens, sum_logprobs)
+        return torch.stack(logits, dim=1), tokens[:, self.sample_begin : -1]
+
+    def preprocess(self, audio: Tensor) -> Tensor:
+        import whisper
+
+        audio = resample(audio, self.sr, self.target_sr)
+        audio = whisper.pad_or_trim(audio.squeeze(1))
+        mel = self.log_mel_spectrogram(audio, self.mel_filters.to(audio.device))
+        return mel
+
+    def log_mel_spectrogram(self, audio: Tensor, mel_fb: Tensor):
+        """From openai/whisper"""
+        window = torch.hann_window(self.n_fft).to(audio.device)
+        stft = torch.stft(audio, self.n_fft, self.hop, window=window, return_complex=True)
+        assert stft.isfinite().all()
+        magnitudes = stft[..., :-1].abs() ** 2
+        assert magnitudes.isfinite().all()
+        assert mel_fb.isfinite().all()
+
+        mel_spec = mel_fb @ magnitudes
+
+        log_spec = torch.clamp(mel_spec, min=1e-10).log10()
+        log_spec = torch.maximum(log_spec, log_spec.max() - 8.0)
+        log_spec = (log_spec + 4.0) / 4.0
+        return log_spec
+
+    def get_mel_filters(self, sr, n_fft, n_mels=128, dtype=None):
+        """From transformers/models/whisper/feature_extraction"""
+        import numpy as np
+
+        dtype = dtype or np.float32
+        # Initialize the weights
+        n_mels = int(n_mels)
+        weights = np.zeros((n_mels, int(1 + n_fft // 2)), dtype=dtype)
+
+        # Center freqs of each FFT bin
+        fftfreqs = np.fft.rfftfreq(n=n_fft, d=1.0 / sr)
+
+        # 'Center freqs' of mel bands - uniformly spaced between limits
+        min_mel = 0.0
+        max_mel = 45.245640471924965
+
+        mels = np.linspace(min_mel, max_mel, n_mels + 2)
+
+        mels = np.asanyarray(mels)
+
+        # Fill in the linear scale
+        f_min = 0.0
+        f_sp = 200.0 / 3
+        freqs = f_min + f_sp * mels
+
+        # And now the nonlinear scale
+        min_log_hz = 1000.0  # beginning of log region (Hz)
+        min_log_mel = (min_log_hz - f_min) / f_sp  # same (Mels)
+        logstep = np.log(6.4) / 27.0  # step size for log region
+
+        # If we have vector data, vectorize
+        log_t = mels >= min_log_mel
+        freqs[log_t] = min_log_hz * np.exp(logstep * (mels[log_t] - min_log_mel))
+
+        mel_f = freqs
+
+        fdiff = np.diff(mel_f)
+        ramps = np.subtract.outer(mel_f, fftfreqs)
+
+        for i in range(n_mels):
+            # lower and upper slopes for all bins
+            lower = -ramps[i] / fdiff[i]
+            upper = ramps[i + 2] / fdiff[i + 1]
+
+            # .. then intersect them with each other and zero
+            weights[i] = np.maximum(0, np.minimum(lower, upper))
+
+        # Slaney-style mel is scaled to be approx constant energy per channel
+        enorm = 2.0 / (mel_f[2 : n_mels + 2] - mel_f[:n_mels])
+        weights *= enorm[:, np.newaxis]
+
+        return weights
+
+    def _get_initial_tokens(self) -> Tuple[int]:
+        tokens = list(self.sot_sequence)
+        prefix = self.options.prefix
+        prompt = self.options.prompt
+
+        if prefix:
+            prefix_tokens = (
+                self.tokenizer.encode(" " + prefix.strip()) if isinstance(prefix, str) else prefix
+            )
+            if self.sample_len is not None:
+                max_prefix_len = self.n_ctx // 2 - self.sample_len
+                prefix_tokens = prefix_tokens[-max_prefix_len:]
+            tokens = tokens + prefix_tokens
+
+        if prompt:
+            prompt_tokens = (
+                self.tokenizer.encode(" " + prompt.strip()) if isinstance(prompt, str) else prompt
+            )
+            tokens = [self.tokenizer.sot_prev] + prompt_tokens[-(self.n_ctx // 2 - 1) :] + tokens
+
+        return tuple(tokens)
+
+
 class Loss(nn.Module):
     """Loss wrapper containing several different loss functions within this file.
 
     The configuration is done via the config file.
     """
 
     def __init__(self, state: DF, istft: Optional[Istft] = None):
@@ -417,24 +661,27 @@
         self.summaries: Dict[str, List[Tensor]] = self.reset_summaries()
         # Mask Loss
         self.ml_f = config("factor", 0, float, section="MaskLoss")  # e.g. 1
         self.ml_mask = config("mask", "iam", str, section="MaskLoss")  # e.g. 1
         self.ml_gamma = config("gamma", 0.6, float, section="MaskLoss")
         self.ml_gamma_pred = config("gamma_pred", 0.6, float, section="MaskLoss")
         self.ml_f_under = config("f_under", 2, float, section="MaskLoss")
-        self.ml = MaskLoss(
-            state,
-            mask=self.ml_mask,
-            factor=self.ml_f,
-            f_under=self.ml_f_under,
-            gamma=self.ml_gamma,
-            gamma_pred=self.ml_gamma_pred,
-            factors=[1, 10],
-            powers=[2, 4],
-        )
+        if self.ml_mask == "spec":
+            self.ml = MaskSpecLoss(state, self.ml_f, self.ml_gamma)
+        else:
+            self.ml = MaskLoss(
+                state,
+                mask=self.ml_mask,
+                factor=self.ml_f,
+                f_under=self.ml_f_under,
+                gamma=self.ml_gamma,
+                gamma_pred=self.ml_gamma_pred,
+                factors=[1, 10],
+                powers=[2, 4],
+            )
         # SpectralLoss
         self.sl_fm = config("factor_magnitude", 0, float, section="SpectralLoss")  # e.g. 1e4
         self.sl_fc = config("factor_complex", 0, float, section="SpectralLoss")
         self.sl_fu = config("factor_under", 1, float, section="SpectralLoss")
         self.sl_gamma = config("gamma", 1, float, section="SpectralLoss")
         self.sl_f = self.sl_fm + self.sl_fc
         if self.sl_f > 0:
@@ -464,98 +711,84 @@
                 self.sdrl = SegSdrLoss(sdr_sgemental_ws, factor=self.sdrl_f)
             else:
                 self.sdrl = SdrLoss(self.sdrl_f)
         self.lsnr_f = config("factor", 0.0005, float, section="LocalSnrLoss")
         self.lsnrl = LocalSnrLoss(self.lsnr_f) if self.lsnr_f > 0 else None
         self.dev_str = get_device().type
 
+        self.asrl = None
+        self.asrl_f = config("factor", 0, float, section="ASRLoss")
+        self.asrl_f_lm = config("factor_lm", 0, float, section="ASRLoss")
+        self.asrl_loss_lm = config("loss_lm", "CrossEntropy", str, section="ASRLoss")
+        self.asrl_m = config("model", "base.en", str, section="ASRLoss")
+        if self.asrl_f > 0 or self.asrl_f_lm > 0:
+            self.asrl = ASRLoss(
+                sr=self.sr,
+                factor=self.asrl_f,
+                factor_lm=self.asrl_f_lm,
+                loss_lm=self.asrl_loss_lm,
+                model=self.asrl_m,
+            )
+
     def forward(
         self,
         clean: Tensor,
         noisy: Tensor,
         enhanced: Tensor,
         mask: Tensor,
         lsnr: Tensor,
         snrs: Tensor,
         max_freq: Optional[Tensor] = None,
-        multi_stage_specs: List[Tensor] = [],
     ):
         """Computes all losses.
 
         Args:
             clean (Tensor): Clean complex spectrum of shape [B, C, T, F].
             noisy (Tensor): Noisy complex spectrum of shape [B, C, T, F].
             enhanced (Tensor): Enhanced complex spectrum of shape [B, C, T, F].
             mask (Tensor): Mask (real-valued) estimate of shape [B, C, T, E], E: Number of ERB bins.
             lsnr (Tensor): Local SNR estimates of shape [B, T, 1].
             snrs (Tensor): Input SNRs of the noisy mixture of shape [B].
-            max_freq (Optional, Tensor): Maximum frequency present in the noisy mixtrue (e.g. due to a lower sampling rate) of shape [B].
-            multi_stage_specs (Optional, Tensor): Enhanced complex spectrums of different intermediate outputs of the DNN.
         """
-        max_bin: Optional[Tensor] = None
-        if max_freq is not None:
-            max_bin = (
-                max_freq.to(device=clean.device)
-                .mul(self.fft_size)
-                .div(self.sr, rounding_mode="trunc")
-            ).long()
         enhanced_td = None
         clean_td = None
-        multi_stage = None
-        multi_stage_td = None
-        if multi_stage_specs:
-            # Stack spectrograms in a channel dimension
-            multi_stage = as_complex(torch.stack(multi_stage_specs, dim=1))
         lsnr_gt = self.lsnr(clean, noise=noisy - clean)
         if self.istft is not None:
             if self.store_losses or self.mrsl is not None or self.sdrl is not None:
                 enhanced_td = self.istft(enhanced)
                 clean_td = self.istft(clean)
-                if multi_stage is not None:
-                    # leave out erb enhanced
-                    multi_stage_td = self.istft(multi_stage)
 
-        ml, sl, mrsl, cal, sdrl, lsnrl = [torch.zeros((), device=clean.device)] * 6
+        ml, sl, mrsl, cal, sdrl, asrl, lsnrl = [torch.zeros((), device=clean.device)] * 7
         if self.ml_f != 0 and self.ml is not None:
-            ml = self.ml(input=mask, clean=clean, noisy=noisy, max_bin=max_bin)
+            ml = self.ml(input=mask, clean=clean, noisy=noisy)
         if self.sl_f != 0 and self.sl is not None:
-            sl = torch.zeros((), device=clean.device)
-            if multi_stage is not None:
-                sl += self.sl(input=multi_stage, target=clean.expand_as(multi_stage))
-            else:
-                sl = self.sl(input=enhanced, target=clean)
+            sl = self.sl(input=enhanced, target=clean)
         if self.mrsl_f > 0 and self.mrsl is not None:
-            if multi_stage_td is not None:
-                ms = multi_stage_td[:, 1:]
-                mrsl = self.mrsl(ms, clean_td.expand_as(ms))
-            else:
-                mrsl = self.mrsl(enhanced_td, clean_td)
+            mrsl = self.mrsl(enhanced_td, clean_td)
+        if self.asrl_f > 0 or self.asrl_f_lm > 0:
+            asrl = self.asrl(enhanced_td, clean_td)
         if self.lsnr_f != 0:
             lsnrl = self.lsnrl(input=lsnr, target_lsnr=lsnr_gt)
         if self.sdrl_f != 0:
-            if multi_stage_td is not None:
-                ms = multi_stage_td[:, 1:]
-                sdrl = self.sdrl(ms, clean_td.expand_as(ms))
-            else:
-                sdrl = self.sdrl(enhanced_td, clean_td)
+            sdrl = self.sdrl(enhanced_td, clean_td)
         if self.store_losses and enhanced_td is not None:
             assert clean_td is not None
             self.store_summaries(
                 enhanced_td,
                 clean_td,
                 snrs,
                 ml,
                 sl,
                 mrsl,
                 sdrl,
+                asrl,
                 lsnrl,
                 cal,
-                multi_stage_td=multi_stage_td,
             )
-        return ml + sl + mrsl + sdrl + lsnrl + cal
+        return ml + sl + mrsl + sdrl + asrl + lsnrl + cal
 
     def reset_summaries(self):
         self.summaries = defaultdict(list)
         return self.summaries
 
     @torch.jit.ignore  # type: ignore
     def get_summaries(self):
@@ -568,42 +801,38 @@
         enh_td: Tensor,
         clean_td: Tensor,
         snrs: Tensor,
         ml: Tensor,
         sl: Tensor,
         mrsl: Tensor,
         sdrl: Tensor,
+        asrl: Tensor,
         lsnrl: Tensor,
         cal: Tensor,
-        multi_stage_td: Optional[Tensor] = None,
     ):
         if ml != 0:
             self.summaries["MaskLoss"].append(ml.detach())
         if sl != 0:
             self.summaries["SpectralLoss"].append(sl.detach())
         if mrsl != 0:
             self.summaries["MultiResSpecLoss"].append(mrsl.detach())
         if sdrl != 0:
             self.summaries["SdrLoss"].append(sdrl.detach())
         if cal != 0:
             self.summaries["DfAlphaLoss"].append(cal.detach())
+        if asrl != 0:
+            self.summaries["ASRLoss"].append(asrl.detach())
         if lsnrl != 0:
             self.summaries["LocalSnrLoss"].append(lsnrl.detach())
         sdr = SiSdr()
         enh_td = enh_td.squeeze(1).detach()
         clean_td = clean_td.squeeze(1).detach()
         sdr_vals: Tensor = sdr(enh_td, target=clean_td)
         stoi_vals: Tensor = stoi(y=enh_td, x=clean_td, fs_source=self.sr)
         sdr_vals_ms, stoi_vals_ms = [], []
-        if multi_stage_td is not None:
-            for i in range(multi_stage_td.shape[1]):
-                sdr_vals_ms.append(sdr(multi_stage_td[:, i].detach(), clean_td))
-                stoi_vals_ms.append(
-                    stoi(y=multi_stage_td[:, i].detach(), x=clean_td, fs_source=self.sr)
-                )
         for snr in torch.unique(snrs, sorted=False):
             self.summaries[f"sdr_snr_{snr.item()}"].extend(
                 sdr_vals.masked_select(snr == snrs).detach().split(1)
             )
             self.summaries[f"stoi_snr_{snr.item()}"].extend(
                 stoi_vals.masked_select(snr == snrs).detach().split(1)
             )
```

### Comparing `deepfilternet-0.4.0/df/lr.py` & `deepfilternet-0.5.0/df/lr.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.4.0/df/model.py` & `deepfilternet-0.5.0/df/model.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.4.0/df/modules.py` & `deepfilternet-0.5.0/df/modules.py`

 * *Files 0% similar despite different names*

```diff
@@ -260,15 +260,17 @@
                 mask = mask.clamp(min=atten_lim.view(-1, 1, 1, 1))
             else:
                 m_out = []
                 for i in range(atten_lim.shape[0]):
                     m_out.append(mask[i].clamp_min(atten_lim[i].item()))
                 mask = torch.stack(m_out, dim=0)
         mask = mask.matmul(self.erb_inv_fb)  # [B, 1, T, F]
-        return spec * mask.unsqueeze(4)
+        if not spec.is_complex():
+            mask = mask.unsqueeze(4)
+        return spec * mask
 
 
 class ExponentialUnitNorm(nn.Module):
     """Unit norm for a complex spectrogram.
 
     This should match the rust code:
     ```rust
```

### Comparing `deepfilternet-0.4.0/df/multiframe.py` & `deepfilternet-0.5.0/df/multiframe.py`

 * *Files 0% similar despite different names*

```diff
@@ -561,15 +561,14 @@
 
     config.use_defaults(allow_reload=True)
     p = ModelParams()
     p.fft_size = 96
     p.hop_size = 24
     p.sr = 24000
     n_freqs = p.fft_size // 2 + 1
-    n_freqs = p.fft_size // 2 + 1
 
     df = libdf.DF(sr=p.sr, fft_size=p.fft_size, hop_size=p.hop_size, nb_bands=p.nb_erb)
     s = load_audio("assets/clean_freesound_33711.wav", p.sr, num_frames=5 * p.sr)[0].mean(
         0, keepdim=True
     )
     n = load_audio("assets/noise_freesound_2530.wav", p.sr, num_frames=5 * p.sr)[0].mean(
         0, keepdim=True
```

### Comparing `deepfilternet-0.4.0/df/scripts/dnsmos.py` & `deepfilternet-0.5.0/df/scripts/dnsmos.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,19 +47,20 @@
 ]
 ORT_SESS = {}
 
 __a_tol = 1e-4
 __r_tol = 1e-4
 
 
-def get_ort_session(onnx: str):
+def get_ort_session(onnx: str, providers="gpu"):
     global ORT_SESS
 
     import onnxruntime as ort
 
+    providers = ORT_PROVIDERS_ALL if providers == "gpu" else ORT_PROVIDERS_CPU
     if onnx not in ORT_SESS:
         try:
             with warnings.catch_warnings():
                 warnings.simplefilter("ignore", UserWarning)
                 sess = ort.InferenceSession(onnx, providers=ORT_PROVIDERS_ALL)
         except ValueError:
             sess = ort.InferenceSession(onnx, providers=ORT_PROVIDERS_CPU)
```

### Comparing `deepfilternet-0.4.0/df/scripts/dnsmos_v2.py` & `deepfilternet-0.5.0/df/scripts/dnsmos_v2.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.4.0/df/scripts/export.py` & `deepfilternet-0.5.0/df/scripts/export.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import shutil
 import tarfile
 from copy import deepcopy
+from pathlib import Path
 from typing import Dict, Iterable, List, Tuple, Union
 
 import numpy as np
 import onnx
 import onnx.checker
 import onnx.helper
 import onnxruntime as ort
@@ -59,15 +60,15 @@
     return path
 
 
 def onnx_check(path: str, input_dict: Dict[str, Tensor], output_names: Tuple[str]):
     model = onnx.load(path)
     logger.debug(os.path.basename(path) + ": " + onnx.helper.printable_graph(model.graph))
     onnx.checker.check_model(model, full_check=True)
-    sess = ort.InferenceSession(path)
+    sess = ort.InferenceSession(path, providers=["CPUExecutionProvider"])
     return sess.run(output_names, {k: v.numpy() for (k, v) in input_dict.items()})
 
 
 def export_impl(
     path: str,
     model: torch.nn.Module,
     inputs: Tuple[Tensor, ...],
@@ -108,15 +109,15 @@
         opset_version=opset_version,
         keep_initializers_as_inputs=False,
     )
 
     input_dict = {k: v for (k, v) in zip(input_names, inputs)}
     if check:
         onnx_outputs = onnx_check(path, input_dict, tuple(output_names))
-        for (name, out, onnx_out) in zip(output_names, outputs, onnx_outputs):
+        for name, out, onnx_out in zip(output_names, outputs, onnx_outputs):
             try:
                 np.testing.assert_allclose(
                     out.numpy().squeeze(), onnx_out.squeeze(), rtol=1e-6, atol=1e-5
                 )
             except AssertionError as e:
                 logger.warning(f"  Elements not close for {name}: {e}")
     if simplify:
@@ -299,32 +300,35 @@
         log_level=args.log_level,
         log_file="export.log",
         config_allow_defaults=True,
         epoch=args.epoch,
     )
     sample = get_test_sample(df_state.sr())
     enhanced = enhance(model, df_state, sample, True)
-    save_audio("out/enhanced.wav", enhanced, df_state.sr())
-    if not os.path.isdir(args.export_dir):
-        os.makedirs(args.export_dir)
+    out_dir = Path("out")
+    if out_dir.is_dir():
+        # attempt saving enhanced audio
+        save_audio(out_dir / "enhanced.wav", enhanced, df_state.sr())
+    export_dir = Path(args.export_dir)
+    export_dir.mkdir(parents=True, exist_ok=True)
     export(
         model,
-        args.export_dir,
+        export_dir,
         df_state=df_state,
         opset=args.opset,
         check=args.check,
         simplify=args.simplify,
     )
     model_base_dir = get_model_basedir(args.model_base_dir)
     if model_base_dir != args.export_dir:
         shutil.copyfile(
             os.path.join(model_base_dir, "config.ini"),
             os.path.join(args.export_dir, "config.ini"),
         )
-    tar_name = os.path.join(args.export_dir, os.path.basename(model_base_dir) + "_onnx.tar.gz")
+    tar_name = export_dir / (Path(model_base_dir).name + "_onnx.tar.gz")
     with tarfile.open(tar_name, mode="w:gz") as f:
         f.add(os.path.join(args.export_dir, "enc.onnx"))
         f.add(os.path.join(args.export_dir, "erb_dec.onnx"))
         f.add(os.path.join(args.export_dir, "df_dec.onnx"))
         f.add(os.path.join(args.export_dir, "config.ini"))
```

### Comparing `deepfilternet-0.4.0/df/scripts/filter_dnsmos.py` & `deepfilternet-0.5.0/df/scripts/filter_dnsmos.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,25 +41,25 @@
     else:
         t = [4.2, 4.5, 4.0]
 
     with h5py.File(args.hdf5_input, "r") as h5_read, h5py.File(args.hdf5_filtered, "a") as h5_write:
         print(f"Opened datatset {args.hdf5_input}")
 
         # Copy attributes
-        for (k, v) in h5_read.attrs.items():
+        for k, v in h5_read.attrs.items():
             h5_write.attrs[k] = v
 
         sr: int = h5_read.attrs["sr"]
         if sr is None:
             print("sr not found.", file=sys.stderr)
             exit(1)
         codec = h5_read.attrs.get("codec", "pcm")
         codec_write = args.codec or codec
         h5_write.attrs["codec"] = codec_write
-        for (grp_name, group_read) in h5_read.items():
+        for grp_name, group_read in h5_read.items():
             if grp_name not in h5_write:
                 group_write = h5_write.create_group(grp_name)
             else:
                 group_write = h5_write[grp_name]
             for key, ds in group_read.items():
                 encoded = ds[...]
                 if codec == "pcm":
@@ -90,15 +90,15 @@
                             audio = audio.unsqueeze(0)
                         data = encode(audio, sr, codec_write, compression=8)
                     if key in group_write:
                         del group_write[key]
                     ds_write = group_write.create_dataset(
                         key, data=data, compression=None if codec_write != "pcm" else ds.compression
                     )
-                    for (k, v) in ds.attrs.items():
+                    for k, v in ds.attrs.items():
                         ds_write.attrs[k] = v
                     ds_write.attrs["n_samples"] = audio.shape[-1]
                 else:
                     print("skipping.")
 
 
 if __name__ == "__main__":
```

### Comparing `deepfilternet-0.4.0/df/scripts/fix_n_samples_hdf5.py` & `deepfilternet-0.5.0/df/scripts/fix_n_samples_hdf5.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.4.0/df/scripts/list_attrs_in_hdf5.py` & `deepfilternet-0.5.0/df/scripts/list_attrs_in_hdf5.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.4.0/df/scripts/model_summary.py` & `deepfilternet-0.5.0/df/scripts/model_summary.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.4.0/df/scripts/plot_lrs.py` & `deepfilternet-0.5.0/df/scripts/plot_lrs.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.4.0/df/scripts/plot_spec.py` & `deepfilternet-0.5.0/df/scripts/plot_spec.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.4.0/df/scripts/plot_summaries.py` & `deepfilternet-0.5.0/df/scripts/plot_summaries.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.4.0/df/scripts/prepare_data.py` & `deepfilternet-0.5.0/df/scripts/prepare_data.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.4.0/df/scripts/sample_from_hdf5.py` & `deepfilternet-0.5.0/df/scripts/sample_from_hdf5.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.4.0/df/scripts/split_hdf5.py` & `deepfilternet-0.5.0/df/scripts/split_hdf5.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.4.0/df/scripts/test_df.py` & `deepfilternet-0.5.0/df/scripts/test_df.py`

 * *Files 9% similar despite different names*

```diff
@@ -60,14 +60,25 @@
             2.75626921653748,
             3.51172018051147,
             -0.91267710924149,
         ],
         "stoi": 0.9725977621169399,
         "sdr": 19.41733717918396,
     },
+    "DeepFilterNet3": {
+        "composite": [
+            3.04712939262390,
+            4.23114347457886,
+            2.77058529853821,
+            3.61812996864319,
+            -1.51538455486298,
+        ],
+        "stoi": 0.9742409586906433,
+        "sdr": 20.014915466308594,
+    },
 }
 
 
 def _get_metric(name: str, sr: int):
     METRICS = {
         "composite": [partial(composite, sr=sr), partial(composite, sr=sr, use_octave=True)],
         "stoi": [partial(stoi, sr=sr)],
@@ -125,10 +136,14 @@
         model = "DeepFilterNet"
         self._test_model(*self.models[model], target_metrics=TARGET_METRICS[model], prefix=model)
 
     def test_deepfilternet2(self):
         model = "DeepFilterNet2"
         self._test_model(*self.models[model], target_metrics=TARGET_METRICS[model], prefix=model)
 
+    def test_deepfilternet3(self):
+        model = "DeepFilterNet3"
+        self._test_model(*self.models[model], target_metrics=TARGET_METRICS[model], prefix=model)
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `deepfilternet-0.4.0/df/scripts/test_dns_2020.py` & `deepfilternet-0.5.0/df/scripts/test_dns_2020.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.4.0/df/scripts/test_noisy_dnsmos.py` & `deepfilternet-0.5.0/df/scripts/test_noisy_dnsmos.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.4.0/df/scripts/test_voicebank_demand.py` & `deepfilternet-0.5.0/df/scripts/test_voicebank_demand.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,14 +37,15 @@
         clean_files,
         noisy_files,
         n_workers=args.metric_workers,
         save_audio_callback=save_audio_callback if args.output_dir is not None else None,
         metrics=["stoi", "composite", "sisdr"],
         csv_path_enh=args.csv_path_enh,
         csv_path_noisy=args.csv_path_noisy,
+        noisy_metric=args.compute_noisy_metric,
         sleep_ms=args.sleep_ms,
     )
     for k, v in metrics.items():
         logger.info(f"{k}: {v}")
 
 
 if __name__ == "__main__":
@@ -69,10 +70,11 @@
     )
     parser.add_argument(
         "--csv-path-noisy",
         type=str,
         default=None,
         help="Path to csv score file containing metrics of noisy audios.",
     )
+    parser.add_argument("--compute-noisy-metric", action="store_true")
     parser.add_argument("--sleep-ms", type=int, default=0)
     args = parser.parse_args()
     main(args)
```

### Comparing `deepfilternet-0.4.0/df/sepm.py` & `deepfilternet-0.5.0/df/sepm.py`

 * *Files 0% similar despite different names*

```diff
@@ -293,15 +293,14 @@
                 n = n - 1
             loc_peaks[ii] = energy[n + 1]
 
     return loc_peaks
 
 
 def wss(clean_speech, processed_speech, fs, frameLen=0.03, overlap=0.75):
-
     Kmax = 20  # value suggested by Klatt, pg 1280
     Klocmax = 1  # value suggested by Klatt, pg 1280
     alpha = 0.95
     if clean_speech.shape != processed_speech.shape:
         raise ValueError("The two signals do not match!")
     eps = np.finfo(np.float64).eps
     clean_speech = clean_speech.astype(np.float64) + eps
```

### Comparing `deepfilternet-0.4.0/df/stoi.py` & `deepfilternet-0.5.0/df/stoi.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.4.0/df/train.py` & `deepfilternet-0.5.0/df/train.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,14 +151,15 @@
         nb_spec=p.nb_df,
         norm_alpha=get_norm_alpha(log=False),
         p_reverb=config("p_reverb", 0.2, float, section="distortion"),
         p_bw_ext=config("p_bandwidth_ext", 0.0, float, section="distortion"),
         p_clipping=config("p_clipping", 0.0, float, section="distortion"),
         p_zeroing=config("p_zeroing", 0.0, float, section="distortion"),
         p_air_absorption=config("p_air_absorption", 0.0, float, section="distortion"),
+        p_interfer_sp=config("p_interfer_sp", 0.0, float, section="distortion"),
         prefetch=config("NUM_PREFETCH_BATCHES", 32, int, section="train"),
         overfit=overfit,
         seed=seed,
         min_nb_erb_freqs=p.min_nb_freqs,
         log_timings=log_timings,
         global_sampling_factor=config("GLOBAL_DS_SAMPLING_F", 1.0, float, section="train"),
         snrs=config("DATALOADER_SNRS", [-5, 0, 5, 10, 20, 40], Csv(int), section="train"),  # type: ignore
@@ -227,15 +228,15 @@
         log_metrics(f"[{epoch - 1}] [valid]", metrics)
     losses.reset_summaries()
     # Save default values to disk
     config.save(os.path.join(args.base_dir, "config.ini"))
     for epoch in range(epoch, max_epochs):
         if len(batch_size_scheduling) > 0:
             # Get current batch size
-            for (e, b) in batch_size_scheduling:
+            for e, b in batch_size_scheduling:
                 if e <= epoch:
                     # Update bs, but don't go higher than the batch size specified in the config
                     scheduling_bs = min(b, bs)
             if prev_scheduling_bs != scheduling_bs:
                 logger.info(f"Batch scheduling | Setting batch size to {scheduling_bs}")
                 dataloader.set_batch_size(scheduling_bs, "train")
                 # Update lr/wd scheduling since dataloader len changed
@@ -371,28 +372,16 @@
             else:
                 input = as_real(noisy)
             enh, m, lsnr, other = model.forward(
                 spec=input,
                 feat_erb=feat_erb,
                 feat_spec=feat_spec,
             )
-            multi_stage_specs = []
-            if isinstance(other, (list, tuple)):
-                multi_stage_specs = other
             try:
-                err = losses.forward(
-                    clean,
-                    noisy,
-                    enh,
-                    m,
-                    lsnr,
-                    max_freq=batch.max_freq,
-                    snrs=snrs,
-                    multi_stage_specs=multi_stage_specs,
-                )
+                err = losses.forward(clean, noisy, enh, m, lsnr, snrs=snrs)
             except Exception as e:
                 if "nan" in str(e).lower() or "finite" in str(e).lower():
                     logger.warning("NaN in loss computation: {}. Skipping backward.".format(str(e)))
                     check_finite_module(model)
                     n_nans += 1
                     if n_nans > MAX_NANS:
                         raise e
@@ -437,15 +426,15 @@
             l_dict = {"loss": l_mean.item()}
             if lr_scheduler_values is not None:
                 l_dict["lr"] = opt.param_groups[0]["lr"]
             if wd_scheduler_values is not None:
                 l_dict["wd"] = opt.param_groups[0]["weight_decay"]
             if log_timings:
                 l_dict["t_sample"] = batch.timings[:-1].sum()
-                l_dict["t_batch"] = batch.timings[-1].mean()  # last if for whole batch
+                l_dict["t_batch"] = batch.timings[-1].mean()  # last is for whole batch
             if debug:
                 l_dict.update(
                     {
                         n: torch.mean(torch.stack(vals[-bs:])).item()
                         for n, vals in losses.get_summaries()
                     }
                 )
```

### Comparing `deepfilternet-0.4.0/df/utils.py` & `deepfilternet-0.5.0/df/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from socket import gethostname
 from typing import Any, Optional, Set, Tuple, Union
 
 import numpy as np
 import torch
 from loguru import logger
 from torch import Tensor
-from torch._six import string_classes
 from torch.autograd import Function
 from torch.types import Number
 
 from df.config import config
 from df.model import ModelParams
 
 
@@ -180,15 +179,15 @@
     """Apply a function on a tensor or mapping, or sequence of tensors."""
     if isinstance(input_, torch.nn.Module):
         return [apply_to_tensor(c, func) for c in input_.children()]
     elif isinstance(input_, torch.nn.Parameter):
         return func(input_.data)
     elif isinstance(input_, Tensor):
         return func(input_)
-    elif isinstance(input_, string_classes):
+    elif isinstance(input_, (str, bytes)):
         return input_
     elif isinstance(input_, collections.Mapping):
         return {k: apply_to_tensor(sample, func) for k, sample in input_.items()}
     elif isinstance(input_, collections.Iterable):
         return [apply_to_tensor(sample, func) for sample in input_]
     elif input_ is None:
         return input_
@@ -210,15 +209,15 @@
 
     import requests
 
     local_filename = url.split("/")[-1]
     local_filename = os.path.join(download_dir, local_filename)
     with requests.get(url, stream=True) as r:
         if r.status_code >= 400:
-            logger.error(f"Error downloading file ({r.status_code}): {r.reason}")
+            logger.error(f"Error downloading file {url} ({r.status_code}): {r.reason}")
             exit(1)
         with open(local_filename, "wb") as f:
             shutil.copyfileobj(r.raw, f)
     if extract:
         if os.path.splitext(local_filename)[1] != ".zip":
             logger.error("File not supported. Cannot extract.")
             exit(1)
```

### Comparing `deepfilternet-0.4.0/df/version.py` & `deepfilternet-0.5.0/df/version.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.4.0/df/visualization.py` & `deepfilternet-0.5.0/df/visualization.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,19 +11,22 @@
     figsize=(15, 5),
     colorbar=False,
     colorbar_format=None,
     from_audio=False,
     figure=None,
     return_im=False,
     labels=False,
+    xlabels=False,
+    ylabels=False,
     **kwargs,
 ) -> plt.Figure:
     spec = torch.as_tensor(spec).detach()
-    if labels:
+    if labels or xlabels:
         kwargs.setdefault("xlabel", "Time [s]")
+    if labels or ylabels:
         if kwargs.get("kHz", False):
             kwargs.setdefault("ylabel", "Frequency [kHz]")
         else:
             kwargs.setdefault("ylabel", "Frequency [Hz]")
     if from_audio:
         n_fft = kwargs.setdefault("n_fft", 1024)
         hop = kwargs.setdefault("hop", 256)
```

### Comparing `deepfilternet-0.4.0/pyproject.toml` & `deepfilternet-0.5.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "DeepFilterNet"
-version = "0.4.0"
+version = "0.5.0"
 description = "Noise supression using deep filtering"
 authors = ["Hendrik Schröter"]
 repository = "https://github.com/Rikorose/DeepFilterNet"
 keywords = ["noise reduction", "neural network"]
 classifiers = [
   "Topic :: Multimedia :: Sound/Audio :: Speech",
   "Topic :: Software Development :: Libraries :: Python Modules",
@@ -19,49 +19,52 @@
   { path = "pretrained_models/DeepFilterNet/config.ini" },
   { path = "pretrained_models/DeepFilterNet/checkpoints/*" },
   { path = "pretrained_models/DeepFilterNet2/config.ini" },
   { path = "pretrained_models/DeepFilterNet2/checkpoints/*" },
 ]
 
 [tool.poetry.dependencies]
-deepfilterlib = "0.4.0"
-deepfilterdataloader = { version = "0.4.0", optional = true }
+deepfilterlib = "0.5.0"
+deepfilterdataloader = { version = "0.5.0", optional = true }
 python = ">=3.8,<4.0"
 numpy = ">=1.22,<2.0"
 loguru = ">=0.5"
 appdirs = "^1.4"
 requests = "^2.27"
-soundfile = { version = "^0.10", optional = true }
+packaging = "^23.0"
+sympy = ">=1.6"
+soundfile = { version = ">=0.10,<0.13", optional = true }
 icecream = { version = ">=2,<3", optional = true }
 pystoi = { version = "^0.3", optional = true }
-pesq = { version = "^0.0.3", optional = true }
+pesq = { version = ">=0.0.3,<0.0.5", optional = true }
 scipy = { version = "^1", optional = true }
-onnxruntime = { version = "^1.11", optional = true }
+onnxruntime = { version = "^1.15", optional = true }
 
 [tool.poetry.extras]
 train = ["deepfilterdataloader", "icecream"]
 eval = ["pystoi", "pesq", "scipy"]
 soundfile = ["soundfile"]
 dnsmos-local = ["onnxruntime"]
 
 [tool.poetry.scripts]
 deepFilter = "df.enhance:run"
 deep-filter-py = "df.enhance:run"
 
 [tool.poetry.dev-dependencies]
-poethepoet = "^0.11"
-pre-commit = "^2.17"
+poethepoet = "^0.20"
 
 [tool.poe.tasks]
-install-torch-cuda11 = "python -m pip install torch==1.12.0 torchaudio==0.12.0 --extra-index-url https://download.pytorch.org/whl/cu113/"
-install-torch-cpu = "python -m pip install torch==1.12.0 torchaudio==0.12.0 --extra-index-url https://download.pytorch.org/whl/cpu/"
+install-torch-cuda11 = "python -m pip install torch==1.13.1 torchaudio==0.13.1 --extra-index-url https://download.pytorch.org/whl/cu113/"
+install-torch-cpu = "python -m pip install torch==1.13.1 torchaudio==0.13.1 --extra-index-url https://download.pytorch.org/whl/cpu/"
+install-eval-utils = "python -m pip install -r requirements_eval.txt"
+install-dnsmos-utils = "python -m pip install -r requirements_dnsmos.txt"
 
 [build-system]
-requires = ["poetry>=1.0"]
-build-backend = "poetry.masonry.api"
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 100
 target-version = ["py38", "py39", "py310"]
 include = '\.pyi?$'
 
 [tool.isort]
```

### Comparing `deepfilternet-0.4.0/PKG-INFO` & `deepfilternet-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepfilternet
-Version: 0.4.0
+Version: 0.5.0
 Summary: Noise supression using deep filtering
 Home-page: https://github.com/Rikorose/DeepFilterNet
 License: MIT
 Keywords: noise reduction,neural network
 Author: Hendrik Schröter
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -20,19 +20,21 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Provides-Extra: dnsmos-local
 Provides-Extra: eval
 Provides-Extra: soundfile
 Provides-Extra: train
 Requires-Dist: appdirs (>=1.4,<2.0)
-Requires-Dist: deepfilterdataloader (==0.4.0) ; extra == "train"
-Requires-Dist: deepfilterlib (==0.4.0)
+Requires-Dist: deepfilterdataloader (==0.5.0) ; extra == "train"
+Requires-Dist: deepfilterlib (==0.5.0)
 Requires-Dist: icecream (>=2,<3) ; extra == "train"
 Requires-Dist: loguru (>=0.5)
 Requires-Dist: numpy (>=1.22,<2.0)
-Requires-Dist: onnxruntime (>=1.11,<2.0) ; extra == "dnsmos-local"
-Requires-Dist: pesq (>=0.0.3,<0.0.4) ; extra == "eval"
+Requires-Dist: onnxruntime (>=1.15,<2.0) ; extra == "dnsmos-local"
+Requires-Dist: packaging (>=23.0,<24.0)
+Requires-Dist: pesq (>=0.0.3,<0.0.5) ; extra == "eval"
 Requires-Dist: pystoi (>=0.3,<0.4) ; extra == "eval"
 Requires-Dist: requests (>=2.27,<3.0)
 Requires-Dist: scipy (>=1,<2) ; extra == "eval"
-Requires-Dist: soundfile (>=0.10,<0.11) ; extra == "soundfile"
+Requires-Dist: soundfile (>=0.10,<0.13) ; extra == "soundfile"
+Requires-Dist: sympy (>=1.6)
 Project-URL: Repository, https://github.com/Rikorose/DeepFilterNet
```

