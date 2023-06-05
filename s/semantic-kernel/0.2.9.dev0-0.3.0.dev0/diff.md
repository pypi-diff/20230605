# Comparing `tmp/semantic_kernel-0.2.9.dev0.tar.gz` & `tmp/semantic_kernel-0.3.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantic_kernel-0.2.9.dev0.tar", max compression
+gzip compressed data, was "semantic_kernel-0.3.0.dev0.tar", max compression
```

## Comparing `semantic_kernel-0.2.9.dev0.tar` & `semantic_kernel-0.3.0.dev0.tar`

### file list

```diff
@@ -1,91 +1,92 @@
--rw-r--r--   0        0        0     1186 2023-05-08 23:38:10.955726 semantic_kernel-0.2.9.dev0/pip/README.md
--rw-r--r--   0        0        0      835 2023-05-30 18:59:46.699650 semantic_kernel-0.2.9.dev0/pyproject.toml
--rw-r--r--   0        0        0     1227 2023-05-08 23:38:10.959435 semantic_kernel-0.2.9.dev0/semantic_kernel/__init__.py
--rw-r--r--   0        0        0      719 2023-05-25 17:48:21.153018 semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/__init__.py
--rw-r--r--   0        0        0     1647 2023-04-30 18:57:02.983569 semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/ai_exception.py
--rw-r--r--   0        0        0      709 2023-05-25 17:48:21.153502 semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/chat_completion_client_base.py
--rw-r--r--   0        0        0     1129 2023-04-30 18:57:02.985239 semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/chat_request_settings.py
--rw-r--r--   0        0        0     1332 2023-04-30 18:57:02.985587 semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/complete_request_settings.py
--rw-r--r--   0        0        0      282 2023-04-30 18:57:02.986074 semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/embeddings/embedding_generator_base.py
--rw-r--r--   0        0        0      352 2023-04-30 18:57:02.986678 semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/hugging_face/__init__.py
--rw-r--r--   0        0        0     4980 2023-05-25 17:48:21.154076 semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py
--rw-r--r--   0        0        0     2317 2023-05-08 23:38:10.960592 semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py
--rw-r--r--   0        0        0      892 2023-04-30 18:57:02.988571 semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/open_ai/__init__.py
--rw-r--r--   0        0        0     2615 2023-05-15 18:12:57.030156 semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py
--rw-r--r--   0        0        0     2607 2023-05-15 18:12:57.032300 semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py
--rw-r--r--   0        0        0     2602 2023-05-15 18:12:57.034473 semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py
--rw-r--r--   0        0        0     7130 2023-05-25 17:48:21.154688 semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py
--rw-r--r--   0        0        0     5296 2023-05-25 17:48:21.155487 semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py
--rw-r--r--   0        0        0     2723 2023-05-15 18:12:57.041646 semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py
--rw-r--r--   0        0        0      679 2023-05-25 17:48:21.156192 semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/text_completion_client_base.py
--rw-r--r--   0        0        0      182 2023-05-18 17:32:52.334054 semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/memory/chroma/__init__.py
--rw-r--r--   0        0        0    14953 2023-05-18 17:32:52.334557 semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py
--rw-r--r--   0        0        0     3568 2023-05-18 17:32:52.335005 semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/memory/chroma/utils.py
--rw-r--r--   0        0        0      691 2023-05-19 18:06:11.089827 semantic_kernel-0.2.9.dev0/semantic_kernel/core_skills/__init__.py
--rw-r--r--   0        0        0     2510 2023-05-15 18:12:57.044314 semantic_kernel-0.2.9.dev0/semantic_kernel/core_skills/conversation_summary_skill.py
--rw-r--r--   0        0        0     2072 2023-04-13 23:12:46.166679 semantic_kernel-0.2.9.dev0/semantic_kernel/core_skills/file_io_skill.py
--rw-r--r--   0        0        0     3754 2023-04-22 04:06:40.780276 semantic_kernel-0.2.9.dev0/semantic_kernel/core_skills/http_skill.py
--rw-r--r--   0        0        0     3164 2023-05-15 18:12:57.045974 semantic_kernel-0.2.9.dev0/semantic_kernel/core_skills/math_skill.py
--rw-r--r--   0        0        0     4641 2023-04-14 00:51:57.194344 semantic_kernel-0.2.9.dev0/semantic_kernel/core_skills/text_memory_skill.py
--rw-r--r--   0        0        0     2403 2023-04-13 23:12:46.167467 semantic_kernel-0.2.9.dev0/semantic_kernel/core_skills/text_skill.py
--rw-r--r--   0        0        0     7504 2023-05-25 23:34:34.714729 semantic_kernel-0.2.9.dev0/semantic_kernel/core_skills/time_skill.py
--rw-r--r--   0        0        0    27735 2023-05-19 23:02:13.063161 semantic_kernel-0.2.9.dev0/semantic_kernel/kernel.py
--rw-r--r--   0        0        0     1626 2023-04-30 18:57:02.993735 semantic_kernel-0.2.9.dev0/semantic_kernel/kernel_exception.py
--rw-r--r--   0        0        0      160 2023-04-13 23:12:46.173418 semantic_kernel-0.2.9.dev0/semantic_kernel/memory/__init__.py
--rw-r--r--   0        0        0     2345 2023-04-30 18:57:02.996159 semantic_kernel-0.2.9.dev0/semantic_kernel/memory/memory_query_result.py
--rw-r--r--   0        0        0     3090 2023-05-08 23:38:10.963328 semantic_kernel-0.2.9.dev0/semantic_kernel/memory/memory_record.py
--rw-r--r--   0        0        0     2014 2023-05-19 23:02:13.063945 semantic_kernel-0.2.9.dev0/semantic_kernel/memory/memory_store_base.py
--rw-r--r--   0        0        0     1137 2023-04-13 23:12:46.175270 semantic_kernel-0.2.9.dev0/semantic_kernel/memory/null_memory.py
--rw-r--r--   0        0        0     6045 2023-05-08 23:26:22.334494 semantic_kernel-0.2.9.dev0/semantic_kernel/memory/semantic_text_memory.py
--rw-r--r--   0        0        0     1196 2023-04-30 18:57:02.998063 semantic_kernel-0.2.9.dev0/semantic_kernel/memory/semantic_text_memory_base.py
--rw-r--r--   0        0        0    12032 2023-05-15 18:12:57.047968 semantic_kernel-0.2.9.dev0/semantic_kernel/memory/volatile_memory_store.py
--rw-r--r--   0        0        0     2361 2023-04-22 04:06:40.782347 semantic_kernel-0.2.9.dev0/semantic_kernel/orchestration/context_variables.py
--rw-r--r--   0        0        0     5079 2023-04-14 00:51:57.199808 semantic_kernel-0.2.9.dev0/semantic_kernel/orchestration/delegate_handlers.py
--rw-r--r--   0        0        0     9005 2023-05-19 23:02:13.064609 semantic_kernel-0.2.9.dev0/semantic_kernel/orchestration/delegate_inference.py
--rw-r--r--   0        0        0      638 2023-04-13 23:12:46.179530 semantic_kernel-0.2.9.dev0/semantic_kernel/orchestration/delegate_types.py
--rw-r--r--   0        0        0     7514 2023-04-14 00:52:05.160748 semantic_kernel-0.2.9.dev0/semantic_kernel/orchestration/sk_context.py
--rw-r--r--   0        0        0    15915 2023-05-08 23:26:29.698891 semantic_kernel-0.2.9.dev0/semantic_kernel/orchestration/sk_function.py
--rw-r--r--   0        0        0     6158 2023-04-30 18:57:02.999492 semantic_kernel-0.2.9.dev0/semantic_kernel/orchestration/sk_function_base.py
--rw-r--r--   0        0        0      158 2023-05-08 23:38:10.963774 semantic_kernel-0.2.9.dev0/semantic_kernel/planning/__init__.py
--rw-r--r--   0        0        0     7287 2023-05-25 17:48:21.156811 semantic_kernel-0.2.9.dev0/semantic_kernel/planning/basic_planner.py
--rw-r--r--   0        0        0      396 2023-05-08 23:26:29.700122 semantic_kernel-0.2.9.dev0/semantic_kernel/planning/plan.py
--rw-r--r--   0        0        0      932 2023-05-19 23:02:13.065230 semantic_kernel-0.2.9.dev0/semantic_kernel/reliability/pass_through_without_retry.py
--rw-r--r--   0        0        0      694 2023-05-19 23:02:13.065627 semantic_kernel-0.2.9.dev0/semantic_kernel/reliability/retry_mechanism_base.py
--rw-r--r--   0        0        0     2101 2023-04-13 23:12:46.182583 semantic_kernel-0.2.9.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py
--rw-r--r--   0        0        0     2332 2023-04-14 00:51:57.203325 semantic_kernel-0.2.9.dev0/semantic_kernel/semantic_functions/prompt_template.py
--rw-r--r--   0        0        0      506 2023-04-13 23:12:46.183441 semantic_kernel-0.2.9.dev0/semantic_kernel/semantic_functions/prompt_template_base.py
--rw-r--r--   0        0        0     4269 2023-04-30 18:57:02.999997 semantic_kernel-0.2.9.dev0/semantic_kernel/semantic_functions/prompt_template_config.py
--rw-r--r--   0        0        0      671 2023-04-14 00:51:57.204455 semantic_kernel-0.2.9.dev0/semantic_kernel/semantic_functions/semantic_function_config.py
--rw-r--r--   0        0        0      322 2023-04-14 00:51:57.205241 semantic_kernel-0.2.9.dev0/semantic_kernel/skill_definition/__init__.py
--rw-r--r--   0        0        0     2053 2023-04-14 00:51:57.205757 semantic_kernel-0.2.9.dev0/semantic_kernel/skill_definition/function_view.py
--rw-r--r--   0        0        0     1717 2023-04-13 23:12:46.186028 semantic_kernel-0.2.9.dev0/semantic_kernel/skill_definition/functions_view.py
--rw-r--r--   0        0        0     1026 2023-04-14 00:51:57.206300 semantic_kernel-0.2.9.dev0/semantic_kernel/skill_definition/parameter_view.py
--rw-r--r--   0        0        0     2104 2023-04-14 00:51:57.206885 semantic_kernel-0.2.9.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py
--rw-r--r--   0        0        0     1345 2023-04-14 00:51:57.207475 semantic_kernel-0.2.9.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py
--rw-r--r--   0        0        0      858 2023-04-13 23:12:46.187552 semantic_kernel-0.2.9.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py
--rw-r--r--   0        0        0      837 2023-04-14 00:51:57.208334 semantic_kernel-0.2.9.dev0/semantic_kernel/skill_definition/sk_function_decorator.py
--rw-r--r--   0        0        0     6056 2023-04-14 00:51:57.208951 semantic_kernel-0.2.9.dev0/semantic_kernel/skill_definition/skill_collection.py
--rw-r--r--   0        0        0      803 2023-04-13 23:12:46.188719 semantic_kernel-0.2.9.dev0/semantic_kernel/skill_definition/skill_collection_base.py
--rw-r--r--   0        0        0     1115 2023-04-13 23:12:46.189034 semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/README.md
--rw-r--r--   0        0        0      830 2023-04-14 00:51:57.209567 semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/blocks/block.py
--rw-r--r--   0        0        0      228 2023-04-14 00:51:57.210164 semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/blocks/block_types.py
--rw-r--r--   0        0        0     4577 2023-04-30 18:57:03.000489 semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/blocks/code_block.py
--rw-r--r--   0        0        0     2653 2023-04-13 23:12:46.192355 semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/blocks/function_id_block.py
--rw-r--r--   0        0        0      276 2023-04-13 23:12:46.192840 semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/blocks/symbols.py
--rw-r--r--   0        0        0     1534 2023-04-14 00:51:57.211524 semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/blocks/text_block.py
--rw-r--r--   0        0        0     2274 2023-04-13 23:12:46.193631 semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/blocks/val_block.py
--rw-r--r--   0        0        0     2517 2023-04-14 00:51:57.212261 semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/blocks/var_block.py
--rw-r--r--   0        0        0     6535 2023-04-13 23:12:46.194683 semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/code_tokenizer.py
--rw-r--r--   0        0        0     6051 2023-04-14 00:51:57.212967 semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/prompt_template_engine.py
--rw-r--r--   0        0        0      532 2023-04-13 23:12:46.195769 semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/protocols/code_renderer.py
--rw-r--r--   0        0        0     3043 2023-04-13 23:12:46.196165 semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py
--rw-r--r--   0        0        0      596 2023-04-13 23:12:46.196572 semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/protocols/text_renderer.py
--rw-r--r--   0        0        0     7637 2023-04-13 23:12:46.196999 semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/template_tokenizer.py
--rw-r--r--   0        0        0      473 2023-04-30 18:57:03.001133 semantic_kernel-0.2.9.dev0/semantic_kernel/text/__init__.py
--rw-r--r--   0        0        0      667 2023-04-30 18:57:03.001562 semantic_kernel-0.2.9.dev0/semantic_kernel/text/function_extension.py
--rw-r--r--   0        0        0     6467 2023-05-15 18:12:57.049895 semantic_kernel-0.2.9.dev0/semantic_kernel/text/text_chunker.py
--rw-r--r--   0        0        0      403 2023-04-13 23:12:46.197533 semantic_kernel-0.2.9.dev0/semantic_kernel/utils/null_logger.py
--rw-r--r--   0        0        0     2436 2023-04-14 00:51:57.213683 semantic_kernel-0.2.9.dev0/semantic_kernel/utils/settings.py
--rw-r--r--   0        0        0      221 2023-04-13 23:12:46.198404 semantic_kernel-0.2.9.dev0/semantic_kernel/utils/static_property.py
--rw-r--r--   0        0        0     2198 2023-04-13 23:12:46.198764 semantic_kernel-0.2.9.dev0/semantic_kernel/utils/validation.py
--rw-r--r--   0        0        0     1760 1970-01-01 00:00:00.000000 semantic_kernel-0.2.9.dev0/PKG-INFO
+-rw-r--r--   0        0        0     1186 2023-05-08 23:38:10.955726 semantic_kernel-0.3.0.dev0/pip/README.md
+-rw-r--r--   0        0        0      907 2023-06-05 21:39:22.282927 semantic_kernel-0.3.0.dev0/pyproject.toml
+-rw-r--r--   0        0        0     1227 2023-05-08 23:38:10.959435 semantic_kernel-0.3.0.dev0/semantic_kernel/__init__.py
+-rw-r--r--   0        0        0      719 2023-05-25 17:48:21.153018 semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/__init__.py
+-rw-r--r--   0        0        0     1647 2023-04-30 18:57:02.983569 semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/ai_exception.py
+-rw-r--r--   0        0        0      709 2023-05-25 17:48:21.153502 semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/chat_completion_client_base.py
+-rw-r--r--   0        0        0     1129 2023-04-30 18:57:02.985239 semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/chat_request_settings.py
+-rw-r--r--   0        0        0     1332 2023-04-30 18:57:02.985587 semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/complete_request_settings.py
+-rw-r--r--   0        0        0      282 2023-04-30 18:57:02.986074 semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/embeddings/embedding_generator_base.py
+-rw-r--r--   0        0        0      352 2023-04-30 18:57:02.986678 semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/hugging_face/__init__.py
+-rw-r--r--   0        0        0     4980 2023-05-25 17:48:21.154076 semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py
+-rw-r--r--   0        0        0     2317 2023-05-08 23:38:10.960592 semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py
+-rw-r--r--   0        0        0      892 2023-04-30 18:57:02.988571 semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/open_ai/__init__.py
+-rw-r--r--   0        0        0     2615 2023-05-15 18:12:57.030156 semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py
+-rw-r--r--   0        0        0     2607 2023-05-15 18:12:57.032300 semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py
+-rw-r--r--   0        0        0     2602 2023-05-15 18:12:57.034473 semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py
+-rw-r--r--   0        0        0     7130 2023-05-25 17:48:21.154688 semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py
+-rw-r--r--   0        0        0     5296 2023-05-25 17:48:21.155487 semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py
+-rw-r--r--   0        0        0     2723 2023-05-15 18:12:57.041646 semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py
+-rw-r--r--   0        0        0      679 2023-05-25 17:48:21.156192 semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/text_completion_client_base.py
+-rw-r--r--   0        0        0      182 2023-05-18 17:32:52.334054 semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/memory/chroma/__init__.py
+-rw-r--r--   0        0        0    15118 2023-06-05 21:39:19.137459 semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py
+-rw-r--r--   0        0        0     3568 2023-05-18 17:32:52.335005 semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/memory/chroma/utils.py
+-rw-r--r--   0        0        0    10783 2023-06-05 21:39:19.137785 semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/memory/weaviate_memory_store.py
+-rw-r--r--   0        0        0      691 2023-05-19 18:06:11.089827 semantic_kernel-0.3.0.dev0/semantic_kernel/core_skills/__init__.py
+-rw-r--r--   0        0        0     2510 2023-05-15 18:12:57.044314 semantic_kernel-0.3.0.dev0/semantic_kernel/core_skills/conversation_summary_skill.py
+-rw-r--r--   0        0        0     2072 2023-04-13 23:12:46.166679 semantic_kernel-0.3.0.dev0/semantic_kernel/core_skills/file_io_skill.py
+-rw-r--r--   0        0        0     3754 2023-04-22 04:06:40.780276 semantic_kernel-0.3.0.dev0/semantic_kernel/core_skills/http_skill.py
+-rw-r--r--   0        0        0     3164 2023-05-15 18:12:57.045974 semantic_kernel-0.3.0.dev0/semantic_kernel/core_skills/math_skill.py
+-rw-r--r--   0        0        0     4641 2023-04-14 00:51:57.194344 semantic_kernel-0.3.0.dev0/semantic_kernel/core_skills/text_memory_skill.py
+-rw-r--r--   0        0        0     2403 2023-04-13 23:12:46.167467 semantic_kernel-0.3.0.dev0/semantic_kernel/core_skills/text_skill.py
+-rw-r--r--   0        0        0     7504 2023-05-25 23:34:34.714729 semantic_kernel-0.3.0.dev0/semantic_kernel/core_skills/time_skill.py
+-rw-r--r--   0        0        0    27735 2023-05-19 23:02:13.063161 semantic_kernel-0.3.0.dev0/semantic_kernel/kernel.py
+-rw-r--r--   0        0        0     1626 2023-04-30 18:57:02.993735 semantic_kernel-0.3.0.dev0/semantic_kernel/kernel_exception.py
+-rw-r--r--   0        0        0      160 2023-04-13 23:12:46.173418 semantic_kernel-0.3.0.dev0/semantic_kernel/memory/__init__.py
+-rw-r--r--   0        0        0     2345 2023-04-30 18:57:02.996159 semantic_kernel-0.3.0.dev0/semantic_kernel/memory/memory_query_result.py
+-rw-r--r--   0        0        0     3090 2023-05-08 23:38:10.963328 semantic_kernel-0.3.0.dev0/semantic_kernel/memory/memory_record.py
+-rw-r--r--   0        0        0     2014 2023-05-19 23:02:13.063945 semantic_kernel-0.3.0.dev0/semantic_kernel/memory/memory_store_base.py
+-rw-r--r--   0        0        0     1137 2023-04-13 23:12:46.175270 semantic_kernel-0.3.0.dev0/semantic_kernel/memory/null_memory.py
+-rw-r--r--   0        0        0     6050 2023-06-05 17:09:41.373093 semantic_kernel-0.3.0.dev0/semantic_kernel/memory/semantic_text_memory.py
+-rw-r--r--   0        0        0     1196 2023-04-30 18:57:02.998063 semantic_kernel-0.3.0.dev0/semantic_kernel/memory/semantic_text_memory_base.py
+-rw-r--r--   0        0        0    12032 2023-05-15 18:12:57.047968 semantic_kernel-0.3.0.dev0/semantic_kernel/memory/volatile_memory_store.py
+-rw-r--r--   0        0        0     2361 2023-04-22 04:06:40.782347 semantic_kernel-0.3.0.dev0/semantic_kernel/orchestration/context_variables.py
+-rw-r--r--   0        0        0     5079 2023-04-14 00:51:57.199808 semantic_kernel-0.3.0.dev0/semantic_kernel/orchestration/delegate_handlers.py
+-rw-r--r--   0        0        0     9005 2023-05-19 23:02:13.064609 semantic_kernel-0.3.0.dev0/semantic_kernel/orchestration/delegate_inference.py
+-rw-r--r--   0        0        0      638 2023-04-13 23:12:46.179530 semantic_kernel-0.3.0.dev0/semantic_kernel/orchestration/delegate_types.py
+-rw-r--r--   0        0        0     7514 2023-04-14 00:52:05.160748 semantic_kernel-0.3.0.dev0/semantic_kernel/orchestration/sk_context.py
+-rw-r--r--   0        0        0    15915 2023-05-08 23:26:29.698891 semantic_kernel-0.3.0.dev0/semantic_kernel/orchestration/sk_function.py
+-rw-r--r--   0        0        0     6158 2023-04-30 18:57:02.999492 semantic_kernel-0.3.0.dev0/semantic_kernel/orchestration/sk_function_base.py
+-rw-r--r--   0        0        0      158 2023-05-08 23:38:10.963774 semantic_kernel-0.3.0.dev0/semantic_kernel/planning/__init__.py
+-rw-r--r--   0        0        0     7287 2023-05-25 17:48:21.156811 semantic_kernel-0.3.0.dev0/semantic_kernel/planning/basic_planner.py
+-rw-r--r--   0        0        0      396 2023-05-08 23:26:29.700122 semantic_kernel-0.3.0.dev0/semantic_kernel/planning/plan.py
+-rw-r--r--   0        0        0      932 2023-05-19 23:02:13.065230 semantic_kernel-0.3.0.dev0/semantic_kernel/reliability/pass_through_without_retry.py
+-rw-r--r--   0        0        0      694 2023-06-05 21:39:19.138269 semantic_kernel-0.3.0.dev0/semantic_kernel/reliability/retry_mechanism_base.py
+-rw-r--r--   0        0        0     2101 2023-04-13 23:12:46.182583 semantic_kernel-0.3.0.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py
+-rw-r--r--   0        0        0     2332 2023-04-14 00:51:57.203325 semantic_kernel-0.3.0.dev0/semantic_kernel/semantic_functions/prompt_template.py
+-rw-r--r--   0        0        0      506 2023-04-13 23:12:46.183441 semantic_kernel-0.3.0.dev0/semantic_kernel/semantic_functions/prompt_template_base.py
+-rw-r--r--   0        0        0     4269 2023-04-30 18:57:02.999997 semantic_kernel-0.3.0.dev0/semantic_kernel/semantic_functions/prompt_template_config.py
+-rw-r--r--   0        0        0      671 2023-04-14 00:51:57.204455 semantic_kernel-0.3.0.dev0/semantic_kernel/semantic_functions/semantic_function_config.py
+-rw-r--r--   0        0        0      322 2023-04-14 00:51:57.205241 semantic_kernel-0.3.0.dev0/semantic_kernel/skill_definition/__init__.py
+-rw-r--r--   0        0        0     2053 2023-04-14 00:51:57.205757 semantic_kernel-0.3.0.dev0/semantic_kernel/skill_definition/function_view.py
+-rw-r--r--   0        0        0     1717 2023-04-13 23:12:46.186028 semantic_kernel-0.3.0.dev0/semantic_kernel/skill_definition/functions_view.py
+-rw-r--r--   0        0        0     1026 2023-04-14 00:51:57.206300 semantic_kernel-0.3.0.dev0/semantic_kernel/skill_definition/parameter_view.py
+-rw-r--r--   0        0        0     2104 2023-04-14 00:51:57.206885 semantic_kernel-0.3.0.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py
+-rw-r--r--   0        0        0     1345 2023-04-14 00:51:57.207475 semantic_kernel-0.3.0.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py
+-rw-r--r--   0        0        0      858 2023-04-13 23:12:46.187552 semantic_kernel-0.3.0.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py
+-rw-r--r--   0        0        0      837 2023-04-14 00:51:57.208334 semantic_kernel-0.3.0.dev0/semantic_kernel/skill_definition/sk_function_decorator.py
+-rw-r--r--   0        0        0     6056 2023-04-14 00:51:57.208951 semantic_kernel-0.3.0.dev0/semantic_kernel/skill_definition/skill_collection.py
+-rw-r--r--   0        0        0      803 2023-04-13 23:12:46.188719 semantic_kernel-0.3.0.dev0/semantic_kernel/skill_definition/skill_collection_base.py
+-rw-r--r--   0        0        0     1115 2023-04-13 23:12:46.189034 semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/README.md
+-rw-r--r--   0        0        0      830 2023-04-14 00:51:57.209567 semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/blocks/block.py
+-rw-r--r--   0        0        0      228 2023-04-14 00:51:57.210164 semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/blocks/block_types.py
+-rw-r--r--   0        0        0     4577 2023-04-30 18:57:03.000489 semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/blocks/code_block.py
+-rw-r--r--   0        0        0     2653 2023-04-13 23:12:46.192355 semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/blocks/function_id_block.py
+-rw-r--r--   0        0        0      276 2023-04-13 23:12:46.192840 semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/blocks/symbols.py
+-rw-r--r--   0        0        0     1534 2023-04-14 00:51:57.211524 semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/blocks/text_block.py
+-rw-r--r--   0        0        0     2274 2023-04-13 23:12:46.193631 semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/blocks/val_block.py
+-rw-r--r--   0        0        0     2517 2023-04-14 00:51:57.212261 semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/blocks/var_block.py
+-rw-r--r--   0        0        0     6535 2023-04-13 23:12:46.194683 semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/code_tokenizer.py
+-rw-r--r--   0        0        0     6051 2023-04-14 00:51:57.212967 semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/prompt_template_engine.py
+-rw-r--r--   0        0        0      532 2023-04-13 23:12:46.195769 semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/protocols/code_renderer.py
+-rw-r--r--   0        0        0     3043 2023-04-13 23:12:46.196165 semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py
+-rw-r--r--   0        0        0      596 2023-04-13 23:12:46.196572 semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/protocols/text_renderer.py
+-rw-r--r--   0        0        0     7637 2023-04-13 23:12:46.196999 semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/template_tokenizer.py
+-rw-r--r--   0        0        0      473 2023-04-30 18:57:03.001133 semantic_kernel-0.3.0.dev0/semantic_kernel/text/__init__.py
+-rw-r--r--   0        0        0      667 2023-04-30 18:57:03.001562 semantic_kernel-0.3.0.dev0/semantic_kernel/text/function_extension.py
+-rw-r--r--   0        0        0     6467 2023-05-15 18:12:57.049895 semantic_kernel-0.3.0.dev0/semantic_kernel/text/text_chunker.py
+-rw-r--r--   0        0        0      403 2023-04-13 23:12:46.197533 semantic_kernel-0.3.0.dev0/semantic_kernel/utils/null_logger.py
+-rw-r--r--   0        0        0     2436 2023-04-14 00:51:57.213683 semantic_kernel-0.3.0.dev0/semantic_kernel/utils/settings.py
+-rw-r--r--   0        0        0      221 2023-04-13 23:12:46.198404 semantic_kernel-0.3.0.dev0/semantic_kernel/utils/static_property.py
+-rw-r--r--   0        0        0     2198 2023-04-13 23:12:46.198764 semantic_kernel-0.3.0.dev0/semantic_kernel/utils/validation.py
+-rw-r--r--   0        0        0     1760 1970-01-01 00:00:00.000000 semantic_kernel-0.3.0.dev0/PKG-INFO
```

### Comparing `semantic_kernel-0.2.9.dev0/pip/README.md` & `semantic_kernel-0.3.0.dev0/pip/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/pyproject.toml` & `semantic_kernel-0.3.0.dev0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "semantic-kernel"
-version = "0.2.9.dev"
+version = "0.3.0.dev"
 description = ""
 authors = ["Microsoft <SK-Support@microsoft.com>"]
 readme = "pip/README.md"
 packages = [{include = "semantic_kernel"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -25,14 +25,18 @@
 transformers = "^4.28.1"
 sentence-transformers = "^2.2.2"
 torch = "2.0.0"
 
 [tool.poetry.group.chromadb.dependencies]
 chromadb = "^0.3.23"
 
+
+[tool.poetry.group.weaviate.dependencies]
+weaviate-client = "^3.18.0"
+
 [tool.isort]
 profile = "black"
 
 [tool.ruff]
 line-length = 120
 
 [build-system]
```

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/__init__.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/__init__.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/ai_exception.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/ai_exception.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/chat_completion_client_base.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/chat_completion_client_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/chat_request_settings.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/chat_request_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/complete_request_settings.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/complete_request_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/open_ai/__init__.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/open_ai/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/ai/text_completion_client_base.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/ai/text_completion_client_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,14 +123,16 @@
             collection_name {str} -- The name of the collection to delete.
 
         Returns:
             None
         """
         # Current version of ChromeDB reject camel case collection names.
         self._client.delete_collection(name=camel_to_snake(collection_name))
+        if self._persist_directory is not None:
+            self._client.persist()
 
     async def does_collection_exist_async(self, collection_name: str) -> bool:
         """Checks if a collection exists.
 
         Arguments:
             collection_name {str} -- The name of the collection to check.
 
@@ -167,15 +169,16 @@
         collection.add(
             metadatas=metadata,
             # by providing embeddings, we can skip the chroma's embedding function call
             embeddings=record.embedding.tolist(),
             documents=record._text,
             ids=record._id,
         )
-
+        if self._persist_directory is not None:
+            self._client.persist()
         return record._id
 
     async def upsert_batch_async(
         self, collection_name: str, records: List[MemoryRecord]
     ) -> List[str]:
         """Upserts a batch of records.
```

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/connectors/memory/chroma/utils.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/connectors/memory/chroma/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/core_skills/__init__.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/core_skills/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/core_skills/conversation_summary_skill.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/core_skills/conversation_summary_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/core_skills/file_io_skill.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/core_skills/file_io_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/core_skills/http_skill.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/core_skills/http_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/core_skills/math_skill.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/core_skills/math_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/core_skills/text_memory_skill.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/core_skills/text_memory_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/core_skills/text_skill.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/core_skills/text_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/core_skills/time_skill.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/core_skills/time_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/kernel.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/kernel.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/kernel_exception.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/kernel_exception.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/memory/memory_query_result.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/memory/memory_query_result.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/memory/memory_record.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/memory/memory_record.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/memory/memory_store_base.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/memory/memory_store_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/memory/null_memory.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/memory/null_memory.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/memory/semantic_text_memory.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/memory/semantic_text_memory.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
             collection {str} -- The collection to get the information from.
             key {str} -- The key of the information.
 
         Returns:
             Optional[MemoryQueryResult] -- The MemoryQueryResult if found, None otherwise.
         """
         record = await self._storage.get_async(collection_name=collection, key=key)
-        return MemoryQueryResult.from_memory_record(record) if record else None
+        return MemoryQueryResult.from_memory_record(record, 1.0) if record else None
 
     async def search_async(
         self,
         collection: str,
         query: str,
         limit: int = 1,
         min_relevance_score: float = 0.0,
```

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/memory/semantic_text_memory_base.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/memory/semantic_text_memory_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/memory/volatile_memory_store.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/memory/volatile_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/orchestration/context_variables.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/orchestration/context_variables.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/orchestration/delegate_handlers.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/orchestration/delegate_handlers.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/orchestration/delegate_inference.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/orchestration/delegate_inference.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/orchestration/delegate_types.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/orchestration/delegate_types.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/orchestration/sk_context.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/orchestration/sk_context.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/orchestration/sk_function.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/orchestration/sk_function.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/orchestration/sk_function_base.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/orchestration/sk_function_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/planning/basic_planner.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/planning/basic_planner.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/reliability/pass_through_without_retry.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/reliability/pass_through_without_retry.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/reliability/retry_mechanism_base.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/reliability/retry_mechanism_base.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) Microsoft. All rights reserved.
 
-from abc import ABC, abstractmethod
 import logging
+from abc import ABC, abstractmethod
 from typing import Awaitable, Callable, TypeVar
 
 T = TypeVar("T")
 
 
 class RetryMechanismBase(ABC):
     @abstractmethod
```

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/semantic_functions/prompt_template.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/semantic_functions/prompt_template.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/semantic_functions/prompt_template_config.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/semantic_functions/prompt_template_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/semantic_functions/semantic_function_config.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/semantic_functions/semantic_function_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/skill_definition/function_view.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/skill_definition/function_view.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/skill_definition/functions_view.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/skill_definition/functions_view.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/skill_definition/parameter_view.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/skill_definition/parameter_view.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/skill_definition/sk_function_decorator.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/skill_definition/sk_function_decorator.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/skill_definition/skill_collection.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/skill_definition/skill_collection.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/skill_definition/skill_collection_base.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/skill_definition/skill_collection_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/README.md` & `semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/blocks/block.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/blocks/block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/blocks/code_block.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/blocks/code_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/blocks/function_id_block.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/blocks/function_id_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/blocks/text_block.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/blocks/text_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/blocks/val_block.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/blocks/val_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/blocks/var_block.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/blocks/var_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/code_tokenizer.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/code_tokenizer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/prompt_template_engine.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/prompt_template_engine.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/protocols/code_renderer.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/protocols/code_renderer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/protocols/text_renderer.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/protocols/text_renderer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/template_engine/template_tokenizer.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/template_engine/template_tokenizer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/text/function_extension.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/text/function_extension.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/text/text_chunker.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/text/text_chunker.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/utils/settings.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/utils/settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/semantic_kernel/utils/validation.py` & `semantic_kernel-0.3.0.dev0/semantic_kernel/utils/validation.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.9.dev0/PKG-INFO` & `semantic_kernel-0.3.0.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantic-kernel
-Version: 0.2.9.dev0
+Version: 0.3.0.dev0
 Summary: 
 Author: Microsoft
 Author-email: SK-Support@microsoft.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

