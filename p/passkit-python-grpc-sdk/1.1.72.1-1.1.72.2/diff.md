# Comparing `tmp/passkit_python_grpc_sdk-1.1.72.1.tar.gz` & `tmp/passkit-python-grpc-sdk-1.1.72.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "passkit-python-grpc-sdk-1.1.72.2.tar", last modified: Mon Jun  5 10:49:42 2023, max compression
```

## Comparing `passkit_python_grpc_sdk-1.1.72.1.tar` & `passkit-python-grpc-sdk-1.1.72.2.tar`

### file list

```diff
@@ -1,151 +1,165 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/__init__.py
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/readMe.md
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/setup.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/ct/scheduler/__init__.py
--rw-r--r--   0        0        0     5059 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/ct/scheduler/scheduler_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/ct/scheduler/scheduler_pb2_grpc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/analytics/__init__.py
--rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/analytics/a_rpc_pb2.py
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/analytics/a_rpc_pb2_grpc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/certificate/__init__.py
--rw-r--r--   0        0        0     3683 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/certificate/certificate_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/certificate/certificate_pb2_grpc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/common/__init__.py
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/common/attributes_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/common/attributes_pb2_grpc.py
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/common/billing_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/common/billing_pb2_grpc.py
--rw-r--r--   0        0        0     8103 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/common/common_objects_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/common/common_objects_pb2_grpc.py
--rw-r--r--   0        0        0     8056 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/common/distribution_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/common/distribution_pb2_grpc.py
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/common/expiry_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/common/expiry_pb2_grpc.py
--rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/common/filter_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/common/filter_pb2_grpc.py
--rw-r--r--   0        0        0    11757 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/common/integration_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/common/integration_pb2_grpc.py
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/common/links_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/common/links_pb2_grpc.py
--rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/common/localization_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/common/localization_pb2_grpc.py
--rw-r--r--   0        0        0     4101 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/common/message_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/common/message_pb2_grpc.py
--rw-r--r--   0        0        0     4831 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/common/metrics_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/common/metrics_pb2_grpc.py
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/common/note_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/common/note_pb2_grpc.py
--rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/common/pagination_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/common/pagination_pb2_grpc.py
--rw-r--r--   0        0        0     3868 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/common/pass_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/common/pass_pb2_grpc.py
--rw-r--r--   0        0        0     2960 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/common/personal_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/common/personal_pb2_grpc.py
--rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/common/project_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/common/project_pb2_grpc.py
--rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/common/protocols_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/common/protocols_pb2_grpc.py
--rw-r--r--   0        0        0     3974 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/common/proximity_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/common/proximity_pb2_grpc.py
--rw-r--r--   0        0        0     6955 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/common/reporting_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/common/reporting_pb2_grpc.py
--rw-r--r--   0        0        0    27313 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/common/template_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/common/template_pb2_grpc.py
--rw-r--r--   0        0        0     4777 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/common/tracking_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/common/tracking_pb2_grpc.py
--rw-r--r--   0        0        0     3282 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/common/transaction_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/common/transaction_pb2_grpc.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/common/useragent_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/common/useragent_pb2_grpc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/core/__init__.py
--rw-r--r--   0        0        0     9673 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/core/a_rpc_certificates_pb2.py
--rw-r--r--   0        0        0    16842 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/core/a_rpc_certificates_pb2_grpc.py
--rw-r--r--   0        0        0     8692 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/core/a_rpc_distribution_pb2.py
--rw-r--r--   0        0        0    11237 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/core/a_rpc_distribution_pb2_grpc.py
--rw-r--r--   0        0        0    14027 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/core/a_rpc_images_pb2.py
--rw-r--r--   0        0        0    33423 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/core/a_rpc_images_pb2_grpc.py
--rw-r--r--   0        0        0     4523 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/core/a_rpc_messages_pb2.py
--rw-r--r--   0        0        0     9017 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/core/a_rpc_messages_pb2_grpc.py
--rw-r--r--   0        0        0    23117 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/core/a_rpc_others_pb2.py
--rw-r--r--   0        0        0    64337 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/core/a_rpc_others_pb2_grpc.py
--rw-r--r--   0        0        0    35407 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/core/a_rpc_templates_pb2.py
--rw-r--r--   0        0        0    67418 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/core/a_rpc_templates_pb2_grpc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/event_tickets/__init__.py
--rw-r--r--   0        0        0    36045 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/event_tickets/a_rpc_pb2.py
--rw-r--r--   0        0        0    73514 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/event_tickets/a_rpc_pb2_grpc.py
--rw-r--r--   0        0        0     8777 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/event_tickets/event_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/event_tickets/event_pb2_grpc.py
--rw-r--r--   0        0        0     5862 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/event_tickets/production_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/event_tickets/production_pb2_grpc.py
--rw-r--r--   0        0        0    17226 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/event_tickets/ticket_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/event_tickets/ticket_pb2_grpc.py
--rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/event_tickets/ticket_type_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/event_tickets/ticket_type_pb2_grpc.py
--rw-r--r--   0        0        0     3579 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/event_tickets/venue_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/event_tickets/venue_pb2_grpc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/flights/__init__.py
--rw-r--r--   0        0        0    23535 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/flights/a_rpc_pb2.py
--rw-r--r--   0        0        0    36450 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/flights/a_rpc_pb2_grpc.py
--rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/flights/airport_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/flights/airport_pb2_grpc.py
--rw-r--r--   0        0        0     6183 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/flights/barcode_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/flights/barcode_pb2_grpc.py
--rw-r--r--   0        0        0    13526 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/flights/boarding_pass_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/flights/boarding_pass_pb2_grpc.py
--rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/flights/carrier_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/flights/carrier_pb2_grpc.py
--rw-r--r--   0        0        0     9069 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/flights/flight_designator_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/flights/flight_designator_pb2_grpc.py
--rw-r--r--   0        0        0     8262 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/flights/flight_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/flights/flight_pb2_grpc.py
--rw-r--r--   0        0        0     4630 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/flights/passenger_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/flights/passenger_pb2_grpc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/flights/cabin_codes/__init__.py
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/flights/cabin_codes/cabin_codes_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/flights/cabin_codes/cabin_codes_pb2_grpc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/image/__init__.py
--rw-r--r--   0        0        0     9318 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/image/image_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/image/image_pb2_grpc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/member/__init__.py
--rw-r--r--   0        0        0    33471 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/member/a_rpc_pb2.py
--rw-r--r--   0        0        0    73596 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/member/a_rpc_pb2_grpc.py
--rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/member/event_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/member/event_pb2_grpc.py
--rw-r--r--   0        0        0     3948 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/member/member_events_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/member/member_events_pb2_grpc.py
--rw-r--r--   0        0        0     8953 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/member/member_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/member/member_pb2_grpc.py
--rw-r--r--   0        0        0     7178 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/member/program_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/member/program_pb2_grpc.py
--rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/member/tier_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/member/tier_pb2_grpc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/raw/__init__.py
--rw-r--r--   0        0        0    10381 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/raw/a_rpc_pb2.py
--rw-r--r--   0        0        0    21771 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/raw/a_rpc_pb2_grpc.py
--rw-r--r--   0        0        0     4136 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/raw/pass_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/raw/pass_pb2_grpc.py
--rw-r--r--   0        0        0     3259 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/raw/project_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/raw/project_pb2_grpc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/scheduler/__init__.py
--rw-r--r--   0        0        0     9176 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/scheduler/a_rpc_pb2.py
--rw-r--r--   0        0        0    13051 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/scheduler/a_rpc_pb2_grpc.py
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/scheduler/scheduler_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/scheduler/scheduler_pb2_grpc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/single_use_coupons/__init__.py
--rw-r--r--   0        0        0    27529 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/single_use_coupons/a_rpc_pb2.py
--rw-r--r--   0        0        0    52128 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/single_use_coupons/a_rpc_pb2_grpc.py
--rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/single_use_coupons/campaign_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/single_use_coupons/campaign_pb2_grpc.py
--rw-r--r--   0        0        0     5693 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/single_use_coupons/coupon_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/single_use_coupons/coupon_pb2_grpc.py
--rw-r--r--   0        0        0    10828 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/single_use_coupons/offer_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/single_use_coupons/offer_pb2_grpc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/user/__init__.py
--rw-r--r--   0        0        0     7564 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/user/user_pb2.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/io/user/user_pb2_grpc.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/.gitignore
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/pyproject.toml
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/readME.md
--rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 passkit_python_grpc_sdk-1.1.72.1/PKG-INFO
+drwxr-xr-x   0 claudia    (501) staff       (20)        0 2023-06-05 10:49:42.417741 passkit-python-grpc-sdk-1.1.72.2/
+-rw-r--r--   0 claudia    (501) staff       (20)     1916 2023-06-05 10:49:42.417177 passkit-python-grpc-sdk-1.1.72.2/PKG-INFO
+drwxr-xr-x   0 claudia    (501) staff       (20)        0 2023-06-05 10:49:42.191815 passkit-python-grpc-sdk-1.1.72.2/io/
+-rw-r--r--   0 claudia    (501) staff       (20)        0 2023-02-24 08:09:05.000000 passkit-python-grpc-sdk-1.1.72.2/io/__init__.py
+drwxr-xr-x   0 claudia    (501) staff       (20)        0 2023-06-05 10:49:42.193878 passkit-python-grpc-sdk-1.1.72.2/io/analytics/
+-rw-r--r--   0 claudia    (501) staff       (20)        0 2023-02-24 08:02:31.000000 passkit-python-grpc-sdk-1.1.72.2/io/analytics/__init__.py
+-rw-r--r--   0 claudia    (501) staff       (20)     4504 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/analytics/a_rpc_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)     2599 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/analytics/a_rpc_pb2_grpc.py
+drwxr-xr-x   0 claudia    (501) staff       (20)        0 2023-06-05 10:49:42.195941 passkit-python-grpc-sdk-1.1.72.2/io/certificate/
+-rw-r--r--   0 claudia    (501) staff       (20)        0 2023-02-24 08:02:35.000000 passkit-python-grpc-sdk-1.1.72.2/io/certificate/__init__.py
+-rw-r--r--   0 claudia    (501) staff       (20)     3683 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/certificate/certificate_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)      159 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/certificate/certificate_pb2_grpc.py
+drwxr-xr-x   0 claudia    (501) staff       (20)        0 2023-06-05 10:49:42.269823 passkit-python-grpc-sdk-1.1.72.2/io/common/
+-rw-r--r--   0 claudia    (501) staff       (20)        0 2023-02-24 08:02:38.000000 passkit-python-grpc-sdk-1.1.72.2/io/common/__init__.py
+-rw-r--r--   0 claudia    (501) staff       (20)     1637 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/common/attributes_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)      159 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/common/attributes_pb2_grpc.py
+-rw-r--r--   0 claudia    (501) staff       (20)     1693 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/common/billing_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)      159 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/common/billing_pb2_grpc.py
+-rw-r--r--   0 claudia    (501) staff       (20)     8103 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/common/common_objects_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)      159 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/common/common_objects_pb2_grpc.py
+-rw-r--r--   0 claudia    (501) staff       (20)     8056 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/common/distribution_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)      159 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/common/distribution_pb2_grpc.py
+-rw-r--r--   0 claudia    (501) staff       (20)     1814 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/common/expiry_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)      159 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/common/expiry_pb2_grpc.py
+-rw-r--r--   0 claudia    (501) staff       (20)     2384 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/common/filter_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)      159 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/common/filter_pb2_grpc.py
+-rw-r--r--   0 claudia    (501) staff       (20)    11757 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/common/integration_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)      159 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/common/integration_pb2_grpc.py
+-rw-r--r--   0 claudia    (501) staff       (20)     2163 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/common/links_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)      159 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/common/links_pb2_grpc.py
+-rw-r--r--   0 claudia    (501) staff       (20)     2823 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/common/localization_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)      159 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/common/localization_pb2_grpc.py
+-rw-r--r--   0 claudia    (501) staff       (20)     4101 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/common/message_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)      159 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/common/message_pb2_grpc.py
+-rw-r--r--   0 claudia    (501) staff       (20)     4831 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/common/metrics_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)      159 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/common/metrics_pb2_grpc.py
+-rw-r--r--   0 claudia    (501) staff       (20)     1433 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/common/note_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)      159 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/common/note_pb2_grpc.py
+-rw-r--r--   0 claudia    (501) staff       (20)     2074 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/common/pagination_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)      159 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/common/pagination_pb2_grpc.py
+-rw-r--r--   0 claudia    (501) staff       (20)     3868 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/common/pass_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)      159 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/common/pass_pb2_grpc.py
+-rw-r--r--   0 claudia    (501) staff       (20)     2960 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/common/personal_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)      159 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/common/personal_pb2_grpc.py
+-rw-r--r--   0 claudia    (501) staff       (20)     2695 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/common/project_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)      159 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/common/project_pb2_grpc.py
+-rw-r--r--   0 claudia    (501) staff       (20)     1970 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/common/protocols_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)      159 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/common/protocols_pb2_grpc.py
+-rw-r--r--   0 claudia    (501) staff       (20)     3974 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/common/proximity_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)      159 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/common/proximity_pb2_grpc.py
+-rw-r--r--   0 claudia    (501) staff       (20)     6955 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/common/reporting_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)      159 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/common/reporting_pb2_grpc.py
+-rw-r--r--   0 claudia    (501) staff       (20)    27313 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/common/template_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)      159 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/common/template_pb2_grpc.py
+-rw-r--r--   0 claudia    (501) staff       (20)     4777 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/common/tracking_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)      159 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/common/tracking_pb2_grpc.py
+-rw-r--r--   0 claudia    (501) staff       (20)     3282 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/common/transaction_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)      159 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/common/transaction_pb2_grpc.py
+-rw-r--r--   0 claudia    (501) staff       (20)     1629 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/common/useragent_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)      159 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/common/useragent_pb2_grpc.py
+drwxr-xr-x   0 claudia    (501) staff       (20)        0 2023-06-05 10:49:42.292998 passkit-python-grpc-sdk-1.1.72.2/io/core/
+-rw-r--r--   0 claudia    (501) staff       (20)        0 2023-02-24 08:02:47.000000 passkit-python-grpc-sdk-1.1.72.2/io/core/__init__.py
+-rw-r--r--   0 claudia    (501) staff       (20)     9673 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/core/a_rpc_certificates_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)    16842 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/core/a_rpc_certificates_pb2_grpc.py
+-rw-r--r--   0 claudia    (501) staff       (20)     8692 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/core/a_rpc_distribution_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)    11237 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/core/a_rpc_distribution_pb2_grpc.py
+-rw-r--r--   0 claudia    (501) staff       (20)    14027 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/core/a_rpc_images_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)    33423 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/core/a_rpc_images_pb2_grpc.py
+-rw-r--r--   0 claudia    (501) staff       (20)     4523 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/core/a_rpc_messages_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)     9017 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/core/a_rpc_messages_pb2_grpc.py
+-rw-r--r--   0 claudia    (501) staff       (20)    23117 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/core/a_rpc_others_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)    64337 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/core/a_rpc_others_pb2_grpc.py
+-rw-r--r--   0 claudia    (501) staff       (20)    35407 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/core/a_rpc_templates_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)    67418 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/core/a_rpc_templates_pb2_grpc.py
+drwxr-xr-x   0 claudia    (501) staff       (20)        0 2023-06-05 10:49:42.312093 passkit-python-grpc-sdk-1.1.72.2/io/event_tickets/
+-rw-r--r--   0 claudia    (501) staff       (20)        0 2023-02-24 08:02:50.000000 passkit-python-grpc-sdk-1.1.72.2/io/event_tickets/__init__.py
+-rw-r--r--   0 claudia    (501) staff       (20)    36045 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/event_tickets/a_rpc_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)    73514 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/event_tickets/a_rpc_pb2_grpc.py
+-rw-r--r--   0 claudia    (501) staff       (20)     8777 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/event_tickets/event_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)      159 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/event_tickets/event_pb2_grpc.py
+-rw-r--r--   0 claudia    (501) staff       (20)     5862 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/event_tickets/production_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)      159 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/event_tickets/production_pb2_grpc.py
+-rw-r--r--   0 claudia    (501) staff       (20)    17226 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/event_tickets/ticket_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)      159 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/event_tickets/ticket_pb2_grpc.py
+-rw-r--r--   0 claudia    (501) staff       (20)     4473 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/event_tickets/ticket_type_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)      159 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/event_tickets/ticket_type_pb2_grpc.py
+-rw-r--r--   0 claudia    (501) staff       (20)     3579 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/event_tickets/venue_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)      159 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/event_tickets/venue_pb2_grpc.py
+drwxr-xr-x   0 claudia    (501) staff       (20)        0 2023-06-05 10:49:42.336045 passkit-python-grpc-sdk-1.1.72.2/io/flights/
+-rw-r--r--   0 claudia    (501) staff       (20)        0 2023-02-24 08:02:55.000000 passkit-python-grpc-sdk-1.1.72.2/io/flights/__init__.py
+-rw-r--r--   0 claudia    (501) staff       (20)    23535 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/flights/a_rpc_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)    36450 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/flights/a_rpc_pb2_grpc.py
+-rw-r--r--   0 claudia    (501) staff       (20)     2913 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/flights/airport_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)      159 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/flights/airport_pb2_grpc.py
+-rw-r--r--   0 claudia    (501) staff       (20)     6183 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/flights/barcode_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)      159 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/flights/barcode_pb2_grpc.py
+-rw-r--r--   0 claudia    (501) staff       (20)    13526 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/flights/boarding_pass_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)      159 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/flights/boarding_pass_pb2_grpc.py
+drwxr-xr-x   0 claudia    (501) staff       (20)        0 2023-06-05 10:49:42.372708 passkit-python-grpc-sdk-1.1.72.2/io/flights/cabin_codes/
+-rw-r--r--   0 claudia    (501) staff       (20)        0 2023-02-24 08:02:58.000000 passkit-python-grpc-sdk-1.1.72.2/io/flights/cabin_codes/__init__.py
+-rw-r--r--   0 claudia    (501) staff       (20)     1993 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/flights/cabin_codes/cabin_codes_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)      159 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/flights/cabin_codes/cabin_codes_pb2_grpc.py
+-rw-r--r--   0 claudia    (501) staff       (20)     3389 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/flights/carrier_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)      159 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/flights/carrier_pb2_grpc.py
+-rw-r--r--   0 claudia    (501) staff       (20)     9069 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/flights/flight_designator_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)      159 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/flights/flight_designator_pb2_grpc.py
+-rw-r--r--   0 claudia    (501) staff       (20)     8262 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/flights/flight_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)      159 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/flights/flight_pb2_grpc.py
+-rw-r--r--   0 claudia    (501) staff       (20)     4630 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/flights/passenger_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)      159 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/flights/passenger_pb2_grpc.py
+drwxr-xr-x   0 claudia    (501) staff       (20)        0 2023-06-05 10:49:42.375015 passkit-python-grpc-sdk-1.1.72.2/io/image/
+-rw-r--r--   0 claudia    (501) staff       (20)        0 2023-02-24 08:03:06.000000 passkit-python-grpc-sdk-1.1.72.2/io/image/__init__.py
+-rw-r--r--   0 claudia    (501) staff       (20)     9318 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/image/image_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)      159 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/image/image_pb2_grpc.py
+drwxr-xr-x   0 claudia    (501) staff       (20)        0 2023-06-05 10:49:42.390542 passkit-python-grpc-sdk-1.1.72.2/io/member/
+-rw-r--r--   0 claudia    (501) staff       (20)        0 2023-02-24 08:03:11.000000 passkit-python-grpc-sdk-1.1.72.2/io/member/__init__.py
+-rw-r--r--   0 claudia    (501) staff       (20)    33471 2023-02-27 08:33:35.000000 passkit-python-grpc-sdk-1.1.72.2/io/member/a_rpc_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)    73596 2023-02-27 08:33:38.000000 passkit-python-grpc-sdk-1.1.72.2/io/member/a_rpc_pb2_grpc.py
+-rw-r--r--   0 claudia    (501) staff       (20)     1940 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/member/event_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)      159 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/member/event_pb2_grpc.py
+-rw-r--r--   0 claudia    (501) staff       (20)     3948 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/member/member_events_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)      159 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/member/member_events_pb2_grpc.py
+-rw-r--r--   0 claudia    (501) staff       (20)     8953 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/member/member_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)      159 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/member/member_pb2_grpc.py
+-rw-r--r--   0 claudia    (501) staff       (20)     7178 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/member/program_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)      159 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/member/program_pb2_grpc.py
+-rw-r--r--   0 claudia    (501) staff       (20)     3532 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/member/tier_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)      159 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/member/tier_pb2_grpc.py
+drwxr-xr-x   0 claudia    (501) staff       (20)        0 2023-06-05 10:49:42.397470 passkit-python-grpc-sdk-1.1.72.2/io/raw/
+-rw-r--r--   0 claudia    (501) staff       (20)        0 2023-02-24 08:03:14.000000 passkit-python-grpc-sdk-1.1.72.2/io/raw/__init__.py
+-rw-r--r--   0 claudia    (501) staff       (20)    10381 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/raw/a_rpc_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)    21771 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/raw/a_rpc_pb2_grpc.py
+-rw-r--r--   0 claudia    (501) staff       (20)     4136 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/raw/pass_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)      159 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/raw/pass_pb2_grpc.py
+-rw-r--r--   0 claudia    (501) staff       (20)     3259 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/raw/project_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)      159 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/raw/project_pb2_grpc.py
+drwxr-xr-x   0 claudia    (501) staff       (20)        0 2023-06-05 10:49:42.402422 passkit-python-grpc-sdk-1.1.72.2/io/scheduler/
+-rw-r--r--   0 claudia    (501) staff       (20)        0 2023-02-24 08:03:18.000000 passkit-python-grpc-sdk-1.1.72.2/io/scheduler/__init__.py
+-rw-r--r--   0 claudia    (501) staff       (20)     9176 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/scheduler/a_rpc_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)    13051 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/scheduler/a_rpc_pb2_grpc.py
+-rw-r--r--   0 claudia    (501) staff       (20)     1425 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/scheduler/scheduler_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)      159 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/scheduler/scheduler_pb2_grpc.py
+drwxr-xr-x   0 claudia    (501) staff       (20)        0 2023-06-05 10:49:42.410319 passkit-python-grpc-sdk-1.1.72.2/io/single_use_coupons/
+-rw-r--r--   0 claudia    (501) staff       (20)        0 2023-02-24 08:03:23.000000 passkit-python-grpc-sdk-1.1.72.2/io/single_use_coupons/__init__.py
+-rw-r--r--   0 claudia    (501) staff       (20)    27529 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/single_use_coupons/a_rpc_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)    52128 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/single_use_coupons/a_rpc_pb2_grpc.py
+-rw-r--r--   0 claudia    (501) staff       (20)     4095 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/single_use_coupons/campaign_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)      159 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/single_use_coupons/campaign_pb2_grpc.py
+-rw-r--r--   0 claudia    (501) staff       (20)     5693 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/single_use_coupons/coupon_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)      159 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/single_use_coupons/coupon_pb2_grpc.py
+-rw-r--r--   0 claudia    (501) staff       (20)    10828 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/single_use_coupons/offer_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)      159 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/single_use_coupons/offer_pb2_grpc.py
+drwxr-xr-x   0 claudia    (501) staff       (20)        0 2023-06-05 10:49:42.412254 passkit-python-grpc-sdk-1.1.72.2/io/user/
+-rw-r--r--   0 claudia    (501) staff       (20)        0 2023-02-24 08:03:29.000000 passkit-python-grpc-sdk-1.1.72.2/io/user/__init__.py
+-rw-r--r--   0 claudia    (501) staff       (20)     7564 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/user/user_pb2.py
+-rw-r--r--   0 claudia    (501) staff       (20)      159 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/io/user/user_pb2_grpc.py
+drwxr-xr-x   0 claudia    (501) staff       (20)        0 2023-06-05 10:49:42.415842 passkit-python-grpc-sdk-1.1.72.2/passkit_python_grpc_sdk.egg-info/
+-rw-r--r--   0 claudia    (501) staff       (20)     1916 2023-06-05 10:49:42.000000 passkit-python-grpc-sdk-1.1.72.2/passkit_python_grpc_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 claudia    (501) staff       (20)     4393 2023-06-05 10:49:42.000000 passkit-python-grpc-sdk-1.1.72.2/passkit_python_grpc_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 claudia    (501) staff       (20)        1 2023-06-05 10:49:42.000000 passkit-python-grpc-sdk-1.1.72.2/passkit_python_grpc_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 claudia    (501) staff       (20)        3 2023-06-05 10:49:42.000000 passkit-python-grpc-sdk-1.1.72.2/passkit_python_grpc_sdk.egg-info/top_level.txt
+-rw-r--r--   0 claudia    (501) staff       (20)      687 2023-06-05 10:44:25.000000 passkit-python-grpc-sdk-1.1.72.2/pyproject.toml
+-rw-r--r--   0 claudia    (501) staff       (20)     1294 2023-02-24 08:00:59.000000 passkit-python-grpc-sdk-1.1.72.2/readME.md
+-rw-r--r--   0 claudia    (501) staff       (20)       38 2023-06-05 10:49:42.418406 passkit-python-grpc-sdk-1.1.72.2/setup.cfg
+-rw-r--r--   0 claudia    (501) staff       (20)      527 2023-06-05 10:44:23.000000 passkit-python-grpc-sdk-1.1.72.2/setup.py
```

### Comparing `passkit_python_grpc_sdk-1.1.72.1/readMe.md` & `passkit-python-grpc-sdk-1.1.72.2/readME.md`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/ct/scheduler/scheduler_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/flights/passenger_pb2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,40 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: ct/scheduler/scheduler.proto
+# source: io/flights/passenger.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from io.flights import barcode_pb2 as io_dot_flights_dot_barcode__pb2
+from io.common import common_objects_pb2 as io_dot_common_dot_common__objects__pb2
+from io.common import personal_pb2 as io_dot_common_dot_personal__pb2
 from protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
-from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1c\x63t/scheduler/scheduler.proto\x12\x02\x63t\x1a.protoc-gen-openapiv2/options/annotations.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\x86\x04\n\rSchedulingJob\x12\n\n\x02id\x18\x01 \x01(\t\x12\x13\n\x0bjobFunction\x18\x02 \x01(\t\x12\x12\n\njobPayload\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x05 \x01(\t\x12\x1e\n\x08schedule\x18\x06 \x01(\x0b\x32\x0c.ct.Schedule\x12\x1d\n\x06status\x18\x07 \x01(\x0e\x32\r.ct.JobStatus\x12\x33\n\x0fnextRunDatetime\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x33\n\x0flastRunDatetime\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1c\n\x04logs\x18\n \x03(\x0b\x32\x0e.ct.JobHistory\x12+\n\x07\x63reated\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12+\n\x07updated\x18\x0c \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12*\n\x06\x65xpiry\x18\r \x01(\x0b\x32\x1a.google.protobuf.Timestamp:P\x92\x41M\nK*\x0eScheduling Job2\x19Recursive or one-off job.\xd2\x01\x0bjobFunction\xd2\x01\x04name\xd2\x01\x08schedule\"\x91\x02\n\x08Schedule\x12\x10\n\x08schedule\x18\x01 \x01(\t\x12\x10\n\x08timezone\x18\x02 \x01(\t\x12,\n\x08startsAt\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x15\n\x0brepeatCount\x18\x0f \x01(\x11H\x00\x12\x30\n\nexpiryDate\x18\x10 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x00:`\x92\x41]\n[*\x08Schedule2DSet a schedule for the job. Set repeatCount to -1 if job is one-off.\xd2\x01\x08scheduleB\x08\n\x06\x65xpiry\"\xfc\x01\n\x15SchedulingJobResponse\x12\n\n\x02id\x18\x01 \x01(\t\x12\x1d\n\x06status\x18\x02 \x01(\x0e\x32\r.ct.JobStatus\x12\x33\n\x0fnextRunDatetime\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12*\n\x06\x65xpiry\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp:W\x92\x41T\nR*\x17Scheduling Job Response27A response object for create and update scheduling job.\"\x8f\x02\n\nJobHistory\x12\n\n\x02id\x18\x01 \x01(\t\x12\r\n\x05jobId\x18\x02 \x01(\t\x12\x0f\n\x07success\x18\x03 \x01(\x08\x12\x0b\n\x03log\x18\x04 \x01(\t\x12\x12\n\nstatusCode\x18\x05 \x01(\r\x12\x38\n\x14scheduledRunDateTime\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0b\x63ompletedAt\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp:I\x92\x41\x46\nD*\x0bJob History2\x19Results of executed jobs.\xd2\x01\x05jobId\xd2\x01\x03log\xd2\x01\x0b\x63ompletedAt*\xdf\x01\n\tJobStatus\x12\x13\n\x0fJOB_STATUS_NONE\x10\x00\x12\x16\n\x12JOB_STATUS_CREATED\x10\x01\x12\x14\n\x10JOB_STATUS_READY\x10\x02\x12\x17\n\x13JOB_STATUS_INFLIGHT\x10\x03\x12\x18\n\x14JOB_STATUS_SUCCEEDED\x10\x04\x12\x15\n\x11JOB_STATUS_FAILED\x10\x05\x12\x15\n\x11JOB_STATUS_PAUSED\x10\x06\x12\x16\n\x12JOB_STATUS_EXPIRED\x10\x07\x12\x16\n\x12JOB_STATUS_DELETED\x10\x08\x42M\n\x13\x63om.passkit.grpc.ctZ$stash.passkit.com/io/model/sdk/go/ct\xaa\x02\x0fPassKit.Grpc.Ctb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1aio/flights/passenger.proto\x12\x07\x66lights\x1a\x18io/flights/barcode.proto\x1a\x1eio/common/common_objects.proto\x1a\x18io/common/personal.proto\x1a.protoc-gen-openapiv2/options/annotations.proto\"\xc9\x04\n\tPassenger\x12$\n\x10passengerDetails\x18\x01 \x01(\x0b\x32\n.io.Person\x12\x35\n\x11\x66requentFlyerInfo\x18\x02 \x01(\x0b\x32\x1a.flights.FrequentFlyerInfo\x12\x31\n\x0fidentityDetails\x18\x03 \x01(\x0b\x32\x18.flights.IdentityDetails\x12\x12\n\nwithInfant\x18\x04 \x01(\x08\x12&\n\rinfantDetails\x18\x05 \x01(\x0b\x32\x0f.flights.Infant\x12\x1b\n\x13knownTravelerNumber\x18\x07 \x01(\t:\xd2\x02\x92\x41\xce\x02\n\xcb\x02*\tPassenger2\xaa\x02Passenger information can optionally be provided. All fields are optional with the exception of the Passenger name to be rendered on the boarding pass. All passenger is treated as PII and encrypted at rest. Passenger information is deleted or rendered unusable once the pass record has invalidated.\xd2\x01\x10passengerDetails\"a\n\x11\x46requentFlyerInfo\x12\x13\n\x0bprogramName\x18\x01 \x01(\t\x12\x19\n\x11\x61irlineDesignator\x18\x02 \x01(\t\x12\x0e\n\x06number\x18\x03 \x01(\t\x12\x0c\n\x04tier\x18\x04 \x01(\t\"\x82\x02\n\x0fIdentityDetails\x12\x33\n\x10identityDocument\x18\x01 \x01(\x0e\x32\x19.flights.IdentityDocument\x12\x16\n\x0eissuingCountry\x18\x02 \x01(\t\x12\x13\n\x0bnationality\x18\x03 \x01(\t\x12\x16\n\x0e\x64ocumentNumber\x18\x04 \x01(\t\x12\x1d\n\x0b\x64\x61teOfBirth\x18\x05 \x01(\x0b\x32\x08.io.Date\x12\x1a\n\x06gender\x18\x06 \x01(\x0e\x32\n.io.Gender\x12\x1c\n\nissuedDate\x18\x07 \x01(\x0b\x32\x08.io.Date\x12\x1c\n\nexpiryDate\x18\x08 \x01(\x0b\x32\x08.io.Date\"\x8e\x02\n\x06Infant\x12!\n\rinfantDetails\x18\x01 \x01(\x0b\x32\n.io.Person\x12\x31\n\x0fidentityDetails\x18\x02 \x01(\x0b\x32\x18.flights.IdentityDetails\x12\x16\n\x0e\x62\x61rcodePayload\x18\x03 \x01(\t\x12\x33\n\x10\x63onditionalItems\x18\x04 \x01(\x0b\x32\x19.flights.ConditionalItems\x12\x1d\n\x15\x62\x61rcodeAdditionalData\x18\x05 \x01(\t\x12\x15\n\rsecurityImage\x18\x06 \x01(\t\x12\x16\n\x0eprivilegeImage\x18\x07 \x01(\t\x12\x13\n\x0b\x66ooterImage\x18\x08 \x01(\t*\x90\x01\n\x10IdentityDocument\x12\x0c\n\x08PASSPORT\x10\x00\x12\x14\n\x10NATIONAL_ID_CARD\x10\x01\x12\x13\n\x0f\x44RIVING_LICENSE\x10\x02\x12\x0f\n\x0b\x43REDIT_CARD\x10\x03\x12\x17\n\x13\x46REQUENT_FLYER_CARD\x10\x04\x12\x19\n\x15OTHER_TRAVEL_DOCUMENT\x10\x05\x42_\n\x18\x63om.passkit.grpc.FlightsZ,stash.passkit.com/io/model/sdk/go/io/flights\xaa\x02\x14PassKit.Grpc.Flightsb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'ct.scheduler.scheduler_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'io.flights.passenger_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\023com.passkit.grpc.ctZ$stash.passkit.com/io/model/sdk/go/ct\252\002\017PassKit.Grpc.Ct'
-  _SCHEDULINGJOB._options = None
-  _SCHEDULINGJOB._serialized_options = b'\222AM\nK*\016Scheduling Job2\031Recursive or one-off job.\322\001\013jobFunction\322\001\004name\322\001\010schedule'
-  _SCHEDULE._options = None
-  _SCHEDULE._serialized_options = b'\222A]\n[*\010Schedule2DSet a schedule for the job. Set repeatCount to -1 if job is one-off.\322\001\010schedule'
-  _SCHEDULINGJOBRESPONSE._options = None
-  _SCHEDULINGJOBRESPONSE._serialized_options = b'\222AT\nR*\027Scheduling Job Response27A response object for create and update scheduling job.'
-  _JOBHISTORY._options = None
-  _JOBHISTORY._serialized_options = b'\222AF\nD*\013Job History2\031Results of executed jobs.\322\001\005jobId\322\001\003log\322\001\013completedAt'
-  _JOBSTATUS._serialized_start=1444
-  _JOBSTATUS._serialized_end=1667
-  _SCHEDULINGJOB._serialized_start=118
-  _SCHEDULINGJOB._serialized_end=636
-  _SCHEDULE._serialized_start=639
-  _SCHEDULE._serialized_end=912
-  _SCHEDULINGJOBRESPONSE._serialized_start=915
-  _SCHEDULINGJOBRESPONSE._serialized_end=1167
-  _JOBHISTORY._serialized_start=1170
-  _JOBHISTORY._serialized_end=1441
+  DESCRIPTOR._serialized_options = b'\n\030com.passkit.grpc.FlightsZ,stash.passkit.com/io/model/sdk/go/io/flights\252\002\024PassKit.Grpc.Flights'
+  _PASSENGER._options = None
+  _PASSENGER._serialized_options = b'\222A\316\002\n\313\002*\tPassenger2\252\002Passenger information can optionally be provided. All fields are optional with the exception of the Passenger name to be rendered on the boarding pass. All passenger is treated as PII and encrypted at rest. Passenger information is deleted or rendered unusable once the pass record has invalidated.\322\001\020passengerDetails'
+  _IDENTITYDOCUMENT._serialized_start=1393
+  _IDENTITYDOCUMENT._serialized_end=1537
+  _PASSENGER._serialized_start=172
+  _PASSENGER._serialized_end=757
+  _FREQUENTFLYERINFO._serialized_start=759
+  _FREQUENTFLYERINFO._serialized_end=856
+  _IDENTITYDETAILS._serialized_start=859
+  _IDENTITYDETAILS._serialized_end=1117
+  _INFANT._serialized_start=1120
+  _INFANT._serialized_end=1390
 # @@protoc_insertion_point(module_scope)
```

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/analytics/a_rpc_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/analytics/a_rpc_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/analytics/a_rpc_pb2_grpc.py` & `passkit-python-grpc-sdk-1.1.72.2/io/analytics/a_rpc_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/certificate/certificate_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/certificate/certificate_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/common/attributes_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/common/attributes_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/common/billing_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/common/billing_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/common/common_objects_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/common/common_objects_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/common/distribution_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/common/distribution_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/common/expiry_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/common/expiry_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/common/filter_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/common/filter_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/common/integration_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/common/integration_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/common/links_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/common/links_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/common/localization_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/common/localization_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/common/message_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/common/message_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/common/metrics_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/common/metrics_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/common/note_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/common/note_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/common/pagination_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/common/pagination_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/common/pass_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/common/pass_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/common/personal_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/common/personal_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/common/project_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/common/project_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/common/protocols_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/common/protocols_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/common/proximity_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/common/proximity_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/common/reporting_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/common/reporting_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/common/template_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/common/template_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/common/tracking_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/common/tracking_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/common/transaction_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/common/transaction_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/common/useragent_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/common/useragent_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/core/a_rpc_certificates_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/core/a_rpc_certificates_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/core/a_rpc_certificates_pb2_grpc.py` & `passkit-python-grpc-sdk-1.1.72.2/io/core/a_rpc_certificates_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/core/a_rpc_distribution_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/core/a_rpc_distribution_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/core/a_rpc_distribution_pb2_grpc.py` & `passkit-python-grpc-sdk-1.1.72.2/io/core/a_rpc_distribution_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/core/a_rpc_images_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/core/a_rpc_images_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/core/a_rpc_images_pb2_grpc.py` & `passkit-python-grpc-sdk-1.1.72.2/io/core/a_rpc_images_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/core/a_rpc_messages_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/core/a_rpc_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/core/a_rpc_messages_pb2_grpc.py` & `passkit-python-grpc-sdk-1.1.72.2/io/core/a_rpc_messages_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/core/a_rpc_others_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/core/a_rpc_others_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/core/a_rpc_others_pb2_grpc.py` & `passkit-python-grpc-sdk-1.1.72.2/io/core/a_rpc_others_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/core/a_rpc_templates_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/core/a_rpc_templates_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/core/a_rpc_templates_pb2_grpc.py` & `passkit-python-grpc-sdk-1.1.72.2/io/core/a_rpc_templates_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/event_tickets/a_rpc_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/event_tickets/a_rpc_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/event_tickets/a_rpc_pb2_grpc.py` & `passkit-python-grpc-sdk-1.1.72.2/io/event_tickets/a_rpc_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/event_tickets/event_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/event_tickets/event_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/event_tickets/production_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/event_tickets/production_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/event_tickets/ticket_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/event_tickets/ticket_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/event_tickets/ticket_type_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/event_tickets/ticket_type_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/event_tickets/venue_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/event_tickets/venue_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/flights/a_rpc_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/flights/a_rpc_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/flights/a_rpc_pb2_grpc.py` & `passkit-python-grpc-sdk-1.1.72.2/io/flights/a_rpc_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/flights/airport_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/flights/airport_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/flights/barcode_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/flights/barcode_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/flights/boarding_pass_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/flights/boarding_pass_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/flights/carrier_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/flights/carrier_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/flights/flight_designator_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/flights/flight_designator_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/flights/flight_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/flights/flight_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/flights/passenger_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/member/member_events_pb2.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: io/flights/passenger.proto
+# source: io/member/member_events.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from io.flights import barcode_pb2 as io_dot_flights_dot_barcode__pb2
-from io.common import common_objects_pb2 as io_dot_common_dot_common__objects__pb2
+from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from io.common import personal_pb2 as io_dot_common_dot_personal__pb2
 from protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1aio/flights/passenger.proto\x12\x07\x66lights\x1a\x18io/flights/barcode.proto\x1a\x1eio/common/common_objects.proto\x1a\x18io/common/personal.proto\x1a.protoc-gen-openapiv2/options/annotations.proto\"\xc9\x04\n\tPassenger\x12$\n\x10passengerDetails\x18\x01 \x01(\x0b\x32\n.io.Person\x12\x35\n\x11\x66requentFlyerInfo\x18\x02 \x01(\x0b\x32\x1a.flights.FrequentFlyerInfo\x12\x31\n\x0fidentityDetails\x18\x03 \x01(\x0b\x32\x18.flights.IdentityDetails\x12\x12\n\nwithInfant\x18\x04 \x01(\x08\x12&\n\rinfantDetails\x18\x05 \x01(\x0b\x32\x0f.flights.Infant\x12\x1b\n\x13knownTravelerNumber\x18\x07 \x01(\t:\xd2\x02\x92\x41\xce\x02\n\xcb\x02*\tPassenger2\xaa\x02Passenger information can optionally be provided. All fields are optional with the exception of the Passenger name to be rendered on the boarding pass. All passenger is treated as PII and encrypted at rest. Passenger information is deleted or rendered unusable once the pass record has invalidated.\xd2\x01\x10passengerDetails\"a\n\x11\x46requentFlyerInfo\x12\x13\n\x0bprogramName\x18\x01 \x01(\t\x12\x19\n\x11\x61irlineDesignator\x18\x02 \x01(\t\x12\x0e\n\x06number\x18\x03 \x01(\t\x12\x0c\n\x04tier\x18\x04 \x01(\t\"\x82\x02\n\x0fIdentityDetails\x12\x33\n\x10identityDocument\x18\x01 \x01(\x0e\x32\x19.flights.IdentityDocument\x12\x16\n\x0eissuingCountry\x18\x02 \x01(\t\x12\x13\n\x0bnationality\x18\x03 \x01(\t\x12\x16\n\x0e\x64ocumentNumber\x18\x04 \x01(\t\x12\x1d\n\x0b\x64\x61teOfBirth\x18\x05 \x01(\x0b\x32\x08.io.Date\x12\x1a\n\x06gender\x18\x06 \x01(\x0e\x32\n.io.Gender\x12\x1c\n\nissuedDate\x18\x07 \x01(\x0b\x32\x08.io.Date\x12\x1c\n\nexpiryDate\x18\x08 \x01(\x0b\x32\x08.io.Date\"\x8e\x02\n\x06Infant\x12!\n\rinfantDetails\x18\x01 \x01(\x0b\x32\n.io.Person\x12\x31\n\x0fidentityDetails\x18\x02 \x01(\x0b\x32\x18.flights.IdentityDetails\x12\x16\n\x0e\x62\x61rcodePayload\x18\x03 \x01(\t\x12\x33\n\x10\x63onditionalItems\x18\x04 \x01(\x0b\x32\x19.flights.ConditionalItems\x12\x1d\n\x15\x62\x61rcodeAdditionalData\x18\x05 \x01(\t\x12\x15\n\rsecurityImage\x18\x06 \x01(\t\x12\x16\n\x0eprivilegeImage\x18\x07 \x01(\t\x12\x13\n\x0b\x66ooterImage\x18\x08 \x01(\t*\x90\x01\n\x10IdentityDocument\x12\x0c\n\x08PASSPORT\x10\x00\x12\x14\n\x10NATIONAL_ID_CARD\x10\x01\x12\x13\n\x0f\x44RIVING_LICENSE\x10\x02\x12\x0f\n\x0b\x43REDIT_CARD\x10\x03\x12\x17\n\x13\x46REQUENT_FLYER_CARD\x10\x04\x12\x19\n\x15OTHER_TRAVEL_DOCUMENT\x10\x05\x42_\n\x18\x63om.passkit.grpc.FlightsZ,stash.passkit.com/io/model/sdk/go/io/flights\xaa\x02\x14PassKit.Grpc.Flightsb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1dio/member/member_events.proto\x12\x07members\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x18io/common/personal.proto\x1a.protoc-gen-openapiv2/options/annotations.proto\"\x86\x05\n\x0bMemberEvent\x12\n\n\x02id\x18\x01 \x01(\t\x12\'\n\x06member\x18\x02 \x01(\x0b\x32\x17.members.MemberMininmal\x12(\n\teventType\x18\x03 \x01(\x0e\x32\x15.members.MemberEvents\x12\x0f\n\x07\x61\x64\x64ress\x18\x04 \x01(\t\x12\x0b\n\x03lat\x18\x05 \x01(\x01\x12\x0b\n\x03lon\x18\x06 \x01(\x01\x12\x0b\n\x03\x61lt\x18\x07 \x01(\x05\x12\x12\n\nexternalId\x18\x08 \x01(\t\x12\x16\n\x0e\x65xternalUserId\x18\t \x01(\t\x12\x18\n\x10\x65xternalDeviceId\x18\n \x01(\t\x12\x19\n\x11\x65xternalServiceId\x18\x0b \x01(\t\x12\x34\n\x08metaData\x18\x0c \x03(\x0b\x32\".members.MemberEvent.MetaDataEntry\x12\r\n\x05notes\x18\r \x01(\t\x12(\n\x04\x64\x61te\x18\x0e \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x35\n\x11retainedUntilDate\x18\x0f \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12+\n\x07\x63reated\x18\x10 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x1a/\n\rMetaDataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01:{\x92\x41x\nv*\rMember Events2eEvents that have happened for a member. Events are generated by the Membership API and are immutable.\"\x8b\x01\n\x0eMemberMininmal\x12\n\n\x02id\x18\x01 \x01(\t\x12\x12\n\nexternalId\x18\x02 \x01(\t\x12\x1a\n\x12groupingIdentifier\x18\x03 \x01(\t\x12\x0e\n\x06tierId\x18\x04 \x01(\t\x12\x11\n\tprogramId\x18\x05 \x01(\t\x12\x1a\n\x06person\x18\x06 \x01(\x0b\x32\n.io.Person*\xfd\x01\n\x0cMemberEvents\x12\x1b\n\x17\x45VENT_MEMBER_DO_NOT_USE\x10\x00\x12\x1b\n\x17\x45VENT_MEMBER_CHECKED_IN\x10\x01\x12\x1c\n\x18\x45VENT_MEMBER_CHECKED_OUT\x10\x02\x12\x19\n\x15\x45VENT_MEMBER_VERIFIED\x10\x03\x12\x1e\n\x1a\x45VENT_MEMBER_POINTS_EARNED\x10\x04\x12\x1e\n\x1a\x45VENT_MEMBER_POINTS_BURNED\x10\x05\x12\x1b\n\x17\x45VENT_MEMBER_POINTS_SET\x10\x06\x12\x1d\n\x19\x45VENT_MEMBER_TIER_CHANGED\x10\x07\x42_\n\x18\x63om.passkit.grpc.MembersZ,stash.passkit.com/io/model/sdk/go/io/members\xaa\x02\x14PassKit.Grpc.Membersb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'io.flights.passenger_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'io.member.member_events_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\030com.passkit.grpc.FlightsZ,stash.passkit.com/io/model/sdk/go/io/flights\252\002\024PassKit.Grpc.Flights'
-  _PASSENGER._options = None
-  _PASSENGER._serialized_options = b'\222A\316\002\n\313\002*\tPassenger2\252\002Passenger information can optionally be provided. All fields are optional with the exception of the Passenger name to be rendered on the boarding pass. All passenger is treated as PII and encrypted at rest. Passenger information is deleted or rendered unusable once the pass record has invalidated.\322\001\020passengerDetails'
-  _IDENTITYDOCUMENT._serialized_start=1393
-  _IDENTITYDOCUMENT._serialized_end=1537
-  _PASSENGER._serialized_start=172
-  _PASSENGER._serialized_end=757
-  _FREQUENTFLYERINFO._serialized_start=759
-  _FREQUENTFLYERINFO._serialized_end=856
-  _IDENTITYDETAILS._serialized_start=859
-  _IDENTITYDETAILS._serialized_end=1117
-  _INFANT._serialized_start=1120
-  _INFANT._serialized_end=1390
+  DESCRIPTOR._serialized_options = b'\n\030com.passkit.grpc.MembersZ,stash.passkit.com/io/model/sdk/go/io/members\252\002\024PassKit.Grpc.Members'
+  _MEMBEREVENT_METADATAENTRY._options = None
+  _MEMBEREVENT_METADATAENTRY._serialized_options = b'8\001'
+  _MEMBEREVENT._options = None
+  _MEMBEREVENT._serialized_options = b'\222Ax\nv*\rMember Events2eEvents that have happened for a member. Events are generated by the Membership API and are immutable.'
+  _MEMBEREVENTS._serialized_start=941
+  _MEMBEREVENTS._serialized_end=1194
+  _MEMBEREVENT._serialized_start=150
+  _MEMBEREVENT._serialized_end=796
+  _MEMBEREVENT_METADATAENTRY._serialized_start=624
+  _MEMBEREVENT_METADATAENTRY._serialized_end=671
+  _MEMBERMININMAL._serialized_start=799
+  _MEMBERMININMAL._serialized_end=938
 # @@protoc_insertion_point(module_scope)
```

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/flights/cabin_codes/cabin_codes_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/flights/cabin_codes/cabin_codes_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/image/image_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/image/image_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/member/a_rpc_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/member/a_rpc_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/member/a_rpc_pb2_grpc.py` & `passkit-python-grpc-sdk-1.1.72.2/io/member/a_rpc_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/member/event_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/member/event_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/member/member_events_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/member/tier_pb2.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,35 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: io/member/member_events.proto
+# source: io/member/tier.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
-from io.common import personal_pb2 as io_dot_common_dot_personal__pb2
 from protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
+from io.common import localization_pb2 as io_dot_common_dot_localization__pb2
+from io.common import common_objects_pb2 as io_dot_common_dot_common__objects__pb2
+from io.common import expiry_pb2 as io_dot_common_dot_expiry__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1dio/member/member_events.proto\x12\x07members\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x18io/common/personal.proto\x1a.protoc-gen-openapiv2/options/annotations.proto\"\x86\x05\n\x0bMemberEvent\x12\n\n\x02id\x18\x01 \x01(\t\x12\'\n\x06member\x18\x02 \x01(\x0b\x32\x17.members.MemberMininmal\x12(\n\teventType\x18\x03 \x01(\x0e\x32\x15.members.MemberEvents\x12\x0f\n\x07\x61\x64\x64ress\x18\x04 \x01(\t\x12\x0b\n\x03lat\x18\x05 \x01(\x01\x12\x0b\n\x03lon\x18\x06 \x01(\x01\x12\x0b\n\x03\x61lt\x18\x07 \x01(\x05\x12\x12\n\nexternalId\x18\x08 \x01(\t\x12\x16\n\x0e\x65xternalUserId\x18\t \x01(\t\x12\x18\n\x10\x65xternalDeviceId\x18\n \x01(\t\x12\x19\n\x11\x65xternalServiceId\x18\x0b \x01(\t\x12\x34\n\x08metaData\x18\x0c \x03(\x0b\x32\".members.MemberEvent.MetaDataEntry\x12\r\n\x05notes\x18\r \x01(\t\x12(\n\x04\x64\x61te\x18\x0e \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x35\n\x11retainedUntilDate\x18\x0f \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12+\n\x07\x63reated\x18\x10 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x1a/\n\rMetaDataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01:{\x92\x41x\nv*\rMember Events2eEvents that have happened for a member. Events are generated by the Membership API and are immutable.\"\x8b\x01\n\x0eMemberMininmal\x12\n\n\x02id\x18\x01 \x01(\t\x12\x12\n\nexternalId\x18\x02 \x01(\t\x12\x1a\n\x12groupingIdentifier\x18\x03 \x01(\t\x12\x0e\n\x06tierId\x18\x04 \x01(\t\x12\x11\n\tprogramId\x18\x05 \x01(\t\x12\x1a\n\x06person\x18\x06 \x01(\x0b\x32\n.io.Person*\xfd\x01\n\x0cMemberEvents\x12\x1b\n\x17\x45VENT_MEMBER_DO_NOT_USE\x10\x00\x12\x1b\n\x17\x45VENT_MEMBER_CHECKED_IN\x10\x01\x12\x1c\n\x18\x45VENT_MEMBER_CHECKED_OUT\x10\x02\x12\x19\n\x15\x45VENT_MEMBER_VERIFIED\x10\x03\x12\x1e\n\x1a\x45VENT_MEMBER_POINTS_EARNED\x10\x04\x12\x1e\n\x1a\x45VENT_MEMBER_POINTS_BURNED\x10\x05\x12\x1b\n\x17\x45VENT_MEMBER_POINTS_SET\x10\x06\x12\x1d\n\x19\x45VENT_MEMBER_TIER_CHANGED\x10\x07\x42_\n\x18\x63om.passkit.grpc.MembersZ,stash.passkit.com/io/model/sdk/go/io/members\xaa\x02\x14PassKit.Grpc.Membersb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14io/member/tier.proto\x12\x07members\x1a\x1fgoogle/protobuf/timestamp.proto\x1a.protoc-gen-openapiv2/options/annotations.proto\x1a\x1cio/common/localization.proto\x1a\x1eio/common/common_objects.proto\x1a\x16io/common/expiry.proto\"\xa3\x06\n\x04Tier\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\ttierIndex\x18\x02 \x01(\r\x12\x0c\n\x04name\x18\x03 \x01(\t\x12*\n\rlocalizedName\x18\x04 \x01(\x0b\x32\x13.io.LocalizedString\x12\x19\n\x11secondaryTierName\x18\x05 \x01(\t\x12\x37\n\x1alocalizedSecondaryTierName\x18\x06 \x01(\x0b\x32\x13.io.LocalizedString\x12\x11\n\tprogramId\x18\x07 \x01(\t\x12\x16\n\x0epassTemplateId\x18\x08 \x01(\t\x12\x1a\n\x12tierUpgradeMessage\x18\t \x01(\t\x12\x38\n\x1blocalizedTierUpgradeMessage\x18\n \x01(\x0b\x32\x13.io.LocalizedString\x12\x1c\n\x14tierDowngradeMessage\x18\x0b \x01(\t\x12:\n\x1dlocalizedTierDowngradeMessage\x18\x0c \x01(\x0b\x32\x13.io.LocalizedString\x12+\n\x07\x63reated\x18\r \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12+\n\x07updated\x18\x0e \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x17\n\x0fpointsOverdrawn\x18\x0f \x01(\x08\x12 \n\x18secondaryPointsOverdrawn\x18\x10 \x01(\x08\x12*\n\x0e\x65xpirySettings\x18\x11 \x01(\x0b\x32\x12.io.ExpirySettings\x12\x10\n\x08timezone\x18\x12 \x01(\t\x12&\n\x12\x61llowTierEnrolment\x18\x13 \x01(\x0b\x32\n.io.PkBool\x12\x11\n\tshortCode\x18\x14 \x01(\t:\x84\x01\x92\x41\x80\x01\n~*\x04Tier2ATier allows a company to override certain details in the program.\xd2\x01\x02id\xd2\x01\ttierIndex\xd2\x01\tprogramId\xd2\x01\x04name\xd2\x01\x0epassTemplateId\"5\n\x10TierRequestInput\x12\x11\n\tprogramId\x18\x01 \x01(\t\x12\x0e\n\x06tierId\x18\x02 \x01(\tB_\n\x18\x63om.passkit.grpc.MembersZ,stash.passkit.com/io/model/sdk/go/io/members\xaa\x02\x14PassKit.Grpc.Membersb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'io.member.member_events_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'io.member.tier_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\030com.passkit.grpc.MembersZ,stash.passkit.com/io/model/sdk/go/io/members\252\002\024PassKit.Grpc.Members'
-  _MEMBEREVENT_METADATAENTRY._options = None
-  _MEMBEREVENT_METADATAENTRY._serialized_options = b'8\001'
-  _MEMBEREVENT._options = None
-  _MEMBEREVENT._serialized_options = b'\222Ax\nv*\rMember Events2eEvents that have happened for a member. Events are generated by the Membership API and are immutable.'
-  _MEMBEREVENTS._serialized_start=941
-  _MEMBEREVENTS._serialized_end=1194
-  _MEMBEREVENT._serialized_start=150
-  _MEMBEREVENT._serialized_end=796
-  _MEMBEREVENT_METADATAENTRY._serialized_start=624
-  _MEMBEREVENT_METADATAENTRY._serialized_end=671
-  _MEMBERMININMAL._serialized_start=799
-  _MEMBERMININMAL._serialized_end=938
+  _TIER._options = None
+  _TIER._serialized_options = b'\222A\200\001\n~*\004Tier2ATier allows a company to override certain details in the program.\322\001\002id\322\001\ttierIndex\322\001\tprogramId\322\001\004name\322\001\016passTemplateId'
+  _TIER._serialized_start=201
+  _TIER._serialized_end=1004
+  _TIERREQUESTINPUT._serialized_start=1006
+  _TIERREQUESTINPUT._serialized_end=1059
 # @@protoc_insertion_point(module_scope)
```

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/member/member_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/member/member_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/member/program_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/member/program_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/member/tier_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/raw/project_pb2.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: io/member/tier.proto
+# source: io/raw/project.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
-from protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
+from io.common import distribution_pb2 as io_dot_common_dot_distribution__pb2
 from io.common import localization_pb2 as io_dot_common_dot_localization__pb2
-from io.common import common_objects_pb2 as io_dot_common_dot_common__objects__pb2
-from io.common import expiry_pb2 as io_dot_common_dot_expiry__pb2
+from io.common import project_pb2 as io_dot_common_dot_project__pb2
+from io.common import billing_pb2 as io_dot_common_dot_billing__pb2
+from protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14io/member/tier.proto\x12\x07members\x1a\x1fgoogle/protobuf/timestamp.proto\x1a.protoc-gen-openapiv2/options/annotations.proto\x1a\x1cio/common/localization.proto\x1a\x1eio/common/common_objects.proto\x1a\x16io/common/expiry.proto\"\xa3\x06\n\x04Tier\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\ttierIndex\x18\x02 \x01(\r\x12\x0c\n\x04name\x18\x03 \x01(\t\x12*\n\rlocalizedName\x18\x04 \x01(\x0b\x32\x13.io.LocalizedString\x12\x19\n\x11secondaryTierName\x18\x05 \x01(\t\x12\x37\n\x1alocalizedSecondaryTierName\x18\x06 \x01(\x0b\x32\x13.io.LocalizedString\x12\x11\n\tprogramId\x18\x07 \x01(\t\x12\x16\n\x0epassTemplateId\x18\x08 \x01(\t\x12\x1a\n\x12tierUpgradeMessage\x18\t \x01(\t\x12\x38\n\x1blocalizedTierUpgradeMessage\x18\n \x01(\x0b\x32\x13.io.LocalizedString\x12\x1c\n\x14tierDowngradeMessage\x18\x0b \x01(\t\x12:\n\x1dlocalizedTierDowngradeMessage\x18\x0c \x01(\x0b\x32\x13.io.LocalizedString\x12+\n\x07\x63reated\x18\r \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12+\n\x07updated\x18\x0e \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x17\n\x0fpointsOverdrawn\x18\x0f \x01(\x08\x12 \n\x18secondaryPointsOverdrawn\x18\x10 \x01(\x08\x12*\n\x0e\x65xpirySettings\x18\x11 \x01(\x0b\x32\x12.io.ExpirySettings\x12\x10\n\x08timezone\x18\x12 \x01(\t\x12&\n\x12\x61llowTierEnrolment\x18\x13 \x01(\x0b\x32\n.io.PkBool\x12\x11\n\tshortCode\x18\x14 \x01(\t:\x84\x01\x92\x41\x80\x01\n~*\x04Tier2ATier allows a company to override certain details in the program.\xd2\x01\x02id\xd2\x01\ttierIndex\xd2\x01\tprogramId\xd2\x01\x04name\xd2\x01\x0epassTemplateId\"5\n\x10TierRequestInput\x12\x11\n\tprogramId\x18\x01 \x01(\t\x12\x0e\n\x06tierId\x18\x02 \x01(\tB_\n\x18\x63om.passkit.grpc.MembersZ,stash.passkit.com/io/model/sdk/go/io/members\xaa\x02\x14PassKit.Grpc.Membersb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14io/raw/project.proto\x12\x03raw\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1cio/common/distribution.proto\x1a\x1cio/common/localization.proto\x1a\x17io/common/project.proto\x1a\x17io/common/billing.proto\x1a.protoc-gen-openapiv2/options/annotations.proto\"\xfe\x03\n\x0bPassProject\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12*\n\rlocalizedName\x18\x03 \x01(\x0b\x32\x13.io.LocalizedString\x12!\n\x06status\x18\x04 \x03(\x0e\x32\x11.io.ProjectStatus\x12\x18\n\x05quota\x18\x05 \x01(\x0b\x32\t.io.Quota\x12\x1a\n\x12passTypeIdentifier\x18\x06 \x01(\t\x12\x36\n\x14\x64istributionSettings\x18\x07 \x01(\x0b\x32\x18.io.DistributionSettings\x12+\n\x07\x63reated\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12+\n\x07updated\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp:\xbd\x01\x92\x41\xb9\x01\n\xb6\x01*\x0cPass Project2\x95\x01Pass Project holds the basic business logic. Pass Project holds details on pass distribution, quotas, Apple certificate, integrations & hooks to use.\xd2\x01\x04name\xd2\x01\x06status\"q\n\x16PassProjectCopyRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12!\n\x06status\x18\x03 \x03(\x0e\x32\x11.io.ProjectStatus\x12\x1a\n\x12passTypeIdentifier\x18\x04 \x01(\tBS\n\x14\x63om.passkit.grpc.RawZ(stash.passkit.com/io/model/sdk/go/io/raw\xaa\x02\x10PassKit.Grpc.Rawb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'io.member.tier_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'io.raw.project_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\030com.passkit.grpc.MembersZ,stash.passkit.com/io/model/sdk/go/io/members\252\002\024PassKit.Grpc.Members'
-  _TIER._options = None
-  _TIER._serialized_options = b'\222A\200\001\n~*\004Tier2ATier allows a company to override certain details in the program.\322\001\002id\322\001\ttierIndex\322\001\tprogramId\322\001\004name\322\001\016passTemplateId'
-  _TIER._serialized_start=201
-  _TIER._serialized_end=1004
-  _TIERREQUESTINPUT._serialized_start=1006
-  _TIERREQUESTINPUT._serialized_end=1059
+  DESCRIPTOR._serialized_options = b'\n\024com.passkit.grpc.RawZ(stash.passkit.com/io/model/sdk/go/io/raw\252\002\020PassKit.Grpc.Raw'
+  _PASSPROJECT._options = None
+  _PASSPROJECT._serialized_options = b'\222A\271\001\n\266\001*\014Pass Project2\225\001Pass Project holds the basic business logic. Pass Project holds details on pass distribution, quotas, Apple certificate, integrations & hooks to use.\322\001\004name\322\001\006status'
+  _PASSPROJECT._serialized_start=221
+  _PASSPROJECT._serialized_end=731
+  _PASSPROJECTCOPYREQUEST._serialized_start=733
+  _PASSPROJECTCOPYREQUEST._serialized_end=846
 # @@protoc_insertion_point(module_scope)
```

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/raw/a_rpc_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/raw/a_rpc_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/raw/a_rpc_pb2_grpc.py` & `passkit-python-grpc-sdk-1.1.72.2/io/raw/a_rpc_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/raw/pass_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/raw/pass_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/scheduler/a_rpc_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/scheduler/a_rpc_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/scheduler/a_rpc_pb2_grpc.py` & `passkit-python-grpc-sdk-1.1.72.2/io/scheduler/a_rpc_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/scheduler/scheduler_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/scheduler/scheduler_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/single_use_coupons/a_rpc_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/single_use_coupons/a_rpc_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/single_use_coupons/a_rpc_pb2_grpc.py` & `passkit-python-grpc-sdk-1.1.72.2/io/single_use_coupons/a_rpc_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/single_use_coupons/campaign_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/single_use_coupons/campaign_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/single_use_coupons/coupon_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/single_use_coupons/coupon_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/single_use_coupons/offer_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/single_use_coupons/offer_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/io/user/user_pb2.py` & `passkit-python-grpc-sdk-1.1.72.2/io/user/user_pb2.py`

 * *Files identical despite different names*

### Comparing `passkit_python_grpc_sdk-1.1.72.1/pyproject.toml` & `passkit-python-grpc-sdk-1.1.72.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "passkit-python-grpc-sdk"
-version = "1.1.72.1"
+version = "1.1.72.2"
 authors = [
   { name="passkit", email="support@passkit.com" },
 ]
 description = "Python SDK for Apple Wallet and Google Pay Membership / Loyalty / Access Cards, Coupons, Flights & Event-Tickets."
 readme = "readME.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `passkit_python_grpc_sdk-1.1.72.1/PKG-INFO` & `passkit-python-grpc-sdk-1.1.72.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: passkit-python-grpc-sdk
-Version: 1.1.72.1
+Version: 1.1.72.2
 Summary: Python SDK for Apple Wallet and Google Pay Membership / Loyalty / Access Cards, Coupons, Flights & Event-Tickets.
+Author: passkit
+Author-email: passkit <support@passkit.com>
 Project-URL: Homepage, https://github.com/PassKit/passkit-python-grpc-sdk
 Project-URL: Bug Tracker, https://github.com/PassKit/passkit-python-grpc-sdk/issues
-Author-email: passkit <support@passkit.com>
+Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 PassKit Python gRPC SDK
 =====================
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
@@ -45,8 +46,8 @@
 GUI tool can be accessed from [your PassKit account](https://app.passkit.com/login).
 
 ## Getting Help
 * Email [support@passkit.com](email:support@passkit.com)
 * [Online chat support](https://passkit.com/)
 
 ## License
-Distributed under MIT License.
+Distributed under MIT License.
```

