# Comparing `tmp/devopstestor-1.7.tar.gz` & `tmp/devopstestor-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devopstestor-1.7.tar", last modified: Fri Jun  2 12:37:33 2023, max compression
+gzip compressed data, was "devopstestor-1.7.1.tar", last modified: Mon Jun  5 10:46:39 2023, max compression
```

## Comparing `devopstestor-1.7.tar` & `devopstestor-1.7.1.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.742342 devopstestor-1.7/
--rw-rw-rw-   0 root         (0) root         (0)    22958 2023-06-02 12:37:23.000000 devopstestor-1.7/LICENCE
--rw-rw-rw-   0 root         (0) root         (0)      176 2023-06-02 12:37:23.000000 devopstestor-1.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      706 2023-06-02 12:37:33.742342 devopstestor-1.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      289 2023-06-02 12:37:23.000000 devopstestor-1.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.726342 devopstestor-1.7/devopstestor/
--rw-rw-rw-   0 root         (0) root         (0)      430 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.728342 devopstestor-1.7/devopstestor/config/
--rw-rw-rw-   0 root         (0) root         (0)     2837 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/config/arguments.yml
--rw-rw-rw-   0 root         (0) root         (0)      323 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/config/core.yml
--rw-rw-rw-   0 root         (0) root         (0)      778 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/config/machine.yml
--rw-rw-rw-   0 root         (0) root         (0)      353 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/config/provisionner.yml
--rw-rw-rw-   0 root         (0) root         (0)      568 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/config/report.yml
--rw-rw-rw-   0 root         (0) root         (0)     1584 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/config/source_manager.yml
--rw-rw-rw-   0 root         (0) root         (0)      829 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/config/testcase.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.728342 devopstestor-1.7/devopstestor/src/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.729342 devopstestor-1.7/devopstestor/src/abstract/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/abstract/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5424 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/abstract/abstract_machine_controller.py
--rw-rw-rw-   0 root         (0) root         (0)     1677 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/abstract/abstract_provisionner.py
--rw-rw-rw-   0 root         (0) root         (0)     3498 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/abstract/abstract_report.py
--rw-rw-rw-   0 root         (0) root         (0)      932 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/abstract/abstract_source_accessor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.731342 devopstestor-1.7/devopstestor/src/core/
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5789 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/core/devopstestor.py
--rw-rw-rw-   0 root         (0) root         (0)     1469 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/core/devopstestor_client.py
--rw-rw-rw-   0 root         (0) root         (0)     2230 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/core/devopstestor_server.py
--rw-rw-rw-   0 root         (0) root         (0)     8011 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/core/global_config_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     8219 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/core/machines_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     4851 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/core/ordonnanceur.py
--rw-rw-rw-   0 root         (0) root         (0)     2532 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/core/report_render_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     2083 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/core/source_manager.py
--rw-rw-rw-   0 root         (0) root         (0)      636 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/core/testcase_executor_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.732342 devopstestor-1.7/devopstestor/src/lib/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/lib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2808 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/lib/config.py
--rw-rw-rw-   0 root         (0) root         (0)     2539 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/lib/core_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1713 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/lib/json_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2719 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/lib/log_manager.py
--rw-rw-rw-   0 root         (0) root         (0)    11155 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/lib/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.732342 devopstestor-1.7/devopstestor/src/machine/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/machine/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2093 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/machine/debug_controller.py
--rw-rw-rw-   0 root         (0) root         (0)     7573 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/machine/docker_controller.py
--rw-rw-rw-   0 root         (0) root         (0)     3754 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/machine/local_controller.py
--rw-rw-rw-   0 root         (0) root         (0)     7560 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/machine/vagrant_controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.733342 devopstestor-1.7/devopstestor/src/provisionner/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/provisionner/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      743 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/provisionner/empty_provisionner.py
--rw-rw-rw-   0 root         (0) root         (0)     4850 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/provisionner/logstash_provisionner.py
--rw-rw-rw-   0 root         (0) root         (0)     8768 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/provisionner/minion_provisionner.py
--rw-rw-rw-   0 root         (0) root         (0)     4402 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/provisionner/systemd_provisionner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.735342 devopstestor-1.7/devopstestor/src/reporting/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/reporting/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      440 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/reporting/campaign_report.py
--rw-rw-rw-   0 root         (0) root         (0)      143 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/reporting/deployment_report.py
--rw-rw-rw-   0 root         (0) root         (0)     5666 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/reporting/report_elk_renderer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.735342 devopstestor-1.7/devopstestor/src/reporting/report_html_renderer/
--rw-rw-rw-   0 root         (0) root         (0)     1487 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/reporting/report_html_renderer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9223 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/reporting/report_html_renderer/html_template.html.jinja
--rw-rw-rw-   0 root         (0) root         (0)     7258 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/reporting/report_text_renderer.py
--rw-rw-rw-   0 root         (0) root         (0)      908 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/reporting/scenario_report.py
--rw-rw-rw-   0 root         (0) root         (0)      552 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/reporting/testcase_report.py
--rw-rw-rw-   0 root         (0) root         (0)     1110 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/reporting/verifier_report.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.736342 devopstestor-1.7/devopstestor/src/scenarios/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/scenarios/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      522 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/scenarios/devopstestor.py
--rw-rw-rw-   0 root         (0) root         (0)     1586 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/scenarios/logstash.py
--rw-rw-rw-   0 root         (0) root         (0)     6385 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/scenarios/mock_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1432 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/scenarios/systemd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.737342 devopstestor-1.7/devopstestor/src/sources/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/sources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2604 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/sources/copytemplate_source_accessor.py
--rw-rw-rw-   0 root         (0) root         (0)     2334 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/sources/dirlink_source_accessor.py
--rw-rw-rw-   0 root         (0) root         (0)     2587 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/sources/git_source_accessor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.738342 devopstestor-1.7/devopstestor/src/testcase/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/testcase/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8757 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/testcase/scenario_executor.py
--rw-rw-rw-   0 root         (0) root         (0)     6314 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/testcase/test_case.py
--rw-rw-rw-   0 root         (0) root         (0)     2539 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/testcase/testcase_executor.py
--rw-rw-rw-   0 root         (0) root         (0)     3114 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/src/testcase/tests_cases_loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.723342 devopstestor-1.7/devopstestor/testconf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.724342 devopstestor-1.7/devopstestor/testconf/verifiers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.738342 devopstestor-1.7/devopstestor/testconf/verifiers/fixtures/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/testconf/verifiers/fixtures/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1677 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/testconf/verifiers/fixtures/context_fixtures.py
--rw-rw-rw-   0 root         (0) root         (0)      332 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/testconf/verifiers/fixtures/logstash_fixtures.py
--rw-rw-rw-   0 root         (0) root         (0)     1437 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/testconf/verifiers/fixtures/saltstack_fixtures.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.739342 devopstestor-1.7/devopstestor/testconf/verifiers/service/
--rw-rw-rw-   0 root         (0) root         (0)     4529 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/testconf/verifiers/service/http_logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.739342 devopstestor-1.7/devopstestor/testconf/verifiers/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.739342 devopstestor-1.7/devopstestor/testconf/verifiers/tests/http_logger/
--rw-rw-rw-   0 root         (0) root         (0)     1317 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/testconf/verifiers/tests/http_logger/check_requests.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.739342 devopstestor-1.7/devopstestor/testconf/verifiers/tests/logstash/
--rw-rw-rw-   0 root         (0) root         (0)     5411 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/testconf/verifiers/tests/logstash/test_logstash_IO.py
--rw-rw-rw-   0 root         (0) root         (0)     1089 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/testconf/verifiers/tests/logstash/test_status_is_green.py
--rw-rw-rw-   0 root         (0) root         (0)       42 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/testconf/verifiers/tests/pytest.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.740342 devopstestor-1.7/devopstestor/testconf/verifiers/tests/system/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/testconf/verifiers/tests/system/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.740342 devopstestor-1.7/devopstestor/testconf/verifiers/tests/system/filesystem/
--rw-rw-rw-   0 root         (0) root         (0)     1581 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/testconf/verifiers/tests/system/filesystem/directories_are_present.py
--rw-rw-rw-   0 root         (0) root         (0)     1539 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/testconf/verifiers/tests/system/filesystem/files_are_present.py
--rw-rw-rw-   0 root         (0) root         (0)     1133 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/testconf/verifiers/tests/system/filesystem/symlinks_are_present.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.740342 devopstestor-1.7/devopstestor/testconf/verifiers/tests/system/packages/
--rw-rw-rw-   0 root         (0) root         (0)      776 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/testconf/verifiers/tests/system/packages/packages_are_present.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.741342 devopstestor-1.7/devopstestor/testconf/verifiers/tests/system/systemd/
--rw-rw-rw-   0 root         (0) root         (0)      720 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/testconf/verifiers/tests/system/systemd/service_is_down.py
--rw-rw-rw-   0 root         (0) root         (0)     2256 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/testconf/verifiers/tests/system/systemd/service_is_up.py
--rw-rw-rw-   0 root         (0) root         (0)     3336 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/testconf/verifiers/tests/system/systemd/services_are_up.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.741342 devopstestor-1.7/devopstestor/testconf/verifiers/tests/system/users/
--rw-rw-rw-   0 root         (0) root         (0)      826 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/testconf/verifiers/tests/system/users/users_are_present.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.741342 devopstestor-1.7/devopstestor/testconf/verifiers/utils/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.742342 devopstestor-1.7/devopstestor/testconf/verifiers/utils/logstash/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/testconf/verifiers/utils/logstash/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6214 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/testconf/verifiers/utils/logstash/logstash_manipulator.py
--rw-rw-rw-   0 root         (0) root         (0)     4964 2023-06-02 12:37:23.000000 devopstestor-1.7/devopstestor/testconf/verifiers/utils/verififier_luncher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:37:33.726342 devopstestor-1.7/devopstestor.egg-info/
--rw-r--r--   0 root         (0) root         (0)      706 2023-06-02 12:37:33.000000 devopstestor-1.7/devopstestor.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4372 2023-06-02 12:37:33.000000 devopstestor-1.7/devopstestor.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 12:37:33.000000 devopstestor-1.7/devopstestor.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       68 2023-06-02 12:37:33.000000 devopstestor-1.7/devopstestor.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-02 12:37:33.000000 devopstestor-1.7/devopstestor.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-02 12:37:33.742342 devopstestor-1.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1002 2023-06-02 12:37:23.000000 devopstestor-1.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.419587 devopstestor-1.7.1/
+-rw-rw-rw-   0 root         (0) root         (0)    22958 2023-06-05 10:46:29.000000 devopstestor-1.7.1/LICENCE
+-rw-rw-rw-   0 root         (0) root         (0)      176 2023-06-05 10:46:29.000000 devopstestor-1.7.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      708 2023-06-05 10:46:39.418587 devopstestor-1.7.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      289 2023-06-05 10:46:29.000000 devopstestor-1.7.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.399587 devopstestor-1.7.1/devopstestor/
+-rw-rw-rw-   0 root         (0) root         (0)      430 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.401587 devopstestor-1.7.1/devopstestor/config/
+-rw-rw-rw-   0 root         (0) root         (0)     2837 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/config/arguments.yml
+-rw-rw-rw-   0 root         (0) root         (0)      323 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/config/core.yml
+-rw-rw-rw-   0 root         (0) root         (0)      778 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/config/machine.yml
+-rw-rw-rw-   0 root         (0) root         (0)      353 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/config/provisionner.yml
+-rw-rw-rw-   0 root         (0) root         (0)      568 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/config/report.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1584 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/config/source_manager.yml
+-rw-rw-rw-   0 root         (0) root         (0)      829 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/config/testcase.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.401587 devopstestor-1.7.1/devopstestor/src/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.402587 devopstestor-1.7.1/devopstestor/src/abstract/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/abstract/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5424 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/abstract/abstract_machine_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)     1677 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/abstract/abstract_provisionner.py
+-rw-rw-rw-   0 root         (0) root         (0)     3498 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/abstract/abstract_report.py
+-rw-rw-rw-   0 root         (0) root         (0)      932 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/abstract/abstract_source_accessor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.404587 devopstestor-1.7.1/devopstestor/src/core/
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5789 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/core/devopstestor.py
+-rw-rw-rw-   0 root         (0) root         (0)     1469 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/core/devopstestor_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     2230 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/core/devopstestor_server.py
+-rw-rw-rw-   0 root         (0) root         (0)     8433 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/core/global_config_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     8219 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/core/machines_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     4851 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/core/ordonnanceur.py
+-rw-rw-rw-   0 root         (0) root         (0)     2532 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/core/report_render_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     2083 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/core/source_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)      636 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/core/testcase_executor_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.406587 devopstestor-1.7.1/devopstestor/src/lib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/lib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2835 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/lib/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2619 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/lib/core_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1713 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/lib/json_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2719 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/lib/log_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)    11155 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/lib/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.407587 devopstestor-1.7.1/devopstestor/src/machine/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/machine/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2093 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/machine/debug_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)     7573 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/machine/docker_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)     3754 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/machine/local_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)     7560 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/machine/vagrant_controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.408587 devopstestor-1.7.1/devopstestor/src/provisionner/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/provisionner/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      743 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/provisionner/empty_provisionner.py
+-rw-rw-rw-   0 root         (0) root         (0)     4850 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/provisionner/logstash_provisionner.py
+-rw-rw-rw-   0 root         (0) root         (0)     8768 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/provisionner/minion_provisionner.py
+-rw-rw-rw-   0 root         (0) root         (0)     4402 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/provisionner/systemd_provisionner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.409587 devopstestor-1.7.1/devopstestor/src/reporting/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/reporting/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      440 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/reporting/campaign_report.py
+-rw-rw-rw-   0 root         (0) root         (0)      143 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/reporting/deployment_report.py
+-rw-rw-rw-   0 root         (0) root         (0)     5666 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/reporting/report_elk_renderer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.410587 devopstestor-1.7.1/devopstestor/src/reporting/report_html_renderer/
+-rw-rw-rw-   0 root         (0) root         (0)     1487 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/reporting/report_html_renderer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9223 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/reporting/report_html_renderer/html_template.html.jinja
+-rw-rw-rw-   0 root         (0) root         (0)     7258 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/reporting/report_text_renderer.py
+-rw-rw-rw-   0 root         (0) root         (0)      908 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/reporting/scenario_report.py
+-rw-rw-rw-   0 root         (0) root         (0)      552 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/reporting/testcase_report.py
+-rw-rw-rw-   0 root         (0) root         (0)     1110 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/reporting/verifier_report.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.411587 devopstestor-1.7.1/devopstestor/src/scenarios/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/scenarios/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      522 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/scenarios/devopstestor.py
+-rw-rw-rw-   0 root         (0) root         (0)     1586 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/scenarios/logstash.py
+-rw-rw-rw-   0 root         (0) root         (0)     6385 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/scenarios/mock_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1432 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/scenarios/systemd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.411587 devopstestor-1.7.1/devopstestor/src/sources/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/sources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2604 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/sources/copytemplate_source_accessor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2334 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/sources/dirlink_source_accessor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2587 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/sources/git_source_accessor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.413587 devopstestor-1.7.1/devopstestor/src/testcase/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/testcase/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8757 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/testcase/scenario_executor.py
+-rw-rw-rw-   0 root         (0) root         (0)     6314 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/testcase/test_case.py
+-rw-rw-rw-   0 root         (0) root         (0)     2539 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/testcase/testcase_executor.py
+-rw-rw-rw-   0 root         (0) root         (0)     3114 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/src/testcase/tests_cases_loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.396587 devopstestor-1.7.1/devopstestor/testconf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.397587 devopstestor-1.7.1/devopstestor/testconf/verifiers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.414587 devopstestor-1.7.1/devopstestor/testconf/verifiers/fixtures/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/testconf/verifiers/fixtures/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1677 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/testconf/verifiers/fixtures/context_fixtures.py
+-rw-rw-rw-   0 root         (0) root         (0)      332 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/testconf/verifiers/fixtures/logstash_fixtures.py
+-rw-rw-rw-   0 root         (0) root         (0)     1437 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/testconf/verifiers/fixtures/saltstack_fixtures.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.414587 devopstestor-1.7.1/devopstestor/testconf/verifiers/service/
+-rw-rw-rw-   0 root         (0) root         (0)     4529 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/testconf/verifiers/service/http_logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.414587 devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.414587 devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/http_logger/
+-rw-rw-rw-   0 root         (0) root         (0)     1317 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/http_logger/check_requests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.415587 devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/logstash/
+-rw-rw-rw-   0 root         (0) root         (0)     5411 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/logstash/test_logstash_IO.py
+-rw-rw-rw-   0 root         (0) root         (0)     1089 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/logstash/test_status_is_green.py
+-rw-rw-rw-   0 root         (0) root         (0)       42 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/pytest.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.415587 devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/system/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/system/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.416587 devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/system/filesystem/
+-rw-rw-rw-   0 root         (0) root         (0)     1581 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/system/filesystem/directories_are_present.py
+-rw-rw-rw-   0 root         (0) root         (0)     1539 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/system/filesystem/files_are_present.py
+-rw-rw-rw-   0 root         (0) root         (0)     1133 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/system/filesystem/symlinks_are_present.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.416587 devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/system/packages/
+-rw-rw-rw-   0 root         (0) root         (0)      776 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/system/packages/packages_are_present.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.417587 devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/system/systemd/
+-rw-rw-rw-   0 root         (0) root         (0)      720 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/system/systemd/service_is_down.py
+-rw-rw-rw-   0 root         (0) root         (0)     2256 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/system/systemd/service_is_up.py
+-rw-rw-rw-   0 root         (0) root         (0)     3336 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/system/systemd/services_are_up.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.417587 devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/system/users/
+-rw-rw-rw-   0 root         (0) root         (0)      826 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/system/users/users_are_present.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.418587 devopstestor-1.7.1/devopstestor/testconf/verifiers/utils/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.418587 devopstestor-1.7.1/devopstestor/testconf/verifiers/utils/logstash/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/testconf/verifiers/utils/logstash/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6214 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/testconf/verifiers/utils/logstash/logstash_manipulator.py
+-rw-rw-rw-   0 root         (0) root         (0)     4964 2023-06-05 10:46:29.000000 devopstestor-1.7.1/devopstestor/testconf/verifiers/utils/verififier_luncher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:46:39.400587 devopstestor-1.7.1/devopstestor.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      708 2023-06-05 10:46:39.000000 devopstestor-1.7.1/devopstestor.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4372 2023-06-05 10:46:39.000000 devopstestor-1.7.1/devopstestor.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 10:46:39.000000 devopstestor-1.7.1/devopstestor.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       68 2023-06-05 10:46:39.000000 devopstestor-1.7.1/devopstestor.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-05 10:46:39.000000 devopstestor-1.7.1/devopstestor.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-05 10:46:39.419587 devopstestor-1.7.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1002 2023-06-05 10:46:29.000000 devopstestor-1.7.1/setup.py
```

### Comparing `devopstestor-1.7/LICENCE` & `devopstestor-1.7.1/LICENCE`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/PKG-INFO` & `devopstestor-1.7.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devopstestor
-Version: 1.7
+Version: 1.7.1
 Summary: Framwork to auto test machine provisioning
 Home-page: https://gitlab.com/alexis.porzier.pro/devopstestor
 Author: Alexis PORZIER
 Author-email: alexis.porzier.pro@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
```

### Comparing `devopstestor-1.7/devopstestor/config/arguments.yml` & `devopstestor-1.7.1/devopstestor/config/arguments.yml`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/config/machine.yml` & `devopstestor-1.7.1/devopstestor/config/machine.yml`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/config/report.yml` & `devopstestor-1.7.1/devopstestor/config/report.yml`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/config/source_manager.yml` & `devopstestor-1.7.1/devopstestor/config/source_manager.yml`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/config/testcase.yml` & `devopstestor-1.7.1/devopstestor/config/testcase.yml`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/src/abstract/abstract_machine_controller.py` & `devopstestor-1.7.1/devopstestor/src/abstract/abstract_machine_controller.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/src/abstract/abstract_provisionner.py` & `devopstestor-1.7.1/devopstestor/src/abstract/abstract_provisionner.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/src/abstract/abstract_report.py` & `devopstestor-1.7.1/devopstestor/src/abstract/abstract_report.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/src/abstract/abstract_source_accessor.py` & `devopstestor-1.7.1/devopstestor/src/abstract/abstract_source_accessor.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/src/core/devopstestor.py` & `devopstestor-1.7.1/devopstestor/src/core/devopstestor.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/src/core/devopstestor_client.py` & `devopstestor-1.7.1/devopstestor/src/core/devopstestor_client.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/src/core/devopstestor_server.py` & `devopstestor-1.7.1/devopstestor/src/core/devopstestor_server.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/src/core/global_config_factory.py` & `devopstestor-1.7.1/devopstestor/src/core/global_config_factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 
+from core_utils import get_global_path
 from glob import glob
 import os
 from log_manager import logging
 log = logging.getLogger('core.GlobalConfigLoader')
 from pathlib import Path
 import yaml
 import argparse
@@ -86,17 +87,20 @@
         :param lib_path: chemin global vers les sources du framwork
         :param client_path: chemin global vers le dossier de surcharge spcifique
         :param global_config_overload: dict de surcharge de la configuration global
         :param main_args: dict d'arguments comme defini dans la configuration "arguments::parameters"
         :return: un objet Config avec tous les elements
         """
         base_config = base_config.clone()
+        base_config.set('lib_path', lib_path, force=True)
+        base_config.set('client_path', client_path, force=True)
+
         log.debut('Chargement des configurations')
-        for path in [lib_path, client_path]:
-            path = path + '/config'
+        env_conf_dir_params = [get_global_path(global_config=base_config, relative_path=lpath) for lpath in os.environ['DEVOPSTESTOR_OTHER_CONF_DIRS'].split(':')] if os.getenv('DEVOPSTESTOR_OTHER_CONF_DIRS', '') != '' else []
+        for path in [os.path.join(lib_path, 'config'), os.path.join(client_path, 'config')] + env_conf_dir_params:
             for file in os.listdir(path):
                 file_path = path + "/" + file
                 node_name = Path(file).stem
                 if node_name in base_config.config:
                     # La config cote lib sert de valeur par defaut
                     base_config.config[node_name] = copy_merge_recursive_dict(defaut=base_config.config[node_name], source=yaml.load(open(file_path), Loader=yaml.Loader))
                 else:
```

### Comparing `devopstestor-1.7/devopstestor/src/core/machines_factory.py` & `devopstestor-1.7.1/devopstestor/src/core/machines_factory.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/src/core/ordonnanceur.py` & `devopstestor-1.7.1/devopstestor/src/core/ordonnanceur.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/src/core/report_render_manager.py` & `devopstestor-1.7.1/devopstestor/src/core/report_render_manager.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/src/core/source_manager.py` & `devopstestor-1.7.1/devopstestor/src/core/source_manager.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/src/core/testcase_executor_factory.py` & `devopstestor-1.7.1/devopstestor/src/core/testcase_executor_factory.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/src/lib/config.py` & `devopstestor-1.7.1/devopstestor/src/lib/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
     def items(self):
         """
         Permet d'iterer sur le noeud
         """
         return list(self.config.items())
 
-    def set(self, name, value):
+    def set(self, name, value, force=False):
         """
         Set value to config
         """
-        if not self.exist(name):
+        if not force and not self.exist(name):
             raise Exception(f"Config error, cannot change config {name} : not exist")
         self.flat_config[name] = value
         self.config = flat_dict_to_nested_dict_with_array(self.flat_config, separator="::")
```

### Comparing `devopstestor-1.7/devopstestor/src/lib/core_utils.py` & `devopstestor-1.7.1/devopstestor/src/lib/core_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -49,27 +49,29 @@
     Instancie la classe dont le nom est passe en parametre
     :param class_name: Nom de la classe a instancier
     :param args: arguments a passer au constructeur
     :return: instance de la classe correspondante
     """
     return getattr(__import__(get_module_name(class_name)), class_name)(**args)
 
-def get_global_path(global_config, relative_path):
+def get_global_path(global_config, in_path):
     """
     Recherche un fichier ou dossier
     :param global_config: instance de configuration global
-    :param relative_path: chemin relatif du fichier a importer
+    :param in_path: chemin a convertir
     :return: chemin absolu si existant
     """
+    if os.path.isabs(in_path) and os.path.exists(in_path):
+        return in_path  # Le chemin existe deja, il est absolu
     rel_base_paths = [global_config.get('client_path'), global_config.get('lib_path')]
     for base_path in rel_base_paths:
-        test_path = os.path.join(base_path, relative_path)
+        test_path = os.path.join(base_path, in_path)
         if os.path.exists(test_path):
             return test_path
-    raise Exception('file {} not found'.format(relative_path))
+    raise Exception('file {} not found'.format(in_path))
 
 def import_py_file(global_config, relative_path):
     """
     Importe un fichier python selon son chemin relatif
     Le fichier est d'abords recuperer cote client, puis cote framwork
     :param global_config: instance de configuration global
     :param relative_path: chemin relatif du fichier a importer
```

### Comparing `devopstestor-1.7/devopstestor/src/lib/json_utils.py` & `devopstestor-1.7.1/devopstestor/src/lib/json_utils.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/src/lib/log_manager.py` & `devopstestor-1.7.1/devopstestor/src/lib/log_manager.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/src/lib/utils.py` & `devopstestor-1.7.1/devopstestor/src/lib/utils.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/src/machine/debug_controller.py` & `devopstestor-1.7.1/devopstestor/src/machine/debug_controller.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/src/machine/docker_controller.py` & `devopstestor-1.7.1/devopstestor/src/machine/docker_controller.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/src/machine/local_controller.py` & `devopstestor-1.7.1/devopstestor/src/machine/local_controller.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/src/machine/vagrant_controller.py` & `devopstestor-1.7.1/devopstestor/src/machine/vagrant_controller.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/src/provisionner/empty_provisionner.py` & `devopstestor-1.7.1/devopstestor/src/provisionner/empty_provisionner.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/src/provisionner/logstash_provisionner.py` & `devopstestor-1.7.1/devopstestor/src/provisionner/logstash_provisionner.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/src/provisionner/minion_provisionner.py` & `devopstestor-1.7.1/devopstestor/src/provisionner/minion_provisionner.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/src/provisionner/systemd_provisionner.py` & `devopstestor-1.7.1/devopstestor/src/provisionner/systemd_provisionner.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/src/reporting/report_elk_renderer.py` & `devopstestor-1.7.1/devopstestor/src/reporting/report_elk_renderer.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/src/reporting/report_html_renderer/__init__.py` & `devopstestor-1.7.1/devopstestor/src/reporting/report_html_renderer/__init__.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/src/reporting/report_html_renderer/html_template.html.jinja` & `devopstestor-1.7.1/devopstestor/src/reporting/report_html_renderer/html_template.html.jinja`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/src/reporting/report_text_renderer.py` & `devopstestor-1.7.1/devopstestor/src/reporting/report_text_renderer.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/src/reporting/scenario_report.py` & `devopstestor-1.7.1/devopstestor/src/reporting/scenario_report.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/src/reporting/testcase_report.py` & `devopstestor-1.7.1/devopstestor/src/reporting/testcase_report.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/src/reporting/verifier_report.py` & `devopstestor-1.7.1/devopstestor/src/reporting/verifier_report.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/src/scenarios/devopstestor.py` & `devopstestor-1.7.1/devopstestor/src/scenarios/devopstestor.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/src/scenarios/logstash.py` & `devopstestor-1.7.1/devopstestor/src/scenarios/logstash.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/src/scenarios/mock_utils.py` & `devopstestor-1.7.1/devopstestor/src/scenarios/mock_utils.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/src/scenarios/systemd.py` & `devopstestor-1.7.1/devopstestor/src/scenarios/systemd.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/src/sources/copytemplate_source_accessor.py` & `devopstestor-1.7.1/devopstestor/src/sources/copytemplate_source_accessor.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/src/sources/dirlink_source_accessor.py` & `devopstestor-1.7.1/devopstestor/src/sources/dirlink_source_accessor.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/src/sources/git_source_accessor.py` & `devopstestor-1.7.1/devopstestor/src/sources/git_source_accessor.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/src/testcase/scenario_executor.py` & `devopstestor-1.7.1/devopstestor/src/testcase/scenario_executor.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/src/testcase/test_case.py` & `devopstestor-1.7.1/devopstestor/src/testcase/test_case.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/src/testcase/testcase_executor.py` & `devopstestor-1.7.1/devopstestor/src/testcase/testcase_executor.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/src/testcase/tests_cases_loader.py` & `devopstestor-1.7.1/devopstestor/src/testcase/tests_cases_loader.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/testconf/verifiers/fixtures/context_fixtures.py` & `devopstestor-1.7.1/devopstestor/testconf/verifiers/fixtures/context_fixtures.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/testconf/verifiers/fixtures/saltstack_fixtures.py` & `devopstestor-1.7.1/devopstestor/testconf/verifiers/fixtures/saltstack_fixtures.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/testconf/verifiers/service/http_logger.py` & `devopstestor-1.7.1/devopstestor/testconf/verifiers/service/http_logger.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/testconf/verifiers/tests/http_logger/check_requests.py` & `devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/http_logger/check_requests.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/testconf/verifiers/tests/logstash/test_logstash_IO.py` & `devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/logstash/test_logstash_IO.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/testconf/verifiers/tests/logstash/test_status_is_green.py` & `devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/logstash/test_status_is_green.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/testconf/verifiers/tests/system/filesystem/directories_are_present.py` & `devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/system/filesystem/directories_are_present.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/testconf/verifiers/tests/system/filesystem/files_are_present.py` & `devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/system/filesystem/files_are_present.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/testconf/verifiers/tests/system/filesystem/symlinks_are_present.py` & `devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/system/filesystem/symlinks_are_present.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/testconf/verifiers/tests/system/packages/packages_are_present.py` & `devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/system/packages/packages_are_present.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/testconf/verifiers/tests/system/systemd/service_is_down.py` & `devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/system/systemd/service_is_down.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/testconf/verifiers/tests/system/systemd/service_is_up.py` & `devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/system/systemd/service_is_up.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/testconf/verifiers/tests/system/systemd/services_are_up.py` & `devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/system/systemd/services_are_up.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/testconf/verifiers/tests/system/users/users_are_present.py` & `devopstestor-1.7.1/devopstestor/testconf/verifiers/tests/system/users/users_are_present.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/testconf/verifiers/utils/logstash/logstash_manipulator.py` & `devopstestor-1.7.1/devopstestor/testconf/verifiers/utils/logstash/logstash_manipulator.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor/testconf/verifiers/utils/verififier_luncher.py` & `devopstestor-1.7.1/devopstestor/testconf/verifiers/utils/verififier_luncher.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/devopstestor.egg-info/PKG-INFO` & `devopstestor-1.7.1/devopstestor.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devopstestor
-Version: 1.7
+Version: 1.7.1
 Summary: Framwork to auto test machine provisioning
 Home-page: https://gitlab.com/alexis.porzier.pro/devopstestor
 Author: Alexis PORZIER
 Author-email: alexis.porzier.pro@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
```

### Comparing `devopstestor-1.7/devopstestor.egg-info/SOURCES.txt` & `devopstestor-1.7.1/devopstestor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `devopstestor-1.7/setup.py` & `devopstestor-1.7.1/setup.py`

 * *Files identical despite different names*

