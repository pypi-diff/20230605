# Comparing `tmp/mypy-boto3-finspace-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-finspace-1.26.147.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-finspace-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:26 2022, max compression
+gzip compressed data, was "mypy-boto3-finspace-1.26.147.tar", last modified: Mon Jun  5 19:33:55 2023, max compression
```

## Comparing `mypy-boto3-finspace-1.26.0.post1.tar` & `mypy-boto3-finspace-1.26.147.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:26.464829 mypy-boto3-finspace-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:34:39.000000 mypy-boto3-finspace-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    12525 2022-11-01 21:43:26.464829 mypy-boto3-finspace-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    11080 2022-11-01 21:34:39.000000 mypy-boto3-finspace-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:26.460829 mypy-boto3-finspace-1.26.0.post1/mypy_boto3_finspace/
--rw-r--r--   0 runner    (1001) docker     (121)      381 2022-11-01 21:34:39.000000 mypy-boto3-finspace-1.26.0.post1/mypy_boto3_finspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      380 2022-11-01 21:34:39.000000 mypy-boto3-finspace-1.26.0.post1/mypy_boto3_finspace/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      921 2022-11-01 21:34:39.000000 mypy-boto3-finspace-1.26.0.post1/mypy_boto3_finspace/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7829 2022-11-01 21:34:39.000000 mypy-boto3-finspace-1.26.0.post1/mypy_boto3_finspace/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     7815 2022-11-01 21:34:39.000000 mypy-boto3-finspace-1.26.0.post1/mypy_boto3_finspace/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     7274 2022-11-01 21:34:39.000000 mypy-boto3-finspace-1.26.0.post1/mypy_boto3_finspace/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     7272 2022-11-01 21:34:39.000000 mypy-boto3-finspace-1.26.0.post1/mypy_boto3_finspace/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:34:39.000000 mypy-boto3-finspace-1.26.0.post1/mypy_boto3_finspace/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     5882 2022-11-01 21:34:39.000000 mypy-boto3-finspace-1.26.0.post1/mypy_boto3_finspace/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)     5877 2022-11-01 21:34:39.000000 mypy-boto3-finspace-1.26.0.post1/mypy_boto3_finspace/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:34:39.000000 mypy-boto3-finspace-1.26.0.post1/mypy_boto3_finspace/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:26.464829 mypy-boto3-finspace-1.26.0.post1/mypy_boto3_finspace.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    12525 2022-11-01 21:43:26.000000 mypy-boto3-finspace-1.26.0.post1/mypy_boto3_finspace.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      632 2022-11-01 21:43:26.000000 mypy-boto3-finspace-1.26.0.post1/mypy_boto3_finspace.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:26.000000 mypy-boto3-finspace-1.26.0.post1/mypy_boto3_finspace.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:26.000000 mypy-boto3-finspace-1.26.0.post1/mypy_boto3_finspace.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:26.000000 mypy-boto3-finspace-1.26.0.post1/mypy_boto3_finspace.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-11-01 21:43:26.000000 mypy-boto3-finspace-1.26.0.post1/mypy_boto3_finspace.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:26.464829 mypy-boto3-finspace-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1975 2022-11-01 21:34:39.000000 mypy-boto3-finspace-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:33:55.844227 mypy-boto3-finspace-1.26.147/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-05 19:33:21.000000 mypy-boto3-finspace-1.26.147/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16081 2023-06-05 19:33:55.840227 mypy-boto3-finspace-1.26.147/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14588 2023-06-05 19:33:21.000000 mypy-boto3-finspace-1.26.147/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:33:55.832227 mypy-boto3-finspace-1.26.147/mypy_boto3_finspace/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-05 19:33:21.000000 mypy-boto3-finspace-1.26.147/mypy_boto3_finspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-05 19:33:21.000000 mypy-boto3-finspace-1.26.147/mypy_boto3_finspace/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-05 19:33:21.000000 mypy-boto3-finspace-1.26.147/mypy_boto3_finspace/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24718 2023-06-05 19:33:21.000000 mypy-boto3-finspace-1.26.147/mypy_boto3_finspace/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24676 2023-06-05 19:33:21.000000 mypy-boto3-finspace-1.26.147/mypy_boto3_finspace/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9564 2023-06-05 19:33:22.000000 mypy-boto3-finspace-1.26.147/mypy_boto3_finspace/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9562 2023-06-05 19:33:22.000000 mypy-boto3-finspace-1.26.147/mypy_boto3_finspace/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-05 19:33:22.000000 mypy-boto3-finspace-1.26.147/mypy_boto3_finspace/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-06-05 19:33:21.000000 mypy-boto3-finspace-1.26.147/mypy_boto3_finspace/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 19:33:21.000000 mypy-boto3-finspace-1.26.147/mypy_boto3_finspace/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    34873 2023-06-05 19:33:23.000000 mypy-boto3-finspace-1.26.147/mypy_boto3_finspace/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34835 2023-06-05 19:33:22.000000 mypy-boto3-finspace-1.26.147/mypy_boto3_finspace/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-05 19:33:21.000000 mypy-boto3-finspace-1.26.147/mypy_boto3_finspace/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:33:55.840227 mypy-boto3-finspace-1.26.147/mypy_boto3_finspace.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16081 2023-06-05 19:33:55.000000 mypy-boto3-finspace-1.26.147/mypy_boto3_finspace.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-05 19:33:55.000000 mypy-boto3-finspace-1.26.147/mypy_boto3_finspace.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 19:33:55.000000 mypy-boto3-finspace-1.26.147/mypy_boto3_finspace.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 19:33:55.000000 mypy-boto3-finspace-1.26.147/mypy_boto3_finspace.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-05 19:33:55.000000 mypy-boto3-finspace-1.26.147/mypy_boto3_finspace.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-05 19:33:55.000000 mypy-boto3-finspace-1.26.147/mypy_boto3_finspace.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 19:33:55.844227 mypy-boto3-finspace-1.26.147/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-05 19:33:21.000000 mypy-boto3-finspace-1.26.147/setup.py
```

### Comparing `mypy-boto3-finspace-1.26.0.post1/LICENSE` & `mypy-boto3-finspace-1.26.147/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Vlad Emelianov
+Copyright (c) 2023 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-finspace-1.26.0.post1/mypy_boto3_finspace/__main__.py` & `mypy-boto3-finspace-1.26.147/mypy_boto3_finspace/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.finspace 1.26.0\nVersion:         1.26.0.post1\nBuilder"
-        " version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.finspace 1.26.147\nVersion:         1.26.147\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.0.post1")
+    print("1.26.147")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-finspace-1.26.0.post1/mypy_boto3_finspace/literals.py` & `mypy-boto3-finspace-1.26.147/mypy_boto3_finspace/literals.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -2,50 +2,98 @@
 Type annotations for finspace service literal definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/literals/)
 
 Usage::
 
     ```python
-    from mypy_boto3_finspace.literals import EnvironmentStatusType
+    from mypy_boto3_finspace.literals import AutoScalingMetricType
 
-    data: EnvironmentStatusType = "CREATE_REQUESTED"
+    data: AutoScalingMetricType = "CPU_UTILIZATION_PERCENTAGE"
     ```
 """
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
+    "AutoScalingMetricType",
+    "ChangeTypeType",
+    "ChangesetStatusType",
     "EnvironmentStatusType",
+    "ErrorDetailsType",
     "FederationModeType",
+    "IPAddressTypeType",
+    "KxAzModeType",
+    "KxClusterStatusType",
+    "KxClusterTypeType",
+    "KxSavedownStorageTypeType",
+    "ListKxEnvironmentsPaginatorName",
+    "dnsStatusType",
+    "tgwStatusType",
     "finspaceServiceName",
     "ServiceName",
     "ResourceServiceName",
+    "PaginatorName",
     "RegionName",
 )
 
-
+AutoScalingMetricType = Literal["CPU_UTILIZATION_PERCENTAGE"]
+ChangeTypeType = Literal["DELETE", "PUT"]
+ChangesetStatusType = Literal["COMPLETED", "FAILED", "PENDING", "PROCESSING"]
 EnvironmentStatusType = Literal[
     "CREATED",
     "CREATE_REQUESTED",
     "CREATING",
     "DELETED",
     "DELETE_REQUESTED",
     "DELETING",
     "FAILED_CREATION",
     "FAILED_DELETION",
+    "FAILED_UPDATING_NETWORK",
     "RETRY_DELETION",
     "SUSPENDED",
+    "UPDATE_NETWORK_REQUESTED",
+    "UPDATING_NETWORK",
+]
+ErrorDetailsType = Literal[
+    "A user recoverable error has occurred",
+    "An internal error has occurred.",
+    "Cancelled",
+    "Missing required permission to perform this request.",
+    "One or more inputs to this request were not found.",
+    "Service limits have been exceeded.",
+    "The inputs to this request are invalid.",
+    "The system temporarily lacks sufficient resources to process the request.",
 ]
 FederationModeType = Literal["FEDERATED", "LOCAL"]
+IPAddressTypeType = Literal["IP_V4"]
+KxAzModeType = Literal["MULTI", "SINGLE"]
+KxClusterStatusType = Literal[
+    "CREATE_FAILED",
+    "CREATING",
+    "DELETED",
+    "DELETE_FAILED",
+    "DELETING",
+    "PENDING",
+    "RUNNING",
+    "UPDATING",
+]
+KxClusterTypeType = Literal["GATEWAY", "HDB", "RDB"]
+KxSavedownStorageTypeType = Literal["SDS01"]
+ListKxEnvironmentsPaginatorName = Literal["list_kx_environments"]
+dnsStatusType = Literal[
+    "FAILED_UPDATE", "NONE", "SUCCESSFULLY_UPDATED", "UPDATE_REQUESTED", "UPDATING"
+]
+tgwStatusType = Literal[
+    "FAILED_UPDATE", "NONE", "SUCCESSFULLY_UPDATED", "UPDATE_REQUESTED", "UPDATING"
+]
 finspaceServiceName = Literal["finspace"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -63,14 +111,15 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
+    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -80,27 +129,31 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
+    "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -129,14 +182,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -181,51 +235,57 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
+    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -238,14 +298,15 @@
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
+    "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
@@ -257,28 +318,33 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
+    "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
+    "osis",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -287,14 +353,15 @@
     "rds",
     "rds-data",
     "redshift",
     "redshift-data",
     "redshift-serverless",
     "rekognition",
     "resiliencehub",
+    "resource-explorer-2",
     "resource-groups",
     "resourcegroupstaggingapi",
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
@@ -305,55 +372,63 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
+    "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
+    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
+    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
@@ -371,8 +446,9 @@
     "glacier",
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
+PaginatorName = Literal["list_kx_environments"]
 RegionName = Literal["ca-central-1", "eu-west-1", "us-east-1", "us-east-2", "us-west-2"]
```

### Comparing `mypy-boto3-finspace-1.26.0.post1/mypy_boto3_finspace.egg-info/SOURCES.txt` & `mypy-boto3-finspace-1.26.147/mypy_boto3_finspace.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 mypy_boto3_finspace/__init__.py
 mypy_boto3_finspace/__init__.pyi
 mypy_boto3_finspace/__main__.py
 mypy_boto3_finspace/client.py
 mypy_boto3_finspace/client.pyi
 mypy_boto3_finspace/literals.py
 mypy_boto3_finspace/literals.pyi
+mypy_boto3_finspace/paginator.py
+mypy_boto3_finspace/paginator.pyi
 mypy_boto3_finspace/py.typed
 mypy_boto3_finspace/type_defs.py
 mypy_boto3_finspace/type_defs.pyi
 mypy_boto3_finspace/version.py
 mypy_boto3_finspace.egg-info/PKG-INFO
 mypy_boto3_finspace.egg-info/SOURCES.txt
 mypy_boto3_finspace.egg-info/dependency_links.txt
```

### Comparing `mypy-boto3-finspace-1.26.0.post1/setup.py` & `mypy-boto3-finspace-1.26.147/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-finspace.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-finspace",
-    version="1.26.0.post1",
+    version="1.26.147",
     packages=["mypy_boto3_finspace"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.finspace 1.26.0 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.finspace 1.26.147 service generated with mypy-boto3-builder"
+        " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
     keywords="boto3 finspace type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_finspace": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_finspace": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
-        "typing-extensions>=4.1.0",
+        'typing-extensions>=4.1.0; python_version<"3.9"',
     ],
     zip_safe=False,
 )
```

