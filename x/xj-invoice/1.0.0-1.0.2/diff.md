# Comparing `tmp/xj_invoice-1.0.0.tar.gz` & `tmp/xj_invoice-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\xj_invoice-1.0.0.tar", last modified: Tue May 30 07:39:37 2023, max compression
+gzip compressed data, was "xj_invoice-1.0.2.tar", last modified: Mon Jun  5 01:13:22 2023, max compression
```

## Comparing `xj_invoice-1.0.0.tar` & `xj_invoice-1.0.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 07:39:37.000000 xj_invoice-1.0.0/
--rw-rw-rw-   0        0        0     1980 2023-05-30 07:39:37.000000 xj_invoice-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1354 2023-05-29 09:33:56.000000 xj_invoice-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-30 07:39:37.000000 xj_invoice-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      904 2023-05-29 04:05:13.000000 xj_invoice-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-30 07:39:37.000000 xj_invoice-1.0.0/xj_invoice/
--rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_invoice-1.0.0/xj_invoice/__init__.py
--rw-rw-rw-   0        0        0     1571 2023-05-29 08:07:17.000000 xj_invoice-1.0.0/xj_invoice/admin.py
-drwxrwxrwx   0        0        0        0 2023-05-30 07:39:37.000000 xj_invoice-1.0.0/xj_invoice/apis/
--rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_invoice-1.0.0/xj_invoice/apis/__init__.py
--rw-rw-rw-   0        0        0     3421 2023-05-30 02:31:22.000000 xj_invoice-1.0.0/xj_invoice/apis/invoice_apis.py
--rw-rw-rw-   0        0        0     2133 2022-08-16 02:23:15.000000 xj_invoice-1.0.0/xj_invoice/apis/middleware.py
--rw-rw-rw-   0        0        0     4180 2022-08-19 03:17:51.000000 xj_invoice-1.0.0/xj_invoice/apis/router.py
--rw-rw-rw-   0        0        0      204 2023-05-29 04:04:21.000000 xj_invoice-1.0.0/xj_invoice/apps.py
--rw-rw-rw-   0        0        0    18444 2023-05-29 08:06:46.000000 xj_invoice-1.0.0/xj_invoice/models.py
--rw-rw-rw-   0        0        0      695 2023-05-19 05:42:53.000000 xj_invoice-1.0.0/xj_invoice/search_indexes.py
-drwxrwxrwx   0        0        0        0 2023-05-30 07:39:37.000000 xj_invoice-1.0.0/xj_invoice/services/
--rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_invoice-1.0.0/xj_invoice/services/__init__.py
--rw-rw-rw-   0        0        0     7754 2023-05-29 05:59:27.000000 xj_invoice-1.0.0/xj_invoice/services/invoice_extend_service.py
--rw-rw-rw-   0        0        0    10196 2023-05-30 03:13:59.000000 xj_invoice-1.0.0/xj_invoice/services/invoice_service.py
--rw-rw-rw-   0        0        0       63 2022-08-16 02:23:15.000000 xj_invoice-1.0.0/xj_invoice/tests.py
--rw-rw-rw-   0        0        0      372 2023-05-30 02:28:27.000000 xj_invoice-1.0.0/xj_invoice/urls.py
-drwxrwxrwx   0        0        0        0 2023-05-30 07:39:37.000000 xj_invoice-1.0.0/xj_invoice/utils/
--rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_invoice-1.0.0/xj_invoice/utils/__init__.py
--rw-rw-rw-   0        0        0     1011 2023-03-06 08:50:03.000000 xj_invoice-1.0.0/xj_invoice/utils/custom_response.py
--rw-rw-rw-   0        0        0    31480 2023-05-30 05:45:25.000000 xj_invoice-1.0.0/xj_invoice/utils/custom_tool.py
--rw-rw-rw-   0        0        0      988 2022-08-29 07:52:36.000000 xj_invoice-1.0.0/xj_invoice/utils/j_config.py
--rw-rw-rw-   0        0        0      429 2022-10-17 01:16:10.000000 xj_invoice-1.0.0/xj_invoice/utils/j_dict.py
--rw-rw-rw-   0        0        0      660 2022-12-08 07:49:05.000000 xj_invoice-1.0.0/xj_invoice/utils/join_list.py
--rw-rw-rw-   0        0        0     4634 2022-08-24 03:27:40.000000 xj_invoice-1.0.0/xj_invoice/utils/jt.py
--rw-rw-rw-   0        0        0     7314 2022-08-22 01:46:29.000000 xj_invoice-1.0.0/xj_invoice/utils/model_handle.py
--rw-rw-rw-   0        0        0     4154 2023-04-06 03:09:14.000000 xj_invoice-1.0.0/xj_invoice/utils/user_wrapper.py
--rw-rw-rw-   0        0        0     3661 2022-08-16 02:23:15.000000 xj_invoice-1.0.0/xj_invoice/views.py
-drwxrwxrwx   0        0        0        0 2023-05-30 07:39:37.000000 xj_invoice-1.0.0/xj_invoice.egg-info/
--rw-rw-rw-   0        0        0     1980 2023-05-30 07:39:36.000000 xj_invoice-1.0.0/xj_invoice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      830 2023-05-30 07:39:37.000000 xj_invoice-1.0.0/xj_invoice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 07:39:36.000000 xj_invoice-1.0.0/xj_invoice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-30 07:39:36.000000 xj_invoice-1.0.0/xj_invoice.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-05 01:13:22.489232 xj_invoice-1.0.2/
+-rw-rw-rw-   0        0        0     1616 2023-06-05 01:13:22.489232 xj_invoice-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1354 2023-05-29 09:33:56.000000 xj_invoice-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-05 01:13:22.489232 xj_invoice-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      904 2023-06-02 07:04:03.000000 xj_invoice-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 01:13:22.454225 xj_invoice-1.0.2/xj_invoice/
+-rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_invoice-1.0.2/xj_invoice/__init__.py
+-rw-rw-rw-   0        0        0     1571 2023-05-29 08:07:17.000000 xj_invoice-1.0.2/xj_invoice/admin.py
+drwxrwxrwx   0        0        0        0 2023-06-05 01:13:22.467254 xj_invoice-1.0.2/xj_invoice/apis/
+-rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_invoice-1.0.2/xj_invoice/apis/__init__.py
+-rw-rw-rw-   0        0        0     3412 2023-05-31 09:09:10.000000 xj_invoice-1.0.2/xj_invoice/apis/invoice_apis.py
+-rw-rw-rw-   0        0        0     2133 2022-08-16 02:23:15.000000 xj_invoice-1.0.2/xj_invoice/apis/middleware.py
+-rw-rw-rw-   0        0        0     4180 2022-08-19 03:17:51.000000 xj_invoice-1.0.2/xj_invoice/apis/router.py
+-rw-rw-rw-   0        0        0      204 2023-05-29 04:04:21.000000 xj_invoice-1.0.2/xj_invoice/apps.py
+-rw-rw-rw-   0        0        0    18443 2023-06-02 06:58:32.000000 xj_invoice-1.0.2/xj_invoice/models.py
+-rw-rw-rw-   0        0        0      636 2023-06-02 07:02:38.000000 xj_invoice-1.0.2/xj_invoice/service_register.py
+drwxrwxrwx   0        0        0        0 2023-06-05 01:13:22.472254 xj_invoice-1.0.2/xj_invoice/services/
+-rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_invoice-1.0.2/xj_invoice/services/__init__.py
+-rw-rw-rw-   0        0        0     7754 2023-05-29 05:59:27.000000 xj_invoice-1.0.2/xj_invoice/services/invoice_extend_service.py
+-rw-rw-rw-   0        0        0    10537 2023-06-02 07:48:34.000000 xj_invoice-1.0.2/xj_invoice/services/invoice_service.py
+-rw-rw-rw-   0        0        0       63 2022-08-16 02:23:15.000000 xj_invoice-1.0.2/xj_invoice/tests.py
+-rw-rw-rw-   0        0        0      492 2023-06-02 07:22:08.000000 xj_invoice-1.0.2/xj_invoice/urls.py
+drwxrwxrwx   0        0        0        0 2023-06-05 01:13:22.487231 xj_invoice-1.0.2/xj_invoice/utils/
+-rw-rw-rw-   0        0        0        0 2022-08-16 02:23:15.000000 xj_invoice-1.0.2/xj_invoice/utils/__init__.py
+-rw-rw-rw-   0        0        0     1011 2023-03-06 08:50:03.000000 xj_invoice-1.0.2/xj_invoice/utils/custom_response.py
+-rw-rw-rw-   0        0        0    31480 2023-05-30 05:45:25.000000 xj_invoice-1.0.2/xj_invoice/utils/custom_tool.py
+-rw-rw-rw-   0        0        0      988 2022-08-29 07:52:36.000000 xj_invoice-1.0.2/xj_invoice/utils/j_config.py
+-rw-rw-rw-   0        0        0      429 2022-10-17 01:16:10.000000 xj_invoice-1.0.2/xj_invoice/utils/j_dict.py
+-rw-rw-rw-   0        0        0      660 2022-12-08 07:49:05.000000 xj_invoice-1.0.2/xj_invoice/utils/join_list.py
+-rw-rw-rw-   0        0        0     4634 2022-08-24 03:27:40.000000 xj_invoice-1.0.2/xj_invoice/utils/jt.py
+-rw-rw-rw-   0        0        0     7314 2022-08-22 01:46:29.000000 xj_invoice-1.0.2/xj_invoice/utils/model_handle.py
+-rw-rw-rw-   0        0        0     4154 2023-04-06 03:09:14.000000 xj_invoice-1.0.2/xj_invoice/utils/user_wrapper.py
+-rw-rw-rw-   0        0        0     3661 2022-08-16 02:23:15.000000 xj_invoice-1.0.2/xj_invoice/views.py
+drwxrwxrwx   0        0        0        0 2023-06-05 01:13:22.460259 xj_invoice-1.0.2/xj_invoice.egg-info/
+-rw-rw-rw-   0        0        0     1616 2023-06-05 01:13:22.000000 xj_invoice-1.0.2/xj_invoice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      832 2023-06-05 01:13:22.000000 xj_invoice-1.0.2/xj_invoice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 01:13:22.000000 xj_invoice-1.0.2/xj_invoice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-05 01:13:22.000000 xj_invoice-1.0.2/xj_invoice.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `xj_invoice-1.0.0/PKG-INFO` & `xj_invoice-1.0.2/xj_invoice.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,52 +1,50 @@
 Metadata-Version: 2.1
-Name: xj_invoice
-Version: 1.0.0
+Name: xj-invoice
+Version: 1.0.2
 Summary: 发票模块
-Home-page: UNKNOWN
 Author: 高栋天
 Author-email: 1499593644@qq.com
 Maintainer: ['高栋天']
 Maintainer-email: angelvy@foxmail.com
 License: apache 3.0
-Description: # xj-invoice
-        
-        #### 介绍
-        {**以下是 Gitee 平台说明，您可以替换此简介**
-        Gitee 是 OSCHINA 推出的基于 Git 的代码托管平台（同时支持 SVN）。专为开发者提供稳定、高效、安全的云端软件开发协作平台
-        无论是个人、团队、或是企业，都能够用 Gitee 实现代码托管、项目管理、协作开发。企业项目请看 [https://gitee.com/enterprises](https://gitee.com/enterprises)}
-        
-        #### 软件架构
-        软件架构说明
-        
-        
-        #### 安装教程
-        
-        1.  xxxx
-        2.  xxxx
-        3.  xxxx
-        
-        #### 使用说明
-        
-        1.  xxxx
-        2.  xxxx
-        3.  xxxx
-        
-        #### 参与贡献
-        
-        1.  Fork 本仓库
-        2.  新建 Feat_xxx 分支
-        3.  提交代码
-        4.  新建 Pull Request
-        
-        
-        #### 特技
-        
-        1.  使用 Readme\_XXX.md 来支持不同的语言，例如 Readme\_en.md, Readme\_zh.md
-        2.  Gitee 官方博客 [blog.gitee.com](https://blog.gitee.com)
-        3.  你可以 [https://gitee.com/explore](https://gitee.com/explore) 这个地址来了解 Gitee 上的优秀开源项目
-        4.  [GVP](https://gitee.com/gvp) 全称是 Gitee 最有价值开源项目，是综合评定出的优秀开源项目
-        5.  Gitee 官方提供的使用手册 [https://gitee.com/help](https://gitee.com/help)
-        6.  Gitee 封面人物是一档用来展示 Gitee 会员风采的栏目 [https://gitee.com/gitee-stars/](https://gitee.com/gitee-stars/)
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+
+# xj-invoice
+
+#### 介绍
+{**以下是 Gitee 平台说明，您可以替换此简介**
+Gitee 是 OSCHINA 推出的基于 Git 的代码托管平台（同时支持 SVN）。专为开发者提供稳定、高效、安全的云端软件开发协作平台
+无论是个人、团队、或是企业，都能够用 Gitee 实现代码托管、项目管理、协作开发。企业项目请看 [https://gitee.com/enterprises](https://gitee.com/enterprises)}
+
+#### 软件架构
+软件架构说明
+
+
+#### 安装教程
+
+1.  xxxx
+2.  xxxx
+3.  xxxx
+
+#### 使用说明
+
+1.  xxxx
+2.  xxxx
+3.  xxxx
+
+#### 参与贡献
+
+1.  Fork 本仓库
+2.  新建 Feat_xxx 分支
+3.  提交代码
+4.  新建 Pull Request
+
+
+#### 特技
+
+1.  使用 Readme\_XXX.md 来支持不同的语言，例如 Readme\_en.md, Readme\_zh.md
+2.  Gitee 官方博客 [blog.gitee.com](https://blog.gitee.com)
+3.  你可以 [https://gitee.com/explore](https://gitee.com/explore) 这个地址来了解 Gitee 上的优秀开源项目
+4.  [GVP](https://gitee.com/gvp) 全称是 Gitee 最有价值开源项目，是综合评定出的优秀开源项目
+5.  Gitee 官方提供的使用手册 [https://gitee.com/help](https://gitee.com/help)
+6.  Gitee 封面人物是一档用来展示 Gitee 会员风采的栏目 [https://gitee.com/gitee-stars/](https://gitee.com/gitee-stars/)
```

### Comparing `xj_invoice-1.0.0/README.md` & `xj_invoice-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.0/setup.py` & `xj_invoice-1.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf8') as fp:
     log_desc = fp.read()
 
 setup(
     name='xj_invoice',  # 模块名称
-    version='1.0.0',  # 模块版本
+    version='1.0.2',  # 模块版本
     description='发票模块',  # 项目 摘要描述
     long_description=log_desc,  # 项目描述
     long_description_content_type="text/markdown",  # md文件，markdown格式
     author='高栋天',  # 作者
     author_email='1499593644@qq.com',  # 作者邮箱
     maintainer=["高栋天"],  # 维护者
     maintainer_email="angelvy@foxmail.com",  # 维护者的邮箱地址
```

### Comparing `xj_invoice-1.0.0/xj_invoice/admin.py` & `xj_invoice-1.0.2/xj_invoice/admin.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.0/xj_invoice/apis/invoice_apis.py` & `xj_invoice-1.0.2/xj_invoice/apis/invoice_apis.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     @request_params_wrapper
     def list(self, *args, user_info, request_params, **kwargs, ):
         params = request_params
         # ============   字段验证处理 start ============
         user_id = user_info.get("user_id")
         params.setdefault("user_id", user_id)  # 用户ID
 
-        invoice_set, err = InvoiceService.list(params, user_id)
+        invoice_set, err = InvoiceService.list(params)
 
         if err is None:
             return util_response(data=invoice_set)
 
         return util_response(err=47767, msg=err)
 
     # 发票详细
```

### Comparing `xj_invoice-1.0.0/xj_invoice/apis/middleware.py` & `xj_invoice-1.0.2/xj_invoice/apis/middleware.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.0/xj_invoice/apis/router.py` & `xj_invoice-1.0.2/xj_invoice/apis/router.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.0/xj_invoice/models.py` & `xj_invoice-1.0.2/xj_invoice/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 
 
 class Invoice(models.Model):
     """ 8、*invoice_invoice 发票表 """
     id = models.AutoField(verbose_name='平台ID', primary_key=True, help_text='必填。自动生成。')
     user_id = models.IntegerField(verbose_name='开票用户', primary_key=False, help_text='')
     thread_id = models.IntegerField(verbose_name='合同ID（信息id）', primary_key=False, help_text='')
-    finance_id_list = models.CharField(verbose_name='财务列表', max_length=128, blank=True, null=True,
+    enroll_id_list = models.CharField(verbose_name='报名列表', max_length=128, blank=True, null=True,
                                        db_index=True,
-                                       help_text='要开票的财务表数据')
+                                       help_text='要开票的报名表数据')
     invoice_time = models.DateTimeField(verbose_name='开票时间', default=timezone.now, help_text='')
     invoice_type = models.ForeignKey(InvoiceType, verbose_name='发票类型', on_delete=models.DO_NOTHING, help_text='')
     invoice_number = models.CharField(verbose_name='发票号码', max_length=128, unique=True, blank=True, null=True,
                                       db_index=True,
                                       help_text='')
     invoice_price = models.DecimalField(verbose_name='开票金额', max_digits=32, decimal_places=2, blank=True, null=True)
     tax_rate = models.CharField(verbose_name='发票税率', max_length=128, blank=True, null=True, help_text='')
```

### Comparing `xj_invoice-1.0.0/xj_invoice/services/invoice_extend_service.py` & `xj_invoice-1.0.2/xj_invoice/services/invoice_extend_service.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.0/xj_invoice/services/invoice_service.py` & `xj_invoice-1.0.2/xj_invoice/services/invoice_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         try:
             main_form_data = format_params_handle(
                 param_dict=params.copy(),
                 is_remove_empty=True,
                 filter_filed_list=[
                     "user_id|int",
                     "thread_id|int",
-                    "finance_id_list",
+                    "enroll_id_list",
                     "invoice_time|date",
                     "invoice_type_id|int",
                     "invoice_price|float",
                     "invoice_number",
                     "tax_rate",
                     "invoice_tax",
                     "invoice_untaxed",
@@ -120,15 +120,15 @@
             params = format_params_handle(
                 param_dict=params,
                 is_validate_type=True,
                 is_remove_empty=True,
                 filter_filed_list=[
                     "user_id|int",
                     "thread_id|int",
-                    "finance_id_list",
+                    "enroll_id_list",
                     "invoice_time|date",
                     "invoice_type_id|int",
                     "invoice_price|float",
                     "invoice_number",
                     "tax_rate",
                     "invoice_tax",
                     "invoice_untaxed",
@@ -165,20 +165,22 @@
         try:
             invoice_obj.update(**params)
         except Exception as e:
             return None, "修改异常:" + str(e)
         return invoice_obj.first().to_json(), None
 
     @staticmethod
-    def list(params, user_id):
+    def list(params):
 
         page = int(params['page']) - 1 if 'page' in params else 0
         size = int(params['size']) if 'size' in params else 10
         invoice = Invoice.objects
         invoice = invoice.order_by('-invoice_time')
+        if params.get("is_all", 0) >= 1:
+            params.pop("user_id")
 
         params = format_params_handle(
             param_dict=params,
             is_remove_empty=True,
             filter_filed_list=[
                 "id|int", "id_list|list", "thread_id|int", "user_id|int", "invoice_type_code",
                 "thread_id_list|list",
@@ -191,30 +193,27 @@
                 "thread_id_list": "thread_id__in", "id_list": "id__in",
                 "invoice_type_code": "invoice_type__invoice_type_code__iexact"
             },
         )
         invoice = invoice.extra(select={'invoice_time': 'DATE_FORMAT(invoice_time, "%%Y-%%m-%%d %%H:%%i:%%s")'})
         invoice = invoice.annotate(invoice_typee_code=F("invoice_type__invoice_type_code"), )
         invoice = invoice.filter(**params).values()
-
         total = invoice.count()
         #
         current_page_set = invoice[page * size: page * size + size] if page >= 0 and size > 0 else invoice
         res_list = []
         for i, it in enumerate(current_page_set):
             it['order'] = page * size + i + 1
             it['invoice_time'] = it['invoice_time'].strftime("%Y-%m-%d %H:%M:%S")
             res_list.append(it)
 
         data = res_list
-
         # ========== 四、相关前置业务逻辑处理 ==========
 
         # ========== 五、翻页 ==========
-        data = res_list
 
         user_id_list = [item.get("user_id", None) for item in res_list]
         user_list, err = UserService.user_list(allow_user_list=user_id_list)
         if user_list:
             data = JoinList(res_list, user_list['list'], "user_id", "user_id").join()
 
         data = filter_result_field(
@@ -233,16 +232,22 @@
         extend_list, err = InvoiceExtendService.get_extend_info(extend_id_list)
         if extend_list:
             data = JoinList(data, extend_list, "invoice_id", "invoice_id").join()
 
         return {'size': int(size), 'page': int(page + 1), 'total': total, 'list': data, }, None
 
     @staticmethod
-    def detail(params):
-        return None, None
+    def detail(invoice_id):
+        invoice = Invoice.objects.filter(id=invoice_id).first()
+        data = model_to_dict(invoice)
+        extend_id_list = [data.get("id", None)]
+        extend_list, err = InvoiceExtendService.get_extend_info(extend_id_list)
+        if extend_list:
+            data.update(extend_list[0])
+        return data, None
 
     @staticmethod
     def examine_approve(params):
         invoice_id = params.get("invoice_id", 0)
         invoice_status = params.get("invoice_status", "")
         data = {}
         if not invoice_id:
```

### Comparing `xj_invoice-1.0.0/xj_invoice/utils/custom_response.py` & `xj_invoice-1.0.2/xj_invoice/utils/custom_response.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.0/xj_invoice/utils/custom_tool.py` & `xj_invoice-1.0.2/xj_invoice/utils/custom_tool.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.0/xj_invoice/utils/j_config.py` & `xj_invoice-1.0.2/xj_invoice/utils/j_config.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.0/xj_invoice/utils/join_list.py` & `xj_invoice-1.0.2/xj_invoice/utils/join_list.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.0/xj_invoice/utils/jt.py` & `xj_invoice-1.0.2/xj_invoice/utils/jt.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.0/xj_invoice/utils/model_handle.py` & `xj_invoice-1.0.2/xj_invoice/utils/model_handle.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.0/xj_invoice/utils/user_wrapper.py` & `xj_invoice-1.0.2/xj_invoice/utils/user_wrapper.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.0/xj_invoice/views.py` & `xj_invoice-1.0.2/xj_invoice/views.py`

 * *Files identical despite different names*

### Comparing `xj_invoice-1.0.0/xj_invoice.egg-info/PKG-INFO` & `xj_invoice-1.0.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,52 +1,50 @@
 Metadata-Version: 2.1
-Name: xj-invoice
-Version: 1.0.0
+Name: xj_invoice
+Version: 1.0.2
 Summary: 发票模块
-Home-page: UNKNOWN
 Author: 高栋天
 Author-email: 1499593644@qq.com
 Maintainer: ['高栋天']
 Maintainer-email: angelvy@foxmail.com
 License: apache 3.0
-Description: # xj-invoice
-        
-        #### 介绍
-        {**以下是 Gitee 平台说明，您可以替换此简介**
-        Gitee 是 OSCHINA 推出的基于 Git 的代码托管平台（同时支持 SVN）。专为开发者提供稳定、高效、安全的云端软件开发协作平台
-        无论是个人、团队、或是企业，都能够用 Gitee 实现代码托管、项目管理、协作开发。企业项目请看 [https://gitee.com/enterprises](https://gitee.com/enterprises)}
-        
-        #### 软件架构
-        软件架构说明
-        
-        
-        #### 安装教程
-        
-        1.  xxxx
-        2.  xxxx
-        3.  xxxx
-        
-        #### 使用说明
-        
-        1.  xxxx
-        2.  xxxx
-        3.  xxxx
-        
-        #### 参与贡献
-        
-        1.  Fork 本仓库
-        2.  新建 Feat_xxx 分支
-        3.  提交代码
-        4.  新建 Pull Request
-        
-        
-        #### 特技
-        
-        1.  使用 Readme\_XXX.md 来支持不同的语言，例如 Readme\_en.md, Readme\_zh.md
-        2.  Gitee 官方博客 [blog.gitee.com](https://blog.gitee.com)
-        3.  你可以 [https://gitee.com/explore](https://gitee.com/explore) 这个地址来了解 Gitee 上的优秀开源项目
-        4.  [GVP](https://gitee.com/gvp) 全称是 Gitee 最有价值开源项目，是综合评定出的优秀开源项目
-        5.  Gitee 官方提供的使用手册 [https://gitee.com/help](https://gitee.com/help)
-        6.  Gitee 封面人物是一档用来展示 Gitee 会员风采的栏目 [https://gitee.com/gitee-stars/](https://gitee.com/gitee-stars/)
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+
+# xj-invoice
+
+#### 介绍
+{**以下是 Gitee 平台说明，您可以替换此简介**
+Gitee 是 OSCHINA 推出的基于 Git 的代码托管平台（同时支持 SVN）。专为开发者提供稳定、高效、安全的云端软件开发协作平台
+无论是个人、团队、或是企业，都能够用 Gitee 实现代码托管、项目管理、协作开发。企业项目请看 [https://gitee.com/enterprises](https://gitee.com/enterprises)}
+
+#### 软件架构
+软件架构说明
+
+
+#### 安装教程
+
+1.  xxxx
+2.  xxxx
+3.  xxxx
+
+#### 使用说明
+
+1.  xxxx
+2.  xxxx
+3.  xxxx
+
+#### 参与贡献
+
+1.  Fork 本仓库
+2.  新建 Feat_xxx 分支
+3.  提交代码
+4.  新建 Pull Request
+
+
+#### 特技
+
+1.  使用 Readme\_XXX.md 来支持不同的语言，例如 Readme\_en.md, Readme\_zh.md
+2.  Gitee 官方博客 [blog.gitee.com](https://blog.gitee.com)
+3.  你可以 [https://gitee.com/explore](https://gitee.com/explore) 这个地址来了解 Gitee 上的优秀开源项目
+4.  [GVP](https://gitee.com/gvp) 全称是 Gitee 最有价值开源项目，是综合评定出的优秀开源项目
+5.  Gitee 官方提供的使用手册 [https://gitee.com/help](https://gitee.com/help)
+6.  Gitee 封面人物是一档用来展示 Gitee 会员风采的栏目 [https://gitee.com/gitee-stars/](https://gitee.com/gitee-stars/)
```

### Comparing `xj_invoice-1.0.0/xj_invoice.egg-info/SOURCES.txt` & `xj_invoice-1.0.2/xj_invoice.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 README.md
 setup.py
 xj_invoice/__init__.py
 xj_invoice/admin.py
 xj_invoice/apps.py
 xj_invoice/models.py
-xj_invoice/search_indexes.py
+xj_invoice/service_register.py
 xj_invoice/tests.py
 xj_invoice/urls.py
 xj_invoice/views.py
 xj_invoice.egg-info/PKG-INFO
 xj_invoice.egg-info/SOURCES.txt
 xj_invoice.egg-info/dependency_links.txt
 xj_invoice.egg-info/top_level.txt
```

