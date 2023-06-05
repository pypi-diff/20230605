# Comparing `tmp/pyclpu-0.1.0.tar.gz` & `tmp/pyclpu-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyclpu-0.1.0.tar", last modified: Fri Jun  2 09:57:51 2023, max compression
+gzip compressed data, was "dist\pyclpu-0.1.2.tar", last modified: Mon Jun  5 18:16:42 2023, max compression
```

## Comparing `pyclpu-0.1.0.tar` & `pyclpu-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 09:57:51.000000 pyclpu-0.1.0/
--rw-rw-rw-   0        0        0      382 2023-06-02 09:57:51.000000 pyclpu-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-02 09:57:51.000000 pyclpu-0.1.0/pyclpu/
--rw-rw-rw-   0        0        0     1878 2023-06-01 14:29:35.000000 pyclpu-0.1.0/pyclpu/constants.py
--rw-rw-rw-   0        0        0      942 2022-04-16 17:02:37.000000 pyclpu-0.1.0/pyclpu/formats.py
--rw-rw-rw-   0        0        0    19125 2023-06-02 09:47:41.000000 pyclpu-0.1.0/pyclpu/image.py
--rw-rw-rw-   0        0        0    30733 2023-05-31 09:32:25.000000 pyclpu-0.1.0/pyclpu/main.py
--rw-rw-rw-   0        0        0     7425 2022-04-16 17:02:37.000000 pyclpu-0.1.0/pyclpu/s33293804.py
--rw-rw-rw-   0        0        0      629 2023-06-02 08:58:53.000000 pyclpu-0.1.0/pyclpu/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 09:57:51.000000 pyclpu-0.1.0/pyclpu.egg-info/
--rw-rw-rw-   0        0        0        1 2023-06-02 09:57:51.000000 pyclpu-0.1.0/pyclpu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      382 2023-06-02 09:57:51.000000 pyclpu-0.1.0/pyclpu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       51 2023-06-02 09:57:51.000000 pyclpu-0.1.0/pyclpu.egg-info/requires.txt
--rw-rw-rw-   0        0        0      285 2023-06-02 09:57:51.000000 pyclpu-0.1.0/pyclpu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-06-02 09:57:51.000000 pyclpu-0.1.0/pyclpu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2558 2023-06-02 09:30:25.000000 pyclpu-0.1.0/README.md
--rw-rw-rw-   0        0        0       92 2023-06-02 09:57:51.000000 pyclpu-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1827 2023-06-02 09:41:36.000000 pyclpu-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 18:16:42.000000 pyclpu-0.1.2/
+-rw-rw-rw-   0        0        0     1082 2023-06-02 09:58:39.000000 pyclpu-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     4942 2023-06-05 18:16:42.000000 pyclpu-0.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-05 18:16:42.000000 pyclpu-0.1.2/pyclpu/
+-rw-rw-rw-   0        0        0     1878 2023-06-02 09:58:39.000000 pyclpu-0.1.2/pyclpu/constants.py
+-rw-rw-rw-   0        0        0      942 2023-06-02 09:58:39.000000 pyclpu-0.1.2/pyclpu/formats.py
+-rw-rw-rw-   0        0        0    17586 2023-06-05 18:10:54.000000 pyclpu-0.1.2/pyclpu/image.py
+-rw-rw-rw-   0        0        0    30733 2023-06-02 09:58:39.000000 pyclpu-0.1.2/pyclpu/main.py
+-rw-rw-rw-   0        0        0    11328 2023-06-05 15:34:37.000000 pyclpu-0.1.2/pyclpu/manager.py
+-rw-rw-rw-   0        0        0     7425 2023-06-02 09:58:39.000000 pyclpu-0.1.2/pyclpu/s33293804.py
+-rw-rw-rw-   0        0        0      629 2023-06-05 18:14:49.000000 pyclpu-0.1.2/pyclpu/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 18:16:42.000000 pyclpu-0.1.2/pyclpu.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-06-05 18:16:42.000000 pyclpu-0.1.2/pyclpu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     4942 2023-06-05 18:16:42.000000 pyclpu-0.1.2/pyclpu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       51 2023-06-05 18:16:42.000000 pyclpu-0.1.2/pyclpu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      311 2023-06-05 18:16:42.000000 pyclpu-0.1.2/pyclpu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-06-05 18:16:42.000000 pyclpu-0.1.2/pyclpu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4512 2023-06-05 18:16:30.000000 pyclpu-0.1.2/README.md
+-rw-rw-rw-   0        0        0       92 2023-06-05 18:16:42.000000 pyclpu-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     2090 2023-06-02 13:14:02.000000 pyclpu-0.1.2/setup.py
```

### Comparing `pyclpu-0.1.0/pyclpu/constants.py` & `pyclpu-0.1.2/pyclpu/constants.py`

 * *Files identical despite different names*

### Comparing `pyclpu-0.1.0/pyclpu/formats.py` & `pyclpu-0.1.2/pyclpu/formats.py`

 * *Files identical despite different names*

### Comparing `pyclpu-0.1.0/pyclpu/image.py` & `pyclpu-0.1.2/pyclpu/image.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 
 interpreter         python > 3.5
 version control     git
 
 requires explicitely {
  - os
  - sys
- - warnings
- - math
  - numpy
+ - cv2
+ - PIL
 }
 
 import after installation of pyclpu via {
   from pyclpu import image
 }
 
 import without installation via {
@@ -54,31 +54,33 @@
 
 # INTERNAL
 root = os.path.dirname(os.path.abspath(getsourcefile(lambda:0))) # get environment
 sys.path.append(os.path.abspath(root))                           # add environment
 sys.path.append(os.path.abspath(root)+os.path.sep+"LIB")         # add library
 
 if "constants" not in globals() or globals()['constants'] == False:
-    import constants            # import all global constants from                   constants.py
-    import formats              # import all global formats from                     formats.py
-    from s33293804 import *     # import zoom PanZoomWindow for display images from  s33293804.py
+    import constants                        # import all global constants from                   constants.py
+    import formats                          # import all global formats from                     formats.py
+    from manager import error               # import error() from management                     manager.py
+    from manager import message             # import message() from management                   manager.py
+    from manager import warning             # import warning() from management                   manager.py
+    from manager import give_extension      # import give_extension() from management            manager.py
+    from s33293804 import *                 # import zoom PanZoomWindow for display images from  s33293804.py
     reload(constants)
     reload(formats)
 
 # STYLE
 
 # =============================================================================
 # CONSTANTS
 # =============================================================================
 # INTEGRATION AND TESTING
 test = True
 
-# HELPER PARAMETERS
-global_list = []
-global_bool = False
+# PARAMETERS
 
 # METHODOLOGY SELECTORS
 # define method used to load images, 
 # possible values are
 # opencv   :: use the module opencv
 # tifffile :: use the module tifffile # !!! tifffile not part of the project !!!
 global_load_method = 'opencv'
@@ -97,74 +99,14 @@
         for arg in args:
             print(arg)
         for key, value in kwargs.items():
             print(str(key) + " : "+ str(value))
     except:
         return False
     return True
-    
-# MANAGEMENT
-def error(source,string,code = None):
-    print("\nError ............. "+source+" : "+string)
-    lead_string = "                    "
-    intend_string = "      "
-    if code != None:
-        if code == 0:
-            print(lead_string+'ERROR_DIVISION_BY_ZERO\n'+intend_string+'The system cannot divide by zero.')
-        elif code == 2:
-            print(lead_string+'ERROR_FILE_NOT_FOUND\n'+intend_string+'The system cannot find the file specified.')
-        elif code == 5:
-            print(lead_string+'ERROR_ACCESS_DENIED\n'+intend_string+'Access is denied.')
-        elif code == 13:
-            print(lead_string+'ERROR_INVALID_DATA\n'+intend_string+'The data is invalid.')
-        elif code == 161:    
-            print(lead_string+'ERROR_BAD_PATHNAME\n'+intend_string+'The specified path is invalid.')
-        elif code == 232:
-            print(lead_string+'ERROR_NO_DATA\n'+intend_string+'The pipe is being closed.')
-        elif code == 677:
-            print(lead_string+'ERROR_EXTRANEOUS_INFORMATION\n'+intend_string+'Too Much Information.')
-        elif code == 1160:
-            print(lead_string+'ERROR_SOURCE_ELEMENT_EMPTY\n'+intend_string+'The indicated source element has no media.')
-        elif code == 1169:
-            print(lead_string+'ERROR_NO_MATCH\n'+intend_string+'There was no match for the specified key in the index.')
-        elif code == 1287:
-            print(lead_string+'ERROR_UNIDENTIFIED_ERROR\n'+intend_string+'Insufficient information exists to identify the cause of failure.')
-        elif code == 8322:
-            print(lead_string+'ERROR_DS_RANGE_CONSTRAINT\n'+intend_string+'A value for the attribute was not in the acceptable range of values.')
-        else:
-            print('ERROR\nNo idea what happened.\n')
-    print("\n")
-    return None
-    
-def message(source,string,headline = ""):
-    print("\nMessage ........... "+source+" :")
-    lead_string = "                    "
-    if headline != "": print(lead_string+headline)
-    intend_string = "      "
-    string_list = string.split("\n")
-    for s in string_list:
-        print(intend_string + s)
-    return None
-
-def warning(source,string):
-    try:
-        print("\nWarning ........... "+source+" : "+string+"\n")
-    except:
-        error(warning.__name__,"Fail to print.")
-    return None
-    
-def give_extension(filename):
-    """
-    Function returns extension of a filename as string or `None`.
-    """
-    try:
-        extension = filename.rsplit(".",1)[1]
-    except:
-        extension = None
-    return extension
 
 # IMAGE T/I/O
 def isimg(path):
     global global_load_method
     try:
         extension = give_extension(path)
         if extension in formats.acceptedinput[global_load_method]:
@@ -371,15 +313,19 @@
 
     ```
     from pyclpu import image
 
     warp = image.PerspectiveTransform(source = image.imread("path/to/test.jpg")) 
     ```
 
-    with the warped image in `warp.warped` and the coordinates of cornes from the source image stored in `sourcecorners`. Note that the source image is not part of the object in its final form. A more object oriented use case can deal with loops where all warps have the same source corner coordinates
+    with output
+    - the warped image in `warp.warped` and 
+    - the coordinates of cornes from the source image stored in `warp.sourcecorners`.
+
+    Note that the source image is not part of the object in its final form. The coordinates of the corner points of the target rectangle can also be parsed to the function as `np.array()` of shape `(4,2)` with the keyword `sourcecorners`. A more object oriented use case can deal with loops where all warps have the same source corner coordinates
 
     ```
     from pyclpu import image
 
     warp_it = image.PerspectiveTransform()
 
     image_stack = image.imread(path/to/directory/with/many/images/)
@@ -387,24 +333,26 @@
     warp = []
 
     for image in image_stack:
         warp_it.source = image
         warp.append[{"warped" : warp.warped, "sourcecorners" : warp.sourcecorners}]
     ```
 
-    with results beeing stored in a list `warp`.
+    with results beeing stored in a list `warp`. The dynamic modification of `warp.sourcecorners` is possible.
     """
     # INI
     def __new__(cls, *args, **kwargs):
         return super().__new__(cls)
     def __init__(self, *args, **kwargs):
         self.__dict__.update(kwargs)
         # INTEGRITY
         if not hasattr(self, 'source'):
             warning(self.__class__.__name__,"No source image `IMG` defined, expect key `source` as `source=IMG`.")
+        if not hasattr(self, 'sourcecorners'):
+            warning(self.__class__.__name__,"Found no corners (x,y) of target rectangle, optional key `sourcecorners` as `sourcecorners=np.array((4,2),dtype='int')`.")
         # IN PLACE
         if hasattr(self, 'source'):
             self.__run__()
         return None
     def __setattr__(self, name, value):
         super().__setattr__(name, value)
         if name == "source":
@@ -446,15 +394,17 @@
                 [0, maxHeight - 1]], dtype = "float32")
             # compute perspective transform matrix and apply it
             M = cv2.getPerspectiveTransform(rect, dst)
             warped = cv2.warpPerspective(image, M, (maxWidth, maxHeight))
             # return the warped image
             return warped    
         # MAIN
-        self.sourcecorners = PointPicker(image=self.source,n=4)
+        if not hasattr(self,'sourcecorners'):
+            warning(self.__class__.__name__,"Found no corners of target rectangle, open interactive dialogue to pick them.")
+            self.sourcecorners = PointPicker(image=self.source,n=4)
         self.warped = four_point_transform(self.source, self.sourcecorners.point_list)
         message(self.__class__.__name__,"PRESS ANY KEY TO CLOSE IMAGE AND PROCEED",headline="DISPLAY WARP")
         cv2.namedWindow(self.__class__.__name__)
         cv2.imshow(self.__class__.__name__, self.warped)
         cv2.waitKey(0)
         # housekeeping
         cv2.destroyAllWindows()
```

### Comparing `pyclpu-0.1.0/pyclpu/main.py` & `pyclpu-0.1.2/pyclpu/main.py`

 * *Files identical despite different names*

### Comparing `pyclpu-0.1.0/pyclpu/s33293804.py` & `pyclpu-0.1.2/pyclpu/s33293804.py`

 * *Files identical despite different names*

### Comparing `pyclpu-0.1.0/pyclpu/__init__.py` & `pyclpu-0.1.2/pyclpu/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 pyclpu.
 
 CLPU Utilities.
 """
 # main attributes
-__version__ = "0.1.0"
+__version__ = "0.1.2"
 __author__ = 'Michael Ehret'
 __credits__ = 'Centro de Laseres Pulsados, Villamayor, Spain'
 
 """
 DEVELOPMENT ZONE
 
 Until the following is not resolved, attributes below __init__.py require manual import as from pyclpu import ATTRIBUTE
```

### Comparing `pyclpu-0.1.0/setup.py` & `pyclpu-0.1.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -38,17 +38,24 @@
 
 # credits to https://betterscientificsoftware.github.io/python-for-hpc/tutorials/python-pypi-packaging/
 
 from setuptools import setup
 
 import glob
 
+# read the contents of README file
+from pathlib import Path
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
+
 setup(\
     name="pyclpu",\
     description='CLPU Utilities',\
+    long_description = long_description,\
+    long_description_content_type='text/markdown',\
     author='Michael Ehret',\
     author_email='mehret@clpu.es',\
     url='https://git.clpu.es/mehret/pyclpu',\
     license='MIT',\
     packages=['pyclpu'],
     scripts=glob.glob("pyclpu/*.py"),
     install_requires=[\
```

