# Comparing `tmp/myDynamixel-1.3.1-py3-none-any.whl.zip` & `tmp/myDynamixel-1.3.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 3859 bytes, number of entries: 6
+Zip file size: 3920 bytes, number of entries: 6
 -rw-rw-rw-  2.0 fat       37 b- defN 22-Dec-12 06:36 myDynamixel/__init__.py
--rw-rw-rw-  2.0 fat    12620 b- defN 23-Jun-05 08:15 myDynamixel/myDynamixel.py
--rw-rw-rw-  2.0 fat      258 b- defN 23-Jun-05 08:16 myDynamixel-1.3.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-05 08:16 myDynamixel-1.3.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-Jun-05 08:16 myDynamixel-1.3.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      475 b- defN 23-Jun-05 08:16 myDynamixel-1.3.1.dist-info/RECORD
-6 files, 13494 bytes uncompressed, 2995 bytes compressed:  77.8%
+-rw-rw-rw-  2.0 fat    13012 b- defN 23-Jun-05 08:59 myDynamixel/myDynamixel.py
+-rw-rw-rw-  2.0 fat      258 b- defN 23-Jun-05 09:09 myDynamixel-1.3.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-05 09:09 myDynamixel-1.3.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-Jun-05 09:09 myDynamixel-1.3.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      475 b- defN 23-Jun-05 09:09 myDynamixel-1.3.2.dist-info/RECORD
+6 files, 13886 bytes uncompressed, 3056 bytes compressed:  78.0%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: myDynamixel/__init__.py
 Comment: 
 
 Filename: myDynamixel/myDynamixel.py
 Comment: 
 
-Filename: myDynamixel-1.3.1.dist-info/METADATA
+Filename: myDynamixel-1.3.2.dist-info/METADATA
 Comment: 
 
-Filename: myDynamixel-1.3.1.dist-info/WHEEL
+Filename: myDynamixel-1.3.2.dist-info/WHEEL
 Comment: 
 
-Filename: myDynamixel-1.3.1.dist-info/top_level.txt
+Filename: myDynamixel-1.3.2.dist-info/top_level.txt
 Comment: 
 
-Filename: myDynamixel-1.3.1.dist-info/RECORD
+Filename: myDynamixel-1.3.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## myDynamixel/myDynamixel.py

```diff
@@ -1,8 +1,8 @@
-# ver 1.3.1
+# ver 1.3.2
 
 import numpy as np
 from dynamixel_sdk import *
 
 class Dxlfunc:
     class Adrress:
         ModelNumber         = 0
@@ -233,32 +233,38 @@
             now_frag = self.read(MotorID, self.Adrress.TorqueEnable)
             self.write(MotorID, self.Adrress.TorqueEnable, 0)
             self.write(MotorID, self.Adrress.OperatingMode, INPUT_OPERATING_MODE)
             self.write(MotorID, self.Adrress.TorqueEnable, now_frag)
         self.Present_OperatingMode = INPUT_OPERATING_MODE
 
     def PosCnt_Vbase(self, MotorID, Goal_position, Goal_velocity):
+        if Goal_velocity < 0:
+            raise self.DXL_Error('Goal velocity should be positive value in PosCnt_Vbase function')
         self.Change_OperatingMode(MotorID, self.operating_mode.extended_Position_control)
         self.write(MotorID, self.Adrress.TorqueEnable, False)
         self.write(MotorID, self.Adrress.DriveMode, 0)
         self.write(MotorID, self.Adrress.TorqueEnable, True)
         self.write(MotorID, self.Adrress.ProfileVelocity, Goal_velocity)
         self.write(MotorID, self.Adrress.GoalPosition, Goal_position)
         self.write(MotorID, self.Adrress.ProfileVelocity, 0)
 
     def PosCnt_Tbase(self, MotorID, Goal_position, Goal_Time):
+        if Goal_Time < 0:
+            raise self.DXL_Error('Goal time should be positive value in PosCnt_Tbase function')
         self.Change_OperatingMode(MotorID, self.operating_mode.extended_Position_control)
         self.write(MotorID, self.Adrress.TorqueEnable, False)
         self.write(MotorID, self.Adrress.DriveMode, 4)
         self.write(MotorID, self.Adrress.TorqueEnable, True)
         self.write(MotorID, self.Adrress.ProfileVelocity, Goal_Time)
         self.write(MotorID, self.Adrress.GoalPosition, Goal_position)
         self.write(MotorID, self.Adrress.ProfileVelocity, 0)
 
     def CurrentCnt_Vbase(self, MotorID, Goal_current, Goal_velocity):
+        if Goal_velocity < 0:
+            raise self.DXL_Error('Goal velocity should be positive value in CurrentCnt_Vbase function')
         if self.Present_OperatingMode != self.operating_mode.current_base_position_control:
             self.Change_OperatingMode(MotorID, self.operating_mode.current_base_position_control)
         self.write(MotorID, self.Adrress.TorqueEnable, False)
         self.write(MotorID, self.Adrress.DriveMode, 0)
         self.write(MotorID, self.Adrress.TorqueEnable, True)
         self.write(MotorID, self.Adrress.ProfileVelocity, Goal_velocity)
         self.write(MotorID, self.Adrress.GoalCurrent, np.abs(Goal_current))
```

