# Comparing `tmp/easyvec-0.0.8.tar.gz` & `tmp/easyvec-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\easyvec-0.0.8.tar", last modified: Mon Feb 24 18:45:21 2020, max compression
+gzip compressed data, was "dist\easyvec-0.0.9.tar", last modified: Mon Feb 24 20:01:58 2020, max compression
```

## Comparing `easyvec-0.0.8.tar` & `easyvec-0.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2020-02-24 18:45:21.000000 easyvec-0.0.8/
--rw-rw-rw-   0        0        0     1073 2020-02-08 12:57:32.000000 easyvec-0.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0      130 2020-02-08 15:04:13.000000 easyvec-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     1457 2020-02-24 18:45:21.000000 easyvec-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0        9 2020-02-08 12:58:45.000000 easyvec-0.0.8/README.md
--rw-rw-rw-   0        0        0       46 2020-02-09 10:31:37.000000 easyvec-0.0.8/requirements-dev.txt
--rw-rw-rw-   0        0        0       14 2020-02-08 14:51:41.000000 easyvec-0.0.8/requirements.txt
--rw-rw-rw-   0        0        0     1404 2020-02-24 18:45:21.000000 easyvec-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1809 2020-02-18 17:41:21.000000 easyvec-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2020-02-24 18:45:21.000000 easyvec-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2020-02-24 18:45:21.000000 easyvec-0.0.8/src/easyvec/
--rw-rw-rw-   0        0        0       98 2020-02-19 18:05:09.000000 easyvec-0.0.8/src/easyvec/__init__.py
--rw-rw-rw-   0        0        0  1563588 2020-02-24 18:42:57.000000 easyvec-0.0.8/src/easyvec/geometry.cpp
--rw-rw-rw-   0        0        0   782609 2020-02-24 18:42:58.000000 easyvec-0.0.8/src/easyvec/geometry.html
--rw-rw-rw-   0        0        0     2256 2020-02-24 14:41:16.000000 easyvec-0.0.8/src/easyvec/geometry.pxd
--rw-rw-rw-   0        0        0    22422 2020-02-24 18:42:36.000000 easyvec-0.0.8/src/easyvec/geometry.pyx
--rw-rw-rw-   0        0        0  1289704 2020-02-24 18:42:07.000000 easyvec-0.0.8/src/easyvec/matrixes.cpp
--rw-rw-rw-   0        0        0   544529 2020-02-24 18:42:07.000000 easyvec-0.0.8/src/easyvec/matrixes.html
--rw-rw-rw-   0        0        0     1318 2020-02-12 11:42:34.000000 easyvec-0.0.8/src/easyvec/matrixes.pxd
--rw-rw-rw-   0        0        0    15345 2020-02-23 16:36:57.000000 easyvec-0.0.8/src/easyvec/matrixes.pyx
--rw-rw-rw-   0        0        0  3016377 2020-02-24 18:42:10.000000 easyvec-0.0.8/src/easyvec/vectors.cpp
--rw-rw-rw-   0        0        0  2472508 2020-02-24 18:42:10.000000 easyvec-0.0.8/src/easyvec/vectors.html
--rw-rw-rw-   0        0        0     5330 2020-02-24 13:59:35.000000 easyvec-0.0.8/src/easyvec/vectors.pxd
--rw-rw-rw-   0        0        0    33734 2020-02-24 14:01:02.000000 easyvec-0.0.8/src/easyvec/vectors.pyx
-drwxrwxrwx   0        0        0        0 2020-02-24 18:45:21.000000 easyvec-0.0.8/src/easyvec.egg-info/
--rw-rw-rw-   0        0        0     1457 2020-02-24 18:45:21.000000 easyvec-0.0.8/src/easyvec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      695 2020-02-24 18:45:21.000000 easyvec-0.0.8/src/easyvec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-02-24 18:45:21.000000 easyvec-0.0.8/src/easyvec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2020-02-24 18:42:23.000000 easyvec-0.0.8/src/easyvec.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       91 2020-02-24 18:45:21.000000 easyvec-0.0.8/src/easyvec.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2020-02-24 18:45:21.000000 easyvec-0.0.8/src/easyvec.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2020-02-24 20:01:58.000000 easyvec-0.0.9/
+-rw-rw-rw-   0        0        0     1073 2020-02-08 12:57:32.000000 easyvec-0.0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0      130 2020-02-08 15:04:13.000000 easyvec-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1457 2020-02-24 20:01:58.000000 easyvec-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0        9 2020-02-08 12:58:45.000000 easyvec-0.0.9/README.md
+-rw-rw-rw-   0        0        0       46 2020-02-09 10:31:37.000000 easyvec-0.0.9/requirements-dev.txt
+-rw-rw-rw-   0        0        0       14 2020-02-08 14:51:41.000000 easyvec-0.0.9/requirements.txt
+-rw-rw-rw-   0        0        0     1404 2020-02-24 20:01:58.000000 easyvec-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1809 2020-02-18 17:41:21.000000 easyvec-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2020-02-24 20:01:58.000000 easyvec-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2020-02-24 20:01:58.000000 easyvec-0.0.9/src/easyvec/
+-rw-rw-rw-   0        0        0       98 2020-02-19 18:05:09.000000 easyvec-0.0.9/src/easyvec/__init__.py
+-rw-rw-rw-   0        0        0  1578976 2020-02-24 20:01:37.000000 easyvec-0.0.9/src/easyvec/geometry.cpp
+-rw-rw-rw-   0        0        0   803299 2020-02-24 20:01:37.000000 easyvec-0.0.9/src/easyvec/geometry.html
+-rw-rw-rw-   0        0        0     2256 2020-02-24 14:41:16.000000 easyvec-0.0.9/src/easyvec/geometry.pxd
+-rw-rw-rw-   0        0        0    22758 2020-02-24 20:00:38.000000 easyvec-0.0.9/src/easyvec/geometry.pyx
+-rw-rw-rw-   0        0        0  1289704 2020-02-24 20:01:38.000000 easyvec-0.0.9/src/easyvec/matrixes.cpp
+-rw-rw-rw-   0        0        0   544529 2020-02-24 20:01:38.000000 easyvec-0.0.9/src/easyvec/matrixes.html
+-rw-rw-rw-   0        0        0     1318 2020-02-12 11:42:34.000000 easyvec-0.0.9/src/easyvec/matrixes.pxd
+-rw-rw-rw-   0        0        0    15345 2020-02-23 16:36:57.000000 easyvec-0.0.9/src/easyvec/matrixes.pyx
+-rw-rw-rw-   0        0        0  3016377 2020-02-24 20:01:41.000000 easyvec-0.0.9/src/easyvec/vectors.cpp
+-rw-rw-rw-   0        0        0  2472508 2020-02-24 20:01:41.000000 easyvec-0.0.9/src/easyvec/vectors.html
+-rw-rw-rw-   0        0        0     5330 2020-02-24 13:59:35.000000 easyvec-0.0.9/src/easyvec/vectors.pxd
+-rw-rw-rw-   0        0        0    33734 2020-02-24 14:01:02.000000 easyvec-0.0.9/src/easyvec/vectors.pyx
+drwxrwxrwx   0        0        0        0 2020-02-24 20:01:58.000000 easyvec-0.0.9/src/easyvec.egg-info/
+-rw-rw-rw-   0        0        0     1457 2020-02-24 20:01:57.000000 easyvec-0.0.9/src/easyvec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      695 2020-02-24 20:01:57.000000 easyvec-0.0.9/src/easyvec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2020-02-24 20:01:57.000000 easyvec-0.0.9/src/easyvec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2020-02-24 20:01:54.000000 easyvec-0.0.9/src/easyvec.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       91 2020-02-24 20:01:57.000000 easyvec-0.0.9/src/easyvec.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2020-02-24 20:01:57.000000 easyvec-0.0.9/src/easyvec.egg-info/top_level.txt
```

### Comparing `easyvec-0.0.8/LICENSE.txt` & `easyvec-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `easyvec-0.0.8/PKG-INFO` & `easyvec-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyvec
-Version: 0.0.8
+Version: 0.0.9
 Summary: Vector library
 Home-page: https://github.com/TovarnovM/easyvec
 Author: Mikhail Tovarnov
 Author-email: mtovarnov@mail.com
 License: MIT
 Project-URL: Documentation, https://github.com/TovarnovM/easyvec
 Project-URL: Code, https://github.com/TovarnovM/easyvec
```

### Comparing `easyvec-0.0.8/setup.cfg` & `easyvec-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 6173 7976 6563 0d0a 7665 7273   = easyvec..vers
-00000020: 696f 6e20 3d20 302e 302e 380d 0a64 6573  ion = 0.0.8..des
+00000020: 696f 6e20 3d20 302e 302e 390d 0a64 6573  ion = 0.0.9..des
 00000030: 6372 6970 7469 6f6e 203d 2056 6563 746f  cription = Vecto
 00000040: 7220 6c69 6272 6172 790d 0a6c 6f6e 675f  r library..long_
 00000050: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
 00000060: 6c65 3a20 5245 4144 4d45 2e6d 640d 0a6c  le: README.md..l
 00000070: 6f6e 675f 6465 7363 7269 7074 696f 6e5f  ong_description_
 00000080: 636f 6e74 656e 745f 7479 7065 203d 2074  content_type = t
 00000090: 6578 742f 6d61 726b 646f 776e 0d0a 6c69  ext/markdown..li
```

### Comparing `easyvec-0.0.8/setup.py` & `easyvec-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `easyvec-0.0.8/src/easyvec/geometry.cpp` & `easyvec-0.0.9/src/easyvec/geometry.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1128,16 +1128,16 @@
  * 
  * 
  */
 struct __pyx_opt_args_7easyvec_7vectors_4Vec2_rotate {
   int __pyx_n;
   int degrees;
 };
-struct __pyx_ctuple_d78dc__int__and___dunderpyx_t_7easyvec_7vectors_real__and___dunderpyx_t_7easyvec_7vectors_real__etc;
-typedef struct __pyx_ctuple_d78dc__int__and___dunderpyx_t_7easyvec_7vectors_real__and___dunderpyx_t_7easyvec_7vectors_real__etc __pyx_ctuple_d78dc__int__and___dunderpyx_t_7easyvec_7vectors_real__and___dunderpyx_t_7easyvec_7vectors_real__etc;
+struct __pyx_ctuple_acdc9__int__and___dunderpyx_t_7easyvec_7vectors_real__and___dunderpyx_t_7easyvec_7vectors_real__etc;
+typedef struct __pyx_ctuple_acdc9__int__and___dunderpyx_t_7easyvec_7vectors_real__and___dunderpyx_t_7easyvec_7vectors_real__etc __pyx_ctuple_acdc9__int__and___dunderpyx_t_7easyvec_7vectors_real__and___dunderpyx_t_7easyvec_7vectors_real__etc;
 struct __pyx_opt_args_7easyvec_8geometry_4Rect_intersect_general;
 struct __pyx_opt_args_7easyvec_8geometry_4Rect_intersect_segment;
 struct __pyx_opt_args_7easyvec_8geometry_4Rect_intersect_ray;
 struct __pyx_opt_args_7easyvec_8geometry_4Rect_intersect_line;
 struct __pyx_opt_args_7easyvec_8geometry_8PolyLine_intersect_general;
 struct __pyx_opt_args_7easyvec_8geometry_8PolyLine_intersect_line;
 struct __pyx_opt_args_7easyvec_8geometry_8PolyLine_intersect_ray;
@@ -1146,15 +1146,15 @@
 /* "easyvec/geometry.pxd":7
  * cpdef Vec2 _convert(object candidate)
  * cpdef bint is_bbox_intersect(Vec2 u1, Vec2 u2, Vec2 v1, Vec2 v2)
  * cpdef (bint, real, real) _intersect_ts(Vec2 u1, Vec2 u2, Vec2 v1, Vec2 v2)             # <<<<<<<<<<<<<<
  * cpdef Vec2 intersect_lines(Vec2 u1, Vec2 u2, Vec2 v1, Vec2 v2)
  * cpdef Vec2 intersect_segments(Vec2 u1, Vec2 u2, Vec2 v1, Vec2 v2)
  */
-struct __pyx_ctuple_d78dc__int__and___dunderpyx_t_7easyvec_7vectors_real__and___dunderpyx_t_7easyvec_7vectors_real__etc {
+struct __pyx_ctuple_acdc9__int__and___dunderpyx_t_7easyvec_7vectors_real__and___dunderpyx_t_7easyvec_7vectors_real__etc {
   int f0;
   __pyx_t_7easyvec_7vectors_real f1;
   __pyx_t_7easyvec_7vectors_real f2;
 };
 
 /* "easyvec/geometry.pxd":28
  *     cpdef bint is_null(self)
@@ -1639,16 +1639,16 @@
 static int __pyx_f_7easyvec_8geometry_4Rect_is_bbox_intersect(struct __pyx_obj_7easyvec_8geometry_Rect *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, int __pyx_skip_dispatch);
 
 
 /* "easyvec/geometry.pyx":558
  * 
  * @cython.final
  * cdef class PolyLine:             # <<<<<<<<<<<<<<
- *     def __cinit__(self, vecs: list, enclosed=True, copy_data=False):
- *         cdef int vec_len, i
+ *     @classmethod
+ *     def from_dict(cls, dct):
  */
 
 struct __pyx_vtabstruct_7easyvec_8geometry_PolyLine {
   PyObject *(*intersect_general)(struct __pyx_obj_7easyvec_8geometry_PolyLine *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, __pyx_t_7easyvec_7vectors_real, __pyx_t_7easyvec_7vectors_real, int __pyx_skip_dispatch, struct __pyx_opt_args_7easyvec_8geometry_8PolyLine_intersect_general *__pyx_optional_args);
   PyObject *(*intersect_line)(struct __pyx_obj_7easyvec_8geometry_PolyLine *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, int __pyx_skip_dispatch, struct __pyx_opt_args_7easyvec_8geometry_8PolyLine_intersect_line *__pyx_optional_args);
   PyObject *(*intersect_ray)(struct __pyx_obj_7easyvec_8geometry_PolyLine *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, int __pyx_skip_dispatch, struct __pyx_opt_args_7easyvec_8geometry_8PolyLine_intersect_ray *__pyx_optional_args);
   PyObject *(*intersect_segment)(struct __pyx_obj_7easyvec_8geometry_PolyLine *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, int __pyx_skip_dispatch, struct __pyx_opt_args_7easyvec_8geometry_8PolyLine_intersect_segment *__pyx_optional_args);
@@ -2562,15 +2562,15 @@
 /* ObjectToMemviewSlice.proto */
 static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_7easyvec_7vectors_real(PyObject *, int writable_flag);
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
 
 /* ToPyCTupleUtility.proto */
-static PyObject* __pyx_convert__to_py___pyx_ctuple_d78dc__int__and___dunderpyx_t_7easyvec_7vectors_real__and___dunderpyx_t_7easyvec_7vectors_real__etc(__pyx_ctuple_d78dc__int__and___dunderpyx_t_7easyvec_7vectors_real__and___dunderpyx_t_7easyvec_7vectors_real__etc);
+static PyObject* __pyx_convert__to_py___pyx_ctuple_acdc9__int__and___dunderpyx_t_7easyvec_7vectors_real__and___dunderpyx_t_7easyvec_7vectors_real__etc(__pyx_ctuple_acdc9__int__and___dunderpyx_t_7easyvec_7vectors_real__and___dunderpyx_t_7easyvec_7vectors_real__etc);
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
 
 /* MemviewSliceCopyTemplate.proto */
 static __Pyx_memviewslice
 __pyx_memoryview_copy_new_contig(const __Pyx_memviewslice *from_mvs,
@@ -2838,15 +2838,15 @@
 static PyObject *indirect = 0;
 static PyObject *contiguous = 0;
 static PyObject *indirect_contiguous = 0;
 static int __pyx_memoryview_thread_locks_used;
 static PyThread_type_lock __pyx_memoryview_thread_locks[8];
 static struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_f_7easyvec_8geometry__convert(PyObject *, int __pyx_skip_dispatch); /*proto*/
 static int __pyx_f_7easyvec_8geometry_is_bbox_intersect(struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, int __pyx_skip_dispatch); /*proto*/
-static __pyx_ctuple_d78dc__int__and___dunderpyx_t_7easyvec_7vectors_real__and___dunderpyx_t_7easyvec_7vectors_real__etc __pyx_f_7easyvec_8geometry__intersect_ts(struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, int __pyx_skip_dispatch); /*proto*/
+static __pyx_ctuple_acdc9__int__and___dunderpyx_t_7easyvec_7vectors_real__and___dunderpyx_t_7easyvec_7vectors_real__etc __pyx_f_7easyvec_8geometry__intersect_ts(struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, int __pyx_skip_dispatch); /*proto*/
 static struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_f_7easyvec_8geometry_intersect_lines(struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, int __pyx_skip_dispatch); /*proto*/
 static struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_f_7easyvec_8geometry_intersect_segments(struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, int __pyx_skip_dispatch); /*proto*/
 static struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_f_7easyvec_8geometry_intersect_rays(struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, int __pyx_skip_dispatch); /*proto*/
 static struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_f_7easyvec_8geometry_intersect_ray_line(struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, int __pyx_skip_dispatch); /*proto*/
 static struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_f_7easyvec_8geometry_intersect_ray_segment(struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, int __pyx_skip_dispatch); /*proto*/
 static struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_f_7easyvec_8geometry_intersect_line_segment(struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, int __pyx_skip_dispatch); /*proto*/
 static CYTHON_INLINE __pyx_t_7easyvec_7vectors_real __pyx_f_7easyvec_8geometry_fmax(__pyx_t_7easyvec_7vectors_real, __pyx_t_7easyvec_7vectors_real, int __pyx_skip_dispatch); /*proto*/
@@ -3005,14 +3005,15 @@
 static const char __pyx_k_update[] = "update";
 static const char __pyx_k_fortran[] = "fortran";
 static const char __pyx_k_memview[] = "memview";
 static const char __pyx_k_ndarray[] = "ndarray";
 static const char __pyx_k_popitem[] = "popitem";
 static const char __pyx_k_ray_set[] = "ray_set";
 static const char __pyx_k_segment[] = "segment";
+static const char __pyx_k_to_dict[] = "to_dict";
 static const char __pyx_k_Ellipsis[] = "Ellipsis";
 static const char __pyx_k_PolyLine[] = "PolyLine(";
 static const char __pyx_k_enclosed[] = "enclosed";
 static const char __pyx_k_getstate[] = "__getstate__";
 static const char __pyx_k_itemsize[] = "itemsize";
 static const char __pyx_k_line_set[] = "line_set";
 static const char __pyx_k_pyx_type[] = "__pyx_type";
@@ -3143,14 +3144,15 @@
 static PyObject *__pyx_kp_s_contiguous_and_indirect;
 static PyObject *__pyx_n_s_copy_data;
 static PyObject *__pyx_n_u_d;
 static PyObject *__pyx_n_s_dict;
 static PyObject *__pyx_n_s_dtype_is_object;
 static PyObject *__pyx_n_s_easyvec_geometry;
 static PyObject *__pyx_n_s_enclosed;
+static PyObject *__pyx_n_u_enclosed;
 static PyObject *__pyx_kp_u_enclosed_2;
 static PyObject *__pyx_n_s_encode;
 static PyObject *__pyx_n_s_enumerate;
 static PyObject *__pyx_n_s_error;
 static PyObject *__pyx_n_s_f_high;
 static PyObject *__pyx_n_s_f_low;
 static PyObject *__pyx_n_s_flags;
@@ -3245,23 +3247,25 @@
 static PyObject *__pyx_kp_s_strided_and_direct;
 static PyObject *__pyx_kp_s_strided_and_direct_or_indirect;
 static PyObject *__pyx_kp_s_strided_and_indirect;
 static PyObject *__pyx_kp_s_stringsource;
 static PyObject *__pyx_n_s_struct;
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_n_s_throw;
+static PyObject *__pyx_n_s_to_dict;
 static PyObject *__pyx_n_s_u1;
 static PyObject *__pyx_n_s_u2;
 static PyObject *__pyx_kp_s_unable_to_allocate_array_data;
 static PyObject *__pyx_kp_s_unable_to_allocate_shape_and_str;
 static PyObject *__pyx_n_s_unpack;
 static PyObject *__pyx_n_s_update;
 static PyObject *__pyx_n_s_v1;
 static PyObject *__pyx_n_s_v2;
 static PyObject *__pyx_n_s_vecs;
+static PyObject *__pyx_n_u_vecs;
 static PyObject *__pyx_n_s_x;
 static PyObject *__pyx_n_u_x1;
 static PyObject *__pyx_n_u_x2;
 static PyObject *__pyx_n_s_y;
 static PyObject *__pyx_n_u_y1;
 static PyObject *__pyx_n_u_y2;
 static PyObject *__pyx_pf_7easyvec_8geometry__convert(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_candidate); /* proto */
@@ -3318,28 +3322,30 @@
 static int __pyx_pf_7easyvec_8geometry_4Rect_2x2_2__set__(struct __pyx_obj_7easyvec_8geometry_Rect *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
 static PyObject *__pyx_pf_7easyvec_8geometry_4Rect_2y1___get__(struct __pyx_obj_7easyvec_8geometry_Rect *__pyx_v_self); /* proto */
 static int __pyx_pf_7easyvec_8geometry_4Rect_2y1_2__set__(struct __pyx_obj_7easyvec_8geometry_Rect *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
 static PyObject *__pyx_pf_7easyvec_8geometry_4Rect_2y2___get__(struct __pyx_obj_7easyvec_8geometry_Rect *__pyx_v_self); /* proto */
 static int __pyx_pf_7easyvec_8geometry_4Rect_2y2_2__set__(struct __pyx_obj_7easyvec_8geometry_Rect *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
 static PyObject *__pyx_pf_7easyvec_8geometry_4Rect_69__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_7easyvec_8geometry_Rect *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_7easyvec_8geometry_4Rect_71__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_7easyvec_8geometry_Rect *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
-static int __pyx_pf_7easyvec_8geometry_8PolyLine___cinit__(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self, PyObject *__pyx_v_vecs, PyObject *__pyx_v_enclosed, PyObject *__pyx_v_copy_data); /* proto */
-static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_2__str__(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_4__repr__(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_6intersect_general(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p2, __pyx_t_7easyvec_7vectors_real __pyx_v_f_low, __pyx_t_7easyvec_7vectors_real __pyx_v_f_high, int __pyx_v_sortreduce); /* proto */
-static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_8intersect_line(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p2, int __pyx_v_sortreduce); /* proto */
-static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_10intersect_ray(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p2, int __pyx_v_sortreduce); /* proto */
-static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_12intersect_segment(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p2, int __pyx_v_sortreduce); /* proto */
+static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_from_dict(PyTypeObject *__pyx_v_cls, PyObject *__pyx_v_dct); /* proto */
+static int __pyx_pf_7easyvec_8geometry_8PolyLine_2__cinit__(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self, PyObject *__pyx_v_vecs, PyObject *__pyx_v_enclosed, PyObject *__pyx_v_copy_data); /* proto */
+static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_4to_dict(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_6__str__(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_8__repr__(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_10intersect_general(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p2, __pyx_t_7easyvec_7vectors_real __pyx_v_f_low, __pyx_t_7easyvec_7vectors_real __pyx_v_f_high, int __pyx_v_sortreduce); /* proto */
+static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_12intersect_line(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p2, int __pyx_v_sortreduce); /* proto */
+static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_14intersect_ray(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p2, int __pyx_v_sortreduce); /* proto */
+static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_16intersect_segment(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p2, int __pyx_v_sortreduce); /* proto */
 static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_4vecs___get__(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self); /* proto */
 static int __pyx_pf_7easyvec_8geometry_8PolyLine_4vecs_2__set__(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
 static int __pyx_pf_7easyvec_8geometry_8PolyLine_4vecs_4__del__(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_8enclosed___get__(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self); /* proto */
 static int __pyx_pf_7easyvec_8geometry_8PolyLine_8enclosed_2__set__(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
-static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_14__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_16__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_18__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_20__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static int __pyx_pf_7cpython_5array_5array___getbuffer__(arrayobject *__pyx_v_self, Py_buffer *__pyx_v_info, CYTHON_UNUSED int __pyx_v_flags); /* proto */
 static void __pyx_pf_7cpython_5array_5array_2__releasebuffer__(CYTHON_UNUSED arrayobject *__pyx_v_self, Py_buffer *__pyx_v_info); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array___cinit__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_shape, Py_ssize_t __pyx_v_itemsize, PyObject *__pyx_v_format, PyObject *__pyx_v_mode, int __pyx_v_allocate_buffer); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array_2__getbuffer__(struct __pyx_array_obj *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /* proto */
 static void __pyx_array___pyx_pf_15View_dot_MemoryView_5array_4__dealloc__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_15View_dot_MemoryView_5array_7memview___get__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static Py_ssize_t __pyx_array___pyx_pf_15View_dot_MemoryView_5array_6__len__(struct __pyx_array_obj *__pyx_v_self); /* proto */
@@ -5006,27 +5012,27 @@
  * @cython.cdivision(True)
  * cpdef (bint, real, real) _intersect_ts(Vec2 u1, Vec2 u2, Vec2 v1, Vec2 v2):             # <<<<<<<<<<<<<<
  *     cdef Vec2 vec1 = u1.sub(v1)
  *     cdef Vec2 vec2 = v2.sub(v1)
  */
 
 static PyObject *__pyx_pw_7easyvec_8geometry_7_intersect_ts(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static __pyx_ctuple_d78dc__int__and___dunderpyx_t_7easyvec_7vectors_real__and___dunderpyx_t_7easyvec_7vectors_real__etc __pyx_f_7easyvec_8geometry__intersect_ts(struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_u1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_u2, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_v1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_v2, CYTHON_UNUSED int __pyx_skip_dispatch) {
+static __pyx_ctuple_acdc9__int__and___dunderpyx_t_7easyvec_7vectors_real__and___dunderpyx_t_7easyvec_7vectors_real__etc __pyx_f_7easyvec_8geometry__intersect_ts(struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_u1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_u2, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_v1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_v2, CYTHON_UNUSED int __pyx_skip_dispatch) {
   struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_vec1 = 0;
   struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_vec2 = 0;
   struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_vec3 = 0;
   __pyx_t_7easyvec_7vectors_real __pyx_v_dot;
   __pyx_t_7easyvec_7vectors_real __pyx_v_t1;
   __pyx_t_7easyvec_7vectors_real __pyx_v_t2;
-  __pyx_ctuple_d78dc__int__and___dunderpyx_t_7easyvec_7vectors_real__and___dunderpyx_t_7easyvec_7vectors_real__etc __pyx_r;
+  __pyx_ctuple_acdc9__int__and___dunderpyx_t_7easyvec_7vectors_real__and___dunderpyx_t_7easyvec_7vectors_real__etc __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_t_3;
-  __pyx_ctuple_d78dc__int__and___dunderpyx_t_7easyvec_7vectors_real__and___dunderpyx_t_7easyvec_7vectors_real__etc __pyx_t_4;
+  __pyx_ctuple_acdc9__int__and___dunderpyx_t_7easyvec_7vectors_real__and___dunderpyx_t_7easyvec_7vectors_real__etc __pyx_t_4;
   __Pyx_RefNannySetupContext("_intersect_ts", 0);
 
   /* "easyvec/geometry.pyx":88
  * @cython.cdivision(True)
  * cpdef (bint, real, real) _intersect_ts(Vec2 u1, Vec2 u2, Vec2 v1, Vec2 v2):
  *     cdef Vec2 vec1 = u1.sub(v1)             # <<<<<<<<<<<<<<
  *     cdef Vec2 vec2 = v2.sub(v1)
@@ -5284,15 +5290,15 @@
 
 static PyObject *__pyx_pf_7easyvec_8geometry_6_intersect_ts(CYTHON_UNUSED PyObject *__pyx_self, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_u1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_u2, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_v1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_v2) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("_intersect_ts", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_convert__to_py___pyx_ctuple_d78dc__int__and___dunderpyx_t_7easyvec_7vectors_real__and___dunderpyx_t_7easyvec_7vectors_real__etc(__pyx_f_7easyvec_8geometry__intersect_ts(__pyx_v_u1, __pyx_v_u2, __pyx_v_v1, __pyx_v_v2, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 87, __pyx_L1_error)
+  __pyx_t_1 = __pyx_convert__to_py___pyx_ctuple_acdc9__int__and___dunderpyx_t_7easyvec_7vectors_real__and___dunderpyx_t_7easyvec_7vectors_real__etc(__pyx_f_7easyvec_8geometry__intersect_ts(__pyx_v_u1, __pyx_v_u2, __pyx_v_v1, __pyx_v_v2, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -5316,15 +5322,15 @@
 static PyObject *__pyx_pw_7easyvec_8geometry_9intersect_lines(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_f_7easyvec_8geometry_intersect_lines(struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_u1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_u2, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_v1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_v2, CYTHON_UNUSED int __pyx_skip_dispatch) {
   int __pyx_v_suc;
   __pyx_t_7easyvec_7vectors_real __pyx_v_t1;
   CYTHON_UNUSED __pyx_t_7easyvec_7vectors_real __pyx_v_t2;
   struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  __pyx_ctuple_d78dc__int__and___dunderpyx_t_7easyvec_7vectors_real__and___dunderpyx_t_7easyvec_7vectors_real__etc __pyx_t_1;
+  __pyx_ctuple_acdc9__int__and___dunderpyx_t_7easyvec_7vectors_real__and___dunderpyx_t_7easyvec_7vectors_real__etc __pyx_t_1;
   int __pyx_t_2;
   __pyx_t_7easyvec_7vectors_real __pyx_t_3;
   __pyx_t_7easyvec_7vectors_real __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   __Pyx_RefNannySetupContext("intersect_lines", 0);
 
@@ -5540,15 +5546,15 @@
 static struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_f_7easyvec_8geometry_intersect_segments(struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_u1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_u2, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_v1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_v2, CYTHON_UNUSED int __pyx_skip_dispatch) {
   int __pyx_v_suc;
   __pyx_t_7easyvec_7vectors_real __pyx_v_t1;
   __pyx_t_7easyvec_7vectors_real __pyx_v_t2;
   struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
-  __pyx_ctuple_d78dc__int__and___dunderpyx_t_7easyvec_7vectors_real__and___dunderpyx_t_7easyvec_7vectors_real__etc __pyx_t_2;
+  __pyx_ctuple_acdc9__int__and___dunderpyx_t_7easyvec_7vectors_real__and___dunderpyx_t_7easyvec_7vectors_real__etc __pyx_t_2;
   __pyx_t_7easyvec_7vectors_real __pyx_t_3;
   __pyx_t_7easyvec_7vectors_real __pyx_t_4;
   int __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   __Pyx_RefNannySetupContext("intersect_segments", 0);
 
@@ -5819,15 +5825,15 @@
 static PyObject *__pyx_pw_7easyvec_8geometry_13intersect_rays(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_f_7easyvec_8geometry_intersect_rays(struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_u1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_u2, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_v1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_v2, CYTHON_UNUSED int __pyx_skip_dispatch) {
   int __pyx_v_suc;
   __pyx_t_7easyvec_7vectors_real __pyx_v_t1;
   __pyx_t_7easyvec_7vectors_real __pyx_v_t2;
   struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  __pyx_ctuple_d78dc__int__and___dunderpyx_t_7easyvec_7vectors_real__and___dunderpyx_t_7easyvec_7vectors_real__etc __pyx_t_1;
+  __pyx_ctuple_acdc9__int__and___dunderpyx_t_7easyvec_7vectors_real__and___dunderpyx_t_7easyvec_7vectors_real__etc __pyx_t_1;
   int __pyx_t_2;
   __pyx_t_7easyvec_7vectors_real __pyx_t_3;
   __pyx_t_7easyvec_7vectors_real __pyx_t_4;
   int __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   __Pyx_RefNannySetupContext("intersect_rays", 0);
@@ -6057,15 +6063,15 @@
 static PyObject *__pyx_pw_7easyvec_8geometry_15intersect_ray_line(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_f_7easyvec_8geometry_intersect_ray_line(struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_r1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_r2, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_v1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_v2, CYTHON_UNUSED int __pyx_skip_dispatch) {
   int __pyx_v_suc;
   __pyx_t_7easyvec_7vectors_real __pyx_v_t1;
   CYTHON_UNUSED __pyx_t_7easyvec_7vectors_real __pyx_v_t2;
   struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  __pyx_ctuple_d78dc__int__and___dunderpyx_t_7easyvec_7vectors_real__and___dunderpyx_t_7easyvec_7vectors_real__etc __pyx_t_1;
+  __pyx_ctuple_acdc9__int__and___dunderpyx_t_7easyvec_7vectors_real__and___dunderpyx_t_7easyvec_7vectors_real__etc __pyx_t_1;
   int __pyx_t_2;
   __pyx_t_7easyvec_7vectors_real __pyx_t_3;
   __pyx_t_7easyvec_7vectors_real __pyx_t_4;
   int __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   __Pyx_RefNannySetupContext("intersect_ray_line", 0);
@@ -6289,15 +6295,15 @@
 static PyObject *__pyx_pw_7easyvec_8geometry_17intersect_ray_segment(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_f_7easyvec_8geometry_intersect_ray_segment(struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_r1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_r2, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_v1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_v2, CYTHON_UNUSED int __pyx_skip_dispatch) {
   int __pyx_v_suc;
   __pyx_t_7easyvec_7vectors_real __pyx_v_t1;
   __pyx_t_7easyvec_7vectors_real __pyx_v_t2;
   struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  __pyx_ctuple_d78dc__int__and___dunderpyx_t_7easyvec_7vectors_real__and___dunderpyx_t_7easyvec_7vectors_real__etc __pyx_t_1;
+  __pyx_ctuple_acdc9__int__and___dunderpyx_t_7easyvec_7vectors_real__and___dunderpyx_t_7easyvec_7vectors_real__etc __pyx_t_1;
   int __pyx_t_2;
   __pyx_t_7easyvec_7vectors_real __pyx_t_3;
   __pyx_t_7easyvec_7vectors_real __pyx_t_4;
   int __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   __Pyx_RefNannySetupContext("intersect_ray_segment", 0);
@@ -6533,15 +6539,15 @@
 static PyObject *__pyx_pw_7easyvec_8geometry_19intersect_line_segment(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_f_7easyvec_8geometry_intersect_line_segment(struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_u1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_u2, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_s1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_s2, CYTHON_UNUSED int __pyx_skip_dispatch) {
   int __pyx_v_suc;
   __pyx_t_7easyvec_7vectors_real __pyx_v_t1;
   __pyx_t_7easyvec_7vectors_real __pyx_v_t2;
   struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  __pyx_ctuple_d78dc__int__and___dunderpyx_t_7easyvec_7vectors_real__and___dunderpyx_t_7easyvec_7vectors_real__etc __pyx_t_1;
+  __pyx_ctuple_acdc9__int__and___dunderpyx_t_7easyvec_7vectors_real__and___dunderpyx_t_7easyvec_7vectors_real__etc __pyx_t_1;
   int __pyx_t_2;
   __pyx_t_7easyvec_7vectors_real __pyx_t_3;
   __pyx_t_7easyvec_7vectors_real __pyx_t_4;
   int __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   __Pyx_RefNannySetupContext("intersect_line_segment", 0);
@@ -15100,25 +15106,208 @@
   __Pyx_AddTraceback("easyvec.geometry.Rect.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "easyvec/geometry.pyx":559
- * @cython.final
+/* "easyvec/geometry.pyx":560
+ * cdef class PolyLine:
+ *     @classmethod
+ *     def from_dict(cls, dct):             # <<<<<<<<<<<<<<
+ *         vecs = [Vec2.from_dict(vd) for vd in dct['vecs']]
+ *         enclosed = dct['enclosed']
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_1from_dict(PyObject *__pyx_v_cls, PyObject *__pyx_v_dct); /*proto*/
+static char __pyx_doc_7easyvec_8geometry_8PolyLine_from_dict[] = "PolyLine.from_dict(type cls, dct)";
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_1from_dict(PyObject *__pyx_v_cls, PyObject *__pyx_v_dct) {
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("from_dict (wrapper)", 0);
+  __pyx_r = __pyx_pf_7easyvec_8geometry_8PolyLine_from_dict(((PyTypeObject*)__pyx_v_cls), ((PyObject *)__pyx_v_dct));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_from_dict(PyTypeObject *__pyx_v_cls, PyObject *__pyx_v_dct) {
+  PyObject *__pyx_v_vecs = NULL;
+  PyObject *__pyx_v_enclosed = NULL;
+  PyObject *__pyx_7genexpr__pyx_v_vd = NULL;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  Py_ssize_t __pyx_t_4;
+  PyObject *(*__pyx_t_5)(PyObject *);
+  PyObject *__pyx_t_6 = NULL;
+  PyObject *__pyx_t_7 = NULL;
+  __Pyx_RefNannySetupContext("from_dict", 0);
+
+  /* "easyvec/geometry.pyx":561
+ *     @classmethod
+ *     def from_dict(cls, dct):
+ *         vecs = [Vec2.from_dict(vd) for vd in dct['vecs']]             # <<<<<<<<<<<<<<
+ *         enclosed = dct['enclosed']
+ *         return cls(vecs, enclosed)
+ */
+  { /* enter inner scope */
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 561, __pyx_L5_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_v_dct, __pyx_n_u_vecs); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 561, __pyx_L5_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    if (likely(PyList_CheckExact(__pyx_t_2)) || PyTuple_CheckExact(__pyx_t_2)) {
+      __pyx_t_3 = __pyx_t_2; __Pyx_INCREF(__pyx_t_3); __pyx_t_4 = 0;
+      __pyx_t_5 = NULL;
+    } else {
+      __pyx_t_4 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 561, __pyx_L5_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __pyx_t_5 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 561, __pyx_L5_error)
+    }
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    for (;;) {
+      if (likely(!__pyx_t_5)) {
+        if (likely(PyList_CheckExact(__pyx_t_3))) {
+          if (__pyx_t_4 >= PyList_GET_SIZE(__pyx_t_3)) break;
+          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+          __pyx_t_2 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 561, __pyx_L5_error)
+          #else
+          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 561, __pyx_L5_error)
+          __Pyx_GOTREF(__pyx_t_2);
+          #endif
+        } else {
+          if (__pyx_t_4 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
+          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+          __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 561, __pyx_L5_error)
+          #else
+          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 561, __pyx_L5_error)
+          __Pyx_GOTREF(__pyx_t_2);
+          #endif
+        }
+      } else {
+        __pyx_t_2 = __pyx_t_5(__pyx_t_3);
+        if (unlikely(!__pyx_t_2)) {
+          PyObject* exc_type = PyErr_Occurred();
+          if (exc_type) {
+            if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+            else __PYX_ERR(0, 561, __pyx_L5_error)
+          }
+          break;
+        }
+        __Pyx_GOTREF(__pyx_t_2);
+      }
+      __Pyx_XDECREF_SET(__pyx_7genexpr__pyx_v_vd, __pyx_t_2);
+      __pyx_t_2 = 0;
+      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_7easyvec_7vectors_Vec2), __pyx_n_s_from_dict); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 561, __pyx_L5_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __pyx_t_7 = NULL;
+      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
+        __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
+        if (likely(__pyx_t_7)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
+          __Pyx_INCREF(__pyx_t_7);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_6, function);
+        }
+      }
+      __pyx_t_2 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_7, __pyx_7genexpr__pyx_v_vd) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_7genexpr__pyx_v_vd);
+      __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 561, __pyx_L5_error)
+      __Pyx_GOTREF(__pyx_t_2);
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_2))) __PYX_ERR(0, 561, __pyx_L5_error)
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    }
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_XDECREF(__pyx_7genexpr__pyx_v_vd); __pyx_7genexpr__pyx_v_vd = 0;
+    goto __pyx_L8_exit_scope;
+    __pyx_L5_error:;
+    __Pyx_XDECREF(__pyx_7genexpr__pyx_v_vd); __pyx_7genexpr__pyx_v_vd = 0;
+    goto __pyx_L1_error;
+    __pyx_L8_exit_scope:;
+  } /* exit inner scope */
+  __pyx_v_vecs = ((PyObject*)__pyx_t_1);
+  __pyx_t_1 = 0;
+
+  /* "easyvec/geometry.pyx":562
+ *     def from_dict(cls, dct):
+ *         vecs = [Vec2.from_dict(vd) for vd in dct['vecs']]
+ *         enclosed = dct['enclosed']             # <<<<<<<<<<<<<<
+ *         return cls(vecs, enclosed)
+ * 
+ */
+  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_dct, __pyx_n_u_enclosed); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 562, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_v_enclosed = __pyx_t_1;
+  __pyx_t_1 = 0;
+
+  /* "easyvec/geometry.pyx":563
+ *         vecs = [Vec2.from_dict(vd) for vd in dct['vecs']]
+ *         enclosed = dct['enclosed']
+ *         return cls(vecs, enclosed)             # <<<<<<<<<<<<<<
+ * 
+ *     def __cinit__(self, vecs: list, enclosed=True, copy_data=False):
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 563, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_INCREF(__pyx_v_vecs);
+  __Pyx_GIVEREF(__pyx_v_vecs);
+  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_vecs);
+  __Pyx_INCREF(__pyx_v_enclosed);
+  __Pyx_GIVEREF(__pyx_v_enclosed);
+  PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_enclosed);
+  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_v_cls), __pyx_t_1, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 563, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_r = __pyx_t_3;
+  __pyx_t_3 = 0;
+  goto __pyx_L0;
+
+  /* "easyvec/geometry.pyx":560
  * cdef class PolyLine:
+ *     @classmethod
+ *     def from_dict(cls, dct):             # <<<<<<<<<<<<<<
+ *         vecs = [Vec2.from_dict(vd) for vd in dct['vecs']]
+ *         enclosed = dct['enclosed']
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_AddTraceback("easyvec.geometry.PolyLine.from_dict", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_vecs);
+  __Pyx_XDECREF(__pyx_v_enclosed);
+  __Pyx_XDECREF(__pyx_7genexpr__pyx_v_vd);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "easyvec/geometry.pyx":565
+ *         return cls(vecs, enclosed)
+ * 
  *     def __cinit__(self, vecs: list, enclosed=True, copy_data=False):             # <<<<<<<<<<<<<<
  *         cdef int vec_len, i
  *         if copy_data:
  */
 
 /* Python wrapper */
-static int __pyx_pw_7easyvec_8geometry_8PolyLine_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static int __pyx_pw_7easyvec_8geometry_8PolyLine_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static int __pyx_pw_7easyvec_8geometry_8PolyLine_3__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static int __pyx_pw_7easyvec_8geometry_8PolyLine_3__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_vecs = 0;
   PyObject *__pyx_v_enclosed = 0;
   PyObject *__pyx_v_copy_data = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__ (wrapper)", 0);
   {
@@ -15154,15 +15343,15 @@
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_copy_data);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 559, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 565, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
@@ -15173,33 +15362,33 @@
     }
     __pyx_v_vecs = ((PyObject*)values[0]);
     __pyx_v_enclosed = values[1];
     __pyx_v_copy_data = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 559, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 565, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("easyvec.geometry.PolyLine.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_vecs), (&PyList_Type), 1, "vecs", 1))) __PYX_ERR(0, 559, __pyx_L1_error)
-  __pyx_r = __pyx_pf_7easyvec_8geometry_8PolyLine___cinit__(((struct __pyx_obj_7easyvec_8geometry_PolyLine *)__pyx_v_self), __pyx_v_vecs, __pyx_v_enclosed, __pyx_v_copy_data);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_vecs), (&PyList_Type), 1, "vecs", 1))) __PYX_ERR(0, 565, __pyx_L1_error)
+  __pyx_r = __pyx_pf_7easyvec_8geometry_8PolyLine_2__cinit__(((struct __pyx_obj_7easyvec_8geometry_PolyLine *)__pyx_v_self), __pyx_v_vecs, __pyx_v_enclosed, __pyx_v_copy_data);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static int __pyx_pf_7easyvec_8geometry_8PolyLine___cinit__(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self, PyObject *__pyx_v_vecs, PyObject *__pyx_v_enclosed, PyObject *__pyx_v_copy_data) {
+static int __pyx_pf_7easyvec_8geometry_8PolyLine_2__cinit__(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self, PyObject *__pyx_v_vecs, PyObject *__pyx_v_enclosed, PyObject *__pyx_v_copy_data) {
   int __pyx_v_vec_len;
   int __pyx_v_i;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   Py_ssize_t __pyx_t_3;
@@ -15207,100 +15396,100 @@
   int __pyx_t_5;
   int __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_t_8;
   PyObject *__pyx_t_9 = NULL;
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "easyvec/geometry.pyx":561
+  /* "easyvec/geometry.pyx":567
  *     def __cinit__(self, vecs: list, enclosed=True, copy_data=False):
  *         cdef int vec_len, i
  *         if copy_data:             # <<<<<<<<<<<<<<
  *             self.vecs = []
  *             vec_len = len(vecs)
  */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_copy_data); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 561, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_copy_data); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 567, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "easyvec/geometry.pyx":562
+    /* "easyvec/geometry.pyx":568
  *         cdef int vec_len, i
  *         if copy_data:
  *             self.vecs = []             # <<<<<<<<<<<<<<
  *             vec_len = len(vecs)
  *             for i in range(vec_len):
  */
-    __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 562, __pyx_L1_error)
+    __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 568, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_GIVEREF(__pyx_t_2);
     __Pyx_GOTREF(__pyx_v_self->vecs);
     __Pyx_DECREF(__pyx_v_self->vecs);
     __pyx_v_self->vecs = ((PyObject*)__pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "easyvec/geometry.pyx":563
+    /* "easyvec/geometry.pyx":569
  *         if copy_data:
  *             self.vecs = []
  *             vec_len = len(vecs)             # <<<<<<<<<<<<<<
  *             for i in range(vec_len):
  *                 self.vecs.append( (<Vec2>(vecs[i])).copy() )
  */
     if (unlikely(__pyx_v_vecs == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-      __PYX_ERR(0, 563, __pyx_L1_error)
+      __PYX_ERR(0, 569, __pyx_L1_error)
     }
-    __pyx_t_3 = PyList_GET_SIZE(__pyx_v_vecs); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 563, __pyx_L1_error)
+    __pyx_t_3 = PyList_GET_SIZE(__pyx_v_vecs); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 569, __pyx_L1_error)
     __pyx_v_vec_len = __pyx_t_3;
 
-    /* "easyvec/geometry.pyx":564
+    /* "easyvec/geometry.pyx":570
  *             self.vecs = []
  *             vec_len = len(vecs)
  *             for i in range(vec_len):             # <<<<<<<<<<<<<<
  *                 self.vecs.append( (<Vec2>(vecs[i])).copy() )
  *         else:
  */
     __pyx_t_4 = __pyx_v_vec_len;
     __pyx_t_5 = __pyx_t_4;
     for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
       __pyx_v_i = __pyx_t_6;
 
-      /* "easyvec/geometry.pyx":565
+      /* "easyvec/geometry.pyx":571
  *             vec_len = len(vecs)
  *             for i in range(vec_len):
  *                 self.vecs.append( (<Vec2>(vecs[i])).copy() )             # <<<<<<<<<<<<<<
  *         else:
  *             self.vecs = vecs
  */
       if (unlikely(__pyx_v_self->vecs == Py_None)) {
         PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "append");
-        __PYX_ERR(0, 565, __pyx_L1_error)
+        __PYX_ERR(0, 571, __pyx_L1_error)
       }
       if (unlikely(__pyx_v_vecs == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 565, __pyx_L1_error)
+        __PYX_ERR(0, 571, __pyx_L1_error)
       }
-      __pyx_t_2 = __Pyx_GetItemInt_List(__pyx_v_vecs, __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 565, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_GetItemInt_List(__pyx_v_vecs, __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 571, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_7 = ((PyObject *)((struct __pyx_vtabstruct_7easyvec_7vectors_Vec2 *)((struct __pyx_obj_7easyvec_7vectors_Vec2 *)__pyx_t_2)->__pyx_vtab)->copy(((struct __pyx_obj_7easyvec_7vectors_Vec2 *)__pyx_t_2), 0)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 565, __pyx_L1_error)
+      __pyx_t_7 = ((PyObject *)((struct __pyx_vtabstruct_7easyvec_7vectors_Vec2 *)((struct __pyx_obj_7easyvec_7vectors_Vec2 *)__pyx_t_2)->__pyx_vtab)->copy(((struct __pyx_obj_7easyvec_7vectors_Vec2 *)__pyx_t_2), 0)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 571, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __pyx_t_8 = __Pyx_PyList_Append(__pyx_v_self->vecs, __pyx_t_7); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(0, 565, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyList_Append(__pyx_v_self->vecs, __pyx_t_7); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(0, 571, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     }
 
-    /* "easyvec/geometry.pyx":561
+    /* "easyvec/geometry.pyx":567
  *     def __cinit__(self, vecs: list, enclosed=True, copy_data=False):
  *         cdef int vec_len, i
  *         if copy_data:             # <<<<<<<<<<<<<<
  *             self.vecs = []
  *             vec_len = len(vecs)
  */
     goto __pyx_L3;
   }
 
-  /* "easyvec/geometry.pyx":567
+  /* "easyvec/geometry.pyx":573
  *                 self.vecs.append( (<Vec2>(vecs[i])).copy() )
  *         else:
  *             self.vecs = vecs             # <<<<<<<<<<<<<<
  *         self.vlen = len(self.vecs)
  *         if self.vlen < 2:
  */
   /*else*/ {
@@ -15308,107 +15497,107 @@
     __Pyx_GIVEREF(__pyx_v_vecs);
     __Pyx_GOTREF(__pyx_v_self->vecs);
     __Pyx_DECREF(__pyx_v_self->vecs);
     __pyx_v_self->vecs = __pyx_v_vecs;
   }
   __pyx_L3:;
 
-  /* "easyvec/geometry.pyx":568
+  /* "easyvec/geometry.pyx":574
  *         else:
  *             self.vecs = vecs
  *         self.vlen = len(self.vecs)             # <<<<<<<<<<<<<<
  *         if self.vlen < 2:
  *             raise ValueError(f'    .  ,  1')
  */
   __pyx_t_7 = __pyx_v_self->vecs;
   __Pyx_INCREF(__pyx_t_7);
   if (unlikely(__pyx_t_7 == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 568, __pyx_L1_error)
+    __PYX_ERR(0, 574, __pyx_L1_error)
   }
-  __pyx_t_3 = PyList_GET_SIZE(__pyx_t_7); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 568, __pyx_L1_error)
+  __pyx_t_3 = PyList_GET_SIZE(__pyx_t_7); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 574, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_v_self->vlen = __pyx_t_3;
 
-  /* "easyvec/geometry.pyx":569
+  /* "easyvec/geometry.pyx":575
  *             self.vecs = vecs
  *         self.vlen = len(self.vecs)
  *         if self.vlen < 2:             # <<<<<<<<<<<<<<
  *             raise ValueError(f'    .  ,  1')
  *         self.enclosed = enclosed
  */
   __pyx_t_1 = ((__pyx_v_self->vlen < 2) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "easyvec/geometry.pyx":570
+    /* "easyvec/geometry.pyx":576
  *         self.vlen = len(self.vecs)
  *         if self.vlen < 2:
  *             raise ValueError(f'    .  ,  1')             # <<<<<<<<<<<<<<
  *         self.enclosed = enclosed
  *         self.bbox = Rect.bbox(self.vecs)
  */
-    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__15, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 570, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__15, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 576, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_Raise(__pyx_t_7, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __PYX_ERR(0, 570, __pyx_L1_error)
+    __PYX_ERR(0, 576, __pyx_L1_error)
 
-    /* "easyvec/geometry.pyx":569
+    /* "easyvec/geometry.pyx":575
  *             self.vecs = vecs
  *         self.vlen = len(self.vecs)
  *         if self.vlen < 2:             # <<<<<<<<<<<<<<
  *             raise ValueError(f'    .  ,  1')
  *         self.enclosed = enclosed
  */
   }
 
-  /* "easyvec/geometry.pyx":571
+  /* "easyvec/geometry.pyx":577
  *         if self.vlen < 2:
  *             raise ValueError(f'    .  ,  1')
  *         self.enclosed = enclosed             # <<<<<<<<<<<<<<
  *         self.bbox = Rect.bbox(self.vecs)
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_enclosed); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 571, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_enclosed); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 577, __pyx_L1_error)
   __pyx_v_self->enclosed = __pyx_t_1;
 
-  /* "easyvec/geometry.pyx":572
+  /* "easyvec/geometry.pyx":578
  *             raise ValueError(f'    .  ,  1')
  *         self.enclosed = enclosed
  *         self.bbox = Rect.bbox(self.vecs)             # <<<<<<<<<<<<<<
  * 
- *     def __str__(self):
+ *     def to_dict(self):
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_7easyvec_8geometry_Rect), __pyx_n_s_bbox); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 572, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_7easyvec_8geometry_Rect), __pyx_n_s_bbox); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 578, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_9 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_9)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_9);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_7 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_9, __pyx_v_self->vecs) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_self->vecs);
   __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-  if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 572, __pyx_L1_error)
+  if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 578, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (!(likely(((__pyx_t_7) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_7, __pyx_ptype_7easyvec_8geometry_Rect))))) __PYX_ERR(0, 572, __pyx_L1_error)
+  if (!(likely(((__pyx_t_7) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_7, __pyx_ptype_7easyvec_8geometry_Rect))))) __PYX_ERR(0, 578, __pyx_L1_error)
   __Pyx_GIVEREF(__pyx_t_7);
   __Pyx_GOTREF(__pyx_v_self->bbox);
   __Pyx_DECREF(((PyObject *)__pyx_v_self->bbox));
   __pyx_v_self->bbox = ((struct __pyx_obj_7easyvec_8geometry_Rect *)__pyx_t_7);
   __pyx_t_7 = 0;
 
-  /* "easyvec/geometry.pyx":559
- * @cython.final
- * cdef class PolyLine:
+  /* "easyvec/geometry.pyx":565
+ *         return cls(vecs, enclosed)
+ * 
  *     def __cinit__(self, vecs: list, enclosed=True, copy_data=False):             # <<<<<<<<<<<<<<
  *         cdef int vec_len, i
  *         if copy_data:
  */
 
   /* function exit code */
   __pyx_r = 0;
@@ -15420,176 +15609,320 @@
   __Pyx_AddTraceback("easyvec.geometry.PolyLine.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "easyvec/geometry.pyx":574
+/* "easyvec/geometry.pyx":580
  *         self.bbox = Rect.bbox(self.vecs)
  * 
+ *     def to_dict(self):             # <<<<<<<<<<<<<<
+ *         return {
+ *             'vecs': [v.to_dict() for v in self.vecs],
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_5to_dict(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_7easyvec_8geometry_8PolyLine_4to_dict[] = "PolyLine.to_dict(self)";
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_5to_dict(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("to_dict (wrapper)", 0);
+  __pyx_r = __pyx_pf_7easyvec_8geometry_8PolyLine_4to_dict(((struct __pyx_obj_7easyvec_8geometry_PolyLine *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_4to_dict(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self) {
+  PyObject *__pyx_8genexpr1__pyx_v_v = NULL;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  Py_ssize_t __pyx_t_4;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  PyObject *__pyx_t_7 = NULL;
+  int __pyx_t_8;
+  __Pyx_RefNannySetupContext("to_dict", 0);
+
+  /* "easyvec/geometry.pyx":581
+ * 
+ *     def to_dict(self):
+ *         return {             # <<<<<<<<<<<<<<
+ *             'vecs': [v.to_dict() for v in self.vecs],
+ *             'enclosed': bool(self.enclosed)
+ */
+  __Pyx_XDECREF(__pyx_r);
+
+  /* "easyvec/geometry.pyx":582
+ *     def to_dict(self):
+ *         return {
+ *             'vecs': [v.to_dict() for v in self.vecs],             # <<<<<<<<<<<<<<
+ *             'enclosed': bool(self.enclosed)
+ *         }
+ */
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 582, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  { /* enter inner scope */
+    __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 582, __pyx_L5_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    if (unlikely(__pyx_v_self->vecs == Py_None)) {
+      PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
+      __PYX_ERR(0, 582, __pyx_L5_error)
+    }
+    __pyx_t_3 = __pyx_v_self->vecs; __Pyx_INCREF(__pyx_t_3); __pyx_t_4 = 0;
+    for (;;) {
+      if (__pyx_t_4 >= PyList_GET_SIZE(__pyx_t_3)) break;
+      #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+      __pyx_t_5 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_5); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 582, __pyx_L5_error)
+      #else
+      __pyx_t_5 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 582, __pyx_L5_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      #endif
+      __Pyx_XDECREF_SET(__pyx_8genexpr1__pyx_v_v, __pyx_t_5);
+      __pyx_t_5 = 0;
+      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_8genexpr1__pyx_v_v, __pyx_n_s_to_dict); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 582, __pyx_L5_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __pyx_t_7 = NULL;
+      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
+        __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
+        if (likely(__pyx_t_7)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
+          __Pyx_INCREF(__pyx_t_7);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_6, function);
+        }
+      }
+      __pyx_t_5 = (__pyx_t_7) ? __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_7) : __Pyx_PyObject_CallNoArg(__pyx_t_6);
+      __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
+      if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 582, __pyx_L5_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_5))) __PYX_ERR(0, 582, __pyx_L5_error)
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    }
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_v); __pyx_8genexpr1__pyx_v_v = 0;
+    goto __pyx_L8_exit_scope;
+    __pyx_L5_error:;
+    __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_v); __pyx_8genexpr1__pyx_v_v = 0;
+    goto __pyx_L1_error;
+    __pyx_L8_exit_scope:;
+  } /* exit inner scope */
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_vecs, __pyx_t_2) < 0) __PYX_ERR(0, 582, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+  /* "easyvec/geometry.pyx":583
+ *         return {
+ *             'vecs': [v.to_dict() for v in self.vecs],
+ *             'enclosed': bool(self.enclosed)             # <<<<<<<<<<<<<<
+ *         }
+ * 
+ */
+  __pyx_t_8 = __pyx_v_self->enclosed;
+  __pyx_t_2 = __Pyx_PyBool_FromLong((!(!__pyx_t_8))); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 583, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_enclosed, __pyx_t_2) < 0) __PYX_ERR(0, 582, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "easyvec/geometry.pyx":580
+ *         self.bbox = Rect.bbox(self.vecs)
+ * 
+ *     def to_dict(self):             # <<<<<<<<<<<<<<
+ *         return {
+ *             'vecs': [v.to_dict() for v in self.vecs],
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_AddTraceback("easyvec.geometry.PolyLine.to_dict", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_v);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "easyvec/geometry.pyx":586
+ *         }
+ * 
  *     def __str__(self):             # <<<<<<<<<<<<<<
  *         s = [f'({v.x:.2f}, {v.y:.2f})' for v in self.vecs]
  *         s = ', '.join(s)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_3__str__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_3__str__(PyObject *__pyx_v_self) {
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_7__str__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_7__str__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__str__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_7easyvec_8geometry_8PolyLine_2__str__(((struct __pyx_obj_7easyvec_8geometry_PolyLine *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7easyvec_8geometry_8PolyLine_6__str__(((struct __pyx_obj_7easyvec_8geometry_PolyLine *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_2__str__(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self) {
+static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_6__str__(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self) {
   PyObject *__pyx_v_s = NULL;
-  PyObject *__pyx_7genexpr__pyx_v_v = NULL;
+  PyObject *__pyx_8genexpr2__pyx_v_v = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   Py_ssize_t __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   Py_ssize_t __pyx_t_5;
   Py_UCS4 __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   __Pyx_RefNannySetupContext("__str__", 0);
 
-  /* "easyvec/geometry.pyx":575
+  /* "easyvec/geometry.pyx":587
  * 
  *     def __str__(self):
  *         s = [f'({v.x:.2f}, {v.y:.2f})' for v in self.vecs]             # <<<<<<<<<<<<<<
  *         s = ', '.join(s)
  *         return f'PolyLine({s})'
  */
   { /* enter inner scope */
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 575, __pyx_L5_error)
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 587, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_1);
     if (unlikely(__pyx_v_self->vecs == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-      __PYX_ERR(0, 575, __pyx_L5_error)
+      __PYX_ERR(0, 587, __pyx_L5_error)
     }
     __pyx_t_2 = __pyx_v_self->vecs; __Pyx_INCREF(__pyx_t_2); __pyx_t_3 = 0;
     for (;;) {
       if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_2)) break;
       #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-      __pyx_t_4 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_4); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 575, __pyx_L5_error)
+      __pyx_t_4 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_4); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 587, __pyx_L5_error)
       #else
-      __pyx_t_4 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 575, __pyx_L5_error)
+      __pyx_t_4 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 587, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_4);
       #endif
-      __Pyx_XDECREF_SET(__pyx_7genexpr__pyx_v_v, __pyx_t_4);
+      __Pyx_XDECREF_SET(__pyx_8genexpr2__pyx_v_v, __pyx_t_4);
       __pyx_t_4 = 0;
-      __pyx_t_4 = PyTuple_New(5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 575, __pyx_L5_error)
+      __pyx_t_4 = PyTuple_New(5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 587, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_5 = 0;
       __pyx_t_6 = 127;
       __Pyx_INCREF(__pyx_kp_u__16);
       __pyx_t_5 += 1;
       __Pyx_GIVEREF(__pyx_kp_u__16);
       PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_kp_u__16);
-      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_7genexpr__pyx_v_v, __pyx_n_s_x); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 575, __pyx_L5_error)
+      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_8genexpr2__pyx_v_v, __pyx_n_s_x); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 587, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_7);
-      __pyx_t_8 = __Pyx_PyObject_Format(__pyx_t_7, __pyx_kp_u_2f); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 575, __pyx_L5_error)
+      __pyx_t_8 = __Pyx_PyObject_Format(__pyx_t_7, __pyx_kp_u_2f); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 587, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __pyx_t_6 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_8) > __pyx_t_6) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_8) : __pyx_t_6;
       __pyx_t_5 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_8);
       __Pyx_GIVEREF(__pyx_t_8);
       PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_8);
       __pyx_t_8 = 0;
       __Pyx_INCREF(__pyx_kp_u__4);
       __pyx_t_5 += 2;
       __Pyx_GIVEREF(__pyx_kp_u__4);
       PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_kp_u__4);
-      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_7genexpr__pyx_v_v, __pyx_n_s_y); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 575, __pyx_L5_error)
+      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_8genexpr2__pyx_v_v, __pyx_n_s_y); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 587, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_8);
-      __pyx_t_7 = __Pyx_PyObject_Format(__pyx_t_8, __pyx_kp_u_2f); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 575, __pyx_L5_error)
+      __pyx_t_7 = __Pyx_PyObject_Format(__pyx_t_8, __pyx_kp_u_2f); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 587, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __pyx_t_6 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) > __pyx_t_6) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) : __pyx_t_6;
       __pyx_t_5 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
       __Pyx_GIVEREF(__pyx_t_7);
       PyTuple_SET_ITEM(__pyx_t_4, 3, __pyx_t_7);
       __pyx_t_7 = 0;
       __Pyx_INCREF(__pyx_kp_u__5);
       __pyx_t_5 += 1;
       __Pyx_GIVEREF(__pyx_kp_u__5);
       PyTuple_SET_ITEM(__pyx_t_4, 4, __pyx_kp_u__5);
-      __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_4, 5, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 575, __pyx_L5_error)
+      __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_4, 5, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 587, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_7))) __PYX_ERR(0, 575, __pyx_L5_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_7))) __PYX_ERR(0, 587, __pyx_L5_error)
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_XDECREF(__pyx_7genexpr__pyx_v_v); __pyx_7genexpr__pyx_v_v = 0;
+    __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_v); __pyx_8genexpr2__pyx_v_v = 0;
     goto __pyx_L8_exit_scope;
     __pyx_L5_error:;
-    __Pyx_XDECREF(__pyx_7genexpr__pyx_v_v); __pyx_7genexpr__pyx_v_v = 0;
+    __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_v); __pyx_8genexpr2__pyx_v_v = 0;
     goto __pyx_L1_error;
     __pyx_L8_exit_scope:;
   } /* exit inner scope */
   __pyx_v_s = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "easyvec/geometry.pyx":576
+  /* "easyvec/geometry.pyx":588
  *     def __str__(self):
  *         s = [f'({v.x:.2f}, {v.y:.2f})' for v in self.vecs]
  *         s = ', '.join(s)             # <<<<<<<<<<<<<<
  *         return f'PolyLine({s})'
  * 
  */
-  __pyx_t_1 = PyUnicode_Join(__pyx_kp_u__4, __pyx_v_s); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 576, __pyx_L1_error)
+  __pyx_t_1 = PyUnicode_Join(__pyx_kp_u__4, __pyx_v_s); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 588, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF_SET(__pyx_v_s, __pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "easyvec/geometry.pyx":577
+  /* "easyvec/geometry.pyx":589
  *         s = [f'({v.x:.2f}, {v.y:.2f})' for v in self.vecs]
  *         s = ', '.join(s)
  *         return f'PolyLine({s})'             # <<<<<<<<<<<<<<
  * 
  *     def __repr__(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 577, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 589, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_3 = 0;
   __pyx_t_6 = 127;
   __Pyx_INCREF(__pyx_kp_u_PolyLine);
   __pyx_t_3 += 9;
   __Pyx_GIVEREF(__pyx_kp_u_PolyLine);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_kp_u_PolyLine);
-  __pyx_t_2 = __Pyx_PyObject_FormatSimple(__pyx_v_s, __pyx_empty_unicode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 577, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_FormatSimple(__pyx_v_s, __pyx_empty_unicode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 589, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_6 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_2) > __pyx_t_6) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_2) : __pyx_t_6;
   __pyx_t_3 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_2);
   __pyx_t_2 = 0;
   __Pyx_INCREF(__pyx_kp_u__5);
   __pyx_t_3 += 1;
   __Pyx_GIVEREF(__pyx_kp_u__5);
   PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_kp_u__5);
-  __pyx_t_2 = __Pyx_PyUnicode_Join(__pyx_t_1, 3, __pyx_t_3, __pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 577, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyUnicode_Join(__pyx_t_1, 3, __pyx_t_3, __pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 589, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "easyvec/geometry.pyx":574
- *         self.bbox = Rect.bbox(self.vecs)
+  /* "easyvec/geometry.pyx":586
+ *         }
  * 
  *     def __str__(self):             # <<<<<<<<<<<<<<
  *         s = [f'({v.x:.2f}, {v.y:.2f})' for v in self.vecs]
  *         s = ', '.join(s)
  */
 
   /* function exit code */
@@ -15599,191 +15932,191 @@
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_8);
   __Pyx_AddTraceback("easyvec.geometry.PolyLine.__str__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_s);
-  __Pyx_XDECREF(__pyx_7genexpr__pyx_v_v);
+  __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_v);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "easyvec/geometry.pyx":579
+/* "easyvec/geometry.pyx":591
  *         return f'PolyLine({s})'
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         s = [f'({v.x}, {v.y})' for v in self.vecs]
  *         s = ', '.join(s)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_5__repr__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_5__repr__(PyObject *__pyx_v_self) {
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_9__repr__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_9__repr__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__repr__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_7easyvec_8geometry_8PolyLine_4__repr__(((struct __pyx_obj_7easyvec_8geometry_PolyLine *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7easyvec_8geometry_8PolyLine_8__repr__(((struct __pyx_obj_7easyvec_8geometry_PolyLine *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_4__repr__(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self) {
+static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_8__repr__(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self) {
   PyObject *__pyx_v_s = NULL;
-  PyObject *__pyx_8genexpr1__pyx_v_v = NULL;
+  PyObject *__pyx_8genexpr3__pyx_v_v = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   Py_ssize_t __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   Py_ssize_t __pyx_t_5;
   Py_UCS4 __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   __Pyx_RefNannySetupContext("__repr__", 0);
 
-  /* "easyvec/geometry.pyx":580
+  /* "easyvec/geometry.pyx":592
  * 
  *     def __repr__(self):
  *         s = [f'({v.x}, {v.y})' for v in self.vecs]             # <<<<<<<<<<<<<<
  *         s = ', '.join(s)
  *         return f'PolyLine(vecs=[{s}], enclosed={self.enclosed})'
  */
   { /* enter inner scope */
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 580, __pyx_L5_error)
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 592, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_1);
     if (unlikely(__pyx_v_self->vecs == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-      __PYX_ERR(0, 580, __pyx_L5_error)
+      __PYX_ERR(0, 592, __pyx_L5_error)
     }
     __pyx_t_2 = __pyx_v_self->vecs; __Pyx_INCREF(__pyx_t_2); __pyx_t_3 = 0;
     for (;;) {
       if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_2)) break;
       #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-      __pyx_t_4 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_4); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 580, __pyx_L5_error)
+      __pyx_t_4 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_4); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 592, __pyx_L5_error)
       #else
-      __pyx_t_4 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 580, __pyx_L5_error)
+      __pyx_t_4 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 592, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_4);
       #endif
-      __Pyx_XDECREF_SET(__pyx_8genexpr1__pyx_v_v, __pyx_t_4);
+      __Pyx_XDECREF_SET(__pyx_8genexpr3__pyx_v_v, __pyx_t_4);
       __pyx_t_4 = 0;
-      __pyx_t_4 = PyTuple_New(5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 580, __pyx_L5_error)
+      __pyx_t_4 = PyTuple_New(5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 592, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_5 = 0;
       __pyx_t_6 = 127;
       __Pyx_INCREF(__pyx_kp_u__16);
       __pyx_t_5 += 1;
       __Pyx_GIVEREF(__pyx_kp_u__16);
       PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_kp_u__16);
-      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_8genexpr1__pyx_v_v, __pyx_n_s_x); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 580, __pyx_L5_error)
+      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_8genexpr3__pyx_v_v, __pyx_n_s_x); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 592, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_7);
-      __pyx_t_8 = __Pyx_PyObject_FormatSimple(__pyx_t_7, __pyx_empty_unicode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 580, __pyx_L5_error)
+      __pyx_t_8 = __Pyx_PyObject_FormatSimple(__pyx_t_7, __pyx_empty_unicode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 592, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __pyx_t_6 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_8) > __pyx_t_6) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_8) : __pyx_t_6;
       __pyx_t_5 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_8);
       __Pyx_GIVEREF(__pyx_t_8);
       PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_8);
       __pyx_t_8 = 0;
       __Pyx_INCREF(__pyx_kp_u__4);
       __pyx_t_5 += 2;
       __Pyx_GIVEREF(__pyx_kp_u__4);
       PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_kp_u__4);
-      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_8genexpr1__pyx_v_v, __pyx_n_s_y); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 580, __pyx_L5_error)
+      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_8genexpr3__pyx_v_v, __pyx_n_s_y); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 592, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_8);
-      __pyx_t_7 = __Pyx_PyObject_FormatSimple(__pyx_t_8, __pyx_empty_unicode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 580, __pyx_L5_error)
+      __pyx_t_7 = __Pyx_PyObject_FormatSimple(__pyx_t_8, __pyx_empty_unicode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 592, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __pyx_t_6 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) > __pyx_t_6) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) : __pyx_t_6;
       __pyx_t_5 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
       __Pyx_GIVEREF(__pyx_t_7);
       PyTuple_SET_ITEM(__pyx_t_4, 3, __pyx_t_7);
       __pyx_t_7 = 0;
       __Pyx_INCREF(__pyx_kp_u__5);
       __pyx_t_5 += 1;
       __Pyx_GIVEREF(__pyx_kp_u__5);
       PyTuple_SET_ITEM(__pyx_t_4, 4, __pyx_kp_u__5);
-      __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_4, 5, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 580, __pyx_L5_error)
+      __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_4, 5, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 592, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_7))) __PYX_ERR(0, 580, __pyx_L5_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_7))) __PYX_ERR(0, 592, __pyx_L5_error)
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_v); __pyx_8genexpr1__pyx_v_v = 0;
+    __Pyx_XDECREF(__pyx_8genexpr3__pyx_v_v); __pyx_8genexpr3__pyx_v_v = 0;
     goto __pyx_L8_exit_scope;
     __pyx_L5_error:;
-    __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_v); __pyx_8genexpr1__pyx_v_v = 0;
+    __Pyx_XDECREF(__pyx_8genexpr3__pyx_v_v); __pyx_8genexpr3__pyx_v_v = 0;
     goto __pyx_L1_error;
     __pyx_L8_exit_scope:;
   } /* exit inner scope */
   __pyx_v_s = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "easyvec/geometry.pyx":581
+  /* "easyvec/geometry.pyx":593
  *     def __repr__(self):
  *         s = [f'({v.x}, {v.y})' for v in self.vecs]
  *         s = ', '.join(s)             # <<<<<<<<<<<<<<
  *         return f'PolyLine(vecs=[{s}], enclosed={self.enclosed})'
  * 
  */
-  __pyx_t_1 = PyUnicode_Join(__pyx_kp_u__4, __pyx_v_s); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 581, __pyx_L1_error)
+  __pyx_t_1 = PyUnicode_Join(__pyx_kp_u__4, __pyx_v_s); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 593, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF_SET(__pyx_v_s, __pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "easyvec/geometry.pyx":582
+  /* "easyvec/geometry.pyx":594
  *         s = [f'({v.x}, {v.y})' for v in self.vecs]
  *         s = ', '.join(s)
  *         return f'PolyLine(vecs=[{s}], enclosed={self.enclosed})'             # <<<<<<<<<<<<<<
  * 
  *     @cython.nonecheck(False)
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyTuple_New(5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 582, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 594, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_3 = 0;
   __pyx_t_6 = 127;
   __Pyx_INCREF(__pyx_kp_u_PolyLine_vecs);
   __pyx_t_3 += 15;
   __Pyx_GIVEREF(__pyx_kp_u_PolyLine_vecs);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_kp_u_PolyLine_vecs);
-  __pyx_t_2 = __Pyx_PyObject_FormatSimple(__pyx_v_s, __pyx_empty_unicode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 582, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_FormatSimple(__pyx_v_s, __pyx_empty_unicode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 594, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_6 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_2) > __pyx_t_6) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_2) : __pyx_t_6;
   __pyx_t_3 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_2);
   __pyx_t_2 = 0;
   __Pyx_INCREF(__pyx_kp_u_enclosed_2);
   __pyx_t_3 += 12;
   __Pyx_GIVEREF(__pyx_kp_u_enclosed_2);
   PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_kp_u_enclosed_2);
-  __pyx_t_2 = __Pyx_PyUnicode_FromBInt_int(__pyx_v_self->enclosed); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 582, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyUnicode_FromBInt_int(__pyx_v_self->enclosed); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 594, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_1, 3, __pyx_t_2);
   __pyx_t_2 = 0;
   __Pyx_INCREF(__pyx_kp_u__5);
   __pyx_t_3 += 1;
   __Pyx_GIVEREF(__pyx_kp_u__5);
   PyTuple_SET_ITEM(__pyx_t_1, 4, __pyx_kp_u__5);
-  __pyx_t_2 = __Pyx_PyUnicode_Join(__pyx_t_1, 5, __pyx_t_3, __pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 582, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyUnicode_Join(__pyx_t_1, 5, __pyx_t_3, __pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 594, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "easyvec/geometry.pyx":579
+  /* "easyvec/geometry.pyx":591
  *         return f'PolyLine({s})'
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         s = [f'({v.x}, {v.y})' for v in self.vecs]
  *         s = ', '.join(s)
  */
 
@@ -15794,29 +16127,29 @@
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_8);
   __Pyx_AddTraceback("easyvec.geometry.PolyLine.__repr__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_s);
-  __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_v);
+  __Pyx_XDECREF(__pyx_8genexpr3__pyx_v_v);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "easyvec/geometry.pyx":587
+/* "easyvec/geometry.pyx":599
  *     @cython.boundscheck(False)
  *     @cython.wraparound(False)
  *     cpdef list intersect_general(self, Vec2 p1, Vec2 p2, real f_low, real f_high, bint sortreduce=True):             # <<<<<<<<<<<<<<
  *         cdef list res = []
  *         if self.bbox.intersect_general(p1, p2, f_low, f_high) is None:
  */
 
-static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_7intersect_general(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_11intersect_general(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_f_7easyvec_8geometry_8PolyLine_intersect_general(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p2, __pyx_t_7easyvec_7vectors_real __pyx_v_f_low, __pyx_t_7easyvec_7vectors_real __pyx_v_f_high, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_opt_args_7easyvec_8geometry_8PolyLine_intersect_general *__pyx_optional_args) {
   int __pyx_v_sortreduce = ((int)1);
   PyObject *__pyx_v_res = 0;
   int __pyx_v_i;
   struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_v1 = 0;
   struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_v2 = 0;
   struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_v_cr = 0;
@@ -15827,134 +16160,134 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
   int __pyx_t_5;
   int __pyx_t_6;
-  __pyx_ctuple_d78dc__int__and___dunderpyx_t_7easyvec_7vectors_real__and___dunderpyx_t_7easyvec_7vectors_real__etc __pyx_t_7;
+  __pyx_ctuple_acdc9__int__and___dunderpyx_t_7easyvec_7vectors_real__and___dunderpyx_t_7easyvec_7vectors_real__etc __pyx_t_7;
   __pyx_t_7easyvec_7vectors_real __pyx_t_8;
   __pyx_t_7easyvec_7vectors_real __pyx_t_9;
   int __pyx_t_10;
   PyObject *__pyx_t_11 = NULL;
   int __pyx_t_12;
   __Pyx_RefNannySetupContext("intersect_general", 0);
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_sortreduce = __pyx_optional_args->sortreduce;
     }
   }
 
-  /* "easyvec/geometry.pyx":588
+  /* "easyvec/geometry.pyx":600
  *     @cython.wraparound(False)
  *     cpdef list intersect_general(self, Vec2 p1, Vec2 p2, real f_low, real f_high, bint sortreduce=True):
  *         cdef list res = []             # <<<<<<<<<<<<<<
  *         if self.bbox.intersect_general(p1, p2, f_low, f_high) is None:
  *             return res
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 588, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 600, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_res = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "easyvec/geometry.pyx":589
+  /* "easyvec/geometry.pyx":601
  *     cpdef list intersect_general(self, Vec2 p1, Vec2 p2, real f_low, real f_high, bint sortreduce=True):
  *         cdef list res = []
  *         if self.bbox.intersect_general(p1, p2, f_low, f_high) is None:             # <<<<<<<<<<<<<<
  *             return res
  *         cdef int i
  */
-  __pyx_t_1 = ((PyObject *)__pyx_f_7easyvec_8geometry_4Rect_intersect_general(__pyx_v_self->bbox, __pyx_v_p1, __pyx_v_p2, __pyx_v_f_low, __pyx_v_f_high, 0, NULL)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 589, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)__pyx_f_7easyvec_8geometry_4Rect_intersect_general(__pyx_v_self->bbox, __pyx_v_p1, __pyx_v_p2, __pyx_v_f_low, __pyx_v_f_high, 0, NULL)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 601, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = (__pyx_t_1 == Py_None);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
-    /* "easyvec/geometry.pyx":590
+    /* "easyvec/geometry.pyx":602
  *         cdef list res = []
  *         if self.bbox.intersect_general(p1, p2, f_low, f_high) is None:
  *             return res             # <<<<<<<<<<<<<<
  *         cdef int i
  *         cdef Vec2 v1, v2, v_cr
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_v_res);
     __pyx_r = __pyx_v_res;
     goto __pyx_L0;
 
-    /* "easyvec/geometry.pyx":589
+    /* "easyvec/geometry.pyx":601
  *     cpdef list intersect_general(self, Vec2 p1, Vec2 p2, real f_low, real f_high, bint sortreduce=True):
  *         cdef list res = []
  *         if self.bbox.intersect_general(p1, p2, f_low, f_high) is None:             # <<<<<<<<<<<<<<
  *             return res
  *         cdef int i
  */
   }
 
-  /* "easyvec/geometry.pyx":595
+  /* "easyvec/geometry.pyx":607
  *         cdef bint inter
  *         cdef real t1, t2
  *         v1 = <Vec2>(self.vecs[0])             # <<<<<<<<<<<<<<
  *         for i in range(1, self.vlen):
  *             v2 = <Vec2>(self.vecs[i])
  */
   if (unlikely(__pyx_v_self->vecs == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 595, __pyx_L1_error)
+    __PYX_ERR(0, 607, __pyx_L1_error)
   }
   __pyx_t_1 = PyList_GET_ITEM(__pyx_v_self->vecs, 0);
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v_v1 = ((struct __pyx_obj_7easyvec_7vectors_Vec2 *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "easyvec/geometry.pyx":596
+  /* "easyvec/geometry.pyx":608
  *         cdef real t1, t2
  *         v1 = <Vec2>(self.vecs[0])
  *         for i in range(1, self.vlen):             # <<<<<<<<<<<<<<
  *             v2 = <Vec2>(self.vecs[i])
  *             inter, t1, t2 = _intersect_ts(p1, p2, v1, v2)
  */
   __pyx_t_4 = __pyx_v_self->vlen;
   __pyx_t_5 = __pyx_t_4;
   for (__pyx_t_6 = 1; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
     __pyx_v_i = __pyx_t_6;
 
-    /* "easyvec/geometry.pyx":597
+    /* "easyvec/geometry.pyx":609
  *         v1 = <Vec2>(self.vecs[0])
  *         for i in range(1, self.vlen):
  *             v2 = <Vec2>(self.vecs[i])             # <<<<<<<<<<<<<<
  *             inter, t1, t2 = _intersect_ts(p1, p2, v1, v2)
  *             if inter and (0.0 <= t2 <= 1.0) and (f_low <= t1 <= f_high):
  */
     if (unlikely(__pyx_v_self->vecs == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 597, __pyx_L1_error)
+      __PYX_ERR(0, 609, __pyx_L1_error)
     }
     __pyx_t_1 = PyList_GET_ITEM(__pyx_v_self->vecs, __pyx_v_i);
     __Pyx_INCREF(__pyx_t_1);
     __Pyx_XDECREF_SET(__pyx_v_v2, ((struct __pyx_obj_7easyvec_7vectors_Vec2 *)__pyx_t_1));
     __pyx_t_1 = 0;
 
-    /* "easyvec/geometry.pyx":598
+    /* "easyvec/geometry.pyx":610
  *         for i in range(1, self.vlen):
  *             v2 = <Vec2>(self.vecs[i])
  *             inter, t1, t2 = _intersect_ts(p1, p2, v1, v2)             # <<<<<<<<<<<<<<
  *             if inter and (0.0 <= t2 <= 1.0) and (f_low <= t1 <= f_high):
  *                 v_cr = p1.add( p2.sub(p1).mul_num(t1) )
  */
     __pyx_t_7 = __pyx_f_7easyvec_8geometry__intersect_ts(__pyx_v_p1, __pyx_v_p2, __pyx_v_v1, __pyx_v_v2, 0);
     __pyx_t_3 = __pyx_t_7.f0;
     __pyx_t_8 = __pyx_t_7.f1;
     __pyx_t_9 = __pyx_t_7.f2;
     __pyx_v_inter = __pyx_t_3;
     __pyx_v_t1 = __pyx_t_8;
     __pyx_v_t2 = __pyx_t_9;
 
-    /* "easyvec/geometry.pyx":599
+    /* "easyvec/geometry.pyx":611
  *             v2 = <Vec2>(self.vecs[i])
  *             inter, t1, t2 = _intersect_ts(p1, p2, v1, v2)
  *             if inter and (0.0 <= t2 <= 1.0) and (f_low <= t1 <= f_high):             # <<<<<<<<<<<<<<
  *                 v_cr = p1.add( p2.sub(p1).mul_num(t1) )
  *                 res.append(v_cr)
  */
     __pyx_t_2 = (__pyx_v_inter != 0);
@@ -15978,103 +16311,103 @@
       __pyx_t_10 = (__pyx_v_t1 <= __pyx_v_f_high);
     }
     __pyx_t_2 = (__pyx_t_10 != 0);
     __pyx_t_3 = __pyx_t_2;
     __pyx_L7_bool_binop_done:;
     if (__pyx_t_3) {
 
-      /* "easyvec/geometry.pyx":600
+      /* "easyvec/geometry.pyx":612
  *             inter, t1, t2 = _intersect_ts(p1, p2, v1, v2)
  *             if inter and (0.0 <= t2 <= 1.0) and (f_low <= t1 <= f_high):
  *                 v_cr = p1.add( p2.sub(p1).mul_num(t1) )             # <<<<<<<<<<<<<<
  *                 res.append(v_cr)
  *             v1 = v2
  */
-      __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_7easyvec_7vectors_Vec2 *)__pyx_v_p2->__pyx_vtab)->sub(__pyx_v_p2, __pyx_v_p1, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 600, __pyx_L1_error)
+      __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_7easyvec_7vectors_Vec2 *)__pyx_v_p2->__pyx_vtab)->sub(__pyx_v_p2, __pyx_v_p1, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 612, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_11 = ((PyObject *)((struct __pyx_vtabstruct_7easyvec_7vectors_Vec2 *)((struct __pyx_obj_7easyvec_7vectors_Vec2 *)__pyx_t_1)->__pyx_vtab)->mul_num(((struct __pyx_obj_7easyvec_7vectors_Vec2 *)__pyx_t_1), __pyx_v_t1, 0)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 600, __pyx_L1_error)
+      __pyx_t_11 = ((PyObject *)((struct __pyx_vtabstruct_7easyvec_7vectors_Vec2 *)((struct __pyx_obj_7easyvec_7vectors_Vec2 *)__pyx_t_1)->__pyx_vtab)->mul_num(((struct __pyx_obj_7easyvec_7vectors_Vec2 *)__pyx_t_1), __pyx_v_t1, 0)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 612, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_7easyvec_7vectors_Vec2 *)__pyx_v_p1->__pyx_vtab)->add(__pyx_v_p1, ((struct __pyx_obj_7easyvec_7vectors_Vec2 *)__pyx_t_11), 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 600, __pyx_L1_error)
+      __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_7easyvec_7vectors_Vec2 *)__pyx_v_p1->__pyx_vtab)->add(__pyx_v_p1, ((struct __pyx_obj_7easyvec_7vectors_Vec2 *)__pyx_t_11), 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 612, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
       __Pyx_XDECREF_SET(__pyx_v_v_cr, ((struct __pyx_obj_7easyvec_7vectors_Vec2 *)__pyx_t_1));
       __pyx_t_1 = 0;
 
-      /* "easyvec/geometry.pyx":601
+      /* "easyvec/geometry.pyx":613
  *             if inter and (0.0 <= t2 <= 1.0) and (f_low <= t1 <= f_high):
  *                 v_cr = p1.add( p2.sub(p1).mul_num(t1) )
  *                 res.append(v_cr)             # <<<<<<<<<<<<<<
  *             v1 = v2
  *         if self.enclosed:
  */
-      __pyx_t_12 = __Pyx_PyList_Append(__pyx_v_res, ((PyObject *)__pyx_v_v_cr)); if (unlikely(__pyx_t_12 == ((int)-1))) __PYX_ERR(0, 601, __pyx_L1_error)
+      __pyx_t_12 = __Pyx_PyList_Append(__pyx_v_res, ((PyObject *)__pyx_v_v_cr)); if (unlikely(__pyx_t_12 == ((int)-1))) __PYX_ERR(0, 613, __pyx_L1_error)
 
-      /* "easyvec/geometry.pyx":599
+      /* "easyvec/geometry.pyx":611
  *             v2 = <Vec2>(self.vecs[i])
  *             inter, t1, t2 = _intersect_ts(p1, p2, v1, v2)
  *             if inter and (0.0 <= t2 <= 1.0) and (f_low <= t1 <= f_high):             # <<<<<<<<<<<<<<
  *                 v_cr = p1.add( p2.sub(p1).mul_num(t1) )
  *                 res.append(v_cr)
  */
     }
 
-    /* "easyvec/geometry.pyx":602
+    /* "easyvec/geometry.pyx":614
  *                 v_cr = p1.add( p2.sub(p1).mul_num(t1) )
  *                 res.append(v_cr)
  *             v1 = v2             # <<<<<<<<<<<<<<
  *         if self.enclosed:
  *             v2 = <Vec2>(self.vecs[0])
  */
     __Pyx_INCREF(((PyObject *)__pyx_v_v2));
     __Pyx_DECREF_SET(__pyx_v_v1, __pyx_v_v2);
   }
 
-  /* "easyvec/geometry.pyx":603
+  /* "easyvec/geometry.pyx":615
  *                 res.append(v_cr)
  *             v1 = v2
  *         if self.enclosed:             # <<<<<<<<<<<<<<
  *             v2 = <Vec2>(self.vecs[0])
  *             inter, t1, t2 = _intersect_ts(p1, p2, v1, v2)
  */
   __pyx_t_3 = (__pyx_v_self->enclosed != 0);
   if (__pyx_t_3) {
 
-    /* "easyvec/geometry.pyx":604
+    /* "easyvec/geometry.pyx":616
  *             v1 = v2
  *         if self.enclosed:
  *             v2 = <Vec2>(self.vecs[0])             # <<<<<<<<<<<<<<
  *             inter, t1, t2 = _intersect_ts(p1, p2, v1, v2)
  *             if inter and (0.0 <= t2 <= 1.0) and (f_low <= t1 <= f_high):
  */
     if (unlikely(__pyx_v_self->vecs == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 604, __pyx_L1_error)
+      __PYX_ERR(0, 616, __pyx_L1_error)
     }
     __pyx_t_1 = PyList_GET_ITEM(__pyx_v_self->vecs, 0);
     __Pyx_INCREF(__pyx_t_1);
     __Pyx_XDECREF_SET(__pyx_v_v2, ((struct __pyx_obj_7easyvec_7vectors_Vec2 *)__pyx_t_1));
     __pyx_t_1 = 0;
 
-    /* "easyvec/geometry.pyx":605
+    /* "easyvec/geometry.pyx":617
  *         if self.enclosed:
  *             v2 = <Vec2>(self.vecs[0])
  *             inter, t1, t2 = _intersect_ts(p1, p2, v1, v2)             # <<<<<<<<<<<<<<
  *             if inter and (0.0 <= t2 <= 1.0) and (f_low <= t1 <= f_high):
  *                 v_cr = p1.add( p2.sub(p1).mul_num(t1) )
  */
     __pyx_t_7 = __pyx_f_7easyvec_8geometry__intersect_ts(__pyx_v_p1, __pyx_v_p2, __pyx_v_v1, __pyx_v_v2, 0);
     __pyx_t_3 = __pyx_t_7.f0;
     __pyx_t_9 = __pyx_t_7.f1;
     __pyx_t_8 = __pyx_t_7.f2;
     __pyx_v_inter = __pyx_t_3;
     __pyx_v_t1 = __pyx_t_9;
     __pyx_v_t2 = __pyx_t_8;
 
-    /* "easyvec/geometry.pyx":606
+    /* "easyvec/geometry.pyx":618
  *             v2 = <Vec2>(self.vecs[0])
  *             inter, t1, t2 = _intersect_ts(p1, p2, v1, v2)
  *             if inter and (0.0 <= t2 <= 1.0) and (f_low <= t1 <= f_high):             # <<<<<<<<<<<<<<
  *                 v_cr = p1.add( p2.sub(p1).mul_num(t1) )
  *                 res.append(v_cr)
  */
     __pyx_t_2 = (__pyx_v_inter != 0);
@@ -16098,105 +16431,105 @@
       __pyx_t_10 = (__pyx_v_t1 <= __pyx_v_f_high);
     }
     __pyx_t_2 = (__pyx_t_10 != 0);
     __pyx_t_3 = __pyx_t_2;
     __pyx_L12_bool_binop_done:;
     if (__pyx_t_3) {
 
-      /* "easyvec/geometry.pyx":607
+      /* "easyvec/geometry.pyx":619
  *             inter, t1, t2 = _intersect_ts(p1, p2, v1, v2)
  *             if inter and (0.0 <= t2 <= 1.0) and (f_low <= t1 <= f_high):
  *                 v_cr = p1.add( p2.sub(p1).mul_num(t1) )             # <<<<<<<<<<<<<<
  *                 res.append(v_cr)
  *         if sortreduce:
  */
-      __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_7easyvec_7vectors_Vec2 *)__pyx_v_p2->__pyx_vtab)->sub(__pyx_v_p2, __pyx_v_p1, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 607, __pyx_L1_error)
+      __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_7easyvec_7vectors_Vec2 *)__pyx_v_p2->__pyx_vtab)->sub(__pyx_v_p2, __pyx_v_p1, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 619, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_11 = ((PyObject *)((struct __pyx_vtabstruct_7easyvec_7vectors_Vec2 *)((struct __pyx_obj_7easyvec_7vectors_Vec2 *)__pyx_t_1)->__pyx_vtab)->mul_num(((struct __pyx_obj_7easyvec_7vectors_Vec2 *)__pyx_t_1), __pyx_v_t1, 0)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 607, __pyx_L1_error)
+      __pyx_t_11 = ((PyObject *)((struct __pyx_vtabstruct_7easyvec_7vectors_Vec2 *)((struct __pyx_obj_7easyvec_7vectors_Vec2 *)__pyx_t_1)->__pyx_vtab)->mul_num(((struct __pyx_obj_7easyvec_7vectors_Vec2 *)__pyx_t_1), __pyx_v_t1, 0)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 619, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_7easyvec_7vectors_Vec2 *)__pyx_v_p1->__pyx_vtab)->add(__pyx_v_p1, ((struct __pyx_obj_7easyvec_7vectors_Vec2 *)__pyx_t_11), 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 607, __pyx_L1_error)
+      __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_7easyvec_7vectors_Vec2 *)__pyx_v_p1->__pyx_vtab)->add(__pyx_v_p1, ((struct __pyx_obj_7easyvec_7vectors_Vec2 *)__pyx_t_11), 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 619, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
       __Pyx_XDECREF_SET(__pyx_v_v_cr, ((struct __pyx_obj_7easyvec_7vectors_Vec2 *)__pyx_t_1));
       __pyx_t_1 = 0;
 
-      /* "easyvec/geometry.pyx":608
+      /* "easyvec/geometry.pyx":620
  *             if inter and (0.0 <= t2 <= 1.0) and (f_low <= t1 <= f_high):
  *                 v_cr = p1.add( p2.sub(p1).mul_num(t1) )
  *                 res.append(v_cr)             # <<<<<<<<<<<<<<
  *         if sortreduce:
  *             return _sortreduce_by_distance(res, p1)
  */
-      __pyx_t_12 = __Pyx_PyList_Append(__pyx_v_res, ((PyObject *)__pyx_v_v_cr)); if (unlikely(__pyx_t_12 == ((int)-1))) __PYX_ERR(0, 608, __pyx_L1_error)
+      __pyx_t_12 = __Pyx_PyList_Append(__pyx_v_res, ((PyObject *)__pyx_v_v_cr)); if (unlikely(__pyx_t_12 == ((int)-1))) __PYX_ERR(0, 620, __pyx_L1_error)
 
-      /* "easyvec/geometry.pyx":606
+      /* "easyvec/geometry.pyx":618
  *             v2 = <Vec2>(self.vecs[0])
  *             inter, t1, t2 = _intersect_ts(p1, p2, v1, v2)
  *             if inter and (0.0 <= t2 <= 1.0) and (f_low <= t1 <= f_high):             # <<<<<<<<<<<<<<
  *                 v_cr = p1.add( p2.sub(p1).mul_num(t1) )
  *                 res.append(v_cr)
  */
     }
 
-    /* "easyvec/geometry.pyx":603
+    /* "easyvec/geometry.pyx":615
  *                 res.append(v_cr)
  *             v1 = v2
  *         if self.enclosed:             # <<<<<<<<<<<<<<
  *             v2 = <Vec2>(self.vecs[0])
  *             inter, t1, t2 = _intersect_ts(p1, p2, v1, v2)
  */
   }
 
-  /* "easyvec/geometry.pyx":609
+  /* "easyvec/geometry.pyx":621
  *                 v_cr = p1.add( p2.sub(p1).mul_num(t1) )
  *                 res.append(v_cr)
  *         if sortreduce:             # <<<<<<<<<<<<<<
  *             return _sortreduce_by_distance(res, p1)
  *         return res
  */
   __pyx_t_3 = (__pyx_v_sortreduce != 0);
   if (__pyx_t_3) {
 
-    /* "easyvec/geometry.pyx":610
+    /* "easyvec/geometry.pyx":622
  *                 res.append(v_cr)
  *         if sortreduce:
  *             return _sortreduce_by_distance(res, p1)             # <<<<<<<<<<<<<<
  *         return res
  * 
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_1 = __pyx_f_7easyvec_8geometry__sortreduce_by_distance(__pyx_v_res, __pyx_v_p1, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 610, __pyx_L1_error)
+    __pyx_t_1 = __pyx_f_7easyvec_8geometry__sortreduce_by_distance(__pyx_v_res, __pyx_v_p1, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 622, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_r = ((PyObject*)__pyx_t_1);
     __pyx_t_1 = 0;
     goto __pyx_L0;
 
-    /* "easyvec/geometry.pyx":609
+    /* "easyvec/geometry.pyx":621
  *                 v_cr = p1.add( p2.sub(p1).mul_num(t1) )
  *                 res.append(v_cr)
  *         if sortreduce:             # <<<<<<<<<<<<<<
  *             return _sortreduce_by_distance(res, p1)
  *         return res
  */
   }
 
-  /* "easyvec/geometry.pyx":611
+  /* "easyvec/geometry.pyx":623
  *         if sortreduce:
  *             return _sortreduce_by_distance(res, p1)
  *         return res             # <<<<<<<<<<<<<<
  * 
  *     @cython.nonecheck(False)
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_res);
   __pyx_r = __pyx_v_res;
   goto __pyx_L0;
 
-  /* "easyvec/geometry.pyx":587
+  /* "easyvec/geometry.pyx":599
  *     @cython.boundscheck(False)
  *     @cython.wraparound(False)
  *     cpdef list intersect_general(self, Vec2 p1, Vec2 p2, real f_low, real f_high, bint sortreduce=True):             # <<<<<<<<<<<<<<
  *         cdef list res = []
  *         if self.bbox.intersect_general(p1, p2, f_low, f_high) is None:
  */
 
@@ -16213,17 +16546,17 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_v_cr);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_7intersect_general(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_7easyvec_8geometry_8PolyLine_6intersect_general[] = "PolyLine.intersect_general(self, Vec2 p1, Vec2 p2, real f_low, real f_high, bool sortreduce=True) -> list";
-static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_7intersect_general(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_11intersect_general(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_7easyvec_8geometry_8PolyLine_10intersect_general[] = "PolyLine.intersect_general(self, Vec2 p1, Vec2 p2, real f_low, real f_high, bool sortreduce=True) -> list";
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_11intersect_general(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p1 = 0;
   struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p2 = 0;
   __pyx_t_7easyvec_7vectors_real __pyx_v_f_low;
   __pyx_t_7easyvec_7vectors_real __pyx_v_f_high;
   int __pyx_v_sortreduce;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -16253,37 +16586,37 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_p1)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_p2)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("intersect_general", 0, 4, 5, 1); __PYX_ERR(0, 587, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("intersect_general", 0, 4, 5, 1); __PYX_ERR(0, 599, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_f_low)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("intersect_general", 0, 4, 5, 2); __PYX_ERR(0, 587, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("intersect_general", 0, 4, 5, 2); __PYX_ERR(0, 599, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_f_high)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("intersect_general", 0, 4, 5, 3); __PYX_ERR(0, 587, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("intersect_general", 0, 4, 5, 3); __PYX_ERR(0, 599, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_sortreduce);
           if (value) { values[4] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "intersect_general") < 0)) __PYX_ERR(0, 587, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "intersect_general") < 0)) __PYX_ERR(0, 599, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
@@ -16291,53 +16624,53 @@
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_p1 = ((struct __pyx_obj_7easyvec_7vectors_Vec2 *)values[0]);
     __pyx_v_p2 = ((struct __pyx_obj_7easyvec_7vectors_Vec2 *)values[1]);
-    __pyx_v_f_low = __pyx_PyFloat_AsDouble(values[2]); if (unlikely((__pyx_v_f_low == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 587, __pyx_L3_error)
-    __pyx_v_f_high = __pyx_PyFloat_AsDouble(values[3]); if (unlikely((__pyx_v_f_high == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 587, __pyx_L3_error)
+    __pyx_v_f_low = __pyx_PyFloat_AsDouble(values[2]); if (unlikely((__pyx_v_f_low == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 599, __pyx_L3_error)
+    __pyx_v_f_high = __pyx_PyFloat_AsDouble(values[3]); if (unlikely((__pyx_v_f_high == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 599, __pyx_L3_error)
     if (values[4]) {
-      __pyx_v_sortreduce = __Pyx_PyObject_IsTrue(values[4]); if (unlikely((__pyx_v_sortreduce == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 587, __pyx_L3_error)
+      __pyx_v_sortreduce = __Pyx_PyObject_IsTrue(values[4]); if (unlikely((__pyx_v_sortreduce == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 599, __pyx_L3_error)
     } else {
       __pyx_v_sortreduce = ((int)1);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("intersect_general", 0, 4, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 587, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("intersect_general", 0, 4, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 599, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("easyvec.geometry.PolyLine.intersect_general", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_p1), __pyx_ptype_7easyvec_7vectors_Vec2, 1, "p1", 0))) __PYX_ERR(0, 587, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_p2), __pyx_ptype_7easyvec_7vectors_Vec2, 1, "p2", 0))) __PYX_ERR(0, 587, __pyx_L1_error)
-  __pyx_r = __pyx_pf_7easyvec_8geometry_8PolyLine_6intersect_general(((struct __pyx_obj_7easyvec_8geometry_PolyLine *)__pyx_v_self), __pyx_v_p1, __pyx_v_p2, __pyx_v_f_low, __pyx_v_f_high, __pyx_v_sortreduce);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_p1), __pyx_ptype_7easyvec_7vectors_Vec2, 1, "p1", 0))) __PYX_ERR(0, 599, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_p2), __pyx_ptype_7easyvec_7vectors_Vec2, 1, "p2", 0))) __PYX_ERR(0, 599, __pyx_L1_error)
+  __pyx_r = __pyx_pf_7easyvec_8geometry_8PolyLine_10intersect_general(((struct __pyx_obj_7easyvec_8geometry_PolyLine *)__pyx_v_self), __pyx_v_p1, __pyx_v_p2, __pyx_v_f_low, __pyx_v_f_high, __pyx_v_sortreduce);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_6intersect_general(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p2, __pyx_t_7easyvec_7vectors_real __pyx_v_f_low, __pyx_t_7easyvec_7vectors_real __pyx_v_f_high, int __pyx_v_sortreduce) {
+static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_10intersect_general(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p2, __pyx_t_7easyvec_7vectors_real __pyx_v_f_low, __pyx_t_7easyvec_7vectors_real __pyx_v_f_high, int __pyx_v_sortreduce) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   struct __pyx_opt_args_7easyvec_8geometry_8PolyLine_intersect_general __pyx_t_2;
   __Pyx_RefNannySetupContext("intersect_general", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2.__pyx_n = 1;
   __pyx_t_2.sortreduce = __pyx_v_sortreduce;
-  __pyx_t_1 = __pyx_vtabptr_7easyvec_8geometry_PolyLine->intersect_general(__pyx_v_self, __pyx_v_p1, __pyx_v_p2, __pyx_v_f_low, __pyx_v_f_high, 1, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 587, __pyx_L1_error)
+  __pyx_t_1 = __pyx_vtabptr_7easyvec_8geometry_PolyLine->intersect_general(__pyx_v_self, __pyx_v_p1, __pyx_v_p2, __pyx_v_f_low, __pyx_v_f_high, 1, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 599, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -16346,53 +16679,53 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "easyvec/geometry.pyx":614
+/* "easyvec/geometry.pyx":626
  * 
  *     @cython.nonecheck(False)
  *     cpdef list intersect_line(self, Vec2 p1, Vec2 p2, bint sortreduce=True):             # <<<<<<<<<<<<<<
  *         return self.intersect_general(p1, p2, MINUS_BIG_REAL, BIG_REAL, sortreduce)
  * 
  */
 
-static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_9intersect_line(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_13intersect_line(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_f_7easyvec_8geometry_8PolyLine_intersect_line(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p2, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_opt_args_7easyvec_8geometry_8PolyLine_intersect_line *__pyx_optional_args) {
   int __pyx_v_sortreduce = ((int)1);
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   struct __pyx_opt_args_7easyvec_8geometry_8PolyLine_intersect_general __pyx_t_2;
   __Pyx_RefNannySetupContext("intersect_line", 0);
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_sortreduce = __pyx_optional_args->sortreduce;
     }
   }
 
-  /* "easyvec/geometry.pyx":615
+  /* "easyvec/geometry.pyx":627
  *     @cython.nonecheck(False)
  *     cpdef list intersect_line(self, Vec2 p1, Vec2 p2, bint sortreduce=True):
  *         return self.intersect_general(p1, p2, MINUS_BIG_REAL, BIG_REAL, sortreduce)             # <<<<<<<<<<<<<<
  * 
  *     @cython.nonecheck(False)
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2.__pyx_n = 1;
   __pyx_t_2.sortreduce = __pyx_v_sortreduce;
-  __pyx_t_1 = __pyx_f_7easyvec_8geometry_8PolyLine_intersect_general(__pyx_v_self, __pyx_v_p1, __pyx_v_p2, __pyx_v_7easyvec_7vectors_MINUS_BIG_REAL, __pyx_v_7easyvec_7vectors_BIG_REAL, 0, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 615, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_7easyvec_8geometry_8PolyLine_intersect_general(__pyx_v_self, __pyx_v_p1, __pyx_v_p2, __pyx_v_7easyvec_7vectors_MINUS_BIG_REAL, __pyx_v_7easyvec_7vectors_BIG_REAL, 0, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 627, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "easyvec/geometry.pyx":614
+  /* "easyvec/geometry.pyx":626
  * 
  *     @cython.nonecheck(False)
  *     cpdef list intersect_line(self, Vec2 p1, Vec2 p2, bint sortreduce=True):             # <<<<<<<<<<<<<<
  *         return self.intersect_general(p1, p2, MINUS_BIG_REAL, BIG_REAL, sortreduce)
  * 
  */
 
@@ -16404,17 +16737,17 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_9intersect_line(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_7easyvec_8geometry_8PolyLine_8intersect_line[] = "PolyLine.intersect_line(self, Vec2 p1, Vec2 p2, bool sortreduce=True) -> list";
-static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_9intersect_line(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_13intersect_line(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_7easyvec_8geometry_8PolyLine_12intersect_line[] = "PolyLine.intersect_line(self, Vec2 p1, Vec2 p2, bool sortreduce=True) -> list";
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_13intersect_line(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p1 = 0;
   struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p2 = 0;
   int __pyx_v_sortreduce;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("intersect_line (wrapper)", 0);
   {
@@ -16438,75 +16771,75 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_p1)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_p2)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("intersect_line", 0, 2, 3, 1); __PYX_ERR(0, 614, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("intersect_line", 0, 2, 3, 1); __PYX_ERR(0, 626, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_sortreduce);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "intersect_line") < 0)) __PYX_ERR(0, 614, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "intersect_line") < 0)) __PYX_ERR(0, 626, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_p1 = ((struct __pyx_obj_7easyvec_7vectors_Vec2 *)values[0]);
     __pyx_v_p2 = ((struct __pyx_obj_7easyvec_7vectors_Vec2 *)values[1]);
     if (values[2]) {
-      __pyx_v_sortreduce = __Pyx_PyObject_IsTrue(values[2]); if (unlikely((__pyx_v_sortreduce == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 614, __pyx_L3_error)
+      __pyx_v_sortreduce = __Pyx_PyObject_IsTrue(values[2]); if (unlikely((__pyx_v_sortreduce == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 626, __pyx_L3_error)
     } else {
       __pyx_v_sortreduce = ((int)1);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("intersect_line", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 614, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("intersect_line", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 626, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("easyvec.geometry.PolyLine.intersect_line", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_p1), __pyx_ptype_7easyvec_7vectors_Vec2, 1, "p1", 0))) __PYX_ERR(0, 614, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_p2), __pyx_ptype_7easyvec_7vectors_Vec2, 1, "p2", 0))) __PYX_ERR(0, 614, __pyx_L1_error)
-  __pyx_r = __pyx_pf_7easyvec_8geometry_8PolyLine_8intersect_line(((struct __pyx_obj_7easyvec_8geometry_PolyLine *)__pyx_v_self), __pyx_v_p1, __pyx_v_p2, __pyx_v_sortreduce);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_p1), __pyx_ptype_7easyvec_7vectors_Vec2, 1, "p1", 0))) __PYX_ERR(0, 626, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_p2), __pyx_ptype_7easyvec_7vectors_Vec2, 1, "p2", 0))) __PYX_ERR(0, 626, __pyx_L1_error)
+  __pyx_r = __pyx_pf_7easyvec_8geometry_8PolyLine_12intersect_line(((struct __pyx_obj_7easyvec_8geometry_PolyLine *)__pyx_v_self), __pyx_v_p1, __pyx_v_p2, __pyx_v_sortreduce);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_8intersect_line(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p2, int __pyx_v_sortreduce) {
+static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_12intersect_line(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p2, int __pyx_v_sortreduce) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   struct __pyx_opt_args_7easyvec_8geometry_8PolyLine_intersect_line __pyx_t_2;
   __Pyx_RefNannySetupContext("intersect_line", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2.__pyx_n = 1;
   __pyx_t_2.sortreduce = __pyx_v_sortreduce;
-  __pyx_t_1 = __pyx_vtabptr_7easyvec_8geometry_PolyLine->intersect_line(__pyx_v_self, __pyx_v_p1, __pyx_v_p2, 1, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 614, __pyx_L1_error)
+  __pyx_t_1 = __pyx_vtabptr_7easyvec_8geometry_PolyLine->intersect_line(__pyx_v_self, __pyx_v_p1, __pyx_v_p2, 1, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 626, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -16515,53 +16848,53 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "easyvec/geometry.pyx":618
+/* "easyvec/geometry.pyx":630
  * 
  *     @cython.nonecheck(False)
  *     cpdef list intersect_ray(self, Vec2 p1, Vec2 p2, bint sortreduce=True):             # <<<<<<<<<<<<<<
  *         return self.intersect_general(p1, p2, 0.0, BIG_REAL, sortreduce)
  * 
  */
 
-static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_11intersect_ray(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_15intersect_ray(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_f_7easyvec_8geometry_8PolyLine_intersect_ray(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p2, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_opt_args_7easyvec_8geometry_8PolyLine_intersect_ray *__pyx_optional_args) {
   int __pyx_v_sortreduce = ((int)1);
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   struct __pyx_opt_args_7easyvec_8geometry_8PolyLine_intersect_general __pyx_t_2;
   __Pyx_RefNannySetupContext("intersect_ray", 0);
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_sortreduce = __pyx_optional_args->sortreduce;
     }
   }
 
-  /* "easyvec/geometry.pyx":619
+  /* "easyvec/geometry.pyx":631
  *     @cython.nonecheck(False)
  *     cpdef list intersect_ray(self, Vec2 p1, Vec2 p2, bint sortreduce=True):
  *         return self.intersect_general(p1, p2, 0.0, BIG_REAL, sortreduce)             # <<<<<<<<<<<<<<
  * 
  *     @cython.nonecheck(False)
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2.__pyx_n = 1;
   __pyx_t_2.sortreduce = __pyx_v_sortreduce;
-  __pyx_t_1 = __pyx_f_7easyvec_8geometry_8PolyLine_intersect_general(__pyx_v_self, __pyx_v_p1, __pyx_v_p2, 0.0, __pyx_v_7easyvec_7vectors_BIG_REAL, 0, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 619, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_7easyvec_8geometry_8PolyLine_intersect_general(__pyx_v_self, __pyx_v_p1, __pyx_v_p2, 0.0, __pyx_v_7easyvec_7vectors_BIG_REAL, 0, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 631, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "easyvec/geometry.pyx":618
+  /* "easyvec/geometry.pyx":630
  * 
  *     @cython.nonecheck(False)
  *     cpdef list intersect_ray(self, Vec2 p1, Vec2 p2, bint sortreduce=True):             # <<<<<<<<<<<<<<
  *         return self.intersect_general(p1, p2, 0.0, BIG_REAL, sortreduce)
  * 
  */
 
@@ -16573,17 +16906,17 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_11intersect_ray(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_7easyvec_8geometry_8PolyLine_10intersect_ray[] = "PolyLine.intersect_ray(self, Vec2 p1, Vec2 p2, bool sortreduce=True) -> list";
-static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_11intersect_ray(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_15intersect_ray(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_7easyvec_8geometry_8PolyLine_14intersect_ray[] = "PolyLine.intersect_ray(self, Vec2 p1, Vec2 p2, bool sortreduce=True) -> list";
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_15intersect_ray(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p1 = 0;
   struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p2 = 0;
   int __pyx_v_sortreduce;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("intersect_ray (wrapper)", 0);
   {
@@ -16607,75 +16940,75 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_p1)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_p2)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("intersect_ray", 0, 2, 3, 1); __PYX_ERR(0, 618, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("intersect_ray", 0, 2, 3, 1); __PYX_ERR(0, 630, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_sortreduce);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "intersect_ray") < 0)) __PYX_ERR(0, 618, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "intersect_ray") < 0)) __PYX_ERR(0, 630, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_p1 = ((struct __pyx_obj_7easyvec_7vectors_Vec2 *)values[0]);
     __pyx_v_p2 = ((struct __pyx_obj_7easyvec_7vectors_Vec2 *)values[1]);
     if (values[2]) {
-      __pyx_v_sortreduce = __Pyx_PyObject_IsTrue(values[2]); if (unlikely((__pyx_v_sortreduce == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 618, __pyx_L3_error)
+      __pyx_v_sortreduce = __Pyx_PyObject_IsTrue(values[2]); if (unlikely((__pyx_v_sortreduce == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 630, __pyx_L3_error)
     } else {
       __pyx_v_sortreduce = ((int)1);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("intersect_ray", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 618, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("intersect_ray", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 630, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("easyvec.geometry.PolyLine.intersect_ray", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_p1), __pyx_ptype_7easyvec_7vectors_Vec2, 1, "p1", 0))) __PYX_ERR(0, 618, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_p2), __pyx_ptype_7easyvec_7vectors_Vec2, 1, "p2", 0))) __PYX_ERR(0, 618, __pyx_L1_error)
-  __pyx_r = __pyx_pf_7easyvec_8geometry_8PolyLine_10intersect_ray(((struct __pyx_obj_7easyvec_8geometry_PolyLine *)__pyx_v_self), __pyx_v_p1, __pyx_v_p2, __pyx_v_sortreduce);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_p1), __pyx_ptype_7easyvec_7vectors_Vec2, 1, "p1", 0))) __PYX_ERR(0, 630, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_p2), __pyx_ptype_7easyvec_7vectors_Vec2, 1, "p2", 0))) __PYX_ERR(0, 630, __pyx_L1_error)
+  __pyx_r = __pyx_pf_7easyvec_8geometry_8PolyLine_14intersect_ray(((struct __pyx_obj_7easyvec_8geometry_PolyLine *)__pyx_v_self), __pyx_v_p1, __pyx_v_p2, __pyx_v_sortreduce);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_10intersect_ray(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p2, int __pyx_v_sortreduce) {
+static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_14intersect_ray(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p2, int __pyx_v_sortreduce) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   struct __pyx_opt_args_7easyvec_8geometry_8PolyLine_intersect_ray __pyx_t_2;
   __Pyx_RefNannySetupContext("intersect_ray", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2.__pyx_n = 1;
   __pyx_t_2.sortreduce = __pyx_v_sortreduce;
-  __pyx_t_1 = __pyx_vtabptr_7easyvec_8geometry_PolyLine->intersect_ray(__pyx_v_self, __pyx_v_p1, __pyx_v_p2, 1, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 618, __pyx_L1_error)
+  __pyx_t_1 = __pyx_vtabptr_7easyvec_8geometry_PolyLine->intersect_ray(__pyx_v_self, __pyx_v_p1, __pyx_v_p2, 1, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 630, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -16684,53 +17017,53 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "easyvec/geometry.pyx":622
+/* "easyvec/geometry.pyx":634
  * 
  *     @cython.nonecheck(False)
  *     cpdef list intersect_segment(self, Vec2 p1, Vec2 p2, bint sortreduce=True):             # <<<<<<<<<<<<<<
  *         return self.intersect_general(p1, p2, 0.0, 1.0, sortreduce)
  * 
  */
 
-static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_13intersect_segment(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_17intersect_segment(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_f_7easyvec_8geometry_8PolyLine_intersect_segment(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p2, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_opt_args_7easyvec_8geometry_8PolyLine_intersect_segment *__pyx_optional_args) {
   int __pyx_v_sortreduce = ((int)1);
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   struct __pyx_opt_args_7easyvec_8geometry_8PolyLine_intersect_general __pyx_t_2;
   __Pyx_RefNannySetupContext("intersect_segment", 0);
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_sortreduce = __pyx_optional_args->sortreduce;
     }
   }
 
-  /* "easyvec/geometry.pyx":623
+  /* "easyvec/geometry.pyx":635
  *     @cython.nonecheck(False)
  *     cpdef list intersect_segment(self, Vec2 p1, Vec2 p2, bint sortreduce=True):
  *         return self.intersect_general(p1, p2, 0.0, 1.0, sortreduce)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2.__pyx_n = 1;
   __pyx_t_2.sortreduce = __pyx_v_sortreduce;
-  __pyx_t_1 = __pyx_f_7easyvec_8geometry_8PolyLine_intersect_general(__pyx_v_self, __pyx_v_p1, __pyx_v_p2, 0.0, 1.0, 0, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 623, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_7easyvec_8geometry_8PolyLine_intersect_general(__pyx_v_self, __pyx_v_p1, __pyx_v_p2, 0.0, 1.0, 0, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 635, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "easyvec/geometry.pyx":622
+  /* "easyvec/geometry.pyx":634
  * 
  *     @cython.nonecheck(False)
  *     cpdef list intersect_segment(self, Vec2 p1, Vec2 p2, bint sortreduce=True):             # <<<<<<<<<<<<<<
  *         return self.intersect_general(p1, p2, 0.0, 1.0, sortreduce)
  * 
  */
 
@@ -16742,17 +17075,17 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_13intersect_segment(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_7easyvec_8geometry_8PolyLine_12intersect_segment[] = "PolyLine.intersect_segment(self, Vec2 p1, Vec2 p2, bool sortreduce=True) -> list";
-static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_13intersect_segment(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_17intersect_segment(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_7easyvec_8geometry_8PolyLine_16intersect_segment[] = "PolyLine.intersect_segment(self, Vec2 p1, Vec2 p2, bool sortreduce=True) -> list";
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_17intersect_segment(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p1 = 0;
   struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p2 = 0;
   int __pyx_v_sortreduce;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("intersect_segment (wrapper)", 0);
   {
@@ -16776,75 +17109,75 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_p1)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_p2)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("intersect_segment", 0, 2, 3, 1); __PYX_ERR(0, 622, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("intersect_segment", 0, 2, 3, 1); __PYX_ERR(0, 634, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_sortreduce);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "intersect_segment") < 0)) __PYX_ERR(0, 622, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "intersect_segment") < 0)) __PYX_ERR(0, 634, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_p1 = ((struct __pyx_obj_7easyvec_7vectors_Vec2 *)values[0]);
     __pyx_v_p2 = ((struct __pyx_obj_7easyvec_7vectors_Vec2 *)values[1]);
     if (values[2]) {
-      __pyx_v_sortreduce = __Pyx_PyObject_IsTrue(values[2]); if (unlikely((__pyx_v_sortreduce == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 622, __pyx_L3_error)
+      __pyx_v_sortreduce = __Pyx_PyObject_IsTrue(values[2]); if (unlikely((__pyx_v_sortreduce == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 634, __pyx_L3_error)
     } else {
       __pyx_v_sortreduce = ((int)1);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("intersect_segment", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 622, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("intersect_segment", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 634, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("easyvec.geometry.PolyLine.intersect_segment", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_p1), __pyx_ptype_7easyvec_7vectors_Vec2, 1, "p1", 0))) __PYX_ERR(0, 622, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_p2), __pyx_ptype_7easyvec_7vectors_Vec2, 1, "p2", 0))) __PYX_ERR(0, 622, __pyx_L1_error)
-  __pyx_r = __pyx_pf_7easyvec_8geometry_8PolyLine_12intersect_segment(((struct __pyx_obj_7easyvec_8geometry_PolyLine *)__pyx_v_self), __pyx_v_p1, __pyx_v_p2, __pyx_v_sortreduce);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_p1), __pyx_ptype_7easyvec_7vectors_Vec2, 1, "p1", 0))) __PYX_ERR(0, 634, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_p2), __pyx_ptype_7easyvec_7vectors_Vec2, 1, "p2", 0))) __PYX_ERR(0, 634, __pyx_L1_error)
+  __pyx_r = __pyx_pf_7easyvec_8geometry_8PolyLine_16intersect_segment(((struct __pyx_obj_7easyvec_8geometry_PolyLine *)__pyx_v_self), __pyx_v_p1, __pyx_v_p2, __pyx_v_sortreduce);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_12intersect_segment(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p2, int __pyx_v_sortreduce) {
+static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_16intersect_segment(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p2, int __pyx_v_sortreduce) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   struct __pyx_opt_args_7easyvec_8geometry_8PolyLine_intersect_segment __pyx_t_2;
   __Pyx_RefNannySetupContext("intersect_segment", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2.__pyx_n = 1;
   __pyx_t_2.sortreduce = __pyx_v_sortreduce;
-  __pyx_t_1 = __pyx_vtabptr_7easyvec_8geometry_PolyLine->intersect_segment(__pyx_v_self, __pyx_v_p1, __pyx_v_p2, 1, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 622, __pyx_L1_error)
+  __pyx_t_1 = __pyx_vtabptr_7easyvec_8geometry_PolyLine->intersect_segment(__pyx_v_self, __pyx_v_p1, __pyx_v_p2, 1, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 634, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -17041,28 +17374,28 @@
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_15__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_7easyvec_8geometry_8PolyLine_14__reduce_cython__[] = "PolyLine.__reduce_cython__(self)";
-static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_15__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_19__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_7easyvec_8geometry_8PolyLine_18__reduce_cython__[] = "PolyLine.__reduce_cython__(self)";
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_19__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_7easyvec_8geometry_8PolyLine_14__reduce_cython__(((struct __pyx_obj_7easyvec_8geometry_PolyLine *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7easyvec_8geometry_8PolyLine_18__reduce_cython__(((struct __pyx_obj_7easyvec_8geometry_PolyLine *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_14__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self) {
+static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_18__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("__reduce_cython__", 0);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
@@ -17096,28 +17429,28 @@
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_17__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
-static char __pyx_doc_7easyvec_8geometry_8PolyLine_16__setstate_cython__[] = "PolyLine.__setstate_cython__(self, __pyx_state)";
-static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_17__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_21__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
+static char __pyx_doc_7easyvec_8geometry_8PolyLine_20__setstate_cython__[] = "PolyLine.__setstate_cython__(self, __pyx_state)";
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_21__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_7easyvec_8geometry_8PolyLine_16__setstate_cython__(((struct __pyx_obj_7easyvec_8geometry_PolyLine *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
+  __pyx_r = __pyx_pf_7easyvec_8geometry_8PolyLine_20__setstate_cython__(((struct __pyx_obj_7easyvec_8geometry_PolyLine *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_16__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_20__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
@@ -30895,15 +31228,15 @@
   PyObject *o;
   o = (*t->tp_alloc)(t, 0);
   if (unlikely(!o)) return 0;
   p = ((struct __pyx_obj_7easyvec_8geometry_PolyLine *)o);
   p->__pyx_vtab = __pyx_vtabptr_7easyvec_8geometry_PolyLine;
   p->vecs = ((PyObject*)Py_None); Py_INCREF(Py_None);
   p->bbox = ((struct __pyx_obj_7easyvec_8geometry_Rect *)Py_None); Py_INCREF(Py_None);
-  if (unlikely(__pyx_pw_7easyvec_8geometry_8PolyLine_1__cinit__(o, a, k) < 0)) goto bad;
+  if (unlikely(__pyx_pw_7easyvec_8geometry_8PolyLine_3__cinit__(o, a, k) < 0)) goto bad;
   return o;
   bad:
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_7easyvec_8geometry_PolyLine(PyObject *o) {
@@ -30962,20 +31295,22 @@
   else {
     PyErr_SetString(PyExc_NotImplementedError, "__del__");
     return -1;
   }
 }
 
 static PyMethodDef __pyx_methods_7easyvec_8geometry_PolyLine[] = {
-  {"intersect_general", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7easyvec_8geometry_8PolyLine_7intersect_general, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7easyvec_8geometry_8PolyLine_6intersect_general},
-  {"intersect_line", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7easyvec_8geometry_8PolyLine_9intersect_line, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7easyvec_8geometry_8PolyLine_8intersect_line},
-  {"intersect_ray", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7easyvec_8geometry_8PolyLine_11intersect_ray, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7easyvec_8geometry_8PolyLine_10intersect_ray},
-  {"intersect_segment", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7easyvec_8geometry_8PolyLine_13intersect_segment, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7easyvec_8geometry_8PolyLine_12intersect_segment},
-  {"__reduce_cython__", (PyCFunction)__pyx_pw_7easyvec_8geometry_8PolyLine_15__reduce_cython__, METH_NOARGS, __pyx_doc_7easyvec_8geometry_8PolyLine_14__reduce_cython__},
-  {"__setstate_cython__", (PyCFunction)__pyx_pw_7easyvec_8geometry_8PolyLine_17__setstate_cython__, METH_O, __pyx_doc_7easyvec_8geometry_8PolyLine_16__setstate_cython__},
+  {"from_dict", (PyCFunction)__pyx_pw_7easyvec_8geometry_8PolyLine_1from_dict, METH_O, __pyx_doc_7easyvec_8geometry_8PolyLine_from_dict},
+  {"to_dict", (PyCFunction)__pyx_pw_7easyvec_8geometry_8PolyLine_5to_dict, METH_NOARGS, __pyx_doc_7easyvec_8geometry_8PolyLine_4to_dict},
+  {"intersect_general", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7easyvec_8geometry_8PolyLine_11intersect_general, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7easyvec_8geometry_8PolyLine_10intersect_general},
+  {"intersect_line", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7easyvec_8geometry_8PolyLine_13intersect_line, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7easyvec_8geometry_8PolyLine_12intersect_line},
+  {"intersect_ray", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7easyvec_8geometry_8PolyLine_15intersect_ray, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7easyvec_8geometry_8PolyLine_14intersect_ray},
+  {"intersect_segment", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7easyvec_8geometry_8PolyLine_17intersect_segment, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7easyvec_8geometry_8PolyLine_16intersect_segment},
+  {"__reduce_cython__", (PyCFunction)__pyx_pw_7easyvec_8geometry_8PolyLine_19__reduce_cython__, METH_NOARGS, __pyx_doc_7easyvec_8geometry_8PolyLine_18__reduce_cython__},
+  {"__setstate_cython__", (PyCFunction)__pyx_pw_7easyvec_8geometry_8PolyLine_21__setstate_cython__, METH_O, __pyx_doc_7easyvec_8geometry_8PolyLine_20__setstate_cython__},
   {0, 0, 0, 0}
 };
 
 static struct PyGetSetDef __pyx_getsets_7easyvec_8geometry_PolyLine[] = {
   {(char *)"vecs", __pyx_getprop_7easyvec_8geometry_8PolyLine_vecs, __pyx_setprop_7easyvec_8geometry_8PolyLine_vecs, (char *)"vecs: list", 0},
   {(char *)"enclosed", __pyx_getprop_7easyvec_8geometry_8PolyLine_enclosed, __pyx_setprop_7easyvec_8geometry_8PolyLine_enclosed, (char *)"enclosed: 'bool'", 0},
   {0, 0, 0, 0, 0}
@@ -30997,21 +31332,21 @@
   0, /*tp_setattr*/
   #if PY_MAJOR_VERSION < 3
   0, /*tp_compare*/
   #endif
   #if PY_MAJOR_VERSION >= 3
   0, /*tp_as_async*/
   #endif
-  __pyx_pw_7easyvec_8geometry_8PolyLine_5__repr__, /*tp_repr*/
+  __pyx_pw_7easyvec_8geometry_8PolyLine_9__repr__, /*tp_repr*/
   0, /*tp_as_number*/
   0, /*tp_as_sequence*/
   0, /*tp_as_mapping*/
   0, /*tp_hash*/
   0, /*tp_call*/
-  __pyx_pw_7easyvec_8geometry_8PolyLine_3__str__, /*tp_str*/
+  __pyx_pw_7easyvec_8geometry_8PolyLine_7__str__, /*tp_str*/
   0, /*tp_getattro*/
   0, /*tp_setattro*/
   0, /*tp_as_buffer*/
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_HAVE_GC, /*tp_flags*/
   0, /*tp_doc*/
   __pyx_tp_traverse_7easyvec_8geometry_PolyLine, /*tp_traverse*/
   __pyx_tp_clear_7easyvec_8geometry_PolyLine, /*tp_clear*/
@@ -31993,14 +32328,15 @@
   {&__pyx_kp_s_contiguous_and_indirect, __pyx_k_contiguous_and_indirect, sizeof(__pyx_k_contiguous_and_indirect), 0, 0, 1, 0},
   {&__pyx_n_s_copy_data, __pyx_k_copy_data, sizeof(__pyx_k_copy_data), 0, 0, 1, 1},
   {&__pyx_n_u_d, __pyx_k_d, sizeof(__pyx_k_d), 0, 1, 0, 1},
   {&__pyx_n_s_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
   {&__pyx_n_s_dtype_is_object, __pyx_k_dtype_is_object, sizeof(__pyx_k_dtype_is_object), 0, 0, 1, 1},
   {&__pyx_n_s_easyvec_geometry, __pyx_k_easyvec_geometry, sizeof(__pyx_k_easyvec_geometry), 0, 0, 1, 1},
   {&__pyx_n_s_enclosed, __pyx_k_enclosed, sizeof(__pyx_k_enclosed), 0, 0, 1, 1},
+  {&__pyx_n_u_enclosed, __pyx_k_enclosed, sizeof(__pyx_k_enclosed), 0, 1, 0, 1},
   {&__pyx_kp_u_enclosed_2, __pyx_k_enclosed_2, sizeof(__pyx_k_enclosed_2), 0, 1, 0, 0},
   {&__pyx_n_s_encode, __pyx_k_encode, sizeof(__pyx_k_encode), 0, 0, 1, 1},
   {&__pyx_n_s_enumerate, __pyx_k_enumerate, sizeof(__pyx_k_enumerate), 0, 0, 1, 1},
   {&__pyx_n_s_error, __pyx_k_error, sizeof(__pyx_k_error), 0, 0, 1, 1},
   {&__pyx_n_s_f_high, __pyx_k_f_high, sizeof(__pyx_k_f_high), 0, 0, 1, 1},
   {&__pyx_n_s_f_low, __pyx_k_f_low, sizeof(__pyx_k_f_low), 0, 0, 1, 1},
   {&__pyx_n_s_flags, __pyx_k_flags, sizeof(__pyx_k_flags), 0, 0, 1, 1},
@@ -32095,23 +32431,25 @@
   {&__pyx_kp_s_strided_and_direct, __pyx_k_strided_and_direct, sizeof(__pyx_k_strided_and_direct), 0, 0, 1, 0},
   {&__pyx_kp_s_strided_and_direct_or_indirect, __pyx_k_strided_and_direct_or_indirect, sizeof(__pyx_k_strided_and_direct_or_indirect), 0, 0, 1, 0},
   {&__pyx_kp_s_strided_and_indirect, __pyx_k_strided_and_indirect, sizeof(__pyx_k_strided_and_indirect), 0, 0, 1, 0},
   {&__pyx_kp_s_stringsource, __pyx_k_stringsource, sizeof(__pyx_k_stringsource), 0, 0, 1, 0},
   {&__pyx_n_s_struct, __pyx_k_struct, sizeof(__pyx_k_struct), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_n_s_throw, __pyx_k_throw, sizeof(__pyx_k_throw), 0, 0, 1, 1},
+  {&__pyx_n_s_to_dict, __pyx_k_to_dict, sizeof(__pyx_k_to_dict), 0, 0, 1, 1},
   {&__pyx_n_s_u1, __pyx_k_u1, sizeof(__pyx_k_u1), 0, 0, 1, 1},
   {&__pyx_n_s_u2, __pyx_k_u2, sizeof(__pyx_k_u2), 0, 0, 1, 1},
   {&__pyx_kp_s_unable_to_allocate_array_data, __pyx_k_unable_to_allocate_array_data, sizeof(__pyx_k_unable_to_allocate_array_data), 0, 0, 1, 0},
   {&__pyx_kp_s_unable_to_allocate_shape_and_str, __pyx_k_unable_to_allocate_shape_and_str, sizeof(__pyx_k_unable_to_allocate_shape_and_str), 0, 0, 1, 0},
   {&__pyx_n_s_unpack, __pyx_k_unpack, sizeof(__pyx_k_unpack), 0, 0, 1, 1},
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
   {&__pyx_n_s_v1, __pyx_k_v1, sizeof(__pyx_k_v1), 0, 0, 1, 1},
   {&__pyx_n_s_v2, __pyx_k_v2, sizeof(__pyx_k_v2), 0, 0, 1, 1},
   {&__pyx_n_s_vecs, __pyx_k_vecs, sizeof(__pyx_k_vecs), 0, 0, 1, 1},
+  {&__pyx_n_u_vecs, __pyx_k_vecs, sizeof(__pyx_k_vecs), 0, 1, 0, 1},
   {&__pyx_n_s_x, __pyx_k_x, sizeof(__pyx_k_x), 0, 0, 1, 1},
   {&__pyx_n_u_x1, __pyx_k_x1, sizeof(__pyx_k_x1), 0, 1, 0, 1},
   {&__pyx_n_u_x2, __pyx_k_x2, sizeof(__pyx_k_x2), 0, 1, 0, 1},
   {&__pyx_n_s_y, __pyx_k_y, sizeof(__pyx_k_y), 0, 0, 1, 1},
   {&__pyx_n_u_y1, __pyx_k_y1, sizeof(__pyx_k_y1), 0, 1, 0, 1},
   {&__pyx_n_u_y2, __pyx_k_y2, sizeof(__pyx_k_y2), 0, 1, 0, 1},
   {0, 0, 0, 0, 0, 0, 0}
@@ -32183,22 +32521,22 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__14 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__14);
   __Pyx_GIVEREF(__pyx_tuple__14);
 
-  /* "easyvec/geometry.pyx":570
+  /* "easyvec/geometry.pyx":576
  *         self.vlen = len(self.vecs)
  *         if self.vlen < 2:
  *             raise ValueError(f'    .  ,  1')             # <<<<<<<<<<<<<<
  *         self.enclosed = enclosed
  *         self.bbox = Rect.bbox(self.vecs)
  */
-  __pyx_tuple__15 = PyTuple_Pack(1, __pyx_kp_u_1); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 570, __pyx_L1_error)
+  __pyx_tuple__15 = PyTuple_Pack(1, __pyx_kp_u_1); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 576, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__15);
   __Pyx_GIVEREF(__pyx_tuple__15);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
@@ -32540,15 +32878,15 @@
 
 static int __Pyx_modinit_function_export_code(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_export_code", 0);
   /*--- Function export code ---*/
   if (__Pyx_ExportFunction("_convert", (void (*)(void))__pyx_f_7easyvec_8geometry__convert, "struct __pyx_obj_7easyvec_7vectors_Vec2 *(PyObject *, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   if (__Pyx_ExportFunction("is_bbox_intersect", (void (*)(void))__pyx_f_7easyvec_8geometry_is_bbox_intersect, "int (struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ExportFunction("_intersect_ts", (void (*)(void))__pyx_f_7easyvec_8geometry__intersect_ts, "__pyx_ctuple_d78dc__int__and___dunderpyx_t_7easyvec_7vectors_real__and___dunderpyx_t_7easyvec_7vectors_real__etc (struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ExportFunction("_intersect_ts", (void (*)(void))__pyx_f_7easyvec_8geometry__intersect_ts, "__pyx_ctuple_acdc9__int__and___dunderpyx_t_7easyvec_7vectors_real__and___dunderpyx_t_7easyvec_7vectors_real__etc (struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   if (__Pyx_ExportFunction("intersect_lines", (void (*)(void))__pyx_f_7easyvec_8geometry_intersect_lines, "struct __pyx_obj_7easyvec_7vectors_Vec2 *(struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   if (__Pyx_ExportFunction("intersect_segments", (void (*)(void))__pyx_f_7easyvec_8geometry_intersect_segments, "struct __pyx_obj_7easyvec_7vectors_Vec2 *(struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   if (__Pyx_ExportFunction("intersect_rays", (void (*)(void))__pyx_f_7easyvec_8geometry_intersect_rays, "struct __pyx_obj_7easyvec_7vectors_Vec2 *(struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   if (__Pyx_ExportFunction("intersect_ray_line", (void (*)(void))__pyx_f_7easyvec_8geometry_intersect_ray_line, "struct __pyx_obj_7easyvec_7vectors_Vec2 *(struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   if (__Pyx_ExportFunction("intersect_ray_segment", (void (*)(void))__pyx_f_7easyvec_8geometry_intersect_ray_segment, "struct __pyx_obj_7easyvec_7vectors_Vec2 *(struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   if (__Pyx_ExportFunction("intersect_line_segment", (void (*)(void))__pyx_f_7easyvec_8geometry_intersect_line_segment, "struct __pyx_obj_7easyvec_7vectors_Vec2 *(struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   if (__Pyx_ExportFunction("fmax", (void (*)(void))__pyx_f_7easyvec_8geometry_fmax, "__pyx_t_7easyvec_7vectors_real (__pyx_t_7easyvec_7vectors_real, __pyx_t_7easyvec_7vectors_real, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -33091,106 +33429,130 @@
   __pyx_t_2 = __Pyx_Method_ClassMethod(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 240, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (PyDict_SetItem((PyObject *)__pyx_ptype_7easyvec_8geometry_Rect->tp_dict, __pyx_n_s_bbox, __pyx_t_2) < 0) __PYX_ERR(0, 241, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_7easyvec_8geometry_Rect);
 
+  /* "easyvec/geometry.pyx":560
+ * cdef class PolyLine:
+ *     @classmethod
+ *     def from_dict(cls, dct):             # <<<<<<<<<<<<<<
+ *         vecs = [Vec2.from_dict(vd) for vd in dct['vecs']]
+ *         enclosed = dct['enclosed']
+ */
+  __Pyx_GetNameInClass(__pyx_t_2, (PyObject *)__pyx_ptype_7easyvec_8geometry_PolyLine, __pyx_n_s_from_dict); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 560, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+
+  /* "easyvec/geometry.pyx":559
+ * @cython.final
+ * cdef class PolyLine:
+ *     @classmethod             # <<<<<<<<<<<<<<
+ *     def from_dict(cls, dct):
+ *         vecs = [Vec2.from_dict(vd) for vd in dct['vecs']]
+ */
+  __pyx_t_1 = __Pyx_Method_ClassMethod(__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 559, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_7easyvec_8geometry_PolyLine->tp_dict, __pyx_n_s_from_dict, __pyx_t_1) < 0) __PYX_ERR(0, 560, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  PyType_Modified(__pyx_ptype_7easyvec_8geometry_PolyLine);
+
   /* "easyvec/geometry.pyx":1
  * import numpy as np             # <<<<<<<<<<<<<<
  * from libc.math cimport fabs
  * cimport cython
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "View.MemoryView":209
  *         info.obj = self
  * 
  *     __pyx_getbuffer = capsule(<void *> &__pyx_array_getbuffer, "getbuffer(obj, view, flags)")             # <<<<<<<<<<<<<<
  * 
  *     def __dealloc__(array self):
  */
-  __pyx_t_2 = __pyx_capsule_create(((void *)(&__pyx_array_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 209, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem((PyObject *)__pyx_array_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_2) < 0) __PYX_ERR(1, 209, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_1 = __pyx_capsule_create(((void *)(&__pyx_array_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 209, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem((PyObject *)__pyx_array_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_1) < 0) __PYX_ERR(1, 209, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   PyType_Modified(__pyx_array_type);
 
   /* "View.MemoryView":286
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
  */
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__39, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 286, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__39, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 286, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(generic);
-  __Pyx_DECREF_SET(generic, __pyx_t_2);
-  __Pyx_GIVEREF(__pyx_t_2);
-  __pyx_t_2 = 0;
+  __Pyx_DECREF_SET(generic, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_1);
+  __pyx_t_1 = 0;
 
   /* "View.MemoryView":287
  * 
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default             # <<<<<<<<<<<<<<
  * cdef indirect = Enum("<strided and indirect>")
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__40, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 287, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__40, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 287, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(strided);
-  __Pyx_DECREF_SET(strided, __pyx_t_2);
-  __Pyx_GIVEREF(__pyx_t_2);
-  __pyx_t_2 = 0;
+  __Pyx_DECREF_SET(strided, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_1);
+  __pyx_t_1 = 0;
 
   /* "View.MemoryView":288
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__41, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 288, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__41, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 288, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(indirect);
-  __Pyx_DECREF_SET(indirect, __pyx_t_2);
-  __Pyx_GIVEREF(__pyx_t_2);
-  __pyx_t_2 = 0;
+  __Pyx_DECREF_SET(indirect, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_1);
+  __pyx_t_1 = 0;
 
   /* "View.MemoryView":291
  * 
  * 
  * cdef contiguous = Enum("<contiguous and direct>")             # <<<<<<<<<<<<<<
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__42, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 291, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__42, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 291, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(contiguous);
-  __Pyx_DECREF_SET(contiguous, __pyx_t_2);
-  __Pyx_GIVEREF(__pyx_t_2);
-  __pyx_t_2 = 0;
+  __Pyx_DECREF_SET(contiguous, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_1);
+  __pyx_t_1 = 0;
 
   /* "View.MemoryView":292
  * 
  * cdef contiguous = Enum("<contiguous and direct>")
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__43, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 292, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__43, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 292, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(indirect_contiguous);
-  __Pyx_DECREF_SET(indirect_contiguous, __pyx_t_2);
-  __Pyx_GIVEREF(__pyx_t_2);
-  __pyx_t_2 = 0;
+  __Pyx_DECREF_SET(indirect_contiguous, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_1);
+  __pyx_t_1 = 0;
 
   /* "View.MemoryView":316
  * 
  * DEF THREAD_LOCKS_PREALLOCATED = 8
  * cdef int __pyx_memoryview_thread_locks_used = 0             # <<<<<<<<<<<<<<
  * cdef PyThread_type_lock[THREAD_LOCKS_PREALLOCATED] __pyx_memoryview_thread_locks = [
  *     PyThread_allocate_lock(),
@@ -33217,42 +33579,42 @@
   /* "View.MemoryView":549
  *         info.obj = self
  * 
  *     __pyx_getbuffer = capsule(<void *> &__pyx_memoryview_getbuffer, "getbuffer(obj, view, flags)")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_2 = __pyx_capsule_create(((void *)(&__pyx_memoryview_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 549, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem((PyObject *)__pyx_memoryview_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_2) < 0) __PYX_ERR(1, 549, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_1 = __pyx_capsule_create(((void *)(&__pyx_memoryview_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 549, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem((PyObject *)__pyx_memoryview_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_1) < 0) __PYX_ERR(1, 549, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   PyType_Modified(__pyx_memoryview_type);
 
   /* "View.MemoryView":995
  *         return self.from_object
  * 
  *     __pyx_getbuffer = capsule(<void *> &__pyx_memoryview_getbuffer, "getbuffer(obj, view, flags)")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_2 = __pyx_capsule_create(((void *)(&__pyx_memoryview_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 995, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem((PyObject *)__pyx_memoryviewslice_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_2) < 0) __PYX_ERR(1, 995, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_1 = __pyx_capsule_create(((void *)(&__pyx_memoryview_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 995, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem((PyObject *)__pyx_memoryviewslice_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_1) < 0) __PYX_ERR(1, 995, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   PyType_Modified(__pyx_memoryviewslice_type);
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_Enum(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_15View_dot_MemoryView_1__pyx_unpickle_Enum, NULL, __pyx_n_s_View_MemoryView); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_Enum, __pyx_t_2) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_15View_dot_MemoryView_1__pyx_unpickle_Enum, NULL, __pyx_n_s_View_MemoryView); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_Enum, __pyx_t_1) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":11
  *         __pyx_unpickle_Enum__set_state(<Enum> __pyx_result, __pyx_state)
  *     return __pyx_result
  * cdef __pyx_unpickle_Enum__set_state(Enum __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_result.name = __pyx_state[0]
  *     if len(__pyx_state) > 1 and hasattr(__pyx_result, '__dict__'):
@@ -37183,15 +37545,15 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(long),
                                      little, !is_unsigned);
     }
 }
 
 /* ToPyCTupleUtility */
-  static PyObject* __pyx_convert__to_py___pyx_ctuple_d78dc__int__and___dunderpyx_t_7easyvec_7vectors_real__and___dunderpyx_t_7easyvec_7vectors_real__etc(__pyx_ctuple_d78dc__int__and___dunderpyx_t_7easyvec_7vectors_real__and___dunderpyx_t_7easyvec_7vectors_real__etc value) {
+  static PyObject* __pyx_convert__to_py___pyx_ctuple_acdc9__int__and___dunderpyx_t_7easyvec_7vectors_real__and___dunderpyx_t_7easyvec_7vectors_real__etc(__pyx_ctuple_acdc9__int__and___dunderpyx_t_7easyvec_7vectors_real__and___dunderpyx_t_7easyvec_7vectors_real__etc value) {
     PyObject* item = NULL;
     PyObject* result = PyTuple_New(3);
     if (!result) goto bad;
         item = __Pyx_PyBool_FromLong(value.f0);
         if (!item) goto bad;
         PyTuple_SET_ITEM(result, 0, item);
         item = PyFloat_FromDouble(value.f1);
```

### Comparing `easyvec-0.0.8/src/easyvec/geometry.html` & `easyvec-0.0.9/src/easyvec/geometry.html`

 * *Files 0% similar despite different names*

```diff
@@ -366,18 +366,18 @@
 <p>Raw output: <a href="geometry.cpp">geometry.cpp</a></p>
 <div class="cython"><pre class="cython line score-16" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">001</span>: <span class="k">import</span> <span class="nn">numpy</span> <span class="k">as</span> <span class="nn">np</span></pre>
 <pre class='cython code score-16 '>  __pyx_t_1 = <span class='pyx_c_api'>__Pyx_Import</span>(__pyx_n_s_numpy, 0, 0);<span class='error_goto'> if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)</span>
   <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_1);
   if (<span class='py_c_api'>PyDict_SetItem</span>(__pyx_d, __pyx_n_s_np, __pyx_t_1) &lt; 0) <span class='error_goto'>__PYX_ERR(0, 1, __pyx_L1_error)</span>
   <span class='pyx_macro_api'>__Pyx_DECREF</span>(__pyx_t_1); __pyx_t_1 = 0;
 /* … */
-  __pyx_t_2 = <span class='pyx_c_api'>__Pyx_PyDict_NewPresized</span>(0);<span class='error_goto'> if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)</span>
-  <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_2);
-  if (<span class='py_c_api'>PyDict_SetItem</span>(__pyx_d, __pyx_n_s_test, __pyx_t_2) &lt; 0) <span class='error_goto'>__PYX_ERR(0, 1, __pyx_L1_error)</span>
-  <span class='pyx_macro_api'>__Pyx_DECREF</span>(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_1 = <span class='pyx_c_api'>__Pyx_PyDict_NewPresized</span>(0);<span class='error_goto'> if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)</span>
+  <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_1);
+  if (<span class='py_c_api'>PyDict_SetItem</span>(__pyx_d, __pyx_n_s_test, __pyx_t_1) &lt; 0) <span class='error_goto'>__PYX_ERR(0, 1, __pyx_L1_error)</span>
+  <span class='pyx_macro_api'>__Pyx_DECREF</span>(__pyx_t_1); __pyx_t_1 = 0;
 </pre><pre class="cython line score-0">&#xA0;<span class="">002</span>: <span class="k">from</span> <span class="nn">libc.math</span> <span class="k">cimport</span> <span class="n">fabs</span></pre>
 <pre class="cython line score-0">&#xA0;<span class="">003</span>: <span class="k">cimport</span> <span class="nn">cython</span></pre>
 <pre class="cython line score-0">&#xA0;<span class="">004</span>: <span class="k">from</span> <span class="nn">.vectors</span> <span class="k">cimport</span> <span class="n">CMP_TOL</span><span class="p">,</span> <span class="n">real</span><span class="p">,</span> <span class="n">Vec2</span><span class="p">,</span> <span class="n">rational</span><span class="p">,</span> <span class="n">BIG_REAL</span><span class="p">,</span> <span class="n">MINUS_BIG_REAL</span></pre>
 <pre class="cython line score-0">&#xA0;<span class="">005</span>: <span class="k">from</span> <span class="nn">cpython.object</span> <span class="k">cimport</span> <span class="n">Py_LT</span><span class="p">,</span> <span class="n">Py_LE</span><span class="p">,</span> <span class="n">Py_EQ</span><span class="p">,</span> <span class="n">Py_GE</span><span class="p">,</span> <span class="n">Py_GT</span><span class="p">,</span> <span class="n">Py_NE</span></pre>
 <pre class="cython line score-0">&#xA0;<span class="">006</span>: </pre>
 <pre class="cython line score-17" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">007</span>: <span class="k">cdef</span> <span class="kt">array</span>.<span class="kt">array</span> <span class="nf">_int_array_template</span> <span class="o">=</span> <span class="n">array</span><span class="o">.</span><span class="n">array</span><span class="p">(</span><span class="s">&#39;i&#39;</span><span class="p">,</span> <span class="p">[])</span></pre>
 <pre class='cython code score-17 '>  __pyx_t_1 = <span class='py_c_api'>PyList_New</span>(0);<span class='error_goto'> if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 7, __pyx_L1_error)</span>
@@ -1400,22 +1400,22 @@
   goto __pyx_L0;
 </pre><pre class="cython line score-0">&#xA0;<span class="">083</span>: </pre>
 <pre class="cython line score-0">&#xA0;<span class="">084</span>: </pre>
 <pre class="cython line score-0">&#xA0;<span class="">085</span>: <span class="nd">@cython</span><span class="o">.</span><span class="n">nonecheck</span><span class="p">(</span><span class="bp">False</span><span class="p">)</span></pre>
 <pre class="cython line score-0">&#xA0;<span class="">086</span>: <span class="nd">@cython</span><span class="o">.</span><span class="n">cdivision</span><span class="p">(</span><span class="bp">True</span><span class="p">)</span></pre>
 <pre class="cython line score-55" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">087</span>: <span class="k">cpdef</span> (<span class="nf">bint</span><span class="p">,</span> <span class="nf">real</span><span class="p">,</span> <span class="kt">real</span>) <span class="nf">_intersect_ts</span><span class="p">(</span><span class="n">Vec2</span> <span class="n">u1</span><span class="p">,</span> <span class="n">Vec2</span> <span class="n">u2</span><span class="p">,</span> <span class="n">Vec2</span> <span class="n">v1</span><span class="p">,</span> <span class="n">Vec2</span> <span class="n">v2</span><span class="p">):</span></pre>
 <pre class='cython code score-55 '>static PyObject *__pyx_pw_7easyvec_8geometry_7_intersect_ts(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static __pyx_ctuple_d78dc__int__and___dunderpyx_t_7easyvec_7vectors_real__and___dunderpyx_t_7easyvec_7vectors_real__etc __pyx_f_7easyvec_8geometry__intersect_ts(struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_u1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_u2, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_v1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_v2, CYTHON_UNUSED int __pyx_skip_dispatch) {
+static __pyx_ctuple_acdc9__int__and___dunderpyx_t_7easyvec_7vectors_real__and___dunderpyx_t_7easyvec_7vectors_real__etc __pyx_f_7easyvec_8geometry__intersect_ts(struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_u1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_u2, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_v1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_v2, CYTHON_UNUSED int __pyx_skip_dispatch) {
   struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_vec1 = 0;
   struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_vec2 = 0;
   struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_vec3 = 0;
   __pyx_t_7easyvec_7vectors_real __pyx_v_dot;
   __pyx_t_7easyvec_7vectors_real __pyx_v_t1;
   __pyx_t_7easyvec_7vectors_real __pyx_v_t2;
-  __pyx_ctuple_d78dc__int__and___dunderpyx_t_7easyvec_7vectors_real__and___dunderpyx_t_7easyvec_7vectors_real__etc __pyx_r;
+  __pyx_ctuple_acdc9__int__and___dunderpyx_t_7easyvec_7vectors_real__and___dunderpyx_t_7easyvec_7vectors_real__etc __pyx_r;
   <span class='refnanny'>__Pyx_RefNannyDeclarations</span>
   <span class='refnanny'>__Pyx_RefNannySetupContext</span>("_intersect_ts", 0);
 /* … */
   /* function exit code */
   __pyx_L1_error:;
   <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_t_1);
   <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_t_2);
@@ -1522,15 +1522,15 @@
 }
 
 static PyObject *__pyx_pf_7easyvec_8geometry_6_intersect_ts(CYTHON_UNUSED PyObject *__pyx_self, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_u1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_u2, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_v1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_v2) {
   PyObject *__pyx_r = NULL;
   <span class='refnanny'>__Pyx_RefNannyDeclarations</span>
   <span class='refnanny'>__Pyx_RefNannySetupContext</span>("_intersect_ts", 0);
   <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_r);
-  __pyx_t_1 = __pyx_convert__to_py___pyx_ctuple_d78dc__int__and___dunderpyx_t_7easyvec_7vectors_real__and___dunderpyx_t_7easyvec_7vectors_real__etc(__pyx_f_7easyvec_8geometry__intersect_ts(__pyx_v_u1, __pyx_v_u2, __pyx_v_v1, __pyx_v_v2, 0));<span class='error_goto'> if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 87, __pyx_L1_error)</span>
+  __pyx_t_1 = __pyx_convert__to_py___pyx_ctuple_acdc9__int__and___dunderpyx_t_7easyvec_7vectors_real__and___dunderpyx_t_7easyvec_7vectors_real__etc(__pyx_f_7easyvec_8geometry__intersect_ts(__pyx_v_u1, __pyx_v_u2, __pyx_v_v1, __pyx_v_v2, 0));<span class='error_goto'> if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 87, __pyx_L1_error)</span>
   <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -7812,18 +7812,168 @@
 };
 static struct __pyx_vtabstruct_7easyvec_8geometry_PolyLine *__pyx_vtabptr_7easyvec_8geometry_PolyLine;
 static PyObject *__pyx_f_7easyvec_8geometry_8PolyLine_intersect_general(struct __pyx_obj_7easyvec_8geometry_PolyLine *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, __pyx_t_7easyvec_7vectors_real, __pyx_t_7easyvec_7vectors_real, int __pyx_skip_dispatch, struct __pyx_opt_args_7easyvec_8geometry_8PolyLine_intersect_general *__pyx_optional_args);
 static PyObject *__pyx_f_7easyvec_8geometry_8PolyLine_intersect_line(struct __pyx_obj_7easyvec_8geometry_PolyLine *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, int __pyx_skip_dispatch, struct __pyx_opt_args_7easyvec_8geometry_8PolyLine_intersect_line *__pyx_optional_args);
 static PyObject *__pyx_f_7easyvec_8geometry_8PolyLine_intersect_ray(struct __pyx_obj_7easyvec_8geometry_PolyLine *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, int __pyx_skip_dispatch, struct __pyx_opt_args_7easyvec_8geometry_8PolyLine_intersect_ray *__pyx_optional_args);
 static PyObject *__pyx_f_7easyvec_8geometry_8PolyLine_intersect_segment(struct __pyx_obj_7easyvec_8geometry_PolyLine *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *, int __pyx_skip_dispatch, struct __pyx_opt_args_7easyvec_8geometry_8PolyLine_intersect_segment *__pyx_optional_args);
 
-</pre><pre class="cython line score-33" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">559</span>:     <span class="k">def</span> <span class="nf">__cinit__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">vecs</span><span class="p">:</span> <span class="nb">list</span><span class="p">,</span> <span class="n">enclosed</span><span class="o">=</span><span class="bp">True</span><span class="p">,</span> <span class="n">copy_data</span><span class="o">=</span><span class="bp">False</span><span class="p">):</span></pre>
+</pre><pre class="cython line score-14" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">559</span>:     <span class="nd">@classmethod</span></pre>
+<pre class='cython code score-14 '>  __pyx_t_1 = <span class='pyx_c_api'>__Pyx_Method_ClassMethod</span>(__pyx_t_2);<span class='error_goto'> if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 559, __pyx_L1_error)</span>
+  <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_1);
+  <span class='pyx_macro_api'>__Pyx_DECREF</span>(__pyx_t_2); __pyx_t_2 = 0;
+  if (<span class='py_c_api'>PyDict_SetItem</span>((PyObject *)__pyx_ptype_7easyvec_8geometry_PolyLine-&gt;tp_dict, __pyx_n_s_from_dict, __pyx_t_1) &lt; 0) <span class='error_goto'>__PYX_ERR(0, 560, __pyx_L1_error)</span>
+  <span class='pyx_macro_api'>__Pyx_DECREF</span>(__pyx_t_1); __pyx_t_1 = 0;
+  <span class='py_c_api'>PyType_Modified</span>(__pyx_ptype_7easyvec_8geometry_PolyLine);
+</pre><pre class="cython line score-12" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">560</span>:     <span class="k">def</span> <span class="nf">from_dict</span><span class="p">(</span><span class="n">cls</span><span class="p">,</span> <span class="n">dct</span><span class="p">):</span></pre>
+<pre class='cython code score-12 '>/* Python wrapper */
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_1from_dict(PyObject *__pyx_v_cls, PyObject *__pyx_v_dct); /*proto*/
+static char __pyx_doc_7easyvec_8geometry_8PolyLine_from_dict[] = "PolyLine.from_dict(type cls, dct)";
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_1from_dict(PyObject *__pyx_v_cls, PyObject *__pyx_v_dct) {
+  PyObject *__pyx_r = 0;
+  <span class='refnanny'>__Pyx_RefNannyDeclarations</span>
+  <span class='refnanny'>__Pyx_RefNannySetupContext</span>("from_dict (wrapper)", 0);
+  __pyx_r = __pyx_pf_7easyvec_8geometry_8PolyLine_from_dict(((PyTypeObject*)__pyx_v_cls), ((PyObject *)__pyx_v_dct));
+
+  /* function exit code */
+  <span class='refnanny'>__Pyx_RefNannyFinishContext</span>();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_from_dict(PyTypeObject *__pyx_v_cls, PyObject *__pyx_v_dct) {
+  PyObject *__pyx_v_vecs = NULL;
+  PyObject *__pyx_v_enclosed = NULL;
+  PyObject *__pyx_7genexpr__pyx_v_vd = NULL;
+  PyObject *__pyx_r = NULL;
+  <span class='refnanny'>__Pyx_RefNannyDeclarations</span>
+  <span class='refnanny'>__Pyx_RefNannySetupContext</span>("from_dict", 0);
+/* … */
+  /* function exit code */
+  __pyx_L1_error:;
+  <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_t_1);
+  <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_t_2);
+  <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_t_3);
+  <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_t_6);
+  <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_t_7);
+  <span class='pyx_c_api'>__Pyx_AddTraceback</span>("easyvec.geometry.PolyLine.from_dict", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_v_vecs);
+  <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_v_enclosed);
+  <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_7genexpr__pyx_v_vd);
+  <span class='refnanny'>__Pyx_XGIVEREF</span>(__pyx_r);
+  <span class='refnanny'>__Pyx_RefNannyFinishContext</span>();
+  return __pyx_r;
+}
+/* … */
+  <span class='pyx_c_api'>__Pyx_GetNameInClass</span>(__pyx_t_2, (PyObject *)__pyx_ptype_7easyvec_8geometry_PolyLine, __pyx_n_s_from_dict);<span class='error_goto'> if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 560, __pyx_L1_error)</span>
+  <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_2);
+</pre><pre class="cython line score-72" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">561</span>:         <span class="n">vecs</span> <span class="o">=</span> <span class="p">[</span><span class="n">Vec2</span><span class="o">.</span><span class="n">from_dict</span><span class="p">(</span><span class="n">vd</span><span class="p">)</span> <span class="k">for</span> <span class="n">vd</span> <span class="ow">in</span> <span class="n">dct</span><span class="p">[</span><span class="s">&#39;vecs&#39;</span><span class="p">]]</span></pre>
+<pre class='cython code score-72 '>  { /* enter inner scope */
+    __pyx_t_1 = <span class='py_c_api'>PyList_New</span>(0);<span class='error_goto'> if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 561, __pyx_L5_error)</span>
+    <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_1);
+    __pyx_t_2 = <span class='pyx_c_api'>__Pyx_PyObject_Dict_GetItem</span>(__pyx_v_dct, __pyx_n_u_vecs);<span class='error_goto'> if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 561, __pyx_L5_error)</span>
+    <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_2);
+    if (likely(<span class='py_c_api'>PyList_CheckExact</span>(__pyx_t_2)) || <span class='py_c_api'>PyTuple_CheckExact</span>(__pyx_t_2)) {
+      __pyx_t_3 = __pyx_t_2; <span class='pyx_macro_api'>__Pyx_INCREF</span>(__pyx_t_3); __pyx_t_4 = 0;
+      __pyx_t_5 = NULL;
+    } else {
+      __pyx_t_4 = -1; __pyx_t_3 = <span class='py_c_api'>PyObject_GetIter</span>(__pyx_t_2);<span class='error_goto'> if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 561, __pyx_L5_error)</span>
+      <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_3);
+      __pyx_t_5 = Py_TYPE(__pyx_t_3)-&gt;tp_iternext;<span class='error_goto'> if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 561, __pyx_L5_error)</span>
+    }
+    <span class='pyx_macro_api'>__Pyx_DECREF</span>(__pyx_t_2); __pyx_t_2 = 0;
+    for (;;) {
+      if (likely(!__pyx_t_5)) {
+        if (likely(<span class='py_c_api'>PyList_CheckExact</span>(__pyx_t_3))) {
+          if (__pyx_t_4 &gt;= <span class='py_macro_api'>PyList_GET_SIZE</span>(__pyx_t_3)) break;
+          #if CYTHON_ASSUME_SAFE_MACROS &amp;&amp; !CYTHON_AVOID_BORROWED_REFS
+          __pyx_t_2 = <span class='py_macro_api'>PyList_GET_ITEM</span>(__pyx_t_3, __pyx_t_4); <span class='pyx_macro_api'>__Pyx_INCREF</span>(__pyx_t_2); __pyx_t_4++; if (unlikely(0 &lt; 0)) <span class='error_goto'>__PYX_ERR(0, 561, __pyx_L5_error)</span>
+          #else
+          __pyx_t_2 = <span class='py_macro_api'>PySequence_ITEM</span>(__pyx_t_3, __pyx_t_4); __pyx_t_4++;<span class='error_goto'> if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 561, __pyx_L5_error)</span>
+          <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_2);
+          #endif
+        } else {
+          if (__pyx_t_4 &gt;= <span class='py_macro_api'>PyTuple_GET_SIZE</span>(__pyx_t_3)) break;
+          #if CYTHON_ASSUME_SAFE_MACROS &amp;&amp; !CYTHON_AVOID_BORROWED_REFS
+          __pyx_t_2 = <span class='py_macro_api'>PyTuple_GET_ITEM</span>(__pyx_t_3, __pyx_t_4); <span class='pyx_macro_api'>__Pyx_INCREF</span>(__pyx_t_2); __pyx_t_4++; if (unlikely(0 &lt; 0)) <span class='error_goto'>__PYX_ERR(0, 561, __pyx_L5_error)</span>
+          #else
+          __pyx_t_2 = <span class='py_macro_api'>PySequence_ITEM</span>(__pyx_t_3, __pyx_t_4); __pyx_t_4++;<span class='error_goto'> if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 561, __pyx_L5_error)</span>
+          <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_2);
+          #endif
+        }
+      } else {
+        __pyx_t_2 = __pyx_t_5(__pyx_t_3);
+        if (unlikely(!__pyx_t_2)) {
+          PyObject* exc_type = <span class='py_c_api'>PyErr_Occurred</span>();
+          if (exc_type) {
+            if (likely(<span class='pyx_c_api'>__Pyx_PyErr_GivenExceptionMatches</span>(exc_type, PyExc_StopIteration))) <span class='py_c_api'>PyErr_Clear</span>();
+            else <span class='error_goto'>__PYX_ERR(0, 561, __pyx_L5_error)</span>
+          }
+          break;
+        }
+        <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_2);
+      }
+      <span class='pyx_macro_api'>__Pyx_XDECREF_SET</span>(__pyx_7genexpr__pyx_v_vd, __pyx_t_2);
+      __pyx_t_2 = 0;
+      __pyx_t_6 = <span class='pyx_c_api'>__Pyx_PyObject_GetAttrStr</span>(((PyObject *)__pyx_ptype_7easyvec_7vectors_Vec2), __pyx_n_s_from_dict);<span class='error_goto'> if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 561, __pyx_L5_error)</span>
+      <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_6);
+      __pyx_t_7 = NULL;
+      if (CYTHON_UNPACK_METHODS &amp;&amp; likely(<span class='py_c_api'>PyMethod_Check</span>(__pyx_t_6))) {
+        __pyx_t_7 = <span class='py_macro_api'>PyMethod_GET_SELF</span>(__pyx_t_6);
+        if (likely(__pyx_t_7)) {
+          PyObject* function = <span class='py_macro_api'>PyMethod_GET_FUNCTION</span>(__pyx_t_6);
+          <span class='pyx_macro_api'>__Pyx_INCREF</span>(__pyx_t_7);
+          <span class='pyx_macro_api'>__Pyx_INCREF</span>(function);
+          <span class='pyx_macro_api'>__Pyx_DECREF_SET</span>(__pyx_t_6, function);
+        }
+      }
+      __pyx_t_2 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_7, __pyx_7genexpr__pyx_v_vd) : <span class='pyx_c_api'>__Pyx_PyObject_CallOneArg</span>(__pyx_t_6, __pyx_7genexpr__pyx_v_vd);
+      <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_t_7); __pyx_t_7 = 0;
+      if (unlikely(!__pyx_t_2)) <span class='error_goto'>__PYX_ERR(0, 561, __pyx_L5_error)</span>
+      <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_2);
+      <span class='pyx_macro_api'>__Pyx_DECREF</span>(__pyx_t_6); __pyx_t_6 = 0;
+      if (unlikely(<span class='pyx_c_api'>__Pyx_ListComp_Append</span>(__pyx_t_1, (PyObject*)__pyx_t_2))) <span class='error_goto'>__PYX_ERR(0, 561, __pyx_L5_error)</span>
+      <span class='pyx_macro_api'>__Pyx_DECREF</span>(__pyx_t_2); __pyx_t_2 = 0;
+    }
+    <span class='pyx_macro_api'>__Pyx_DECREF</span>(__pyx_t_3); __pyx_t_3 = 0;
+    <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_7genexpr__pyx_v_vd); __pyx_7genexpr__pyx_v_vd = 0;
+    goto __pyx_L8_exit_scope;
+    __pyx_L5_error:;
+    <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_7genexpr__pyx_v_vd); __pyx_7genexpr__pyx_v_vd = 0;
+    goto __pyx_L1_error;
+    __pyx_L8_exit_scope:;
+  } /* exit inner scope */
+  __pyx_v_vecs = ((PyObject*)__pyx_t_1);
+  __pyx_t_1 = 0;
+</pre><pre class="cython line score-2" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">562</span>:         <span class="n">enclosed</span> <span class="o">=</span> <span class="n">dct</span><span class="p">[</span><span class="s">&#39;enclosed&#39;</span><span class="p">]</span></pre>
+<pre class='cython code score-2 '>  __pyx_t_1 = <span class='pyx_c_api'>__Pyx_PyObject_Dict_GetItem</span>(__pyx_v_dct, __pyx_n_u_enclosed);<span class='error_goto'> if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 562, __pyx_L1_error)</span>
+  <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_1);
+  __pyx_v_enclosed = __pyx_t_1;
+  __pyx_t_1 = 0;
+</pre><pre class="cython line score-13" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">563</span>:         <span class="k">return</span> <span class="n">cls</span><span class="p">(</span><span class="n">vecs</span><span class="p">,</span> <span class="n">enclosed</span><span class="p">)</span></pre>
+<pre class='cython code score-13 '>  <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_r);
+  __pyx_t_1 = <span class='py_c_api'>PyTuple_New</span>(2);<span class='error_goto'> if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 563, __pyx_L1_error)</span>
+  <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_1);
+  <span class='pyx_macro_api'>__Pyx_INCREF</span>(__pyx_v_vecs);
+  <span class='refnanny'>__Pyx_GIVEREF</span>(__pyx_v_vecs);
+  <span class='py_macro_api'>PyTuple_SET_ITEM</span>(__pyx_t_1, 0, __pyx_v_vecs);
+  <span class='pyx_macro_api'>__Pyx_INCREF</span>(__pyx_v_enclosed);
+  <span class='refnanny'>__Pyx_GIVEREF</span>(__pyx_v_enclosed);
+  <span class='py_macro_api'>PyTuple_SET_ITEM</span>(__pyx_t_1, 1, __pyx_v_enclosed);
+  __pyx_t_3 = <span class='pyx_c_api'>__Pyx_PyObject_Call</span>(((PyObject *)__pyx_v_cls), __pyx_t_1, NULL);<span class='error_goto'> if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 563, __pyx_L1_error)</span>
+  <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_3);
+  <span class='pyx_macro_api'>__Pyx_DECREF</span>(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_r = __pyx_t_3;
+  __pyx_t_3 = 0;
+  goto __pyx_L0;
+</pre><pre class="cython line score-0">&#xA0;<span class="">564</span>: </pre>
+<pre class="cython line score-33" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">565</span>:     <span class="k">def</span> <span class="nf">__cinit__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">vecs</span><span class="p">:</span> <span class="nb">list</span><span class="p">,</span> <span class="n">enclosed</span><span class="o">=</span><span class="bp">True</span><span class="p">,</span> <span class="n">copy_data</span><span class="o">=</span><span class="bp">False</span><span class="p">):</span></pre>
 <pre class='cython code score-33 '>/* Python wrapper */
-static int __pyx_pw_7easyvec_8geometry_8PolyLine_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static int __pyx_pw_7easyvec_8geometry_8PolyLine_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static int __pyx_pw_7easyvec_8geometry_8PolyLine_3__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static int __pyx_pw_7easyvec_8geometry_8PolyLine_3__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_vecs = 0;
   PyObject *__pyx_v_enclosed = 0;
   PyObject *__pyx_v_copy_data = 0;
   int __pyx_r;
   <span class='refnanny'>__Pyx_RefNannyDeclarations</span>
   <span class='refnanny'>__Pyx_RefNannySetupContext</span>("__cinit__ (wrapper)", 0);
   {
@@ -7859,15 +8009,15 @@
         case  2:
         if (kw_args &gt; 0) {
           PyObject* value = <span class='pyx_c_api'>__Pyx_PyDict_GetItemStr</span>(__pyx_kwds, __pyx_n_s_copy_data);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args &gt; 0)) {
-        if (unlikely(<span class='pyx_c_api'>__Pyx_ParseOptionalKeywords</span>(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") &lt; 0)) <span class='error_goto'>__PYX_ERR(0, 559, __pyx_L3_error)</span>
+        if (unlikely(<span class='pyx_c_api'>__Pyx_ParseOptionalKeywords</span>(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") &lt; 0)) <span class='error_goto'>__PYX_ERR(0, 565, __pyx_L3_error)</span>
       }
     } else {
       switch (<span class='py_macro_api'>PyTuple_GET_SIZE</span>(__pyx_args)) {
         case  3: values[2] = <span class='py_macro_api'>PyTuple_GET_ITEM</span>(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = <span class='py_macro_api'>PyTuple_GET_ITEM</span>(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
@@ -7878,33 +8028,33 @@
     }
     __pyx_v_vecs = ((PyObject*)values[0]);
     __pyx_v_enclosed = values[1];
     __pyx_v_copy_data = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  <span class='pyx_c_api'>__Pyx_RaiseArgtupleInvalid</span>("__cinit__", 0, 1, 3, <span class='py_macro_api'>PyTuple_GET_SIZE</span>(__pyx_args)); <span class='error_goto'>__PYX_ERR(0, 559, __pyx_L3_error)</span>
+  <span class='pyx_c_api'>__Pyx_RaiseArgtupleInvalid</span>("__cinit__", 0, 1, 3, <span class='py_macro_api'>PyTuple_GET_SIZE</span>(__pyx_args)); <span class='error_goto'>__PYX_ERR(0, 565, __pyx_L3_error)</span>
   __pyx_L3_error:;
   <span class='pyx_c_api'>__Pyx_AddTraceback</span>("easyvec.geometry.PolyLine.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   <span class='refnanny'>__Pyx_RefNannyFinishContext</span>();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!<span class='pyx_c_api'>__Pyx_ArgTypeTest</span>(((PyObject *)__pyx_v_vecs), (&amp;PyList_Type), 1, "vecs", 1))) <span class='error_goto'>__PYX_ERR(0, 559, __pyx_L1_error)</span>
-  __pyx_r = __pyx_pf_7easyvec_8geometry_8PolyLine___cinit__(((struct __pyx_obj_7easyvec_8geometry_PolyLine *)__pyx_v_self), __pyx_v_vecs, __pyx_v_enclosed, __pyx_v_copy_data);
+  if (unlikely(!<span class='pyx_c_api'>__Pyx_ArgTypeTest</span>(((PyObject *)__pyx_v_vecs), (&amp;PyList_Type), 1, "vecs", 1))) <span class='error_goto'>__PYX_ERR(0, 565, __pyx_L1_error)</span>
+  __pyx_r = __pyx_pf_7easyvec_8geometry_8PolyLine_2__cinit__(((struct __pyx_obj_7easyvec_8geometry_PolyLine *)__pyx_v_self), __pyx_v_vecs, __pyx_v_enclosed, __pyx_v_copy_data);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = -1;
   __pyx_L0:;
   <span class='refnanny'>__Pyx_RefNannyFinishContext</span>();
   return __pyx_r;
 }
 
-static int __pyx_pf_7easyvec_8geometry_8PolyLine___cinit__(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self, PyObject *__pyx_v_vecs, PyObject *__pyx_v_enclosed, PyObject *__pyx_v_copy_data) {
+static int __pyx_pf_7easyvec_8geometry_8PolyLine_2__cinit__(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self, PyObject *__pyx_v_vecs, PyObject *__pyx_v_enclosed, PyObject *__pyx_v_copy_data) {
   int __pyx_v_vec_len;
   int __pyx_v_i;
   int __pyx_r;
   <span class='refnanny'>__Pyx_RefNannyDeclarations</span>
   <span class='refnanny'>__Pyx_RefNannySetupContext</span>("__cinit__", 0);
 /* … */
   /* function exit code */
@@ -7916,138 +8066,239 @@
   <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_t_9);
   <span class='pyx_c_api'>__Pyx_AddTraceback</span>("easyvec.geometry.PolyLine.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   <span class='refnanny'>__Pyx_RefNannyFinishContext</span>();
   return __pyx_r;
 }
-</pre><pre class="cython line score-0">&#xA0;<span class="">560</span>:         <span class="k">cdef</span> <span class="kt">int</span> <span class="nf">vec_len</span><span class="p">,</span> <span class="nf">i</span></pre>
-<pre class="cython line score-2" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">561</span>:         <span class="k">if</span> <span class="n">copy_data</span><span class="p">:</span></pre>
-<pre class='cython code score-2 '>  __pyx_t_1 = <span class='pyx_c_api'>__Pyx_PyObject_IsTrue</span>(__pyx_v_copy_data); if (unlikely(__pyx_t_1 &lt; 0)) <span class='error_goto'>__PYX_ERR(0, 561, __pyx_L1_error)</span>
+</pre><pre class="cython line score-0">&#xA0;<span class="">566</span>:         <span class="k">cdef</span> <span class="kt">int</span> <span class="nf">vec_len</span><span class="p">,</span> <span class="nf">i</span></pre>
+<pre class="cython line score-2" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">567</span>:         <span class="k">if</span> <span class="n">copy_data</span><span class="p">:</span></pre>
+<pre class='cython code score-2 '>  __pyx_t_1 = <span class='pyx_c_api'>__Pyx_PyObject_IsTrue</span>(__pyx_v_copy_data); if (unlikely(__pyx_t_1 &lt; 0)) <span class='error_goto'>__PYX_ERR(0, 567, __pyx_L1_error)</span>
   if (__pyx_t_1) {
 /* … */
     goto __pyx_L3;
   }
-</pre><pre class="cython line score-6" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">562</span>:             <span class="bp">self</span><span class="o">.</span><span class="n">vecs</span> <span class="o">=</span> <span class="p">[]</span></pre>
-<pre class='cython code score-6 '>    __pyx_t_2 = <span class='py_c_api'>PyList_New</span>(0);<span class='error_goto'> if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 562, __pyx_L1_error)</span>
+</pre><pre class="cython line score-6" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">568</span>:             <span class="bp">self</span><span class="o">.</span><span class="n">vecs</span> <span class="o">=</span> <span class="p">[]</span></pre>
+<pre class='cython code score-6 '>    __pyx_t_2 = <span class='py_c_api'>PyList_New</span>(0);<span class='error_goto'> if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 568, __pyx_L1_error)</span>
     <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_2);
     <span class='refnanny'>__Pyx_GIVEREF</span>(__pyx_t_2);
     <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_v_self-&gt;vecs);
     <span class='pyx_macro_api'>__Pyx_DECREF</span>(__pyx_v_self-&gt;vecs);
     __pyx_v_self-&gt;vecs = ((PyObject*)__pyx_t_2);
     __pyx_t_2 = 0;
-</pre><pre class="cython line score-6" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">563</span>:             <span class="n">vec_len</span> <span class="o">=</span> <span class="nb">len</span><span class="p">(</span><span class="n">vecs</span><span class="p">)</span></pre>
+</pre><pre class="cython line score-6" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">569</span>:             <span class="n">vec_len</span> <span class="o">=</span> <span class="nb">len</span><span class="p">(</span><span class="n">vecs</span><span class="p">)</span></pre>
 <pre class='cython code score-6 '>    if (unlikely(__pyx_v_vecs == Py_None)) {
       <span class='py_c_api'>PyErr_SetString</span>(PyExc_TypeError, "object of type 'NoneType' has no len()");
-      <span class='error_goto'>__PYX_ERR(0, 563, __pyx_L1_error)</span>
+      <span class='error_goto'>__PYX_ERR(0, 569, __pyx_L1_error)</span>
     }
-    __pyx_t_3 = <span class='py_macro_api'>PyList_GET_SIZE</span>(__pyx_v_vecs);<span class='error_goto'> if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 563, __pyx_L1_error)</span>
+    __pyx_t_3 = <span class='py_macro_api'>PyList_GET_SIZE</span>(__pyx_v_vecs);<span class='error_goto'> if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 569, __pyx_L1_error)</span>
     __pyx_v_vec_len = __pyx_t_3;
-</pre><pre class="cython line score-0" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">564</span>:             <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="n">vec_len</span><span class="p">):</span></pre>
+</pre><pre class="cython line score-0" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">570</span>:             <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="n">vec_len</span><span class="p">):</span></pre>
 <pre class='cython code score-0 '>    __pyx_t_4 = __pyx_v_vec_len;
     __pyx_t_5 = __pyx_t_4;
     for (__pyx_t_6 = 0; __pyx_t_6 &lt; __pyx_t_5; __pyx_t_6+=1) {
       __pyx_v_i = __pyx_t_6;
-</pre><pre class="cython line score-16" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">565</span>:                 <span class="bp">self</span><span class="o">.</span><span class="n">vecs</span><span class="o">.</span><span class="n">append</span><span class="p">(</span> <span class="p">(&lt;</span><span class="kt">Vec2</span><span class="p">&gt;(</span><span class="n">vecs</span><span class="p">[</span><span class="n">i</span><span class="p">]))</span><span class="o">.</span><span class="n">copy</span><span class="p">()</span> <span class="p">)</span></pre>
+</pre><pre class="cython line score-16" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">571</span>:                 <span class="bp">self</span><span class="o">.</span><span class="n">vecs</span><span class="o">.</span><span class="n">append</span><span class="p">(</span> <span class="p">(&lt;</span><span class="kt">Vec2</span><span class="p">&gt;(</span><span class="n">vecs</span><span class="p">[</span><span class="n">i</span><span class="p">]))</span><span class="o">.</span><span class="n">copy</span><span class="p">()</span> <span class="p">)</span></pre>
 <pre class='cython code score-16 '>      if (unlikely(__pyx_v_self-&gt;vecs == Py_None)) {
         <span class='py_c_api'>PyErr_Format</span>(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "append");
-        <span class='error_goto'>__PYX_ERR(0, 565, __pyx_L1_error)</span>
+        <span class='error_goto'>__PYX_ERR(0, 571, __pyx_L1_error)</span>
       }
       if (unlikely(__pyx_v_vecs == Py_None)) {
         <span class='py_c_api'>PyErr_SetString</span>(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        <span class='error_goto'>__PYX_ERR(0, 565, __pyx_L1_error)</span>
+        <span class='error_goto'>__PYX_ERR(0, 571, __pyx_L1_error)</span>
       }
-      __pyx_t_2 = <span class='pyx_c_api'>__Pyx_GetItemInt_List</span>(__pyx_v_vecs, __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 1, 1, 1);<span class='error_goto'> if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 565, __pyx_L1_error)</span>
+      __pyx_t_2 = <span class='pyx_c_api'>__Pyx_GetItemInt_List</span>(__pyx_v_vecs, __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 1, 1, 1);<span class='error_goto'> if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 571, __pyx_L1_error)</span>
       <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_2);
-      __pyx_t_7 = ((PyObject *)((struct __pyx_vtabstruct_7easyvec_7vectors_Vec2 *)((struct __pyx_obj_7easyvec_7vectors_Vec2 *)__pyx_t_2)-&gt;__pyx_vtab)-&gt;copy(((struct __pyx_obj_7easyvec_7vectors_Vec2 *)__pyx_t_2), 0));<span class='error_goto'> if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 565, __pyx_L1_error)</span>
+      __pyx_t_7 = ((PyObject *)((struct __pyx_vtabstruct_7easyvec_7vectors_Vec2 *)((struct __pyx_obj_7easyvec_7vectors_Vec2 *)__pyx_t_2)-&gt;__pyx_vtab)-&gt;copy(((struct __pyx_obj_7easyvec_7vectors_Vec2 *)__pyx_t_2), 0));<span class='error_goto'> if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 571, __pyx_L1_error)</span>
       <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_7);
       <span class='pyx_macro_api'>__Pyx_DECREF</span>(__pyx_t_2); __pyx_t_2 = 0;
-      __pyx_t_8 = <span class='pyx_c_api'>__Pyx_PyList_Append</span>(__pyx_v_self-&gt;vecs, __pyx_t_7);<span class='error_goto'> if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(0, 565, __pyx_L1_error)</span>
+      __pyx_t_8 = <span class='pyx_c_api'>__Pyx_PyList_Append</span>(__pyx_v_self-&gt;vecs, __pyx_t_7);<span class='error_goto'> if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(0, 571, __pyx_L1_error)</span>
       <span class='pyx_macro_api'>__Pyx_DECREF</span>(__pyx_t_7); __pyx_t_7 = 0;
     }
-</pre><pre class="cython line score-0">&#xA0;<span class="">566</span>:         <span class="k">else</span><span class="p">:</span></pre>
-<pre class="cython line score-2" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">567</span>:             <span class="bp">self</span><span class="o">.</span><span class="n">vecs</span> <span class="o">=</span> <span class="n">vecs</span></pre>
+</pre><pre class="cython line score-0">&#xA0;<span class="">572</span>:         <span class="k">else</span><span class="p">:</span></pre>
+<pre class="cython line score-2" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">573</span>:             <span class="bp">self</span><span class="o">.</span><span class="n">vecs</span> <span class="o">=</span> <span class="n">vecs</span></pre>
 <pre class='cython code score-2 '>  /*else*/ {
     <span class='pyx_macro_api'>__Pyx_INCREF</span>(__pyx_v_vecs);
     <span class='refnanny'>__Pyx_GIVEREF</span>(__pyx_v_vecs);
     <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_v_self-&gt;vecs);
     <span class='pyx_macro_api'>__Pyx_DECREF</span>(__pyx_v_self-&gt;vecs);
     __pyx_v_self-&gt;vecs = __pyx_v_vecs;
   }
   __pyx_L3:;
-</pre><pre class="cython line score-8" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">568</span>:         <span class="bp">self</span><span class="o">.</span><span class="n">vlen</span> <span class="o">=</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">vecs</span><span class="p">)</span></pre>
+</pre><pre class="cython line score-8" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">574</span>:         <span class="bp">self</span><span class="o">.</span><span class="n">vlen</span> <span class="o">=</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">vecs</span><span class="p">)</span></pre>
 <pre class='cython code score-8 '>  __pyx_t_7 = __pyx_v_self-&gt;vecs;
   <span class='pyx_macro_api'>__Pyx_INCREF</span>(__pyx_t_7);
   if (unlikely(__pyx_t_7 == Py_None)) {
     <span class='py_c_api'>PyErr_SetString</span>(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    <span class='error_goto'>__PYX_ERR(0, 568, __pyx_L1_error)</span>
+    <span class='error_goto'>__PYX_ERR(0, 574, __pyx_L1_error)</span>
   }
-  __pyx_t_3 = <span class='py_macro_api'>PyList_GET_SIZE</span>(__pyx_t_7);<span class='error_goto'> if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 568, __pyx_L1_error)</span>
+  __pyx_t_3 = <span class='py_macro_api'>PyList_GET_SIZE</span>(__pyx_t_7);<span class='error_goto'> if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 574, __pyx_L1_error)</span>
   <span class='pyx_macro_api'>__Pyx_DECREF</span>(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_v_self-&gt;vlen = __pyx_t_3;
-</pre><pre class="cython line score-0" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">569</span>:         <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">vlen</span> <span class="o">&lt;</span> <span class="mf">2</span><span class="p">:</span></pre>
+</pre><pre class="cython line score-0" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">575</span>:         <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">vlen</span> <span class="o">&lt;</span> <span class="mf">2</span><span class="p">:</span></pre>
 <pre class='cython code score-0 '>  __pyx_t_1 = ((__pyx_v_self-&gt;vlen &lt; 2) != 0);
   if (unlikely(__pyx_t_1)) {
 /* … */
   }
-</pre><pre class="cython line score-10" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">570</span>:             <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="n">f</span><span class="s">&#39;Слишком мало точек для линии. Необходимо больше, чем 1&#39;</span><span class="p">)</span></pre>
-<pre class='cython code score-10 '>    __pyx_t_7 = <span class='pyx_c_api'>__Pyx_PyObject_Call</span>(__pyx_builtin_ValueError, __pyx_tuple__15, NULL);<span class='error_goto'> if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 570, __pyx_L1_error)</span>
+</pre><pre class="cython line score-10" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">576</span>:             <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="n">f</span><span class="s">&#39;Слишком мало точек для линии. Необходимо больше, чем 1&#39;</span><span class="p">)</span></pre>
+<pre class='cython code score-10 '>    __pyx_t_7 = <span class='pyx_c_api'>__Pyx_PyObject_Call</span>(__pyx_builtin_ValueError, __pyx_tuple__15, NULL);<span class='error_goto'> if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 576, __pyx_L1_error)</span>
     <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_7);
     <span class='pyx_c_api'>__Pyx_Raise</span>(__pyx_t_7, 0, 0, 0);
     <span class='pyx_macro_api'>__Pyx_DECREF</span>(__pyx_t_7); __pyx_t_7 = 0;
-    <span class='error_goto'>__PYX_ERR(0, 570, __pyx_L1_error)</span>
+    <span class='error_goto'>__PYX_ERR(0, 576, __pyx_L1_error)</span>
 /* … */
-  __pyx_tuple__15 = <span class='py_c_api'>PyTuple_Pack</span>(1, __pyx_kp_u_1);<span class='error_goto'> if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 570, __pyx_L1_error)</span>
+  __pyx_tuple__15 = <span class='py_c_api'>PyTuple_Pack</span>(1, __pyx_kp_u_1);<span class='error_goto'> if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 576, __pyx_L1_error)</span>
   <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_tuple__15);
   <span class='refnanny'>__Pyx_GIVEREF</span>(__pyx_tuple__15);
-</pre><pre class="cython line score-7" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">571</span>:         <span class="bp">self</span><span class="o">.</span><span class="n">enclosed</span> <span class="o">=</span> <span class="n">enclosed</span></pre>
-<pre class='cython code score-7 '>  __pyx_t_1 = <span class='pyx_c_api'>__Pyx_PyObject_IsTrue</span>(__pyx_v_enclosed); if (unlikely((__pyx_t_1 == (int)-1) &amp;&amp; <span class='py_c_api'>PyErr_Occurred</span>())) <span class='error_goto'>__PYX_ERR(0, 571, __pyx_L1_error)</span>
+</pre><pre class="cython line score-7" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">577</span>:         <span class="bp">self</span><span class="o">.</span><span class="n">enclosed</span> <span class="o">=</span> <span class="n">enclosed</span></pre>
+<pre class='cython code score-7 '>  __pyx_t_1 = <span class='pyx_c_api'>__Pyx_PyObject_IsTrue</span>(__pyx_v_enclosed); if (unlikely((__pyx_t_1 == (int)-1) &amp;&amp; <span class='py_c_api'>PyErr_Occurred</span>())) <span class='error_goto'>__PYX_ERR(0, 577, __pyx_L1_error)</span>
   __pyx_v_self-&gt;enclosed = __pyx_t_1;
-</pre><pre class="cython line score-19" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">572</span>:         <span class="bp">self</span><span class="o">.</span><span class="n">bbox</span> <span class="o">=</span> <span class="n">Rect</span><span class="o">.</span><span class="n">bbox</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">vecs</span><span class="p">)</span></pre>
-<pre class='cython code score-19 '>  __pyx_t_2 = <span class='pyx_c_api'>__Pyx_PyObject_GetAttrStr</span>(((PyObject *)__pyx_ptype_7easyvec_8geometry_Rect), __pyx_n_s_bbox);<span class='error_goto'> if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 572, __pyx_L1_error)</span>
+</pre><pre class="cython line score-19" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">578</span>:         <span class="bp">self</span><span class="o">.</span><span class="n">bbox</span> <span class="o">=</span> <span class="n">Rect</span><span class="o">.</span><span class="n">bbox</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">vecs</span><span class="p">)</span></pre>
+<pre class='cython code score-19 '>  __pyx_t_2 = <span class='pyx_c_api'>__Pyx_PyObject_GetAttrStr</span>(((PyObject *)__pyx_ptype_7easyvec_8geometry_Rect), __pyx_n_s_bbox);<span class='error_goto'> if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 578, __pyx_L1_error)</span>
   <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_2);
   __pyx_t_9 = NULL;
   if (CYTHON_UNPACK_METHODS &amp;&amp; likely(<span class='py_c_api'>PyMethod_Check</span>(__pyx_t_2))) {
     __pyx_t_9 = <span class='py_macro_api'>PyMethod_GET_SELF</span>(__pyx_t_2);
     if (likely(__pyx_t_9)) {
       PyObject* function = <span class='py_macro_api'>PyMethod_GET_FUNCTION</span>(__pyx_t_2);
       <span class='pyx_macro_api'>__Pyx_INCREF</span>(__pyx_t_9);
       <span class='pyx_macro_api'>__Pyx_INCREF</span>(function);
       <span class='pyx_macro_api'>__Pyx_DECREF_SET</span>(__pyx_t_2, function);
     }
   }
   __pyx_t_7 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_9, __pyx_v_self-&gt;vecs) : <span class='pyx_c_api'>__Pyx_PyObject_CallOneArg</span>(__pyx_t_2, __pyx_v_self-&gt;vecs);
   <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_t_9); __pyx_t_9 = 0;
-  if (unlikely(!__pyx_t_7)) <span class='error_goto'>__PYX_ERR(0, 572, __pyx_L1_error)</span>
+  if (unlikely(!__pyx_t_7)) <span class='error_goto'>__PYX_ERR(0, 578, __pyx_L1_error)</span>
   <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_7);
   <span class='pyx_macro_api'>__Pyx_DECREF</span>(__pyx_t_2); __pyx_t_2 = 0;
-  if (!(likely(((__pyx_t_7) == Py_None) || likely(<span class='pyx_c_api'>__Pyx_TypeTest</span>(__pyx_t_7, __pyx_ptype_7easyvec_8geometry_Rect))))) <span class='error_goto'>__PYX_ERR(0, 572, __pyx_L1_error)</span>
+  if (!(likely(((__pyx_t_7) == Py_None) || likely(<span class='pyx_c_api'>__Pyx_TypeTest</span>(__pyx_t_7, __pyx_ptype_7easyvec_8geometry_Rect))))) <span class='error_goto'>__PYX_ERR(0, 578, __pyx_L1_error)</span>
   <span class='refnanny'>__Pyx_GIVEREF</span>(__pyx_t_7);
   <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_v_self-&gt;bbox);
   <span class='pyx_macro_api'>__Pyx_DECREF</span>(((PyObject *)__pyx_v_self-&gt;bbox));
   __pyx_v_self-&gt;bbox = ((struct __pyx_obj_7easyvec_8geometry_Rect *)__pyx_t_7);
   __pyx_t_7 = 0;
-</pre><pre class="cython line score-0">&#xA0;<span class="">573</span>: </pre>
-<pre class="cython line score-9" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">574</span>:     <span class="k">def</span> <span class="nf">__str__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span></pre>
+</pre><pre class="cython line score-0">&#xA0;<span class="">579</span>: </pre>
+<pre class="cython line score-9" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">580</span>:     <span class="k">def</span> <span class="nf">to_dict</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span></pre>
 <pre class='cython code score-9 '>/* Python wrapper */
-static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_3__str__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_3__str__(PyObject *__pyx_v_self) {
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_5to_dict(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_7easyvec_8geometry_8PolyLine_4to_dict[] = "PolyLine.to_dict(self)";
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_5to_dict(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+  PyObject *__pyx_r = 0;
+  <span class='refnanny'>__Pyx_RefNannyDeclarations</span>
+  <span class='refnanny'>__Pyx_RefNannySetupContext</span>("to_dict (wrapper)", 0);
+  __pyx_r = __pyx_pf_7easyvec_8geometry_8PolyLine_4to_dict(((struct __pyx_obj_7easyvec_8geometry_PolyLine *)__pyx_v_self));
+
+  /* function exit code */
+  <span class='refnanny'>__Pyx_RefNannyFinishContext</span>();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_4to_dict(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self) {
+  PyObject *__pyx_8genexpr1__pyx_v_v = NULL;
+  PyObject *__pyx_r = NULL;
+  <span class='refnanny'>__Pyx_RefNannyDeclarations</span>
+  <span class='refnanny'>__Pyx_RefNannySetupContext</span>("to_dict", 0);
+/* … */
+  /* function exit code */
+  __pyx_L1_error:;
+  <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_t_1);
+  <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_t_2);
+  <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_t_3);
+  <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_t_5);
+  <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_t_6);
+  <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_t_7);
+  <span class='pyx_c_api'>__Pyx_AddTraceback</span>("easyvec.geometry.PolyLine.to_dict", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_8genexpr1__pyx_v_v);
+  <span class='refnanny'>__Pyx_XGIVEREF</span>(__pyx_r);
+  <span class='refnanny'>__Pyx_RefNannyFinishContext</span>();
+  return __pyx_r;
+}
+</pre><pre class="cython line score-1" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">581</span>:         <span class="k">return</span> <span class="p">{</span></pre>
+<pre class='cython code score-1 '>  <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_r);
+</pre><pre class="cython line score-48" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">582</span>:             <span class="s">&#39;vecs&#39;</span><span class="p">:</span> <span class="p">[</span><span class="n">v</span><span class="o">.</span><span class="n">to_dict</span><span class="p">()</span> <span class="k">for</span> <span class="n">v</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">vecs</span><span class="p">],</span></pre>
+<pre class='cython code score-48 '>  __pyx_t_1 = <span class='pyx_c_api'>__Pyx_PyDict_NewPresized</span>(2);<span class='error_goto'> if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 582, __pyx_L1_error)</span>
+  <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_1);
+  { /* enter inner scope */
+    __pyx_t_2 = <span class='py_c_api'>PyList_New</span>(0);<span class='error_goto'> if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 582, __pyx_L5_error)</span>
+    <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_2);
+    if (unlikely(__pyx_v_self-&gt;vecs == Py_None)) {
+      <span class='py_c_api'>PyErr_SetString</span>(PyExc_TypeError, "'NoneType' object is not iterable");
+      <span class='error_goto'>__PYX_ERR(0, 582, __pyx_L5_error)</span>
+    }
+    __pyx_t_3 = __pyx_v_self-&gt;vecs; <span class='pyx_macro_api'>__Pyx_INCREF</span>(__pyx_t_3); __pyx_t_4 = 0;
+    for (;;) {
+      if (__pyx_t_4 &gt;= <span class='py_macro_api'>PyList_GET_SIZE</span>(__pyx_t_3)) break;
+      #if CYTHON_ASSUME_SAFE_MACROS &amp;&amp; !CYTHON_AVOID_BORROWED_REFS
+      __pyx_t_5 = <span class='py_macro_api'>PyList_GET_ITEM</span>(__pyx_t_3, __pyx_t_4); <span class='pyx_macro_api'>__Pyx_INCREF</span>(__pyx_t_5); __pyx_t_4++; if (unlikely(0 &lt; 0)) <span class='error_goto'>__PYX_ERR(0, 582, __pyx_L5_error)</span>
+      #else
+      __pyx_t_5 = <span class='py_macro_api'>PySequence_ITEM</span>(__pyx_t_3, __pyx_t_4); __pyx_t_4++;<span class='error_goto'> if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 582, __pyx_L5_error)</span>
+      <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_5);
+      #endif
+      <span class='pyx_macro_api'>__Pyx_XDECREF_SET</span>(__pyx_8genexpr1__pyx_v_v, __pyx_t_5);
+      __pyx_t_5 = 0;
+      __pyx_t_6 = <span class='pyx_c_api'>__Pyx_PyObject_GetAttrStr</span>(__pyx_8genexpr1__pyx_v_v, __pyx_n_s_to_dict);<span class='error_goto'> if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 582, __pyx_L5_error)</span>
+      <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_6);
+      __pyx_t_7 = NULL;
+      if (CYTHON_UNPACK_METHODS &amp;&amp; likely(<span class='py_c_api'>PyMethod_Check</span>(__pyx_t_6))) {
+        __pyx_t_7 = <span class='py_macro_api'>PyMethod_GET_SELF</span>(__pyx_t_6);
+        if (likely(__pyx_t_7)) {
+          PyObject* function = <span class='py_macro_api'>PyMethod_GET_FUNCTION</span>(__pyx_t_6);
+          <span class='pyx_macro_api'>__Pyx_INCREF</span>(__pyx_t_7);
+          <span class='pyx_macro_api'>__Pyx_INCREF</span>(function);
+          <span class='pyx_macro_api'>__Pyx_DECREF_SET</span>(__pyx_t_6, function);
+        }
+      }
+      __pyx_t_5 = (__pyx_t_7) ? <span class='pyx_c_api'>__Pyx_PyObject_CallOneArg</span>(__pyx_t_6, __pyx_t_7) : <span class='pyx_c_api'>__Pyx_PyObject_CallNoArg</span>(__pyx_t_6);
+      <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_t_7); __pyx_t_7 = 0;
+      if (unlikely(!__pyx_t_5)) <span class='error_goto'>__PYX_ERR(0, 582, __pyx_L5_error)</span>
+      <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_5);
+      <span class='pyx_macro_api'>__Pyx_DECREF</span>(__pyx_t_6); __pyx_t_6 = 0;
+      if (unlikely(<span class='pyx_c_api'>__Pyx_ListComp_Append</span>(__pyx_t_2, (PyObject*)__pyx_t_5))) <span class='error_goto'>__PYX_ERR(0, 582, __pyx_L5_error)</span>
+      <span class='pyx_macro_api'>__Pyx_DECREF</span>(__pyx_t_5); __pyx_t_5 = 0;
+    }
+    <span class='pyx_macro_api'>__Pyx_DECREF</span>(__pyx_t_3); __pyx_t_3 = 0;
+    <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_8genexpr1__pyx_v_v); __pyx_8genexpr1__pyx_v_v = 0;
+    goto __pyx_L8_exit_scope;
+    __pyx_L5_error:;
+    <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_8genexpr1__pyx_v_v); __pyx_8genexpr1__pyx_v_v = 0;
+    goto __pyx_L1_error;
+    __pyx_L8_exit_scope:;
+  } /* exit inner scope */
+  if (<span class='py_c_api'>PyDict_SetItem</span>(__pyx_t_1, __pyx_n_u_vecs, __pyx_t_2) &lt; 0) <span class='error_goto'>__PYX_ERR(0, 582, __pyx_L1_error)</span>
+  <span class='pyx_macro_api'>__Pyx_DECREF</span>(__pyx_t_2); __pyx_t_2 = 0;
+</pre><pre class="cython line score-8" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">583</span>:             <span class="s">&#39;enclosed&#39;</span><span class="p">:</span> <span class="nb">bool</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">enclosed</span><span class="p">)</span></pre>
+<pre class='cython code score-8 '>  __pyx_t_8 = __pyx_v_self-&gt;enclosed;
+  __pyx_t_2 = <span class='pyx_c_api'>__Pyx_PyBool_FromLong</span>((!(!__pyx_t_8)));<span class='error_goto'> if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 583, __pyx_L1_error)</span>
+  <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_2);
+  if (<span class='py_c_api'>PyDict_SetItem</span>(__pyx_t_1, __pyx_n_u_enclosed, __pyx_t_2) &lt; 0) <span class='error_goto'>__PYX_ERR(0, 582, __pyx_L1_error)</span>
+  <span class='pyx_macro_api'>__Pyx_DECREF</span>(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+</pre><pre class="cython line score-0">&#xA0;<span class="">584</span>:         <span class="p">}</span></pre>
+<pre class="cython line score-0">&#xA0;<span class="">585</span>: </pre>
+<pre class="cython line score-9" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">586</span>:     <span class="k">def</span> <span class="nf">__str__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span></pre>
+<pre class='cython code score-9 '>/* Python wrapper */
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_7__str__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_7__str__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   <span class='refnanny'>__Pyx_RefNannyDeclarations</span>
   <span class='refnanny'>__Pyx_RefNannySetupContext</span>("__str__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_7easyvec_8geometry_8PolyLine_2__str__(((struct __pyx_obj_7easyvec_8geometry_PolyLine *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7easyvec_8geometry_8PolyLine_6__str__(((struct __pyx_obj_7easyvec_8geometry_PolyLine *)__pyx_v_self));
 
   /* function exit code */
   <span class='refnanny'>__Pyx_RefNannyFinishContext</span>();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_2__str__(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self) {
+static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_6__str__(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self) {
   PyObject *__pyx_v_s = NULL;
-  PyObject *__pyx_7genexpr__pyx_v_v = NULL;
+  PyObject *__pyx_8genexpr2__pyx_v_v = NULL;
   PyObject *__pyx_r = NULL;
   <span class='refnanny'>__Pyx_RefNannyDeclarations</span>
   <span class='refnanny'>__Pyx_RefNannySetupContext</span>("__str__", 0);
 /* … */
   /* function exit code */
   __pyx_L1_error:;
   <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_t_1);
@@ -8055,140 +8306,140 @@
   <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_t_4);
   <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_t_7);
   <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_t_8);
   <span class='pyx_c_api'>__Pyx_AddTraceback</span>("easyvec.geometry.PolyLine.__str__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_v_s);
-  <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_7genexpr__pyx_v_v);
+  <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_8genexpr2__pyx_v_v);
   <span class='refnanny'>__Pyx_XGIVEREF</span>(__pyx_r);
   <span class='refnanny'>__Pyx_RefNannyFinishContext</span>();
   return __pyx_r;
 }
-</pre><pre class="cython line score-60" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">575</span>:         <span class="n">s</span> <span class="o">=</span> <span class="p">[</span><span class="n">f</span><span class="s">&#39;({v.x:.2f}, {v.y:.2f})&#39;</span> <span class="k">for</span> <span class="n">v</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">vecs</span><span class="p">]</span></pre>
+</pre><pre class="cython line score-60" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">587</span>:         <span class="n">s</span> <span class="o">=</span> <span class="p">[</span><span class="n">f</span><span class="s">&#39;({v.x:.2f}, {v.y:.2f})&#39;</span> <span class="k">for</span> <span class="n">v</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">vecs</span><span class="p">]</span></pre>
 <pre class='cython code score-60 '>  { /* enter inner scope */
-    __pyx_t_1 = <span class='py_c_api'>PyList_New</span>(0);<span class='error_goto'> if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 575, __pyx_L5_error)</span>
+    __pyx_t_1 = <span class='py_c_api'>PyList_New</span>(0);<span class='error_goto'> if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 587, __pyx_L5_error)</span>
     <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_1);
     if (unlikely(__pyx_v_self-&gt;vecs == Py_None)) {
       <span class='py_c_api'>PyErr_SetString</span>(PyExc_TypeError, "'NoneType' object is not iterable");
-      <span class='error_goto'>__PYX_ERR(0, 575, __pyx_L5_error)</span>
+      <span class='error_goto'>__PYX_ERR(0, 587, __pyx_L5_error)</span>
     }
     __pyx_t_2 = __pyx_v_self-&gt;vecs; <span class='pyx_macro_api'>__Pyx_INCREF</span>(__pyx_t_2); __pyx_t_3 = 0;
     for (;;) {
       if (__pyx_t_3 &gt;= <span class='py_macro_api'>PyList_GET_SIZE</span>(__pyx_t_2)) break;
       #if CYTHON_ASSUME_SAFE_MACROS &amp;&amp; !CYTHON_AVOID_BORROWED_REFS
-      __pyx_t_4 = <span class='py_macro_api'>PyList_GET_ITEM</span>(__pyx_t_2, __pyx_t_3); <span class='pyx_macro_api'>__Pyx_INCREF</span>(__pyx_t_4); __pyx_t_3++; if (unlikely(0 &lt; 0)) <span class='error_goto'>__PYX_ERR(0, 575, __pyx_L5_error)</span>
+      __pyx_t_4 = <span class='py_macro_api'>PyList_GET_ITEM</span>(__pyx_t_2, __pyx_t_3); <span class='pyx_macro_api'>__Pyx_INCREF</span>(__pyx_t_4); __pyx_t_3++; if (unlikely(0 &lt; 0)) <span class='error_goto'>__PYX_ERR(0, 587, __pyx_L5_error)</span>
       #else
-      __pyx_t_4 = <span class='py_macro_api'>PySequence_ITEM</span>(__pyx_t_2, __pyx_t_3); __pyx_t_3++;<span class='error_goto'> if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 575, __pyx_L5_error)</span>
+      __pyx_t_4 = <span class='py_macro_api'>PySequence_ITEM</span>(__pyx_t_2, __pyx_t_3); __pyx_t_3++;<span class='error_goto'> if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 587, __pyx_L5_error)</span>
       <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_4);
       #endif
-      <span class='pyx_macro_api'>__Pyx_XDECREF_SET</span>(__pyx_7genexpr__pyx_v_v, __pyx_t_4);
+      <span class='pyx_macro_api'>__Pyx_XDECREF_SET</span>(__pyx_8genexpr2__pyx_v_v, __pyx_t_4);
       __pyx_t_4 = 0;
-      __pyx_t_4 = <span class='py_c_api'>PyTuple_New</span>(5);<span class='error_goto'> if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 575, __pyx_L5_error)</span>
+      __pyx_t_4 = <span class='py_c_api'>PyTuple_New</span>(5);<span class='error_goto'> if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 587, __pyx_L5_error)</span>
       <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_4);
       __pyx_t_5 = 0;
       __pyx_t_6 = 127;
       <span class='pyx_macro_api'>__Pyx_INCREF</span>(__pyx_kp_u__16);
       __pyx_t_5 += 1;
       <span class='refnanny'>__Pyx_GIVEREF</span>(__pyx_kp_u__16);
       <span class='py_macro_api'>PyTuple_SET_ITEM</span>(__pyx_t_4, 0, __pyx_kp_u__16);
-      __pyx_t_7 = <span class='pyx_c_api'>__Pyx_PyObject_GetAttrStr</span>(__pyx_7genexpr__pyx_v_v, __pyx_n_s_x);<span class='error_goto'> if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 575, __pyx_L5_error)</span>
+      __pyx_t_7 = <span class='pyx_c_api'>__Pyx_PyObject_GetAttrStr</span>(__pyx_8genexpr2__pyx_v_v, __pyx_n_s_x);<span class='error_goto'> if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 587, __pyx_L5_error)</span>
       <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_7);
-      __pyx_t_8 = <span class='pyx_c_api'>__Pyx_PyObject_Format</span>(__pyx_t_7, __pyx_kp_u_2f);<span class='error_goto'> if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 575, __pyx_L5_error)</span>
+      __pyx_t_8 = <span class='pyx_c_api'>__Pyx_PyObject_Format</span>(__pyx_t_7, __pyx_kp_u_2f);<span class='error_goto'> if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 587, __pyx_L5_error)</span>
       <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_8);
       <span class='pyx_macro_api'>__Pyx_DECREF</span>(__pyx_t_7); __pyx_t_7 = 0;
       __pyx_t_6 = (<span class='pyx_c_api'>__Pyx_PyUnicode_MAX_CHAR_VALUE</span>(__pyx_t_8) &gt; __pyx_t_6) ? <span class='pyx_c_api'>__Pyx_PyUnicode_MAX_CHAR_VALUE</span>(__pyx_t_8) : __pyx_t_6;
       __pyx_t_5 += <span class='pyx_c_api'>__Pyx_PyUnicode_GET_LENGTH</span>(__pyx_t_8);
       <span class='refnanny'>__Pyx_GIVEREF</span>(__pyx_t_8);
       <span class='py_macro_api'>PyTuple_SET_ITEM</span>(__pyx_t_4, 1, __pyx_t_8);
       __pyx_t_8 = 0;
       <span class='pyx_macro_api'>__Pyx_INCREF</span>(__pyx_kp_u__4);
       __pyx_t_5 += 2;
       <span class='refnanny'>__Pyx_GIVEREF</span>(__pyx_kp_u__4);
       <span class='py_macro_api'>PyTuple_SET_ITEM</span>(__pyx_t_4, 2, __pyx_kp_u__4);
-      __pyx_t_8 = <span class='pyx_c_api'>__Pyx_PyObject_GetAttrStr</span>(__pyx_7genexpr__pyx_v_v, __pyx_n_s_y);<span class='error_goto'> if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 575, __pyx_L5_error)</span>
+      __pyx_t_8 = <span class='pyx_c_api'>__Pyx_PyObject_GetAttrStr</span>(__pyx_8genexpr2__pyx_v_v, __pyx_n_s_y);<span class='error_goto'> if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 587, __pyx_L5_error)</span>
       <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_8);
-      __pyx_t_7 = <span class='pyx_c_api'>__Pyx_PyObject_Format</span>(__pyx_t_8, __pyx_kp_u_2f);<span class='error_goto'> if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 575, __pyx_L5_error)</span>
+      __pyx_t_7 = <span class='pyx_c_api'>__Pyx_PyObject_Format</span>(__pyx_t_8, __pyx_kp_u_2f);<span class='error_goto'> if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 587, __pyx_L5_error)</span>
       <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_7);
       <span class='pyx_macro_api'>__Pyx_DECREF</span>(__pyx_t_8); __pyx_t_8 = 0;
       __pyx_t_6 = (<span class='pyx_c_api'>__Pyx_PyUnicode_MAX_CHAR_VALUE</span>(__pyx_t_7) &gt; __pyx_t_6) ? <span class='pyx_c_api'>__Pyx_PyUnicode_MAX_CHAR_VALUE</span>(__pyx_t_7) : __pyx_t_6;
       __pyx_t_5 += <span class='pyx_c_api'>__Pyx_PyUnicode_GET_LENGTH</span>(__pyx_t_7);
       <span class='refnanny'>__Pyx_GIVEREF</span>(__pyx_t_7);
       <span class='py_macro_api'>PyTuple_SET_ITEM</span>(__pyx_t_4, 3, __pyx_t_7);
       __pyx_t_7 = 0;
       <span class='pyx_macro_api'>__Pyx_INCREF</span>(__pyx_kp_u__5);
       __pyx_t_5 += 1;
       <span class='refnanny'>__Pyx_GIVEREF</span>(__pyx_kp_u__5);
       <span class='py_macro_api'>PyTuple_SET_ITEM</span>(__pyx_t_4, 4, __pyx_kp_u__5);
-      __pyx_t_7 = <span class='pyx_c_api'>__Pyx_PyUnicode_Join</span>(__pyx_t_4, 5, __pyx_t_5, __pyx_t_6);<span class='error_goto'> if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 575, __pyx_L5_error)</span>
+      __pyx_t_7 = <span class='pyx_c_api'>__Pyx_PyUnicode_Join</span>(__pyx_t_4, 5, __pyx_t_5, __pyx_t_6);<span class='error_goto'> if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 587, __pyx_L5_error)</span>
       <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_7);
       <span class='pyx_macro_api'>__Pyx_DECREF</span>(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(<span class='pyx_c_api'>__Pyx_ListComp_Append</span>(__pyx_t_1, (PyObject*)__pyx_t_7))) <span class='error_goto'>__PYX_ERR(0, 575, __pyx_L5_error)</span>
+      if (unlikely(<span class='pyx_c_api'>__Pyx_ListComp_Append</span>(__pyx_t_1, (PyObject*)__pyx_t_7))) <span class='error_goto'>__PYX_ERR(0, 587, __pyx_L5_error)</span>
       <span class='pyx_macro_api'>__Pyx_DECREF</span>(__pyx_t_7); __pyx_t_7 = 0;
     }
     <span class='pyx_macro_api'>__Pyx_DECREF</span>(__pyx_t_2); __pyx_t_2 = 0;
-    <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_7genexpr__pyx_v_v); __pyx_7genexpr__pyx_v_v = 0;
+    <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_8genexpr2__pyx_v_v); __pyx_8genexpr2__pyx_v_v = 0;
     goto __pyx_L8_exit_scope;
     __pyx_L5_error:;
-    <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_7genexpr__pyx_v_v); __pyx_7genexpr__pyx_v_v = 0;
+    <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_8genexpr2__pyx_v_v); __pyx_8genexpr2__pyx_v_v = 0;
     goto __pyx_L1_error;
     __pyx_L8_exit_scope:;
   } /* exit inner scope */
   __pyx_v_s = __pyx_t_1;
   __pyx_t_1 = 0;
-</pre><pre class="cython line score-6" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">576</span>:         <span class="n">s</span> <span class="o">=</span> <span class="s">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">s</span><span class="p">)</span></pre>
-<pre class='cython code score-6 '>  __pyx_t_1 = <span class='py_c_api'>PyUnicode_Join</span>(__pyx_kp_u__4, __pyx_v_s);<span class='error_goto'> if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 576, __pyx_L1_error)</span>
+</pre><pre class="cython line score-6" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">588</span>:         <span class="n">s</span> <span class="o">=</span> <span class="s">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">s</span><span class="p">)</span></pre>
+<pre class='cython code score-6 '>  __pyx_t_1 = <span class='py_c_api'>PyUnicode_Join</span>(__pyx_kp_u__4, __pyx_v_s);<span class='error_goto'> if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 588, __pyx_L1_error)</span>
   <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_1);
   <span class='pyx_macro_api'>__Pyx_DECREF_SET</span>(__pyx_v_s, __pyx_t_1);
   __pyx_t_1 = 0;
-</pre><pre class="cython line score-22" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">577</span>:         <span class="k">return</span> <span class="n">f</span><span class="s">&#39;PolyLine({s})&#39;</span></pre>
+</pre><pre class="cython line score-22" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">589</span>:         <span class="k">return</span> <span class="n">f</span><span class="s">&#39;PolyLine({s})&#39;</span></pre>
 <pre class='cython code score-22 '>  <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_r);
-  __pyx_t_1 = <span class='py_c_api'>PyTuple_New</span>(3);<span class='error_goto'> if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 577, __pyx_L1_error)</span>
+  __pyx_t_1 = <span class='py_c_api'>PyTuple_New</span>(3);<span class='error_goto'> if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 589, __pyx_L1_error)</span>
   <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_1);
   __pyx_t_3 = 0;
   __pyx_t_6 = 127;
   <span class='pyx_macro_api'>__Pyx_INCREF</span>(__pyx_kp_u_PolyLine);
   __pyx_t_3 += 9;
   <span class='refnanny'>__Pyx_GIVEREF</span>(__pyx_kp_u_PolyLine);
   <span class='py_macro_api'>PyTuple_SET_ITEM</span>(__pyx_t_1, 0, __pyx_kp_u_PolyLine);
-  __pyx_t_2 = <span class='pyx_c_api'>__Pyx_PyObject_FormatSimple</span>(__pyx_v_s, __pyx_empty_unicode);<span class='error_goto'> if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 577, __pyx_L1_error)</span>
+  __pyx_t_2 = <span class='pyx_c_api'>__Pyx_PyObject_FormatSimple</span>(__pyx_v_s, __pyx_empty_unicode);<span class='error_goto'> if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 589, __pyx_L1_error)</span>
   <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_2);
   __pyx_t_6 = (<span class='pyx_c_api'>__Pyx_PyUnicode_MAX_CHAR_VALUE</span>(__pyx_t_2) &gt; __pyx_t_6) ? <span class='pyx_c_api'>__Pyx_PyUnicode_MAX_CHAR_VALUE</span>(__pyx_t_2) : __pyx_t_6;
   __pyx_t_3 += <span class='pyx_c_api'>__Pyx_PyUnicode_GET_LENGTH</span>(__pyx_t_2);
   <span class='refnanny'>__Pyx_GIVEREF</span>(__pyx_t_2);
   <span class='py_macro_api'>PyTuple_SET_ITEM</span>(__pyx_t_1, 1, __pyx_t_2);
   __pyx_t_2 = 0;
   <span class='pyx_macro_api'>__Pyx_INCREF</span>(__pyx_kp_u__5);
   __pyx_t_3 += 1;
   <span class='refnanny'>__Pyx_GIVEREF</span>(__pyx_kp_u__5);
   <span class='py_macro_api'>PyTuple_SET_ITEM</span>(__pyx_t_1, 2, __pyx_kp_u__5);
-  __pyx_t_2 = <span class='pyx_c_api'>__Pyx_PyUnicode_Join</span>(__pyx_t_1, 3, __pyx_t_3, __pyx_t_6);<span class='error_goto'> if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 577, __pyx_L1_error)</span>
+  __pyx_t_2 = <span class='pyx_c_api'>__Pyx_PyUnicode_Join</span>(__pyx_t_1, 3, __pyx_t_3, __pyx_t_6);<span class='error_goto'> if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 589, __pyx_L1_error)</span>
   <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_2);
   <span class='pyx_macro_api'>__Pyx_DECREF</span>(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
-</pre><pre class="cython line score-0">&#xA0;<span class="">578</span>: </pre>
-<pre class="cython line score-9" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">579</span>:     <span class="k">def</span> <span class="nf">__repr__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span></pre>
+</pre><pre class="cython line score-0">&#xA0;<span class="">590</span>: </pre>
+<pre class="cython line score-9" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">591</span>:     <span class="k">def</span> <span class="nf">__repr__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span></pre>
 <pre class='cython code score-9 '>/* Python wrapper */
-static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_5__repr__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_5__repr__(PyObject *__pyx_v_self) {
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_9__repr__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_9__repr__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   <span class='refnanny'>__Pyx_RefNannyDeclarations</span>
   <span class='refnanny'>__Pyx_RefNannySetupContext</span>("__repr__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_7easyvec_8geometry_8PolyLine_4__repr__(((struct __pyx_obj_7easyvec_8geometry_PolyLine *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7easyvec_8geometry_8PolyLine_8__repr__(((struct __pyx_obj_7easyvec_8geometry_PolyLine *)__pyx_v_self));
 
   /* function exit code */
   <span class='refnanny'>__Pyx_RefNannyFinishContext</span>();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_4__repr__(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self) {
+static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_8__repr__(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self) {
   PyObject *__pyx_v_s = NULL;
-  PyObject *__pyx_8genexpr1__pyx_v_v = NULL;
+  PyObject *__pyx_8genexpr3__pyx_v_v = NULL;
   PyObject *__pyx_r = NULL;
   <span class='refnanny'>__Pyx_RefNannyDeclarations</span>
   <span class='refnanny'>__Pyx_RefNannySetupContext</span>("__repr__", 0);
 /* … */
   /* function exit code */
   __pyx_L1_error:;
   <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_t_1);
@@ -8196,138 +8447,138 @@
   <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_t_4);
   <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_t_7);
   <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_t_8);
   <span class='pyx_c_api'>__Pyx_AddTraceback</span>("easyvec.geometry.PolyLine.__repr__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_v_s);
-  <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_8genexpr1__pyx_v_v);
+  <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_8genexpr3__pyx_v_v);
   <span class='refnanny'>__Pyx_XGIVEREF</span>(__pyx_r);
   <span class='refnanny'>__Pyx_RefNannyFinishContext</span>();
   return __pyx_r;
 }
-</pre><pre class="cython line score-60" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">580</span>:         <span class="n">s</span> <span class="o">=</span> <span class="p">[</span><span class="n">f</span><span class="s">&#39;({v.x}, {v.y})&#39;</span> <span class="k">for</span> <span class="n">v</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">vecs</span><span class="p">]</span></pre>
+</pre><pre class="cython line score-60" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">592</span>:         <span class="n">s</span> <span class="o">=</span> <span class="p">[</span><span class="n">f</span><span class="s">&#39;({v.x}, {v.y})&#39;</span> <span class="k">for</span> <span class="n">v</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">vecs</span><span class="p">]</span></pre>
 <pre class='cython code score-60 '>  { /* enter inner scope */
-    __pyx_t_1 = <span class='py_c_api'>PyList_New</span>(0);<span class='error_goto'> if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 580, __pyx_L5_error)</span>
+    __pyx_t_1 = <span class='py_c_api'>PyList_New</span>(0);<span class='error_goto'> if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 592, __pyx_L5_error)</span>
     <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_1);
     if (unlikely(__pyx_v_self-&gt;vecs == Py_None)) {
       <span class='py_c_api'>PyErr_SetString</span>(PyExc_TypeError, "'NoneType' object is not iterable");
-      <span class='error_goto'>__PYX_ERR(0, 580, __pyx_L5_error)</span>
+      <span class='error_goto'>__PYX_ERR(0, 592, __pyx_L5_error)</span>
     }
     __pyx_t_2 = __pyx_v_self-&gt;vecs; <span class='pyx_macro_api'>__Pyx_INCREF</span>(__pyx_t_2); __pyx_t_3 = 0;
     for (;;) {
       if (__pyx_t_3 &gt;= <span class='py_macro_api'>PyList_GET_SIZE</span>(__pyx_t_2)) break;
       #if CYTHON_ASSUME_SAFE_MACROS &amp;&amp; !CYTHON_AVOID_BORROWED_REFS
-      __pyx_t_4 = <span class='py_macro_api'>PyList_GET_ITEM</span>(__pyx_t_2, __pyx_t_3); <span class='pyx_macro_api'>__Pyx_INCREF</span>(__pyx_t_4); __pyx_t_3++; if (unlikely(0 &lt; 0)) <span class='error_goto'>__PYX_ERR(0, 580, __pyx_L5_error)</span>
+      __pyx_t_4 = <span class='py_macro_api'>PyList_GET_ITEM</span>(__pyx_t_2, __pyx_t_3); <span class='pyx_macro_api'>__Pyx_INCREF</span>(__pyx_t_4); __pyx_t_3++; if (unlikely(0 &lt; 0)) <span class='error_goto'>__PYX_ERR(0, 592, __pyx_L5_error)</span>
       #else
-      __pyx_t_4 = <span class='py_macro_api'>PySequence_ITEM</span>(__pyx_t_2, __pyx_t_3); __pyx_t_3++;<span class='error_goto'> if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 580, __pyx_L5_error)</span>
+      __pyx_t_4 = <span class='py_macro_api'>PySequence_ITEM</span>(__pyx_t_2, __pyx_t_3); __pyx_t_3++;<span class='error_goto'> if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 592, __pyx_L5_error)</span>
       <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_4);
       #endif
-      <span class='pyx_macro_api'>__Pyx_XDECREF_SET</span>(__pyx_8genexpr1__pyx_v_v, __pyx_t_4);
+      <span class='pyx_macro_api'>__Pyx_XDECREF_SET</span>(__pyx_8genexpr3__pyx_v_v, __pyx_t_4);
       __pyx_t_4 = 0;
-      __pyx_t_4 = <span class='py_c_api'>PyTuple_New</span>(5);<span class='error_goto'> if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 580, __pyx_L5_error)</span>
+      __pyx_t_4 = <span class='py_c_api'>PyTuple_New</span>(5);<span class='error_goto'> if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 592, __pyx_L5_error)</span>
       <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_4);
       __pyx_t_5 = 0;
       __pyx_t_6 = 127;
       <span class='pyx_macro_api'>__Pyx_INCREF</span>(__pyx_kp_u__16);
       __pyx_t_5 += 1;
       <span class='refnanny'>__Pyx_GIVEREF</span>(__pyx_kp_u__16);
       <span class='py_macro_api'>PyTuple_SET_ITEM</span>(__pyx_t_4, 0, __pyx_kp_u__16);
-      __pyx_t_7 = <span class='pyx_c_api'>__Pyx_PyObject_GetAttrStr</span>(__pyx_8genexpr1__pyx_v_v, __pyx_n_s_x);<span class='error_goto'> if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 580, __pyx_L5_error)</span>
+      __pyx_t_7 = <span class='pyx_c_api'>__Pyx_PyObject_GetAttrStr</span>(__pyx_8genexpr3__pyx_v_v, __pyx_n_s_x);<span class='error_goto'> if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 592, __pyx_L5_error)</span>
       <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_7);
-      __pyx_t_8 = <span class='pyx_c_api'>__Pyx_PyObject_FormatSimple</span>(__pyx_t_7, __pyx_empty_unicode);<span class='error_goto'> if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 580, __pyx_L5_error)</span>
+      __pyx_t_8 = <span class='pyx_c_api'>__Pyx_PyObject_FormatSimple</span>(__pyx_t_7, __pyx_empty_unicode);<span class='error_goto'> if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 592, __pyx_L5_error)</span>
       <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_8);
       <span class='pyx_macro_api'>__Pyx_DECREF</span>(__pyx_t_7); __pyx_t_7 = 0;
       __pyx_t_6 = (<span class='pyx_c_api'>__Pyx_PyUnicode_MAX_CHAR_VALUE</span>(__pyx_t_8) &gt; __pyx_t_6) ? <span class='pyx_c_api'>__Pyx_PyUnicode_MAX_CHAR_VALUE</span>(__pyx_t_8) : __pyx_t_6;
       __pyx_t_5 += <span class='pyx_c_api'>__Pyx_PyUnicode_GET_LENGTH</span>(__pyx_t_8);
       <span class='refnanny'>__Pyx_GIVEREF</span>(__pyx_t_8);
       <span class='py_macro_api'>PyTuple_SET_ITEM</span>(__pyx_t_4, 1, __pyx_t_8);
       __pyx_t_8 = 0;
       <span class='pyx_macro_api'>__Pyx_INCREF</span>(__pyx_kp_u__4);
       __pyx_t_5 += 2;
       <span class='refnanny'>__Pyx_GIVEREF</span>(__pyx_kp_u__4);
       <span class='py_macro_api'>PyTuple_SET_ITEM</span>(__pyx_t_4, 2, __pyx_kp_u__4);
-      __pyx_t_8 = <span class='pyx_c_api'>__Pyx_PyObject_GetAttrStr</span>(__pyx_8genexpr1__pyx_v_v, __pyx_n_s_y);<span class='error_goto'> if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 580, __pyx_L5_error)</span>
+      __pyx_t_8 = <span class='pyx_c_api'>__Pyx_PyObject_GetAttrStr</span>(__pyx_8genexpr3__pyx_v_v, __pyx_n_s_y);<span class='error_goto'> if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 592, __pyx_L5_error)</span>
       <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_8);
-      __pyx_t_7 = <span class='pyx_c_api'>__Pyx_PyObject_FormatSimple</span>(__pyx_t_8, __pyx_empty_unicode);<span class='error_goto'> if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 580, __pyx_L5_error)</span>
+      __pyx_t_7 = <span class='pyx_c_api'>__Pyx_PyObject_FormatSimple</span>(__pyx_t_8, __pyx_empty_unicode);<span class='error_goto'> if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 592, __pyx_L5_error)</span>
       <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_7);
       <span class='pyx_macro_api'>__Pyx_DECREF</span>(__pyx_t_8); __pyx_t_8 = 0;
       __pyx_t_6 = (<span class='pyx_c_api'>__Pyx_PyUnicode_MAX_CHAR_VALUE</span>(__pyx_t_7) &gt; __pyx_t_6) ? <span class='pyx_c_api'>__Pyx_PyUnicode_MAX_CHAR_VALUE</span>(__pyx_t_7) : __pyx_t_6;
       __pyx_t_5 += <span class='pyx_c_api'>__Pyx_PyUnicode_GET_LENGTH</span>(__pyx_t_7);
       <span class='refnanny'>__Pyx_GIVEREF</span>(__pyx_t_7);
       <span class='py_macro_api'>PyTuple_SET_ITEM</span>(__pyx_t_4, 3, __pyx_t_7);
       __pyx_t_7 = 0;
       <span class='pyx_macro_api'>__Pyx_INCREF</span>(__pyx_kp_u__5);
       __pyx_t_5 += 1;
       <span class='refnanny'>__Pyx_GIVEREF</span>(__pyx_kp_u__5);
       <span class='py_macro_api'>PyTuple_SET_ITEM</span>(__pyx_t_4, 4, __pyx_kp_u__5);
-      __pyx_t_7 = <span class='pyx_c_api'>__Pyx_PyUnicode_Join</span>(__pyx_t_4, 5, __pyx_t_5, __pyx_t_6);<span class='error_goto'> if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 580, __pyx_L5_error)</span>
+      __pyx_t_7 = <span class='pyx_c_api'>__Pyx_PyUnicode_Join</span>(__pyx_t_4, 5, __pyx_t_5, __pyx_t_6);<span class='error_goto'> if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 592, __pyx_L5_error)</span>
       <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_7);
       <span class='pyx_macro_api'>__Pyx_DECREF</span>(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(<span class='pyx_c_api'>__Pyx_ListComp_Append</span>(__pyx_t_1, (PyObject*)__pyx_t_7))) <span class='error_goto'>__PYX_ERR(0, 580, __pyx_L5_error)</span>
+      if (unlikely(<span class='pyx_c_api'>__Pyx_ListComp_Append</span>(__pyx_t_1, (PyObject*)__pyx_t_7))) <span class='error_goto'>__PYX_ERR(0, 592, __pyx_L5_error)</span>
       <span class='pyx_macro_api'>__Pyx_DECREF</span>(__pyx_t_7); __pyx_t_7 = 0;
     }
     <span class='pyx_macro_api'>__Pyx_DECREF</span>(__pyx_t_2); __pyx_t_2 = 0;
-    <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_8genexpr1__pyx_v_v); __pyx_8genexpr1__pyx_v_v = 0;
+    <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_8genexpr3__pyx_v_v); __pyx_8genexpr3__pyx_v_v = 0;
     goto __pyx_L8_exit_scope;
     __pyx_L5_error:;
-    <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_8genexpr1__pyx_v_v); __pyx_8genexpr1__pyx_v_v = 0;
+    <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_8genexpr3__pyx_v_v); __pyx_8genexpr3__pyx_v_v = 0;
     goto __pyx_L1_error;
     __pyx_L8_exit_scope:;
   } /* exit inner scope */
   __pyx_v_s = __pyx_t_1;
   __pyx_t_1 = 0;
-</pre><pre class="cython line score-6" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">581</span>:         <span class="n">s</span> <span class="o">=</span> <span class="s">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">s</span><span class="p">)</span></pre>
-<pre class='cython code score-6 '>  __pyx_t_1 = <span class='py_c_api'>PyUnicode_Join</span>(__pyx_kp_u__4, __pyx_v_s);<span class='error_goto'> if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 581, __pyx_L1_error)</span>
+</pre><pre class="cython line score-6" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">593</span>:         <span class="n">s</span> <span class="o">=</span> <span class="s">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">s</span><span class="p">)</span></pre>
+<pre class='cython code score-6 '>  __pyx_t_1 = <span class='py_c_api'>PyUnicode_Join</span>(__pyx_kp_u__4, __pyx_v_s);<span class='error_goto'> if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 593, __pyx_L1_error)</span>
   <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_1);
   <span class='pyx_macro_api'>__Pyx_DECREF_SET</span>(__pyx_v_s, __pyx_t_1);
   __pyx_t_1 = 0;
-</pre><pre class="cython line score-29" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">582</span>:         <span class="k">return</span> <span class="n">f</span><span class="s">&#39;PolyLine(vecs=[{s}], enclosed={self.enclosed})&#39;</span></pre>
+</pre><pre class="cython line score-29" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">594</span>:         <span class="k">return</span> <span class="n">f</span><span class="s">&#39;PolyLine(vecs=[{s}], enclosed={self.enclosed})&#39;</span></pre>
 <pre class='cython code score-29 '>  <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_r);
-  __pyx_t_1 = <span class='py_c_api'>PyTuple_New</span>(5);<span class='error_goto'> if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 582, __pyx_L1_error)</span>
+  __pyx_t_1 = <span class='py_c_api'>PyTuple_New</span>(5);<span class='error_goto'> if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 594, __pyx_L1_error)</span>
   <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_1);
   __pyx_t_3 = 0;
   __pyx_t_6 = 127;
   <span class='pyx_macro_api'>__Pyx_INCREF</span>(__pyx_kp_u_PolyLine_vecs);
   __pyx_t_3 += 15;
   <span class='refnanny'>__Pyx_GIVEREF</span>(__pyx_kp_u_PolyLine_vecs);
   <span class='py_macro_api'>PyTuple_SET_ITEM</span>(__pyx_t_1, 0, __pyx_kp_u_PolyLine_vecs);
-  __pyx_t_2 = <span class='pyx_c_api'>__Pyx_PyObject_FormatSimple</span>(__pyx_v_s, __pyx_empty_unicode);<span class='error_goto'> if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 582, __pyx_L1_error)</span>
+  __pyx_t_2 = <span class='pyx_c_api'>__Pyx_PyObject_FormatSimple</span>(__pyx_v_s, __pyx_empty_unicode);<span class='error_goto'> if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 594, __pyx_L1_error)</span>
   <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_2);
   __pyx_t_6 = (<span class='pyx_c_api'>__Pyx_PyUnicode_MAX_CHAR_VALUE</span>(__pyx_t_2) &gt; __pyx_t_6) ? <span class='pyx_c_api'>__Pyx_PyUnicode_MAX_CHAR_VALUE</span>(__pyx_t_2) : __pyx_t_6;
   __pyx_t_3 += <span class='pyx_c_api'>__Pyx_PyUnicode_GET_LENGTH</span>(__pyx_t_2);
   <span class='refnanny'>__Pyx_GIVEREF</span>(__pyx_t_2);
   <span class='py_macro_api'>PyTuple_SET_ITEM</span>(__pyx_t_1, 1, __pyx_t_2);
   __pyx_t_2 = 0;
   <span class='pyx_macro_api'>__Pyx_INCREF</span>(__pyx_kp_u_enclosed_2);
   __pyx_t_3 += 12;
   <span class='refnanny'>__Pyx_GIVEREF</span>(__pyx_kp_u_enclosed_2);
   <span class='py_macro_api'>PyTuple_SET_ITEM</span>(__pyx_t_1, 2, __pyx_kp_u_enclosed_2);
-  __pyx_t_2 = <span class='pyx_c_api'>__Pyx_PyUnicode_FromBInt_int</span>(__pyx_v_self-&gt;enclosed);<span class='error_goto'> if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 582, __pyx_L1_error)</span>
+  __pyx_t_2 = <span class='pyx_c_api'>__Pyx_PyUnicode_FromBInt_int</span>(__pyx_v_self-&gt;enclosed);<span class='error_goto'> if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 594, __pyx_L1_error)</span>
   <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_2);
   __pyx_t_3 += <span class='pyx_c_api'>__Pyx_PyUnicode_GET_LENGTH</span>(__pyx_t_2);
   <span class='refnanny'>__Pyx_GIVEREF</span>(__pyx_t_2);
   <span class='py_macro_api'>PyTuple_SET_ITEM</span>(__pyx_t_1, 3, __pyx_t_2);
   __pyx_t_2 = 0;
   <span class='pyx_macro_api'>__Pyx_INCREF</span>(__pyx_kp_u__5);
   __pyx_t_3 += 1;
   <span class='refnanny'>__Pyx_GIVEREF</span>(__pyx_kp_u__5);
   <span class='py_macro_api'>PyTuple_SET_ITEM</span>(__pyx_t_1, 4, __pyx_kp_u__5);
-  __pyx_t_2 = <span class='pyx_c_api'>__Pyx_PyUnicode_Join</span>(__pyx_t_1, 5, __pyx_t_3, __pyx_t_6);<span class='error_goto'> if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 582, __pyx_L1_error)</span>
+  __pyx_t_2 = <span class='pyx_c_api'>__Pyx_PyUnicode_Join</span>(__pyx_t_1, 5, __pyx_t_3, __pyx_t_6);<span class='error_goto'> if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 594, __pyx_L1_error)</span>
   <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_2);
   <span class='pyx_macro_api'>__Pyx_DECREF</span>(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
-</pre><pre class="cython line score-0">&#xA0;<span class="">583</span>: </pre>
-<pre class="cython line score-0">&#xA0;<span class="">584</span>:     <span class="nd">@cython</span><span class="o">.</span><span class="n">nonecheck</span><span class="p">(</span><span class="bp">False</span><span class="p">)</span></pre>
-<pre class="cython line score-0">&#xA0;<span class="">585</span>:     <span class="nd">@cython</span><span class="o">.</span><span class="n">boundscheck</span><span class="p">(</span><span class="bp">False</span><span class="p">)</span></pre>
-<pre class="cython line score-0">&#xA0;<span class="">586</span>:     <span class="nd">@cython</span><span class="o">.</span><span class="n">wraparound</span><span class="p">(</span><span class="bp">False</span><span class="p">)</span></pre>
-<pre class="cython line score-83" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">587</span>:     <span class="k">cpdef</span> <span class="kt">list</span> <span class="nf">intersect_general</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">Vec2</span> <span class="n">p1</span><span class="p">,</span> <span class="n">Vec2</span> <span class="n">p2</span><span class="p">,</span> <span class="n">real</span> <span class="n">f_low</span><span class="p">,</span> <span class="n">real</span> <span class="n">f_high</span><span class="p">,</span> <span class="n">bint</span> <span class="n">sortreduce</span><span class="o">=</span><span class="bp">True</span><span class="p">):</span></pre>
-<pre class='cython code score-83 '>static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_7intersect_general(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+</pre><pre class="cython line score-0">&#xA0;<span class="">595</span>: </pre>
+<pre class="cython line score-0">&#xA0;<span class="">596</span>:     <span class="nd">@cython</span><span class="o">.</span><span class="n">nonecheck</span><span class="p">(</span><span class="bp">False</span><span class="p">)</span></pre>
+<pre class="cython line score-0">&#xA0;<span class="">597</span>:     <span class="nd">@cython</span><span class="o">.</span><span class="n">boundscheck</span><span class="p">(</span><span class="bp">False</span><span class="p">)</span></pre>
+<pre class="cython line score-0">&#xA0;<span class="">598</span>:     <span class="nd">@cython</span><span class="o">.</span><span class="n">wraparound</span><span class="p">(</span><span class="bp">False</span><span class="p">)</span></pre>
+<pre class="cython line score-83" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">599</span>:     <span class="k">cpdef</span> <span class="kt">list</span> <span class="nf">intersect_general</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">Vec2</span> <span class="n">p1</span><span class="p">,</span> <span class="n">Vec2</span> <span class="n">p2</span><span class="p">,</span> <span class="n">real</span> <span class="n">f_low</span><span class="p">,</span> <span class="n">real</span> <span class="n">f_high</span><span class="p">,</span> <span class="n">bint</span> <span class="n">sortreduce</span><span class="o">=</span><span class="bp">True</span><span class="p">):</span></pre>
+<pre class='cython code score-83 '>static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_11intersect_general(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_f_7easyvec_8geometry_8PolyLine_intersect_general(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p2, __pyx_t_7easyvec_7vectors_real __pyx_v_f_low, __pyx_t_7easyvec_7vectors_real __pyx_v_f_high, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_opt_args_7easyvec_8geometry_8PolyLine_intersect_general *__pyx_optional_args) {
   int __pyx_v_sortreduce = ((int)1);
   PyObject *__pyx_v_res = 0;
   int __pyx_v_i;
   struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_v1 = 0;
   struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_v2 = 0;
   struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_v_cr = 0;
@@ -8356,17 +8607,17 @@
   <span class='pyx_macro_api'>__Pyx_XDECREF</span>((PyObject *)__pyx_v_v_cr);
   <span class='refnanny'>__Pyx_XGIVEREF</span>(__pyx_r);
   <span class='refnanny'>__Pyx_RefNannyFinishContext</span>();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_7intersect_general(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_7easyvec_8geometry_8PolyLine_6intersect_general[] = "PolyLine.intersect_general(self, Vec2 p1, Vec2 p2, real f_low, real f_high, bool sortreduce=True) -&gt; list";
-static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_7intersect_general(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_11intersect_general(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_7easyvec_8geometry_8PolyLine_10intersect_general[] = "PolyLine.intersect_general(self, Vec2 p1, Vec2 p2, real f_low, real f_high, bool sortreduce=True) -&gt; list";
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_11intersect_general(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p1 = 0;
   struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p2 = 0;
   __pyx_t_7easyvec_7vectors_real __pyx_v_f_low;
   __pyx_t_7easyvec_7vectors_real __pyx_v_f_high;
   int __pyx_v_sortreduce;
   PyObject *__pyx_r = 0;
   <span class='refnanny'>__Pyx_RefNannyDeclarations</span>
@@ -8396,37 +8647,37 @@
         case  0:
         if (likely((values[0] = <span class='pyx_c_api'>__Pyx_PyDict_GetItemStr</span>(__pyx_kwds, __pyx_n_s_p1)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = <span class='pyx_c_api'>__Pyx_PyDict_GetItemStr</span>(__pyx_kwds, __pyx_n_s_p2)) != 0)) kw_args--;
         else {
-          <span class='pyx_c_api'>__Pyx_RaiseArgtupleInvalid</span>("intersect_general", 0, 4, 5, 1); <span class='error_goto'>__PYX_ERR(0, 587, __pyx_L3_error)</span>
+          <span class='pyx_c_api'>__Pyx_RaiseArgtupleInvalid</span>("intersect_general", 0, 4, 5, 1); <span class='error_goto'>__PYX_ERR(0, 599, __pyx_L3_error)</span>
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = <span class='pyx_c_api'>__Pyx_PyDict_GetItemStr</span>(__pyx_kwds, __pyx_n_s_f_low)) != 0)) kw_args--;
         else {
-          <span class='pyx_c_api'>__Pyx_RaiseArgtupleInvalid</span>("intersect_general", 0, 4, 5, 2); <span class='error_goto'>__PYX_ERR(0, 587, __pyx_L3_error)</span>
+          <span class='pyx_c_api'>__Pyx_RaiseArgtupleInvalid</span>("intersect_general", 0, 4, 5, 2); <span class='error_goto'>__PYX_ERR(0, 599, __pyx_L3_error)</span>
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = <span class='pyx_c_api'>__Pyx_PyDict_GetItemStr</span>(__pyx_kwds, __pyx_n_s_f_high)) != 0)) kw_args--;
         else {
-          <span class='pyx_c_api'>__Pyx_RaiseArgtupleInvalid</span>("intersect_general", 0, 4, 5, 3); <span class='error_goto'>__PYX_ERR(0, 587, __pyx_L3_error)</span>
+          <span class='pyx_c_api'>__Pyx_RaiseArgtupleInvalid</span>("intersect_general", 0, 4, 5, 3); <span class='error_goto'>__PYX_ERR(0, 599, __pyx_L3_error)</span>
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (kw_args &gt; 0) {
           PyObject* value = <span class='pyx_c_api'>__Pyx_PyDict_GetItemStr</span>(__pyx_kwds, __pyx_n_s_sortreduce);
           if (value) { values[4] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args &gt; 0)) {
-        if (unlikely(<span class='pyx_c_api'>__Pyx_ParseOptionalKeywords</span>(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "intersect_general") &lt; 0)) <span class='error_goto'>__PYX_ERR(0, 587, __pyx_L3_error)</span>
+        if (unlikely(<span class='pyx_c_api'>__Pyx_ParseOptionalKeywords</span>(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "intersect_general") &lt; 0)) <span class='error_goto'>__PYX_ERR(0, 599, __pyx_L3_error)</span>
       }
     } else {
       switch (<span class='py_macro_api'>PyTuple_GET_SIZE</span>(__pyx_args)) {
         case  5: values[4] = <span class='py_macro_api'>PyTuple_GET_ITEM</span>(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
         case  4: values[3] = <span class='py_macro_api'>PyTuple_GET_ITEM</span>(__pyx_args, 3);
         values[2] = <span class='py_macro_api'>PyTuple_GET_ITEM</span>(__pyx_args, 2);
@@ -8434,51 +8685,51 @@
         values[0] = <span class='py_macro_api'>PyTuple_GET_ITEM</span>(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_p1 = ((struct __pyx_obj_7easyvec_7vectors_Vec2 *)values[0]);
     __pyx_v_p2 = ((struct __pyx_obj_7easyvec_7vectors_Vec2 *)values[1]);
-    __pyx_v_f_low = __pyx_<span class='py_c_api'>PyFloat_AsDouble</span>(values[2]); if (unlikely((__pyx_v_f_low == (double)-1) &amp;&amp; <span class='py_c_api'>PyErr_Occurred</span>())) <span class='error_goto'>__PYX_ERR(0, 587, __pyx_L3_error)</span>
-    __pyx_v_f_high = __pyx_<span class='py_c_api'>PyFloat_AsDouble</span>(values[3]); if (unlikely((__pyx_v_f_high == (double)-1) &amp;&amp; <span class='py_c_api'>PyErr_Occurred</span>())) <span class='error_goto'>__PYX_ERR(0, 587, __pyx_L3_error)</span>
+    __pyx_v_f_low = __pyx_<span class='py_c_api'>PyFloat_AsDouble</span>(values[2]); if (unlikely((__pyx_v_f_low == (double)-1) &amp;&amp; <span class='py_c_api'>PyErr_Occurred</span>())) <span class='error_goto'>__PYX_ERR(0, 599, __pyx_L3_error)</span>
+    __pyx_v_f_high = __pyx_<span class='py_c_api'>PyFloat_AsDouble</span>(values[3]); if (unlikely((__pyx_v_f_high == (double)-1) &amp;&amp; <span class='py_c_api'>PyErr_Occurred</span>())) <span class='error_goto'>__PYX_ERR(0, 599, __pyx_L3_error)</span>
     if (values[4]) {
-      __pyx_v_sortreduce = <span class='pyx_c_api'>__Pyx_PyObject_IsTrue</span>(values[4]); if (unlikely((__pyx_v_sortreduce == (int)-1) &amp;&amp; <span class='py_c_api'>PyErr_Occurred</span>())) <span class='error_goto'>__PYX_ERR(0, 587, __pyx_L3_error)</span>
+      __pyx_v_sortreduce = <span class='pyx_c_api'>__Pyx_PyObject_IsTrue</span>(values[4]); if (unlikely((__pyx_v_sortreduce == (int)-1) &amp;&amp; <span class='py_c_api'>PyErr_Occurred</span>())) <span class='error_goto'>__PYX_ERR(0, 599, __pyx_L3_error)</span>
     } else {
       __pyx_v_sortreduce = ((int)1);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  <span class='pyx_c_api'>__Pyx_RaiseArgtupleInvalid</span>("intersect_general", 0, 4, 5, <span class='py_macro_api'>PyTuple_GET_SIZE</span>(__pyx_args)); <span class='error_goto'>__PYX_ERR(0, 587, __pyx_L3_error)</span>
+  <span class='pyx_c_api'>__Pyx_RaiseArgtupleInvalid</span>("intersect_general", 0, 4, 5, <span class='py_macro_api'>PyTuple_GET_SIZE</span>(__pyx_args)); <span class='error_goto'>__PYX_ERR(0, 599, __pyx_L3_error)</span>
   __pyx_L3_error:;
   <span class='pyx_c_api'>__Pyx_AddTraceback</span>("easyvec.geometry.PolyLine.intersect_general", __pyx_clineno, __pyx_lineno, __pyx_filename);
   <span class='refnanny'>__Pyx_RefNannyFinishContext</span>();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!<span class='pyx_c_api'>__Pyx_ArgTypeTest</span>(((PyObject *)__pyx_v_p1), __pyx_ptype_7easyvec_7vectors_Vec2, 1, "p1", 0))) <span class='error_goto'>__PYX_ERR(0, 587, __pyx_L1_error)</span>
-  if (unlikely(!<span class='pyx_c_api'>__Pyx_ArgTypeTest</span>(((PyObject *)__pyx_v_p2), __pyx_ptype_7easyvec_7vectors_Vec2, 1, "p2", 0))) <span class='error_goto'>__PYX_ERR(0, 587, __pyx_L1_error)</span>
-  __pyx_r = __pyx_pf_7easyvec_8geometry_8PolyLine_6intersect_general(((struct __pyx_obj_7easyvec_8geometry_PolyLine *)__pyx_v_self), __pyx_v_p1, __pyx_v_p2, __pyx_v_f_low, __pyx_v_f_high, __pyx_v_sortreduce);
+  if (unlikely(!<span class='pyx_c_api'>__Pyx_ArgTypeTest</span>(((PyObject *)__pyx_v_p1), __pyx_ptype_7easyvec_7vectors_Vec2, 1, "p1", 0))) <span class='error_goto'>__PYX_ERR(0, 599, __pyx_L1_error)</span>
+  if (unlikely(!<span class='pyx_c_api'>__Pyx_ArgTypeTest</span>(((PyObject *)__pyx_v_p2), __pyx_ptype_7easyvec_7vectors_Vec2, 1, "p2", 0))) <span class='error_goto'>__PYX_ERR(0, 599, __pyx_L1_error)</span>
+  __pyx_r = __pyx_pf_7easyvec_8geometry_8PolyLine_10intersect_general(((struct __pyx_obj_7easyvec_8geometry_PolyLine *)__pyx_v_self), __pyx_v_p1, __pyx_v_p2, __pyx_v_f_low, __pyx_v_f_high, __pyx_v_sortreduce);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   <span class='refnanny'>__Pyx_RefNannyFinishContext</span>();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_6intersect_general(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p2, __pyx_t_7easyvec_7vectors_real __pyx_v_f_low, __pyx_t_7easyvec_7vectors_real __pyx_v_f_high, int __pyx_v_sortreduce) {
+static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_10intersect_general(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p2, __pyx_t_7easyvec_7vectors_real __pyx_v_f_low, __pyx_t_7easyvec_7vectors_real __pyx_v_f_high, int __pyx_v_sortreduce) {
   PyObject *__pyx_r = NULL;
   <span class='refnanny'>__Pyx_RefNannyDeclarations</span>
   <span class='refnanny'>__Pyx_RefNannySetupContext</span>("intersect_general", 0);
   <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_r);
   __pyx_t_2.__pyx_n = 1;
   __pyx_t_2.sortreduce = __pyx_v_sortreduce;
-  __pyx_t_1 = __pyx_vtabptr_7easyvec_8geometry_PolyLine-&gt;intersect_general(__pyx_v_self, __pyx_v_p1, __pyx_v_p2, __pyx_v_f_low, __pyx_v_f_high, 1, &amp;__pyx_t_2);<span class='error_goto'> if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 587, __pyx_L1_error)</span>
+  __pyx_t_1 = __pyx_vtabptr_7easyvec_8geometry_PolyLine-&gt;intersect_general(__pyx_v_self, __pyx_v_p1, __pyx_v_p2, __pyx_v_f_low, __pyx_v_f_high, 1, &amp;__pyx_t_2);<span class='error_goto'> if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 599, __pyx_L1_error)</span>
   <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -8486,69 +8737,69 @@
   <span class='pyx_c_api'>__Pyx_AddTraceback</span>("easyvec.geometry.PolyLine.intersect_general", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   <span class='refnanny'>__Pyx_XGIVEREF</span>(__pyx_r);
   <span class='refnanny'>__Pyx_RefNannyFinishContext</span>();
   return __pyx_r;
 }
-</pre><pre class="cython line score-5" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">588</span>:         <span class="k">cdef</span> <span class="kt">list</span> <span class="nf">res</span> <span class="o">=</span> <span class="p">[]</span></pre>
-<pre class='cython code score-5 '>  __pyx_t_1 = <span class='py_c_api'>PyList_New</span>(0);<span class='error_goto'> if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 588, __pyx_L1_error)</span>
+</pre><pre class="cython line score-5" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">600</span>:         <span class="k">cdef</span> <span class="kt">list</span> <span class="nf">res</span> <span class="o">=</span> <span class="p">[]</span></pre>
+<pre class='cython code score-5 '>  __pyx_t_1 = <span class='py_c_api'>PyList_New</span>(0);<span class='error_goto'> if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 600, __pyx_L1_error)</span>
   <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_1);
   __pyx_v_res = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
-</pre><pre class="cython line score-1" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">589</span>:         <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">bbox</span><span class="o">.</span><span class="n">intersect_general</span><span class="p">(</span><span class="n">p1</span><span class="p">,</span> <span class="n">p2</span><span class="p">,</span> <span class="n">f_low</span><span class="p">,</span> <span class="n">f_high</span><span class="p">)</span> <span class="ow">is</span> <span class="bp">None</span><span class="p">:</span></pre>
-<pre class='cython code score-1 '>  __pyx_t_1 = ((PyObject *)__pyx_f_7easyvec_8geometry_4Rect_intersect_general(__pyx_v_self-&gt;bbox, __pyx_v_p1, __pyx_v_p2, __pyx_v_f_low, __pyx_v_f_high, 0, NULL));<span class='error_goto'> if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 589, __pyx_L1_error)</span>
+</pre><pre class="cython line score-1" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">601</span>:         <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">bbox</span><span class="o">.</span><span class="n">intersect_general</span><span class="p">(</span><span class="n">p1</span><span class="p">,</span> <span class="n">p2</span><span class="p">,</span> <span class="n">f_low</span><span class="p">,</span> <span class="n">f_high</span><span class="p">)</span> <span class="ow">is</span> <span class="bp">None</span><span class="p">:</span></pre>
+<pre class='cython code score-1 '>  __pyx_t_1 = ((PyObject *)__pyx_f_7easyvec_8geometry_4Rect_intersect_general(__pyx_v_self-&gt;bbox, __pyx_v_p1, __pyx_v_p2, __pyx_v_f_low, __pyx_v_f_high, 0, NULL));<span class='error_goto'> if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 601, __pyx_L1_error)</span>
   <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_1);
   __pyx_t_2 = (__pyx_t_1 == Py_None);
   <span class='pyx_macro_api'>__Pyx_DECREF</span>(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 /* … */
   }
-</pre><pre class="cython line score-2" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">590</span>:             <span class="k">return</span> <span class="n">res</span></pre>
+</pre><pre class="cython line score-2" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">602</span>:             <span class="k">return</span> <span class="n">res</span></pre>
 <pre class='cython code score-2 '>    <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_r);
     <span class='pyx_macro_api'>__Pyx_INCREF</span>(__pyx_v_res);
     __pyx_r = __pyx_v_res;
     goto __pyx_L0;
-</pre><pre class="cython line score-0">&#xA0;<span class="">591</span>:         <span class="k">cdef</span> <span class="kt">int</span> <span class="nf">i</span></pre>
-<pre class="cython line score-0">&#xA0;<span class="">592</span>:         <span class="k">cdef</span> <span class="kt">Vec2</span> <span class="nf">v1</span><span class="p">,</span> <span class="nf">v2</span><span class="p">,</span> <span class="nf">v_cr</span></pre>
-<pre class="cython line score-0">&#xA0;<span class="">593</span>:         <span class="k">cdef</span> <span class="kt">bint</span> <span class="nf">inter</span></pre>
-<pre class="cython line score-0">&#xA0;<span class="">594</span>:         <span class="k">cdef</span> <span class="kt">real</span> <span class="nf">t1</span><span class="p">,</span> <span class="nf">t2</span></pre>
-<pre class="cython line score-7" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">595</span>:         <span class="n">v1</span> <span class="o">=</span> <span class="p">&lt;</span><span class="kt">Vec2</span><span class="p">&gt;(</span><span class="bp">self</span><span class="o">.</span><span class="n">vecs</span><span class="p">[</span><span class="mf">0</span><span class="p">])</span></pre>
+</pre><pre class="cython line score-0">&#xA0;<span class="">603</span>:         <span class="k">cdef</span> <span class="kt">int</span> <span class="nf">i</span></pre>
+<pre class="cython line score-0">&#xA0;<span class="">604</span>:         <span class="k">cdef</span> <span class="kt">Vec2</span> <span class="nf">v1</span><span class="p">,</span> <span class="nf">v2</span><span class="p">,</span> <span class="nf">v_cr</span></pre>
+<pre class="cython line score-0">&#xA0;<span class="">605</span>:         <span class="k">cdef</span> <span class="kt">bint</span> <span class="nf">inter</span></pre>
+<pre class="cython line score-0">&#xA0;<span class="">606</span>:         <span class="k">cdef</span> <span class="kt">real</span> <span class="nf">t1</span><span class="p">,</span> <span class="nf">t2</span></pre>
+<pre class="cython line score-7" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">607</span>:         <span class="n">v1</span> <span class="o">=</span> <span class="p">&lt;</span><span class="kt">Vec2</span><span class="p">&gt;(</span><span class="bp">self</span><span class="o">.</span><span class="n">vecs</span><span class="p">[</span><span class="mf">0</span><span class="p">])</span></pre>
 <pre class='cython code score-7 '>  if (unlikely(__pyx_v_self-&gt;vecs == Py_None)) {
     <span class='py_c_api'>PyErr_SetString</span>(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    <span class='error_goto'>__PYX_ERR(0, 595, __pyx_L1_error)</span>
+    <span class='error_goto'>__PYX_ERR(0, 607, __pyx_L1_error)</span>
   }
   __pyx_t_1 = <span class='py_macro_api'>PyList_GET_ITEM</span>(__pyx_v_self-&gt;vecs, 0);
   <span class='pyx_macro_api'>__Pyx_INCREF</span>(__pyx_t_1);
   __pyx_v_v1 = ((struct __pyx_obj_7easyvec_7vectors_Vec2 *)__pyx_t_1);
   __pyx_t_1 = 0;
-</pre><pre class="cython line score-0" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">596</span>:         <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mf">1</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">vlen</span><span class="p">):</span></pre>
+</pre><pre class="cython line score-0" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">608</span>:         <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mf">1</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">vlen</span><span class="p">):</span></pre>
 <pre class='cython code score-0 '>  __pyx_t_4 = __pyx_v_self-&gt;vlen;
   __pyx_t_5 = __pyx_t_4;
   for (__pyx_t_6 = 1; __pyx_t_6 &lt; __pyx_t_5; __pyx_t_6+=1) {
     __pyx_v_i = __pyx_t_6;
-</pre><pre class="cython line score-8" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">597</span>:             <span class="n">v2</span> <span class="o">=</span> <span class="p">&lt;</span><span class="kt">Vec2</span><span class="p">&gt;(</span><span class="bp">self</span><span class="o">.</span><span class="n">vecs</span><span class="p">[</span><span class="n">i</span><span class="p">])</span></pre>
+</pre><pre class="cython line score-8" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">609</span>:             <span class="n">v2</span> <span class="o">=</span> <span class="p">&lt;</span><span class="kt">Vec2</span><span class="p">&gt;(</span><span class="bp">self</span><span class="o">.</span><span class="n">vecs</span><span class="p">[</span><span class="n">i</span><span class="p">])</span></pre>
 <pre class='cython code score-8 '>    if (unlikely(__pyx_v_self-&gt;vecs == Py_None)) {
       <span class='py_c_api'>PyErr_SetString</span>(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      <span class='error_goto'>__PYX_ERR(0, 597, __pyx_L1_error)</span>
+      <span class='error_goto'>__PYX_ERR(0, 609, __pyx_L1_error)</span>
     }
     __pyx_t_1 = <span class='py_macro_api'>PyList_GET_ITEM</span>(__pyx_v_self-&gt;vecs, __pyx_v_i);
     <span class='pyx_macro_api'>__Pyx_INCREF</span>(__pyx_t_1);
     <span class='pyx_macro_api'>__Pyx_XDECREF_SET</span>(__pyx_v_v2, ((struct __pyx_obj_7easyvec_7vectors_Vec2 *)__pyx_t_1));
     __pyx_t_1 = 0;
-</pre><pre class="cython line score-0" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">598</span>:             <span class="n">inter</span><span class="p">,</span> <span class="n">t1</span><span class="p">,</span> <span class="n">t2</span> <span class="o">=</span> <span class="n">_intersect_ts</span><span class="p">(</span><span class="n">p1</span><span class="p">,</span> <span class="n">p2</span><span class="p">,</span> <span class="n">v1</span><span class="p">,</span> <span class="n">v2</span><span class="p">)</span></pre>
+</pre><pre class="cython line score-0" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">610</span>:             <span class="n">inter</span><span class="p">,</span> <span class="n">t1</span><span class="p">,</span> <span class="n">t2</span> <span class="o">=</span> <span class="n">_intersect_ts</span><span class="p">(</span><span class="n">p1</span><span class="p">,</span> <span class="n">p2</span><span class="p">,</span> <span class="n">v1</span><span class="p">,</span> <span class="n">v2</span><span class="p">)</span></pre>
 <pre class='cython code score-0 '>    __pyx_t_7 = __pyx_f_7easyvec_8geometry__intersect_ts(__pyx_v_p1, __pyx_v_p2, __pyx_v_v1, __pyx_v_v2, 0);
     __pyx_t_3 = __pyx_t_7.f0;
     __pyx_t_8 = __pyx_t_7.f1;
     __pyx_t_9 = __pyx_t_7.f2;
     __pyx_v_inter = __pyx_t_3;
     __pyx_v_t1 = __pyx_t_8;
     __pyx_v_t2 = __pyx_t_9;
-</pre><pre class="cython line score-0" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">599</span>:             <span class="k">if</span> <span class="n">inter</span> <span class="ow">and</span> <span class="p">(</span><span class="mf">0.0</span> <span class="o">&lt;=</span> <span class="n">t2</span> <span class="o">&lt;=</span> <span class="mf">1.0</span><span class="p">)</span> <span class="ow">and</span> <span class="p">(</span><span class="n">f_low</span> <span class="o">&lt;=</span> <span class="n">t1</span> <span class="o">&lt;=</span> <span class="n">f_high</span><span class="p">):</span></pre>
+</pre><pre class="cython line score-0" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">611</span>:             <span class="k">if</span> <span class="n">inter</span> <span class="ow">and</span> <span class="p">(</span><span class="mf">0.0</span> <span class="o">&lt;=</span> <span class="n">t2</span> <span class="o">&lt;=</span> <span class="mf">1.0</span><span class="p">)</span> <span class="ow">and</span> <span class="p">(</span><span class="n">f_low</span> <span class="o">&lt;=</span> <span class="n">t1</span> <span class="o">&lt;=</span> <span class="n">f_high</span><span class="p">):</span></pre>
 <pre class='cython code score-0 '>    __pyx_t_2 = (__pyx_v_inter != 0);
     if (__pyx_t_2) {
     } else {
       __pyx_t_3 = __pyx_t_2;
       goto __pyx_L7_bool_binop_done;
     }
     __pyx_t_2 = (0.0 &lt;= __pyx_v_t2);
@@ -8567,54 +8818,54 @@
     }
     __pyx_t_2 = (__pyx_t_10 != 0);
     __pyx_t_3 = __pyx_t_2;
     __pyx_L7_bool_binop_done:;
     if (__pyx_t_3) {
 /* … */
     }
-</pre><pre class="cython line score-3" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">600</span>:                 <span class="n">v_cr</span> <span class="o">=</span> <span class="n">p1</span><span class="o">.</span><span class="n">add</span><span class="p">(</span> <span class="n">p2</span><span class="o">.</span><span class="n">sub</span><span class="p">(</span><span class="n">p1</span><span class="p">)</span><span class="o">.</span><span class="n">mul_num</span><span class="p">(</span><span class="n">t1</span><span class="p">)</span> <span class="p">)</span></pre>
-<pre class='cython code score-3 '>      __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_7easyvec_7vectors_Vec2 *)__pyx_v_p2-&gt;__pyx_vtab)-&gt;sub(__pyx_v_p2, __pyx_v_p1, 0));<span class='error_goto'> if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 600, __pyx_L1_error)</span>
+</pre><pre class="cython line score-3" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">612</span>:                 <span class="n">v_cr</span> <span class="o">=</span> <span class="n">p1</span><span class="o">.</span><span class="n">add</span><span class="p">(</span> <span class="n">p2</span><span class="o">.</span><span class="n">sub</span><span class="p">(</span><span class="n">p1</span><span class="p">)</span><span class="o">.</span><span class="n">mul_num</span><span class="p">(</span><span class="n">t1</span><span class="p">)</span> <span class="p">)</span></pre>
+<pre class='cython code score-3 '>      __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_7easyvec_7vectors_Vec2 *)__pyx_v_p2-&gt;__pyx_vtab)-&gt;sub(__pyx_v_p2, __pyx_v_p1, 0));<span class='error_goto'> if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 612, __pyx_L1_error)</span>
       <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_1);
-      __pyx_t_11 = ((PyObject *)((struct __pyx_vtabstruct_7easyvec_7vectors_Vec2 *)((struct __pyx_obj_7easyvec_7vectors_Vec2 *)__pyx_t_1)-&gt;__pyx_vtab)-&gt;mul_num(((struct __pyx_obj_7easyvec_7vectors_Vec2 *)__pyx_t_1), __pyx_v_t1, 0));<span class='error_goto'> if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 600, __pyx_L1_error)</span>
+      __pyx_t_11 = ((PyObject *)((struct __pyx_vtabstruct_7easyvec_7vectors_Vec2 *)((struct __pyx_obj_7easyvec_7vectors_Vec2 *)__pyx_t_1)-&gt;__pyx_vtab)-&gt;mul_num(((struct __pyx_obj_7easyvec_7vectors_Vec2 *)__pyx_t_1), __pyx_v_t1, 0));<span class='error_goto'> if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 612, __pyx_L1_error)</span>
       <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_11);
       <span class='pyx_macro_api'>__Pyx_DECREF</span>(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_7easyvec_7vectors_Vec2 *)__pyx_v_p1-&gt;__pyx_vtab)-&gt;add(__pyx_v_p1, ((struct __pyx_obj_7easyvec_7vectors_Vec2 *)__pyx_t_11), 0));<span class='error_goto'> if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 600, __pyx_L1_error)</span>
+      __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_7easyvec_7vectors_Vec2 *)__pyx_v_p1-&gt;__pyx_vtab)-&gt;add(__pyx_v_p1, ((struct __pyx_obj_7easyvec_7vectors_Vec2 *)__pyx_t_11), 0));<span class='error_goto'> if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 612, __pyx_L1_error)</span>
       <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_1);
       <span class='pyx_macro_api'>__Pyx_DECREF</span>(__pyx_t_11); __pyx_t_11 = 0;
       <span class='pyx_macro_api'>__Pyx_XDECREF_SET</span>(__pyx_v_v_cr, ((struct __pyx_obj_7easyvec_7vectors_Vec2 *)__pyx_t_1));
       __pyx_t_1 = 0;
-</pre><pre class="cython line score-2" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">601</span>:                 <span class="n">res</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">v_cr</span><span class="p">)</span></pre>
-<pre class='cython code score-2 '>      __pyx_t_12 = <span class='pyx_c_api'>__Pyx_PyList_Append</span>(__pyx_v_res, ((PyObject *)__pyx_v_v_cr));<span class='error_goto'> if (unlikely(__pyx_t_12 == ((int)-1))) __PYX_ERR(0, 601, __pyx_L1_error)</span>
-</pre><pre class="cython line score-2" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">602</span>:             <span class="n">v1</span> <span class="o">=</span> <span class="n">v2</span></pre>
+</pre><pre class="cython line score-2" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">613</span>:                 <span class="n">res</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">v_cr</span><span class="p">)</span></pre>
+<pre class='cython code score-2 '>      __pyx_t_12 = <span class='pyx_c_api'>__Pyx_PyList_Append</span>(__pyx_v_res, ((PyObject *)__pyx_v_v_cr));<span class='error_goto'> if (unlikely(__pyx_t_12 == ((int)-1))) __PYX_ERR(0, 613, __pyx_L1_error)</span>
+</pre><pre class="cython line score-2" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">614</span>:             <span class="n">v1</span> <span class="o">=</span> <span class="n">v2</span></pre>
 <pre class='cython code score-2 '>    <span class='pyx_macro_api'>__Pyx_INCREF</span>(((PyObject *)__pyx_v_v2));
     <span class='pyx_macro_api'>__Pyx_DECREF_SET</span>(__pyx_v_v1, __pyx_v_v2);
   }
-</pre><pre class="cython line score-0" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">603</span>:         <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">enclosed</span><span class="p">:</span></pre>
+</pre><pre class="cython line score-0" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">615</span>:         <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">enclosed</span><span class="p">:</span></pre>
 <pre class='cython code score-0 '>  __pyx_t_3 = (__pyx_v_self-&gt;enclosed != 0);
   if (__pyx_t_3) {
 /* … */
   }
-</pre><pre class="cython line score-8" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">604</span>:             <span class="n">v2</span> <span class="o">=</span> <span class="p">&lt;</span><span class="kt">Vec2</span><span class="p">&gt;(</span><span class="bp">self</span><span class="o">.</span><span class="n">vecs</span><span class="p">[</span><span class="mf">0</span><span class="p">])</span></pre>
+</pre><pre class="cython line score-8" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">616</span>:             <span class="n">v2</span> <span class="o">=</span> <span class="p">&lt;</span><span class="kt">Vec2</span><span class="p">&gt;(</span><span class="bp">self</span><span class="o">.</span><span class="n">vecs</span><span class="p">[</span><span class="mf">0</span><span class="p">])</span></pre>
 <pre class='cython code score-8 '>    if (unlikely(__pyx_v_self-&gt;vecs == Py_None)) {
       <span class='py_c_api'>PyErr_SetString</span>(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      <span class='error_goto'>__PYX_ERR(0, 604, __pyx_L1_error)</span>
+      <span class='error_goto'>__PYX_ERR(0, 616, __pyx_L1_error)</span>
     }
     __pyx_t_1 = <span class='py_macro_api'>PyList_GET_ITEM</span>(__pyx_v_self-&gt;vecs, 0);
     <span class='pyx_macro_api'>__Pyx_INCREF</span>(__pyx_t_1);
     <span class='pyx_macro_api'>__Pyx_XDECREF_SET</span>(__pyx_v_v2, ((struct __pyx_obj_7easyvec_7vectors_Vec2 *)__pyx_t_1));
     __pyx_t_1 = 0;
-</pre><pre class="cython line score-0" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">605</span>:             <span class="n">inter</span><span class="p">,</span> <span class="n">t1</span><span class="p">,</span> <span class="n">t2</span> <span class="o">=</span> <span class="n">_intersect_ts</span><span class="p">(</span><span class="n">p1</span><span class="p">,</span> <span class="n">p2</span><span class="p">,</span> <span class="n">v1</span><span class="p">,</span> <span class="n">v2</span><span class="p">)</span></pre>
+</pre><pre class="cython line score-0" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">617</span>:             <span class="n">inter</span><span class="p">,</span> <span class="n">t1</span><span class="p">,</span> <span class="n">t2</span> <span class="o">=</span> <span class="n">_intersect_ts</span><span class="p">(</span><span class="n">p1</span><span class="p">,</span> <span class="n">p2</span><span class="p">,</span> <span class="n">v1</span><span class="p">,</span> <span class="n">v2</span><span class="p">)</span></pre>
 <pre class='cython code score-0 '>    __pyx_t_7 = __pyx_f_7easyvec_8geometry__intersect_ts(__pyx_v_p1, __pyx_v_p2, __pyx_v_v1, __pyx_v_v2, 0);
     __pyx_t_3 = __pyx_t_7.f0;
     __pyx_t_9 = __pyx_t_7.f1;
     __pyx_t_8 = __pyx_t_7.f2;
     __pyx_v_inter = __pyx_t_3;
     __pyx_v_t1 = __pyx_t_9;
     __pyx_v_t2 = __pyx_t_8;
-</pre><pre class="cython line score-0" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">606</span>:             <span class="k">if</span> <span class="n">inter</span> <span class="ow">and</span> <span class="p">(</span><span class="mf">0.0</span> <span class="o">&lt;=</span> <span class="n">t2</span> <span class="o">&lt;=</span> <span class="mf">1.0</span><span class="p">)</span> <span class="ow">and</span> <span class="p">(</span><span class="n">f_low</span> <span class="o">&lt;=</span> <span class="n">t1</span> <span class="o">&lt;=</span> <span class="n">f_high</span><span class="p">):</span></pre>
+</pre><pre class="cython line score-0" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">618</span>:             <span class="k">if</span> <span class="n">inter</span> <span class="ow">and</span> <span class="p">(</span><span class="mf">0.0</span> <span class="o">&lt;=</span> <span class="n">t2</span> <span class="o">&lt;=</span> <span class="mf">1.0</span><span class="p">)</span> <span class="ow">and</span> <span class="p">(</span><span class="n">f_low</span> <span class="o">&lt;=</span> <span class="n">t1</span> <span class="o">&lt;=</span> <span class="n">f_high</span><span class="p">):</span></pre>
 <pre class='cython code score-0 '>    __pyx_t_2 = (__pyx_v_inter != 0);
     if (__pyx_t_2) {
     } else {
       __pyx_t_3 = __pyx_t_2;
       goto __pyx_L12_bool_binop_done;
     }
     __pyx_t_2 = (0.0 &lt;= __pyx_v_t2);
@@ -8633,48 +8884,48 @@
     }
     __pyx_t_2 = (__pyx_t_10 != 0);
     __pyx_t_3 = __pyx_t_2;
     __pyx_L12_bool_binop_done:;
     if (__pyx_t_3) {
 /* … */
     }
-</pre><pre class="cython line score-3" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">607</span>:                 <span class="n">v_cr</span> <span class="o">=</span> <span class="n">p1</span><span class="o">.</span><span class="n">add</span><span class="p">(</span> <span class="n">p2</span><span class="o">.</span><span class="n">sub</span><span class="p">(</span><span class="n">p1</span><span class="p">)</span><span class="o">.</span><span class="n">mul_num</span><span class="p">(</span><span class="n">t1</span><span class="p">)</span> <span class="p">)</span></pre>
-<pre class='cython code score-3 '>      __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_7easyvec_7vectors_Vec2 *)__pyx_v_p2-&gt;__pyx_vtab)-&gt;sub(__pyx_v_p2, __pyx_v_p1, 0));<span class='error_goto'> if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 607, __pyx_L1_error)</span>
+</pre><pre class="cython line score-3" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">619</span>:                 <span class="n">v_cr</span> <span class="o">=</span> <span class="n">p1</span><span class="o">.</span><span class="n">add</span><span class="p">(</span> <span class="n">p2</span><span class="o">.</span><span class="n">sub</span><span class="p">(</span><span class="n">p1</span><span class="p">)</span><span class="o">.</span><span class="n">mul_num</span><span class="p">(</span><span class="n">t1</span><span class="p">)</span> <span class="p">)</span></pre>
+<pre class='cython code score-3 '>      __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_7easyvec_7vectors_Vec2 *)__pyx_v_p2-&gt;__pyx_vtab)-&gt;sub(__pyx_v_p2, __pyx_v_p1, 0));<span class='error_goto'> if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 619, __pyx_L1_error)</span>
       <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_1);
-      __pyx_t_11 = ((PyObject *)((struct __pyx_vtabstruct_7easyvec_7vectors_Vec2 *)((struct __pyx_obj_7easyvec_7vectors_Vec2 *)__pyx_t_1)-&gt;__pyx_vtab)-&gt;mul_num(((struct __pyx_obj_7easyvec_7vectors_Vec2 *)__pyx_t_1), __pyx_v_t1, 0));<span class='error_goto'> if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 607, __pyx_L1_error)</span>
+      __pyx_t_11 = ((PyObject *)((struct __pyx_vtabstruct_7easyvec_7vectors_Vec2 *)((struct __pyx_obj_7easyvec_7vectors_Vec2 *)__pyx_t_1)-&gt;__pyx_vtab)-&gt;mul_num(((struct __pyx_obj_7easyvec_7vectors_Vec2 *)__pyx_t_1), __pyx_v_t1, 0));<span class='error_goto'> if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 619, __pyx_L1_error)</span>
       <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_11);
       <span class='pyx_macro_api'>__Pyx_DECREF</span>(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_7easyvec_7vectors_Vec2 *)__pyx_v_p1-&gt;__pyx_vtab)-&gt;add(__pyx_v_p1, ((struct __pyx_obj_7easyvec_7vectors_Vec2 *)__pyx_t_11), 0));<span class='error_goto'> if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 607, __pyx_L1_error)</span>
+      __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_7easyvec_7vectors_Vec2 *)__pyx_v_p1-&gt;__pyx_vtab)-&gt;add(__pyx_v_p1, ((struct __pyx_obj_7easyvec_7vectors_Vec2 *)__pyx_t_11), 0));<span class='error_goto'> if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 619, __pyx_L1_error)</span>
       <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_1);
       <span class='pyx_macro_api'>__Pyx_DECREF</span>(__pyx_t_11); __pyx_t_11 = 0;
       <span class='pyx_macro_api'>__Pyx_XDECREF_SET</span>(__pyx_v_v_cr, ((struct __pyx_obj_7easyvec_7vectors_Vec2 *)__pyx_t_1));
       __pyx_t_1 = 0;
-</pre><pre class="cython line score-2" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">608</span>:                 <span class="n">res</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">v_cr</span><span class="p">)</span></pre>
-<pre class='cython code score-2 '>      __pyx_t_12 = <span class='pyx_c_api'>__Pyx_PyList_Append</span>(__pyx_v_res, ((PyObject *)__pyx_v_v_cr));<span class='error_goto'> if (unlikely(__pyx_t_12 == ((int)-1))) __PYX_ERR(0, 608, __pyx_L1_error)</span>
-</pre><pre class="cython line score-0" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">609</span>:         <span class="k">if</span> <span class="n">sortreduce</span><span class="p">:</span></pre>
+</pre><pre class="cython line score-2" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">620</span>:                 <span class="n">res</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">v_cr</span><span class="p">)</span></pre>
+<pre class='cython code score-2 '>      __pyx_t_12 = <span class='pyx_c_api'>__Pyx_PyList_Append</span>(__pyx_v_res, ((PyObject *)__pyx_v_v_cr));<span class='error_goto'> if (unlikely(__pyx_t_12 == ((int)-1))) __PYX_ERR(0, 620, __pyx_L1_error)</span>
+</pre><pre class="cython line score-0" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">621</span>:         <span class="k">if</span> <span class="n">sortreduce</span><span class="p">:</span></pre>
 <pre class='cython code score-0 '>  __pyx_t_3 = (__pyx_v_sortreduce != 0);
   if (__pyx_t_3) {
 /* … */
   }
-</pre><pre class="cython line score-1" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">610</span>:             <span class="k">return</span> <span class="n">_sortreduce_by_distance</span><span class="p">(</span><span class="n">res</span><span class="p">,</span> <span class="n">p1</span><span class="p">)</span></pre>
+</pre><pre class="cython line score-1" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">622</span>:             <span class="k">return</span> <span class="n">_sortreduce_by_distance</span><span class="p">(</span><span class="n">res</span><span class="p">,</span> <span class="n">p1</span><span class="p">)</span></pre>
 <pre class='cython code score-1 '>    <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_r);
-    __pyx_t_1 = __pyx_f_7easyvec_8geometry__sortreduce_by_distance(__pyx_v_res, __pyx_v_p1, 0);<span class='error_goto'> if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 610, __pyx_L1_error)</span>
+    __pyx_t_1 = __pyx_f_7easyvec_8geometry__sortreduce_by_distance(__pyx_v_res, __pyx_v_p1, 0);<span class='error_goto'> if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 622, __pyx_L1_error)</span>
     <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_1);
     __pyx_r = ((PyObject*)__pyx_t_1);
     __pyx_t_1 = 0;
     goto __pyx_L0;
-</pre><pre class="cython line score-2" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">611</span>:         <span class="k">return</span> <span class="n">res</span></pre>
+</pre><pre class="cython line score-2" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">623</span>:         <span class="k">return</span> <span class="n">res</span></pre>
 <pre class='cython code score-2 '>  <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_r);
   <span class='pyx_macro_api'>__Pyx_INCREF</span>(__pyx_v_res);
   __pyx_r = __pyx_v_res;
   goto __pyx_L0;
-</pre><pre class="cython line score-0">&#xA0;<span class="">612</span>: </pre>
-<pre class="cython line score-0">&#xA0;<span class="">613</span>:     <span class="nd">@cython</span><span class="o">.</span><span class="n">nonecheck</span><span class="p">(</span><span class="bp">False</span><span class="p">)</span></pre>
-<pre class="cython line score-46" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">614</span>:     <span class="k">cpdef</span> <span class="kt">list</span> <span class="nf">intersect_line</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">Vec2</span> <span class="n">p1</span><span class="p">,</span> <span class="n">Vec2</span> <span class="n">p2</span><span class="p">,</span> <span class="n">bint</span> <span class="n">sortreduce</span><span class="o">=</span><span class="bp">True</span><span class="p">):</span></pre>
-<pre class='cython code score-46 '>static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_9intersect_line(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+</pre><pre class="cython line score-0">&#xA0;<span class="">624</span>: </pre>
+<pre class="cython line score-0">&#xA0;<span class="">625</span>:     <span class="nd">@cython</span><span class="o">.</span><span class="n">nonecheck</span><span class="p">(</span><span class="bp">False</span><span class="p">)</span></pre>
+<pre class="cython line score-46" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">626</span>:     <span class="k">cpdef</span> <span class="kt">list</span> <span class="nf">intersect_line</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">Vec2</span> <span class="n">p1</span><span class="p">,</span> <span class="n">Vec2</span> <span class="n">p2</span><span class="p">,</span> <span class="n">bint</span> <span class="n">sortreduce</span><span class="o">=</span><span class="bp">True</span><span class="p">):</span></pre>
+<pre class='cython code score-46 '>static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_13intersect_line(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_f_7easyvec_8geometry_8PolyLine_intersect_line(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p2, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_opt_args_7easyvec_8geometry_8PolyLine_intersect_line *__pyx_optional_args) {
   int __pyx_v_sortreduce = ((int)1);
   PyObject *__pyx_r = NULL;
   <span class='refnanny'>__Pyx_RefNannyDeclarations</span>
   <span class='refnanny'>__Pyx_RefNannySetupContext</span>("intersect_line", 0);
   if (__pyx_optional_args) {
     if (__pyx_optional_args-&gt;__pyx_n &gt; 0) {
@@ -8690,17 +8941,17 @@
   __pyx_L0:;
   <span class='refnanny'>__Pyx_XGIVEREF</span>(__pyx_r);
   <span class='refnanny'>__Pyx_RefNannyFinishContext</span>();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_9intersect_line(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_7easyvec_8geometry_8PolyLine_8intersect_line[] = "PolyLine.intersect_line(self, Vec2 p1, Vec2 p2, bool sortreduce=True) -&gt; list";
-static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_9intersect_line(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_13intersect_line(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_7easyvec_8geometry_8PolyLine_12intersect_line[] = "PolyLine.intersect_line(self, Vec2 p1, Vec2 p2, bool sortreduce=True) -&gt; list";
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_13intersect_line(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p1 = 0;
   struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p2 = 0;
   int __pyx_v_sortreduce;
   PyObject *__pyx_r = 0;
   <span class='refnanny'>__Pyx_RefNannyDeclarations</span>
   <span class='refnanny'>__Pyx_RefNannySetupContext</span>("intersect_line (wrapper)", 0);
   {
@@ -8724,73 +8975,73 @@
         case  0:
         if (likely((values[0] = <span class='pyx_c_api'>__Pyx_PyDict_GetItemStr</span>(__pyx_kwds, __pyx_n_s_p1)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = <span class='pyx_c_api'>__Pyx_PyDict_GetItemStr</span>(__pyx_kwds, __pyx_n_s_p2)) != 0)) kw_args--;
         else {
-          <span class='pyx_c_api'>__Pyx_RaiseArgtupleInvalid</span>("intersect_line", 0, 2, 3, 1); <span class='error_goto'>__PYX_ERR(0, 614, __pyx_L3_error)</span>
+          <span class='pyx_c_api'>__Pyx_RaiseArgtupleInvalid</span>("intersect_line", 0, 2, 3, 1); <span class='error_goto'>__PYX_ERR(0, 626, __pyx_L3_error)</span>
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args &gt; 0) {
           PyObject* value = <span class='pyx_c_api'>__Pyx_PyDict_GetItemStr</span>(__pyx_kwds, __pyx_n_s_sortreduce);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args &gt; 0)) {
-        if (unlikely(<span class='pyx_c_api'>__Pyx_ParseOptionalKeywords</span>(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "intersect_line") &lt; 0)) <span class='error_goto'>__PYX_ERR(0, 614, __pyx_L3_error)</span>
+        if (unlikely(<span class='pyx_c_api'>__Pyx_ParseOptionalKeywords</span>(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "intersect_line") &lt; 0)) <span class='error_goto'>__PYX_ERR(0, 626, __pyx_L3_error)</span>
       }
     } else {
       switch (<span class='py_macro_api'>PyTuple_GET_SIZE</span>(__pyx_args)) {
         case  3: values[2] = <span class='py_macro_api'>PyTuple_GET_ITEM</span>(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = <span class='py_macro_api'>PyTuple_GET_ITEM</span>(__pyx_args, 1);
         values[0] = <span class='py_macro_api'>PyTuple_GET_ITEM</span>(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_p1 = ((struct __pyx_obj_7easyvec_7vectors_Vec2 *)values[0]);
     __pyx_v_p2 = ((struct __pyx_obj_7easyvec_7vectors_Vec2 *)values[1]);
     if (values[2]) {
-      __pyx_v_sortreduce = <span class='pyx_c_api'>__Pyx_PyObject_IsTrue</span>(values[2]); if (unlikely((__pyx_v_sortreduce == (int)-1) &amp;&amp; <span class='py_c_api'>PyErr_Occurred</span>())) <span class='error_goto'>__PYX_ERR(0, 614, __pyx_L3_error)</span>
+      __pyx_v_sortreduce = <span class='pyx_c_api'>__Pyx_PyObject_IsTrue</span>(values[2]); if (unlikely((__pyx_v_sortreduce == (int)-1) &amp;&amp; <span class='py_c_api'>PyErr_Occurred</span>())) <span class='error_goto'>__PYX_ERR(0, 626, __pyx_L3_error)</span>
     } else {
       __pyx_v_sortreduce = ((int)1);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  <span class='pyx_c_api'>__Pyx_RaiseArgtupleInvalid</span>("intersect_line", 0, 2, 3, <span class='py_macro_api'>PyTuple_GET_SIZE</span>(__pyx_args)); <span class='error_goto'>__PYX_ERR(0, 614, __pyx_L3_error)</span>
+  <span class='pyx_c_api'>__Pyx_RaiseArgtupleInvalid</span>("intersect_line", 0, 2, 3, <span class='py_macro_api'>PyTuple_GET_SIZE</span>(__pyx_args)); <span class='error_goto'>__PYX_ERR(0, 626, __pyx_L3_error)</span>
   __pyx_L3_error:;
   <span class='pyx_c_api'>__Pyx_AddTraceback</span>("easyvec.geometry.PolyLine.intersect_line", __pyx_clineno, __pyx_lineno, __pyx_filename);
   <span class='refnanny'>__Pyx_RefNannyFinishContext</span>();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!<span class='pyx_c_api'>__Pyx_ArgTypeTest</span>(((PyObject *)__pyx_v_p1), __pyx_ptype_7easyvec_7vectors_Vec2, 1, "p1", 0))) <span class='error_goto'>__PYX_ERR(0, 614, __pyx_L1_error)</span>
-  if (unlikely(!<span class='pyx_c_api'>__Pyx_ArgTypeTest</span>(((PyObject *)__pyx_v_p2), __pyx_ptype_7easyvec_7vectors_Vec2, 1, "p2", 0))) <span class='error_goto'>__PYX_ERR(0, 614, __pyx_L1_error)</span>
-  __pyx_r = __pyx_pf_7easyvec_8geometry_8PolyLine_8intersect_line(((struct __pyx_obj_7easyvec_8geometry_PolyLine *)__pyx_v_self), __pyx_v_p1, __pyx_v_p2, __pyx_v_sortreduce);
+  if (unlikely(!<span class='pyx_c_api'>__Pyx_ArgTypeTest</span>(((PyObject *)__pyx_v_p1), __pyx_ptype_7easyvec_7vectors_Vec2, 1, "p1", 0))) <span class='error_goto'>__PYX_ERR(0, 626, __pyx_L1_error)</span>
+  if (unlikely(!<span class='pyx_c_api'>__Pyx_ArgTypeTest</span>(((PyObject *)__pyx_v_p2), __pyx_ptype_7easyvec_7vectors_Vec2, 1, "p2", 0))) <span class='error_goto'>__PYX_ERR(0, 626, __pyx_L1_error)</span>
+  __pyx_r = __pyx_pf_7easyvec_8geometry_8PolyLine_12intersect_line(((struct __pyx_obj_7easyvec_8geometry_PolyLine *)__pyx_v_self), __pyx_v_p1, __pyx_v_p2, __pyx_v_sortreduce);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   <span class='refnanny'>__Pyx_RefNannyFinishContext</span>();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_8intersect_line(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p2, int __pyx_v_sortreduce) {
+static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_12intersect_line(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p2, int __pyx_v_sortreduce) {
   PyObject *__pyx_r = NULL;
   <span class='refnanny'>__Pyx_RefNannyDeclarations</span>
   <span class='refnanny'>__Pyx_RefNannySetupContext</span>("intersect_line", 0);
   <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_r);
   __pyx_t_2.__pyx_n = 1;
   __pyx_t_2.sortreduce = __pyx_v_sortreduce;
-  __pyx_t_1 = __pyx_vtabptr_7easyvec_8geometry_PolyLine-&gt;intersect_line(__pyx_v_self, __pyx_v_p1, __pyx_v_p2, 1, &amp;__pyx_t_2);<span class='error_goto'> if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 614, __pyx_L1_error)</span>
+  __pyx_t_1 = __pyx_vtabptr_7easyvec_8geometry_PolyLine-&gt;intersect_line(__pyx_v_self, __pyx_v_p1, __pyx_v_p2, 1, &amp;__pyx_t_2);<span class='error_goto'> if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 626, __pyx_L1_error)</span>
   <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -8798,27 +9049,27 @@
   <span class='pyx_c_api'>__Pyx_AddTraceback</span>("easyvec.geometry.PolyLine.intersect_line", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   <span class='refnanny'>__Pyx_XGIVEREF</span>(__pyx_r);
   <span class='refnanny'>__Pyx_RefNannyFinishContext</span>();
   return __pyx_r;
 }
-</pre><pre class="cython line score-1" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">615</span>:         <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">intersect_general</span><span class="p">(</span><span class="n">p1</span><span class="p">,</span> <span class="n">p2</span><span class="p">,</span> <span class="n">MINUS_BIG_REAL</span><span class="p">,</span> <span class="n">BIG_REAL</span><span class="p">,</span> <span class="n">sortreduce</span><span class="p">)</span></pre>
+</pre><pre class="cython line score-1" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">627</span>:         <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">intersect_general</span><span class="p">(</span><span class="n">p1</span><span class="p">,</span> <span class="n">p2</span><span class="p">,</span> <span class="n">MINUS_BIG_REAL</span><span class="p">,</span> <span class="n">BIG_REAL</span><span class="p">,</span> <span class="n">sortreduce</span><span class="p">)</span></pre>
 <pre class='cython code score-1 '>  <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_r);
   __pyx_t_2.__pyx_n = 1;
   __pyx_t_2.sortreduce = __pyx_v_sortreduce;
-  __pyx_t_1 = __pyx_f_7easyvec_8geometry_8PolyLine_intersect_general(__pyx_v_self, __pyx_v_p1, __pyx_v_p2, __pyx_v_7easyvec_7vectors_MINUS_BIG_REAL, __pyx_v_7easyvec_7vectors_BIG_REAL, 0, &amp;__pyx_t_2);<span class='error_goto'> if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 615, __pyx_L1_error)</span>
+  __pyx_t_1 = __pyx_f_7easyvec_8geometry_8PolyLine_intersect_general(__pyx_v_self, __pyx_v_p1, __pyx_v_p2, __pyx_v_7easyvec_7vectors_MINUS_BIG_REAL, __pyx_v_7easyvec_7vectors_BIG_REAL, 0, &amp;__pyx_t_2);<span class='error_goto'> if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 627, __pyx_L1_error)</span>
   <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_1);
   __pyx_r = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
   goto __pyx_L0;
-</pre><pre class="cython line score-0">&#xA0;<span class="">616</span>: </pre>
-<pre class="cython line score-0">&#xA0;<span class="">617</span>:     <span class="nd">@cython</span><span class="o">.</span><span class="n">nonecheck</span><span class="p">(</span><span class="bp">False</span><span class="p">)</span></pre>
-<pre class="cython line score-46" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">618</span>:     <span class="k">cpdef</span> <span class="kt">list</span> <span class="nf">intersect_ray</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">Vec2</span> <span class="n">p1</span><span class="p">,</span> <span class="n">Vec2</span> <span class="n">p2</span><span class="p">,</span> <span class="n">bint</span> <span class="n">sortreduce</span><span class="o">=</span><span class="bp">True</span><span class="p">):</span></pre>
-<pre class='cython code score-46 '>static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_11intersect_ray(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+</pre><pre class="cython line score-0">&#xA0;<span class="">628</span>: </pre>
+<pre class="cython line score-0">&#xA0;<span class="">629</span>:     <span class="nd">@cython</span><span class="o">.</span><span class="n">nonecheck</span><span class="p">(</span><span class="bp">False</span><span class="p">)</span></pre>
+<pre class="cython line score-46" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">630</span>:     <span class="k">cpdef</span> <span class="kt">list</span> <span class="nf">intersect_ray</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">Vec2</span> <span class="n">p1</span><span class="p">,</span> <span class="n">Vec2</span> <span class="n">p2</span><span class="p">,</span> <span class="n">bint</span> <span class="n">sortreduce</span><span class="o">=</span><span class="bp">True</span><span class="p">):</span></pre>
+<pre class='cython code score-46 '>static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_15intersect_ray(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_f_7easyvec_8geometry_8PolyLine_intersect_ray(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p2, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_opt_args_7easyvec_8geometry_8PolyLine_intersect_ray *__pyx_optional_args) {
   int __pyx_v_sortreduce = ((int)1);
   PyObject *__pyx_r = NULL;
   <span class='refnanny'>__Pyx_RefNannyDeclarations</span>
   <span class='refnanny'>__Pyx_RefNannySetupContext</span>("intersect_ray", 0);
   if (__pyx_optional_args) {
     if (__pyx_optional_args-&gt;__pyx_n &gt; 0) {
@@ -8834,17 +9085,17 @@
   __pyx_L0:;
   <span class='refnanny'>__Pyx_XGIVEREF</span>(__pyx_r);
   <span class='refnanny'>__Pyx_RefNannyFinishContext</span>();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_11intersect_ray(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_7easyvec_8geometry_8PolyLine_10intersect_ray[] = "PolyLine.intersect_ray(self, Vec2 p1, Vec2 p2, bool sortreduce=True) -&gt; list";
-static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_11intersect_ray(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_15intersect_ray(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_7easyvec_8geometry_8PolyLine_14intersect_ray[] = "PolyLine.intersect_ray(self, Vec2 p1, Vec2 p2, bool sortreduce=True) -&gt; list";
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_15intersect_ray(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p1 = 0;
   struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p2 = 0;
   int __pyx_v_sortreduce;
   PyObject *__pyx_r = 0;
   <span class='refnanny'>__Pyx_RefNannyDeclarations</span>
   <span class='refnanny'>__Pyx_RefNannySetupContext</span>("intersect_ray (wrapper)", 0);
   {
@@ -8868,73 +9119,73 @@
         case  0:
         if (likely((values[0] = <span class='pyx_c_api'>__Pyx_PyDict_GetItemStr</span>(__pyx_kwds, __pyx_n_s_p1)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = <span class='pyx_c_api'>__Pyx_PyDict_GetItemStr</span>(__pyx_kwds, __pyx_n_s_p2)) != 0)) kw_args--;
         else {
-          <span class='pyx_c_api'>__Pyx_RaiseArgtupleInvalid</span>("intersect_ray", 0, 2, 3, 1); <span class='error_goto'>__PYX_ERR(0, 618, __pyx_L3_error)</span>
+          <span class='pyx_c_api'>__Pyx_RaiseArgtupleInvalid</span>("intersect_ray", 0, 2, 3, 1); <span class='error_goto'>__PYX_ERR(0, 630, __pyx_L3_error)</span>
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args &gt; 0) {
           PyObject* value = <span class='pyx_c_api'>__Pyx_PyDict_GetItemStr</span>(__pyx_kwds, __pyx_n_s_sortreduce);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args &gt; 0)) {
-        if (unlikely(<span class='pyx_c_api'>__Pyx_ParseOptionalKeywords</span>(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "intersect_ray") &lt; 0)) <span class='error_goto'>__PYX_ERR(0, 618, __pyx_L3_error)</span>
+        if (unlikely(<span class='pyx_c_api'>__Pyx_ParseOptionalKeywords</span>(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "intersect_ray") &lt; 0)) <span class='error_goto'>__PYX_ERR(0, 630, __pyx_L3_error)</span>
       }
     } else {
       switch (<span class='py_macro_api'>PyTuple_GET_SIZE</span>(__pyx_args)) {
         case  3: values[2] = <span class='py_macro_api'>PyTuple_GET_ITEM</span>(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = <span class='py_macro_api'>PyTuple_GET_ITEM</span>(__pyx_args, 1);
         values[0] = <span class='py_macro_api'>PyTuple_GET_ITEM</span>(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_p1 = ((struct __pyx_obj_7easyvec_7vectors_Vec2 *)values[0]);
     __pyx_v_p2 = ((struct __pyx_obj_7easyvec_7vectors_Vec2 *)values[1]);
     if (values[2]) {
-      __pyx_v_sortreduce = <span class='pyx_c_api'>__Pyx_PyObject_IsTrue</span>(values[2]); if (unlikely((__pyx_v_sortreduce == (int)-1) &amp;&amp; <span class='py_c_api'>PyErr_Occurred</span>())) <span class='error_goto'>__PYX_ERR(0, 618, __pyx_L3_error)</span>
+      __pyx_v_sortreduce = <span class='pyx_c_api'>__Pyx_PyObject_IsTrue</span>(values[2]); if (unlikely((__pyx_v_sortreduce == (int)-1) &amp;&amp; <span class='py_c_api'>PyErr_Occurred</span>())) <span class='error_goto'>__PYX_ERR(0, 630, __pyx_L3_error)</span>
     } else {
       __pyx_v_sortreduce = ((int)1);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  <span class='pyx_c_api'>__Pyx_RaiseArgtupleInvalid</span>("intersect_ray", 0, 2, 3, <span class='py_macro_api'>PyTuple_GET_SIZE</span>(__pyx_args)); <span class='error_goto'>__PYX_ERR(0, 618, __pyx_L3_error)</span>
+  <span class='pyx_c_api'>__Pyx_RaiseArgtupleInvalid</span>("intersect_ray", 0, 2, 3, <span class='py_macro_api'>PyTuple_GET_SIZE</span>(__pyx_args)); <span class='error_goto'>__PYX_ERR(0, 630, __pyx_L3_error)</span>
   __pyx_L3_error:;
   <span class='pyx_c_api'>__Pyx_AddTraceback</span>("easyvec.geometry.PolyLine.intersect_ray", __pyx_clineno, __pyx_lineno, __pyx_filename);
   <span class='refnanny'>__Pyx_RefNannyFinishContext</span>();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!<span class='pyx_c_api'>__Pyx_ArgTypeTest</span>(((PyObject *)__pyx_v_p1), __pyx_ptype_7easyvec_7vectors_Vec2, 1, "p1", 0))) <span class='error_goto'>__PYX_ERR(0, 618, __pyx_L1_error)</span>
-  if (unlikely(!<span class='pyx_c_api'>__Pyx_ArgTypeTest</span>(((PyObject *)__pyx_v_p2), __pyx_ptype_7easyvec_7vectors_Vec2, 1, "p2", 0))) <span class='error_goto'>__PYX_ERR(0, 618, __pyx_L1_error)</span>
-  __pyx_r = __pyx_pf_7easyvec_8geometry_8PolyLine_10intersect_ray(((struct __pyx_obj_7easyvec_8geometry_PolyLine *)__pyx_v_self), __pyx_v_p1, __pyx_v_p2, __pyx_v_sortreduce);
+  if (unlikely(!<span class='pyx_c_api'>__Pyx_ArgTypeTest</span>(((PyObject *)__pyx_v_p1), __pyx_ptype_7easyvec_7vectors_Vec2, 1, "p1", 0))) <span class='error_goto'>__PYX_ERR(0, 630, __pyx_L1_error)</span>
+  if (unlikely(!<span class='pyx_c_api'>__Pyx_ArgTypeTest</span>(((PyObject *)__pyx_v_p2), __pyx_ptype_7easyvec_7vectors_Vec2, 1, "p2", 0))) <span class='error_goto'>__PYX_ERR(0, 630, __pyx_L1_error)</span>
+  __pyx_r = __pyx_pf_7easyvec_8geometry_8PolyLine_14intersect_ray(((struct __pyx_obj_7easyvec_8geometry_PolyLine *)__pyx_v_self), __pyx_v_p1, __pyx_v_p2, __pyx_v_sortreduce);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   <span class='refnanny'>__Pyx_RefNannyFinishContext</span>();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_10intersect_ray(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p2, int __pyx_v_sortreduce) {
+static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_14intersect_ray(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p2, int __pyx_v_sortreduce) {
   PyObject *__pyx_r = NULL;
   <span class='refnanny'>__Pyx_RefNannyDeclarations</span>
   <span class='refnanny'>__Pyx_RefNannySetupContext</span>("intersect_ray", 0);
   <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_r);
   __pyx_t_2.__pyx_n = 1;
   __pyx_t_2.sortreduce = __pyx_v_sortreduce;
-  __pyx_t_1 = __pyx_vtabptr_7easyvec_8geometry_PolyLine-&gt;intersect_ray(__pyx_v_self, __pyx_v_p1, __pyx_v_p2, 1, &amp;__pyx_t_2);<span class='error_goto'> if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 618, __pyx_L1_error)</span>
+  __pyx_t_1 = __pyx_vtabptr_7easyvec_8geometry_PolyLine-&gt;intersect_ray(__pyx_v_self, __pyx_v_p1, __pyx_v_p2, 1, &amp;__pyx_t_2);<span class='error_goto'> if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 630, __pyx_L1_error)</span>
   <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -8942,27 +9193,27 @@
   <span class='pyx_c_api'>__Pyx_AddTraceback</span>("easyvec.geometry.PolyLine.intersect_ray", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   <span class='refnanny'>__Pyx_XGIVEREF</span>(__pyx_r);
   <span class='refnanny'>__Pyx_RefNannyFinishContext</span>();
   return __pyx_r;
 }
-</pre><pre class="cython line score-1" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">619</span>:         <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">intersect_general</span><span class="p">(</span><span class="n">p1</span><span class="p">,</span> <span class="n">p2</span><span class="p">,</span> <span class="mf">0.0</span><span class="p">,</span> <span class="n">BIG_REAL</span><span class="p">,</span> <span class="n">sortreduce</span><span class="p">)</span></pre>
+</pre><pre class="cython line score-1" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">631</span>:         <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">intersect_general</span><span class="p">(</span><span class="n">p1</span><span class="p">,</span> <span class="n">p2</span><span class="p">,</span> <span class="mf">0.0</span><span class="p">,</span> <span class="n">BIG_REAL</span><span class="p">,</span> <span class="n">sortreduce</span><span class="p">)</span></pre>
 <pre class='cython code score-1 '>  <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_r);
   __pyx_t_2.__pyx_n = 1;
   __pyx_t_2.sortreduce = __pyx_v_sortreduce;
-  __pyx_t_1 = __pyx_f_7easyvec_8geometry_8PolyLine_intersect_general(__pyx_v_self, __pyx_v_p1, __pyx_v_p2, 0.0, __pyx_v_7easyvec_7vectors_BIG_REAL, 0, &amp;__pyx_t_2);<span class='error_goto'> if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 619, __pyx_L1_error)</span>
+  __pyx_t_1 = __pyx_f_7easyvec_8geometry_8PolyLine_intersect_general(__pyx_v_self, __pyx_v_p1, __pyx_v_p2, 0.0, __pyx_v_7easyvec_7vectors_BIG_REAL, 0, &amp;__pyx_t_2);<span class='error_goto'> if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 631, __pyx_L1_error)</span>
   <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_1);
   __pyx_r = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
   goto __pyx_L0;
-</pre><pre class="cython line score-0">&#xA0;<span class="">620</span>: </pre>
-<pre class="cython line score-0">&#xA0;<span class="">621</span>:     <span class="nd">@cython</span><span class="o">.</span><span class="n">nonecheck</span><span class="p">(</span><span class="bp">False</span><span class="p">)</span></pre>
-<pre class="cython line score-46" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">622</span>:     <span class="k">cpdef</span> <span class="kt">list</span> <span class="nf">intersect_segment</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">Vec2</span> <span class="n">p1</span><span class="p">,</span> <span class="n">Vec2</span> <span class="n">p2</span><span class="p">,</span> <span class="n">bint</span> <span class="n">sortreduce</span><span class="o">=</span><span class="bp">True</span><span class="p">):</span></pre>
-<pre class='cython code score-46 '>static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_13intersect_segment(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+</pre><pre class="cython line score-0">&#xA0;<span class="">632</span>: </pre>
+<pre class="cython line score-0">&#xA0;<span class="">633</span>:     <span class="nd">@cython</span><span class="o">.</span><span class="n">nonecheck</span><span class="p">(</span><span class="bp">False</span><span class="p">)</span></pre>
+<pre class="cython line score-46" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">634</span>:     <span class="k">cpdef</span> <span class="kt">list</span> <span class="nf">intersect_segment</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">Vec2</span> <span class="n">p1</span><span class="p">,</span> <span class="n">Vec2</span> <span class="n">p2</span><span class="p">,</span> <span class="n">bint</span> <span class="n">sortreduce</span><span class="o">=</span><span class="bp">True</span><span class="p">):</span></pre>
+<pre class='cython code score-46 '>static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_17intersect_segment(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_f_7easyvec_8geometry_8PolyLine_intersect_segment(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p2, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_opt_args_7easyvec_8geometry_8PolyLine_intersect_segment *__pyx_optional_args) {
   int __pyx_v_sortreduce = ((int)1);
   PyObject *__pyx_r = NULL;
   <span class='refnanny'>__Pyx_RefNannyDeclarations</span>
   <span class='refnanny'>__Pyx_RefNannySetupContext</span>("intersect_segment", 0);
   if (__pyx_optional_args) {
     if (__pyx_optional_args-&gt;__pyx_n &gt; 0) {
@@ -8978,17 +9229,17 @@
   __pyx_L0:;
   <span class='refnanny'>__Pyx_XGIVEREF</span>(__pyx_r);
   <span class='refnanny'>__Pyx_RefNannyFinishContext</span>();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_13intersect_segment(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_7easyvec_8geometry_8PolyLine_12intersect_segment[] = "PolyLine.intersect_segment(self, Vec2 p1, Vec2 p2, bool sortreduce=True) -&gt; list";
-static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_13intersect_segment(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_17intersect_segment(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_7easyvec_8geometry_8PolyLine_16intersect_segment[] = "PolyLine.intersect_segment(self, Vec2 p1, Vec2 p2, bool sortreduce=True) -&gt; list";
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_17intersect_segment(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p1 = 0;
   struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p2 = 0;
   int __pyx_v_sortreduce;
   PyObject *__pyx_r = 0;
   <span class='refnanny'>__Pyx_RefNannyDeclarations</span>
   <span class='refnanny'>__Pyx_RefNannySetupContext</span>("intersect_segment (wrapper)", 0);
   {
@@ -9012,73 +9263,73 @@
         case  0:
         if (likely((values[0] = <span class='pyx_c_api'>__Pyx_PyDict_GetItemStr</span>(__pyx_kwds, __pyx_n_s_p1)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = <span class='pyx_c_api'>__Pyx_PyDict_GetItemStr</span>(__pyx_kwds, __pyx_n_s_p2)) != 0)) kw_args--;
         else {
-          <span class='pyx_c_api'>__Pyx_RaiseArgtupleInvalid</span>("intersect_segment", 0, 2, 3, 1); <span class='error_goto'>__PYX_ERR(0, 622, __pyx_L3_error)</span>
+          <span class='pyx_c_api'>__Pyx_RaiseArgtupleInvalid</span>("intersect_segment", 0, 2, 3, 1); <span class='error_goto'>__PYX_ERR(0, 634, __pyx_L3_error)</span>
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args &gt; 0) {
           PyObject* value = <span class='pyx_c_api'>__Pyx_PyDict_GetItemStr</span>(__pyx_kwds, __pyx_n_s_sortreduce);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args &gt; 0)) {
-        if (unlikely(<span class='pyx_c_api'>__Pyx_ParseOptionalKeywords</span>(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "intersect_segment") &lt; 0)) <span class='error_goto'>__PYX_ERR(0, 622, __pyx_L3_error)</span>
+        if (unlikely(<span class='pyx_c_api'>__Pyx_ParseOptionalKeywords</span>(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "intersect_segment") &lt; 0)) <span class='error_goto'>__PYX_ERR(0, 634, __pyx_L3_error)</span>
       }
     } else {
       switch (<span class='py_macro_api'>PyTuple_GET_SIZE</span>(__pyx_args)) {
         case  3: values[2] = <span class='py_macro_api'>PyTuple_GET_ITEM</span>(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = <span class='py_macro_api'>PyTuple_GET_ITEM</span>(__pyx_args, 1);
         values[0] = <span class='py_macro_api'>PyTuple_GET_ITEM</span>(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_p1 = ((struct __pyx_obj_7easyvec_7vectors_Vec2 *)values[0]);
     __pyx_v_p2 = ((struct __pyx_obj_7easyvec_7vectors_Vec2 *)values[1]);
     if (values[2]) {
-      __pyx_v_sortreduce = <span class='pyx_c_api'>__Pyx_PyObject_IsTrue</span>(values[2]); if (unlikely((__pyx_v_sortreduce == (int)-1) &amp;&amp; <span class='py_c_api'>PyErr_Occurred</span>())) <span class='error_goto'>__PYX_ERR(0, 622, __pyx_L3_error)</span>
+      __pyx_v_sortreduce = <span class='pyx_c_api'>__Pyx_PyObject_IsTrue</span>(values[2]); if (unlikely((__pyx_v_sortreduce == (int)-1) &amp;&amp; <span class='py_c_api'>PyErr_Occurred</span>())) <span class='error_goto'>__PYX_ERR(0, 634, __pyx_L3_error)</span>
     } else {
       __pyx_v_sortreduce = ((int)1);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  <span class='pyx_c_api'>__Pyx_RaiseArgtupleInvalid</span>("intersect_segment", 0, 2, 3, <span class='py_macro_api'>PyTuple_GET_SIZE</span>(__pyx_args)); <span class='error_goto'>__PYX_ERR(0, 622, __pyx_L3_error)</span>
+  <span class='pyx_c_api'>__Pyx_RaiseArgtupleInvalid</span>("intersect_segment", 0, 2, 3, <span class='py_macro_api'>PyTuple_GET_SIZE</span>(__pyx_args)); <span class='error_goto'>__PYX_ERR(0, 634, __pyx_L3_error)</span>
   __pyx_L3_error:;
   <span class='pyx_c_api'>__Pyx_AddTraceback</span>("easyvec.geometry.PolyLine.intersect_segment", __pyx_clineno, __pyx_lineno, __pyx_filename);
   <span class='refnanny'>__Pyx_RefNannyFinishContext</span>();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!<span class='pyx_c_api'>__Pyx_ArgTypeTest</span>(((PyObject *)__pyx_v_p1), __pyx_ptype_7easyvec_7vectors_Vec2, 1, "p1", 0))) <span class='error_goto'>__PYX_ERR(0, 622, __pyx_L1_error)</span>
-  if (unlikely(!<span class='pyx_c_api'>__Pyx_ArgTypeTest</span>(((PyObject *)__pyx_v_p2), __pyx_ptype_7easyvec_7vectors_Vec2, 1, "p2", 0))) <span class='error_goto'>__PYX_ERR(0, 622, __pyx_L1_error)</span>
-  __pyx_r = __pyx_pf_7easyvec_8geometry_8PolyLine_12intersect_segment(((struct __pyx_obj_7easyvec_8geometry_PolyLine *)__pyx_v_self), __pyx_v_p1, __pyx_v_p2, __pyx_v_sortreduce);
+  if (unlikely(!<span class='pyx_c_api'>__Pyx_ArgTypeTest</span>(((PyObject *)__pyx_v_p1), __pyx_ptype_7easyvec_7vectors_Vec2, 1, "p1", 0))) <span class='error_goto'>__PYX_ERR(0, 634, __pyx_L1_error)</span>
+  if (unlikely(!<span class='pyx_c_api'>__Pyx_ArgTypeTest</span>(((PyObject *)__pyx_v_p2), __pyx_ptype_7easyvec_7vectors_Vec2, 1, "p2", 0))) <span class='error_goto'>__PYX_ERR(0, 634, __pyx_L1_error)</span>
+  __pyx_r = __pyx_pf_7easyvec_8geometry_8PolyLine_16intersect_segment(((struct __pyx_obj_7easyvec_8geometry_PolyLine *)__pyx_v_self), __pyx_v_p1, __pyx_v_p2, __pyx_v_sortreduce);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   <span class='refnanny'>__Pyx_RefNannyFinishContext</span>();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_12intersect_segment(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p2, int __pyx_v_sortreduce) {
+static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_16intersect_segment(struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p1, struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p2, int __pyx_v_sortreduce) {
   PyObject *__pyx_r = NULL;
   <span class='refnanny'>__Pyx_RefNannyDeclarations</span>
   <span class='refnanny'>__Pyx_RefNannySetupContext</span>("intersect_segment", 0);
   <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_r);
   __pyx_t_2.__pyx_n = 1;
   __pyx_t_2.sortreduce = __pyx_v_sortreduce;
-  __pyx_t_1 = __pyx_vtabptr_7easyvec_8geometry_PolyLine-&gt;intersect_segment(__pyx_v_self, __pyx_v_p1, __pyx_v_p2, 1, &amp;__pyx_t_2);<span class='error_goto'> if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 622, __pyx_L1_error)</span>
+  __pyx_t_1 = __pyx_vtabptr_7easyvec_8geometry_PolyLine-&gt;intersect_segment(__pyx_v_self, __pyx_v_p1, __pyx_v_p2, 1, &amp;__pyx_t_2);<span class='error_goto'> if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 634, __pyx_L1_error)</span>
   <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -9086,21 +9337,21 @@
   <span class='pyx_c_api'>__Pyx_AddTraceback</span>("easyvec.geometry.PolyLine.intersect_segment", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   <span class='refnanny'>__Pyx_XGIVEREF</span>(__pyx_r);
   <span class='refnanny'>__Pyx_RefNannyFinishContext</span>();
   return __pyx_r;
 }
-</pre><pre class="cython line score-1" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">623</span>:         <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">intersect_general</span><span class="p">(</span><span class="n">p1</span><span class="p">,</span> <span class="n">p2</span><span class="p">,</span> <span class="mf">0.0</span><span class="p">,</span> <span class="mf">1.0</span><span class="p">,</span> <span class="n">sortreduce</span><span class="p">)</span></pre>
+</pre><pre class="cython line score-1" onclick="(function(s){s.display=s.display==='block'?'none':'block'})(this.nextElementSibling.style)">+<span class="">635</span>:         <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">intersect_general</span><span class="p">(</span><span class="n">p1</span><span class="p">,</span> <span class="n">p2</span><span class="p">,</span> <span class="mf">0.0</span><span class="p">,</span> <span class="mf">1.0</span><span class="p">,</span> <span class="n">sortreduce</span><span class="p">)</span></pre>
 <pre class='cython code score-1 '>  <span class='pyx_macro_api'>__Pyx_XDECREF</span>(__pyx_r);
   __pyx_t_2.__pyx_n = 1;
   __pyx_t_2.sortreduce = __pyx_v_sortreduce;
-  __pyx_t_1 = __pyx_f_7easyvec_8geometry_8PolyLine_intersect_general(__pyx_v_self, __pyx_v_p1, __pyx_v_p2, 0.0, 1.0, 0, &amp;__pyx_t_2);<span class='error_goto'> if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 623, __pyx_L1_error)</span>
+  __pyx_t_1 = __pyx_f_7easyvec_8geometry_8PolyLine_intersect_general(__pyx_v_self, __pyx_v_p1, __pyx_v_p2, 0.0, 1.0, 0, &amp;__pyx_t_2);<span class='error_goto'> if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 635, __pyx_L1_error)</span>
   <span class='refnanny'>__Pyx_GOTREF</span>(__pyx_t_1);
   __pyx_r = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
   goto __pyx_L0;
-</pre><pre class="cython line score-0">&#xA0;<span class="">624</span>: </pre>
-<pre class="cython line score-0">&#xA0;<span class="">625</span>: </pre>
-<pre class="cython line score-0">&#xA0;<span class="">626</span>: </pre>
-<pre class="cython line score-0">&#xA0;<span class="">627</span>: </pre>
+</pre><pre class="cython line score-0">&#xA0;<span class="">636</span>: </pre>
+<pre class="cython line score-0">&#xA0;<span class="">637</span>: </pre>
+<pre class="cython line score-0">&#xA0;<span class="">638</span>: </pre>
+<pre class="cython line score-0">&#xA0;<span class="">639</span>: </pre>
 </div></body></html>
```

#### html2text {}

```diff
@@ -8,20 +8,20 @@
   __pyx_t_1 = __Pyx_Import(__pyx_n_s_numpy, 0, 0); if (unlikely(!__pyx_t_1))
 __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_1) < 0) __PYX_ERR(0, 1,
 __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 /* … */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR
 (0, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1,
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1,
 __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 &#xA0;002: from libc.math cimport fabs
 &#xA0;003: cimport cython
 &#xA0;004: from .vectors cimport CMP_TOL, real, Vec2, rational, BIG_REAL,
 MINUS_BIG_REAL
 &#xA0;005: from cpython.object cimport Py_LT, Py_LE, Py_EQ, Py_GE, Py_GT, Py_NE
 &#xA0;006:
 +007: cdef array.array _int_array_template = array.array('i', [])
@@ -1292,29 +1292,29 @@
 &#xA0;085: @cython.nonecheck(False)
 &#xA0;086: @cython.cdivision(True)
 +087: cpdef (bint, real, real) _intersect_ts(Vec2 u1, Vec2 u2, Vec2 v1, Vec2
 v2):
 static PyObject *__pyx_pw_7easyvec_8geometry_7_intersect_ts(PyObject
 *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static
-__pyx_ctuple_d78dc__int__and___dunderpyx_t_7easyvec_7vectors_real__and___dunderpyx_t_7easyvec_7vectors_real__etc
+__pyx_ctuple_acdc9__int__and___dunderpyx_t_7easyvec_7vectors_real__and___dunderpyx_t_7easyvec_7vectors_real__etc
 __pyx_f_7easyvec_8geometry__intersect_ts(struct
 __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_u1, struct
 __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_u2, struct
 __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_v1, struct
 __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_v2, CYTHON_UNUSED int
 __pyx_skip_dispatch) {
   struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_vec1 = 0;
   struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_vec2 = 0;
   struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_vec3 = 0;
   __pyx_t_7easyvec_7vectors_real __pyx_v_dot;
   __pyx_t_7easyvec_7vectors_real __pyx_v_t1;
   __pyx_t_7easyvec_7vectors_real __pyx_v_t2;
 
-__pyx_ctuple_d78dc__int__and___dunderpyx_t_7easyvec_7vectors_real__and___dunderpyx_t_7easyvec_7vectors_real__etc
+__pyx_ctuple_acdc9__int__and___dunderpyx_t_7easyvec_7vectors_real__and___dunderpyx_t_7easyvec_7vectors_real__etc
 __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_intersect_ts", 0);
 /* … */
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
@@ -1451,15 +1451,15 @@
 __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_v1, struct
 __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_v2) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_intersect_ts", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 =
-__pyx_convert__to_py___pyx_ctuple_d78dc__int__and___dunderpyx_t_7easyvec_7vectors_real__and___dunderpyx_t_7easyvec_7vectors_real__etc
+__pyx_convert__to_py___pyx_ctuple_acdc9__int__and___dunderpyx_t_7easyvec_7vectors_real__and___dunderpyx_t_7easyvec_7vectors_real__etc
 (__pyx_f_7easyvec_8geometry__intersect_ts(__pyx_v_u1, __pyx_v_u2, __pyx_v_v1,
 __pyx_v_v2, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
@@ -9288,19 +9288,200 @@
 *__pyx_optional_args);
 static PyObject *__pyx_f_7easyvec_8geometry_8PolyLine_intersect_segment(struct
 __pyx_obj_7easyvec_8geometry_PolyLine *, struct
 __pyx_obj_7easyvec_7vectors_Vec2 *, struct __pyx_obj_7easyvec_7vectors_Vec2 *,
 int __pyx_skip_dispatch, struct
 __pyx_opt_args_7easyvec_8geometry_8PolyLine_intersect_segment
 *__pyx_optional_args);
-+559:     def __cinit__(self, vecs: list, enclosed=True, copy_data=False):
++559:     @classmethod
+  __pyx_t_1 = __Pyx_Method_ClassMethod(__pyx_t_2); if (unlikely(!__pyx_t_1))
+__PYX_ERR(0, 559, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_7easyvec_8geometry_PolyLine-
+>tp_dict, __pyx_n_s_from_dict, __pyx_t_1) < 0) __PYX_ERR(0, 560,
+__pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  PyType_Modified(__pyx_ptype_7easyvec_8geometry_PolyLine);
++560:     def from_dict(cls, dct):
 /* Python wrapper */
-static int __pyx_pw_7easyvec_8geometry_8PolyLine_1__cinit__(PyObject
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_1from_dict(PyObject
+*__pyx_v_cls, PyObject *__pyx_v_dct); /*proto*/
+static char __pyx_doc_7easyvec_8geometry_8PolyLine_from_dict[] =
+"PolyLine.from_dict(type cls, dct)";
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_1from_dict(PyObject
+*__pyx_v_cls, PyObject *__pyx_v_dct) {
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("from_dict (wrapper)", 0);
+  __pyx_r = __pyx_pf_7easyvec_8geometry_8PolyLine_from_dict((
+(PyTypeObject*)__pyx_v_cls), ((PyObject *)__pyx_v_dct));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_from_dict(PyTypeObject
+*__pyx_v_cls, PyObject *__pyx_v_dct) {
+  PyObject *__pyx_v_vecs = NULL;
+  PyObject *__pyx_v_enclosed = NULL;
+  PyObject *__pyx_7genexpr__pyx_v_vd = NULL;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("from_dict", 0);
+/* … */
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_AddTraceback("easyvec.geometry.PolyLine.from_dict", __pyx_clineno,
+__pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_vecs);
+  __Pyx_XDECREF(__pyx_v_enclosed);
+  __Pyx_XDECREF(__pyx_7genexpr__pyx_v_vd);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+/* … */
+  __Pyx_GetNameInClass(__pyx_t_2, (PyObject
+*)__pyx_ptype_7easyvec_8geometry_PolyLine, __pyx_n_s_from_dict); if (unlikely
+(!__pyx_t_2)) __PYX_ERR(0, 560, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
++561:         vecs = [Vec2.from_dict(vd) for vd in dct['vecs']]
+  { /* enter inner scope */
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 561,
+__pyx_L5_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_v_dct, __pyx_n_u_vecs); if
+(unlikely(!__pyx_t_2)) __PYX_ERR(0, 561, __pyx_L5_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    if (likely(PyList_CheckExact(__pyx_t_2)) || PyTuple_CheckExact(__pyx_t_2))
+{
+      __pyx_t_3 = __pyx_t_2; __Pyx_INCREF(__pyx_t_3); __pyx_t_4 = 0;
+      __pyx_t_5 = NULL;
+    } else {
+      __pyx_t_4 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_t_2); if (unlikely
+(!__pyx_t_3)) __PYX_ERR(0, 561, __pyx_L5_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __pyx_t_5 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_5))
+__PYX_ERR(0, 561, __pyx_L5_error)
+    }
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    for (;;) {
+      if (likely(!__pyx_t_5)) {
+        if (likely(PyList_CheckExact(__pyx_t_3))) {
+          if (__pyx_t_4 >= PyList_GET_SIZE(__pyx_t_3)) break;
+          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+          __pyx_t_2 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF
+(__pyx_t_2); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 561,
+__pyx_L5_error)
+          #else
+          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if
+(unlikely(!__pyx_t_2)) __PYX_ERR(0, 561, __pyx_L5_error)
+          __Pyx_GOTREF(__pyx_t_2);
+          #endif
+        } else {
+          if (__pyx_t_4 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
+          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+          __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF
+(__pyx_t_2); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 561,
+__pyx_L5_error)
+          #else
+          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if
+(unlikely(!__pyx_t_2)) __PYX_ERR(0, 561, __pyx_L5_error)
+          __Pyx_GOTREF(__pyx_t_2);
+          #endif
+        }
+      } else {
+        __pyx_t_2 = __pyx_t_5(__pyx_t_3);
+        if (unlikely(!__pyx_t_2)) {
+          PyObject* exc_type = PyErr_Occurred();
+          if (exc_type) {
+            if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type,
+PyExc_StopIteration))) PyErr_Clear();
+            else __PYX_ERR(0, 561, __pyx_L5_error)
+          }
+          break;
+        }
+        __Pyx_GOTREF(__pyx_t_2);
+      }
+      __Pyx_XDECREF_SET(__pyx_7genexpr__pyx_v_vd, __pyx_t_2);
+      __pyx_t_2 = 0;
+      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(((PyObject
+*)__pyx_ptype_7easyvec_7vectors_Vec2), __pyx_n_s_from_dict); if (unlikely
+(!__pyx_t_6)) __PYX_ERR(0, 561, __pyx_L5_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __pyx_t_7 = NULL;
+      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
+        __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
+        if (likely(__pyx_t_7)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
+          __Pyx_INCREF(__pyx_t_7);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_6, function);
+        }
+      }
+      __pyx_t_2 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_7,
+__pyx_7genexpr__pyx_v_vd) : __Pyx_PyObject_CallOneArg(__pyx_t_6,
+__pyx_7genexpr__pyx_v_vd);
+      __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 561, __pyx_L5_error)
+      __Pyx_GOTREF(__pyx_t_2);
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_2)))
+__PYX_ERR(0, 561, __pyx_L5_error)
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    }
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_XDECREF(__pyx_7genexpr__pyx_v_vd); __pyx_7genexpr__pyx_v_vd = 0;
+    goto __pyx_L8_exit_scope;
+    __pyx_L5_error:;
+    __Pyx_XDECREF(__pyx_7genexpr__pyx_v_vd); __pyx_7genexpr__pyx_v_vd = 0;
+    goto __pyx_L1_error;
+    __pyx_L8_exit_scope:;
+  } /* exit inner scope */
+  __pyx_v_vecs = ((PyObject*)__pyx_t_1);
+  __pyx_t_1 = 0;
++562:         enclosed = dct['enclosed']
+  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_dct, __pyx_n_u_enclosed); if
+(unlikely(!__pyx_t_1)) __PYX_ERR(0, 562, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_v_enclosed = __pyx_t_1;
+  __pyx_t_1 = 0;
++563:         return cls(vecs, enclosed)
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 563,
+__pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_INCREF(__pyx_v_vecs);
+  __Pyx_GIVEREF(__pyx_v_vecs);
+  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_vecs);
+  __Pyx_INCREF(__pyx_v_enclosed);
+  __Pyx_GIVEREF(__pyx_v_enclosed);
+  PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_enclosed);
+  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_v_cls), __pyx_t_1, NULL);
+if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 563, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_r = __pyx_t_3;
+  __pyx_t_3 = 0;
+  goto __pyx_L0;
+&#xA0;564:
++565:     def __cinit__(self, vecs: list, enclosed=True, copy_data=False):
+/* Python wrapper */
+static int __pyx_pw_7easyvec_8geometry_8PolyLine_3__cinit__(PyObject
 *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static int __pyx_pw_7easyvec_8geometry_8PolyLine_1__cinit__(PyObject
+static int __pyx_pw_7easyvec_8geometry_8PolyLine_3__cinit__(PyObject
 *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_vecs = 0;
   PyObject *__pyx_v_enclosed = 0;
   PyObject *__pyx_v_copy_data = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__ (wrapper)", 0);
@@ -9342,15 +9523,15 @@
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds,
 __pyx_n_s_copy_data);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
         if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames,
-0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 559, __pyx_L3_error)
+0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 565, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
@@ -9362,37 +9543,37 @@
     __pyx_v_vecs = ((PyObject*)values[0]);
     __pyx_v_enclosed = values[1];
     __pyx_v_copy_data = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 1, 3, PyTuple_GET_SIZE
-(__pyx_args)); __PYX_ERR(0, 559, __pyx_L3_error)
+(__pyx_args)); __PYX_ERR(0, 565, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("easyvec.geometry.PolyLine.__cinit__", __pyx_clineno,
 __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_vecs), (&PyList_Type),
-1, "vecs", 1))) __PYX_ERR(0, 559, __pyx_L1_error)
-  __pyx_r = __pyx_pf_7easyvec_8geometry_8PolyLine___cinit__(((struct
+1, "vecs", 1))) __PYX_ERR(0, 565, __pyx_L1_error)
+  __pyx_r = __pyx_pf_7easyvec_8geometry_8PolyLine_2__cinit__(((struct
 __pyx_obj_7easyvec_8geometry_PolyLine *)__pyx_v_self), __pyx_v_vecs,
 __pyx_v_enclosed, __pyx_v_copy_data);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static int __pyx_pf_7easyvec_8geometry_8PolyLine___cinit__(struct
+static int __pyx_pf_7easyvec_8geometry_8PolyLine_2__cinit__(struct
 __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self, PyObject *__pyx_v_vecs,
 PyObject *__pyx_v_enclosed, PyObject *__pyx_v_copy_data) {
   int __pyx_v_vec_len;
   int __pyx_v_i;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__", 0);
@@ -9407,163 +9588,281 @@
   __Pyx_AddTraceback("easyvec.geometry.PolyLine.__cinit__", __pyx_clineno,
 __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
-&#xA0;560:         cdef int vec_len, i
-+561:         if copy_data:
+&#xA0;566:         cdef int vec_len, i
++567:         if copy_data:
   __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_copy_data); if (unlikely(__pyx_t_1
-< 0)) __PYX_ERR(0, 561, __pyx_L1_error)
+< 0)) __PYX_ERR(0, 567, __pyx_L1_error)
   if (__pyx_t_1) {
 /* … */
     goto __pyx_L3;
   }
-+562:             self.vecs = []
-    __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 562,
++568:             self.vecs = []
+    __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 568,
 __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_GIVEREF(__pyx_t_2);
     __Pyx_GOTREF(__pyx_v_self->vecs);
     __Pyx_DECREF(__pyx_v_self->vecs);
     __pyx_v_self->vecs = ((PyObject*)__pyx_t_2);
     __pyx_t_2 = 0;
-+563:             vec_len = len(vecs)
++569:             vec_len = len(vecs)
     if (unlikely(__pyx_v_vecs == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len
 ()");
-      __PYX_ERR(0, 563, __pyx_L1_error)
+      __PYX_ERR(0, 569, __pyx_L1_error)
     }
     __pyx_t_3 = PyList_GET_SIZE(__pyx_v_vecs); if (unlikely(__pyx_t_3 == (
-(Py_ssize_t)-1))) __PYX_ERR(0, 563, __pyx_L1_error)
+(Py_ssize_t)-1))) __PYX_ERR(0, 569, __pyx_L1_error)
     __pyx_v_vec_len = __pyx_t_3;
-+564:             for i in range(vec_len):
++570:             for i in range(vec_len):
     __pyx_t_4 = __pyx_v_vec_len;
     __pyx_t_5 = __pyx_t_4;
     for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
       __pyx_v_i = __pyx_t_6;
-+565:                 self.vecs.append( (<Vec2>(vecs[i])).copy() )
++571:                 self.vecs.append( (<Vec2>(vecs[i])).copy() )
       if (unlikely(__pyx_v_self->vecs == Py_None)) {
         PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute
 '%.30s'", "append");
-        __PYX_ERR(0, 565, __pyx_L1_error)
+        __PYX_ERR(0, 571, __pyx_L1_error)
       }
       if (unlikely(__pyx_v_vecs == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not
 subscriptable");
-        __PYX_ERR(0, 565, __pyx_L1_error)
+        __PYX_ERR(0, 571, __pyx_L1_error)
       }
       __pyx_t_2 = __Pyx_GetItemInt_List(__pyx_v_vecs, __pyx_v_i, int, 1,
-__Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 565,
+__Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 571,
 __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __pyx_t_7 = ((PyObject *)((struct __pyx_vtabstruct_7easyvec_7vectors_Vec2
 *)((struct __pyx_obj_7easyvec_7vectors_Vec2 *)__pyx_t_2)->__pyx_vtab)->copy((
 (struct __pyx_obj_7easyvec_7vectors_Vec2 *)__pyx_t_2), 0)); if (unlikely
-(!__pyx_t_7)) __PYX_ERR(0, 565, __pyx_L1_error)
+(!__pyx_t_7)) __PYX_ERR(0, 571, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __pyx_t_8 = __Pyx_PyList_Append(__pyx_v_self->vecs, __pyx_t_7); if
-(unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(0, 565, __pyx_L1_error)
+(unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(0, 571, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     }
-&#xA0;566:         else:
-+567:             self.vecs = vecs
+&#xA0;572:         else:
++573:             self.vecs = vecs
   /*else*/ {
     __Pyx_INCREF(__pyx_v_vecs);
     __Pyx_GIVEREF(__pyx_v_vecs);
     __Pyx_GOTREF(__pyx_v_self->vecs);
     __Pyx_DECREF(__pyx_v_self->vecs);
     __pyx_v_self->vecs = __pyx_v_vecs;
   }
   __pyx_L3:;
-+568:         self.vlen = len(self.vecs)
++574:         self.vlen = len(self.vecs)
   __pyx_t_7 = __pyx_v_self->vecs;
   __Pyx_INCREF(__pyx_t_7);
   if (unlikely(__pyx_t_7 == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 568, __pyx_L1_error)
+    __PYX_ERR(0, 574, __pyx_L1_error)
   }
   __pyx_t_3 = PyList_GET_SIZE(__pyx_t_7); if (unlikely(__pyx_t_3 == (
-(Py_ssize_t)-1))) __PYX_ERR(0, 568, __pyx_L1_error)
+(Py_ssize_t)-1))) __PYX_ERR(0, 574, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_v_self->vlen = __pyx_t_3;
-+569:         if self.vlen < 2:
++575:         if self.vlen < 2:
   __pyx_t_1 = ((__pyx_v_self->vlen < 2) != 0);
   if (unlikely(__pyx_t_1)) {
 /* … */
   }
-+570:             raise ValueError(f'Слишком мало точек для линии. Необходимо
++576:             raise ValueError(f'Слишком мало точек для линии. Необходимо
 больше, чем 1')
     __pyx_t_7 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__15,
-NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 570, __pyx_L1_error)
+NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 576, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_Raise(__pyx_t_7, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __PYX_ERR(0, 570, __pyx_L1_error)
+    __PYX_ERR(0, 576, __pyx_L1_error)
 /* … */
   __pyx_tuple__15 = PyTuple_Pack(1, __pyx_kp_u_1); if (unlikely
-(!__pyx_tuple__15)) __PYX_ERR(0, 570, __pyx_L1_error)
+(!__pyx_tuple__15)) __PYX_ERR(0, 576, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__15);
   __Pyx_GIVEREF(__pyx_tuple__15);
-+571:         self.enclosed = enclosed
++577:         self.enclosed = enclosed
   __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_enclosed); if (unlikely((__pyx_t_1
-== (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 571, __pyx_L1_error)
+== (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 577, __pyx_L1_error)
   __pyx_v_self->enclosed = __pyx_t_1;
-+572:         self.bbox = Rect.bbox(self.vecs)
++578:         self.bbox = Rect.bbox(self.vecs)
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject
 *)__pyx_ptype_7easyvec_8geometry_Rect), __pyx_n_s_bbox); if (unlikely
-(!__pyx_t_2)) __PYX_ERR(0, 572, __pyx_L1_error)
+(!__pyx_t_2)) __PYX_ERR(0, 578, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_9 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_9)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_9);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_7 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_9,
 __pyx_v_self->vecs) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_self->vecs);
   __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-  if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 572, __pyx_L1_error)
+  if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 578, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (!(likely(((__pyx_t_7) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_7,
-__pyx_ptype_7easyvec_8geometry_Rect))))) __PYX_ERR(0, 572, __pyx_L1_error)
+__pyx_ptype_7easyvec_8geometry_Rect))))) __PYX_ERR(0, 578, __pyx_L1_error)
   __Pyx_GIVEREF(__pyx_t_7);
   __Pyx_GOTREF(__pyx_v_self->bbox);
   __Pyx_DECREF(((PyObject *)__pyx_v_self->bbox));
   __pyx_v_self->bbox = ((struct __pyx_obj_7easyvec_8geometry_Rect *)__pyx_t_7);
   __pyx_t_7 = 0;
-&#xA0;573:
-+574:     def __str__(self):
+&#xA0;579:
++580:     def to_dict(self):
+/* Python wrapper */
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_5to_dict(PyObject
+*__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_7easyvec_8geometry_8PolyLine_4to_dict[] =
+"PolyLine.to_dict(self)";
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_5to_dict(PyObject
+*__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("to_dict (wrapper)", 0);
+  __pyx_r = __pyx_pf_7easyvec_8geometry_8PolyLine_4to_dict(((struct
+__pyx_obj_7easyvec_8geometry_PolyLine *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_4to_dict(struct
+__pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self) {
+  PyObject *__pyx_8genexpr1__pyx_v_v = NULL;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("to_dict", 0);
+/* … */
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_AddTraceback("easyvec.geometry.PolyLine.to_dict", __pyx_clineno,
+__pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_v);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
++581:         return {
+  __Pyx_XDECREF(__pyx_r);
++582:             'vecs': [v.to_dict() for v in self.vecs],
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR
+(0, 582, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  { /* enter inner scope */
+    __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 582,
+__pyx_L5_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    if (unlikely(__pyx_v_self->vecs == Py_None)) {
+      PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
+      __PYX_ERR(0, 582, __pyx_L5_error)
+    }
+    __pyx_t_3 = __pyx_v_self->vecs; __Pyx_INCREF(__pyx_t_3); __pyx_t_4 = 0;
+    for (;;) {
+      if (__pyx_t_4 >= PyList_GET_SIZE(__pyx_t_3)) break;
+      #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+      __pyx_t_5 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF
+(__pyx_t_5); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 582,
+__pyx_L5_error)
+      #else
+      __pyx_t_5 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if
+(unlikely(!__pyx_t_5)) __PYX_ERR(0, 582, __pyx_L5_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      #endif
+      __Pyx_XDECREF_SET(__pyx_8genexpr1__pyx_v_v, __pyx_t_5);
+      __pyx_t_5 = 0;
+      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_8genexpr1__pyx_v_v,
+__pyx_n_s_to_dict); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 582, __pyx_L5_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __pyx_t_7 = NULL;
+      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
+        __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
+        if (likely(__pyx_t_7)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
+          __Pyx_INCREF(__pyx_t_7);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_6, function);
+        }
+      }
+      __pyx_t_5 = (__pyx_t_7) ? __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_7)
+: __Pyx_PyObject_CallNoArg(__pyx_t_6);
+      __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
+      if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 582, __pyx_L5_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_5)))
+__PYX_ERR(0, 582, __pyx_L5_error)
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    }
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_v); __pyx_8genexpr1__pyx_v_v = 0;
+    goto __pyx_L8_exit_scope;
+    __pyx_L5_error:;
+    __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_v); __pyx_8genexpr1__pyx_v_v = 0;
+    goto __pyx_L1_error;
+    __pyx_L8_exit_scope:;
+  } /* exit inner scope */
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_vecs, __pyx_t_2) < 0) __PYX_ERR(0,
+582, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
++583:             'enclosed': bool(self.enclosed)
+  __pyx_t_8 = __pyx_v_self->enclosed;
+  __pyx_t_2 = __Pyx_PyBool_FromLong((!(!__pyx_t_8))); if (unlikely(!__pyx_t_2))
+__PYX_ERR(0, 583, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_enclosed, __pyx_t_2) < 0) __PYX_ERR
+(0, 582, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+&#xA0;584:         }
+&#xA0;585:
++586:     def __str__(self):
 /* Python wrapper */
-static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_3__str__(PyObject
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_7__str__(PyObject
 *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_3__str__(PyObject
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_7__str__(PyObject
 *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__str__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_7easyvec_8geometry_8PolyLine_2__str__(((struct
+  __pyx_r = __pyx_pf_7easyvec_8geometry_8PolyLine_6__str__(((struct
 __pyx_obj_7easyvec_8geometry_PolyLine *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_2__str__(struct
+static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_6__str__(struct
 __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self) {
   PyObject *__pyx_v_s = NULL;
-  PyObject *__pyx_7genexpr__pyx_v_v = NULL;
+  PyObject *__pyx_8genexpr2__pyx_v_v = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__str__", 0);
 /* … */
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
@@ -9572,162 +9871,162 @@
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_8);
   __Pyx_AddTraceback("easyvec.geometry.PolyLine.__str__", __pyx_clineno,
 __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_s);
-  __Pyx_XDECREF(__pyx_7genexpr__pyx_v_v);
+  __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_v);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
-+575:         s = [f'({v.x:.2f}, {v.y:.2f})' for v in self.vecs]
++587:         s = [f'({v.x:.2f}, {v.y:.2f})' for v in self.vecs]
   { /* enter inner scope */
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 575,
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 587,
 __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_1);
     if (unlikely(__pyx_v_self->vecs == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-      __PYX_ERR(0, 575, __pyx_L5_error)
+      __PYX_ERR(0, 587, __pyx_L5_error)
     }
     __pyx_t_2 = __pyx_v_self->vecs; __Pyx_INCREF(__pyx_t_2); __pyx_t_3 = 0;
     for (;;) {
       if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_2)) break;
       #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
       __pyx_t_4 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF
-(__pyx_t_4); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 575,
+(__pyx_t_4); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 587,
 __pyx_L5_error)
       #else
       __pyx_t_4 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if
-(unlikely(!__pyx_t_4)) __PYX_ERR(0, 575, __pyx_L5_error)
+(unlikely(!__pyx_t_4)) __PYX_ERR(0, 587, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_4);
       #endif
-      __Pyx_XDECREF_SET(__pyx_7genexpr__pyx_v_v, __pyx_t_4);
+      __Pyx_XDECREF_SET(__pyx_8genexpr2__pyx_v_v, __pyx_t_4);
       __pyx_t_4 = 0;
-      __pyx_t_4 = PyTuple_New(5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 575,
+      __pyx_t_4 = PyTuple_New(5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 587,
 __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_5 = 0;
       __pyx_t_6 = 127;
       __Pyx_INCREF(__pyx_kp_u__16);
       __pyx_t_5 += 1;
       __Pyx_GIVEREF(__pyx_kp_u__16);
       PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_kp_u__16);
-      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_7genexpr__pyx_v_v,
-__pyx_n_s_x); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 575, __pyx_L5_error)
+      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_8genexpr2__pyx_v_v,
+__pyx_n_s_x); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 587, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_7);
       __pyx_t_8 = __Pyx_PyObject_Format(__pyx_t_7, __pyx_kp_u_2f); if (unlikely
-(!__pyx_t_8)) __PYX_ERR(0, 575, __pyx_L5_error)
+(!__pyx_t_8)) __PYX_ERR(0, 587, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __pyx_t_6 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_8) > __pyx_t_6) ?
 __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_8) : __pyx_t_6;
       __pyx_t_5 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_8);
       __Pyx_GIVEREF(__pyx_t_8);
       PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_8);
       __pyx_t_8 = 0;
       __Pyx_INCREF(__pyx_kp_u__4);
       __pyx_t_5 += 2;
       __Pyx_GIVEREF(__pyx_kp_u__4);
       PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_kp_u__4);
-      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_7genexpr__pyx_v_v,
-__pyx_n_s_y); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 575, __pyx_L5_error)
+      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_8genexpr2__pyx_v_v,
+__pyx_n_s_y); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 587, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_8);
       __pyx_t_7 = __Pyx_PyObject_Format(__pyx_t_8, __pyx_kp_u_2f); if (unlikely
-(!__pyx_t_7)) __PYX_ERR(0, 575, __pyx_L5_error)
+(!__pyx_t_7)) __PYX_ERR(0, 587, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __pyx_t_6 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) > __pyx_t_6) ?
 __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) : __pyx_t_6;
       __pyx_t_5 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
       __Pyx_GIVEREF(__pyx_t_7);
       PyTuple_SET_ITEM(__pyx_t_4, 3, __pyx_t_7);
       __pyx_t_7 = 0;
       __Pyx_INCREF(__pyx_kp_u__5);
       __pyx_t_5 += 1;
       __Pyx_GIVEREF(__pyx_kp_u__5);
       PyTuple_SET_ITEM(__pyx_t_4, 4, __pyx_kp_u__5);
       __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_4, 5, __pyx_t_5, __pyx_t_6); if
-(unlikely(!__pyx_t_7)) __PYX_ERR(0, 575, __pyx_L5_error)
+(unlikely(!__pyx_t_7)) __PYX_ERR(0, 587, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_7)))
-__PYX_ERR(0, 575, __pyx_L5_error)
+__PYX_ERR(0, 587, __pyx_L5_error)
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_XDECREF(__pyx_7genexpr__pyx_v_v); __pyx_7genexpr__pyx_v_v = 0;
+    __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_v); __pyx_8genexpr2__pyx_v_v = 0;
     goto __pyx_L8_exit_scope;
     __pyx_L5_error:;
-    __Pyx_XDECREF(__pyx_7genexpr__pyx_v_v); __pyx_7genexpr__pyx_v_v = 0;
+    __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_v); __pyx_8genexpr2__pyx_v_v = 0;
     goto __pyx_L1_error;
     __pyx_L8_exit_scope:;
   } /* exit inner scope */
   __pyx_v_s = __pyx_t_1;
   __pyx_t_1 = 0;
-+576:         s = ', '.join(s)
++588:         s = ', '.join(s)
   __pyx_t_1 = PyUnicode_Join(__pyx_kp_u__4, __pyx_v_s); if (unlikely
-(!__pyx_t_1)) __PYX_ERR(0, 576, __pyx_L1_error)
+(!__pyx_t_1)) __PYX_ERR(0, 588, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF_SET(__pyx_v_s, __pyx_t_1);
   __pyx_t_1 = 0;
-+577:         return f'PolyLine({s})'
++589:         return f'PolyLine({s})'
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 577,
+  __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 589,
 __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_3 = 0;
   __pyx_t_6 = 127;
   __Pyx_INCREF(__pyx_kp_u_PolyLine);
   __pyx_t_3 += 9;
   __Pyx_GIVEREF(__pyx_kp_u_PolyLine);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_kp_u_PolyLine);
   __pyx_t_2 = __Pyx_PyObject_FormatSimple(__pyx_v_s, __pyx_empty_unicode); if
-(unlikely(!__pyx_t_2)) __PYX_ERR(0, 577, __pyx_L1_error)
+(unlikely(!__pyx_t_2)) __PYX_ERR(0, 589, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_6 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_2) > __pyx_t_6) ?
 __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_2) : __pyx_t_6;
   __pyx_t_3 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_2);
   __pyx_t_2 = 0;
   __Pyx_INCREF(__pyx_kp_u__5);
   __pyx_t_3 += 1;
   __Pyx_GIVEREF(__pyx_kp_u__5);
   PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_kp_u__5);
   __pyx_t_2 = __Pyx_PyUnicode_Join(__pyx_t_1, 3, __pyx_t_3, __pyx_t_6); if
-(unlikely(!__pyx_t_2)) __PYX_ERR(0, 577, __pyx_L1_error)
+(unlikely(!__pyx_t_2)) __PYX_ERR(0, 589, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
-&#xA0;578:
-+579:     def __repr__(self):
+&#xA0;590:
++591:     def __repr__(self):
 /* Python wrapper */
-static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_5__repr__(PyObject
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_9__repr__(PyObject
 *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_5__repr__(PyObject
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_9__repr__(PyObject
 *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__repr__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_7easyvec_8geometry_8PolyLine_4__repr__(((struct
+  __pyx_r = __pyx_pf_7easyvec_8geometry_8PolyLine_8__repr__(((struct
 __pyx_obj_7easyvec_8geometry_PolyLine *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_4__repr__(struct
+static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_8__repr__(struct
 __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self) {
   PyObject *__pyx_v_s = NULL;
-  PyObject *__pyx_8genexpr1__pyx_v_v = NULL;
+  PyObject *__pyx_8genexpr3__pyx_v_v = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__repr__", 0);
 /* … */
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
@@ -9736,158 +10035,158 @@
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_8);
   __Pyx_AddTraceback("easyvec.geometry.PolyLine.__repr__", __pyx_clineno,
 __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_s);
-  __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_v);
+  __Pyx_XDECREF(__pyx_8genexpr3__pyx_v_v);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
-+580:         s = [f'({v.x}, {v.y})' for v in self.vecs]
++592:         s = [f'({v.x}, {v.y})' for v in self.vecs]
   { /* enter inner scope */
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 580,
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 592,
 __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_1);
     if (unlikely(__pyx_v_self->vecs == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-      __PYX_ERR(0, 580, __pyx_L5_error)
+      __PYX_ERR(0, 592, __pyx_L5_error)
     }
     __pyx_t_2 = __pyx_v_self->vecs; __Pyx_INCREF(__pyx_t_2); __pyx_t_3 = 0;
     for (;;) {
       if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_2)) break;
       #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
       __pyx_t_4 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF
-(__pyx_t_4); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 580,
+(__pyx_t_4); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 592,
 __pyx_L5_error)
       #else
       __pyx_t_4 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if
-(unlikely(!__pyx_t_4)) __PYX_ERR(0, 580, __pyx_L5_error)
+(unlikely(!__pyx_t_4)) __PYX_ERR(0, 592, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_4);
       #endif
-      __Pyx_XDECREF_SET(__pyx_8genexpr1__pyx_v_v, __pyx_t_4);
+      __Pyx_XDECREF_SET(__pyx_8genexpr3__pyx_v_v, __pyx_t_4);
       __pyx_t_4 = 0;
-      __pyx_t_4 = PyTuple_New(5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 580,
+      __pyx_t_4 = PyTuple_New(5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 592,
 __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_5 = 0;
       __pyx_t_6 = 127;
       __Pyx_INCREF(__pyx_kp_u__16);
       __pyx_t_5 += 1;
       __Pyx_GIVEREF(__pyx_kp_u__16);
       PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_kp_u__16);
-      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_8genexpr1__pyx_v_v,
-__pyx_n_s_x); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 580, __pyx_L5_error)
+      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_8genexpr3__pyx_v_v,
+__pyx_n_s_x); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 592, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_7);
       __pyx_t_8 = __Pyx_PyObject_FormatSimple(__pyx_t_7, __pyx_empty_unicode);
-if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 580, __pyx_L5_error)
+if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 592, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __pyx_t_6 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_8) > __pyx_t_6) ?
 __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_8) : __pyx_t_6;
       __pyx_t_5 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_8);
       __Pyx_GIVEREF(__pyx_t_8);
       PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_8);
       __pyx_t_8 = 0;
       __Pyx_INCREF(__pyx_kp_u__4);
       __pyx_t_5 += 2;
       __Pyx_GIVEREF(__pyx_kp_u__4);
       PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_kp_u__4);
-      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_8genexpr1__pyx_v_v,
-__pyx_n_s_y); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 580, __pyx_L5_error)
+      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_8genexpr3__pyx_v_v,
+__pyx_n_s_y); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 592, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_8);
       __pyx_t_7 = __Pyx_PyObject_FormatSimple(__pyx_t_8, __pyx_empty_unicode);
-if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 580, __pyx_L5_error)
+if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 592, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __pyx_t_6 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) > __pyx_t_6) ?
 __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) : __pyx_t_6;
       __pyx_t_5 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
       __Pyx_GIVEREF(__pyx_t_7);
       PyTuple_SET_ITEM(__pyx_t_4, 3, __pyx_t_7);
       __pyx_t_7 = 0;
       __Pyx_INCREF(__pyx_kp_u__5);
       __pyx_t_5 += 1;
       __Pyx_GIVEREF(__pyx_kp_u__5);
       PyTuple_SET_ITEM(__pyx_t_4, 4, __pyx_kp_u__5);
       __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_4, 5, __pyx_t_5, __pyx_t_6); if
-(unlikely(!__pyx_t_7)) __PYX_ERR(0, 580, __pyx_L5_error)
+(unlikely(!__pyx_t_7)) __PYX_ERR(0, 592, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_7)))
-__PYX_ERR(0, 580, __pyx_L5_error)
+__PYX_ERR(0, 592, __pyx_L5_error)
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_v); __pyx_8genexpr1__pyx_v_v = 0;
+    __Pyx_XDECREF(__pyx_8genexpr3__pyx_v_v); __pyx_8genexpr3__pyx_v_v = 0;
     goto __pyx_L8_exit_scope;
     __pyx_L5_error:;
-    __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_v); __pyx_8genexpr1__pyx_v_v = 0;
+    __Pyx_XDECREF(__pyx_8genexpr3__pyx_v_v); __pyx_8genexpr3__pyx_v_v = 0;
     goto __pyx_L1_error;
     __pyx_L8_exit_scope:;
   } /* exit inner scope */
   __pyx_v_s = __pyx_t_1;
   __pyx_t_1 = 0;
-+581:         s = ', '.join(s)
++593:         s = ', '.join(s)
   __pyx_t_1 = PyUnicode_Join(__pyx_kp_u__4, __pyx_v_s); if (unlikely
-(!__pyx_t_1)) __PYX_ERR(0, 581, __pyx_L1_error)
+(!__pyx_t_1)) __PYX_ERR(0, 593, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF_SET(__pyx_v_s, __pyx_t_1);
   __pyx_t_1 = 0;
-+582:         return f'PolyLine(vecs=[{s}], enclosed={self.enclosed})'
++594:         return f'PolyLine(vecs=[{s}], enclosed={self.enclosed})'
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyTuple_New(5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 582,
+  __pyx_t_1 = PyTuple_New(5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 594,
 __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_3 = 0;
   __pyx_t_6 = 127;
   __Pyx_INCREF(__pyx_kp_u_PolyLine_vecs);
   __pyx_t_3 += 15;
   __Pyx_GIVEREF(__pyx_kp_u_PolyLine_vecs);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_kp_u_PolyLine_vecs);
   __pyx_t_2 = __Pyx_PyObject_FormatSimple(__pyx_v_s, __pyx_empty_unicode); if
-(unlikely(!__pyx_t_2)) __PYX_ERR(0, 582, __pyx_L1_error)
+(unlikely(!__pyx_t_2)) __PYX_ERR(0, 594, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_6 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_2) > __pyx_t_6) ?
 __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_2) : __pyx_t_6;
   __pyx_t_3 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_2);
   __pyx_t_2 = 0;
   __Pyx_INCREF(__pyx_kp_u_enclosed_2);
   __pyx_t_3 += 12;
   __Pyx_GIVEREF(__pyx_kp_u_enclosed_2);
   PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_kp_u_enclosed_2);
   __pyx_t_2 = __Pyx_PyUnicode_FromBInt_int(__pyx_v_self->enclosed); if
-(unlikely(!__pyx_t_2)) __PYX_ERR(0, 582, __pyx_L1_error)
+(unlikely(!__pyx_t_2)) __PYX_ERR(0, 594, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_1, 3, __pyx_t_2);
   __pyx_t_2 = 0;
   __Pyx_INCREF(__pyx_kp_u__5);
   __pyx_t_3 += 1;
   __Pyx_GIVEREF(__pyx_kp_u__5);
   PyTuple_SET_ITEM(__pyx_t_1, 4, __pyx_kp_u__5);
   __pyx_t_2 = __Pyx_PyUnicode_Join(__pyx_t_1, 5, __pyx_t_3, __pyx_t_6); if
-(unlikely(!__pyx_t_2)) __PYX_ERR(0, 582, __pyx_L1_error)
+(unlikely(!__pyx_t_2)) __PYX_ERR(0, 594, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
-&#xA0;583:
-&#xA0;584:     @cython.nonecheck(False)
-&#xA0;585:     @cython.boundscheck(False)
-&#xA0;586:     @cython.wraparound(False)
-+587:     cpdef list intersect_general(self, Vec2 p1, Vec2 p2, real f_low, real
+&#xA0;595:
+&#xA0;596:     @cython.nonecheck(False)
+&#xA0;597:     @cython.boundscheck(False)
+&#xA0;598:     @cython.wraparound(False)
++599:     cpdef list intersect_general(self, Vec2 p1, Vec2 p2, real f_low, real
 f_high, bint sortreduce=True):
-static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_7intersect_general
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_11intersect_general
 (PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_f_7easyvec_8geometry_8PolyLine_intersect_general(struct
 __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self, struct
 __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p1, struct
 __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p2, __pyx_t_7easyvec_7vectors_real
 __pyx_v_f_low, __pyx_t_7easyvec_7vectors_real __pyx_v_f_high, CYTHON_UNUSED int
 __pyx_skip_dispatch, struct
@@ -9925,20 +10224,20 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_v_cr);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_7intersect_general
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_11intersect_general
 (PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_7easyvec_8geometry_8PolyLine_6intersect_general[] =
+static char __pyx_doc_7easyvec_8geometry_8PolyLine_10intersect_general[] =
 "PolyLine.intersect_general(self, Vec2 p1, Vec2 p2, real f_low, real f_high,
 bool sortreduce=True) -> list";
-static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_7intersect_general
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_11intersect_general
 (PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p1 = 0;
   struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p2 = 0;
   __pyx_t_7easyvec_7vectors_real __pyx_v_f_low;
   __pyx_t_7easyvec_7vectors_real __pyx_v_f_high;
   int __pyx_v_sortreduce;
   PyObject *__pyx_r = 0;
@@ -9973,43 +10272,43 @@
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds,
 __pyx_n_s_p2)) != 0)) kw_args--;
         else {
           __Pyx_RaiseArgtupleInvalid("intersect_general", 0, 4, 5, 1);
-__PYX_ERR(0, 587, __pyx_L3_error)
+__PYX_ERR(0, 599, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds,
 __pyx_n_s_f_low)) != 0)) kw_args--;
         else {
           __Pyx_RaiseArgtupleInvalid("intersect_general", 0, 4, 5, 2);
-__PYX_ERR(0, 587, __pyx_L3_error)
+__PYX_ERR(0, 599, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds,
 __pyx_n_s_f_high)) != 0)) kw_args--;
         else {
           __Pyx_RaiseArgtupleInvalid("intersect_general", 0, 4, 5, 3);
-__PYX_ERR(0, 587, __pyx_L3_error)
+__PYX_ERR(0, 599, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds,
 __pyx_n_s_sortreduce);
           if (value) { values[4] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
         if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames,
-0, values, pos_args, "intersect_general") < 0)) __PYX_ERR(0, 587,
+0, values, pos_args, "intersect_general") < 0)) __PYX_ERR(0, 599,
 __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
@@ -10019,71 +10318,71 @@
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_p1 = ((struct __pyx_obj_7easyvec_7vectors_Vec2 *)values[0]);
     __pyx_v_p2 = ((struct __pyx_obj_7easyvec_7vectors_Vec2 *)values[1]);
     __pyx_v_f_low = __pyx_PyFloat_AsDouble(values[2]); if (unlikely(
-(__pyx_v_f_low == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 587,
+(__pyx_v_f_low == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 599,
 __pyx_L3_error)
     __pyx_v_f_high = __pyx_PyFloat_AsDouble(values[3]); if (unlikely(
-(__pyx_v_f_high == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 587,
+(__pyx_v_f_high == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 599,
 __pyx_L3_error)
     if (values[4]) {
       __pyx_v_sortreduce = __Pyx_PyObject_IsTrue(values[4]); if (unlikely(
-(__pyx_v_sortreduce == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 587,
+(__pyx_v_sortreduce == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 599,
 __pyx_L3_error)
     } else {
       __pyx_v_sortreduce = ((int)1);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("intersect_general", 0, 4, 5, PyTuple_GET_SIZE
-(__pyx_args)); __PYX_ERR(0, 587, __pyx_L3_error)
+(__pyx_args)); __PYX_ERR(0, 599, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("easyvec.geometry.PolyLine.intersect_general",
 __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_p1),
-__pyx_ptype_7easyvec_7vectors_Vec2, 1, "p1", 0))) __PYX_ERR(0, 587,
+__pyx_ptype_7easyvec_7vectors_Vec2, 1, "p1", 0))) __PYX_ERR(0, 599,
 __pyx_L1_error)
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_p2),
-__pyx_ptype_7easyvec_7vectors_Vec2, 1, "p2", 0))) __PYX_ERR(0, 587,
+__pyx_ptype_7easyvec_7vectors_Vec2, 1, "p2", 0))) __PYX_ERR(0, 599,
 __pyx_L1_error)
-  __pyx_r = __pyx_pf_7easyvec_8geometry_8PolyLine_6intersect_general(((struct
+  __pyx_r = __pyx_pf_7easyvec_8geometry_8PolyLine_10intersect_general(((struct
 __pyx_obj_7easyvec_8geometry_PolyLine *)__pyx_v_self), __pyx_v_p1, __pyx_v_p2,
 __pyx_v_f_low, __pyx_v_f_high, __pyx_v_sortreduce);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_6intersect_general
+static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_10intersect_general
 (struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self, struct
 __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p1, struct
 __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p2, __pyx_t_7easyvec_7vectors_real
 __pyx_v_f_low, __pyx_t_7easyvec_7vectors_real __pyx_v_f_high, int
 __pyx_v_sortreduce) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("intersect_general", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2.__pyx_n = 1;
   __pyx_t_2.sortreduce = __pyx_v_sortreduce;
   __pyx_t_1 = __pyx_vtabptr_7easyvec_8geometry_PolyLine->intersect_general
 (__pyx_v_self, __pyx_v_p1, __pyx_v_p2, __pyx_v_f_low, __pyx_v_f_high, 1,
-&__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 587, __pyx_L1_error)
+&__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 599, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -10092,75 +10391,75 @@
 __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
-+588:         cdef list res = []
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 588,
++600:         cdef list res = []
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 600,
 __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_res = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
-+589:         if self.bbox.intersect_general(p1, p2, f_low, f_high) is None:
++601:         if self.bbox.intersect_general(p1, p2, f_low, f_high) is None:
   __pyx_t_1 = ((PyObject *)__pyx_f_7easyvec_8geometry_4Rect_intersect_general
 (__pyx_v_self->bbox, __pyx_v_p1, __pyx_v_p2, __pyx_v_f_low, __pyx_v_f_high, 0,
-NULL)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 589, __pyx_L1_error)
+NULL)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 601, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = (__pyx_t_1 == Py_None);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 /* … */
   }
-+590:             return res
++602:             return res
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_v_res);
     __pyx_r = __pyx_v_res;
     goto __pyx_L0;
-&#xA0;591:         cdef int i
-&#xA0;592:         cdef Vec2 v1, v2, v_cr
-&#xA0;593:         cdef bint inter
-&#xA0;594:         cdef real t1, t2
-+595:         v1 = <Vec2>(self.vecs[0])
+&#xA0;603:         cdef int i
+&#xA0;604:         cdef Vec2 v1, v2, v_cr
+&#xA0;605:         cdef bint inter
+&#xA0;606:         cdef real t1, t2
++607:         v1 = <Vec2>(self.vecs[0])
   if (unlikely(__pyx_v_self->vecs == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 595, __pyx_L1_error)
+    __PYX_ERR(0, 607, __pyx_L1_error)
   }
   __pyx_t_1 = PyList_GET_ITEM(__pyx_v_self->vecs, 0);
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v_v1 = ((struct __pyx_obj_7easyvec_7vectors_Vec2 *)__pyx_t_1);
   __pyx_t_1 = 0;
-+596:         for i in range(1, self.vlen):
++608:         for i in range(1, self.vlen):
   __pyx_t_4 = __pyx_v_self->vlen;
   __pyx_t_5 = __pyx_t_4;
   for (__pyx_t_6 = 1; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
     __pyx_v_i = __pyx_t_6;
-+597:             v2 = <Vec2>(self.vecs[i])
++609:             v2 = <Vec2>(self.vecs[i])
     if (unlikely(__pyx_v_self->vecs == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not
 subscriptable");
-      __PYX_ERR(0, 597, __pyx_L1_error)
+      __PYX_ERR(0, 609, __pyx_L1_error)
     }
     __pyx_t_1 = PyList_GET_ITEM(__pyx_v_self->vecs, __pyx_v_i);
     __Pyx_INCREF(__pyx_t_1);
     __Pyx_XDECREF_SET(__pyx_v_v2, ((struct __pyx_obj_7easyvec_7vectors_Vec2
 *)__pyx_t_1));
     __pyx_t_1 = 0;
-+598:             inter, t1, t2 = _intersect_ts(p1, p2, v1, v2)
++610:             inter, t1, t2 = _intersect_ts(p1, p2, v1, v2)
     __pyx_t_7 = __pyx_f_7easyvec_8geometry__intersect_ts(__pyx_v_p1,
 __pyx_v_p2, __pyx_v_v1, __pyx_v_v2, 0);
     __pyx_t_3 = __pyx_t_7.f0;
     __pyx_t_8 = __pyx_t_7.f1;
     __pyx_t_9 = __pyx_t_7.f2;
     __pyx_v_inter = __pyx_t_3;
     __pyx_v_t1 = __pyx_t_8;
     __pyx_v_t2 = __pyx_t_9;
-+599:             if inter and (0.0 <= t2 <= 1.0) and (f_low <= t1 <= f_high):
++611:             if inter and (0.0 <= t2 <= 1.0) and (f_low <= t1 <= f_high):
     __pyx_t_2 = (__pyx_v_inter != 0);
     if (__pyx_t_2) {
     } else {
       __pyx_t_3 = __pyx_t_2;
       goto __pyx_L7_bool_binop_done;
     }
     __pyx_t_2 = (0.0 <= __pyx_v_t2);
@@ -10179,69 +10478,69 @@
     }
     __pyx_t_2 = (__pyx_t_10 != 0);
     __pyx_t_3 = __pyx_t_2;
     __pyx_L7_bool_binop_done:;
     if (__pyx_t_3) {
 /* … */
     }
-+600:                 v_cr = p1.add( p2.sub(p1).mul_num(t1) )
++612:                 v_cr = p1.add( p2.sub(p1).mul_num(t1) )
       __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_7easyvec_7vectors_Vec2
 *)__pyx_v_p2->__pyx_vtab)->sub(__pyx_v_p2, __pyx_v_p1, 0)); if (unlikely
-(!__pyx_t_1)) __PYX_ERR(0, 600, __pyx_L1_error)
+(!__pyx_t_1)) __PYX_ERR(0, 612, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_t_11 = ((PyObject *)((struct
 __pyx_vtabstruct_7easyvec_7vectors_Vec2 *)((struct
 __pyx_obj_7easyvec_7vectors_Vec2 *)__pyx_t_1)->__pyx_vtab)->mul_num(((struct
 __pyx_obj_7easyvec_7vectors_Vec2 *)__pyx_t_1), __pyx_v_t1, 0)); if (unlikely
-(!__pyx_t_11)) __PYX_ERR(0, 600, __pyx_L1_error)
+(!__pyx_t_11)) __PYX_ERR(0, 612, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_7easyvec_7vectors_Vec2
 *)__pyx_v_p1->__pyx_vtab)->add(__pyx_v_p1, ((struct
 __pyx_obj_7easyvec_7vectors_Vec2 *)__pyx_t_11), 0)); if (unlikely(!__pyx_t_1))
-__PYX_ERR(0, 600, __pyx_L1_error)
+__PYX_ERR(0, 612, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
       __Pyx_XDECREF_SET(__pyx_v_v_cr, ((struct __pyx_obj_7easyvec_7vectors_Vec2
 *)__pyx_t_1));
       __pyx_t_1 = 0;
-+601:                 res.append(v_cr)
++613:                 res.append(v_cr)
       __pyx_t_12 = __Pyx_PyList_Append(__pyx_v_res, ((PyObject
-*)__pyx_v_v_cr)); if (unlikely(__pyx_t_12 == ((int)-1))) __PYX_ERR(0, 601,
+*)__pyx_v_v_cr)); if (unlikely(__pyx_t_12 == ((int)-1))) __PYX_ERR(0, 613,
 __pyx_L1_error)
-+602:             v1 = v2
++614:             v1 = v2
     __Pyx_INCREF(((PyObject *)__pyx_v_v2));
     __Pyx_DECREF_SET(__pyx_v_v1, __pyx_v_v2);
   }
-+603:         if self.enclosed:
++615:         if self.enclosed:
   __pyx_t_3 = (__pyx_v_self->enclosed != 0);
   if (__pyx_t_3) {
 /* … */
   }
-+604:             v2 = <Vec2>(self.vecs[0])
++616:             v2 = <Vec2>(self.vecs[0])
     if (unlikely(__pyx_v_self->vecs == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not
 subscriptable");
-      __PYX_ERR(0, 604, __pyx_L1_error)
+      __PYX_ERR(0, 616, __pyx_L1_error)
     }
     __pyx_t_1 = PyList_GET_ITEM(__pyx_v_self->vecs, 0);
     __Pyx_INCREF(__pyx_t_1);
     __Pyx_XDECREF_SET(__pyx_v_v2, ((struct __pyx_obj_7easyvec_7vectors_Vec2
 *)__pyx_t_1));
     __pyx_t_1 = 0;
-+605:             inter, t1, t2 = _intersect_ts(p1, p2, v1, v2)
++617:             inter, t1, t2 = _intersect_ts(p1, p2, v1, v2)
     __pyx_t_7 = __pyx_f_7easyvec_8geometry__intersect_ts(__pyx_v_p1,
 __pyx_v_p2, __pyx_v_v1, __pyx_v_v2, 0);
     __pyx_t_3 = __pyx_t_7.f0;
     __pyx_t_9 = __pyx_t_7.f1;
     __pyx_t_8 = __pyx_t_7.f2;
     __pyx_v_inter = __pyx_t_3;
     __pyx_v_t1 = __pyx_t_9;
     __pyx_v_t2 = __pyx_t_8;
-+606:             if inter and (0.0 <= t2 <= 1.0) and (f_low <= t1 <= f_high):
++618:             if inter and (0.0 <= t2 <= 1.0) and (f_low <= t1 <= f_high):
     __pyx_t_2 = (__pyx_v_inter != 0);
     if (__pyx_t_2) {
     } else {
       __pyx_t_3 = __pyx_t_2;
       goto __pyx_L12_bool_binop_done;
     }
     __pyx_t_2 = (0.0 <= __pyx_v_t2);
@@ -10260,63 +10559,63 @@
     }
     __pyx_t_2 = (__pyx_t_10 != 0);
     __pyx_t_3 = __pyx_t_2;
     __pyx_L12_bool_binop_done:;
     if (__pyx_t_3) {
 /* … */
     }
-+607:                 v_cr = p1.add( p2.sub(p1).mul_num(t1) )
++619:                 v_cr = p1.add( p2.sub(p1).mul_num(t1) )
       __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_7easyvec_7vectors_Vec2
 *)__pyx_v_p2->__pyx_vtab)->sub(__pyx_v_p2, __pyx_v_p1, 0)); if (unlikely
-(!__pyx_t_1)) __PYX_ERR(0, 607, __pyx_L1_error)
+(!__pyx_t_1)) __PYX_ERR(0, 619, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_t_11 = ((PyObject *)((struct
 __pyx_vtabstruct_7easyvec_7vectors_Vec2 *)((struct
 __pyx_obj_7easyvec_7vectors_Vec2 *)__pyx_t_1)->__pyx_vtab)->mul_num(((struct
 __pyx_obj_7easyvec_7vectors_Vec2 *)__pyx_t_1), __pyx_v_t1, 0)); if (unlikely
-(!__pyx_t_11)) __PYX_ERR(0, 607, __pyx_L1_error)
+(!__pyx_t_11)) __PYX_ERR(0, 619, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_7easyvec_7vectors_Vec2
 *)__pyx_v_p1->__pyx_vtab)->add(__pyx_v_p1, ((struct
 __pyx_obj_7easyvec_7vectors_Vec2 *)__pyx_t_11), 0)); if (unlikely(!__pyx_t_1))
-__PYX_ERR(0, 607, __pyx_L1_error)
+__PYX_ERR(0, 619, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
       __Pyx_XDECREF_SET(__pyx_v_v_cr, ((struct __pyx_obj_7easyvec_7vectors_Vec2
 *)__pyx_t_1));
       __pyx_t_1 = 0;
-+608:                 res.append(v_cr)
++620:                 res.append(v_cr)
       __pyx_t_12 = __Pyx_PyList_Append(__pyx_v_res, ((PyObject
-*)__pyx_v_v_cr)); if (unlikely(__pyx_t_12 == ((int)-1))) __PYX_ERR(0, 608,
+*)__pyx_v_v_cr)); if (unlikely(__pyx_t_12 == ((int)-1))) __PYX_ERR(0, 620,
 __pyx_L1_error)
-+609:         if sortreduce:
++621:         if sortreduce:
   __pyx_t_3 = (__pyx_v_sortreduce != 0);
   if (__pyx_t_3) {
 /* … */
   }
-+610:             return _sortreduce_by_distance(res, p1)
++622:             return _sortreduce_by_distance(res, p1)
     __Pyx_XDECREF(__pyx_r);
     __pyx_t_1 = __pyx_f_7easyvec_8geometry__sortreduce_by_distance(__pyx_v_res,
-__pyx_v_p1, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 610, __pyx_L1_error)
+__pyx_v_p1, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 622, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_r = ((PyObject*)__pyx_t_1);
     __pyx_t_1 = 0;
     goto __pyx_L0;
-+611:         return res
++623:         return res
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_res);
   __pyx_r = __pyx_v_res;
   goto __pyx_L0;
-&#xA0;612:
-&#xA0;613:     @cython.nonecheck(False)
-+614:     cpdef list intersect_line(self, Vec2 p1, Vec2 p2, bint
+&#xA0;624:
+&#xA0;625:     @cython.nonecheck(False)
++626:     cpdef list intersect_line(self, Vec2 p1, Vec2 p2, bint
 sortreduce=True):
-static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_9intersect_line(PyObject
-*__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_13intersect_line
+(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_f_7easyvec_8geometry_8PolyLine_intersect_line(struct
 __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self, struct
 __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p1, struct
 __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p2, CYTHON_UNUSED int
 __pyx_skip_dispatch, struct
 __pyx_opt_args_7easyvec_8geometry_8PolyLine_intersect_line
 *__pyx_optional_args) {
@@ -10339,21 +10638,21 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_9intersect_line(PyObject
-*__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_7easyvec_8geometry_8PolyLine_8intersect_line[] =
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_13intersect_line
+(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_7easyvec_8geometry_8PolyLine_12intersect_line[] =
 "PolyLine.intersect_line(self, Vec2 p1, Vec2 p2, bool sortreduce=True) -
 > list";
-static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_9intersect_line(PyObject
-*__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_13intersect_line
+(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p1 = 0;
   struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p2 = 0;
   int __pyx_v_sortreduce;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("intersect_line (wrapper)", 0);
   {
@@ -10381,27 +10680,27 @@
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds,
 __pyx_n_s_p2)) != 0)) kw_args--;
         else {
           __Pyx_RaiseArgtupleInvalid("intersect_line", 0, 2, 3, 1); __PYX_ERR
-(0, 614, __pyx_L3_error)
+(0, 626, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds,
 __pyx_n_s_sortreduce);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
         if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames,
-0, values, pos_args, "intersect_line") < 0)) __PYX_ERR(0, 614, __pyx_L3_error)
+0, values, pos_args, "intersect_line") < 0)) __PYX_ERR(0, 626, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
@@ -10409,62 +10708,62 @@
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_p1 = ((struct __pyx_obj_7easyvec_7vectors_Vec2 *)values[0]);
     __pyx_v_p2 = ((struct __pyx_obj_7easyvec_7vectors_Vec2 *)values[1]);
     if (values[2]) {
       __pyx_v_sortreduce = __Pyx_PyObject_IsTrue(values[2]); if (unlikely(
-(__pyx_v_sortreduce == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 614,
+(__pyx_v_sortreduce == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 626,
 __pyx_L3_error)
     } else {
       __pyx_v_sortreduce = ((int)1);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("intersect_line", 0, 2, 3, PyTuple_GET_SIZE
-(__pyx_args)); __PYX_ERR(0, 614, __pyx_L3_error)
+(__pyx_args)); __PYX_ERR(0, 626, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("easyvec.geometry.PolyLine.intersect_line", __pyx_clineno,
 __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_p1),
-__pyx_ptype_7easyvec_7vectors_Vec2, 1, "p1", 0))) __PYX_ERR(0, 614,
+__pyx_ptype_7easyvec_7vectors_Vec2, 1, "p1", 0))) __PYX_ERR(0, 626,
 __pyx_L1_error)
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_p2),
-__pyx_ptype_7easyvec_7vectors_Vec2, 1, "p2", 0))) __PYX_ERR(0, 614,
+__pyx_ptype_7easyvec_7vectors_Vec2, 1, "p2", 0))) __PYX_ERR(0, 626,
 __pyx_L1_error)
-  __pyx_r = __pyx_pf_7easyvec_8geometry_8PolyLine_8intersect_line(((struct
+  __pyx_r = __pyx_pf_7easyvec_8geometry_8PolyLine_12intersect_line(((struct
 __pyx_obj_7easyvec_8geometry_PolyLine *)__pyx_v_self), __pyx_v_p1, __pyx_v_p2,
 __pyx_v_sortreduce);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_8intersect_line(struct
+static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_12intersect_line(struct
 __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self, struct
 __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p1, struct
 __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p2, int __pyx_v_sortreduce) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("intersect_line", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2.__pyx_n = 1;
   __pyx_t_2.sortreduce = __pyx_v_sortreduce;
   __pyx_t_1 = __pyx_vtabptr_7easyvec_8geometry_PolyLine->intersect_line
 (__pyx_v_self, __pyx_v_p1, __pyx_v_p2, 1, &__pyx_t_2); if (unlikely
-(!__pyx_t_1)) __PYX_ERR(0, 614, __pyx_L1_error)
+(!__pyx_t_1)) __PYX_ERR(0, 626, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -10473,32 +10772,32 @@
 __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
-+615:         return self.intersect_general(p1, p2, MINUS_BIG_REAL, BIG_REAL,
++627:         return self.intersect_general(p1, p2, MINUS_BIG_REAL, BIG_REAL,
 sortreduce)
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2.__pyx_n = 1;
   __pyx_t_2.sortreduce = __pyx_v_sortreduce;
   __pyx_t_1 = __pyx_f_7easyvec_8geometry_8PolyLine_intersect_general
 (__pyx_v_self, __pyx_v_p1, __pyx_v_p2,
 __pyx_v_7easyvec_7vectors_MINUS_BIG_REAL, __pyx_v_7easyvec_7vectors_BIG_REAL,
-0, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 615, __pyx_L1_error)
+0, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 627, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
   goto __pyx_L0;
-&#xA0;616:
-&#xA0;617:     @cython.nonecheck(False)
-+618:     cpdef list intersect_ray(self, Vec2 p1, Vec2 p2, bint
+&#xA0;628:
+&#xA0;629:     @cython.nonecheck(False)
++630:     cpdef list intersect_ray(self, Vec2 p1, Vec2 p2, bint
 sortreduce=True):
-static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_11intersect_ray(PyObject
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_15intersect_ray(PyObject
 *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_f_7easyvec_8geometry_8PolyLine_intersect_ray(struct
 __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self, struct
 __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p1, struct
 __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p2, CYTHON_UNUSED int
 __pyx_skip_dispatch, struct
 __pyx_opt_args_7easyvec_8geometry_8PolyLine_intersect_ray *__pyx_optional_args)
@@ -10522,19 +10821,19 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_11intersect_ray(PyObject
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_15intersect_ray(PyObject
 *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_7easyvec_8geometry_8PolyLine_10intersect_ray[] =
+static char __pyx_doc_7easyvec_8geometry_8PolyLine_14intersect_ray[] =
 "PolyLine.intersect_ray(self, Vec2 p1, Vec2 p2, bool sortreduce=True) -> list";
-static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_11intersect_ray(PyObject
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_15intersect_ray(PyObject
 *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p1 = 0;
   struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p2 = 0;
   int __pyx_v_sortreduce;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("intersect_ray (wrapper)", 0);
@@ -10563,27 +10862,27 @@
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds,
 __pyx_n_s_p2)) != 0)) kw_args--;
         else {
           __Pyx_RaiseArgtupleInvalid("intersect_ray", 0, 2, 3, 1); __PYX_ERR(0,
-618, __pyx_L3_error)
+630, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds,
 __pyx_n_s_sortreduce);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
         if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames,
-0, values, pos_args, "intersect_ray") < 0)) __PYX_ERR(0, 618, __pyx_L3_error)
+0, values, pos_args, "intersect_ray") < 0)) __PYX_ERR(0, 630, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
@@ -10591,62 +10890,62 @@
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_p1 = ((struct __pyx_obj_7easyvec_7vectors_Vec2 *)values[0]);
     __pyx_v_p2 = ((struct __pyx_obj_7easyvec_7vectors_Vec2 *)values[1]);
     if (values[2]) {
       __pyx_v_sortreduce = __Pyx_PyObject_IsTrue(values[2]); if (unlikely(
-(__pyx_v_sortreduce == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 618,
+(__pyx_v_sortreduce == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 630,
 __pyx_L3_error)
     } else {
       __pyx_v_sortreduce = ((int)1);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("intersect_ray", 0, 2, 3, PyTuple_GET_SIZE
-(__pyx_args)); __PYX_ERR(0, 618, __pyx_L3_error)
+(__pyx_args)); __PYX_ERR(0, 630, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("easyvec.geometry.PolyLine.intersect_ray", __pyx_clineno,
 __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_p1),
-__pyx_ptype_7easyvec_7vectors_Vec2, 1, "p1", 0))) __PYX_ERR(0, 618,
+__pyx_ptype_7easyvec_7vectors_Vec2, 1, "p1", 0))) __PYX_ERR(0, 630,
 __pyx_L1_error)
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_p2),
-__pyx_ptype_7easyvec_7vectors_Vec2, 1, "p2", 0))) __PYX_ERR(0, 618,
+__pyx_ptype_7easyvec_7vectors_Vec2, 1, "p2", 0))) __PYX_ERR(0, 630,
 __pyx_L1_error)
-  __pyx_r = __pyx_pf_7easyvec_8geometry_8PolyLine_10intersect_ray(((struct
+  __pyx_r = __pyx_pf_7easyvec_8geometry_8PolyLine_14intersect_ray(((struct
 __pyx_obj_7easyvec_8geometry_PolyLine *)__pyx_v_self), __pyx_v_p1, __pyx_v_p2,
 __pyx_v_sortreduce);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_10intersect_ray(struct
+static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_14intersect_ray(struct
 __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self, struct
 __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p1, struct
 __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p2, int __pyx_v_sortreduce) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("intersect_ray", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2.__pyx_n = 1;
   __pyx_t_2.sortreduce = __pyx_v_sortreduce;
   __pyx_t_1 = __pyx_vtabptr_7easyvec_8geometry_PolyLine->intersect_ray
 (__pyx_v_self, __pyx_v_p1, __pyx_v_p2, 1, &__pyx_t_2); if (unlikely
-(!__pyx_t_1)) __PYX_ERR(0, 618, __pyx_L1_error)
+(!__pyx_t_1)) __PYX_ERR(0, 630, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -10655,30 +10954,30 @@
 __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
-+619:         return self.intersect_general(p1, p2, 0.0, BIG_REAL, sortreduce)
++631:         return self.intersect_general(p1, p2, 0.0, BIG_REAL, sortreduce)
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2.__pyx_n = 1;
   __pyx_t_2.sortreduce = __pyx_v_sortreduce;
   __pyx_t_1 = __pyx_f_7easyvec_8geometry_8PolyLine_intersect_general
 (__pyx_v_self, __pyx_v_p1, __pyx_v_p2, 0.0, __pyx_v_7easyvec_7vectors_BIG_REAL,
-0, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 619, __pyx_L1_error)
+0, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 631, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
   goto __pyx_L0;
-&#xA0;620:
-&#xA0;621:     @cython.nonecheck(False)
-+622:     cpdef list intersect_segment(self, Vec2 p1, Vec2 p2, bint
+&#xA0;632:
+&#xA0;633:     @cython.nonecheck(False)
++634:     cpdef list intersect_segment(self, Vec2 p1, Vec2 p2, bint
 sortreduce=True):
-static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_13intersect_segment
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_17intersect_segment
 (PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_f_7easyvec_8geometry_8PolyLine_intersect_segment(struct
 __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self, struct
 __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p1, struct
 __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p2, CYTHON_UNUSED int
 __pyx_skip_dispatch, struct
 __pyx_opt_args_7easyvec_8geometry_8PolyLine_intersect_segment
@@ -10702,20 +11001,20 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_13intersect_segment
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_17intersect_segment
 (PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_7easyvec_8geometry_8PolyLine_12intersect_segment[] =
+static char __pyx_doc_7easyvec_8geometry_8PolyLine_16intersect_segment[] =
 "PolyLine.intersect_segment(self, Vec2 p1, Vec2 p2, bool sortreduce=True) -
 > list";
-static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_13intersect_segment
+static PyObject *__pyx_pw_7easyvec_8geometry_8PolyLine_17intersect_segment
 (PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p1 = 0;
   struct __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p2 = 0;
   int __pyx_v_sortreduce;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("intersect_segment (wrapper)", 0);
@@ -10744,27 +11043,27 @@
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds,
 __pyx_n_s_p2)) != 0)) kw_args--;
         else {
           __Pyx_RaiseArgtupleInvalid("intersect_segment", 0, 2, 3, 1);
-__PYX_ERR(0, 622, __pyx_L3_error)
+__PYX_ERR(0, 634, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds,
 __pyx_n_s_sortreduce);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
         if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames,
-0, values, pos_args, "intersect_segment") < 0)) __PYX_ERR(0, 622,
+0, values, pos_args, "intersect_segment") < 0)) __PYX_ERR(0, 634,
 __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
@@ -10773,62 +11072,62 @@
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_p1 = ((struct __pyx_obj_7easyvec_7vectors_Vec2 *)values[0]);
     __pyx_v_p2 = ((struct __pyx_obj_7easyvec_7vectors_Vec2 *)values[1]);
     if (values[2]) {
       __pyx_v_sortreduce = __Pyx_PyObject_IsTrue(values[2]); if (unlikely(
-(__pyx_v_sortreduce == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 622,
+(__pyx_v_sortreduce == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 634,
 __pyx_L3_error)
     } else {
       __pyx_v_sortreduce = ((int)1);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("intersect_segment", 0, 2, 3, PyTuple_GET_SIZE
-(__pyx_args)); __PYX_ERR(0, 622, __pyx_L3_error)
+(__pyx_args)); __PYX_ERR(0, 634, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("easyvec.geometry.PolyLine.intersect_segment",
 __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_p1),
-__pyx_ptype_7easyvec_7vectors_Vec2, 1, "p1", 0))) __PYX_ERR(0, 622,
+__pyx_ptype_7easyvec_7vectors_Vec2, 1, "p1", 0))) __PYX_ERR(0, 634,
 __pyx_L1_error)
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_p2),
-__pyx_ptype_7easyvec_7vectors_Vec2, 1, "p2", 0))) __PYX_ERR(0, 622,
+__pyx_ptype_7easyvec_7vectors_Vec2, 1, "p2", 0))) __PYX_ERR(0, 634,
 __pyx_L1_error)
-  __pyx_r = __pyx_pf_7easyvec_8geometry_8PolyLine_12intersect_segment(((struct
+  __pyx_r = __pyx_pf_7easyvec_8geometry_8PolyLine_16intersect_segment(((struct
 __pyx_obj_7easyvec_8geometry_PolyLine *)__pyx_v_self), __pyx_v_p1, __pyx_v_p2,
 __pyx_v_sortreduce);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_12intersect_segment
+static PyObject *__pyx_pf_7easyvec_8geometry_8PolyLine_16intersect_segment
 (struct __pyx_obj_7easyvec_8geometry_PolyLine *__pyx_v_self, struct
 __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p1, struct
 __pyx_obj_7easyvec_7vectors_Vec2 *__pyx_v_p2, int __pyx_v_sortreduce) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("intersect_segment", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2.__pyx_n = 1;
   __pyx_t_2.sortreduce = __pyx_v_sortreduce;
   __pyx_t_1 = __pyx_vtabptr_7easyvec_8geometry_PolyLine->intersect_segment
 (__pyx_v_self, __pyx_v_p1, __pyx_v_p2, 1, &__pyx_t_2); if (unlikely
-(!__pyx_t_1)) __PYX_ERR(0, 622, __pyx_L1_error)
+(!__pyx_t_1)) __PYX_ERR(0, 634, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -10837,22 +11136,22 @@
 __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
-+623:         return self.intersect_general(p1, p2, 0.0, 1.0, sortreduce)
++635:         return self.intersect_general(p1, p2, 0.0, 1.0, sortreduce)
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2.__pyx_n = 1;
   __pyx_t_2.sortreduce = __pyx_v_sortreduce;
   __pyx_t_1 = __pyx_f_7easyvec_8geometry_8PolyLine_intersect_general
 (__pyx_v_self, __pyx_v_p1, __pyx_v_p2, 0.0, 1.0, 0, &__pyx_t_2); if (unlikely
-(!__pyx_t_1)) __PYX_ERR(0, 623, __pyx_L1_error)
+(!__pyx_t_1)) __PYX_ERR(0, 635, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
   goto __pyx_L0;
-&#xA0;624:
-&#xA0;625:
-&#xA0;626:
-&#xA0;627:
+&#xA0;636:
+&#xA0;637:
+&#xA0;638:
+&#xA0;639:
```

### Comparing `easyvec-0.0.8/src/easyvec/geometry.pxd` & `easyvec-0.0.9/src/easyvec/geometry.pxd`

 * *Files identical despite different names*

### Comparing `easyvec-0.0.8/src/easyvec/geometry.pyx` & `easyvec-0.0.9/src/easyvec/geometry.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -552,14 +552,20 @@
     cpdef bint is_bbox_intersect(self, Vec2 p1, Vec2 p2):
         return (self.x1 <= fmax(p1.x, p2.x)) and (self.x2 >= fmin(p1.x, p2.x)) \
            and (self.y1 <= fmax(p1.y, p2.y)) and (self.y2 >= fmin(p1.y, p2.y))
  
 
 @cython.final
 cdef class PolyLine:
+    @classmethod
+    def from_dict(cls, dct):
+        vecs = [Vec2.from_dict(vd) for vd in dct['vecs']]
+        enclosed = dct['enclosed']
+        return cls(vecs, enclosed)
+
     def __cinit__(self, vecs: list, enclosed=True, copy_data=False):
         cdef int vec_len, i
         if copy_data:
             self.vecs = []
             vec_len = len(vecs)
             for i in range(vec_len):
                 self.vecs.append( (<Vec2>(vecs[i])).copy() )
@@ -567,14 +573,20 @@
             self.vecs = vecs
         self.vlen = len(self.vecs)
         if self.vlen < 2:
             raise ValueError(f'Слишком мало точек для линии. Необходимо больше, чем 1')
         self.enclosed = enclosed
         self.bbox = Rect.bbox(self.vecs)
 
+    def to_dict(self):
+        return {
+            'vecs': [v.to_dict() for v in self.vecs],
+            'enclosed': bool(self.enclosed)
+        }
+
     def __str__(self):
         s = [f'({v.x:.2f}, {v.y:.2f})' for v in self.vecs]
         s = ', '.join(s)
         return f'PolyLine({s})'
 
     def __repr__(self):
         s = [f'({v.x}, {v.y})' for v in self.vecs]
```

### Comparing `easyvec-0.0.8/src/easyvec/matrixes.cpp` & `easyvec-0.0.9/src/easyvec/matrixes.cpp`

 * *Files identical despite different names*

### Comparing `easyvec-0.0.8/src/easyvec/matrixes.html` & `easyvec-0.0.9/src/easyvec/matrixes.html`

 * *Files identical despite different names*

### Comparing `easyvec-0.0.8/src/easyvec/matrixes.pxd` & `easyvec-0.0.9/src/easyvec/matrixes.pxd`

 * *Files identical despite different names*

### Comparing `easyvec-0.0.8/src/easyvec/matrixes.pyx` & `easyvec-0.0.9/src/easyvec/matrixes.pyx`

 * *Files identical despite different names*

### Comparing `easyvec-0.0.8/src/easyvec/vectors.cpp` & `easyvec-0.0.9/src/easyvec/vectors.cpp`

 * *Files identical despite different names*

### Comparing `easyvec-0.0.8/src/easyvec/vectors.html` & `easyvec-0.0.9/src/easyvec/vectors.html`

 * *Files identical despite different names*

### Comparing `easyvec-0.0.8/src/easyvec/vectors.pxd` & `easyvec-0.0.9/src/easyvec/vectors.pxd`

 * *Files identical despite different names*

### Comparing `easyvec-0.0.8/src/easyvec/vectors.pyx` & `easyvec-0.0.9/src/easyvec/vectors.pyx`

 * *Files identical despite different names*

### Comparing `easyvec-0.0.8/src/easyvec.egg-info/PKG-INFO` & `easyvec-0.0.9/src/easyvec.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyvec
-Version: 0.0.8
+Version: 0.0.9
 Summary: Vector library
 Home-page: https://github.com/TovarnovM/easyvec
 Author: Mikhail Tovarnov
 Author-email: mtovarnov@mail.com
 License: MIT
 Project-URL: Documentation, https://github.com/TovarnovM/easyvec
 Project-URL: Code, https://github.com/TovarnovM/easyvec
```

### Comparing `easyvec-0.0.8/src/easyvec.egg-info/SOURCES.txt` & `easyvec-0.0.9/src/easyvec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

