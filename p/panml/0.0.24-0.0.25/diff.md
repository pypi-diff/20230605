# Comparing `tmp/panml-0.0.24.tar.gz` & `tmp/panml-0.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panml-0.0.24.tar", last modified: Sun Jun  4 01:50:25 2023, max compression
+gzip compressed data, was "panml-0.0.25.tar", last modified: Mon Jun  5 12:57:49 2023, max compression
```

## Comparing `panml-0.0.24.tar` & `panml-0.0.25.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-04 01:50:25.647239 panml-0.0.24/
--rw-r--r--   0 williamzheng   (501) staff       (20)     1063 2023-05-11 06:11:04.000000 panml-0.0.24/LICENSE
--rw-r--r--   0 williamzheng   (501) staff       (20)    14672 2023-06-04 01:50:25.647704 panml-0.0.24/PKG-INFO
--rw-r--r--   0 williamzheng   (501) staff       (20)    13493 2023-06-04 01:49:06.000000 panml-0.0.24/README.md
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-04 01:50:25.634129 panml-0.0.24/panml/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-19 12:08:24.000000 panml-0.0.24/panml/__init__.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     3617 2023-06-01 11:12:21.000000 panml-0.0.24/panml/constants.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-04 01:50:25.639180 panml-0.0.24/panml/core/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-21 05:11:31.000000 panml-0.0.24/panml/core/__init__.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-04 01:50:25.640376 panml-0.0.24/panml/core/clustering/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-21 05:11:31.000000 panml-0.0.24/panml/core/clustering/__init__.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     9033 2023-05-24 12:19:14.000000 panml-0.0.24/panml/core/clustering/faiss.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-04 01:50:25.643984 panml-0.0.24/panml/core/llm/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-21 05:11:31.000000 panml-0.0.24/panml/core/llm/__init__.py
--rw-r--r--   0 williamzheng   (501) staff       (20)    20353 2023-06-01 22:37:04.000000 panml-0.0.24/panml/core/llm/huggingface.py
--rw-r--r--   0 williamzheng   (501) staff       (20)    13741 2023-06-01 22:37:04.000000 panml-0.0.24/panml/core/llm/openai.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     3085 2023-05-28 12:46:27.000000 panml-0.0.24/panml/models.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     2608 2023-05-28 12:46:27.000000 panml-0.0.24/panml/search.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-04 01:50:25.638504 panml-0.0.24/panml.egg-info/
--rw-r--r--   0 williamzheng   (501) staff       (20)    14672 2023-06-04 01:50:25.000000 panml-0.0.24/panml.egg-info/PKG-INFO
--rw-r--r--   0 williamzheng   (501) staff       (20)      468 2023-06-04 01:50:25.000000 panml-0.0.24/panml.egg-info/SOURCES.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)        1 2023-06-04 01:50:25.000000 panml-0.0.24/panml.egg-info/dependency_links.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)      215 2023-06-04 01:50:25.000000 panml-0.0.24/panml.egg-info/requires.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)        6 2023-06-04 01:50:25.000000 panml-0.0.24/panml.egg-info/top_level.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)       79 2023-06-04 01:50:25.649281 panml-0.0.24/setup.cfg
--rw-r--r--   0 williamzheng   (501) staff       (20)     2384 2023-06-04 01:49:06.000000 panml-0.0.24/setup.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-04 01:50:25.646038 panml-0.0.24/test/
--rw-r--r--   0 williamzheng   (501) staff       (20)     4383 2023-05-25 13:23:02.000000 panml-0.0.24/test/test_ModelPack.py
--rw-r--r--   0 williamzheng   (501) staff       (20)    11162 2023-05-22 09:48:53.000000 panml-0.0.24/test/test_VectorEngine.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-05 12:57:49.205567 panml-0.0.25/
+-rw-r--r--   0 williamzheng   (501) staff       (20)     1063 2023-05-11 06:11:04.000000 panml-0.0.25/LICENSE
+-rw-r--r--   0 williamzheng   (501) staff       (20)    14677 2023-06-05 12:57:49.205810 panml-0.0.25/PKG-INFO
+-rw-r--r--   0 williamzheng   (501) staff       (20)    13498 2023-06-05 12:56:17.000000 panml-0.0.25/README.md
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-05 12:57:49.197886 panml-0.0.25/panml/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-19 12:08:24.000000 panml-0.0.25/panml/__init__.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     4497 2023-06-05 12:56:17.000000 panml-0.0.25/panml/constants.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-05 12:57:49.200363 panml-0.0.25/panml/core/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-21 05:11:31.000000 panml-0.0.25/panml/core/__init__.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-05 12:57:49.201298 panml-0.0.25/panml/core/clustering/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-21 05:11:31.000000 panml-0.0.25/panml/core/clustering/__init__.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     9033 2023-05-24 12:19:14.000000 panml-0.0.25/panml/core/clustering/faiss.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-05 12:57:49.203129 panml-0.0.25/panml/core/llm/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-21 05:11:31.000000 panml-0.0.25/panml/core/llm/__init__.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)    23368 2023-06-05 12:56:17.000000 panml-0.0.25/panml/core/llm/huggingface.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)    13741 2023-06-01 22:37:04.000000 panml-0.0.25/panml/core/llm/openai.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     3090 2023-06-05 12:56:17.000000 panml-0.0.25/panml/models.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     2608 2023-05-28 12:46:27.000000 panml-0.0.25/panml/search.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-05 12:57:49.199873 panml-0.0.25/panml.egg-info/
+-rw-r--r--   0 williamzheng   (501) staff       (20)    14677 2023-06-05 12:57:49.000000 panml-0.0.25/panml.egg-info/PKG-INFO
+-rw-r--r--   0 williamzheng   (501) staff       (20)      468 2023-06-05 12:57:49.000000 panml-0.0.25/panml.egg-info/SOURCES.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)        1 2023-06-05 12:57:49.000000 panml-0.0.25/panml.egg-info/dependency_links.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)      227 2023-06-05 12:57:49.000000 panml-0.0.25/panml.egg-info/requires.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)        6 2023-06-05 12:57:49.000000 panml-0.0.25/panml.egg-info/top_level.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)       79 2023-06-05 12:57:49.206751 panml-0.0.25/setup.cfg
+-rw-r--r--   0 williamzheng   (501) staff       (20)     2407 2023-06-05 12:56:17.000000 panml-0.0.25/setup.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-05 12:57:49.204679 panml-0.0.25/test/
+-rw-r--r--   0 williamzheng   (501) staff       (20)     4383 2023-05-25 13:23:02.000000 panml-0.0.25/test/test_ModelPack.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)    11162 2023-05-22 09:48:53.000000 panml-0.0.25/test/test_VectorEngine.py
```

### Comparing `panml-0.0.24/LICENSE` & `panml-0.0.25/LICENSE`

 * *Files identical despite different names*

### Comparing `panml-0.0.24/PKG-INFO` & `panml-0.0.25/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panml
-Version: 0.0.24
+Version: 0.0.25
 Summary: PanML is a high level generative AI/ML development library designed for ease of use and fast experimentation.
 Home-page: https://github.com/Pan-ML/panml
 Author: PanML team
 Author-email: teampanml@gmail.com
 License: MIT
 Keywords: generative AI,generative model,machine learning,large language model,LLM,prompt engineering,fine tuning,prompt tuning,retrieval augmentation,AI safety,AI alignment
 Platform: UNKNOWN
@@ -25,23 +25,23 @@
 License-File: LICENSE
 
 ## PanML: A high level generative AI/ML development and analysis library
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) 
 [![](https://dcbadge.vercel.app/api/server/cCsaqv9KFf?compact=true&style=flat)](https://discord.gg/cCsaqv9KFf)
 
-A library with simple to use abstractions when working with LLMs inspired by the sckit-learn style API. <br>
+A library with simple-to-use abstractions when working with LLMs, inspired by the scikit-learn style API. <br>
 🔍 Easily explore and experiment with commercial and open source LLMs, including ones that can be run on your local machine. <br>
 ⚡ Easily integrate language models of different sizes, including smaller, less compute heavy but still very useful LLMs in NLP-based Data Science contexts. <br>
 🚀 Support the development of LLM workflows with off-the-shelf or custom-built generative models. <br><br>
 Please note this is a work in progress, and it's open for collabration and contribution.
 
 ### What this library covers
 - [Inference and analysis of LLM](https://github.com/Pan-ML/panml/wiki/5.-Generative-model-analysis)
-- [Prompt chain engineering a LLM](https://github.com/Pan-ML/panml/wiki/2.-Prompt-chain-engineering)
+- [Prompt chain engineering with LLM](https://github.com/Pan-ML/panml/wiki/2.-Prompt-chain-engineering)
 - [Fine tuning of LLM](https://github.com/Pan-ML/panml/wiki/3.-Fine-tuning-your-LLM)
 - [Document question answering using LLM](https://github.com/Pan-ML/panml/wiki/7.-Retrieve-similar-documents-using-vector-search)
 - [Variable integrated code generation using LLM](https://github.com/Pan-ML/panml/wiki/4.-Prompted-code-generation)
 
 ### Current supported foundation models
 - [HuggingFace Hub](https://huggingface.co) - open source LLMs from Google, EleutherAI, Cerebras, StabilityAI, H2O, Salesforce, and others
 - [OpenAI](https://openai.com) - text-davinci-002/003, GPT3/3.5
```

### Comparing `panml-0.0.24/README.md` & `panml-0.0.25/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ## PanML: A high level generative AI/ML development and analysis library
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) 
 [![](https://dcbadge.vercel.app/api/server/cCsaqv9KFf?compact=true&style=flat)](https://discord.gg/cCsaqv9KFf)
 
-A library with simple to use abstractions when working with LLMs inspired by the sckit-learn style API. <br>
+A library with simple-to-use abstractions when working with LLMs, inspired by the scikit-learn style API. <br>
 🔍 Easily explore and experiment with commercial and open source LLMs, including ones that can be run on your local machine. <br>
 ⚡ Easily integrate language models of different sizes, including smaller, less compute heavy but still very useful LLMs in NLP-based Data Science contexts. <br>
 🚀 Support the development of LLM workflows with off-the-shelf or custom-built generative models. <br><br>
 Please note this is a work in progress, and it's open for collabration and contribution.
 
 ### What this library covers
 - [Inference and analysis of LLM](https://github.com/Pan-ML/panml/wiki/5.-Generative-model-analysis)
-- [Prompt chain engineering a LLM](https://github.com/Pan-ML/panml/wiki/2.-Prompt-chain-engineering)
+- [Prompt chain engineering with LLM](https://github.com/Pan-ML/panml/wiki/2.-Prompt-chain-engineering)
 - [Fine tuning of LLM](https://github.com/Pan-ML/panml/wiki/3.-Fine-tuning-your-LLM)
 - [Document question answering using LLM](https://github.com/Pan-ML/panml/wiki/7.-Retrieve-similar-documents-using-vector-search)
 - [Variable integrated code generation using LLM](https://github.com/Pan-ML/panml/wiki/4.-Prompted-code-generation)
 
 ### Current supported foundation models
 - [HuggingFace Hub](https://huggingface.co) - open source LLMs from Google, EleutherAI, Cerebras, StabilityAI, H2O, Salesforce, and others
 - [OpenAI](https://openai.com) - text-davinci-002/003, GPT3/3.5
```

### Comparing `panml-0.0.24/panml/constants.py` & `panml-0.0.25/panml/constants.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,15 +17,18 @@
         'cerebras/Cerebras-GPT-111M',
         'cerebras/Cerebras-GPT-256M',
         'cerebras/Cerebras-GPT-590M',
         'cerebras/Cerebras-GPT-1.3B',
         'cerebras/Cerebras-GPT-2.7B',
         'cerebras/Cerebras-GPT-6.7B',
         'cerebras/Cerebras-GPT-13B',
+        'EleutherAI/gpt-neo-125m',
+        'EleutherAI/gpt-neo-1.3B',
         'EleutherAI/gpt-neo-2.7B',
+        'EleutherAI/gpt-neox-20b',
         'EleutherAI/gpt-j-6B',
         'togethercomputer/GPT-JT-6B-v1',
         'togethercomputer/GPT-NeoXT-Chat-Base-20B',
         'StabilityAI/stablelm-base-alpha-3b',
         'StabilityAI/stablelm-base-alpha-7b',
         'StabilityAI/stablelm-tuned-alpha-3b',
         'StabilityAI/stablelm-tuned-alpha-7b',
@@ -41,23 +44,52 @@
         'togethercomputer/RedPajama-INCITE-Base-3B-v1',
         'togethercomputer/RedPajama-INCITE-Instruct-3B-v1',
         'togethercomputer/RedPajama-INCITE-Chat-3B-v1',
         'tiiuae/falcon-7b',
         'tiiuae/falcon-7b-instruct',
         'tiiuae/falcon-40b',
         'tiiuae/falcon-40b-instruct',
+        'bigscience/bloomz-560m',
+        'bigscience/bloomz-1b1',
+        'bigscience/bloomz-1b7',
+        'bigscience/bloomz-3b',
+        'bigscience/bloomz-7b1',
+        'bigscience/bloomz',
     ],
     'openai': [
         'text-davinci-002', 
         'text-davinci-003',
         'gpt-3.5-turbo',
         'gpt-3.5-turbo-0301',
     ],
 }
 
+SUPPORTED_LLMS_PEFT_LORA = [
+    'gpt2',
+    'gpt2-medium',
+    'gpt2-xl',
+    'google/flan-t5-base',
+    'google/flan-t5-small',
+    'google/flan-t5-large',
+    'google/flan-t5-xl',
+    'google/flan-t5-xxl',
+    'EleutherAI/gpt-neo-125m',
+    'EleutherAI/gpt-neo-1.3B',
+    'EleutherAI/gpt-neo-2.7B',
+    'EleutherAI/gpt-neo-2.7B',
+    'EleutherAI/gpt-j-6B',
+    'togethercomputer/GPT-NeoXT-Chat-Base-20B',
+    'bigscience/bloomz-560m',
+    'bigscience/bloomz-1b1',
+    'bigscience/bloomz-1b7',
+    'bigscience/bloomz-3b',
+    'bigscience/bloomz-7b1',
+    'bigscience/bloomz',
+]
+
 # Supported OpenAI models for code completion
 SUPPORTED_OAI_CODE_MODELS = [
     'text-davinci-002', 
     'text-davinci-002',
 ]
 
 # Supported OpenAI models for completion
```

### Comparing `panml-0.0.24/panml/core/clustering/faiss.py` & `panml-0.0.25/panml/core/clustering/faiss.py`

 * *Files identical despite different names*

### Comparing `panml-0.0.24/panml/core/llm/huggingface.py` & `panml-0.0.25/panml/core/llm/huggingface.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from __future__ import annotations
 import pandas as pd
 import torch
 from typing import Union, Callable
 from transformers import AutoModelForCausalLM, AutoModelForSeq2SeqLM, AutoModelForMaskedLM, AutoTokenizer
 from transformers import TrainingArguments, Trainer, Seq2SeqTrainingArguments, Seq2SeqTrainer, DataCollatorForLanguageModeling, DataCollatorForSeq2Seq
 from datasets import Dataset
+from peft import get_peft_model, PeftModel, PeftConfig, LoraConfig, TaskType
+from panml.constants import SUPPORTED_LLMS_PEFT_LORA
 
 # HuggingFace model class
 class HuggingFaceModelPack:
     '''
     HuggingFace Hub model pack class
     '''
     # Initialize class variables
@@ -16,15 +18,36 @@
         self.model_name = model
         self.padding_length = padding_length
         self.input_block_size = input_block_size
         self.tokenizer_batch = tokenizer_batch
         self.prediction_history = []
         self.evaluation_result = None
         self.device = 'cpu'
+        self.supported_models_peft_lora = SUPPORTED_LLMS_PEFT_LORA
+        self.peft_config = None
+        self.train_default_args = ['title', 'num_train_epochs', 'optimizer', 'mlm', 
+                                   'per_device_train_batch_size', 'per_device_eval_batch_size',
+                                   'warmup_steps', 'weight_decay', 'logging_steps', 
+                                   'output_dir', 'logging_dir', 'save_model']
         
+        # Get PEFT LoRA configuration from model args
+        peft_lora_args, load_peft_lora = {}, None
+        if 'peft_lora' in model_args:
+            peft_lora_args = model_args.pop('peft_lora')
+            if 'load' in peft_lora_args:
+                load_peft_lora = peft_lora_args.pop('load')
+            else:
+                if not isinstance(load_peft_lora, bool):
+                    raise TypeError('Input model args, peft_lora, load needs to be of type: boolean')
+                
+            if 'task_type' in peft_lora_args:
+                _ = peft_lora_args.pop('task_type') # remove task_type from input args to avoid duplication
+
+        # Get CPU/GPU configuration from model args
+        set_gpu = False
         if 'gpu' in model_args:
             if not isinstance(model_args['gpu'], bool):
                 raise TypeError('Input model args, gpu needs to be of type: boolean')
             set_gpu = model_args.pop('gpu')
             if set_gpu: # set model processing on GPU else defaults on CPU
                 if torch.cuda.is_available(): # for CUDA compatible chips
                     self.device = 'cuda'
@@ -32,39 +55,69 @@
                     try:
                         if torch.backends.mps.is_available():
                             self.device = 'mps'
                         else:
                             print('CUDA (GPU support) is not available')
                     except:
                         print('CUDA (GPU support) is not available')
-
         print(f'Model processing is set on {self.device.upper()}')
-        self.train_default_args = ['title', 'num_train_epochs', 'optimizer', 'mlm', 
-                                   'per_device_train_batch_size', 'per_device_eval_batch_size',
-                                   'warmup_steps', 'weight_decay', 'logging_steps', 
-                                   'output_dir', 'logging_dir', 'save_model']
 
+        # Set model
         if source == 'huggingface':
             if 'flan' in self.model_name:
                 self.model_hf = AutoModelForSeq2SeqLM.from_pretrained(self.model_name, **model_args)
             elif 'bert' in self.model_name:
                 self.model_hf = AutoModelForMaskedLM.from_pretrained(self.model_name, **model_args)
             else:
                 self.model_hf = AutoModelForCausalLM.from_pretrained(self.model_name, **model_args)
         elif source == 'local':
-            if 'flan' in self.model_name:
-                self.model_hf = AutoModelForSeq2SeqLM.from_pretrained(self.model_name, **model_args, local_files_only=True)
-            elif 'bert' in self.model_name:
-                self.model_hf = AutoModelForMaskedLM.from_pretrained(self.model_name, **model_args, local_files_only=True)
+            if load_peft_lora:
+                # Set LoRA trained model
+                self.peft_config = PeftConfig.from_pretrained(self.model_name)
+                if 'flan' in self.model_name:
+                    self.model_hf = AutoModelForSeq2SeqLM.from_pretrained(self.peft_config.base_model_name_or_path, **model_args, local_files_only=True)
+                elif 'bert' in self.model_name:
+                    self.model_hf = AutoModelForMaskedLM.from_pretrained(self.peft_config.base_model_name_or_path, **model_args, local_files_only=True)
+                else:
+                    self.model_hf = AutoModelForCausalLM.from_pretrained(self.peft_config.base_model_name_or_path, **model_args, local_files_only=True)
+                self.model_hf = PeftModel.from_pretrained(self.model_hf, self.peft_config)
             else:
-                self.model_hf = AutoModelForCausalLM.from_pretrained(self.model_name, **model_args, local_files_only=True)
-        if self.model_hf.config.tokenizer_class:
-            self.tokenizer = AutoTokenizer.from_pretrained(self.model_hf.config.tokenizer_class.lower().replace('tokenizer', ''), mirror='https://huggingface.co')
+                # Set non-LoRA trained model
+                if 'flan' in self.model_name:
+                    self.model_hf = AutoModelForSeq2SeqLM.from_pretrained(self.model_name, **model_args, local_files_only=True)
+                elif 'bert' in self.model_name:
+                    self.model_hf = AutoModelForMaskedLM.from_pretrained(self.model_name, **model_args, local_files_only=True)
+                else:
+                    self.model_hf = AutoModelForCausalLM.from_pretrained(self.model_name, **model_args, local_files_only=True)
+        
+        # Set tokenizer
+        if load_peft_lora:
+            # Set LoRA trained model's tokenizer
+            self.tokenizer = AutoTokenizer.from_pretrained(self.peft_config.base_model_name_or_path)
         else:
-            self.tokenizer = AutoTokenizer.from_pretrained(self.model_name, mirror='https://huggingface.co')
+            # Set non-LoRA trained model's tokenizer
+            if self.model_hf.config.tokenizer_class:
+                self.tokenizer = AutoTokenizer.from_pretrained(self.model_hf.config.tokenizer_class.lower().replace('tokenizer', ''), mirror='https://huggingface.co')
+            else:
+                self.tokenizer = AutoTokenizer.from_pretrained(self.model_name, mirror='https://huggingface.co')
+
+        # Set LoRA for training
+        if peft_lora_args is not {} and load_peft_lora is False:
+            if self.model_name in self.supported_models_peft_lora:
+                if 'flan' in self.model_name:
+                    self.peft_config = LoraConfig(task_type=TaskType['SEQ_2_SEQ_LM'], **peft_lora_args)
+                else:
+                    self.peft_config = LoraConfig(task_type=TaskType['CAUSAL_LM'], **peft_lora_args)
+                
+                self.model_hf = get_peft_model(self.model_hf, self.peft_config)
+                
+                print('PEFT LoRA configuration applied:')
+                self.model_hf.print_trainable_parameters()
+            else:
+                print('PEFT LoRA configuration not set. Current supported models for LoRA are: ' + ' '.join([f"{m}" for m in self.supported_models_peft_lora]))
 
         # Set model on GPU if available and specified
         self.model_hf.to(torch.device(self.device))
         
     # Set initial prompt
     def _init_prompt(self) -> list[dict[str, Union[str, Callable]]]:
         return [{'prepend': '', 'append': '', 'transform': None}]
```

### Comparing `panml-0.0.24/panml/core/llm/openai.py` & `panml-0.0.25/panml/core/llm/openai.py`

 * *Files identical despite different names*

### Comparing `panml-0.0.24/panml/models.py` & `panml-0.0.25/panml/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 # Entry model pack class           
 class ModelPack:
     '''
     Main model pack class
     '''
     def __init__(self, model: str, tokenizer: AutoTokenizer=None, input_block_size: int=20, padding_length: int=100, 
-                 tokenizer_batch: bool=False, source: str='huggingface', api_key: str=None, model_args={}) -> None:
+                 tokenizer_batch: bool=False, source: str='huggingface', api_key: str=None, model_args: dict={}) -> None:
         self.padding_length = padding_length
         self.tokenizer = tokenizer
         self.model = model
         self.input_block_size = input_block_size
         self.tokenizer_batch = tokenizer_batch
         self.source = source
         self.api_key = api_key
@@ -41,15 +41,15 @@
         # Locally trained model call of HuggingFace Hub model
         elif self.source == 'local':
             self.instance = HuggingFaceModelPack(self.model, self.input_block_size, self.padding_length, self.tokenizer_batch, self.source, self.model_args)
 
         # OpenAI model call
         elif self.source == 'openai':
             if self.model not in self.supported_models['openai']:
-                raise ValueError('The specified model currently is not supported in this pacckage. Supported OpenAI models are: ' + ' '.join([f"{m}" for m in self.supported_models['openai']]))
+                raise ValueError('The specified model currently is not supported in this package. Supported OpenAI models are: ' + ' '.join([f"{m}" for m in self.supported_models['openai']]))
             if self.api_key is None:
                 raise ValueError('api key has not been specified for OpenAI model call')
             self.instance = OpenAIModelPack(model=self.model, api_key=self.api_key)
 
     # Direct to the attribute ofthe sub model pack class (attribute not found in the main model pack class)
     def __getattr__(self, name):
         return self.instance.__getattribute__(name)
```

### Comparing `panml-0.0.24/panml/search.py` & `panml-0.0.25/panml/search.py`

 * *Files identical despite different names*

### Comparing `panml-0.0.24/panml.egg-info/PKG-INFO` & `panml-0.0.25/panml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panml
-Version: 0.0.24
+Version: 0.0.25
 Summary: PanML is a high level generative AI/ML development library designed for ease of use and fast experimentation.
 Home-page: https://github.com/Pan-ML/panml
 Author: PanML team
 Author-email: teampanml@gmail.com
 License: MIT
 Keywords: generative AI,generative model,machine learning,large language model,LLM,prompt engineering,fine tuning,prompt tuning,retrieval augmentation,AI safety,AI alignment
 Platform: UNKNOWN
@@ -25,23 +25,23 @@
 License-File: LICENSE
 
 ## PanML: A high level generative AI/ML development and analysis library
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) 
 [![](https://dcbadge.vercel.app/api/server/cCsaqv9KFf?compact=true&style=flat)](https://discord.gg/cCsaqv9KFf)
 
-A library with simple to use abstractions when working with LLMs inspired by the sckit-learn style API. <br>
+A library with simple-to-use abstractions when working with LLMs, inspired by the scikit-learn style API. <br>
 🔍 Easily explore and experiment with commercial and open source LLMs, including ones that can be run on your local machine. <br>
 ⚡ Easily integrate language models of different sizes, including smaller, less compute heavy but still very useful LLMs in NLP-based Data Science contexts. <br>
 🚀 Support the development of LLM workflows with off-the-shelf or custom-built generative models. <br><br>
 Please note this is a work in progress, and it's open for collabration and contribution.
 
 ### What this library covers
 - [Inference and analysis of LLM](https://github.com/Pan-ML/panml/wiki/5.-Generative-model-analysis)
-- [Prompt chain engineering a LLM](https://github.com/Pan-ML/panml/wiki/2.-Prompt-chain-engineering)
+- [Prompt chain engineering with LLM](https://github.com/Pan-ML/panml/wiki/2.-Prompt-chain-engineering)
 - [Fine tuning of LLM](https://github.com/Pan-ML/panml/wiki/3.-Fine-tuning-your-LLM)
 - [Document question answering using LLM](https://github.com/Pan-ML/panml/wiki/7.-Retrieve-similar-documents-using-vector-search)
 - [Variable integrated code generation using LLM](https://github.com/Pan-ML/panml/wiki/4.-Prompted-code-generation)
 
 ### Current supported foundation models
 - [HuggingFace Hub](https://huggingface.co) - open source LLMs from Google, EleutherAI, Cerebras, StabilityAI, H2O, Salesforce, and others
 - [OpenAI](https://openai.com) - text-davinci-002/003, GPT3/3.5
```

### Comparing `panml-0.0.24/setup.py` & `panml-0.0.25/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding="utf-8")
 
 setup(
   name = 'panml', # package name     
   packages = find_packages(exclude=['test']), # package name
-  version = '0.0.24', # version
+  version = '0.0.25', # version
   license = 'MIT', # license
   description = 'PanML is a high level generative AI/ML development library designed for ease of use and fast experimentation.', # short description about the package
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'PanML team', # team name
   author_email = 'teampanml@gmail.com', # contact email
   url = 'https://github.com/Pan-ML/panml', # url link
@@ -29,14 +29,15 @@
         'datasets>=2.12.0',
         'torch>=2.0.0',
         'tqdm>=4.65.0',
         'transformers<=4.27.4',
         'faiss-cpu>=1.7.4',
         'sentence-transformers>=2.2.2',
         'accelerate<=0.19.0',
+        'peft==0.3.0',
       ],
   classifiers=[
     'Development Status :: 4 - Beta', # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of the package
     'Intended Audience :: Science/Research', # Define the audience type
     'Intended Audience :: Developers',
     'Intended Audience :: Education',
     'Intended Audience :: Information Technology',
```

### Comparing `panml-0.0.24/test/test_ModelPack.py` & `panml-0.0.25/test/test_ModelPack.py`

 * *Files identical despite different names*

### Comparing `panml-0.0.24/test/test_VectorEngine.py` & `panml-0.0.25/test/test_VectorEngine.py`

 * *Files identical despite different names*

