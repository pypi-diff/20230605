# Comparing `tmp/kui-1.3.7.tar.gz` & `tmp/kui-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kui-1.3.7.tar", last modified: Thu Apr 20 06:02:16 2023, max compression
+gzip compressed data, was "kui-1.4.0.tar", last modified: Mon Jun  5 05:55:36 2023, max compression
```

## Comparing `kui-1.3.7.tar` & `kui-1.4.0.tar`

### file list

```diff
@@ -1,85 +1,86 @@
--rw-r--r--   0        0        0    11341 2023-04-20 06:01:59.028175 kui-1.3.7/LICENSE
--rw-r--r--   0        0        0      440 2023-04-20 06:01:59.028175 kui-1.3.7/README.md
--rw-r--r--   0        0        0        0 2023-04-20 06:01:59.032175 kui-1.3.7/kui/__init__.py
--rw-r--r--   0        0        0       63 2023-04-20 06:01:59.032175 kui-1.3.7/kui/__version__.py
--rw-r--r--   0        0        0     1754 2023-04-20 06:01:59.032175 kui-1.3.7/kui/asgi/__init__.py
--rw-r--r--   0        0        0     8139 2023-04-20 06:01:59.032175 kui-1.3.7/kui/asgi/applications.py
--rw-r--r--   0        0        0     2090 2023-04-20 06:01:59.032175 kui-1.3.7/kui/asgi/cors.py
--rw-r--r--   0        0        0     2366 2023-04-20 06:01:59.032175 kui-1.3.7/kui/asgi/exceptions.py
--rw-r--r--   0        0        0     1470 2023-04-20 06:01:59.032175 kui-1.3.7/kui/asgi/openapi.py
--rw-r--r--   0        0        0     5502 2023-04-20 06:01:59.032175 kui-1.3.7/kui/asgi/parameters.py
--rw-r--r--   0        0        0     3754 2023-04-20 06:01:59.032175 kui-1.3.7/kui/asgi/requests.py
--rw-r--r--   0        0        0     2879 2023-04-20 06:01:59.032175 kui-1.3.7/kui/asgi/responses.py
--rw-r--r--   0        0        0      972 2023-04-20 06:01:59.032175 kui-1.3.7/kui/asgi/routing.py
--rw-r--r--   0        0        0     3177 2023-04-20 06:01:59.032175 kui-1.3.7/kui/asgi/templates.py
--rw-r--r--   0        0        0     4614 2023-04-20 06:01:59.032175 kui-1.3.7/kui/asgi/views.py
--rw-r--r--   0        0        0     3849 2023-04-20 06:01:59.032175 kui-1.3.7/kui/exceptions.py
--rw-r--r--   0        0        0      123 2023-04-20 06:01:59.032175 kui-1.3.7/kui/openapi/__init__.py
--rw-r--r--   0        0        0     9465 2023-04-20 06:01:59.032175 kui-1.3.7/kui/openapi/application.py
--rw-r--r--   0        0        0     1565 2023-04-20 06:01:59.032175 kui-1.3.7/kui/openapi/extra_docs.py
--rw-r--r--   0        0        0     1632 2023-04-20 06:01:59.032175 kui-1.3.7/kui/openapi/schema.py
--rw-r--r--   0        0        0     7726 2023-04-20 06:01:59.032175 kui-1.3.7/kui/openapi/specification.py
--rw-r--r--   0        0        0      224 2023-04-20 06:01:59.032175 kui-1.3.7/kui/openapi/templates/rapidoc.html
--rw-r--r--   0        0        0      743 2023-04-20 06:01:59.032175 kui-1.3.7/kui/openapi/templates/redoc.html
--rw-r--r--   0        0        0     1522 2023-04-20 06:01:59.032175 kui-1.3.7/kui/openapi/templates/swagger.html
--rw-r--r--   0        0        0      586 2023-04-20 06:01:59.032175 kui-1.3.7/kui/openapi/types.py
--rw-r--r--   0        0        0    15327 2023-04-20 06:01:59.032175 kui-1.3.7/kui/parameters/__init__.py
--rw-r--r--   0        0        0     9051 2023-04-20 06:01:59.032175 kui-1.3.7/kui/parameters/field_functions.py
--rw-r--r--   0        0        0     2219 2023-04-20 06:01:59.032175 kui-1.3.7/kui/parameters/fields.py
--rw-r--r--   0        0        0        0 2023-04-20 06:01:59.032175 kui-1.3.7/kui/py.typed
--rw-r--r--   0        0        0     7577 2023-04-20 06:01:59.032175 kui-1.3.7/kui/responses.py
--rw-r--r--   0        0        0      429 2023-04-20 06:01:59.032175 kui-1.3.7/kui/routing/__init__.py
--rw-r--r--   0        0        0       82 2023-04-20 06:01:59.032175 kui-1.3.7/kui/routing/__main__.py
--rw-r--r--   0        0        0     1402 2023-04-20 06:01:59.032175 kui-1.3.7/kui/routing/commands.py
--rw-r--r--   0        0        0      130 2023-04-20 06:01:59.032175 kui-1.3.7/kui/routing/extensions/__init__.py
--rw-r--r--   0        0        0     2551 2023-04-20 06:01:59.032175 kui-1.3.7/kui/routing/extensions/file.py
--rw-r--r--   0        0        0     2982 2023-04-20 06:01:59.032175 kui-1.3.7/kui/routing/extensions/multimethod.py
--rw-r--r--   0        0        0    17789 2023-04-20 06:01:59.032175 kui-1.3.7/kui/routing/routers.py
--rw-r--r--   0        0        0     3040 2023-04-20 06:01:59.032175 kui-1.3.7/kui/routing/routes.py
--rw-r--r--   0        0        0     6234 2023-04-20 06:01:59.032175 kui-1.3.7/kui/routing/tree.py
--rw-r--r--   0        0        0      273 2023-04-20 06:01:59.032175 kui-1.3.7/kui/routing/typing.py
--rw-r--r--   0        0        0     2825 2023-04-20 06:01:59.032175 kui-1.3.7/kui/security.py
--rw-r--r--   0        0        0     2783 2023-04-20 06:01:59.032175 kui-1.3.7/kui/status.py
--rw-r--r--   0        0        0     1250 2023-04-20 06:01:59.032175 kui-1.3.7/kui/templates.py
--rw-r--r--   0        0        0      757 2023-04-20 06:01:59.032175 kui-1.3.7/kui/utils/__init__.py
--rw-r--r--   0        0        0      856 2023-04-20 06:01:59.032175 kui-1.3.7/kui/utils/contextvars.py
--rw-r--r--   0        0        0     1576 2023-04-20 06:01:59.032175 kui-1.3.7/kui/utils/importer.py
--rw-r--r--   0        0        0     1907 2023-04-20 06:01:59.032175 kui-1.3.7/kui/utils/inspect.py
--rw-r--r--   0        0        0     1647 2023-04-20 06:01:59.032175 kui-1.3.7/kui/utils/objects.py
--rw-r--r--   0        0        0      530 2023-04-20 06:01:59.032175 kui-1.3.7/kui/utils/pipe.py
--rw-r--r--   0        0        0     1123 2023-04-20 06:01:59.032175 kui-1.3.7/kui/utils/state.py
--rw-r--r--   0        0        0     1603 2023-04-20 06:01:59.032175 kui-1.3.7/kui/wsgi/__init__.py
--rw-r--r--   0        0        0     5249 2023-04-20 06:01:59.032175 kui-1.3.7/kui/wsgi/applications.py
--rw-r--r--   0        0        0     2067 2023-04-20 06:01:59.032175 kui-1.3.7/kui/wsgi/cors.py
--rw-r--r--   0        0        0     2309 2023-04-20 06:01:59.032175 kui-1.3.7/kui/wsgi/exceptions.py
--rw-r--r--   0        0        0     1428 2023-04-20 06:01:59.032175 kui-1.3.7/kui/wsgi/openapi.py
--rw-r--r--   0        0        0     4204 2023-04-20 06:01:59.032175 kui-1.3.7/kui/wsgi/parameters.py
--rw-r--r--   0        0        0     1833 2023-04-20 06:01:59.032175 kui-1.3.7/kui/wsgi/requests.py
--rw-r--r--   0        0        0     2879 2023-04-20 06:01:59.032175 kui-1.3.7/kui/wsgi/responses.py
--rw-r--r--   0        0        0      966 2023-04-20 06:01:59.032175 kui-1.3.7/kui/wsgi/routing.py
--rw-r--r--   0        0        0     2884 2023-04-20 06:01:59.032175 kui-1.3.7/kui/wsgi/templates.py
--rw-r--r--   0        0        0     2281 2023-04-20 06:01:59.032175 kui-1.3.7/kui/wsgi/views.py
--rw-r--r--   0        0        0     2208 2023-04-20 06:01:59.036175 kui-1.3.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-20 06:01:59.036175 kui-1.3.7/tests/asgi/__init__.py
--rw-r--r--   0        0        0     2416 2023-04-20 06:01:59.036175 kui-1.3.7/tests/asgi/test_application.py
--rw-r--r--   0        0        0      689 2023-04-20 06:01:59.036175 kui-1.3.7/tests/asgi/test_cors.py
--rw-r--r--   0        0        0     7058 2023-04-20 06:01:59.036175 kui-1.3.7/tests/asgi/test_parameters.py
--rw-r--r--   0        0        0      535 2023-04-20 06:01:59.036175 kui-1.3.7/tests/asgi/test_views.py
--rw-r--r--   0        0        0    32402 2023-04-20 06:01:59.036175 kui-1.3.7/tests/openapi/test_application.py
--rw-r--r--   0        0        0      429 2023-04-20 06:01:59.036175 kui-1.3.7/tests/openapi/test_extra_docs.py
--rw-r--r--   0        0        0      247 2023-04-20 06:01:59.036175 kui-1.3.7/tests/routing/extensions/test_fileroutes.py
--rw-r--r--   0        0        0     3155 2023-04-20 06:01:59.036175 kui-1.3.7/tests/routing/extensions/test_multimethod.py
--rw-r--r--   0        0        0       88 2023-04-20 06:01:59.036175 kui-1.3.7/tests/routing/test_commands.py
--rw-r--r--   0        0        0     3788 2023-04-20 06:01:59.036175 kui-1.3.7/tests/routing/test_routes.py
--rw-r--r--   0        0        0     2444 2023-04-20 06:01:59.036175 kui-1.3.7/tests/routing/test_tree.py
--rw-r--r--   0        0        0      242 2023-04-20 06:01:59.036175 kui-1.3.7/tests/test_export_all.py
--rw-r--r--   0        0        0     4505 2023-04-20 06:01:59.036175 kui-1.3.7/tests/test_responses.py
--rw-r--r--   0        0        0     3032 2023-04-20 06:01:59.036175 kui-1.3.7/tests/test_security.py
--rw-r--r--   0        0        0        0 2023-04-20 06:01:59.036175 kui-1.3.7/tests/utils/__init__.py
--rw-r--r--   0        0        0      722 2023-04-20 06:01:59.036175 kui-1.3.7/tests/utils/test_importer.py
--rw-r--r--   0        0        0      170 2023-04-20 06:01:59.036175 kui-1.3.7/tests/utils/test_objects.py
--rw-r--r--   0        0        0      426 2023-04-20 06:01:59.036175 kui-1.3.7/tests/utils/test_state.py
--rw-r--r--   0        0        0      648 2023-04-20 06:01:59.036175 kui-1.3.7/tests/wsgi/test_cors.py
--rw-r--r--   0        0        0     6790 2023-04-20 06:01:59.036175 kui-1.3.7/tests/wsgi/test_parameters.py
--rw-r--r--   0        0        0      453 2023-04-20 06:01:59.036175 kui-1.3.7/tests/wsgi/test_views.py
--rw-r--r--   0        0        0     1032 1970-01-01 00:00:00.000000 kui-1.3.7/PKG-INFO
+-rw-r--r--   0        0        0    11341 2023-06-05 05:55:19.288698 kui-1.4.0/LICENSE
+-rw-r--r--   0        0        0      440 2023-06-05 05:55:19.288698 kui-1.4.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-05 05:55:19.288698 kui-1.4.0/kui/__init__.py
+-rw-r--r--   0        0        0       63 2023-06-05 05:55:19.288698 kui-1.4.0/kui/__version__.py
+-rw-r--r--   0        0        0     1754 2023-06-05 05:55:19.288698 kui-1.4.0/kui/asgi/__init__.py
+-rw-r--r--   0        0        0     8405 2023-06-05 05:55:19.288698 kui-1.4.0/kui/asgi/applications.py
+-rw-r--r--   0        0        0     2090 2023-06-05 05:55:19.288698 kui-1.4.0/kui/asgi/cors.py
+-rw-r--r--   0        0        0     2366 2023-06-05 05:55:19.288698 kui-1.4.0/kui/asgi/exceptions.py
+-rw-r--r--   0        0        0     1470 2023-06-05 05:55:19.288698 kui-1.4.0/kui/asgi/openapi.py
+-rw-r--r--   0        0        0     5502 2023-06-05 05:55:19.288698 kui-1.4.0/kui/asgi/parameters.py
+-rw-r--r--   0        0        0     3754 2023-06-05 05:55:19.288698 kui-1.4.0/kui/asgi/requests.py
+-rw-r--r--   0        0        0     2879 2023-06-05 05:55:19.288698 kui-1.4.0/kui/asgi/responses.py
+-rw-r--r--   0        0        0      972 2023-06-05 05:55:19.288698 kui-1.4.0/kui/asgi/routing.py
+-rw-r--r--   0        0        0     3177 2023-06-05 05:55:19.288698 kui-1.4.0/kui/asgi/templates.py
+-rw-r--r--   0        0        0     4614 2023-06-05 05:55:19.288698 kui-1.4.0/kui/asgi/views.py
+-rw-r--r--   0        0        0      304 2023-06-05 05:55:19.288698 kui-1.4.0/kui/cors.py
+-rw-r--r--   0        0        0     3849 2023-06-05 05:55:19.288698 kui-1.4.0/kui/exceptions.py
+-rw-r--r--   0        0        0      123 2023-06-05 05:55:19.288698 kui-1.4.0/kui/openapi/__init__.py
+-rw-r--r--   0        0        0     9465 2023-06-05 05:55:19.288698 kui-1.4.0/kui/openapi/application.py
+-rw-r--r--   0        0        0     1565 2023-06-05 05:55:19.288698 kui-1.4.0/kui/openapi/extra_docs.py
+-rw-r--r--   0        0        0     1632 2023-06-05 05:55:19.288698 kui-1.4.0/kui/openapi/schema.py
+-rw-r--r--   0        0        0     7726 2023-06-05 05:55:19.288698 kui-1.4.0/kui/openapi/specification.py
+-rw-r--r--   0        0        0      224 2023-06-05 05:55:19.288698 kui-1.4.0/kui/openapi/templates/rapidoc.html
+-rw-r--r--   0        0        0      743 2023-06-05 05:55:19.288698 kui-1.4.0/kui/openapi/templates/redoc.html
+-rw-r--r--   0        0        0     1522 2023-06-05 05:55:19.288698 kui-1.4.0/kui/openapi/templates/swagger.html
+-rw-r--r--   0        0        0      586 2023-06-05 05:55:19.288698 kui-1.4.0/kui/openapi/types.py
+-rw-r--r--   0        0        0    15327 2023-06-05 05:55:19.288698 kui-1.4.0/kui/parameters/__init__.py
+-rw-r--r--   0        0        0     9051 2023-06-05 05:55:19.288698 kui-1.4.0/kui/parameters/field_functions.py
+-rw-r--r--   0        0        0     2219 2023-06-05 05:55:19.288698 kui-1.4.0/kui/parameters/fields.py
+-rw-r--r--   0        0        0        0 2023-06-05 05:55:19.288698 kui-1.4.0/kui/py.typed
+-rw-r--r--   0        0        0     7577 2023-06-05 05:55:19.288698 kui-1.4.0/kui/responses.py
+-rw-r--r--   0        0        0      429 2023-06-05 05:55:19.288698 kui-1.4.0/kui/routing/__init__.py
+-rw-r--r--   0        0        0       82 2023-06-05 05:55:19.288698 kui-1.4.0/kui/routing/__main__.py
+-rw-r--r--   0        0        0     1402 2023-06-05 05:55:19.288698 kui-1.4.0/kui/routing/commands.py
+-rw-r--r--   0        0        0      130 2023-06-05 05:55:19.288698 kui-1.4.0/kui/routing/extensions/__init__.py
+-rw-r--r--   0        0        0     2551 2023-06-05 05:55:19.288698 kui-1.4.0/kui/routing/extensions/file.py
+-rw-r--r--   0        0        0     2982 2023-06-05 05:55:19.288698 kui-1.4.0/kui/routing/extensions/multimethod.py
+-rw-r--r--   0        0        0    17890 2023-06-05 05:55:19.288698 kui-1.4.0/kui/routing/routers.py
+-rw-r--r--   0        0        0     3040 2023-06-05 05:55:19.288698 kui-1.4.0/kui/routing/routes.py
+-rw-r--r--   0        0        0     6234 2023-06-05 05:55:19.288698 kui-1.4.0/kui/routing/tree.py
+-rw-r--r--   0        0        0      273 2023-06-05 05:55:19.288698 kui-1.4.0/kui/routing/typing.py
+-rw-r--r--   0        0        0     2825 2023-06-05 05:55:19.288698 kui-1.4.0/kui/security.py
+-rw-r--r--   0        0        0     2783 2023-06-05 05:55:19.288698 kui-1.4.0/kui/status.py
+-rw-r--r--   0        0        0     1250 2023-06-05 05:55:19.288698 kui-1.4.0/kui/templates.py
+-rw-r--r--   0        0        0      757 2023-06-05 05:55:19.288698 kui-1.4.0/kui/utils/__init__.py
+-rw-r--r--   0        0        0      856 2023-06-05 05:55:19.288698 kui-1.4.0/kui/utils/contextvars.py
+-rw-r--r--   0        0        0     1576 2023-06-05 05:55:19.288698 kui-1.4.0/kui/utils/importer.py
+-rw-r--r--   0        0        0     1907 2023-06-05 05:55:19.288698 kui-1.4.0/kui/utils/inspect.py
+-rw-r--r--   0        0        0     1647 2023-06-05 05:55:19.288698 kui-1.4.0/kui/utils/objects.py
+-rw-r--r--   0        0        0      530 2023-06-05 05:55:19.288698 kui-1.4.0/kui/utils/pipe.py
+-rw-r--r--   0        0        0     1123 2023-06-05 05:55:19.288698 kui-1.4.0/kui/utils/state.py
+-rw-r--r--   0        0        0     1603 2023-06-05 05:55:19.288698 kui-1.4.0/kui/wsgi/__init__.py
+-rw-r--r--   0        0        0     5515 2023-06-05 05:55:19.288698 kui-1.4.0/kui/wsgi/applications.py
+-rw-r--r--   0        0        0     2067 2023-06-05 05:55:19.288698 kui-1.4.0/kui/wsgi/cors.py
+-rw-r--r--   0        0        0     2309 2023-06-05 05:55:19.288698 kui-1.4.0/kui/wsgi/exceptions.py
+-rw-r--r--   0        0        0     1428 2023-06-05 05:55:19.288698 kui-1.4.0/kui/wsgi/openapi.py
+-rw-r--r--   0        0        0     4204 2023-06-05 05:55:19.288698 kui-1.4.0/kui/wsgi/parameters.py
+-rw-r--r--   0        0        0     1833 2023-06-05 05:55:19.288698 kui-1.4.0/kui/wsgi/requests.py
+-rw-r--r--   0        0        0     2879 2023-06-05 05:55:19.288698 kui-1.4.0/kui/wsgi/responses.py
+-rw-r--r--   0        0        0      966 2023-06-05 05:55:19.288698 kui-1.4.0/kui/wsgi/routing.py
+-rw-r--r--   0        0        0     2884 2023-06-05 05:55:19.288698 kui-1.4.0/kui/wsgi/templates.py
+-rw-r--r--   0        0        0     2281 2023-06-05 05:55:19.288698 kui-1.4.0/kui/wsgi/views.py
+-rw-r--r--   0        0        0     2189 2023-06-05 05:55:19.292698 kui-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-05 05:55:19.292698 kui-1.4.0/tests/asgi/__init__.py
+-rw-r--r--   0        0        0     2416 2023-06-05 05:55:19.292698 kui-1.4.0/tests/asgi/test_application.py
+-rw-r--r--   0        0        0     1338 2023-06-05 05:55:19.292698 kui-1.4.0/tests/asgi/test_cors.py
+-rw-r--r--   0        0        0     7058 2023-06-05 05:55:19.292698 kui-1.4.0/tests/asgi/test_parameters.py
+-rw-r--r--   0        0        0      535 2023-06-05 05:55:19.292698 kui-1.4.0/tests/asgi/test_views.py
+-rw-r--r--   0        0        0    32402 2023-06-05 05:55:19.292698 kui-1.4.0/tests/openapi/test_application.py
+-rw-r--r--   0        0        0      429 2023-06-05 05:55:19.292698 kui-1.4.0/tests/openapi/test_extra_docs.py
+-rw-r--r--   0        0        0      247 2023-06-05 05:55:19.292698 kui-1.4.0/tests/routing/extensions/test_fileroutes.py
+-rw-r--r--   0        0        0     3155 2023-06-05 05:55:19.292698 kui-1.4.0/tests/routing/extensions/test_multimethod.py
+-rw-r--r--   0        0        0       88 2023-06-05 05:55:19.292698 kui-1.4.0/tests/routing/test_commands.py
+-rw-r--r--   0        0        0     4076 2023-06-05 05:55:19.292698 kui-1.4.0/tests/routing/test_routes.py
+-rw-r--r--   0        0        0     2444 2023-06-05 05:55:19.292698 kui-1.4.0/tests/routing/test_tree.py
+-rw-r--r--   0        0        0      242 2023-06-05 05:55:19.292698 kui-1.4.0/tests/test_export_all.py
+-rw-r--r--   0        0        0     4505 2023-06-05 05:55:19.292698 kui-1.4.0/tests/test_responses.py
+-rw-r--r--   0        0        0     3032 2023-06-05 05:55:19.292698 kui-1.4.0/tests/test_security.py
+-rw-r--r--   0        0        0        0 2023-06-05 05:55:19.292698 kui-1.4.0/tests/utils/__init__.py
+-rw-r--r--   0        0        0      722 2023-06-05 05:55:19.292698 kui-1.4.0/tests/utils/test_importer.py
+-rw-r--r--   0        0        0      170 2023-06-05 05:55:19.292698 kui-1.4.0/tests/utils/test_objects.py
+-rw-r--r--   0        0        0      426 2023-06-05 05:55:19.292698 kui-1.4.0/tests/utils/test_state.py
+-rw-r--r--   0        0        0     1290 2023-06-05 05:55:19.292698 kui-1.4.0/tests/wsgi/test_cors.py
+-rw-r--r--   0        0        0     6790 2023-06-05 05:55:19.292698 kui-1.4.0/tests/wsgi/test_parameters.py
+-rw-r--r--   0        0        0      453 2023-06-05 05:55:19.292698 kui-1.4.0/tests/wsgi/test_views.py
+-rw-r--r--   0        0        0     1032 1970-01-01 00:00:00.000000 kui-1.4.0/PKG-INFO
```

### Comparing `kui-1.3.7/LICENSE` & `kui-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/kui/asgi/__init__.py` & `kui-1.4.0/kui/asgi/__init__.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/kui/asgi/applications.py` & `kui-1.4.0/kui/asgi/applications.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,16 +19,18 @@
     TypeVar,
 )
 
 from baize.datastructures import URL
 from baize.typing import Receive, Scope, Send
 from typing_extensions import Literal
 
+from ..cors import CORSConfig
 from ..routing import AsyncViewType, BaseRoute, MiddlewareType, NoMatchFound
 from ..utils import ImmutableAttribute, State
+from .cors import allow_cors
 from .exceptions import ErrorHandlerType, ExceptionMiddleware, HTTPException
 from .requests import HttpRequest, WebSocket, request_var, websocket_var
 from .responses import (
     FileResponse,
     HttpResponse,
     JSONResponse,
     PlainTextResponse,
@@ -96,28 +98,35 @@
         templates: Optional[BaseTemplates] = None,
         on_startup: List[LifespanCallback] = [],
         on_shutdown: List[LifespanCallback] = [],
         routes: Iterable[BaseRoute] = [],
         http_middlewares: List[MiddlewareType[AsyncViewType]] = [],
         socket_middlewares: List[MiddlewareType[AsyncViewType]] = [],
         exception_handlers: Mapping[int | Type[BaseException], ErrorHandlerType] = {},
+        cors_config: Optional[CORSConfig] = None,
         factory_class: FactoryClass = FactoryClass(),
         response_converters: Mapping[type, Callable[..., HttpResponse]] = {},
     ) -> None:
         self.should_exit = False
 
         self.state = State()
         self.response_converter = create_response_converter(response_converters)
         self.factory_class = factory_class
         self.templates = templates
         self.lifespan = Lifespan(copy.copy(on_startup), copy.copy(on_shutdown))
+
+        http_middlewares = [*http_middlewares]
+
         self.exception_middleware = ExceptionMiddleware(exception_handlers)
-        self.router = Router(
-            routes, [*http_middlewares, self.exception_middleware], socket_middlewares
-        )
+        http_middlewares.append(self.exception_middleware)
+
+        if cors_config is not None:
+            http_middlewares.append(allow_cors(**cors_config))
+
+        self.router = Router(routes, http_middlewares, socket_middlewares)
 
     def add_exception_handler(
         self, exc_class_or_status_code: int | Type[Exception], handler: ErrorHandlerType
     ) -> None:
         self.exception_middleware.add_exception_handler(
             exc_class_or_status_code, handler
         )
```

### Comparing `kui-1.3.7/kui/asgi/cors.py` & `kui-1.4.0/kui/asgi/cors.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/kui/asgi/exceptions.py` & `kui-1.4.0/kui/asgi/exceptions.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/kui/asgi/openapi.py` & `kui-1.4.0/kui/asgi/openapi.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/kui/asgi/parameters.py` & `kui-1.4.0/kui/asgi/parameters.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/kui/asgi/requests.py` & `kui-1.4.0/kui/asgi/requests.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/kui/asgi/responses.py` & `kui-1.4.0/kui/asgi/responses.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/kui/asgi/routing.py` & `kui-1.4.0/kui/asgi/routing.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/kui/asgi/templates.py` & `kui-1.4.0/kui/asgi/templates.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/kui/asgi/views.py` & `kui-1.4.0/kui/asgi/views.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/kui/exceptions.py` & `kui-1.4.0/kui/exceptions.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/kui/openapi/application.py` & `kui-1.4.0/kui/openapi/application.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/kui/openapi/extra_docs.py` & `kui-1.4.0/kui/openapi/extra_docs.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/kui/openapi/schema.py` & `kui-1.4.0/kui/openapi/schema.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/kui/openapi/specification.py` & `kui-1.4.0/kui/openapi/specification.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/kui/openapi/templates/redoc.html` & `kui-1.4.0/kui/openapi/templates/redoc.html`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/kui/openapi/templates/swagger.html` & `kui-1.4.0/kui/openapi/templates/swagger.html`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/kui/openapi/types.py` & `kui-1.4.0/kui/openapi/types.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/kui/parameters/__init__.py` & `kui-1.4.0/kui/parameters/__init__.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/kui/parameters/field_functions.py` & `kui-1.4.0/kui/parameters/field_functions.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/kui/parameters/fields.py` & `kui-1.4.0/kui/parameters/fields.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/kui/responses.py` & `kui-1.4.0/kui/responses.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/kui/routing/commands.py` & `kui-1.4.0/kui/routing/commands.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/kui/routing/extensions/file.py` & `kui-1.4.0/kui/routing/extensions/file.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/kui/routing/extensions/multimethod.py` & `kui-1.4.0/kui/routing/extensions/multimethod.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/kui/routing/routers.py` & `kui-1.4.0/kui/routing/routers.py`

 * *Files 2% similar despite different names*

```diff
@@ -379,22 +379,19 @@
             _ = self << route
 
     @typing.overload
     def __getitem__(self, index: int) -> BaseRoute[ViewType]:
         ...
 
     @typing.overload
-    def __getitem__(self, index: slice) -> typing.NoReturn:
+    def __getitem__(self, index: slice) -> typing.List[BaseRoute[ViewType]]:
         ...
 
     def __getitem__(self, index):
-        if isinstance(index, int):
-            return self._list[index]
-        else:
-            raise TypeError("Slicing syntax is not allowed")
+        return self._list[index]
 
     def __len__(self) -> int:
         return len(self._list)
 
     def append(self: Self, route: BaseRoute[ViewType]) -> Self:
         self._list.append(route)
         return self
@@ -436,14 +433,17 @@
             @routes.http_middleware
             def middleware(endpoint):
                 async def wrapper():
                     return await endpoint()
                 return wrapper
         ```
         """
+        if len(self) > 0:
+            raise RuntimeError("Can not append middleware after route")
+
         self._http_middlewares.append(middleware)
         return middleware
 
     def socket_middleware(self, middleware: MiddlewareType) -> MiddlewareType:
         """
         append middleware in routes
 
@@ -452,14 +452,17 @@
             @routes.socket_middleware
             def middleware(endpoint):
                 async def wrapper():
                     await endpoint()
                 return wrapper
         ```
         """
+        if len(self) > 0:
+            raise RuntimeError("Can not append middleware after route")
+
         self._socket_middlewares.append(middleware)
         return middleware
 
 
 _RouteSequence = typing.TypeVar("_RouteSequence", bound=typing.Iterable[BaseRoute])
```

### Comparing `kui-1.3.7/kui/routing/routes.py` & `kui-1.4.0/kui/routing/routes.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/kui/routing/tree.py` & `kui-1.4.0/kui/routing/tree.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/kui/security.py` & `kui-1.4.0/kui/security.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/kui/status.py` & `kui-1.4.0/kui/status.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/kui/templates.py` & `kui-1.4.0/kui/templates.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/kui/utils/__init__.py` & `kui-1.4.0/kui/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/kui/utils/contextvars.py` & `kui-1.4.0/kui/utils/contextvars.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/kui/utils/importer.py` & `kui-1.4.0/kui/utils/importer.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/kui/utils/inspect.py` & `kui-1.4.0/kui/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/kui/utils/objects.py` & `kui-1.4.0/kui/utils/objects.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/kui/utils/pipe.py` & `kui-1.4.0/kui/utils/pipe.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/kui/utils/state.py` & `kui-1.4.0/kui/utils/state.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/kui/wsgi/__init__.py` & `kui-1.4.0/kui/wsgi/__init__.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/kui/wsgi/applications.py` & `kui-1.4.0/kui/wsgi/applications.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,18 @@
 from pathlib import PurePath
 from types import GeneratorType
 from typing import Any, Callable, Iterable, List, Mapping, NoReturn, Optional, Type
 
 from baize.datastructures import URL
 from baize.typing import Environ, StartResponse
 
+from ..cors import CORSConfig
 from ..routing import BaseRoute, MiddlewareType, NoMatchFound, SyncViewType
 from ..utils import ImmutableAttribute, State
+from .cors import allow_cors
 from .exceptions import ErrorHandlerType, ExceptionMiddleware, HTTPException
 from .requests import HttpRequest, request_var
 from .responses import (
     FileResponse,
     HttpResponse,
     JSONResponse,
     PlainTextResponse,
@@ -37,28 +39,35 @@
         self,
         *,
         templates: Optional[BaseTemplates] = None,
         routes: Iterable[BaseRoute] = [],
         http_middlewares: List[MiddlewareType[SyncViewType]] = [],
         socket_middlewares: List[MiddlewareType[SyncViewType]] = [],
         exception_handlers: Mapping[int | Type[BaseException], ErrorHandlerType] = {},
+        cors_config: Optional[CORSConfig] = None,
         factory_class: FactoryClass = FactoryClass(),
         response_converters: Mapping[type, Callable[..., HttpResponse]] = {},
     ) -> None:
         self.should_exit = False
 
         self.state = State()
         self.response_converter = create_response_converter(response_converters)
         self.should_exit = False
         self.factory_class = factory_class
         self.templates = templates
+
+        http_middlewares = [*http_middlewares]
+
         self.exception_middleware = ExceptionMiddleware(exception_handlers)
-        self.router = Router(
-            routes, [*http_middlewares, self.exception_middleware], socket_middlewares
-        )
+        http_middlewares.append(self.exception_middleware)
+
+        if cors_config is not None:
+            http_middlewares.append(allow_cors(**cors_config))
+
+        self.router = Router(routes, http_middlewares, socket_middlewares)
 
     def add_exception_handler(
         self, exc_class_or_status_code: int | Type[Exception], handler: ErrorHandlerType
     ) -> None:
         self.exception_middleware.add_exception_handler(
             exc_class_or_status_code, handler
         )
```

### Comparing `kui-1.3.7/kui/wsgi/cors.py` & `kui-1.4.0/kui/wsgi/cors.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/kui/wsgi/exceptions.py` & `kui-1.4.0/kui/wsgi/exceptions.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/kui/wsgi/openapi.py` & `kui-1.4.0/kui/wsgi/openapi.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/kui/wsgi/parameters.py` & `kui-1.4.0/kui/wsgi/parameters.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/kui/wsgi/requests.py` & `kui-1.4.0/kui/wsgi/requests.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/kui/wsgi/responses.py` & `kui-1.4.0/kui/wsgi/responses.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/kui/wsgi/routing.py` & `kui-1.4.0/kui/wsgi/routing.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/kui/wsgi/templates.py` & `kui-1.4.0/kui/wsgi/templates.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/kui/wsgi/views.py` & `kui-1.4.0/kui/wsgi/views.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/pyproject.toml` & `kui-1.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "kui"
-version = "1.3.7"
+version = "1.4.0"
 description = "An easy-to-use web framework."
 authors = [
     { name = "abersheeran", email = "me@abersheeran.com" },
 ]
 dependencies = [
     "baize<0.21.0,>=0.20.0",
     "pydantic<2.0,>=1.8",
@@ -27,16 +27,14 @@
 documentation = "https://kui.aber.sh"
 
 [project.optional-dependencies]
 cli = [
     "click<9.0,>=8.0",
 ]
 
-[project.scripts]
-
 [tool.pdm.scripts]
 lint-isort = "isort {args}"
 lint-black = "black {args}"
 check-isort = "isort --check --diff {args}"
 check-black = "black --check --diff {args}"
 check-flake8 = "flake8 --ignore W503,E203,E501,E731 {args}"
 check-mypy = "mypy {args}"
```

### Comparing `kui-1.3.7/tests/asgi/test_application.py` & `kui-1.4.0/tests/asgi/test_application.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/tests/asgi/test_parameters.py` & `kui-1.4.0/tests/asgi/test_parameters.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/tests/asgi/test_views.py` & `kui-1.4.0/tests/asgi/test_views.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/tests/openapi/test_application.py` & `kui-1.4.0/tests/openapi/test_application.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/tests/routing/extensions/test_multimethod.py` & `kui-1.4.0/tests/routing/extensions/test_multimethod.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/tests/routing/test_routes.py` & `kui-1.4.0/tests/routing/test_routes.py`

 * *Files 6% similar despite different names*

```diff
@@ -159,7 +159,22 @@
     app = Kui()
 
     @app.router.http("")
     async def homepage():
         return "homepage"
 
     assert app.router.search("http", "/")[0] == {}
+
+
+def test_routes_slice():
+    from kui.asgi import HttpRoute, Routes
+
+    async def endpoint():
+        pass
+
+    routes = Routes(
+        HttpRoute("/login", endpoint),
+        HttpRoute("/register", endpoint),
+    )
+
+    assert routes[:] == routes
+    assert routes[1:] == [routes[1]]
```

### Comparing `kui-1.3.7/tests/routing/test_tree.py` & `kui-1.4.0/tests/routing/test_tree.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/tests/test_responses.py` & `kui-1.4.0/tests/test_responses.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/tests/test_security.py` & `kui-1.4.0/tests/test_security.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/tests/utils/test_importer.py` & `kui-1.4.0/tests/utils/test_importer.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/tests/wsgi/test_cors.py` & `kui-1.4.0/tests/wsgi/test_cors.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from __future__ import annotations
 
+import re
+
 from httpx import Client
 
 from kui.wsgi import allow_cors
 
 
 def test_cors():
     cors_middleware = allow_cors()
@@ -19,9 +21,35 @@
 
     with Client(
         app=app, base_url="http://testServer", headers={"origin": "testserver"}
     ) as client:
         resp = client.get("/")
         assert resp.headers["access-control-allow-origin"] == "testserver"
 
+        resp = client.options("/")
+        assert resp.headers["access-control-allow-origin"] == "testserver"
+
+
+def test_cors_global():
+    from kui.wsgi import HttpRoute, Kui
+
+    app = Kui(
+        cors_config={
+            "allow_origins": [
+                re.compile("testserver"),
+            ]
+        }
+    )
+
+    def homepage():
+        return "homepage"
+
+    app.router <<= HttpRoute("/", homepage)
+
+    with Client(
+        app=app, base_url="http://testServer", headers={"origin": "testserver"}
+    ) as client:
+        resp = client.get("/")
+        assert resp.headers["access-control-allow-origin"] == "testserver"
+
         resp = client.options("/")
         assert resp.headers["access-control-allow-origin"] == "testserver"
```

### Comparing `kui-1.3.7/tests/wsgi/test_parameters.py` & `kui-1.4.0/tests/wsgi/test_parameters.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.7/PKG-INFO` & `kui-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kui
-Version: 1.3.7
+Version: 1.4.0
 Summary: An easy-to-use web framework.
 License: Apache-2.0
 Author-email: abersheeran <me@abersheeran.com>
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

