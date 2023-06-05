# Comparing `tmp/huntflow_webhook_models-0.0.1.tar.gz` & `tmp/huntflow_webhook_models-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huntflow_webhook_models-0.0.1.tar", last modified: Mon Jun  5 11:18:36 2023, max compression
+gzip compressed data, was "huntflow_webhook_models-0.0.3.tar", last modified: Mon Jun  5 12:40:44 2023, max compression
```

## Comparing `huntflow_webhook_models-0.0.1.tar` & `huntflow_webhook_models-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1071 2023-06-05 11:18:21.282213 huntflow_webhook_models-0.0.1/LICENSE
--rw-r--r--   0        0        0       69 2023-06-05 11:18:21.282213 huntflow_webhook_models-0.0.1/README.md
--rw-r--r--   0        0        0      122 2023-06-05 11:18:21.282213 huntflow_webhook_models-0.0.1/models/__init__.py
--rw-r--r--   0        0        0      615 2023-06-05 11:18:21.282213 huntflow_webhook_models-0.0.1/models/applicant.py
--rw-r--r--   0        0        0     1314 2023-06-05 11:18:21.282213 huntflow_webhook_models-0.0.1/models/base.py
--rw-r--r--   0        0        0        0 2023-06-05 11:18:21.282213 huntflow_webhook_models-0.0.1/models/common_models/__init__.py
--rw-r--r--   0        0        0     6500 2023-06-05 11:18:21.282213 huntflow_webhook_models-0.0.1/models/common_models/applicant.py
--rw-r--r--   0        0        0     5442 2023-06-05 11:18:21.282213 huntflow_webhook_models-0.0.1/models/common_models/calendar_event.py
--rw-r--r--   0        0        0      669 2023-06-05 11:18:21.282213 huntflow_webhook_models-0.0.1/models/common_models/hf_base.py
--rw-r--r--   0        0        0     2950 2023-06-05 11:18:21.282213 huntflow_webhook_models-0.0.1/models/common_models/survey_questionary.py
--rw-r--r--   0        0        0     3000 2023-06-05 11:18:21.282213 huntflow_webhook_models-0.0.1/models/common_models/vacancy.py
--rw-r--r--   0        0        0     1638 2023-06-05 11:18:21.282213 huntflow_webhook_models-0.0.1/models/consts.py
--rw-r--r--   0        0        0     1403 2023-06-05 11:18:36.522228 huntflow_webhook_models-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      648 1970-01-01 00:00:00.000000 huntflow_webhook_models-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-05 12:40:29.258196 huntflow_webhook_models-0.0.3/LICENSE
+-rw-r--r--   0        0        0       69 2023-06-05 12:40:29.258196 huntflow_webhook_models-0.0.3/README.md
+-rw-r--r--   0        0        0      122 2023-06-05 12:40:29.258196 huntflow_webhook_models-0.0.3/huntflow_webhook_models/__init__.py
+-rw-r--r--   0        0        0      666 2023-06-05 12:40:29.258196 huntflow_webhook_models-0.0.3/huntflow_webhook_models/applicant.py
+-rw-r--r--   0        0        0     1331 2023-06-05 12:40:29.258196 huntflow_webhook_models-0.0.3/huntflow_webhook_models/base.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:40:29.258196 huntflow_webhook_models-0.0.3/huntflow_webhook_models/common_models/__init__.py
+-rw-r--r--   0        0        0     6585 2023-06-05 12:40:29.258196 huntflow_webhook_models-0.0.3/huntflow_webhook_models/common_models/applicant.py
+-rw-r--r--   0        0        0     5459 2023-06-05 12:40:29.258196 huntflow_webhook_models-0.0.3/huntflow_webhook_models/common_models/calendar_event.py
+-rw-r--r--   0        0        0      669 2023-06-05 12:40:29.258196 huntflow_webhook_models-0.0.3/huntflow_webhook_models/common_models/hf_base.py
+-rw-r--r--   0        0        0     2950 2023-06-05 12:40:29.258196 huntflow_webhook_models-0.0.3/huntflow_webhook_models/common_models/survey_questionary.py
+-rw-r--r--   0        0        0     3017 2023-06-05 12:40:29.258196 huntflow_webhook_models-0.0.3/huntflow_webhook_models/common_models/vacancy.py
+-rw-r--r--   0        0        0     1638 2023-06-05 12:40:29.258196 huntflow_webhook_models-0.0.3/huntflow_webhook_models/consts.py
+-rw-r--r--   0        0        0     1403 2023-06-05 12:40:44.106388 huntflow_webhook_models-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      648 1970-01-01 00:00:00.000000 huntflow_webhook_models-0.0.3/PKG-INFO
```

### Comparing `huntflow_webhook_models-0.0.1/LICENSE` & `huntflow_webhook_models-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `huntflow_webhook_models-0.0.1/models/applicant.py` & `huntflow_webhook_models-0.0.3/huntflow_webhook_models/applicant.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import List
 
 from pydantic import BaseModel
 
-from models.base import BaseHuntflowWebhookRequest, WebhookMetaInfoBase
-from models.common_models.applicant import Applicant, ApplicantLog, ApplicantTag
-from models.consts import ApplicantWebhookActionType
+from huntflow_webhook_models.base import BaseHuntflowWebhookRequest, WebhookMetaInfoBase
+from huntflow_webhook_models.common_models.applicant import Applicant, ApplicantLog, ApplicantTag
+from huntflow_webhook_models.consts import ApplicantWebhookActionType
 
 
 class ApplicantEvent(BaseModel):
     applicant: Applicant
     applicant_log: ApplicantLog
     applicant_tags: List[ApplicantTag]
```

### Comparing `huntflow_webhook_models-0.0.1/models/base.py` & `huntflow_webhook_models-0.0.3/huntflow_webhook_models/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Dict, Optional
 
 from pydantic import BaseModel, Field
 
-from models.consts import WebhookEventType
+from huntflow_webhook_models.consts import WebhookEventType
 
 
 class Account(BaseModel):
     id: int = Field(..., description="Account ID", example=1)
     name: str = Field(..., description="Account name", example="Huntflow")
     nick: str = Field(..., description="Account nick", example="HF")
```

### Comparing `huntflow_webhook_models-0.0.1/models/common_models/applicant.py` & `huntflow_webhook_models-0.0.3/huntflow_webhook_models/common_models/applicant.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from datetime import date, datetime
 from typing import Any, Dict, List, Optional
 
 from pydantic import BaseModel, Field
 
-from models.common_models.calendar_event import ApplicantLogCalendarEvent
-from models.common_models.hf_base import AccountFile
-from models.common_models.survey_questionary import SurveyQuestionary
-from models.common_models.vacancy import Vacancy
-from models.consts import AgreementState, ApplicantLogType, SurveyType
+from huntflow_webhook_models.common_models.calendar_event import ApplicantLogCalendarEvent
+from huntflow_webhook_models.common_models.hf_base import AccountFile
+from huntflow_webhook_models.common_models.survey_questionary import SurveyQuestionary
+from huntflow_webhook_models.common_models.vacancy import Vacancy
+from huntflow_webhook_models.consts import AgreementState, ApplicantLogType, SurveyType
 
 
 class ApplicantSocial(BaseModel):
     id: int = Field(..., description="Social ID", example=1)
     social_type: str = Field(..., description="Social type", example="TELEGRAM")
     value: str = Field(..., description="Social nick/email", example="test_tg")
     verified: bool = Field(..., description="Verification flag", example=True)
```

### Comparing `huntflow_webhook_models-0.0.1/models/common_models/calendar_event.py` & `huntflow_webhook_models-0.0.3/huntflow_webhook_models/common_models/calendar_event.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import datetime
 from typing import List, Optional
 
 from pydantic import BaseModel, Field
 
-from models.consts import (
+from huntflow_webhook_models.consts import (
     CalendarEventReminderMethod,
     CalendarEventStatus,
     CalendarEventType,
     Transparency,
 )
```

### Comparing `huntflow_webhook_models-0.0.1/models/common_models/hf_base.py` & `huntflow_webhook_models-0.0.3/huntflow_webhook_models/common_models/hf_base.py`

 * *Files identical despite different names*

### Comparing `huntflow_webhook_models-0.0.1/models/common_models/survey_questionary.py` & `huntflow_webhook_models-0.0.3/huntflow_webhook_models/common_models/survey_questionary.py`

 * *Files identical despite different names*

### Comparing `huntflow_webhook_models-0.0.1/models/common_models/vacancy.py` & `huntflow_webhook_models-0.0.3/huntflow_webhook_models/common_models/vacancy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import date, datetime
 from typing import Dict, Optional
 
 from pydantic import BaseModel, Field
 
-from models.consts import VacancyState
+from huntflow_webhook_models.consts import VacancyState
 
 
 class FillQuota(BaseModel):
     id: int = Field(..., description="Fill quota ID", example=1)
     applicants_to_hire: int = Field(..., description="Amoun of applicant to hire", example=1)
     closed: Optional[datetime] = Field(
         None,
```

### Comparing `huntflow_webhook_models-0.0.1/models/consts.py` & `huntflow_webhook_models-0.0.3/huntflow_webhook_models/consts.py`

 * *Files identical despite different names*

### Comparing `huntflow_webhook_models-0.0.1/pyproject.toml` & `huntflow_webhook_models-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "huntflow-webhook-models"
-version = "0.0.1"
+version = "0.0.3"
 description = "Huntflow webhooks requests data models"
 authors = [
     { name = "Developers huntflow", email = "developer@huntflow.ru" },
 ]
 dependencies = [
     "pydantic>=1.7.2",
     "openapi-schema-pydantic>=1.2.4",
```

### Comparing `huntflow_webhook_models-0.0.1/PKG-INFO` & `huntflow_webhook_models-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huntflow-webhook-models
-Version: 0.0.1
+Version: 0.0.3
 Summary: Huntflow webhooks requests data models
 Author-Email: Developers huntflow <developer@huntflow.ru>
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

