# Comparing `tmp/georgio-2023.119.77-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip` & `tmp/georgio-2023.156.924-cp311-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 1059429 bytes, number of entries: 7
--rw-r--r--  4.6 unx     3045 b- defN 23-Apr-29 01:19 georgio-2023.119.77.dist-info/METADATA
--rw-r--r--  4.6 unx      129 b- defN 23-Apr-29 01:19 georgio-2023.119.77.dist-info/WHEEL
--rw-r--r--  4.6 unx    11350 b- defN 23-Apr-29 01:19 georgio-2023.119.77.dist-info/license_files/LICENSE
--rw-r--r--  4.6 unx       47 b- defN 23-Apr-29 01:19 georgio-2023.119.77.dist-info/license_files/NOTICE
--rw-r--r--  4.6 unx      111 b- defN 23-Apr-29 01:19 georgio/__init__.py
--rwxr-xr-x  4.6 unx  4415240 b- defN 23-Apr-29 01:19 georgio/georgio.cpython-39-x86_64-linux-gnu.so
--rw-r--r--  4.6 unx      620 b- defN 23-Apr-29 01:19 georgio-2023.119.77.dist-info/RECORD
-7 files, 4430542 bytes uncompressed, 1058325 bytes compressed:  76.1%
+Zip file size: 114934 bytes, number of entries: 7
+-rw-r--r--  4.6 unx     3109 b- defN 23-Jun-05 15:29 georgio-2023.156.924.dist-info/METADATA
+-rw-r--r--  4.6 unx       95 b- defN 23-Jun-05 15:29 georgio-2023.156.924.dist-info/WHEEL
+-rw-r--r--  4.6 unx    11552 b- defN 23-Jun-05 15:29 georgio-2023.156.924.dist-info/license_files/LICENSE
+-rw-r--r--  4.6 unx       49 b- defN 23-Jun-05 15:29 georgio-2023.156.924.dist-info/license_files/NOTICE
+-rw-r--r--  4.6 unx      111 b- defN 23-Jun-05 15:29 georgio/__init__.py
+-rwxr-xr-x  4.6 unx   243712 b- defN 23-Jun-05 15:29 georgio/georgio.cp311-win_amd64.pyd
+-rw-r--r--  4.6 unx      612 b- defN 23-Jun-05 15:29 georgio-2023.156.924.dist-info/RECORD
+7 files, 259240 bytes uncompressed, 113842 bytes compressed:  56.1%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
-Filename: georgio-2023.119.77.dist-info/METADATA
+Filename: georgio-2023.156.924.dist-info/METADATA
 Comment: 
 
-Filename: georgio-2023.119.77.dist-info/WHEEL
+Filename: georgio-2023.156.924.dist-info/WHEEL
 Comment: 
 
-Filename: georgio-2023.119.77.dist-info/license_files/LICENSE
+Filename: georgio-2023.156.924.dist-info/license_files/LICENSE
 Comment: 
 
-Filename: georgio-2023.119.77.dist-info/license_files/NOTICE
+Filename: georgio-2023.156.924.dist-info/license_files/NOTICE
 Comment: 
 
 Filename: georgio/__init__.py
 Comment: 
 
-Filename: georgio/georgio.cpython-39-x86_64-linux-gnu.so
+Filename: georgio/georgio.cp311-win_amd64.pyd
 Comment: 
 
-Filename: georgio-2023.119.77.dist-info/RECORD
+Filename: georgio-2023.156.924.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `georgio-2023.119.77.dist-info/METADATA` & `georgio-2023.156.924.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,79 +1,79 @@
 Metadata-Version: 2.1
 Name: georgio
-Version: 2023.119.77
+Version: 2023.156.924
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 License-File: NOTICE
 Summary: Fast Geo Rust functions for Python
 Author-email: Spectric Labs <foss@spectric.com>
 License: Apache-2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: repository, https://github.com/spectriclabs/georgio
 
-# georgio
-
-Fast **geo** **R**ust helper functions for Python.
-
-## Great Circle
-
-To get the great circle distance between two points in meters, this function will use the IUGG mean Earth radius.
-
-```python
-distance_in_meters = georgio.great_circle_distance(lon1, lat1, lon2, lat2)
-```
-
-If you want to provide your own radius in meters, you can use this function instead.
-
-```python
-distance_in_meters = georgio.great_circle_distance_with_radius(lon1, lat1, lon2, lat2, radius_in_meters)
-```
-
-## Line Of Bearing (LOB)
-
-Returns the destination coordinates based on a starting position, bearing, and distance in meters.  Bearing is in degrees, clockwise from north.  It uses the IUGG mean Earth radius.
-
-```python
-dest_lon, dest_lat = georgio.line_of_bearing(start_lon, start_lat, bearing_in_degrees, distance_in_meters)
-```
-
-If you want to provide your own radius in meters, you can use this function instead.
-
-```python
-dest_lon, dest_lat = georgio.line_of_bearing_with_radius(start_lon, start_lat, bearing_in_degrees, distance_in_meters, radius_in_meters)
-```
-
-## Bounding Box
-
-This function will return a bounding box that encompasses  the specified distance around a center point.
-Note that the bounding box will never extend across the antimeridian (longitude +/-180), below latitude -90, or above latitude 90.
-
-```python
-west, south, east, north = georgio.bounding_box_for_point(lon, lat, distance_in_meters)
-```
-
-## Web Mercator
-
-To get the longitude/latitude bounds of a Web Mercator tile, use the following function, which will return the values in west, south, east, north order.
-
-```python
-west, south, east, north = georgio.wm_bounds(x, y, z)
-```
-
-To get the upper left corner of a tile in longitude, latitude order, use the following function.
-
-```python
-longitude, latitude = georgio.wm_upper_left(x, y, z)
-```
-
-To get a bounding box that surrounds a tile at a certain distance, use the following function.
-This can be useful when searching for centerpoints of objects that might be outside of the tile, where the object might extend into the tile.
-Note that the bounding box size is calculated in the WGS-84 projection based on the tile's longitude/latitude bounds, since Web Mercator is notoriously bad for calculating sizes/distances.
-Also note that the bounding box will never extend across the antimeridian (longitude +/-180), below latitude -90, or above latitude 90.
-
-```python
-west, south, east, north = georgio.wm_tile_expanded_bbox(x, y, z, search_distance_in_meters)
-```
+# georgio
+
+Fast **geo** **R**ust helper functions for Python.
+
+## Great Circle
+
+To get the great circle distance between two points in meters, this function will use the IUGG mean Earth radius.
+
+```python
+distance_in_meters = georgio.great_circle_distance(lon1, lat1, lon2, lat2)
+```
+
+If you want to provide your own radius in meters, you can use this function instead.
+
+```python
+distance_in_meters = georgio.great_circle_distance_with_radius(lon1, lat1, lon2, lat2, radius_in_meters)
+```
+
+## Line Of Bearing (LOB)
+
+Returns the destination coordinates based on a starting position, bearing, and distance in meters.  Bearing is in degrees, clockwise from north.  It uses the IUGG mean Earth radius.
+
+```python
+dest_lon, dest_lat = georgio.line_of_bearing(start_lon, start_lat, bearing_in_degrees, distance_in_meters)
+```
+
+If you want to provide your own radius in meters, you can use this function instead.
+
+```python
+dest_lon, dest_lat = georgio.line_of_bearing_with_radius(start_lon, start_lat, bearing_in_degrees, distance_in_meters, radius_in_meters)
+```
+
+## Bounding Box
+
+This function will return a bounding box that encompasses  the specified distance around a center point.
+Note that the bounding box will never extend across the antimeridian (longitude +/-180), below latitude -90, or above latitude 90.
+
+```python
+west, south, east, north = georgio.bounding_box_for_point(lon, lat, distance_in_meters)
+```
+
+## Web Mercator
+
+To get the longitude/latitude bounds of a Web Mercator tile, use the following function, which will return the values in west, south, east, north order.
+
+```python
+west, south, east, north = georgio.wm_bounds(x, y, z)
+```
+
+To get the upper left corner of a tile in longitude, latitude order, use the following function.
+
+```python
+longitude, latitude = georgio.wm_upper_left(x, y, z)
+```
+
+To get a bounding box that surrounds a tile at a certain distance, use the following function.
+This can be useful when searching for centerpoints of objects that might be outside of the tile, where the object might extend into the tile.
+Note that the bounding box size is calculated in the WGS-84 projection based on the tile's longitude/latitude bounds, since Web Mercator is notoriously bad for calculating sizes/distances.
+Also note that the bounding box will never extend across the antimeridian (longitude +/-180), below latitude -90, or above latitude 90.
+
+```python
+west, south, east, north = georgio.wm_tile_expanded_bbox(x, y, z, search_distance_in_meters)
+```
```

## Comparing `georgio-2023.119.77.dist-info/license_files/LICENSE` & `georgio-2023.156.924.dist-info/license_files/LICENSE`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,202 +1,202 @@
-
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright 2023 Spectric Labs, Inc.
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright 2023 Spectric Labs, Inc.
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

## Comparing `georgio-2023.119.77.dist-info/RECORD` & `georgio-2023.156.924.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-georgio-2023.119.77.dist-info/METADATA,sha256=Yj3RfttQQDqRtbHVnqRe7YgFa482mg_N_lA8BYQTbow,3045
-georgio-2023.119.77.dist-info/WHEEL,sha256=d0gyNHk0b2RiWczoqHO_rmfWlP6BdcdaQOG_CcKx5DE,129
-georgio-2023.119.77.dist-info/license_files/LICENSE,sha256=ywzEKttt6hjlwzpjOdfub5SuDwEcX8nUEGmyeWcrXI8,11350
-georgio-2023.119.77.dist-info/license_files/NOTICE,sha256=HLkdtb5SdwR3MrOcfQ3PA62FtpSXM_wm1AJuaaRMWfg,47
+georgio-2023.156.924.dist-info/METADATA,sha256=iHRP119L_87t1-_KIpS9aAiPmVDRP5yePj_n1zRnxx0,3109
+georgio-2023.156.924.dist-info/WHEEL,sha256=LjoxhToe_g3LjK352karwl00dg-XjN5wKdGekYlIa-U,95
+georgio-2023.156.924.dist-info/license_files/LICENSE,sha256=PN3LKywYLihv4OnVb3rkSuPQh7UAApC-EfeXG9T0x1Y,11552
+georgio-2023.156.924.dist-info/license_files/NOTICE,sha256=yb7DarER_BqOwSvocVhKctuotDp5V5gWhz5UW-WpPKg,49
 georgio/__init__.py,sha256=fYu96aUNXs6kyIUQ-Tmxa_froNoccWR5b8VeVwmz7s0,111
-georgio/georgio.cpython-39-x86_64-linux-gnu.so,sha256=YY3TiP_Qx8SIRZ7RDgTNU6TqAkWwwfB1xvCwVXV_XW8,4415240
-georgio-2023.119.77.dist-info/RECORD,,
+georgio/georgio.cp311-win_amd64.pyd,sha256=r2EsFDU-XA5aing2tK6ocPkVfuVu_21YYb4n3ctOtgM,243712
+georgio-2023.156.924.dist-info/RECORD,,
```

