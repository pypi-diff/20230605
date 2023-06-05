# Comparing `tmp/netbox-validity-1.2.1.tar.gz` & `tmp/netbox-validity-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-validity-1.2.1.tar", last modified: Thu May 25 19:54:24 2023, max compression
+gzip compressed data, was "netbox-validity-1.3.0.tar", last modified: Mon Jun  5 21:12:16 2023, max compression
```

## Comparing `netbox-validity-1.2.1.tar` & `netbox-validity-1.3.0.tar`

### file list

```diff
@@ -1,139 +1,142 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:24.473896 netbox-validity-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-05-25 19:54:24.473896 netbox-validity-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:24.453896 netbox-validity-1.2.1/netbox_validity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-05-25 19:54:24.000000 netbox-validity-1.2.1/netbox_validity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-05-25 19:54:24.000000 netbox-validity-1.2.1/netbox_validity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 19:54:24.000000 netbox-validity-1.2.1/netbox_validity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-25 19:54:24.000000 netbox-validity-1.2.1/netbox_validity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-25 19:54:24.000000 netbox-validity-1.2.1/netbox_validity.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:24.453896 netbox-validity-1.2.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 19:54:24.473896 netbox-validity-1.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:24.457896 netbox-validity-1.2.1/validity/
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:24.457896 netbox-validity-1.2.1/validity/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/api/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9744 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/choices.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:24.457896 netbox-validity-1.2.1/validity/config_compliance/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:24.457896 netbox-validity-1.2.1/validity/config_compliance/device_config/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/config_compliance/device_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/config_compliance/device_config/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/config_compliance/device_config/routeros.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/config_compliance/device_config/ttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/config_compliance/device_config/yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/config_compliance/dynamic_pairs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:24.461896 netbox-validity-1.2.1/validity/config_compliance/eval/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/config_compliance/eval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/config_compliance/eval/default_nameset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/config_compliance/eval/eval.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/config_compliance/eval/eval_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/config_compliance/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/filtersets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:24.461896 netbox-validity-1.2.1/validity/forms/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/forms/filterset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/forms/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/forms/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/graphql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:24.461896 netbox-validity-1.2.1/validity/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:24.461896 netbox-validity-1.2.1/validity/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/management/commands/linkscripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/managers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:24.461896 netbox-validity-1.2.1/validity/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    12486 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/migrations/0002_custom_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/migrations/0003_complianceselector_dp_tag_prefix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/migrations/0004_netbox35_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:24.465896 netbox-validity-1.2.1/validity/models/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/models/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/models/nameset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/models/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/models/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/models/selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/models/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/models/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/models/test_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/navigation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:24.465896 netbox-validity-1.2.1/validity/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/scripts/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/scripts/run_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/scripts/validity_git.py
--rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/scripts/validity_run_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:24.449896 netbox-validity-1.2.1/validity/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:24.465896 netbox-validity-1.2.1/validity/templates/validity/
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/templates/validity/compliance_results.html
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/templates/validity/compliancereport.html
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/templates/validity/complianceselector.html
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/templates/validity/compliancetest.html
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/templates/validity/compliancetestresult.html
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/templates/validity/configserializer.html
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/templates/validity/device_config.html
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/templates/validity/gitrepo.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:24.465896 netbox-validity-1.2.1/validity/templates/validity/inc/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/templates/validity/inc/git_link.html
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/templates/validity/inc/path_with_link.html
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/templates/validity/inc/report_stats_row.html
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/templates/validity/inc/search_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/templates/validity/nameset.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:24.469896 netbox-validity-1.2.1/validity/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/templatetags/validity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:24.469896 netbox-validity-1.2.1/validity/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/tests/test_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:24.469896 netbox-validity-1.2.1/validity/tests/test_config_compliance/
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/tests/test_config_compliance/test_device_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/tests/test_config_compliance/test_dynamic_pairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/tests/test_config_compliance/test_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/tests/test_graphql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:24.469896 netbox-validity-1.2.1/validity/tests/test_models/
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/tests/test_models/test_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/tests/test_models/test_git_link.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/tests/test_models/test_git_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/tests/test_models/test_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/tests/test_models/test_vdevice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:24.473896 netbox-validity-1.2.1/validity/tests/test_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/tests/test_scripts/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6804 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/tests/test_scripts/test_run_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:24.473896 netbox-validity-1.2.1/validity/tests/test_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/tests/test_utils/test_git.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/tests/test_utils/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:24.473896 netbox-validity-1.2.1/validity/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/utils/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/utils/password.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:24.473896 netbox-validity-1.2.1/validity/views/
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/views/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/views/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/views/git_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/views/nameset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/views/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/views/selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/views/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/views/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/views/test_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:16.610605 netbox-validity-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-06-05 21:12:16.610605 netbox-validity-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:16.594604 netbox-validity-1.3.0/netbox_validity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-06-05 21:12:16.000000 netbox-validity-1.3.0/netbox_validity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-06-05 21:12:16.000000 netbox-validity-1.3.0/netbox_validity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 21:12:16.000000 netbox-validity-1.3.0/netbox_validity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-05 21:12:16.000000 netbox-validity-1.3.0/netbox_validity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-05 21:12:16.000000 netbox-validity-1.3.0/netbox_validity.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:16.598604 netbox-validity-1.3.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 21:12:16.610605 netbox-validity-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:16.598604 netbox-validity-1.3.0/validity/
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:16.598604 netbox-validity-1.3.0/validity/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/api/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10318 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/choices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:16.598604 netbox-validity-1.3.0/validity/config_compliance/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:16.598604 netbox-validity-1.3.0/validity/config_compliance/device_config/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/config_compliance/device_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/config_compliance/device_config/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/config_compliance/device_config/routeros.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/config_compliance/device_config/ttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/config_compliance/device_config/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/config_compliance/dynamic_pairs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:16.598604 netbox-validity-1.3.0/validity/config_compliance/eval/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/config_compliance/eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/config_compliance/eval/default_nameset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/config_compliance/eval/eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/config_compliance/eval/eval_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/config_compliance/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/filtersets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:16.602604 netbox-validity-1.3.0/validity/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/forms/filterset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/forms/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/forms/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/graphql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:16.602604 netbox-validity-1.3.0/validity/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:16.602604 netbox-validity-1.3.0/validity/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/management/commands/linkscripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/managers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:16.602604 netbox-validity-1.3.0/validity/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    12705 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/migrations/0002_custom_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/migrations/0003_complianceselector_dp_tag_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/migrations/0004_netbox35_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:16.602604 netbox-validity-1.3.0/validity/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/models/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/models/nameset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/models/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/models/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/models/selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/models/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/models/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/models/test_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/navigation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:16.602604 netbox-validity-1.3.0/validity/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/scripts/validity_git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/scripts/validity_run_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9786 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:16.594604 netbox-validity-1.3.0/validity/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:16.606604 netbox-validity-1.3.0/validity/templates/validity/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/templates/validity/aux_tab_table.html
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/templates/validity/compliance_results.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/templates/validity/compliancereport.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/templates/validity/complianceselector.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/templates/validity/compliancetest.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/templates/validity/compliancetestresult.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/templates/validity/configserializer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/templates/validity/device_config.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/templates/validity/gitrepo.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:16.606604 netbox-validity-1.3.0/validity/templates/validity/inc/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/templates/validity/inc/git_link.html
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/templates/validity/inc/path_with_link.html
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/templates/validity/inc/prism.html
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/templates/validity/inc/report_stats_row.html
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/templates/validity/inc/search_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/templates/validity/nameset.html
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/templates/validity/report_devices.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:16.606604 netbox-validity-1.3.0/validity/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/templatetags/validity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:16.606604 netbox-validity-1.3.0/validity/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/tests/test_choices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:16.606604 netbox-validity-1.3.0/validity/tests/test_config_compliance/
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/tests/test_config_compliance/test_device_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/tests/test_config_compliance/test_dynamic_pairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/tests/test_config_compliance/test_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/tests/test_graphql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:16.606604 netbox-validity-1.3.0/validity/tests/test_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/tests/test_models/test_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/tests/test_models/test_git_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/tests/test_models/test_git_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/tests/test_models/test_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/tests/test_models/test_vdevice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:16.606604 netbox-validity-1.3.0/validity/tests/test_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/tests/test_scripts/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6804 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/tests/test_scripts/test_run_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:16.606604 netbox-validity-1.3.0/validity/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/tests/test_utils/test_git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/tests/test_utils/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:16.606604 netbox-validity-1.3.0/validity/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/utils/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/utils/password.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:12:16.610605 netbox-validity-1.3.0/validity/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/views/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/views/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/views/git_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/views/nameset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/views/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/views/selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/views/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/views/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-06-05 21:12:03.000000 netbox-validity-1.3.0/validity/views/test_result.py
```

### Comparing `netbox-validity-1.2.1/LICENSE` & `netbox-validity-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.1/PKG-INFO` & `netbox-validity-1.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-validity
-Version: 1.2.1
+Version: 1.3.0
 Summary: NetBox plugin for vendor-agnostic configuration compliance
 Author-email: Anton Miasnikov <anton2008m@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Anton Miasnikov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -43,15 +43,15 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE
 
 <div align="center">
-    <a href="https://validity.readthedocs.io"><img src="https://raw.githubusercontent.com/amyasnikov/validity/master/docs/validity_logo.png" alt="Click to view Validity docs"/></a>
+    <a href="https://validity.readthedocs.io"><img src="https://raw.githubusercontent.com/amyasnikov/validity/master/docs/images/validity_logo.png" alt="Click to view Validity docs"/></a>
     <h1>Validity: vendor-agnostic configuration compliance</h1>
     <p>
         <img src="https://github.com/amyasnikov/validity/actions/workflows/ci.yml/badge.svg" alt="CI">
         <img src="https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/amyasnikov/9e518ae8babd18b7edd8ee5aad58146b/raw/cov.json" alt="Coverage">
         <img src="https://img.shields.io/badge/Python-3.10+-blue.svg" alt="Python version">
         <img src="https://img.shields.io/badge/NetBox-3.4|3.5-blue.svg" alt="NetBox version">
     </p>
@@ -101,14 +101,25 @@
 
 ## Documentation
 Read the full documentation on [validity.readthedocs.io](https://validity.readthedocs.io)
 
 
 ## Quick Start
 
-The short video about first steps with Validity:
+A short video about first steps with Validity:
 
 [![Watch the video](https://img.youtube.com/vi/Hs2IUE6rKC4/0.jpg)](https://youtu.be/Hs2IUE6rKC4)
 
+
 ## Contributing
 
 Feel free to ask a [Question](https://github.com/amyasnikov/validity/discussions), report an [Issue](https://github.com/amyasnikov/validity/issues) or even make a [PR](CONTRIBUTING.md). Read more about contribution in the [CONTRIBUTING](CONTRIBUTING.md) guide.
+
+## Screenshots
+
+![Report Per Device](docs/images/screen_report.png)
+
+![Compliance Test](docs/images/screen_test.png)
+
+![Compliance Test Result](docs/images/screen_result.png)
+
+![Device Serialized Configuration](docs/images/screen_config.png)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: netbox-validity Version: 1.2.1 Summary: NetBox
+Metadata-Version: 2.1 Name: netbox-validity Version: 1.3.0 Summary: NetBox
 plugin for vendor-agnostic configuration compliance Author-email: Anton
 Miasnikov
 gmail.com> License: MIT License Copyright (c) 2023 Anton Miasnikov Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
@@ -72,14 +72,18 @@
 generated. * **Test extensibility**. You can define your own python functions
 or classes to reuse the code between multiple compliance tests. * Possibility
 to store all heavy text-based entities (like compliance tests or TTP Templates)
 in a **Git repository** ## Download and Install You can download Validity via
 **pip** ``` pip install netbox-validity ``` After that follow the [installation
 guide](https://validity.readthedocs.io/en/latest/installation/) to correctly
 add Validity to your NetBox.  ## Documentation Read the full documentation on
-[validity.readthedocs.io](https://validity.readthedocs.io) ## Quick Start The
+[validity.readthedocs.io](https://validity.readthedocs.io) ## Quick Start A
 short video about first steps with Validity: [![Watch the video](https://
 img.youtube.com/vi/Hs2IUE6rKC4/0.jpg)](https://youtu.be/Hs2IUE6rKC4) ##
 Contributing Feel free to ask a [Question](https://github.com/amyasnikov/
 validity/discussions), report an [Issue](https://github.com/amyasnikov/
 validity/issues) or even make a [PR](CONTRIBUTING.md). Read more about
-contribution in the [CONTRIBUTING](CONTRIBUTING.md) guide.
+contribution in the [CONTRIBUTING](CONTRIBUTING.md) guide. ## Screenshots !
+[Report Per Device](docs/images/screen_report.png) ![Compliance Test](docs/
+images/screen_test.png) ![Compliance Test Result](docs/images/
+screen_result.png) ![Device Serialized Configuration](docs/images/
+screen_config.png)
```

### Comparing `netbox-validity-1.2.1/README.md` & `netbox-validity-1.3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <div align="center">
-    <a href="https://validity.readthedocs.io"><img src="https://raw.githubusercontent.com/amyasnikov/validity/master/docs/validity_logo.png" alt="Click to view Validity docs"/></a>
+    <a href="https://validity.readthedocs.io"><img src="https://raw.githubusercontent.com/amyasnikov/validity/master/docs/images/validity_logo.png" alt="Click to view Validity docs"/></a>
     <h1>Validity: vendor-agnostic configuration compliance</h1>
     <p>
         <img src="https://github.com/amyasnikov/validity/actions/workflows/ci.yml/badge.svg" alt="CI">
         <img src="https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/amyasnikov/9e518ae8babd18b7edd8ee5aad58146b/raw/cov.json" alt="Coverage">
         <img src="https://img.shields.io/badge/Python-3.10+-blue.svg" alt="Python version">
         <img src="https://img.shields.io/badge/NetBox-3.4|3.5-blue.svg" alt="NetBox version">
     </p>
@@ -53,14 +53,25 @@
 
 ## Documentation
 Read the full documentation on [validity.readthedocs.io](https://validity.readthedocs.io)
 
 
 ## Quick Start
 
-The short video about first steps with Validity:
+A short video about first steps with Validity:
 
 [![Watch the video](https://img.youtube.com/vi/Hs2IUE6rKC4/0.jpg)](https://youtu.be/Hs2IUE6rKC4)
 
+
 ## Contributing
 
 Feel free to ask a [Question](https://github.com/amyasnikov/validity/discussions), report an [Issue](https://github.com/amyasnikov/validity/issues) or even make a [PR](CONTRIBUTING.md). Read more about contribution in the [CONTRIBUTING](CONTRIBUTING.md) guide.
+
+## Screenshots
+
+![Report Per Device](docs/images/screen_report.png)
+
+![Compliance Test](docs/images/screen_test.png)
+
+![Compliance Test Result](docs/images/screen_result.png)
+
+![Device Serialized Configuration](docs/images/screen_config.png)
```

#### html2text {}

```diff
@@ -43,14 +43,18 @@
 generated. * **Test extensibility**. You can define your own python functions
 or classes to reuse the code between multiple compliance tests. * Possibility
 to store all heavy text-based entities (like compliance tests or TTP Templates)
 in a **Git repository** ## Download and Install You can download Validity via
 **pip** ``` pip install netbox-validity ``` After that follow the [installation
 guide](https://validity.readthedocs.io/en/latest/installation/) to correctly
 add Validity to your NetBox.  ## Documentation Read the full documentation on
-[validity.readthedocs.io](https://validity.readthedocs.io) ## Quick Start The
+[validity.readthedocs.io](https://validity.readthedocs.io) ## Quick Start A
 short video about first steps with Validity: [![Watch the video](https://
 img.youtube.com/vi/Hs2IUE6rKC4/0.jpg)](https://youtu.be/Hs2IUE6rKC4) ##
 Contributing Feel free to ask a [Question](https://github.com/amyasnikov/
 validity/discussions), report an [Issue](https://github.com/amyasnikov/
 validity/issues) or even make a [PR](CONTRIBUTING.md). Read more about
-contribution in the [CONTRIBUTING](CONTRIBUTING.md) guide.
+contribution in the [CONTRIBUTING](CONTRIBUTING.md) guide. ## Screenshots !
+[Report Per Device](docs/images/screen_report.png) ![Compliance Test](docs/
+images/screen_test.png) ![Compliance Test Result](docs/images/
+screen_result.png) ![Device Serialized Configuration](docs/images/
+screen_config.png)
```

### Comparing `netbox-validity-1.2.1/netbox_validity.egg-info/PKG-INFO` & `netbox-validity-1.3.0/netbox_validity.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-validity
-Version: 1.2.1
+Version: 1.3.0
 Summary: NetBox plugin for vendor-agnostic configuration compliance
 Author-email: Anton Miasnikov <anton2008m@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Anton Miasnikov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -43,15 +43,15 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE
 
 <div align="center">
-    <a href="https://validity.readthedocs.io"><img src="https://raw.githubusercontent.com/amyasnikov/validity/master/docs/validity_logo.png" alt="Click to view Validity docs"/></a>
+    <a href="https://validity.readthedocs.io"><img src="https://raw.githubusercontent.com/amyasnikov/validity/master/docs/images/validity_logo.png" alt="Click to view Validity docs"/></a>
     <h1>Validity: vendor-agnostic configuration compliance</h1>
     <p>
         <img src="https://github.com/amyasnikov/validity/actions/workflows/ci.yml/badge.svg" alt="CI">
         <img src="https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/amyasnikov/9e518ae8babd18b7edd8ee5aad58146b/raw/cov.json" alt="Coverage">
         <img src="https://img.shields.io/badge/Python-3.10+-blue.svg" alt="Python version">
         <img src="https://img.shields.io/badge/NetBox-3.4|3.5-blue.svg" alt="NetBox version">
     </p>
@@ -101,14 +101,25 @@
 
 ## Documentation
 Read the full documentation on [validity.readthedocs.io](https://validity.readthedocs.io)
 
 
 ## Quick Start
 
-The short video about first steps with Validity:
+A short video about first steps with Validity:
 
 [![Watch the video](https://img.youtube.com/vi/Hs2IUE6rKC4/0.jpg)](https://youtu.be/Hs2IUE6rKC4)
 
+
 ## Contributing
 
 Feel free to ask a [Question](https://github.com/amyasnikov/validity/discussions), report an [Issue](https://github.com/amyasnikov/validity/issues) or even make a [PR](CONTRIBUTING.md). Read more about contribution in the [CONTRIBUTING](CONTRIBUTING.md) guide.
+
+## Screenshots
+
+![Report Per Device](docs/images/screen_report.png)
+
+![Compliance Test](docs/images/screen_test.png)
+
+![Compliance Test Result](docs/images/screen_result.png)
+
+![Device Serialized Configuration](docs/images/screen_config.png)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: netbox-validity Version: 1.2.1 Summary: NetBox
+Metadata-Version: 2.1 Name: netbox-validity Version: 1.3.0 Summary: NetBox
 plugin for vendor-agnostic configuration compliance Author-email: Anton
 Miasnikov
 gmail.com> License: MIT License Copyright (c) 2023 Anton Miasnikov Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
@@ -72,14 +72,18 @@
 generated. * **Test extensibility**. You can define your own python functions
 or classes to reuse the code between multiple compliance tests. * Possibility
 to store all heavy text-based entities (like compliance tests or TTP Templates)
 in a **Git repository** ## Download and Install You can download Validity via
 **pip** ``` pip install netbox-validity ``` After that follow the [installation
 guide](https://validity.readthedocs.io/en/latest/installation/) to correctly
 add Validity to your NetBox.  ## Documentation Read the full documentation on
-[validity.readthedocs.io](https://validity.readthedocs.io) ## Quick Start The
+[validity.readthedocs.io](https://validity.readthedocs.io) ## Quick Start A
 short video about first steps with Validity: [![Watch the video](https://
 img.youtube.com/vi/Hs2IUE6rKC4/0.jpg)](https://youtu.be/Hs2IUE6rKC4) ##
 Contributing Feel free to ask a [Question](https://github.com/amyasnikov/
 validity/discussions), report an [Issue](https://github.com/amyasnikov/
 validity/issues) or even make a [PR](CONTRIBUTING.md). Read more about
-contribution in the [CONTRIBUTING](CONTRIBUTING.md) guide.
+contribution in the [CONTRIBUTING](CONTRIBUTING.md) guide. ## Screenshots !
+[Report Per Device](docs/images/screen_report.png) ![Compliance Test](docs/
+images/screen_test.png) ![Compliance Test Result](docs/images/
+screen_result.png) ![Device Serialized Configuration](docs/images/
+screen_config.png)
```

### Comparing `netbox-validity-1.2.1/netbox_validity.egg-info/SOURCES.txt` & `netbox-validity-1.3.0/netbox_validity.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 netbox_validity.egg-info/dependency_links.txt
 netbox_validity.egg-info/requires.txt
 netbox_validity.egg-info/top_level.txt
 requirements/base.txt
 requirements/dev.txt
 requirements/docs.txt
 validity/__init__.py
+validity/admin.py
 validity/choices.py
 validity/filtersets.py
 validity/graphql.py
 validity/managers.py
 validity/navigation.py
 validity/search.py
 validity/tables.py
@@ -54,37 +55,39 @@
 validity/models/repo.py
 validity/models/report.py
 validity/models/selector.py
 validity/models/serializer.py
 validity/models/test.py
 validity/models/test_result.py
 validity/scripts/__init__.py
-validity/scripts/git.py
-validity/scripts/run_tests.py
 validity/scripts/validity_git.py
 validity/scripts/validity_run_tests.py
+validity/templates/validity/aux_tab_table.html
 validity/templates/validity/compliance_results.html
 validity/templates/validity/compliancereport.html
 validity/templates/validity/complianceselector.html
 validity/templates/validity/compliancetest.html
 validity/templates/validity/compliancetestresult.html
 validity/templates/validity/configserializer.html
 validity/templates/validity/device_config.html
 validity/templates/validity/gitrepo.html
 validity/templates/validity/nameset.html
+validity/templates/validity/report_devices.html
 validity/templates/validity/inc/git_link.html
 validity/templates/validity/inc/path_with_link.html
+validity/templates/validity/inc/prism.html
 validity/templates/validity/inc/report_stats_row.html
 validity/templates/validity/inc/search_form.html
 validity/templatetags/__init__.py
 validity/templatetags/validity.py
 validity/tests/base.py
 validity/tests/conftest.py
 validity/tests/factories.py
 validity/tests/test_api.py
+validity/tests/test_choices.py
 validity/tests/test_graphql.py
 validity/tests/test_version.py
 validity/tests/test_views.py
 validity/tests/test_config_compliance/test_device_config.py
 validity/tests/test_config_compliance/test_dynamic_pairs.py
 validity/tests/test_config_compliance/test_eval.py
 validity/tests/test_models/test_clean.py
```

### Comparing `netbox-validity-1.2.1/pyproject.toml` & `netbox-validity-1.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "netbox-validity"
-version = "1.2.1"
+version = "1.3.0"
 description = "NetBox plugin for vendor-agnostic configuration compliance"
 authors = [
     {name = "Anton Miasnikov", email = "anton2008m@gmail.com"},
 ]
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `netbox-validity-1.2.1/validity/__init__.py` & `netbox-validity-1.3.0/validity/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 class NetBoxValidityConfig(PluginConfig):
     name = "validity"
     verbose_name = "Validity: Configuration Compliance"
     description = "Vendor-agnostic framework to build your own configuration compliance rule set"
     author = "Anton Miasnikov"
     author_email = "anton2008m@gmail.com"
-    version = "1.2.1"
+    version = "1.3.0"
     base_url = "validity"
     django_apps = ["bootstrap5"]
     min_version = "3.4.0"
 
     # custom field
     netbox_version = NetboxVersion(VERSION)
```

### Comparing `netbox-validity-1.2.1/validity/api/helpers.py` & `netbox-validity-1.3.0/validity/api/helpers.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.1/validity/api/serializers.py` & `netbox-validity-1.3.0/validity/api/serializers.py`

 * *Files 4% similar despite different names*

```diff
@@ -291,7 +291,24 @@
     repo = NestedGitRepoSerializer(read_only=True, source="device.repo")
     local_copy_last_updated = serializers.DateTimeField(allow_null=True, source="last_modified")
     config_web_link = serializers.SerializerMethodField()
     serialized_config = serializers.JSONField(source="serialized")
 
     def get_config_web_link(self, obj):
         return urljoin(obj.device.repo.web_url, obj.config_path.as_posix())
+
+
+class DeviceReportSerializer(NestedDeviceSerializer):
+    compliance_passed = serializers.BooleanField()
+    results_passed = serializers.IntegerField()
+    results_count = serializers.IntegerField()
+    results = SerializedPKRelatedField(
+        serializer=NestedComplianceTestResultSerializer, many=True, required=False, read_only=True
+    )
+
+    class Meta(NestedDeviceSerializer.Meta):
+        fields = NestedDeviceSerializer.Meta.fields + [
+            "compliance_passed",
+            "results_passed",
+            "results_count",
+            "results",
+        ]
```

### Comparing `netbox-validity-1.2.1/validity/api/urls.py` & `netbox-validity-1.3.0/validity/api/urls.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,17 @@
 router.register("tests", views.ComplianceTestViewSet)
 router.register("test-results", views.ComplianceTestResultViewSet)
 router.register("git-repositories", views.GitRepoViewSet)
 router.register("serializers", views.ConfigSerializerViewSet)
 router.register("namesets", views.NameSetViewSet)
 router.register("reports", views.ComplianceReportViewSet)
 
-urlpatterns = router.urls
+urlpatterns = [
+    path("reports/<int:pk>/devices/", views.DeviceReportView.as_view(), name="report_devices"),
+] + router.urls
 
 app_name = "validity"
 
 
 dcim_urls.append(
     path("devices/<int:pk>/serialized_config/", views.SerializedConfigView.as_view(), name="serialized_config")
 )
```

### Comparing `netbox-validity-1.2.1/validity/api/views.py` & `netbox-validity-1.3.0/validity/api/views.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from http import HTTPStatus
 
 from netbox.api.viewsets import NetBoxModelViewSet
 from rest_framework.exceptions import NotFound
+from rest_framework.generics import ListAPIView
 from rest_framework.response import Response
 from rest_framework.views import APIView
 
 from validity import config, filtersets, models
 from validity.config_compliance.device_config import DeviceConfig
-from ..config_compliance.exceptions import DeviceConfigError
+from validity.config_compliance.exceptions import DeviceConfigError
+from ..choices import SeverityChoices
 from . import serializers
 
 
 if config.netbox_version < "3.5.0":
     from drf_yasg.utils import swagger_auto_schema as extend_schema
 else:
     from drf_spectacular.utils import extend_schema
@@ -67,14 +69,29 @@
 
 
 class ComplianceReportViewSet(ReadOnlyNetboxViewSet):
     queryset = models.ComplianceReport.objects.annotate_result_stats().count_devices_and_tests()
     serializer_class = serializers.ComplianceReportSerializer
 
 
+class DeviceReportView(ListAPIView):
+    serializer_class = serializers.DeviceReportSerializer
+    filterset_class = filtersets.DeviceReportFilterSet
+    queryset = models.VDevice.objects.all()
+
+    def get_queryset(self):
+        severity_ge = SeverityChoices.from_request(self.request)
+        pk = self.kwargs["pk"]
+        return (
+            self.queryset.filter(results__report__pk=pk)
+            .annotate_result_stats(pk, severity_ge)
+            .prefetch_results(pk, severity_ge)
+        )
+
+
 class SerializedConfigView(APIView):
     queryset = models.VDevice.objects.all()
 
     def get_object(self, pk):
         try:
             return self.queryset.get(pk=pk)
         except models.VDevice.DoesNotExist:
```

### Comparing `netbox-validity-1.2.1/validity/choices.py` & `netbox-validity-1.3.0/validity/choices.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional
+from typing import Any, Optional, TypeVar
 
 from django.db.models import TextChoices
 from django.db.models.enums import ChoicesMeta
 from django.utils.translation import gettext_lazy as _
 
 
 class ColoredChoiceMeta(ChoicesMeta):
@@ -12,75 +12,94 @@
         option2 = ('option2', 'yellow')
         option3 = ('option3', 'Option3', 'green')
     """
 
     def __new__(cls, name, bases, namespace, **kwargs):
         colors = {}
         member_names = namespace._member_names
-        namespace._member_names = []
+        namespace._member_names = type(namespace._member_names)()  # clean container
         for key in member_names:
             attr = namespace.pop(key)
             if isinstance(attr, str):
                 colors[key] = attr
                 attr = key
             elif isinstance(attr, (list, tuple)):
                 colors[key] = attr[-1]
                 attr = attr[:-1]
             namespace[key] = attr
-        namespace["_colors"] = colors
-        namespace._member_names.remove("_colors")
+        namespace["__colors__"] = colors
         return super().__new__(cls, name, bases, namespace, **kwargs)
 
     @property
     def colors(self):
-        return self._colors
+        return self.__colors__
+
+
+_Type = TypeVar("_Type")
+
+
+class MemberMixin:
+    @classmethod
+    def member(cls: type[_Type], value: Any) -> Optional[_Type]:
+        return cls._value2member_map_.get(value)  # type: ignore
 
 
 class BoolOperationChoices(TextChoices, metaclass=ColoredChoiceMeta):
     OR = "OR", _("OR"), "purple"
     AND = "AND", _("AND"), "blue"
 
 
 class DynamicPairsChoices(TextChoices, metaclass=ColoredChoiceMeta):
     NO = "NO", _("NO"), "red"
     NAME = "NAME", _("By name"), "blue"
     TAG = "TAG", _("By tag"), "purple"
 
 
-class SeverityChoices(TextChoices, metaclass=ColoredChoiceMeta):
+class SeverityChoices(MemberMixin, TextChoices, metaclass=ColoredChoiceMeta):
     LOW = "LOW", _("LOW"), "green"
     MIDDLE = "MIDDLE", _("MIDDLE"), "yellow"
     HIGH = "HIGH", _("HIGH"), "red"
 
+    @classmethod
+    def from_request(cls, request):
+        severity_query = request.GET.get("severity_ge")
+        if isinstance(severity_query, str):
+            severity_query = severity_query.upper()
+        severity_ge = SeverityChoices.member(severity_query)
+        if not severity_ge:
+            severity_ge = SeverityChoices.LOW
+        return severity_ge
+
+    @classmethod
+    def ge(cls, severity: "SeverityChoices") -> list[str]:
+        index = SeverityChoices.labels.index(severity.label)
+        return cls.labels[index:]
+
 
 class ConfigExtractionChoices(TextChoices, metaclass=ColoredChoiceMeta):
     TTP = "TTP", "TTP", "purple"
     YAML = "YAML", "YAML", "info"
     ROUTEROS = "ROUTEROS", "ROUTEROS", "green"
 
 
-class DeviceGroupByChoices(TextChoices):
+class DeviceGroupByChoices(MemberMixin, TextChoices):
     DEVICE = "device__name", _("Device")
     DEVICE_TYPE = "device__device_type__slug", _("Device Type")
     MANUFACTURER = "device__device_type__manufacturer__slug", _("Manufacturer")
     DEVICE_ROLE = "device__device_role__slug", _("Device Role")
     TENANT = "device__tenant__slug", _("Tenant")
     PLATFORM = "device__platform__slug", _("Platform")
     LOCATION = "device__location__slug", _("Location")
     SITE = "device__site__slug", _("Site")
     TEST = "test__name", _("Test")
 
     @classmethod
     def contains(cls, value: str) -> bool:
         return value in cls._value2member_map_
 
-    @classmethod
-    def member(cls, value: str) -> Optional["DeviceGroupByChoices"]:
-        return cls._value2member_map_.get(value)  # type: ignore
-
     def viewname(self) -> str:
         view_prefixes = {self.TENANT: "tenancy:", self.TEST: "plugins:validity:compliance"}
         default_prefix = "dcim:"
         model_name = self.value.split("__")[-2].replace("_", "")
         return view_prefixes.get(self, default_prefix) + model_name
 
     def pk_field(self):
```

### Comparing `netbox-validity-1.2.1/validity/config_compliance/device_config/base.py` & `netbox-validity-1.3.0/validity/config_compliance/device_config/base.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.1/validity/config_compliance/device_config/routeros.py` & `netbox-validity-1.3.0/validity/config_compliance/device_config/routeros.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.1/validity/config_compliance/device_config/ttp.py` & `netbox-validity-1.3.0/validity/config_compliance/device_config/ttp.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.1/validity/config_compliance/device_config/yaml.py` & `netbox-validity-1.3.0/validity/config_compliance/device_config/yaml.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.1/validity/config_compliance/dynamic_pairs.py` & `netbox-validity-1.3.0/validity/config_compliance/dynamic_pairs.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.1/validity/config_compliance/eval/default_nameset.py` & `netbox-validity-1.3.0/validity/config_compliance/eval/default_nameset.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.1/validity/config_compliance/eval/eval.py` & `netbox-validity-1.3.0/validity/config_compliance/eval/eval.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import ast
+import re
 
 import deepdiff
 from simpleeval import EvalWithCompoundTypes, InvalidExpression
 
 from ..exceptions import EvalError
 from . import default_nameset, eval_defaults
 
@@ -30,19 +31,22 @@
         kwargs["names"] = eval_defaults.DEFAULT_NAMES | kwargs["names"]
         return kwargs["operators"], kwargs["functions"], kwargs["names"]
 
     def _eval(self, node):
         result = super()._eval(node)
         unparsed = ast.unparse(node)
         if not isinstance(node, self.do_not_explain) and str(result) != unparsed and unparsed:
-            self.explanation.append((unparsed, result))
+            self.explanation.append((self._format_unparsed(unparsed), result))
         self.explanation.extend(self._deepdiff)
         self._deepdiff = []
         return result
 
+    def _format_unparsed(self, unparsed) -> str:
+        return re.sub(r" *\\n *", "", unparsed)
+
     def _eval_compare(self, node):
         right = self._eval(node.left)
         to_return = True
         for i, (operation, comp) in enumerate(zip(node.ops, node.comparators), 1):
             if not to_return:
                 break
             left = right
```

### Comparing `netbox-validity-1.2.1/validity/config_compliance/eval/eval_defaults.py` & `netbox-validity-1.3.0/validity/config_compliance/eval/eval_defaults.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.1/validity/filtersets.py` & `netbox-validity-1.3.0/validity/filtersets.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import operator
 from functools import reduce
 from typing import Sequence
 
+from dcim.filtersets import DeviceFilterSet
 from dcim.models import Device, DeviceRole, DeviceType, Location, Manufacturer, Platform, Site
 from django.db.models import Q
 from django_filters import BooleanFilter, ChoiceFilter, ModelMultipleChoiceFilter
 from netbox.filtersets import NetBoxModelFilterSet
 from tenancy.models import Tenant
 
 from validity import models
@@ -106,7 +107,11 @@
         search_fields = ("name", "description", "definitions")
 
     @classmethod
     def get_filters(cls):
         filters = super().get_filters()
         filters["global"] = filters.pop("_global")
         return filters
+
+
+class DeviceReportFilterSet(DeviceFilterSet):
+    compliance_passed = BooleanFilter()
```

### Comparing `netbox-validity-1.2.1/validity/forms/filterset.py` & `netbox-validity-1.3.0/validity/forms/filterset.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,24 @@
     DeviceGroupByChoices,
     DynamicPairsChoices,
     SeverityChoices,
 )
 from .helpers import ExcludeMixin, PlaceholderChoiceField
 
 
+class DeviceReportFilterForm(ExcludeMixin, Form):
+    q = CharField(label=_("Device Search"), required=False)
+    compliance_passed = PlaceholderChoiceField(
+        required=False, placeholder=_("Compliance Passed"), choices=BOOLEAN_WITH_BLANK_CHOICES[1:]
+    )
+    severity_ge = PlaceholderChoiceField(
+        required=False, placeholder=_("Minimum Severity"), choices=SeverityChoices.choices[1:]
+    )
+
+
 class TestResultFilterForm(ExcludeMixin, Form):
     latest = PlaceholderChoiceField(required=False, placeholder=_("Latest"), choices=BOOLEAN_WITH_BLANK_CHOICES[1:])
     passed = PlaceholderChoiceField(
         required=False,
         placeholder=_("Passed"),
         choices=BOOLEAN_WITH_BLANK_CHOICES[1:],
     )
```

### Comparing `netbox-validity-1.2.1/validity/forms/general.py` & `netbox-validity-1.3.0/validity/forms/general.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from dcim.models import DeviceType, Location, Manufacturer, Platform, Site
-from django.forms import PasswordInput, ValidationError
-from django.forms.fields import CharField
+from django.forms import CharField, PasswordInput, Textarea, ValidationError
 from django.utils.translation import gettext_lazy as _
 from extras.models import Tag
 from netbox.forms import NetBoxModelForm
 from tenancy.models import Tenant
 from utilities.forms.fields import DynamicModelChoiceField, DynamicModelMultipleChoiceField
 
 from validity import models
 
 
 class ComplianceTestForm(NetBoxModelForm):
     selectors = DynamicModelMultipleChoiceField(queryset=models.ComplianceSelector.objects.all())
     repo = DynamicModelChoiceField(queryset=models.GitRepo.objects.all(), required=False, label=_("Git Repository"))
+    expression = CharField(required=False, widget=Textarea(attrs={"style": "font-family:monospace"}))
 
     fieldsets = (
         (_("Compliance Test"), ("name", "severity", "description", "selectors", "tags")),
         (_("Expression from Git"), ("repo", "file_path")),
         (_("Expression from DB"), ("expression",)),
     )
 
@@ -108,14 +108,15 @@
         if password := self.cleaned_data.pop("password", None):
             self.instance.password = password
         return super().save(commit)
 
 
 class ConfigSerializerForm(NetBoxModelForm):
     repo = DynamicModelChoiceField(queryset=models.GitRepo.objects.all(), required=False, label=_("Git Repository"))
+    ttp_template = CharField(required=False, widget=Textarea(attrs={"style": "font-family:monospace"}))
 
     fieldsets = (
         (_("Config Serializer"), ("name", "extraction_method", "tags")),
         (_("Template from Git"), ("repo", "file_path")),
         (_("Template from DB"), ("ttp_template",)),
     )
 
@@ -123,14 +124,15 @@
         model = models.ConfigSerializer
         fields = ("name", "extraction_method", "ttp_template", "repo", "file_path", "tags")
 
 
 class NameSetForm(NetBoxModelForm):
     tests = DynamicModelMultipleChoiceField(queryset=models.ComplianceTest.objects.all(), required=False)
     repo = DynamicModelChoiceField(queryset=models.GitRepo.objects.all(), required=False, label=_("Git Repository"))
+    definitions = CharField(required=False, widget=Textarea(attrs={"style": "font-family:monospace"}))
 
     fieldsets = (
         (_("Name Set"), ("name", "description", "_global", "tests", "tags")),
         (_("Definitions from Git"), ("repo", "file_path")),
         (_("Definitions from DB"), ("definitions",)),
     )
```

### Comparing `netbox-validity-1.2.1/validity/forms/helpers.py` & `netbox-validity-1.3.0/validity/forms/helpers.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.1/validity/graphql.py` & `netbox-validity-1.3.0/validity/graphql.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.1/validity/management/commands/linkscripts.py` & `netbox-validity-1.3.0/validity/management/commands/linkscripts.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.1/validity/managers.py` & `netbox-validity-1.3.0/validity/managers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,26 @@
 from itertools import chain
 from typing import TYPE_CHECKING, TypeVar
 
 from django.contrib.postgres.aggregates import ArrayAgg
-from django.db.models import BigIntegerField, Case, Count, F, FloatField, OuterRef, Prefetch, Q, QuerySet, Value, When
+from django.db.models import (
+    BigIntegerField,
+    BooleanField,
+    Case,
+    Count,
+    ExpressionWrapper,
+    F,
+    FloatField,
+    OuterRef,
+    Prefetch,
+    Q,
+    QuerySet,
+    Value,
+    When,
+)
 from django.db.models.fields.json import KeyTextTransform
 from django.db.models.functions import Cast, JSONObject
 from netbox.models import RestrictedQuerySet
 
 from validity import settings
 from validity.choices import DeviceGroupByChoices, SeverityChoices
 
@@ -70,23 +84,24 @@
     pass
 
 
 class NameSetQS(JSONObjMixin, RestrictedQuerySet):
     pass
 
 
+def percentage(field1: str, field2: str) -> Case:
+    return Case(
+        When(Q(**{f"{field2}__gt": 0}), then=Value(100.0) * F(field1) / F(field2)),
+        default=100.0,
+        output_field=FloatField(),
+    )
+
+
 class ComplianceReportQS(RestrictedQuerySet):
     def annotate_result_stats(self, groupby_field: DeviceGroupByChoices | None = None):
-        def percentage(field1: str, field2: str) -> Case:
-            return Case(
-                When(Q(**{f"{field2}__gt": 0}), then=Value(100.0) * F(field1) / F(field2)),
-                default=100.0,
-                output_field=FloatField(),
-            )
-
         qs = self
         if groupby_field:
             qs = self.values(f"results__{groupby_field.pk_field()}", f"results__{groupby_field}")
         only_passed = Q(results__passed=True)
         qs = qs.annotate(
             total_count=Count("results"),
             total_passed=Count("results", filter=only_passed),
@@ -199,7 +214,35 @@
         return result
 
     def count_per_repo(self) -> dict[int | None, int]:
         return self._count_per_something("repo_id", "annotate_git_repo_id")
 
     def count_per_serializer(self) -> dict[int | None, int]:
         return self._count_per_something("serializer_id", "annotate_serializer_id")
+
+    def annotate_result_stats(self, report_id: int, severity_ge: SeverityChoices = SeverityChoices.LOW):
+        results_filter = Q(results__report__pk=report_id) & self._severity_filter(severity_ge, "results")
+        return self.annotate(
+            results_count=Count("results", filter=results_filter),
+            results_passed=Count("results", filter=results_filter & Q(results__passed=True)),
+            results_percentage=percentage("results_passed", "results_count"),
+            compliance_passed=ExpressionWrapper(Q(results_count=F("results_passed")), output_field=BooleanField()),
+        )
+
+    @staticmethod
+    def _severity_filter(severity: SeverityChoices, query_base: str = "") -> Q:
+        query_path = "test__severity__in"
+        if query_base:
+            query_path = f"{query_base}__{query_path}"
+        return Q(**{query_path: SeverityChoices.ge(severity)})
+
+    def prefetch_results(self, report_id: int, severity_ge: SeverityChoices = SeverityChoices.LOW):
+        from validity.models import ComplianceTestResult
+
+        return self.prefetch_related(
+            Prefetch(
+                "results",
+                queryset=ComplianceTestResult.objects.filter(self._severity_filter(severity_ge), report__pk=report_id)
+                .select_related("test")
+                .order_by("test__name"),
+            )
+        )
```

### Comparing `netbox-validity-1.2.1/validity/migrations/0001_initial.py` & `netbox-validity-1.3.0/validity/migrations/0001_initial.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,14 +83,15 @@
                 ("name", models.CharField(max_length=255, unique=True)),
                 ("description", models.TextField()),
                 ("severity", models.CharField(default="MIDDLE", max_length=10)),
                 ("expression", models.TextField(blank=True)),
             ],
             options={
                 "abstract": False,
+                "ordering": ("name",),
             },
             bases=(validity.models.base.URLMixin, models.Model),
         ),
         migrations.CreateModel(
             name="GitRepo",
             fields=[
                 ("id", models.BigAutoField(auto_created=True, primary_key=True, serialize=False)),
@@ -207,25 +208,32 @@
                 (
                     "custom_field_data",
                     models.JSONField(blank=True, default=dict, encoder=utilities.json.CustomFieldJSONEncoder),
                 ),
                 ("created", models.DateTimeField(auto_now_add=True, null=True)),
                 ("last_updated", models.DateTimeField(auto_now=True, null=True)),
                 ("passed", models.BooleanField()),
-                ("explanation", models.JSONField(default=list, encoder=validity.models.test_result.DeepDiffEncoder)),
+                (
+                    "explanation",
+                    models.JSONField(blank=True, default=list, encoder=validity.models.test_result.DeepDiffEncoder),
+                ),
                 (
                     "device",
                     models.ForeignKey(
                         on_delete=django.db.models.deletion.CASCADE, related_name="results", to="validity.vdevice"
                     ),
                 ),
                 (
                     "dynamic_pair",
                     models.ForeignKey(
-                        null=True, on_delete=django.db.models.deletion.CASCADE, related_name="+", to="validity.vdevice"
+                        blank=True,
+                        null=True,
+                        on_delete=django.db.models.deletion.CASCADE,
+                        related_name="+",
+                        to="validity.vdevice",
                     ),
                 ),
                 (
                     "report",
                     models.ForeignKey(
                         blank=True,
                         null=True,
```

### Comparing `netbox-validity-1.2.1/validity/migrations/0002_custom_fields.py` & `netbox-validity-1.3.0/validity/migrations/0002_custom_fields.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.1/validity/migrations/0004_netbox35_scripts.py` & `netbox-validity-1.3.0/validity/migrations/0004_netbox35_scripts.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.1/validity/models/base.py` & `netbox-validity-1.3.0/validity/models/base.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.1/validity/models/device.py` & `netbox-validity-1.3.0/validity/models/device.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.1/validity/models/nameset.py` & `netbox-validity-1.3.0/validity/models/nameset.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.1/validity/models/repo.py` & `netbox-validity-1.3.0/validity/models/repo.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.1/validity/models/selector.py` & `netbox-validity-1.3.0/validity/models/selector.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.1/validity/models/serializer.py` & `netbox-validity-1.3.0/validity/models/serializer.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.1/validity/models/test.py` & `netbox-validity-1.3.0/validity/models/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,17 @@
     selectors = models.ManyToManyField(to="ComplianceSelector", related_name="tests", verbose_name=_("Selectors"))
 
     clone_fields = ("expression", "selectors", "severity", "repo", "file_path")
     text_db_field_name = "expression"
 
     objects = ComplianceTestQS.as_manager()
 
+    class Meta:
+        ordering = ("name",)
+
     def clean(self):
         super().clean()
         if self.expression:
             err = {"expression": "Invalid Python expression"}
             try:
                 expr = ast.parse(self.expression)
                 if len(expr.body) != 1 or not isinstance(expr.body[0], ast.Expr):
```

### Comparing `netbox-validity-1.2.1/validity/models/test_result.py` & `netbox-validity-1.3.0/validity/models/test_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,18 +15,18 @@
         return json_dumps(o, default_mapping={type({}.values()): list, type({}.keys()): list, object: str})
 
 
 class ComplianceTestResult(BaseReadOnlyModel):
     test = models.ForeignKey(ComplianceTest, verbose_name=_("Test"), related_name="results", on_delete=models.CASCADE)
     device = models.ForeignKey(VDevice, verbose_name=_("Device"), related_name="results", on_delete=models.CASCADE)
     dynamic_pair = models.ForeignKey(
-        VDevice, verbose_name=_("Dynamic Pair"), related_name="+", on_delete=models.CASCADE, null=True
+        VDevice, verbose_name=_("Dynamic Pair"), related_name="+", on_delete=models.CASCADE, null=True, blank=True
     )
     passed = models.BooleanField(_("Passed"))
-    explanation = models.JSONField(_("Explanation"), default=list, encoder=DeepDiffEncoder)
+    explanation = models.JSONField(_("Explanation"), default=list, encoder=DeepDiffEncoder, blank=True)
     report = models.ForeignKey(
         "ComplianceReport",
         verbose_name=_("Report"),
         on_delete=models.CASCADE,
         null=True,
         blank=True,
         related_name="results",
```

### Comparing `netbox-validity-1.2.1/validity/navigation.py` & `netbox-validity-1.3.0/validity/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.1/validity/scripts/git.py` & `netbox-validity-1.3.0/validity/scripts/validity_git.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.1/validity/scripts/run_tests.py` & `netbox-validity-1.3.0/validity/scripts/validity_run_tests.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.1/validity/search.py` & `netbox-validity-1.3.0/validity/search.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.1/validity/tables.py` & `netbox-validity-1.3.0/validity/tables.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,18 @@
+import itertools
 from functools import partial
 
 from dcim.models import Device
 from dcim.tables import DeviceTable
+from dcim.tables.template_code import DEVICE_LINK
 from django.urls import reverse
 from django.utils.html import format_html
 from django.utils.safestring import mark_safe
 from django.utils.translation import gettext_lazy as _
-from django_tables2 import Column, RequestConfig, Table
+from django_tables2 import Column, RequestConfig, Table, TemplateColumn
 from netbox.tables import BooleanColumn as BooleanColumn
 from netbox.tables import ChoiceFieldColumn, ManyToManyColumn, NetBoxTable
 from utilities.paginator import EnhancedPaginator
 
 from validity import models
 from validity.utils.misc import colorful_percentage
 
@@ -59,25 +61,27 @@
         default_columns = fields
 
 
 class ComplianceResultTable(NetBoxTable):
     id = Column(linkify=True)
     test = Column(linkify=True)
     device = Column(linkify=True)
+    passed = BooleanColumn()
 
     class Meta(NetBoxTable.Meta):
         model = models.ComplianceTestResult
         fields = ("id", "test", "device", "passed", "created")
         exclude = ("actions",)
         default_columns = fields
 
 
 class GitRepoTable(NetBoxTable):
     name = Column(linkify=True)
     total_devices = Column(empty_values=())
+    default = BooleanColumn()
 
     class Meta(NetBoxTable.Meta):
         model = models.GitRepo
         fields = ("name", "default", "total_devices")
         default_columns = fields
 
     def __init__(self, *args, extra_columns=None, **kwargs):
@@ -104,48 +108,71 @@
 
     def render_total_devices(self, record):
         return self.total_devices_map.get(record.id, 0)
 
 
 class ExplanationColumn(Column):
     def render(self, value):
-        return format_html("<code>{}</code>", value)
+        return format_html('<code class="language-python">{}</code>', value)
 
 
 class ExplanationTable(Table):
+    counter = Column(verbose_name="#", empty_values=(), orderable=False)
     left = ExplanationColumn(empty_values=(), verbose_name=_("Expression"))
     right = ExplanationColumn(empty_values=(), verbose_name=_("Value"))
 
+    def render_counter(self):
+        self.row_counter = getattr(self, "row_counter", itertools.count(start=1))
+        return format_html('<b class="mr-5">{}</b>', next(self.row_counter))
+
     class Meta:
         template_name = "django_tables2/bootstrap.html"
 
 
 class NameSetTable(NetBoxTable):
     name = Column(linkify=True)
     tests = ManyToManyColumn(linkify_item=True)
+    _global = BooleanColumn()
 
     class Meta(NetBoxTable.Meta):
         model = models.NameSet
         fields = ("name", "_global", "tests")
         default_columns = fields
 
 
+class StatsColumn(Column):
+    def __init__(self, data_prefix: str, **kwargs):
+        super().__init__(**kwargs)
+        self.data_prefix = data_prefix
+
+    def render(self, value, record):
+        def get_table_attr(obj, attr_name):
+            return getattr(obj, attr_name) if hasattr(obj, attr_name) else obj.get(attr_name)
+
+        count = get_table_attr(record, f"{self.data_prefix}_count")
+        if not count:
+            return "—"
+        passed = get_table_attr(record, f"{self.data_prefix}_passed")
+        percentage = get_table_attr(record, f"{self.data_prefix}_percentage")
+        return mark_safe(f"{passed}/{count} ") + colorful_percentage(percentage)
+
+
 class ComplianceReportTable(NetBoxTable):
     id = Column(linkify=True)
     groupby_value = Column(
         verbose_name=_("GroupBy Value"),
         linkify=lambda record: reverse(record["viewname"], kwargs={"pk": record["groupby_pk"]}),
         empty_values=(None,),
     )
     device_count = Column(verbose_name=_("Devices"), empty_values=())
     test_count = Column(verbose_name=_("Unique Tests"), empty_values=())
-    total_stats = Column(verbose_name=_("Overall Passed"), empty_values=())
-    low_stats = Column(verbose_name=_("Low Severity"), empty_values=())
-    middle_stats = Column(verbose_name=_("Middle Severity"), empty_values=())
-    high_stats = Column(verbose_name=_("High Severity"), empty_values=())
+    total_stats = StatsColumn(data_prefix="total", verbose_name=_("Overall Passed"), empty_values=())
+    low_stats = StatsColumn(data_prefix="low", verbose_name=_("Low Severity"), empty_values=())
+    middle_stats = StatsColumn(data_prefix="middle", verbose_name=_("Middle Severity"), empty_values=())
+    high_stats = StatsColumn(data_prefix="high", verbose_name=_("High Severity"), empty_values=())
 
     class Meta(NetBoxTable.Meta):
         model = models.ComplianceReport
         fields = (
             "id",
             "groupby_value",
             "device_count",
@@ -155,36 +182,62 @@
             "middle_stats",
             "high_stats",
             "created",
         )
         exclude = ("actions",)
         default_columns = fields
 
-    def _render_stats(self, severity, record):
-        def get_table_attr(obj, attr_name):
-            return getattr(obj, attr_name) if hasattr(obj, attr_name) else obj.get(attr_name)
 
-        count = get_table_attr(record, f"{severity}_count")
-        if not count:
-            return "—"
-        passed = get_table_attr(record, f"{severity}_passed")
-        percentage = get_table_attr(record, f"{severity}_percentage")
-        return mark_safe(f"{passed}/{count} ") + colorful_percentage(percentage)
+class DeviceReportM2MColumn(ManyToManyColumn):
+    def __init__(self, *args, badge_color: str = "", **kwargs):
+        if badge_color:
+            kwargs["attrs"] = kwargs.get("attrs", {}) | {
+                "a": {"class": f"mb-1 badge rounded-pill text-{badge_color} border border-{badge_color}"}
+            }
+            kwargs["separator"] = " "
+        kwargs.setdefault("transform", lambda obj: str(obj.test))
+        super().__init__(*args, **kwargs)
 
-    def render_total_stats(self, record):
-        return self._render_stats("total", record)
+    def render(self, value):
+        """
+        Default implementation does not draw "-" when all the results are filtered out
+        """
+        result = super().render(value)
+        return result if result else "—"
 
-    def render_low_stats(self, record):
-        return self._render_stats("low", record)
 
-    def render_middle_stats(self, record):
-        return self._render_stats("middle", record)
+class ComplianceReportDeviceTable(NetBoxTable):
+    device = TemplateColumn(
+        order_by=("_name",), template_code=DEVICE_LINK, linkify=True, accessor="name", attrs={"th": {"class": "col-2"}}
+    )
+    compliance_passed = BooleanColumn(
+        verbose_name=_("Compliance Passed"),
+        empty_values=(),
+    )
+    result_stats = StatsColumn(data_prefix="results", empty_values=(), verbose_name=_("Result Statistics"))
+    passed_results = DeviceReportM2MColumn(
+        linkify_item=True,
+        verbose_name=_("Passed Tests"),
+        filter=lambda qs: (obj for obj in qs.all() if obj.passed),
+        accessor="results",
+        badge_color="success",
+    )
+    failed_results = DeviceReportM2MColumn(
+        linkify_item=True,
+        verbose_name=_("Failed Tests"),
+        filter=lambda qs: (obj for obj in qs.all() if not obj.passed),
+        accessor="results",
+        badge_color="danger",
+    )
 
-    def render_high_stats(self, record):
-        return self._render_stats("high", record)
+    class Meta(NetBoxTable.Meta):
+        model = models.VDevice
+        fields = ("device", "compliance_passed", "result_stats", "passed_results", "failed_results")
+        default_columns = fields
+        exclude = ("actions",)
 
 
 class DynamicPairsTable(DeviceTable):
     dynamic_pair = Column(verbose_name="Dynamic Pair", linkify=True)
 
     class Meta(DeviceTable.Meta):
         model = Device
```

### Comparing `netbox-validity-1.2.1/validity/templates/validity/compliance_results.html` & `netbox-validity-1.3.0/validity/templates/validity/aux_tab_table.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 {% extends 'generic/object.html' %}
 {% load helpers %}
 {% load bootstrap5 %}
 {% load render_table from django_tables2 %}
 {% block head %}
 {% endblock %}
-{% block title %}{{ object }}: Test Results{% endblock %}
 {% block subtitle %}
 <div class="object-subtitle"></div>
 {% endblock %}
 {% block controls %}
 {%if read_only %}
 <div class="controls"></div>
 {% else %}
@@ -16,29 +15,23 @@
 {% endif %}
 {% endblock %}
 {% block content %}
   <div class="row mb-3">
     <div class="col-auto">
     <form role="form" class="row" method="get">
       {% bootstrap_form filterset_form layout="inline" %}
-      <div class="col-auto">{% buttons submit="Search" %}{% endbuttons %}</div>
+      <div class="col-auto">{% buttons submit=search_button_name|default:"Search" %}{% endbuttons %}</div>
       <div class="col-auto">
-        <a
-          class="btn btn-primary"
-          target="_blank"
-          href="{% url 'plugins:validity:compliancetestresult_list' %}?{{ result_relation }}_id={{ object.pk }}"
-        >
-          Advanced Search ⤴
-        </a>
+        {% block extra_button %}{% endblock %}
       </div>
     </form>
   </div>
 </div>
 <div class="card mb-3">
   <div class="card-body">
-    <h5 class="card-title mb-2">All Results related to {{ object }}</h5>
+    <h5 class="card-title mb-2">{% block table_title %}{% endblock %}</h5>
     <div class="table-responsive">
       {% render_table table 'inc/table.html' %}
     </div>
     {%include 'inc/paginator.html' with paginator=table.paginator page=table.page%}
   </div>
   {% endblock %}
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `netbox-validity-1.2.1/validity/templates/validity/compliancereport.html` & `netbox-validity-1.3.0/validity/templates/validity/compliancereport.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.1/validity/templates/validity/complianceselector.html` & `netbox-validity-1.3.0/validity/templates/validity/complianceselector.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.1/validity/templates/validity/compliancetest.html` & `netbox-validity-1.3.0/validity/templates/validity/gitrepo.html`

 * *Files 22% similar despite different names*

```diff
@@ -1,55 +1,77 @@
 {% extends 'generic/object.html' %}
 {% load validity %}
 {% load render_table from django_tables2 %}
+
+{% block extra_controls %}
+<form action="{% url 'extras:script' module='validity_git' name='SyncGitRepos' %}" method="post">
+  {% csrf_token %}
+  <input type="hidden" name="repos" value="{{ object.pk }}">
+  <button class="btn btn-sm btn-primary" type="submit">⟳ Sync</button>
+</form>
+{% endblock %}
+
 {% block content %}
-  <div class="row">
-    <div class="col col-md-4">
-      <div class="card mb-3">
-        <h5 class="card-header">Compliance Test</h5>
+  <div class="row mb-3">
+    <div class="col col-md-6">
+      <div class="card">
+        <h5 class="card-header">Git Repository</h5>
         <div class="card-body">
           <table class="table table-hover attr-table">
             <tr>
               <th scope="row">Name</th>
               <td>{{ object.name }}</td>
             </tr>
             <tr>
-              <th scope="row">Severity</th>
-              <td>{{ object | colored_choice:"severity" }}</td>
+              <th scope="row">Head Hash</th>
+              <td>{{ object.head_hash | placeholder }}</td>
             </tr>
             <tr>
-              <th scope="row">Selectors</th>
-              <td>{{ object.selectors.all | linkify_list }}</td>
+              <th scope="row">Default</th>
+              <td>{{ object.default | checkmark }}</td>
             </tr>
             <tr>
-              <th scope="row">Description</th>
-              <td>{{ object.description }}</td>
+              <th scope="row">Device Config Path</th>
+              <td><code>{{ object.device_config_path }}</code></td>
+            </tr>
+            <tr>
+              <th scope="row">Git URL</th>
+              <td><code>{{ object.git_url }}</code></td>
+            </tr>
+            <tr>
+              <th scope="row">Web URL</th>
+              <td><code>{{ object.web_url | placeholder }}</code></td>
+            </tr>
+            <tr>
+              <th scope="row">Username</th>
+              <td>{{ object.username | placeholder }}</td>
+            </tr>
+            <tr>
+              <th scope="row">Password</th>
+              <td>{% if object.encrypted_password %}$encrypted{% else %}{{ '' | placeholder }}{% endif %}</td>
+            </tr>
+            <tr>
+              <th scope="row">Branch</th>
+              <td>{{ object.branch | placeholder }}</td>
             </tr>
-            {% include "validity/inc/git_link.html" %}
           </table>
         </div>
       </div>
-      {% include 'inc/panels/tags.html' %}
     </div>
-    <div class="col col-md-8">
-      <div class="card mb-3">
-        <h5 class="card-header">Expression [source: {{ object | data_source }}]</h5>
-        <div class="card-body">
-          <pre>{{ object.effective_expression }}</pre>
-        </div>
-      </div>
+    <div class="col col-md-6">
+      {% include 'inc/panels/tags.html' %}
     </div>
   </div>
   <div class="row">
     <div class="col col-md-12">
       <div class="card">
-        <h5 class="card-header">Bound Namesets</h5>
+        <h5 class="card-header">Bound Devices</h5>
         <div class="card-body">
           <div class="pt-0 mb-3 col col-md-3">
-            {% include 'validity/inc/search_form.html' with model='NameSet' %}
+            {% include 'validity/inc/search_form.html' with model='Device' %}
           </div>
           <div class="table-responsive">
             {% render_table table 'inc/table.html' %}
           </div>
           {%include 'inc/paginator.html' with paginator=table.paginator page=table.page%}
         </div>
       </div>
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,15 +1,21 @@
 {% extends 'generic/object.html' %} {% load validity %} {% load render_table
-from django_tables2 %} {% block content %}
-** Compliance Test **
-Name        {{ object.name }}
-Severity    {{ object | colored_choice:"severity" }}
-Selectors   {{ object.selectors.all | linkify_list }}
-Description {{ object.description }}
+from django_tables2 %} {% block extra_controls %}
+{% csrf_token %}  â³ Sync
+{% endblock %} {% block content %}
+** Git Repository **
+Name               {{ object.name }}
+Head Hash          {{ object.head_hash | placeholder }}
+Default            {{ object.default | checkmark }}
+Device Config Path {{ object.device_config_path }}
+Git URL            {{ object.git_url }}
+Web URL            {{ object.web_url | placeholder }}
+Username           {{ object.username | placeholder }}
+Password           {% if object.encrypted_password %}$encrypted{% else %}{{ ''
+                   | placeholder }}{% endif %}
+Branch             {{ object.branch | placeholder }}
 {% include 'inc/panels/tags.html' %}
-** Expression [source: {{ object | data_source }}] **
-{{ object.effective_expression }}
-** Bound Namesets **
-{% include 'validity/inc/search_form.html' with model='NameSet' %}
+** Bound Devices **
+{% include 'validity/inc/search_form.html' with model='Device' %}
 {% render_table table 'inc/table.html' %}
 {%include 'inc/paginator.html' with paginator=table.paginator page=table.page%}
 {% endblock content %}
```

### Comparing `netbox-validity-1.2.1/validity/templates/validity/compliancetestresult.html` & `netbox-validity-1.3.0/validity/templates/validity/compliancetestresult.html`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 {% extends 'generic/object.html' %}
 {% load validity %}
 {% load render_table from django_tables2 %}
+
+{% block head %}
+  {{ block.super }}
+  {% include "validity/inc/prism.html" with header=True only %}
+{% endblock head %}
 {% block controls %}
 <div class="controls"></div>
 {% endblock %}
+
 {% block content %}
 <div class="row mb-3">
   <div class="col col-md-4">
     <div class="card">
       <h5 class="card-header">Compliance Test Results</h5>
       <div class="card-body">
         <table class="table table-hover attr-table">
@@ -56,15 +62,15 @@
           <h5 class="card-header">Explanation</h5>
         </div>
         <div class="col d-flex align-items-center mb-0 pb-0 justify-content-end me-5">
           <a class="btn btn-sm btn-primary" href="?verbose=true">Verbose</a>
         </div>
       </div>
       <div class="card-body pt-0">
-        <div class="table-responsive">{% render_table explanation_table 'inc/table.html' %}</div>
+        <div class="table-responsive">{% render_table explanation_table %}</div>
       </div>
     </div>
   </div>
 </div>
 <div class="row">
   <div class="col col-md-12">
     <div class="card">
@@ -74,8 +80,13 @@
           {% render_table result_table %}
         </div>
         {%include 'inc/paginator.html' with paginator=result_table.paginator page=result_table.page%}
       </div>
     </div>
   </div>
 </div>
-{% endblock content %}
+{% endblock content %}
+
+{% block javascript %}
+{{ block.super }}
+{% include "validity/inc/prism.html" %}
+{% endblock %}
```

#### html2text {}

```diff
@@ -1,19 +1,22 @@
 {% extends 'generic/object.html' %} {% load validity %} {% load render_table
-from django_tables2 %} {% block controls %}
+from django_tables2 %} {% block head %} {{ block.super }} {% include "validity/
+inc/prism.html" with header=True only %} {% endblock head %} {% block controls
+%}
 {% endblock %} {% block content %}
 ** Compliance Test Results **
 ID            {{ object.id }}
 Test          {{ object.test | linkify }}
 Test Severity {{ object.test | colored_choice:"severity" }}
 Device        {{ object.device | linkify }}
 Dynamic Pair  {{ object.dynamic_pair | linkify | placeholder }}
 Result        {% if object.passed %} PASSED {% else %} FAILED {% endif %}
 Created       {{ object.created | date:"Y-m-d G:i:s" }}
 ** Explanation **
 Verbose
-{% render_table explanation_table 'inc/table.html' %}
+{% render_table explanation_table %}
 ** Other results for the same test and device **
 {% render_table result_table %}
 {%include 'inc/paginator.html' with paginator=result_table.paginator
 page=result_table.page%}
-{% endblock content %}
+{% endblock content %} {% block javascript %} {{ block.super }} {% include
+"validity/inc/prism.html" %} {% endblock %}
```

### Comparing `netbox-validity-1.2.1/validity/templates/validity/configserializer.html` & `netbox-validity-1.3.0/validity/templates/validity/configserializer.html`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         {% include 'inc/panels/tags.html' %}
       </div>
     </div>
     <div class="col col-md-8">
       <div class="card">
         <h5 class="card-header">TTP Template [Source: {{ object | data_source }}]</h5>
         <div class="card-body">
-          <pre class="bg-light">{{ object.effective_template }}</pre>
+          {% include 'extras/inc/configcontext_data.html' with data=object.effective_template %}
         </div>
       </div>
     </div>
   </div>
   <div class="row">
     <div class="col col-md-12">
       <div class="card">
```

#### html2text {}

```diff
@@ -1,13 +1,14 @@
 {% extends 'generic/object.html' %} {% load validity %} {% load render_table
 from django_tables2 %} {% block content %}
 ** Config Serializer **
 Name                     {{ object.name }}
 Config Extraction Method {{ object | colored_choice:"extraction_method" }}
 {% include 'inc/panels/tags.html' %}
 ** TTP Template [Source: {{ object | data_source }}] **
-{{ object.effective_template }}
+{% include 'extras/inc/configcontext_data.html' with
+data=object.effective_template %}
 ** Bound Devices **
 {% include 'validity/inc/search_form.html' with model='Device' %}
 {% render_table table 'inc/table.html' %}
 {%include 'inc/paginator.html' with paginator=table.paginator page=table.page%}
 {% endblock content %}
```

### Comparing `netbox-validity-1.2.1/validity/templates/validity/device_config.html` & `netbox-validity-1.3.0/validity/templates/validity/device_config.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.1/validity/templates/validity/gitrepo.html` & `netbox-validity-1.3.0/validity/templates/validity/compliancetest.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,80 +1,68 @@
 {% extends 'generic/object.html' %}
 {% load validity %}
 {% load render_table from django_tables2 %}
-
-{% block extra_controls %}
-<form action="{% url 'extras:script' module='validity_git' name='SyncGitRepos' %}" method="post">
-  {% csrf_token %}
-  <input type="hidden" name="repos" value="{{ object.pk }}">
-  <button class="btn btn-sm btn-primary" type="submit">⟳ Sync</button>
-</form>
-{% endblock %}
+{% block head %}
+  {{ block.super }}
+  {% include "validity/inc/prism.html" with header=True only %}
+{% endblock head %}
 
 {% block content %}
-  <div class="row mb-3">
-    <div class="col col-md-6">
-      <div class="card">
-        <h5 class="card-header">Git Repository</h5>
+  <div class="row">
+    <div class="col col-md-4">
+      <div class="card mb-3">
+        <h5 class="card-header">Compliance Test</h5>
         <div class="card-body">
           <table class="table table-hover attr-table">
             <tr>
               <th scope="row">Name</th>
               <td>{{ object.name }}</td>
             </tr>
             <tr>
-              <th scope="row">Head Hash</th>
-              <td>{{ object.head_hash | placeholder }}</td>
-            </tr>
-            <tr>
-              <th scope="row">Default</th>
-              <td>{{ object.default | checkmark }}</td>
+              <th scope="row">Severity</th>
+              <td>{{ object | colored_choice:"severity" }}</td>
             </tr>
             <tr>
-              <th scope="row">Device Config Path</th>
-              <td><code>{{ object.device_config_path }}</code></td>
+              <th scope="row">Selectors</th>
+              <td>{{ object.selectors.all | linkify_list }}</td>
             </tr>
             <tr>
-              <th scope="row">Git URL</th>
-              <td><code>{{ object.git_url }}</code></td>
-            </tr>
-            <tr>
-              <th scope="row">Web URL</th>
-              <td><code>{{ object.web_url | placeholder }}</code></td>
-            </tr>
-            <tr>
-              <th scope="row">Username</th>
-              <td>{{ object.username | placeholder }}</td>
-            </tr>
-            <tr>
-              <th scope="row">Password</th>
-              <td>{% if object.encrypted_password %}$encrypted{% else %}{{ '' | placeholder }}{% endif %}</td>
-            </tr>
-            <tr>
-              <th scope="row">Branch</th>
-              <td>{{ object.branch | placeholder }}</td>
+              <th scope="row">Description</th>
+              <td>{{ object.description }}</td>
             </tr>
+            {% include "validity/inc/git_link.html" %}
           </table>
         </div>
       </div>
-    </div>
-    <div class="col col-md-6">
       {% include 'inc/panels/tags.html' %}
     </div>
+    <div class="col col-md-8">
+      <div class="card mb-3">
+        <h5 class="card-header">Expression [source: {{ object | data_source }}]</h5>
+        <div class="card-body">
+          <pre><code class="language-python">{{ object.effective_expression }}</code></pre>
+        </div>
+      </div>
+    </div>
   </div>
   <div class="row">
     <div class="col col-md-12">
       <div class="card">
-        <h5 class="card-header">Bound Devices</h5>
+        <h5 class="card-header">Bound Namesets</h5>
         <div class="card-body">
           <div class="pt-0 mb-3 col col-md-3">
-            {% include 'validity/inc/search_form.html' with model='Device' %}
+            {% include 'validity/inc/search_form.html' with model='NameSet' %}
           </div>
           <div class="table-responsive">
             {% render_table table 'inc/table.html' %}
           </div>
           {%include 'inc/paginator.html' with paginator=table.paginator page=table.page%}
         </div>
       </div>
     </div>
   </div>
 {% endblock content %}
+
+{% block javascript %}
+{{ block.super }}
+{% include "validity/inc/prism.html" %}
+{% endblock %}
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,21 +1,18 @@
 {% extends 'generic/object.html' %} {% load validity %} {% load render_table
-from django_tables2 %} {% block extra_controls %}
-{% csrf_token %}  â³ Sync
-{% endblock %} {% block content %}
-** Git Repository **
-Name               {{ object.name }}
-Head Hash          {{ object.head_hash | placeholder }}
-Default            {{ object.default | checkmark }}
-Device Config Path {{ object.device_config_path }}
-Git URL            {{ object.git_url }}
-Web URL            {{ object.web_url | placeholder }}
-Username           {{ object.username | placeholder }}
-Password           {% if object.encrypted_password %}$encrypted{% else %}{{ ''
-                   | placeholder }}{% endif %}
-Branch             {{ object.branch | placeholder }}
+from django_tables2 %} {% block head %} {{ block.super }} {% include "validity/
+inc/prism.html" with header=True only %} {% endblock head %} {% block content
+%}
+** Compliance Test **
+Name        {{ object.name }}
+Severity    {{ object | colored_choice:"severity" }}
+Selectors   {{ object.selectors.all | linkify_list }}
+Description {{ object.description }}
 {% include 'inc/panels/tags.html' %}
-** Bound Devices **
-{% include 'validity/inc/search_form.html' with model='Device' %}
+** Expression [source: {{ object | data_source }}] **
+{{ object.effective_expression }}
+** Bound Namesets **
+{% include 'validity/inc/search_form.html' with model='NameSet' %}
 {% render_table table 'inc/table.html' %}
 {%include 'inc/paginator.html' with paginator=table.paginator page=table.page%}
-{% endblock content %}
+{% endblock content %} {% block javascript %} {{ block.super }} {% include
+"validity/inc/prism.html" %} {% endblock %}
```

### Comparing `netbox-validity-1.2.1/validity/templates/validity/nameset.html` & `netbox-validity-1.3.0/validity/templates/validity/nameset.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 {% extends 'generic/object.html' %}
 {% load validity %}
 {% load helpers %}
+
+{% block head %}
+  {{ block.super }}
+  {% include "validity/inc/prism.html" with header=True only %}
+{% endblock head %}
+
 {% block content %}
   <div class="row">
     <div class="col col-md-4">
       <div class="card mb-3">
         <h5 class="card-header">Compliance Test</h5>
         <div class="card-body">
           <table class="table table-hover attr-table">
@@ -30,13 +36,18 @@
       </div>
       {% include 'inc/panels/tags.html' %}
     </div>
     <div class="col col-md-8">
       <div class="card mb-3">
         <h5 class="card-header">Definitions [source: {{ object | data_source }}]</h5>
         <div class="card-body">
-          <pre>{{ object.effective_definitions }}</pre>
+          <pre><code class="language-python">{{ object.effective_definitions }}</code></pre>
         </div>
       </div>
     </div>
   </div>
 {% endblock content %}
+
+{% block javascript %}
+{{ block.super }}
+{% include "validity/inc/prism.html" %}
+{% endblock %}
```

#### html2text {}

```diff
@@ -1,11 +1,13 @@
 {% extends 'generic/object.html' %} {% load validity %} {% load helpers %} {%
-block content %}
+block head %} {{ block.super }} {% include "validity/inc/prism.html" with
+header=True only %} {% endblock head %} {% block content %}
 ** Compliance Test **
 Name        {{ object.name }}
 Description {{ object.description | placeholder}}
 Global      {{ global | checkmark }}
 Bound Tests {{ object.tests.all | linkify_list }}
 {% include 'inc/panels/tags.html' %}
 ** Definitions [source: {{ object | data_source }}] **
 {{ object.effective_definitions }}
-{% endblock content %}
+{% endblock content %} {% block javascript %} {{ block.super }} {% include
+"validity/inc/prism.html" %} {% endblock %}
```

### Comparing `netbox-validity-1.2.1/validity/templatetags/validity.py` & `netbox-validity-1.3.0/validity/templatetags/validity.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.1/validity/tests/base.py` & `netbox-validity-1.3.0/validity/tests/base.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.1/validity/tests/conftest.py` & `netbox-validity-1.3.0/validity/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.1/validity/tests/factories.py` & `netbox-validity-1.3.0/validity/tests/factories.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.1/validity/tests/test_api.py` & `netbox-validity-1.3.0/validity/tests/test_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -156,7 +156,19 @@
         "repo",
         "local_copy_last_updated",
         "config_web_link",
         "serialized_config",
     }
     assert resp.json()["serialized_config"] == {"key1": "value1"}
     assert resp.json()["local_copy_last_updated"] == lm.isoformat().replace("+00:00", "Z")
+
+
+@pytest.mark.django_db
+def test_report_devices(admin_client):
+    report = ReportFactory(passed_results=2, failed_results=1)
+    resp = admin_client.get(f"/api/plugins/validity/reports/{report.pk}/devices/")
+    assert resp.status_code == HTTPStatus.OK
+    results = resp.json()["results"]
+    assert len(results) == 3
+    for device in results:
+        assert len(device["results"]) == 1
+        assert device["results_count"] == 1
```

### Comparing `netbox-validity-1.2.1/validity/tests/test_config_compliance/test_device_config.py` & `netbox-validity-1.3.0/validity/tests/test_config_compliance/test_device_config.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.1/validity/tests/test_config_compliance/test_dynamic_pairs.py` & `netbox-validity-1.3.0/validity/tests/test_config_compliance/test_dynamic_pairs.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.1/validity/tests/test_config_compliance/test_eval.py` & `netbox-validity-1.3.0/validity/tests/test_config_compliance/test_eval.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.1/validity/tests/test_graphql.py` & `netbox-validity-1.3.0/validity/tests/test_graphql.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.1/validity/tests/test_models/test_clean.py` & `netbox-validity-1.3.0/validity/tests/test_models/test_clean.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.1/validity/tests/test_models/test_git_link.py` & `netbox-validity-1.3.0/validity/tests/test_models/test_git_link.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.1/validity/tests/test_models/test_git_repo.py` & `netbox-validity-1.3.0/validity/tests/test_models/test_git_repo.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.1/validity/tests/test_models/test_selector.py` & `netbox-validity-1.3.0/validity/tests/test_models/test_selector.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.1/validity/tests/test_models/test_vdevice.py` & `netbox-validity-1.3.0/validity/tests/test_models/test_vdevice.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.1/validity/tests/test_scripts/test_run_tests.py` & `netbox-validity-1.3.0/validity/tests/test_scripts/test_run_tests.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.1/validity/tests/test_utils/test_git.py` & `netbox-validity-1.3.0/validity/tests/test_utils/test_git.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.1/validity/tests/test_utils/test_misc.py` & `netbox-validity-1.3.0/validity/tests/test_utils/test_misc.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.1/validity/tests/test_views.py` & `netbox-validity-1.3.0/validity/tests/test_views.py`

 * *Files 9% similar despite different names*

```diff
@@ -151,7 +151,14 @@
 
 
 @pytest.mark.django_db
 def test_device_results(admin_client):
     device = DeviceFactory()
     resp = admin_client.get(f"/dcim/devices/{device.pk}/serialized_config/")
     assert resp.status_code == HTTPStatus.OK
+
+
+@pytest.mark.django_db
+def test_report_devices(admin_client):
+    report = ReportFactory(passed_results=4, failed_results=2)
+    resp = admin_client.get(f"/plugins/validity/reports/{report.pk}/devices/")
+    assert resp.status_code == HTTPStatus.OK
```

### Comparing `netbox-validity-1.2.1/validity/urls.py` & `netbox-validity-1.3.0/validity/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.1/validity/utils/git.py` & `netbox-validity-1.3.0/validity/utils/git.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.1/validity/utils/misc.py` & `netbox-validity-1.3.0/validity/utils/misc.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.1/validity/utils/password.py` & `netbox-validity-1.3.0/validity/utils/password.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.1/validity/views/__init__.py` & `netbox-validity-1.3.0/validity/views/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.1/validity/views/base.py` & `netbox-validity-1.3.0/validity/views/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,11 @@
+from typing import Any, Dict
+
 from django.db.models import Model
+from django.forms import Form
 from django.shortcuts import get_object_or_404
 from django_filters import FilterSet
 from django_filters.views import FilterView
 from django_tables2 import SingleTableMixin, Table
 from utilities.views import ViewTab
 
 from validity import filtersets, forms, models, tables
@@ -32,55 +35,73 @@
 
     def get_extra_context(self, request, instance):
         table = self.get_table(request, instance)
         self.configure_table(request, table, instance)
         return {"table": table, "search_value": request.GET.get("q", "")}
 
 
-class TestResultBaseView(SingleTableMixin, FilterView):
+class FilterViewWithForm(FilterView):
+    filterform_class: type[Form]
+    exclude_form_fields: tuple[str, ...] = ()
+
+    def get_filterform_exclude(self):
+        return self.exclude_form_fields
+
+    def get_filterform_initial(self):
+        if not hasattr(self.filterset.form, "cleaned_data"):
+            initial = {}
+        else:
+            initial = {
+                k: v for k, v in self.filterset.form.cleaned_data.items() if k in self.filterform_class.base_fields
+            }
+        return initial
+
+    def get_filterform(self):
+        initial = self.get_filterform_initial()
+        exclude = {"exclude": exclude_fields} if (exclude_fields := self.get_filterform_exclude()) else {}
+        form = self.filterform_class(initial=initial, **exclude)
+        return form
+
+    def get_context_data(self, **kwargs: Any) -> Dict[str, Any]:
+        return super().get_context_data(**kwargs) | {"filterset_form": self.get_filterform()}
+
+
+class TestResultBaseView(SingleTableMixin, FilterViewWithForm):
     template_name = "validity/compliance_results.html"
     tab = ViewTab("Test Results", badge=lambda obj: obj.results.count())
     model = models.ComplianceTestResult
     filterset_class = filtersets.ComplianceTestResultFilterSet
-    filter_form_class = forms.TestResultFilterForm
+    filterform_class = forms.TestResultFilterForm
     table_class = tables.ComplianceResultTable
-    permission_required = "validity.view_compliancetestresult."
+    permission_required = "validity.view_compliancetestresult"
 
     parent_model: type[Model]
     result_relation: str
     read_only: bool = False
     exclude_form_fields: tuple[str, ...] = ()
 
     def get_table(self, **kwargs):
-        table = super().get_table(**kwargs)
+        table_class = self.get_table_class()
+        table = table_class(data=self.get_table_data(), **kwargs)
+        table.configure(request=self.request)
         table.exclude = (self.result_relation,)
         return table
 
     def get_queryset(self):
         return models.ComplianceTestResult.objects.select_related("test", "device").filter(
             **{self.result_relation: self.kwargs["pk"]}
         )
 
     def get_object(self):
         return get_object_or_404(self.parent_model, pk=self.kwargs["pk"])
 
-    def get_filterform(self):
-        if not hasattr(self.filterset.form, "cleaned_data"):
-            initial = {}
-        else:
-            initial = {
-                k: v for k, v in self.filterset.form.cleaned_data.items() if k in self.filter_form_class.base_fields
-            }
-        form = self.filter_form_class(
-            initial=initial, exclude=self.exclude_form_fields + (self.result_relation + "_id",)
-        )
-        return form
+    def get_filterform_exclude(self):
+        return super().get_filterform_exclude() + (self.result_relation + "_id",)
 
     def get_context_data(self, **kwargs):
         context = super().get_context_data(**kwargs)
         return context | {
-            "filterset_form": self.get_filterform(),
             "object": self.get_object(),
             "tab": self.tab,
             "read_only": self.read_only,
             "result_relation": self.result_relation,
         }
```

### Comparing `netbox-validity-1.2.1/validity/views/device.py` & `netbox-validity-1.3.0/validity/views/device.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.1/validity/views/git_repo.py` & `netbox-validity-1.3.0/validity/views/git_repo.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.1/validity/views/nameset.py` & `netbox-validity-1.3.0/validity/views/nameset.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.1/validity/views/report.py` & `netbox-validity-1.3.0/validity/views/report.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,20 @@
-from typing import Any, Iterable, Iterator
+import functools
+from typing import Any, Dict, Iterable, Iterator
 
+from django.db.models.query import QuerySet
+from django.shortcuts import get_object_or_404
+from django.utils.translation import gettext_lazy as _
+from django_tables2 import SingleTableMixin
 from netbox.views import generic
-from utilities.views import register_model_view
+from utilities.views import ViewTab, register_model_view
 
-from validity import forms, models, tables
-from validity.choices import DeviceGroupByChoices
-from .base import TestResultBaseView
+from validity import filtersets, forms, models, tables
+from validity.choices import DeviceGroupByChoices, SeverityChoices
+from .base import FilterViewWithForm, TestResultBaseView
 
 
 class ComplianceReportListView(generic.ObjectListView):
     queryset = models.ComplianceReport.objects.annotate_result_stats().count_devices_and_tests().order_by("-created")
     table = tables.ComplianceReportTable
 
     def get_table(self, data, request, bulk_actions=True):
@@ -49,13 +54,59 @@
             table = self.get_table(self.transform_groupby_qs(groupby_qs, groupby_field))
             table.configure(request)
             context["groupby_table"] = table
             context["groupby_label"] = groupby_field.label
         return context
 
 
+@register_model_view(models.ComplianceReport, "devices")
+class ReportDeviceView(SingleTableMixin, FilterViewWithForm):
+    table_class = tables.ComplianceReportDeviceTable
+    tab = ViewTab(
+        "Devices",
+        badge=lambda obj: models.VDevice.objects.filter(results__in=obj.results.all())
+        .order_by("pk")
+        .distinct("pk")
+        .count(),
+    )
+    filterset_class = filtersets.DeviceReportFilterSet
+    permission_required = "view_compliancereport"
+    template_name = "validity/report_devices.html"
+    filterform_class = forms.DeviceReportFilterForm
+
+    @functools.cached_property
+    def object(self):
+        return get_object_or_404(models.ComplianceReport, pk=self.kwargs["pk"])
+
+    def get_queryset(self) -> QuerySet[models.VDevice]:
+        severity_ge = SeverityChoices.from_request(self.request)
+        return (
+            models.VDevice.objects.filter(results__report=self.object)
+            .annotate_result_stats(self.object.pk, severity_ge)
+            .prefetch_results(self.object.pk, severity_ge)
+        )
+
+    def get_filterform_initial(self):
+        return super().get_filterform_initial() | {"severity_ge": SeverityChoices.from_request(self.request)}
+
+    def get_table(self, **kwargs):
+        table_class = self.get_table_class()
+        table = table_class(data=self.get_table_data(), **kwargs)
+        table.configure(self.request)
+        return table
+
+    def get_context_data(self, **kwargs: Any) -> Dict[str, Any]:
+        return super().get_context_data(**kwargs) | {
+            "object": self.object,
+            "tab": self.tab,
+            "read_only": True,
+            "search_button_name": _("Show"),
+        }
+
+
 @register_model_view(models.ComplianceReport, "results")
 class ReportResultView(TestResultBaseView):
     parent_model = models.ComplianceReport
     result_relation = "report"
     read_only = True
     exclude_form_fields = ("latest", "selector_id", "platform_id", "tenant_id", "device_role_id", "manufacturer_id")
+    permission_required = "view_compliancereport"
```

### Comparing `netbox-validity-1.2.1/validity/views/selector.py` & `netbox-validity-1.3.0/validity/views/selector.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.1/validity/views/serializer.py` & `netbox-validity-1.3.0/validity/views/serializer.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.1/validity/views/test.py` & `netbox-validity-1.3.0/validity/views/test.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.1/validity/views/test_result.py` & `netbox-validity-1.3.0/validity/views/test_result.py`

 * *Files identical despite different names*

