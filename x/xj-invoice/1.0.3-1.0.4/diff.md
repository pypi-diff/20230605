# Comparing `tmp/xj_invoice-1.0.3.tar.gz` & `tmp/xj_invoice-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xj_invoice-1.0.3.tar", last modified: Mon Jun  5 01:39:03 2023, max compression
+gzip compressed data, was "xj_invoice-1.0.4.tar", last modified: Mon Jun  5 01:46:09 2023, max compression
```

## Comparing `xj_invoice-1.0.3.tar` & `xj_invoice-1.0.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 01:39:03.169008 xj_invoice-1.0.3/
--rw-rw-rw-   0        0        0     1616 2023-06-05 01:39:03.168012 xj_invoice-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1354 2023-05-29 09:33:56.000000 xj_invoice-1.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-05 01:39:03.169008 xj_invoice-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      904 2023-06-05 01:38:36.000000 xj_invoice-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-05 01:39:03.130345 xj_invoice-1.0.3/xj_invoice/
--rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_invoice-1.0.3/xj_invoice/__init__.py
--rw-rw-rw-   0        0        0     1571 2023-05-29 08:07:17.000000 xj_invoice-1.0.3/xj_invoice/admin.py
-drwxrwxrwx   0        0        0        0 2023-06-05 01:39:03.144897 xj_invoice-1.0.3/xj_invoice/apis/
--rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_invoice-1.0.3/xj_invoice/apis/__init__.py
--rw-rw-rw-   0        0        0     3412 2023-05-31 09:09:10.000000 xj_invoice-1.0.3/xj_invoice/apis/invoice_apis.py
--rw-rw-rw-   0        0        0     1128 2023-06-05 01:36:21.000000 xj_invoice-1.0.3/xj_invoice/apis/invoice_type_apis.py
--rw-rw-rw-   0        0        0     2133 2022-08-16 02:23:15.000000 xj_invoice-1.0.3/xj_invoice/apis/middleware.py
--rw-rw-rw-   0        0        0     4180 2022-08-19 03:17:51.000000 xj_invoice-1.0.3/xj_invoice/apis/router.py
--rw-rw-rw-   0        0        0      204 2023-05-29 04:04:21.000000 xj_invoice-1.0.3/xj_invoice/apps.py
--rw-rw-rw-   0        0        0    18443 2023-06-02 06:58:32.000000 xj_invoice-1.0.3/xj_invoice/models.py
--rw-rw-rw-   0        0        0      636 2023-06-02 07:02:38.000000 xj_invoice-1.0.3/xj_invoice/service_register.py
-drwxrwxrwx   0        0        0        0 2023-06-05 01:39:03.151446 xj_invoice-1.0.3/xj_invoice/services/
--rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_invoice-1.0.3/xj_invoice/services/__init__.py
--rw-rw-rw-   0        0        0     7754 2023-05-29 05:59:27.000000 xj_invoice-1.0.3/xj_invoice/services/invoice_extend_service.py
--rw-rw-rw-   0        0        0    10537 2023-06-02 07:48:34.000000 xj_invoice-1.0.3/xj_invoice/services/invoice_service.py
--rw-rw-rw-   0        0        0      304 2023-06-05 01:37:37.000000 xj_invoice-1.0.3/xj_invoice/services/invoice_type_service.py
--rw-rw-rw-   0        0        0       63 2022-08-16 02:23:15.000000 xj_invoice-1.0.3/xj_invoice/tests.py
--rw-rw-rw-   0        0        0      609 2023-06-05 01:37:02.000000 xj_invoice-1.0.3/xj_invoice/urls.py
-drwxrwxrwx   0        0        0        0 2023-06-05 01:39:03.167003 xj_invoice-1.0.3/xj_invoice/utils/
--rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_invoice-1.0.3/xj_invoice/utils/__init__.py
--rw-rw-rw-   0        0        0     1011 2023-03-06 08:50:03.000000 xj_invoice-1.0.3/xj_invoice/utils/custom_response.py
--rw-rw-rw-   0        0        0    31480 2023-05-30 05:45:25.000000 xj_invoice-1.0.3/xj_invoice/utils/custom_tool.py
--rw-rw-rw-   0        0        0      988 2022-08-29 07:52:36.000000 xj_invoice-1.0.3/xj_invoice/utils/j_config.py
--rw-rw-rw-   0        0        0      429 2022-10-17 01:16:10.000000 xj_invoice-1.0.3/xj_invoice/utils/j_dict.py
--rw-rw-rw-   0        0        0      660 2022-12-08 07:49:05.000000 xj_invoice-1.0.3/xj_invoice/utils/join_list.py
--rw-rw-rw-   0        0        0     4634 2022-08-24 03:27:40.000000 xj_invoice-1.0.3/xj_invoice/utils/jt.py
--rw-rw-rw-   0        0        0     7314 2022-08-22 01:46:29.000000 xj_invoice-1.0.3/xj_invoice/utils/model_handle.py
--rw-rw-rw-   0        0        0     4154 2023-04-06 03:09:14.000000 xj_invoice-1.0.3/xj_invoice/utils/user_wrapper.py
--rw-rw-rw-   0        0        0     3661 2022-08-16 02:23:15.000000 xj_invoice-1.0.3/xj_invoice/views.py
-drwxrwxrwx   0        0        0        0 2023-06-05 01:39:03.137438 xj_invoice-1.0.3/xj_invoice.egg-info/
--rw-rw-rw-   0        0        0     1616 2023-06-05 01:39:03.000000 xj_invoice-1.0.3/xj_invoice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      913 2023-06-05 01:39:03.000000 xj_invoice-1.0.3/xj_invoice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 01:39:03.000000 xj_invoice-1.0.3/xj_invoice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-05 01:39:03.000000 xj_invoice-1.0.3/xj_invoice.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-05 01:46:09.808264 xj_invoice-1.0.4/
+-rw-rw-rw-   0        0        0     1616 2023-06-05 01:46:09.807290 xj_invoice-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1354 2023-05-29 09:33:56.000000 xj_invoice-1.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-05 01:46:09.808264 xj_invoice-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      904 2023-06-05 01:46:07.000000 xj_invoice-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 01:46:09.766352 xj_invoice-1.0.4/xj_invoice/
+-rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_invoice-1.0.4/xj_invoice/__init__.py
+-rw-rw-rw-   0        0        0     1571 2023-05-29 08:07:17.000000 xj_invoice-1.0.4/xj_invoice/admin.py
+drwxrwxrwx   0        0        0        0 2023-06-05 01:46:09.782514 xj_invoice-1.0.4/xj_invoice/apis/
+-rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_invoice-1.0.4/xj_invoice/apis/__init__.py
+-rw-rw-rw-   0        0        0     3412 2023-05-31 09:09:10.000000 xj_invoice-1.0.4/xj_invoice/apis/invoice_apis.py
+-rw-rw-rw-   0        0        0     1128 2023-06-05 01:36:21.000000 xj_invoice-1.0.4/xj_invoice/apis/invoice_type_apis.py
+-rw-rw-rw-   0        0        0     2133 2022-08-16 02:23:15.000000 xj_invoice-1.0.4/xj_invoice/apis/middleware.py
+-rw-rw-rw-   0        0        0     4180 2022-08-19 03:17:51.000000 xj_invoice-1.0.4/xj_invoice/apis/router.py
+-rw-rw-rw-   0        0        0      204 2023-05-29 04:04:21.000000 xj_invoice-1.0.4/xj_invoice/apps.py
+-rw-rw-rw-   0        0        0    18443 2023-06-02 06:58:32.000000 xj_invoice-1.0.4/xj_invoice/models.py
+-rw-rw-rw-   0        0        0      636 2023-06-02 07:02:38.000000 xj_invoice-1.0.4/xj_invoice/service_register.py
+drwxrwxrwx   0        0        0        0 2023-06-05 01:46:09.790173 xj_invoice-1.0.4/xj_invoice/services/
+-rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_invoice-1.0.4/xj_invoice/services/__init__.py
+-rw-rw-rw-   0        0        0     7754 2023-05-29 05:59:27.000000 xj_invoice-1.0.4/xj_invoice/services/invoice_extend_service.py
+-rw-rw-rw-   0        0        0    10713 2023-06-05 01:45:44.000000 xj_invoice-1.0.4/xj_invoice/services/invoice_service.py
+-rw-rw-rw-   0        0        0      304 2023-06-05 01:37:37.000000 xj_invoice-1.0.4/xj_invoice/services/invoice_type_service.py
+-rw-rw-rw-   0        0        0       63 2022-08-16 02:23:15.000000 xj_invoice-1.0.4/xj_invoice/tests.py
+-rw-rw-rw-   0        0        0      609 2023-06-05 01:37:02.000000 xj_invoice-1.0.4/xj_invoice/urls.py
+drwxrwxrwx   0        0        0        0 2023-06-05 01:46:09.805291 xj_invoice-1.0.4/xj_invoice/utils/
+-rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_invoice-1.0.4/xj_invoice/utils/__init__.py
+-rw-rw-rw-   0        0        0     1011 2023-03-06 08:50:03.000000 xj_invoice-1.0.4/xj_invoice/utils/custom_response.py
+-rw-rw-rw-   0        0        0    31480 2023-05-30 05:45:25.000000 xj_invoice-1.0.4/xj_invoice/utils/custom_tool.py
+-rw-rw-rw-   0        0        0      988 2022-08-29 07:52:36.000000 xj_invoice-1.0.4/xj_invoice/utils/j_config.py
+-rw-rw-rw-   0        0        0      429 2022-10-17 01:16:10.000000 xj_invoice-1.0.4/xj_invoice/utils/j_dict.py
+-rw-rw-rw-   0        0        0      660 2022-12-08 07:49:05.000000 xj_invoice-1.0.4/xj_invoice/utils/join_list.py
+-rw-rw-rw-   0        0        0     4634 2022-08-24 03:27:40.000000 xj_invoice-1.0.4/xj_invoice/utils/jt.py
+-rw-rw-rw-   0        0        0     7314 2022-08-22 01:46:29.000000 xj_invoice-1.0.4/xj_invoice/utils/model_handle.py
+-rw-rw-rw-   0        0        0     4154 2023-04-06 03:09:14.000000 xj_invoice-1.0.4/xj_invoice/utils/user_wrapper.py
+-rw-rw-rw-   0        0        0     3661 2022-08-16 02:23:15.000000 xj_invoice-1.0.4/xj_invoice/views.py
+drwxrwxrwx   0        0        0        0 2023-06-05 01:46:09.773823 xj_invoice-1.0.4/xj_invoice.egg-info/
+-rw-rw-rw-   0        0        0     1616 2023-06-05 01:46:09.000000 xj_invoice-1.0.4/xj_invoice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      913 2023-06-05 01:46:09.000000 xj_invoice-1.0.4/xj_invoice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 01:46:09.000000 xj_invoice-1.0.4/xj_invoice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-05 01:46:09.000000 xj_invoice-1.0.4/xj_invoice.egg-info/top_level.txt
```

### Comparing `xj_invoice-1.0.3/PKG-INFO` & `xj_invoice-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xj_invoice
-Version: 1.0.3
+Version: 1.0.4
 Summary: 发票模块
 Author: 高栋天
 Author-email: 1499593644@qq.com
 Maintainer: ['高栋天']
 Maintainer-email: angelvy@foxmail.com
 License: apache 3.0
 Description-Content-Type: text/markdown
```

### Comparing `xj_invoice-1.0.3/README.md` & `xj_invoice-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.3/setup.py` & `xj_invoice-1.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf8') as fp:
     log_desc = fp.read()
 
 setup(
     name='xj_invoice',  # 模块名称
-    version='1.0.3',  # 模块版本
+    version='1.0.4',  # 模块版本
     description='发票模块',  # 项目 摘要描述
     long_description=log_desc,  # 项目描述
     long_description_content_type="text/markdown",  # md文件，markdown格式
     author='高栋天',  # 作者
     author_email='1499593644@qq.com',  # 作者邮箱
     maintainer=["高栋天"],  # 维护者
     maintainer_email="angelvy@foxmail.com",  # 维护者的邮箱地址
```

### Comparing `xj_invoice-1.0.3/xj_invoice/admin.py` & `xj_invoice-1.0.4/xj_invoice/admin.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.3/xj_invoice/apis/invoice_apis.py` & `xj_invoice-1.0.4/xj_invoice/apis/invoice_apis.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.3/xj_invoice/apis/invoice_type_apis.py` & `xj_invoice-1.0.4/xj_invoice/apis/invoice_type_apis.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.3/xj_invoice/apis/middleware.py` & `xj_invoice-1.0.4/xj_invoice/apis/middleware.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.3/xj_invoice/apis/router.py` & `xj_invoice-1.0.4/xj_invoice/apis/router.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.3/xj_invoice/models.py` & `xj_invoice-1.0.4/xj_invoice/models.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.3/xj_invoice/service_register.py` & `xj_invoice-1.0.4/xj_invoice/service_register.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.3/xj_invoice/services/invoice_extend_service.py` & `xj_invoice-1.0.4/xj_invoice/services/invoice_extend_service.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.3/xj_invoice/services/invoice_service.py` & `xj_invoice-1.0.4/xj_invoice/services/invoice_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,15 +233,19 @@
         if extend_list:
             data = JoinList(data, extend_list, "invoice_id", "invoice_id").join()
 
         return {'size': int(size), 'page': int(page + 1), 'total': total, 'list': data, }, None
 
     @staticmethod
     def detail(invoice_id):
+        if not invoice_id:
+            return None, "发票id不能为空"
         invoice = Invoice.objects.filter(id=invoice_id).first()
+        if not invoice:
+            return None, "无法找到要修改数据，请检查参数"
         data = model_to_dict(invoice)
         extend_id_list = [data.get("id", None)]
         extend_list, err = InvoiceExtendService.get_extend_info(extend_id_list)
         if extend_list:
             data.update(extend_list[0])
         return data, None
```

### Comparing `xj_invoice-1.0.3/xj_invoice/urls.py` & `xj_invoice-1.0.4/xj_invoice/urls.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.3/xj_invoice/utils/custom_response.py` & `xj_invoice-1.0.4/xj_invoice/utils/custom_response.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.3/xj_invoice/utils/custom_tool.py` & `xj_invoice-1.0.4/xj_invoice/utils/custom_tool.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.3/xj_invoice/utils/j_config.py` & `xj_invoice-1.0.4/xj_invoice/utils/j_config.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.3/xj_invoice/utils/join_list.py` & `xj_invoice-1.0.4/xj_invoice/utils/join_list.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.3/xj_invoice/utils/jt.py` & `xj_invoice-1.0.4/xj_invoice/utils/jt.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.3/xj_invoice/utils/model_handle.py` & `xj_invoice-1.0.4/xj_invoice/utils/model_handle.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.3/xj_invoice/utils/user_wrapper.py` & `xj_invoice-1.0.4/xj_invoice/utils/user_wrapper.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.3/xj_invoice/views.py` & `xj_invoice-1.0.4/xj_invoice/views.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.3/xj_invoice.egg-info/PKG-INFO` & `xj_invoice-1.0.4/xj_invoice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xj-invoice
-Version: 1.0.3
+Version: 1.0.4
 Summary: 发票模块
 Author: 高栋天
 Author-email: 1499593644@qq.com
 Maintainer: ['高栋天']
 Maintainer-email: angelvy@foxmail.com
 License: apache 3.0
 Description-Content-Type: text/markdown
```

### Comparing `xj_invoice-1.0.3/xj_invoice.egg-info/SOURCES.txt` & `xj_invoice-1.0.4/xj_invoice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

