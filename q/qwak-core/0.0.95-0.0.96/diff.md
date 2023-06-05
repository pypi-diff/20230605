# Comparing `tmp/qwak_core-0.0.95.tar.gz` & `tmp/qwak_core-0.0.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwak_core-0.0.95.tar", max compression
+gzip compressed data, was "qwak_core-0.0.96.tar", max compression
```

## Comparing `qwak_core-0.0.95.tar` & `qwak_core-0.0.96.tar`

### file list

```diff
@@ -1,588 +1,588 @@
--rw-r--r--   0        0        0      264 2023-06-04 15:02:32.049421 qwak_core-0.0.95/README.md
--rw-r--r--   0        0        0        0 2023-06-04 15:04:11.250141 qwak_core-0.0.95/_qwak_proto/__init__.py
--rw-r--r--   0        0        0     5378 2023-06-04 15:04:11.270141 qwak_core-0.0.95/_qwak_proto/qwak/administration/account/v1/account_pb2.py
--rw-r--r--   0        0        0     6623 2023-06-04 15:03:51.562003 qwak_core-0.0.95/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.270141 qwak_core-0.0.95/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
--rw-r--r--   0        0        0     2390 2023-06-04 15:04:11.266141 qwak_core-0.0.95/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
--rw-r--r--   0        0        0     1475 2023-06-04 15:03:51.222000 qwak_core-0.0.95/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.270141 qwak_core-0.0.95/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     2106 2023-06-04 15:04:11.270141 qwak_core-0.0.95/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
--rw-r--r--   0        0        0     1207 2023-06-04 15:03:51.390001 qwak_core-0.0.95/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.270141 qwak_core-0.0.95/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
--rw-r--r--   0        0        0     6751 2023-06-04 15:04:11.262141 qwak_core-0.0.95/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
--rw-r--r--   0        0        0     4346 2023-06-04 15:03:50.705996 qwak_core-0.0.95/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
--rw-r--r--   0        0        0     7662 2023-06-04 15:04:11.262141 qwak_core-0.0.95/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-06-04 15:04:11.262141 qwak_core-0.0.95/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
--rw-r--r--   0        0        0     2650 2023-06-04 15:03:50.881997 qwak_core-0.0.95/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.266141 qwak_core-0.0.95/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
--rw-r--r--   0        0        0     4901 2023-06-04 15:04:11.266141 qwak_core-0.0.95/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
--rw-r--r--   0        0        0     5995 2023-06-04 15:03:51.049999 qwak_core-0.0.95/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.266141 qwak_core-0.0.95/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
--rw-r--r--   0        0        0     4635 2023-06-04 15:04:11.250141 qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
--rw-r--r--   0        0        0     3664 2023-06-04 15:03:50.537995 qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
--rw-r--r--   0        0        0     3167 2023-06-04 15:04:11.250141 qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
--rw-r--r--   0        0        0     5707 2023-06-04 15:04:11.250141 qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
--rw-r--r--   0        0        0     8170 2023-06-04 15:03:51.734004 qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.254140 qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
--rw-r--r--   0        0        0     4512 2023-06-04 15:04:11.254140 qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
--rw-r--r--   0        0        0     5690 2023-06-04 15:03:52.070007 qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.258141 qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
--rw-r--r--   0        0        0    16001 2023-06-04 15:04:11.258141 qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
--rw-r--r--   0        0        0    12387 2023-06-04 15:03:52.242008 qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
--rw-r--r--   0        0        0    16458 2023-06-04 15:04:11.258141 qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2464 2023-06-04 15:04:11.254140 qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
--rw-r--r--   0        0        0     1347 2023-06-04 15:03:51.898005 qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.254140 qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     6425 2023-06-04 15:04:11.258141 qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/users/user_pb2.py
--rw-r--r--   0        0        0    10323 2023-06-04 15:03:52.414009 qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.262141 qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
--rw-r--r--   0        0        0     9577 2023-06-04 15:04:11.298141 qwak_core-0.0.95/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
--rw-r--r--   0        0        0    13624 2023-06-04 15:03:54.830027 qwak_core-0.0.95/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.298141 qwak_core-0.0.95/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
--rw-r--r--   0        0        0     9270 2023-06-04 15:04:11.298141 qwak_core-0.0.95/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
--rw-r--r--   0        0        0     5571 2023-06-04 15:03:55.010028 qwak_core-0.0.95/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
--rw-r--r--   0        0        0    10742 2023-06-04 15:04:11.302141 qwak_core-0.0.95/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
--rw-r--r--   0        0        0     7365 2023-06-04 15:04:11.370141 qwak_core-0.0.95/_qwak_proto/qwak/analytics/analytics_pb2.py
--rw-r--r--   0        0        0    11839 2023-06-04 15:04:00.370066 qwak_core-0.0.95/_qwak_proto/qwak/analytics/analytics_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.370141 qwak_core-0.0.95/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
--rw-r--r--   0        0        0     9396 2023-06-04 15:04:11.370141 qwak_core-0.0.95/_qwak_proto/qwak/analytics/analytics_service_pb2.py
--rw-r--r--   0        0        0     7896 2023-06-04 15:04:00.546067 qwak_core-0.0.95/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
--rw-r--r--   0        0        0    11917 2023-06-04 15:04:11.370141 qwak_core-0.0.95/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
--rw-r--r--   0        0        0     9021 2023-06-04 15:04:11.374141 qwak_core-0.0.95/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
--rw-r--r--   0        0        0     5865 2023-06-04 15:04:01.422073 qwak_core-0.0.95/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
--rw-r--r--   0        0        0    11486 2023-06-04 15:04:11.374141 qwak_core-0.0.95/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
--rw-r--r--   0        0        0     8807 2023-06-04 15:04:11.374141 qwak_core-0.0.95/_qwak_proto/qwak/audience/v1/audience_pb2.py
--rw-r--r--   0        0        0    13570 2023-06-04 15:04:01.246071 qwak_core-0.0.95/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.374141 qwak_core-0.0.95/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
--rw-r--r--   0        0        0     5777 2023-06-04 15:04:11.378141 qwak_core-0.0.95/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     8264 2023-06-04 15:04:01.590074 qwak_core-0.0.95/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.378141 qwak_core-0.0.95/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     2937 2023-06-04 15:04:11.378141 qwak_core-0.0.95/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
--rw-r--r--   0        0        0     2014 2023-06-04 15:04:01.758075 qwak_core-0.0.95/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
--rw-r--r--   0        0        0     2991 2023-06-04 15:04:11.378141 qwak_core-0.0.95/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
--rw-r--r--   0        0        0    12352 2023-06-04 15:04:11.462142 qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/action_pb2.py
--rw-r--r--   0        0        0    18970 2023-06-04 15:04:09.078126 qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/action_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.462142 qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
--rw-r--r--   0        0        0     5775 2023-06-04 15:04:11.458142 qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     8308 2023-06-04 15:04:08.734123 qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.458142 qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     3373 2023-06-04 15:04:11.458142 qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
--rw-r--r--   0        0        0     4400 2023-06-04 15:04:08.902124 qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.462142 qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
--rw-r--r--   0        0        0    17887 2023-06-04 15:04:11.454142 qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
--rw-r--r--   0        0        0    12310 2023-06-04 15:04:08.382121 qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
--rw-r--r--   0        0        0    23338 2023-06-04 15:04:11.454142 qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
--rw-r--r--   0        0        0     3873 2023-06-04 15:04:11.454142 qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/automation_pb2.py
--rw-r--r--   0        0        0     5291 2023-06-04 15:04:08.562122 qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.458142 qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
--rw-r--r--   0        0        0     2383 2023-06-04 15:04:11.466142 qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/common_pb2.py
--rw-r--r--   0        0        0     2446 2023-06-04 15:04:09.590129 qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/common_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.466142 qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
--rw-r--r--   0        0        0     5209 2023-06-04 15:04:11.466142 qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/notification_pb2.py
--rw-r--r--   0        0        0     5492 2023-06-04 15:04:09.418128 qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.466142 qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
--rw-r--r--   0        0        0     4210 2023-06-04 15:04:11.462142 qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/trigger_pb2.py
--rw-r--r--   0        0        0     4746 2023-06-04 15:04:09.250127 qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.466142 qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
--rw-r--r--   0        0        0    10989 2023-06-04 15:04:11.450142 qwak_core-0.0.95/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
--rw-r--r--   0        0        0    15193 2023-06-04 15:04:08.202119 qwak_core-0.0.95/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.454142 qwak_core-0.0.95/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
--rw-r--r--   0        0        0     2042 2023-06-04 15:04:11.446142 qwak_core-0.0.95/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
--rw-r--r--   0        0        0     1904 2023-06-04 15:04:07.850117 qwak_core-0.0.95/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.450142 qwak_core-0.0.95/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
--rw-r--r--   0        0        0    44118 2023-06-04 15:04:11.450142 qwak_core-0.0.95/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
--rw-r--r--   0        0        0    58036 2023-06-04 15:04:08.030118 qwak_core-0.0.95/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
--rw-r--r--   0        0        0    29918 2023-06-04 15:04:11.450142 qwak_core-0.0.95/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
--rw-r--r--   0        0        0    20255 2023-06-04 15:04:11.402142 qwak_core-0.0.95/_qwak_proto/qwak/build/v1/build_api_pb2.py
--rw-r--r--   0        0        0    17495 2023-06-04 15:04:03.514087 qwak_core-0.0.95/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
--rw-r--r--   0        0        0    20359 2023-06-04 15:04:11.402142 qwak_core-0.0.95/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
--rw-r--r--   0        0        0    16953 2023-06-04 15:04:11.402142 qwak_core-0.0.95/_qwak_proto/qwak/build/v1/build_pb2.py
--rw-r--r--   0        0        0    25941 2023-06-04 15:04:03.342086 qwak_core-0.0.95/_qwak_proto/qwak/build/v1/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.402142 qwak_core-0.0.95/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
--rw-r--r--   0        0        0    11691 2023-06-04 15:04:11.394142 qwak_core-0.0.95/_qwak_proto/qwak/builds/build_pb2.py
--rw-r--r--   0        0        0    18850 2023-06-04 15:04:02.998084 qwak_core-0.0.95/_qwak_proto/qwak/builds/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.394142 qwak_core-0.0.95/_qwak_proto/qwak/builds/build_pb2_grpc.py
--rw-r--r--   0        0        0     4777 2023-06-04 15:04:11.394142 qwak_core-0.0.95/_qwak_proto/qwak/builds/build_url_pb2.py
--rw-r--r--   0        0        0     5773 2023-06-04 15:04:03.166085 qwak_core-0.0.95/_qwak_proto/qwak/builds/build_url_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.394142 qwak_core-0.0.95/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
--rw-r--r--   0        0        0    12490 2023-06-04 15:04:11.394142 qwak_core-0.0.95/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
--rw-r--r--   0        0        0     9351 2023-06-04 15:04:03.690088 qwak_core-0.0.95/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
--rw-r--r--   0        0        0    14916 2023-06-04 15:04:11.398141 qwak_core-0.0.95/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
--rw-r--r--   0        0        0    38290 2023-06-04 15:04:11.398141 qwak_core-0.0.95/_qwak_proto/qwak/builds/builds_pb2.py
--rw-r--r--   0        0        0    52702 2023-06-04 15:04:04.062091 qwak_core-0.0.95/_qwak_proto/qwak/builds/builds_pb2.pyi
--rw-r--r--   0        0        0    11572 2023-06-04 15:04:11.398141 qwak_core-0.0.95/_qwak_proto/qwak/builds/builds_pb2_grpc.py
--rw-r--r--   0        0        0     1671 2023-06-04 15:04:11.410142 qwak_core-0.0.95/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
--rw-r--r--   0        0        0     1689 2023-06-04 15:04:04.418093 qwak_core-0.0.95/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.410142 qwak_core-0.0.95/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4328 2023-06-04 15:04:11.410142 qwak_core-0.0.95/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-06-04 15:04:04.586094 qwak_core-0.0.95/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-06-04 15:04:11.410142 qwak_core-0.0.95/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     7716 2023-06-04 15:04:11.386141 qwak_core-0.0.95/_qwak_proto/qwak/deployment/alert_pb2.py
--rw-r--r--   0        0        0    11197 2023-06-04 15:04:02.474080 qwak_core-0.0.95/_qwak_proto/qwak/deployment/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.386141 qwak_core-0.0.95/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
--rw-r--r--   0        0        0    11580 2023-06-04 15:04:11.390142 qwak_core-0.0.95/_qwak_proto/qwak/deployment/alert_service_pb2.py
--rw-r--r--   0        0        0     7373 2023-06-04 15:04:02.646081 qwak_core-0.0.95/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
--rw-r--r--   0        0        0    12803 2023-06-04 15:04:11.390142 qwak_core-0.0.95/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
--rw-r--r--   0        0        0     2162 2023-06-04 15:04:11.382141 qwak_core-0.0.95/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
--rw-r--r--   0        0        0     2685 2023-06-04 15:04:02.122078 qwak_core-0.0.95/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.382141 qwak_core-0.0.95/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
--rw-r--r--   0        0        0    43712 2023-06-04 15:04:11.382141 qwak_core-0.0.95/_qwak_proto/qwak/deployment/deployment_pb2.py
--rw-r--r--   0        0        0    63341 2023-06-04 15:04:01.946076 qwak_core-0.0.95/_qwak_proto/qwak/deployment/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.382141 qwak_core-0.0.95/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    38320 2023-06-04 15:04:11.386141 qwak_core-0.0.95/_qwak_proto/qwak/deployment/deployment_service_pb2.py
--rw-r--r--   0        0        0    33325 2023-06-04 15:04:02.306079 qwak_core-0.0.95/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
--rw-r--r--   0        0        0    20242 2023-06-04 15:04:11.386141 qwak_core-0.0.95/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2527 2023-06-04 15:04:11.290141 qwak_core-0.0.95/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
--rw-r--r--   0        0        0     2791 2023-06-04 15:03:53.962021 qwak_core-0.0.95/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.290141 qwak_core-0.0.95/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-06-04 15:04:11.290141 qwak_core-0.0.95/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
--rw-r--r--   0        0        0    12641 2023-06-04 15:03:54.134022 qwak_core-0.0.95/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.290141 qwak_core-0.0.95/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
--rw-r--r--   0        0        0    16366 2023-06-04 15:04:11.294141 qwak_core-0.0.95/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
--rw-r--r--   0        0        0    17148 2023-06-04 15:03:54.314024 qwak_core-0.0.95/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
--rw-r--r--   0        0        0    10706 2023-06-04 15:04:11.294141 qwak_core-0.0.95/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
--rw-r--r--   0        0        0     4787 2023-06-04 15:04:11.350141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
--rw-r--r--   0        0        0     6713 2023-06-04 15:03:59.322058 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.350141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
--rw-r--r--   0        0        0     9721 2023-06-04 15:04:11.350141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
--rw-r--r--   0        0        0     7409 2023-06-04 15:03:59.150057 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
--rw-r--r--   0        0        0    12256 2023-06-04 15:04:11.350141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
--rw-r--r--   0        0        0    11432 2023-06-04 15:04:11.326141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
--rw-r--r--   0        0        0    12882 2023-06-04 15:03:57.230044 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.326141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
--rw-r--r--   0        0        0     5303 2023-06-04 15:04:11.322141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/execution_pb2.py
--rw-r--r--   0        0        0     8604 2023-06-04 15:03:57.054043 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.326141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
--rw-r--r--   0        0        0    10074 2023-06-04 15:04:11.318141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
--rw-r--r--   0        0        0    14303 2023-06-04 15:03:56.514039 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.318141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
--rw-r--r--   0        0        0    28920 2023-06-04 15:04:11.322141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
--rw-r--r--   0        0        0    20665 2023-06-04 15:03:56.882041 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
--rw-r--r--   0        0        0    35307 2023-06-04 15:04:11.322141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
--rw-r--r--   0        0        0    12638 2023-06-04 15:04:11.326141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
--rw-r--r--   0        0        0    14071 2023-06-04 15:03:57.406045 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.330141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
--rw-r--r--   0        0        0    10044 2023-06-04 15:04:11.330141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
--rw-r--r--   0        0        0     6846 2023-06-04 15:03:57.578046 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
--rw-r--r--   0        0        0    11647 2023-06-04 15:04:11.330141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
--rw-r--r--   0        0        0    25269 2023-06-04 15:04:11.318141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
--rw-r--r--   0        0        0    37664 2023-06-04 15:03:56.694040 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.322141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
--rw-r--r--   0        0        0     2872 2023-06-04 15:04:11.330141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
--rw-r--r--   0        0        0     2428 2023-06-04 15:03:57.746047 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.334141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
--rw-r--r--   0        0        0    10202 2023-06-04 15:04:11.334141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_pb2.py
--rw-r--r--   0        0        0    16565 2023-06-04 15:03:58.098050 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.338141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_pb2_grpc.py
--rw-r--r--   0        0        0     3559 2023-06-04 15:04:11.338141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2.py
--rw-r--r--   0        0        0     1759 2023-06-04 15:03:58.274051 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2.pyi
--rw-r--r--   0        0        0     3608 2023-06-04 15:04:11.338141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2_grpc.py
--rw-r--r--   0        0        0    10604 2023-06-04 15:04:11.334141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py
--rw-r--r--   0        0        0    13410 2023-06-04 15:03:57.922049 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.334141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2_grpc.py
--rw-r--r--   0        0        0     4196 2023-06-04 15:04:11.354141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
--rw-r--r--   0        0        0     7323 2023-06-04 15:04:10.822138 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.354141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
--rw-r--r--   0        0        0     9895 2023-06-04 15:04:11.354141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
--rw-r--r--   0        0        0     9029 2023-06-04 15:04:10.998139 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
--rw-r--r--   0        0        0    12090 2023-06-04 15:04:11.354141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     3596 2023-06-04 15:04:11.358141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
--rw-r--r--   0        0        0     6664 2023-06-04 15:03:59.850062 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.358141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
--rw-r--r--   0        0        0    11930 2023-06-04 15:04:11.358141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
--rw-r--r--   0        0        0    11052 2023-06-04 15:04:00.026063 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
--rw-r--r--   0        0        0    14459 2023-06-04 15:04:11.358141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     5158 2023-06-04 15:04:11.362141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/reports/report_pb2.py
--rw-r--r--   0        0        0     7436 2023-06-04 15:04:00.198064 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.362141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
--rw-r--r--   0        0        0     4549 2023-06-04 15:04:11.366141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
--rw-r--r--   0        0        0     6442 2023-06-04 15:04:00.902069 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.366141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
--rw-r--r--   0        0        0    16693 2023-06-04 15:04:11.362141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
--rw-r--r--   0        0        0    20355 2023-06-04 15:04:00.722068 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
--rw-r--r--   0        0        0     4809 2023-06-04 15:04:11.362141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
--rw-r--r--   0        0        0     2553 2023-06-04 15:04:11.366141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
--rw-r--r--   0        0        0     4000 2023-06-04 15:04:01.074070 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.366141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
--rw-r--r--   0        0        0    14046 2023-06-04 15:04:11.342141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
--rw-r--r--   0        0        0    23615 2023-06-04 15:03:58.450052 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.342141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
--rw-r--r--   0        0        0     5087 2023-06-04 15:04:11.342141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
--rw-r--r--   0        0        0     6011 2023-06-04 15:03:58.622053 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.342141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
--rw-r--r--   0        0        0    12309 2023-06-04 15:04:11.346141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
--rw-r--r--   0        0        0     9244 2023-06-04 15:03:58.798055 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
--rw-r--r--   0        0        0    17071 2023-06-04 15:04:11.346141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
--rw-r--r--   0        0        0    11014 2023-06-04 15:04:11.346141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
--rw-r--r--   0        0        0    15865 2023-06-04 15:03:58.974056 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.346141 qwak_core-0.0.95/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
--rw-r--r--   0        0        0     4727 2023-06-04 15:04:11.470142 qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
--rw-r--r--   0        0        0     5122 2023-06-04 15:04:09.758130 qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.470142 qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4648 2023-06-04 15:04:11.470142 qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4170 2023-06-04 15:04:09.946132 qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-06-04 15:04:11.470142 qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     5349 2023-06-04 15:04:11.474142 qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
--rw-r--r--   0        0        0     5363 2023-06-04 15:04:10.114133 qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.474142 qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4437 2023-06-04 15:04:11.474142 qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4127 2023-06-04 15:04:10.298134 qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-06-04 15:04:11.474142 qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     6073 2023-06-04 15:04:11.478142 qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
--rw-r--r--   0        0        0     5366 2023-06-04 15:04:10.478135 qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
--rw-r--r--   0        0        0     7395 2023-06-04 15:04:11.478142 qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
--rw-r--r--   0        0        0     4636 2023-06-04 15:04:11.478142 qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
--rw-r--r--   0        0        0     4239 2023-06-04 15:04:10.650136 qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.478142 qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     2376 2023-06-04 15:04:11.414142 qwak_core-0.0.95/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
--rw-r--r--   0        0        0     3018 2023-06-04 15:04:04.754096 qwak_core-0.0.95/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.414142 qwak_core-0.0.95/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4325 2023-06-04 15:04:11.414142 qwak_core-0.0.95/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-06-04 15:04:04.922097 qwak_core-0.0.95/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-06-04 15:04:11.414142 qwak_core-0.0.95/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     6401 2023-06-04 15:04:11.302141 qwak_core-0.0.95/_qwak_proto/qwak/fitness_service/constructs_pb2.py
--rw-r--r--   0        0        0    10192 2023-06-04 15:03:55.810034 qwak_core-0.0.95/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.306141 qwak_core-0.0.95/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-06-04 15:04:11.306141 qwak_core-0.0.95/_qwak_proto/qwak/fitness_service/fitness_pb2.py
--rw-r--r--   0        0        0     4115 2023-06-04 15:03:55.982035 qwak_core-0.0.95/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.310141 qwak_core-0.0.95/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
--rw-r--r--   0        0        0     7123 2023-06-04 15:04:11.310141 qwak_core-0.0.95/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
--rw-r--r--   0        0        0     3981 2023-06-04 15:03:56.158036 qwak_core-0.0.95/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
--rw-r--r--   0        0        0     8546 2023-06-04 15:04:11.314141 qwak_core-0.0.95/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
--rw-r--r--   0        0        0     8428 2023-06-04 15:04:11.314141 qwak_core-0.0.95/_qwak_proto/qwak/fitness_service/status_pb2.py
--rw-r--r--   0        0        0    12205 2023-06-04 15:03:56.330037 qwak_core-0.0.95/_qwak_proto/qwak/fitness_service/status_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.318141 qwak_core-0.0.95/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
--rw-r--r--   0        0        0     8196 2023-06-04 15:04:11.390142 qwak_core-0.0.95/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
--rw-r--r--   0        0        0    10867 2023-06-04 15:04:02.822082 qwak_core-0.0.95/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
--rw-r--r--   0        0        0     4700 2023-06-04 15:04:11.390142 qwak_core-0.0.95/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
--rw-r--r--   0        0        0     3757 2023-06-04 15:04:11.414142 qwak_core-0.0.95/_qwak_proto/qwak/instance_template/instance_template_pb2.py
--rw-r--r--   0        0        0     4235 2023-06-04 15:04:05.094098 qwak_core-0.0.95/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.418142 qwak_core-0.0.95/_qwak_proto/qwak/instance_template/instance_template_pb2_grpc.py
--rw-r--r--   0        0        0     4722 2023-06-04 15:04:11.418142 qwak_core-0.0.95/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py
--rw-r--r--   0        0        0     3245 2023-06-04 15:04:05.262099 qwak_core-0.0.95/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi
--rw-r--r--   0        0        0     5240 2023-06-04 15:04:11.418142 qwak_core-0.0.95/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py
--rw-r--r--   0        0        0     7803 2023-06-04 15:04:11.430142 qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
--rw-r--r--   0        0        0    10487 2023-06-04 15:04:06.286106 qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.430142 qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
--rw-r--r--   0        0        0     3704 2023-06-04 15:04:11.430142 qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
--rw-r--r--   0        0        0     3759 2023-06-04 15:04:06.454107 qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.434142 qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
--rw-r--r--   0        0        0    22089 2023-06-04 15:04:11.434142 qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
--rw-r--r--   0        0        0    25879 2023-06-04 15:04:06.630109 qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.434142 qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
--rw-r--r--   0        0        0    13157 2023-06-04 15:04:11.434142 qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
--rw-r--r--   0        0        0    21705 2023-06-04 15:04:06.802110 qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.438142 qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-06-04 15:04:11.438142 qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
--rw-r--r--   0        0        0    16128 2023-06-04 15:04:06.982111 qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.438142 qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
--rw-r--r--   0        0        0    45273 2023-06-04 15:04:11.438142 qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
--rw-r--r--   0        0        0    35031 2023-06-04 15:04:07.170112 qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
--rw-r--r--   0        0        0    67567 2023-06-04 15:04:11.442142 qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
--rw-r--r--   0        0        0     2411 2023-06-04 15:04:11.442142 qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
--rw-r--r--   0        0        0     2637 2023-06-04 15:04:07.342114 qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.442142 qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
--rw-r--r--   0        0        0     3459 2023-06-04 15:04:11.422142 qwak_core-0.0.95/_qwak_proto/qwak/logging/log_filter_pb2.py
--rw-r--r--   0        0        0     4169 2023-06-04 15:04:05.602102 qwak_core-0.0.95/_qwak_proto/qwak/logging/log_filter_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.422142 qwak_core-0.0.95/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
--rw-r--r--   0        0        0     2233 2023-06-04 15:04:11.426142 qwak_core-0.0.95/_qwak_proto/qwak/logging/log_line_pb2.py
--rw-r--r--   0        0        0     2135 2023-06-04 15:04:06.114105 qwak_core-0.0.95/_qwak_proto/qwak/logging/log_line_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.430142 qwak_core-0.0.95/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
--rw-r--r--   0        0        0     3126 2023-06-04 15:04:11.422142 qwak_core-0.0.95/_qwak_proto/qwak/logging/log_reader_service_pb2.py
--rw-r--r--   0        0        0     3479 2023-06-04 15:04:05.770103 qwak_core-0.0.95/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
--rw-r--r--   0        0        0     2831 2023-06-04 15:04:11.426142 qwak_core-0.0.95/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
--rw-r--r--   0        0        0    10138 2023-06-04 15:04:11.426142 qwak_core-0.0.95/_qwak_proto/qwak/logging/log_source_pb2.py
--rw-r--r--   0        0        0    14337 2023-06-04 15:04:05.942104 qwak_core-0.0.95/_qwak_proto/qwak/logging/log_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.426142 qwak_core-0.0.95/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
--rw-r--r--   0        0        0    22744 2023-06-04 15:04:11.406142 qwak_core-0.0.95/_qwak_proto/qwak/models/models_pb2.py
--rw-r--r--   0        0        0    27142 2023-06-04 15:04:04.250092 qwak_core-0.0.95/_qwak_proto/qwak/models/models_pb2.pyi
--rw-r--r--   0        0        0    14733 2023-06-04 15:04:11.406142 qwak_core-0.0.95/_qwak_proto/qwak/models/models_pb2_grpc.py
--rw-r--r--   0        0        0    10745 2023-06-04 15:04:11.286141 qwak_core-0.0.95/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
--rw-r--r--   0        0        0     6790 2023-06-04 15:03:55.418031 qwak_core-0.0.95/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
--rw-r--r--   0        0        0    13657 2023-06-04 15:04:11.286141 qwak_core-0.0.95/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
--rw-r--r--   0        0        0    11564 2023-06-04 15:04:11.282141 qwak_core-0.0.95/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
--rw-r--r--   0        0        0    14927 2023-06-04 15:03:55.206030 qwak_core-0.0.95/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.282141 qwak_core-0.0.95/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
--rw-r--r--   0        0        0     5283 2023-06-04 15:04:11.286141 qwak_core-0.0.95/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
--rw-r--r--   0        0        0     3745 2023-06-04 15:03:55.626033 qwak_core-0.0.95/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
--rw-r--r--   0        0        0     5551 2023-06-04 15:04:11.286141 qwak_core-0.0.95/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
--rw-r--r--   0        0        0     8701 2023-06-04 15:04:11.406142 qwak_core-0.0.95/_qwak_proto/qwak/projects/projects_pb2.py
--rw-r--r--   0        0        0     9794 2023-06-04 15:04:03.874090 qwak_core-0.0.95/_qwak_proto/qwak/projects/projects_pb2.pyi
--rw-r--r--   0        0        0     7931 2023-06-04 15:04:11.406142 qwak_core-0.0.95/_qwak_proto/qwak/projects/projects_pb2_grpc.py
--rw-r--r--   0        0        0     4752 2023-06-04 15:04:11.418142 qwak_core-0.0.95/_qwak_proto/qwak/secret_service/secret_service_pb2.py
--rw-r--r--   0        0        0     2818 2023-06-04 15:04:05.434100 qwak_core-0.0.95/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
--rw-r--r--   0        0        0     6253 2023-06-04 15:04:11.422142 qwak_core-0.0.95/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
--rw-r--r--   0        0        0     6225 2023-06-04 15:04:11.282141 qwak_core-0.0.95/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
--rw-r--r--   0        0        0     7267 2023-06-04 15:03:53.278016 qwak_core-0.0.95/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.282141 qwak_core-0.0.95/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
--rw-r--r--   0        0        0    16176 2023-06-04 15:04:11.278141 qwak_core-0.0.95/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
--rw-r--r--   0        0        0    10166 2023-06-04 15:03:53.106015 qwak_core-0.0.95/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
--rw-r--r--   0        0        0    19988 2023-06-04 15:04:11.278141 qwak_core-0.0.95/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
--rw-r--r--   0        0        0     1751 2023-06-04 15:04:11.274141 qwak_core-0.0.95/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
--rw-r--r--   0        0        0      777 2023-06-04 15:03:52.582011 qwak_core-0.0.95/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.274141 qwak_core-0.0.95/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
--rw-r--r--   0        0        0     2392 2023-06-04 15:04:11.274141 qwak_core-0.0.95/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
--rw-r--r--   0        0        0     2129 2023-06-04 15:03:52.758012 qwak_core-0.0.95/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.274141 qwak_core-0.0.95/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
--rw-r--r--   0        0        0    10389 2023-06-04 15:04:11.278141 qwak_core-0.0.95/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
--rw-r--r--   0        0        0     8148 2023-06-04 15:03:52.930014 qwak_core-0.0.95/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
--rw-r--r--   0        0        0    10512 2023-06-04 15:04:11.278141 qwak_core-0.0.95/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
--rw-r--r--   0        0        0     6843 2023-06-04 15:04:11.446142 qwak_core-0.0.95/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
--rw-r--r--   0        0        0     4585 2023-06-04 15:04:07.682116 qwak_core-0.0.95/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
--rw-r--r--   0        0        0     8228 2023-06-04 15:04:11.446142 qwak_core-0.0.95/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
--rw-r--r--   0        0        0     7816 2023-06-04 15:04:11.442142 qwak_core-0.0.95/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
--rw-r--r--   0        0        0    11958 2023-06-04 15:04:07.510115 qwak_core-0.0.95/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.446142 qwak_core-0.0.95/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
--rw-r--r--   0        0        0    10961 2023-06-04 15:04:11.294141 qwak_core-0.0.95/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
--rw-r--r--   0        0        0    14256 2023-06-04 15:03:54.486025 qwak_core-0.0.95/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.294141 qwak_core-0.0.95/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
--rw-r--r--   0        0        0     3072 2023-06-04 15:04:11.298141 qwak_core-0.0.95/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
--rw-r--r--   0        0        0     2663 2023-06-04 15:03:54.658026 qwak_core-0.0.95/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-04 15:04:11.298141 qwak_core-0.0.95/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
--rw-r--r--   0        0        0     2661 2023-06-04 15:04:12.946152 qwak_core-0.0.95/pyproject.toml
--rw-r--r--   0        0        0      447 2023-06-04 15:04:12.946152 qwak_core-0.0.95/qwak/__init__.py
--rw-r--r--   0        0        0     1501 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/automations/__init__.py
--rw-r--r--   0        0        0     3132 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/automations/automation_executions.py
--rw-r--r--   0        0        0    12899 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/automations/automations.py
--rw-r--r--   0        0        0     9638 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/automations/batch_execution_action.py
--rw-r--r--   0        0        0    19120 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/automations/build_and_deploy_action.py
--rw-r--r--   0        0        0     1697 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/automations/common.py
--rw-r--r--   0        0        0        0 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/__init__.py
--rw-r--r--   0        0        0      224 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/administration/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/administration/authenticated_user/__init__.py
--rw-r--r--   0        0        0     1456 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/administration/authenticated_user/client.py
--rw-r--r--   0        0        0        0 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/administration/authentication/__init__.py
--rw-r--r--   0        0        0     1076 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/administration/authentication/client.py
--rw-r--r--   0        0        0        0 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/administration/eco_system/__init__.py
--rw-r--r--   0        0        0     5362 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/administration/eco_system/client.py
--rw-r--r--   0        0        0        0 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/administration/environment/__init__.py
--rw-r--r--   0        0        0     2704 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/administration/environment/client.py
--rw-r--r--   0        0        0        0 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/administration/self_service/__init__.py
--rw-r--r--   0        0        0     2602 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/administration/self_service/client.py
--rw-r--r--   0        0        0       43 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/alert_management/__init__.py
--rw-r--r--   0        0        0     2226 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/alert_management/client.py
--rw-r--r--   0        0        0       42 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/analytics/__init__.py
--rw-r--r--   0        0        0     3093 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/analytics/client.py
--rw-r--r--   0        0        0       35 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/audience/__init__.py
--rw-r--r--   0        0        0     2110 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/audience/client.py
--rw-r--r--   0        0        0        0 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/automation_management/__init__.py
--rw-r--r--   0        0        0     8836 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/automation_management/client.py
--rw-r--r--   0        0        0       38 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/autoscaling/__init__.py
--rw-r--r--   0        0        0     1240 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/autoscaling/client.py
--rw-r--r--   0        0        0      211 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/batch_job_management/__init__.py
--rw-r--r--   0        0        0    18388 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/batch_job_management/client.py
--rw-r--r--   0        0        0     6242 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/batch_job_management/executions_config.py
--rw-r--r--   0        0        0     1846 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/batch_job_management/results.py
--rw-r--r--   0        0        0       43 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/build_management/__init__.py
--rw-r--r--   0        0        0     4731 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/build_management/client.py
--rw-r--r--   0        0        0       44 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/build_orchestrator/__init__.py
--rw-r--r--   0        0        0    15319 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/build_orchestrator/client.py
--rw-r--r--   0        0        0        0 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/data_versioning/__init__.py
--rw-r--r--   0        0        0     1835 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/data_versioning/client.py
--rw-r--r--   0        0        0        0 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/deployment/__init__.py
--rw-r--r--   0        0        0     6269 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/deployment/client.py
--rw-r--r--   0        0        0       53 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/feature_store/__init__.py
--rw-r--r--   0        0        0     2635 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/feature_store/job_registry_client.py
--rw-r--r--   0        0        0    15898 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/feature_store/management_client.py
--rw-r--r--   0        0        0     4963 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/feature_store/operator_client.py
--rw-r--r--   0        0        0        0 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/file_versioning/__init__.py
--rw-r--r--   0        0        0     1939 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/file_versioning/client.py
--rw-r--r--   0        0        0        0 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/instance_template/__init__.py
--rw-r--r--   0        0        0     2495 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/instance_template/client.py
--rw-r--r--   0        0        0       41 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/kube_deployment_captain/__init__.py
--rw-r--r--   0        0        0     9276 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/kube_deployment_captain/client.py
--rw-r--r--   0        0        0       34 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/logging_client/__init__.py
--rw-r--r--   0        0        0     4906 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/logging_client/client.py
--rw-r--r--   0        0        0       43 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/model_management/__init__.py
--rw-r--r--   0        0        0     3695 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/model_management/client.py
--rw-r--r--   0        0        0        0 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/project/__init__.py
--rw-r--r--   0        0        0     2128 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/project/client.py
--rw-r--r--   0        0        0       40 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/secret_service/__init__.py
--rw-r--r--   0        0        0     3316 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/secret_service/client.py
--rw-r--r--   0        0        0       50 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/user_application_instance/__init__.py
--rw-r--r--   0        0        0     6013 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/clients/user_application_instance/client.py
--rw-r--r--   0        0        0      380 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/exceptions/__init__.py
--rw-r--r--   0        0        0      559 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/exceptions/quiet_error.py
--rw-r--r--   0        0        0      469 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/exceptions/qwak_build_exception.py
--rw-r--r--   0        0        0      135 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/exceptions/qwak_exception.py
--rw-r--r--   0        0        0      579 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/exceptions/qwak_http_exception.py
--rw-r--r--   0        0        0      100 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/exceptions/qwak_inference_exception.py
--rw-r--r--   0        0        0      274 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/exceptions/qwak_load_model_failed_exception.py
--rw-r--r--   0        0        0      211 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/exceptions/qwak_login_exception.py
--rw-r--r--   0        0        0      152 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/exceptions/qwak_mock_http_exception.py
--rw-r--r--   0        0        0      153 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/exceptions/qwak_model_initialization_exception.py
--rw-r--r--   0        0        0      152 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/exceptions/qwak_not_found_exception.py
--rw-r--r--   0        0        0      356 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/exceptions/qwak_quiet_build_exception.py
--rw-r--r--   0        0        0        0 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/_common/__init__.py
--rw-r--r--   0        0        0     4707 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/_common/featureset_asterisk_handler.py
--rw-r--r--   0        0        0     1298 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/_common/functions.py
--rw-r--r--   0        0        0     1263 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/data_sources/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/data_sources/batch_sources/__init__.py
--rw-r--r--   0        0        0     2108 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/data_sources/batch_sources/_batch.py
--rw-r--r--   0        0        0      666 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/data_sources/batch_sources/_jdbc.py
--rw-r--r--   0        0        0     3059 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/data_sources/batch_sources/big_query.py
--rw-r--r--   0        0        0     1941 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/data_sources/batch_sources/csv.py
--rw-r--r--   0        0        0     2167 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/data_sources/batch_sources/elastic_search.py
--rw-r--r--   0        0        0     2987 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
--rw-r--r--   0        0        0     1930 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/data_sources/batch_sources/mongodb.py
--rw-r--r--   0        0        0     1669 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/data_sources/batch_sources/mysql.py
--rw-r--r--   0        0        0     1717 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/data_sources/batch_sources/parquet.py
--rw-r--r--   0        0        0     1722 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/data_sources/batch_sources/postgres.py
--rw-r--r--   0        0        0     3216 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/data_sources/batch_sources/redshift.py
--rw-r--r--   0        0        0     2616 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/data_sources/batch_sources/snowflake.py
--rw-r--r--   0        0        0     1839 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/data_sources/batch_sources/vertica.py
--rw-r--r--   0        0        0        0 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/entities/__init__.py
--rw-r--r--   0        0        0     1794 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/entities/entity.py
--rw-r--r--   0        0        0        0 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/feature_sets/__init__.py
--rw-r--r--   0        0        0     1547 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/feature_sets/backfill.py
--rw-r--r--   0        0        0    17012 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/feature_sets/batch.py
--rw-r--r--   0        0        0      263 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/feature_sets/context.py
--rw-r--r--   0        0        0     1630 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/feature_sets/execution_spec.py
--rw-r--r--   0        0        0      584 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/feature_sets/metadata.py
--rw-r--r--   0        0        0     6820 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/feature_sets/read_policies.py
--rw-r--r--   0        0        0     1554 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/feature_sets/transformations.py
--rw-r--r--   0        0        0       89 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/offline/__init__.py
--rw-r--r--   0        0        0      738 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/offline/_query_engine.py
--rw-r--r--   0        0        0        0 2023-06-04 15:02:32.053421 qwak_core-0.0.95/qwak/feature_store/offline/athena/__init__.py
--rw-r--r--   0        0        0     5182 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/feature_store/offline/athena/athena_query_engine.py
--rw-r--r--   0        0        0    28013 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/feature_store/offline/client.py
--rw-r--r--   0        0        0        0 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/feature_store/online/__init__.py
--rw-r--r--   0        0        0     9261 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/feature_store/online/client.py
--rw-r--r--   0        0        0      226 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/inner/__init__.py
--rw-r--r--   0        0        0      954 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/inner/const.py
--rw-r--r--   0        0        0     1435 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/inner/di_configuration/__init__.py
--rw-r--r--   0        0        0     4768 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/inner/di_configuration/account.py
--rw-r--r--   0        0        0       73 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/inner/di_configuration/config.yml
--rw-r--r--   0        0        0      621 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/inner/di_configuration/containers.py
--rw-r--r--   0        0        0      344 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/inner/di_configuration/session.py
--rw-r--r--   0        0        0     2336 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/inner/model_loggers_utils.py
--rw-r--r--   0        0        0      266 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/inner/runtime_di/__init__.py
--rw-r--r--   0        0        0      349 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/inner/runtime_di/containers.py
--rw-r--r--   0        0        0      627 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/inner/singleton_meta.py
--rw-r--r--   0        0        0       74 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/inner/tool/__init__.py
--rw-r--r--   0        0        0     3414 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/inner/tool/auth.py
--rw-r--r--   0        0        0        0 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/inner/tool/grpc/__init__.py
--rw-r--r--   0        0        0      560 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/inner/tool/grpc/grpc_auth.py
--rw-r--r--   0        0        0     5804 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/inner/tool/grpc/grpc_tools.py
--rw-r--r--   0        0        0      473 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/inner/tool/grpc/grpc_try_wrapping.py
--rw-r--r--   0        0        0      435 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/inner/tool/retry_utils.py
--rw-r--r--   0        0        0      218 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/inner/tool/run_config/__init__.py
--rw-r--r--   0        0        0     3148 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/inner/tool/run_config/base.py
--rw-r--r--   0        0        0     6083 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/inner/tool/run_config/utils.py
--rw-r--r--   0        0        0        0 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/__init__.py
--rw-r--r--   0        0        0     1739 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/adapters/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      198 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/adapters/input_adapters/base_input_adapter.py
--rw-r--r--   0        0        0      210 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
--rw-r--r--   0        0        0      205 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/adapters/input_adapters/file_input_adapter.py
--rw-r--r--   0        0        0      206 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/adapters/input_adapters/image_input_adapter.py
--rw-r--r--   0        0        0      205 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/adapters/input_adapters/json_input_adapter.py
--rw-r--r--   0        0        0     2175 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/adapters/input_adapters/multi_input_adapter.py
--rw-r--r--   0        0        0     3208 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/adapters/input_adapters/numpy_input_adapter.py
--rw-r--r--   0        0        0      862 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/adapters/input_adapters/proto_input_adapter.py
--rw-r--r--   0        0        0      207 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/adapters/input_adapters/string_input_adapter.py
--rw-r--r--   0        0        0      209 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
--rw-r--r--   0        0        0        0 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      315 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/adapters/output_adapters/base_output_adapter.py
--rw-r--r--   0        0        0      221 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
--rw-r--r--   0        0        0      219 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/adapters/output_adapters/default_output_adapter.py
--rw-r--r--   0        0        0      216 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/adapters/output_adapters/json_output_adapter.py
--rw-r--r--   0        0        0     1065 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/adapters/output_adapters/numpy_output_adapter.py
--rw-r--r--   0        0        0      517 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/adapters/output_adapters/proto_output_adapter.py
--rw-r--r--   0        0        0      115 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
--rw-r--r--   0        0        0      220 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
--rw-r--r--   0        0        0      303 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/analytics_logging.py
--rw-r--r--   0        0        0     2825 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/base.py
--rw-r--r--   0        0        0        0 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/decorators/__init__.py
--rw-r--r--   0        0        0     1288 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/decorators/api.py
--rw-r--r--   0        0        0      861 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/decorators/api_implementation.py
--rw-r--r--   0        0        0     1503 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/experiment_tracking.py
--rw-r--r--   0        0        0      873 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/schema.py
--rw-r--r--   0        0        0     2970 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/schema_entities.py
--rw-r--r--   0        0        0      338 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/tools/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/tools/adapters/__init__.py
--rw-r--r--   0        0        0     1193 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/tools/adapters/encoders.py
--rw-r--r--   0        0        0     1963 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/tools/adapters/input.py
--rw-r--r--   0        0        0        0 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/tools/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      606 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/tools/adapters/input_adapters/base_input.py
--rw-r--r--   0        0        0      848 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/tools/adapters/input_adapters/dataframe_input.py
--rw-r--r--   0        0        0      178 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/tools/adapters/input_adapters/file_input.py
--rw-r--r--   0        0        0     1449 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/tools/adapters/input_adapters/image_input.py
--rw-r--r--   0        0        0      608 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/tools/adapters/input_adapters/json_input.py
--rw-r--r--   0        0        0      151 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/tools/adapters/input_adapters/string_input.py
--rw-r--r--   0        0        0     1363 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
--rw-r--r--   0        0        0     2511 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/tools/adapters/output.py
--rw-r--r--   0        0        0        0 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/tools/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      343 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/tools/adapters/output_adapters/base_output.py
--rw-r--r--   0        0        0      650 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/tools/adapters/output_adapters/dataframe_output.py
--rw-r--r--   0        0        0     1738 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/tools/adapters/output_adapters/default_output.py
--rw-r--r--   0        0        0      568 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/tools/adapters/output_adapters/json_output.py
--rw-r--r--   0        0        0     1076 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
--rw-r--r--   0        0        0      975 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/tools/run_model_locally.py
--rw-r--r--   0        0        0        0 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/utils/__init__.py
--rw-r--r--   0        0        0      320 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model/utils/extract_wrapped_function.py
--rw-r--r--   0        0        0        0 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model_loggers/__init__.py
--rw-r--r--   0        0        0     2701 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model_loggers/artifact_logger.py
--rw-r--r--   0        0        0     5186 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model_loggers/data_logger.py
--rw-r--r--   0        0        0      852 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/model_loggers/model_logger.py
--rw-r--r--   0        0        0        0 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/qwak_client/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/qwak_client/builds/__init__.py
--rw-r--r--   0        0        0     3698 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/qwak_client/builds/build.py
--rw-r--r--   0        0        0        0 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/qwak_client/builds/filters/__init__.py
--rw-r--r--   0        0        0     1185 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/qwak_client/builds/filters/metric_filter.py
--rw-r--r--   0        0        0     1088 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/qwak_client/builds/filters/parameter_filter.py
--rw-r--r--   0        0        0    15535 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/qwak_client/client.py
--rw-r--r--   0        0        0        0 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/qwak_client/deployments/__init__.py
--rw-r--r--   0        0        0    13221 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/qwak_client/deployments/deployment.py
--rw-r--r--   0        0        0        0 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/qwak_client/models/__init__.py
--rw-r--r--   0        0        0     1921 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/qwak_client/models/model.py
--rw-r--r--   0        0        0      533 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/qwak_client/models/model_metadata.py
--rw-r--r--   0        0        0        0 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/qwak_client/projects/__init__.py
--rw-r--r--   0        0        0     2284 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/qwak_client/projects/project.py
--rw-r--r--   0        0        0        0 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/testing/__init__.py
--rw-r--r--   0        0        0      318 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/testing/fixtures.py
--rw-r--r--   0        0        0        0 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/tools/__init__.py
--rw-r--r--   0        0        0      107 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/tools/logger/__init__.py
--rw-r--r--   0        0        0     9598 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/tools/logger/logger.py
--rw-r--r--   0        0        0     1941 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak/tools/logger/logging.yml
--rw-r--r--   0        0        0       46 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/__init__.py
--rw-r--r--   0        0        0     2150 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/alert_manager_service_api.py
--rw-r--r--   0        0        0     2129 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/analytics_api.py
--rw-r--r--   0        0        0     2647 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/audience_service_api.py
--rw-r--r--   0        0        0     1067 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/authentication_service.py
--rw-r--r--   0        0        0     8211 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/automation_management_service.py
--rw-r--r--   0        0        0     1019 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/autoscaling_service_api.py
--rw-r--r--   0        0        0    12316 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/batch_job_manager_service.py
--rw-r--r--   0        0        0     3841 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/build_management.py
--rw-r--r--   0        0        0     3909 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/build_orchestrator_build_api.py
--rw-r--r--   0        0        0     4150 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/build_orchestrator_service_api.py
--rw-r--r--   0        0        0     1412 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/data_versioning_service.py
--rw-r--r--   0        0        0    18268 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/deployment_management_service.py
--rw-r--r--   0        0        0     1158 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/ecosystem_service_api.py
--rw-r--r--   0        0        0     1536 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
--rw-r--r--   0        0        0     1782 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/feature_store_entities_manager_api.py
--rw-r--r--   0        0        0     3261 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
--rw-r--r--   0        0        0     5806 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/features_online_serving_api.py
--rw-r--r--   0        0        0     1001 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/features_operator_v3_service.py
--rw-r--r--   0        0        0     2276 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/features_set_state_service_api.py
--rw-r--r--   0        0        0     1127 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/feedback_service.py
--rw-r--r--   0        0        0     1412 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/file_versioning_service.py
--rw-r--r--   0        0        0     3905 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/instance_template_management_service.py
--rw-r--r--   0        0        0     2696 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/job_registry_service_api.py
--rw-r--r--   0        0        0     1583 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/kube_captain_service_api.py
--rw-r--r--   0        0        0     7381 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/logging_service.py
--rw-r--r--   0        0        0     3566 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/model_management_service.py
--rw-r--r--   0        0        0     3090 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/project_manager_service.py
--rw-r--r--   0        0        0     4186 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/qwak_mocks.py
--rw-r--r--   0        0        0     1406 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/secret_service.py
--rw-r--r--   0        0        0     1205 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/self_service_user_service.py
--rw-r--r--   0        0        0     4083 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/user_application_instance_service_api.py
--rw-r--r--   0        0        0        0 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/utils/__init__.py
--rw-r--r--   0        0        0      159 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/mocks/utils/exception_handlers.py
--rw-r--r--   0        0        0    13583 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/services_mock.py
--rw-r--r--   0        0        0        0 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/utils/__init__.py
--rw-r--r--   0        0        0      265 2023-06-04 15:02:32.057422 qwak_core-0.0.95/qwak_services_mock/utils/service_utils.py
--rw-r--r--   0        0        0     4984 1970-01-01 00:00:00.000000 qwak_core-0.0.95/setup.py
--rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 qwak_core-0.0.95/PKG-INFO
+-rw-r--r--   0        0        0      264 2023-06-05 08:15:26.757009 qwak_core-0.0.96/README.md
+-rw-r--r--   0        0        0        0 2023-06-05 08:17:07.409382 qwak_core-0.0.96/_qwak_proto/__init__.py
+-rw-r--r--   0        0        0     5378 2023-06-05 08:17:07.433382 qwak_core-0.0.96/_qwak_proto/qwak/administration/account/v1/account_pb2.py
+-rw-r--r--   0        0        0     6623 2023-06-05 08:16:45.689300 qwak_core-0.0.96/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.433382 qwak_core-0.0.96/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
+-rw-r--r--   0        0        0     2390 2023-06-05 08:17:07.429382 qwak_core-0.0.96/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
+-rw-r--r--   0        0        0     1475 2023-06-05 08:16:45.325299 qwak_core-0.0.96/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.429382 qwak_core-0.0.96/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     2106 2023-06-05 08:17:07.429382 qwak_core-0.0.96/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
+-rw-r--r--   0        0        0     1207 2023-06-05 08:16:45.505299 qwak_core-0.0.96/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.429382 qwak_core-0.0.96/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
+-rw-r--r--   0        0        0     6751 2023-06-05 08:17:07.421382 qwak_core-0.0.96/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
+-rw-r--r--   0        0        0     4346 2023-06-05 08:16:44.781297 qwak_core-0.0.96/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
+-rw-r--r--   0        0        0     7662 2023-06-05 08:17:07.421382 qwak_core-0.0.96/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-06-05 08:17:07.425382 qwak_core-0.0.96/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
+-rw-r--r--   0        0        0     2650 2023-06-05 08:16:44.961297 qwak_core-0.0.96/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.425382 qwak_core-0.0.96/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0     4901 2023-06-05 08:17:07.425382 qwak_core-0.0.96/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
+-rw-r--r--   0        0        0     5995 2023-06-05 08:16:45.141298 qwak_core-0.0.96/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.425382 qwak_core-0.0.96/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
+-rw-r--r--   0        0        0     4635 2023-06-05 08:17:07.409382 qwak_core-0.0.96/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
+-rw-r--r--   0        0        0     3664 2023-06-05 08:16:44.597296 qwak_core-0.0.96/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
+-rw-r--r--   0        0        0     3167 2023-06-05 08:17:07.409382 qwak_core-0.0.96/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5707 2023-06-05 08:17:07.409382 qwak_core-0.0.96/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
+-rw-r--r--   0        0        0     8170 2023-06-05 08:16:45.873301 qwak_core-0.0.96/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.413382 qwak_core-0.0.96/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
+-rw-r--r--   0        0        0     4512 2023-06-05 08:17:07.413382 qwak_core-0.0.96/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
+-rw-r--r--   0        0        0     5690 2023-06-05 08:16:46.241302 qwak_core-0.0.96/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.417382 qwak_core-0.0.96/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
+-rw-r--r--   0        0        0    16001 2023-06-05 08:17:07.417382 qwak_core-0.0.96/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
+-rw-r--r--   0        0        0    12387 2023-06-05 08:16:46.433303 qwak_core-0.0.96/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
+-rw-r--r--   0        0        0    16458 2023-06-05 08:17:07.417382 qwak_core-0.0.96/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2464 2023-06-05 08:17:07.413382 qwak_core-0.0.96/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
+-rw-r--r--   0        0        0     1347 2023-06-05 08:16:46.057301 qwak_core-0.0.96/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.413382 qwak_core-0.0.96/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     6425 2023-06-05 08:17:07.421382 qwak_core-0.0.96/_qwak_proto/qwak/administration/v0/users/user_pb2.py
+-rw-r--r--   0        0        0    10323 2023-06-05 08:16:46.617303 qwak_core-0.0.96/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.421382 qwak_core-0.0.96/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
+-rw-r--r--   0        0        0     9577 2023-06-05 08:17:07.461382 qwak_core-0.0.96/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
+-rw-r--r--   0        0        0    13624 2023-06-05 08:16:49.197313 qwak_core-0.0.96/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.461382 qwak_core-0.0.96/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
+-rw-r--r--   0        0        0     9270 2023-06-05 08:17:07.465382 qwak_core-0.0.96/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
+-rw-r--r--   0        0        0     5571 2023-06-05 08:16:49.381314 qwak_core-0.0.96/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
+-rw-r--r--   0        0        0    10742 2023-06-05 08:17:07.465382 qwak_core-0.0.96/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7365 2023-06-05 08:17:07.537382 qwak_core-0.0.96/_qwak_proto/qwak/analytics/analytics_pb2.py
+-rw-r--r--   0        0        0    11839 2023-06-05 08:16:55.109336 qwak_core-0.0.96/_qwak_proto/qwak/analytics/analytics_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.537382 qwak_core-0.0.96/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
+-rw-r--r--   0        0        0     9396 2023-06-05 08:17:07.537382 qwak_core-0.0.96/_qwak_proto/qwak/analytics/analytics_service_pb2.py
+-rw-r--r--   0        0        0     7896 2023-06-05 08:16:55.321336 qwak_core-0.0.96/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
+-rw-r--r--   0        0        0    11917 2023-06-05 08:17:07.541382 qwak_core-0.0.96/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9021 2023-06-05 08:17:07.541382 qwak_core-0.0.96/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
+-rw-r--r--   0        0        0     5865 2023-06-05 08:16:56.261340 qwak_core-0.0.96/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
+-rw-r--r--   0        0        0    11486 2023-06-05 08:17:07.545383 qwak_core-0.0.96/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
+-rw-r--r--   0        0        0     8807 2023-06-05 08:17:07.541382 qwak_core-0.0.96/_qwak_proto/qwak/audience/v1/audience_pb2.py
+-rw-r--r--   0        0        0    13570 2023-06-05 08:16:56.077339 qwak_core-0.0.96/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.541382 qwak_core-0.0.96/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
+-rw-r--r--   0        0        0     5777 2023-06-05 08:17:07.545383 qwak_core-0.0.96/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     8264 2023-06-05 08:16:56.445341 qwak_core-0.0.96/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.545383 qwak_core-0.0.96/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     2937 2023-06-05 08:17:07.545383 qwak_core-0.0.96/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
+-rw-r--r--   0        0        0     2014 2023-06-05 08:16:56.629341 qwak_core-0.0.96/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
+-rw-r--r--   0        0        0     2991 2023-06-05 08:17:07.549383 qwak_core-0.0.96/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12352 2023-06-05 08:17:07.637383 qwak_core-0.0.96/_qwak_proto/qwak/automation/v1/action_pb2.py
+-rw-r--r--   0        0        0    18970 2023-06-05 08:17:05.045373 qwak_core-0.0.96/_qwak_proto/qwak/automation/v1/action_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.637383 qwak_core-0.0.96/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
+-rw-r--r--   0        0        0     5775 2023-06-05 08:17:07.633383 qwak_core-0.0.96/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     8308 2023-06-05 08:17:04.669372 qwak_core-0.0.96/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.633383 qwak_core-0.0.96/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     3373 2023-06-05 08:17:07.633383 qwak_core-0.0.96/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
+-rw-r--r--   0        0        0     4400 2023-06-05 08:17:04.853372 qwak_core-0.0.96/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.637383 qwak_core-0.0.96/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
+-rw-r--r--   0        0        0    17887 2023-06-05 08:17:07.629383 qwak_core-0.0.96/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
+-rw-r--r--   0        0        0    12310 2023-06-05 08:17:04.297370 qwak_core-0.0.96/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
+-rw-r--r--   0        0        0    23338 2023-06-05 08:17:07.629383 qwak_core-0.0.96/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3873 2023-06-05 08:17:07.629383 qwak_core-0.0.96/_qwak_proto/qwak/automation/v1/automation_pb2.py
+-rw-r--r--   0        0        0     5291 2023-06-05 08:17:04.489371 qwak_core-0.0.96/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.633383 qwak_core-0.0.96/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
+-rw-r--r--   0        0        0     2383 2023-06-05 08:17:07.641383 qwak_core-0.0.96/_qwak_proto/qwak/automation/v1/common_pb2.py
+-rw-r--r--   0        0        0     2446 2023-06-05 08:17:05.605375 qwak_core-0.0.96/_qwak_proto/qwak/automation/v1/common_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.645383 qwak_core-0.0.96/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
+-rw-r--r--   0        0        0     5209 2023-06-05 08:17:07.641383 qwak_core-0.0.96/_qwak_proto/qwak/automation/v1/notification_pb2.py
+-rw-r--r--   0        0        0     5492 2023-06-05 08:17:05.421374 qwak_core-0.0.96/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.641383 qwak_core-0.0.96/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
+-rw-r--r--   0        0        0     4210 2023-06-05 08:17:07.637383 qwak_core-0.0.96/_qwak_proto/qwak/automation/v1/trigger_pb2.py
+-rw-r--r--   0        0        0     4746 2023-06-05 08:17:05.233374 qwak_core-0.0.96/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.641383 qwak_core-0.0.96/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
+-rw-r--r--   0        0        0    10989 2023-06-05 08:17:07.625383 qwak_core-0.0.96/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
+-rw-r--r--   0        0        0    15193 2023-06-05 08:17:04.105369 qwak_core-0.0.96/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.625383 qwak_core-0.0.96/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
+-rw-r--r--   0        0        0     2042 2023-06-05 08:17:07.621383 qwak_core-0.0.96/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
+-rw-r--r--   0        0        0     1904 2023-06-05 08:17:03.717368 qwak_core-0.0.96/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.621383 qwak_core-0.0.96/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
+-rw-r--r--   0        0        0    44118 2023-06-05 08:17:07.625383 qwak_core-0.0.96/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
+-rw-r--r--   0        0        0    58049 2023-06-05 08:17:03.917369 qwak_core-0.0.96/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
+-rw-r--r--   0        0        0    29918 2023-06-05 08:17:07.625383 qwak_core-0.0.96/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
+-rw-r--r--   0        0        0    20255 2023-06-05 08:17:07.573383 qwak_core-0.0.96/_qwak_proto/qwak/build/v1/build_api_pb2.py
+-rw-r--r--   0        0        0    17495 2023-06-05 08:16:58.517348 qwak_core-0.0.96/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
+-rw-r--r--   0        0        0    20359 2023-06-05 08:17:07.573383 qwak_core-0.0.96/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
+-rw-r--r--   0        0        0    16953 2023-06-05 08:17:07.569383 qwak_core-0.0.96/_qwak_proto/qwak/build/v1/build_pb2.py
+-rw-r--r--   0        0        0    25941 2023-06-05 08:16:58.329348 qwak_core-0.0.96/_qwak_proto/qwak/build/v1/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.573383 qwak_core-0.0.96/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
+-rw-r--r--   0        0        0    11691 2023-06-05 08:17:07.561383 qwak_core-0.0.96/_qwak_proto/qwak/builds/build_pb2.py
+-rw-r--r--   0        0        0    18850 2023-06-05 08:16:57.961346 qwak_core-0.0.96/_qwak_proto/qwak/builds/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.561383 qwak_core-0.0.96/_qwak_proto/qwak/builds/build_pb2_grpc.py
+-rw-r--r--   0        0        0     4777 2023-06-05 08:17:07.565383 qwak_core-0.0.96/_qwak_proto/qwak/builds/build_url_pb2.py
+-rw-r--r--   0        0        0     5773 2023-06-05 08:16:58.145347 qwak_core-0.0.96/_qwak_proto/qwak/builds/build_url_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.565383 qwak_core-0.0.96/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
+-rw-r--r--   0        0        0    12490 2023-06-05 08:17:07.565383 qwak_core-0.0.96/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
+-rw-r--r--   0        0        0     9351 2023-06-05 08:16:58.705349 qwak_core-0.0.96/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
+-rw-r--r--   0        0        0    14916 2023-06-05 08:17:07.565383 qwak_core-0.0.96/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
+-rw-r--r--   0        0        0    38290 2023-06-05 08:17:07.569383 qwak_core-0.0.96/_qwak_proto/qwak/builds/builds_pb2.py
+-rw-r--r--   0        0        0    52702 2023-06-05 08:16:59.149351 qwak_core-0.0.96/_qwak_proto/qwak/builds/builds_pb2.pyi
+-rw-r--r--   0        0        0    11572 2023-06-05 08:17:07.569383 qwak_core-0.0.96/_qwak_proto/qwak/builds/builds_pb2_grpc.py
+-rw-r--r--   0        0        0     1671 2023-06-05 08:17:07.577383 qwak_core-0.0.96/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
+-rw-r--r--   0        0        0     1689 2023-06-05 08:16:59.561352 qwak_core-0.0.96/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.581383 qwak_core-0.0.96/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4328 2023-06-05 08:17:07.581383 qwak_core-0.0.96/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-06-05 08:16:59.773353 qwak_core-0.0.96/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-06-05 08:17:07.581383 qwak_core-0.0.96/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7716 2023-06-05 08:17:07.557382 qwak_core-0.0.96/_qwak_proto/qwak/deployment/alert_pb2.py
+-rw-r--r--   0        0        0    11197 2023-06-05 08:16:57.397344 qwak_core-0.0.96/_qwak_proto/qwak/deployment/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.557382 qwak_core-0.0.96/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
+-rw-r--r--   0        0        0    11580 2023-06-05 08:17:07.557382 qwak_core-0.0.96/_qwak_proto/qwak/deployment/alert_service_pb2.py
+-rw-r--r--   0        0        0     7373 2023-06-05 08:16:57.585345 qwak_core-0.0.96/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
+-rw-r--r--   0        0        0    12803 2023-06-05 08:17:07.557382 qwak_core-0.0.96/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2162 2023-06-05 08:17:07.549383 qwak_core-0.0.96/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
+-rw-r--r--   0        0        0     2685 2023-06-05 08:16:57.013343 qwak_core-0.0.96/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.553382 qwak_core-0.0.96/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
+-rw-r--r--   0        0        0    43712 2023-06-05 08:17:07.549383 qwak_core-0.0.96/_qwak_proto/qwak/deployment/deployment_pb2.py
+-rw-r--r--   0        0        0    63341 2023-06-05 08:16:56.825342 qwak_core-0.0.96/_qwak_proto/qwak/deployment/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.549383 qwak_core-0.0.96/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    38320 2023-06-05 08:17:07.553382 qwak_core-0.0.96/_qwak_proto/qwak/deployment/deployment_service_pb2.py
+-rw-r--r--   0        0        0    33325 2023-06-05 08:16:57.209344 qwak_core-0.0.96/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
+-rw-r--r--   0        0        0    20242 2023-06-05 08:17:07.553382 qwak_core-0.0.96/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2527 2023-06-05 08:17:07.449382 qwak_core-0.0.96/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
+-rw-r--r--   0        0        0     2791 2023-06-05 08:16:48.273310 qwak_core-0.0.96/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.453382 qwak_core-0.0.96/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-06-05 08:17:07.453382 qwak_core-0.0.96/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
+-rw-r--r--   0        0        0    12641 2023-06-05 08:16:48.457311 qwak_core-0.0.96/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.453382 qwak_core-0.0.96/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
+-rw-r--r--   0        0        0    16366 2023-06-05 08:17:07.457382 qwak_core-0.0.96/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
+-rw-r--r--   0        0        0    17148 2023-06-05 08:16:48.645311 qwak_core-0.0.96/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
+-rw-r--r--   0        0        0    10706 2023-06-05 08:17:07.457382 qwak_core-0.0.96/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4787 2023-06-05 08:17:07.517382 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
+-rw-r--r--   0        0        0     6713 2023-06-05 08:16:53.993331 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.517382 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
+-rw-r--r--   0        0        0     9721 2023-06-05 08:17:07.513382 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
+-rw-r--r--   0        0        0     7409 2023-06-05 08:16:53.809331 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
+-rw-r--r--   0        0        0    12256 2023-06-05 08:17:07.517382 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11432 2023-06-05 08:17:07.493382 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
+-rw-r--r--   0        0        0    12882 2023-06-05 08:16:51.765323 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.493382 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
+-rw-r--r--   0        0        0     5303 2023-06-05 08:17:07.489382 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/execution_pb2.py
+-rw-r--r--   0        0        0     8604 2023-06-05 08:16:51.581322 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.489382 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
+-rw-r--r--   0        0        0    10074 2023-06-05 08:17:07.481382 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
+-rw-r--r--   0        0        0    14303 2023-06-05 08:16:51.013320 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.485382 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
+-rw-r--r--   0        0        0    28920 2023-06-05 08:17:07.489382 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
+-rw-r--r--   0        0        0    20665 2023-06-05 08:16:51.401322 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
+-rw-r--r--   0        0        0    35307 2023-06-05 08:17:07.489382 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12638 2023-06-05 08:17:07.493382 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
+-rw-r--r--   0        0        0    14071 2023-06-05 08:16:51.945324 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.493382 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
+-rw-r--r--   0        0        0    10044 2023-06-05 08:17:07.497382 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
+-rw-r--r--   0        0        0     6846 2023-06-05 08:16:52.129324 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
+-rw-r--r--   0        0        0    11647 2023-06-05 08:17:07.497382 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
+-rw-r--r--   0        0        0    25269 2023-06-05 08:17:07.485382 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
+-rw-r--r--   0        0        0    37664 2023-06-05 08:16:51.205321 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.485382 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
+-rw-r--r--   0        0        0     2872 2023-06-05 08:17:07.497382 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
+-rw-r--r--   0        0        0     2428 2023-06-05 08:16:52.305325 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.497382 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
+-rw-r--r--   0        0        0    10202 2023-06-05 08:17:07.501382 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_pb2.py
+-rw-r--r--   0        0        0    16565 2023-06-05 08:16:52.677326 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.505382 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_pb2_grpc.py
+-rw-r--r--   0        0        0     3559 2023-06-05 08:17:07.505382 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2.py
+-rw-r--r--   0        0        0     1759 2023-06-05 08:16:52.865327 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2.pyi
+-rw-r--r--   0        0        0     3608 2023-06-05 08:17:07.505382 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2_grpc.py
+-rw-r--r--   0        0        0    10604 2023-06-05 08:17:07.501382 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py
+-rw-r--r--   0        0        0    13410 2023-06-05 08:16:52.489326 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.501382 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2_grpc.py
+-rw-r--r--   0        0        0     4196 2023-06-05 08:17:07.517382 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
+-rw-r--r--   0        0        0     7323 2023-06-05 08:17:06.949380 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.521382 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
+-rw-r--r--   0        0        0     9895 2023-06-05 08:17:07.521382 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
+-rw-r--r--   0        0        0     9029 2023-06-05 08:17:07.133381 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
+-rw-r--r--   0        0        0    12090 2023-06-05 08:17:07.521382 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3596 2023-06-05 08:17:07.525382 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
+-rw-r--r--   0        0        0     6664 2023-06-05 08:16:54.553334 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.525382 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
+-rw-r--r--   0        0        0    11930 2023-06-05 08:17:07.525382 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
+-rw-r--r--   0        0        0    11052 2023-06-05 08:16:54.741334 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
+-rw-r--r--   0        0        0    14459 2023-06-05 08:17:07.525382 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5158 2023-06-05 08:17:07.529382 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/reports/report_pb2.py
+-rw-r--r--   0        0        0     7436 2023-06-05 08:16:54.925335 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.529382 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
+-rw-r--r--   0        0        0     4549 2023-06-05 08:17:07.533383 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
+-rw-r--r--   0        0        0     6442 2023-06-05 08:16:55.701338 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.533383 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
+-rw-r--r--   0        0        0    16693 2023-06-05 08:17:07.529382 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
+-rw-r--r--   0        0        0    20355 2023-06-05 08:16:55.509337 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
+-rw-r--r--   0        0        0     4809 2023-06-05 08:17:07.529382 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
+-rw-r--r--   0        0        0     2553 2023-06-05 08:17:07.533383 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
+-rw-r--r--   0        0        0     4000 2023-06-05 08:16:55.885339 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.533383 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
+-rw-r--r--   0        0        0    14046 2023-06-05 08:17:07.505382 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
+-rw-r--r--   0        0        0    23615 2023-06-05 08:16:53.053328 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.509382 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
+-rw-r--r--   0        0        0     5087 2023-06-05 08:17:07.509382 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
+-rw-r--r--   0        0        0     6011 2023-06-05 08:16:53.241329 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.509382 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
+-rw-r--r--   0        0        0    12309 2023-06-05 08:17:07.509382 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
+-rw-r--r--   0        0        0     9244 2023-06-05 08:16:53.429329 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
+-rw-r--r--   0        0        0    17071 2023-06-05 08:17:07.513382 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11014 2023-06-05 08:17:07.513382 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
+-rw-r--r--   0        0        0    15865 2023-06-05 08:16:53.621330 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.513382 qwak_core-0.0.96/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
+-rw-r--r--   0        0        0     4727 2023-06-05 08:17:07.645383 qwak_core-0.0.96/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
+-rw-r--r--   0        0        0     5122 2023-06-05 08:17:05.837376 qwak_core-0.0.96/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.645383 qwak_core-0.0.96/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4648 2023-06-05 08:17:07.645383 qwak_core-0.0.96/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4170 2023-06-05 08:17:06.021377 qwak_core-0.0.96/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-06-05 08:17:07.649383 qwak_core-0.0.96/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5349 2023-06-05 08:17:07.649383 qwak_core-0.0.96/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
+-rw-r--r--   0        0        0     5363 2023-06-05 08:17:06.201377 qwak_core-0.0.96/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.649383 qwak_core-0.0.96/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4437 2023-06-05 08:17:07.653383 qwak_core-0.0.96/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4127 2023-06-05 08:17:06.397378 qwak_core-0.0.96/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-06-05 08:17:07.653383 qwak_core-0.0.96/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6073 2023-06-05 08:17:07.653383 qwak_core-0.0.96/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
+-rw-r--r--   0        0        0     5366 2023-06-05 08:17:06.589379 qwak_core-0.0.96/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
+-rw-r--r--   0        0        0     7395 2023-06-05 08:17:07.653383 qwak_core-0.0.96/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4636 2023-06-05 08:17:07.657383 qwak_core-0.0.96/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
+-rw-r--r--   0        0        0     4239 2023-06-05 08:17:06.769379 qwak_core-0.0.96/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.657383 qwak_core-0.0.96/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     2376 2023-06-05 08:17:07.585383 qwak_core-0.0.96/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
+-rw-r--r--   0        0        0     3018 2023-06-05 08:16:59.973354 qwak_core-0.0.96/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.585383 qwak_core-0.0.96/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4325 2023-06-05 08:17:07.585383 qwak_core-0.0.96/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-06-05 08:17:00.185355 qwak_core-0.0.96/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-06-05 08:17:07.585383 qwak_core-0.0.96/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6401 2023-06-05 08:17:07.469382 qwak_core-0.0.96/_qwak_proto/qwak/fitness_service/constructs_pb2.py
+-rw-r--r--   0        0        0    10192 2023-06-05 08:16:50.265317 qwak_core-0.0.96/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.469382 qwak_core-0.0.96/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-06-05 08:17:07.473382 qwak_core-0.0.96/_qwak_proto/qwak/fitness_service/fitness_pb2.py
+-rw-r--r--   0        0        0     4115 2023-06-05 08:16:50.453318 qwak_core-0.0.96/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.473382 qwak_core-0.0.96/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
+-rw-r--r--   0        0        0     7123 2023-06-05 08:17:07.477382 qwak_core-0.0.96/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
+-rw-r--r--   0        0        0     3981 2023-06-05 08:16:50.637319 qwak_core-0.0.96/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
+-rw-r--r--   0        0        0     8546 2023-06-05 08:17:07.477382 qwak_core-0.0.96/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8428 2023-06-05 08:17:07.481382 qwak_core-0.0.96/_qwak_proto/qwak/fitness_service/status_pb2.py
+-rw-r--r--   0        0        0    12205 2023-06-05 08:16:50.821319 qwak_core-0.0.96/_qwak_proto/qwak/fitness_service/status_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.481382 qwak_core-0.0.96/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
+-rw-r--r--   0        0        0     8196 2023-06-05 08:17:07.561383 qwak_core-0.0.96/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
+-rw-r--r--   0        0        0    10867 2023-06-05 08:16:57.773346 qwak_core-0.0.96/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
+-rw-r--r--   0        0        0     4700 2023-06-05 08:17:07.561383 qwak_core-0.0.96/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
+-rw-r--r--   0        0        0     3757 2023-06-05 08:17:07.589383 qwak_core-0.0.96/_qwak_proto/qwak/instance_template/instance_template_pb2.py
+-rw-r--r--   0        0        0     4235 2023-06-05 08:17:00.405356 qwak_core-0.0.96/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.589383 qwak_core-0.0.96/_qwak_proto/qwak/instance_template/instance_template_pb2_grpc.py
+-rw-r--r--   0        0        0     4722 2023-06-05 08:17:07.589383 qwak_core-0.0.96/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py
+-rw-r--r--   0        0        0     3245 2023-06-05 08:17:00.649356 qwak_core-0.0.96/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi
+-rw-r--r--   0        0        0     5240 2023-06-05 08:17:07.589383 qwak_core-0.0.96/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7803 2023-06-05 08:17:07.601383 qwak_core-0.0.96/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
+-rw-r--r--   0        0        0    10487 2023-06-05 08:17:01.897361 qwak_core-0.0.96/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.605383 qwak_core-0.0.96/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
+-rw-r--r--   0        0        0     3704 2023-06-05 08:17:07.605383 qwak_core-0.0.96/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
+-rw-r--r--   0        0        0     3759 2023-06-05 08:17:02.097362 qwak_core-0.0.96/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.605383 qwak_core-0.0.96/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
+-rw-r--r--   0        0        0    22089 2023-06-05 08:17:07.605383 qwak_core-0.0.96/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
+-rw-r--r--   0        0        0    25879 2023-06-05 08:17:02.301363 qwak_core-0.0.96/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.609383 qwak_core-0.0.96/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
+-rw-r--r--   0        0        0    13157 2023-06-05 08:17:07.609383 qwak_core-0.0.96/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
+-rw-r--r--   0        0        0    21705 2023-06-05 08:17:02.505364 qwak_core-0.0.96/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.609383 qwak_core-0.0.96/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-06-05 08:17:07.609383 qwak_core-0.0.96/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
+-rw-r--r--   0        0        0    16128 2023-06-05 08:17:02.713364 qwak_core-0.0.96/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.613383 qwak_core-0.0.96/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    45273 2023-06-05 08:17:07.613383 qwak_core-0.0.96/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
+-rw-r--r--   0        0        0    35031 2023-06-05 08:17:02.933365 qwak_core-0.0.96/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
+-rw-r--r--   0        0        0    67567 2023-06-05 08:17:07.613383 qwak_core-0.0.96/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2411 2023-06-05 08:17:07.617383 qwak_core-0.0.96/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
+-rw-r--r--   0        0        0     2637 2023-06-05 08:17:03.133366 qwak_core-0.0.96/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.617383 qwak_core-0.0.96/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
+-rw-r--r--   0        0        0     3459 2023-06-05 08:17:07.593383 qwak_core-0.0.96/_qwak_proto/qwak/logging/log_filter_pb2.py
+-rw-r--r--   0        0        0     4169 2023-06-05 08:17:01.085358 qwak_core-0.0.96/_qwak_proto/qwak/logging/log_filter_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.593383 qwak_core-0.0.96/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
+-rw-r--r--   0        0        0     2233 2023-06-05 08:17:07.601383 qwak_core-0.0.96/_qwak_proto/qwak/logging/log_line_pb2.py
+-rw-r--r--   0        0        0     2135 2023-06-05 08:17:01.693360 qwak_core-0.0.96/_qwak_proto/qwak/logging/log_line_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.601383 qwak_core-0.0.96/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
+-rw-r--r--   0        0        0     3126 2023-06-05 08:17:07.597383 qwak_core-0.0.96/_qwak_proto/qwak/logging/log_reader_service_pb2.py
+-rw-r--r--   0        0        0     3479 2023-06-05 08:17:01.289359 qwak_core-0.0.96/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
+-rw-r--r--   0        0        0     2831 2023-06-05 08:17:07.597383 qwak_core-0.0.96/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
+-rw-r--r--   0        0        0    10138 2023-06-05 08:17:07.597383 qwak_core-0.0.96/_qwak_proto/qwak/logging/log_source_pb2.py
+-rw-r--r--   0        0        0    14337 2023-06-05 08:17:01.493360 qwak_core-0.0.96/_qwak_proto/qwak/logging/log_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.597383 qwak_core-0.0.96/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
+-rw-r--r--   0        0        0    22744 2023-06-05 08:17:07.577383 qwak_core-0.0.96/_qwak_proto/qwak/models/models_pb2.py
+-rw-r--r--   0        0        0    27142 2023-06-05 08:16:59.357352 qwak_core-0.0.96/_qwak_proto/qwak/models/models_pb2.pyi
+-rw-r--r--   0        0        0    14733 2023-06-05 08:17:07.577383 qwak_core-0.0.96/_qwak_proto/qwak/models/models_pb2_grpc.py
+-rw-r--r--   0        0        0    10745 2023-06-05 08:17:07.445382 qwak_core-0.0.96/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
+-rw-r--r--   0        0        0     6790 2023-06-05 08:16:49.781315 qwak_core-0.0.96/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
+-rw-r--r--   0        0        0    13657 2023-06-05 08:17:07.449382 qwak_core-0.0.96/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11564 2023-06-05 08:17:07.445382 qwak_core-0.0.96/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
+-rw-r--r--   0        0        0    14927 2023-06-05 08:16:49.581315 qwak_core-0.0.96/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.445382 qwak_core-0.0.96/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
+-rw-r--r--   0        0        0     5283 2023-06-05 08:17:07.449382 qwak_core-0.0.96/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
+-rw-r--r--   0        0        0     3745 2023-06-05 08:16:50.073316 qwak_core-0.0.96/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
+-rw-r--r--   0        0        0     5551 2023-06-05 08:17:07.449382 qwak_core-0.0.96/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8701 2023-06-05 08:17:07.573383 qwak_core-0.0.96/_qwak_proto/qwak/projects/projects_pb2.py
+-rw-r--r--   0        0        0     9794 2023-06-05 08:16:58.901350 qwak_core-0.0.96/_qwak_proto/qwak/projects/projects_pb2.pyi
+-rw-r--r--   0        0        0     7931 2023-06-05 08:17:07.577383 qwak_core-0.0.96/_qwak_proto/qwak/projects/projects_pb2_grpc.py
+-rw-r--r--   0        0        0     4752 2023-06-05 08:17:07.593383 qwak_core-0.0.96/_qwak_proto/qwak/secret_service/secret_service_pb2.py
+-rw-r--r--   0        0        0     2818 2023-06-05 08:17:00.877357 qwak_core-0.0.96/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
+-rw-r--r--   0        0        0     6253 2023-06-05 08:17:07.593383 qwak_core-0.0.96/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6225 2023-06-05 08:17:07.441382 qwak_core-0.0.96/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
+-rw-r--r--   0        0        0     7267 2023-06-05 08:16:47.537307 qwak_core-0.0.96/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.445382 qwak_core-0.0.96/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
+-rw-r--r--   0        0        0    16176 2023-06-05 08:17:07.441382 qwak_core-0.0.96/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
+-rw-r--r--   0        0        0    10166 2023-06-05 08:16:47.353306 qwak_core-0.0.96/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
+-rw-r--r--   0        0        0    19988 2023-06-05 08:17:07.441382 qwak_core-0.0.96/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1751 2023-06-05 08:17:07.433382 qwak_core-0.0.96/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
+-rw-r--r--   0        0        0      777 2023-06-05 08:16:46.801304 qwak_core-0.0.96/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.433382 qwak_core-0.0.96/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
+-rw-r--r--   0        0        0     2392 2023-06-05 08:17:07.437382 qwak_core-0.0.96/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
+-rw-r--r--   0        0        0     2129 2023-06-05 08:16:46.985305 qwak_core-0.0.96/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.437382 qwak_core-0.0.96/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
+-rw-r--r--   0        0        0    10389 2023-06-05 08:17:07.437382 qwak_core-0.0.96/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
+-rw-r--r--   0        0        0     8148 2023-06-05 08:16:47.169306 qwak_core-0.0.96/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
+-rw-r--r--   0        0        0    10512 2023-06-05 08:17:07.441382 qwak_core-0.0.96/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6843 2023-06-05 08:17:07.621383 qwak_core-0.0.96/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
+-rw-r--r--   0        0        0     4585 2023-06-05 08:17:03.517367 qwak_core-0.0.96/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
+-rw-r--r--   0        0        0     8228 2023-06-05 08:17:07.621383 qwak_core-0.0.96/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
+-rw-r--r--   0        0        0     7816 2023-06-05 08:17:07.617383 qwak_core-0.0.96/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
+-rw-r--r--   0        0        0    11958 2023-06-05 08:17:03.329367 qwak_core-0.0.96/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.617383 qwak_core-0.0.96/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
+-rw-r--r--   0        0        0    10961 2023-06-05 08:17:07.457382 qwak_core-0.0.96/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
+-rw-r--r--   0        0        0    14256 2023-06-05 08:16:48.833312 qwak_core-0.0.96/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.457382 qwak_core-0.0.96/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
+-rw-r--r--   0        0        0     3072 2023-06-05 08:17:07.461382 qwak_core-0.0.96/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
+-rw-r--r--   0        0        0     2663 2023-06-05 08:16:49.013312 qwak_core-0.0.96/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-05 08:17:07.461382 qwak_core-0.0.96/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
+-rw-r--r--   0        0        0     2661 2023-06-05 08:17:09.241389 qwak_core-0.0.96/pyproject.toml
+-rw-r--r--   0        0        0      447 2023-06-05 08:17:09.241389 qwak_core-0.0.96/qwak/__init__.py
+-rw-r--r--   0        0        0     1501 2023-06-05 08:15:26.757009 qwak_core-0.0.96/qwak/automations/__init__.py
+-rw-r--r--   0        0        0     3132 2023-06-05 08:15:26.757009 qwak_core-0.0.96/qwak/automations/automation_executions.py
+-rw-r--r--   0        0        0    12899 2023-06-05 08:15:26.757009 qwak_core-0.0.96/qwak/automations/automations.py
+-rw-r--r--   0        0        0     9638 2023-06-05 08:15:26.757009 qwak_core-0.0.96/qwak/automations/batch_execution_action.py
+-rw-r--r--   0        0        0    19120 2023-06-05 08:15:26.757009 qwak_core-0.0.96/qwak/automations/build_and_deploy_action.py
+-rw-r--r--   0        0        0     1697 2023-06-05 08:15:26.757009 qwak_core-0.0.96/qwak/automations/common.py
+-rw-r--r--   0        0        0        0 2023-06-05 08:15:26.757009 qwak_core-0.0.96/qwak/clients/__init__.py
+-rw-r--r--   0        0        0      224 2023-06-05 08:15:26.757009 qwak_core-0.0.96/qwak/clients/administration/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 08:15:26.757009 qwak_core-0.0.96/qwak/clients/administration/authenticated_user/__init__.py
+-rw-r--r--   0        0        0     1456 2023-06-05 08:15:26.757009 qwak_core-0.0.96/qwak/clients/administration/authenticated_user/client.py
+-rw-r--r--   0        0        0        0 2023-06-05 08:15:26.757009 qwak_core-0.0.96/qwak/clients/administration/authentication/__init__.py
+-rw-r--r--   0        0        0     1076 2023-06-05 08:15:26.757009 qwak_core-0.0.96/qwak/clients/administration/authentication/client.py
+-rw-r--r--   0        0        0        0 2023-06-05 08:15:26.757009 qwak_core-0.0.96/qwak/clients/administration/eco_system/__init__.py
+-rw-r--r--   0        0        0     5362 2023-06-05 08:15:26.757009 qwak_core-0.0.96/qwak/clients/administration/eco_system/client.py
+-rw-r--r--   0        0        0        0 2023-06-05 08:15:26.757009 qwak_core-0.0.96/qwak/clients/administration/environment/__init__.py
+-rw-r--r--   0        0        0     2704 2023-06-05 08:15:26.757009 qwak_core-0.0.96/qwak/clients/administration/environment/client.py
+-rw-r--r--   0        0        0        0 2023-06-05 08:15:26.757009 qwak_core-0.0.96/qwak/clients/administration/self_service/__init__.py
+-rw-r--r--   0        0        0     2602 2023-06-05 08:15:26.757009 qwak_core-0.0.96/qwak/clients/administration/self_service/client.py
+-rw-r--r--   0        0        0       43 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/clients/alert_management/__init__.py
+-rw-r--r--   0        0        0     2226 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/clients/alert_management/client.py
+-rw-r--r--   0        0        0       42 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/clients/analytics/__init__.py
+-rw-r--r--   0        0        0     3093 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/clients/analytics/client.py
+-rw-r--r--   0        0        0       35 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/clients/audience/__init__.py
+-rw-r--r--   0        0        0     2110 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/clients/audience/client.py
+-rw-r--r--   0        0        0        0 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/clients/automation_management/__init__.py
+-rw-r--r--   0        0        0     8836 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/clients/automation_management/client.py
+-rw-r--r--   0        0        0       38 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/clients/autoscaling/__init__.py
+-rw-r--r--   0        0        0     1240 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/clients/autoscaling/client.py
+-rw-r--r--   0        0        0      211 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/clients/batch_job_management/__init__.py
+-rw-r--r--   0        0        0    18388 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/clients/batch_job_management/client.py
+-rw-r--r--   0        0        0     6242 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/clients/batch_job_management/executions_config.py
+-rw-r--r--   0        0        0     1846 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/clients/batch_job_management/results.py
+-rw-r--r--   0        0        0       43 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/clients/build_management/__init__.py
+-rw-r--r--   0        0        0     4731 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/clients/build_management/client.py
+-rw-r--r--   0        0        0       44 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/clients/build_orchestrator/__init__.py
+-rw-r--r--   0        0        0    15319 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/clients/build_orchestrator/client.py
+-rw-r--r--   0        0        0        0 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/clients/data_versioning/__init__.py
+-rw-r--r--   0        0        0     1835 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/clients/data_versioning/client.py
+-rw-r--r--   0        0        0        0 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/clients/deployment/__init__.py
+-rw-r--r--   0        0        0     6269 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/clients/deployment/client.py
+-rw-r--r--   0        0        0       53 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/clients/feature_store/__init__.py
+-rw-r--r--   0        0        0     2635 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/clients/feature_store/job_registry_client.py
+-rw-r--r--   0        0        0    15898 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/clients/feature_store/management_client.py
+-rw-r--r--   0        0        0     4963 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/clients/feature_store/operator_client.py
+-rw-r--r--   0        0        0        0 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/clients/file_versioning/__init__.py
+-rw-r--r--   0        0        0     1939 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/clients/file_versioning/client.py
+-rw-r--r--   0        0        0        0 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/clients/instance_template/__init__.py
+-rw-r--r--   0        0        0     2495 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/clients/instance_template/client.py
+-rw-r--r--   0        0        0       41 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/clients/kube_deployment_captain/__init__.py
+-rw-r--r--   0        0        0     9276 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/clients/kube_deployment_captain/client.py
+-rw-r--r--   0        0        0       34 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/clients/logging_client/__init__.py
+-rw-r--r--   0        0        0     4906 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/clients/logging_client/client.py
+-rw-r--r--   0        0        0       43 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/clients/model_management/__init__.py
+-rw-r--r--   0        0        0     3695 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/clients/model_management/client.py
+-rw-r--r--   0        0        0        0 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/clients/project/__init__.py
+-rw-r--r--   0        0        0     2128 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/clients/project/client.py
+-rw-r--r--   0        0        0       40 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/clients/secret_service/__init__.py
+-rw-r--r--   0        0        0     3316 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/clients/secret_service/client.py
+-rw-r--r--   0        0        0       50 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/clients/user_application_instance/__init__.py
+-rw-r--r--   0        0        0     6013 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/clients/user_application_instance/client.py
+-rw-r--r--   0        0        0      380 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/exceptions/__init__.py
+-rw-r--r--   0        0        0      559 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/exceptions/quiet_error.py
+-rw-r--r--   0        0        0      469 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/exceptions/qwak_build_exception.py
+-rw-r--r--   0        0        0      135 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/exceptions/qwak_exception.py
+-rw-r--r--   0        0        0      579 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/exceptions/qwak_http_exception.py
+-rw-r--r--   0        0        0      100 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/exceptions/qwak_inference_exception.py
+-rw-r--r--   0        0        0      274 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/exceptions/qwak_load_model_failed_exception.py
+-rw-r--r--   0        0        0      211 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/exceptions/qwak_login_exception.py
+-rw-r--r--   0        0        0      152 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/exceptions/qwak_mock_http_exception.py
+-rw-r--r--   0        0        0      153 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/exceptions/qwak_model_initialization_exception.py
+-rw-r--r--   0        0        0      152 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/exceptions/qwak_not_found_exception.py
+-rw-r--r--   0        0        0      356 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/exceptions/qwak_quiet_build_exception.py
+-rw-r--r--   0        0        0        0 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/feature_store/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/feature_store/_common/__init__.py
+-rw-r--r--   0        0        0     4707 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/feature_store/_common/featureset_asterisk_handler.py
+-rw-r--r--   0        0        0     1298 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/feature_store/_common/functions.py
+-rw-r--r--   0        0        0     1263 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/feature_store/data_sources/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/feature_store/data_sources/batch_sources/__init__.py
+-rw-r--r--   0        0        0     2108 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/feature_store/data_sources/batch_sources/_batch.py
+-rw-r--r--   0        0        0      666 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/feature_store/data_sources/batch_sources/_jdbc.py
+-rw-r--r--   0        0        0     3059 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/feature_store/data_sources/batch_sources/big_query.py
+-rw-r--r--   0        0        0     1941 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/feature_store/data_sources/batch_sources/csv.py
+-rw-r--r--   0        0        0     2167 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/feature_store/data_sources/batch_sources/elastic_search.py
+-rw-r--r--   0        0        0     2987 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
+-rw-r--r--   0        0        0     1930 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/feature_store/data_sources/batch_sources/mongodb.py
+-rw-r--r--   0        0        0     1669 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/feature_store/data_sources/batch_sources/mysql.py
+-rw-r--r--   0        0        0     1717 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/feature_store/data_sources/batch_sources/parquet.py
+-rw-r--r--   0        0        0     1722 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/feature_store/data_sources/batch_sources/postgres.py
+-rw-r--r--   0        0        0     3216 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/feature_store/data_sources/batch_sources/redshift.py
+-rw-r--r--   0        0        0     2616 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/feature_store/data_sources/batch_sources/snowflake.py
+-rw-r--r--   0        0        0     1839 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/feature_store/data_sources/batch_sources/vertica.py
+-rw-r--r--   0        0        0        0 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/feature_store/entities/__init__.py
+-rw-r--r--   0        0        0     1794 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/feature_store/entities/entity.py
+-rw-r--r--   0        0        0        0 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/feature_store/feature_sets/__init__.py
+-rw-r--r--   0        0        0     1547 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/feature_store/feature_sets/backfill.py
+-rw-r--r--   0        0        0    17012 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/feature_store/feature_sets/batch.py
+-rw-r--r--   0        0        0      263 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/feature_store/feature_sets/context.py
+-rw-r--r--   0        0        0     1630 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/feature_store/feature_sets/execution_spec.py
+-rw-r--r--   0        0        0      584 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/feature_store/feature_sets/metadata.py
+-rw-r--r--   0        0        0     6820 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/feature_store/feature_sets/read_policies.py
+-rw-r--r--   0        0        0     1554 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/feature_store/feature_sets/transformations.py
+-rw-r--r--   0        0        0       89 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/feature_store/offline/__init__.py
+-rw-r--r--   0        0        0      738 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/feature_store/offline/_query_engine.py
+-rw-r--r--   0        0        0        0 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/feature_store/offline/athena/__init__.py
+-rw-r--r--   0        0        0     5182 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/feature_store/offline/athena/athena_query_engine.py
+-rw-r--r--   0        0        0    28013 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/feature_store/offline/client.py
+-rw-r--r--   0        0        0        0 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/feature_store/online/__init__.py
+-rw-r--r--   0        0        0     9261 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/feature_store/online/client.py
+-rw-r--r--   0        0        0      226 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/inner/__init__.py
+-rw-r--r--   0        0        0      954 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/inner/const.py
+-rw-r--r--   0        0        0     1435 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/inner/di_configuration/__init__.py
+-rw-r--r--   0        0        0     4768 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/inner/di_configuration/account.py
+-rw-r--r--   0        0        0       73 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/inner/di_configuration/config.yml
+-rw-r--r--   0        0        0      621 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/inner/di_configuration/containers.py
+-rw-r--r--   0        0        0      344 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/inner/di_configuration/session.py
+-rw-r--r--   0        0        0     2336 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/inner/model_loggers_utils.py
+-rw-r--r--   0        0        0      266 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/inner/runtime_di/__init__.py
+-rw-r--r--   0        0        0      349 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/inner/runtime_di/containers.py
+-rw-r--r--   0        0        0      627 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/inner/singleton_meta.py
+-rw-r--r--   0        0        0       74 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/inner/tool/__init__.py
+-rw-r--r--   0        0        0     3414 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/inner/tool/auth.py
+-rw-r--r--   0        0        0        0 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/inner/tool/grpc/__init__.py
+-rw-r--r--   0        0        0      560 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/inner/tool/grpc/grpc_auth.py
+-rw-r--r--   0        0        0     5804 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/inner/tool/grpc/grpc_tools.py
+-rw-r--r--   0        0        0      473 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/inner/tool/grpc/grpc_try_wrapping.py
+-rw-r--r--   0        0        0      435 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/inner/tool/retry_utils.py
+-rw-r--r--   0        0        0      218 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/inner/tool/run_config/__init__.py
+-rw-r--r--   0        0        0     3148 2023-06-05 08:15:26.761009 qwak_core-0.0.96/qwak/inner/tool/run_config/base.py
+-rw-r--r--   0        0        0     6083 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/inner/tool/run_config/utils.py
+-rw-r--r--   0        0        0        0 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model/__init__.py
+-rw-r--r--   0        0        0     1739 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      198 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model/adapters/input_adapters/base_input_adapter.py
+-rw-r--r--   0        0        0      210 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model/adapters/input_adapters/file_input_adapter.py
+-rw-r--r--   0        0        0      206 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model/adapters/input_adapters/image_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model/adapters/input_adapters/json_input_adapter.py
+-rw-r--r--   0        0        0     2175 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model/adapters/input_adapters/multi_input_adapter.py
+-rw-r--r--   0        0        0     3208 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model/adapters/input_adapters/numpy_input_adapter.py
+-rw-r--r--   0        0        0      862 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model/adapters/input_adapters/proto_input_adapter.py
+-rw-r--r--   0        0        0      207 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model/adapters/input_adapters/string_input_adapter.py
+-rw-r--r--   0        0        0      209 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
+-rw-r--r--   0        0        0        0 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      315 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model/adapters/output_adapters/base_output_adapter.py
+-rw-r--r--   0        0        0      221 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
+-rw-r--r--   0        0        0      219 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model/adapters/output_adapters/default_output_adapter.py
+-rw-r--r--   0        0        0      216 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model/adapters/output_adapters/json_output_adapter.py
+-rw-r--r--   0        0        0     1065 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model/adapters/output_adapters/numpy_output_adapter.py
+-rw-r--r--   0        0        0      517 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model/adapters/output_adapters/proto_output_adapter.py
+-rw-r--r--   0        0        0      115 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
+-rw-r--r--   0        0        0      220 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
+-rw-r--r--   0        0        0      303 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model/analytics_logging.py
+-rw-r--r--   0        0        0     2825 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model/base.py
+-rw-r--r--   0        0        0        0 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model/decorators/__init__.py
+-rw-r--r--   0        0        0     1288 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model/decorators/api.py
+-rw-r--r--   0        0        0      861 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model/decorators/api_implementation.py
+-rw-r--r--   0        0        0     1503 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model/experiment_tracking.py
+-rw-r--r--   0        0        0      873 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model/schema.py
+-rw-r--r--   0        0        0     2970 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model/schema_entities.py
+-rw-r--r--   0        0        0      338 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model/tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model/tools/adapters/__init__.py
+-rw-r--r--   0        0        0     1193 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model/tools/adapters/encoders.py
+-rw-r--r--   0        0        0     1963 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model/tools/adapters/input.py
+-rw-r--r--   0        0        0        0 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model/tools/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      606 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model/tools/adapters/input_adapters/base_input.py
+-rw-r--r--   0        0        0      848 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model/tools/adapters/input_adapters/dataframe_input.py
+-rw-r--r--   0        0        0      178 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model/tools/adapters/input_adapters/file_input.py
+-rw-r--r--   0        0        0     1449 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model/tools/adapters/input_adapters/image_input.py
+-rw-r--r--   0        0        0      608 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model/tools/adapters/input_adapters/json_input.py
+-rw-r--r--   0        0        0      151 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model/tools/adapters/input_adapters/string_input.py
+-rw-r--r--   0        0        0     1363 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
+-rw-r--r--   0        0        0     2511 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model/tools/adapters/output.py
+-rw-r--r--   0        0        0        0 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model/tools/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      343 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model/tools/adapters/output_adapters/base_output.py
+-rw-r--r--   0        0        0      650 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model/tools/adapters/output_adapters/dataframe_output.py
+-rw-r--r--   0        0        0     1738 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model/tools/adapters/output_adapters/default_output.py
+-rw-r--r--   0        0        0      568 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model/tools/adapters/output_adapters/json_output.py
+-rw-r--r--   0        0        0     1076 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
+-rw-r--r--   0        0        0      975 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model/tools/run_model_locally.py
+-rw-r--r--   0        0        0        0 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model/utils/__init__.py
+-rw-r--r--   0        0        0      320 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model/utils/extract_wrapped_function.py
+-rw-r--r--   0        0        0        0 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model_loggers/__init__.py
+-rw-r--r--   0        0        0     2701 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model_loggers/artifact_logger.py
+-rw-r--r--   0        0        0     5186 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model_loggers/data_logger.py
+-rw-r--r--   0        0        0      852 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/model_loggers/model_logger.py
+-rw-r--r--   0        0        0        0 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/qwak_client/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/qwak_client/builds/__init__.py
+-rw-r--r--   0        0        0     3698 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/qwak_client/builds/build.py
+-rw-r--r--   0        0        0        0 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/qwak_client/builds/filters/__init__.py
+-rw-r--r--   0        0        0     1185 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/qwak_client/builds/filters/metric_filter.py
+-rw-r--r--   0        0        0     1088 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/qwak_client/builds/filters/parameter_filter.py
+-rw-r--r--   0        0        0    15535 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/qwak_client/client.py
+-rw-r--r--   0        0        0        0 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/qwak_client/deployments/__init__.py
+-rw-r--r--   0        0        0    13221 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/qwak_client/deployments/deployment.py
+-rw-r--r--   0        0        0        0 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/qwak_client/models/__init__.py
+-rw-r--r--   0        0        0     1921 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/qwak_client/models/model.py
+-rw-r--r--   0        0        0      533 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/qwak_client/models/model_metadata.py
+-rw-r--r--   0        0        0        0 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/qwak_client/projects/__init__.py
+-rw-r--r--   0        0        0     2284 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/qwak_client/projects/project.py
+-rw-r--r--   0        0        0        0 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/testing/__init__.py
+-rw-r--r--   0        0        0      318 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/testing/fixtures.py
+-rw-r--r--   0        0        0        0 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/tools/__init__.py
+-rw-r--r--   0        0        0      107 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/tools/logger/__init__.py
+-rw-r--r--   0        0        0     9598 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/tools/logger/logger.py
+-rw-r--r--   0        0        0     1941 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak/tools/logger/logging.yml
+-rw-r--r--   0        0        0       46 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak_services_mock/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak_services_mock/mocks/__init__.py
+-rw-r--r--   0        0        0     2150 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak_services_mock/mocks/alert_manager_service_api.py
+-rw-r--r--   0        0        0     2129 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak_services_mock/mocks/analytics_api.py
+-rw-r--r--   0        0        0     2647 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak_services_mock/mocks/audience_service_api.py
+-rw-r--r--   0        0        0     1067 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak_services_mock/mocks/authentication_service.py
+-rw-r--r--   0        0        0     8211 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak_services_mock/mocks/automation_management_service.py
+-rw-r--r--   0        0        0     1019 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak_services_mock/mocks/autoscaling_service_api.py
+-rw-r--r--   0        0        0    12316 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak_services_mock/mocks/batch_job_manager_service.py
+-rw-r--r--   0        0        0     3841 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak_services_mock/mocks/build_management.py
+-rw-r--r--   0        0        0     3909 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak_services_mock/mocks/build_orchestrator_build_api.py
+-rw-r--r--   0        0        0     4150 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak_services_mock/mocks/build_orchestrator_service_api.py
+-rw-r--r--   0        0        0     1412 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak_services_mock/mocks/data_versioning_service.py
+-rw-r--r--   0        0        0    18268 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak_services_mock/mocks/deployment_management_service.py
+-rw-r--r--   0        0        0     1158 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak_services_mock/mocks/ecosystem_service_api.py
+-rw-r--r--   0        0        0     1536 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
+-rw-r--r--   0        0        0     1782 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak_services_mock/mocks/feature_store_entities_manager_api.py
+-rw-r--r--   0        0        0     3261 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
+-rw-r--r--   0        0        0     5806 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak_services_mock/mocks/features_online_serving_api.py
+-rw-r--r--   0        0        0     1001 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak_services_mock/mocks/features_operator_v3_service.py
+-rw-r--r--   0        0        0     2276 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak_services_mock/mocks/features_set_state_service_api.py
+-rw-r--r--   0        0        0     1127 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak_services_mock/mocks/feedback_service.py
+-rw-r--r--   0        0        0     1412 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak_services_mock/mocks/file_versioning_service.py
+-rw-r--r--   0        0        0     3905 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak_services_mock/mocks/instance_template_management_service.py
+-rw-r--r--   0        0        0     2696 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak_services_mock/mocks/job_registry_service_api.py
+-rw-r--r--   0        0        0     1583 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak_services_mock/mocks/kube_captain_service_api.py
+-rw-r--r--   0        0        0     7381 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak_services_mock/mocks/logging_service.py
+-rw-r--r--   0        0        0     3566 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak_services_mock/mocks/model_management_service.py
+-rw-r--r--   0        0        0     3090 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak_services_mock/mocks/project_manager_service.py
+-rw-r--r--   0        0        0     4186 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak_services_mock/mocks/qwak_mocks.py
+-rw-r--r--   0        0        0     1406 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak_services_mock/mocks/secret_service.py
+-rw-r--r--   0        0        0     1205 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak_services_mock/mocks/self_service_user_service.py
+-rw-r--r--   0        0        0     4083 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak_services_mock/mocks/user_application_instance_service_api.py
+-rw-r--r--   0        0        0        0 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak_services_mock/mocks/utils/__init__.py
+-rw-r--r--   0        0        0      159 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak_services_mock/mocks/utils/exception_handlers.py
+-rw-r--r--   0        0        0    13583 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak_services_mock/services_mock.py
+-rw-r--r--   0        0        0        0 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak_services_mock/utils/__init__.py
+-rw-r--r--   0        0        0      265 2023-06-05 08:15:26.765009 qwak_core-0.0.96/qwak_services_mock/utils/service_utils.py
+-rw-r--r--   0        0        0     4984 1970-01-01 00:00:00.000000 qwak_core-0.0.96/setup.py
+-rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 qwak_core-0.0.96/PKG-INFO
```

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/administration/account/v1/account_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/administration/account/v1/account_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py` & `qwak_core-0.0.96/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py` & `qwak_core-0.0.96/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py` & `qwak_core-0.0.96/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/users/user_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/administration/v0/users/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py` & `qwak_core-0.0.96/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/analytics/analytics_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/analytics/analytics_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/analytics/analytics_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/analytics/analytics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/analytics/analytics_service_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/analytics/analytics_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py` & `qwak_core-0.0.96/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/audience/v1/audience_api_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/audience/v1/audience_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py` & `qwak_core-0.0.96/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/audience/v1/audience_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/audience/v1/audience_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/audience/v1/audience_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/audience/v1/audience_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py` & `qwak_core-0.0.96/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/action_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/automation/v1/action_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/action_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/automation/v1/action_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py` & `qwak_core-0.0.96/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/automation_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/automation/v1/automation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/automation_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/automation/v1/automation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/common_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/automation/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/common_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/automation/v1/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/notification_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/automation/v1/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/notification_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/automation/v1/notification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/trigger_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/automation/v1/trigger_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi`

 * *Files identical despite different names*

```diff
@@ -728,15 +728,15 @@
     NUMBER_OF_PODS_FIELD_NUMBER: builtins.int
     POD_COMPUTE_RESOURCES_FIELD_NUMBER: builtins.int
     TEMPLATE_ID_FIELD_NUMBER: builtins.int
     number_of_pods: builtins.int
     """Number of pods in execution"""
     @property
     def pod_compute_resources(self) -> qwak.user_application.common.v0.resources_pb2.PodComputeResources:
-        """Resources"""
+        """Resources Of Execution"""
     template_id: builtins.str
     """Template id used"""
     def __init__(
         self,
         *,
         number_of_pods: builtins.int = ...,
         pod_compute_resources: qwak.user_application.common.v0.resources_pb2.PodComputeResources | None = ...,
```

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py` & `qwak_core-0.0.96/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/build/v1/build_api_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/build/v1/build_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/build/v1/build_api_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/build/v1/build_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py` & `qwak_core-0.0.96/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/build/v1/build_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/build/v1/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/build/v1/build_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/build/v1/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/builds/build_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/builds/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/builds/build_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/builds/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/builds/build_url_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/builds/build_url_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/builds/build_url_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/builds/build_url_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py` & `qwak_core-0.0.96/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/builds/builds_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/builds/builds_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/builds/builds_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/builds/builds_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/builds/builds_pb2_grpc.py` & `qwak_core-0.0.96/_qwak_proto/qwak/builds/builds_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py` & `qwak_core-0.0.96/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/deployment/alert_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/deployment/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/deployment/alert_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/deployment/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/deployment/alert_service_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/deployment/alert_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/deployment/alert_service_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/deployment/alert_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py` & `qwak_core-0.0.96/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/deployment/deployment_messages_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/deployment/deployment_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/deployment/deployment_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/deployment/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/deployment/deployment_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/deployment/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/deployment/deployment_service_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/deployment/deployment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py` & `qwak_core-0.0.96/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py` & `qwak_core-0.0.96/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/entities/entity_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/entities/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/execution_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2_grpc.py` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/jobs/job_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/jobs/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/reports/report_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/reports/report_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/serving/serving_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/serving/serving_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/sources/batch_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/sources/batch_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.96/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.96/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py` & `qwak_core-0.0.96/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py` & `qwak_core-0.0.96/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/fitness_service/constructs_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/fitness_service/constructs_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/fitness_service/fitness_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/fitness_service/fitness_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py` & `qwak_core-0.0.96/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/fitness_service/status_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/fitness_service/status_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/fitness_service/status_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/fitness_service/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/inference/feedback/feedback_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/inference/feedback/feedback_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py` & `qwak_core-0.0.96/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/instance_template/instance_template_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/instance_template/instance_template_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py` & `qwak_core-0.0.96/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py` & `qwak_core-0.0.96/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/logging/log_filter_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/logging/log_filter_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/logging/log_filter_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/logging/log_filter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/logging/log_line_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/logging/log_line_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/logging/log_line_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/logging/log_line_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/logging/log_reader_service_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/logging/log_reader_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py` & `qwak_core-0.0.96/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/logging/log_source_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/logging/log_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/logging/log_source_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/logging/log_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/models/models_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/models/models_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/models/models_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/models/models_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/models/models_pb2_grpc.py` & `qwak_core-0.0.96/_qwak_proto/qwak/models/models_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py` & `qwak_core-0.0.96/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py` & `qwak_core-0.0.96/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/projects/projects_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/projects/projects_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/projects/projects_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/projects/projects_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/projects/projects_pb2_grpc.py` & `qwak_core-0.0.96/_qwak_proto/qwak/projects/projects_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/secret_service/secret_service_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/secret_service/secret_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py` & `qwak_core-0.0.96/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py` & `qwak_core-0.0.96/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/self_service/user/v1/user_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/self_service/user/v1/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py` & `qwak_core-0.0.96/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py` & `qwak_core-0.0.96/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/traffic/v1/traffic_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/traffic/v1/traffic_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/user_application/v0/user_application_pb2.py` & `qwak_core-0.0.96/_qwak_proto/qwak/user_application/v0/user_application_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi` & `qwak_core-0.0.96/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/pyproject.toml` & `qwak_core-0.0.96/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qwak-core"
-version = "0.0.95"
+version = "0.0.96"
 description = "Qwak Core contains the necessary objects and communication tools for using the Qwak Platform"
 authors = ["Qwak <info@qwak.com>"]
 readme = "README.md"
 keywords = ["mlops", "ml", "deployment", "serving", "model"]
 packages = [
     { include = "qwak" },
     { include = "_qwak_proto" },
```

### Comparing `qwak_core-0.0.95/qwak/automations/__init__.py` & `qwak_core-0.0.96/qwak/automations/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/automations/automation_executions.py` & `qwak_core-0.0.96/qwak/automations/automation_executions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/automations/automations.py` & `qwak_core-0.0.96/qwak/automations/automations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/automations/batch_execution_action.py` & `qwak_core-0.0.96/qwak/automations/batch_execution_action.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/automations/build_and_deploy_action.py` & `qwak_core-0.0.96/qwak/automations/build_and_deploy_action.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/automations/common.py` & `qwak_core-0.0.96/qwak/automations/common.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/clients/administration/authenticated_user/client.py` & `qwak_core-0.0.96/qwak/clients/administration/authenticated_user/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/clients/administration/authentication/client.py` & `qwak_core-0.0.96/qwak/clients/administration/authentication/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/clients/administration/eco_system/client.py` & `qwak_core-0.0.96/qwak/clients/administration/eco_system/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/clients/administration/environment/client.py` & `qwak_core-0.0.96/qwak/clients/administration/environment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/clients/administration/self_service/client.py` & `qwak_core-0.0.96/qwak/clients/administration/self_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/clients/alert_management/client.py` & `qwak_core-0.0.96/qwak/clients/alert_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/clients/analytics/client.py` & `qwak_core-0.0.96/qwak/clients/analytics/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/clients/audience/client.py` & `qwak_core-0.0.96/qwak/clients/audience/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/clients/automation_management/client.py` & `qwak_core-0.0.96/qwak/clients/automation_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/clients/autoscaling/client.py` & `qwak_core-0.0.96/qwak/clients/autoscaling/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/clients/batch_job_management/client.py` & `qwak_core-0.0.96/qwak/clients/batch_job_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/clients/batch_job_management/executions_config.py` & `qwak_core-0.0.96/qwak/clients/batch_job_management/executions_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/clients/batch_job_management/results.py` & `qwak_core-0.0.96/qwak/clients/batch_job_management/results.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/clients/build_management/client.py` & `qwak_core-0.0.96/qwak/clients/build_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/clients/build_orchestrator/client.py` & `qwak_core-0.0.96/qwak/clients/build_orchestrator/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/clients/data_versioning/client.py` & `qwak_core-0.0.96/qwak/clients/data_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/clients/deployment/client.py` & `qwak_core-0.0.96/qwak/clients/deployment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/clients/feature_store/job_registry_client.py` & `qwak_core-0.0.96/qwak/clients/feature_store/job_registry_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/clients/feature_store/management_client.py` & `qwak_core-0.0.96/qwak/clients/feature_store/management_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/clients/feature_store/operator_client.py` & `qwak_core-0.0.96/qwak/clients/feature_store/operator_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/clients/file_versioning/client.py` & `qwak_core-0.0.96/qwak/clients/file_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/clients/instance_template/client.py` & `qwak_core-0.0.96/qwak/clients/instance_template/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/clients/kube_deployment_captain/client.py` & `qwak_core-0.0.96/qwak/clients/kube_deployment_captain/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/clients/logging_client/client.py` & `qwak_core-0.0.96/qwak/clients/logging_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/clients/model_management/client.py` & `qwak_core-0.0.96/qwak/clients/model_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/clients/project/client.py` & `qwak_core-0.0.96/qwak/clients/project/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/clients/secret_service/client.py` & `qwak_core-0.0.96/qwak/clients/secret_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/clients/user_application_instance/client.py` & `qwak_core-0.0.96/qwak/clients/user_application_instance/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/exceptions/quiet_error.py` & `qwak_core-0.0.96/qwak/exceptions/quiet_error.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/exceptions/qwak_http_exception.py` & `qwak_core-0.0.96/qwak/exceptions/qwak_http_exception.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/feature_store/_common/featureset_asterisk_handler.py` & `qwak_core-0.0.96/qwak/feature_store/_common/featureset_asterisk_handler.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/feature_store/_common/functions.py` & `qwak_core-0.0.96/qwak/feature_store/_common/functions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/feature_store/data_sources/__init__.py` & `qwak_core-0.0.96/qwak/feature_store/data_sources/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/feature_store/data_sources/batch_sources/_batch.py` & `qwak_core-0.0.96/qwak/feature_store/data_sources/batch_sources/_batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/feature_store/data_sources/batch_sources/_jdbc.py` & `qwak_core-0.0.96/qwak/feature_store/data_sources/batch_sources/_jdbc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/feature_store/data_sources/batch_sources/big_query.py` & `qwak_core-0.0.96/qwak/feature_store/data_sources/batch_sources/big_query.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/feature_store/data_sources/batch_sources/csv.py` & `qwak_core-0.0.96/qwak/feature_store/data_sources/batch_sources/csv.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/feature_store/data_sources/batch_sources/elastic_search.py` & `qwak_core-0.0.96/qwak/feature_store/data_sources/batch_sources/elastic_search.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/feature_store/data_sources/batch_sources/filesystem_config.py` & `qwak_core-0.0.96/qwak/feature_store/data_sources/batch_sources/filesystem_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/feature_store/data_sources/batch_sources/mongodb.py` & `qwak_core-0.0.96/qwak/feature_store/data_sources/batch_sources/mongodb.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/feature_store/data_sources/batch_sources/mysql.py` & `qwak_core-0.0.96/qwak/feature_store/data_sources/batch_sources/mysql.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/feature_store/data_sources/batch_sources/parquet.py` & `qwak_core-0.0.96/qwak/feature_store/data_sources/batch_sources/parquet.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/feature_store/data_sources/batch_sources/postgres.py` & `qwak_core-0.0.96/qwak/feature_store/data_sources/batch_sources/postgres.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/feature_store/data_sources/batch_sources/redshift.py` & `qwak_core-0.0.96/qwak/feature_store/data_sources/batch_sources/redshift.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/feature_store/data_sources/batch_sources/snowflake.py` & `qwak_core-0.0.96/qwak/feature_store/data_sources/batch_sources/snowflake.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/feature_store/data_sources/batch_sources/vertica.py` & `qwak_core-0.0.96/qwak/feature_store/data_sources/batch_sources/vertica.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/feature_store/entities/entity.py` & `qwak_core-0.0.96/qwak/feature_store/entities/entity.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/feature_store/feature_sets/backfill.py` & `qwak_core-0.0.96/qwak/feature_store/feature_sets/backfill.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/feature_store/feature_sets/batch.py` & `qwak_core-0.0.96/qwak/feature_store/feature_sets/batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/feature_store/feature_sets/execution_spec.py` & `qwak_core-0.0.96/qwak/feature_store/feature_sets/execution_spec.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/feature_store/feature_sets/metadata.py` & `qwak_core-0.0.96/qwak/feature_store/feature_sets/metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/feature_store/feature_sets/read_policies.py` & `qwak_core-0.0.96/qwak/feature_store/feature_sets/read_policies.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/feature_store/feature_sets/transformations.py` & `qwak_core-0.0.96/qwak/feature_store/feature_sets/transformations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/feature_store/offline/_query_engine.py` & `qwak_core-0.0.96/qwak/feature_store/offline/_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/feature_store/offline/athena/athena_query_engine.py` & `qwak_core-0.0.96/qwak/feature_store/offline/athena/athena_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/feature_store/offline/client.py` & `qwak_core-0.0.96/qwak/feature_store/offline/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/feature_store/online/client.py` & `qwak_core-0.0.96/qwak/feature_store/online/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/inner/const.py` & `qwak_core-0.0.96/qwak/inner/const.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/inner/di_configuration/__init__.py` & `qwak_core-0.0.96/qwak/inner/di_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/inner/di_configuration/account.py` & `qwak_core-0.0.96/qwak/inner/di_configuration/account.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/inner/di_configuration/containers.py` & `qwak_core-0.0.96/qwak/inner/di_configuration/containers.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/inner/model_loggers_utils.py` & `qwak_core-0.0.96/qwak/inner/model_loggers_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/inner/singleton_meta.py` & `qwak_core-0.0.96/qwak/inner/singleton_meta.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/inner/tool/auth.py` & `qwak_core-0.0.96/qwak/inner/tool/auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/inner/tool/grpc/grpc_auth.py` & `qwak_core-0.0.96/qwak/inner/tool/grpc/grpc_auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/inner/tool/grpc/grpc_tools.py` & `qwak_core-0.0.96/qwak/inner/tool/grpc/grpc_tools.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/inner/tool/run_config/base.py` & `qwak_core-0.0.96/qwak/inner/tool/run_config/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/inner/tool/run_config/utils.py` & `qwak_core-0.0.96/qwak/inner/tool/run_config/utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/model/adapters/__init__.py` & `qwak_core-0.0.96/qwak/model/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/model/adapters/input_adapters/multi_input_adapter.py` & `qwak_core-0.0.96/qwak/model/adapters/input_adapters/multi_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/model/adapters/input_adapters/numpy_input_adapter.py` & `qwak_core-0.0.96/qwak/model/adapters/input_adapters/numpy_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/model/adapters/input_adapters/proto_input_adapter.py` & `qwak_core-0.0.96/qwak/model/adapters/input_adapters/proto_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/model/adapters/output_adapters/numpy_output_adapter.py` & `qwak_core-0.0.96/qwak/model/adapters/output_adapters/numpy_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/model/adapters/output_adapters/proto_output_adapter.py` & `qwak_core-0.0.96/qwak/model/adapters/output_adapters/proto_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/model/base.py` & `qwak_core-0.0.96/qwak/model/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/model/decorators/api.py` & `qwak_core-0.0.96/qwak/model/decorators/api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/model/decorators/api_implementation.py` & `qwak_core-0.0.96/qwak/model/decorators/api_implementation.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/model/experiment_tracking.py` & `qwak_core-0.0.96/qwak/model/experiment_tracking.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/model/schema.py` & `qwak_core-0.0.96/qwak/model/schema.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/model/schema_entities.py` & `qwak_core-0.0.96/qwak/model/schema_entities.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/model/tools/adapters/encoders.py` & `qwak_core-0.0.96/qwak/model/tools/adapters/encoders.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/model/tools/adapters/input.py` & `qwak_core-0.0.96/qwak/model/tools/adapters/input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/model/tools/adapters/input_adapters/base_input.py` & `qwak_core-0.0.96/qwak/model/tools/adapters/input_adapters/base_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/model/tools/adapters/input_adapters/dataframe_input.py` & `qwak_core-0.0.96/qwak/model/tools/adapters/input_adapters/dataframe_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/model/tools/adapters/input_adapters/image_input.py` & `qwak_core-0.0.96/qwak/model/tools/adapters/input_adapters/image_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/model/tools/adapters/input_adapters/json_input.py` & `qwak_core-0.0.96/qwak/model/tools/adapters/input_adapters/json_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py` & `qwak_core-0.0.96/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/model/tools/adapters/output.py` & `qwak_core-0.0.96/qwak/model/tools/adapters/output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/model/tools/adapters/output_adapters/dataframe_output.py` & `qwak_core-0.0.96/qwak/model/tools/adapters/output_adapters/dataframe_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/model/tools/adapters/output_adapters/default_output.py` & `qwak_core-0.0.96/qwak/model/tools/adapters/output_adapters/default_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/model/tools/adapters/output_adapters/json_output.py` & `qwak_core-0.0.96/qwak/model/tools/adapters/output_adapters/json_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py` & `qwak_core-0.0.96/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/model/tools/run_model_locally.py` & `qwak_core-0.0.96/qwak/model/tools/run_model_locally.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/model_loggers/artifact_logger.py` & `qwak_core-0.0.96/qwak/model_loggers/artifact_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/model_loggers/data_logger.py` & `qwak_core-0.0.96/qwak/model_loggers/data_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/model_loggers/model_logger.py` & `qwak_core-0.0.96/qwak/model_loggers/model_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/qwak_client/builds/build.py` & `qwak_core-0.0.96/qwak/qwak_client/builds/build.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/qwak_client/builds/filters/metric_filter.py` & `qwak_core-0.0.96/qwak/qwak_client/builds/filters/metric_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/qwak_client/builds/filters/parameter_filter.py` & `qwak_core-0.0.96/qwak/qwak_client/builds/filters/parameter_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/qwak_client/client.py` & `qwak_core-0.0.96/qwak/qwak_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/qwak_client/deployments/deployment.py` & `qwak_core-0.0.96/qwak/qwak_client/deployments/deployment.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/qwak_client/models/model.py` & `qwak_core-0.0.96/qwak/qwak_client/models/model.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/qwak_client/models/model_metadata.py` & `qwak_core-0.0.96/qwak/qwak_client/models/model_metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/qwak_client/projects/project.py` & `qwak_core-0.0.96/qwak/qwak_client/projects/project.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/tools/logger/logger.py` & `qwak_core-0.0.96/qwak/tools/logger/logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak/tools/logger/logging.yml` & `qwak_core-0.0.96/qwak/tools/logger/logging.yml`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak_services_mock/mocks/alert_manager_service_api.py` & `qwak_core-0.0.96/qwak_services_mock/mocks/alert_manager_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak_services_mock/mocks/analytics_api.py` & `qwak_core-0.0.96/qwak_services_mock/mocks/analytics_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak_services_mock/mocks/audience_service_api.py` & `qwak_core-0.0.96/qwak_services_mock/mocks/audience_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak_services_mock/mocks/authentication_service.py` & `qwak_core-0.0.96/qwak_services_mock/mocks/authentication_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak_services_mock/mocks/automation_management_service.py` & `qwak_core-0.0.96/qwak_services_mock/mocks/automation_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak_services_mock/mocks/autoscaling_service_api.py` & `qwak_core-0.0.96/qwak_services_mock/mocks/autoscaling_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak_services_mock/mocks/batch_job_manager_service.py` & `qwak_core-0.0.96/qwak_services_mock/mocks/batch_job_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak_services_mock/mocks/build_management.py` & `qwak_core-0.0.96/qwak_services_mock/mocks/build_management.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak_services_mock/mocks/build_orchestrator_build_api.py` & `qwak_core-0.0.96/qwak_services_mock/mocks/build_orchestrator_build_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak_services_mock/mocks/build_orchestrator_service_api.py` & `qwak_core-0.0.96/qwak_services_mock/mocks/build_orchestrator_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak_services_mock/mocks/data_versioning_service.py` & `qwak_core-0.0.96/qwak_services_mock/mocks/data_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak_services_mock/mocks/deployment_management_service.py` & `qwak_core-0.0.96/qwak_services_mock/mocks/deployment_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak_services_mock/mocks/ecosystem_service_api.py` & `qwak_core-0.0.96/qwak_services_mock/mocks/ecosystem_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py` & `qwak_core-0.0.96/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak_services_mock/mocks/feature_store_entities_manager_api.py` & `qwak_core-0.0.96/qwak_services_mock/mocks/feature_store_entities_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py` & `qwak_core-0.0.96/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak_services_mock/mocks/features_online_serving_api.py` & `qwak_core-0.0.96/qwak_services_mock/mocks/features_online_serving_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak_services_mock/mocks/features_operator_v3_service.py` & `qwak_core-0.0.96/qwak_services_mock/mocks/features_operator_v3_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak_services_mock/mocks/features_set_state_service_api.py` & `qwak_core-0.0.96/qwak_services_mock/mocks/features_set_state_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak_services_mock/mocks/feedback_service.py` & `qwak_core-0.0.96/qwak_services_mock/mocks/feedback_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak_services_mock/mocks/file_versioning_service.py` & `qwak_core-0.0.96/qwak_services_mock/mocks/file_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak_services_mock/mocks/instance_template_management_service.py` & `qwak_core-0.0.96/qwak_services_mock/mocks/instance_template_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak_services_mock/mocks/job_registry_service_api.py` & `qwak_core-0.0.96/qwak_services_mock/mocks/job_registry_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak_services_mock/mocks/kube_captain_service_api.py` & `qwak_core-0.0.96/qwak_services_mock/mocks/kube_captain_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak_services_mock/mocks/logging_service.py` & `qwak_core-0.0.96/qwak_services_mock/mocks/logging_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak_services_mock/mocks/model_management_service.py` & `qwak_core-0.0.96/qwak_services_mock/mocks/model_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak_services_mock/mocks/project_manager_service.py` & `qwak_core-0.0.96/qwak_services_mock/mocks/project_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak_services_mock/mocks/qwak_mocks.py` & `qwak_core-0.0.96/qwak_services_mock/mocks/qwak_mocks.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak_services_mock/mocks/secret_service.py` & `qwak_core-0.0.96/qwak_services_mock/mocks/secret_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak_services_mock/mocks/self_service_user_service.py` & `qwak_core-0.0.96/qwak_services_mock/mocks/self_service_user_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak_services_mock/mocks/user_application_instance_service_api.py` & `qwak_core-0.0.96/qwak_services_mock/mocks/user_application_instance_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/qwak_services_mock/services_mock.py` & `qwak_core-0.0.96/qwak_services_mock/services_mock.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.95/setup.py` & `qwak_core-0.0.96/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,15 @@
  'typeguard>=2,<3']
 
 extras_require = \
 {'feature-store': ['pyarrow>=6.0.0', 'pyathena>=2.2.0,!=2.18.0']}
 
 setup_kwargs = {
     'name': 'qwak-core',
-    'version': '0.0.95',
+    'version': '0.0.96',
     'description': 'Qwak Core contains the necessary objects and communication tools for using the Qwak Platform',
     'long_description': '# Qwak Core\n\nQwak is an end-to-end production ML platform designed to allow data scientists to build, deploy, and monitor their models in production with minimal engineering friction.\nQwak Core contains all the objects and tools necessary to use the Qwak Platform\n',
     'author': 'Qwak',
     'author_email': 'info@qwak.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `qwak_core-0.0.95/PKG-INFO` & `qwak_core-0.0.96/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwak-core
-Version: 0.0.95
+Version: 0.0.96
 Summary: Qwak Core contains the necessary objects and communication tools for using the Qwak Platform
 License: Apache-2.0
 Keywords: mlops,ml,deployment,serving,model
 Author: Qwak
 Author-email: info@qwak.com
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

