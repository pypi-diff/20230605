# Comparing `tmp/tox-4.5.2.tar.gz` & `tmp/tox-4.6.0.tar.gz`

## Comparing `tox-4.5.2.tar` & `tox-4.6.0.tar`

### file list

```diff
@@ -1,222 +1,222 @@
--rw-r--r--   0        0        0     2750 2020-02-02 00:00:00.000000 tox-4.5.2/tox.ini
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/__init__.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/__main__.py
--rw-r--r--   0        0        0     6005 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/provision.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/py.typed
--rw-r--r--   0        0        0    19145 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/pytest.py
--rw-r--r--   0        0        0     8278 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/report.py
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/run.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/__init__.py
--rw-r--r--   0        0        0     6443 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/main.py
--rw-r--r--   0        0        0     4187 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/of_type.py
--rw-r--r--   0        0        0     4806 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/set_env.py
--rw-r--r--   0        0        0     9891 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/sets.py
--rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/cli/__init__.py
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/cli/env_var.py
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/cli/ini.py
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/cli/parse.py
--rw-r--r--   0        0        0    13671 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/cli/parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/loader/__init__.py
--rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/loader/api.py
--rw-r--r--   0        0        0     6411 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/loader/convert.py
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/loader/memory.py
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/loader/section.py
--rw-r--r--   0        0        0     4795 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/loader/str_convert.py
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/loader/stringify.py
--rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/loader/ini/__init__.py
--rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/loader/ini/factor.py
--rw-r--r--   0        0        0    13352 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/loader/ini/replace.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/source/__init__.py
--rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/source/api.py
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/source/discover.py
--rw-r--r--   0        0        0     4387 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/source/ini.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/source/ini_section.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/source/legacy_toml.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/source/setup_cfg.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/config/source/tox_ini.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/execute/__init__.py
--rw-r--r--   0        0        0     9137 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/execute/api.py
--rw-r--r--   0        0        0     5195 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/execute/pep517_backend.py
--rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/execute/request.py
--rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/execute/stream.py
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/execute/util.py
--rw-r--r--   0        0        0    13863 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/execute/local_sub_process/__init__.py
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/execute/local_sub_process/read_via_thread.py
--rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/execute/local_sub_process/read_via_thread_unix.py
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/execute/local_sub_process/read_via_thread_windows.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/journal/__init__.py
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/journal/env.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/journal/main.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/plugin/__init__.py
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/plugin/inline.py
--rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/plugin/manager.py
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/plugin/spec.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/session/__init__.py
--rw-r--r--   0        0        0    18083 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/session/env_select.py
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/session/state.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/session/cmd/__init__.py
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/session/cmd/depends.py
--rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/session/cmd/devenv.py
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/session/cmd/exec_.py
--rw-r--r--   0        0        0     5476 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/session/cmd/legacy.py
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/session/cmd/list_env.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/session/cmd/quickstart.py
--rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/session/cmd/show_config.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/session/cmd/version_flag.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/session/cmd/run/__init__.py
--rw-r--r--   0        0        0    16573 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/session/cmd/run/common.py
--rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/session/cmd/run/parallel.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/session/cmd/run/sequential.py
--rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/session/cmd/run/single.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/tox_env/__init__.py
--rw-r--r--   0        0        0    20134 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/tox_env/api.py
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/tox_env/errors.py
--rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/tox_env/info.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/tox_env/installer.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/tox_env/package.py
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/tox_env/register.py
--rw-r--r--   0        0        0     7761 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/tox_env/runner.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/tox_env/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/tox_env/python/__init__.py
--rw-r--r--   0        0        0    10900 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/tox_env/python/api.py
--rw-r--r--   0        0        0     4863 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/tox_env/python/package.py
--rw-r--r--   0        0        0     4446 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/tox_env/python/runner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/tox_env/python/pip/__init__.py
--rw-r--r--   0        0        0    10355 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/tox_env/python/pip/pip_install.py
--rw-r--r--   0        0        0     5390 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/tox_env/python/pip/req_file.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/tox_env/python/pip/req/__init__.py
--rw-r--r--   0        0        0     4299 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/tox_env/python/pip/req/args.py
--rw-r--r--   0        0        0    19406 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/tox_env/python/pip/req/file.py
--rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/tox_env/python/pip/req/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/tox_env/python/virtual_env/__init__.py
--rw-r--r--   0        0        0     6352 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/tox_env/python/virtual_env/api.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/tox_env/python/virtual_env/runner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/tox_env/python/virtual_env/package/__init__.py
--rw-r--r--   0        0        0     7053 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/tox_env/python/virtual_env/package/cmd_builder.py
--rw-r--r--   0        0        0    17577 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/tox_env/python/virtual_env/package/pyproject.py
--rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/tox_env/python/virtual_env/package/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/util/__init__.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/util/ci.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/util/cpu.py
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/util/file_view.py
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/util/graph.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/util/path.py
--rw-r--r--   0        0        0     6688 2020-02-02 00:00:00.000000 tox-4.5.2/src/tox/util/spinner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/tests/__init__.py
--rw-r--r--   0        0        0     5439 2020-02-02 00:00:00.000000 tox-4.5.2/tests/conftest.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 tox-4.5.2/tests/test_call_modes.py
--rw-r--r--   0        0        0     9796 2020-02-02 00:00:00.000000 tox-4.5.2/tests/test_provision.py
--rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 tox-4.5.2/tests/test_report.py
--rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 tox-4.5.2/tests/test_run.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 tox-4.5.2/tests/test_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/__init__.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/conftest.py
--rw-r--r--   0        0        0     3888 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/test_main.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/test_of_types.py
--rw-r--r--   0        0        0     5827 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/test_set_env.py
--rw-r--r--   0        0        0     7157 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/test_sets.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/test_types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/cli/__init__.py
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/cli/conftest.py
--rw-r--r--   0        0        0     5105 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/cli/test_cli_env_var.py
--rw-r--r--   0        0        0     7197 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/cli/test_cli_ini.py
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/cli/test_parse.py
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/cli/test_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/loader/__init__.py
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/loader/test_loader.py
--rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/loader/test_memory_loader.py
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/loader/test_section.py
--rw-r--r--   0        0        0     7098 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/loader/test_str_convert.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/loader/ini/__init__.py
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/loader/ini/conftest.py
--rw-r--r--   0        0        0     6454 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/loader/ini/test_factor.py
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/loader/ini/test_ini_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/loader/ini/replace/__init__.py
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/loader/ini/replace/conftest.py
--rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/loader/ini/replace/test_replace.py
--rw-r--r--   0        0        0     7159 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/loader/ini/replace/test_replace_env_var.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/loader/ini/replace/test_replace_os_pathsep.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/loader/ini/replace/test_replace_os_sep.py
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/loader/ini/replace/test_replace_posargs.py
--rw-r--r--   0        0        0     8296 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/loader/ini/replace/test_replace_tox_env.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/loader/ini/replace/test_replace_tty.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/source/__init__.py
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/source/test_discover.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/source/test_legacy_toml.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/source/test_setup_cfg.py
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 tox-4.5.2/tests/config/source/test_source_ini.py
--rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 tox-4.5.2/tests/demo_pkg_inline/build.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 tox-4.5.2/tests/demo_pkg_inline/build.pyi
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 tox-4.5.2/tests/demo_pkg_inline/pyproject.toml
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 tox-4.5.2/tests/demo_pkg_setuptools/pyproject.toml
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 tox-4.5.2/tests/demo_pkg_setuptools/setup.cfg
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 tox-4.5.2/tests/demo_pkg_setuptools/demo_pkg_setuptools/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/tests/execute/__init__.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 tox-4.5.2/tests/execute/conftest.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 tox-4.5.2/tests/execute/test_request.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 tox-4.5.2/tests/execute/test_stream.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/tests/execute/local_subprocess/__init__.py
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 tox-4.5.2/tests/execute/local_subprocess/bad_process.py
--rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 tox-4.5.2/tests/execute/local_subprocess/local_subprocess_sigint.py
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 tox-4.5.2/tests/execute/local_subprocess/test_execute_util.py
--rw-r--r--   0        0        0    14088 2020-02-02 00:00:00.000000 tox-4.5.2/tests/execute/local_subprocess/test_local_subprocess.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 tox-4.5.2/tests/execute/local_subprocess/tty_check.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/tests/journal/__init__.py
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 tox-4.5.2/tests/journal/test_main_journal.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 tox-4.5.2/tests/plugin/conftest.py
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 tox-4.5.2/tests/plugin/test_inline.py
--rw-r--r--   0        0        0     9068 2020-02-02 00:00:00.000000 tox-4.5.2/tests/plugin/test_plugin.py
--rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 tox-4.5.2/tests/plugin/test_plugin_custom_config_set.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/tests/pytest_/__init__.py
--rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 tox-4.5.2/tests/pytest_/test_init.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/tests/session/__init__.py
--rw-r--r--   0        0        0     4250 2020-02-02 00:00:00.000000 tox-4.5.2/tests/session/test_env_select.py
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 tox-4.5.2/tests/session/test_session_common.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/tests/session/cmd/__init__.py
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 tox-4.5.2/tests/session/cmd/test_depends.py
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 tox-4.5.2/tests/session/cmd/test_devenv.py
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 tox-4.5.2/tests/session/cmd/test_exec_.py
--rw-r--r--   0        0        0     5552 2020-02-02 00:00:00.000000 tox-4.5.2/tests/session/cmd/test_legacy.py
--rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 tox-4.5.2/tests/session/cmd/test_list_envs.py
--rw-r--r--   0        0        0     5775 2020-02-02 00:00:00.000000 tox-4.5.2/tests/session/cmd/test_parallel.py
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 tox-4.5.2/tests/session/cmd/test_quickstart.py
--rw-r--r--   0        0        0    18713 2020-02-02 00:00:00.000000 tox-4.5.2/tests/session/cmd/test_sequential.py
--rw-r--r--   0        0        0    11209 2020-02-02 00:00:00.000000 tox-4.5.2/tests/session/cmd/test_show_config.py
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 tox-4.5.2/tests/session/cmd/test_state.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/tests/session/cmd/run/__init__.py
--rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 tox-4.5.2/tests/session/cmd/run/test_common.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/tests/tox_env/__init__.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 tox-4.5.2/tests/tox_env/test_api.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 tox-4.5.2/tests/tox_env/test_info.py
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 tox-4.5.2/tests/tox_env/test_register.py
--rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 tox-4.5.2/tests/tox_env/test_tox_env_api.py
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 tox-4.5.2/tests/tox_env/test_tox_env_runner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/tests/tox_env/python/__init__.py
--rw-r--r--   0        0        0     8593 2020-02-02 00:00:00.000000 tox-4.5.2/tests/tox_env/python/test_python_api.py
--rw-r--r--   0        0        0     5428 2020-02-02 00:00:00.000000 tox-4.5.2/tests/tox_env/python/test_python_runner.py
--rw-r--r--   0        0        0    17036 2020-02-02 00:00:00.000000 tox-4.5.2/tests/tox_env/python/pip/test_pip_install.py
--rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 tox-4.5.2/tests/tox_env/python/pip/test_req_file.py
--rw-r--r--   0        0        0    22126 2020-02-02 00:00:00.000000 tox-4.5.2/tests/tox_env/python/pip/req/test_file.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/tests/tox_env/python/test-pkg/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/tests/tox_env/python/virtual_env/__init__.py
--rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 tox-4.5.2/tests/tox_env/python/virtual_env/test_setuptools.py
--rw-r--r--   0        0        0     6537 2020-02-02 00:00:00.000000 tox-4.5.2/tests/tox_env/python/virtual_env/test_virtualenv_api.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/tests/tox_env/python/virtual_env/package/__init__.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 tox-4.5.2/tests/tox_env/python/virtual_env/package/conftest.py
--rw-r--r--   0        0        0     6178 2020-02-02 00:00:00.000000 tox-4.5.2/tests/tox_env/python/virtual_env/package/test_package_cmd_builder.py
--rw-r--r--   0        0        0    10101 2020-02-02 00:00:00.000000 tox-4.5.2/tests/tox_env/python/virtual_env/package/test_package_pyproject.py
--rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 tox-4.5.2/tests/tox_env/python/virtual_env/package/test_python_package_util.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 tox-4.5.2/tests/type_check/add_config_container_factory.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.2/tests/util/__init__.py
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 tox-4.5.2/tests/util/test_ci.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 tox-4.5.2/tests/util/test_cpu.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 tox-4.5.2/tests/util/test_graph.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 tox-4.5.2/tests/util/test_path.py
--rw-r--r--   0        0        0     5091 2020-02-02 00:00:00.000000 tox-4.5.2/tests/util/test_spinner.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 tox-4.5.2/.gitignore
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 tox-4.5.2/LICENSE
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 tox-4.5.2/README.md
--rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 tox-4.5.2/pyproject.toml
--rw-r--r--   0        0        0     4968 2020-02-02 00:00:00.000000 tox-4.5.2/PKG-INFO
+-rw-r--r--   0        0        0     2750 2020-02-02 00:00:00.000000 tox-4.6.0/tox.ini
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/__init__.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/__main__.py
+-rw-r--r--   0        0        0     6005 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/provision.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/py.typed
+-rw-r--r--   0        0        0    19145 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/pytest.py
+-rw-r--r--   0        0        0     8278 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/report.py
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/run.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/__init__.py
+-rw-r--r--   0        0        0     6443 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/main.py
+-rw-r--r--   0        0        0     4187 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/of_type.py
+-rw-r--r--   0        0        0     4806 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/set_env.py
+-rw-r--r--   0        0        0     9891 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/sets.py
+-rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/cli/__init__.py
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/cli/env_var.py
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/cli/ini.py
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/cli/parse.py
+-rw-r--r--   0        0        0    13671 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/cli/parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/loader/__init__.py
+-rw-r--r--   0        0        0     4775 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/loader/api.py
+-rw-r--r--   0        0        0     6411 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/loader/convert.py
+-rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/loader/memory.py
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/loader/section.py
+-rw-r--r--   0        0        0     4795 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/loader/str_convert.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/loader/stringify.py
+-rw-r--r--   0        0        0     3917 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/loader/ini/__init__.py
+-rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/loader/ini/factor.py
+-rw-r--r--   0        0        0    13352 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/loader/ini/replace.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/source/__init__.py
+-rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/source/api.py
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/source/discover.py
+-rw-r--r--   0        0        0     4387 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/source/ini.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/source/ini_section.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/source/legacy_toml.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/source/setup_cfg.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/source/tox_ini.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/execute/__init__.py
+-rw-r--r--   0        0        0     9137 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/execute/api.py
+-rw-r--r--   0        0        0     5195 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/execute/pep517_backend.py
+-rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/execute/request.py
+-rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/execute/stream.py
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/execute/util.py
+-rw-r--r--   0        0        0    13863 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/execute/local_sub_process/__init__.py
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/execute/local_sub_process/read_via_thread.py
+-rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/execute/local_sub_process/read_via_thread_unix.py
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/execute/local_sub_process/read_via_thread_windows.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/journal/__init__.py
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/journal/env.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/journal/main.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/plugin/__init__.py
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/plugin/inline.py
+-rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/plugin/manager.py
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/plugin/spec.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/session/__init__.py
+-rw-r--r--   0        0        0    18083 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/session/env_select.py
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/session/state.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/session/cmd/__init__.py
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/session/cmd/depends.py
+-rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/session/cmd/devenv.py
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/session/cmd/exec_.py
+-rw-r--r--   0        0        0     5476 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/session/cmd/legacy.py
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/session/cmd/list_env.py
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/session/cmd/quickstart.py
+-rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/session/cmd/show_config.py
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/session/cmd/version_flag.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/session/cmd/run/__init__.py
+-rw-r--r--   0        0        0    17112 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/session/cmd/run/common.py
+-rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/session/cmd/run/parallel.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/session/cmd/run/sequential.py
+-rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/session/cmd/run/single.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/tox_env/__init__.py
+-rw-r--r--   0        0        0    20134 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/tox_env/api.py
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/tox_env/errors.py
+-rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/tox_env/info.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/tox_env/installer.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/tox_env/package.py
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/tox_env/register.py
+-rw-r--r--   0        0        0     7761 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/tox_env/runner.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/tox_env/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/tox_env/python/__init__.py
+-rw-r--r--   0        0        0    10872 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/tox_env/python/api.py
+-rw-r--r--   0        0        0     4863 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/tox_env/python/package.py
+-rw-r--r--   0        0        0     4446 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/tox_env/python/runner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/tox_env/python/pip/__init__.py
+-rw-r--r--   0        0        0    10355 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/tox_env/python/pip/pip_install.py
+-rw-r--r--   0        0        0     5390 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/tox_env/python/pip/req_file.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/tox_env/python/pip/req/__init__.py
+-rw-r--r--   0        0        0     4299 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/tox_env/python/pip/req/args.py
+-rw-r--r--   0        0        0    19406 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/tox_env/python/pip/req/file.py
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/tox_env/python/pip/req/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/tox_env/python/virtual_env/__init__.py
+-rw-r--r--   0        0        0     6352 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/tox_env/python/virtual_env/api.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/tox_env/python/virtual_env/runner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/tox_env/python/virtual_env/package/__init__.py
+-rw-r--r--   0        0        0     7053 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/tox_env/python/virtual_env/package/cmd_builder.py
+-rw-r--r--   0        0        0    17577 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/tox_env/python/virtual_env/package/pyproject.py
+-rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/tox_env/python/virtual_env/package/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/util/__init__.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/util/ci.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/util/cpu.py
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/util/file_view.py
+-rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/util/graph.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/util/path.py
+-rw-r--r--   0        0        0     6688 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/util/spinner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/tests/__init__.py
+-rw-r--r--   0        0        0     5439 2020-02-02 00:00:00.000000 tox-4.6.0/tests/conftest.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 tox-4.6.0/tests/test_call_modes.py
+-rw-r--r--   0        0        0     9796 2020-02-02 00:00:00.000000 tox-4.6.0/tests/test_provision.py
+-rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 tox-4.6.0/tests/test_report.py
+-rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 tox-4.6.0/tests/test_run.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 tox-4.6.0/tests/test_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/__init__.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/conftest.py
+-rw-r--r--   0        0        0     3888 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/test_main.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/test_of_types.py
+-rw-r--r--   0        0        0     5827 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/test_set_env.py
+-rw-r--r--   0        0        0     7157 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/test_sets.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/test_types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/cli/__init__.py
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/cli/conftest.py
+-rw-r--r--   0        0        0     5211 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/cli/test_cli_env_var.py
+-rw-r--r--   0        0        0     7303 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/cli/test_cli_ini.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/cli/test_parse.py
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/cli/test_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/loader/__init__.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/loader/test_loader.py
+-rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/loader/test_memory_loader.py
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/loader/test_section.py
+-rw-r--r--   0        0        0     7098 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/loader/test_str_convert.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/loader/ini/__init__.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/loader/ini/conftest.py
+-rw-r--r--   0        0        0     6454 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/loader/ini/test_factor.py
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/loader/ini/test_ini_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/loader/ini/replace/__init__.py
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/loader/ini/replace/conftest.py
+-rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/loader/ini/replace/test_replace.py
+-rw-r--r--   0        0        0     7159 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/loader/ini/replace/test_replace_env_var.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/loader/ini/replace/test_replace_os_pathsep.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/loader/ini/replace/test_replace_os_sep.py
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/loader/ini/replace/test_replace_posargs.py
+-rw-r--r--   0        0        0     8296 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/loader/ini/replace/test_replace_tox_env.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/loader/ini/replace/test_replace_tty.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/source/__init__.py
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/source/test_discover.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/source/test_legacy_toml.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/source/test_setup_cfg.py
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/source/test_source_ini.py
+-rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 tox-4.6.0/tests/demo_pkg_inline/build.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 tox-4.6.0/tests/demo_pkg_inline/build.pyi
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 tox-4.6.0/tests/demo_pkg_inline/pyproject.toml
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 tox-4.6.0/tests/demo_pkg_setuptools/pyproject.toml
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 tox-4.6.0/tests/demo_pkg_setuptools/setup.cfg
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 tox-4.6.0/tests/demo_pkg_setuptools/demo_pkg_setuptools/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/tests/execute/__init__.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 tox-4.6.0/tests/execute/conftest.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 tox-4.6.0/tests/execute/test_request.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 tox-4.6.0/tests/execute/test_stream.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/tests/execute/local_subprocess/__init__.py
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 tox-4.6.0/tests/execute/local_subprocess/bad_process.py
+-rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 tox-4.6.0/tests/execute/local_subprocess/local_subprocess_sigint.py
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 tox-4.6.0/tests/execute/local_subprocess/test_execute_util.py
+-rw-r--r--   0        0        0    14088 2020-02-02 00:00:00.000000 tox-4.6.0/tests/execute/local_subprocess/test_local_subprocess.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 tox-4.6.0/tests/execute/local_subprocess/tty_check.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/tests/journal/__init__.py
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 tox-4.6.0/tests/journal/test_main_journal.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 tox-4.6.0/tests/plugin/conftest.py
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 tox-4.6.0/tests/plugin/test_inline.py
+-rw-r--r--   0        0        0     9068 2020-02-02 00:00:00.000000 tox-4.6.0/tests/plugin/test_plugin.py
+-rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 tox-4.6.0/tests/plugin/test_plugin_custom_config_set.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/tests/pytest_/__init__.py
+-rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 tox-4.6.0/tests/pytest_/test_init.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/tests/session/__init__.py
+-rw-r--r--   0        0        0     4250 2020-02-02 00:00:00.000000 tox-4.6.0/tests/session/test_env_select.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 tox-4.6.0/tests/session/test_session_common.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/tests/session/cmd/__init__.py
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 tox-4.6.0/tests/session/cmd/test_depends.py
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 tox-4.6.0/tests/session/cmd/test_devenv.py
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 tox-4.6.0/tests/session/cmd/test_exec_.py
+-rw-r--r--   0        0        0     5552 2020-02-02 00:00:00.000000 tox-4.6.0/tests/session/cmd/test_legacy.py
+-rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 tox-4.6.0/tests/session/cmd/test_list_envs.py
+-rw-r--r--   0        0        0     5775 2020-02-02 00:00:00.000000 tox-4.6.0/tests/session/cmd/test_parallel.py
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 tox-4.6.0/tests/session/cmd/test_quickstart.py
+-rw-r--r--   0        0        0    18713 2020-02-02 00:00:00.000000 tox-4.6.0/tests/session/cmd/test_sequential.py
+-rw-r--r--   0        0        0    11209 2020-02-02 00:00:00.000000 tox-4.6.0/tests/session/cmd/test_show_config.py
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 tox-4.6.0/tests/session/cmd/test_state.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/tests/session/cmd/run/__init__.py
+-rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 tox-4.6.0/tests/session/cmd/run/test_common.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/tests/tox_env/__init__.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 tox-4.6.0/tests/tox_env/test_api.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 tox-4.6.0/tests/tox_env/test_info.py
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 tox-4.6.0/tests/tox_env/test_register.py
+-rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 tox-4.6.0/tests/tox_env/test_tox_env_api.py
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 tox-4.6.0/tests/tox_env/test_tox_env_runner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/tests/tox_env/python/__init__.py
+-rw-r--r--   0        0        0     9199 2020-02-02 00:00:00.000000 tox-4.6.0/tests/tox_env/python/test_python_api.py
+-rw-r--r--   0        0        0     5428 2020-02-02 00:00:00.000000 tox-4.6.0/tests/tox_env/python/test_python_runner.py
+-rw-r--r--   0        0        0    17036 2020-02-02 00:00:00.000000 tox-4.6.0/tests/tox_env/python/pip/test_pip_install.py
+-rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 tox-4.6.0/tests/tox_env/python/pip/test_req_file.py
+-rw-r--r--   0        0        0    22126 2020-02-02 00:00:00.000000 tox-4.6.0/tests/tox_env/python/pip/req/test_file.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/tests/tox_env/python/test-pkg/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/tests/tox_env/python/virtual_env/__init__.py
+-rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 tox-4.6.0/tests/tox_env/python/virtual_env/test_setuptools.py
+-rw-r--r--   0        0        0     6537 2020-02-02 00:00:00.000000 tox-4.6.0/tests/tox_env/python/virtual_env/test_virtualenv_api.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/tests/tox_env/python/virtual_env/package/__init__.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 tox-4.6.0/tests/tox_env/python/virtual_env/package/conftest.py
+-rw-r--r--   0        0        0     6178 2020-02-02 00:00:00.000000 tox-4.6.0/tests/tox_env/python/virtual_env/package/test_package_cmd_builder.py
+-rw-r--r--   0        0        0    10101 2020-02-02 00:00:00.000000 tox-4.6.0/tests/tox_env/python/virtual_env/package/test_package_pyproject.py
+-rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 tox-4.6.0/tests/tox_env/python/virtual_env/package/test_python_package_util.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 tox-4.6.0/tests/type_check/add_config_container_factory.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/tests/util/__init__.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 tox-4.6.0/tests/util/test_ci.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 tox-4.6.0/tests/util/test_cpu.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 tox-4.6.0/tests/util/test_graph.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 tox-4.6.0/tests/util/test_path.py
+-rw-r--r--   0        0        0     5091 2020-02-02 00:00:00.000000 tox-4.6.0/tests/util/test_spinner.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 tox-4.6.0/.gitignore
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 tox-4.6.0/LICENSE
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 tox-4.6.0/README.md
+-rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 tox-4.6.0/pyproject.toml
+-rw-r--r--   0        0        0     4968 2020-02-02 00:00:00.000000 tox-4.6.0/PKG-INFO
```

### Comparing `tox-4.5.2/tox.ini` & `tox-4.6.0/tox.ini`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/provision.py` & `tox-4.6.0/src/tox/provision.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/pytest.py` & `tox-4.6.0/src/tox/pytest.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/report.py` & `tox-4.6.0/src/tox/report.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/run.py` & `tox-4.6.0/src/tox/run.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/config/main.py` & `tox-4.6.0/src/tox/config/main.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/config/of_type.py` & `tox-4.6.0/src/tox/config/of_type.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/config/set_env.py` & `tox-4.6.0/src/tox/config/set_env.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/config/sets.py` & `tox-4.6.0/src/tox/config/sets.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/config/types.py` & `tox-4.6.0/src/tox/config/types.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/config/cli/env_var.py` & `tox-4.6.0/src/tox/config/cli/env_var.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/config/cli/ini.py` & `tox-4.6.0/src/tox/config/cli/ini.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/config/cli/parse.py` & `tox-4.6.0/src/tox/config/cli/parse.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/config/cli/parser.py` & `tox-4.6.0/src/tox/config/cli/parser.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/config/loader/api.py` & `tox-4.6.0/src/tox/config/loader/api.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from __future__ import annotations
 
 from abc import abstractmethod
 from argparse import ArgumentTypeError
-from concurrent.futures import Future
-from contextlib import contextmanager
-from typing import TYPE_CHECKING, Any, Generator, List, Mapping, TypeVar
+from typing import TYPE_CHECKING, Any, List, Mapping, TypeVar
 
 from tox.plugin import impl
 
 from .convert import Convert, Factory
 from .section import Section
 from .str_convert import StrConvert
 
@@ -118,41 +116,36 @@
         :param conf: the configuration object of this tox session (needed to manifest the value)
         :param args: the config load arguments
         :return: the converted type
         """
         if key in self.overrides:
             return _STR_CONVERT.to(self.overrides[key].value, of_type, factory)
         raw = self.load_raw(key, conf, args.env_name)
-        future: Future[V] = Future()
-        with self.build(future, key, of_type, conf, raw, args) as prepared:
-            converted = self.to(prepared, of_type, factory)
-            future.set_result(converted)
-        return converted
+        return self.build(key, of_type, factory, conf, raw, args)
 
-    @contextmanager
     def build(
         self,
-        future: Future[V],  # noqa: U100
         key: str,  # noqa: U100
-        of_type: type[V],  # noqa: U100
+        of_type: type[V],
+        factory: Factory[V],
         conf: Config | None,  # noqa: U100
         raw: T,
         args: ConfigLoadArgs,  # noqa: U100
-    ) -> Generator[T, None, None]:
+    ) -> V:
         """
         Materialize the raw configuration value from the loader.
 
         :param future: a future which when called will provide the converted config value
         :param key: the config key
         :param of_type: the config type
         :param conf: the global config
         :param raw: the raw value
         :param args: env args
         """
-        yield raw
+        return self.to(raw, of_type, factory)
 
 
 @impl
 def tox_add_option(parser: ToxParser) -> None:
     parser.add_argument(
         "-x",
         "--override",
```

### Comparing `tox-4.5.2/src/tox/config/loader/convert.py` & `tox-4.6.0/src/tox/config/loader/convert.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/config/loader/memory.py` & `tox-4.6.0/src/tox/config/loader/memory.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/config/loader/section.py` & `tox-4.6.0/src/tox/config/loader/section.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/config/loader/str_convert.py` & `tox-4.6.0/src/tox/config/loader/str_convert.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/config/loader/stringify.py` & `tox-4.6.0/src/tox/config/loader/stringify.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/config/loader/ini/__init__.py` & `tox-4.6.0/src/tox/config/loader/ini/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from __future__ import annotations
 
 import inspect
 import re
-from concurrent.futures import Future
 from configparser import ConfigParser, SectionProxy
-from contextlib import contextmanager
-from typing import TYPE_CHECKING, Generator, TypeVar
+from typing import TYPE_CHECKING, TypeVar
 
 from tox.config.loader.api import ConfigLoadArgs, Loader, Override
+from tox.config.loader.convert import Factory
 from tox.config.loader.ini.factor import filter_for_env
 from tox.config.loader.ini.replace import replace
 from tox.config.loader.section import Section
 from tox.config.loader.str_convert import StrConvert
 from tox.config.set_env import SetEnv
 from tox.report import HandledError
 
@@ -53,24 +52,23 @@
         if conf is None:  # conf is None when we're loading the global tox configuration file for the CLI
             factor_filtered = strip_comments  # we don't support factor and replace functionality there
         else:
             factor_filtered = filter_for_env(strip_comments, env_name)  # select matching factors
         collapsed = factor_filtered.replace("\r", "").replace("\\\n", "")  # collapse explicit new-line escape
         return collapsed
 
-    @contextmanager
     def build(
         self,
-        future: Future[V],
         key: str,
         of_type: type[V],
+        factory: Factory[V],
         conf: Config | None,
         raw: str,
         args: ConfigLoadArgs,
-    ) -> Generator[str, None, None]:
+    ) -> V:
         delay_replace = inspect.isclass(of_type) and issubclass(of_type, SetEnv)
 
         def replacer(raw_: str, args_: ConfigLoadArgs) -> str:
             if conf is None:
                 replaced = raw_  # no replacement supported in the core section
             else:
                 try:
@@ -79,20 +77,19 @@
                     if isinstance(exception, HandledError):
                         raise
                     name = self.core_section.key if args_.env_name is None else args_.env_name
                     msg = f"replace failed in {name}.{key} with {exception!r}"
                     raise HandledError(msg) from exception
             return replaced
 
-        if not delay_replace:
-            raw = replacer(raw, args)
-        yield raw
+        prepared = replacer(raw, args) if not delay_replace else raw
+        converted = self.to(prepared, of_type, factory)
         if delay_replace:
-            converted = future.result()
             converted.use_replacer(replacer, args)  # type: ignore[attr-defined] # this can be only set_env that has it
+        return converted
 
     def found_keys(self) -> set[str]:
         return set(self._section_proxy.keys())
 
     def get_section(self, name: str) -> SectionProxy | None:
         # needed for non tox environment replacements
         if self._parser.has_section(name):
```

### Comparing `tox-4.5.2/src/tox/config/loader/ini/factor.py` & `tox-4.6.0/src/tox/config/loader/ini/factor.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/config/loader/ini/replace.py` & `tox-4.6.0/src/tox/config/loader/ini/replace.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/config/source/api.py` & `tox-4.6.0/src/tox/config/source/api.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/config/source/discover.py` & `tox-4.6.0/src/tox/config/source/discover.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/config/source/ini.py` & `tox-4.6.0/src/tox/config/source/ini.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/config/source/ini_section.py` & `tox-4.6.0/src/tox/config/source/ini_section.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/config/source/legacy_toml.py` & `tox-4.6.0/src/tox/config/source/legacy_toml.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/execute/api.py` & `tox-4.6.0/src/tox/execute/api.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/execute/pep517_backend.py` & `tox-4.6.0/src/tox/execute/pep517_backend.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/execute/request.py` & `tox-4.6.0/src/tox/execute/request.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/execute/stream.py` & `tox-4.6.0/src/tox/execute/stream.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/execute/util.py` & `tox-4.6.0/src/tox/execute/util.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/execute/local_sub_process/__init__.py` & `tox-4.6.0/src/tox/execute/local_sub_process/__init__.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/execute/local_sub_process/read_via_thread.py` & `tox-4.6.0/src/tox/execute/local_sub_process/read_via_thread.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/execute/local_sub_process/read_via_thread_unix.py` & `tox-4.6.0/src/tox/execute/local_sub_process/read_via_thread_unix.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/execute/local_sub_process/read_via_thread_windows.py` & `tox-4.6.0/src/tox/execute/local_sub_process/read_via_thread_windows.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/journal/env.py` & `tox-4.6.0/src/tox/journal/env.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/journal/main.py` & `tox-4.6.0/src/tox/journal/main.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/plugin/__init__.py` & `tox-4.6.0/src/tox/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/plugin/inline.py` & `tox-4.6.0/src/tox/plugin/inline.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/plugin/manager.py` & `tox-4.6.0/src/tox/plugin/manager.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/plugin/spec.py` & `tox-4.6.0/src/tox/plugin/spec.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/session/env_select.py` & `tox-4.6.0/src/tox/session/env_select.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/session/state.py` & `tox-4.6.0/src/tox/session/state.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/session/cmd/depends.py` & `tox-4.6.0/src/tox/session/cmd/depends.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/session/cmd/devenv.py` & `tox-4.6.0/src/tox/session/cmd/devenv.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/session/cmd/exec_.py` & `tox-4.6.0/src/tox/session/cmd/exec_.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/session/cmd/legacy.py` & `tox-4.6.0/src/tox/session/cmd/legacy.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/session/cmd/list_env.py` & `tox-4.6.0/src/tox/session/cmd/list_env.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/session/cmd/quickstart.py` & `tox-4.6.0/src/tox/session/cmd/quickstart.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/session/cmd/show_config.py` & `tox-4.6.0/src/tox/session/cmd/show_config.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/session/cmd/version_flag.py` & `tox-4.6.0/src/tox/session/cmd/version_flag.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/session/cmd/run/common.py` & `tox-4.6.0/src/tox/session/cmd/run/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from tox.config.types import EnvList
 from tox.execute import Outcome
 from tox.journal import write_journal
 from tox.session.cmd.run.single import ToxEnvRunResult, run_one
 from tox.session.state import State
 from tox.tox_env.api import ToxEnv
 from tox.tox_env.runner import RunToxEnv
+from tox.util.ci import is_ci
 from tox.util.graph import stable_topological_sort
 from tox.util.spinner import MISS_DURATION, Spinner
 
 
 class SkipMissingInterpreterAction(Action):
     def __call__(
         self,
@@ -152,14 +153,27 @@
     if mode not in ("depends",):
         parser.add_argument(
             "--no-recreate-pkg",
             dest="no_recreate_pkg",
             help="if recreate is set do not recreate packaging tox environment(s)",
             action="store_true",
         )
+        list_deps = parser.add_mutually_exclusive_group()
+        list_deps.add_argument(
+            "--list-dependencies",
+            action="store_true",
+            default=is_ci(),
+            help="list the dependencies installed during environment setup",
+        )
+        list_deps.add_argument(
+            "--no-list-dependencies",
+            action="store_false",
+            dest="list_dependencies",
+            help="never list the dependencies installed during environment setup",
+        )
     if mode not in ("devenv", "config", "depends"):
         parser.add_argument(
             "--skip-pkg-install",
             dest="skip_pkg_install",
             help="skip package installation for this run",
             action="store_true",
         )
```

### Comparing `tox-4.5.2/src/tox/session/cmd/run/parallel.py` & `tox-4.6.0/src/tox/session/cmd/run/parallel.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/session/cmd/run/sequential.py` & `tox-4.6.0/src/tox/session/cmd/run/sequential.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/session/cmd/run/single.py` & `tox-4.6.0/src/tox/session/cmd/run/single.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/tox_env/api.py` & `tox-4.6.0/src/tox/tox_env/api.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/tox_env/info.py` & `tox-4.6.0/src/tox/tox_env/info.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/tox_env/installer.py` & `tox-4.6.0/src/tox/tox_env/installer.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/tox_env/package.py` & `tox-4.6.0/src/tox/tox_env/package.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/tox_env/register.py` & `tox-4.6.0/src/tox/tox_env/register.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/tox_env/runner.py` & `tox-4.6.0/src/tox/tox_env/runner.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/tox_env/util.py` & `tox-4.6.0/src/tox/tox_env/util.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/tox_env/python/api.py` & `tox-4.6.0/src/tox/tox_env/python/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from typing import Any, List, NamedTuple, cast
 
 from virtualenv.discovery.py_spec import PythonSpec
 
 from tox.config.main import Config
 from tox.tox_env.api import ToxEnv, ToxEnvCreateArgs
 from tox.tox_env.errors import Fail, Recreate, Skip
-from tox.util.ci import is_ci
 
 
 class VersionInfo(NamedTuple):
     major: int
     minor: int
     micro: int
     releaselevel: str
@@ -223,20 +222,19 @@
     @abstractmethod
     def prepend_env_var_path(self) -> list[Path]:
         raise NotImplementedError
 
     def _done_with_setup(self) -> None:
         """called when setup is done"""
         super()._done_with_setup()
-        running_in_ci = is_ci()
-        if self.journal or running_in_ci:
+        if self.journal or self.options.list_dependencies:
             outcome = self.installer.installed()
             if self.journal:
                 self.journal["installed_packages"] = outcome
-            if running_in_ci:
+            if self.options.list_dependencies:
                 logging.warning(",".join(outcome))
 
     def python_cache(self) -> dict[str, Any]:
         return {
             "version_info": list(self.base_python.version_info),
         }
```

### Comparing `tox-4.5.2/src/tox/tox_env/python/package.py` & `tox-4.6.0/src/tox/tox_env/python/package.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/tox_env/python/runner.py` & `tox-4.6.0/src/tox/tox_env/python/runner.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/tox_env/python/pip/pip_install.py` & `tox-4.6.0/src/tox/tox_env/python/pip/pip_install.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/tox_env/python/pip/req_file.py` & `tox-4.6.0/src/tox/tox_env/python/pip/req_file.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/tox_env/python/pip/req/args.py` & `tox-4.6.0/src/tox/tox_env/python/pip/req/args.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/tox_env/python/pip/req/file.py` & `tox-4.6.0/src/tox/tox_env/python/pip/req/file.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/tox_env/python/pip/req/util.py` & `tox-4.6.0/src/tox/tox_env/python/pip/req/util.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/tox_env/python/virtual_env/api.py` & `tox-4.6.0/src/tox/tox_env/python/virtual_env/api.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/tox_env/python/virtual_env/runner.py` & `tox-4.6.0/src/tox/tox_env/python/virtual_env/runner.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/tox_env/python/virtual_env/package/cmd_builder.py` & `tox-4.6.0/src/tox/tox_env/python/virtual_env/package/cmd_builder.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/tox_env/python/virtual_env/package/pyproject.py` & `tox-4.6.0/src/tox/tox_env/python/virtual_env/package/pyproject.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/tox_env/python/virtual_env/package/util.py` & `tox-4.6.0/src/tox/tox_env/python/virtual_env/package/util.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/util/ci.py` & `tox-4.6.0/src/tox/util/ci.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/util/file_view.py` & `tox-4.6.0/src/tox/util/file_view.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/util/graph.py` & `tox-4.6.0/src/tox/util/graph.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/util/path.py` & `tox-4.6.0/src/tox/util/path.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/src/tox/util/spinner.py` & `tox-4.6.0/src/tox/util/spinner.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/conftest.py` & `tox-4.6.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/test_provision.py` & `tox-4.6.0/tests/test_provision.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/test_report.py` & `tox-4.6.0/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/test_run.py` & `tox-4.6.0/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/test_version.py` & `tox-4.6.0/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/config/test_main.py` & `tox-4.6.0/tests/config/test_main.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/config/test_of_types.py` & `tox-4.6.0/tests/config/test_of_types.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/config/test_set_env.py` & `tox-4.6.0/tests/config/test_set_env.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/config/test_sets.py` & `tox-4.6.0/tests/config/test_sets.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/config/test_types.py` & `tox-4.6.0/tests/config/test_types.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/config/cli/conftest.py` & `tox-4.6.0/tests/config/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/config/cli/test_cli_env_var.py` & `tox-4.6.0/tests/config/cli/test_cli_env_var.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import pytest
 
 from tox.config.cli.parse import get_options
 from tox.config.loader.api import Override
 from tox.pytest import CaptureFixture, LogCaptureFixture, MonkeyPatch
 from tox.session.env_select import CliEnv
 from tox.session.state import State
+from tox.util.ci import is_ci
 
 
 def test_verbose() -> None:
     parsed, _, __, ___, ____ = get_options("-v", "-v")
     assert parsed.verbosity == 4
 
 
@@ -59,14 +60,15 @@
         "parallel": 0,
         "parallel_live": False,
         "parallel_no_spinner": False,
         "pre": False,
         "factors": [],
         "labels": [],
         "skip_env": "",
+        "list_dependencies": is_ci(),
     }
 
 
 def test_env_var_exhaustive_parallel_values(
     monkeypatch: MonkeyPatch,
     core_handlers: dict[str, Callable[[State], int]],
 ) -> None:
@@ -117,14 +119,15 @@
         "work_dir": None,
         "root_dir": None,
         "config_file": None,
         "factors": [],
         "labels": [],
         "exit_and_dump_after": 0,
         "skip_env": "",
+        "list_dependencies": is_ci(),
     }
     assert options.parsed.verbosity == 4
     assert options.cmd_handlers == core_handlers
 
 
 def test_ini_help(monkeypatch: MonkeyPatch, capsys: CaptureFixture) -> None:
     monkeypatch.setenv("TOX_VERBOSE", "5")
```

### Comparing `tox-4.5.2/tests/config/cli/test_cli_ini.py` & `tox-4.6.0/tests/config/cli/test_cli_ini.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from tox.config.cli.parser import Parsed
 from tox.config.loader.api import Override
 from tox.config.main import Config
 from tox.config.source import discover_source
 from tox.pytest import CaptureFixture, LogCaptureFixture, MonkeyPatch
 from tox.session.env_select import CliEnv
 from tox.session.state import State
+from tox.util.ci import is_ci
 
 
 @pytest.fixture()
 def exhaustive_ini(tmp_path: Path, monkeypatch: MonkeyPatch) -> Path:
     to = tmp_path / "tox.ini"
     to.write_text(
         textwrap.dedent(
@@ -98,14 +99,15 @@
         "work_dir": None,
         "root_dir": None,
         "config_file": None,
         "factors": [],
         "labels": [],
         "exit_and_dump_after": 0,
         "skip_env": "",
+        "list_dependencies": is_ci(),
     }
 
 
 @pytest.mark.usefixtures("exhaustive_ini")
 def test_ini_exhaustive_parallel_values(core_handlers: dict[str, Callable[[State], int]]) -> None:
     options = get_options("p")
     assert vars(options.parsed) == {
@@ -135,14 +137,15 @@
         "work_dir": None,
         "root_dir": None,
         "config_file": None,
         "factors": [],
         "labels": [],
         "exit_and_dump_after": 0,
         "skip_env": "",
+        "list_dependencies": is_ci(),
     }
     assert options.parsed.verbosity == 4
     assert options.cmd_handlers == core_handlers
 
 
 def test_ini_help(exhaustive_ini: Path, capsys: CaptureFixture) -> None:
     with pytest.raises(SystemExit) as context:
```

### Comparing `tox-4.5.2/tests/config/cli/test_parse.py` & `tox-4.6.0/tests/config/cli/test_parse.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/config/cli/test_parser.py` & `tox-4.6.0/tests/config/cli/test_parser.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/config/loader/test_loader.py` & `tox-4.6.0/tests/config/loader/test_loader.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/config/loader/test_memory_loader.py` & `tox-4.6.0/tests/config/loader/test_memory_loader.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/config/loader/test_section.py` & `tox-4.6.0/tests/config/loader/test_section.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/config/loader/test_str_convert.py` & `tox-4.6.0/tests/config/loader/test_str_convert.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/config/loader/ini/conftest.py` & `tox-4.6.0/tests/config/loader/ini/conftest.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/config/loader/ini/test_factor.py` & `tox-4.6.0/tests/config/loader/ini/test_factor.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/config/loader/ini/test_ini_loader.py` & `tox-4.6.0/tests/config/loader/ini/test_ini_loader.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/config/loader/ini/replace/conftest.py` & `tox-4.6.0/tests/config/loader/ini/replace/conftest.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/config/loader/ini/replace/test_replace.py` & `tox-4.6.0/tests/config/loader/ini/replace/test_replace.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/config/loader/ini/replace/test_replace_env_var.py` & `tox-4.6.0/tests/config/loader/ini/replace/test_replace_env_var.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/config/loader/ini/replace/test_replace_os_sep.py` & `tox-4.6.0/tests/config/loader/ini/replace/test_replace_os_sep.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/config/loader/ini/replace/test_replace_posargs.py` & `tox-4.6.0/tests/config/loader/ini/replace/test_replace_posargs.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/config/loader/ini/replace/test_replace_tox_env.py` & `tox-4.6.0/tests/config/loader/ini/replace/test_replace_tox_env.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/config/loader/ini/replace/test_replace_tty.py` & `tox-4.6.0/tests/config/loader/ini/replace/test_replace_tty.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/config/source/test_discover.py` & `tox-4.6.0/tests/config/source/test_discover.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/config/source/test_setup_cfg.py` & `tox-4.6.0/tests/config/source/test_setup_cfg.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/config/source/test_source_ini.py` & `tox-4.6.0/tests/config/source/test_source_ini.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/demo_pkg_inline/build.py` & `tox-4.6.0/tests/demo_pkg_inline/build.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/demo_pkg_inline/build.pyi` & `tox-4.6.0/tests/demo_pkg_inline/build.pyi`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/execute/test_request.py` & `tox-4.6.0/tests/execute/test_request.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/execute/local_subprocess/bad_process.py` & `tox-4.6.0/tests/execute/local_subprocess/bad_process.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/execute/local_subprocess/local_subprocess_sigint.py` & `tox-4.6.0/tests/execute/local_subprocess/local_subprocess_sigint.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/execute/local_subprocess/test_execute_util.py` & `tox-4.6.0/tests/execute/local_subprocess/test_execute_util.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/execute/local_subprocess/test_local_subprocess.py` & `tox-4.6.0/tests/execute/local_subprocess/test_local_subprocess.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/journal/test_main_journal.py` & `tox-4.6.0/tests/journal/test_main_journal.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/plugin/test_inline.py` & `tox-4.6.0/tests/plugin/test_inline.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/plugin/test_plugin.py` & `tox-4.6.0/tests/plugin/test_plugin.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/plugin/test_plugin_custom_config_set.py` & `tox-4.6.0/tests/plugin/test_plugin_custom_config_set.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/pytest_/test_init.py` & `tox-4.6.0/tests/pytest_/test_init.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/session/test_env_select.py` & `tox-4.6.0/tests/session/test_env_select.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/session/test_session_common.py` & `tox-4.6.0/tests/session/test_session_common.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/session/cmd/test_depends.py` & `tox-4.6.0/tests/session/cmd/test_depends.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/session/cmd/test_devenv.py` & `tox-4.6.0/tests/session/cmd/test_devenv.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/session/cmd/test_exec_.py` & `tox-4.6.0/tests/session/cmd/test_exec_.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/session/cmd/test_legacy.py` & `tox-4.6.0/tests/session/cmd/test_legacy.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/session/cmd/test_list_envs.py` & `tox-4.6.0/tests/session/cmd/test_list_envs.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/session/cmd/test_parallel.py` & `tox-4.6.0/tests/session/cmd/test_parallel.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/session/cmd/test_quickstart.py` & `tox-4.6.0/tests/session/cmd/test_quickstart.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/session/cmd/test_sequential.py` & `tox-4.6.0/tests/session/cmd/test_sequential.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/session/cmd/test_show_config.py` & `tox-4.6.0/tests/session/cmd/test_show_config.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/session/cmd/test_state.py` & `tox-4.6.0/tests/session/cmd/test_state.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/session/cmd/run/test_common.py` & `tox-4.6.0/tests/session/cmd/run/test_common.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/tox_env/test_api.py` & `tox-4.6.0/tests/tox_env/test_api.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/tox_env/test_register.py` & `tox-4.6.0/tests/tox_env/test_register.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/tox_env/test_tox_env_api.py` & `tox-4.6.0/tests/tox_env/test_tox_env_api.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/tox_env/test_tox_env_runner.py` & `tox-4.6.0/tests/tox_env/test_tox_env_runner.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/tox_env/python/test_python_api.py` & `tox-4.6.0/tests/tox_env/python/test_python_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -214,13 +214,29 @@
     result = tox_project({"tox.ini": ""}).run("r", "-e", "py", "--hashseed", "ok")
     result.assert_failed(2)
     assert "tox run: error: argument --hashseed: invalid literal for int() with base 10: 'ok'" in result.err
 
 
 @pytest.mark.parametrize("in_ci", [True, False])
 def test_list_installed_deps(in_ci: bool, tox_project: ToxProjectCreator, mocker: MockerFixture) -> None:
-    mocker.patch("tox.tox_env.python.api.is_ci", return_value=in_ci)
+    mocker.patch("tox.session.cmd.run.common.is_ci", return_value=in_ci)
     result = tox_project({"tox.ini": "[testenv]\nskip_install = true"}).run("r", "-e", "py")
     if in_ci:
         assert "pip==" in result.out
     else:
         assert "pip==" not in result.out
+
+
+@pytest.mark.parametrize("list_deps", ["--list-dependencies", "--no-list-dependencies"])
+@pytest.mark.parametrize("in_ci", [True, False])
+def test_list_installed_deps_explicit_cli(
+    list_deps: str,
+    in_ci: bool,
+    tox_project: ToxProjectCreator,
+    mocker: MockerFixture,
+) -> None:
+    mocker.patch("tox.session.cmd.run.common.is_ci", return_value=in_ci)
+    result = tox_project({"tox.ini": "[testenv]\nskip_install = true"}).run(list_deps, "r", "-e", "py")
+    if list_deps == "--list-dependencies":
+        assert "pip==" in result.out
+    else:
+        assert "pip==" not in result.out
```

### Comparing `tox-4.5.2/tests/tox_env/python/test_python_runner.py` & `tox-4.6.0/tests/tox_env/python/test_python_runner.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/tox_env/python/pip/test_pip_install.py` & `tox-4.6.0/tests/tox_env/python/pip/test_pip_install.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/tox_env/python/pip/test_req_file.py` & `tox-4.6.0/tests/tox_env/python/pip/test_req_file.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/tox_env/python/pip/req/test_file.py` & `tox-4.6.0/tests/tox_env/python/pip/req/test_file.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/tox_env/python/virtual_env/test_setuptools.py` & `tox-4.6.0/tests/tox_env/python/virtual_env/test_setuptools.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/tox_env/python/virtual_env/test_virtualenv_api.py` & `tox-4.6.0/tests/tox_env/python/virtual_env/test_virtualenv_api.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/tox_env/python/virtual_env/package/conftest.py` & `tox-4.6.0/tests/tox_env/python/virtual_env/package/conftest.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/tox_env/python/virtual_env/package/test_package_cmd_builder.py` & `tox-4.6.0/tests/tox_env/python/virtual_env/package/test_package_cmd_builder.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/tox_env/python/virtual_env/package/test_package_pyproject.py` & `tox-4.6.0/tests/tox_env/python/virtual_env/package/test_package_pyproject.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/tox_env/python/virtual_env/package/test_python_package_util.py` & `tox-4.6.0/tests/tox_env/python/virtual_env/package/test_python_package_util.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/util/test_ci.py` & `tox-4.6.0/tests/util/test_ci.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/util/test_graph.py` & `tox-4.6.0/tests/util/test_graph.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/tests/util/test_spinner.py` & `tox-4.6.0/tests/util/test_spinner.py`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/LICENSE` & `tox-4.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/README.md` & `tox-4.6.0/README.md`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/pyproject.toml` & `tox-4.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tox-4.5.2/PKG-INFO` & `tox-4.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tox
-Version: 4.5.2
+Version: 4.6.0
 Summary: tox is a generic virtualenv management and test command line tool
 Project-URL: Documentation, https://tox.wiki
 Project-URL: Homepage, http://tox.readthedocs.org
 Project-URL: Release Notes, https://tox.wiki/en/latest/changelog.html
 Project-URL: Source, https://github.com/tox-dev/tox
 Project-URL: Tracker, https://github.com/tox-dev/tox/issues
 Author-email: Bernát Gábor <gaborjbernat@gmail.com>
```

