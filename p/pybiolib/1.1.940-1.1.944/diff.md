# Comparing `tmp/pybiolib-1.1.940.tar.gz` & `tmp/pybiolib-1.1.944.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybiolib-1.1.940.tar", max compression
+gzip compressed data, was "pybiolib-1.1.944.tar", max compression
```

## Comparing `pybiolib-1.1.940.tar` & `pybiolib-1.1.944.tar`

### file list

```diff
@@ -1,110 +1,110 @@
--rw-r--r--   0        0        0     1067 2023-06-05 08:42:48.148137 pybiolib-1.1.940/LICENSE
--rw-r--r--   0        0        0      368 2023-06-05 08:42:48.148137 pybiolib-1.1.940/README.md
--rw-r--r--   0        0        0     3337 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/__init__.py
--rw-r--r--   0        0        0       95 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/api/__init__.py
--rw-r--r--   0        0        0     3744 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/api/client.py
--rw-r--r--   0        0        0       37 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/app/__init__.py
--rw-r--r--   0        0        0     7652 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/app/app.py
--rw-r--r--   0        0        0     1493 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/app/search_apps.py
--rw-r--r--   0        0        0     4405 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/app/utils.py
--rw-r--r--   0        0        0      182 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/biolib_api_client/__init__.py
--rw-r--r--   0        0        0     5574 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/biolib_api_client/api_client.py
--rw-r--r--   0        0        0     2397 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/biolib_api_client/app_types.py
--rw-r--r--   0        0        0     1668 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/biolib_api_client/auth.py
--rw-r--r--   0        0        0      580 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/biolib_api_client/biolib_account_api.py
--rw-r--r--   0        0        0     2859 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/biolib_api_client/biolib_app_api.py
--rw-r--r--   0        0        0     9865 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/biolib_api_client/biolib_job_api.py
--rw-r--r--   0        0        0     1777 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/biolib_api_client/biolib_large_file_system_api.py
--rw-r--r--   0        0        0      123 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/biolib_api_client/common_types.py
--rw-r--r--   0        0        0     1256 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/biolib_api_client/job_types.py
--rw-r--r--   0        0        0      227 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/biolib_api_client/lfs_types.py
--rw-r--r--   0        0        0      637 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/biolib_api_client/user_state.py
--rw-r--r--   0        0        0      303 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/biolib_binary_format/__init__.py
--rw-r--r--   0        0        0      959 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/biolib_binary_format/base_bbf_package.py
--rw-r--r--   0        0        0      154 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/biolib_binary_format/common_types.py
--rw-r--r--   0        0        0     6450 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/biolib_binary_format/encrypted_module_output.py
--rw-r--r--   0        0        0     2603 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/biolib_binary_format/module_input.py
--rw-r--r--   0        0        0     2640 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/biolib_binary_format/module_output.py
--rw-r--r--   0        0        0     2269 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/biolib_binary_format/rsa_encrypted_aes_package.py
--rw-r--r--   0        0        0     1125 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/biolib_binary_format/saved_job.py
--rw-r--r--   0        0        0     1023 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/biolib_binary_format/stdout_and_stderr.py
--rw-r--r--   0        0        0      853 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/biolib_binary_format/system_exception.py
--rw-r--r--   0        0        0     1191 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/biolib_binary_format/system_status_update.py
--rw-r--r--   0        0        0     8514 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/biolib_binary_format/unencrypted_module_output.py
--rw-r--r--   0        0        0     3938 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/biolib_binary_format/utils.py
--rw-r--r--   0        0        0     1481 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/biolib_docker_client/__init__.py
--rw-r--r--   0        0        0      532 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/biolib_errors.py
--rw-r--r--   0        0        0     2854 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/biolib_logging.py
--rw-r--r--   0        0        0    10225 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/biolib_push.py
--rw-r--r--   0        0        0      947 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/cli/__init__.py
--rw-r--r--   0        0        0      820 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/cli/init.py
--rw-r--r--   0        0        0     1966 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/cli/lfs.py
--rw-r--r--   0        0        0      798 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/cli/push.py
--rw-r--r--   0        0        0     1309 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/cli/run.py
--rw-r--r--   0        0        0      361 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/cli/runtime.py
--rw-r--r--   0        0        0     1284 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/cli/start.py
--rw-r--r--   0        0        0     8947 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/cli_utils.py
--rw-r--r--   0        0        0       45 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/compute_node/.gitignore
--rw-r--r--   0        0        0        0 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/compute_node/__init__.py
--rw-r--r--   0        0        0       67 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/compute_node/cloud_utils/__init__.py
--rw-r--r--   0        0        0     6878 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/compute_node/cloud_utils/cloud_utils.py
--rw-r--r--   0        0        0       71 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/compute_node/job_worker/__init__.py
--rw-r--r--   0        0        0     3670 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/compute_node/job_worker/cache_state.py
--rw-r--r--   0        0        0      891 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/compute_node/job_worker/cache_types.py
--rw-r--r--   0        0        0     7562 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/compute_node/job_worker/docker_image_cache.py
--rw-r--r--   0        0        0      221 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/compute_node/job_worker/executors/__init__.py
--rw-r--r--   0        0        0      448 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/compute_node/job_worker/executors/base_executor.py
--rw-r--r--   0        0        0    24367 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/compute_node/job_worker/executors/docker_executor.py
--rw-r--r--   0        0        0      122 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/compute_node/job_worker/executors/docker_types.py
--rw-r--r--   0        0        0       91 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/compute_node/job_worker/executors/remote/__init__.py
--rw-r--r--   0        0        0     1595 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/compute_node/job_worker/executors/remote/remote_executor.py
--rw-r--r--   0        0        0        0 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/compute_node/job_worker/executors/tars/__init__.py
--rw-r--r--   0        0        0     1564 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/compute_node/job_worker/executors/types.py
--rw-r--r--   0        0        0     1198 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/compute_node/job_worker/job_legacy_input_wait_timeout_thread.py
--rw-r--r--   0        0        0     1174 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/compute_node/job_worker/job_max_runtime_timer_thread.py
--rw-r--r--   0        0        0     4858 2023-06-05 08:42:48.148137 pybiolib-1.1.940/biolib/compute_node/job_worker/job_storage.py
--rw-r--r--   0        0        0    29919 2023-06-05 08:42:48.152137 pybiolib-1.1.940/biolib/compute_node/job_worker/job_worker.py
--rw-r--r--   0        0        0     9363 2023-06-05 08:42:48.152137 pybiolib-1.1.940/biolib/compute_node/job_worker/large_file_system.py
--rw-r--r--   0        0        0     2499 2023-06-05 08:42:48.152137 pybiolib-1.1.940/biolib/compute_node/job_worker/mappings.py
--rw-r--r--   0        0        0     1282 2023-06-05 08:42:48.152137 pybiolib-1.1.940/biolib/compute_node/job_worker/utils.py
--rw-r--r--   0        0        0    12865 2023-06-05 08:42:48.152137 pybiolib-1.1.940/biolib/compute_node/remote_host_proxy.py
--rw-r--r--   0        0        0     1601 2023-06-05 08:42:48.152137 pybiolib-1.1.940/biolib/compute_node/socker_listener_thread.py
--rw-r--r--   0        0        0      971 2023-06-05 08:42:48.152137 pybiolib-1.1.940/biolib/compute_node/socket_sender_thread.py
--rw-r--r--   0        0        0     4434 2023-06-05 08:42:48.152137 pybiolib-1.1.940/biolib/compute_node/utils.py
--rw-r--r--   0        0        0        0 2023-06-05 08:42:48.152137 pybiolib-1.1.940/biolib/compute_node/webserver/__init__.py
--rw-r--r--   0        0        0      914 2023-06-05 08:42:48.152137 pybiolib-1.1.940/biolib/compute_node/webserver/gunicorn_flask_application.py
--rw-r--r--   0        0        0     7647 2023-06-05 08:42:48.152137 pybiolib-1.1.940/biolib/compute_node/webserver/webserver.py
--rw-r--r--   0        0        0      420 2023-06-05 08:42:48.152137 pybiolib-1.1.940/biolib/compute_node/webserver/webserver_types.py
--rw-r--r--   0        0        0     4234 2023-06-05 08:42:48.152137 pybiolib-1.1.940/biolib/compute_node/webserver/webserver_utils.py
--rw-r--r--   0        0        0     9900 2023-06-05 08:42:48.152137 pybiolib-1.1.940/biolib/compute_node/webserver/worker_thread.py
--rw-r--r--   0        0        0        0 2023-06-05 08:42:48.152137 pybiolib-1.1.940/biolib/experiments/__init__.py
--rw-r--r--   0        0        0     5939 2023-06-05 08:42:48.152137 pybiolib-1.1.940/biolib/experiments/experiment.py
--rw-r--r--   0        0        0      171 2023-06-05 08:42:48.152137 pybiolib-1.1.940/biolib/experiments/types.py
--rw-r--r--   0        0        0       32 2023-06-05 08:42:48.152137 pybiolib-1.1.940/biolib/jobs/__init__.py
--rw-r--r--   0        0        0    14468 2023-06-05 08:42:48.152137 pybiolib-1.1.940/biolib/jobs/job.py
--rw-r--r--   0        0        0     5937 2023-06-05 08:42:48.152137 pybiolib-1.1.940/biolib/jobs/job_result.py
--rw-r--r--   0        0        0      905 2023-06-05 08:42:48.152137 pybiolib-1.1.940/biolib/jobs/types.py
--rw-r--r--   0        0        0      193 2023-06-05 08:42:48.152137 pybiolib-1.1.940/biolib/lfs/__init__.py
--rw-r--r--   0        0        0     2226 2023-06-05 08:42:48.152137 pybiolib-1.1.940/biolib/lfs/cache.py
--rw-r--r--   0        0        0     9832 2023-06-05 08:42:48.152137 pybiolib-1.1.940/biolib/lfs/utils.py
--rw-r--r--   0        0        0       44 2023-06-05 08:42:48.152137 pybiolib-1.1.940/biolib/runtime/__init__.py
--rw-r--r--   0        0        0      778 2023-06-05 08:42:48.152137 pybiolib-1.1.940/biolib/runtime/results.py
--rw-r--r--   0        0        0      210 2023-06-05 08:42:48.152137 pybiolib-1.1.940/biolib/start_cli.py
--rw-r--r--   0        0        0      872 2023-06-05 08:42:48.152137 pybiolib-1.1.940/biolib/tables.py
--rw-r--r--   0        0        0       36 2023-06-05 08:42:48.152137 pybiolib-1.1.940/biolib/templates/__init__.py
--rw-r--r--   0        0        0      715 2023-06-05 08:42:48.152137 pybiolib-1.1.940/biolib/templates/example_app.py
--rw-r--r--   0        0        0      263 2023-06-05 08:42:48.152137 pybiolib-1.1.940/biolib/typing_utils.py
--rw-r--r--   0        0        0       39 2023-06-05 08:42:48.152137 pybiolib-1.1.940/biolib/user/__init__.py
--rw-r--r--   0        0        0     2061 2023-06-05 08:42:48.152137 pybiolib-1.1.940/biolib/user/sign_in.py
--rw-r--r--   0        0        0     8190 2023-06-05 08:42:48.152137 pybiolib-1.1.940/biolib/utils/__init__.py
--rw-r--r--   0        0        0     2727 2023-06-05 08:42:48.152137 pybiolib-1.1.940/biolib/utils/cache_state.py
--rw-r--r--   0        0        0     9717 2023-06-05 08:42:48.152137 pybiolib-1.1.940/biolib/utils/multipart_uploader.py
--rw-r--r--   0        0        0     1757 2023-06-05 08:42:48.152137 pybiolib-1.1.940/biolib/utils/seq_util.py
--rw-r--r--   0        0        0    23500 2023-06-05 08:42:48.152137 pybiolib-1.1.940/biolib/utils/zip/remote_zip.py
--rw-r--r--   0        0        0     6916 2023-06-05 08:42:48.152137 pybiolib-1.1.940/biolib/validators/validate_app_version.py
--rw-r--r--   0        0        0     4300 2023-06-05 08:42:48.152137 pybiolib-1.1.940/biolib/validators/validate_argument.py
--rw-r--r--   0        0        0    13298 2023-06-05 08:42:48.152137 pybiolib-1.1.940/biolib/validators/validate_module.py
--rw-r--r--   0        0        0     1655 2023-06-05 08:42:48.152137 pybiolib-1.1.940/biolib/validators/validate_zip_file.py
--rw-r--r--   0        0        0     2135 2023-06-05 08:42:48.152137 pybiolib-1.1.940/biolib/validators/validator_utils.py
--rw-r--r--   0        0        0     1237 2023-06-05 08:43:39.572781 pybiolib-1.1.940/pyproject.toml
--rw-r--r--   0        0        0     1611 1970-01-01 00:00:00.000000 pybiolib-1.1.940/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-05 12:44:22.417800 pybiolib-1.1.944/LICENSE
+-rw-r--r--   0        0        0      368 2023-06-05 12:44:22.417800 pybiolib-1.1.944/README.md
+-rw-r--r--   0        0        0     3337 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/__init__.py
+-rw-r--r--   0        0        0       95 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/api/__init__.py
+-rw-r--r--   0        0        0     3744 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/api/client.py
+-rw-r--r--   0        0        0       37 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/app/__init__.py
+-rw-r--r--   0        0        0     7652 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/app/app.py
+-rw-r--r--   0        0        0     1493 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/app/search_apps.py
+-rw-r--r--   0        0        0     4405 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/app/utils.py
+-rw-r--r--   0        0        0      182 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_api_client/__init__.py
+-rw-r--r--   0        0        0     5574 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_api_client/api_client.py
+-rw-r--r--   0        0        0     2397 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_api_client/app_types.py
+-rw-r--r--   0        0        0     1668 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_api_client/auth.py
+-rw-r--r--   0        0        0      580 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_api_client/biolib_account_api.py
+-rw-r--r--   0        0        0     2859 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_api_client/biolib_app_api.py
+-rw-r--r--   0        0        0     9865 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_api_client/biolib_job_api.py
+-rw-r--r--   0        0        0     1777 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_api_client/biolib_large_file_system_api.py
+-rw-r--r--   0        0        0      123 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_api_client/common_types.py
+-rw-r--r--   0        0        0     1256 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_api_client/job_types.py
+-rw-r--r--   0        0        0      227 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_api_client/lfs_types.py
+-rw-r--r--   0        0        0      637 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_api_client/user_state.py
+-rw-r--r--   0        0        0      303 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_binary_format/__init__.py
+-rw-r--r--   0        0        0      959 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_binary_format/base_bbf_package.py
+-rw-r--r--   0        0        0      154 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_binary_format/common_types.py
+-rw-r--r--   0        0        0     6450 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_binary_format/encrypted_module_output.py
+-rw-r--r--   0        0        0     2603 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_binary_format/module_input.py
+-rw-r--r--   0        0        0     2640 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_binary_format/module_output.py
+-rw-r--r--   0        0        0     2269 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_binary_format/rsa_encrypted_aes_package.py
+-rw-r--r--   0        0        0     1125 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_binary_format/saved_job.py
+-rw-r--r--   0        0        0     1023 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_binary_format/stdout_and_stderr.py
+-rw-r--r--   0        0        0      853 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_binary_format/system_exception.py
+-rw-r--r--   0        0        0     1191 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_binary_format/system_status_update.py
+-rw-r--r--   0        0        0     8514 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_binary_format/unencrypted_module_output.py
+-rw-r--r--   0        0        0     3938 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_binary_format/utils.py
+-rw-r--r--   0        0        0     1481 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_docker_client/__init__.py
+-rw-r--r--   0        0        0      532 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_errors.py
+-rw-r--r--   0        0        0     2854 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_logging.py
+-rw-r--r--   0        0        0    10225 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/biolib_push.py
+-rw-r--r--   0        0        0      947 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/cli/__init__.py
+-rw-r--r--   0        0        0      820 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/cli/init.py
+-rw-r--r--   0        0        0     1966 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/cli/lfs.py
+-rw-r--r--   0        0        0      798 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/cli/push.py
+-rw-r--r--   0        0        0     1309 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/cli/run.py
+-rw-r--r--   0        0        0      361 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/cli/runtime.py
+-rw-r--r--   0        0        0     1284 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/cli/start.py
+-rw-r--r--   0        0        0     8947 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/cli_utils.py
+-rw-r--r--   0        0        0       45 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/.gitignore
+-rw-r--r--   0        0        0        0 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/__init__.py
+-rw-r--r--   0        0        0       67 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/cloud_utils/__init__.py
+-rw-r--r--   0        0        0     6878 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/cloud_utils/cloud_utils.py
+-rw-r--r--   0        0        0       71 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/job_worker/__init__.py
+-rw-r--r--   0        0        0     3670 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/job_worker/cache_state.py
+-rw-r--r--   0        0        0      891 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/job_worker/cache_types.py
+-rw-r--r--   0        0        0     7562 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/job_worker/docker_image_cache.py
+-rw-r--r--   0        0        0      221 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/job_worker/executors/__init__.py
+-rw-r--r--   0        0        0      448 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/job_worker/executors/base_executor.py
+-rw-r--r--   0        0        0    24367 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/job_worker/executors/docker_executor.py
+-rw-r--r--   0        0        0      122 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/job_worker/executors/docker_types.py
+-rw-r--r--   0        0        0       91 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/job_worker/executors/remote/__init__.py
+-rw-r--r--   0        0        0     1595 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/job_worker/executors/remote/remote_executor.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/job_worker/executors/tars/__init__.py
+-rw-r--r--   0        0        0     1564 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/job_worker/executors/types.py
+-rw-r--r--   0        0        0     1198 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/job_worker/job_legacy_input_wait_timeout_thread.py
+-rw-r--r--   0        0        0     1174 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/job_worker/job_max_runtime_timer_thread.py
+-rw-r--r--   0        0        0     4858 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/job_worker/job_storage.py
+-rw-r--r--   0        0        0    30595 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/job_worker/job_worker.py
+-rw-r--r--   0        0        0     9363 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/job_worker/large_file_system.py
+-rw-r--r--   0        0        0     2499 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/job_worker/mappings.py
+-rw-r--r--   0        0        0     1282 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/job_worker/utils.py
+-rw-r--r--   0        0        0    12865 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/remote_host_proxy.py
+-rw-r--r--   0        0        0     1601 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/socker_listener_thread.py
+-rw-r--r--   0        0        0      971 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/socket_sender_thread.py
+-rw-r--r--   0        0        0     4529 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/utils.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:44:22.417800 pybiolib-1.1.944/biolib/compute_node/webserver/__init__.py
+-rw-r--r--   0        0        0      914 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/compute_node/webserver/gunicorn_flask_application.py
+-rw-r--r--   0        0        0     7647 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/compute_node/webserver/webserver.py
+-rw-r--r--   0        0        0      420 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/compute_node/webserver/webserver_types.py
+-rw-r--r--   0        0        0     4234 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/compute_node/webserver/webserver_utils.py
+-rw-r--r--   0        0        0     9900 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/compute_node/webserver/worker_thread.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/experiments/__init__.py
+-rw-r--r--   0        0        0     5939 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/experiments/experiment.py
+-rw-r--r--   0        0        0      171 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/experiments/types.py
+-rw-r--r--   0        0        0       32 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/jobs/__init__.py
+-rw-r--r--   0        0        0    14468 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/jobs/job.py
+-rw-r--r--   0        0        0     5937 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/jobs/job_result.py
+-rw-r--r--   0        0        0      905 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/jobs/types.py
+-rw-r--r--   0        0        0      193 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/lfs/__init__.py
+-rw-r--r--   0        0        0     2226 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/lfs/cache.py
+-rw-r--r--   0        0        0     9832 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/lfs/utils.py
+-rw-r--r--   0        0        0       44 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/runtime/__init__.py
+-rw-r--r--   0        0        0      778 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/runtime/results.py
+-rw-r--r--   0        0        0      210 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/start_cli.py
+-rw-r--r--   0        0        0      872 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/tables.py
+-rw-r--r--   0        0        0       36 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/templates/__init__.py
+-rw-r--r--   0        0        0      715 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/templates/example_app.py
+-rw-r--r--   0        0        0      263 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/typing_utils.py
+-rw-r--r--   0        0        0       39 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/user/__init__.py
+-rw-r--r--   0        0        0     2061 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/user/sign_in.py
+-rw-r--r--   0        0        0     8190 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/utils/__init__.py
+-rw-r--r--   0        0        0     2727 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/utils/cache_state.py
+-rw-r--r--   0        0        0     9717 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/utils/multipart_uploader.py
+-rw-r--r--   0        0        0     1757 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/utils/seq_util.py
+-rw-r--r--   0        0        0    23500 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/utils/zip/remote_zip.py
+-rw-r--r--   0        0        0     6916 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/validators/validate_app_version.py
+-rw-r--r--   0        0        0     4300 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/validators/validate_argument.py
+-rw-r--r--   0        0        0    13298 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/validators/validate_module.py
+-rw-r--r--   0        0        0     1655 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/validators/validate_zip_file.py
+-rw-r--r--   0        0        0     2135 2023-06-05 12:44:22.421800 pybiolib-1.1.944/biolib/validators/validator_utils.py
+-rw-r--r--   0        0        0     1237 2023-06-05 12:45:11.918897 pybiolib-1.1.944/pyproject.toml
+-rw-r--r--   0        0        0     1611 1970-01-01 00:00:00.000000 pybiolib-1.1.944/PKG-INFO
```

### Comparing `pybiolib-1.1.940/LICENSE` & `pybiolib-1.1.944/LICENSE`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/__init__.py` & `pybiolib-1.1.944/biolib/__init__.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/api/client.py` & `pybiolib-1.1.944/biolib/api/client.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/app/app.py` & `pybiolib-1.1.944/biolib/app/app.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/app/search_apps.py` & `pybiolib-1.1.944/biolib/app/search_apps.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/app/utils.py` & `pybiolib-1.1.944/biolib/app/utils.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/biolib_api_client/api_client.py` & `pybiolib-1.1.944/biolib/biolib_api_client/api_client.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/biolib_api_client/app_types.py` & `pybiolib-1.1.944/biolib/biolib_api_client/app_types.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/biolib_api_client/auth.py` & `pybiolib-1.1.944/biolib/biolib_api_client/auth.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/biolib_api_client/biolib_account_api.py` & `pybiolib-1.1.944/biolib/biolib_api_client/biolib_account_api.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/biolib_api_client/biolib_app_api.py` & `pybiolib-1.1.944/biolib/biolib_api_client/biolib_app_api.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/biolib_api_client/biolib_job_api.py` & `pybiolib-1.1.944/biolib/biolib_api_client/biolib_job_api.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/biolib_api_client/biolib_large_file_system_api.py` & `pybiolib-1.1.944/biolib/biolib_api_client/biolib_large_file_system_api.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/biolib_api_client/job_types.py` & `pybiolib-1.1.944/biolib/biolib_api_client/job_types.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/biolib_api_client/user_state.py` & `pybiolib-1.1.944/biolib/biolib_api_client/user_state.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/biolib_binary_format/base_bbf_package.py` & `pybiolib-1.1.944/biolib/biolib_binary_format/base_bbf_package.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/biolib_binary_format/encrypted_module_output.py` & `pybiolib-1.1.944/biolib/biolib_binary_format/encrypted_module_output.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/biolib_binary_format/module_input.py` & `pybiolib-1.1.944/biolib/biolib_binary_format/module_input.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/biolib_binary_format/module_output.py` & `pybiolib-1.1.944/biolib/biolib_binary_format/module_output.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/biolib_binary_format/rsa_encrypted_aes_package.py` & `pybiolib-1.1.944/biolib/biolib_binary_format/rsa_encrypted_aes_package.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/biolib_binary_format/saved_job.py` & `pybiolib-1.1.944/biolib/biolib_binary_format/saved_job.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/biolib_binary_format/stdout_and_stderr.py` & `pybiolib-1.1.944/biolib/biolib_binary_format/stdout_and_stderr.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/biolib_binary_format/system_exception.py` & `pybiolib-1.1.944/biolib/biolib_binary_format/system_exception.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/biolib_binary_format/system_status_update.py` & `pybiolib-1.1.944/biolib/biolib_binary_format/system_status_update.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/biolib_binary_format/unencrypted_module_output.py` & `pybiolib-1.1.944/biolib/biolib_binary_format/unencrypted_module_output.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/biolib_binary_format/utils.py` & `pybiolib-1.1.944/biolib/biolib_binary_format/utils.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/biolib_docker_client/__init__.py` & `pybiolib-1.1.944/biolib/biolib_docker_client/__init__.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/biolib_errors.py` & `pybiolib-1.1.944/biolib/biolib_errors.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/biolib_logging.py` & `pybiolib-1.1.944/biolib/biolib_logging.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/biolib_push.py` & `pybiolib-1.1.944/biolib/biolib_push.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/cli/__init__.py` & `pybiolib-1.1.944/biolib/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/cli/init.py` & `pybiolib-1.1.944/biolib/cli/init.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/cli/lfs.py` & `pybiolib-1.1.944/biolib/cli/lfs.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/cli/push.py` & `pybiolib-1.1.944/biolib/cli/push.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/cli/run.py` & `pybiolib-1.1.944/biolib/cli/run.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/cli/start.py` & `pybiolib-1.1.944/biolib/cli/start.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/cli_utils.py` & `pybiolib-1.1.944/biolib/cli_utils.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/compute_node/cloud_utils/cloud_utils.py` & `pybiolib-1.1.944/biolib/compute_node/cloud_utils/cloud_utils.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/compute_node/job_worker/cache_state.py` & `pybiolib-1.1.944/biolib/compute_node/job_worker/cache_state.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/compute_node/job_worker/cache_types.py` & `pybiolib-1.1.944/biolib/compute_node/job_worker/cache_types.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/compute_node/job_worker/docker_image_cache.py` & `pybiolib-1.1.944/biolib/compute_node/job_worker/docker_image_cache.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/compute_node/job_worker/executors/docker_executor.py` & `pybiolib-1.1.944/biolib/compute_node/job_worker/executors/docker_executor.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/compute_node/job_worker/executors/remote/remote_executor.py` & `pybiolib-1.1.944/biolib/compute_node/job_worker/executors/remote/remote_executor.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/compute_node/job_worker/executors/types.py` & `pybiolib-1.1.944/biolib/compute_node/job_worker/executors/types.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/compute_node/job_worker/job_legacy_input_wait_timeout_thread.py` & `pybiolib-1.1.944/biolib/compute_node/job_worker/job_legacy_input_wait_timeout_thread.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/compute_node/job_worker/job_max_runtime_timer_thread.py` & `pybiolib-1.1.944/biolib/compute_node/job_worker/job_max_runtime_timer_thread.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/compute_node/job_worker/job_storage.py` & `pybiolib-1.1.944/biolib/compute_node/job_worker/job_storage.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/compute_node/job_worker/job_worker.py` & `pybiolib-1.1.944/biolib/compute_node/job_worker/job_worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -488,31 +488,43 @@
             # Log memory and disk after pulling and executing module
             log_disk_and_memory_usage_info()
 
         return module_output_serialized
 
     def _run_module(self, options: LocalExecutorOptions, module_input_serialized: bytes) -> bytes:
         module = options['module']
+        job_id = options['job']['public_id']
+        logger_no_user_data.debug(f'Job "{job_id}" running module "{module["name"]}"...')
         executor_instance: BaseExecutor
 
         if module['environment'] == ModuleEnvironment.BIOLIB_APP.value:
+            logger_no_user_data.debug(f'Job "{job_id}" starting child job...')
             module_input = ModuleInput(module_input_serialized).deserialize()
             module_input_with_runtime_zip = self._add_runtime_zip_and_command_to_module_input(options, module_input)
             module_input_with_runtime_zip_serialized = ModuleInput().serialize(
                 stdin=module_input_with_runtime_zip['stdin'],
                 arguments=module_input_with_runtime_zip['arguments'],
                 files=module_input_with_runtime_zip['files'],
             )
             return self._run_app_version(module['image_uri'], module_input_with_runtime_zip_serialized, options['job'])
 
         elif module['environment'] == ModuleEnvironment.BIOLIB_ECR.value and BiolibDockerClient.is_docker_running():
-            executor_instance = DockerExecutor(options)
-
+            try:
+                executor_instance = DockerExecutor(options)
+            except Exception as exception:
+                raise ComputeProcessException(
+                    exception,
+                    SystemExceptionCodes.FAILED_TO_INITIALIZE_DOCKER_EXECUTOR.value,
+                    self.send_system_exception,
+                    may_contain_user_data=False
+                ) from exception
         else:
-            raise Exception(f"Unsupported module environment {module['environment']}")
+            err_string = f'Job "{job_id}" hit unsupported module environment "{module["environment"]}"'
+            logger_no_user_data.error(err_string)
+            raise Exception(err_string)
 
         self._executors.append(executor_instance)
 
         if utils.IS_RUNNING_IN_CLOUD:
             # Log memory and disk before pulling and executing module
             log_disk_and_memory_usage_info()
```

### Comparing `pybiolib-1.1.940/biolib/compute_node/job_worker/large_file_system.py` & `pybiolib-1.1.944/biolib/compute_node/job_worker/large_file_system.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/compute_node/job_worker/mappings.py` & `pybiolib-1.1.944/biolib/compute_node/job_worker/mappings.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/compute_node/job_worker/utils.py` & `pybiolib-1.1.944/biolib/compute_node/job_worker/utils.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/compute_node/remote_host_proxy.py` & `pybiolib-1.1.944/biolib/compute_node/remote_host_proxy.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/compute_node/socker_listener_thread.py` & `pybiolib-1.1.944/biolib/compute_node/socker_listener_thread.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/compute_node/socket_sender_thread.py` & `pybiolib-1.1.944/biolib/compute_node/socket_sender_thread.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/compute_node/utils.py` & `pybiolib-1.1.944/biolib/compute_node/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,14 +63,15 @@
     FAILED_TO_HANDLE_PACKAGE_IN_WORKER_THREAD = 27
     EXCEEDED_MAX_JOB_RUNTIME = 28
     OUT_OF_MEMORY = 29
     CANCELLED_BY_USER = 30
     COMMAND_OVERRIDE_NOT_ALLOWED = 31
     FAILED_TO_ALLOCATE_JOB_TO_COMPUTE_NODE = 32
     NO_MODULES_FOUND_ON_JOB = 33
+    FAILED_TO_INITIALIZE_DOCKER_EXECUTOR = 34
 
 
 SystemExceptionCodeMap = {
     0: 'Job completed successfully',
     1: 'Failed to init compute process variables',
     2: 'Failed to connect to worker thread socket',
     3: 'Failed to start sender or receiver thread',
@@ -99,15 +100,16 @@
     26: 'Failed to initialize worker thread',
     27: 'Failed to handle package in worker thread',
     28: 'Job exceeded max run time',
     29: 'Container ran out of memory',
     30: 'Job was cancelled by the user',
     31: 'The application does not allow the arguments to override the command',
     32: 'Failed to allocate job to compute node',
-    33: 'No modules found on job'
+    33: 'No modules found on job',
+    34: 'Failed to initialize docker executor',
 }
 
 
 class WorkerThreadException(Exception):
     def __init__(self, original_error, error_code, worker_thread):
         super().__init__()
         worker_thread.compute_state['status']['error_code'] = error_code
```

### Comparing `pybiolib-1.1.940/biolib/compute_node/webserver/gunicorn_flask_application.py` & `pybiolib-1.1.944/biolib/compute_node/webserver/gunicorn_flask_application.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/compute_node/webserver/webserver.py` & `pybiolib-1.1.944/biolib/compute_node/webserver/webserver.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/compute_node/webserver/webserver_utils.py` & `pybiolib-1.1.944/biolib/compute_node/webserver/webserver_utils.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/compute_node/webserver/worker_thread.py` & `pybiolib-1.1.944/biolib/compute_node/webserver/worker_thread.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/experiments/experiment.py` & `pybiolib-1.1.944/biolib/experiments/experiment.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/jobs/job.py` & `pybiolib-1.1.944/biolib/jobs/job.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/jobs/job_result.py` & `pybiolib-1.1.944/biolib/jobs/job_result.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/jobs/types.py` & `pybiolib-1.1.944/biolib/jobs/types.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/lfs/cache.py` & `pybiolib-1.1.944/biolib/lfs/cache.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/lfs/utils.py` & `pybiolib-1.1.944/biolib/lfs/utils.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/runtime/results.py` & `pybiolib-1.1.944/biolib/runtime/results.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/tables.py` & `pybiolib-1.1.944/biolib/tables.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/templates/example_app.py` & `pybiolib-1.1.944/biolib/templates/example_app.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/user/sign_in.py` & `pybiolib-1.1.944/biolib/user/sign_in.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/utils/__init__.py` & `pybiolib-1.1.944/biolib/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/utils/cache_state.py` & `pybiolib-1.1.944/biolib/utils/cache_state.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/utils/multipart_uploader.py` & `pybiolib-1.1.944/biolib/utils/multipart_uploader.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/utils/seq_util.py` & `pybiolib-1.1.944/biolib/utils/seq_util.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/utils/zip/remote_zip.py` & `pybiolib-1.1.944/biolib/utils/zip/remote_zip.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/validators/validate_app_version.py` & `pybiolib-1.1.944/biolib/validators/validate_app_version.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/validators/validate_argument.py` & `pybiolib-1.1.944/biolib/validators/validate_argument.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/validators/validate_module.py` & `pybiolib-1.1.944/biolib/validators/validate_module.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/validators/validate_zip_file.py` & `pybiolib-1.1.944/biolib/validators/validate_zip_file.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/biolib/validators/validator_utils.py` & `pybiolib-1.1.944/biolib/validators/validator_utils.py`

 * *Files identical despite different names*

### Comparing `pybiolib-1.1.940/pyproject.toml` & `pybiolib-1.1.944/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pybiolib"
-version = "1.1.940"
+version = "1.1.944"
 description = "BioLib Python Client"
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/biolib"
 keywords = ["biolib"]
 authors = [
     "biolib <hello@biolib.com>",
```

### Comparing `pybiolib-1.1.940/PKG-INFO` & `pybiolib-1.1.944/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybiolib
-Version: 1.1.940
+Version: 1.1.944
 Summary: BioLib Python Client
 Home-page: https://github.com/biolib
 License: MIT
 Keywords: biolib
 Author: biolib
 Author-email: hello@biolib.com
 Requires-Python: >=3.6.3,<4.0.0
```

