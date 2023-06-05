# Comparing `tmp/symphony_bdk_python-2.6.1.tar.gz` & `tmp/symphony_bdk_python-2.6.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symphony_bdk_python-2.6.1.tar", max compression
+gzip compressed data, was "symphony_bdk_python-2.6.dev0.tar", max compression
```

## Comparing `symphony_bdk_python-2.6.1.tar` & `symphony_bdk_python-2.6.dev0.tar`

### file list

```diff
@@ -1,537 +1,538 @@
--rw-r--r--   0        0        0    11342 2023-06-05 08:53:30.594727 symphony_bdk_python-2.6.1/LICENSE
--rw-r--r--   0        0        0     4670 2023-06-05 08:53:30.594727 symphony_bdk_python-2.6.1/README.md
--rw-r--r--   0        0        0     1544 2023-06-05 08:53:30.722730 symphony_bdk_python-2.6.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-05 08:53:30.722730 symphony_bdk_python-2.6.1/symphony/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 08:53:30.722730 symphony_bdk_python-2.6.1/symphony/bdk/__init__.py
--rw-r--r--   0        0        0      467 2023-06-05 08:53:30.722730 symphony_bdk_python-2.6.1/symphony/bdk/core/__init__.py
--rw-r--r--   0        0        0       66 2023-06-05 08:53:30.722730 symphony_bdk_python-2.6.1/symphony/bdk/core/activity/__init__.py
--rw-r--r--   0        0        0     2045 2023-06-05 08:53:30.722730 symphony_bdk_python-2.6.1/symphony/bdk/core/activity/api.py
--rw-r--r--   0        0        0     4698 2023-06-05 08:53:30.722730 symphony_bdk_python-2.6.1/symphony/bdk/core/activity/command.py
--rw-r--r--   0        0        0      183 2023-06-05 08:53:30.722730 symphony_bdk_python-2.6.1/symphony/bdk/core/activity/exception.py
--rw-r--r--   0        0        0     1454 2023-06-05 08:53:30.722730 symphony_bdk_python-2.6.1/symphony/bdk/core/activity/form.py
--rw-r--r--   0        0        0     1033 2023-06-05 08:53:30.722730 symphony_bdk_python-2.6.1/symphony/bdk/core/activity/help_command.py
--rw-r--r--   0        0        0     2957 2023-06-05 08:53:30.722730 symphony_bdk_python-2.6.1/symphony/bdk/core/activity/parsing/arguments.py
--rw-r--r--   0        0        0     5190 2023-06-05 08:53:30.722730 symphony_bdk_python-2.6.1/symphony/bdk/core/activity/parsing/command_token.py
--rw-r--r--   0        0        0     3632 2023-06-05 08:53:30.722730 symphony_bdk_python-2.6.1/symphony/bdk/core/activity/parsing/input_tokenizer.py
--rw-r--r--   0        0        0     1006 2023-06-05 08:53:30.722730 symphony_bdk_python-2.6.1/symphony/bdk/core/activity/parsing/match_result.py
--rw-r--r--   0        0        0     1611 2023-06-05 08:53:30.722730 symphony_bdk_python-2.6.1/symphony/bdk/core/activity/parsing/message_entities.py
--rw-r--r--   0        0        0     4422 2023-06-05 08:53:30.722730 symphony_bdk_python-2.6.1/symphony/bdk/core/activity/parsing/slash_command_pattern.py
--rw-r--r--   0        0        0     5231 2023-06-05 08:53:30.722730 symphony_bdk_python-2.6.1/symphony/bdk/core/activity/registry.py
--rw-r--r--   0        0        0     1203 2023-06-05 08:53:30.722730 symphony_bdk_python-2.6.1/symphony/bdk/core/activity/user_joined_room.py
--rw-r--r--   0        0        0       64 2023-06-05 08:53:30.722730 symphony_bdk_python-2.6.1/symphony/bdk/core/auth/__init__.py
--rw-r--r--   0        0        0     5518 2023-06-05 08:53:30.722730 symphony_bdk_python-2.6.1/symphony/bdk/core/auth/auth_session.py
--rw-r--r--   0        0        0     5367 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/auth/authenticator_factory.py
--rw-r--r--   0        0        0     3007 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/auth/bot_authenticator.py
--rw-r--r--   0        0        0      576 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/auth/exception.py
--rw-r--r--   0        0        0     7493 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/auth/ext_app_authenticator.py
--rw-r--r--   0        0        0     3470 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/auth/jwt_helper.py
--rw-r--r--   0        0        0     6183 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/auth/obo_authenticator.py
--rw-r--r--   0        0        0     1186 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/auth/tokens_repository.py
--rw-r--r--   0        0        0      171 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/client/__init__.py
--rw-r--r--   0        0        0     8355 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/client/api_client_factory.py
--rw-r--r--   0        0        0     3175 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/client/trace_id.py
--rw-r--r--   0        0        0       56 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/config/__init__.py
--rw-r--r--   0        0        0      400 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/config/exception.py
--rw-r--r--   0        0        0     2595 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/config/loader.py
--rw-r--r--   0        0        0        0 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/config/model/__init__.py
--rw-r--r--   0        0        0      479 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/config/model/bdk_app_config.py
--rw-r--r--   0        0        0     1999 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/config/model/bdk_authentication_config.py
--rw-r--r--   0        0        0      473 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/config/model/bdk_bot_config.py
--rw-r--r--   0        0        0     1271 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/config/model/bdk_certificate_config.py
--rw-r--r--   0        0        0     3347 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/config/model/bdk_client_config.py
--rw-r--r--   0        0        0     2086 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/config/model/bdk_config.py
--rw-r--r--   0        0        0     1817 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/config/model/bdk_datafeed_config.py
--rw-r--r--   0        0        0      726 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/config/model/bdk_datahose_config.py
--rw-r--r--   0        0        0      992 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/config/model/bdk_retry_config.py
--rw-r--r--   0        0        0     2028 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/config/model/bdk_rsa_key_config.py
--rw-r--r--   0        0        0     2833 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/config/model/bdk_server_config.py
--rw-r--r--   0        0        0      496 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/config/model/bdk_ssl_config.py
--rw-r--r--   0        0        0     4720 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/extension.py
--rw-r--r--   0        0        0     2525 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/retry/__init__.py
--rw-r--r--   0        0        0     4227 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/retry/_asyncio.py
--rw-r--r--   0        0        0     5824 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/retry/strategy.py
--rw-r--r--   0        0        0       97 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/service/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/service/application/__init__.py
--rw-r--r--   0        0        0     8763 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/service/application/application_service.py
--rw-r--r--   0        0        0        0 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/service/connection/__init__.py
--rw-r--r--   0        0        0     6634 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/service/connection/connection_service.py
--rw-r--r--   0        0        0        0 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/service/connection/model/__init__.py
--rw-r--r--   0        0        0      389 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/service/connection/model/connection_status.py
--rw-r--r--   0        0        0        0 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/service/datafeed/__init__.py
--rw-r--r--   0        0        0     3132 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/service/datafeed/abstract_ackId_event_loop.py
--rw-r--r--   0        0        0     8062 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/service/datafeed/abstract_datafeed_loop.py
--rw-r--r--   0        0        0     1508 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/service/datafeed/abstract_datahose_loop.py
--rw-r--r--   0        0        0     4226 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/service/datafeed/datafeed_loop_v1.py
--rw-r--r--   0        0        0     4810 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/service/datafeed/datafeed_loop_v2.py
--rw-r--r--   0        0        0     2671 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/service/datafeed/datahose_loop.py
--rw-r--r--   0        0        0      451 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/service/datafeed/exception.py
--rw-r--r--   0        0        0     2634 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/service/datafeed/on_disk_datafeed_id_repository.py
--rw-r--r--   0        0        0     6117 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/service/datafeed/real_time_event_listener.py
--rw-r--r--   0        0        0      321 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/service/exception.py
--rw-r--r--   0        0        0        0 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/service/health/__init__.py
--rw-r--r--   0        0        0     2032 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/service/health/health_service.py
--rw-r--r--   0        0        0        0 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/service/message/__init__.py
--rw-r--r--   0        0        0     3667 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/service/message/message_parser.py
--rw-r--r--   0        0        0    24473 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/service/message/message_service.py
--rw-r--r--   0        0        0     1295 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/service/message/messageml_util.py
--rw-r--r--   0        0        0     3943 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/service/message/model.py
--rw-r--r--   0        0        0    16134 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/service/message/multi_attachments_messages_api.py
--rw-r--r--   0        0        0     2885 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/service/obo_services.py
--rw-r--r--   0        0        0     3527 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/service/pagination.py
--rw-r--r--   0        0        0        0 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/service/presence/__init__.py
--rw-r--r--   0        0        0     9579 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/service/presence/presence_service.py
--rw-r--r--   0        0        0        0 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/service/session/__init__.py
--rw-r--r--   0        0        0     1201 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/service/session/session_service.py
--rw-r--r--   0        0        0        0 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/service/signal/__init__.py
--rw-r--r--   0        0        0     9211 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/service/signal/signal_service.py
--rw-r--r--   0        0        0        0 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/service/stream/__init__.py
--rw-r--r--   0        0        0    21088 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/service/stream/stream_service.py
--rw-r--r--   0        0        0     1029 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/service/stream/stream_util.py
--rw-r--r--   0        0        0        0 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/service/user/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/service/user/model/__init__.py
--rw-r--r--   0        0        0      174 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/service/user/model/delegate_action_enum.py
--rw-r--r--   0        0        0     1037 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/service/user/model/role_id.py
--rw-r--r--   0        0        0    36566 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/service/user/user_service.py
--rw-r--r--   0        0        0     1816 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/service/user/user_util.py
--rw-r--r--   0        0        0    10955 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/service_factory.py
--rw-r--r--   0        0        0    10801 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/core/symphony_bdk.py
--rw-r--r--   0        0        0        0 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/ext/__init__.py
--rw-r--r--   0        0        0    10265 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/ext/group.py
--rw-r--r--   0        0        0     2163 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/gen/__init__.py
--rw-r--r--   0        0        0       93 2023-06-05 08:53:30.726730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_api/__init__.py
--rw-r--r--   0        0        0    20509 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_api/attachments_api.py
--rw-r--r--   0        0        0    10347 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_api/audit_trail_api.py
--rw-r--r--   0        0        0    63950 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_api/datafeed_api.py
--rw-r--r--   0        0        0   126042 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_api/dlp_policies_and_dictionary_management_api.py
--rw-r--r--   0        0        0   104280 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_api/messages_api.py
--rw-r--r--   0        0        0    14022 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_api/share_api.py
--rw-r--r--   0        0        0    51289 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_api/signals_api.py
--rw-r--r--   0        0        0    25055 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_api/system_api.py
--rw-r--r--   0        0        0    13170 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_api/util_api.py
--rw-r--r--   0        0        0    49220 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_api/violations_api.py
--rw-r--r--   0        0        0       95 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/__init__.py
--rw-r--r--   0        0        0    13132 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/ack_id.py
--rw-r--r--   0        0        0    14676 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/agent_info.py
--rw-r--r--   0        0        0    12742 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/attachment_info.py
--rw-r--r--   0        0        0    13431 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/base_message.py
--rw-r--r--   0        0        0    13822 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/base_signal.py
--rw-r--r--   0        0        0    14235 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/channel_subscriber.py
--rw-r--r--   0        0        0    13407 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/channel_subscriber_response.py
--rw-r--r--   0        0        0    12960 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/channel_subscription_error.py
--rw-r--r--   0        0        0    13871 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/channel_subscription_response.py
--rw-r--r--   0        0        0    17116 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/connection_request_message.py
--rw-r--r--   0        0        0    13738 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/connection_request_message_all_of.py
--rw-r--r--   0        0        0    12239 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/datafeed.py
--rw-r--r--   0        0        0    12478 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/error.py
--rw-r--r--   0        0        0    13150 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/import_response.py
--rw-r--r--   0        0        0    12705 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/import_response_list.py
--rw-r--r--   0        0        0    14776 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/imported_message.py
--rw-r--r--   0        0        0    16072 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/message.py
--rw-r--r--   0        0        0    12936 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/message_all_of.py
--rw-r--r--   0        0        0    13188 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/message_import_list.py
--rw-r--r--   0        0        0    12613 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/message_list.py
--rw-r--r--   0        0        0    15645 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/message_search_query.py
--rw-r--r--   0        0        0    12626 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/message_submission.py
--rw-r--r--   0        0        0    13731 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/pagination.py
--rw-r--r--   0        0        0    12934 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/pagination_cursors.py
--rw-r--r--   0        0        0    18391 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/room_created_message.py
--rw-r--r--   0        0        0    15044 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/room_created_message_all_of.py
--rw-r--r--   0        0        0    15781 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/room_deactivated_message.py
--rw-r--r--   0        0        0    12413 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/room_deactivated_message_all_of.py
--rw-r--r--   0        0        0    16130 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/room_member_demoted_from_owner_message.py
--rw-r--r--   0        0        0    12704 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/room_member_demoted_from_owner_message_all_of.py
--rw-r--r--   0        0        0    16134 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/room_member_promoted_to_owner_message.py
--rw-r--r--   0        0        0    12713 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/room_member_promoted_to_owner_message_all_of.py
--rw-r--r--   0        0        0    15781 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/room_reactivated_message.py
--rw-r--r--   0        0        0    12413 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/room_reactivated_message_all_of.py
--rw-r--r--   0        0        0    12566 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/room_tag.py
--rw-r--r--   0        0        0    18047 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/room_updated_message.py
--rw-r--r--   0        0        0    14700 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/room_updated_message_all_of.py
--rw-r--r--   0        0        0    16284 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/share_article.py
--rw-r--r--   0        0        0    12821 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/share_content.py
--rw-r--r--   0        0        0    16631 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/signal.py
--rw-r--r--   0        0        0    13007 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/signal_all_of.py
--rw-r--r--   0        0        0    12600 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/signal_list.py
--rw-r--r--   0        0        0    12284 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/simple_message.py
--rw-r--r--   0        0        0    12608 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/success_response.py
--rw-r--r--   0        0        0    16049 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/user_joined_room_message.py
--rw-r--r--   0        0        0    12685 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/user_joined_room_message_all_of.py
--rw-r--r--   0        0        0    16421 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/user_left_room_message.py
--rw-r--r--   0        0        0    13067 2023-06-05 08:53:30.730730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/user_left_room_message_all_of.py
--rw-r--r--   0        0        0    12987 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_audit_trail_initiator_list.py
--rw-r--r--   0        0        0    14287 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_audit_trail_initiator_response.py
--rw-r--r--   0        0        0    12303 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_dlp_content_type.py
--rw-r--r--   0        0        0    13142 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_dlp_dictionary.py
--rw-r--r--   0        0        0    13026 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_dlp_dictionary_content.py
--rw-r--r--   0        0        0    14217 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_dlp_dictionary_metadata.py
--rw-r--r--   0        0        0    13267 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_dlp_dictionary_metadata_collection_response.py
--rw-r--r--   0        0        0    12919 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_dlp_dictionary_metadata_create_request.py
--rw-r--r--   0        0        0    12563 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_dlp_dictionary_metadata_response.py
--rw-r--r--   0        0        0    12388 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_dlp_dictionary_metadata_update_request.py
--rw-r--r--   0        0        0    13549 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_dlp_dictionary_ref.py
--rw-r--r--   0        0        0    14116 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_dlp_matched_policy.py
--rw-r--r--   0        0        0    12943 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_dlp_matched_policy_list.py
--rw-r--r--   0        0        0    12319 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_dlp_outcome.py
--rw-r--r--   0        0        0    13151 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_dlp_policies_collection_response.py
--rw-r--r--   0        0        0    17758 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_dlp_policy.py
--rw-r--r--   0        0        0    14572 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_dlp_policy_request.py
--rw-r--r--   0        0        0    12423 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_dlp_policy_response.py
--rw-r--r--   0        0        0    13212 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_dlp_signal.py
--rw-r--r--   0        0        0    19191 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_dlp_stream.py
--rw-r--r--   0        0        0    16771 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_dlp_violation.py
--rw-r--r--   0        0        0    13460 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_dlp_violation_message.py
--rw-r--r--   0        0        0    13300 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_dlp_violation_message_response.py
--rw-r--r--   0        0        0    12848 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_dlp_violation_signal.py
--rw-r--r--   0        0        0    13317 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_dlp_violation_signal_response.py
--rw-r--r--   0        0        0    12848 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_dlp_violation_stream.py
--rw-r--r--   0        0        0    13125 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_dlp_violation_stream_response.py
--rw-r--r--   0        0        0    14168 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_health_check_response.py
--rw-r--r--   0        0        0    15600 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v2_base_message.py
--rw-r--r--   0        0        0    12990 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v2_error.py
--rw-r--r--   0        0        0    19393 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v2_health_check_response.py
--rw-r--r--   0        0        0    14012 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v2_import_response.py
--rw-r--r--   0        0        0    12732 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v2_import_response_list.py
--rw-r--r--   0        0        0    15182 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v2_imported_message.py
--rw-r--r--   0        0        0    16657 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v2_message.py
--rw-r--r--   0        0        0    13484 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v2_message_all_of.py
--rw-r--r--   0        0        0    13215 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v2_message_import_list.py
--rw-r--r--   0        0        0    12681 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v2_message_list.py
--rw-r--r--   0        0        0    13174 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v2_message_submission.py
--rw-r--r--   0        0        0    12746 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v3_dlp_dictionary_meta.py
--rw-r--r--   0        0        0    13751 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v3_dlp_file_classifier_config.py
--rw-r--r--   0        0        0    12813 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v3_dlp_file_extension_config.py
--rw-r--r--   0        0        0    13406 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v3_dlp_file_password_config.py
--rw-r--r--   0        0        0    12319 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v3_dlp_file_size_config.py
--rw-r--r--   0        0        0    13461 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v3_dlp_policies_collection_response.py
--rw-r--r--   0        0        0    17561 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v3_dlp_policy.py
--rw-r--r--   0        0        0    13440 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v3_dlp_policy_applies_to.py
--rw-r--r--   0        0        0    13660 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v3_dlp_policy_request.py
--rw-r--r--   0        0        0    12423 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v3_dlp_policy_response.py
--rw-r--r--   0        0        0    15665 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v3_dlp_rule.py
--rw-r--r--   0        0        0    13668 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v3_dlp_text_match_config.py
--rw-r--r--   0        0        0    16430 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v3_dlp_violation.py
--rw-r--r--   0        0        0    13761 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v3_dlp_violation_message.py
--rw-r--r--   0        0        0    13302 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v3_dlp_violation_message_response.py
--rw-r--r--   0        0        0    12848 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v3_dlp_violation_signal.py
--rw-r--r--   0        0        0    13317 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v3_dlp_violation_signal_response.py
--rw-r--r--   0        0        0    12848 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v3_dlp_violation_stream.py
--rw-r--r--   0        0        0    13125 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v3_dlp_violation_stream_response.py
--rw-r--r--   0        0        0    13512 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v3_health.py
--rw-r--r--   0        0        0    12818 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v3_health_auth_type.py
--rw-r--r--   0        0        0    13509 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v3_health_component.py
--rw-r--r--   0        0        0    12822 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v3_health_status.py
--rw-r--r--   0        0        0    13148 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_attachment_info.py
--rw-r--r--   0        0        0    12414 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_connection_accepted.py
--rw-r--r--   0        0        0    12405 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_connection_requested.py
--rw-r--r--   0        0        0    15142 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_event.py
--rw-r--r--   0        0        0    12614 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_event_list.py
--rw-r--r--   0        0        0    14012 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_import_response.py
--rw-r--r--   0        0        0    12732 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_import_response_list.py
--rw-r--r--   0        0        0    16216 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_imported_message.py
--rw-r--r--   0        0        0    12700 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_imported_message_attachment.py
--rw-r--r--   0        0        0    12358 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_initiator.py
--rw-r--r--   0        0        0    12422 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_instant_message_created.py
--rw-r--r--   0        0        0    12487 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_key_value_pair.py
--rw-r--r--   0        0        0    20752 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_message.py
--rw-r--r--   0        0        0    13144 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_message_blast_response.py
--rw-r--r--   0        0        0    13211 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_message_import_list.py
--rw-r--r--   0        0        0    12640 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_message_list.py
--rw-r--r--   0        0        0    12406 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_message_sent.py
--rw-r--r--   0        0        0    12663 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_message_suppressed.py
--rw-r--r--   0        0        0    20135 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_payload.py
--rw-r--r--   0        0        0    12853 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_room_created.py
--rw-r--r--   0        0        0    12404 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_room_deactivated.py
--rw-r--r--   0        0        0    12805 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_room_member_demoted_from_owner.py
--rw-r--r--   0        0        0    12802 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_room_member_promoted_to_owner.py
--rw-r--r--   0        0        0    15839 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_room_properties.py
--rw-r--r--   0        0        0    12404 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_room_reactivated.py
--rw-r--r--   0        0        0    12876 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_room_updated.py
--rw-r--r--   0        0        0    12704 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_shared_post.py
--rw-r--r--   0        0        0    13909 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_stream.py
--rw-r--r--   0        0        0    13720 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_symphony_elements_action.py
--rw-r--r--   0        0        0    12600 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_thumbnail_info.py
--rw-r--r--   0        0        0    13733 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_user.py
--rw-r--r--   0        0        0    12769 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_user_joined_room.py
--rw-r--r--   0        0        0    12763 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_user_left_room.py
--rw-r--r--   0        0        0    12942 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_user_requested_to_join_room.py
--rw-r--r--   0        0        0    12970 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v5_datafeed.py
--rw-r--r--   0        0        0    12461 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v5_datafeed_create_body.py
--rw-r--r--   0        0        0     8582 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v5_datafeed_event_type.py
--rw-r--r--   0        0        0     8508 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v5_datafeed_type.py
--rw-r--r--   0        0        0    12953 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v5_event_list.py
--rw-r--r--   0        0        0    15099 2023-06-05 08:53:30.734730 symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v5_events_read_body.py
--rw-r--r--   0        0        0    38811 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/api_client.py
--rw-r--r--   0        0        0       93 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/auth_api/__init__.py
--rw-r--r--   0        0        0     6384 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/auth_api/authentication_api.py
--rw-r--r--   0        0        0    31054 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/auth_api/certificate_authentication_api.py
--rw-r--r--   0        0        0     5939 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/auth_api/certificate_pod_api.py
--rw-r--r--   0        0        0       95 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/auth_model/__init__.py
--rw-r--r--   0        0        0    11901 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/auth_model/error.py
--rw-r--r--   0        0        0    11830 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/auth_model/extension_app_authenticate_request.py
--rw-r--r--   0        0        0    12982 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/auth_model/extension_app_tokens.py
--rw-r--r--   0        0        0    12180 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/auth_model/obo_auth_response.py
--rw-r--r--   0        0        0    11788 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/auth_model/pod_certificate.py
--rw-r--r--   0        0        0    11713 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/auth_model/success_response.py
--rw-r--r--   0        0        0    13182 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/auth_model/token.py
--rw-r--r--   0        0        0    17598 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/configuration.py
--rw-r--r--   0        0        0     6469 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/exceptions.py
--rw-r--r--   0        0        0       95 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/group_api/__init__.py
--rw-r--r--   0        0        0    40707 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/group_api/group_api.py
--rw-r--r--   0        0        0    12462 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/group_api/type_api.py
--rw-r--r--   0        0        0       95 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/__init__.py
--rw-r--r--   0        0        0    11222 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/add_member.py
--rw-r--r--   0        0        0    11316 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/avatar.py
--rw-r--r--   0        0        0    12250 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/base_group.py
--rw-r--r--   0        0        0    15701 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/base_profile.py
--rw-r--r--   0        0        0    12044 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/base_type.py
--rw-r--r--   0        0        0    17834 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/create_group.py
--rw-r--r--   0        0        0    14454 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/create_group_all_of.py
--rw-r--r--   0        0        0    12684 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/error.py
--rw-r--r--   0        0        0    11597 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/group_implicit_connection.py
--rw-r--r--   0        0        0    11612 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/group_interaction_transfer.py
--rw-r--r--   0        0        0    11629 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/group_list.py
--rw-r--r--   0        0        0    11618 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/group_visibility_restriction.py
--rw-r--r--   0        0        0    11810 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/implicit_connection.py
--rw-r--r--   0        0        0    12802 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/interaction_control.py
--rw-r--r--   0        0        0    12851 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/interaction_transfer.py
--rw-r--r--   0        0        0    11480 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/member.py
--rw-r--r--   0        0        0    13268 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/membership_control.py
--rw-r--r--   0        0        0    11802 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/owner.py
--rw-r--r--   0        0        0    12212 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/pagination.py
--rw-r--r--   0        0        0    11827 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/pagination_cursors.py
--rw-r--r--   0        0        0    18502 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/profile.py
--rw-r--r--   0        0        0    11509 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/profile_all_of.py
--rw-r--r--   0        0        0    13530 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/profile_control.py
--rw-r--r--   0        0        0    19703 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/read_group.py
--rw-r--r--   0        0        0    16333 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/read_group_all_of.py
--rw-r--r--   0        0        0    14902 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/read_member.py
--rw-r--r--   0        0        0    12124 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/read_member_all_of.py
--rw-r--r--   0        0        0    11632 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/sort_order.py
--rw-r--r--   0        0        0    11839 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/status.py
--rw-r--r--   0        0        0    11790 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/transfer_view.py
--rw-r--r--   0        0        0    15640 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/type.py
--rw-r--r--   0        0        0    12326 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/type_all_of.py
--rw-r--r--   0        0        0    11618 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/type_list.py
--rw-r--r--   0        0        0    18774 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/update_group.py
--rw-r--r--   0        0        0    11847 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/update_group_all_of.py
--rw-r--r--   0        0        0    11386 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/upload_avatar.py
--rw-r--r--   0        0        0    11855 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/visibility_restriction.py
--rw-r--r--   0        0        0       93 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/login_api/__init__.py
--rw-r--r--   0        0        0    37169 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/login_api/authentication_api.py
--rw-r--r--   0        0        0       95 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/login_model/__init__.py
--rw-r--r--   0        0        0    12235 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/login_model/authenticate_extension_app_request.py
--rw-r--r--   0        0        0    11917 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/login_model/authenticate_request.py
--rw-r--r--   0        0        0    11853 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/login_model/error.py
--rw-r--r--   0        0        0    12934 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/login_model/extension_app_tokens.py
--rw-r--r--   0        0        0    11748 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/login_model/jwks.py
--rw-r--r--   0        0        0    11354 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/login_model/jwks_entry.py
--rw-r--r--   0        0        0    12712 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/login_model/jwt_token.py
--rw-r--r--   0        0        0    13134 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/login_model/token.py
--rw-r--r--   0        0        0    83460 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/model_utils.py
--rw-r--r--   0        0        0       93 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_api/__init__.py
--rw-r--r--   0        0        0    27908 2023-06-05 08:53:30.738730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_api/app_entitlement_api.py
--rw-r--r--   0        0        0    22182 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_api/application_api.py
--rw-r--r--   0        0        0    34487 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_api/connection_api.py
--rw-r--r--   0        0        0    35945 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_api/default_api.py
--rw-r--r--   0        0        0    16431 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_api/disclaimer_api.py
--rw-r--r--   0        0        0    27615 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_api/info_barriers_api.py
--rw-r--r--   0        0        0     6515 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_api/message_api.py
--rw-r--r--   0        0        0     6673 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_api/message_suppression_api.py
--rw-r--r--   0        0        0    14837 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_api/pod_api.py
--rw-r--r--   0        0        0    50456 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_api/presence_api.py
--rw-r--r--   0        0        0    44405 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_api/room_membership_api.py
--rw-r--r--   0        0        0    44128 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_api/security_api.py
--rw-r--r--   0        0        0     6172 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_api/session_api.py
--rw-r--r--   0        0        0    83658 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_api/streams_api.py
--rw-r--r--   0        0        0    26618 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_api/system_api.py
--rw-r--r--   0        0        0   130397 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_api/user_api.py
--rw-r--r--   0        0        0    19811 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_api/users_api.py
--rw-r--r--   0        0        0       95 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/__init__.py
--rw-r--r--   0        0        0    11800 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/admin_justified_action.py
--rw-r--r--   0        0        0    12111 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/admin_justified_user_action.py
--rw-r--r--   0        0        0     9151 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/admin_stream_attributes.py
--rw-r--r--   0        0        0     9460 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/admin_stream_filter.py
--rw-r--r--   0        0        0     8607 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/admin_stream_info.py
--rw-r--r--   0        0        0     7523 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/admin_stream_info_list.py
--rw-r--r--   0        0        0     8267 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/admin_stream_list.py
--rw-r--r--   0        0        0     7200 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/admin_stream_type_enum.py
--rw-r--r--   0        0        0    12817 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/app_authentication_key.py
--rw-r--r--   0        0        0    12210 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/app_authentication_keys.py
--rw-r--r--   0        0        0    12050 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/app_notification.py
--rw-r--r--   0        0        0    12671 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/app_properties.py
--rw-r--r--   0        0        0    12397 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/app_property.py
--rw-r--r--   0        0        0    16367 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/application_detail.py
--rw-r--r--   0        0        0    13117 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/application_info.py
--rw-r--r--   0        0        0    13318 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/assignee_candidate.py
--rw-r--r--   0        0        0    12246 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/assignee_candidates.py
--rw-r--r--   0        0        0    11994 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/attachment_preview.py
--rw-r--r--   0        0        0    11910 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/avatar.py
--rw-r--r--   0        0        0    11983 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/avatar_list.py
--rw-r--r--   0        0        0    11774 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/avatar_update.py
--rw-r--r--   0        0        0    12069 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/bulk_action_result.py
--rw-r--r--   0        0        0    12039 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/cert_info.py
--rw-r--r--   0        0        0    12065 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/cert_info_item.py
--rw-r--r--   0        0        0    12178 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/company_cert.py
--rw-r--r--   0        0        0    12556 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/company_cert_attributes.py
--rw-r--r--   0        0        0    12810 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/company_cert_detail.py
--rw-r--r--   0        0        0    13899 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/company_cert_info.py
--rw-r--r--   0        0        0    12305 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/company_cert_info_list.py
--rw-r--r--   0        0        0    11827 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/company_cert_status.py
--rw-r--r--   0        0        0    11859 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/company_cert_type.py
--rw-r--r--   0        0        0    12102 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/company_cert_type_list.py
--rw-r--r--   0        0        0    11865 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/conversation_specific_stream_attributes.py
--rw-r--r--   0        0        0    11991 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/delegate_action.py
--rw-r--r--   0        0        0    13744 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/disclaimer.py
--rw-r--r--   0        0        0    12035 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/disclaimer_list.py
--rw-r--r--   0        0        0    11947 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/download_receipt_count.py
--rw-r--r--   0        0        0    11861 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/error.py
--rw-r--r--   0        0        0    11969 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/faceted_match_count.py
--rw-r--r--   0        0        0    12009 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/feature.py
--rw-r--r--   0        0        0    11996 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/feature_list.py
--rw-r--r--   0        0        0    13231 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/file_extension.py
--rw-r--r--   0        0        0    11847 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/file_extensions_response.py
--rw-r--r--   0        0        0    11808 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/followers_list.py
--rw-r--r--   0        0        0    12320 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/followers_list_response.py
--rw-r--r--   0        0        0    12320 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/following_list_response.py
--rw-r--r--   0        0        0    13120 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/group.py
--rw-r--r--   0        0        0    12034 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/group_item.py
--rw-r--r--   0        0        0    11970 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/group_list.py
--rw-r--r--   0        0        0    12742 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/group_role_scope.py
--rw-r--r--   0        0        0    12463 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/im_system_info.py
--rw-r--r--   0        0        0    12603 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/immutable_room_attributes.py
--rw-r--r--   0        0        0    11885 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/integer_list.py
--rw-r--r--   0        0        0    11795 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/languages.py
--rw-r--r--   0        0        0    12723 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/member_info.py
--rw-r--r--   0        0        0    12658 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/membership_data.py
--rw-r--r--   0        0        0    12148 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/membership_list.py
--rw-r--r--   0        0        0    14624 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/message_detail.py
--rw-r--r--   0        0        0    12134 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/message_details.py
--rw-r--r--   0        0        0    11944 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/message_download_receipt_count.py
--rw-r--r--   0        0        0    11809 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/message_ids.py
--rw-r--r--   0        0        0     7794 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/message_ids_from_stream.py
--rw-r--r--   0        0        0    13005 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/message_metadata_response.py
--rw-r--r--   0        0        0    12244 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/message_metadata_response_parent.py
--rw-r--r--   0        0        0    13608 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/message_receipt_detail.py
--rw-r--r--   0        0        0    15316 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/message_receipt_detail_response.py
--rw-r--r--   0        0        0    13350 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/message_status.py
--rw-r--r--   0        0        0    13162 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/message_status_user.py
--rw-r--r--   0        0        0    12114 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/message_stream.py
--rw-r--r--   0        0        0    12358 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/message_suppression_response.py
--rw-r--r--   0        0        0    11849 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/message_user.py
--rw-r--r--   0        0        0    11873 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/name_value_pair.py
--rw-r--r--   0        0        0    13112 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/pagination.py
--rw-r--r--   0        0        0    12332 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/pagination_cursors.py
--rw-r--r--   0        0        0    12752 2023-06-05 08:53:30.742730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/password.py
--rw-r--r--   0        0        0    11834 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/password_reset.py
--rw-r--r--   0        0        0    13356 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/pod_app_entitlement.py
--rw-r--r--   0        0        0    12128 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/pod_app_entitlement_list.py
--rw-r--r--   0        0        0    11748 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/pod_certificate.py
--rw-r--r--   0        0        0    13251 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/policy.py
--rw-r--r--   0        0        0    11983 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/policy_list.py
--rw-r--r--   0        0        0     7428 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/presence.py
--rw-r--r--   0        0        0    13083 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/product.py
--rw-r--r--   0        0        0    11996 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/product_list.py
--rw-r--r--   0        0        0    11759 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/protocol.py
--rw-r--r--   0        0        0    12088 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/role.py
--rw-r--r--   0        0        0    12412 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/role_detail.py
--rw-r--r--   0        0        0    12036 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/role_detail_list.py
--rw-r--r--   0        0        0    11957 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/role_list.py
--rw-r--r--   0        0        0    13076 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/room_attributes.py
--rw-r--r--   0        0        0     7759 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/room_create.py
--rw-r--r--   0        0        0    12887 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/room_detail.py
--rw-r--r--   0        0        0    14341 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/room_search_criteria.py
--rw-r--r--   0        0        0     8737 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/room_search_results.py
--rw-r--r--   0        0        0    11718 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/room_specific_stream_attributes.py
--rw-r--r--   0        0        0    12768 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/room_system_info.py
--rw-r--r--   0        0        0    11949 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/room_tag.py
--rw-r--r--   0        0        0     7088 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/session_info.py
--rw-r--r--   0        0        0    11616 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/stream.py
--rw-r--r--   0        0        0    13706 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/stream_attachment_item.py
--rw-r--r--   0        0        0    12167 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/stream_attachment_response.py
--rw-r--r--   0        0        0    13880 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/stream_attributes.py
--rw-r--r--   0        0        0    12361 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/stream_filter.py
--rw-r--r--   0        0        0    12328 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/stream_list.py
--rw-r--r--   0        0        0    11778 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/stream_type.py
--rw-r--r--   0        0        0    11622 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/string_id.py
--rw-r--r--   0        0        0    11882 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/string_list.py
--rw-r--r--   0        0        0    11991 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/success_response.py
--rw-r--r--   0        0        0     7263 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user.py
--rw-r--r--   0        0        0    13593 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_app_entitlement.py
--rw-r--r--   0        0        0    12141 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_app_entitlement_list.py
--rw-r--r--   0        0        0    14363 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_app_entitlement_patch.py
--rw-r--r--   0        0        0    12405 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_app_entitlement_patch_enum.py
--rw-r--r--   0        0        0    12398 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_app_entitlements_patch_list.py
--rw-r--r--   0        0        0    16006 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_attributes.py
--rw-r--r--   0        0        0    12834 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_compp.py
--rw-r--r--   0        0        0    13331 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_connection.py
--rw-r--r--   0        0        0    12088 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_connection_list.py
--rw-r--r--   0        0        0    11708 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_connection_request.py
--rw-r--r--   0        0        0     7753 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_create.py
--rw-r--r--   0        0        0    12635 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_data.py
--rw-r--r--   0        0        0    14169 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_detail.py
--rw-r--r--   0        0        0    12036 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_detail_list.py
--rw-r--r--   0        0        0    12471 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_error.py
--rw-r--r--   0        0        0    12240 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_filter.py
--rw-r--r--   0        0        0    14000 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_group_assignee.py
--rw-r--r--   0        0        0    12262 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_group_assignee_response.py
--rw-r--r--   0        0        0    11755 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_group_assignee_update.py
--rw-r--r--   0        0        0    14222 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_group_assignment_response.py
--rw-r--r--   0        0        0    12441 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_group_create.py
--rw-r--r--   0        0        0    12645 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_group_data.py
--rw-r--r--   0        0        0    13707 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_group_membership_data.py
--rw-r--r--   0        0        0    11704 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_group_membership_request.py
--rw-r--r--   0        0        0    12382 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_group_membership_response.py
--rw-r--r--   0        0        0    13699 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_group_membership_response_data.py
--rw-r--r--   0        0        0    11751 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_group_membership_update.py
--rw-r--r--   0        0        0    14333 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_group_response.py
--rw-r--r--   0        0        0    12250 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_group_response_list.py
--rw-r--r--   0        0        0    12481 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_group_update.py
--rw-r--r--   0        0        0    11616 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_id.py
--rw-r--r--   0        0        0    11882 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_id_list.py
--rw-r--r--   0        0        0    12242 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_info.py
--rw-r--r--   0        0        0    11658 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_name.py
--rw-r--r--   0        0        0    12010 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_name_list.py
--rw-r--r--   0        0        0    13976 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_search_filter.py
--rw-r--r--   0        0        0    12228 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_search_query.py
--rw-r--r--   0        0        0    13238 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_search_results.py
--rw-r--r--   0        0        0    13096 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_status.py
--rw-r--r--   0        0        0    12264 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_suspension.py
--rw-r--r--   0        0        0    15003 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_system_info.py
--rw-r--r--   0        0        0    16917 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_v2.py
--rw-r--r--   0        0        0    11942 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v1_im_attributes.py
--rw-r--r--   0        0        0    12291 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v1_im_detail.py
--rw-r--r--   0        0        0    14869 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_admin_stream_attributes.py
--rw-r--r--   0        0        0    14878 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_admin_stream_filter.py
--rw-r--r--   0        0        0    14623 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_admin_stream_info.py
--rw-r--r--   0        0        0    12213 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_admin_stream_info_list.py
--rw-r--r--   0        0        0    13231 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_admin_stream_list.py
--rw-r--r--   0        0        0    11661 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_admin_stream_type.py
--rw-r--r--   0        0        0    11871 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_conversation_specific_stream_attributes.py
--rw-r--r--   0        0        0    13427 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_member_info.py
--rw-r--r--   0        0        0    12063 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_member_info_list.py
--rw-r--r--   0        0        0    13640 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_member_user_detail.py
--rw-r--r--   0        0        0    12716 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_membership_list.py
--rw-r--r--   0        0        0    15004 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_presence.py
--rw-r--r--   0        0        0    11841 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_presence_all_of.py
--rw-r--r--   0        0        0    12036 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_presence_list.py
--rw-r--r--   0        0        0    12107 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_presence_status.py
--rw-r--r--   0        0        0     9167 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_room_attributes.py
--rw-r--r--   0        0        0     7670 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_room_detail.py
--rw-r--r--   0        0        0    16985 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_room_search_criteria.py
--rw-r--r--   0        0        0    11858 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_room_search_criteria_all_of.py
--rw-r--r--   0        0        0    12232 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_room_specific_stream_attributes.py
--rw-r--r--   0        0        0    14729 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_stream_attributes.py
--rw-r--r--   0        0        0    11646 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_stream_type.py
--rw-r--r--   0        0        0    18501 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_user_attributes.py
--rw-r--r--   0        0        0    12476 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_user_create.py
--rw-r--r--   0        0        0    14192 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_user_detail.py
--rw-r--r--   0        0        0    12063 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_user_detail_list.py
--rw-r--r--   0        0        0    12795 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_user_key_request.py
--rw-r--r--   0        0        0    12317 2023-06-05 08:53:30.746730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_user_list.py
--rw-r--r--   0        0        0    14643 2023-06-05 08:53:30.750730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_user_presence.py
--rw-r--r--   0        0        0    11796 2023-06-05 08:53:30.750730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_user_presence_all_of.py
--rw-r--r--   0        0        0    17278 2023-06-05 08:53:30.750730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v3_room_attributes.py
--rw-r--r--   0        0        0    12809 2023-06-05 08:53:30.750730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v3_room_detail.py
--rw-r--r--   0        0        0    13851 2023-06-05 08:53:30.750730 symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v3_room_search_results.py
--rw-r--r--   0        0        0    10209 2023-06-05 08:53:30.750730 symphony_bdk_python-2.6.1/symphony/bdk/gen/rest.py
--rw-r--r--   0        0        0     5854 1970-01-01 00:00:00.000000 symphony_bdk_python-2.6.1/PKG-INFO
+-rw-r--r--   0        0        0    11342 2023-02-20 11:55:09.851700 symphony_bdk_python-2.6.dev0/LICENSE
+-rw-r--r--   0        0        0     4670 2023-02-20 11:55:09.851700 symphony_bdk_python-2.6.dev0/README.md
+-rw-r--r--   0        0        0     1547 2023-02-20 11:55:10.003700 symphony_bdk_python-2.6.dev0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-02-20 11:55:10.003700 symphony_bdk_python-2.6.dev0/symphony/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-20 11:55:10.003700 symphony_bdk_python-2.6.dev0/symphony/bdk/__init__.py
+-rw-r--r--   0        0        0      467 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/__init__.py
+-rw-r--r--   0        0        0       66 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/activity/__init__.py
+-rw-r--r--   0        0        0     2045 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/activity/api.py
+-rw-r--r--   0        0        0     4698 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/activity/command.py
+-rw-r--r--   0        0        0      183 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/activity/exception.py
+-rw-r--r--   0        0        0     1454 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/activity/form.py
+-rw-r--r--   0        0        0     1033 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/activity/help_command.py
+-rw-r--r--   0        0        0     2957 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/activity/parsing/arguments.py
+-rw-r--r--   0        0        0     5190 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/activity/parsing/command_token.py
+-rw-r--r--   0        0        0     3632 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/activity/parsing/input_tokenizer.py
+-rw-r--r--   0        0        0     1006 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/activity/parsing/match_result.py
+-rw-r--r--   0        0        0     1611 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/activity/parsing/message_entities.py
+-rw-r--r--   0        0        0     4422 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/activity/parsing/slash_command_pattern.py
+-rw-r--r--   0        0        0     5231 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/activity/registry.py
+-rw-r--r--   0        0        0     1203 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/activity/user_joined_room.py
+-rw-r--r--   0        0        0       64 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/auth/__init__.py
+-rw-r--r--   0        0        0     5518 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/auth/auth_session.py
+-rw-r--r--   0        0        0     5367 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/auth/authenticator_factory.py
+-rw-r--r--   0        0        0     3007 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/auth/bot_authenticator.py
+-rw-r--r--   0        0        0      576 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/auth/exception.py
+-rw-r--r--   0        0        0     7493 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/auth/ext_app_authenticator.py
+-rw-r--r--   0        0        0     3470 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/auth/jwt_helper.py
+-rw-r--r--   0        0        0     6183 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/auth/obo_authenticator.py
+-rw-r--r--   0        0        0     1186 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/auth/tokens_repository.py
+-rw-r--r--   0        0        0      171 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/client/__init__.py
+-rw-r--r--   0        0        0     8355 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/client/api_client_factory.py
+-rw-r--r--   0        0        0     3175 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/client/trace_id.py
+-rw-r--r--   0        0        0       56 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/config/__init__.py
+-rw-r--r--   0        0        0      400 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/config/exception.py
+-rw-r--r--   0        0        0     2595 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/config/loader.py
+-rw-r--r--   0        0        0        0 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/config/model/__init__.py
+-rw-r--r--   0        0        0      479 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/config/model/bdk_app_config.py
+-rw-r--r--   0        0        0     1999 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/config/model/bdk_authentication_config.py
+-rw-r--r--   0        0        0      473 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/config/model/bdk_bot_config.py
+-rw-r--r--   0        0        0     1271 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/config/model/bdk_certificate_config.py
+-rw-r--r--   0        0        0     3347 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/config/model/bdk_client_config.py
+-rw-r--r--   0        0        0     2086 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/config/model/bdk_config.py
+-rw-r--r--   0        0        0     1817 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/config/model/bdk_datafeed_config.py
+-rw-r--r--   0        0        0      726 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/config/model/bdk_datahose_config.py
+-rw-r--r--   0        0        0      992 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/config/model/bdk_retry_config.py
+-rw-r--r--   0        0        0     2028 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/config/model/bdk_rsa_key_config.py
+-rw-r--r--   0        0        0     2833 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/config/model/bdk_server_config.py
+-rw-r--r--   0        0        0      496 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/config/model/bdk_ssl_config.py
+-rw-r--r--   0        0        0     4720 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/extension.py
+-rw-r--r--   0        0        0     2525 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/retry/__init__.py
+-rw-r--r--   0        0        0     4227 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/retry/_asyncio.py
+-rw-r--r--   0        0        0     5824 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/retry/strategy.py
+-rw-r--r--   0        0        0       97 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/application/__init__.py
+-rw-r--r--   0        0        0     8763 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/application/application_service.py
+-rw-r--r--   0        0        0        0 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/connection/__init__.py
+-rw-r--r--   0        0        0     6634 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/connection/connection_service.py
+-rw-r--r--   0        0        0        0 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/connection/model/__init__.py
+-rw-r--r--   0        0        0      389 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/connection/model/connection_status.py
+-rw-r--r--   0        0        0        0 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/datafeed/__init__.py
+-rw-r--r--   0        0        0     3132 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/datafeed/abstract_ackId_event_loop.py
+-rw-r--r--   0        0        0     8062 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/datafeed/abstract_datafeed_loop.py
+-rw-r--r--   0        0        0     1508 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/datafeed/abstract_datahose_loop.py
+-rw-r--r--   0        0        0     4226 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/datafeed/datafeed_loop_v1.py
+-rw-r--r--   0        0        0     4879 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/datafeed/datafeed_loop_v2.py
+-rw-r--r--   0        0        0     2671 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/datafeed/datahose_loop.py
+-rw-r--r--   0        0        0      451 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/datafeed/exception.py
+-rw-r--r--   0        0        0     2634 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/datafeed/on_disk_datafeed_id_repository.py
+-rw-r--r--   0        0        0     6117 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/datafeed/real_time_event_listener.py
+-rw-r--r--   0        0        0      321 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/exception.py
+-rw-r--r--   0        0        0        0 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/health/__init__.py
+-rw-r--r--   0        0        0     2032 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/health/health_service.py
+-rw-r--r--   0        0        0        0 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/message/__init__.py
+-rw-r--r--   0        0        0     3667 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/message/message_parser.py
+-rw-r--r--   0        0        0    24473 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/message/message_service.py
+-rw-r--r--   0        0        0     1295 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/message/messageml_util.py
+-rw-r--r--   0        0        0     3943 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/message/model.py
+-rw-r--r--   0        0        0    16134 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/message/multi_attachments_messages_api.py
+-rw-r--r--   0        0        0     2885 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/obo_services.py
+-rw-r--r--   0        0        0     3527 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/pagination.py
+-rw-r--r--   0        0        0        0 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/presence/__init__.py
+-rw-r--r--   0        0        0     9579 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/presence/presence_service.py
+-rw-r--r--   0        0        0        0 2023-02-20 11:55:10.007700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/session/__init__.py
+-rw-r--r--   0        0        0     1201 2023-02-20 11:55:10.011700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/session/session_service.py
+-rw-r--r--   0        0        0        0 2023-02-20 11:55:10.011700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/signal/__init__.py
+-rw-r--r--   0        0        0     9211 2023-02-20 11:55:10.011700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/signal/signal_service.py
+-rw-r--r--   0        0        0        0 2023-02-20 11:55:10.011700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/stream/__init__.py
+-rw-r--r--   0        0        0    21088 2023-02-20 11:55:10.011700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/stream/stream_service.py
+-rw-r--r--   0        0        0     1029 2023-02-20 11:55:10.011700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/stream/stream_util.py
+-rw-r--r--   0        0        0        0 2023-02-20 11:55:10.011700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/user/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-20 11:55:10.011700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/user/model/__init__.py
+-rw-r--r--   0        0        0      174 2023-02-20 11:55:10.011700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/user/model/delegate_action_enum.py
+-rw-r--r--   0        0        0     1037 2023-02-20 11:55:10.011700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/user/model/role_id.py
+-rw-r--r--   0        0        0    36566 2023-02-20 11:55:10.011700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/user/user_service.py
+-rw-r--r--   0        0        0     1816 2023-02-20 11:55:10.011700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/user/user_util.py
+-rw-r--r--   0        0        0    10955 2023-02-20 11:55:10.011700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/service_factory.py
+-rw-r--r--   0        0        0    10801 2023-02-20 11:55:10.011700 symphony_bdk_python-2.6.dev0/symphony/bdk/core/symphony_bdk.py
+-rw-r--r--   0        0        0        0 2023-02-20 11:55:10.011700 symphony_bdk_python-2.6.dev0/symphony/bdk/ext/__init__.py
+-rw-r--r--   0        0        0    10265 2023-02-20 11:55:10.011700 symphony_bdk_python-2.6.dev0/symphony/bdk/ext/group.py
+-rw-r--r--   0        0        0     2163 2023-02-20 11:55:10.011700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/__init__.py
+-rw-r--r--   0        0        0       93 2023-02-20 11:55:10.011700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_api/__init__.py
+-rw-r--r--   0        0        0    20509 2023-02-20 11:55:10.011700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_api/attachments_api.py
+-rw-r--r--   0        0        0    10347 2023-02-20 11:55:10.011700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_api/audit_trail_api.py
+-rw-r--r--   0        0        0    63950 2023-02-20 11:55:10.011700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_api/datafeed_api.py
+-rw-r--r--   0        0        0   126042 2023-02-20 11:55:10.011700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_api/dlp_policies_and_dictionary_management_api.py
+-rw-r--r--   0        0        0   104280 2023-02-20 11:55:10.011700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_api/messages_api.py
+-rw-r--r--   0        0        0    14022 2023-02-20 11:55:10.011700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_api/share_api.py
+-rw-r--r--   0        0        0    51289 2023-02-20 11:55:10.011700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_api/signals_api.py
+-rw-r--r--   0        0        0    25055 2023-02-20 11:55:10.011700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_api/system_api.py
+-rw-r--r--   0        0        0    13170 2023-02-20 11:55:10.011700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_api/util_api.py
+-rw-r--r--   0        0        0    49220 2023-02-20 11:55:10.011700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_api/violations_api.py
+-rw-r--r--   0        0        0       95 2023-02-20 11:55:10.011700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/__init__.py
+-rw-r--r--   0        0        0    13132 2023-02-20 11:55:10.011700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/ack_id.py
+-rw-r--r--   0        0        0    14676 2023-02-20 11:55:10.011700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/agent_info.py
+-rw-r--r--   0        0        0    12742 2023-02-20 11:55:10.011700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/attachment_info.py
+-rw-r--r--   0        0        0    13431 2023-02-20 11:55:10.011700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/base_message.py
+-rw-r--r--   0        0        0    13822 2023-02-20 11:55:10.011700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/base_signal.py
+-rw-r--r--   0        0        0    14235 2023-02-20 11:55:10.011700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/channel_subscriber.py
+-rw-r--r--   0        0        0    13407 2023-02-20 11:55:10.011700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/channel_subscriber_response.py
+-rw-r--r--   0        0        0    12960 2023-02-20 11:55:10.011700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/channel_subscription_error.py
+-rw-r--r--   0        0        0    13871 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/channel_subscription_response.py
+-rw-r--r--   0        0        0    17116 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/connection_request_message.py
+-rw-r--r--   0        0        0    13738 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/connection_request_message_all_of.py
+-rw-r--r--   0        0        0    12239 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/datafeed.py
+-rw-r--r--   0        0        0    12478 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/error.py
+-rw-r--r--   0        0        0    13150 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/import_response.py
+-rw-r--r--   0        0        0    12705 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/import_response_list.py
+-rw-r--r--   0        0        0    14776 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/imported_message.py
+-rw-r--r--   0        0        0    16072 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/message.py
+-rw-r--r--   0        0        0    12936 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/message_all_of.py
+-rw-r--r--   0        0        0    13188 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/message_import_list.py
+-rw-r--r--   0        0        0    12613 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/message_list.py
+-rw-r--r--   0        0        0    15645 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/message_search_query.py
+-rw-r--r--   0        0        0    12626 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/message_submission.py
+-rw-r--r--   0        0        0    13731 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/pagination.py
+-rw-r--r--   0        0        0    12934 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/pagination_cursors.py
+-rw-r--r--   0        0        0    18391 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/room_created_message.py
+-rw-r--r--   0        0        0    15044 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/room_created_message_all_of.py
+-rw-r--r--   0        0        0    15781 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/room_deactivated_message.py
+-rw-r--r--   0        0        0    12413 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/room_deactivated_message_all_of.py
+-rw-r--r--   0        0        0    16130 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/room_member_demoted_from_owner_message.py
+-rw-r--r--   0        0        0    12704 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/room_member_demoted_from_owner_message_all_of.py
+-rw-r--r--   0        0        0    16134 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/room_member_promoted_to_owner_message.py
+-rw-r--r--   0        0        0    12713 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/room_member_promoted_to_owner_message_all_of.py
+-rw-r--r--   0        0        0    15781 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/room_reactivated_message.py
+-rw-r--r--   0        0        0    12413 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/room_reactivated_message_all_of.py
+-rw-r--r--   0        0        0    12566 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/room_tag.py
+-rw-r--r--   0        0        0    18047 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/room_updated_message.py
+-rw-r--r--   0        0        0    14700 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/room_updated_message_all_of.py
+-rw-r--r--   0        0        0    16284 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/share_article.py
+-rw-r--r--   0        0        0    12821 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/share_content.py
+-rw-r--r--   0        0        0    16631 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/signal.py
+-rw-r--r--   0        0        0    13007 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/signal_all_of.py
+-rw-r--r--   0        0        0    12600 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/signal_list.py
+-rw-r--r--   0        0        0    12284 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/simple_message.py
+-rw-r--r--   0        0        0    12608 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/success_response.py
+-rw-r--r--   0        0        0    16049 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/user_joined_room_message.py
+-rw-r--r--   0        0        0    12685 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/user_joined_room_message_all_of.py
+-rw-r--r--   0        0        0    16421 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/user_left_room_message.py
+-rw-r--r--   0        0        0    13067 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/user_left_room_message_all_of.py
+-rw-r--r--   0        0        0    12987 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_audit_trail_initiator_list.py
+-rw-r--r--   0        0        0    14287 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_audit_trail_initiator_response.py
+-rw-r--r--   0        0        0    12303 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_dlp_content_type.py
+-rw-r--r--   0        0        0    13142 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_dlp_dictionary.py
+-rw-r--r--   0        0        0    13026 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_dlp_dictionary_content.py
+-rw-r--r--   0        0        0    14217 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_dlp_dictionary_metadata.py
+-rw-r--r--   0        0        0    13267 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_dlp_dictionary_metadata_collection_response.py
+-rw-r--r--   0        0        0    12919 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_dlp_dictionary_metadata_create_request.py
+-rw-r--r--   0        0        0    12563 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_dlp_dictionary_metadata_response.py
+-rw-r--r--   0        0        0    12388 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_dlp_dictionary_metadata_update_request.py
+-rw-r--r--   0        0        0    13549 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_dlp_dictionary_ref.py
+-rw-r--r--   0        0        0    14116 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_dlp_matched_policy.py
+-rw-r--r--   0        0        0    12943 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_dlp_matched_policy_list.py
+-rw-r--r--   0        0        0    12319 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_dlp_outcome.py
+-rw-r--r--   0        0        0    13151 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_dlp_policies_collection_response.py
+-rw-r--r--   0        0        0    17758 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_dlp_policy.py
+-rw-r--r--   0        0        0    14572 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_dlp_policy_request.py
+-rw-r--r--   0        0        0    12423 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_dlp_policy_response.py
+-rw-r--r--   0        0        0    13212 2023-02-20 11:55:10.015700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_dlp_signal.py
+-rw-r--r--   0        0        0    19191 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_dlp_stream.py
+-rw-r--r--   0        0        0    16771 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_dlp_violation.py
+-rw-r--r--   0        0        0    13460 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_dlp_violation_message.py
+-rw-r--r--   0        0        0    13300 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_dlp_violation_message_response.py
+-rw-r--r--   0        0        0    12848 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_dlp_violation_signal.py
+-rw-r--r--   0        0        0    13317 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_dlp_violation_signal_response.py
+-rw-r--r--   0        0        0    12848 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_dlp_violation_stream.py
+-rw-r--r--   0        0        0    13125 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_dlp_violation_stream_response.py
+-rw-r--r--   0        0        0    14168 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_health_check_response.py
+-rw-r--r--   0        0        0    15600 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v2_base_message.py
+-rw-r--r--   0        0        0    12990 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v2_error.py
+-rw-r--r--   0        0        0    19393 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v2_health_check_response.py
+-rw-r--r--   0        0        0    14012 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v2_import_response.py
+-rw-r--r--   0        0        0    12732 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v2_import_response_list.py
+-rw-r--r--   0        0        0    15182 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v2_imported_message.py
+-rw-r--r--   0        0        0    16657 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v2_message.py
+-rw-r--r--   0        0        0    13484 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v2_message_all_of.py
+-rw-r--r--   0        0        0    13215 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v2_message_import_list.py
+-rw-r--r--   0        0        0    12681 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v2_message_list.py
+-rw-r--r--   0        0        0    13174 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v2_message_submission.py
+-rw-r--r--   0        0        0    12746 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v3_dlp_dictionary_meta.py
+-rw-r--r--   0        0        0    13751 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v3_dlp_file_classifier_config.py
+-rw-r--r--   0        0        0    12813 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v3_dlp_file_extension_config.py
+-rw-r--r--   0        0        0    13406 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v3_dlp_file_password_config.py
+-rw-r--r--   0        0        0    12319 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v3_dlp_file_size_config.py
+-rw-r--r--   0        0        0    13461 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v3_dlp_policies_collection_response.py
+-rw-r--r--   0        0        0    17561 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v3_dlp_policy.py
+-rw-r--r--   0        0        0    13440 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v3_dlp_policy_applies_to.py
+-rw-r--r--   0        0        0    13660 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v3_dlp_policy_request.py
+-rw-r--r--   0        0        0    12423 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v3_dlp_policy_response.py
+-rw-r--r--   0        0        0    15665 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v3_dlp_rule.py
+-rw-r--r--   0        0        0    13668 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v3_dlp_text_match_config.py
+-rw-r--r--   0        0        0    16430 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v3_dlp_violation.py
+-rw-r--r--   0        0        0    13761 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v3_dlp_violation_message.py
+-rw-r--r--   0        0        0    13302 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v3_dlp_violation_message_response.py
+-rw-r--r--   0        0        0    12848 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v3_dlp_violation_signal.py
+-rw-r--r--   0        0        0    13317 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v3_dlp_violation_signal_response.py
+-rw-r--r--   0        0        0    12848 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v3_dlp_violation_stream.py
+-rw-r--r--   0        0        0    13125 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v3_dlp_violation_stream_response.py
+-rw-r--r--   0        0        0    13512 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v3_health.py
+-rw-r--r--   0        0        0    12818 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v3_health_auth_type.py
+-rw-r--r--   0        0        0    13509 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v3_health_component.py
+-rw-r--r--   0        0        0    12822 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v3_health_status.py
+-rw-r--r--   0        0        0    13148 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_attachment_info.py
+-rw-r--r--   0        0        0    12414 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_connection_accepted.py
+-rw-r--r--   0        0        0    12405 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_connection_requested.py
+-rw-r--r--   0        0        0    15142 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_event.py
+-rw-r--r--   0        0        0    12614 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_event_list.py
+-rw-r--r--   0        0        0    14012 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_import_response.py
+-rw-r--r--   0        0        0    12732 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_import_response_list.py
+-rw-r--r--   0        0        0    16216 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_imported_message.py
+-rw-r--r--   0        0        0    12700 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_imported_message_attachment.py
+-rw-r--r--   0        0        0    12358 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_initiator.py
+-rw-r--r--   0        0        0    12422 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_instant_message_created.py
+-rw-r--r--   0        0        0    12487 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_key_value_pair.py
+-rw-r--r--   0        0        0    20752 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_message.py
+-rw-r--r--   0        0        0    13144 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_message_blast_response.py
+-rw-r--r--   0        0        0    13211 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_message_import_list.py
+-rw-r--r--   0        0        0    12640 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_message_list.py
+-rw-r--r--   0        0        0    12406 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_message_sent.py
+-rw-r--r--   0        0        0    12663 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_message_suppressed.py
+-rw-r--r--   0        0        0    20135 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_payload.py
+-rw-r--r--   0        0        0    12853 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_room_created.py
+-rw-r--r--   0        0        0    12404 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_room_deactivated.py
+-rw-r--r--   0        0        0    12805 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_room_member_demoted_from_owner.py
+-rw-r--r--   0        0        0    12802 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_room_member_promoted_to_owner.py
+-rw-r--r--   0        0        0    15839 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_room_properties.py
+-rw-r--r--   0        0        0    12404 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_room_reactivated.py
+-rw-r--r--   0        0        0    12876 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_room_updated.py
+-rw-r--r--   0        0        0    12704 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_shared_post.py
+-rw-r--r--   0        0        0    13909 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_stream.py
+-rw-r--r--   0        0        0    13720 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_symphony_elements_action.py
+-rw-r--r--   0        0        0    12600 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_thumbnail_info.py
+-rw-r--r--   0        0        0    13733 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_user.py
+-rw-r--r--   0        0        0    12769 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_user_joined_room.py
+-rw-r--r--   0        0        0    12763 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_user_left_room.py
+-rw-r--r--   0        0        0    12942 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_user_requested_to_join_room.py
+-rw-r--r--   0        0        0    12970 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v5_datafeed.py
+-rw-r--r--   0        0        0    12461 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v5_datafeed_create_body.py
+-rw-r--r--   0        0        0     8582 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v5_datafeed_event_type.py
+-rw-r--r--   0        0        0     8508 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v5_datafeed_type.py
+-rw-r--r--   0        0        0    12953 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v5_event_list.py
+-rw-r--r--   0        0        0    15099 2023-02-20 11:55:10.019700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v5_events_read_body.py
+-rw-r--r--   0        0        0    38811 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/api_client.py
+-rw-r--r--   0        0        0       93 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/auth_api/__init__.py
+-rw-r--r--   0        0        0     6384 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/auth_api/authentication_api.py
+-rw-r--r--   0        0        0    31054 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/auth_api/certificate_authentication_api.py
+-rw-r--r--   0        0        0     5939 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/auth_api/certificate_pod_api.py
+-rw-r--r--   0        0        0       95 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/auth_model/__init__.py
+-rw-r--r--   0        0        0    11901 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/auth_model/error.py
+-rw-r--r--   0        0        0    11830 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/auth_model/extension_app_authenticate_request.py
+-rw-r--r--   0        0        0    12982 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/auth_model/extension_app_tokens.py
+-rw-r--r--   0        0        0    12180 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/auth_model/obo_auth_response.py
+-rw-r--r--   0        0        0    11788 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/auth_model/pod_certificate.py
+-rw-r--r--   0        0        0    11713 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/auth_model/success_response.py
+-rw-r--r--   0        0        0    13182 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/auth_model/token.py
+-rw-r--r--   0        0        0    17598 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/configuration.py
+-rw-r--r--   0        0        0     6469 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/exceptions.py
+-rw-r--r--   0        0        0       95 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_api/__init__.py
+-rw-r--r--   0        0        0    40707 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_api/group_api.py
+-rw-r--r--   0        0        0    12462 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_api/type_api.py
+-rw-r--r--   0        0        0       95 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/__init__.py
+-rw-r--r--   0        0        0    11222 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/add_member.py
+-rw-r--r--   0        0        0    11316 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/avatar.py
+-rw-r--r--   0        0        0    12250 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/base_group.py
+-rw-r--r--   0        0        0    15701 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/base_profile.py
+-rw-r--r--   0        0        0    12044 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/base_type.py
+-rw-r--r--   0        0        0    17834 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/create_group.py
+-rw-r--r--   0        0        0    14454 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/create_group_all_of.py
+-rw-r--r--   0        0        0    12684 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/error.py
+-rw-r--r--   0        0        0    11597 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/group_implicit_connection.py
+-rw-r--r--   0        0        0    11612 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/group_interaction_transfer.py
+-rw-r--r--   0        0        0    11629 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/group_list.py
+-rw-r--r--   0        0        0    11618 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/group_visibility_restriction.py
+-rw-r--r--   0        0        0    11810 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/implicit_connection.py
+-rw-r--r--   0        0        0    12802 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/interaction_control.py
+-rw-r--r--   0        0        0    12851 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/interaction_transfer.py
+-rw-r--r--   0        0        0    11480 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/member.py
+-rw-r--r--   0        0        0    13268 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/membership_control.py
+-rw-r--r--   0        0        0    11802 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/owner.py
+-rw-r--r--   0        0        0    12212 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/pagination.py
+-rw-r--r--   0        0        0    11827 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/pagination_cursors.py
+-rw-r--r--   0        0        0    18502 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/profile.py
+-rw-r--r--   0        0        0    11509 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/profile_all_of.py
+-rw-r--r--   0        0        0    13530 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/profile_control.py
+-rw-r--r--   0        0        0    19703 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/read_group.py
+-rw-r--r--   0        0        0    16333 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/read_group_all_of.py
+-rw-r--r--   0        0        0    14902 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/read_member.py
+-rw-r--r--   0        0        0    12124 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/read_member_all_of.py
+-rw-r--r--   0        0        0    11632 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/sort_order.py
+-rw-r--r--   0        0        0    11839 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/status.py
+-rw-r--r--   0        0        0    11790 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/transfer_view.py
+-rw-r--r--   0        0        0    15640 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/type.py
+-rw-r--r--   0        0        0    12326 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/type_all_of.py
+-rw-r--r--   0        0        0    11618 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/type_list.py
+-rw-r--r--   0        0        0    18774 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/update_group.py
+-rw-r--r--   0        0        0    11847 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/update_group_all_of.py
+-rw-r--r--   0        0        0    11386 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/upload_avatar.py
+-rw-r--r--   0        0        0    11855 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/visibility_restriction.py
+-rw-r--r--   0        0        0       93 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/login_api/__init__.py
+-rw-r--r--   0        0        0    37169 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/login_api/authentication_api.py
+-rw-r--r--   0        0        0       95 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/login_model/__init__.py
+-rw-r--r--   0        0        0    12235 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/login_model/authenticate_extension_app_request.py
+-rw-r--r--   0        0        0    11917 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/login_model/authenticate_request.py
+-rw-r--r--   0        0        0    11853 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/login_model/error.py
+-rw-r--r--   0        0        0    12934 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/login_model/extension_app_tokens.py
+-rw-r--r--   0        0        0    11748 2023-02-20 11:55:10.023700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/login_model/jwks.py
+-rw-r--r--   0        0        0    11354 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/login_model/jwks_entry.py
+-rw-r--r--   0        0        0    12712 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/login_model/jwt_token.py
+-rw-r--r--   0        0        0    13134 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/login_model/token.py
+-rw-r--r--   0        0        0    83460 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/model_utils.py
+-rw-r--r--   0        0        0       93 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_api/__init__.py
+-rw-r--r--   0        0        0    27908 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_api/app_entitlement_api.py
+-rw-r--r--   0        0        0    22182 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_api/application_api.py
+-rw-r--r--   0        0        0    34487 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_api/connection_api.py
+-rw-r--r--   0        0        0    35945 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_api/default_api.py
+-rw-r--r--   0        0        0    16431 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_api/disclaimer_api.py
+-rw-r--r--   0        0        0    27615 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_api/info_barriers_api.py
+-rw-r--r--   0        0        0     6515 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_api/message_api.py
+-rw-r--r--   0        0        0     6673 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_api/message_suppression_api.py
+-rw-r--r--   0        0        0    14837 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_api/pod_api.py
+-rw-r--r--   0        0        0    50456 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_api/presence_api.py
+-rw-r--r--   0        0        0    44405 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_api/room_membership_api.py
+-rw-r--r--   0        0        0    44128 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_api/security_api.py
+-rw-r--r--   0        0        0     6172 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_api/session_api.py
+-rw-r--r--   0        0        0    83658 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_api/streams_api.py
+-rw-r--r--   0        0        0    26618 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_api/system_api.py
+-rw-r--r--   0        0        0   130397 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_api/user_api.py
+-rw-r--r--   0        0        0    19811 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_api/users_api.py
+-rw-r--r--   0        0        0       95 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/__init__.py
+-rw-r--r--   0        0        0    11800 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/admin_justified_action.py
+-rw-r--r--   0        0        0    12111 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/admin_justified_user_action.py
+-rw-r--r--   0        0        0     9151 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/admin_stream_attributes.py
+-rw-r--r--   0        0        0     9460 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/admin_stream_filter.py
+-rw-r--r--   0        0        0     8607 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/admin_stream_info.py
+-rw-r--r--   0        0        0     7523 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/admin_stream_info_list.py
+-rw-r--r--   0        0        0     8267 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/admin_stream_list.py
+-rw-r--r--   0        0        0     7200 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/admin_stream_type_enum.py
+-rw-r--r--   0        0        0    12817 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/app_authentication_key.py
+-rw-r--r--   0        0        0    12210 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/app_authentication_keys.py
+-rw-r--r--   0        0        0    12050 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/app_notification.py
+-rw-r--r--   0        0        0    12671 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/app_properties.py
+-rw-r--r--   0        0        0    12397 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/app_property.py
+-rw-r--r--   0        0        0    16367 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/application_detail.py
+-rw-r--r--   0        0        0    13117 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/application_info.py
+-rw-r--r--   0        0        0    13318 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/assignee_candidate.py
+-rw-r--r--   0        0        0    12246 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/assignee_candidates.py
+-rw-r--r--   0        0        0    11994 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/attachment_preview.py
+-rw-r--r--   0        0        0    11910 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/avatar.py
+-rw-r--r--   0        0        0    11983 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/avatar_list.py
+-rw-r--r--   0        0        0    11774 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/avatar_update.py
+-rw-r--r--   0        0        0    12069 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/bulk_action_result.py
+-rw-r--r--   0        0        0    12039 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/cert_info.py
+-rw-r--r--   0        0        0    12065 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/cert_info_item.py
+-rw-r--r--   0        0        0    12178 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/company_cert.py
+-rw-r--r--   0        0        0    12556 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/company_cert_attributes.py
+-rw-r--r--   0        0        0    12810 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/company_cert_detail.py
+-rw-r--r--   0        0        0    13899 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/company_cert_info.py
+-rw-r--r--   0        0        0    12305 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/company_cert_info_list.py
+-rw-r--r--   0        0        0    11827 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/company_cert_status.py
+-rw-r--r--   0        0        0    11859 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/company_cert_type.py
+-rw-r--r--   0        0        0    12102 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/company_cert_type_list.py
+-rw-r--r--   0        0        0    11865 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/conversation_specific_stream_attributes.py
+-rw-r--r--   0        0        0    11991 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/delegate_action.py
+-rw-r--r--   0        0        0    13744 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/disclaimer.py
+-rw-r--r--   0        0        0    12035 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/disclaimer_list.py
+-rw-r--r--   0        0        0    11947 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/download_receipt_count.py
+-rw-r--r--   0        0        0    11861 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/error.py
+-rw-r--r--   0        0        0    11969 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/faceted_match_count.py
+-rw-r--r--   0        0        0    12009 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/feature.py
+-rw-r--r--   0        0        0    11996 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/feature_list.py
+-rw-r--r--   0        0        0    13231 2023-02-20 11:55:10.027700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/file_extension.py
+-rw-r--r--   0        0        0    11847 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/file_extensions_response.py
+-rw-r--r--   0        0        0    11808 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/followers_list.py
+-rw-r--r--   0        0        0    12320 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/followers_list_response.py
+-rw-r--r--   0        0        0    12320 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/following_list_response.py
+-rw-r--r--   0        0        0    13120 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/group.py
+-rw-r--r--   0        0        0    12034 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/group_item.py
+-rw-r--r--   0        0        0    11970 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/group_list.py
+-rw-r--r--   0        0        0    12742 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/group_role_scope.py
+-rw-r--r--   0        0        0    12463 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/im_system_info.py
+-rw-r--r--   0        0        0    12603 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/immutable_room_attributes.py
+-rw-r--r--   0        0        0    11885 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/integer_list.py
+-rw-r--r--   0        0        0    11795 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/languages.py
+-rw-r--r--   0        0        0    12723 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/member_info.py
+-rw-r--r--   0        0        0    12658 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/membership_data.py
+-rw-r--r--   0        0        0    12148 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/membership_list.py
+-rw-r--r--   0        0        0    14624 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/message_detail.py
+-rw-r--r--   0        0        0    12134 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/message_details.py
+-rw-r--r--   0        0        0    11944 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/message_download_receipt_count.py
+-rw-r--r--   0        0        0    11809 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/message_ids.py
+-rw-r--r--   0        0        0     7794 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/message_ids_from_stream.py
+-rw-r--r--   0        0        0    13005 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/message_metadata_response.py
+-rw-r--r--   0        0        0    12244 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/message_metadata_response_parent.py
+-rw-r--r--   0        0        0    13608 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/message_receipt_detail.py
+-rw-r--r--   0        0        0    15316 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/message_receipt_detail_response.py
+-rw-r--r--   0        0        0    13350 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/message_status.py
+-rw-r--r--   0        0        0    13162 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/message_status_user.py
+-rw-r--r--   0        0        0    12114 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/message_stream.py
+-rw-r--r--   0        0        0    12358 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/message_suppression_response.py
+-rw-r--r--   0        0        0    11849 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/message_user.py
+-rw-r--r--   0        0        0    11873 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/name_value_pair.py
+-rw-r--r--   0        0        0    13112 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/pagination.py
+-rw-r--r--   0        0        0    12332 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/pagination_cursors.py
+-rw-r--r--   0        0        0    12752 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/password.py
+-rw-r--r--   0        0        0    11834 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/password_reset.py
+-rw-r--r--   0        0        0    13356 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/pod_app_entitlement.py
+-rw-r--r--   0        0        0    12128 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/pod_app_entitlement_list.py
+-rw-r--r--   0        0        0    11748 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/pod_certificate.py
+-rw-r--r--   0        0        0    13251 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/policy.py
+-rw-r--r--   0        0        0    11983 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/policy_list.py
+-rw-r--r--   0        0        0     7428 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/presence.py
+-rw-r--r--   0        0        0    13083 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/product.py
+-rw-r--r--   0        0        0    11996 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/product_list.py
+-rw-r--r--   0        0        0    11759 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/protocol.py
+-rw-r--r--   0        0        0    12088 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/role.py
+-rw-r--r--   0        0        0    12412 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/role_detail.py
+-rw-r--r--   0        0        0    12036 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/role_detail_list.py
+-rw-r--r--   0        0        0    11957 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/role_list.py
+-rw-r--r--   0        0        0    13076 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/room_attributes.py
+-rw-r--r--   0        0        0     7759 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/room_create.py
+-rw-r--r--   0        0        0    12887 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/room_detail.py
+-rw-r--r--   0        0        0    14341 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/room_search_criteria.py
+-rw-r--r--   0        0        0     8737 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/room_search_results.py
+-rw-r--r--   0        0        0    11718 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/room_specific_stream_attributes.py
+-rw-r--r--   0        0        0    12768 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/room_system_info.py
+-rw-r--r--   0        0        0    11949 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/room_tag.py
+-rw-r--r--   0        0        0     7088 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/session_info.py
+-rw-r--r--   0        0        0    11616 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/stream.py
+-rw-r--r--   0        0        0    13706 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/stream_attachment_item.py
+-rw-r--r--   0        0        0    12167 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/stream_attachment_response.py
+-rw-r--r--   0        0        0    13880 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/stream_attributes.py
+-rw-r--r--   0        0        0    12361 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/stream_filter.py
+-rw-r--r--   0        0        0    12328 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/stream_list.py
+-rw-r--r--   0        0        0    11778 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/stream_type.py
+-rw-r--r--   0        0        0    11622 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/string_id.py
+-rw-r--r--   0        0        0    11882 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/string_list.py
+-rw-r--r--   0        0        0    11991 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/success_response.py
+-rw-r--r--   0        0        0     7263 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user.py
+-rw-r--r--   0        0        0    13593 2023-02-20 11:55:10.031700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_app_entitlement.py
+-rw-r--r--   0        0        0    12141 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_app_entitlement_list.py
+-rw-r--r--   0        0        0    14363 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_app_entitlement_patch.py
+-rw-r--r--   0        0        0    12405 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_app_entitlement_patch_enum.py
+-rw-r--r--   0        0        0    12398 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_app_entitlements_patch_list.py
+-rw-r--r--   0        0        0    16006 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_attributes.py
+-rw-r--r--   0        0        0    12834 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_compp.py
+-rw-r--r--   0        0        0    13331 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_connection.py
+-rw-r--r--   0        0        0    12088 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_connection_list.py
+-rw-r--r--   0        0        0    11708 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_connection_request.py
+-rw-r--r--   0        0        0     7753 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_create.py
+-rw-r--r--   0        0        0    12635 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_data.py
+-rw-r--r--   0        0        0    14169 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_detail.py
+-rw-r--r--   0        0        0    12036 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_detail_list.py
+-rw-r--r--   0        0        0    12471 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_error.py
+-rw-r--r--   0        0        0    12240 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_filter.py
+-rw-r--r--   0        0        0    14000 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_group_assignee.py
+-rw-r--r--   0        0        0    12262 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_group_assignee_response.py
+-rw-r--r--   0        0        0    11755 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_group_assignee_update.py
+-rw-r--r--   0        0        0    14222 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_group_assignment_response.py
+-rw-r--r--   0        0        0    12441 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_group_create.py
+-rw-r--r--   0        0        0    12645 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_group_data.py
+-rw-r--r--   0        0        0    13707 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_group_membership_data.py
+-rw-r--r--   0        0        0    11704 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_group_membership_request.py
+-rw-r--r--   0        0        0    12382 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_group_membership_response.py
+-rw-r--r--   0        0        0    13699 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_group_membership_response_data.py
+-rw-r--r--   0        0        0    11751 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_group_membership_update.py
+-rw-r--r--   0        0        0    14333 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_group_response.py
+-rw-r--r--   0        0        0    12250 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_group_response_list.py
+-rw-r--r--   0        0        0    12481 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_group_update.py
+-rw-r--r--   0        0        0    11616 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_id.py
+-rw-r--r--   0        0        0    11882 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_id_list.py
+-rw-r--r--   0        0        0    12242 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_info.py
+-rw-r--r--   0        0        0    11658 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_name.py
+-rw-r--r--   0        0        0    12010 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_name_list.py
+-rw-r--r--   0        0        0    13976 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_search_filter.py
+-rw-r--r--   0        0        0    12228 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_search_query.py
+-rw-r--r--   0        0        0    13238 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_search_results.py
+-rw-r--r--   0        0        0    13096 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_status.py
+-rw-r--r--   0        0        0    12264 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_suspension.py
+-rw-r--r--   0        0        0    15003 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_system_info.py
+-rw-r--r--   0        0        0    16917 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_v2.py
+-rw-r--r--   0        0        0    11942 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v1_im_attributes.py
+-rw-r--r--   0        0        0    12291 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v1_im_detail.py
+-rw-r--r--   0        0        0    14869 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_admin_stream_attributes.py
+-rw-r--r--   0        0        0    14878 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_admin_stream_filter.py
+-rw-r--r--   0        0        0    14623 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_admin_stream_info.py
+-rw-r--r--   0        0        0    12213 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_admin_stream_info_list.py
+-rw-r--r--   0        0        0    13231 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_admin_stream_list.py
+-rw-r--r--   0        0        0    11661 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_admin_stream_type.py
+-rw-r--r--   0        0        0    11871 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_conversation_specific_stream_attributes.py
+-rw-r--r--   0        0        0    13427 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_member_info.py
+-rw-r--r--   0        0        0    12063 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_member_info_list.py
+-rw-r--r--   0        0        0    13640 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_member_user_detail.py
+-rw-r--r--   0        0        0    12716 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_membership_list.py
+-rw-r--r--   0        0        0    15004 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_presence.py
+-rw-r--r--   0        0        0    11841 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_presence_all_of.py
+-rw-r--r--   0        0        0    12036 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_presence_list.py
+-rw-r--r--   0        0        0    12107 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_presence_status.py
+-rw-r--r--   0        0        0     9167 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_room_attributes.py
+-rw-r--r--   0        0        0     7670 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_room_detail.py
+-rw-r--r--   0        0        0    16985 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_room_search_criteria.py
+-rw-r--r--   0        0        0    11858 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_room_search_criteria_all_of.py
+-rw-r--r--   0        0        0    12232 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_room_specific_stream_attributes.py
+-rw-r--r--   0        0        0    14729 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_stream_attributes.py
+-rw-r--r--   0        0        0    11646 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_stream_type.py
+-rw-r--r--   0        0        0    18501 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_user_attributes.py
+-rw-r--r--   0        0        0    12476 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_user_create.py
+-rw-r--r--   0        0        0    14192 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_user_detail.py
+-rw-r--r--   0        0        0    12063 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_user_detail_list.py
+-rw-r--r--   0        0        0    12795 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_user_key_request.py
+-rw-r--r--   0        0        0    12317 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_user_list.py
+-rw-r--r--   0        0        0    14643 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_user_presence.py
+-rw-r--r--   0        0        0    11796 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_user_presence_all_of.py
+-rw-r--r--   0        0        0    17278 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v3_room_attributes.py
+-rw-r--r--   0        0        0    12809 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v3_room_detail.py
+-rw-r--r--   0        0        0    13851 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v3_room_search_results.py
+-rw-r--r--   0        0        0    10209 2023-02-20 11:55:10.035700 symphony_bdk_python-2.6.dev0/symphony/bdk/gen/rest.py
+-rw-r--r--   0        0        0     6793 1970-01-01 00:00:00.000000 symphony_bdk_python-2.6.dev0/setup.py
+-rw-r--r--   0        0        0     5857 1970-01-01 00:00:00.000000 symphony_bdk_python-2.6.dev0/PKG-INFO
```

### Comparing `symphony_bdk_python-2.6.1/LICENSE` & `symphony_bdk_python-2.6.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/README.md` & `symphony_bdk_python-2.6.dev0/README.md`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/pyproject.toml` & `symphony_bdk_python-2.6.dev0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "symphony_bdk_python"
-version = "2.6.1"
+version = "2.6.dev0"
 license = "Apache-2.0"
 description = "Symphony Bot Development Kit for Python"
 readme = "README.md"
 authors = ["Symphony Platform Solutions <symphony@finos.org>"]
 repository = "https://github.com/finos/symphony-bdk-python"
 documentation = "https://symphony-bdk-python.finos.org/"
 packages = [
@@ -15,15 +15,15 @@
 python = "^3.8"
 nulltype = "^2.3.1"
 python-dateutil = "^2.8.2"
 urllib3 = "^1.26.9"
 aiohttp = "^3.8.1"
 pyyaml = "^6.0"
 PyJWT = "^2.3.0"
-cryptography = "^40.0.2"
+cryptography = "^38.0.3"
 tenacity = "^8.0.1"
 defusedxml = "^0.7.1"
 docutils = "0.16"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.1"
 pylint = "^2.6.0"
```

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/activity/api.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/activity/api.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/activity/command.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/activity/command.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/activity/form.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/activity/form.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/activity/help_command.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/activity/help_command.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/activity/parsing/arguments.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/activity/parsing/arguments.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/activity/parsing/command_token.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/activity/parsing/command_token.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/activity/parsing/input_tokenizer.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/activity/parsing/input_tokenizer.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/activity/parsing/match_result.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/activity/parsing/match_result.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/activity/parsing/message_entities.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/activity/parsing/message_entities.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/activity/parsing/slash_command_pattern.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/activity/parsing/slash_command_pattern.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/activity/registry.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/activity/registry.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/activity/user_joined_room.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/activity/user_joined_room.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/auth/auth_session.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/auth/auth_session.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/auth/authenticator_factory.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/auth/authenticator_factory.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/auth/bot_authenticator.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/auth/bot_authenticator.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/auth/exception.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/auth/exception.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/auth/ext_app_authenticator.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/auth/ext_app_authenticator.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/auth/jwt_helper.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/auth/jwt_helper.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/auth/obo_authenticator.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/auth/obo_authenticator.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/auth/tokens_repository.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/auth/tokens_repository.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/client/api_client_factory.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/client/api_client_factory.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/client/trace_id.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/client/trace_id.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/config/loader.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/config/loader.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/config/model/bdk_authentication_config.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/config/model/bdk_authentication_config.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/config/model/bdk_certificate_config.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/config/model/bdk_certificate_config.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/config/model/bdk_client_config.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/config/model/bdk_client_config.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/config/model/bdk_config.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/config/model/bdk_config.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/config/model/bdk_datafeed_config.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/config/model/bdk_datafeed_config.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/config/model/bdk_datahose_config.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/config/model/bdk_datahose_config.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/config/model/bdk_retry_config.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/config/model/bdk_retry_config.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/config/model/bdk_rsa_key_config.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/config/model/bdk_rsa_key_config.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/config/model/bdk_server_config.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/config/model/bdk_server_config.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/extension.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/extension.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/retry/__init__.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/retry/__init__.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/retry/_asyncio.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/retry/_asyncio.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/retry/strategy.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/retry/strategy.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/service/application/application_service.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/application/application_service.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/service/connection/connection_service.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/connection/connection_service.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/service/datafeed/abstract_ackId_event_loop.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/datafeed/abstract_ackId_event_loop.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/service/datafeed/abstract_datafeed_loop.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/datafeed/abstract_datafeed_loop.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/service/datafeed/abstract_datahose_loop.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/datafeed/abstract_datahose_loop.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/service/datafeed/datafeed_loop_v1.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/datafeed/datafeed_loop_v1.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/service/datafeed/datafeed_loop_v2.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/datafeed/datafeed_loop_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,16 @@
         self._ack_id = ""
 
     @retry
     async def _retrieve_datafeed(self) -> Optional[V5Datafeed]:
         session_token = await self._auth_session.session_token
         key_manager_token = await self._auth_session.key_manager_token
         datafeeds = await self._datafeed_api.list_datafeed(session_token=session_token,
-                                                           key_manager_token=key_manager_token)
+                                                           key_manager_token=key_manager_token,
+                                                           tag=None)
 
         datafeeds = list(filter(lambda df: DATAFEED_V2_ID_PATTERN.match(df.id), datafeeds))
         if datafeeds:
             return datafeeds[0]
         return None
 
     @retry
```

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/service/datafeed/datahose_loop.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/datafeed/datahose_loop.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/service/datafeed/on_disk_datafeed_id_repository.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/datafeed/on_disk_datafeed_id_repository.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/service/datafeed/real_time_event_listener.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/datafeed/real_time_event_listener.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/service/health/health_service.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/health/health_service.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/service/message/message_parser.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/message/message_parser.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/service/message/message_service.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/message/message_service.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/service/message/messageml_util.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/message/messageml_util.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/service/message/model.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/message/model.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/service/message/multi_attachments_messages_api.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/message/multi_attachments_messages_api.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/service/obo_services.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/obo_services.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/service/pagination.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/pagination.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/service/presence/presence_service.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/presence/presence_service.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/service/session/session_service.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/session/session_service.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/service/signal/signal_service.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/signal/signal_service.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/service/stream/stream_service.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/stream/stream_service.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/service/stream/stream_util.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/stream/stream_util.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/service/user/model/role_id.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/user/model/role_id.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/service/user/user_service.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/user/user_service.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/service/user/user_util.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/service/user/user_util.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/service_factory.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/service_factory.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/core/symphony_bdk.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/core/symphony_bdk.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/ext/group.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/ext/group.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/__init__.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/__init__.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_api/attachments_api.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_api/attachments_api.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_api/audit_trail_api.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_api/audit_trail_api.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_api/datafeed_api.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_api/datafeed_api.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_api/dlp_policies_and_dictionary_management_api.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_api/dlp_policies_and_dictionary_management_api.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_api/messages_api.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_api/messages_api.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_api/share_api.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_api/share_api.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_api/signals_api.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_api/signals_api.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_api/system_api.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_api/system_api.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_api/util_api.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_api/util_api.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_api/violations_api.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_api/violations_api.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/ack_id.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/ack_id.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/agent_info.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/agent_info.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/attachment_info.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/attachment_info.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/base_message.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/base_message.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/base_signal.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/base_signal.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/channel_subscriber.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/channel_subscriber.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/channel_subscriber_response.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/channel_subscriber_response.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/channel_subscription_error.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/channel_subscription_error.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/channel_subscription_response.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/channel_subscription_response.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/connection_request_message.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/connection_request_message.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/connection_request_message_all_of.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/connection_request_message_all_of.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/datafeed.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/datafeed.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/error.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/error.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/import_response.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/import_response.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/import_response_list.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/import_response_list.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/imported_message.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/imported_message.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/message.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/message.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/message_all_of.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/message_all_of.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/message_import_list.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/message_import_list.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/message_list.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/message_list.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/message_search_query.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/message_search_query.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/message_submission.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/message_submission.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/pagination.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/pagination.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/pagination_cursors.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/pagination_cursors.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/room_created_message.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/room_created_message.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/room_created_message_all_of.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/room_created_message_all_of.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/room_deactivated_message.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/room_deactivated_message.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/room_deactivated_message_all_of.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/room_deactivated_message_all_of.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/room_member_demoted_from_owner_message.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/room_member_demoted_from_owner_message.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/room_member_demoted_from_owner_message_all_of.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/room_member_demoted_from_owner_message_all_of.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/room_member_promoted_to_owner_message.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/room_member_promoted_to_owner_message.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/room_member_promoted_to_owner_message_all_of.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/room_member_promoted_to_owner_message_all_of.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/room_reactivated_message.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/room_reactivated_message.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/room_reactivated_message_all_of.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/room_reactivated_message_all_of.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/room_tag.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/room_tag.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/room_updated_message.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/room_updated_message.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/room_updated_message_all_of.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/room_updated_message_all_of.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/share_article.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/share_article.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/share_content.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/share_content.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/signal.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/signal.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/signal_all_of.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/signal_all_of.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/signal_list.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/signal_list.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/simple_message.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/simple_message.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/success_response.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/success_response.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/user_joined_room_message.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/user_joined_room_message.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/user_joined_room_message_all_of.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/user_joined_room_message_all_of.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/user_left_room_message.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/user_left_room_message.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/user_left_room_message_all_of.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/user_left_room_message_all_of.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_audit_trail_initiator_list.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_audit_trail_initiator_list.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_audit_trail_initiator_response.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_audit_trail_initiator_response.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_dlp_content_type.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_dlp_content_type.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_dlp_dictionary.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_dlp_dictionary.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_dlp_dictionary_content.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_dlp_dictionary_content.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_dlp_dictionary_metadata.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_dlp_dictionary_metadata.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_dlp_dictionary_metadata_collection_response.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_dlp_dictionary_metadata_collection_response.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_dlp_dictionary_metadata_create_request.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_dlp_dictionary_metadata_create_request.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_dlp_dictionary_metadata_response.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_dlp_dictionary_metadata_response.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_dlp_dictionary_metadata_update_request.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_dlp_dictionary_metadata_update_request.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_dlp_dictionary_ref.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_dlp_dictionary_ref.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_dlp_matched_policy.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_dlp_matched_policy.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_dlp_matched_policy_list.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_dlp_matched_policy_list.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_dlp_outcome.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_dlp_outcome.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_dlp_policies_collection_response.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_dlp_policies_collection_response.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_dlp_policy.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_dlp_policy.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_dlp_policy_request.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_dlp_policy_request.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_dlp_policy_response.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_dlp_policy_response.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_dlp_signal.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_dlp_signal.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_dlp_stream.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_dlp_stream.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_dlp_violation.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_dlp_violation.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_dlp_violation_message.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_dlp_violation_message.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_dlp_violation_message_response.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_dlp_violation_message_response.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_dlp_violation_signal.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_dlp_violation_signal.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_dlp_violation_signal_response.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_dlp_violation_signal_response.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_dlp_violation_stream.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_dlp_violation_stream.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_dlp_violation_stream_response.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_dlp_violation_stream_response.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v1_health_check_response.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v1_health_check_response.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v2_base_message.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v2_base_message.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v2_error.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v2_error.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v2_health_check_response.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v2_health_check_response.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v2_import_response.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v2_import_response.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v2_import_response_list.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v2_import_response_list.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v2_imported_message.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v2_imported_message.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v2_message.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v2_message.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v2_message_all_of.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v2_message_all_of.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v2_message_import_list.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v2_message_import_list.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v2_message_list.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v2_message_list.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v2_message_submission.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v2_message_submission.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v3_dlp_dictionary_meta.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v3_dlp_dictionary_meta.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v3_dlp_file_classifier_config.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v3_dlp_file_classifier_config.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v3_dlp_file_extension_config.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v3_dlp_file_extension_config.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v3_dlp_file_password_config.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v3_dlp_file_password_config.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v3_dlp_file_size_config.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v3_dlp_file_size_config.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v3_dlp_policies_collection_response.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v3_dlp_policies_collection_response.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v3_dlp_policy.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v3_dlp_policy.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v3_dlp_policy_applies_to.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v3_dlp_policy_applies_to.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v3_dlp_policy_request.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v3_dlp_policy_request.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v3_dlp_policy_response.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v3_dlp_policy_response.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v3_dlp_rule.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v3_dlp_rule.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v3_dlp_text_match_config.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v3_dlp_text_match_config.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v3_dlp_violation.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v3_dlp_violation.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v3_dlp_violation_message.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v3_dlp_violation_message.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v3_dlp_violation_message_response.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v3_dlp_violation_message_response.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v3_dlp_violation_signal.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v3_dlp_violation_signal.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v3_dlp_violation_signal_response.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v3_dlp_violation_signal_response.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v3_dlp_violation_stream.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v3_dlp_violation_stream.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v3_dlp_violation_stream_response.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v3_dlp_violation_stream_response.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v3_health.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v3_health.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v3_health_auth_type.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v3_health_auth_type.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v3_health_component.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v3_health_component.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v3_health_status.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v3_health_status.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_attachment_info.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_attachment_info.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_connection_accepted.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_connection_accepted.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_connection_requested.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_connection_requested.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_event.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_event.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_event_list.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_event_list.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_import_response.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_import_response.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_import_response_list.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_import_response_list.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_imported_message.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_imported_message.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_imported_message_attachment.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_imported_message_attachment.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_initiator.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_initiator.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_instant_message_created.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_instant_message_created.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_key_value_pair.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_key_value_pair.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_message.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_message.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_message_blast_response.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_message_blast_response.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_message_import_list.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_message_import_list.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_message_list.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_message_list.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_message_sent.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_message_sent.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_message_suppressed.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_message_suppressed.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_payload.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_payload.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_room_created.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_room_created.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_room_deactivated.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_room_deactivated.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_room_member_demoted_from_owner.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_room_member_demoted_from_owner.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_room_member_promoted_to_owner.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_room_member_promoted_to_owner.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_room_properties.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_room_properties.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_room_reactivated.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_room_reactivated.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_room_updated.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_room_updated.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_shared_post.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_shared_post.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_stream.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_stream.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_symphony_elements_action.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_symphony_elements_action.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_thumbnail_info.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_thumbnail_info.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_user.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_user.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_user_joined_room.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_user_joined_room.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_user_left_room.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_user_left_room.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v4_user_requested_to_join_room.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v4_user_requested_to_join_room.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v5_datafeed.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v5_datafeed.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v5_datafeed_create_body.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v5_datafeed_create_body.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v5_datafeed_event_type.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v5_datafeed_event_type.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v5_datafeed_type.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v5_datafeed_type.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v5_event_list.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v5_event_list.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/agent_model/v5_events_read_body.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/agent_model/v5_events_read_body.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/api_client.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/api_client.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/auth_api/authentication_api.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/auth_api/authentication_api.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/auth_api/certificate_authentication_api.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/auth_api/certificate_authentication_api.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/auth_api/certificate_pod_api.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/auth_api/certificate_pod_api.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/auth_model/error.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/auth_model/error.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/auth_model/extension_app_authenticate_request.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/auth_model/extension_app_authenticate_request.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/auth_model/extension_app_tokens.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/auth_model/extension_app_tokens.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/auth_model/obo_auth_response.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/auth_model/obo_auth_response.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/auth_model/pod_certificate.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/auth_model/pod_certificate.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/auth_model/success_response.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/auth_model/success_response.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/auth_model/token.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/auth_model/token.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/configuration.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/configuration.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/exceptions.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/exceptions.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/group_api/group_api.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_api/group_api.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/group_api/type_api.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_api/type_api.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/add_member.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/add_member.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/avatar.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/avatar.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/base_group.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/base_group.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/base_profile.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/base_profile.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/base_type.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/base_type.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/create_group.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/create_group.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/create_group_all_of.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/create_group_all_of.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/error.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/error.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/group_implicit_connection.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/group_implicit_connection.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/group_interaction_transfer.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/group_interaction_transfer.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/group_list.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/group_list.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/group_visibility_restriction.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/group_visibility_restriction.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/implicit_connection.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/implicit_connection.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/interaction_control.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/interaction_control.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/interaction_transfer.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/interaction_transfer.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/member.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/member.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/membership_control.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/membership_control.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/owner.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/owner.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/pagination.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/pagination.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/pagination_cursors.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/pagination_cursors.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/profile.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/profile.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/profile_all_of.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/profile_all_of.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/profile_control.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/profile_control.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/read_group.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/read_group.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/read_group_all_of.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/read_group_all_of.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/read_member.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/read_member.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/read_member_all_of.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/read_member_all_of.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/sort_order.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/sort_order.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/status.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/status.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/transfer_view.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/transfer_view.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/type.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/type.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/type_all_of.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/type_all_of.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/type_list.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/type_list.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/update_group.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/update_group.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/update_group_all_of.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/update_group_all_of.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/upload_avatar.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/upload_avatar.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/group_model/visibility_restriction.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/group_model/visibility_restriction.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/login_api/authentication_api.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/login_api/authentication_api.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/login_model/authenticate_extension_app_request.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/login_model/authenticate_extension_app_request.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/login_model/authenticate_request.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/login_model/authenticate_request.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/login_model/error.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/login_model/error.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/login_model/extension_app_tokens.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/login_model/extension_app_tokens.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/login_model/jwks.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/login_model/jwks.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/login_model/jwks_entry.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/login_model/jwks_entry.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/login_model/jwt_token.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/login_model/jwt_token.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/login_model/token.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/login_model/token.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/model_utils.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/model_utils.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_api/app_entitlement_api.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_api/app_entitlement_api.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_api/application_api.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_api/application_api.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_api/connection_api.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_api/connection_api.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_api/default_api.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_api/default_api.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_api/disclaimer_api.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_api/disclaimer_api.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_api/info_barriers_api.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_api/info_barriers_api.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_api/message_api.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_api/message_api.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_api/message_suppression_api.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_api/message_suppression_api.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_api/pod_api.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_api/pod_api.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_api/presence_api.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_api/presence_api.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_api/room_membership_api.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_api/room_membership_api.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_api/security_api.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_api/security_api.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_api/session_api.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_api/session_api.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_api/streams_api.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_api/streams_api.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_api/system_api.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_api/system_api.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_api/user_api.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_api/user_api.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_api/users_api.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_api/users_api.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/admin_justified_action.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/admin_justified_action.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/admin_justified_user_action.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/admin_justified_user_action.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/admin_stream_attributes.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/admin_stream_attributes.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/admin_stream_filter.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/admin_stream_filter.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/admin_stream_info.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/admin_stream_info.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/admin_stream_info_list.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/admin_stream_info_list.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/admin_stream_list.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/admin_stream_list.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/admin_stream_type_enum.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/admin_stream_type_enum.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/app_authentication_key.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/app_authentication_key.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/app_authentication_keys.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/app_authentication_keys.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/app_notification.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/app_notification.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/app_properties.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/app_properties.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/app_property.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/app_property.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/application_detail.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/application_detail.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/application_info.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/application_info.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/assignee_candidate.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/assignee_candidate.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/assignee_candidates.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/assignee_candidates.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/attachment_preview.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/attachment_preview.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/avatar.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/avatar.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/avatar_list.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/avatar_list.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/avatar_update.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/avatar_update.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/bulk_action_result.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/bulk_action_result.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/cert_info.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/cert_info.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/cert_info_item.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/cert_info_item.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/company_cert.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/company_cert.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/company_cert_attributes.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/company_cert_attributes.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/company_cert_detail.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/company_cert_detail.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/company_cert_info.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/company_cert_info.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/company_cert_info_list.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/company_cert_info_list.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/company_cert_status.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/company_cert_status.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/company_cert_type.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/company_cert_type.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/company_cert_type_list.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/company_cert_type_list.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/conversation_specific_stream_attributes.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/conversation_specific_stream_attributes.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/delegate_action.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/delegate_action.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/disclaimer.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/disclaimer.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/disclaimer_list.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/disclaimer_list.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/download_receipt_count.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/download_receipt_count.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/error.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/error.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/faceted_match_count.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/faceted_match_count.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/feature.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/feature.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/feature_list.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/feature_list.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/file_extension.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/file_extension.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/file_extensions_response.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/file_extensions_response.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/followers_list.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/followers_list.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/followers_list_response.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/followers_list_response.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/following_list_response.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/following_list_response.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/group.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/group.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/group_item.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/group_item.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/group_list.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/group_list.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/group_role_scope.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/group_role_scope.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/im_system_info.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/im_system_info.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/immutable_room_attributes.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/immutable_room_attributes.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/integer_list.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/integer_list.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/languages.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/languages.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/member_info.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/member_info.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/membership_data.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/membership_data.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/membership_list.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/membership_list.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/message_detail.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/message_detail.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/message_details.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/message_details.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/message_download_receipt_count.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/message_download_receipt_count.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/message_ids.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/message_ids.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/message_ids_from_stream.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/message_ids_from_stream.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/message_metadata_response.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/message_metadata_response.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/message_metadata_response_parent.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/message_metadata_response_parent.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/message_receipt_detail.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/message_receipt_detail.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/message_receipt_detail_response.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/message_receipt_detail_response.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/message_status.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/message_status.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/message_status_user.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/message_status_user.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/message_stream.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/message_stream.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/message_suppression_response.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/message_suppression_response.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/message_user.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/message_user.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/name_value_pair.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/name_value_pair.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/pagination.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/pagination.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/pagination_cursors.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/pagination_cursors.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/password.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/password.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/password_reset.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/password_reset.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/pod_app_entitlement.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/pod_app_entitlement.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/pod_app_entitlement_list.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/pod_app_entitlement_list.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/pod_certificate.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/pod_certificate.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/policy.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/policy.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/policy_list.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/policy_list.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/presence.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/presence.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/product.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/product.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/product_list.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/product_list.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/protocol.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/protocol.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/role.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/role.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/role_detail.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/role_detail.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/role_detail_list.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/role_detail_list.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/role_list.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/role_list.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/room_attributes.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/room_attributes.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/room_create.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/room_create.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/room_detail.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/room_detail.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/room_search_criteria.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/room_search_criteria.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/room_search_results.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/room_search_results.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/room_specific_stream_attributes.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/room_specific_stream_attributes.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/room_system_info.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/room_system_info.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/room_tag.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/room_tag.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/session_info.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/session_info.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/stream.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/stream.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/stream_attachment_item.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/stream_attachment_item.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/stream_attachment_response.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/stream_attachment_response.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/stream_attributes.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/stream_attributes.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/stream_filter.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/stream_filter.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/stream_list.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/stream_list.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/stream_type.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/stream_type.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/string_id.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/string_id.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/string_list.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/string_list.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/success_response.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/success_response.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_app_entitlement.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_app_entitlement.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_app_entitlement_list.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_app_entitlement_list.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_app_entitlement_patch.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_app_entitlement_patch.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_app_entitlement_patch_enum.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_app_entitlement_patch_enum.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_app_entitlements_patch_list.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_app_entitlements_patch_list.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_attributes.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_attributes.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_compp.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_compp.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_connection.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_connection.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_connection_list.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_connection_list.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_connection_request.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_connection_request.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_create.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_create.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_data.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_data.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_detail.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_detail.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_detail_list.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_detail_list.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_error.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_error.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_filter.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_filter.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_group_assignee.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_group_assignee.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_group_assignee_response.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_group_assignee_response.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_group_assignee_update.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_group_assignee_update.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_group_assignment_response.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_group_assignment_response.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_group_create.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_group_create.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_group_data.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_group_data.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_group_membership_data.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_group_membership_data.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_group_membership_request.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_group_membership_request.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_group_membership_response.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_group_membership_response.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_group_membership_response_data.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_group_membership_response_data.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_group_membership_update.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_group_membership_update.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_group_response.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_group_response.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_group_response_list.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_group_response_list.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_group_update.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_group_update.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_id.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_id.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_id_list.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_id_list.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_info.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_info.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_name.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_name.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_name_list.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_name_list.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_search_filter.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_search_filter.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_search_query.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_search_query.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_search_results.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_search_results.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_status.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_status.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_suspension.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_suspension.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_system_info.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_system_info.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/user_v2.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/user_v2.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v1_im_attributes.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v1_im_attributes.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v1_im_detail.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v1_im_detail.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_admin_stream_attributes.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_admin_stream_attributes.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_admin_stream_filter.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_admin_stream_filter.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_admin_stream_info.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_admin_stream_info.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_admin_stream_info_list.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_admin_stream_info_list.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_admin_stream_list.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_admin_stream_list.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_admin_stream_type.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_admin_stream_type.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_conversation_specific_stream_attributes.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_conversation_specific_stream_attributes.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_member_info.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_member_info.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_member_info_list.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_member_info_list.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_member_user_detail.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_member_user_detail.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_membership_list.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_membership_list.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_presence.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_presence.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_presence_all_of.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_presence_all_of.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_presence_list.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_presence_list.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_presence_status.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_presence_status.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_room_attributes.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_room_attributes.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_room_detail.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_room_detail.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_room_search_criteria.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_room_search_criteria.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_room_search_criteria_all_of.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_room_search_criteria_all_of.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_room_specific_stream_attributes.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_room_specific_stream_attributes.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_stream_attributes.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_stream_attributes.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_stream_type.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_stream_type.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_user_attributes.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_user_attributes.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_user_create.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_user_create.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_user_detail.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_user_detail.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_user_detail_list.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_user_detail_list.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_user_key_request.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_user_key_request.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_user_list.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_user_list.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_user_presence.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_user_presence.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v2_user_presence_all_of.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v2_user_presence_all_of.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v3_room_attributes.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v3_room_attributes.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v3_room_detail.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v3_room_detail.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/pod_model/v3_room_search_results.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/pod_model/v3_room_search_results.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/symphony/bdk/gen/rest.py` & `symphony_bdk_python-2.6.dev0/symphony/bdk/gen/rest.py`

 * *Files identical despite different names*

### Comparing `symphony_bdk_python-2.6.1/PKG-INFO` & `symphony_bdk_python-2.6.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: symphony-bdk-python
-Version: 2.6.1
+Version: 2.6.dev0
 Summary: Symphony Bot Development Kit for Python
 Home-page: https://github.com/finos/symphony-bdk-python
 License: Apache-2.0
 Author: Symphony Platform Solutions
 Author-email: symphony@finos.org
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyJWT (>=2.3.0,<3.0.0)
 Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
-Requires-Dist: cryptography (>=40.0.2,<41.0.0)
+Requires-Dist: cryptography (>=38.0.3,<39.0.0)
 Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
 Requires-Dist: docutils (==0.16)
 Requires-Dist: nulltype (>=2.3.1,<3.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: tenacity (>=8.0.1,<9.0.0)
 Requires-Dist: urllib3 (>=1.26.9,<2.0.0)
```

