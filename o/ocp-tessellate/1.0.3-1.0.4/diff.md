# Comparing `tmp/ocp_tessellate-1.0.3.tar.gz` & `tmp/ocp_tessellate-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocp_tessellate-1.0.3.tar", last modified: Sun May  7 14:11:03 2023, max compression
+gzip compressed data, was "ocp_tessellate-1.0.4.tar", last modified: Mon Jun  5 20:14:58 2023, max compression
```

## Comparing `ocp_tessellate-1.0.3.tar` & `ocp_tessellate-1.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-05-07 14:11:03.857151 ocp_tessellate-1.0.3/
--rw-r--r--   0 bernhard   (501) staff       (20)      774 2023-05-07 14:11:03.857212 ocp_tessellate-1.0.3/PKG-INFO
--rw-r--r--   0 bernhard   (501) staff       (20)       17 2023-01-23 07:09:46.000000 ocp_tessellate-1.0.3/README.md
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-05-07 14:11:03.856296 ocp_tessellate-1.0.3/ocp_tessellate/
--rw-r--r--   0 bernhard   (501) staff       (20)     2926 2023-02-10 14:10:23.000000 ocp_tessellate-1.0.3/ocp_tessellate/__init__.py
--rw-r--r--   0 bernhard   (501) staff       (20)     1123 2023-05-07 13:49:09.000000 ocp_tessellate-1.0.3/ocp_tessellate/_version.py
--rw-r--r--   0 bernhard   (501) staff       (20)    12980 2023-04-15 16:48:19.000000 ocp_tessellate-1.0.3/ocp_tessellate/cad_objects.py
--rw-r--r--   0 bernhard   (501) staff       (20)    27059 2023-05-07 13:47:27.000000 ocp_tessellate-1.0.3/ocp_tessellate/convert.py
--rw-r--r--   0 bernhard   (501) staff       (20)    10515 2023-04-27 18:53:44.000000 ocp_tessellate-1.0.3/ocp_tessellate/defaults.py
--rw-r--r--   0 bernhard   (501) staff       (20)     1301 2023-02-10 14:10:23.000000 ocp_tessellate-1.0.3/ocp_tessellate/mp_tess.py
--rw-r--r--   0 bernhard   (501) staff       (20)     3033 2023-03-04 18:53:03.000000 ocp_tessellate-1.0.3/ocp_tessellate/mp_tessellator.py
--rw-r--r--   0 bernhard   (501) staff       (20)    19710 2023-04-07 11:30:03.000000 ocp_tessellate-1.0.3/ocp_tessellate/ocp_utils.py
--rw-r--r--   0 bernhard   (501) staff       (20)    13370 2023-04-22 09:22:57.000000 ocp_tessellate-1.0.3/ocp_tessellate/stepreader.py
--rw-r--r--   0 bernhard   (501) staff       (20)    13224 2023-04-22 15:51:39.000000 ocp_tessellate-1.0.3/ocp_tessellate/tessellator.py
--rw-r--r--   0 bernhard   (501) staff       (20)     6223 2023-04-27 16:19:21.000000 ocp_tessellate-1.0.3/ocp_tessellate/utils.py
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-05-07 14:11:03.857064 ocp_tessellate-1.0.3/ocp_tessellate.egg-info/
--rw-r--r--   0 bernhard   (501) staff       (20)      774 2023-05-07 14:11:03.000000 ocp_tessellate-1.0.3/ocp_tessellate.egg-info/PKG-INFO
--rw-r--r--   0 bernhard   (501) staff       (20)      561 2023-05-07 14:11:03.000000 ocp_tessellate-1.0.3/ocp_tessellate.egg-info/SOURCES.txt
--rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-05-07 14:11:03.000000 ocp_tessellate-1.0.3/ocp_tessellate.egg-info/dependency_links.txt
--rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-05-07 14:11:03.000000 ocp_tessellate-1.0.3/ocp_tessellate.egg-info/not-zip-safe
--rw-r--r--   0 bernhard   (501) staff       (20)      102 2023-05-07 14:11:03.000000 ocp_tessellate-1.0.3/ocp_tessellate.egg-info/requires.txt
--rw-r--r--   0 bernhard   (501) staff       (20)       15 2023-05-07 14:11:03.000000 ocp_tessellate-1.0.3/ocp_tessellate.egg-info/top_level.txt
--rw-r--r--   0 bernhard   (501) staff       (20)      671 2023-05-07 14:11:03.857461 ocp_tessellate-1.0.3/setup.cfg
--rw-r--r--   0 bernhard   (501) staff       (20)     1646 2023-05-07 13:49:09.000000 ocp_tessellate-1.0.3/setup.py
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-06-05 20:14:58.776888 ocp_tessellate-1.0.4/
+-rw-r--r--   0 bernhard   (501) staff       (20)      774 2023-06-05 20:14:58.776946 ocp_tessellate-1.0.4/PKG-INFO
+-rw-r--r--   0 bernhard   (501) staff       (20)       17 2023-02-04 10:28:52.000000 ocp_tessellate-1.0.4/README.md
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-06-05 20:14:58.775842 ocp_tessellate-1.0.4/ocp_tessellate/
+-rw-r--r--   0 bernhard   (501) staff       (20)     2926 2023-02-11 19:32:38.000000 ocp_tessellate-1.0.4/ocp_tessellate/__init__.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     1123 2023-06-05 20:14:48.000000 ocp_tessellate-1.0.4/ocp_tessellate/_version.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    12980 2023-04-23 07:18:10.000000 ocp_tessellate-1.0.4/ocp_tessellate/cad_objects.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    28124 2023-06-05 20:03:27.000000 ocp_tessellate-1.0.4/ocp_tessellate/convert.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    10515 2023-04-23 07:18:10.000000 ocp_tessellate-1.0.4/ocp_tessellate/defaults.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     1301 2023-02-11 19:32:38.000000 ocp_tessellate-1.0.4/ocp_tessellate/mp_tess.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     3033 2023-02-11 19:32:38.000000 ocp_tessellate-1.0.4/ocp_tessellate/mp_tessellator.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    19996 2023-06-05 19:58:43.000000 ocp_tessellate-1.0.4/ocp_tessellate/ocp_utils.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    13370 2023-04-23 10:15:07.000000 ocp_tessellate-1.0.4/ocp_tessellate/stepreader.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    13224 2023-04-23 10:15:07.000000 ocp_tessellate-1.0.4/ocp_tessellate/tessellator.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     6223 2023-04-29 10:55:18.000000 ocp_tessellate-1.0.4/ocp_tessellate/utils.py
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-06-05 20:14:58.776722 ocp_tessellate-1.0.4/ocp_tessellate.egg-info/
+-rw-r--r--   0 bernhard   (501) staff       (20)      774 2023-06-05 20:14:58.000000 ocp_tessellate-1.0.4/ocp_tessellate.egg-info/PKG-INFO
+-rw-r--r--   0 bernhard   (501) staff       (20)      561 2023-06-05 20:14:58.000000 ocp_tessellate-1.0.4/ocp_tessellate.egg-info/SOURCES.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-06-05 20:14:58.000000 ocp_tessellate-1.0.4/ocp_tessellate.egg-info/dependency_links.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-06-05 20:14:58.000000 ocp_tessellate-1.0.4/ocp_tessellate.egg-info/not-zip-safe
+-rw-r--r--   0 bernhard   (501) staff       (20)      102 2023-06-05 20:14:58.000000 ocp_tessellate-1.0.4/ocp_tessellate.egg-info/requires.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)       15 2023-06-05 20:14:58.000000 ocp_tessellate-1.0.4/ocp_tessellate.egg-info/top_level.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)      671 2023-06-05 20:14:58.777206 ocp_tessellate-1.0.4/setup.cfg
+-rw-r--r--   0 bernhard   (501) staff       (20)     1646 2023-06-05 20:14:48.000000 ocp_tessellate-1.0.4/setup.py
```

### Comparing `ocp_tessellate-1.0.3/PKG-INFO` & `ocp_tessellate-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocp_tessellate
-Version: 1.0.3
+Version: 1.0.4
 Summary: Tessellate OCP objects
 Home-page: https://github.com/bernhard-42/ocp-tessellate
 Author: Bernhard Walter
 Author-email: b_walter@arcor.de
 Keywords: CAD,cadquery
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
```

### Comparing `ocp_tessellate-1.0.3/ocp_tessellate/__init__.py` & `ocp_tessellate-1.0.4/ocp_tessellate/__init__.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.0.3/ocp_tessellate/_version.py` & `ocp_tessellate-1.0.4/ocp_tessellate/_version.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,9 +24,9 @@
     r = re.compile(
         r"(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)\-{0,1}(?P<release>\D*)(?P<build>\d*)"
     )
     major, minor, patch, release, build = r.match(version).groups()
     return VersionInfo(major, minor, patch, release, build)
 
 
-__version__ = "1.0.3"  # DO NOT EDIT THIS DIRECTLY!  It is managed by bumpversion
+__version__ = "1.0.4"  # DO NOT EDIT THIS DIRECTLY!  It is managed by bumpversion
 __version_info__ = get_version(__version__)
```

### Comparing `ocp_tessellate-1.0.3/ocp_tessellate/cad_objects.py` & `ocp_tessellate-1.0.4/ocp_tessellate/cad_objects.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.0.3/ocp_tessellate/convert.py` & `ocp_tessellate-1.0.4/ocp_tessellate/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,40 +32,44 @@
 from .mp_tessellator import get_mp_result, is_apply_result
 from .ocp_utils import (
     BoundingBox,
     copy_shape,
     downcast,
     get_downcasted_shape,
     get_edges,
+    get_faces,
     get_location,
     get_rgba,
     get_tshape,
     get_tlocation,
     get_tuple,
     identity_location,
     is_build123d_assembly,
     is_build123d_compound,
     is_build123d_shape,
+    is_build123d_shell,
     is_build123d,
     is_cadquery_assembly,
     is_cadquery_massembly,
     is_cadquery_sketch,
     is_cadquery,
     is_compound,
     is_mixed_compound,
     is_edge_list,
     is_face_list,
     is_compound_list,
     is_solid_list,
+    is_shell_list,
     is_toploc_location,
     is_topods_compound,
     is_topods_edge,
     is_topods_face,
     is_topods_shape,
     is_topods_solid,
+    is_topods_shell,
     is_topods_vertex,
     is_topods_wire,
     is_vector,
     is_vertex_list,
     is_wire_list,
     is_wrapped,
     make_compound,
@@ -247,14 +251,21 @@
         _debug(f"        conv: build123d Builder {type(cad_obj)}")
         cad_obj = getattr(cad_obj, cad_obj._obj_name)  # convert to direct API
 
     if is_build123d_compound(cad_obj):
         _debug(f"        conv: build123d Compound {type(cad_obj)}")
         cad_objs = [cad_obj.wrapped]
 
+    elif is_build123d_shell(cad_obj):
+        _debug(f"        conv: build123d Shell {type(cad_obj)}")
+        cad_objs = []
+        obj_name = "Shell" if obj_name is None else obj_name
+        for obj in cad_obj.faces():
+            cad_objs += get_downcasted_shape(obj.wrapped)
+
     elif is_build123d_shape(cad_obj):
         _debug(f"        conv: build123d Shape {type(cad_obj)}")
         cad_objs = get_downcasted_shape(cad_obj.wrapped)
 
     elif is_cadquery_sketch(cad_obj):
         _debug("        conv: cadquery sketch")
         cad_objs = conv_sketch(cad_obj)
@@ -313,14 +324,25 @@
         _debug("          conv: solid_list")
         return OCP_Part(
             cad_objs,
             name=get_name(obj_name, cad_objs, "Solid", "Solids"),
             color=get_rgba(obj_color, obj_alpha, Color(default_color)),
         )
 
+    elif is_shell_list(cad_objs):
+        _debug("          conv: shell_list")
+        faces = []
+        for shell in cad_objs:
+            faces += list(get_faces(shell))
+        return OCP_Faces(
+            faces,
+            name=get_name(obj_name, cad_objs, "Shell", "Shells"),
+            color=get_rgba(obj_color, obj_alpha, Color(FACE_COLOR)),
+        )
+
     elif is_face_list(cad_objs):
         _debug("          conv: face_list")
         return OCP_Faces(
             cad_objs,
             name=get_name(obj_name, cad_objs, "Face", "Faces"),
             color=get_rgba(obj_color, obj_alpha, Color(FACE_COLOR)),
         )
@@ -650,14 +672,17 @@
                             part.objects[0].loc = part.loc
                         else:
                             part.objects[0].loc = part.loc * part.objects[0].loc
                         pg2.add(part.objects[0])
                     else:
                         pg2.add(part)
 
+                names = make_unique([obj.name for obj in pg2.objects])
+                for name, obj in zip(names, pg2.objects):
+                    obj.name = name
                 pg.add(pg2)
 
             elif is_mixed_compound(cad_obj):
                 _debug("  to_assembly: mixed compound", obj_name)
                 for child in cad_obj:
                     part = conv(child.wrapped, obj_name, color, alpha)
                     pg.add(part)
@@ -767,15 +792,18 @@
                 part = get_instance(cad_obj, obj_name, rgba, instances, progress)
                 if obj_name is None:
                     part.name = get_object_name(part)
 
                 pg.add(part)
 
             elif isinstance(cad_obj, OCP_PartGroup):
-                pg = cad_obj
+                names = make_unique([obj.name for obj in cad_obj.objects])
+                for name, obj in zip(names, cad_obj.objects):
+                    obj.name = name
+                pg.add(cad_obj)
 
             elif isinstance(cad_obj, (OCP_Faces, OCP_Edges, OCP_Vertices)):
                 pg.add(cad_obj)
 
             else:
                 part = conv(cad_obj, obj_name, color, alpha)
                 if part.name is None:
```

### Comparing `ocp_tessellate-1.0.3/ocp_tessellate/defaults.py` & `ocp_tessellate-1.0.4/ocp_tessellate/defaults.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.0.3/ocp_tessellate/mp_tess.py` & `ocp_tessellate-1.0.4/ocp_tessellate/mp_tess.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.0.3/ocp_tessellate/mp_tessellator.py` & `ocp_tessellate-1.0.4/ocp_tessellate/mp_tessellator.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.0.3/ocp_tessellate/ocp_utils.py` & `ocp_tessellate-1.0.4/ocp_tessellate/ocp_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,15 @@
     TopoDS,
     TopoDS_Builder,
     TopoDS_Compound,
     TopoDS_Edge,
     TopoDS_Face,
     TopoDS_Shape,
     TopoDS_Solid,
+    TopoDS_Shell,
     TopoDS_Vertex,
     TopoDS_Wire,
 )
 from quaternion import rotate_vectors
 
 from .utils import Color, distance
 
@@ -161,14 +162,18 @@
     return _has(obj, ["_obj", "_obj_name"])
 
 
 def is_build123d_shape(obj):
     return _has(obj, ["wrapped", "children"])
 
 
+def is_build123d_shell(obj):
+    return hasattr(obj, "wrapped") and is_topods_shell(obj.wrapped)
+
+
 def is_build123d_compound(obj):
     return is_build123d_shape(obj) and isinstance(obj, Iterable)
 
 
 def is_build123d_assembly(obj):
     return (
         (is_build123d_compound(obj) or is_build123d_shape(obj))
@@ -519,15 +524,15 @@
     elif next(get_edges(shape), None) is not None:
         objs = get_edges(shape)
 
     elif next(get_vertices(shape), None) is not None:
         objs = get_vertices(shape)
 
     else:
-        raise NotImplementedError("Unknow TopoDS Compound")
+        raise ValueError("Compound is empty")
 
     return [downcast(obj) for obj in objs]
 
 
 # Check TopLoc_Location
 
 
@@ -546,14 +551,18 @@
     return isinstance(topods_shape, TopoDS_Compound)
 
 
 def is_topods_solid(topods_shape):
     return isinstance(topods_shape, TopoDS_Solid)
 
 
+def is_topods_shell(topods_shape):
+    return isinstance(topods_shape, TopoDS_Shell)
+
+
 def is_topods_face(topods_shape):
     return isinstance(topods_shape, TopoDS_Face)
 
 
 def is_topods_wire(topods_shape):
     return isinstance(topods_shape, TopoDS_Wire)
 
@@ -570,14 +579,18 @@
     return all([is_topods_compound(obj) for obj in topods_list])
 
 
 def is_solid_list(topods_list):
     return all([is_topods_solid(obj) for obj in topods_list])
 
 
+def is_shell_list(topods_list):
+    return all([is_topods_shell(obj) for obj in topods_list])
+
+
 def is_face_list(topods_list):
     return all([is_topods_face(obj) for obj in topods_list])
 
 
 def is_wire_list(topods_list):
     return all([is_topods_wire(obj) for obj in topods_list])
```

### Comparing `ocp_tessellate-1.0.3/ocp_tessellate/stepreader.py` & `ocp_tessellate-1.0.4/ocp_tessellate/stepreader.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.0.3/ocp_tessellate/tessellator.py` & `ocp_tessellate-1.0.4/ocp_tessellate/tessellator.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.0.3/ocp_tessellate/utils.py` & `ocp_tessellate-1.0.4/ocp_tessellate/utils.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.0.3/ocp_tessellate.egg-info/PKG-INFO` & `ocp_tessellate-1.0.4/ocp_tessellate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocp-tessellate
-Version: 1.0.3
+Version: 1.0.4
 Summary: Tessellate OCP objects
 Home-page: https://github.com/bernhard-42/ocp-tessellate
 Author: Bernhard Walter
 Author-email: b_walter@arcor.de
 Keywords: CAD,cadquery
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
```

### Comparing `ocp_tessellate-1.0.3/ocp_tessellate.egg-info/SOURCES.txt` & `ocp_tessellate-1.0.4/ocp_tessellate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.0.3/setup.cfg` & `ocp_tessellate-1.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.0.3
+current_version = 1.0.4
 commit = False
 tag = False
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?P<release>\D*)(?P<build>\d*)
 serialize = 
 	{major}.{minor}.{patch}{release}{build}
 	{major}.{minor}.{patch}
```

### Comparing `ocp_tessellate-1.0.3/setup.py` & `ocp_tessellate-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 LONG_DESCRIPTION = (
     "Tessellate OCP (https://github.com/cadquery/OCP) objects to use with threejs"
 )
 
 setup_args = {
     "name": "ocp_tessellate",
-    "version": "1.0.3",
+    "version": "1.0.4",
     "description": "Tessellate OCP objects",
     "long_description": LONG_DESCRIPTION,
     "include_package_data": True,
     "python_requires": ">=3.9",
     "install_requires": [
         "webcolors~=1.12",
         "numpy",
```

