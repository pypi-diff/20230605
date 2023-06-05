# Comparing `tmp/empyric-0.2.3.tar.gz` & `tmp/empyric-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "empyric-0.2.3.tar", max compression
+gzip compressed data, was "empyric-0.2.5.tar", max compression
```

## Comparing `empyric-0.2.3.tar` & `empyric-0.2.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1057 2022-02-05 04:17:18.866045 empyric-0.2.3/LICENSE
--rw-r--r--   0        0        0     6412 2023-05-31 15:01:11.750049 empyric-0.2.3/README.md
--rw-r--r--   0        0        0     2312 2023-05-31 15:01:11.751075 empyric-0.2.3/empyric/__init__.py
--rw-r--r--   0        0        0        0 2023-05-27 14:57:14.109740 empyric-0.2.3/empyric/__main__.py
--rw-r--r--   0        0        0    38454 2023-05-31 15:01:11.751723 empyric-0.2.3/empyric/adapters.py
--rw-r--r--   0        0        0       36 2023-03-29 06:16:12.180511 empyric-0.2.3/empyric/collection/__init__.py
--rw-r--r--   0        0        0     1686 2023-05-31 15:01:11.752149 empyric-0.2.3/empyric/collection/barometers.py
--rw-r--r--   0        0        0    10912 2023-05-31 15:01:11.752528 empyric-0.2.3/empyric/collection/controllers.py
--rw-r--r--   0        0        0     8565 2023-05-31 15:01:11.752878 empyric-0.2.3/empyric/collection/generators.py
--rw-r--r--   0        0        0     1182 2023-05-31 15:01:11.753110 empyric-0.2.3/empyric/collection/humans.py
--rw-r--r--   0        0        0    10487 2023-05-31 15:01:11.753366 empyric-0.2.3/empyric/collection/instrument.py
--rw-r--r--   0        0        0     3177 2023-05-31 15:01:11.753753 empyric-0.2.3/empyric/collection/io.py
--rw-r--r--   0        0        0    17628 2023-05-31 15:01:11.753942 empyric-0.2.3/empyric/collection/multimeters.py
--rw-r--r--   0        0        0    22234 2023-05-31 15:01:11.754634 empyric-0.2.3/empyric/collection/scopes.py
--rw-r--r--   0        0        0    28089 2023-05-31 15:01:11.755229 empyric-0.2.3/empyric/collection/sourcemeters.py
--rw-r--r--   0        0        0     3639 2023-05-31 15:01:11.755459 empyric-0.2.3/empyric/collection/spectrometers.py
--rw-r--r--   0        0        0     6525 2023-05-31 15:01:11.755664 empyric-0.2.3/empyric/collection/supplies.py
--rw-r--r--   0        0        0     2167 2023-05-31 15:01:11.755920 empyric-0.2.3/empyric/collection/thermometers.py
--rw-r--r--   0        0        0     9763 2023-05-31 15:01:11.756218 empyric-0.2.3/empyric/collection/virtual.py
--rw-r--r--   0        0        0    29892 2023-05-31 15:01:11.756509 empyric-0.2.3/empyric/experiment.py
--rw-r--r--   0        0        0    37351 2023-05-31 15:01:11.756847 empyric-0.2.3/empyric/graphics.py
--rw-r--r--   0        0        0      761 2023-05-31 15:01:11.757347 empyric-0.2.3/empyric/instruments.py
--rw-r--r--   0        0        0    32083 2023-05-31 15:01:11.757721 empyric-0.2.3/empyric/routines.py
--rw-r--r--   0        0        0     2329 2023-05-17 04:53:19.435384 empyric-0.2.3/empyric/runcard_schema.yaml
--rw-r--r--   0        0        0       16 2022-09-30 05:37:52.005391 empyric-0.2.3/empyric/tests/__init__.py
--rw-r--r--   0        0        0     1420 2023-05-27 14:57:14.113113 empyric-0.2.3/empyric/tests/henon_runcard_example.yaml
--rw-r--r--   0        0        0      634 2023-05-31 15:01:11.758110 empyric-0.2.3/empyric/tests/test_adapter.py
--rw-r--r--   0        0        0     2122 2023-05-31 15:01:11.758329 empyric-0.2.3/empyric/tests/test_experiment.py
--rw-r--r--   0        0        0      638 2023-05-31 15:01:11.759672 empyric-0.2.3/empyric/tests/test_variable.py
--rw-r--r--   0        0        0     8112 2023-05-31 15:01:11.760402 empyric-0.2.3/empyric/tools.py
--rw-r--r--   0        0        0     6296 2023-05-31 15:01:11.760792 empyric-0.2.3/empyric/types.py
--rw-r--r--   0        0        0    15879 2023-05-31 15:01:11.761215 empyric-0.2.3/empyric/variables.py
--rw-r--r--   0        0        0      799 2023-05-31 15:01:11.762859 empyric-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     7221 1970-01-01 00:00:00.000000 empyric-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1057 2022-02-05 04:17:18.866045 empyric-0.2.5/LICENSE
+-rw-r--r--   0        0        0     6412 2023-05-31 15:01:11.750049 empyric-0.2.5/README.md
+-rw-r--r--   0        0        0     2312 2023-05-31 15:01:11.751075 empyric-0.2.5/empyric/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-27 14:57:14.109740 empyric-0.2.5/empyric/__main__.py
+-rw-r--r--   0        0        0    38882 2023-06-04 21:44:41.067403 empyric-0.2.5/empyric/adapters.py
+-rw-r--r--   0        0        0       36 2023-03-29 06:16:12.180511 empyric-0.2.5/empyric/collection/__init__.py
+-rw-r--r--   0        0        0     1686 2023-05-31 15:01:11.752149 empyric-0.2.5/empyric/collection/barometers.py
+-rw-r--r--   0        0        0    10912 2023-05-31 15:01:11.752528 empyric-0.2.5/empyric/collection/controllers.py
+-rw-r--r--   0        0        0     9778 2023-06-02 01:59:14.990281 empyric-0.2.5/empyric/collection/generators.py
+-rw-r--r--   0        0        0     1182 2023-05-31 15:01:11.753110 empyric-0.2.5/empyric/collection/humans.py
+-rw-r--r--   0        0        0    10753 2023-06-04 21:44:41.067911 empyric-0.2.5/empyric/collection/instrument.py
+-rw-r--r--   0        0        0     3177 2023-05-31 15:01:11.753753 empyric-0.2.5/empyric/collection/io.py
+-rw-r--r--   0        0        0    17628 2023-05-31 15:01:11.753942 empyric-0.2.5/empyric/collection/multimeters.py
+-rw-r--r--   0        0        0    22234 2023-05-31 15:01:11.754634 empyric-0.2.5/empyric/collection/scopes.py
+-rw-r--r--   0        0        0    28366 2023-06-04 21:44:41.068531 empyric-0.2.5/empyric/collection/sourcemeters.py
+-rw-r--r--   0        0        0     3639 2023-05-31 15:01:11.755459 empyric-0.2.5/empyric/collection/spectrometers.py
+-rw-r--r--   0        0        0     6525 2023-05-31 15:01:11.755664 empyric-0.2.5/empyric/collection/supplies.py
+-rw-r--r--   0        0        0     2167 2023-05-31 15:01:11.755920 empyric-0.2.5/empyric/collection/thermometers.py
+-rw-r--r--   0        0        0     9763 2023-05-31 15:01:11.756218 empyric-0.2.5/empyric/collection/virtual.py
+-rw-r--r--   0        0        0    30073 2023-06-04 21:44:28.937395 empyric-0.2.5/empyric/experiment.py
+-rw-r--r--   0        0        0    37351 2023-05-31 15:01:11.756847 empyric-0.2.5/empyric/graphics.py
+-rw-r--r--   0        0        0      761 2023-05-31 15:01:11.757347 empyric-0.2.5/empyric/instruments.py
+-rw-r--r--   0        0        0    32794 2023-06-05 18:09:48.183596 empyric-0.2.5/empyric/routines.py
+-rw-r--r--   0        0        0     2329 2023-05-17 04:53:19.435384 empyric-0.2.5/empyric/runcard_schema.yaml
+-rw-r--r--   0        0        0       16 2022-09-30 05:37:52.005391 empyric-0.2.5/empyric/tests/__init__.py
+-rw-r--r--   0        0        0     1420 2023-05-27 14:57:14.113113 empyric-0.2.5/empyric/tests/henon_runcard_example.yaml
+-rw-r--r--   0        0        0      634 2023-05-31 15:01:11.758110 empyric-0.2.5/empyric/tests/test_adapter.py
+-rw-r--r--   0        0        0     2122 2023-05-31 15:01:11.758329 empyric-0.2.5/empyric/tests/test_experiment.py
+-rw-r--r--   0        0        0      638 2023-05-31 15:01:11.759672 empyric-0.2.5/empyric/tests/test_variable.py
+-rw-r--r--   0        0        0     8112 2023-05-31 15:01:11.760402 empyric-0.2.5/empyric/tools.py
+-rw-r--r--   0        0        0     6471 2023-06-02 01:59:14.991494 empyric-0.2.5/empyric/types.py
+-rw-r--r--   0        0        0    15879 2023-05-31 15:01:11.761215 empyric-0.2.5/empyric/variables.py
+-rw-r--r--   0        0        0      798 2023-06-05 18:16:02.594619 empyric-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     7192 1970-01-01 00:00:00.000000 empyric-0.2.5/PKG-INFO
```

### Comparing `empyric-0.2.3/LICENSE` & `empyric-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `empyric-0.2.3/README.md` & `empyric-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `empyric-0.2.3/empyric/__init__.py` & `empyric-0.2.5/empyric/__init__.py`

 * *Files identical despite different names*

### Comparing `empyric-0.2.3/empyric/adapters.py` & `empyric-0.2.5/empyric/adapters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import importlib
 import socket
 import time
 import re
+from threading import Lock
 
 import numpy as np
 
 from empyric.tools import read_from_socket, write_to_socket
 
 
 def chaperone(method):
@@ -20,24 +21,21 @@
     def wrapped_method(self, *args, validator=None, **kwargs):
         if not self.connected:
             raise AdapterError(
                 "Adapter is not connected for instrument "
                 f"at address {self.instrument.address}"
             )
 
-        while self.busy:  # wait for turn to talk to the instrument
-            time.sleep(0.05)
-
-        self.busy = True  # block other methods from talking to the instrument
-
         # Catch communication errors and either try to repeat communication
         # or reset the connection
         attempts = 0
         reconnects = 0
 
+        self.lock.acquire()
+
         while reconnects <= self.max_reconnects:
             while attempts < self.max_attempts:
                 try:
                     response = method(self, *args, **kwargs)
 
                     if validator and not validator(response):
                         if hasattr(response, "__len__") and len(response) > 100:
@@ -47,15 +45,15 @@
                             f"invalid response, {response}, "
                             f"from {method.__name__} method"
                         )
 
                     elif attempts > 0 or reconnects > 0:
                         print("Resolved")
 
-                    self.busy = False
+                    self.lock.release()
                     return response
 
                 except BaseException as err:
                     print(
                         f"Encountered {err} while trying "
                         f"to talk to {self.instrument.name}"
                         "\nRetrying..."
@@ -69,15 +67,15 @@
             self.connect()
 
             attempts = 0
             reconnects += 1
 
         # Getting here means that both repeats
         # and reconnects have been maxed out
-        self.busy = False
+        self.lock.release()
         raise AdapterError(f"Unable to communicate with {self.instrument.name}!")
 
     wrapped_method.__doc__ = method.__doc__  # keep method doc string
 
     return wrapped_method
 
 
@@ -124,15 +122,19 @@
         for key, value in kwargs.items():
             self.__setattr__(key, value)
 
         self.connect()
 
         self.instrument.adapter = self
 
-        self.busy = False  # indicator for multithreading
+        # This lock is used by the chaperone wrapper function to prevent
+        # cross-talk from different threads. Each time an adapter's write, read
+        # or query methods is called, the lock is acquired and then released
+        # when the transaction is complete.
+        self.lock = Lock()
 
     def __del__(self):
         # Try to cleanly close communications when adapters are deleted
         if self.connected:
             try:
                 self.disconnect()
             except BaseException as err:
@@ -368,19 +370,19 @@
         "unplug-it-then-plug-it-back-in" method.
 
         :return: None (address is printed to console)
         """
 
         input("Press enter when the instrument is disconnected")
 
-        other_devices = Serial.list(verbose=False)
+        other_devices = Serial.list()
 
         input("Press enter when the instrument is connected")
 
-        all_devices = Serial.list(verbose=False)
+        all_devices = Serial.list()
 
         try:
             instrument_address = [
                 device for device in all_devices if device not in other_devices
             ][0]
 
             print(f"Address: {instrument_address}\n")
@@ -463,17 +465,14 @@
                 if timeout is None:
                     self.backend.timeout = None
                 else:
                     self.backend.timeout = timeout * 1000
                 self._timeout = timeout
             elif self.lib == "linux-gpib":
                 self._timeout = self._linux_gpib_set_timeout(timeout)
-            elif self.lib == "prologix-gpib":
-                self.backend.timeout = timeout
-                self._timeout = timeout
         else:
             self._timeout = None
 
     def connect(self):
         if self.prologix_address is not None:
             self.lib = "prologix-gpib"
 
@@ -1034,27 +1033,35 @@
     timeout = 0.05
     byte_size = 8
     stop_bits = 1
     parity = "N"
     delay = 0.05
 
     _protocol = None
-    _serial_adapters = {}  # for Modbus Serial
+
+    # This dict contains all active Modbus serial adapters. When a new adapter
+    # is initialized with the same com port as an existing one, it uses the
+    # same Modbus client object as its backend (they are differentiated by
+    # their slave IDs).
+    _serial_adapters = {}
 
     # Locate PyModbus library
     if importlib.util.find_spec("pymodbus"):
         lib = "pymodbus"
     else:
         lib = None
 
     @property
     def busy(self):
         if self._protocol == "Serial":
             return bool(
-                sum([adapter._busy for adapter in Modbus.adapters.get(self.port, [])])
+                sum([
+                    adapter._busy for adapter in
+                    Modbus._serial_adapters.get(self.port, [])
+                ])
             )
         else:
             return self._busy
 
     @busy.setter
     def busy(self, busy):
         self._busy = busy
@@ -1068,39 +1075,52 @@
         if re.match("\d+\.\d+\.\d+\.\d+", address[0]):
             # Modbus TCP
             self._protocol = "TCP"
 
             if len(address) == 1:
                 address.append(502)  # standard Modbus TCP port
 
-            self.backend = client.ModbusTcpClient(host=address[0], port=int(address[1]))
+            self.backend = client.ModbusTcpClient(
+                host=address[0],
+                port=int(address[1])
+            )
 
         else:
             # Modbus Serial
             self._protocol = "Serial"
 
             if len(address) == 1:
-                raise ValueError(
-                    "Modbus over serial requires both the "
-                    "serial port address and slave address"
-                )
 
-            if address[0] in Modbus._serial_adapters:
-                ModbusSerial.adapters[address[0]].append(self)
+                # assume slave id is zero if not specified
+                port, slave_id = address[0], 0
+
             else:
-                ModbusSerial.adapters[self.port] = [self]
+                port, slave_id = address
+
+            if port in Modbus._serial_adapters:
+
+                Modbus._serial_adapters[port].append(self)
+
+                # use existing backend
+                self.backend = Modbus._serial_adapters[port].backend
+
+            else:
+
+                Modbus._serial_adapters[port] = [self]
 
                 self.backend = client.ModbusSerialClient(
-                    address=address[0],
+                    address=port,
                     baudrate=self.baud_rate,
                     bytesize=self.byte_size,
                     parity=self.parity,
                     stopbits=self.stop_bits,
                 )
 
+            self.slave_id = slave_id
+
         # Get data reading/writing utility classes
         payload_module = importlib.import_module(".payload", package="pymodbus")
 
         # Utility for encoding data
         self._builder_cls = payload_module.BinaryPayloadBuilder
 
         # Utility for decoding data
@@ -1120,15 +1140,16 @@
         values = np.array([values]).flatten()
 
         if func_code not in [5, 15, 6, 16]:
             raise ValueError(f"invalid Modbus function code {func_code}")
 
         if _type and _type not in self.types:
             raise TypeError(
-                "invalid _type argument; must be one of:\n" + ", ".join(self.types)
+                "invalid _type argument; must be one of:\n"
+                + ", ".join(self.types)
             )
 
         if "5" in str(func_code):
             # Write coils
 
             bool_values = [bool(value) for value in values]
 
@@ -1284,15 +1305,14 @@
         if len(address_parts) == 3:
             self.backend.setHubPort(address_parts[1])
             self.backend.setChannel(address_parts[2])
 
         self.backend.openWaitForAttachment(1000 * self.timeout)
 
         self.connected = True
-        self.busy = False
 
     def _write(self, parameter, value):
         self.backend.__getattribute__("set" + parameter)(value)
         return "Success"
 
     def _query(self, parameter):
         return self.backend.__getattribute__("get" + parameter)()
```

### Comparing `empyric-0.2.3/empyric/collection/barometers.py` & `empyric-0.2.5/empyric/collection/barometers.py`

 * *Files identical despite different names*

### Comparing `empyric-0.2.3/empyric/collection/controllers.py` & `empyric-0.2.5/empyric/collection/controllers.py`

 * *Files identical despite different names*

### Comparing `empyric-0.2.3/empyric/collection/generators.py` & `empyric-0.2.5/empyric/collection/generators.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Function/signal generators
+from typing import Union
 
 from empyric.adapters import Socket
 from empyric.instruments import Instrument, setter, getter, measurer
 from empyric.types import ON, OFF, Toggle, Integer, String, Float, recast
-from typing import Union
 
 
 class SiglentSDG1000(Instrument):
     supported_adapters = (
         (Socket, {"write_termination": "\n", "read_termination": "\n"}),
     )
 
@@ -26,14 +26,17 @@
         "channel 2 low level",
         "channel 1 frequency",
         "channel 2 frequency",
         "channel 1 pulse width",
         "channel 2 pulse width",
         "channel 1 pulse delay",
         "channel 2 pulse delay",
+        'channel 1 invert',
+        'channel 2 invert',
+        'equal phase'
     )
 
     wave_forms = ("SINE", "SQUARE", "RAMP", "PULSE", "NOISE", "ARB", "DC", "PRBS", "IQ")
 
     def _set_channel_n_output(self, n, output: Toggle, load: String, polarity: String):
         self.write(f"C{n}:OUTP {output},LOAD,{load},PLRT,{polarity}")
 
@@ -74,28 +77,48 @@
                     f'{kwargs["WVTP"]}'
                 )
 
         parameter_string = f"C{n}:BSWV " + ",".join(
             [f"{key.upper()},{value}" for key, value in kwargs.items()]
         )
 
+        # Changing the waveform parameters can cause the relative phase
+        # of the two channels to shift
+        self.equal_phase = OFF
+
         self.write(parameter_string)
 
     def _get_channel_n_waveform(self, n):
         response = self.query(f"C{n}:BSWV?")
 
         response = response.split(f"C{n}:BSWV ")[1].split(",")
 
         keys = response[::2]
         values = response[1::2]
 
         waveform_dict = {key: value for key, value in zip(keys, values)}
 
         return waveform_dict
 
+    def _set_channel_n_invert(self, n, state: Toggle):
+
+        if state == ON:
+            self.write('C%d:INVT ON' % n)
+        elif state == OFF:
+            self.write('C%d:INVT OFF' % n)
+
+    def _get_channel_n_invert(self, n):
+
+        response = self.query('C%d:INVT?' % n)
+
+        if 'ON' in response:
+            return ON
+        if 'OFF' in response:
+            return OFF
+
     # Output
     @setter
     def set_channel_1_output(self, output: Toggle):
         _, load, polarity = self._get_channel_n_output(1)
 
         self._set_channel_n_output(1, output, load, polarity)
 
@@ -272,7 +295,31 @@
         self._set_channel_n_waveform(2, dly=f"{delay}")
 
     @getter
     def get_channel_2_pulse_delay(self) -> Float:
         delay_str = self._get_channel_n_waveform(2).get("DLY", "nan")
 
         return float(delay_str.replace("S", ""))
+
+    # Output inversion
+    @setter
+    def set_channel_1_invert(self, state: Toggle):
+        self._set_channel_n_invert(1, state)
+
+    @getter
+    def get_channel_1_invert(self) -> Toggle:
+        return self._get_channel_n_invert(1)
+
+    @setter
+    def set_channel_2_invert(self, state: Toggle):
+        self._set_channel_n_invert(2, state)
+
+    @getter
+    def get_channel_2_invert(self) -> Toggle:
+        return self._get_channel_n_invert(2)
+
+    # Equalize phase of both channels
+    @setter
+    def set_equal_phase(self, state: Toggle):
+
+        if state == ON:
+            self.write('EQPHASE')
```

### Comparing `empyric-0.2.3/empyric/collection/humans.py` & `empyric-0.2.5/empyric/collection/humans.py`

 * *Files identical despite different names*

### Comparing `empyric-0.2.3/empyric/collection/instrument.py` & `empyric-0.2.5/empyric/collection/instrument.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import typing
+from threading import RLock
 from functools import wraps
 from empyric.adapters import *
 from empyric.types import recast, Type
 
 
 def setter(method):
     """
@@ -32,27 +33,28 @@
         dtype = Type
 
     @wraps(method)
     def wrapped_method(*args, **kwargs):
         self = args[0]
         value = args[1]
 
-        while self._busy:
-            time.sleep(0.01)
+        self.lock.acquire()
 
-        returned_value = method(*args, **kwargs)
+        try:
+            returned_value = method(*args, **kwargs)
 
-        # The knob attribute is set to the returned value of the method, or
-        # the value argument if the returned value is None
-        if returned_value is not None:
-            self.__setattr__(knob, recast(returned_value, to=dtype))
-        else:
-            self.__setattr__(knob, recast(value, to=dtype))
+            # The knob attribute is set to the returned value of the method, or
+            # the value argument if the returned value is None
+            if returned_value is not None:
+                self.__setattr__(knob, recast(returned_value, to=dtype))
+            else:
+                self.__setattr__(knob, recast(value, to=dtype))
+        finally:
 
-        self._busy = False
+            self.lock.release()
 
     return wrapped_method
 
 
 def getter(method):
     """
     Utility function that wraps all get_[knob] methods and records the
@@ -67,30 +69,29 @@
 
     dtype = typing.get_type_hints(method).get("return", Type)
 
     @wraps(method)
     def wrapped_method(*args, **kwargs):
         self = args[0]
 
-        while self._busy:
-            time.sleep(0.01)
+        self.lock.acquire()
 
         try:
             value = recast(method(*args, **kwargs), to=dtype)
         except AttributeError as err:
             # catches most errors caused by the adapter returning None
             if "NoneType" in str(err):
                 value = None
             else:
                 raise AttributeError(err)
+        finally:
+            self.lock.release()
 
         self.__setattr__(knob, value)
 
-        self._busy = False
-
         return value
 
     return wrapped_method
 
 
 def measurer(method):
     """
@@ -106,30 +107,29 @@
 
     dtype = typing.get_type_hints(method).get("return", Type)
 
     @wraps(method)
     def wrapped_method(*args, **kwargs):
         self = args[0]
 
-        while self._busy:
-            time.sleep(0.01)
+        self.lock.acquire()
 
         try:
             value = recast(method(*args, **kwargs), to=dtype)
         except AttributeError as err:
             # catches most errors caused by the adapter returning None
             if "NoneType" in str(err):
                 value = None
             else:
                 raise AttributeError(err)
+        finally:
+            self.lock.release()
 
         self.__setattr__(meter, value)
 
-        self._busy = False
-
         return value
 
     return wrapped_method
 
 
 class Instrument:
     """
@@ -163,18 +163,21 @@
 
     presets = {}
 
     postsets = {}
 
     meters = tuple()
 
-    # Flag for blocking concurrent operations; useful for set, get or measure
-    # methods that involve multiple adapter operations that might overlap in
-    # time with those of other set, get or measure calls.
-    _busy = False
+    # This lock is used to prevent commands executed in separate threads from
+    # interfering with each other. The lock is acquired in the setter, getter
+    # and measurer wrapper functions and then released when the wrapped
+    # operation is complete. Using an RLock allows set, get and measure
+    # methods to call other such methods without blocking, as long as it
+    # happens in the same thread, which is the norm.
+    lock = RLock()
 
     def __init__(
         self, address=None, adapter=None, presets=None, postsets=None, **kwargs
     ):
         """
 
         :param address: (str/int) address of instrument
```

### Comparing `empyric-0.2.3/empyric/collection/io.py` & `empyric-0.2.5/empyric/collection/io.py`

 * *Files identical despite different names*

### Comparing `empyric-0.2.3/empyric/collection/multimeters.py` & `empyric-0.2.5/empyric/collection/multimeters.py`

 * *Files identical despite different names*

### Comparing `empyric-0.2.3/empyric/collection/scopes.py` & `empyric-0.2.5/empyric/collection/scopes.py`

 * *Files identical despite different names*

### Comparing `empyric-0.2.3/empyric/collection/sourcemeters.py` & `empyric-0.2.5/empyric/collection/sourcemeters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import datetime
 import re
+from typing import Union
 
 import numpy as np
 import pandas as pd
 
 from empyric.collection.instrument import Instrument, setter, getter, measurer
 from empyric.adapters import GPIB
 from empyric.types import Toggle, ON, OFF, String, Float, Array
@@ -334,15 +335,15 @@
         self.adapter.delay = delay
 
     @getter
     def get_delay(self) -> Float:
         return self.adapter.delay
 
     @setter
-    def set_fast_voltages(self, voltages: [Array, String]):
+    def set_fast_voltages(self, voltages: Union[Array, String]):
         # import fast voltages, if specified as a path
         if type(voltages) == str:
             is_csv = ".csv" in voltages.lower()
             is_file = os.path.isfile(voltages)
 
             if not is_csv or not is_file:
                 raise ValueError(
@@ -369,15 +370,17 @@
         if np.ndim(voltages) == 1:
             return np.array(voltages, dtype=float)  # --> self.fast_voltages
         else:
             raise ValueError(f"invalid fast voltages: {voltages}")
 
     @measurer
     def measure_fast_currents(self) -> Array:
-        self._busy = True
+
+        normal_timeout = self.adapter.timeout
+        self.adapter.timeout = None  # measurements can take a while
 
         list_length = len(self.fast_voltages)
 
         if list_length == 0:
             raise ValueError(f"fast voltages for {self.name} have not been set")
         elif list_length <= 100:
             sub_lists = []
@@ -401,15 +404,15 @@
 
         for voltage_list in sub_lists:
             voltage_str = ", ".join(["%.4E" % voltage for voltage in voltage_list])
 
             self.write(":SOUR:LIST:VOLT " + voltage_str)
             self.write(":TRIG:COUN %d" % len(voltage_list))
 
-            raw_response = self.query(":READ?", timeout=60)
+            raw_response = self.query(":READ?")
 
             if raw_response is not None:
                 raw_response = raw_response.strip()
 
                 current_list += [
                     float(current_str) for current_str in raw_response.split(",")
                 ]
@@ -418,15 +421,15 @@
                 # truncated data; nullify measurement
                 current_list = [np.nan for _ in self.fast_voltages]
                 break
 
         self.write(":SOUR:VOLT:MODE FIX")
         self.write(":TRIG:COUN 1")
 
-        self._busy = False
+        self.adapter.timeout = normal_timeout
 
         return np.array(current_list)
 
     @setter
     def set_source_delay(self, delay: Float):
         self.write(":SOUR:DEL %.4E" % delay)
 
@@ -646,22 +649,26 @@
 
         path = self.name + "-fast_iv_measurement.csv"
 
         list_length = len(self.fast_voltages)
 
         if list_length >= 100:
             sub_lists = [
-                self.fast_voltages[i * 100 : (i + 1) * 100]
+                self.fast_voltages[ # pylint: disable=unsubscriptable-object
+                    i * 100 : (i + 1) * 100
+                ]
                 for i in range(list_length // 100)
             ]
         else:
             sub_lists = []
 
         if list_length % 100 > 0:
-            sub_lists.append(self.fast_voltages[-(list_length % 100) :])
+            sub_lists.append(
+                self.fast_voltages[-(list_length % 100) :] # pylint: disable=unsubscriptable-object
+            )
 
         current_list = []
 
         normal_timeout = self.adapter.timeout
         self.adapter.timeout = None  # the response times can be long
 
         start = datetime.datetime.now()
```

### Comparing `empyric-0.2.3/empyric/collection/spectrometers.py` & `empyric-0.2.5/empyric/collection/spectrometers.py`

 * *Files identical despite different names*

### Comparing `empyric-0.2.3/empyric/collection/supplies.py` & `empyric-0.2.5/empyric/collection/supplies.py`

 * *Files identical despite different names*

### Comparing `empyric-0.2.3/empyric/collection/thermometers.py` & `empyric-0.2.5/empyric/collection/thermometers.py`

 * *Files identical despite different names*

### Comparing `empyric-0.2.3/empyric/collection/virtual.py` & `empyric-0.2.5/empyric/collection/virtual.py`

 * *Files identical despite different names*

### Comparing `empyric-0.2.3/empyric/experiment.py` & `empyric-0.2.5/empyric/experiment.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,21 +212,25 @@
 
             value = self.variables[name].value
 
             self.eval_events[name].set()
             # unblock threads evaluating dependents
 
             if np.size(value) > 1:  # store array data as CSV files
-                dataframe = pd.DataFrame(
-                    {name: value}, index=[self.state.name] * len(value)
-                )
-                path = name.replace(" ", "_") + "_"
-                path += self.state.name.strftime("%Y%m%d-%H%M%S") + ".csv"
-                dataframe.to_csv(path)
-                self.state[name] = path
+                if np.any(value):
+                    # only save non-empty arrays
+                    dataframe = pd.DataFrame(
+                        {name: value}, index=[self.state.name] * len(value)
+                    )
+                    path = name.replace(" ", "_") + "_"
+                    path += self.state.name.strftime("%Y%m%d-%H%M%S") + ".csv"
+                    dataframe.to_csv(path)
+                    self.state[name] = path
+                else:
+                    self.state[name] = None
             else:
                 self.state[name] = value
         except BaseException as err:
             self.terminate()
             raise err
 
     def _update_routine(self, name):
@@ -793,27 +797,27 @@
 
             alphabet = "abcdefghijklmnopqrstuvwxyz"
             for var_name, variable in variables.items():
                 # Variables can be called by name in the condition
                 if var_name in condition:
                     temp_name = "".join(
                         [
-                            alphabet[
+                            alphabet[  # pylint: disable=invalid-sequence-index
                                 np.random.randint(0, len(alphabet))
-                            ]  # pylint: disable=invalid-sequence-index
+                            ]
                             for i in range(3)
                         ]
                     )
                     while temp_name in alarm_variables:
                         # make sure temp_name is not repeated
                         temp_name = "".join(
                             [
-                                alphabet[
+                                alphabet[  # pylint: disable=invalid-sequence-index
                                     np.random.randint(0, len(alphabet))
-                                ]  # pylint: disable=invalid-sequence-index
+                                ]
                                 for i in range(3)
                             ]
                         )
 
                     alarm_variables.update({temp_name: variable})
                     condition = condition.replace(var_name, temp_name)
```

### Comparing `empyric-0.2.3/empyric/graphics.py` & `empyric-0.2.5/empyric/graphics.py`

 * *Files identical despite different names*

### Comparing `empyric-0.2.3/empyric/instruments.py` & `empyric-0.2.5/empyric/instruments.py`

 * *Files identical despite different names*

### Comparing `empyric-0.2.3/empyric/routines.py` & `empyric-0.2.5/empyric/routines.py`

 * *Files 3% similar despite different names*

```diff
@@ -106,14 +106,18 @@
                     for name, knob in self.knobs.items():
                         if knob._controller == self:
                             knob._controller = None
 
                 return
 
             else:
+
+                if not self.prepped:
+                    self.prep(state)
+
                 for name, knob in self.knobs.items():
                     if knob._controller and knob._controller != self:
                         # take no action if another routine has control
                         return
                     elif self.assert_control:
                         # assert control if needed
                         knob._controller = self
@@ -298,14 +302,15 @@
         if "end" not in kwargs:
             self.end = np.max(self.times)
 
     @Routine.enabler
     def update(self, state):
         knobs_times_values = zip(self.knobs, self.times, self.values)
         for knob, times, values in knobs_times_values:
+
             if np.min(times) > state["Time"] or np.max(times) < state["Time"]:
                 continue
 
             j_last = np.argwhere(times <= state["Time"]).flatten()[-1]
             j_next = np.argwhere(times > state["Time"]).flatten()[0]
 
             last_time = times[j_last]
@@ -315,34 +320,49 @@
             next_value = values[j_next]
 
             if last_value in list(state.keys()):
                 # if last_value is a variable name,
                 # use that variable's value from state
                 last_value = state[last_value]
 
-            last_is_number = isinstance(last_value, numbers.Number)
-            next_is_number = isinstance(next_value, numbers.Number)
+            if next_value in list(state.keys()):
+                next_value = state[next_value]
 
-            if next_is_number and last_is_number:
-                # ramp linearly between numerical values
-                value = last_value + (next_value - last_value) * (
-                    state["Time"] - last_time
-                ) / (next_time - last_time)
-            else:
-                # stay at last value until next time,
-                # when value variable will be evaluated
-                value = last_value
+            # Ramp linearly between numerical values
+            value = last_value + (next_value - last_value) * (
+                state["Time"] - last_time
+            ) / (next_time - last_time)
 
             self.knobs[knob].value = value
 
+    def prep(self, state):
+
+        # Validate values
+        for knob, value_list in zip(self.knobs.keys(), self.values):
+            for value in value_list:
+
+                is_number = isinstance(value, numbers.Number)
+                is_variable = value in list(state.keys())
+
+                if not is_number and not is_variable:
+                    raise ValueError(
+                        f'value {value} given for knob {knob} in Timecourse '
+                        f'routine is invalid; value must be a numeric type or '
+                        f'the name of a variable in the updating state'
+                    )
+
     def finish(self, state):
         # Upon routine completion, set each knob to its final value
         for knob, value in zip(self.knobs.values(), self.values[:, -1]):
             if knob._controller is None or knob._controller == self:
-                knob.value = value
+
+                if isinstance(value, String) and value in state:
+                    knob.value = state[value]
+                else:
+                    knob.value = value
 
 
 class Sequence(Routine):
     """
     Passes the `knobs` through a series of `values` regardless of time.
 
     The `values` should be a 1D or 2D array of keys/values; if 2D then the first
@@ -381,15 +401,19 @@
 
         self.iteration = (self.iteration + 1) % len(self.values[0])
 
     def finish(self, state):
         # Upon routine completion, set each knob to its final value
         for knob, value in zip(self.knobs.values(), self.values[:, -1]):
             if knob._controller is None or knob._controller == self:
-                knob.value = value
+
+                if isinstance(value, String) and value in state:
+                    knob.value = state[value]
+                else:
+                    knob.value = value
 
 
 class Minimization(Routine):
     """
     Minimize a `meter`(/expression) influenced by the set of `knobs`, using
     simulated annealing.
```

### Comparing `empyric-0.2.3/empyric/runcard_schema.yaml` & `empyric-0.2.5/empyric/runcard_schema.yaml`

 * *Files identical despite different names*

### Comparing `empyric-0.2.3/empyric/tests/henon_runcard_example.yaml` & `empyric-0.2.5/empyric/tests/henon_runcard_example.yaml`

 * *Files identical despite different names*

### Comparing `empyric-0.2.3/empyric/tests/test_adapter.py` & `empyric-0.2.5/empyric/tests/test_adapter.py`

 * *Files identical despite different names*

### Comparing `empyric-0.2.3/empyric/tests/test_experiment.py` & `empyric-0.2.5/empyric/tests/test_experiment.py`

 * *Files identical despite different names*

### Comparing `empyric-0.2.3/empyric/tests/test_variable.py` & `empyric-0.2.5/empyric/tests/test_variable.py`

 * *Files identical despite different names*

### Comparing `empyric-0.2.3/empyric/tools.py` & `empyric-0.2.5/empyric/tools.py`

 * *Files identical despite different names*

### Comparing `empyric-0.2.3/empyric/types.py` & `empyric-0.2.5/empyric/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Standardization of data types
 import abc
 import os
 import re
 from abc import ABC
 import pandas as pd
 import numpy as np
-from typing import Any, Union
+from typing import Any, Union, get_origin, get_args
 
 
 class Type(ABC):
     """Abstract base class for all supported data types"""
 
     pass
 
@@ -151,28 +151,34 @@
     """
 
     if to != Type:
         if value is None:
             return None
 
         for dtype in np.array([to], dtype=object).flatten():
+            # Recast to desired type
             try:
-                # recast to desired
+
+                if get_origin(dtype) is Union:
+                    # Expand type unions
+                    return recast(value, to=get_args(dtype))
+
                 if issubclass(dtype, Boolean):
                     return np.bool_(value)
                 elif issubclass(dtype, Toggle):
                     return Toggle(value)
                 elif issubclass(dtype, Integer):
                     return np.int64(value)
                 elif issubclass(dtype, Float):
                     return np.float64(value)
                 elif issubclass(dtype, String):
                     return np.str_(value)
                 elif issubclass(dtype, Array) and np.ndim(value) > 0:
                     return np.array(value)
+
             except ValueError:
                 pass
 
         print(f"Warning: unable to recast value {value} to type {to}")
 
         return None
```

### Comparing `empyric-0.2.3/empyric/variables.py` & `empyric-0.2.5/empyric/variables.py`

 * *Files identical despite different names*

### Comparing `empyric-0.2.3/pyproject.toml` & `empyric-0.2.5/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "empyric"
-version = "0.2.3"
+version = "0.2.5"
 description = "A package for experiment automation"
 authors = ["Daniel Merthe <dmerthe@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/dmerthe/empyric"
 packages = [
     { include = "empyric"},
 ]
@@ -12,19 +12,19 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-numpy = "~1.24.3"
-scipy = "~1.9.3"
-matplotlib = "~3.6"
-pandas = "~1.5.3"
-pykwalify = "~1.8"
+numpy = "1.24.3"
+scipy = "1.9.3"
+matplotlib = "3.6.2"
+pandas = "1.5.3"
+pykwalify = "1.8.0"
 "ruamel.yaml" = "0.17.21"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "*"
 pylint = "*"
 black = "*"
```

### Comparing `empyric-0.2.3/PKG-INFO` & `empyric-0.2.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: empyric
-Version: 0.2.3
+Version: 0.2.5
 Summary: A package for experiment automation
 Home-page: https://github.com/dmerthe/empyric
 Author: Daniel Merthe
 Author-email: dmerthe@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: matplotlib (>=3.6,<3.7)
-Requires-Dist: numpy (>=1.24.3,<1.25.0)
-Requires-Dist: pandas (>=1.5.3,<1.6.0)
-Requires-Dist: pykwalify (>=1.8,<1.9)
+Requires-Dist: matplotlib (==3.6.2)
+Requires-Dist: numpy (==1.24.3)
+Requires-Dist: pandas (==1.5.3)
+Requires-Dist: pykwalify (==1.8.0)
 Requires-Dist: ruamel.yaml (==0.17.21)
-Requires-Dist: scipy (>=1.9.3,<1.10.0)
+Requires-Dist: scipy (==1.9.3)
 Project-URL: Repository, https://github.com/dmerthe/empyric
 Description-Content-Type: text/markdown
 
 # Empyric 
 ## A Python Library for Experiment Automation
 
 For more details, [read the docs](https://empyric.readthedocs.io/en/latest/).
```

