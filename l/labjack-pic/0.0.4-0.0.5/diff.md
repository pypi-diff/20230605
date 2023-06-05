# Comparing `tmp/labjack_pic-0.0.4.tar.gz` & `tmp/labjack_pic-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labjack_pic-0.0.4.tar", last modified: Wed Dec 14 02:42:43 2022, max compression
+gzip compressed data, was "labjack_pic-0.0.5.tar", last modified: Mon Jun  5 16:05:54 2023, max compression
```

## Comparing `labjack_pic-0.0.4.tar` & `labjack_pic-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 markrages  (1001) markrages  (1000)        0 2022-12-14 02:42:43.923676 labjack_pic-0.0.4/
--rw-rw-r--   0 markrages  (1001) markrages  (1000)    11357 2022-11-20 02:22:29.000000 labjack_pic-0.0.4/LICENSE
--rw-rw-r--   0 markrages  (1001) markrages  (1000)     3182 2022-12-14 02:42:43.923676 labjack_pic-0.0.4/PKG-INFO
--rw-rw-r--   0 markrages  (1001) markrages  (1000)     2642 2022-12-14 01:50:19.000000 labjack_pic-0.0.4/README.md
--rw-rw-r--   0 markrages  (1001) markrages  (1000)      726 2022-12-14 02:40:24.000000 labjack_pic-0.0.4/pyproject.toml
--rw-rw-r--   0 markrages  (1001) markrages  (1000)       38 2022-12-14 02:42:43.923676 labjack_pic-0.0.4/setup.cfg
-drwxrwxr-x   0 markrages  (1001) markrages  (1000)        0 2022-12-14 02:42:43.919676 labjack_pic-0.0.4/src/
-drwxrwxr-x   0 markrages  (1001) markrages  (1000)        0 2022-12-14 02:42:43.919676 labjack_pic-0.0.4/src/labjack_pic/
--rw-rw-r--   0 markrages  (1001) markrages  (1000)        1 2022-12-01 04:10:46.000000 labjack_pic-0.0.4/src/labjack_pic/__init__.py
--rwxr--r--   0 markrages  (1001) markrages  (1000)    15613 2022-12-14 02:40:53.000000 labjack_pic-0.0.4/src/labjack_pic/lj_pic.py
-drwxrwxr-x   0 markrages  (1001) markrages  (1000)        0 2022-12-14 02:42:43.923676 labjack_pic-0.0.4/src/labjack_pic/u3_manager/
--rw-rw-r--   0 markrages  (1001) markrages  (1000)        0 2022-12-01 04:10:38.000000 labjack_pic-0.0.4/src/labjack_pic/u3_manager/__init__.py
--rwxrwxr-x   0 markrages  (1001) markrages  (1000)    12856 2022-11-28 23:45:17.000000 labjack_pic-0.0.4/src/labjack_pic/u3_manager/u3_manager.py
-drwxrwxr-x   0 markrages  (1001) markrages  (1000)        0 2022-12-14 02:42:43.923676 labjack_pic-0.0.4/src/labjack_pic.egg-info/
--rw-rw-r--   0 markrages  (1001) markrages  (1000)     3182 2022-12-14 02:42:43.000000 labjack_pic-0.0.4/src/labjack_pic.egg-info/PKG-INFO
--rw-rw-r--   0 markrages  (1001) markrages  (1000)      402 2022-12-14 02:42:43.000000 labjack_pic-0.0.4/src/labjack_pic.egg-info/SOURCES.txt
--rw-rw-r--   0 markrages  (1001) markrages  (1000)        1 2022-12-14 02:42:43.000000 labjack_pic-0.0.4/src/labjack_pic.egg-info/dependency_links.txt
--rw-rw-r--   0 markrages  (1001) markrages  (1000)       56 2022-12-14 02:42:43.000000 labjack_pic-0.0.4/src/labjack_pic.egg-info/entry_points.txt
--rw-rw-r--   0 markrages  (1001) markrages  (1000)       23 2022-12-14 02:42:43.000000 labjack_pic-0.0.4/src/labjack_pic.egg-info/requires.txt
--rw-rw-r--   0 markrages  (1001) markrages  (1000)       12 2022-12-14 02:42:43.000000 labjack_pic-0.0.4/src/labjack_pic.egg-info/top_level.txt
+drwxrwxr-x   0 markrages  (1001) markrages  (1000)        0 2023-06-05 16:05:54.302288 labjack_pic-0.0.5/
+-rw-rw-r--   0 markrages  (1001) markrages  (1000)    11357 2022-11-20 02:22:29.000000 labjack_pic-0.0.5/LICENSE
+-rw-rw-r--   0 markrages  (1001) markrages  (1000)     3182 2023-06-05 16:05:54.302288 labjack_pic-0.0.5/PKG-INFO
+-rw-rw-r--   0 markrages  (1001) markrages  (1000)     2642 2022-12-14 01:50:19.000000 labjack_pic-0.0.5/README.md
+-rw-rw-r--   0 markrages  (1001) markrages  (1000)      726 2023-06-05 16:04:43.000000 labjack_pic-0.0.5/pyproject.toml
+-rw-rw-r--   0 markrages  (1001) markrages  (1000)       38 2023-06-05 16:05:54.302288 labjack_pic-0.0.5/setup.cfg
+drwxrwxr-x   0 markrages  (1001) markrages  (1000)        0 2023-06-05 16:05:54.298288 labjack_pic-0.0.5/src/
+drwxrwxr-x   0 markrages  (1001) markrages  (1000)        0 2023-06-05 16:05:54.302288 labjack_pic-0.0.5/src/labjack_pic/
+-rw-rw-r--   0 markrages  (1001) markrages  (1000)        1 2022-12-01 04:10:46.000000 labjack_pic-0.0.5/src/labjack_pic/__init__.py
+-rwxrwxr-x   0 markrages  (1001) markrages  (1000)    15613 2023-06-05 16:00:08.000000 labjack_pic-0.0.5/src/labjack_pic/lj_pic.py
+drwxrwxr-x   0 markrages  (1001) markrages  (1000)        0 2023-06-05 16:05:54.302288 labjack_pic-0.0.5/src/labjack_pic/u3_manager/
+-rw-rw-r--   0 markrages  (1001) markrages  (1000)        0 2022-12-01 04:10:38.000000 labjack_pic-0.0.5/src/labjack_pic/u3_manager/__init__.py
+-rwxr--r--   0 markrages  (1001) markrages  (1000)    13637 2023-06-05 16:00:37.000000 labjack_pic-0.0.5/src/labjack_pic/u3_manager/u3_manager.py
+drwxrwxr-x   0 markrages  (1001) markrages  (1000)        0 2023-06-05 16:05:54.302288 labjack_pic-0.0.5/src/labjack_pic.egg-info/
+-rw-rw-r--   0 markrages  (1001) markrages  (1000)     3182 2023-06-05 16:05:54.000000 labjack_pic-0.0.5/src/labjack_pic.egg-info/PKG-INFO
+-rw-rw-r--   0 markrages  (1001) markrages  (1000)      402 2023-06-05 16:05:54.000000 labjack_pic-0.0.5/src/labjack_pic.egg-info/SOURCES.txt
+-rw-rw-r--   0 markrages  (1001) markrages  (1000)        1 2023-06-05 16:05:54.000000 labjack_pic-0.0.5/src/labjack_pic.egg-info/dependency_links.txt
+-rw-rw-r--   0 markrages  (1001) markrages  (1000)       56 2023-06-05 16:05:54.000000 labjack_pic-0.0.5/src/labjack_pic.egg-info/entry_points.txt
+-rw-rw-r--   0 markrages  (1001) markrages  (1000)       23 2023-06-05 16:05:54.000000 labjack_pic-0.0.5/src/labjack_pic.egg-info/requires.txt
+-rw-rw-r--   0 markrages  (1001) markrages  (1000)       12 2023-06-05 16:05:54.000000 labjack_pic-0.0.5/src/labjack_pic.egg-info/top_level.txt
```

### Comparing `labjack_pic-0.0.4/LICENSE` & `labjack_pic-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `labjack_pic-0.0.4/PKG-INFO` & `labjack_pic-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labjack_pic
-Version: 0.0.4
+Version: 0.0.5
 Summary: Program PIC microcontrollers using LabJack U3
 Author-email: Mark Rages <markrages@gmail.com>
 Project-URL: Homepage, https://github.com/markrages/labjack_pic/
 Project-URL: Bug Tracker, https://github.com/markrages/labjack_pic/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `labjack_pic-0.0.4/README.md` & `labjack_pic-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `labjack_pic-0.0.4/pyproject.toml` & `labjack_pic-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "labjack_pic"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Mark Rages", email="markrages@gmail.com" },
 ]
 description = "Program PIC microcontrollers using LabJack U3"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `labjack_pic-0.0.4/src/labjack_pic/lj_pic.py` & `labjack_pic-0.0.5/src/labjack_pic/lj_pic.py`

 * *Files identical despite different names*

### Comparing `labjack_pic-0.0.4/src/labjack_pic/u3_manager/u3_manager.py` & `labjack_pic-0.0.5/src/labjack_pic/u3_manager/u3_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -264,42 +264,72 @@
             self._fill_rx_buffer()
 
     def _fill_rx_buffer(self):
         rb = self.parent.asynchRX()
         ct = rb['NumAsynchBytesInRXBuffer']
         self.readbuffer += bytes(rb['AsynchBytes'][:ct])
 
-class I2C(object):
-    "LabJack I2C bus using the interface of nrf5x.py and drivers.py"
-    def __init__(self, scl_pin, sda_pin, address):
-        assert scl_pin.parent == sda_pin.parent # both pins must be same labjack
-        self.parent = scl_pin.parent
-        self.sda = sda_pin.number
-        self.scl = scl_pin.number
+class I2CAddressed(object):
+    def __init__(self, parent, address):
+        self.parent = parent
         self.address = address
 
     def write(self, command, data, stop=True):
         return self(I2CBytes = [command]+data,
                     NumI2CBytesToReceive = 0)
 
     def read(self, count, stop=True):
         return self(I2CBytes = [],
                     NumI2CBytesToReceive = count)
 
     def __call__(self, *args, **kwargs):
+        kwargs.setdefault('Address', self.address)
+        return self.parent(*args, **kwargs)
+
+    def compat(self):
+        return I2CAddressedCompat(self)
+
+class I2CAddressedCompat(object):
+    def __init__(self, parent):
+        self.parent = parent
+
+    def write(self, data):
+        print('data',data)
+        return self.exchange(data=data, count=0)
+
+    def read(self, count):
+        return self.exchange(data=[], count=count)
+
+    def exchange(self, data, count):
+        ret = self.parent(I2CBytes = list(data),
+                          NumI2CBytesToReceive = count)
+        print(ret)
+        return bytes(ret['I2CBytes'])
+
+class I2C(object):
+    "LabJack I2C bus using the interface of nrf5x.py and drivers.py"
+    def __init__(self, scl_pin, sda_pin):
+        assert scl_pin.parent == sda_pin.parent # both pins must be same labjack
+        self.parent = scl_pin.parent
+        self.sda = sda_pin.number
+        self.scl = scl_pin.number
+
+    def address(self, address):
+        return I2CAddressed(self, address)
+
+    def __call__(self, *args, **kwargs):
         """ Here's a giant back door.
 
         Calling the object is the same as calling u3 objects's "i2c" method.
 
         So this is not at all the same interface as the nrf5x.py i2c objects.
 
         But *this* interface could be grafted on to nrf5x.py fairly easily.
         """
 
-        kwargs.setdefault('Address', self.address)
         kwargs.setdefault('I2CBytes',[])
         kwargs.setdefault('EnableClockStretching',True)
         kwargs.setdefault('NumI2CBytesToReceive', 0)
         #kwargs.setdefault('SpeedAdjust',200)
         #kwargs['ResetAtStart'] = True
 
         kwargs['SDAPinNum']=self.sda
@@ -330,15 +360,15 @@
         return ret
 
 class ManagedU3(u3py.U3):
     def __init__(self, *args, **kwargs):
         super(ManagedU3, self).__init__(*args, **kwargs)
         self.getCalibrationData()
 
-        #assert self.deviceName in ['U3-HV']
+        # assert self.deviceName in ['U3-HV']
 
         self.FIO = [FIOPin(self, pin) for pin in range(8)]
         self.EIO = [FIOPin(self, pin+8) for pin in range(8)]
         self.CIO = [FIOPin(self, pin+16) for pin in range(8)]
 
         for pin in range(8):
             setattr(self, 'FIO%d'%pin, self.FIO[pin])
@@ -374,15 +404,15 @@
             volts = (bits - self.calData['dac%sOffset' % dacNumber]) / self.calData['dac%sSlope' % dacNumber]
         else:
             volts = bits / 51.717
 
         return volts
 
     def i2c_bus(self, sda, scl):
-        return I2C(sda_pin=sda, scl_pin=scl, address=None)
+        return I2C(sda_pin=sda, scl_pin=scl)
 
 u3_devices = {}
 
 def u3(*args, **kwargs):
     global u3_devices
 
     if ('serial' not in kwargs) or (kwargs['serial'] not in u3_devices):
```

### Comparing `labjack_pic-0.0.4/src/labjack_pic.egg-info/PKG-INFO` & `labjack_pic-0.0.5/src/labjack_pic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labjack-pic
-Version: 0.0.4
+Version: 0.0.5
 Summary: Program PIC microcontrollers using LabJack U3
 Author-email: Mark Rages <markrages@gmail.com>
 Project-URL: Homepage, https://github.com/markrages/labjack_pic/
 Project-URL: Bug Tracker, https://github.com/markrages/labjack_pic/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

