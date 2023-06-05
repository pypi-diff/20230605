# Comparing `tmp/pymodbus-3.3.0.tar.gz` & `tmp/pymodbus-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymodbus-3.3.0.tar", last modified: Fri Jun  2 13:19:46 2023, max compression
+gzip compressed data, was "pymodbus-3.3.1.tar", last modified: Mon Jun  5 18:50:48 2023, max compression
```

## Comparing `pymodbus-3.3.0.tar` & `pymodbus-3.3.1.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-02 13:19:46.515583 pymodbus-3.3.0/
--rw-r--r--   0 jan        (501) staff       (20)    26147 2023-06-02 12:16:59.000000 pymodbus-3.3.0/CHANGELOG.rst
--rw-r--r--   0 jan        (501) staff       (20)     1392 2023-06-02 12:16:19.000000 pymodbus-3.3.0/LICENSE
--rw-r--r--   0 jan        (501) staff       (20)       82 2023-06-02 12:16:19.000000 pymodbus-3.3.0/MANIFEST.in
--rw-r--r--   0 jan        (501) staff       (20)    18285 2023-06-02 13:19:46.515666 pymodbus-3.3.0/PKG-INFO
--rw-r--r--   0 jan        (501) staff       (20)    16791 2023-06-02 12:17:24.000000 pymodbus-3.3.0/README.rst
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-02 13:19:46.504496 pymodbus-3.3.0/pymodbus/
--rw-r--r--   0 jan        (501) staff       (20)      316 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)     9369 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/bit_read_message.py
--rw-r--r--   0 jan        (501) staff       (20)     9267 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/bit_write_message.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-02 13:19:46.506046 pymodbus-3.3.0/pymodbus/client/
--rw-r--r--   0 jan        (501) staff       (20)      602 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/client/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)    11857 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/client/base.py
--rw-r--r--   0 jan        (501) staff       (20)    20812 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/client/mixin.py
--rw-r--r--   0 jan        (501) staff       (20)     9904 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/client/serial.py
--rw-r--r--   0 jan        (501) staff       (20)     9645 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/client/tcp.py
--rw-r--r--   0 jan        (501) staff       (20)     6879 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/client/tls.py
--rw-r--r--   0 jan        (501) staff       (20)     5367 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/client/udp.py
--rw-r--r--   0 jan        (501) staff       (20)     8654 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/constants.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-02 13:19:46.506581 pymodbus-3.3.0/pymodbus/datastore/
--rw-r--r--   0 jan        (501) staff       (20)      491 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/datastore/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)     7312 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/datastore/context.py
--rw-r--r--   0 jan        (501) staff       (20)     4851 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/datastore/remote.py
--rwxr-xr-x   0 jan        (501) staff       (20)    29689 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/datastore/simulator.py
--rw-r--r--   0 jan        (501) staff       (20)    11410 2023-06-01 14:23:34.000000 pymodbus-3.3.0/pymodbus/datastore/store.py
--rw-r--r--   0 jan        (501) staff       (20)    22669 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/device.py
--rw-r--r--   0 jan        (501) staff       (20)    30049 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/diag_message.py
--rw-r--r--   0 jan        (501) staff       (20)     6481 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/events.py
--rw-r--r--   0 jan        (501) staff       (20)     3206 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/exceptions.py
--rw-r--r--   0 jan        (501) staff       (20)    13673 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/factory.py
--rw-r--r--   0 jan        (501) staff       (20)    14722 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/file_message.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-02 13:19:46.507251 pymodbus-3.3.0/pymodbus/framer/
--rw-r--r--   0 jan        (501) staff       (20)      509 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/framer/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)     7335 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/framer/ascii_framer.py
--rw-r--r--   0 jan        (501) staff       (20)     1822 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/framer/base.py
--rw-r--r--   0 jan        (501) staff       (20)     8043 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/framer/binary_framer.py
--rw-r--r--   0 jan        (501) staff       (20)    13507 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/framer/rtu_framer.py
--rw-r--r--   0 jan        (501) staff       (20)     7903 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/framer/socket_framer.py
--rw-r--r--   0 jan        (501) staff       (20)     6100 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/framer/tls_framer.py
--rw-r--r--   0 jan        (501) staff       (20)     3910 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/logging.py
--rw-r--r--   0 jan        (501) staff       (20)     7745 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/mei_message.py
--rw-r--r--   0 jan        (501) staff       (20)    15358 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/other_message.py
--rw-r--r--   0 jan        (501) staff       (20)    15651 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/payload.py
--rw-r--r--   0 jan        (501) staff       (20)     7786 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/pdu.py
--rw-r--r--   0 jan        (501) staff       (20)        0 2023-06-01 14:23:34.000000 pymodbus-3.3.0/pymodbus/py.typed
--rw-r--r--   0 jan        (501) staff       (20)    14021 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/register_read_message.py
--rw-r--r--   0 jan        (501) staff       (20)    12160 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/register_write_message.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-02 13:19:46.507358 pymodbus-3.3.0/pymodbus/repl/
--rw-r--r--   0 jan        (501) staff       (20)       28 2023-02-06 09:07:10.000000 pymodbus-3.3.0/pymodbus/repl/__init__.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-02 13:19:46.507846 pymodbus-3.3.0/pymodbus/repl/client/
--rw-r--r--   0 jan        (501) staff       (20)       19 2023-02-06 09:07:10.000000 pymodbus-3.3.0/pymodbus/repl/client/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)     5187 2023-06-01 14:23:34.000000 pymodbus-3.3.0/pymodbus/repl/client/completer.py
--rw-r--r--   0 jan        (501) staff       (20)     9526 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/repl/client/helper.py
--rw-r--r--   0 jan        (501) staff       (20)    13305 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/repl/client/main.py
--rw-r--r--   0 jan        (501) staff       (20)    23176 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/repl/client/mclient.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-02 13:19:46.508160 pymodbus-3.3.0/pymodbus/repl/server/
--rw-r--r--   0 jan        (501) staff       (20)       19 2023-02-06 09:07:10.000000 pymodbus-3.3.0/pymodbus/repl/server/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)     6912 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/repl/server/cli.py
--rw-r--r--   0 jan        (501) staff       (20)     6421 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/repl/server/main.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-02 13:19:46.508390 pymodbus-3.3.0/pymodbus/server/
--rw-r--r--   0 jan        (501) staff       (20)      975 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/server/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)    47435 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/server/async_io.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-02 13:19:46.508739 pymodbus-3.3.0/pymodbus/server/reactive/
--rw-r--r--   0 jan        (501) staff       (20)       18 2023-02-06 09:07:10.000000 pymodbus-3.3.0/pymodbus/server/reactive/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)     1977 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/server/reactive/default_config.py
--rw-r--r--   0 jan        (501) staff       (20)    18735 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/server/reactive/main.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-02 13:19:46.509297 pymodbus-3.3.0/pymodbus/server/simulator/
--rw-r--r--   0 jan        (501) staff       (20)       18 2023-02-06 09:15:57.000000 pymodbus-3.3.0/pymodbus/server/simulator/__init__.py
--rwxr-xr-x   0 jan        (501) staff       (20)      186 2023-02-06 09:15:57.000000 pymodbus-3.3.0/pymodbus/server/simulator/custom_actions.py
--rw-r--r--   0 jan        (501) staff       (20)    25063 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/server/simulator/http_server.py
--rwxr-xr-x   0 jan        (501) staff       (20)     4068 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/server/simulator/main.py
--rw-r--r--   0 jan        (501) staff       (20)     6788 2023-06-01 14:23:34.000000 pymodbus-3.3.0/pymodbus/server/simulator/setup.json
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-02 13:19:46.510828 pymodbus-3.3.0/pymodbus/server/simulator/web/
--rw-r--r--   0 jan        (501) staff       (20)    11369 2023-02-06 09:15:57.000000 pymodbus-3.3.0/pymodbus/server/simulator/web/apple120.png
--rw-r--r--   0 jan        (501) staff       (20)    15391 2023-02-06 09:15:57.000000 pymodbus-3.3.0/pymodbus/server/simulator/web/apple152.png
--rw-r--r--   0 jan        (501) staff       (20)     4817 2023-02-06 09:15:57.000000 pymodbus-3.3.0/pymodbus/server/simulator/web/apple60.png
--rw-r--r--   0 jan        (501) staff       (20)     6344 2023-02-06 09:15:57.000000 pymodbus-3.3.0/pymodbus/server/simulator/web/apple76.png
--rw-r--r--   0 jan        (501) staff       (20)    12014 2023-02-06 09:15:57.000000 pymodbus-3.3.0/pymodbus/server/simulator/web/favicon.ico
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-02 13:19:46.511585 pymodbus-3.3.0/pymodbus/server/simulator/web/generator/
--rw-r--r--   0 jan        (501) staff       (20)     4314 2023-06-01 14:23:34.000000 pymodbus-3.3.0/pymodbus/server/simulator/web/generator/calls
--rw-r--r--   0 jan        (501) staff       (20)     1132 2023-06-01 14:23:34.000000 pymodbus-3.3.0/pymodbus/server/simulator/web/generator/log
--rw-r--r--   0 jan        (501) staff       (20)     5850 2023-02-06 09:15:57.000000 pymodbus-3.3.0/pymodbus/server/simulator/web/generator/pymodbus_icon_original.png
--rw-r--r--   0 jan        (501) staff       (20)     2710 2023-06-01 14:23:34.000000 pymodbus-3.3.0/pymodbus/server/simulator/web/generator/registers
--rw-r--r--   0 jan        (501) staff       (20)      893 2023-06-01 14:23:34.000000 pymodbus-3.3.0/pymodbus/server/simulator/web/generator/server
--rw-r--r--   0 jan        (501) staff       (20)     1944 2023-06-01 14:23:34.000000 pymodbus-3.3.0/pymodbus/server/simulator/web/index.html
--rw-r--r--   0 jan        (501) staff       (20)      919 2023-06-01 14:23:34.000000 pymodbus-3.3.0/pymodbus/server/simulator/web/pymodbus.css
--rw-r--r--   0 jan        (501) staff       (20)      710 2023-06-01 14:23:34.000000 pymodbus-3.3.0/pymodbus/server/simulator/web/welcome.html
--rw-r--r--   0 jan        (501) staff       (20)    23769 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/transaction.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-02 13:19:46.511809 pymodbus-3.3.0/pymodbus/transport/
--rw-r--r--   0 jan        (501) staff       (20)      109 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/transport/__init__.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-02 13:19:46.511902 pymodbus-3.3.0/pymodbus/transport/serial_asyncio/
--rw-r--r--   0 jan        (501) staff       (20)    19336 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/transport/serial_asyncio/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)    14300 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/transport/transport.py
--rw-r--r--   0 jan        (501) staff       (20)     7797 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/utilities.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-02 13:19:46.505208 pymodbus-3.3.0/pymodbus.egg-info/
--rw-r--r--   0 jan        (501) staff       (20)    18285 2023-06-02 13:19:46.000000 pymodbus-3.3.0/pymodbus.egg-info/PKG-INFO
--rw-r--r--   0 jan        (501) staff       (20)     3509 2023-06-02 13:19:46.000000 pymodbus-3.3.0/pymodbus.egg-info/SOURCES.txt
--rw-r--r--   0 jan        (501) staff       (20)        1 2023-06-02 13:19:46.000000 pymodbus-3.3.0/pymodbus.egg-info/dependency_links.txt
--rw-r--r--   0 jan        (501) staff       (20)      173 2023-06-02 13:19:46.000000 pymodbus-3.3.0/pymodbus.egg-info/entry_points.txt
--rw-r--r--   0 jan        (501) staff       (20)      481 2023-06-02 13:19:46.000000 pymodbus-3.3.0/pymodbus.egg-info/requires.txt
--rw-r--r--   0 jan        (501) staff       (20)        9 2023-06-02 13:19:46.000000 pymodbus-3.3.0/pymodbus.egg-info/top_level.txt
--rw-r--r--   0 jan        (501) staff       (20)        1 2022-11-08 12:27:57.000000 pymodbus-3.3.0/pymodbus.egg-info/zip-safe
--rw-r--r--   0 jan        (501) staff       (20)     1897 2023-06-02 12:16:19.000000 pymodbus-3.3.0/requirements.txt
--rw-r--r--   0 jan        (501) staff       (20)     4391 2023-06-02 13:19:46.516276 pymodbus-3.3.0/setup.cfg
--rw-r--r--   0 jan        (501) staff       (20)     1105 2023-06-02 12:17:58.000000 pymodbus-3.3.0/setup.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-02 13:19:46.515489 pymodbus-3.3.0/test/
--rw-r--r--   0 jan        (501) staff       (20)     3738 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_all_messages.py
--rw-r--r--   0 jan        (501) staff       (20)     4594 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_bit_read_messages.py
--rw-r--r--   0 jan        (501) staff       (20)     5244 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_bit_write_messages.py
--rwxr-xr-x   0 jan        (501) staff       (20)    19470 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_client.py
--rw-r--r--   0 jan        (501) staff       (20)     1315 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_client_faulty_response.py
--rwxr-xr-x   0 jan        (501) staff       (20)    16833 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_client_sync.py
--rw-r--r--   0 jan        (501) staff       (20)    13200 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_device.py
--rw-r--r--   0 jan        (501) staff       (20)     8330 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_diag_messages.py
--rw-r--r--   0 jan        (501) staff       (20)     2359 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_events.py
--rwxr-xr-x   0 jan        (501) staff       (20)     3503 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_example_client_server.py
--rwxr-xr-x   0 jan        (501) staff       (20)     7225 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_examples.py
--rw-r--r--   0 jan        (501) staff       (20)      771 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_exceptions.py
--rw-r--r--   0 jan        (501) staff       (20)     8499 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_factory.py
--rw-r--r--   0 jan        (501) staff       (20)    10180 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_file_message.py
--rw-r--r--   0 jan        (501) staff       (20)    10928 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_framers.py
--rw-r--r--   0 jan        (501) staff       (20)     1238 2023-06-02 12:18:32.000000 pymodbus-3.3.0/test/test_logging.py
--rw-r--r--   0 jan        (501) staff       (20)     6297 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_mei_messages.py
--rw-r--r--   0 jan        (501) staff       (20)     5687 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_other_messages.py
--rw-r--r--   0 jan        (501) staff       (20)     8771 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_payload.py
--rw-r--r--   0 jan        (501) staff       (20)     2814 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_pdu.py
--rw-r--r--   0 jan        (501) staff       (20)     7450 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_register_read_messages.py
--rw-r--r--   0 jan        (501) staff       (20)     7658 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_register_write_messages.py
--rw-r--r--   0 jan        (501) staff       (20)     2448 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_remote_datastore.py
--rwxr-xr-x   0 jan        (501) staff       (20)     1463 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_repl_client.py
--rwxr-xr-x   0 jan        (501) staff       (20)    17385 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_server_asyncio.py
--rw-r--r--   0 jan        (501) staff       (20)     3546 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_server_context.py
--rw-r--r--   0 jan        (501) staff       (20)     8192 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_server_multidrop.py
--rwxr-xr-x   0 jan        (501) staff       (20)    10893 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_server_task.py
--rw-r--r--   0 jan        (501) staff       (20)    18298 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_simulator.py
--rw-r--r--   0 jan        (501) staff       (20)      649 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_sparse_datastore.py
--rwxr-xr-x   0 jan        (501) staff       (20)    30391 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_transaction.py
--rwxr-xr-x   0 jan        (501) staff       (20)     1974 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_unix_socket.py
--rw-r--r--   0 jan        (501) staff       (20)     3107 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_utilities.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-05 18:50:48.994661 pymodbus-3.3.1/
+-rw-r--r--   0 jan        (501) staff       (20)    26536 2023-06-05 18:50:02.000000 pymodbus-3.3.1/CHANGELOG.rst
+-rw-r--r--   0 jan        (501) staff       (20)     1392 2023-06-04 13:17:31.000000 pymodbus-3.3.1/LICENSE
+-rw-r--r--   0 jan        (501) staff       (20)       82 2023-06-04 13:17:31.000000 pymodbus-3.3.1/MANIFEST.in
+-rw-r--r--   0 jan        (501) staff       (20)    18285 2023-06-05 18:50:48.994750 pymodbus-3.3.1/PKG-INFO
+-rw-r--r--   0 jan        (501) staff       (20)    16791 2023-06-05 18:50:02.000000 pymodbus-3.3.1/README.rst
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-05 18:50:48.980409 pymodbus-3.3.1/pymodbus/
+-rw-r--r--   0 jan        (501) staff       (20)      316 2023-06-05 18:50:02.000000 pymodbus-3.3.1/pymodbus/__init__.py
+-rw-r--r--   0 jan        (501) staff       (20)     9369 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/bit_read_message.py
+-rw-r--r--   0 jan        (501) staff       (20)     9267 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/bit_write_message.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-05 18:50:48.982099 pymodbus-3.3.1/pymodbus/client/
+-rw-r--r--   0 jan        (501) staff       (20)      602 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/client/__init__.py
+-rw-r--r--   0 jan        (501) staff       (20)    11845 2023-06-05 18:30:16.000000 pymodbus-3.3.1/pymodbus/client/base.py
+-rw-r--r--   0 jan        (501) staff       (20)    20812 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/client/mixin.py
+-rw-r--r--   0 jan        (501) staff       (20)     9904 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/client/serial.py
+-rw-r--r--   0 jan        (501) staff       (20)     9645 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/client/tcp.py
+-rw-r--r--   0 jan        (501) staff       (20)     6879 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/client/tls.py
+-rw-r--r--   0 jan        (501) staff       (20)     5367 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/client/udp.py
+-rw-r--r--   0 jan        (501) staff       (20)     8654 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/constants.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-05 18:50:48.982755 pymodbus-3.3.1/pymodbus/datastore/
+-rw-r--r--   0 jan        (501) staff       (20)      491 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/datastore/__init__.py
+-rw-r--r--   0 jan        (501) staff       (20)     7312 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/datastore/context.py
+-rw-r--r--   0 jan        (501) staff       (20)     4851 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/datastore/remote.py
+-rwxr-xr-x   0 jan        (501) staff       (20)    29689 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/datastore/simulator.py
+-rw-r--r--   0 jan        (501) staff       (20)    11410 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/datastore/store.py
+-rw-r--r--   0 jan        (501) staff       (20)    22669 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/device.py
+-rw-r--r--   0 jan        (501) staff       (20)    30049 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/diag_message.py
+-rw-r--r--   0 jan        (501) staff       (20)     6481 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/events.py
+-rw-r--r--   0 jan        (501) staff       (20)     3206 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/exceptions.py
+-rw-r--r--   0 jan        (501) staff       (20)    13673 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/factory.py
+-rw-r--r--   0 jan        (501) staff       (20)    14722 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/file_message.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-05 18:50:48.983717 pymodbus-3.3.1/pymodbus/framer/
+-rw-r--r--   0 jan        (501) staff       (20)      509 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/framer/__init__.py
+-rw-r--r--   0 jan        (501) staff       (20)     7335 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/framer/ascii_framer.py
+-rw-r--r--   0 jan        (501) staff       (20)     1822 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/framer/base.py
+-rw-r--r--   0 jan        (501) staff       (20)     8043 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/framer/binary_framer.py
+-rw-r--r--   0 jan        (501) staff       (20)    13507 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/framer/rtu_framer.py
+-rw-r--r--   0 jan        (501) staff       (20)     7903 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/framer/socket_framer.py
+-rw-r--r--   0 jan        (501) staff       (20)     6100 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/framer/tls_framer.py
+-rw-r--r--   0 jan        (501) staff       (20)     3910 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/logging.py
+-rw-r--r--   0 jan        (501) staff       (20)     7745 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/mei_message.py
+-rw-r--r--   0 jan        (501) staff       (20)    15358 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/other_message.py
+-rw-r--r--   0 jan        (501) staff       (20)    15651 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/payload.py
+-rw-r--r--   0 jan        (501) staff       (20)     7786 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/pdu.py
+-rw-r--r--   0 jan        (501) staff       (20)        0 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/py.typed
+-rw-r--r--   0 jan        (501) staff       (20)    14021 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/register_read_message.py
+-rw-r--r--   0 jan        (501) staff       (20)    12160 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/register_write_message.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-05 18:50:48.983852 pymodbus-3.3.1/pymodbus/repl/
+-rw-r--r--   0 jan        (501) staff       (20)       28 2023-02-06 09:07:10.000000 pymodbus-3.3.1/pymodbus/repl/__init__.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-05 18:50:48.984692 pymodbus-3.3.1/pymodbus/repl/client/
+-rw-r--r--   0 jan        (501) staff       (20)       19 2023-02-06 09:07:10.000000 pymodbus-3.3.1/pymodbus/repl/client/__init__.py
+-rw-r--r--   0 jan        (501) staff       (20)     5187 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/repl/client/completer.py
+-rw-r--r--   0 jan        (501) staff       (20)     9526 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/repl/client/helper.py
+-rw-r--r--   0 jan        (501) staff       (20)    13305 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/repl/client/main.py
+-rw-r--r--   0 jan        (501) staff       (20)    23176 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/repl/client/mclient.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-05 18:50:48.985113 pymodbus-3.3.1/pymodbus/repl/server/
+-rw-r--r--   0 jan        (501) staff       (20)       19 2023-02-06 09:07:10.000000 pymodbus-3.3.1/pymodbus/repl/server/__init__.py
+-rw-r--r--   0 jan        (501) staff       (20)     6912 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/repl/server/cli.py
+-rw-r--r--   0 jan        (501) staff       (20)     6421 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/repl/server/main.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-05 18:50:48.985391 pymodbus-3.3.1/pymodbus/server/
+-rw-r--r--   0 jan        (501) staff       (20)      975 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/server/__init__.py
+-rw-r--r--   0 jan        (501) staff       (20)    47906 2023-06-05 18:30:16.000000 pymodbus-3.3.1/pymodbus/server/async_io.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-05 18:50:48.986152 pymodbus-3.3.1/pymodbus/server/reactive/
+-rw-r--r--   0 jan        (501) staff       (20)       18 2023-02-06 09:07:10.000000 pymodbus-3.3.1/pymodbus/server/reactive/__init__.py
+-rw-r--r--   0 jan        (501) staff       (20)     1977 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/server/reactive/default_config.py
+-rw-r--r--   0 jan        (501) staff       (20)    18735 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/server/reactive/main.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-05 18:50:48.987063 pymodbus-3.3.1/pymodbus/server/simulator/
+-rw-r--r--   0 jan        (501) staff       (20)       18 2023-02-06 09:15:57.000000 pymodbus-3.3.1/pymodbus/server/simulator/__init__.py
+-rwxr-xr-x   0 jan        (501) staff       (20)      186 2023-02-06 09:15:57.000000 pymodbus-3.3.1/pymodbus/server/simulator/custom_actions.py
+-rw-r--r--   0 jan        (501) staff       (20)    25063 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/server/simulator/http_server.py
+-rwxr-xr-x   0 jan        (501) staff       (20)     4068 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/server/simulator/main.py
+-rw-r--r--   0 jan        (501) staff       (20)     6788 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/server/simulator/setup.json
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-05 18:50:48.988409 pymodbus-3.3.1/pymodbus/server/simulator/web/
+-rw-r--r--   0 jan        (501) staff       (20)    11369 2023-02-06 09:15:57.000000 pymodbus-3.3.1/pymodbus/server/simulator/web/apple120.png
+-rw-r--r--   0 jan        (501) staff       (20)    15391 2023-02-06 09:15:57.000000 pymodbus-3.3.1/pymodbus/server/simulator/web/apple152.png
+-rw-r--r--   0 jan        (501) staff       (20)     4817 2023-02-06 09:15:57.000000 pymodbus-3.3.1/pymodbus/server/simulator/web/apple60.png
+-rw-r--r--   0 jan        (501) staff       (20)     6344 2023-02-06 09:15:57.000000 pymodbus-3.3.1/pymodbus/server/simulator/web/apple76.png
+-rw-r--r--   0 jan        (501) staff       (20)    12014 2023-02-06 09:15:57.000000 pymodbus-3.3.1/pymodbus/server/simulator/web/favicon.ico
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-05 18:50:48.989202 pymodbus-3.3.1/pymodbus/server/simulator/web/generator/
+-rw-r--r--   0 jan        (501) staff       (20)     4314 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/server/simulator/web/generator/calls
+-rw-r--r--   0 jan        (501) staff       (20)     1132 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/server/simulator/web/generator/log
+-rw-r--r--   0 jan        (501) staff       (20)     5850 2023-02-06 09:15:57.000000 pymodbus-3.3.1/pymodbus/server/simulator/web/generator/pymodbus_icon_original.png
+-rw-r--r--   0 jan        (501) staff       (20)     2710 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/server/simulator/web/generator/registers
+-rw-r--r--   0 jan        (501) staff       (20)      893 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/server/simulator/web/generator/server
+-rw-r--r--   0 jan        (501) staff       (20)     1944 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/server/simulator/web/index.html
+-rw-r--r--   0 jan        (501) staff       (20)      919 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/server/simulator/web/pymodbus.css
+-rw-r--r--   0 jan        (501) staff       (20)      710 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/server/simulator/web/welcome.html
+-rw-r--r--   0 jan        (501) staff       (20)    23769 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/transaction.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-05 18:50:48.989458 pymodbus-3.3.1/pymodbus/transport/
+-rw-r--r--   0 jan        (501) staff       (20)       17 2023-06-05 18:30:16.000000 pymodbus-3.3.1/pymodbus/transport/__init__.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-05 18:50:48.989576 pymodbus-3.3.1/pymodbus/transport/serial_asyncio/
+-rw-r--r--   0 jan        (501) staff       (20)    19336 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/transport/serial_asyncio/__init__.py
+-rw-r--r--   0 jan        (501) staff       (20)    14940 2023-06-05 18:50:02.000000 pymodbus-3.3.1/pymodbus/transport/transport.py
+-rw-r--r--   0 jan        (501) staff       (20)     7797 2023-06-04 13:17:31.000000 pymodbus-3.3.1/pymodbus/utilities.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-05 18:50:48.981166 pymodbus-3.3.1/pymodbus.egg-info/
+-rw-r--r--   0 jan        (501) staff       (20)    18285 2023-06-05 18:50:48.000000 pymodbus-3.3.1/pymodbus.egg-info/PKG-INFO
+-rw-r--r--   0 jan        (501) staff       (20)     3509 2023-06-05 18:50:48.000000 pymodbus-3.3.1/pymodbus.egg-info/SOURCES.txt
+-rw-r--r--   0 jan        (501) staff       (20)        1 2023-06-05 18:50:48.000000 pymodbus-3.3.1/pymodbus.egg-info/dependency_links.txt
+-rw-r--r--   0 jan        (501) staff       (20)      173 2023-06-05 18:50:48.000000 pymodbus-3.3.1/pymodbus.egg-info/entry_points.txt
+-rw-r--r--   0 jan        (501) staff       (20)      481 2023-06-05 18:50:48.000000 pymodbus-3.3.1/pymodbus.egg-info/requires.txt
+-rw-r--r--   0 jan        (501) staff       (20)        9 2023-06-05 18:50:48.000000 pymodbus-3.3.1/pymodbus.egg-info/top_level.txt
+-rw-r--r--   0 jan        (501) staff       (20)        1 2022-11-08 12:27:57.000000 pymodbus-3.3.1/pymodbus.egg-info/zip-safe
+-rw-r--r--   0 jan        (501) staff       (20)     1897 2023-06-04 13:17:31.000000 pymodbus-3.3.1/requirements.txt
+-rw-r--r--   0 jan        (501) staff       (20)     4391 2023-06-05 18:50:48.995351 pymodbus-3.3.1/setup.cfg
+-rw-r--r--   0 jan        (501) staff       (20)     1105 2023-06-04 13:17:31.000000 pymodbus-3.3.1/setup.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-05 18:50:48.994544 pymodbus-3.3.1/test/
+-rw-r--r--   0 jan        (501) staff       (20)     3738 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_all_messages.py
+-rw-r--r--   0 jan        (501) staff       (20)     4594 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_bit_read_messages.py
+-rw-r--r--   0 jan        (501) staff       (20)     5244 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_bit_write_messages.py
+-rwxr-xr-x   0 jan        (501) staff       (20)    19470 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_client.py
+-rw-r--r--   0 jan        (501) staff       (20)     1315 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_client_faulty_response.py
+-rwxr-xr-x   0 jan        (501) staff       (20)    16833 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_client_sync.py
+-rw-r--r--   0 jan        (501) staff       (20)    13200 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_device.py
+-rw-r--r--   0 jan        (501) staff       (20)     8330 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_diag_messages.py
+-rw-r--r--   0 jan        (501) staff       (20)     2359 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_events.py
+-rwxr-xr-x   0 jan        (501) staff       (20)     3503 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_example_client_server.py
+-rwxr-xr-x   0 jan        (501) staff       (20)     7225 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_examples.py
+-rw-r--r--   0 jan        (501) staff       (20)      771 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_exceptions.py
+-rw-r--r--   0 jan        (501) staff       (20)     8499 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_factory.py
+-rw-r--r--   0 jan        (501) staff       (20)    10180 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_file_message.py
+-rw-r--r--   0 jan        (501) staff       (20)    10928 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_framers.py
+-rw-r--r--   0 jan        (501) staff       (20)     1238 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_logging.py
+-rw-r--r--   0 jan        (501) staff       (20)     6297 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_mei_messages.py
+-rw-r--r--   0 jan        (501) staff       (20)     5687 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_other_messages.py
+-rw-r--r--   0 jan        (501) staff       (20)     8771 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_payload.py
+-rw-r--r--   0 jan        (501) staff       (20)     2814 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_pdu.py
+-rw-r--r--   0 jan        (501) staff       (20)     7450 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_register_read_messages.py
+-rw-r--r--   0 jan        (501) staff       (20)     7658 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_register_write_messages.py
+-rw-r--r--   0 jan        (501) staff       (20)     2448 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_remote_datastore.py
+-rwxr-xr-x   0 jan        (501) staff       (20)     1463 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_repl_client.py
+-rwxr-xr-x   0 jan        (501) staff       (20)    17385 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_server_asyncio.py
+-rw-r--r--   0 jan        (501) staff       (20)     3546 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_server_context.py
+-rw-r--r--   0 jan        (501) staff       (20)     8192 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_server_multidrop.py
+-rwxr-xr-x   0 jan        (501) staff       (20)    10930 2023-06-05 18:30:16.000000 pymodbus-3.3.1/test/test_server_task.py
+-rw-r--r--   0 jan        (501) staff       (20)    18298 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_simulator.py
+-rw-r--r--   0 jan        (501) staff       (20)      649 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_sparse_datastore.py
+-rwxr-xr-x   0 jan        (501) staff       (20)    30391 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_transaction.py
+-rwxr-xr-x   0 jan        (501) staff       (20)     1974 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_unix_socket.py
+-rw-r--r--   0 jan        (501) staff       (20)     3107 2023-06-04 13:17:31.000000 pymodbus-3.3.1/test/test_utilities.py
```

### Comparing `pymodbus-3.3.0/CHANGELOG.rst` & `pymodbus-3.3.1/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+version 3.3.1
+----------------------------------------------------------
+* transport fixes and 100% test coverage. (#1580)
+* Delay self.loop until connect(). (#1579)
+* Added mechanism to determine if server did not start cleanly (#1539)
+* Proof transport reconnect works. (#1577)
+* Fix non-shared block doc in config.rst. (#1573)
+
+Thanks to:
+  Hayden Roche
+  jan iversen
+  Philip Couling
+
 version 3.3.0
 ----------------------------------------------------------
 * Stabilize windows tests. (#1567)
 * Bump mypy 1.3.0 (#1568)
 * Transport integrated in async clients. (#1541)
 * Client async corrections (due to 3.1.2) (#1565)
 * Server_async[udp], solve 3.1.1 problem. (#1564)
```

### Comparing `pymodbus-3.3.0/LICENSE` & `pymodbus-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/PKG-INFO` & `pymodbus-3.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymodbus
-Version: 3.3.0
+Version: 3.3.1
 Summary: A fully featured modbus protocol stack in python
 Home-page: https://github.com/pymodbus-dev/pymodbus/
 Author: "Galen Collins, Jan Iversen"
 Maintainer: "dhoomakethu, janiversen"
 License: BSD-3-Clause
 Project-URL: Source Code, https://github.com/pymodbus-dev/pymodbus
 Project-URL: Bug Reports, https://github.com/pymodbus-dev/pymodbus/issues
@@ -57,15 +57,15 @@
 
 ------------------------------------------------------------
 Supported versions
 ------------------------------------------------------------
 
 Version `2.5.3 <https://github.com/pymodbus-dev/pymodbus/releases/tag/v2.5.3>`_ is the last 2.x release (Supports python >= 2.7, no longer supported).
 
-Version `3.3.0 <https://github.com/pymodbus-dev/pymodbus/releases/tag/v3.3.0>`_ is the current release (Supports Python >= 3.8).
+Version `3.3.0 <https://github.com/pymodbus-dev/pymodbus/releases/tag/v3.3.1>`_ is the current release (Supports Python >= 3.8).
 
 .. important::
    All API changes after 3.0.0 are documented in `API_changes.rst <https://github.com/pymodbus-dev/pymodbus/blob/dev/API_changes.rst>`_
 
 
 ------------------------------------------------------------
 Summary
```

### Comparing `pymodbus-3.3.0/README.rst` & `pymodbus-3.3.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 ------------------------------------------------------------
 Supported versions
 ------------------------------------------------------------
 
 Version `2.5.3 <https://github.com/pymodbus-dev/pymodbus/releases/tag/v2.5.3>`_ is the last 2.x release (Supports python >= 2.7, no longer supported).
 
-Version `3.3.0 <https://github.com/pymodbus-dev/pymodbus/releases/tag/v3.3.0>`_ is the current release (Supports Python >= 3.8).
+Version `3.3.0 <https://github.com/pymodbus-dev/pymodbus/releases/tag/v3.3.1>`_ is the current release (Supports Python >= 3.8).
 
 .. important::
    All API changes after 3.0.0 are documented in `API_changes.rst <https://github.com/pymodbus-dev/pymodbus/blob/dev/API_changes.rst>`_
 
 
 ------------------------------------------------------------
 Summary
```

### Comparing `pymodbus-3.3.0/pymodbus/bit_read_message.py` & `pymodbus-3.3.1/pymodbus/bit_read_message.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/bit_write_message.py` & `pymodbus-3.3.1/pymodbus/bit_write_message.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/client/__init__.py` & `pymodbus-3.3.1/pymodbus/client/__init__.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/client/base.py` & `pymodbus-3.3.1/pymodbus/client/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 from pymodbus.constants import Defaults
 from pymodbus.exceptions import ConnectionException
 from pymodbus.factory import ClientDecoder
 from pymodbus.framer import ModbusFramer
 from pymodbus.logging import Log
 from pymodbus.pdu import ModbusRequest, ModbusResponse
 from pymodbus.transaction import DictTransactionManager
-from pymodbus.transport import BaseTransport
+from pymodbus.transport.transport import Transport
 from pymodbus.utilities import ModbusTransactionState
 
 
-class ModbusBaseClient(ModbusClientMixin, BaseTransport):
+class ModbusBaseClient(ModbusClientMixin, Transport):
     """**ModbusBaseClient**
 
     **Parameters common to all clients**:
 
     :param framer: (optional) Modbus Framer class.
     :param timeout: (optional) Timeout for a request, in seconds.
     :param retries: (optional) Max number of retries per request.
@@ -90,20 +90,20 @@
         broadcast_enable: bool = Defaults.BroadcastEnable,
         reconnect_delay: int = 0.1,
         reconnect_delay_max: int = 300,
         on_reconnect_callback: Callable[[], None] | None = None,
         **kwargs: Any,
     ) -> None:
         """Initialize a client instance."""
-        BaseTransport.__init__(
+        Transport.__init__(
             self,
             "comm",
-            (reconnect_delay * 1000, reconnect_delay_max * 1000),
+            reconnect_delay * 1000,
+            reconnect_delay_max * 1000,
             timeout * 1000,
-            framer,
             lambda: None,
             self.cb_base_connection_lost,
             self.cb_base_handle_data,
         )
         self.framer = framer
         self.params = self._params()
         self.params.framer = framer
```

### Comparing `pymodbus-3.3.0/pymodbus/client/mixin.py` & `pymodbus-3.3.1/pymodbus/client/mixin.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/client/serial.py` & `pymodbus-3.3.1/pymodbus/client/serial.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/client/tcp.py` & `pymodbus-3.3.1/pymodbus/client/tcp.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/client/tls.py` & `pymodbus-3.3.1/pymodbus/client/tls.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/client/udp.py` & `pymodbus-3.3.1/pymodbus/client/udp.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/constants.py` & `pymodbus-3.3.1/pymodbus/constants.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/datastore/context.py` & `pymodbus-3.3.1/pymodbus/datastore/context.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/datastore/remote.py` & `pymodbus-3.3.1/pymodbus/datastore/remote.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/datastore/simulator.py` & `pymodbus-3.3.1/pymodbus/datastore/simulator.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/datastore/store.py` & `pymodbus-3.3.1/pymodbus/datastore/store.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/device.py` & `pymodbus-3.3.1/pymodbus/device.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/diag_message.py` & `pymodbus-3.3.1/pymodbus/diag_message.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/events.py` & `pymodbus-3.3.1/pymodbus/events.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/exceptions.py` & `pymodbus-3.3.1/pymodbus/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/factory.py` & `pymodbus-3.3.1/pymodbus/factory.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/file_message.py` & `pymodbus-3.3.1/pymodbus/file_message.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/framer/ascii_framer.py` & `pymodbus-3.3.1/pymodbus/framer/ascii_framer.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/framer/base.py` & `pymodbus-3.3.1/pymodbus/framer/base.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/framer/binary_framer.py` & `pymodbus-3.3.1/pymodbus/framer/binary_framer.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/framer/rtu_framer.py` & `pymodbus-3.3.1/pymodbus/framer/rtu_framer.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/framer/socket_framer.py` & `pymodbus-3.3.1/pymodbus/framer/socket_framer.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/framer/tls_framer.py` & `pymodbus-3.3.1/pymodbus/framer/tls_framer.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/logging.py` & `pymodbus-3.3.1/pymodbus/logging.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/mei_message.py` & `pymodbus-3.3.1/pymodbus/mei_message.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/other_message.py` & `pymodbus-3.3.1/pymodbus/other_message.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/payload.py` & `pymodbus-3.3.1/pymodbus/payload.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/pdu.py` & `pymodbus-3.3.1/pymodbus/pdu.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/register_read_message.py` & `pymodbus-3.3.1/pymodbus/register_read_message.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/register_write_message.py` & `pymodbus-3.3.1/pymodbus/register_write_message.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/repl/client/completer.py` & `pymodbus-3.3.1/pymodbus/repl/client/completer.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/repl/client/helper.py` & `pymodbus-3.3.1/pymodbus/repl/client/helper.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/repl/client/main.py` & `pymodbus-3.3.1/pymodbus/repl/client/main.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/repl/client/mclient.py` & `pymodbus-3.3.1/pymodbus/repl/client/mclient.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/repl/server/cli.py` & `pymodbus-3.3.1/pymodbus/repl/server/cli.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/repl/server/main.py` & `pymodbus-3.3.1/pymodbus/repl/server/main.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/server/__init__.py` & `pymodbus-3.3.1/pymodbus/server/__init__.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/server/async_io.py` & `pymodbus-3.3.1/pymodbus/server/async_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -530,14 +530,15 @@
         self.broadcast_enable = kwargs.get("broadcast_enable", Defaults.BroadcastEnable)
         self.response_manipulator = kwargs.get("response_manipulator", None)
         if isinstance(identity, ModbusDeviceIdentification):
             self.control.Identity.update(identity)
 
         # asyncio future that will be done once server has started
         self.serving = asyncio.Future()
+        self.serving_done = asyncio.Future()
         # constructors cannot be declared async, so we have to
         # defer the initialization of the server
         self.server = None
         self.request_tracer = None
         self.factory_parms = {}
 
     async def serve_forever(self):
@@ -548,21 +549,23 @@
                     lambda: self.handler(self),
                     self.path,
                 )
                 self.serving.set_result(True)
                 Log.info("Server(Unix) listening.")
                 await self.server.serve_forever()
             except asyncio.exceptions.CancelledError:
+                self.serving_done.set_result(True)
                 raise
             except Exception as exc:  # pylint: disable=broad-except
                 Log.error("Server unexpected exception {}", exc)
         else:
             raise RuntimeError(
                 "Can't call serve_forever on an already running server object"
             )
+        self.serving_done.set_result(True)
         Log.info("Server graceful shutdown.")
 
     async def shutdown(self):
         """Shutdown server."""
         await self.server_close()
 
     async def server_close(self):
@@ -637,14 +640,15 @@
         self.response_manipulator = kwargs.get("response_manipulator", None)
         self.request_tracer = kwargs.get("request_tracer", None)
         if isinstance(identity, ModbusDeviceIdentification):
             self.control.Identity.update(identity)
 
         # asyncio future that will be done once server has started
         self.serving = asyncio.Future()
+        self.serving_done = asyncio.Future()
         # constructors cannot be declared async, so we have to
         # defer the initialization of the server
         self.server = None
         self.factory_parms = {
             "reuse_address": allow_reuse_address,
             "backlog": backlog,
             "start_serving": True,
@@ -659,21 +663,23 @@
                 **self.factory_parms,
             )
             self.serving.set_result(True)
             Log.info("Server(TCP) listening.")
             try:
                 await self.server.serve_forever()
             except asyncio.exceptions.CancelledError:
+                self.serving_done.set_result(False)
                 raise
             except Exception as exc:  # pylint: disable=broad-except
                 Log.error("Server unexpected exception {}", exc)
         else:
             raise RuntimeError(
                 "Can't call serve_forever on an already running server object"
             )
+        self.serving_done.set_result(True)
         Log.info("Server graceful shutdown.")
 
     async def shutdown(self):
         """Shutdown server."""
         await self.server_close()
 
     async def server_close(self):
@@ -817,14 +823,15 @@
 
         self.protocol = None
         self.endpoint = None
         self.on_connection_terminated = None
         self.stop_serving = self.loop.create_future()
         # asyncio future that will be done once server has started
         self.serving = asyncio.Future()
+        self.serving_done = asyncio.Future()
         self.factory_parms = {
             "local_addr": self.address,
             "allow_broadcast": True,
         }
         self.request_tracer = None
 
     async def serve_forever(self):
@@ -832,25 +839,28 @@
         if self.protocol is None:
             try:
                 self.protocol, self.endpoint = await self.loop.create_datagram_endpoint(
                     lambda: self.handler(self),
                     **self.factory_parms,
                 )
             except asyncio.exceptions.CancelledError:
+                self.serving_done.set_result(False)
                 raise
             except Exception as exc:
                 Log.error("Server unexpected exception {}", exc)
+                self.serving_done.set_result(False)
                 raise RuntimeError(exc) from exc
             Log.info("Server(UDP) listening.")
             self.serving.set_result(True)
             await self.stop_serving
         else:
             raise RuntimeError(
                 "Can't call serve_forever on an already running server object"
             )
+        self.serving_done.set_result(True)
 
     async def shutdown(self):
         """Shutdown server."""
         await self.server_close()
 
     async def server_close(self):
         """Close server."""
```

### Comparing `pymodbus-3.3.0/pymodbus/server/reactive/default_config.py` & `pymodbus-3.3.1/pymodbus/server/reactive/default_config.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/server/reactive/main.py` & `pymodbus-3.3.1/pymodbus/server/reactive/main.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/server/simulator/http_server.py` & `pymodbus-3.3.1/pymodbus/server/simulator/http_server.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/server/simulator/main.py` & `pymodbus-3.3.1/pymodbus/server/simulator/main.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/server/simulator/setup.json` & `pymodbus-3.3.1/pymodbus/server/simulator/setup.json`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/server/simulator/web/apple120.png` & `pymodbus-3.3.1/pymodbus/server/simulator/web/apple120.png`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/server/simulator/web/apple152.png` & `pymodbus-3.3.1/pymodbus/server/simulator/web/apple152.png`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/server/simulator/web/apple60.png` & `pymodbus-3.3.1/pymodbus/server/simulator/web/apple60.png`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/server/simulator/web/apple76.png` & `pymodbus-3.3.1/pymodbus/server/simulator/web/apple76.png`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/server/simulator/web/favicon.ico` & `pymodbus-3.3.1/pymodbus/server/simulator/web/favicon.ico`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/server/simulator/web/generator/calls` & `pymodbus-3.3.1/pymodbus/server/simulator/web/generator/calls`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/server/simulator/web/generator/log` & `pymodbus-3.3.1/pymodbus/server/simulator/web/generator/log`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/server/simulator/web/generator/pymodbus_icon_original.png` & `pymodbus-3.3.1/pymodbus/server/simulator/web/generator/pymodbus_icon_original.png`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/server/simulator/web/generator/registers` & `pymodbus-3.3.1/pymodbus/server/simulator/web/generator/registers`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/server/simulator/web/generator/server` & `pymodbus-3.3.1/pymodbus/server/simulator/web/generator/server`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/server/simulator/web/index.html` & `pymodbus-3.3.1/pymodbus/server/simulator/web/index.html`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/server/simulator/web/pymodbus.css` & `pymodbus-3.3.1/pymodbus/server/simulator/web/pymodbus.css`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/server/simulator/web/welcome.html` & `pymodbus-3.3.1/pymodbus/server/simulator/web/welcome.html`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/transaction.py` & `pymodbus-3.3.1/pymodbus/transaction.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/transport/serial_asyncio/__init__.py` & `pymodbus-3.3.1/pymodbus/transport/serial_asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus/transport/transport.py` & `pymodbus-3.3.1/pymodbus/transport/transport.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,38 +6,42 @@
 import asyncio
 import ssl
 import sys
 from contextlib import suppress
 from dataclasses import dataclass
 from typing import Any, Callable, Coroutine
 
-from pymodbus.framer import ModbusFramer
 from pymodbus.logging import Log
 from pymodbus.transport.serial_asyncio import create_serial_connection
 
 
-class BaseTransport:
-    """Base class for transport types.
+class Transport:
+    """Transport layer.
 
-    BaseTransport contains functions common to all transport types and client/server.
+    Contains pure transport methods needed to connect/listen, send/receive and close connections
+    for unix socket, tcp, tls and serial communications.
 
-    This class is not available in the pymodbus API, and should not be referenced in Applications.
+    Contains high level methods like reconnect.
+
+    This class is not available in the pymodbus API, and should not be referenced in Applications
+    nor in the pymodbus documentation.
+
+    The class is designed to be an object in the message level class.
     """
 
     @dataclass
     class CommParamsClass:
         """Parameter class."""
 
         # generic
         done: bool = False
         comm_name: str = None
         reconnect_delay: float = None
         reconnect_delay_max: float = None
         timeout_connect: float = None
-        framer: ModbusFramer = None
 
         # tcp / tls / udp / serial
         host: str = None
 
         # tcp / tls / udp
         port: int = None
 
@@ -56,57 +60,57 @@
             if self.done:
                 raise RuntimeError("Already setup!")
             self.done = True
 
     def __init__(
         self,
         comm_name: str,
-        reconnect_delay: tuple[int, int],
+        reconnect_delay: int,
+        reconnect_max: int,
         timeout_connect: int,
-        framer: ModbusFramer,
         callback_connected: Callable[[], None],
         callback_disconnected: Callable[[Exception], None],
         callback_data: Callable[[bytes], int],
     ) -> None:
         """Initialize a transport instance.
 
         :param comm_name: name of this transport connection
-        :param reconnect_delay: delay and max in milliseconds for first reconnect (0,0 for no reconnect)
+        :param reconnect_delay: delay in milliseconds for first reconnect (0 for no reconnect)
+        :param reconnect_delay: max reconnect delay in milliseconds
         :param timeout_connect: Max. time in milliseconds for connect to complete
-        :param framer: Modbus framer to decode/encode messagees.
         :param callback_connected: Called when connection is established
         :param callback_disconnected: Called when connection is disconnected
         :param callback_data: Called when data is received
         """
         self.cb_connection_made = callback_connected
         self.cb_connection_lost = callback_disconnected
         self.cb_handle_data = callback_data
 
         # properties, can be read, but may not be mingled with
         self.comm_params = self.CommParamsClass(
             comm_name=comm_name,
-            reconnect_delay=reconnect_delay[0] / 1000,
-            reconnect_delay_max=reconnect_delay[1] / 1000,
+            reconnect_delay=reconnect_delay / 1000,
+            reconnect_delay_max=reconnect_max / 1000,
             timeout_connect=timeout_connect / 1000,
-            framer=framer,
         )
 
-        self.reconnect_delay_current: float = 0
+        self.reconnect_delay_current: float = 0.0
         self.transport: asyncio.BaseTransport | asyncio.Server = None
         self.protocol: asyncio.BaseProtocol = None
+        self.loop: asyncio.AbstractEventLoop = None
         with suppress(RuntimeError):
-            self.loop: asyncio.AbstractEventLoop = asyncio.get_running_loop()
-        self.reconnect_timer: asyncio.TimerHandle = None
+            self.loop = asyncio.get_running_loop()
+        self.reconnect_task: asyncio.Task = None
         self.recv_buffer: bytes = b""
         self.call_connect_listen: Callable[[], Coroutine[Any, Any, Any]] = lambda: None
         self.use_udp = False
 
-    # ----------------------------- #
-    # Transport specific parameters #
-    # ----------------------------- #
+    # ------------------------ #
+    # Transport specific setup #
+    # ------------------------ #
     def setup_unix(self, setup_server: bool, host: str):
         """Prepare transport unix"""
         if sys.platform.startswith("win"):
             raise RuntimeError("Modbus_unix is not supported on Windows!")
         self.comm_params.check_done()
         self.comm_params.done = True
         self.comm_params.host = host
@@ -259,14 +263,17 @@
                 parity=self.comm_params.parity,
                 timeout=self.comm_params.timeout_connect,
             )
 
     async def transport_connect(self):
         """Handle generic connect and call on to specific transport connect."""
         Log.debug("Connecting {}", self.comm_params.comm_name)
+        if not self.loop:
+            self.loop = asyncio.get_running_loop()
+        self.transport, self.protocol = None, None
         try:
             self.transport, self.protocol = await asyncio.wait_for(
                 self.call_connect_listen(),
                 timeout=self.comm_params.timeout_connect,
             )
         except (
             asyncio.TimeoutError,
@@ -291,26 +298,30 @@
     # ---------------------------------- #
     def connection_made(self, transport: asyncio.BaseTransport):
         """Call from asyncio, when a connection is made.
 
         :param transport: socket etc. representing the connection.
         """
         Log.debug("Connected to {}", self.comm_params.comm_name)
+        if not self.loop:
+            self.loop = asyncio.get_running_loop()
         self.transport = transport
         self.reset_delay()
         self.cb_connection_made()
 
     def connection_lost(self, reason: Exception):
         """Call from asyncio, when the connection is lost or closed.
 
         :param reason: None or an exception object
         """
         Log.debug("Connection lost {} due to {}", self.comm_params.comm_name, reason)
         self.cb_connection_lost(reason)
-        self.close(reconnect=True)
+        if self.transport:
+            self.close()
+            self.reconnect_task = asyncio.create_task(self.reconnect_connect())
 
     def eof_received(self):
         """Call when eof received (other end closed connection).
 
         Handling is moved to connection_lost()
         """
 
@@ -348,48 +359,51 @@
         """
         if self.transport:
             if hasattr(self.transport, "abort"):
                 self.transport.abort()
             self.transport.close()
             self.transport = None
         self.protocol = None
-        if self.reconnect_timer:
-            self.reconnect_timer.cancel()
-            self.reconnect_timer = None
+        if not reconnect and self.reconnect_task:
+            self.reconnect_task.cancel()
+            self.reconnect_task = None
         self.recv_buffer = b""
 
-        if not reconnect or not self.reconnect_delay_current:
-            self.reconnect_delay_current = 0
-            return
-
-        Log.debug(
-            "Waiting {} {} ms reconnecting.",
-            self.comm_params.comm_name,
-            self.reconnect_delay_current * 1000,
-        )
-        self.reconnect_timer = self.loop.call_later(
-            self.reconnect_delay_current,
-            asyncio.create_task,
-            self.transport_connect(),
-        )
-        self.reconnect_delay_current = min(
-            2 * self.reconnect_delay_current, self.comm_params.reconnect_delay_max
-        )
-
     def reset_delay(self) -> None:
         """Reset wait time before next reconnect to minimal period."""
         self.reconnect_delay_current = self.comm_params.reconnect_delay
 
     # ---------------- #
     # Internal methods #
     # ---------------- #
     def handle_listen(self):
         """Handle incoming connect."""
         return self
 
+    async def reconnect_connect(self):
+        """Handle reconnect as a task."""
+        try:
+            self.reconnect_delay_current = self.comm_params.reconnect_delay
+            transport = None
+            while not transport:
+                Log.debug(
+                    "Wait {} {} ms before reconnecting.",
+                    self.comm_params.comm_name,
+                    self.reconnect_delay_current * 1000,
+                )
+                await asyncio.sleep(self.reconnect_delay_current)
+                transport, _protocol = await self.transport_connect()
+                self.reconnect_delay_current = min(
+                    2 * self.reconnect_delay_current,
+                    self.comm_params.reconnect_delay_max,
+                )
+        except asyncio.CancelledError:
+            pass
+        self.reconnect_task = None
+
     # ----------------- #
     # The magic methods #
     # ----------------- #
     async def __aenter__(self):
         """Implement the client with async enter block."""
         return self
```

### Comparing `pymodbus-3.3.0/pymodbus/utilities.py` & `pymodbus-3.3.1/pymodbus/utilities.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/pymodbus.egg-info/PKG-INFO` & `pymodbus-3.3.1/pymodbus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymodbus
-Version: 3.3.0
+Version: 3.3.1
 Summary: A fully featured modbus protocol stack in python
 Home-page: https://github.com/pymodbus-dev/pymodbus/
 Author: "Galen Collins, Jan Iversen"
 Maintainer: "dhoomakethu, janiversen"
 License: BSD-3-Clause
 Project-URL: Source Code, https://github.com/pymodbus-dev/pymodbus
 Project-URL: Bug Reports, https://github.com/pymodbus-dev/pymodbus/issues
@@ -57,15 +57,15 @@
 
 ------------------------------------------------------------
 Supported versions
 ------------------------------------------------------------
 
 Version `2.5.3 <https://github.com/pymodbus-dev/pymodbus/releases/tag/v2.5.3>`_ is the last 2.x release (Supports python >= 2.7, no longer supported).
 
-Version `3.3.0 <https://github.com/pymodbus-dev/pymodbus/releases/tag/v3.3.0>`_ is the current release (Supports Python >= 3.8).
+Version `3.3.0 <https://github.com/pymodbus-dev/pymodbus/releases/tag/v3.3.1>`_ is the current release (Supports Python >= 3.8).
 
 .. important::
    All API changes after 3.0.0 are documented in `API_changes.rst <https://github.com/pymodbus-dev/pymodbus/blob/dev/API_changes.rst>`_
 
 
 ------------------------------------------------------------
 Summary
```

### Comparing `pymodbus-3.3.0/pymodbus.egg-info/SOURCES.txt` & `pymodbus-3.3.1/pymodbus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/requirements.txt` & `pymodbus-3.3.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/setup.cfg` & `pymodbus-3.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/setup.py` & `pymodbus-3.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/test/test_all_messages.py` & `pymodbus-3.3.1/test/test_all_messages.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/test/test_bit_read_messages.py` & `pymodbus-3.3.1/test/test_bit_read_messages.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/test/test_bit_write_messages.py` & `pymodbus-3.3.1/test/test_bit_write_messages.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/test/test_client.py` & `pymodbus-3.3.1/test/test_client.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/test/test_client_faulty_response.py` & `pymodbus-3.3.1/test/test_client_faulty_response.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/test/test_client_sync.py` & `pymodbus-3.3.1/test/test_client_sync.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/test/test_device.py` & `pymodbus-3.3.1/test/test_device.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/test/test_diag_messages.py` & `pymodbus-3.3.1/test/test_diag_messages.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/test/test_events.py` & `pymodbus-3.3.1/test/test_events.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/test/test_example_client_server.py` & `pymodbus-3.3.1/test/test_example_client_server.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/test/test_examples.py` & `pymodbus-3.3.1/test/test_examples.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/test/test_exceptions.py` & `pymodbus-3.3.1/test/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/test/test_factory.py` & `pymodbus-3.3.1/test/test_factory.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/test/test_file_message.py` & `pymodbus-3.3.1/test/test_file_message.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/test/test_framers.py` & `pymodbus-3.3.1/test/test_framers.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/test/test_logging.py` & `pymodbus-3.3.1/test/test_logging.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/test/test_mei_messages.py` & `pymodbus-3.3.1/test/test_mei_messages.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/test/test_other_messages.py` & `pymodbus-3.3.1/test/test_other_messages.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/test/test_payload.py` & `pymodbus-3.3.1/test/test_payload.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/test/test_pdu.py` & `pymodbus-3.3.1/test/test_pdu.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/test/test_register_read_messages.py` & `pymodbus-3.3.1/test/test_register_read_messages.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/test/test_register_write_messages.py` & `pymodbus-3.3.1/test/test_register_write_messages.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/test/test_remote_datastore.py` & `pymodbus-3.3.1/test/test_remote_datastore.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/test/test_repl_client.py` & `pymodbus-3.3.1/test/test_repl_client.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/test/test_server_asyncio.py` & `pymodbus-3.3.1/test/test_server_asyncio.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/test/test_server_context.py` & `pymodbus-3.3.1/test/test_server_context.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/test/test_server_multidrop.py` & `pymodbus-3.3.1/test/test_server_multidrop.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/test/test_server_task.py` & `pymodbus-3.3.1/test/test_server_task.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,14 +213,16 @@
     await task
 
 
 @pytest.mark.xdist_group(name="server_serialize")
 @pytest.mark.parametrize("comm", TEST_TYPES)
 async def test_async_task_server_stop(comm):
     """Test normal client/server handling."""
+    if comm == "udp":
+        return
     run_server, server_args, run_client, client_args = helper_config(comm, "async")
     task = asyncio.create_task(run_server(**server_args))
     await asyncio.sleep(0.5)
 
     on_reconnect_callback = mock.Mock()
 
     client = run_client(**client_args, on_reconnect_callback=on_reconnect_callback)
```

### Comparing `pymodbus-3.3.0/test/test_simulator.py` & `pymodbus-3.3.1/test/test_simulator.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/test/test_sparse_datastore.py` & `pymodbus-3.3.1/test/test_sparse_datastore.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/test/test_transaction.py` & `pymodbus-3.3.1/test/test_transaction.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/test/test_unix_socket.py` & `pymodbus-3.3.1/test/test_unix_socket.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.3.0/test/test_utilities.py` & `pymodbus-3.3.1/test/test_utilities.py`

 * *Files identical despite different names*

