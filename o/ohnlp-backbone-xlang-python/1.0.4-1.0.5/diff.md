# Comparing `tmp/ohnlp-backbone-xlang-python-1.0.4.tar.gz` & `tmp/ohnlp-backbone-xlang-python-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ohnlp-backbone-xlang-python-1.0.4.tar", last modified: Mon Jun  5 16:57:26 2023, max compression
+gzip compressed data, was "ohnlp-backbone-xlang-python-1.0.5.tar", last modified: Mon Jun  5 18:32:03 2023, max compression
```

## Comparing `ohnlp-backbone-xlang-python-1.0.4.tar` & `ohnlp-backbone-xlang-python-1.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 16:57:26.659074 ohnlp-backbone-xlang-python-1.0.4/
--rw-rw-rw-   0        0        0    11558 2023-05-25 17:32:33.000000 ohnlp-backbone-xlang-python-1.0.4/LICENSE
--rw-rw-rw-   0        0        0      236 2023-06-05 16:57:26.659074 ohnlp-backbone-xlang-python-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      739 2023-06-05 15:53:15.000000 ohnlp-backbone-xlang-python-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 16:57:26.615074 ohnlp-backbone-xlang-python-1.0.4/ohnlp/
--rw-rw-rw-   0        0        0        0 2023-06-05 15:31:44.000000 ohnlp-backbone-xlang-python-1.0.4/ohnlp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 16:57:26.617074 ohnlp-backbone-xlang-python-1.0.4/ohnlp/toolkit/
--rw-rw-rw-   0        0        0        0 2023-06-05 15:31:44.000000 ohnlp-backbone-xlang-python-1.0.4/ohnlp/toolkit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 16:57:26.634072 ohnlp-backbone-xlang-python-1.0.4/ohnlp/toolkit/backbone/
--rw-rw-rw-   0        0        0        0 2023-06-05 15:31:44.000000 ohnlp-backbone-xlang-python-1.0.4/ohnlp/toolkit/backbone/__init__.py
--rw-rw-rw-   0        0        0     7691 2023-06-05 16:51:51.000000 ohnlp-backbone-xlang-python-1.0.4/ohnlp/toolkit/backbone/api.py
--rw-rw-rw-   0        0        0     1589 2023-05-26 20:57:11.000000 ohnlp-backbone-xlang-python-1.0.4/ohnlp/toolkit/backbone/backbone_module_launcher.py
-drwxrwxrwx   0        0        0        0 2023-06-05 16:57:26.657074 ohnlp-backbone-xlang-python-1.0.4/ohnlp_backbone_xlang_python.egg-info/
--rw-rw-rw-   0        0        0      236 2023-06-05 16:57:26.000000 ohnlp-backbone-xlang-python-1.0.4/ohnlp_backbone_xlang_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      440 2023-06-05 16:57:26.000000 ohnlp-backbone-xlang-python-1.0.4/ohnlp_backbone_xlang_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 16:57:26.000000 ohnlp-backbone-xlang-python-1.0.4/ohnlp_backbone_xlang_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      501 2023-06-05 16:57:26.000000 ohnlp-backbone-xlang-python-1.0.4/ohnlp_backbone_xlang_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-05 16:57:26.000000 ohnlp-backbone-xlang-python-1.0.4/ohnlp_backbone_xlang_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 16:57:26.660074 ohnlp-backbone-xlang-python-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1222 2023-06-05 16:54:18.000000 ohnlp-backbone-xlang-python-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:32:03.037952 ohnlp-backbone-xlang-python-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-05 18:31:59.000000 ohnlp-backbone-xlang-python-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-05 18:32:03.037952 ohnlp-backbone-xlang-python-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-05 18:31:59.000000 ohnlp-backbone-xlang-python-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:32:03.037952 ohnlp-backbone-xlang-python-1.0.5/ohnlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 18:31:59.000000 ohnlp-backbone-xlang-python-1.0.5/ohnlp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:32:03.037952 ohnlp-backbone-xlang-python-1.0.5/ohnlp/toolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 18:31:59.000000 ohnlp-backbone-xlang-python-1.0.5/ohnlp/toolkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:32:03.037952 ohnlp-backbone-xlang-python-1.0.5/ohnlp/toolkit/backbone/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 18:31:59.000000 ohnlp-backbone-xlang-python-1.0.5/ohnlp/toolkit/backbone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7466 2023-06-05 18:31:59.000000 ohnlp-backbone-xlang-python-1.0.5/ohnlp/toolkit/backbone/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-05 18:31:59.000000 ohnlp-backbone-xlang-python-1.0.5/ohnlp/toolkit/backbone/backbone_module_launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:32:03.037952 ohnlp-backbone-xlang-python-1.0.5/ohnlp_backbone_xlang_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-05 18:32:03.000000 ohnlp-backbone-xlang-python-1.0.5/ohnlp_backbone_xlang_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-05 18:32:03.000000 ohnlp-backbone-xlang-python-1.0.5/ohnlp_backbone_xlang_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 18:32:03.000000 ohnlp-backbone-xlang-python-1.0.5/ohnlp_backbone_xlang_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-05 18:32:03.000000 ohnlp-backbone-xlang-python-1.0.5/ohnlp_backbone_xlang_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-05 18:32:03.000000 ohnlp-backbone-xlang-python-1.0.5/ohnlp_backbone_xlang_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 18:32:03.037952 ohnlp-backbone-xlang-python-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-05 18:31:59.000000 ohnlp-backbone-xlang-python-1.0.5/setup.py
```

### Comparing `ohnlp-backbone-xlang-python-1.0.4/LICENSE` & `ohnlp-backbone-xlang-python-1.0.5/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
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
-   Copyright [yyyy] [name of copyright owner]
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
+   Copyright [yyyy] [name of copyright owner]
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

### Comparing `ohnlp-backbone-xlang-python-1.0.4/ohnlp/toolkit/backbone/api.py` & `ohnlp-backbone-xlang-python-1.0.5/ohnlp/toolkit/backbone/api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,220 +1,222 @@
-from __future__ import annotations
-from enum import Enum
-from typing import List, Union
-
-
-class FieldType(object):
-    def __init__(self, type_name: TypeName, array_content_type: Union[FieldType, None] = None,
-                 row_content_type: Union[Schema, None] = None):
-        if row_content_type is None:
-            row_content_type = []
-        self.type_name: TypeName = type_name
-        self.array_content_type: FieldType = array_content_type
-        self.content_obj_fields: Schema = row_content_type
-
-
-class TypeName(Enum):
-    STRING = "STRING",
-    BYTE = "BYTE",
-    BYTES = "BYTES",
-    INT16 = "INT16",
-    INT32 = "INT32",
-    INT64 = "INT64",
-    FLOAT = "FLOAT",
-    DOUBLE = "DOUBLE",
-    DECIMAL = "DECIMAL",
-    BOOLEAN = "BOOLEAN",
-    DATETIME = "DATETIME",
-    ROW = "ROW",
-    ARRAY = "ARRAY"
-
-
-class SchemaField(object):
-    def __init__(self, name: str, field_meta: FieldType):
-        self.name: str = name
-        self.field_type: FieldType = field_meta
-
-    class Java:
-        implements = ["org.ohnlp.backbone.api.components.xlang.python.PythonSchema$PythonSchemaField"]
-
-
-class Schema(object):
-    def __init__(self, fields: List[SchemaField]):
-        self.fields: List[SchemaField] = fields
-        self.fields_by_name: dict = {}
-        for field in fields:
-            self.fields_by_name[field.name] = field
-
-    def get_fields(self) -> List[SchemaField]:
-        return self.fields
-
-    def get_field(self, name: str) -> SchemaField:
-        return self.fields_by_name[name]
-
-    class Java:
-        implements = ["org.ohnlp.backbone.api.components.xlang.python.PythonSchema"]
-
-
-class Row(object):
-    def __init__(self, schema: Schema, values: List[object]):
-        self.schema: Schema = schema
-        self.field_idx: dict[str, int] = {}
-        for i in range(0, len(schema.fields)):
-            self.field_idx[schema.fields[i].name] = i
-        self.values: List[object] = values
-
-    def get_schema(self) -> Schema:
-        return self.schema
-
-    def get_value(self, field_name: str) -> Union[object, None]:
-        if self.field_idx[field_name] is not None:
-            return self.values[self.field_idx[field_name]]
-        else:
-            return None
-
-    def get_values(self) -> List[object]:
-        return self.values
-
-    class Java:
-        implements = ["org.ohnlp.backbone.api.components.xlang.python.PythonRow"]
-
-
-class BridgedInterfaceWithConvertableDataTypes(object):
-    def python_schema_from_json_string(self, json_schema: str) -> Schema:
-        schema_def: dict = json.loads(json_schema)
-        return self.parse_schema_from_json(schema_def)
-
-    def parse_schema_from_json(self, schema_def: dict) -> Schema:
-        schema_fields: List[SchemaField] = []
-        for field_name in schema_def:
-            schema_fields.append(SchemaField.of(field_name, self.parse_schema_field_type_from_json(schema_def[field_name])))
-        return Schema(schema_fields)
-
-    def parse_schema_field_type_from_json(self, val) -> FieldType:
-        if type(val) == str:
-            return FieldType(TypeName(str(val)))
-        elif type(val) == dict:
-            return FieldType(TypeName.ROW, row_content_type=self.parse_schema_from_json(val))
-        else:
-            return FieldType(TypeName.ARRAY, array_content_type=self.parse_schema_field_type_from_json(val[0]))
-
-    def python_row_from_json_string(self, json_row: str) -> Row:
-        data: dict = json.loads(json_row)
-        schema: Schema = parse_schema(data['schema'])
-        raw_row: dict = data['contents']
-        return self.parse_row_from_json(schema, raw_row)
-
-    def parse_row_from_json(self, schema: Schema, data: dict) -> Row:
-        values: List[object] = []
-        for field in schema.fields:
-            values.append(self.parse_field_value_from_json(field.field_type, data[field.name]))
-
-        return Row(schema, values)
-
-    def parse_field_value_from_json(self, content_type: FieldType, val) -> Union[object, None]:
-        if val is None:
-            return None
-        else:
-            if content_type.type_name == TypeName.ROW:
-                return self.parse_row_from_json(field.field_type.content_obj_fields, data[field.name])
-            elif content_type.type_name == TypeName.ARRAY:
-                child_type: FieldType = field.field_type.array_content_type
-                sub_values: List[object] = []
-                for entry in data[field.name]:
-                    sub_values.append(self.parse_field_value_from_json(child_type, entry))
-                return sub_values
-            else:
-                return val
-
-    def json_string_from_python_schema(self, schema: Schema) -> str:
-        return json.dumps(self.parse_schema_to_json(schema))
-
-    def parse_schema_to_json(self, schema: Schema) -> dict:
-        ret: dict = {}
-        for field in schema.fields:
-            ret[field.name] = self.parse_schema_field_type_to_json(field.field_type)
-        return ret
-
-    def parse_schema_field_type_to_json(self, field_type: FieldType):
-        if field_type.type_name == TypeName.ROW:
-            return self.parse_schema_to_json(field_type.content_obj_fields)
-        elif field_type.type_name == TypeName.ARRAY:
-            return [self.parse_schema_field_type_to_json(field_type.array_content_type)]
-        else:
-            return field_type.type_name.value
-
-    def json_string_from_python_row(self, row: Row) -> str:
-        schema_json = self.parse_schema_to_json(row.schema)
-        contents = self.parse_row_to_json(row)
-        return json.dumps({
-            "schema": schema_json,
-            "contents": contents
-        })
-
-    def parse_row_to_json(self, row: Row) -> dict:
-        ret: dict = {}
-        for field in row.schema.fields:
-            ret[field.name] = self.parse_row_field_value_to_json(field.field_type, row.get_value(field.name))
-        return ret
-
-    def parse_row_field_value_to_json(self, field_type: FieldType, data):
-        if field_type.type_name == TypeName.ROW:
-            return self.parse_row_to_json(data)
-        elif field_type.type_name == TypeName.ARRAY:
-            ret = []
-            for element in data:
-                ret.append(self.parse_row_field_value_to_json(field_type.array_content_type, element))
-            return ret
-        else:
-            return data
-
-
-class BackboneComponentDefinition(object):
-    def get_component_def(self) -> BackboneComponent:
-        pass
-
-    def get_do_fn(self) -> BackboneComponentOneToOneDoFn:
-        pass
-
-
-class BackboneComponent(BridgedInterfaceWithConvertableDataTypes):
-    def __init__(self):
-        pass
-
-    def init(self, configstr: str) -> None:
-        pass
-
-    def to_do_fn_config(self) -> str:
-        pass
-
-    def get_input_tag(self) -> str:
-        pass
-
-    def get_output_tags(self) -> List[str]:
-        pass
-
-    def calculate_output_schema(self, input_schema: Schema) -> Schema:
-        pass
-
-    class Java:
-        implements = ["org.ohnlp.backbone.api.components.xlang.python.PythonBackbonePipelineComponent"]
-
-
-class BackboneComponentOneToOneDoFn(BridgedInterfaceWithConvertableDataTypes):
-    def __init__(self):
-        pass
-
-    def init_from_driver(self, config_json_str: str) -> None:
-        pass
-
-    def on_bundle_start(self) -> None:
-        pass
-
-    def on_bundle_end(self) -> None:
-        pass
-
-    def apply(self, input_row: Row) -> Row:
-        pass
-
-    class Java:
+from __future__ import annotations
+
+import json
+from enum import Enum
+from typing import List, Union
+
+
+class FieldType(object):
+    def __init__(self, type_name: TypeName, array_content_type: Union[FieldType, None] = None,
+                 row_content_type: Union[Schema, None] = None):
+        if row_content_type is None:
+            row_content_type = []
+        self.type_name: TypeName = type_name
+        self.array_content_type: FieldType = array_content_type
+        self.content_obj_fields: Schema = row_content_type
+
+
+class TypeName(Enum):
+    STRING = "STRING",
+    BYTE = "BYTE",
+    BYTES = "BYTES",
+    INT16 = "INT16",
+    INT32 = "INT32",
+    INT64 = "INT64",
+    FLOAT = "FLOAT",
+    DOUBLE = "DOUBLE",
+    DECIMAL = "DECIMAL",
+    BOOLEAN = "BOOLEAN",
+    DATETIME = "DATETIME",
+    ROW = "ROW",
+    ARRAY = "ARRAY"
+
+
+class SchemaField(object):
+    def __init__(self, name: str, field_meta: FieldType):
+        self.name: str = name
+        self.field_type: FieldType = field_meta
+
+    class Java:
+        implements = ["org.ohnlp.backbone.api.components.xlang.python.PythonSchema$PythonSchemaField"]
+
+
+class Schema(object):
+    def __init__(self, fields: List[SchemaField]):
+        self.fields: List[SchemaField] = fields
+        self.fields_by_name: dict = {}
+        for field in fields:
+            self.fields_by_name[field.name] = field
+
+    def get_fields(self) -> List[SchemaField]:
+        return self.fields
+
+    def get_field(self, name: str) -> SchemaField:
+        return self.fields_by_name[name]
+
+    class Java:
+        implements = ["org.ohnlp.backbone.api.components.xlang.python.PythonSchema"]
+
+
+class Row(object):
+    def __init__(self, schema: Schema, values: List[object]):
+        self.schema: Schema = schema
+        self.field_idx: dict[str, int] = {}
+        for i in range(0, len(schema.fields)):
+            self.field_idx[schema.fields[i].name] = i
+        self.values: List[object] = values
+
+    def get_schema(self) -> Schema:
+        return self.schema
+
+    def get_value(self, field_name: str) -> Union[object, None]:
+        if self.field_idx[field_name] is not None:
+            return self.values[self.field_idx[field_name]]
+        else:
+            return None
+
+    def get_values(self) -> List[object]:
+        return self.values
+
+    class Java:
+        implements = ["org.ohnlp.backbone.api.components.xlang.python.PythonRow"]
+
+
+class BridgedInterfaceWithConvertableDataTypes(object):
+    def python_schema_from_json_string(self, json_schema: str) -> Schema:
+        schema_def: dict = json.loads(json_schema)
+        return self.parse_schema_from_json(schema_def)
+
+    def parse_schema_from_json(self, schema_def: dict) -> Schema:
+        schema_fields: List[SchemaField] = []
+        for field_name in schema_def:
+            schema_fields.append(SchemaField.of(field_name, self.parse_schema_field_type_from_json(schema_def[field_name])))
+        return Schema(schema_fields)
+
+    def parse_schema_field_type_from_json(self, val) -> FieldType:
+        if type(val) == str:
+            return FieldType(TypeName(str(val)))
+        elif type(val) == dict:
+            return FieldType(TypeName.ROW, row_content_type=self.parse_schema_from_json(val))
+        else:
+            return FieldType(TypeName.ARRAY, array_content_type=self.parse_schema_field_type_from_json(val[0]))
+
+    def python_row_from_json_string(self, json_row: str) -> Row:
+        data: dict = json.loads(json_row)
+        schema: Schema = self.parse_schema_from_json(data['schema'])
+        raw_row: dict = data['contents']
+        return self.parse_row_from_json(schema, raw_row)
+
+    def parse_row_from_json(self, schema: Schema, data: dict) -> Row:
+        values: List[object] = []
+        for field in schema.fields:
+            values.append(self.parse_field_value_from_json(field.field_type, data[field.name]))
+
+        return Row(schema, values)
+
+    def parse_field_value_from_json(self, content_type: FieldType, val) -> Union[object, None]:
+        if val is None:
+            return None
+        else:
+            if content_type.type_name == TypeName.ROW:
+                return self.parse_row_from_json(content_type.content_obj_fields, val)
+            elif content_type.type_name == TypeName.ARRAY:
+                child_type: FieldType = content_type.array_content_type
+                sub_values: List[object] = []
+                for entry in val:
+                    sub_values.append(self.parse_field_value_from_json(child_type, entry))
+                return sub_values
+            else:
+                return val
+
+    def json_string_from_python_schema(self, schema: Schema) -> str:
+        return json.dumps(self.parse_schema_to_json(schema))
+
+    def parse_schema_to_json(self, schema: Schema) -> dict:
+        ret: dict = {}
+        for field in schema.fields:
+            ret[field.name] = self.parse_schema_field_type_to_json(field.field_type)
+        return ret
+
+    def parse_schema_field_type_to_json(self, field_type: FieldType):
+        if field_type.type_name == TypeName.ROW:
+            return self.parse_schema_to_json(field_type.content_obj_fields)
+        elif field_type.type_name == TypeName.ARRAY:
+            return [self.parse_schema_field_type_to_json(field_type.array_content_type)]
+        else:
+            return field_type.type_name.value
+
+    def json_string_from_python_row(self, row: Row) -> str:
+        schema_json = self.parse_schema_to_json(row.schema)
+        contents = self.parse_row_to_json(row)
+        return json.dumps({
+            "schema": schema_json,
+            "contents": contents
+        })
+
+    def parse_row_to_json(self, row: Row) -> dict:
+        ret: dict = {}
+        for field in row.schema.fields:
+            ret[field.name] = self.parse_row_field_value_to_json(field.field_type, row.get_value(field.name))
+        return ret
+
+    def parse_row_field_value_to_json(self, field_type: FieldType, data):
+        if field_type.type_name == TypeName.ROW:
+            return self.parse_row_to_json(data)
+        elif field_type.type_name == TypeName.ARRAY:
+            ret = []
+            for element in data:
+                ret.append(self.parse_row_field_value_to_json(field_type.array_content_type, element))
+            return ret
+        else:
+            return data
+
+
+class BackboneComponentDefinition(object):
+    def get_component_def(self) -> BackboneComponent:
+        pass
+
+    def get_do_fn(self) -> BackboneComponentOneToOneDoFn:
+        pass
+
+
+class BackboneComponent(BridgedInterfaceWithConvertableDataTypes):
+    def __init__(self):
+        pass
+
+    def init(self, configstr: str) -> None:
+        pass
+
+    def to_do_fn_config(self) -> str:
+        pass
+
+    def get_input_tag(self) -> str:
+        pass
+
+    def get_output_tags(self) -> List[str]:
+        pass
+
+    def calculate_output_schema(self, input_schema: Schema) -> Schema:
+        pass
+
+    class Java:
+        implements = ["org.ohnlp.backbone.api.components.xlang.python.PythonBackbonePipelineComponent"]
+
+
+class BackboneComponentOneToOneDoFn(BridgedInterfaceWithConvertableDataTypes):
+    def __init__(self):
+        pass
+
+    def init_from_driver(self, config_json_str: str) -> None:
+        pass
+
+    def on_bundle_start(self) -> None:
+        pass
+
+    def on_bundle_end(self) -> None:
+        pass
+
+    def apply(self, input_row: Row) -> Row:
+        pass
+
+    class Java:
         implements = ["org.ohnlp.backbone.api.components.xlang.python.PythonOneToOneTransformDoFn"]
```

### Comparing `ohnlp-backbone-xlang-python-1.0.4/ohnlp/toolkit/backbone/backbone_module_launcher.py` & `ohnlp-backbone-xlang-python-1.0.5/ohnlp/toolkit/backbone/backbone_module_launcher.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,49 +1,50 @@
-import importlib
-import json
-import secrets
-import string
-import sys
-from types import ModuleType
-
-from py4j.clientserver import ClientServer, JavaParameters, PythonParameters
-
-if __name__ == '__main__':
-    args = sys.argv[1:]
-    entrypoint_import: str = args[0]
-    class_name: str = args[1]
-    first_init: bool = args[2] == 'component'
-
-    # Import the backbone module to be used
-    module: ModuleType = importlib.import_module(entrypoint_import)
-
-    # Generate an authentication token for this session
-    auth_token = ''.join(secrets.choice(string.ascii_uppercase + string.digits)
-                         for i in range(16))
-
-    # Get appropriate entry point
-    if first_init:
-        entry_point = module.get_component_def()
-    else:
-        entry_point = module.get_do_fn()
-
-    # Bootup python endpoint
-    gateway = ClientServer(
-        java_parameters=JavaParameters(port=0, auth_token=auth_token),
-        python_parameters=PythonParameters(port=0, auth_token=auth_token),
-        python_server_entry_point=entry_point
-    )
-
-    java_port: int = gateway.java_parameters.port
-    python_port: int = gateway.python_parameters.port
-
-    # Write vars out to JSON
-    with open('python_bridge_meta.json', 'rw') as f:
-        json.dump({
-            'token': auth_token,
-            'java_port': java_port,
-            'python_port': python_port
-        }, f)
-
-    # Create monitor file used by java process to indicate gateway init complete
-    with open('python_bridge_meta.done', 'rw') as f:
-        f.writelines('done')
+import importlib
+import json
+import secrets
+import string
+from types import ModuleType
+
+from py4j.clientserver import ClientServer, JavaParameters, PythonParameters
+
+from ohnlp.toolkit.backbone.api import BackboneComponentDefinition
+
+
+def launch_bridge(entrypoint: str, class_name: str, init_type: str):
+    first_init: bool = init_type == 'component'
+
+    # Import the backbone module to be used
+    module: ModuleType = importlib.import_module(entrypoint)
+    cls = getattr(module, class_name)
+    entry_class: BackboneComponentDefinition = cls()
+
+    # Generate an authentication token for this session
+    auth_token = ''.join(secrets.choice(string.ascii_uppercase + string.digits)
+                         for i in range(16))
+
+    # Get appropriate entry point
+    if first_init:
+        entry_point = entry_class.get_component_def()
+    else:
+        entry_point = entry_class.get_do_fn()
+
+    # Bootup python endpoint
+    gateway = ClientServer(
+        java_parameters=JavaParameters(port=0, auth_token=auth_token),
+        python_parameters=PythonParameters(port=0, auth_token=auth_token),
+        python_server_entry_point=entry_point
+    )
+
+    java_port: int = gateway.java_parameters.port
+    python_port: int = gateway.python_parameters.port
+
+    # Write vars out to JSON
+    with open('python_bridge_meta.json', 'rw') as f:
+        json.dump({
+            'token': auth_token,
+            'java_port': java_port,
+            'python_port': python_port
+        }, f)
+
+    # Create monitor file used by java process to indicate gateway init complete
+    with open('python_bridge_meta.done', 'rw') as f:
+        f.writelines('done')
```

