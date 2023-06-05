# Comparing `tmp/cohere-4.7.0.tar.gz` & `tmp/cohere-4.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cohere-4.7.0.tar", max compression
+gzip compressed data, was "cohere-4.8.0.tar", max compression
```

## Comparing `cohere-4.7.0.tar` & `cohere-4.8.0.tar`

### file list

```diff
@@ -1,25 +1,27 @@
--rw-r--r--   0        0        0     1063 2023-06-02 17:04:01.524493 cohere-4.7.0/LICENSE
--rw-r--r--   0        0        0     4480 2023-06-02 17:04:01.524493 cohere-4.7.0/README.md
--rw-r--r--   0        0        0      771 2023-06-02 17:04:01.524493 cohere-4.7.0/cohere/__init__.py
--rw-r--r--   0        0        0    38178 2023-06-02 17:04:01.524493 cohere-4.7.0/cohere/client.py
--rw-r--r--   0        0        0    28216 2023-06-02 17:04:01.524493 cohere-4.7.0/cohere/client_async.py
--rw-r--r--   0        0        0     1187 2023-06-02 17:04:01.524493 cohere-4.7.0/cohere/error.py
--rw-r--r--   0        0        0      529 2023-06-02 17:04:01.524493 cohere-4.7.0/cohere/logging.py
--rw-r--r--   0        0        0      839 2023-06-02 17:04:01.524493 cohere-4.7.0/cohere/responses/__init__.py
--rw-r--r--   0        0        0     2678 2023-06-02 17:04:01.524493 cohere-4.7.0/cohere/responses/base.py
--rw-r--r--   0        0        0     3438 2023-06-02 17:04:01.524493 cohere-4.7.0/cohere/responses/bulk_embed.py
--rw-r--r--   0        0        0     4309 2023-06-02 17:04:01.524493 cohere-4.7.0/cohere/responses/chat.py
--rw-r--r--   0        0        0     1461 2023-06-02 17:04:01.524493 cohere-4.7.0/cohere/responses/classify.py
--rw-r--r--   0        0        0     4826 2023-06-02 17:04:01.524493 cohere-4.7.0/cohere/responses/cluster.py
--rw-r--r--   0        0        0      436 2023-06-02 17:04:01.524493 cohere-4.7.0/cohere/responses/codebook.py
--rw-r--r--   0        0        0      552 2023-06-02 17:04:01.524493 cohere-4.7.0/cohere/responses/detectlang.py
--rw-r--r--   0        0        0      587 2023-06-02 17:04:01.524493 cohere-4.7.0/cohere/responses/embeddings.py
--rw-r--r--   0        0        0      342 2023-06-02 17:04:01.524493 cohere-4.7.0/cohere/responses/feedback.py
--rw-r--r--   0        0        0     5990 2023-06-02 17:04:01.524493 cohere-4.7.0/cohere/responses/generation.py
--rw-r--r--   0        0        0     2057 2023-06-02 17:04:01.524493 cohere-4.7.0/cohere/responses/rerank.py
--rw-r--r--   0        0        0      667 2023-06-02 17:04:01.524493 cohere-4.7.0/cohere/responses/summarize.py
--rw-r--r--   0        0        0     1221 2023-06-02 17:04:01.524493 cohere-4.7.0/cohere/responses/tokenize.py
--rw-r--r--   0        0        0     3283 2023-06-02 17:04:01.524493 cohere-4.7.0/cohere/utils.py
--rw-r--r--   0        0        0      653 2023-06-02 17:04:01.528493 cohere-4.7.0/pyproject.toml
--rw-r--r--   0        0        0     5227 1970-01-01 00:00:00.000000 cohere-4.7.0/setup.py
--rw-r--r--   0        0        0     5034 1970-01-01 00:00:00.000000 cohere-4.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-05 07:10:14.680087 cohere-4.8.0/LICENSE
+-rw-r--r--   0        0        0     4480 2023-06-05 07:10:14.680087 cohere-4.8.0/README.md
+-rw-r--r--   0        0        0      801 2023-06-05 07:10:14.680087 cohere-4.8.0/cohere/__init__.py
+-rw-r--r--   0        0        0    44486 2023-06-05 07:10:14.680087 cohere-4.8.0/cohere/client.py
+-rw-r--r--   0        0        0    34666 2023-06-05 07:10:14.680087 cohere-4.8.0/cohere/client_async.py
+-rw-r--r--   0        0        0     5215 2023-06-05 07:10:14.680087 cohere-4.8.0/cohere/custom_model_dataset.py
+-rw-r--r--   0        0        0     1187 2023-06-05 07:10:14.680087 cohere-4.8.0/cohere/error.py
+-rw-r--r--   0        0        0      529 2023-06-05 07:10:14.680087 cohere-4.8.0/cohere/logging.py
+-rw-r--r--   0        0        0      839 2023-06-05 07:10:14.680087 cohere-4.8.0/cohere/responses/__init__.py
+-rw-r--r--   0        0        0     2678 2023-06-05 07:10:14.680087 cohere-4.8.0/cohere/responses/base.py
+-rw-r--r--   0        0        0     3438 2023-06-05 07:10:14.680087 cohere-4.8.0/cohere/responses/bulk_embed.py
+-rw-r--r--   0        0        0     4309 2023-06-05 07:10:14.680087 cohere-4.8.0/cohere/responses/chat.py
+-rw-r--r--   0        0        0     1461 2023-06-05 07:10:14.680087 cohere-4.8.0/cohere/responses/classify.py
+-rw-r--r--   0        0        0     4826 2023-06-05 07:10:14.680087 cohere-4.8.0/cohere/responses/cluster.py
+-rw-r--r--   0        0        0      436 2023-06-05 07:10:14.680087 cohere-4.8.0/cohere/responses/codebook.py
+-rw-r--r--   0        0        0     2205 2023-06-05 07:10:14.680087 cohere-4.8.0/cohere/responses/custom_model.py
+-rw-r--r--   0        0        0      552 2023-06-05 07:10:14.680087 cohere-4.8.0/cohere/responses/detectlang.py
+-rw-r--r--   0        0        0      587 2023-06-05 07:10:14.680087 cohere-4.8.0/cohere/responses/embeddings.py
+-rw-r--r--   0        0        0      342 2023-06-05 07:10:14.680087 cohere-4.8.0/cohere/responses/feedback.py
+-rw-r--r--   0        0        0     5990 2023-06-05 07:10:14.680087 cohere-4.8.0/cohere/responses/generation.py
+-rw-r--r--   0        0        0     2057 2023-06-05 07:10:14.680087 cohere-4.8.0/cohere/responses/rerank.py
+-rw-r--r--   0        0        0      667 2023-06-05 07:10:14.680087 cohere-4.8.0/cohere/responses/summarize.py
+-rw-r--r--   0        0        0     1221 2023-06-05 07:10:14.680087 cohere-4.8.0/cohere/responses/tokenize.py
+-rw-r--r--   0        0        0     3283 2023-06-05 07:10:14.684087 cohere-4.8.0/cohere/utils.py
+-rw-r--r--   0        0        0      653 2023-06-05 07:10:14.684087 cohere-4.8.0/pyproject.toml
+-rw-r--r--   0        0        0     5227 1970-01-01 00:00:00.000000 cohere-4.8.0/setup.py
+-rw-r--r--   0        0        0     5034 1970-01-01 00:00:00.000000 cohere-4.8.0/PKG-INFO
```

### Comparing `cohere-4.7.0/LICENSE` & `cohere-4.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cohere-4.7.0/README.md` & `cohere-4.8.0/README.md`

 * *Files identical despite different names*

### Comparing `cohere-4.7.0/cohere/__init__.py` & `cohere-4.8.0/cohere/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,7 +20,8 @@
 
 CHECK_API_KEY_URL = "check-api-key"
 TOKENIZE_URL = "tokenize"
 DETOKENIZE_URL = "detokenize"
 
 CLUSTER_JOBS_URL = "cluster-jobs"
 BULK_EMBED_JOBS_URL = "embed-jobs"
+CUSTOM_MODEL_URL = "finetune"
```

### Comparing `cohere-4.7.0/cohere/client.py` & `cohere-4.8.0/cohere/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 import json as jsonlib
 import os
 from concurrent.futures import ThreadPoolExecutor
 from dataclasses import asdict
+from datetime import datetime, timezone
 from functools import partial
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Dict, Iterable, List, Optional, Union
+
+try:
+    from typing import Literal, TypedDict
+except ImportError:
+    from typing_extensions import Literal, TypedDict
 
 import requests
 from requests.adapters import HTTPAdapter
 from urllib3 import Retry
 
 import cohere
+from cohere.custom_model_dataset import CustomModelDataset
 from cohere.error import CohereAPIError, CohereConnectionError, CohereError
 from cohere.logging import logger
 from cohere.responses import (
     Classification,
     Classifications,
     Codebook,
     Detokenization,
@@ -22,14 +29,21 @@
     Tokens,
 )
 from cohere.responses.bulk_embed import BulkEmbedJob, CreateBulkEmbedJobResponse
 from cohere.responses.chat import Chat, StreamingChat
 from cohere.responses.classify import Example as ClassifyExample
 from cohere.responses.classify import LabelPrediction
 from cohere.responses.cluster import ClusterJobResult, CreateClusterJobResponse
+from cohere.responses.custom_model import (
+    CUSTOM_MODEL_PRODUCT_MAPPING,
+    CUSTOM_MODEL_STATUS,
+    CUSTOM_MODEL_TYPE,
+    INTERNAL_CUSTOM_MODEL_TYPE,
+    CustomModel,
+)
 from cohere.responses.detectlang import DetectLanguageResponse, Language
 from cohere.responses.embeddings import Embeddings
 from cohere.responses.feedback import (
     GenerateFeedbackResponse,
     GeneratePreferenceFeedbackResponse,
     PreferenceRating,
 )
@@ -893,7 +907,130 @@
         """
 
         return wait_for_job(
             get_job=partial(self.get_bulk_embed_job, job_id),
             timeout=timeout,
             interval=interval,
         )
+
+    def create_custom_model(self, name: str, model_type: CUSTOM_MODEL_TYPE, dataset: CustomModelDataset) -> CustomModel:
+        """Create a new custom model
+
+        Args:
+            name (str): name of your custom model, has to be unique across your organization
+            model_type (GENERATIVE, EMBED, CLASSIFY): type of custom model
+            dataset (InMemoryDataset, CsvDataset, JsonlDataset, TextDataset): A dataset for your training. Consists of a train and optional eval file.
+        Returns:
+            str: the id of the custom model that was created
+
+        Examples:
+            prompt completion custom model with csv file
+                >>> from cohere.custom_model_dataset import CsvDataset
+                >>> co = cohere.Client("YOUR_API_KEY")
+                >>> dataset = CsvDataset(train_file="/path/to/your/file.csv", delimiter=",")
+                >>> finetune = co.create_custom_model("prompt-completion-ft", dataset=dataset, model_type="GENERATIVE")
+
+            prompt completion custom model with in-memory dataset
+                >>> from cohere.custom_model_dataset import InMemoryDataset
+                >>> co = cohere.Client("YOUR_API_KEY")
+                >>> dataset = InMemoryDataset(training_data=[
+                >>>     ("this is the prompt", "and this is the completion"),
+                >>>     ("another prompt", "and another completion")
+                >>> ])
+                >>> finetune = co.create_custom_model("prompt-completion-ft", dataset=dataset, model_type="GENERATIVE")
+
+        """
+        internal_custom_model_type = CUSTOM_MODEL_PRODUCT_MAPPING[model_type]
+        json = {
+            "name": name,
+            "settings": {
+                "trainFiles": [],
+                "evalFiles": [],
+                "baseModel": "medium",
+                "finetuneType": internal_custom_model_type,
+            },
+        }
+        remote_path = self._upload_dataset(
+            dataset.get_train_data(), name, dataset.train_file_name(), internal_custom_model_type
+        )
+        json["settings"]["trainFiles"].append({"path": remote_path, **dataset.file_config()})
+        if dataset.has_eval_file():
+            remote_path = self._upload_dataset(
+                dataset.get_eval_data(), name, dataset.eval_file_name(), internal_custom_model_type
+            )
+            json["settings"]["evalFiles"].append({"path": remote_path, **dataset.file_config()})
+
+        response = self._request(f"{cohere.CUSTOM_MODEL_URL}/CreateFinetune", method="POST", json=json)
+        return CustomModel.from_dict(response["finetune"])
+
+    def _upload_dataset(
+        self, content: Iterable[bytes], custom_model_name: str, file_name: str, type: INTERNAL_CUSTOM_MODEL_TYPE
+    ) -> str:
+        gcs = self._create_signed_url(custom_model_name, file_name, type)
+        response = requests.put(gcs["url"], data=content, headers={"content-type": "text/plain"})
+        if response.status_code != 200:
+            raise CohereError(message=f"Unexpected server error (status {response.status_code}): {response.text}")
+        return gcs["gcspath"]
+
+    def _create_signed_url(
+        self, custom_model_name: str, file_name: str, type: INTERNAL_CUSTOM_MODEL_TYPE
+    ) -> TypedDict("gcsData", {"url": str, "gcspath": str}):
+        json = {"finetuneName": custom_model_name, "fileName": file_name, "finetuneType": type}
+        return self._request(f"{cohere.CUSTOM_MODEL_URL}/GetFinetuneUploadSignedURL", method="POST", json=json)
+
+    def get_custom_model(self, custom_model_id: str) -> CustomModel:
+        """Get a custom model by id.
+
+        Args:
+            custom_model_id (str): custom model id
+        Returns:
+            CustomModel: the custom model
+        """
+        json = {"finetuneID": custom_model_id}
+        response = self._request(f"{cohere.CUSTOM_MODEL_URL}/GetFinetune", method="POST", json=json)
+        return CustomModel.from_dict(response["finetune"])
+
+    def get_custom_model_by_name(self, name: str) -> CustomModel:
+        """Get a custom model by name.
+
+        Args:
+            name (str): custom model name
+        Returns:
+            CustomModel: the custom model
+        """
+        json = {"name": name}
+        response = self._request(f"{cohere.CUSTOM_MODEL_URL}/GetFinetuneByName", method="POST", json=json)
+        return CustomModel.from_dict(response["finetune"])
+
+    def list_custom_models(
+        self,
+        statuses: Optional[List[CUSTOM_MODEL_STATUS]] = None,
+        before: Optional[datetime] = None,
+        after: Optional[datetime] = None,
+        order_by: Optional[Literal["asc", "desc"]] = None,
+    ) -> List[CustomModel]:
+        """List custom models of your organization. Limit is 50.
+
+        Args:
+            statuses (CUSTOM_MODEL_STATUS, optional): search for fintunes which are in one of these states
+            before (datetime, optional): search for custom models that were created before this timestamp
+            after (datetime, optional): search for custom models that were created after this timestamp
+            order_by (Literal["asc", "desc"], optional): sort custom models by created at, either asc or desc
+        Returns:
+            List[CustomModel]: a list of custom models.
+        """
+        if before:
+            before = before.replace(tzinfo=before.tzinfo or timezone.utc)
+        if after:
+            after = after.replace(tzinfo=after.tzinfo or timezone.utc)
+
+        json = {
+            "query": {
+                "statuses": statuses,
+                "before": before.isoformat(timespec="seconds") if before else None,
+                "after": after.isoformat(timespec="seconds") if after else None,
+                "orderBy": order_by,
+            }
+        }
+
+        response = self._request(f"{cohere.CUSTOM_MODEL_URL}/ListFinetunes", method="POST", json=json)
+        return [CustomModel.from_dict(r) for r in response["finetunes"]]
```

### Comparing `cohere-4.7.0/cohere/client_async.py` & `cohere-4.8.0/cohere/client_async.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 import asyncio
 import json as jsonlib
 import os
 import posixpath
 import time
 from collections import defaultdict
 from dataclasses import asdict
+from datetime import datetime, timezone
 from functools import partial
-from typing import Any, Callable, Dict, List, Optional, Union
+from typing import Any, Callable, Dict, Iterable, List, Optional, Union
+
+try:
+    from typing import Literal, TypedDict
+except ImportError:
+    from typing_extensions import Literal, TypedDict
 
 import aiohttp
 import backoff
 
 import cohere
 from cohere.client import Client
+from cohere.custom_model_dataset import CustomModelDataset
 from cohere.error import CohereAPIError, CohereConnectionError, CohereError
 from cohere.logging import logger
 from cohere.responses import (
     AsyncCreateClusterJobResponse,
     Classification,
     Classifications,
     ClusterJobResult,
@@ -34,14 +41,21 @@
     StreamingGenerations,
     SummarizeResponse,
     Tokens,
 )
 from cohere.responses.bulk_embed import AsyncCreateBulkEmbedJobResponse, BulkEmbedJob
 from cohere.responses.chat import AsyncChat, StreamingChat
 from cohere.responses.classify import Example as ClassifyExample
+from cohere.responses.custom_model import (
+    CUSTOM_MODEL_PRODUCT_MAPPING,
+    CUSTOM_MODEL_STATUS,
+    CUSTOM_MODEL_TYPE,
+    INTERNAL_CUSTOM_MODEL_TYPE,
+    CustomModel,
+)
 from cohere.utils import async_wait_for_job, is_api_key_valid, np_json_dumps
 
 JSON = Union[Dict, List]
 
 
 class AsyncClient(Client):
     """AsyncClient
@@ -639,14 +653,140 @@
 
         return await async_wait_for_job(
             get_job=partial(self.get_bulk_embed_job, job_id),
             timeout=timeout,
             interval=interval,
         )
 
+    async def create_custom_model(
+        self, name: str, model_type: CUSTOM_MODEL_TYPE, dataset: CustomModelDataset
+    ) -> CustomModel:
+        """Create a new custom model
+
+        Args:
+            name (str): name of your custom model, has to be unique across your organization
+            model_type (GENERATIVE, EMBED, CLASSIFY): type of custom model
+            dataset (InMemoryDataset, CsvDataset, JsonlDataset, TextDataset): A dataset for your training. Consists of a train and optional eval file.
+        Returns:
+            str: the id of the custom model that was created
+
+        Examples:
+            prompt completion custom model with csv file
+                >>> from cohere.custom_model_dataset import CsvDataset
+                >>> co = cohere.Client("YOUR_API_KEY")
+                >>> dataset = CsvDataset(train_file="/path/to/your/file.csv", delimiter=",")
+                >>> finetune = co.create_custom_model("prompt-completion-ft", dataset=dataset, model_type="GENERATIVE")
+
+            prompt completion custom model with in-memory dataset
+                >>> from cohere.custom_model_dataset import InMemoryDataset
+                >>> co = cohere.Client("YOUR_API_KEY")
+                >>> dataset = InMemoryDataset(training_data=[
+                >>>     ("this is the prompt", "and this is the completion"),
+                >>>     ("another prompt", "and another completion")
+                >>> ])
+                >>> finetune = co.create_custom_model("prompt-completion-ft", dataset=dataset, model_type="GENERATIVE")
+
+        """
+        internal_custom_model_type = CUSTOM_MODEL_PRODUCT_MAPPING[model_type]
+        json = {
+            "name": name,
+            "settings": {
+                "trainFiles": [],
+                "evalFiles": [],
+                "baseModel": "medium",
+                "finetuneType": internal_custom_model_type,
+            },
+        }
+        remote_path = await self._upload_dataset(
+            dataset.get_train_data(), name, dataset.train_file_name(), internal_custom_model_type
+        )
+        json["settings"]["trainFiles"].append({"path": remote_path, **dataset.file_config()})
+        if dataset.has_eval_file():
+            remote_path = await self._upload_dataset(
+                dataset.get_eval_data(), name, dataset.eval_file_name(), internal_custom_model_type
+            )
+            json["settings"]["evalFiles"].append({"path": remote_path, **dataset.file_config()})
+
+        response = await self._request(f"{cohere.CUSTOM_MODEL_URL}/CreateFinetune", method="POST", json=json)
+        return CustomModel.from_dict(response["finetune"])
+
+    async def _upload_dataset(
+        self, content: Iterable[bytes], custom_model_name: str, file_name: str, type: INTERNAL_CUSTOM_MODEL_TYPE
+    ) -> str:
+        gcs = await self._create_signed_url(custom_model_name, file_name, type)
+        session = await self._backend.session()
+        response = await session.put(url=gcs["url"], data=b"".join(content), headers={"content-type": "text/plain"})
+        if response.status != 200:
+            raise CohereError(message=f"Unexpected server error (status {response.status}): {response.text}")
+        return gcs["gcspath"]
+
+    async def _create_signed_url(
+        self, custom_model_name: str, file_name: str, type: INTERNAL_CUSTOM_MODEL_TYPE
+    ) -> TypedDict("gcsData", {"url": str, "gcspath": str}):
+        json = {"finetuneName": custom_model_name, "fileName": file_name, "finetuneType": type}
+        return await self._request(f"{cohere.CUSTOM_MODEL_URL}/GetFinetuneUploadSignedURL", method="POST", json=json)
+
+    async def get_custom_model(self, custom_model_id: str) -> CustomModel:
+        """Get a custom model by id.
+
+        Args:
+            custom_model_id (str): custom model id
+        Returns:
+            CustomModel: the custom model
+        """
+        json = {"finetuneID": custom_model_id}
+        response = await self._request(f"{cohere.CUSTOM_MODEL_URL}/GetFinetune", method="POST", json=json)
+        return CustomModel.from_dict(response["finetune"])
+
+    async def get_custom_model_by_name(self, name: str) -> CustomModel:
+        """Get a custom model by name.
+
+        Args:
+            name (str): custom model name
+        Returns:
+            CustomModel: the custom model
+        """
+        json = {"name": name}
+        response = await self._request(f"{cohere.CUSTOM_MODEL_URL}/GetFinetuneByName", method="POST", json=json)
+        return CustomModel.from_dict(response["finetune"])
+
+    async def list_custom_models(
+        self,
+        statuses: Optional[List[CUSTOM_MODEL_STATUS]] = None,
+        before: Optional[datetime] = None,
+        after: Optional[datetime] = None,
+        order_by: Optional[Literal["asc", "desc"]] = None,
+    ) -> List[CustomModel]:
+        """List custom models of your organization.
+
+        Args:
+            statuses (CUSTOM_MODEL_STATUS, optional): search for fintunes which are in one of these states
+            before (datetime, optional): search for custom models that were created before this timestamp
+            after (datetime, optional): search for custom models that were created after this timestamp
+            order_by (Literal["asc", "desc"], optional): sort custom models by created at, either asc or desc
+        Returns:
+            List[CustomModel]: a list of custom models.
+        """
+        if before:
+            before = before.replace(tzinfo=before.tzinfo or timezone.utc)
+        if after:
+            after = after.replace(tzinfo=after.tzinfo or timezone.utc)
+
+        json = {
+            "query": {
+                "statuses": statuses,
+                "before": before.isoformat(timespec="seconds") if before else None,
+                "after": after.isoformat(timespec="seconds") if after else None,
+                "orderBy": order_by,
+            }
+        }
+
+        response = await self._request(f"{cohere.CUSTOM_MODEL_URL}/ListFinetunes", method="POST", json=json)
+        return [CustomModel.from_dict(r) for r in response["finetunes"]]
+
 
 class AIOHTTPBackend:
     """HTTP backend which handles retries, concurrency limiting and logging"""
 
     SLEEP_AFTER_FAILURE = defaultdict(lambda: 0.25, {429: 5})
 
     def __init__(self, logger, max_concurrent_requests: int = 64, max_retries: int = 5, timeout: int = 120):
```

### Comparing `cohere-4.7.0/cohere/error.py` & `cohere-4.8.0/cohere/error.py`

 * *Files identical despite different names*

### Comparing `cohere-4.7.0/cohere/logging.py` & `cohere-4.8.0/cohere/logging.py`

 * *Files identical despite different names*

### Comparing `cohere-4.7.0/cohere/responses/__init__.py` & `cohere-4.8.0/cohere/responses/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-4.7.0/cohere/responses/base.py` & `cohere-4.8.0/cohere/responses/base.py`

 * *Files identical despite different names*

### Comparing `cohere-4.7.0/cohere/responses/bulk_embed.py` & `cohere-4.8.0/cohere/responses/bulk_embed.py`

 * *Files identical despite different names*

### Comparing `cohere-4.7.0/cohere/responses/chat.py` & `cohere-4.8.0/cohere/responses/chat.py`

 * *Files identical despite different names*

### Comparing `cohere-4.7.0/cohere/responses/classify.py` & `cohere-4.8.0/cohere/responses/classify.py`

 * *Files identical despite different names*

### Comparing `cohere-4.7.0/cohere/responses/cluster.py` & `cohere-4.8.0/cohere/responses/cluster.py`

 * *Files identical despite different names*

### Comparing `cohere-4.7.0/cohere/responses/detectlang.py` & `cohere-4.8.0/cohere/responses/detectlang.py`

 * *Files identical despite different names*

### Comparing `cohere-4.7.0/cohere/responses/embeddings.py` & `cohere-4.8.0/cohere/responses/embeddings.py`

 * *Files identical despite different names*

### Comparing `cohere-4.7.0/cohere/responses/generation.py` & `cohere-4.8.0/cohere/responses/generation.py`

 * *Files identical despite different names*

### Comparing `cohere-4.7.0/cohere/responses/rerank.py` & `cohere-4.8.0/cohere/responses/rerank.py`

 * *Files identical despite different names*

### Comparing `cohere-4.7.0/cohere/responses/summarize.py` & `cohere-4.8.0/cohere/responses/summarize.py`

 * *Files identical despite different names*

### Comparing `cohere-4.7.0/cohere/responses/tokenize.py` & `cohere-4.8.0/cohere/responses/tokenize.py`

 * *Files identical despite different names*

### Comparing `cohere-4.7.0/cohere/utils.py` & `cohere-4.8.0/cohere/utils.py`

 * *Files identical despite different names*

### Comparing `cohere-4.7.0/pyproject.toml` & `cohere-4.8.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cohere"
-version = "4.7.0"
+version = "4.8.0"
 description = ""
 authors = ["Cohere"]
 readme = "README.md"
 
 [tool.black]
 line-length = 120
 target_version = ['py38']
```

### Comparing `cohere-4.7.0/setup.py` & `cohere-4.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['aiohttp>=3.0,<4.0', 'backoff>=2.0,<3.0', 'requests>=2.0,<3.0']
 
 setup_kwargs = {
     'name': 'cohere',
-    'version': '4.7.0',
+    'version': '4.8.0',
     'description': '',
     'long_description': '![ci badge](https://github.com/cohere-ai/cohere-python/actions/workflows/test.yaml/badge.svg)\n![version badge](https://img.shields.io/pypi/v/cohere)\n![license badge](https://img.shields.io/github/license/cohere-ai/cohere-python)\n\n# Cohere Python SDK\n\nThis package provides functionality developed to simplify interfacing with the [Cohere API](https://docs.cohere.ai/) in Python 3.\n\n## Documentation\n\n* SDK Documentation is hosted on [Read the docs](https://cohere-sdk.readthedocs.io/en/latest/).\n  * You can build SDK documentation locally using `cd docs; make clean html`.\n* For more details on advanced parameters, you can also consult the [API documentation](https://docs.cohere.ai/reference/about).\n* See the [examples](examples/) directory for examples, including  some additional functionality for visualizations in Jupyter notebooks.\n\n## Installation\n\nThe package can be installed with `pip`:\n\n```bash\npip install --upgrade cohere\n```\n\nInstall from source:\n\n```bash\npip install .\n```\n\n### Requirements\n\n- Python 3.7+\n\n## Quick Start\n\nTo use this library, you must have an API key and specify it as a string when creating the `cohere.Client` object. API keys can be created through the [platform](https://os.cohere.ai). This is a basic example of the creating the client and using the `generate` endpoint.\n\n```python\nimport cohere\n\n# initialize the Cohere Client with an API Key\nco = cohere.Client(\'YOUR_API_KEY\')\n\n# generate a prediction for a prompt\nprediction = co.generate(\n            model=\'large\',\n            prompt=\'co:here\',\n            max_tokens=10)\n\n# print the predicted text\nprint(\'prediction: {}\'.format(prediction.generations[0].text))\n```\n\nThere is also an asyncio compatible client called `cohere.AsyncClient` with an equivalent interface. Consult the [SDK Docs](https://cohere-sdk.readthedocs.io/en/latest/) for more details.\n\n## Versioning\n\nEach SDK release is only compatible with the latest version of the Cohere API at the time of release. To use the SDK with an older API version, you need to download a version of the SDK tied to the API version you want. Look at the [Changelog](https://github.com/cohere-ai/cohere-python/blob/main/CHANGELOG.md) to see which SDK version to download.\n\n\n## Endpoints\n\nFor a full breakdown of endpoints and arguments, please consult the [SDK Docs](https://cohere-sdk.readthedocs.io/en/latest/) and [Cohere API Docs](https://docs.cohere.ai/).\n\n| Cohere Endpoint  | Function             |\n| ---------------- | -------------------- |\n| /generate        | co.generate()        |\n| /embed           | co.embed()           |\n| /classify        | co.classify()        |\n| /tokenize        | co.tokenize()        |\n| /detokenize      | co.detokenize()      |\n| /detect-language | co.detect_language() |\n\n## Models\n\nWhen you call Cohere\'s APIs we decide on a good default model for your use-case behind the scenes. The default model is great to get you started, but in production environments we recommend that you specify the model size yourself via the `model` parameter. Learn more about the available models here(https://os.cohere.ai)\n\n## Responses\n\nAll of the endpoint functions will return a Cohere object corresponding to the endpoint (e.g. for generation, it would be `Generation`). The responses can be found as instance variables of the object (e.g. generation would be `Generation.text`). The names of these instance variables and a detailed breakdown of the response body can be found in the [SDK Docs](https://cohere-sdk.readthedocs.io/en/latest/) and [Cohere Docs](https://docs.cohere.ai/). Printing the Cohere response object itself will display an organized view of the instance variables.\n\n## Exceptions\n\nUnsuccessful API calls from the SDK will raise an exception. Please see the documentation\'s page on [errors](https://docs.cohere.ai/errors-reference) for more information about what the errors mean.\n\n## Contributing\n\nTo set up a development environment, run:\n\n```\npoetry shell    # any time you want to run code or tests\npoetry install  # install and update dependencies in your environment, the first time\n```\n\nIn addition, to ensure your code is formatted correctly, install pre-commit hooks using:\n\n```bash\npre-commit install\n```\n\nYou can run tests locally using:\n```\npython -m pytest\n```\n\nYou can configure a different base url with:\n```bash\nCO_API_URL="https://localhost:8050" python3 foo.py\n```\nor\n```python\ncohere.COHERE_API_URL = "https://localhost:8050" # Place before client initilization\n```\n',
     'author': 'Cohere',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `cohere-4.7.0/PKG-INFO` & `cohere-4.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cohere
-Version: 4.7.0
+Version: 4.8.0
 Summary: 
 Author: Cohere
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

