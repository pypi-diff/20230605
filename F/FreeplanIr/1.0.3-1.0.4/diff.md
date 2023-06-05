# Comparing `tmp/FreeplanIr-1.0.3.tar.gz` & `tmp/FreeplanIr-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FreeplanIr-1.0.3.tar", last modified: Thu May 25 02:47:27 2023, max compression
+gzip compressed data, was "FreeplanIr-1.0.4.tar", last modified: Mon Jun  5 06:52:46 2023, max compression
```

## Comparing `FreeplanIr-1.0.3.tar` & `FreeplanIr-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 02:47:27.191463 FreeplanIr-1.0.3/
-drwxrwxrwx   0        0        0        0 2023-05-25 02:47:27.181465 FreeplanIr-1.0.3/FreeplanIr/
--rw-rw-rw-   0        0        0       47 2023-05-24 09:10:22.000000 FreeplanIr-1.0.3/FreeplanIr/__init__.py
--rw-rw-rw-   0        0        0     3324 2023-05-25 02:17:24.000000 FreeplanIr-1.0.3/FreeplanIr/main.py
-drwxrwxrwx   0        0        0        0 2023-05-25 02:47:27.188465 FreeplanIr-1.0.3/FreeplanIr.egg-info/
--rw-rw-rw-   0        0        0     1484 2023-05-25 02:47:27.000000 FreeplanIr-1.0.3/FreeplanIr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-05-25 02:47:27.000000 FreeplanIr-1.0.3/FreeplanIr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 02:47:27.000000 FreeplanIr-1.0.3/FreeplanIr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-05-25 02:47:27.000000 FreeplanIr-1.0.3/FreeplanIr.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-25 02:47:27.000000 FreeplanIr-1.0.3/FreeplanIr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1094 2023-05-24 08:32:25.000000 FreeplanIr-1.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0     1484 2023-05-25 02:47:27.190464 FreeplanIr-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1016 2023-05-25 02:26:52.000000 FreeplanIr-1.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-25 02:47:27.191463 FreeplanIr-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      766 2023-05-25 02:47:24.000000 FreeplanIr-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 06:52:46.796779 FreeplanIr-1.0.4/
+drwxrwxrwx   0        0        0        0 2023-06-05 06:52:46.785751 FreeplanIr-1.0.4/FreeplanIr/
+-rw-rw-rw-   0        0        0       47 2023-05-24 09:10:22.000000 FreeplanIr-1.0.4/FreeplanIr/__init__.py
+-rw-rw-rw-   0        0        0     4038 2023-06-05 06:50:24.000000 FreeplanIr-1.0.4/FreeplanIr/main.py
+drwxrwxrwx   0        0        0        0 2023-06-05 06:52:46.793749 FreeplanIr-1.0.4/FreeplanIr.egg-info/
+-rw-rw-rw-   0        0        0     1706 2023-06-05 06:52:46.000000 FreeplanIr-1.0.4/FreeplanIr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-06-05 06:52:46.000000 FreeplanIr-1.0.4/FreeplanIr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 06:52:46.000000 FreeplanIr-1.0.4/FreeplanIr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-06-05 06:52:46.000000 FreeplanIr-1.0.4/FreeplanIr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-05 06:52:46.000000 FreeplanIr-1.0.4/FreeplanIr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1094 2023-05-24 08:32:25.000000 FreeplanIr-1.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     1706 2023-06-05 06:52:46.795748 FreeplanIr-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-06-05 06:41:44.000000 FreeplanIr-1.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-05 06:52:46.796779 FreeplanIr-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      766 2023-06-05 06:41:44.000000 FreeplanIr-1.0.4/setup.py
```

### Comparing `FreeplanIr-1.0.3/FreeplanIr/main.py` & `FreeplanIr-1.0.4/FreeplanIr/main.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-
+import csv
 from typing import List
 import xml.etree.ElementTree as Et
 from xml.etree.ElementTree import Element
 import xlsxwriter
 
 
 class FreeplanIr:
@@ -18,14 +18,15 @@
         mind_map = Et.parse(self.file_path)
         self.root = mind_map.getroot()
 
     def plan_test(self) -> List[List[str]]:
         data_list = []
 
         def traverse_nodes(node: Element, data: List[str]):
+            text = node.get('TEXT').replace('\n', '\\n')
             data.append(node.get('TEXT'))
             for child_node in node.findall('node'):
                 self._count += 1
                 if self._count > self._max_num:
                     self._max_num = self._count
                 traverse_nodes(child_node, data.copy())
 
@@ -80,13 +81,28 @@
         for datas in data_list:
             for index in range(len(datas)):
                 writesheet.write(row, index, datas[index])
             row += 1
         write_worke.close()
         return xlsx_path
 
+    # 下载禅道csv
+    def download_chandao(self) -> str:
+        title = ["所属模块", "用例标题", "前置条件", "步骤", "预期", "用例类型"]
+        plan_data = self.plan_test()
+        csv_path = self.file_path.replace(".mm", ".csv")
+        with open(csv_path, 'w', encoding='GBK', newline='') as f:
+            writer_csv = csv.writer(f)
+            writer_csv.writerow(title)
+            for i in plan_data:
+                csv_data = i[2:]
+                csv_data[0] = "/(#0)"
+                csv_data.append("功能测试")
+                writer_csv.writerow(csv_data)
+        return csv_path
+
 
 if __name__ == '__main__':
     file_path = r"E:\项目文件\社区电商一起\RMS系统\v2.1轨迹\RMS轨迹测试用例.mm"
     test_plan = FreeplanIr(file_path)
-    datas = test_plan.download()
+    datas = test_plan.download_chandao()
     print(datas)
```

### Comparing `FreeplanIr-1.0.3/FreeplanIr.egg-info/PKG-INFO` & `FreeplanIr-1.0.4/FreeplanIr.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FreeplanIr
-Version: 1.0.3
+Version: 1.0.4
 Summary: 一个可以解析freeplan *.mm格式文件的工具
 Home-page: https://github.com/leslie110
 Author: wangdashuai
 Author-email: hanchaodaming@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -35,9 +35,14 @@
 ### 获取转换数据
     datas = test_plan.plan_test() # 调用plan_test方法即可，返回为转换好数据
     print(datas)  
 ### 下载为xlxs
     path = test_plan.download() # 调用plan_test方法即可，返回为文件保存地址
     print(datas)  
   此方法返回的结果就是如上所说，需要注意次方返回目前仅支持所有节点的长度一致。
+### 下载为csv，导入禅道中生成测试用例
+    path = test_plan.download_chandao() # download_chandao，返回为文件保存地址
+    print(datas)  
+  使用此方法无需做其他数据源头更改
+
```

### Comparing `FreeplanIr-1.0.3/LICENSE.txt` & `FreeplanIr-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `FreeplanIr-1.0.3/PKG-INFO` & `FreeplanIr-1.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FreeplanIr
-Version: 1.0.3
+Version: 1.0.4
 Summary: 一个可以解析freeplan *.mm格式文件的工具
 Home-page: https://github.com/leslie110
 Author: wangdashuai
 Author-email: hanchaodaming@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -35,9 +35,14 @@
 ### 获取转换数据
     datas = test_plan.plan_test() # 调用plan_test方法即可，返回为转换好数据
     print(datas)  
 ### 下载为xlxs
     path = test_plan.download() # 调用plan_test方法即可，返回为文件保存地址
     print(datas)  
   此方法返回的结果就是如上所说，需要注意次方返回目前仅支持所有节点的长度一致。
+### 下载为csv，导入禅道中生成测试用例
+    path = test_plan.download_chandao() # download_chandao，返回为文件保存地址
+    print(datas)  
+  使用此方法无需做其他数据源头更改
+
```

### Comparing `FreeplanIr-1.0.3/setup.py` & `FreeplanIr-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="FreeplanIr",
-    version="1.0.3",
+    version="1.0.4",
     author="wangdashuai",
     author_email="hanchaodaming@outlook.com",
     description="一个可以解析freeplan *.mm格式文件的工具",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/leslie110",
     packages=setuptools.find_packages(),
```

