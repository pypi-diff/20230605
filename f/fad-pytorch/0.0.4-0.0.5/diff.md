# Comparing `tmp/fad_pytorch-0.0.4.tar.gz` & `tmp/fad_pytorch-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fad_pytorch-0.0.4.tar", last modified: Fri Jun  2 01:22:54 2023, max compression
+gzip compressed data, was "fad_pytorch-0.0.5.tar", last modified: Mon Jun  5 19:29:14 2023, max compression
```

## Comparing `fad_pytorch-0.0.4.tar` & `fad_pytorch-0.0.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 shawley    (501) staff       (20)        0 2023-06-02 01:22:54.906273 fad_pytorch-0.0.4/
--rw-r--r--   0 shawley    (501) staff       (20)     1072 2023-05-24 22:59:09.000000 fad_pytorch-0.0.4/LICENSE
--rw-r--r--   0 shawley    (501) staff       (20)      111 2023-05-24 22:59:09.000000 fad_pytorch-0.0.4/MANIFEST.in
--rw-r--r--   0 shawley    (501) staff       (20)     3998 2023-06-02 01:22:54.906129 fad_pytorch-0.0.4/PKG-INFO
--rw-r--r--   0 shawley    (501) staff       (20)     3196 2023-06-01 23:44:14.000000 fad_pytorch-0.0.4/README.md
-drwxr-xr-x   0 shawley    (501) staff       (20)        0 2023-06-02 01:22:54.905030 fad_pytorch-0.0.4/fad_pytorch/
--rw-r--r--   0 shawley    (501) staff       (20)       22 2023-06-01 23:44:14.000000 fad_pytorch-0.0.4/fad_pytorch/__init__.py
--rw-r--r--   0 shawley    (501) staff       (20)    31274 2023-06-01 23:44:14.000000 fad_pytorch-0.0.4/fad_pytorch/_modidx.py
--rw-r--r--   0 shawley    (501) staff       (20)      142 2023-05-24 22:59:09.000000 fad_pytorch-0.0.4/fad_pytorch/core.py
--rw-r--r--   0 shawley    (501) staff       (20)    16610 2023-06-02 01:22:48.000000 fad_pytorch-0.0.4/fad_pytorch/fad_embed.py
--rw-r--r--   0 shawley    (501) staff       (20)     4423 2023-05-31 21:21:07.000000 fad_pytorch-0.0.4/fad_pytorch/fad_gen.py
--rw-r--r--   0 shawley    (501) staff       (20)     3773 2023-05-31 21:21:07.000000 fad_pytorch-0.0.4/fad_pytorch/fad_score.py
--rw-r--r--   0 shawley    (501) staff       (20)   123697 2023-05-31 21:21:07.000000 fad_pytorch-0.0.4/fad_pytorch/pann.py
--rw-r--r--   0 shawley    (501) staff       (20)     9559 2023-05-25 06:50:08.000000 fad_pytorch-0.0.4/fad_pytorch/pann_pytorch_utils.py
--rw-r--r--   0 shawley    (501) staff       (20)     8474 2023-05-31 21:21:07.000000 fad_pytorch-0.0.4/fad_pytorch/sqrtm.py
-drwxr-xr-x   0 shawley    (501) staff       (20)        0 2023-06-02 01:22:54.905966 fad_pytorch-0.0.4/fad_pytorch.egg-info/
--rw-r--r--   0 shawley    (501) staff       (20)     3998 2023-06-02 01:22:54.000000 fad_pytorch-0.0.4/fad_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 shawley    (501) staff       (20)      512 2023-06-02 01:22:54.000000 fad_pytorch-0.0.4/fad_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 shawley    (501) staff       (20)        1 2023-06-02 01:22:54.000000 fad_pytorch-0.0.4/fad_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 shawley    (501) staff       (20)      176 2023-06-02 01:22:54.000000 fad_pytorch-0.0.4/fad_pytorch.egg-info/entry_points.txt
--rw-r--r--   0 shawley    (501) staff       (20)        1 2023-05-24 22:59:30.000000 fad_pytorch-0.0.4/fad_pytorch.egg-info/not-zip-safe
--rw-r--r--   0 shawley    (501) staff       (20)       93 2023-06-02 01:22:54.000000 fad_pytorch-0.0.4/fad_pytorch.egg-info/requires.txt
--rw-r--r--   0 shawley    (501) staff       (20)       12 2023-06-02 01:22:54.000000 fad_pytorch-0.0.4/fad_pytorch.egg-info/top_level.txt
--rw-r--r--   0 shawley    (501) staff       (20)     1274 2023-06-02 01:22:48.000000 fad_pytorch-0.0.4/settings.ini
--rw-r--r--   0 shawley    (501) staff       (20)       38 2023-06-02 01:22:54.906311 fad_pytorch-0.0.4/setup.cfg
--rw-r--r--   0 shawley    (501) staff       (20)     2596 2023-05-24 22:59:09.000000 fad_pytorch-0.0.4/setup.py
+drwxr-xr-x   0 shawley    (501) staff       (20)        0 2023-06-05 19:29:14.420126 fad_pytorch-0.0.5/
+-rw-r--r--   0 shawley    (501) staff       (20)     1072 2023-05-24 22:59:09.000000 fad_pytorch-0.0.5/LICENSE
+-rw-r--r--   0 shawley    (501) staff       (20)      111 2023-05-24 22:59:09.000000 fad_pytorch-0.0.5/MANIFEST.in
+-rw-r--r--   0 shawley    (501) staff       (20)     4690 2023-06-05 19:29:14.419998 fad_pytorch-0.0.5/PKG-INFO
+-rw-r--r--   0 shawley    (501) staff       (20)     3888 2023-06-05 19:29:08.000000 fad_pytorch-0.0.5/README.md
+drwxr-xr-x   0 shawley    (501) staff       (20)        0 2023-06-05 19:29:14.418918 fad_pytorch-0.0.5/fad_pytorch/
+-rw-r--r--   0 shawley    (501) staff       (20)       22 2023-06-05 19:29:08.000000 fad_pytorch-0.0.5/fad_pytorch/__init__.py
+-rw-r--r--   0 shawley    (501) staff       (20)    31274 2023-06-01 23:44:14.000000 fad_pytorch-0.0.5/fad_pytorch/_modidx.py
+-rw-r--r--   0 shawley    (501) staff       (20)      142 2023-05-24 22:59:09.000000 fad_pytorch-0.0.5/fad_pytorch/core.py
+-rw-r--r--   0 shawley    (501) staff       (20)    18465 2023-06-05 19:29:08.000000 fad_pytorch-0.0.5/fad_pytorch/fad_embed.py
+-rw-r--r--   0 shawley    (501) staff       (20)     4423 2023-05-31 21:21:07.000000 fad_pytorch-0.0.5/fad_pytorch/fad_gen.py
+-rw-r--r--   0 shawley    (501) staff       (20)     3773 2023-05-31 21:21:07.000000 fad_pytorch-0.0.5/fad_pytorch/fad_score.py
+-rw-r--r--   0 shawley    (501) staff       (20)   123697 2023-05-31 21:21:07.000000 fad_pytorch-0.0.5/fad_pytorch/pann.py
+-rw-r--r--   0 shawley    (501) staff       (20)     9559 2023-05-25 06:50:08.000000 fad_pytorch-0.0.5/fad_pytorch/pann_pytorch_utils.py
+-rw-r--r--   0 shawley    (501) staff       (20)     8474 2023-05-31 21:21:07.000000 fad_pytorch-0.0.5/fad_pytorch/sqrtm.py
+drwxr-xr-x   0 shawley    (501) staff       (20)        0 2023-06-05 19:29:14.419853 fad_pytorch-0.0.5/fad_pytorch.egg-info/
+-rw-r--r--   0 shawley    (501) staff       (20)     4690 2023-06-05 19:29:14.000000 fad_pytorch-0.0.5/fad_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 shawley    (501) staff       (20)      512 2023-06-05 19:29:14.000000 fad_pytorch-0.0.5/fad_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 shawley    (501) staff       (20)        1 2023-06-05 19:29:14.000000 fad_pytorch-0.0.5/fad_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 shawley    (501) staff       (20)      176 2023-06-05 19:29:14.000000 fad_pytorch-0.0.5/fad_pytorch.egg-info/entry_points.txt
+-rw-r--r--   0 shawley    (501) staff       (20)        1 2023-05-24 22:59:30.000000 fad_pytorch-0.0.5/fad_pytorch.egg-info/not-zip-safe
+-rw-r--r--   0 shawley    (501) staff       (20)       93 2023-06-05 19:29:14.000000 fad_pytorch-0.0.5/fad_pytorch.egg-info/requires.txt
+-rw-r--r--   0 shawley    (501) staff       (20)       12 2023-06-05 19:29:14.000000 fad_pytorch-0.0.5/fad_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 shawley    (501) staff       (20)     1274 2023-06-05 19:29:08.000000 fad_pytorch-0.0.5/settings.ini
+-rw-r--r--   0 shawley    (501) staff       (20)       38 2023-06-05 19:29:14.420159 fad_pytorch-0.0.5/setup.cfg
+-rw-r--r--   0 shawley    (501) staff       (20)     2596 2023-05-24 22:59:09.000000 fad_pytorch-0.0.5/setup.py
```

### Comparing `fad_pytorch-0.0.4/LICENSE` & `fad_pytorch-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fad_pytorch-0.0.4/PKG-INFO` & `fad_pytorch-0.0.5/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: fad_pytorch
-Version: 0.0.4
-Summary: Frechet Audio Distance evaluation in PyTorch
-Home-page: https://github.com/drscotthawley/fad_pytorch
-Author: Scott H. Hawley
-Author-email: scott.hawley@belmont.edu
-License: Apache Software License 2.0
-Keywords: nbdev jupyter notebook python
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 fad_pytorch
 ================
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 [Original FAD paper (PDF)](https://arxiv.org/pdf/1812.08466.pdf)
 
@@ -31,44 +9,55 @@
 
 ``` sh
 pip install fad_pytorch
 ```
 
 ## About
 
-(Intended) Features:
+Features:
 
-- runs in parallel on multiple GPUs
-- supports 48kHz sample rates and stereo when possible
-- supports CLAP embeddings, in addition to VGGish and PANN
-- favors ops in PyTorch instead of numpy
-- allows dataset access via WebDataset (over s3://)
+- runs in parallel on multiple processors and multiple GPUs (via
+  `accelerate`)
+- supports multiple embedding methods:
+  - VGGish and PANN, both mono @ 16kHz
+  - OpenL3 and (LAION-)CLAP, stereo @ 48kHz
+- favors ops in PyTorch rather than numpy (or tensorflow)
+- `fad_gen` supports WebDataset (audio data stored in S3 buckets)
 - runs on CPU, CUDA, or MPS
 
 This is designed to be run as 3 command-line scripts in succession. The
 latter 2 (`fad_embed` and `fad_score`) are probably what most people
 will want:
 
-1.  `fad_gen`: produces directories of real & fake audio
-2.  `fad_embed <real_audio_dir> <fake_audio_dir>`: produces directories
-    of *embeddings* of real & fake audio
-3.  `fad_score <real_emb_dir> <fake_emb_dir>`: reads the embeddings &
-    generates FAD score, for real (“$r$”) and fake (“$f$”):
+1.  `fad_gen`: produces directories of real & fake audio. See
+    `fad_gen docs` for calling sequence.
+2.  `fad_embed [options] <real_audio_dir> <fake_audio_dir>`: produces
+    directories of *embeddings* of real & fake audio
+3.  `fad_score [optoions] <real_emb_dir> <fake_emb_dir>`: reads the
+    embeddings & generates FAD score, for real (“$r$”) and fake (“$f$”):
 
 $$ FAD = || \mu_r - \mu_f ||^2 + tr\left(\Sigma_r + \Sigma_f - 2 \sqrt{\Sigma_r \Sigma_f}\right)$$
 
-## FAQ / Troubleshooting
+## Comments / FAQ / Troubleshooting
 
 - “`RuntimeError: CUDA error: invalid device ordinal`”: This happens
   when you have a “bad node” on an AWS cluster. [Haven’t yet figured out
   what causes it or how to fix
   it](https://discuss.huggingface.co/t/solved-accelerate-accelerator-cuda-error-invalid-device-ordinal/21509/1).
   Workaround: Just add the current node to your SLURM `--exclude` list,
   exit and retry. Note: it may take as many as 5 to 7 retries before you
   get a “good node”.
+- “FAD scores obtained from different embedding methods are *wildly*
+  different!” …Yea. It’s not obvious that scores from different
+  embedding methods should be comparable. Rather, compare different
+  groups of audio files using the same embedding method, and/or check
+  that FAD scores go *down* as similarity improves.
+- “FAD score for the same dataset repeated (twice) is not exactly zero!”
+  …Yea. There seems to be an uncertainty of around +/- 0.008. I’d say,
+  don’t quote any numbers past the first decimal point.
 
 ## Contributing
 
 This repo is still fairly “bare bones” and will benefit from more
 documentation and features as time goes on. Note that it is written
 using [nbdev](https://nbdev.fast.ai/), so the things to are:
```

### Comparing `fad_pytorch-0.0.4/fad_pytorch/_modidx.py` & `fad_pytorch-0.0.5/fad_pytorch/_modidx.py`

 * *Files identical despite different names*

### Comparing `fad_pytorch-0.0.4/fad_pytorch/fad_embed.py` & `fad_pytorch-0.0.5/fad_pytorch/fad_embed.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 # %% auto 0
 __all__ = ['OPENL3_VERSION', 'GUDGUD_LICENSE', 'download_file', 'download_if_needed', 'get_ckpt', 'setup_embedder', 'embed',
            'main']
 
 # %% ../nbs/02_fad_embed.ipynb 5
 import os
+import numpy as np
 import argparse
 import laion_clap 
 from laion_clap.training.data import get_audio_features
 from accelerate import Accelerator
 import warnings
 import torch
 
@@ -77,14 +78,15 @@
         ckpt_dl_path=os.path.expanduser("~/checkpoints"),
     ):
     "load the embedder model"
     embedder = None
     
     sample_rate = 16000
     if model_choice == 'clap':
+        print(f"Starting basic CLAP setup")
         clap_fusion, clap_amodel = True, "HTSAT-base"
         #doesn't work:  warnings.filterwarnings('ignore')  # temporarily disable CLAP warnings as they are super annoying. 
         clap_module = laion_clap.CLAP_Module(enable_fusion=clap_fusion, device=device, amodel=clap_amodel).requires_grad_(False).eval()
         clap_ckpt_path = os.getenv('CLAP_CKPT')  # NOTE: CLAP_CKPT env var overrides ckpt_file kwarg
         if clap_ckpt_path is not None:
             #print(f"Loading CLAP from {clap_ckpt_path}")
             clap_module.load_ckpt(ckpt=clap_ckpt_path, verbose=False)
@@ -161,14 +163,15 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 # %% ../nbs/02_fad_embed.ipynb 10
 def embed(args): 
     model_choice, real_path, fake_path, chunk_size, sr, max_batch_size, debug = args.embed_model, args.real_path, args.fake_path, args.chunk_size, args.sr, args.batch_size, args.debug
+    
     sample_rate = sr
     local_rank = int(os.environ.get("LOCAL_RANK", 0))
     world_size = int(os.environ.get("WORLD_SIZE", 1))
     ddps = f"[{local_rank}/{world_size}]"  # string for distributed computing info, e.g. "[1/8]" 
 
     accelerator = Accelerator()
     hprint = HostPrinter(accelerator)  # hprint only prints on head node
@@ -196,105 +199,121 @@
     """
 
     model_choices = [model_choice] if model_choice != 'all' else ['clap','vggish','pann','openl3']
     
     for model_choice in model_choices: # loop over multiple embedders
         hprint(f"\n ** Model_choice = {model_choice}")
         # setup embedder and dataloader
-        embedder, emb_sample_rate = setup_embedder(model_choice, device, accelerator)
+        embedder, emb_sample_rate = setup_embedder(model_choice, device=device, accelerator=accelerator)
         if sr != emb_sample_rate:
             hprint(f"\n*******\nWARNING: sr={sr} != {model_choice}'s emb_sample_rate={emb_sample_rate}. Will resample audio to the latter\n*******\n")
             sr = emb_sample_rate
         hprint(f"{ddps} Embedder '{model_choice}' ready to go!")
 
-        real_dataset = AudioDataset(real_path, augs='Stereo(), PhaseFlipper()', sample_rate=emb_sample_rate, sample_size=chunk_size, return_dict=True, verbose=args.verbose)
-        fake_dataset = AudioDataset(fake_path, augs='Stereo(), PhaseFlipper()', sample_rate=emb_sample_rate, sample_size=chunk_size, return_dict=True, verbose=args.verbose)
+        # we read audio in length args.sample_size, cut it into chunks of args,chunk_size to embed, and skip args.hop_size between chunks
+        # pads with zeros btw
+        real_dataset = AudioDataset(real_path,  sample_rate=emb_sample_rate, sample_size=args.sample_size, return_dict=True, verbose=args.verbose)
+        fake_dataset = AudioDataset(fake_path,  sample_rate=emb_sample_rate, sample_size=args.sample_size, return_dict=True, verbose=args.verbose)
         batch_size = min( len(real_dataset) // world_size , max_batch_size ) 
         hprint(f"\nGiven max_batch_size = {max_batch_size}, len(real_dataset) = {len(real_dataset)}, and world_size = {world_size}, we'll use batch_size = {batch_size}")
         real_dl = DataLoader(real_dataset, batch_size=batch_size, shuffle=False)
         fake_dl = DataLoader(fake_dataset, batch_size=batch_size, shuffle=False)
 
         real_dl, fake_dl, embedder = accelerator.prepare( real_dl, fake_dl, embedder )  # prepare handles distributing things among GPUs
 
         # note that we don't actually care if real & fake files are pulled in the same order; we'll only be comparing the *distributions* of the data.
         with torch.no_grad():
-            for dl, name in zip([real_dl, fake_dl],['real','fake']):
-                newdir_already = False
-                for i, data_dict in enumerate(dl):
-                    audio, filename_batch = data_dict['inputs'], data_dict['filename']
+            for dl, name in zip([real_dl, fake_dl],['real','fake']):  
+                for i, data_dict in enumerate(dl):  # load audio files
+                    audio_sample_batch, filename_batch = data_dict['inputs'], data_dict['filename']
+                    newdir_already = False
                     if not newdir_already: 
                         p = Path( filename_batch[0] )
                         dir_already = True
                         newdir = f"{p.parents[0]}_emb_{model_choice}"
-                        hprint(f"newdir = {newdir}")
+                        hprint(f"creating new directory = {newdir}")
                         makedir(newdir) 
-
-                    #print(f"{ddps} i = {i}/{len(real_dataset)}, filename = {filename_batch[0]}")
-                    audio = audio.to(device)
-
-
-                    if model_choice == 'clap': 
-                        while len(audio.shape) < 3: 
-                            audio = audio.unsqueeze(0) # add batch and/or channel dims 
-                        embeddings = embedder.get_audio_embedding_from_data(audio.mean(dim=1).to(device), use_tensor=True).to(audio.dtype)
-
-                    elif model_choice == "vggish":
-                        audio = torch.mean(audio, dim=1)   # vggish requries we convert to mono
-                        embeddings = []                    # ...whoa, vggish can't even handle batches?  we have to pass 'em through singly?
-                        for bi, waveform in enumerate(audio): 
-                            e = embedder.forward(waveform.cpu().numpy(), emb_sample_rate)
-                            embeddings.append(e) 
-                        embeddings = torch.cat(embeddings, dim=0)
-
-                    elif model_choice == "pann": 
-                        audio = torch.mean(audio, dim=1)  # mono only.  todo:  keepdim=True ?
-                        out = embedder.forward(audio, None)
-                        embeddings = out['embedding'].data
-                        
-                    elif model_choice == "openl3" and OPENL3_VERSION == "hugo":
-                        ##audio = torch.mean(audio, dim=1)  # mono only.
-                        embeddings = []
-                        for bi, waveform in enumerate( audio.cpu().numpy() ): # no batch processing, expects numpy 
-                            e = torchopenl3.embed(model=embedder, 
-                                audio=waveform, # shape sould be (channels, samples)
-                                sample_rate=emb_sample_rate, # sample rate of input file
-                                hop_size=1,  device=device)
-                            if debug: hprint(f"bi = {bi}, waveform.shape = {waveform.shape},  e.shape = {e.shape}") 
-                            embeddings.append(torch.tensor(e))
-                        embeddings = torch.cat(embeddings, dim=0)
+                        newdir_already = True
+                    # cut audio samples into chunks spaced out by hops, and loop over them
+                    hop_samples = int(args.hop_size * args.sample_size)
+                    hop_starts = np.arange(0, args.sample_size, hop_samples)
+                    if args.max_hops <= 0:  
+                        hop_starts = hop_starts[:min(len(hop_starts), args.max_hops)]
+                    if args.sample_size - hop_starts[-1] < args.hop_size: # judgement call: let's not zero-pad on the very end, rather just don't do the last hop
+                        hop_starts = hop_starts[:-1]
+                    for h_ind, hop_loc in enumerate(hop_starts):               # proceed through audio file batch via chunks, skipping by hop_samples each time
+                        chunk = audio_sample_batch[:,:,hop_loc:hop_loc+hop_samples]
+                        audio = chunk 
                         
-                    elif model_choice == "openl3" and OPENL3_VERSION == "turian":
-                        # Note: turian's can/will do multiple time-stamped embeddings if the sample_size is long enough! 
-                        
-                        audio = rearrange(audio, 'b c s -> b s c')  # make channels_first
-                        embeddings, timestamps = torchopenl3.get_audio_embedding(audio, emb_sample_rate, model=embedder)
-                        embeddings = torch.squeeze(embeddings, 1)  # get rid of any spurious dimensions of 1 in middle position 
-                        
-                    else:
-                        raise ValueError(f"Unknown model_choice = {model_choice}")
+                        #print(f"{ddps} i = {i}/{len(real_dataset)}, filename = {filename_batch[0]}")
+                        audio = audio.to(device)
+
 
-                    hprint(f"embeddings.shape = {embeddings.shape}")
-                    # TODO: for now we'll just dump each batch on each proc to its own file; this could be improved
-                    outfilename = f"{newdir}/emb_p{local_rank}_b{i}.pt"
-                    hprint(f"{ddps} Saving embeddings to {outfilename}")
-                    torch.save(embeddings.cpu().detach(), outfilename)
+                        if model_choice == 'clap': 
+                            while len(audio.shape) < 3: 
+                                audio = audio.unsqueeze(0) # add batch and/or channel dims 
+                            embeddings = accelerator.unwrap_model(embedder).get_audio_embedding_from_data(audio.mean(dim=1).to(device), use_tensor=True).to(audio.dtype)
+
+                        elif model_choice == "vggish":
+                            audio = torch.mean(audio, dim=1)   # vggish requries we convert to mono
+                            embeddings = []                    # ...whoa, vggish can't even handle batches?  we have to pass 'em through singly?
+                            for bi, waveform in enumerate(audio): 
+                                e =  accelerator.unwrap_model(embedder).forward(waveform.cpu().numpy(), emb_sample_rate)
+                                embeddings.append(e) 
+                            embeddings = torch.cat(embeddings, dim=0)
+
+                        elif model_choice == "pann": 
+                            audio = torch.mean(audio, dim=1)  # mono only.  todo:  keepdim=True ?
+                            out = embedder.forward(audio, None)
+                            embeddings = out['embedding'].data
+
+                        elif model_choice == "openl3" and OPENL3_VERSION == "hugo":
+                            ##audio = torch.mean(audio, dim=1)  # mono only.
+                            embeddings = []
+                            for bi, waveform in enumerate( audio.cpu().numpy() ): # no batch processing, expects numpy 
+                                e = torchopenl3.embed(model=embedder, 
+                                    audio=waveform, # shape sould be (channels, samples)
+                                    sample_rate=emb_sample_rate, # sample rate of input file
+                                    hop_size=1,  device=device)
+                                if debug: hprint(f"bi = {bi}, waveform.shape = {waveform.shape},  e.shape = {e.shape}") 
+                                embeddings.append(torch.tensor(e))
+                            embeddings = torch.cat(embeddings, dim=0)
+
+                        elif model_choice == "openl3" and OPENL3_VERSION == "turian":
+                            # Note: turian's can/will do multiple time-stamped embeddings if the sample_size is long enough. but our chunks/hops precludes this
+
+                            #not needed, turns out: audio = renot needed, turns out: arrange(audio, 'b c s -> b s c')       # this torchopen3 expects channels-first ordering
+                            embeddings, timestamps = torchopenl3.get_audio_embedding(audio, emb_sample_rate, model=embedder)
+                            embeddings = torch.squeeze(embeddings, 1)        # get rid of any spurious dimensions of 1 in middle position 
+
+                        else:
+                            raise ValueError(f"Unknown model_choice = {model_choice}")
+
+                        hprint(f"embeddings.shape = {embeddings.shape}")
+                        # TODO: for now we'll just dump each batch on each proc to its own file; this could be improved
+                        outfilename = f"{newdir}/emb_p{local_rank}_b{i}_h{h_ind}.pt"
+                        hprint(f"{ddps} Saving embeddings to {outfilename}")
+                        torch.save(embeddings.cpu().detach(), outfilename)
                     
         del embedder
         torch.cuda.empty_cache()
         # end loop over various embedders
     return        
 
 # %% ../nbs/02_fad_embed.ipynb 11
 def main(): 
     parser = argparse.ArgumentParser(formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     parser.add_argument('embed_model', help='choice of embedding model(s): clap | vggish | pann | openl3 | all ', default='clap')
     parser.add_argument('real_path', help='Path of files of real audio', default='real/')
     parser.add_argument('fake_path', help='Path of files of fake audio', default='fake/')
-    parser.add_argument('--chunk_size', type=int, default=24000, help='Length of chunks (in audio samples) to embed')
     parser.add_argument('--batch_size', type=int, default=64, help='MAXIMUM Batch size for computing embeddings (may go smaller)')
+    parser.add_argument('--sample_size', type=int, default=2**18, help='Number of audio samples to read from each audio file')
+    parser.add_argument('--chunk_size', type=int, default=24000, help='Length of chunks (in audio samples) to embed')
+    parser.add_argument('--hop_size', type=float, default=0.100, help='(approximate) time difference (in seconds) between each chunk')
+    parser.add_argument('--max_hops', type=int, default=-1, help="Don't exceed this many hops/chunks/embeddings per audio file. <= 0 disables this.")
     parser.add_argument('--sr', type=int, default=48000, help='sample rate (will resample inputs at this rate)')
     parser.add_argument('--verbose', action='store_true',  help='Show notices of resampling when reading files')
     parser.add_argument('--debug', action='store_true',  help='Extra messages for debugging this program')
 
     args = parser.parse_args()
     embed(args)
```

### Comparing `fad_pytorch-0.0.4/fad_pytorch/fad_gen.py` & `fad_pytorch-0.0.5/fad_pytorch/fad_gen.py`

 * *Files identical despite different names*

### Comparing `fad_pytorch-0.0.4/fad_pytorch/fad_score.py` & `fad_pytorch-0.0.5/fad_pytorch/fad_score.py`

 * *Files identical despite different names*

### Comparing `fad_pytorch-0.0.4/fad_pytorch/pann.py` & `fad_pytorch-0.0.5/fad_pytorch/pann.py`

 * *Files identical despite different names*

### Comparing `fad_pytorch-0.0.4/fad_pytorch/pann_pytorch_utils.py` & `fad_pytorch-0.0.5/fad_pytorch/pann_pytorch_utils.py`

 * *Files identical despite different names*

### Comparing `fad_pytorch-0.0.4/fad_pytorch/sqrtm.py` & `fad_pytorch-0.0.5/fad_pytorch/sqrtm.py`

 * *Files identical despite different names*

### Comparing `fad_pytorch-0.0.4/fad_pytorch.egg-info/PKG-INFO` & `fad_pytorch-0.0.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: fad-pytorch
-Version: 0.0.4
+Name: fad_pytorch
+Version: 0.0.5
 Summary: Frechet Audio Distance evaluation in PyTorch
 Home-page: https://github.com/drscotthawley/fad_pytorch
 Author: Scott H. Hawley
 Author-email: scott.hawley@belmont.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
@@ -31,44 +31,55 @@
 
 ``` sh
 pip install fad_pytorch
 ```
 
 ## About
 
-(Intended) Features:
+Features:
 
-- runs in parallel on multiple GPUs
-- supports 48kHz sample rates and stereo when possible
-- supports CLAP embeddings, in addition to VGGish and PANN
-- favors ops in PyTorch instead of numpy
-- allows dataset access via WebDataset (over s3://)
+- runs in parallel on multiple processors and multiple GPUs (via
+  `accelerate`)
+- supports multiple embedding methods:
+  - VGGish and PANN, both mono @ 16kHz
+  - OpenL3 and (LAION-)CLAP, stereo @ 48kHz
+- favors ops in PyTorch rather than numpy (or tensorflow)
+- `fad_gen` supports WebDataset (audio data stored in S3 buckets)
 - runs on CPU, CUDA, or MPS
 
 This is designed to be run as 3 command-line scripts in succession. The
 latter 2 (`fad_embed` and `fad_score`) are probably what most people
 will want:
 
-1.  `fad_gen`: produces directories of real & fake audio
-2.  `fad_embed <real_audio_dir> <fake_audio_dir>`: produces directories
-    of *embeddings* of real & fake audio
-3.  `fad_score <real_emb_dir> <fake_emb_dir>`: reads the embeddings &
-    generates FAD score, for real (“$r$”) and fake (“$f$”):
+1.  `fad_gen`: produces directories of real & fake audio. See
+    `fad_gen docs` for calling sequence.
+2.  `fad_embed [options] <real_audio_dir> <fake_audio_dir>`: produces
+    directories of *embeddings* of real & fake audio
+3.  `fad_score [optoions] <real_emb_dir> <fake_emb_dir>`: reads the
+    embeddings & generates FAD score, for real (“$r$”) and fake (“$f$”):
 
 $$ FAD = || \mu_r - \mu_f ||^2 + tr\left(\Sigma_r + \Sigma_f - 2 \sqrt{\Sigma_r \Sigma_f}\right)$$
 
-## FAQ / Troubleshooting
+## Comments / FAQ / Troubleshooting
 
 - “`RuntimeError: CUDA error: invalid device ordinal`”: This happens
   when you have a “bad node” on an AWS cluster. [Haven’t yet figured out
   what causes it or how to fix
   it](https://discuss.huggingface.co/t/solved-accelerate-accelerator-cuda-error-invalid-device-ordinal/21509/1).
   Workaround: Just add the current node to your SLURM `--exclude` list,
   exit and retry. Note: it may take as many as 5 to 7 retries before you
   get a “good node”.
+- “FAD scores obtained from different embedding methods are *wildly*
+  different!” …Yea. It’s not obvious that scores from different
+  embedding methods should be comparable. Rather, compare different
+  groups of audio files using the same embedding method, and/or check
+  that FAD scores go *down* as similarity improves.
+- “FAD score for the same dataset repeated (twice) is not exactly zero!”
+  …Yea. There seems to be an uncertainty of around +/- 0.008. I’d say,
+  don’t quote any numbers past the first decimal point.
 
 ## Contributing
 
 This repo is still fairly “bare bones” and will benefit from more
 documentation and features as time goes on. Note that it is written
 using [nbdev](https://nbdev.fast.ai/), so the things to are:
```

### Comparing `fad_pytorch-0.0.4/fad_pytorch.egg-info/SOURCES.txt` & `fad_pytorch-0.0.5/fad_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fad_pytorch-0.0.4/settings.ini` & `fad_pytorch-0.0.5/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = fad_pytorch
 lib_name = %(repo)s
-version = 0.0.4
+version = 0.0.5
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = fad_pytorch
```

### Comparing `fad_pytorch-0.0.4/setup.py` & `fad_pytorch-0.0.5/setup.py`

 * *Files identical despite different names*

