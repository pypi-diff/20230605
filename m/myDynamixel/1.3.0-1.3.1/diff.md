# Comparing `tmp/myDynamixel-1.3.0-py3-none-any.whl.zip` & `tmp/myDynamixel-1.3.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 3772 bytes, number of entries: 6
+Zip file size: 3859 bytes, number of entries: 6
 -rw-rw-rw-  2.0 fat       37 b- defN 22-Dec-12 06:36 myDynamixel/__init__.py
--rw-rw-rw-  2.0 fat    11773 b- defN 23-May-31 02:03 myDynamixel/myDynamixel.py
--rw-rw-rw-  2.0 fat      258 b- defN 23-May-31 02:06 myDynamixel-1.3.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-31 02:06 myDynamixel-1.3.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-May-31 02:06 myDynamixel-1.3.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      475 b- defN 23-May-31 02:06 myDynamixel-1.3.0.dist-info/RECORD
-6 files, 12647 bytes uncompressed, 2908 bytes compressed:  77.0%
+-rw-rw-rw-  2.0 fat    12620 b- defN 23-Jun-05 08:15 myDynamixel/myDynamixel.py
+-rw-rw-rw-  2.0 fat      258 b- defN 23-Jun-05 08:16 myDynamixel-1.3.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-05 08:16 myDynamixel-1.3.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-Jun-05 08:16 myDynamixel-1.3.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      475 b- defN 23-Jun-05 08:16 myDynamixel-1.3.1.dist-info/RECORD
+6 files, 13494 bytes uncompressed, 2995 bytes compressed:  77.8%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: myDynamixel/__init__.py
 Comment: 
 
 Filename: myDynamixel/myDynamixel.py
 Comment: 
 
-Filename: myDynamixel-1.3.0.dist-info/METADATA
+Filename: myDynamixel-1.3.1.dist-info/METADATA
 Comment: 
 
-Filename: myDynamixel-1.3.0.dist-info/WHEEL
+Filename: myDynamixel-1.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: myDynamixel-1.3.0.dist-info/top_level.txt
+Filename: myDynamixel-1.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: myDynamixel-1.3.0.dist-info/RECORD
+Filename: myDynamixel-1.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## myDynamixel/myDynamixel.py

```diff
@@ -1,8 +1,8 @@
-# ver 1.3.0
+# ver 1.3.1
 
 import numpy as np
 from dynamixel_sdk import *
 
 class Dxlfunc:
     class Adrress:
         ModelNumber         = 0
@@ -249,7 +249,21 @@
         self.Change_OperatingMode(MotorID, self.operating_mode.extended_Position_control)
         self.write(MotorID, self.Adrress.TorqueEnable, False)
         self.write(MotorID, self.Adrress.DriveMode, 4)
         self.write(MotorID, self.Adrress.TorqueEnable, True)
         self.write(MotorID, self.Adrress.ProfileVelocity, Goal_Time)
         self.write(MotorID, self.Adrress.GoalPosition, Goal_position)
         self.write(MotorID, self.Adrress.ProfileVelocity, 0)
+
+    def CurrentCnt_Vbase(self, MotorID, Goal_current, Goal_velocity):
+        if self.Present_OperatingMode != self.operating_mode.current_base_position_control:
+            self.Change_OperatingMode(MotorID, self.operating_mode.current_base_position_control)
+        self.write(MotorID, self.Adrress.TorqueEnable, False)
+        self.write(MotorID, self.Adrress.DriveMode, 0)
+        self.write(MotorID, self.Adrress.TorqueEnable, True)
+        self.write(MotorID, self.Adrress.ProfileVelocity, Goal_velocity)
+        self.write(MotorID, self.Adrress.GoalCurrent, np.abs(Goal_current))
+        if Goal_current < 0:
+            self.write(MotorID, self.Adrress.GoalPosition, -256*4096+1)
+        else:
+            self.write(MotorID, self.Adrress.GoalPosition, 256*4096-1)
+        self.write(MotorID, self.Adrress.ProfileVelocity, 0)
```

