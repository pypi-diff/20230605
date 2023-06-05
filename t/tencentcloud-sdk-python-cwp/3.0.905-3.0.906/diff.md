# Comparing `tmp/tencentcloud-sdk-python-cwp-3.0.905.tar.gz` & `tmp/tencentcloud-sdk-python-cwp-3.0.906.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cwp-3.0.905.tar", last modified: Fri Jun  2 00:25:49 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cwp-3.0.906.tar", last modified: Mon Jun  5 00:32:07 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cwp-3.0.905.tar` & `tencentcloud-sdk-python-cwp-3.0.906.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:25:49.000000 tencentcloud-sdk-python-cwp-3.0.905/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-02 00:25:49.000000 tencentcloud-sdk-python-cwp-3.0.905/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:25:49.000000 tencentcloud-sdk-python-cwp-3.0.905/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:25:49.000000 tencentcloud-sdk-python-cwp-3.0.905/tencentcloud/cwp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:25:49.000000 tencentcloud-sdk-python-cwp-3.0.905/tencentcloud/cwp/v20180228/
--rw-r--r--   0 root         (0) root         (0)     3900 2023-06-02 00:25:49.000000 tencentcloud-sdk-python-cwp-3.0.905/tencentcloud/cwp/v20180228/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   253287 2023-06-02 00:25:49.000000 tencentcloud-sdk-python-cwp-3.0.905/tencentcloud/cwp/v20180228/cwp_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 00:25:49.000000 tencentcloud-sdk-python-cwp-3.0.905/tencentcloud/cwp/v20180228/__init__.py
--rw-r--r--   0 root         (0) root         (0)   911378 2023-06-02 00:25:49.000000 tencentcloud-sdk-python-cwp-3.0.905/tencentcloud/cwp/v20180228/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 00:25:49.000000 tencentcloud-sdk-python-cwp-3.0.905/tencentcloud/cwp/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-02 00:25:49.000000 tencentcloud-sdk-python-cwp-3.0.905/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-02 00:25:49.000000 tencentcloud-sdk-python-cwp-3.0.905/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:25:49.000000 tencentcloud-sdk-python-cwp-3.0.905/tencentcloud_sdk_python_cwp.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 00:25:49.000000 tencentcloud-sdk-python-cwp-3.0.905/tencentcloud_sdk_python_cwp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-02 00:25:49.000000 tencentcloud-sdk-python-cwp-3.0.905/tencentcloud_sdk_python_cwp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-02 00:25:49.000000 tencentcloud-sdk-python-cwp-3.0.905/tencentcloud_sdk_python_cwp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-02 00:25:49.000000 tencentcloud-sdk-python-cwp-3.0.905/tencentcloud_sdk_python_cwp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-02 00:25:49.000000 tencentcloud-sdk-python-cwp-3.0.905/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-02 00:25:49.000000 tencentcloud-sdk-python-cwp-3.0.905/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:32:07.000000 tencentcloud-sdk-python-cwp-3.0.906/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-05 00:32:07.000000 tencentcloud-sdk-python-cwp-3.0.906/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:32:07.000000 tencentcloud-sdk-python-cwp-3.0.906/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:32:07.000000 tencentcloud-sdk-python-cwp-3.0.906/tencentcloud/cwp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:32:07.000000 tencentcloud-sdk-python-cwp-3.0.906/tencentcloud/cwp/v20180228/
+-rw-r--r--   0 root         (0) root         (0)     3900 2023-06-05 00:32:07.000000 tencentcloud-sdk-python-cwp-3.0.906/tencentcloud/cwp/v20180228/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   253159 2023-06-05 00:32:07.000000 tencentcloud-sdk-python-cwp-3.0.906/tencentcloud/cwp/v20180228/cwp_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:32:07.000000 tencentcloud-sdk-python-cwp-3.0.906/tencentcloud/cwp/v20180228/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   915364 2023-06-05 00:32:07.000000 tencentcloud-sdk-python-cwp-3.0.906/tencentcloud/cwp/v20180228/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:32:07.000000 tencentcloud-sdk-python-cwp-3.0.906/tencentcloud/cwp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-05 00:32:07.000000 tencentcloud-sdk-python-cwp-3.0.906/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-05 00:32:07.000000 tencentcloud-sdk-python-cwp-3.0.906/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:32:07.000000 tencentcloud-sdk-python-cwp-3.0.906/tencentcloud_sdk_python_cwp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 00:32:07.000000 tencentcloud-sdk-python-cwp-3.0.906/tencentcloud_sdk_python_cwp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-05 00:32:07.000000 tencentcloud-sdk-python-cwp-3.0.906/tencentcloud_sdk_python_cwp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-05 00:32:07.000000 tencentcloud-sdk-python-cwp-3.0.906/tencentcloud_sdk_python_cwp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-05 00:32:07.000000 tencentcloud-sdk-python-cwp-3.0.906/tencentcloud_sdk_python_cwp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-05 00:32:07.000000 tencentcloud-sdk-python-cwp-3.0.906/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-05 00:32:07.000000 tencentcloud-sdk-python-cwp-3.0.906/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cwp-3.0.905/README.rst` & `tencentcloud-sdk-python-cwp-3.0.906/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cwp-3.0.905/tencentcloud/cwp/v20180228/errorcodes.py` & `tencentcloud-sdk-python-cwp-3.0.906/tencentcloud/cwp/v20180228/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cwp-3.0.905/tencentcloud/cwp/v20180228/cwp_client.py` & `tencentcloud-sdk-python-cwp-3.0.906/tencentcloud/cwp/v20180228/cwp_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -3889,39 +3889,14 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def DescribeSaveOrUpdateWarnings(self, request):
-        """下线
-
-        更新或者插入用户告警设置(该接口废弃,请调用 ModifyWarningSetting )
-
-        :param request: Request instance for DescribeSaveOrUpdateWarnings.
-        :type request: :class:`tencentcloud.cwp.v20180228.models.DescribeSaveOrUpdateWarningsRequest`
-        :rtype: :class:`tencentcloud.cwp.v20180228.models.DescribeSaveOrUpdateWarningsResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("DescribeSaveOrUpdateWarnings", params, headers=headers)
-            response = json.loads(body)
-            model = models.DescribeSaveOrUpdateWarningsResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
     def DescribeScanMalwareSchedule(self, request):
         """查询木马扫描进度
 
         :param request: Request instance for DescribeScanMalwareSchedule.
         :type request: :class:`tencentcloud.cwp.v20180228.models.DescribeScanMalwareScheduleRequest`
         :rtype: :class:`tencentcloud.cwp.v20180228.models.DescribeScanMalwareScheduleResponse`
 
@@ -4581,14 +4556,37 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeVulStoreList(self, request):
+        """获取漏洞库列表
+
+        :param request: Request instance for DescribeVulStoreList.
+        :type request: :class:`tencentcloud.cwp.v20180228.models.DescribeVulStoreListRequest`
+        :rtype: :class:`tencentcloud.cwp.v20180228.models.DescribeVulStoreListResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeVulStoreList", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeVulStoreListResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeVulTop(self, request):
         """漏洞top统计
 
         :param request: Request instance for DescribeVulTop.
         :type request: :class:`tencentcloud.cwp.v20180228.models.DescribeVulTopRequest`
```

### Comparing `tencentcloud-sdk-python-cwp-3.0.905/tencentcloud/cwp/v20180228/models.py` & `tencentcloud-sdk-python-cwp-3.0.906/tencentcloud/cwp/v20180228/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -15827,60 +15827,14 @@
                 obj = RiskDnsList()
                 obj._deserialize(item)
                 self.RiskDnsList.append(obj)
         self.TotalCount = params.get("TotalCount")
         self.RequestId = params.get("RequestId")
 
 
-class DescribeSaveOrUpdateWarningsRequest(AbstractModel):
-    """DescribeSaveOrUpdateWarnings请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param WarningObjects: 告警设置的修改内容
-        :type WarningObjects: list of WarningObject
-        """
-        self.WarningObjects = None
-
-
-    def _deserialize(self, params):
-        if params.get("WarningObjects") is not None:
-            self.WarningObjects = []
-            for item in params.get("WarningObjects"):
-                obj = WarningObject()
-                obj._deserialize(item)
-                self.WarningObjects.append(obj)
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class DescribeSaveOrUpdateWarningsResponse(AbstractModel):
-    """DescribeSaveOrUpdateWarnings返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self.RequestId = None
-
-
-    def _deserialize(self, params):
-        self.RequestId = params.get("RequestId")
-
-
 class DescribeScanMalwareScheduleRequest(AbstractModel):
     """DescribeScanMalwareSchedule请求参数结构体
 
     """
 
 
 class DescribeScanMalwareScheduleResponse(AbstractModel):
@@ -17914,14 +17868,105 @@
                 obj._deserialize(item)
                 self.VulInfoList.append(obj)
         self.TotalCount = params.get("TotalCount")
         self.FollowVulCount = params.get("FollowVulCount")
         self.RequestId = params.get("RequestId")
 
 
+class DescribeVulStoreListRequest(AbstractModel):
+    """DescribeVulStoreList请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Filters: 
+<li>VulName- string - 是否必填：否 - 漏洞名称</li>
+<li>CveId- string - 是否必填：否 - cveid</li>
+<li>VulCategory- string - 是否必填：否 - 漏洞分类  1 Web-CMS漏洞 ,2 应用漏洞 ,4 Linux软件漏洞,5 Windows系统漏洞</li>
+<li>Method- string - 是否必填：否 - 检测方法 0版本对比,1 poc检测 </li>
+<li>SupportDefense- string - 是否必填：否 - 是否支持防御 0不支持,1支持</li>
+<li>FixSwitch- string - 是否必填：否 - 是否支持自动修复 0不支持,1支持</li>
+
+        :type Filters: list of Filter
+        :param Limit: 限制条数,默认10,最大100
+        :type Limit: int
+        :param Offset: 偏移量,默认0
+        :type Offset: int
+        :param Order: 排序方式: [ASC:升序|DESC:降序]
+        :type Order: str
+        :param By: 可选排序列: [PublishDate]
+        :type By: str
+        """
+        self.Filters = None
+        self.Limit = None
+        self.Offset = None
+        self.Order = None
+        self.By = None
+
+
+    def _deserialize(self, params):
+        if params.get("Filters") is not None:
+            self.Filters = []
+            for item in params.get("Filters"):
+                obj = Filter()
+                obj._deserialize(item)
+                self.Filters.append(obj)
+        self.Limit = params.get("Limit")
+        self.Offset = params.get("Offset")
+        self.Order = params.get("Order")
+        self.By = params.get("By")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeVulStoreListResponse(AbstractModel):
+    """DescribeVulStoreList返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param List: 漏洞信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type List: list of VulStoreListInfo
+        :param TotalCount: 总数
+        :type TotalCount: int
+        :param Remaining: 今日剩余搜索此时
+        :type Remaining: int
+        :param FreeSearchTimes: 免费搜索次数
+        :type FreeSearchTimes: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.List = None
+        self.TotalCount = None
+        self.Remaining = None
+        self.FreeSearchTimes = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("List") is not None:
+            self.List = []
+            for item in params.get("List"):
+                obj = VulStoreListInfo()
+                obj._deserialize(item)
+                self.List.append(obj)
+        self.TotalCount = params.get("TotalCount")
+        self.Remaining = params.get("Remaining")
+        self.FreeSearchTimes = params.get("FreeSearchTimes")
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeVulTopRequest(AbstractModel):
     """DescribeVulTop请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -26965,14 +27010,76 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
+
+
+class VulStoreListInfo(AbstractModel):
+    """漏洞仓库列表信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param VulId: 漏洞ID
+        :type VulId: int
+        :param Level: 漏洞级别
+        :type Level: int
+        :param Name: 漏洞名称
+        :type Name: str
+        :param CveId: cve编号
+        :type CveId: str
+        :param VulCategory: 1: web-cms漏洞 2:应用漏洞  4: Linux软件漏洞 5: Windows系统漏洞 0= 应急漏洞
+        :type VulCategory: int
+        :param PublishDate: 发布时间
+        :type PublishDate: str
+        :param Method: 漏洞检测方法 0 - 版本比对, 1 - POC验证
+        :type Method: int
+        :param AttackLevel: 漏洞攻击热度
+        :type AttackLevel: int
+        :param FixSwitch: 漏洞是否支持自动修复
+0-windows/linux均关闭; 1-windows/linux均打开; 2-仅linux; 3-仅windows
+        :type FixSwitch: int
+        :param SupportDefense: 漏洞是否支持防御
+0:不支持 1:支持
+        :type SupportDefense: int
+        """
+        self.VulId = None
+        self.Level = None
+        self.Name = None
+        self.CveId = None
+        self.VulCategory = None
+        self.PublishDate = None
+        self.Method = None
+        self.AttackLevel = None
+        self.FixSwitch = None
+        self.SupportDefense = None
+
+
+    def _deserialize(self, params):
+        self.VulId = params.get("VulId")
+        self.Level = params.get("Level")
+        self.Name = params.get("Name")
+        self.CveId = params.get("CveId")
+        self.VulCategory = params.get("VulCategory")
+        self.PublishDate = params.get("PublishDate")
+        self.Method = params.get("Method")
+        self.AttackLevel = params.get("AttackLevel")
+        self.FixSwitch = params.get("FixSwitch")
+        self.SupportDefense = params.get("SupportDefense")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
 
 
 class VulTopInfo(AbstractModel):
     """漏洞top统计实体
 
     """
```

### Comparing `tencentcloud-sdk-python-cwp-3.0.905/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cwp-3.0.906/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.905'
+__version__ = '3.0.906'
```

### Comparing `tencentcloud-sdk-python-cwp-3.0.905/PKG-INFO` & `tencentcloud-sdk-python-cwp-3.0.906/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cwp
-Version: 3.0.905
+Version: 3.0.906
 Summary: Tencent Cloud Cwp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cwp-3.0.905/tencentcloud_sdk_python_cwp.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cwp-3.0.906/tencentcloud_sdk_python_cwp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cwp
-Version: 3.0.905
+Version: 3.0.906
 Summary: Tencent Cloud Cwp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cwp-3.0.905/setup.py` & `tencentcloud-sdk-python-cwp-3.0.906/setup.py`

 * *Files identical despite different names*

