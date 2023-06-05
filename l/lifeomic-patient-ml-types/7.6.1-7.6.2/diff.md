# Comparing `tmp/lifeomic_patient_ml_types-7.6.1.tar.gz` & `tmp/lifeomic_patient_ml_types-7.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifeomic_patient_ml_types-7.6.1.tar", max compression
+gzip compressed data, was "lifeomic_patient_ml_types-7.6.2.tar", max compression
```

## Comparing `lifeomic_patient_ml_types-7.6.1.tar` & `lifeomic_patient_ml_types-7.6.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0    14545 2023-05-30 17:37:25.675744 lifeomic_patient_ml_types-7.6.1/lifeomic_patient_ml_types/schemas.py
--rw-r--r--   0        0        0      664 2023-05-30 17:38:45.752365 lifeomic_patient_ml_types-7.6.1/pyproject.toml
--rw-r--r--   0        0        0      585 1970-01-01 00:00:00.000000 lifeomic_patient_ml_types-7.6.1/setup.py
--rw-r--r--   0        0        0      478 1970-01-01 00:00:00.000000 lifeomic_patient_ml_types-7.6.1/PKG-INFO
+-rw-r--r--   0        0        0    15045 2023-06-05 19:27:08.715935 lifeomic_patient_ml_types-7.6.2/lifeomic_patient_ml_types/schemas.py
+-rw-r--r--   0        0        0      664 2023-06-05 19:28:26.884631 lifeomic_patient_ml_types-7.6.2/pyproject.toml
+-rw-r--r--   0        0        0      585 1970-01-01 00:00:00.000000 lifeomic_patient_ml_types-7.6.2/setup.py
+-rw-r--r--   0        0        0      478 1970-01-01 00:00:00.000000 lifeomic_patient_ml_types-7.6.2/PKG-INFO
```

### Comparing `lifeomic_patient_ml_types-7.6.1/lifeomic_patient_ml_types/schemas.py` & `lifeomic_patient_ml_types-7.6.2/lifeomic_patient_ml_types/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -341,22 +341,37 @@
     type: Literal["cloud"]
 
 
 class DeployApproach(BaseModel):
     __root__: Union[EdgeDeployApproach, CloudDeployApproach]
 
 
+class EvaluationApproach(BaseModel):
+    class Config:
+        extra = Extra.forbid
+
+    type: Literal["customImage"]
+    imageUri: str = Field(
+        ...,
+        regex="^[0-9]+\\.dkr.ecr.[-a-z0-9]+\\.amazonaws\\.com\\/[-_a-zA-Z0-9]+:[-_a-zA-Z0-9]+$",
+    )
+    """
+    An aws ecr image uri of the form <account-id>.dkr.ecr.<region>.amazonaws.com/<repo-name>:<tag>
+    """
+
+
 class ModelConfigBase(BaseModel):
     class Config:
         extra = Extra.allow
 
     name: str
     description: str
     trainingApproach: TrainingApproach
     deployApproach: DeployApproach
+    evaluationApproach: Optional[EvaluationApproach] = None
 
 
 class Split(BaseModel):
     class Config:
         extra = Extra.forbid
 
     n: float
@@ -519,15 +534,16 @@
     """
     UUID uniquely identifying this model config.
     """
     accountId: str
     problemDefinition: MlProblemDefinition
     deployedId: Optional[str] = None
     """
-    The ID of the model version currently deployed for this model config. (deprecated, use championId instead)
+    The ID of the model version currently deployed for this model config.
+    @deprecated use championId instead
     """
     championId: Optional[str] = None
     """
     The ID of the champion model run for this model config.
     """
 
 
@@ -587,7 +603,8 @@
     approvals: List[ApprovalDecision]
     """
     Decisions made by various actors representing whether they think this model version should be used in production and become the new champion.
     """
     problemDefinition: MlProblemDefinition
     trainingApproach: TrainingApproach
     deployApproach: DeployApproach
+    evaluationApproach: Optional[EvaluationApproach] = None
```

### Comparing `lifeomic_patient_ml_types-7.6.1/pyproject.toml` & `lifeomic_patient_ml_types-7.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lifeomic-patient-ml-types"
-version = "7.6.1"
+version = "7.6.2"
 description = "Shared types for the patient-ml-service repos."
 authors = ["LifeOmic <development@lifeomic.com>"]
 license = "UNLICENSED"
 
 [tool.poe.tasks]
 format = "black lifeomic_patient_ml_types"
 lint = "pyright lifeomic_patient_ml_types"
```

### Comparing `lifeomic_patient_ml_types-7.6.1/setup.py` & `lifeomic_patient_ml_types-7.6.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['lifeomic_patient_ml_types']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'lifeomic-patient-ml-types',
-    'version': '7.6.1',
+    'version': '7.6.2',
     'description': 'Shared types for the patient-ml-service repos.',
     'long_description': 'None',
     'author': 'LifeOmic',
     'author_email': 'development@lifeomic.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

