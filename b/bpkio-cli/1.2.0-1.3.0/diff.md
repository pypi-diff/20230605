# Comparing `tmp/bpkio_cli-1.2.0.tar.gz` & `tmp/bpkio_cli-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpkio_cli-1.2.0.tar", max compression
+gzip compressed data, was "bpkio_cli-1.3.0.tar", max compression
```

## Comparing `bpkio_cli-1.2.0.tar` & `bpkio_cli-1.3.0.tar`

### file list

```diff
@@ -1,59 +1,67 @@
--rw-r--r--   0        0        0        0 2023-03-28 20:04:37.409875 bpkio_cli-1.2.0/README.md
--rw-r--r--   0        0        0       22 2023-05-17 22:57:42.076244 bpkio_cli-1.2.0/bpkio_cli/__init__.py
--rw-r--r--   0        0        0     3338 2023-04-29 21:08:44.550102 bpkio_cli-1.2.0/bpkio_cli/__main__.py
--rw-r--r--   0        0        0       91 2023-04-29 21:05:12.410693 bpkio_cli-1.2.0/bpkio_cli/click_mods/__init__.py
--rw-r--r--   0        0        0     4511 2023-05-16 18:51:59.357188 bpkio_cli-1.2.0/bpkio_cli/click_mods/group_rest_resource.py
--rw-r--r--   0        0        0     1747 2023-03-23 13:12:03.515867 bpkio_cli-1.2.0/bpkio_cli/click_mods/option_eat_all.py
--rw-r--r--   0        0        0      564 2023-04-29 21:08:44.551140 bpkio_cli-1.2.0/bpkio_cli/commands/__init__.py
--rw-r--r--   0        0        0     4669 2023-05-17 17:39:31.235348 bpkio_cli-1.2.0/bpkio_cli/commands/configure.py
--rw-r--r--   0        0        0     1758 2023-04-28 08:13:42.029805 bpkio_cli-1.2.0/bpkio_cli/commands/consumption.py
--rw-r--r--   0        0        0      762 2023-04-26 12:03:04.836639 bpkio_cli-1.2.0/bpkio_cli/commands/hello.py
--rw-r--r--   0        0        0      983 2023-04-26 12:03:04.836946 bpkio_cli-1.2.0/bpkio_cli/commands/memory.py
--rw-r--r--   0        0        0     3134 2023-04-26 12:03:04.837256 bpkio_cli-1.2.0/bpkio_cli/commands/package.py
--rw-r--r--   0        0        0     8349 2023-05-17 22:14:59.854931 bpkio_cli-1.2.0/bpkio_cli/commands/profiles.py
--rw-r--r--   0        0        0     3329 2023-05-16 18:56:25.674679 bpkio_cli-1.2.0/bpkio_cli/commands/services.py
--rw-r--r--   0        0        0     3714 2023-05-12 22:00:13.183439 bpkio_cli-1.2.0/bpkio_cli/commands/services_create.py
--rw-r--r--   0        0        0     5411 2023-05-16 18:54:19.088895 bpkio_cli-1.2.0/bpkio_cli/commands/sources.py
--rw-r--r--   0        0        0    17617 2023-05-17 17:37:14.203105 bpkio_cli-1.2.0/bpkio_cli/commands/template_crud.py
--rw-r--r--   0        0        0     7223 2023-05-12 07:39:22.268209 bpkio_cli-1.2.0/bpkio_cli/commands/template_crud_slots.py
--rw-r--r--   0        0        0      332 2023-04-28 08:33:05.100937 bpkio_cli-1.2.0/bpkio_cli/commands/tenants.py
--rw-r--r--   0        0        0     5348 2023-05-12 07:40:30.476002 bpkio_cli-1.2.0/bpkio_cli/commands/url.py
--rw-r--r--   0        0        0      359 2023-04-28 08:33:22.939414 bpkio_cli-1.2.0/bpkio_cli/commands/users.py
--rw-r--r--   0        0        0     1043 2023-04-30 21:10:36.024729 bpkio_cli-1.2.0/bpkio_cli/core/app_settings.py
--rw-r--r--   0        0        0      135 2023-04-20 16:43:38.934392 bpkio_cli-1.2.0/bpkio_cli/core/exceptions.py
--rw-r--r--   0        0        0     2128 2023-04-30 21:09:27.517510 bpkio_cli-1.2.0/bpkio_cli/core/initialize.py
--rw-r--r--   0        0        0     1718 2023-04-07 16:07:08.180945 bpkio_cli-1.2.0/bpkio_cli/core/logger.py
--rw-r--r--   0        0        0     8594 2023-05-17 14:18:10.837863 bpkio_cli-1.2.0/bpkio_cli/core/packager.py
--rw-r--r--   0        0        0     5767 2023-05-16 18:56:45.783044 bpkio_cli-1.2.0/bpkio_cli/core/resource_recorder.py
--rw-r--r--   0        0        0     2207 2023-04-26 12:03:04.840592 bpkio_cli-1.2.0/bpkio_cli/core/resources_context.py
--rw-r--r--   0        0        0     5128 2023-05-16 19:08:30.137349 bpkio_cli-1.2.0/bpkio_cli/core/response_handler.py
--rw-r--r--   0        0        0      545 2023-05-12 07:26:04.407684 bpkio_cli-1.2.0/bpkio_cli/options/__init__.py
--rw-r--r--   0        0        0      848 2023-05-17 22:07:10.594805 bpkio_cli-1.2.0/bpkio_cli/options/admin.py
--rw-r--r--   0        0        0      355 2023-05-12 19:07:07.722647 bpkio_cli-1.2.0/bpkio_cli/options/json.py
--rw-r--r--   0        0        0      958 2023-05-12 07:26:58.744571 bpkio_cli-1.2.0/bpkio_cli/options/list.py
--rw-r--r--   0        0        0      933 2023-04-27 14:26:01.185185 bpkio_cli-1.2.0/bpkio_cli/options/poll.py
--rw-r--r--   0        0        0      568 2023-05-02 19:55:34.650018 bpkio_cli-1.2.0/bpkio_cli/options/read.py
--rw-r--r--   0        0        0     1183 2023-04-27 14:26:01.185667 bpkio_cli-1.2.0/bpkio_cli/options/search.py
--rw-r--r--   0        0        0      445 2023-05-04 18:13:29.662132 bpkio_cli-1.2.0/bpkio_cli/options/table.py
--rw-r--r--   0        0        0      777 2023-05-04 11:31:15.973002 bpkio_cli-1.2.0/bpkio_cli/options/urls.py
--rw-r--r--   0        0        0      396 2023-05-17 16:16:32.031925 bpkio_cli-1.2.0/bpkio_cli/utils/__init__.py
--rw-r--r--   0        0        0     2288 2023-05-12 07:34:26.643986 bpkio_cli-1.2.0/bpkio_cli/utils/arrays.py
--rw-r--r--   0        0        0     3398 2023-05-12 19:50:24.682253 bpkio_cli-1.2.0/bpkio_cli/utils/config_provider.py
--rw-r--r--   0        0        0     1202 2023-04-28 08:03:11.236380 bpkio_cli-1.2.0/bpkio_cli/utils/datetimes.py
--rw-r--r--   0        0        0     1829 2023-05-17 22:20:51.013190 bpkio_cli-1.2.0/bpkio_cli/utils/editor.py
--rw-r--r--   0        0        0      136 2023-04-14 20:15:18.159888 bpkio_cli-1.2.0/bpkio_cli/utils/json.py
--rw-r--r--   0        0        0      567 2023-04-29 21:58:38.435162 bpkio_cli-1.2.0/bpkio_cli/utils/profile_maker.py
--rw-r--r--   0        0        0     4658 2023-05-12 19:12:42.208834 bpkio_cli-1.2.0/bpkio_cli/utils/url_builders.py
--rw-r--r--   0        0        0      583 2023-04-09 19:02:06.960542 bpkio_cli-1.2.0/bpkio_cli/utils/urls.py
--rw-r--r--   0        0        0      611 2023-04-21 22:26:37.261644 bpkio_cli-1.2.0/bpkio_cli/writers/breadcrumbs.py
--rw-r--r--   0        0        0     1404 2023-05-02 20:19:18.033992 bpkio_cli-1.2.0/bpkio_cli/writers/colorizer.py
--rw-r--r--   0        0        0     4128 2023-05-02 20:54:33.828754 bpkio_cli-1.2.0/bpkio_cli/writers/content_display.py
--rw-r--r--   0        0        0      840 2023-04-26 12:03:04.848088 bpkio_cli-1.2.0/bpkio_cli/writers/diff.py
--rw-r--r--   0        0        0      152 2023-04-26 12:03:04.848777 bpkio_cli-1.2.0/bpkio_cli/writers/formatter.py
--rw-r--r--   0        0        0     4533 2023-05-09 10:21:54.315733 bpkio_cli-1.2.0/bpkio_cli/writers/hls_formatter.py
--rw-r--r--   0        0        0      715 2023-05-12 19:01:29.004428 bpkio_cli-1.2.0/bpkio_cli/writers/json_formatter.py
--rw-r--r--   0        0        0     1583 2023-04-29 21:08:44.553756 bpkio_cli-1.2.0/bpkio_cli/writers/players.py
--rw-r--r--   0        0        0     1865 2023-05-12 07:26:12.170387 bpkio_cli-1.2.0/bpkio_cli/writers/tables.py
--rw-r--r--   0        0        0     5205 2023-04-26 12:03:04.849885 bpkio_cli-1.2.0/bpkio_cli/writers/xml_formatter.py
--rw-r--r--   0        0        0     1207 2023-05-17 22:57:42.075576 bpkio_cli-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      885 1970-01-01 00:00:00.000000 bpkio_cli-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-03-28 20:04:37.409875 bpkio_cli-1.3.0/README.md
+-rw-r--r--   0        0        0       22 2023-06-05 14:47:30.710905 bpkio_cli-1.3.0/bpkio_cli/__init__.py
+-rw-r--r--   0        0        0     3812 2023-05-24 04:05:57.379943 bpkio_cli-1.3.0/bpkio_cli/app.py
+-rw-r--r--   0        0        0       91 2023-04-29 21:05:12.410693 bpkio_cli-1.3.0/bpkio_cli/click_mods/__init__.py
+-rw-r--r--   0        0        0      771 2023-05-24 04:19:18.738931 bpkio_cli-1.3.0/bpkio_cli/click_mods/default_last_command.py
+-rw-r--r--   0        0        0     5145 2023-06-01 09:13:30.452845 bpkio_cli-1.3.0/bpkio_cli/click_mods/group_rest_resource.py
+-rw-r--r--   0        0        0     1747 2023-03-23 13:12:03.515867 bpkio_cli-1.3.0/bpkio_cli/click_mods/option_eat_all.py
+-rw-r--r--   0        0        0      599 2023-05-21 21:17:36.965795 bpkio_cli-1.3.0/bpkio_cli/click_options/__init__.py
+-rw-r--r--   0        0        0      848 2023-05-17 22:07:10.594805 bpkio_cli-1.3.0/bpkio_cli/click_options/admin.py
+-rw-r--r--   0        0        0      355 2023-05-12 19:07:07.722647 bpkio_cli-1.3.0/bpkio_cli/click_options/json.py
+-rw-r--r--   0        0        0      958 2023-05-12 07:26:58.744571 bpkio_cli-1.3.0/bpkio_cli/click_options/list.py
+-rw-r--r--   0        0        0      933 2023-04-27 14:26:01.185185 bpkio_cli-1.3.0/bpkio_cli/click_options/poll.py
+-rw-r--r--   0        0        0      851 2023-05-23 10:02:17.547439 bpkio_cli-1.3.0/bpkio_cli/click_options/read.py
+-rw-r--r--   0        0        0     1183 2023-04-27 14:26:01.185667 bpkio_cli-1.3.0/bpkio_cli/click_options/search.py
+-rw-r--r--   0        0        0      445 2023-05-04 18:13:29.662132 bpkio_cli-1.3.0/bpkio_cli/click_options/table.py
+-rw-r--r--   0        0        0     1161 2023-05-22 16:50:12.003620 bpkio_cli-1.3.0/bpkio_cli/click_options/urls.py
+-rw-r--r--   0        0        0      656 2023-05-21 21:48:40.162730 bpkio_cli-1.3.0/bpkio_cli/commands/__init__.py
+-rw-r--r--   0        0        0      751 2023-05-21 21:49:06.651917 bpkio_cli-1.3.0/bpkio_cli/commands/addons.py
+-rw-r--r--   0        0        0     4878 2023-06-01 13:43:54.231560 bpkio_cli-1.3.0/bpkio_cli/commands/configure.py
+-rw-r--r--   0        0        0     1758 2023-04-28 08:13:42.029805 bpkio_cli-1.3.0/bpkio_cli/commands/consumption.py
+-rw-r--r--   0        0        0     4388 2023-05-23 21:27:26.436574 bpkio_cli-1.3.0/bpkio_cli/commands/creators/ad_insertion.py
+-rw-r--r--   0        0        0     7930 2023-05-23 21:19:19.179090 bpkio_cli-1.3.0/bpkio_cli/commands/creators/sources.py
+-rw-r--r--   0        0        0     4064 2023-05-22 08:49:01.223413 bpkio_cli-1.3.0/bpkio_cli/commands/creators/virtual_channel.py
+-rw-r--r--   0        0        0     8808 2023-05-21 21:14:37.474798 bpkio_cli-1.3.0/bpkio_cli/commands/creators/virtual_channel_populate.py
+-rw-r--r--   0        0        0      761 2023-05-21 21:14:37.453890 bpkio_cli-1.3.0/bpkio_cli/commands/hello.py
+-rw-r--r--   0        0        0     1251 2023-05-21 21:14:37.453903 bpkio_cli-1.3.0/bpkio_cli/commands/memory.py
+-rw-r--r--   0        0        0     3118 2023-05-21 21:14:37.453880 bpkio_cli-1.3.0/bpkio_cli/commands/package.py
+-rw-r--r--   0        0        0     9969 2023-05-23 22:13:49.593225 bpkio_cli-1.3.0/bpkio_cli/commands/profiles.py
+-rw-r--r--   0        0        0     2700 2023-05-21 20:35:26.716484 bpkio_cli-1.3.0/bpkio_cli/commands/recorder.py
+-rw-r--r--   0        0        0     3669 2023-06-01 13:42:32.164671 bpkio_cli-1.3.0/bpkio_cli/commands/services.py
+-rw-r--r--   0        0        0     7952 2023-06-01 13:44:49.316974 bpkio_cli-1.3.0/bpkio_cli/commands/sources.py
+-rw-r--r--   0        0        0    18465 2023-06-02 14:22:43.378526 bpkio_cli-1.3.0/bpkio_cli/commands/template_crud.py
+-rw-r--r--   0        0        0     7306 2023-05-21 21:17:10.206971 bpkio_cli-1.3.0/bpkio_cli/commands/template_crud_slots.py
+-rw-r--r--   0        0        0      332 2023-04-28 08:33:05.100937 bpkio_cli-1.3.0/bpkio_cli/commands/tenants.py
+-rw-r--r--   0        0        0     5477 2023-05-22 16:05:47.390346 bpkio_cli-1.3.0/bpkio_cli/commands/url.py
+-rw-r--r--   0        0        0      359 2023-04-28 08:33:22.939414 bpkio_cli-1.3.0/bpkio_cli/commands/users.py
+-rw-r--r--   0        0        0     1036 2023-05-22 17:10:47.554934 bpkio_cli-1.3.0/bpkio_cli/core/app_context.py
+-rw-r--r--   0        0        0     3753 2023-05-24 04:10:19.009730 bpkio_cli-1.3.0/bpkio_cli/core/config_provider.py
+-rw-r--r--   0        0        0      135 2023-04-20 16:43:38.934392 bpkio_cli-1.3.0/bpkio_cli/core/exceptions.py
+-rw-r--r--   0        0        0     2565 2023-05-24 04:11:25.852254 bpkio_cli-1.3.0/bpkio_cli/core/initialize.py
+-rw-r--r--   0        0        0     1718 2023-04-07 16:07:08.180945 bpkio_cli-1.3.0/bpkio_cli/core/logger.py
+-rw-r--r--   0        0        0     8783 2023-05-19 21:18:11.983457 bpkio_cli-1.3.0/bpkio_cli/core/packager.py
+-rw-r--r--   0        0        0     8775 2023-05-22 09:50:46.909212 bpkio_cli-1.3.0/bpkio_cli/core/resource_recorder.py
+-rw-r--r--   0        0        0     2204 2023-05-21 21:15:26.397241 bpkio_cli-1.3.0/bpkio_cli/core/resource_trail.py
+-rw-r--r--   0        0        0     5128 2023-05-16 19:08:30.137349 bpkio_cli-1.3.0/bpkio_cli/core/response_handler.py
+-rw-r--r--   0        0        0     1234 2023-05-21 20:37:15.106665 bpkio_cli-1.3.0/bpkio_cli/core/session_recorder.py
+-rw-r--r--   0        0        0      395 2023-05-21 21:21:56.973900 bpkio_cli-1.3.0/bpkio_cli/utils/__init__.py
+-rw-r--r--   0        0        0     2288 2023-05-12 07:34:26.643986 bpkio_cli-1.3.0/bpkio_cli/utils/arrays.py
+-rw-r--r--   0        0        0     1358 2023-05-19 19:23:50.776214 bpkio_cli-1.3.0/bpkio_cli/utils/datetimes.py
+-rw-r--r--   0        0        0     1828 2023-05-21 21:21:56.974288 bpkio_cli-1.3.0/bpkio_cli/utils/editor.py
+-rw-r--r--   0        0        0      476 2023-05-19 16:10:53.950053 bpkio_cli-1.3.0/bpkio_cli/utils/inquirer_defaults.py
+-rw-r--r--   0        0        0      136 2023-04-14 20:15:18.159888 bpkio_cli-1.3.0/bpkio_cli/utils/json.py
+-rw-r--r--   0        0        0      567 2023-04-29 21:58:38.435162 bpkio_cli-1.3.0/bpkio_cli/utils/profile_maker.py
+-rw-r--r--   0        0        0     8758 2023-06-02 14:32:29.030983 bpkio_cli-1.3.0/bpkio_cli/utils/url_builders.py
+-rw-r--r--   0        0        0      861 2023-05-22 14:30:20.340741 bpkio_cli-1.3.0/bpkio_cli/utils/urls.py
+-rw-r--r--   0        0        0     1034 2023-05-24 04:10:59.495781 bpkio_cli-1.3.0/bpkio_cli/writers/breadcrumbs.py
+-rw-r--r--   0        0        0     1404 2023-05-02 20:19:18.033992 bpkio_cli-1.3.0/bpkio_cli/writers/colorizer.py
+-rw-r--r--   0        0        0     4503 2023-05-23 20:32:04.036975 bpkio_cli-1.3.0/bpkio_cli/writers/content_display.py
+-rw-r--r--   0        0        0      840 2023-04-26 12:03:04.848088 bpkio_cli-1.3.0/bpkio_cli/writers/diff.py
+-rw-r--r--   0        0        0      152 2023-04-26 12:03:04.848777 bpkio_cli-1.3.0/bpkio_cli/writers/formatter.py
+-rw-r--r--   0        0        0     4533 2023-05-09 10:21:54.315733 bpkio_cli-1.3.0/bpkio_cli/writers/hls_formatter.py
+-rw-r--r--   0        0        0      714 2023-05-21 21:21:56.975414 bpkio_cli-1.3.0/bpkio_cli/writers/json_formatter.py
+-rw-r--r--   0        0        0     1674 2023-05-22 15:17:28.335555 bpkio_cli-1.3.0/bpkio_cli/writers/players.py
+-rw-r--r--   0        0        0     1865 2023-05-12 07:26:12.170387 bpkio_cli-1.3.0/bpkio_cli/writers/tables.py
+-rw-r--r--   0        0        0     5205 2023-04-26 12:03:04.849885 bpkio_cli-1.3.0/bpkio_cli/writers/xml_formatter.py
+-rw-r--r--   0        0        0     1220 2023-06-05 14:47:30.709930 bpkio_cli-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      929 1970-01-01 00:00:00.000000 bpkio_cli-1.3.0/PKG-INFO
```

### Comparing `bpkio_cli-1.2.0/bpkio_cli/__main__.py` & `bpkio_cli-1.3.0/bpkio_cli/app.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 
 import logging
 
 import click
 import cloup
 
 import bpkio_cli.commands as commands
+from bpkio_cli.click_mods.default_last_command import DefaultLastCommandGroup
 from bpkio_cli.commands.configure import init
+from bpkio_cli.core.config_provider import ConfigProvider
 from bpkio_cli.core.initialize import initialize
 from bpkio_cli.core.logger import (
     get_child_logger,
     get_level_names,
     set_console_logging_level,
 )
 from bpkio_cli.writers.breadcrumbs import display_tenant_info
@@ -22,104 +24,127 @@
 
 
 SETTINGS = cloup.Context.settings(
     formatter_settings=cloup.HelpFormatter.settings(theme=cloup.HelpTheme.dark())
 )
 
 
-@cloup.group(show_subcommand_aliases=True, context_settings=SETTINGS)
+@cloup.group(
+    show_subcommand_aliases=True, context_settings=SETTINGS, cls=DefaultLastCommandGroup
+)
 @click.version_option(
     package_name="bpkio_cli", prog_name="Command Line helpers for broadpeak.io"
 )
 @click.option("-t", "--tenant", help="Identifier of the tenant profile to impersonate")
 @click.option(
     "--log-level",
     type=click.Choice(get_level_names()),
     required=False,
+    show_default=True,
     help="Set the log level",
 )
 @click.option(
     "--log-sdk",
     type=bool,
     is_flag=True,
     required=False,
     default=False,
+    show_default=True,
     help="Log messages from the underlying API client",
 )
 @click.option(
     "-cc / -nc",
     "--cache / --no-cache",
     "use_cache",
     is_flag=True,
     default=True,
-    help="Enable or disable resource caches (enabled by default)",
+    show_default=True,
+    help="Enable or disable resource caches",
 )
 @click.option(
-    "--breadcrumbs / --no-breadcrumbs",
-    "display_breadcrumbs",
+    "-pp / -np",
+    "--prompts / --no-prompts",
+    "use_prompts",
     is_flag=True,
     default=True,
-    help="Display or hide information about the resources accessed (enabled by default)",
+    show_default=True,
+    help="Enable or disable the use of prompts to ask for some information (where supported)",
 )
 @click.pass_context
-def cli(ctx, tenant, log_level, log_sdk, use_cache, display_breadcrumbs):
+def bic(ctx, tenant, log_level, log_sdk, use_cache, use_prompts):
     if log_level or LOG_LEVEL:
         set_console_logging_level(
             log_level or LOG_LEVEL, include_sdk=log_sdk or LOG_SDK
         )
 
-    # Bypass initialisation if there is an explicit call to initialise the configuration
-    if ctx.invoked_subcommand not in ["init", "config"]:
-        app_context = initialize(tenant, use_cache, get_tenant_info=display_breadcrumbs)
+    requires_api = True
+    if ctx.invoked_subcommand in ["init", "config", "record"]:
+        requires_api = False
+
+    app_context = initialize(
+        tenant=tenant,
+        use_cache=use_cache,
+        use_prompts=use_prompts,
+        requires_api=requires_api,
+    )
 
-        if display_breadcrumbs:
-            display_tenant_info(app_context.tenant)
+    if app_context:
+        display_tenant_info(app_context.tenant)
 
-        # TODO - validate the token in the initialisation of BroadpeakApi
-        ctx.obj = app_context
+    # TODO - validate the token in the initialisation of BroadpeakApi
+    ctx.obj = app_context
 
     @ctx.call_on_close
     def close_cleanly():
         try:
+            # Save the cache to disk
             app_context.cache.save()
+
+            # Save the current command
+            with open(".last_command", "w") as f:
+                f.write(ctx.invoked_subcommand)
+
         except Exception as e:
             pass
 
 
-cli.section("Configuration", commands.hello, init, commands.configure)
+bic.section("Configuration", commands.hello, init, commands.configure)
 
-commands.add_sources_section(cli)
-commands.add_services_section(cli)
+commands.add_sources_section(bic)
+commands.add_services_section(bic)
+
+bic.section(
+    "Other resources",
+    commands.profile,
+    commands.url,
+)
 
-cli.section(
+bic.section(
     "Account resources",
     commands.add_tenants_commands(),
     commands.add_users_commands(),
     commands.consumption,
 )
 
-cli.section(
-    "Other resources",
-    commands.profile,
+bic.section(
+    "Advanced", commands.package, commands.record, commands.memory, commands.addons
 )
 
-cli.section("Advanced", commands.url, commands.memory, commands.package)
-
 
 def debug_entry_point():
     global LOG_LEVEL
     LOG_LEVEL = logging.DEBUG
     global LOG_SDK
     LOG_SDK = True
-    cli(obj={})
+    bic(obj={})
 
 
 def safe_entry_point():
     try:
-        cli()
+        bic()
     except Exception as e:
         if hasattr(e, "status_code"):
             st = " [{}] ".format(e.status_code)
         else:
             st = ""
         msg = "{}:{}{}".format(e.__class__.__name__, st, e)
         click.secho(msg, fg="red")
```

### Comparing `bpkio_cli-1.2.0/bpkio_cli/click_mods/group_rest_resource.py` & `bpkio_cli-1.3.0/bpkio_cli/click_mods/group_rest_resource.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import re
 from typing import Any
 
 import bpkio_api.models as models
 import click
 import cloup
 
-from bpkio_cli.core.resources_context import ResourcesContext
+from bpkio_cli.core.resource_trail import ResourceTrail
+from bpkio_cli.writers.breadcrumbs import display_context
 
 
 class ApiResourceGroup(cloup.Group):
     """A click.Group sub-class that enables the use of command lines that
     1.  mirror REST endpoint structure that use resource identifiers
         (eg. `mycli sources 123 slots 456`
         -> http://myapi/sources/:source_id/slots/:slot_id)
@@ -22,20 +23,23 @@
     Inspired by https://stackoverflow.com/a/44056564/2215413"""
 
     def __init__(self, *args: Any, resource_class: type | None = None, **kwargs: Any):
         super().__init__(*args, **kwargs)
         self.resource_class = resource_class
 
     def parse_args(self, ctx, args):
-        commands_without_resource_id = ["list", "search", "create", "json", "clear"]
+        commands_without_resource_id = ["list", "search", "create", "clear"]
 
         # No sub-command?  Then it's an implicit `list`
         #  eg. "bic sources" -> "bic sources list"
         if len(args) == 0 and "list" in self.commands:
             args.append("list")
+            display_context(
+                "No sub-command provided, assuming 'list'.",
+            )
 
         # Some commands do not take an ID argument,
         # so inject an empty one to prevent parse failure
         #  eg. "bic sources list" -> "bic sources '' list"
         if args[0] in commands_without_resource_id:
             args.insert(0, "")
 
@@ -45,26 +49,33 @@
         if args[0] in self.commands and any(a in args for a in ["--help"]):
             args.insert(0, "")
 
         # Single argument, which is not a command?
         # It must be an ID, and we treat it as an implicit `get`
         #  eg. "bic sources 123" -> "bic sources 123 get"
         #  eg. "bic sources 123 --help" -> "bic sources 123 get --help"
-        if args[0] not in self.commands:
+        if args[0] not in self.commands and args[0] not in self.alias2name:
             if (len(args) == 1) or (len(args) == 2 and args[1] in ["--help"]):
                 args.insert(1, "get")
+                display_context(
+                    "No sub-command provided, assuming 'get'.",
+                )
 
         # If the command is one that require an ID, but there isn't one, it's an error
         #  eg. "bic sources get" -> BadArgumentUsage
         if (args[0] in self.commands or args[0] in self.alias2name) and (
             args[0] not in commands_without_resource_id
         ):
-            raise click.BadArgumentUsage(
-                f"The `{args[0]}` command must be preceded by a {self.name} ID"
+            display_context(
+                "No ID provided, using '$' to reuse the previous resource.",
             )
+            args.insert(0, "$")
+            # raise click.BadArgumentUsage(
+            #     f"The `{args[0]}` command must be preceded by a {self.name} ID"
+            # )
 
         # If there is a resource-based command preceded by a non-empty string,
         # that's an error
         #  eg. "bic sources 123 list" -> BadArgumentUsage
         if args[0] != "" and args[1] in [
             c for c in commands_without_resource_id if c != "json"
         ]:
@@ -80,28 +91,32 @@
             and args[0] not in self.commands
             and (args[1] in self.commands or args[1] in self.alias2name)
         ):
             target_type = self._get_resource_class_for_command()
 
             # Lookup in the cache if the ID is not a recognised value
             if not args[0].isdigit() and not args[0].startswith("-"):
-                args[0] = ctx.obj.cache.resolve(args[0], target_type)
+                placeholder = args[0]
+                args[0] = ctx.obj.cache.resolve(placeholder, target_type)
+                display_context(
+                    f"Resolved '{placeholder}' to {target_type.__name__} id {args[0]}",
+                )
 
-            resources: ResourcesContext = ctx.obj.resources
+            resources: ResourceTrail = ctx.obj.resources
             resources.record_resource_id(self.name, args[0])
 
         super(ApiResourceGroup, self).parse_args(ctx, args)
 
     def full_command_name(self, ctx):
         """Generate an optionally composite command name
         by traversing the chain of commands to the current one
         """
         cmd = ctx.command.name
         if hasattr(ctx, "parent"):
-            if ctx.parent.command.name != "cli":
+            if ctx.parent.command.name != "bic":
                 cmd = self.full_command_name(ctx.parent) + ":" + cmd
         return cmd
 
     def _get_resource_class_for_command(self):
         if self.resource_class:
             return self.resource_class
         else:
```

### Comparing `bpkio_cli-1.2.0/bpkio_cli/click_mods/option_eat_all.py` & `bpkio_cli-1.3.0/bpkio_cli/click_mods/option_eat_all.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.2.0/bpkio_cli/commands/__init__.py` & `bpkio_cli-1.3.0/bpkio_cli/commands/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+from bpkio_cli.commands.addons import addons
 from bpkio_cli.commands.configure import configure
 from bpkio_cli.commands.consumption import consumption
 from bpkio_cli.commands.hello import hello
 from bpkio_cli.commands.memory import memory
 from bpkio_cli.commands.package import package
 from bpkio_cli.commands.profiles import profile
+from bpkio_cli.commands.recorder import record
 from bpkio_cli.commands.services import add_services_section
 from bpkio_cli.commands.sources import add_sources_section
 from bpkio_cli.commands.tenants import add_tenants_commands
-from bpkio_cli.commands.users import add_users_commands
 from bpkio_cli.commands.url import url
+from bpkio_cli.commands.users import add_users_commands
```

### Comparing `bpkio_cli-1.2.0/bpkio_cli/commands/configure.py` & `bpkio_cli-1.3.0/bpkio_cli/commands/configure.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import click
 import cloup
 from bpkio_api.api import DEFAULT_FQDN, BroadpeakIoApi
 from bpkio_api.credential_provider import TenantProfileProvider
 from InquirerPy import inquirer
 
 from bpkio_cli.commands.hello import hello
+from bpkio_cli.core.config_provider import ConfigProvider
 from bpkio_cli.core.initialize import initialize
 from bpkio_cli.core.response_handler import ResponseHandler
-from bpkio_cli.utils.config_provider import ConfigProvider
 
 
 # Command: INIT
 # To be attached to the root group
 @cloup.command(help="Initialize the tool, and create a first tenant profile")
 @click.pass_context
 def init(ctx):
@@ -41,15 +41,22 @@
 @click.argument("key", required=True)
 @click.argument("value", required=True)
 def set(key, value):
     cp = ConfigProvider()
     cp.set_config(key, value)
 
 
-# Group: TENANTS
+# Command: EDIT
+@configure.command(help="Edit the config file")
+def edit():
+    config_file = ConfigProvider().config_path
+    click.edit(filename=str(config_file), editor=ConfigProvider().get("editor"))
+
+
+# Sub-Group: TENANTS
 @configure.group(
     aliases=["tenant", "tnt"],
     help="Define CLI credential profiles to be able to easily switch tenant",
 )
 @click.pass_obj
 def tenants(obj):
     pass
```

### Comparing `bpkio_cli-1.2.0/bpkio_cli/commands/consumption.py` & `bpkio_cli-1.3.0/bpkio_cli/commands/consumption.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.2.0/bpkio_cli/commands/hello.py` & `bpkio_cli-1.3.0/bpkio_cli/commands/hello.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import click
 
-from bpkio_cli.core.app_settings import AppContext
+from bpkio_cli.core.app_context import AppContext
 
 
 # Command: HELLO
 @click.command()
 @click.pass_obj
 def hello(obj: AppContext):
     """Validate access to the API and display tenant information"""
```

### Comparing `bpkio_cli-1.2.0/bpkio_cli/commands/memory.py` & `bpkio_cli-1.3.0/bpkio_cli/commands/memory.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import click
 import cloup
 
-from bpkio_cli.core.app_settings import AppContext
+from bpkio_cli.core.app_context import AppContext
 
 
 @cloup.group(aliases=["mem"], help="App resource registry comands")
 @click.pass_obj
 def memory(obj: AppContext):
     pass
 
@@ -26,9 +26,17 @@
 
     click.secho("Last lists retrieved", fg="yellow")
     for k, lst in obj.cache.list_lists().items():
         try:
             list_ids = [item.id for item in lst]
             click.secho(" · " + k + " ", fg="green", nl=False)
             click.secho(list_ids)
-        except:
+        except Exception:
+            pass
+
+    click.secho("Last Metadata", fg="yellow")
+    for k, metadata in obj.cache.list_metadata().items():
+        try:
+            click.secho(" · " + k + " ", fg="green", nl=False)
+            click.secho(metadata)
+        except Exception:
             pass
```

### Comparing `bpkio_cli-1.2.0/bpkio_cli/commands/package.py` & `bpkio_cli-1.3.0/bpkio_cli/commands/package.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import click
 import cloup
 from bpkio_api.models.common import summary
 from InquirerPy import inquirer
 from InquirerPy.base.control import Choice
 
-from bpkio_cli.core.app_settings import AppContext
+from bpkio_cli.core.app_context import AppContext
 from bpkio_cli.core.packager import PackageInstaller, ResourcePackager
 
 logger = logging.getLogger(__name__)
 
 
 @cloup.group(aliases=["pkg"], help="Work with reusable packages of resources")
 def package():
@@ -96,15 +96,15 @@
 
     package = json.load(file)
 
     output = installer.deploy(package)
 
     table = [
         dict(
-            status=installer.statuses[st],
+            status=st.name,
             resource=summary(res, with_class=True),
             message=msg,
         )
         for (res, st, msg) in output.values()
     ]
 
     obj.response_handler.treat_simple_list(table)
```

### Comparing `bpkio_cli-1.2.0/bpkio_cli/commands/profiles.py` & `bpkio_cli-1.3.0/bpkio_cli/commands/profiles.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import json as j
 
+import bpkio_api.models as models
 import click
 import cloup
 from bpkio_api.api import BroadpeakIoApi
+from bpkio_api.helpers.recorder import SessionRecorder, SessionSection
 from bpkio_api.models import TranscodingProfile, TranscodingProfileIn
 from InquirerPy import inquirer
 
-import bpkio_cli.options as bic_options
+import bpkio_cli.click_options as bic_options
 from bpkio_cli.click_mods import ApiResourceGroup
-from bpkio_cli.core.app_settings import AppContext
+from bpkio_cli.core.app_context import AppContext
 from bpkio_cli.core.exceptions import BroadpeakIoCliError
 from bpkio_cli.utils.arrays import order_by_dict_keys
 from bpkio_cli.utils.editor import edit_payload
 from bpkio_cli.utils.json import is_json
 from bpkio_cli.writers.breadcrumbs import display_resource_info
 from bpkio_cli.writers.tables import display_table
 
@@ -64,27 +66,39 @@
         "Leave empty for commands operating on a list of profiles."
     ),
 )
 @click.pass_obj
 def profile(obj, profile_id: str):
     """Manage Transcoding Profiles"""
 
-    if profile_id:
-        # TODO - find a way of passing the target tenant (admin mode)
-        profile = obj.api.transcoding_profiles.retrieve(profile_id)
-        display_resource_info(profile)
+    @SessionRecorder.do_not_record
+    def show_breadcrumb():
+        if profile_id:
+            # TODO - find a way of passing the target tenant (admin mode)
+            profile = obj.api.transcoding_profiles.retrieve(profile_id)
+            display_resource_info(profile)
+
+    show_breadcrumb()
 
 
 # --- LIST Command
-@cloup.command(help="Retrieve a list of all Transcoding Profiles", aliases=["ls"])
+@cloup.command(
+    help="Retrieve a list of all Transcoding Profiles", aliases=["ls"], name="list"
+)
 @bic_options.json
 @bic_options.list(default_fields=default_fields)
 @bic_options.tenant(required=False)
 @click.pass_obj
-def list(obj, json, select_fields, sort_fields, tenant):
+def lst(obj, json, select_fields, sort_fields, tenant):
+    SessionRecorder.record(
+        SessionSection(
+            title="List of Transcoding Profiles", description="This is for a test"
+        )
+    )
+
     profiles = obj.api.transcoding_profiles.list(tenantId=tenant)
 
     obj.response_handler.treat_list_resources(
         profiles,
         select_fields=select_fields,
         sort_fields=sort_fields,
         json=json,
@@ -271,19 +285,62 @@
 
 
 # --- DELETE Command
 @cloup.command(help="[ADMIN] Delete a Transcoding Profile, by its ID")
 @click.confirmation_option(
     prompt="Are you sure you want to delete this transcoding profile?"
 )
-def delete():
+@click.pass_obj
+def delete(obj: AppContext):
     profile = get_profile_resource()
     endpoint = get_admin_endpoint()
 
     endpoint.delete(profile.id)
 
+    # remove from cache
+    obj.cache.remove(profile)
+
+    click.secho(f"Resource {profile.id} deleted", fg="green")
+
+
+# --- USAGE Command
+@cloup.command(help="Find all Services that use the profile")
+@bic_options.json
+@bic_options.list(default_fields=["id", "name", "type"])
+@click.pass_obj
+def usage(obj: AppContext, json, select_fields, sort_fields, **kwargs):
+    select_fields = list(select_fields)
+
+    profile = get_profile_resource()
+    id = profile.id
+
+    services = obj.api.services.list()
+
+    selected_services = []
+    for service in services:
+        svc = obj.api.services.retrieve(service.id)
+
+        if isinstance(svc, models.VirtualChannelService):
+            if svc.transcodingProfile and svc.transcodingProfile.id == id:
+                selected_services.append(svc)
+
+        if isinstance(svc, models.AdInsertionService):
+            if svc.transcodingProfile and svc.transcodingProfile.id == id:
+                selected_services.append(svc)
+
+    obj.response_handler.treat_list_resources(
+        selected_services,
+        select_fields=select_fields,
+        sort_fields=sort_fields,
+        json=json,
+    )
+
+
+# ===
 
 profile.add_section(
     cloup.Section(
-        "CRUD commands", [list, get, table, json, search, create, update, delete]
+        "CRUD commands", [lst, get, table, json, search, create, update, delete]
     )
 )
+
+profile.add_section(cloup.Section("Other commands", [usage]))
```

### Comparing `bpkio_cli-1.2.0/bpkio_cli/commands/services.py` & `bpkio_cli-1.3.0/bpkio_cli/commands/services.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,21 @@
     ContentReplacementService,
     ContentReplacementSlot,
     ServiceIn,
     VirtualChannelService,
     VirtualChannelSlot,
 )
 
-from bpkio_cli.commands.services_create import create_ad_insertion_service_command
+from bpkio_cli.commands.creators.ad_insertion import create_ad_insertion_service_command
+from bpkio_cli.commands.creators.virtual_channel import (
+    create_virtual_channel_service_command,
+)
+from bpkio_cli.commands.creators.virtual_channel_populate import (
+    populate_virtual_channel_slots_command,
+)
 from bpkio_cli.commands.template_crud import create_resource_group
 from bpkio_cli.commands.template_crud_slots import create_child_resource_group
 
 default_fields = ["id", "name", "type", "serviceId", "format"]
 
 
 def add_services_section(cli):
@@ -65,28 +71,30 @@
             "virtual-channel",
             resource_class=VirtualChannelService,
             endpoint_path=[root_endpoint, "virtual_channel"],
             aliases=["vc"],
             default_fields=default_fields,
             with_content_commands=["all"],
             extra_commands=[
+                create_virtual_channel_service_command(),
+                populate_virtual_channel_slots_command(),
                 add_slots_commands(
                     resource_class=VirtualChannelSlot,
                     parent_path=[root_endpoint, "virtual_channel"],
                     default_fields=[
                         "id",
                         "name",
                         "type",
                         "relativeStartTime",
                         "relativeEndTime",
                         "duration",
                         "replacement.id",
                         "replacement.name",
                     ],
-                )
+                ),
             ],
         ),
     )
 
 
 def add_slots_commands(resource_class, parent_path, default_fields):
     return create_child_resource_group(
```

### Comparing `bpkio_cli-1.2.0/bpkio_cli/commands/services_create.py` & `bpkio_cli-1.3.0/bpkio_cli/commands/creators/ad_insertion.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-import json
-
 import click
 import cloup
 import InquirerPy.inquirer as inquirer
 from bpkio_api.models import AdInsertionServiceIn, SourceType
 
-from bpkio_cli.core.app_settings import AppContext
+import bpkio_cli.utils.inquirer_defaults as inqdef
+from bpkio_cli.core.app_context import AppContext
 
 
 def create_ad_insertion_service_command():
     # COMMAND: CREATE
     @cloup.command(help="Create a (simple) Ad Insertion service")
     @click.pass_obj
     def create(obj: AppContext):
@@ -18,64 +17,75 @@
         # Ask for the source
         sources = [
             s
             for s in all_sources
             if s.type in (SourceType.LIVE, SourceType.ASSET_CATALOG)
         ]
         sources = sorted(sources, key=lambda s: s.id, reverse=True)
+        sources = obj.cache.sort_resources_by_most_recently_accessed(sources)
         choices = [
             dict(value=s.id, name=f"({s.id})  {s.name}  [{s.type.value}]")
             for s in sources
         ]
-        source_id = inquirer.fuzzy(message="Source", choices=choices).execute()
+        source_id = inquirer.fuzzy(
+            message="Source", choices=choices, **inqdef.select_markers()
+        ).execute()
         source_type = next(s for s in sources if s.id == source_id).type
 
         # Then ask for the ad server
         ad_sources = [s for s in all_sources if s.type == SourceType.AD_SERVER]
         ad_sources = sorted(ad_sources, key=lambda s: s.id, reverse=True)
+        ad_sources = obj.cache.sort_resources_by_most_recently_accessed(ad_sources)
         choices = [dict(value=s.id, name=f"({s.id})  {s.name}") for s in ad_sources]
-        ad_source_id = inquirer.fuzzy(message="Ad Server", choices=choices).execute()
+        ad_source_id = inquirer.fuzzy(
+            message="Ad Server", choices=choices, **inqdef.select_markers()
+        ).execute()
 
         # Then ask for the gap filler
         slate_sources = [s for s in all_sources if s.type == SourceType.SLATE]
         slate_sources = sorted(slate_sources, key=lambda s: s.id, reverse=True)
+        slate_sources = obj.cache.sort_resources_by_most_recently_accessed(
+            slate_sources
+        )
         choices = [dict(value=s.id, name=f"({s.id})  {s.name}") for s in slate_sources]
         choices = [dict(value=None, name="-- No gap filler --")] + choices
         slate_source_id = inquirer.fuzzy(
-            message="Gap Filler", choices=choices
+            message="Gap Filler", choices=choices, **inqdef.select_markers()
         ).execute()
 
         # Ask for the type of ad insertion (optionally)
         if source_type in (SourceType.ASSET, SourceType.ASSET_CATALOG):
             insertion_type = "vodAdInsertion"
         else:
             choices = [
                 dict(value="liveAdPreRoll", name="Live Pre-Roll"),
                 dict(value="liveAdReplacement", name="Live Ad Replacment"),
             ]
             insertion_type = inquirer.select(
-                message="Ad Insertion Type", choices=choices
+                message="Ad Insertion Type", choices=choices, **inqdef.select_markers()
             ).execute()
 
         # Ask for transcoding profile
         profiles = obj.api.transcoding_profiles.list()
+        profiles = obj.cache.sort_resources_by_most_recently_accessed(profiles)
         choices = [dict(value=s.id, name=f"{s.name} ({s.id})") for s in profiles]
         # ... add a "none" one
         choices = [dict(value=None, name="-- No transcoding --")] + choices
         transcoding_profile_id = inquirer.fuzzy(
-            message="Transcoding Profile", choices=choices
+            message="Transcoding Profile", choices=choices, **inqdef.select_markers()
         ).execute()
 
         # Ask for other options
         with_transcoding = transcoding_profile_id is not None
 
         name = inquirer.text(
-            message="Name",
+            message="Name for the service",
             validate=lambda result: len(result) > 0,
             invalid_message="The name cannot be empty.",
+            **inqdef.markers(0),
         ).execute()
 
         # Create the service object
         service = AdInsertionServiceIn(
             name=name, source=dict(id=source_id), enableAdTranscoding=with_transcoding
         )
         ad_insertion = dict(adServer=dict(id=ad_source_id))
@@ -84,16 +94,15 @@
 
         setattr(
             service,
             insertion_type,
             ad_insertion,
         )
         if with_transcoding:
+            # setattr(service, "transcodingProfile", dict(id=transcoding_profile_id))
             service.transcodingProfile = dict(id=transcoding_profile_id)
 
-        print(service.json())
-
         service_out = obj.api.services.ad_insertion.create(service)
 
         obj.response_handler.treat_single_resource(service_out)
 
     return create
```

### Comparing `bpkio_cli-1.2.0/bpkio_cli/commands/template_crud.py` & `bpkio_cli-1.3.0/bpkio_cli/commands/template_crud.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
+import json as j
 import re
 from typing import List
 from urllib.parse import quote_plus
 
 import bpkio_api.mappings as mappings
 import click
 import cloup
+from bpkio_api.helpers.recorder import SessionRecorder
 from bpkio_api.models import ServiceIn, SourceIn
 
-import bpkio_cli.options as bic_options
+import bpkio_cli.click_options as bic_options
 from bpkio_cli.click_mods.group_rest_resource import ApiResourceGroup
 from bpkio_cli.commands.package import package_resources
-from bpkio_cli.core.app_settings import AppContext
+from bpkio_cli.core.app_context import AppContext
 from bpkio_cli.core.exceptions import BroadpeakIoCliError
-from bpkio_cli.core.resources_context import ResourcesContext, UnknownResourceError
+from bpkio_cli.core.resource_trail import ResourceTrail, UnknownResourceError
 from bpkio_cli.utils.editor import edit_payload
 from bpkio_cli.utils.profile_maker import make_transcoding_profile
 from bpkio_cli.utils.url_builders import get_service_handler, get_source_handler
 from bpkio_cli.writers.breadcrumbs import display_resource_info
 from bpkio_cli.writers.content_display import display_content
 from bpkio_cli.writers.players import StreamPlayer
 from bpkio_cli.writers.tables import display_table
@@ -62,15 +64,15 @@
         endpoint = api
         for p in path:
             endpoint = getattr(endpoint, p)
         return endpoint
 
     def retrieve_resource(id: int | str | None = None):
         ctx = click.get_current_context()
-        resource_context: ResourcesContext = ctx.obj.resources
+        resource_context: ResourceTrail = ctx.obj.resources
         if not id:
             id = resource_context.last()
         endpoint = get_api_endpoint()
         resource = endpoint.retrieve(id)
 
         # Record the resource
         if ctx.obj.cache and hasattr(resource, "id"):
@@ -115,14 +117,15 @@
         help=(
             f"The identifier of the {resource_title} to work with. "
             f"Leave empty for commands operating on a list of {resource_title}s."
             "You can use $ and @ notation to refer to previously selected resources"
         ),
     )
     @click.pass_context
+    @SessionRecorder.do_not_record
     def resource_group(ctx, id):
         if id:
             resource = retrieve_resource(id)
             if ctx.invoked_subcommand != "get":
                 display_resource_info(resource)
 
     # === CRUD Commands ===
@@ -161,26 +164,20 @@
             try:
                 ctx.invoke(table, header=False)
             except NameError:
                 pass
 
     # --- JSON Commmand
     @cloup.command(
-        help=f"Get the JSON representation of a single {resource_title} "
-        f"or list of {resource_title}s",
+        help=f"Get the JSON representation of a single {resource_title}",
     )
     @click.pass_obj
     def json(obj: AppContext):
-        try:
-            resource = retrieve_resource()
-            obj.response_handler.treat_single_resource(resource, json=True)
-        except UnknownResourceError:
-            endpoint = get_api_endpoint()
-            resources = endpoint.list()
-            obj.response_handler.treat_list_resources(resources, json=True)
+        resource = retrieve_resource()
+        obj.response_handler.treat_single_resource(resource, json=True)
 
     # --- SEARCH Command
     @cloup.command(
         help=f"Retrieve a list of all {resource_title}s "
         "that match given terms in all or selected fields"
     )
     @bic_options.search
@@ -213,29 +210,36 @@
     @click.pass_context
     def delete(ctx):
         resource = retrieve_resource()
 
         endpoint = get_api_endpoint()
         endpoint.delete(resource.id)
 
+        # remove from cache
+        ctx.obj.cache.remove(resource)
+
         click.secho(f"Resource {resource.id} deleted", fg="green")
 
     # --- UPDATE Command
     @cloup.command(aliases=["put"], help=f"Update a {resource_title}")
     @click.pass_context
     def update(ctx):
         resource = retrieve_resource()
+        resource_id = resource.id
+
+        # remap to an input model
+        resource = mappings.to_input_model(resource)
 
         updated_resource = edit_payload(resource)
 
         endpoint = get_api_endpoint()
         # TODO - try to parse into the resource class (otherwise can only work with specific resource sub-types)
-        endpoint.update(resource.id, updated_resource)
+        endpoint.update(resource_id, updated_resource)
 
-        click.secho(f"Resource {resource.id} updated", fg="green")
+        click.secho(f"Resource {resource_id} updated", fg="green")
 
     # --- DUPLICATE Command
     @cloup.command(aliases=["copy"], help=f"Duplicate a {resource_title}")
     @click.option(
         "-e",
         "--edit",
         help="Edit the duplicated resource before saving it",
@@ -268,15 +272,14 @@
     # === CONTENT Commands ===
 
     content_section = cloup.Section("Content commands", [])
 
     if any(x in with_content_commands for x in ["all", "url"]):
         # --- URL Command
         @cloup.command(help="Retrieve the full URL of the resource")
-        @bic_options.read
         @bic_options.url
         def url(
             sub: int,
             url: str,
             fqdn: str,
             **kwargs,
         ):
@@ -354,14 +357,15 @@
             url: str,
             fqdn: str,
             table: bool,
             raw: bool,
             top: bool,
             tail: bool,
             header: bool = True,
+            pager: bool = False,
         ):
             resource = retrieve_resource()
             handler = get_content_handler(
                 resource, replacement_fqdn=fqdn, extra_url=url, subplaylist_index=sub
             )
             if handler:
                 try:
@@ -370,14 +374,15 @@
                         max=1,
                         interval=0,
                         table=table,
                         raw=raw,
                         top=top,
                         tail=tail,
                         header=header,
+                        pager=pager,
                     )
                 except BroadpeakIoCliError as e:
                     pass
 
         content_section.add_command(read)
 
     if any(x in with_content_commands for x in ["all", "poll"]):
@@ -398,14 +403,15 @@
             interval: int,
             raw: bool,
             diff: bool,
             top: bool,
             tail: bool,
             clear: bool,
             table: bool,
+            pager: bool,
         ):
             resource = retrieve_resource()
             handler = get_content_handler(
                 resource, replacement_fqdn=fqdn, extra_url=url, subplaylist_index=sub
             )
 
             if handler:
@@ -415,14 +421,15 @@
                     interval=interval,
                     table=table,
                     raw=raw,
                     diff=diff,
                     top=top,
                     tail=tail,
                     clear=clear,
+                    pager=pager,
                 )
 
         content_section.add_command(poll)
 
     if any(x in with_content_commands for x in ["all", "play"]):
         # --- PLAY Command
         @cloup.command(
@@ -471,29 +478,43 @@
         @click.option(
             "--table/--no-table",
             "with_table",
             is_flag=True,
             default=False,
             help="Add or hide summary information about the content of the resource",
         )
+        @click.option(
+            "--save",
+            is_flag=True,
+            default=False,
+            help="Save the profile to a file",
+        )
         @bic_options.url
         @click.pass_obj
-        def profile(obj: AppContext, fqdn: str, url: str, sub: int, with_table: bool):
+        def profile(
+            obj: AppContext, fqdn: str, url: str, sub: int, with_table: bool, save: bool
+        ):
             resource = retrieve_resource()
             handler = get_content_handler(
                 resource, replacement_fqdn=fqdn, extra_url=url, subplaylist_index=sub
             )
 
             profile = make_transcoding_profile(handler)
 
             if with_table:
                 display_table(profile["transcoding"]["jobs"])
             else:
                 obj.response_handler.treat_single_resource(profile, json=True)
 
+            if save:
+                filename = f"profile_{resource.id}.json"
+                with open(filename, "w") as f:
+                    j.dump(profile, f, indent=4)
+                click.secho(f"Profile saved to {filename}", fg="green")
+
         content_section.add_command(profile)
 
     sections.append(content_section)
 
     # === PACKAGE Commands
 
     # COMMAND: PACKAGE
@@ -521,14 +542,20 @@
             for k in section.commands.keys():
                 if k == new_command.name:
                     # ... override an existing one ...
                     section.commands[k] = new_command
                     inserted = True
         if not inserted:
             # ... or add it to the last section
-            sections[-1].add_command(new_command)
+            if new_command.name in ["create", "update", "delete"]:
+                for section in sections:
+                    if section.title == "CRUD commands":
+                        section.add_command(new_command)
+                        break
+            else:
+                sections[-1].add_command(new_command)
 
     # === END OF GROUP ===
     for section in sections:
         resource_group.add_section(section)
 
     return resource_group
```

### Comparing `bpkio_cli-1.2.0/bpkio_cli/commands/template_crud_slots.py` & `bpkio_cli-1.3.0/bpkio_cli/commands/template_crud_slots.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from typing import List
 
 import click
 import cloup
+from bpkio_api.helpers.recorder import SessionRecorder
 from bpkio_api.helpers.times import to_local_tz, to_relative_time
 
-import bpkio_cli.options as bic_options
+import bpkio_cli.click_options as bic_options
 from bpkio_cli.click_mods.group_rest_resource import ApiResourceGroup
 from bpkio_cli.click_mods.option_eat_all import OptionEatAll
-from bpkio_cli.core.app_settings import AppContext
-from bpkio_cli.core.resources_context import ResourcesContext
+from bpkio_cli.core.app_context import AppContext
+from bpkio_cli.core.resource_trail import ResourceTrail
 from bpkio_cli.utils.datetimes import parse_date_expression_as_utc
 from bpkio_cli.writers.breadcrumbs import display_resource_info
 
 
 def create_child_resource_group(
     name: str,
     resource_class: type,
@@ -48,15 +49,15 @@
         api = click.get_current_context().obj.api
         endpoint = api
         for p in endpoint_path:
             endpoint = getattr(endpoint, p)
         return endpoint
 
     def retrieve_resource(id: int | str | None = None):
-        resource_context: ResourcesContext = click.get_current_context().obj.resources
+        resource_context: ResourceTrail = click.get_current_context().obj.resources
         if not id:
             id = resource_context.last()
         parent_id = resource_context.parent()
         endpoint = get_api_endpoint()
         return endpoint.retrieve(parent_id, id)
 
     # === GROUP ===
@@ -73,14 +74,15 @@
         "id",
         metavar=f"<{name.replace('-', '_')}_id>",
         help=(
             f"The identifier of the {resource_title} to work with. "
             f"Leave empty for commands operating on a list of {resource_title}s."
         ),
     )
+    @SessionRecorder.do_not_record
     def resource_group(id):
         if id:
             resource = retrieve_resource(id)
             display_resource_info(resource)
 
     # === CRUD Commands ===
 
@@ -183,15 +185,15 @@
         )
 
     # --- DELETE Commmand
     @cloup.command(aliases=["del"], help=f"Delete a specific {resource_title} by ID")
     @click.confirmation_option(prompt="Are you sure you want to delete this resource?")
     @click.pass_context
     def delete(ctx):
-        resource_context: ResourcesContext = click.get_current_context().obj.resources
+        resource_context: ResourceTrail = click.get_current_context().obj.resources
         id = resource_context.last()
         parent_id = resource_context.parent()
 
         endpoint = get_api_endpoint()
         endpoint.delete(parent_id, id)
 
         click.secho(f"Resource {id} deleted", fg="green")
```

### Comparing `bpkio_cli-1.2.0/bpkio_cli/commands/url.py` & `bpkio_cli-1.3.0/bpkio_cli/commands/url.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import click
 import cloup
 from bpkio_api.helpers.handlers import ContentHandler, factory
 from bpkio_api.helpers.source_type import SourceTypeDetector
 from bpkio_api.models import SourceType
 from pydantic import HttpUrl, parse_obj_as
 
-import bpkio_cli.options as bic_options
+import bpkio_cli.click_options as bic_options
 from bpkio_cli.click_mods import ApiResourceGroup
 from bpkio_cli.commands.sources import create as source_create
-from bpkio_cli.core.app_settings import AppContext
-from bpkio_cli.utils.config_provider import ConfigProvider
+from bpkio_cli.core.app_context import AppContext
+from bpkio_cli.core.config_provider import ConfigProvider
 from bpkio_cli.utils.profile_maker import make_transcoding_profile
 from bpkio_cli.writers.content_display import display_content
 from bpkio_cli.writers.players import StreamPlayer
 from bpkio_cli.writers.tables import display_table
 
 
 def determine_source_type(full_url) -> SourceType | None:
@@ -88,25 +88,28 @@
 @cloup.command(
     help="Loads and displays the content of a URL"
     ", optionally highlighted with relevant information"
 )
 @bic_options.read
 @bic_options.url
 @bic_options.table
-def read(sub: int, table: bool, raw: bool, top: bool, tail: bool, **kwargs):
+def read(
+    sub: int, table: bool, raw: bool, top: bool, tail: bool, pager: bool, **kwargs
+):
     handler = get_handler(sub)
 
     display_content(
         handler=handler,
         max=1,
         interval=0,
         table=table,
         raw=raw,
         top=top,
         tail=tail,
+        pager=pager,
     )
 
 
 # --- POLL Command
 @cloup.command(help="Similar to `read`, but regularly re-load the URL's content")
 @bic_options.read
 @bic_options.url
@@ -168,19 +171,20 @@
         player = StreamPlayer.prompt_player()
 
     StreamPlayer().launch(url=handler.url, template=player, name="")
 
 
 # --- CREATE Command
 @cloup.command(help="Create a Source from the URL")
+@cloup.option("--name", help="Name for the source", required=False)
 @click.pass_context
-def store(ctx):
+def store(ctx, name):
     full_url = ctx.obj.resources.last()
 
-    ctx.invoke(source_create, url=full_url)
+    ctx.invoke(source_create, url=full_url, name=name)
 
 
 # --- PROFILE Command
 @cloup.command(help="Create a Transcoding Profile from the content of the URL")
 @click.option(
     "--table/--no-table",
     "with_table",
```

### Comparing `bpkio_cli-1.2.0/bpkio_cli/core/app_settings.py` & `bpkio_cli-1.3.0/bpkio_cli/core/app_context.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 from typing import Optional
 
 from bpkio_api.api import BroadpeakIoApi
 from bpkio_api.models import Tenant
 
+from bpkio_cli.core.config_provider import ConfigProvider
 from bpkio_cli.core.resource_recorder import ResourceRecorder
-from bpkio_cli.core.resources_context import ResourcesContext
+from bpkio_cli.core.resource_trail import ResourceTrail
 from bpkio_cli.core.response_handler import ResponseHandler
-from bpkio_cli.utils.config_provider import ConfigProvider
 
 
 class AppContext:
-    def __init__(self, api: BroadpeakIoApi, tenant_provider):
+    def __init__(self, api: BroadpeakIoApi, tenant_provider=None):
         self.api = api
         self.tenant_provider = tenant_provider
         self._tenant: Optional[Tenant] = None
 
-        self.settings = dict()
-        self.resources = ResourcesContext()
+        self.flags = dict()
+        self.resources = ResourceTrail()
         self.cache: ResourceRecorder = None
         self.response_handler = ResponseHandler()
         self.config = ConfigProvider()
 
     @property
     def tenant(self):
         return self._tenant
 
     @tenant.setter
     def tenant(self, new_value: Tenant):
         self._tenant = new_value
         self.cache = ResourceRecorder(self.api.fqdn, new_value.id)
         self.response_handler = ResponseHandler(self.cache)
+
```

### Comparing `bpkio_cli-1.2.0/bpkio_cli/core/logger.py` & `bpkio_cli-1.3.0/bpkio_cli/core/logger.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.2.0/bpkio_cli/core/packager.py` & `bpkio_cli-1.3.0/bpkio_cli/core/packager.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 import logging
 import uuid
 from typing import Dict, List
 
 import bpkio_api.mappings as mappings
 import bpkio_api.models as models
+from bpkio_api.endpoints.enums import UpsertOperationType
 from bpkio_api.models.common import summary
 from pydantic import BaseModel
 
 logger = logging.getLogger(__name__)
 
 
 class ResourcePackager:
@@ -132,16 +133,14 @@
                 dict(guid=guid, model=in_obj.__class__.__name__, payload=json_payload)
             )
 
         return self.in_resources
 
 
 class PackageInstaller:
-    statuses = {1: "created", 0: "existing", -1: "error"}
-
     def __init__(self, api, name_suffix: str | None = None) -> None:
         self.guid_mappings: Dict = {}
         self.resources: Dict = {}
         self.api = api
         self._suffix = name_suffix
 
     def deploy(self, package: list):
@@ -192,24 +191,30 @@
                 else:
                     if hasattr(endpoint, "upsert"):
                         (resource, status) = endpoint.upsert(
                             in_obj, if_exists="retrieve"
                         )
                     elif hasattr(endpoint, "create"):
                         resource = endpoint.create(in_obj)
-                        status = 1
+                        status = UpsertOperationType.CREATED
                     else:
                         raise Exception(f"No create endpoint for model {model}")
             except Exception as e:
                 resource = in_obj
-                status = -1
+                status = UpsertOperationType.ERROR
                 message = e.args[0]
 
             logger.info(
-                f"{self.statuses[status]}: {resource.__class__.__name__} {resource.name} {resource.id} ({message})"
+                "{}: {} {} {} ({})".format(
+                    status.name,
+                    resource.__class__.__name__,
+                    resource.name,
+                    getattr(resource, "id", ""),
+                    message,
+                )
             )
 
             # Record the new ID, and map it to the guid
             if hasattr(resource, "id"):
                 self.guid_mappings[instruction["guid"]] = resource.id
                 self.resources[resource.id] = (resource, status, message)
             else:
```

### Comparing `bpkio_cli-1.2.0/bpkio_cli/core/resource_recorder.py` & `bpkio_cli-1.3.0/bpkio_cli/core/resource_recorder.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,46 +14,49 @@
     def __init__(self, fqdn: str, tenant: str | int):
         temp_dir = tempfile.gettempdir()
         cache_dir = os.path.join(temp_dir, "bpkio_cli", fqdn, str(tenant))
         logger.debug("Cache folder: " + cache_dir)
 
         self._resources_file = os.path.join(cache_dir, "resources.pkl")
         self._lists_file = os.path.join(cache_dir, "lists.pkl")
+        self._metadata_file = os.path.join(cache_dir, "metadata.pkl")
 
         self._cache_singles: MoveToFrontList = self._read_file_or_new(
             self._resources_file, MoveToFrontList(50)
         )
         self._cache_lists: dict = self._read_file_or_new(self._lists_file, dict())
+        self._cache_metadata: dict = self._read_file_or_new(self._metadata_file, dict())
 
     def _read_file_or_new(self, file_path: str, default):
         if os.path.exists(file_path):
             with open(file_path, "rb") as file:
                 try:
                     content = pickle.load(file)
                     if isinstance(content, default.__class__):
                         return content
-                except (
-                    pickle.UnpicklingError,
-                    EOFError,
-                    AttributeError,
-                    ModuleNotFoundError,
-                ):
+                except Exception:
                     logger.warning(
                         "Issue encountered with loading the cache. No cache will be used"
                     )
                     pass
 
         return default
 
     def clear(self):
+        """Reset the cache"""
         self._cache_singles = MoveToFrontList(maxlen=50)
         self._cache_lists = dict()
+        self._cache_metadata = dict()
         self.save()
 
     def save(self):
+        """Save the cache to disk.
+
+        This will overwrite any existing cache.
+        """
         try:
             os.makedirs(os.path.dirname(self._resources_file), exist_ok=True)
             with open(
                 self._resources_file,
                 "wb",
             ) as file:
                 pickle.dump(self._cache_singles, file)
@@ -62,56 +65,81 @@
 
         try:
             with open(self._lists_file, "wb") as file:
                 pickle.dump(self._cache_lists, file)
         except IOError:
             logger.warn("Unable to write Lists file to cache")
 
-    def record(self, value):
-        if isinstance(value, List) and len(value) > 0:
-            self._cache_lists[value[0].__class__.__name__] = value
+        try:
+            with open(self._metadata_file, "wb") as file:
+                pickle.dump(self._cache_metadata, file)
+        except IOError:
+            logger.warn("Unable to write Metadata file to cache")
+
+    def record(self, item):
+        """Add something to the cache.
+
+        The correct cache is chosen based on the type of the value to store"""
+        if isinstance(item, List) and len(item) > 0:
+            self._cache_lists[item[0].__class__.__name__] = item
         else:
-            self._cache_singles.add(value)
+            self._cache_singles.add(item)
+
+    def remove(self, item):
+        """Remove a value from the cache"""
+        self._cache_singles.remove(item)
+
+        # remove it from all lists too
+        for list in self._cache_lists.values():
+            if item in list:
+                list.remove(item)
 
-    def resolve(self, value, target_type):
+    def resolve(self, token, target_type):
         """Resolve non-integer references from data in the cache"""
-        if value == "$":
+        if token == "$":
             last_id = self.last_id_by_type(target_type)
             if last_id:
                 return str(last_id)
             else:
                 raise ValueError(
                     "There is no resource in memory that can be found to "
-                    "replace '$' for this context. It may have been deleted"
+                    "replace '$' for this context. Use an explicit ID"
                 )
 
-        if value.startswith("@"):
-            match = re.search(r"(-?\d+)", value)
+        if token.startswith("@"):
+            match = re.search(r"(-?\d+)", token)
             if match:
                 pos = int(match.group(1))
                 id = self.id_by_position_in_last_list_by_type(target_type, pos)
                 if id:
                     return str(id)
                 else:
                     raise ValueError(
                         f"There is no resource in position {pos} "
                         f"in the last list of {target_type.__name__}"
                     )
 
-        return value
+        return token
 
     def last_id(self):
         return getattr(self._cache_singles[0], "id", self._cache_singles[0])
 
     def last_id_by_type(self, type: type):
         candidates = [v for v in self._cache_singles.values() if isinstance(v, type)]
         if len(candidates):
             return getattr(candidates[0], "id", candidates[0])
 
     def id_by_position_in_last_list_by_type(self, type_: type, position: int):
+        """Find the id of a resource in a list of resources of a specific type.
+
+        The list of resources is found by looking at the cache, and the position
+        is found by looking at the last list of resources of that type.
+
+        If the list is empty, or the position is out of bounds, None is returned.
+        """
         if type_.__name__ in self._cache_lists:
             # Try strict type first:
             list = self._cache_lists[type_.__name__]
         else:
             try:
                 # Otherwise, find first list that contains super-types
                 list = next(
@@ -127,33 +155,84 @@
         except IndexError:
             raise RecorderCacheError(
                 f"The list of resources of type {type_.__name__} currently "
                 f"in cache only contains {len(list)} resources"
             )
 
     def list_resources(self):
+        """Return a list of all resources in the cache"""
         return self._cache_singles.values()
 
     def list_lists(self):
+        """Return a list of all lists in the cache"""
         return self._cache_lists
 
+    def record_metadata(self, item, key, value):
+        """Records metadata against an item"""
+        item_key = item.summary
+        if item_key not in self._cache_metadata:
+            self._cache_metadata[item_key] = dict()
+
+        if key not in self._cache_metadata[item_key]:
+            self._cache_metadata[item_key][key] = MoveToFrontList(maxlen=10)
+
+        self._cache_metadata[item_key][key].add(value)
+
+    def get_metadata(self, item, key):
+        """Returns the metadata for an item"""
+        item_key = item.summary
+        if item_key in self._cache_metadata:
+            lst: MoveToFrontList = self._cache_metadata[item_key].get(key)
+            if lst:
+                return lst.values()
+
+        return None
+
+    def list_metadata(self):
+        """Return a list of all metadata in the cache"""
+        return self._cache_metadata
+
+    def sort_resources_by_most_recently_accessed(self, original_list):
+        """Sort a list of resources by placing the most recently accessed first,
+        as recorded in the cache"""
+
+        accessed_resources = self.list_resources()
+        order_dict = {
+            getattr(item, "summary", str(item)): i
+            for i, item in enumerate(accessed_resources)
+        }
+
+        # Create a key function for the sorted() function
+        # If the object is in access_order, its sort key is its position,
+        # otherwise it's the length of access_order (which puts it at the end)
+        key_func = lambda obj: order_dict.get(obj.summary, len(accessed_resources))
+
+        # Sort the list
+        sorted_main_list = sorted(original_list, key=key_func)
+
+        return sorted_main_list
+
 
 class MoveToFrontList:
     def __init__(self, maxlen: int = None):
         self._list = []
         self._maxlen = maxlen
 
     def add(self, item):
         if item in self._list:
             self._list.remove(item)
         self._list.insert(0, item)
 
         if self._maxlen is not None and len(self._list) > self._maxlen:
             self._list.pop()
 
+    def remove(self, item):
+        if item in self._list:
+            self._list.remove(item)
+
     def search(self, item):
         if item in self._list:
             self._list.remove(item)
             self._list.insert(0, item)
             return True
         return False
 
@@ -168,11 +247,14 @@
 
     def __setitem__(self, key, value):
         self._list[key] = value
 
     def __delitem__(self, key):
         del self._list[key]
 
+    def __repr__(self) -> str:
+        return str(self._list)
+
 
 class RecorderCacheError(BroadpeakIoCliError):
     def __init__(self, message):
         super().__init__(message)
```

### Comparing `bpkio_cli-1.2.0/bpkio_cli/core/resources_context.py` & `bpkio_cli-1.3.0/bpkio_cli/core/resource_trail.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Dict, Optional
 
 
-class ResourcesContext:
+class ResourceTrail:
     def __init__(self) -> None:
         self._resource_breadcrumbs: Dict[str, int] = dict()
 
     # TODO - this needs to be moved to a separate object,
     # directly linked to the RestResourceGroup
     def record_resource_id(self, key, value):
         """Records a REST resource id, against a key (usually the name
```

### Comparing `bpkio_cli-1.2.0/bpkio_cli/core/response_handler.py` & `bpkio_cli-1.3.0/bpkio_cli/core/response_handler.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.2.0/bpkio_cli/options/admin.py` & `bpkio_cli-1.3.0/bpkio_cli/click_options/admin.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.2.0/bpkio_cli/options/list.py` & `bpkio_cli-1.3.0/bpkio_cli/click_options/list.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.2.0/bpkio_cli/options/poll.py` & `bpkio_cli-1.3.0/bpkio_cli/click_options/poll.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.2.0/bpkio_cli/options/read.py` & `bpkio_cli-1.3.0/bpkio_cli/click_options/read.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,12 +14,19 @@
     )
     @click.option(
         "--top", type=int, default=None, help="Only display the first N lines"
     )
     @click.option(
         "--tail", type=int, default=None, help="Only display the last N lines"
     )
+    @click.option(
+        "--pager/--no-pager",
+        type=bool,
+        is_flag=True,
+        default=None,
+        help="Display through a pager (to allow scrolling). If the flag is not set, a pager will automatically be used if the content is too long to fit on screen",
+    )
     @functools.wraps(fn)
     def wrapper(*args, **kwargs):
         return fn(*args, **kwargs)
 
     return wrapper
```

### Comparing `bpkio_cli-1.2.0/bpkio_cli/options/search.py` & `bpkio_cli-1.3.0/bpkio_cli/click_options/search.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.2.0/bpkio_cli/utils/arrays.py` & `bpkio_cli-1.3.0/bpkio_cli/utils/arrays.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.2.0/bpkio_cli/utils/config_provider.py` & `bpkio_cli-1.3.0/bpkio_cli/core/config_provider.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,19 +3,20 @@
 from typing import Any, Dict, List
 
 
 class ConfigProvider:
     def __init__(self, config_path="~/.bpkio/cli.cfg"):
         self.config_path = os.path.expanduser(config_path)
         self.config = configparser.ConfigParser()
+        self.temporary = dict()  # For temporary or overrides values
         self.initialize()
 
     def initialize(self):
         default_values = {
-            "settings": {"player": "browser", "editor": "vim"},
+            "settings": {"player": "browser", "editor": "vim", "verbose": "2"},
             "pygments": {"style": "monokai", "linenos": "0"},
             "players": {
                 "browser": "{url}",
                 "demo": "https://theoplayer.ridgeline.fr/?url1={url}&title1={name}&autoplay=true",
                 "hls": "https://hlsjs.video-dev.org/demo/?src={url}",
                 "dash": "https://reference.dashif.org/dash.js/nightly/samples/dash-if-reference-player/index.html?mpd={url}",
             },
@@ -32,22 +33,28 @@
                     self.config.add_section(section)
 
                 for key, value in values.items():
                     if key not in self.config[section]:
                         self._set(key, value, section)
 
     def get(self, key, cast_type=None, section="settings"):
-        value = self.config.get(section, key)
+        if key in self.temporary:
+            value = self.temporary[key]
+        else:
+            value = self.config.get(section, key)
+        
         return self.cast_value(value, cast_type)
 
     def cast_value(self, value, cast_type):
         if cast_type is None:
             return value
         elif cast_type == bool:
             return value.lower() in {"true", "1"}
+        elif cast_type == int:
+            return int(value)
         elif cast_type.__class__.__name__ == "Type":
             return cast_type(value)
         elif cast_type.__origin__ == List:
             item_type = cast_type.__args__[0]
             return [item_type(item.strip()) for item in value.split(",")]
         else:
             raise ValueError(f"Unsupported cast_type: {cast_type}")
@@ -69,18 +76,22 @@
             case "player":
                 self.set_player(value)
             case _:
                 if key not in self.config["settings"]:
                     raise ValueError(f"There is no setting called '{key}'.")
 
                 self._set(key, value)
+                
+    def set_temporary(self, key, value):
+        self.temporary[key] = value
 
     def save_config(self):
         with open(self.config_path, "w") as config_file:
             self.config.write(config_file)
+            
 
     # --- Specific config parameters ---
 
     def set_player(self, value):
         if value in self.config["players"]:
             self._set("player", value)
         else:
@@ -88,7 +99,8 @@
 
     def add_player(self, label, player_string):
         self.config.set("players", label, player_string)
         self.save_config()
 
     def list_players(self) -> Dict[str, Any]:
         return self.get_section_items("players")
+
```

### Comparing `bpkio_cli-1.2.0/bpkio_cli/utils/datetimes.py` & `bpkio_cli-1.3.0/bpkio_cli/utils/datetimes.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from datetime import datetime
 from typing import Optional
 
 import arrow
 import dateparser
+import pytimeparse
 import pytz
+from tzlocal import get_localzone
 
 
 def parse_date_string(date: str) -> float:
     return dateparser.parse(date).timestamp()
 
 
 def get_utc_date_ranges(
@@ -25,19 +27,25 @@
     return [(s.datetime, e.datetime) for (s, e) in range]
 
 
 def parse_date_expression_as_utc(exp: str | tuple | list) -> datetime:
     if isinstance(exp, (tuple, list)):
         exp = " ".join(exp)
 
-    current_tz_name = datetime.now().astimezone().strftime("%Z")
-    # current_tz_name = current_tz.zone
+    current_tz_name = str(get_localzone())
 
     # Parse the input string into a datetime object considering the timezone information
     dt_local = dateparser.parse(
         exp, settings={"TIMEZONE": current_tz_name, "RETURN_AS_TIMEZONE_AWARE": True}
     )
 
     # Convert the datetime object to UTC timezone
-    dt_utc = dt_local.astimezone(pytz.UTC)
+    dt_utc = dt_local.replace(microsecond=0).astimezone(pytz.UTC)
 
     return dt_utc
+
+
+def parse_duration_expression(t: str) -> float:
+    try:
+        return float(t)
+    except ValueError:
+        return pytimeparse.parse(t)
```

### Comparing `bpkio_cli-1.2.0/bpkio_cli/utils/editor.py` & `bpkio_cli-1.3.0/bpkio_cli/utils/editor.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import subprocess
 import tempfile
 
 import click
 from pydantic import BaseModel
 
-from bpkio_cli.utils.config_provider import ConfigProvider
+from bpkio_cli.core.config_provider import ConfigProvider
 
 
 def edit_payload(payload: object, is_json=False):
     if isinstance(payload, BaseModel):
         payload_str = json.dumps(json.loads(payload.json()), indent=2)
     else:
         if is_json:
```

### Comparing `bpkio_cli-1.2.0/bpkio_cli/utils/profile_maker.py` & `bpkio_cli-1.3.0/bpkio_cli/utils/profile_maker.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.2.0/bpkio_cli/writers/colorizer.py` & `bpkio_cli-1.3.0/bpkio_cli/writers/colorizer.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.2.0/bpkio_cli/writers/diff.py` & `bpkio_cli-1.3.0/bpkio_cli/writers/diff.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.2.0/bpkio_cli/writers/hls_formatter.py` & `bpkio_cli-1.3.0/bpkio_cli/writers/hls_formatter.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.2.0/bpkio_cli/writers/json_formatter.py` & `bpkio_cli-1.3.0/bpkio_cli/writers/json_formatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 
 from pygments import formatters, highlight, lexers
 
-from bpkio_cli.utils.config_provider import ConfigProvider
+from bpkio_cli.core.config_provider import ConfigProvider
 from bpkio_cli.writers.formatter import OutputFormatter
 
 
 class JSONFormatter(OutputFormatter):
     def __init__(self) -> None:
         super().__init__()
```

### Comparing `bpkio_cli-1.2.0/bpkio_cli/writers/players.py` & `bpkio_cli-1.3.0/bpkio_cli/writers/players.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import click
 from InquirerPy import inquirer
 
-from bpkio_cli.utils.config_provider import ConfigProvider
+from bpkio_cli.core.config_provider import ConfigProvider
+from bpkio_cli.utils.inquirer_defaults import select_markers
 
 
 class StreamPlayer:
     def __init__(self):
         self.config_provider = ConfigProvider()
         self._player_templates = None
 
@@ -35,12 +36,13 @@
         click.launch(full_url)
 
     def available_player_templates(self):
         return self.config_provider.list_players().keys()
 
     @staticmethod
     def prompt_player():
-        player = inquirer.select(
+        player = inquirer.fuzzy(
             message="What (top-level) resources do you want to include in the package?  ",
             choices=[p for p in StreamPlayer().available_player_templates()],
+            **select_markers(),
         ).execute()
         return player
```

### Comparing `bpkio_cli-1.2.0/bpkio_cli/writers/tables.py` & `bpkio_cli-1.3.0/bpkio_cli/writers/tables.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.2.0/bpkio_cli/writers/xml_formatter.py` & `bpkio_cli-1.3.0/bpkio_cli/writers/xml_formatter.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.2.0/pyproject.toml` & `bpkio_cli-1.3.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 [tool.poetry]
 name = "bpkio-cli"
-version = "1.2.0"
+version = "1.3.0"
 description = "A command line interface to the broadpeak.io APIs, with additional helpers"
 authors = ["Fabre Lambeau <fabre.lambeau@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "bpkio_cli" }]
 
 [tool.poetry-dynamic-versioning]
 enable = true
 vcs = "git"
 style = "semver"
 
 [tool.poetry-dynamic-versioning.substitution]
 files = ["*/__init__.py", "*/__version__.py", "*/_version.py"]
 
 [tool.poetry.dependencies]
-bpkio-python-sdk = "^1.1.0"
+bpkio-python-sdk = "^1.2.0"
 python = "^3.10"
 click = "^8.1.3"
 colorama = "^0.4.6"
 # inquirerpy = { git = "https://github.com/kazhala/InquirerPy" }
 inquirerpy = "^0.3.4"
 tabulate = "^0.9.0"
 arrow = "^1.2.3"
 dateparser = "^1.1.8"
 setuptools = "^67.6.1"
 cloup = "^2.0.0.post1"
 diskcache = "^5.4.0"
 pygments = "^2.15.1"
+pytimeparse = "^1.1.8"
 
 [tool.poetry.scripts]
-bic = "bpkio_cli.__main__:safe_entry_point"
-bic-debug = "bpkio_cli.__main__:debug_entry_point"
+bic = "bpkio_cli.app:safe_entry_point"
+bic-debug = "bpkio_cli.app:debug_entry_point"
 
 [tool.poetry.group.dev.dependencies]
 bpkio-python-sdk = { path = "../bpkio-python-sdk", develop = true }
 pytest = "^7.2.2"
 black = "^23.1.0"
 isort = "^5.12.0"
 flake8 = "^6.0.0"
```

### Comparing `bpkio_cli-1.2.0/PKG-INFO` & `bpkio_cli-1.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: bpkio-cli
-Version: 1.2.0
+Version: 1.3.0
 Summary: A command line interface to the broadpeak.io APIs, with additional helpers
 Author: Fabre Lambeau
 Author-email: fabre.lambeau@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: arrow (>=1.2.3,<2.0.0)
-Requires-Dist: bpkio-python-sdk (>=1.1.0,<2.0.0)
+Requires-Dist: bpkio-python-sdk (>=1.2.0,<2.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: cloup (>=2.0.0.post1,<3.0.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: dateparser (>=1.1.8,<2.0.0)
 Requires-Dist: diskcache (>=5.4.0,<6.0.0)
 Requires-Dist: inquirerpy (>=0.3.4,<0.4.0)
 Requires-Dist: pygments (>=2.15.1,<3.0.0)
+Requires-Dist: pytimeparse (>=1.1.8,<2.0.0)
 Requires-Dist: setuptools (>=67.6.1,<68.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
```

