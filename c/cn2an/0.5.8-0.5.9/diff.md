# Comparing `tmp/cn2an-0.5.8.tar.gz` & `tmp/cn2an-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cn2an-0.5.8.tar", last modified: Wed Nov 11 16:07:26 2020, max compression
+gzip compressed data, was "dist/cn2an-0.5.9.tar", last modified: Thu Jan 28 09:34:14 2021, max compression
```

## Comparing `cn2an-0.5.8.tar` & `cn2an-0.5.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 havetwobrush   (501) staff       (20)        0 2020-11-11 16:07:26.000000 cn2an-0.5.8/
--rw-r--r--   0 havetwobrush   (501) staff       (20)    12170 2020-11-11 16:07:26.000000 cn2an-0.5.8/PKG-INFO
-drwxr-xr-x   0 havetwobrush   (501) staff       (20)        0 2020-11-11 16:07:26.000000 cn2an-0.5.8/cn2an.egg-info/
--rw-r--r--   0 havetwobrush   (501) staff       (20)    12170 2020-11-11 16:07:26.000000 cn2an-0.5.8/cn2an.egg-info/PKG-INFO
--rw-r--r--   0 havetwobrush   (501) staff       (20)        1 2020-07-05 11:43:33.000000 cn2an-0.5.8/cn2an.egg-info/not-zip-safe
--rw-r--r--   0 havetwobrush   (501) staff       (20)      484 2020-11-11 16:07:26.000000 cn2an-0.5.8/cn2an.egg-info/SOURCES.txt
--rw-r--r--   0 havetwobrush   (501) staff       (20)       33 2020-11-11 16:07:26.000000 cn2an-0.5.8/cn2an.egg-info/requires.txt
--rw-r--r--   0 havetwobrush   (501) staff       (20)        6 2020-11-11 16:07:26.000000 cn2an-0.5.8/cn2an.egg-info/top_level.txt
--rw-r--r--   0 havetwobrush   (501) staff       (20)        1 2020-11-11 16:07:26.000000 cn2an-0.5.8/cn2an.egg-info/dependency_links.txt
--rw-r--r--   0 havetwobrush   (501) staff       (20)     1062 2020-08-16 11:02:43.000000 cn2an-0.5.8/LICENSE
--rw-r--r--   0 havetwobrush   (501) staff       (20)       32 2020-06-30 22:16:20.000000 cn2an-0.5.8/requirements.txt
-drwxr-xr-x   0 havetwobrush   (501) staff       (20)        0 2020-11-11 16:07:26.000000 cn2an-0.5.8/cn2an/
--rw-r--r--   0 havetwobrush   (501) staff       (20)     8309 2020-11-11 15:56:49.000000 cn2an-0.5.8/cn2an/an2cn.py
--rw-r--r--   0 havetwobrush   (501) staff       (20)    10950 2020-11-11 15:53:41.000000 cn2an-0.5.8/cn2an/cn2an.py
--rw-r--r--   0 havetwobrush   (501) staff       (20)     1779 2020-09-23 21:37:11.000000 cn2an-0.5.8/cn2an/transform_test.py
--rw-r--r--   0 havetwobrush   (501) staff       (20)     1356 2020-07-02 10:58:32.000000 cn2an-0.5.8/cn2an/config.yaml
--rw-r--r--   0 havetwobrush   (501) staff       (20)      261 2020-11-11 15:57:27.000000 cn2an-0.5.8/cn2an/__init__.py
--rw-r--r--   0 havetwobrush   (501) staff       (20)     7583 2020-08-19 05:45:27.000000 cn2an-0.5.8/cn2an/cn2an_test.py
--rw-r--r--   0 havetwobrush   (501) staff       (20)     1530 2020-06-30 22:16:20.000000 cn2an-0.5.8/cn2an/utils.py
--rw-r--r--   0 havetwobrush   (501) staff       (20)     5378 2020-09-23 21:36:17.000000 cn2an-0.5.8/cn2an/transform.py
--rw-r--r--   0 havetwobrush   (501) staff       (20)      614 2020-06-30 22:16:20.000000 cn2an-0.5.8/cn2an/performance.py
--rw-r--r--   0 havetwobrush   (501) staff       (20)     3693 2020-11-11 16:01:17.000000 cn2an-0.5.8/cn2an/an2cn_test.py
--rw-r--r--   0 havetwobrush   (501) staff       (20)      226 2019-12-10 07:40:39.000000 cn2an-0.5.8/MANIFEST.in
--rw-r--r--   0 havetwobrush   (501) staff       (20)     9315 2020-11-11 16:04:24.000000 cn2an-0.5.8/README.md
--rw-r--r--   0 havetwobrush   (501) staff       (20)      956 2020-11-11 15:57:46.000000 cn2an-0.5.8/setup.py
--rw-r--r--   0 havetwobrush   (501) staff       (20)       38 2020-11-11 16:07:26.000000 cn2an-0.5.8/setup.cfg
-drwxr-xr-x   0 havetwobrush   (501) staff       (20)        0 2020-11-11 16:07:26.000000 cn2an-0.5.8/src/
--rw-r--r--   0 havetwobrush   (501) staff       (20)   113074 2020-01-17 18:48:24.000000 cn2an-0.5.8/src/cn2an-site-v0.3.11.png
--rw-r--r--   0 havetwobrush   (501) staff       (20)   112347 2019-05-23 21:19:07.000000 cn2an-0.5.8/src/cn2an-site.png
--rw-r--r--   0 havetwobrush   (501) staff       (20)    41509 2020-05-27 16:32:54.000000 cn2an-0.5.8/src/cn2an-site-v0.4.1.png
+drwxr-xr-x   0 havetwobrush   (501) staff       (20)        0 2021-01-28 09:34:14.000000 cn2an-0.5.9/
+-rw-r--r--   0 havetwobrush   (501) staff       (20)    12176 2021-01-28 09:34:14.000000 cn2an-0.5.9/PKG-INFO
+drwxr-xr-x   0 havetwobrush   (501) staff       (20)        0 2021-01-28 09:34:14.000000 cn2an-0.5.9/cn2an.egg-info/
+-rw-r--r--   0 havetwobrush   (501) staff       (20)    12176 2021-01-28 09:34:14.000000 cn2an-0.5.9/cn2an.egg-info/PKG-INFO
+-rw-r--r--   0 havetwobrush   (501) staff       (20)        1 2020-07-05 11:43:33.000000 cn2an-0.5.9/cn2an.egg-info/not-zip-safe
+-rw-r--r--   0 havetwobrush   (501) staff       (20)      484 2021-01-28 09:34:14.000000 cn2an-0.5.9/cn2an.egg-info/SOURCES.txt
+-rw-r--r--   0 havetwobrush   (501) staff       (20)       33 2021-01-28 09:34:14.000000 cn2an-0.5.9/cn2an.egg-info/requires.txt
+-rw-r--r--   0 havetwobrush   (501) staff       (20)        6 2021-01-28 09:34:14.000000 cn2an-0.5.9/cn2an.egg-info/top_level.txt
+-rw-r--r--   0 havetwobrush   (501) staff       (20)        1 2021-01-28 09:34:14.000000 cn2an-0.5.9/cn2an.egg-info/dependency_links.txt
+-rw-r--r--   0 havetwobrush   (501) staff       (20)     1062 2020-08-16 11:02:43.000000 cn2an-0.5.9/LICENSE
+-rw-r--r--   0 havetwobrush   (501) staff       (20)       32 2020-06-30 22:16:20.000000 cn2an-0.5.9/requirements.txt
+drwxr-xr-x   0 havetwobrush   (501) staff       (20)        0 2021-01-28 09:34:14.000000 cn2an-0.5.9/cn2an/
+-rw-r--r--   0 havetwobrush   (501) staff       (20)     8281 2021-01-28 09:26:20.000000 cn2an-0.5.9/cn2an/an2cn.py
+-rw-r--r--   0 havetwobrush   (501) staff       (20)    10950 2020-11-11 15:53:41.000000 cn2an-0.5.9/cn2an/cn2an.py
+-rw-r--r--   0 havetwobrush   (501) staff       (20)     1779 2020-09-23 21:37:11.000000 cn2an-0.5.9/cn2an/transform_test.py
+-rw-r--r--   0 havetwobrush   (501) staff       (20)     1356 2020-07-02 10:58:32.000000 cn2an-0.5.9/cn2an/config.yaml
+-rw-r--r--   0 havetwobrush   (501) staff       (20)      261 2021-01-28 09:22:45.000000 cn2an-0.5.9/cn2an/__init__.py
+-rw-r--r--   0 havetwobrush   (501) staff       (20)     7583 2020-08-19 05:45:27.000000 cn2an-0.5.9/cn2an/cn2an_test.py
+-rw-r--r--   0 havetwobrush   (501) staff       (20)     1530 2020-06-30 22:16:20.000000 cn2an-0.5.9/cn2an/utils.py
+-rw-r--r--   0 havetwobrush   (501) staff       (20)     5378 2020-09-23 21:36:17.000000 cn2an-0.5.9/cn2an/transform.py
+-rw-r--r--   0 havetwobrush   (501) staff       (20)      614 2020-06-30 22:16:20.000000 cn2an-0.5.9/cn2an/performance.py
+-rw-r--r--   0 havetwobrush   (501) staff       (20)     3717 2021-01-28 09:27:42.000000 cn2an-0.5.9/cn2an/an2cn_test.py
+-rw-r--r--   0 havetwobrush   (501) staff       (20)      226 2019-12-10 07:40:39.000000 cn2an-0.5.9/MANIFEST.in
+-rw-r--r--   0 havetwobrush   (501) staff       (20)     9321 2021-01-28 09:30:47.000000 cn2an-0.5.9/README.md
+-rw-r--r--   0 havetwobrush   (501) staff       (20)      956 2021-01-28 09:33:31.000000 cn2an-0.5.9/setup.py
+-rw-r--r--   0 havetwobrush   (501) staff       (20)       38 2021-01-28 09:34:14.000000 cn2an-0.5.9/setup.cfg
+drwxr-xr-x   0 havetwobrush   (501) staff       (20)        0 2021-01-28 09:34:14.000000 cn2an-0.5.9/src/
+-rw-r--r--   0 havetwobrush   (501) staff       (20)   113074 2020-01-17 18:48:24.000000 cn2an-0.5.9/src/cn2an-site-v0.3.11.png
+-rw-r--r--   0 havetwobrush   (501) staff       (20)   112347 2019-05-23 21:19:07.000000 cn2an-0.5.9/src/cn2an-site.png
+-rw-r--r--   0 havetwobrush   (501) staff       (20)    41509 2020-05-27 16:32:54.000000 cn2an-0.5.9/src/cn2an-site-v0.4.1.png
```

### Comparing `cn2an-0.5.8/PKG-INFO` & `cn2an-0.5.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cn2an
-Version: 0.5.8
+Version: 0.5.9
 Summary: Convert Chinese numerals and Arabic numerals.
 Home-page: https://github.com/Ailln/cn2an
 Author: Ailln
 Author-email: kinggreenhall@gmail.com
 License: UNKNOWN
 Description: # cn2an: Chinese Numerals To Arabic Numerals
         
@@ -16,15 +16,15 @@
         
         📦 **`cn2an`** 是一个快速转化 `中文数字` 和 `阿拉伯数字` 的工具包！
         
         [![](https://ailln.oss-cn-hangzhou.aliyuncs.com/github/cn2an/cn2an-site-latest.png)](https://www.dovolopor.com/cn2an)
         
         🔗[点击访问 DEMO](https://www.dovolopor.com/cn2an)
         
-        > 🎈 `v0.5.8 update`: fix "万亿万" => "万亿"
+        > 🎈 `v0.5.9 update`: fix "拾壹" => "壹拾壹"
         > 
         > 🎈 [`en2an`](https://github.com/Ailln/en2an): 「英文数字」和「阿拉伯数字」互转正在收集需求中！ [详情](https://github.com/Ailln/en2an)
         >
         > 🎈 [`Cn2An.jl`](https://github.com/Ailln/Cn2An.jl): Julia 语言版本已经上线，正在丰富基础功能。[详情](https://github.com/Ailln/Cn2An.jl)
         
         ## 1 功能
         
@@ -96,15 +96,15 @@
         
         ```python
         # 在文件首部引入包
         import cn2an
         
         # 查看当前版本号
         print(cn2an.__version__)
-        # 0.5.8
+        # 0.5.9
         ```
         
         ### 3.1 `中文数字` => `阿拉伯数字`
         
         > 最大支持到 `10**16`，即 `千万亿`，最小支持到 `10**-16`。
         
         ```python
@@ -263,15 +263,15 @@
             pip install -r requirements_test.txt
         
             python -m cn2an.performance
             ```
         
         - 测试结果：
         
-            | 序号 | 功能 | 执行次数 | 执行时间(平均) | 性能(次/秒)
+            | 序号 | 功能 | 执行次数 | 执行时间(万次平均) | 性能(次/秒)
             | :-: | :-: | :-: | :-: | :-: |
             |  1  | an2cn | 10000 | 0.15 | **67k** |
             |  2  | cn2an | 10000 | 0.35 | **29k** |
         
         测试时，我使用的是最大长度的测试数据！因此，大多数情况下该库的性能会更好～
         
         ## 7 许可证
```

### Comparing `cn2an-0.5.8/cn2an.egg-info/PKG-INFO` & `cn2an-0.5.9/cn2an.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cn2an
-Version: 0.5.8
+Version: 0.5.9
 Summary: Convert Chinese numerals and Arabic numerals.
 Home-page: https://github.com/Ailln/cn2an
 Author: Ailln
 Author-email: kinggreenhall@gmail.com
 License: UNKNOWN
 Description: # cn2an: Chinese Numerals To Arabic Numerals
         
@@ -16,15 +16,15 @@
         
         📦 **`cn2an`** 是一个快速转化 `中文数字` 和 `阿拉伯数字` 的工具包！
         
         [![](https://ailln.oss-cn-hangzhou.aliyuncs.com/github/cn2an/cn2an-site-latest.png)](https://www.dovolopor.com/cn2an)
         
         🔗[点击访问 DEMO](https://www.dovolopor.com/cn2an)
         
-        > 🎈 `v0.5.8 update`: fix "万亿万" => "万亿"
+        > 🎈 `v0.5.9 update`: fix "拾壹" => "壹拾壹"
         > 
         > 🎈 [`en2an`](https://github.com/Ailln/en2an): 「英文数字」和「阿拉伯数字」互转正在收集需求中！ [详情](https://github.com/Ailln/en2an)
         >
         > 🎈 [`Cn2An.jl`](https://github.com/Ailln/Cn2An.jl): Julia 语言版本已经上线，正在丰富基础功能。[详情](https://github.com/Ailln/Cn2An.jl)
         
         ## 1 功能
         
@@ -96,15 +96,15 @@
         
         ```python
         # 在文件首部引入包
         import cn2an
         
         # 查看当前版本号
         print(cn2an.__version__)
-        # 0.5.8
+        # 0.5.9
         ```
         
         ### 3.1 `中文数字` => `阿拉伯数字`
         
         > 最大支持到 `10**16`，即 `千万亿`，最小支持到 `10**-16`。
         
         ```python
@@ -263,15 +263,15 @@
             pip install -r requirements_test.txt
         
             python -m cn2an.performance
             ```
         
         - 测试结果：
         
-            | 序号 | 功能 | 执行次数 | 执行时间(平均) | 性能(次/秒)
+            | 序号 | 功能 | 执行次数 | 执行时间(万次平均) | 性能(次/秒)
             | :-: | :-: | :-: | :-: | :-: |
             |  1  | an2cn | 10000 | 0.15 | **67k** |
             |  2  | cn2an | 10000 | 0.35 | **29k** |
         
         测试时，我使用的是最大长度的测试数据！因此，大多数情况下该库的性能会更好～
         
         ## 7 许可证
```

### Comparing `cn2an-0.5.8/LICENSE` & `cn2an-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cn2an-0.5.8/cn2an/an2cn.py` & `cn2an-0.5.9/cn2an/an2cn.py`

 * *Files 4% similar despite different names*

```diff
@@ -169,16 +169,16 @@
 
                 if i > 0 and not output_an[-1] == "零":
                     output_an += numeral_list[int(d)]
 
         output_an = output_an.replace("零零", "零").replace("零万", "万").replace("零亿", "亿").replace("亿万", "亿") \
             .strip("零")
 
-        # 解决「一十几」和「壹拾几」问题
-        if output_an[:2] in ["一十", "壹拾"]:
+        # 解决「一十几」问题
+        if output_an[:2] in ["一十"]:
             output_an = output_an[1:]
 
         # 0 - 1 之间的小数
         if not output_an:
             output_an = "零"
 
         return output_an
```

### Comparing `cn2an-0.5.8/cn2an/cn2an.py` & `cn2an-0.5.9/cn2an/cn2an.py`

 * *Files identical despite different names*

### Comparing `cn2an-0.5.8/cn2an/transform_test.py` & `cn2an-0.5.9/cn2an/transform_test.py`

 * *Files identical despite different names*

### Comparing `cn2an-0.5.8/cn2an/config.yaml` & `cn2an-0.5.9/cn2an/config.yaml`

 * *Files identical despite different names*

### Comparing `cn2an-0.5.8/cn2an/cn2an_test.py` & `cn2an-0.5.9/cn2an/cn2an_test.py`

 * *Files identical despite different names*

### Comparing `cn2an-0.5.8/cn2an/utils.py` & `cn2an-0.5.9/cn2an/utils.py`

 * *Files identical despite different names*

### Comparing `cn2an-0.5.8/cn2an/transform.py` & `cn2an-0.5.9/cn2an/transform.py`

 * *Files identical despite different names*

### Comparing `cn2an-0.5.8/cn2an/performance.py` & `cn2an-0.5.9/cn2an/performance.py`

 * *Files identical despite different names*

### Comparing `cn2an-0.5.8/cn2an/an2cn_test.py` & `cn2an-0.5.9/cn2an/an2cn_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 
 
 class An2CnTest(unittest.TestCase):
     def setUp(self) -> None:
         self.input_data = {
             0: ["零", "零", "零元整", "零"],
             1: ["一", "壹", "壹元整", "一"],
-            11: ["十一", "拾壹", "拾壹元整", "一一"],
+            11: ["十一", "壹拾壹", "壹拾壹元整", "一一"],
             1000000: ["一百万", "壹佰万", "壹佰万元整", "一零零零零零零"],
             1000054: ["一百万零五十四", "壹佰万零伍拾肆", "壹佰万零伍拾肆元整", "一零零零零五四"],
             31000054: ["三千一百万零五十四", "叁仟壹佰万零伍拾肆", "叁仟壹佰万零伍拾肆元整", "三一零零零零五四"],
             9876543298765432: [
                 "九千八百七十六万五千四百三十二亿九千八百七十六万五千四百三十二",
                 "玖仟捌佰柒拾陆万伍仟肆佰叁拾贰亿玖仟捌佰柒拾陆万伍仟肆佰叁拾贰",
                 "玖仟捌佰柒拾陆万伍仟肆佰叁拾贰亿玖仟捌佰柒拾陆万伍仟肆佰叁拾贰元整",
                 "九八七六五四三二九八七六五四三二"
             ],
-            10000000000000: ["十万亿", "拾万亿", "拾万亿元整", "一零零零零零零零零零零零零零"],
+            10000000000000: ["十万亿", "壹拾万亿", "壹拾万亿元整", "一零零零零零零零零零零零零零"],
             -0: ["零", "零", "零元整", "零"],
             -1: ["负一", "负壹", "负壹元整", "负一"],
-            -11: ["负十一", "负拾壹", "负拾壹元整", "负一一"],
+            -11: ["负十一", "负壹拾壹", "负壹拾壹元整", "负一一"],
             0.000500050005005: [
                 "零点零零零五零零零五零零零五零零五",
                 "零点零零零伍零零零伍零零零伍零零伍",
                 "零元整",
                 "零点零零零五零零零五零零零五零零五"
             ],
             0.00005: ["零点零零零零五", "零点零零零零伍", "零元整", "零点零零零零五"],
@@ -38,15 +38,15 @@
             ],
             1.01: ["一点零一", "壹点零壹", "壹元零壹分", "一点零一"],
             1.2: ["一点二", "壹点贰", "壹元贰角", "一点二"],
             0.01: ["零点零一", "零点零壹", "壹分", "零点零一"],
             -0.1: ["负零点一", "负零点壹", "负壹角", "负零点一"],
             -0: ["零", "零", "零元整", "零"],
             1.10: ["一点一", "壹点壹", "壹元壹角", "一点一"],
-            12.0: ["十二点零", "拾贰点零", "拾贰元整", "一二点零"],
+            12.0: ["十二点零", "壹拾贰点零", "壹拾贰元整", "一二点零"],
             2.0: ["二点零", "贰点零", "贰元整", "二点零"],
             0.10: ["零点一", "零点壹", "壹角", "零点一"]
         }
 
         self.error_input_data = [
             "123.1.1",
             "0.1零"
```

### Comparing `cn2an-0.5.8/README.md` & `cn2an-0.5.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 📦 **`cn2an`** 是一个快速转化 `中文数字` 和 `阿拉伯数字` 的工具包！
 
 [![](https://ailln.oss-cn-hangzhou.aliyuncs.com/github/cn2an/cn2an-site-latest.png)](https://www.dovolopor.com/cn2an)
 
 🔗[点击访问 DEMO](https://www.dovolopor.com/cn2an)
 
-> 🎈 `v0.5.8 update`: fix "万亿万" => "万亿"
+> 🎈 `v0.5.9 update`: fix "拾壹" => "壹拾壹"
 > 
 > 🎈 [`en2an`](https://github.com/Ailln/en2an): 「英文数字」和「阿拉伯数字」互转正在收集需求中！ [详情](https://github.com/Ailln/en2an)
 >
 > 🎈 [`Cn2An.jl`](https://github.com/Ailln/Cn2An.jl): Julia 语言版本已经上线，正在丰富基础功能。[详情](https://github.com/Ailln/Cn2An.jl)
 
 ## 1 功能
 
@@ -88,15 +88,15 @@
 
 ```python
 # 在文件首部引入包
 import cn2an
 
 # 查看当前版本号
 print(cn2an.__version__)
-# 0.5.8
+# 0.5.9
 ```
 
 ### 3.1 `中文数字` => `阿拉伯数字`
 
 > 最大支持到 `10**16`，即 `千万亿`，最小支持到 `10**-16`。
 
 ```python
@@ -255,15 +255,15 @@
     pip install -r requirements_test.txt
 
     python -m cn2an.performance
     ```
 
 - 测试结果：
 
-    | 序号 | 功能 | 执行次数 | 执行时间(平均) | 性能(次/秒)
+    | 序号 | 功能 | 执行次数 | 执行时间(万次平均) | 性能(次/秒)
     | :-: | :-: | :-: | :-: | :-: |
     |  1  | an2cn | 10000 | 0.15 | **67k** |
     |  2  | cn2an | 10000 | 0.35 | **29k** |
 
 测试时，我使用的是最大长度的测试数据！因此，大多数情况下该库的性能会更好～
 
 ## 7 许可证
```

### Comparing `cn2an-0.5.8/setup.py` & `cn2an-0.5.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 if sys.version_info[:2] < (3, 6):
     raise RuntimeError('cn2an requires Python 3.6 or later')
 
 setup(
     name="cn2an",
-    version="0.5.8",
+    version="0.5.9",
     author="Ailln",
     author_email="kinggreenhall@gmail.com",
     url="https://github.com/Ailln/cn2an",
     packages=find_packages(),
     include_package_data=True,
     install_requires=open("./requirements.txt", "r", encoding="utf-8").read().splitlines(),
     description="Convert Chinese numerals and Arabic numerals.",
```

### Comparing `cn2an-0.5.8/src/cn2an-site-v0.3.11.png` & `cn2an-0.5.9/src/cn2an-site-v0.3.11.png`

 * *Files identical despite different names*

### Comparing `cn2an-0.5.8/src/cn2an-site.png` & `cn2an-0.5.9/src/cn2an-site.png`

 * *Files identical despite different names*

### Comparing `cn2an-0.5.8/src/cn2an-site-v0.4.1.png` & `cn2an-0.5.9/src/cn2an-site-v0.4.1.png`

 * *Files identical despite different names*

