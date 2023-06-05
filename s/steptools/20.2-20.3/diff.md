# Comparing `tmp/steptools-20.2-cp37-abi3-win_amd64.whl.zip` & `tmp/steptools-20.3-cp37-abi3-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 7379375 bytes, number of entries: 8
+Zip file size: 7379502 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat        2 b- defN 22-Aug-19 14:38 steptools/py.typed
--rw-rw-rw-  2.0 fat 30931688 b- defN 23-May-26 00:34 steptools/step.pyd
--rw-rw-rw-  2.0 fat   120367 b- defN 23-May-25 18:36 steptools/step.pyi
--rw-rw-rw-  2.0 fat     3043 b- defN 23-May-26 00:34 steptools-20.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     7014 b- defN 23-May-26 00:34 steptools-20.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-May-26 00:34 steptools-20.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 23-May-26 00:34 steptools-20.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      620 b- defN 23-May-26 00:34 steptools-20.2.dist-info/RECORD
-8 files, 31062849 bytes uncompressed, 7378309 bytes compressed:  76.2%
+-rw-rw-rw-  2.0 fat 30932712 b- defN 23-Jun-05 17:47 steptools/step.pyd
+-rw-rw-rw-  2.0 fat   120834 b- defN 23-Jun-05 14:54 steptools/step.pyi
+-rw-rw-rw-  2.0 fat     3043 b- defN 23-Jun-05 17:47 steptools-20.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     7045 b- defN 23-Jun-05 17:47 steptools-20.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-05 17:47 steptools-20.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 23-Jun-05 17:47 steptools-20.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      620 b- defN 23-Jun-05 17:47 steptools-20.3.dist-info/RECORD
+8 files, 31064371 bytes uncompressed, 7378436 bytes compressed:  76.2%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: steptools/step.pyd
 Comment: 
 
 Filename: steptools/step.pyi
 Comment: 
 
-Filename: steptools-20.2.dist-info/LICENSE
+Filename: steptools-20.3.dist-info/LICENSE
 Comment: 
 
-Filename: steptools-20.2.dist-info/METADATA
+Filename: steptools-20.3.dist-info/METADATA
 Comment: 
 
-Filename: steptools-20.2.dist-info/WHEEL
+Filename: steptools-20.3.dist-info/WHEEL
 Comment: 
 
-Filename: steptools-20.2.dist-info/top_level.txt
+Filename: steptools-20.3.dist-info/top_level.txt
 Comment: 
 
-Filename: steptools-20.2.dist-info/RECORD
+Filename: steptools-20.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## steptools/step.pyi

```diff
@@ -20,82 +20,73 @@
     StrOrBytesPath
     )
 
 # ==================================================
 # MODULE FUNCTIONS
 #
 def keystone() -> Design:
-    '''
-    Return keystone schema design, initializes library.
-    '''
+    '''Return keystone schema design, initializes library.'''
     pass
 
-@overload    
-def verbose() -> bool: ...
-@overload    
-def verbose(yn: bool) -> None:
-    '''Get or set verbose flag'''
+def aim_type(obj: Object) -> str:
+    '''Return the AIM (EXPRESS) type of an object.'''
     pass
 
-def find_design(filename: StrOrBytesPath) -> Design:
-    '''
-    Read STEP file into memory, return design object.
-    '''
+def arm_type(obj: Object) -> str:
+    '''Return the ARM typename of an object.'''
     pass
 
 def type(obj: Object) -> str:
-    '''
-    Returns the AIM (EXPRESS) typename of an object.
-    '''
+    '''Returns the AIM (EXPRESS) typename of an object.'''
     pass
 
-def aim_type(obj: Object) -> str:
-    '''
-    Return the AIM (EXPRESS) type of an object.
-    '''
+def isinstance(obj: Object, typename: str) -> bool:
+    '''Test if object is instance of EXPRESS type.'''
     pass
 
-def arm_type(obj: Object) -> str:
+def new_project(name: str) -> Design:
     '''
-    Return the ARM typename of an object.
+    Create a new STEP-NC project for use with high level APIs, 
+    return design object containing it.
     '''
     pass
 
-def arm(obj: Object) -> ArmObject:
+def open_project(filename: StrOrBytesPath) -> Design:
     '''
-    Return the ARM object, if any, for a STEP data object.
+    Read STEP or STEP-NC file, do ARM recognition, set as the target of
+    the high level APIs and prepare any required indexes.  Return design
+    object.
     '''
     pass
 
-def arm_recognize(obj: Design) -> int:
+def save_project(
+        filename: StrOrBytesPath,
+        modules: bool = True,
+        xml: bool = False) -> None:
     '''
-    Recognize ARM objects in STEP data set, return count of ARM objects found.
+    Save current project as filename.  The modules flag groups the 
+    instances in the file by ARM concept.
     '''
     pass
 
-
-def isinstance(obj: Object, typename: str) -> bool:
+def find_design(filename: StrOrBytesPath) -> Design:
     '''
-    Is object an instance of EXPRESS type.
+    Read STEP file into memory if not already present and return design
+    object.  Does no ARM recognition.  Consider open_project() if using
+    high level APIs.
     '''
     pass
 
 @overload    
-def schema_type(d: Design) -> SchemaType: ...
+def verbose() -> bool: ...
 @overload    
-def schema_type(d: Design, schema: SchemaType) -> None:
-    '''Get or set design schema type enum'''
+def verbose(yn: bool) -> None:
+    '''Control printing of informational messages'''
     pass
 
-@overload    
-def schema_name(d: Design) -> str: ...
-@overload    
-def schema_name(d: Design, name: str) -> None:
-    '''Get or set design schema type name string'''
-    pass
 
 
 
 class SchemaType(IntEnum,auto):
     '''
     Identifies the STEP protocol that is declared in the header of an
     exchange file.
@@ -118,66 +109,98 @@
 #
 class Object:
     '''
     STEP data object class.  All ARM and EXPRESS AIM attributes in the
     underlying STEP data are automatically available.
 
     '''
+    def keys(self) -> Set[str]:
+        '''Get STEP ARM and AIM object attribute keys'''
+        pass
+
+    def aim(self) -> AimView:
+        '''Get STEP AIM object view'''
+        pass
+    
+    def arm(obj: Object) -> ArmObject:
+        '''Get STEP ARM object view, if any.'''
+        pass
+    
+    def design(self) -> Design:
+        '''Get the Design that owns an Object'''
+        pass
+
     @overload    
     def entity_id(self) -> int: ...
     @overload    
     def entity_id(self, id: int) -> None:
         '''Get or set exchange file entity id #123'''
         pass
 
-    def keys(self) -> Set[str]:
-        '''Get STEP ARM and AIM object attribute keys'''
-        pass
-    
-    def aim(self) -> AimView:
-        '''STEP AIM object view'''
-        pass
-
 
 # ==================================================
 # STEP DESIGN CLASS
 #
 class Design:
     '''
     Class containing all data from a STEP exchange file.
     '''
+    def arm_recognize(self) -> int:
+        '''
+        Recognize ARM concepts in STEP data set, return count of 
+        ARM objects found.
+        '''
+        pass
+
+    def find(self, id: str | int) -> Object:
+        '''Find an object by ANCHOR name or #123 entity id'''
+        pass
+    
+    def header_name(self) -> Object:
+        '''Get header name object'''
+        pass
+
+    def header_description(self) -> Object:
+        '''Get header description object'''
+        pass
+
+    def keys(self) -> Set[str]:
+        '''Design name table keys'''
+        pass
+    
     @overload    
     def name(self) -> str: ...
     @overload    
     def name(self, nm: StrOrBytesPath) -> None:
         '''Get or set design name'''
         pass
 
     @overload    
     def path(self) -> str: ...
     @overload    
     def path(self, nm: StrOrBytesPath) -> None:
         '''Get or set design file path'''
         pass
-    
-    def header_name(self) -> Object:
-        '''Get header name object'''
-        pass
 
-    def header_description(self) -> Object:
-        '''Get header description object'''
+    @overload    
+    def schema_type(self) -> SchemaType: ...
+    @overload    
+    def schema_type(self, schema: SchemaType) -> None:
+        '''Get or set design schema type enum'''
         pass
 
-    def find(self, id: str | int) -> Object:
-        '''Find an object by ANCHOR name or #123 entity id'''
+    @overload    
+    def schema_name(self) -> str: ...
+    @overload    
+    def schema_name(self, name: str) -> None:
+        '''Get or set design schema type name string'''
         pass
 
-    def keys() -> Set[str]:
-        '''Design name table keys'''
-        pass
+
+
 
 
 class DesignCursor(Iterator[Object]):
     '''
     Iterator over the STEP AIM instances in a design.
 
     '''
@@ -205,39 +228,40 @@
     
 class AimView:
     '''
     STEP AIM data object view class.  All EXPRESS AIM attributes in the
     underlying STEP data are automatically available.
 
     '''
+    def keys(self) -> Set[str]:
+        '''Get AIM object attribute keys'''
+        pass
+
     @overload    
     def entity_id(self) -> int: ...
     @overload    
     def entity_id(self, id: int) -> None:
         '''Get or set exchange file entity id #123'''
         pass
 
-    def keys(self) -> Set[str]:
-        '''Get AIM object attribute keys'''
-        pass
-
 
 class ArmObject:
     '''
     STEP ARM data object view class.  All ARM attributes in the
     underlying STEP data are automatically available.
 
     '''
-    def root(self) -> Object:
-        '''Get ARM root object'''
-        pass
     def keys(self) -> Set[str]:
         '''Get ARM object attribute keys'''
         pass
 
+    def root(self) -> Object:
+        '''Get ARM root object'''
+        pass
+
 
 # ==================================================
 # ADAPTIVE PROCESS CURSOR CLASS
 #
 # 
 class Unit(IntEnum,auto):
     '''Enumeration that identifies common units'''
@@ -2468,24 +2492,14 @@
         '''Create and return new workplan as the current workplan.'''
         pass
     
     @classmethod
     def nest_workplan_after(cls, name: str, index: int, plan: Object) -> Object:
         '''Create and return new workplan as the current workplan.'''
         pass
-    
-    @classmethod
-    def new_project(cls, name: str) -> Design:
-        '''Create a new project, return containing design.'''
-        pass
-
-    @classmethod
-    def open_project(cls, filename: StrOrBytesPath) -> Design:
-        '''Read STEP or STEP-NC file.'''
-        pass
 
     @classmethod
     def partno(cls, partname: str) -> None:
         '''Set part name in process.'''
         pass
 
     @classmethod
@@ -2529,21 +2543,14 @@
 
     @classmethod
     def retract_plane(cls, z_value: float) -> None:
         '''Set the Z value for the retract plane for the process.'''
         pass
 
     @classmethod
-    def save(cls, filename: StrOrBytesPath,
-             modules: bool = True,
-             xml: bool = False) -> None:
-        '''Save file as filename.  Modules flag groups instances by ARM object.'''
-        pass
-
-    @classmethod
     def set_make_display_messages(cls, yn: bool) -> None:
         '''Control whether certain APT commands are included as message NC functions.'''
         pass
 
     @classmethod
     def set_name(cls, obj: Object, name: str) -> None:
         '''Set name of STEP-NC data object.'''
@@ -2624,19 +2631,14 @@
     
 class FinderAPI:
     '''High level API for examining process contents'''
     @classmethod
     def design(cls) -> Design:
         '''Get the current design object.'''
         pass
-    @classmethod
-    def open_project(cls, filename: StrOrBytesPath) -> Design:
-        '''Read STEP or STEP-NC file.'''
-        pass
-
 
     @classmethod
     def get_probe_ball_radius(cls, ws_or_tool: Object) -> float:
         '''Get ball radius of probe tool.'''
         pass
     @classmethod
     def get_probe_ball_radius_unit(cls, ws_or_tool: Object) -> Unit:
@@ -2980,14 +2982,21 @@
         '''Get unit for vertical distance length of tool.'''
         pass
     
     def get_tool_workpiece(cls, ws_or_tool: Object) -> Object:
         '''Get workpiece that defines geometry of tool'''
         pass
 
+    def set_api_units(
+            cls,
+            system: Unit = UNKNOWN,
+            feed: Unit = UNKNOWN,
+            speed: Unit = UNKNOWN) -> None:
+        '''Set preference for returned units'''
+        pass
 
 
     
 # ==================================================
 # TOLERANCE API CLASS
 #
 class ToleranceAPI:
```

## Comparing `steptools-20.2.dist-info/LICENSE` & `steptools-20.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `steptools-20.2.dist-info/METADATA` & `steptools-20.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: steptools
-Version: 20.2
+Version: 20.3
 Summary: STEP and STEP-NC (ISO 10303) native extension for large CAD/CAM/CAE models and machine tool interfaces.
 Author-email: "STEP Tools, Inc" <support@steptools.com>
 License: 
         STEP Python Interface
         END USER LICENSE AGREEMENT
         REDISTRIBUTION NOT PERMITTED        
         STEP Tools, Inc. ("STI") grants you ("Customer") a non-exclusive,
@@ -64,15 +64,15 @@
 Classifier: Topic :: File Formats
 Classifier: Topic :: Multimedia :: Graphics :: 3D Modeling
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# STEP Python Interface
+# STEP Python Interface for Digital Twin Manufacturing
 
 The `steptools` package wraps the STEP Tools APIs with a Python
 interface for high-level operations on STEP-NC process descriptions
 and STEP assemblies.  It also provides STEP data classes and ARM
 concept indexes, previously only available in C++, for detailed work
 in areas not covered by the high-level operations.
```

