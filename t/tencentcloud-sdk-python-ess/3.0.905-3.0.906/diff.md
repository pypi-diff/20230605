# Comparing `tmp/tencentcloud-sdk-python-ess-3.0.905.tar.gz` & `tmp/tencentcloud-sdk-python-ess-3.0.906.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.905.tar", last modified: Fri Jun  2 00:28:31 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.906.tar", last modified: Mon Jun  5 00:34:27 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ess-3.0.905.tar` & `tencentcloud-sdk-python-ess-3.0.906.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:28:31.000000 tencentcloud-sdk-python-ess-3.0.905/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-02 00:28:31.000000 tencentcloud-sdk-python-ess-3.0.905/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:28:31.000000 tencentcloud-sdk-python-ess-3.0.905/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-02 00:28:31.000000 tencentcloud-sdk-python-ess-3.0.905/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:28:31.000000 tencentcloud-sdk-python-ess-3.0.905/tencentcloud/ess/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 00:28:31.000000 tencentcloud-sdk-python-ess-3.0.905/tencentcloud/ess/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:28:31.000000 tencentcloud-sdk-python-ess-3.0.905/tencentcloud/ess/v20201111/
--rw-r--r--   0 root         (0) root         (0)    51121 2023-06-02 00:28:31.000000 tencentcloud-sdk-python-ess-3.0.905/tencentcloud/ess/v20201111/ess_client.py
--rw-r--r--   0 root         (0) root         (0)    24243 2023-06-02 00:28:31.000000 tencentcloud-sdk-python-ess-3.0.905/tencentcloud/ess/v20201111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 00:28:31.000000 tencentcloud-sdk-python-ess-3.0.905/tencentcloud/ess/v20201111/__init__.py
--rw-r--r--   0 root         (0) root         (0)   225854 2023-06-02 00:28:31.000000 tencentcloud-sdk-python-ess-3.0.905/tencentcloud/ess/v20201111/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:28:31.000000 tencentcloud-sdk-python-ess-3.0.905/tencentcloud_sdk_python_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 00:28:31.000000 tencentcloud-sdk-python-ess-3.0.905/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-02 00:28:31.000000 tencentcloud-sdk-python-ess-3.0.905/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-02 00:28:31.000000 tencentcloud-sdk-python-ess-3.0.905/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-02 00:28:31.000000 tencentcloud-sdk-python-ess-3.0.905/tencentcloud_sdk_python_ess.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-02 00:28:31.000000 tencentcloud-sdk-python-ess-3.0.905/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-02 00:28:31.000000 tencentcloud-sdk-python-ess-3.0.905/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-02 00:28:31.000000 tencentcloud-sdk-python-ess-3.0.905/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:34:27.000000 tencentcloud-sdk-python-ess-3.0.906/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-05 00:34:27.000000 tencentcloud-sdk-python-ess-3.0.906/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:34:27.000000 tencentcloud-sdk-python-ess-3.0.906/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-05 00:34:27.000000 tencentcloud-sdk-python-ess-3.0.906/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:34:27.000000 tencentcloud-sdk-python-ess-3.0.906/tencentcloud/ess/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:34:27.000000 tencentcloud-sdk-python-ess-3.0.906/tencentcloud/ess/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:34:27.000000 tencentcloud-sdk-python-ess-3.0.906/tencentcloud/ess/v20201111/
+-rw-r--r--   0 root         (0) root         (0)    51319 2023-06-05 00:34:27.000000 tencentcloud-sdk-python-ess-3.0.906/tencentcloud/ess/v20201111/ess_client.py
+-rw-r--r--   0 root         (0) root         (0)    24361 2023-06-05 00:34:27.000000 tencentcloud-sdk-python-ess-3.0.906/tencentcloud/ess/v20201111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:34:27.000000 tencentcloud-sdk-python-ess-3.0.906/tencentcloud/ess/v20201111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   228117 2023-06-05 00:34:27.000000 tencentcloud-sdk-python-ess-3.0.906/tencentcloud/ess/v20201111/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:34:27.000000 tencentcloud-sdk-python-ess-3.0.906/tencentcloud_sdk_python_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 00:34:27.000000 tencentcloud-sdk-python-ess-3.0.906/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-05 00:34:27.000000 tencentcloud-sdk-python-ess-3.0.906/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-05 00:34:27.000000 tencentcloud-sdk-python-ess-3.0.906/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-05 00:34:27.000000 tencentcloud-sdk-python-ess-3.0.906/tencentcloud_sdk_python_ess.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-05 00:34:27.000000 tencentcloud-sdk-python-ess-3.0.906/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-05 00:34:27.000000 tencentcloud-sdk-python-ess-3.0.906/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-05 00:34:27.000000 tencentcloud-sdk-python-ess-3.0.906/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ess-3.0.905/README.rst` & `tencentcloud-sdk-python-ess-3.0.906/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.905/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ess-3.0.906/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ess-3.0.905/tencentcloud/ess/v20201111/ess_client.py` & `tencentcloud-sdk-python-ess-3.0.906/tencentcloud/ess/v20201111/ess_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,17 +190,18 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateFlow(self, request):
-        """通过模板创建签署流程
-        适用场景：在标准制式的合同场景中，可通过提前预制好模板文件，每次调用模板文件的id，补充合同内容信息及签署信息生成电子合同。
-        注：该接口是通过模板生成合同流程的前置接口，先创建一个不包含签署文件的流程。配合“创建电子文档”接口和“发起流程”接口使用。
+        """通过模板创建签署流程<br/>
+        适用场景：在标准制式的合同场景中，可通过提前预制好模板文件，每次调用模板文件的id，补充合同内容信息及签署信息生成电子合同。<br/>
+        注：该接口是通过模板生成合同流程的前置接口，先创建一个不包含签署文件的流程。<br/>
+        配合“创建电子文档”接口和“发起流程”接口使用。<br/>
 
         :param request: Request instance for CreateFlow.
         :type request: :class:`tencentcloud.ess.v20201111.models.CreateFlowRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.CreateFlowResponse`
 
         """
         try:
@@ -242,18 +243,18 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateFlowByFiles(self, request):
-        """此接口（CreateFlowByFiles）用来通过上传后的pdf资源编号来创建待签署的合同流程。
-        适用场景1：适用非制式的合同文件签署。一般开发者自己有完整的签署文件，可以通过该接口传入完整的PDF文件及流程信息生成待签署的合同流程。
-        适用场景2：可通过该接口传入制式合同文件，同时在指定位置添加签署控件。可以起到接口创建临时模板的效果。如果是标准的制式文件，建议使用模板功能生成模板ID进行合同流程的生成。
-        注意事项：该接口需要依赖“多文件上传”接口生成pdf资源编号（FileIds）进行使用。
+        """此接口（CreateFlowByFiles）用来通过上传后的pdf资源编号来创建待签署的合同流程。<br/>
+        适用场景1：适用非制式的合同文件签署。一般开发者自己有完整的签署文件，可以通过该接口传入完整的PDF文件及流程信息生成待签署的合同流程。<br/>
+        适用场景2：可通过该接口传入制式合同文件，同时在指定位置添加签署控件。可以起到接口创建临时模板的效果。如果是标准的制式文件，建议使用模板功能生成模板ID进行合同流程的生成。<br/>
+        注意事项：该接口需要依赖“多文件上传”接口生成pdf资源编号（FileIds）进行使用。<br/>
 
         :param request: Request instance for CreateFlowByFiles.
         :type request: :class:`tencentcloud.ess.v20201111.models.CreateFlowByFilesRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.CreateFlowByFilesResponse`
 
         """
         try:
@@ -668,15 +669,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeFileUrls(self, request):
-        """查询文件下载URL
+        """查询文件下载URL。
         适用场景：通过传参合同流程编号，下载对应的合同PDF文件流到本地。
 
         :param request: Request instance for DescribeFileUrls.
         :type request: :class:`tencentcloud.ess.v20201111.models.DescribeFileUrlsRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.DescribeFileUrlsResponse`
 
         """
@@ -764,15 +765,16 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeFlowTemplates(self, request):
-        """当模板较多或模板中的控件较多时，可以通过查询模板接口更方便的获取模板列表，以及每个模板内的控件信息。该接口常用来配合“创建电子文档”接口作为前置的接口使用。
+        """当模板较多或模板中的控件较多时，可以通过查询模板接口更方便的获取模板列表，以及每个模板内的控件信息。<br/>
+        该接口常用来配合“创建电子文档”接口作为前置的接口使用。<br/>
 
         :param request: Request instance for DescribeFlowTemplates.
         :type request: :class:`tencentcloud.ess.v20201111.models.DescribeFlowTemplatesRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.DescribeFlowTemplatesResponse`
 
         """
         try:
@@ -972,15 +974,16 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def GetTaskResultApi(self, request):
-        """通过发起转换任务接口（CreateConvertTaskApi）返回的任务Id查询转换任务状态，通过本接口确认转换任务是否完成。大文件转换所需的时间可能会比较长。
+        """通过发起转换任务接口（CreateConvertTaskApi）返回的任务Id查询转换任务状态，通过本接口确认转换任务是否完成。<br/>
+        大文件转换所需的时间可能会比较长。
 
         :param request: Request instance for GetTaskResultApi.
         :type request: :class:`tencentcloud.ess.v20201111.models.GetTaskResultApiRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.GetTaskResultApiResponse`
 
         """
         try:
@@ -1091,18 +1094,21 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def UploadFiles(self, request):
-        """此接口（UploadFiles）用于文件上传。
-        适用场景：用于生成pdf资源编号（FileIds）来配合“用PDF创建流程”接口使用，使用场景可详见“用PDF创建流程”接口说明。
-        其中上传的文件，图片类型(png/jpg/jpeg)大小限制为5M，其他大小限制为60M。
-        调用时需要设置Domain/接口请求域名为 file.ess.tencent.cn，并设置参数Version/版本号为2020-12-22
+        """此接口（UploadFiles）用于文件上传。<br/>
+        适用场景：用于生成pdf资源编号（FileIds）来配合“用PDF创建流程”接口使用，使用场景可详见“用PDF创建流程”接口说明。<br/>
+
+        其中上传的文件，图片类型(png/jpg/jpeg)大小限制为5M，其他大小限制为60M。<br/>
+        调用时需要设置Domain/接口请求域名为 file.ess.tencent.cn,代码示例：<br/>
+        HttpProfile httpProfile = new HttpProfile();<br/>
+        httpProfile.setEndpoint("file.test.ess.tencent.cn");<br/>
 
         :param request: Request instance for UploadFiles.
         :type request: :class:`tencentcloud.ess.v20201111.models.UploadFilesRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.UploadFilesResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-ess-3.0.905/tencentcloud/ess/v20201111/errorcodes.py` & `tencentcloud-sdk-python-ess-3.0.906/tencentcloud/ess/v20201111/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -262,14 +262,17 @@
 
 # 不合法的手机号，请检查后重试。
 INVALIDPARAMETER_MOBILE = 'InvalidParameter.Mobile'
 
 # 不合法的用户名称，请修改后重试。
 INVALIDPARAMETER_NAME = 'InvalidParameter.Name'
 
+# 手机号为空或者非法的手机号。
+INVALIDPARAMETER_NONSUPPORTMOBILE = 'InvalidParameter.NonsupportMobile'
+
 # 不支持的通知类型，请检查并联系客服处理。
 INVALIDPARAMETER_NOTIFYTYPE = 'InvalidParameter.NotifyType'
 
 # 参数Offset不正确
 INVALIDPARAMETER_OFFSET = 'InvalidParameter.Offset'
 
 # 不合法的企业名称，请修改后重试。
```

### Comparing `tencentcloud-sdk-python-ess-3.0.905/tencentcloud/ess/v20201111/models.py` & `tencentcloud-sdk-python-ess-3.0.906/tencentcloud/ess/v20201111/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -327,15 +327,15 @@
 class BindEmployeeUserIdWithClientOpenIdRequest(AbstractModel):
     """BindEmployeeUserIdWithClientOpenId请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param Operator: 用户信息，OpenId与UserId二选一必填一个，OpenId是第三方客户ID，userId是用户实名后的电子签生成的ID,当传入客户系统openId，传入的openId需与电子签员工userId绑定，且参数Channel必填，Channel值为INTEGRATE；当传入参数UserId，Channel无需指定
+        :param Operator: 用户信息，OpenId与UserId二选一必填一个，OpenId是第三方客户ID，userId是用户实名后的电子签生成的ID,当传入客户系统openId，传入的openId需与电子签员工userId绑定，且参数Channel必填，Channel值为INTEGRATE；当传入参数UserId，Channel无需指定。（参数参考示例）
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
         :param UserId: 电子签系统员工UserId
         :type UserId: str
         :param OpenId: 客户系统OpenId
         :type OpenId: str
         """
         self.Operator = None
@@ -384,24 +384,32 @@
 
     """
 
     def __init__(self):
         r"""
         :param CallbackUrl: 回调url
         :type CallbackUrl: str
-        :param Token: 回调加密token
+        :param Token: 回调加密key，已废弃
         :type Token: str
+        :param CallbackKey: 回调加密key
+        :type CallbackKey: str
+        :param CallbackToken: 回调验签token
+        :type CallbackToken: str
         """
         self.CallbackUrl = None
         self.Token = None
+        self.CallbackKey = None
+        self.CallbackToken = None
 
 
     def _deserialize(self, params):
         self.CallbackUrl = params.get("CallbackUrl")
         self.Token = params.get("Token")
+        self.CallbackKey = params.get("CallbackKey")
+        self.CallbackToken = params.get("CallbackToken")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -452,15 +460,15 @@
         r"""
         :param Operator: 调用方用户信息，userId 必填
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
         :param FlowId: 签署流程id
         :type FlowId: str
         :param CancelMessage: 撤销原因，最长200个字符；
         :type CancelMessage: str
-        :param Agent: 应用相关信息
+        :param Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填
         :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         """
         self.Operator = None
         self.FlowId = None
         self.CancelMessage = None
         self.Agent = None
 
@@ -503,19 +511,19 @@
 class CancelMultiFlowSignQRCodeRequest(AbstractModel):
     """CancelMultiFlowSignQRCode请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param Operator: 用户信息
+        :param Operator: 调用方用户信息，userId 必填
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
         :param QrCodeId: 二维码id
         :type QrCodeId: str
-        :param Agent: 应用信息
+        :param Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填
         :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         """
         self.Operator = None
         self.QrCodeId = None
         self.Agent = None
 
 
@@ -894,15 +902,15 @@
 class CreateChannelSubOrganizationModifyQrCodeRequest(AbstractModel):
     """CreateChannelSubOrganizationModifyQrCode请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param Operator: 操作人
+        :param Operator: 操作人信息，userId必填
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
         :param ApplicationId: 应用编号
         :type ApplicationId: str
         """
         self.Operator = None
         self.ApplicationId = None
 
@@ -1592,15 +1600,15 @@
         :param ReviewType: 企业内部审核结果
 PASS: 通过 
 REJECT: 拒绝
         :type ReviewType: str
         :param ReviewMessage: 审核原因 
 当ReviewType 是REJECT 时此字段必填,字符串长度不超过200
         :type ReviewMessage: str
-        :param Agent: 应用相关信息
+        :param Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填
         :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         """
         self.Operator = None
         self.FlowId = None
         self.ReviewType = None
         self.ReviewMessage = None
         self.Agent = None
@@ -1786,15 +1794,15 @@
 class CreateIntegrationUserRolesRequest(AbstractModel):
     """CreateIntegrationUserRoles请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param Operator: 操作人信息
+        :param Operator: 操作人信息，UserId必填
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
         :param UserIds: 绑定角色的用户id列表
         :type UserIds: list of str
         :param RoleIds: 绑定角色的角色id列表
         :type RoleIds: list of str
         :param Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填
         :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
@@ -1852,15 +1860,15 @@
 class CreateMultiFlowSignQRCodeRequest(AbstractModel):
     """CreateMultiFlowSignQRCode请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param Operator: 用户信息
+        :param Operator: 用户信息，其中UserId为必填参数
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
         :param TemplateId: 模板ID
         :type TemplateId: str
         :param FlowName: 签署流程名称，最大长度不超过200字符
         :type FlowName: str
         :param MaxFlowNum: 最大可发起签署流程份数，默认5份 
 发起流程数量超过此上限后二维码自动失效
@@ -2019,15 +2027,15 @@
 class CreatePrepareFlowResponse(AbstractModel):
     """CreatePrepareFlow返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param Url: 快速发起预览链接
+        :param Url: 快速发起预览链接，有效期5分钟
         :type Url: str
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.Url = None
         self.RequestId = None
 
@@ -2046,25 +2054,27 @@
         r"""
         :param UserName: 个人用户姓名
         :type UserName: str
         :param IdCardNumber: 身份证件号码
         :type IdCardNumber: str
         :param SealName: 印章名称
         :type SealName: str
-        :param SealImage: 印章图片的base64，最大不超过 8M
-        :type SealImage: str
         :param Operator: 调用方用户信息，userId 必填。支持填入集团子公司经办人 userId代发合同。
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
         :param IdCardType: 身份证件类型:
 ID_CARD 身份证
 PASSPORT 护照
 HONGKONG_AND_MACAO 中国香港
 FOREIGN_ID_CARD 境外身份
 HONGKONG_MACAO_AND_TAIWAN 中国台湾
         :type IdCardType: str
+        :param SealImage: 印章图片的base64
+注：已废弃
+请先通过UploadFiles接口上传文件，获取 FileId
+        :type SealImage: str
         :param SealImageCompress: 是否开启印章图片压缩处理，默认不开启，如需开启请设置为 true。当印章超过 2M 时建议开启，开启后图片的 hash 将发生变化。
         :type SealImageCompress: bool
         :param Mobile: 手机号码；当需要开通自动签时，该参数必传
         :type Mobile: str
         :param EnableAutoSign: 是否开通自动签，该功能需联系运营工作人员开通后使用
         :type EnableAutoSign: bool
         :param SealColor: 印章颜色（参数ProcessSeal=true时生效）
@@ -2075,42 +2085,48 @@
 BLUE 蓝色。
         :type SealColor: str
         :param ProcessSeal: 是否处理印章
 默认不做印章处理。
 取值：false：不做任何处理；
 true：做透明化处理和颜色增强。
         :type ProcessSeal: bool
+        :param FileId: 印章图片文件 id
+取值：
+填写的FileId通过UploadFiles接口上传文件获取。
+        :type FileId: str
         """
         self.UserName = None
         self.IdCardNumber = None
         self.SealName = None
-        self.SealImage = None
         self.Operator = None
         self.IdCardType = None
+        self.SealImage = None
         self.SealImageCompress = None
         self.Mobile = None
         self.EnableAutoSign = None
         self.SealColor = None
         self.ProcessSeal = None
+        self.FileId = None
 
 
     def _deserialize(self, params):
         self.UserName = params.get("UserName")
         self.IdCardNumber = params.get("IdCardNumber")
         self.SealName = params.get("SealName")
-        self.SealImage = params.get("SealImage")
         if params.get("Operator") is not None:
             self.Operator = UserInfo()
             self.Operator._deserialize(params.get("Operator"))
         self.IdCardType = params.get("IdCardType")
+        self.SealImage = params.get("SealImage")
         self.SealImageCompress = params.get("SealImageCompress")
         self.Mobile = params.get("Mobile")
         self.EnableAutoSign = params.get("EnableAutoSign")
         self.SealColor = params.get("SealColor")
         self.ProcessSeal = params.get("ProcessSeal")
+        self.FileId = params.get("FileId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -2272,15 +2288,15 @@
 class CreateSchemeUrlResponse(AbstractModel):
     """CreateSchemeUrl返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param SchemeUrl: 小程序链接地址
+        :param SchemeUrl: 小程序链接地址，有效期5分钟
         :type SchemeUrl: str
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.SchemeUrl = None
         self.RequestId = None
 
@@ -2293,55 +2309,55 @@
 class CreateSealPolicyRequest(AbstractModel):
     """CreateSealPolicy请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param Operator: 授权发起人在平台信息，具体参考UserInfo结构体
+        :param Operator: 调用方用户信息，userId 必填
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
         :param Users: 用户在电子文件签署平台标识信息，具体参考UserInfo结构体。可跟下面的UserIds可叠加起作用
         :type Users: list of UserInfo
         :param SealId: 印章ID
         :type SealId: str
         :param Expired: 授权有效期。时间戳秒级
         :type Expired: int
+        :param UserIds: 需要授权的用户UserId集合。跟上面的SealId参数配合使用。选填，跟上面的Users同时起作用
+        :type UserIds: list of str
         :param Policy: 印章授权内容
         :type Policy: str
-        :param Agent: 应用相关
+        :param Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填
         :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
-        :param UserIds: 需要授权的用户UserId集合。跟上面的SealId参数配合使用。选填，跟上面的Users同时起作用
-        :type UserIds: list of str
         """
         self.Operator = None
         self.Users = None
         self.SealId = None
         self.Expired = None
+        self.UserIds = None
         self.Policy = None
         self.Agent = None
-        self.UserIds = None
 
 
     def _deserialize(self, params):
         if params.get("Operator") is not None:
             self.Operator = UserInfo()
             self.Operator._deserialize(params.get("Operator"))
         if params.get("Users") is not None:
             self.Users = []
             for item in params.get("Users"):
                 obj = UserInfo()
                 obj._deserialize(item)
                 self.Users.append(obj)
         self.SealId = params.get("SealId")
         self.Expired = params.get("Expired")
+        self.UserIds = params.get("UserIds")
         self.Policy = params.get("Policy")
         if params.get("Agent") is not None:
             self.Agent = Agent()
             self.Agent._deserialize(params.get("Agent"))
-        self.UserIds = params.get("UserIds")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -2411,15 +2427,15 @@
 class CreateUserAutoSignEnableUrlRequest(AbstractModel):
     """CreateUserAutoSignEnableUrl请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param Operator: 操作人信息
+        :param Operator: 操作人信息,UserId必填
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
         :param SceneKey: 自动签场景:
 E_PRESCRIPTION_AUTO_SIGN 电子处方
         :type SceneKey: str
         :param AutoSignConfig: 自动签开通，签署相关配置
         :type AutoSignConfig: :class:`tencentcloud.ess.v20201111.models.AutoSignConfig`
         :param UrlType: 链接类型，空-默认小程序端链接，H5SIGN-h5端链接
@@ -2569,21 +2585,21 @@
 class DeleteIntegrationRoleUsersRequest(AbstractModel):
     """DeleteIntegrationRoleUsers请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param Operator: 操作人
+        :param Operator: 操作人信息，userId必填
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
         :param RoleId: 角色id
         :type RoleId: str
         :param Users: 用户信息
         :type Users: list of UserInfo
-        :param Agent: 代理信息
+        :param Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填
         :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         """
         self.Operator = None
         self.RoleId = None
         self.Users = None
         self.Agent = None
 
@@ -2635,42 +2651,42 @@
 class DeleteSealPoliciesRequest(AbstractModel):
     """DeleteSealPolicies请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param Operator: 操作撤销的用户信息
+        :param Operator: 调用方用户信息，userId 必填
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
         :param PolicyIds: 印章授权编码数组。这个参数跟下面的SealId其中一个必填，另外一个可选填
         :type PolicyIds: list of str
-        :param Agent: 应用相关
-        :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         :param SealId: 印章ID。这个参数跟上面的PolicyIds其中一个必填，另外一个可选填
         :type SealId: str
         :param UserIds: 待授权的员工ID
         :type UserIds: list of str
+        :param Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填
+        :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         """
         self.Operator = None
         self.PolicyIds = None
-        self.Agent = None
         self.SealId = None
         self.UserIds = None
+        self.Agent = None
 
 
     def _deserialize(self, params):
         if params.get("Operator") is not None:
             self.Operator = UserInfo()
             self.Operator._deserialize(params.get("Operator"))
         self.PolicyIds = params.get("PolicyIds")
+        self.SealId = params.get("SealId")
+        self.UserIds = params.get("UserIds")
         if params.get("Agent") is not None:
             self.Agent = Agent()
             self.Agent._deserialize(params.get("Agent"))
-        self.SealId = params.get("SealId")
-        self.UserIds = params.get("UserIds")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -2870,17 +2886,17 @@
 
     """
 
     def __init__(self):
         r"""
         :param Operator: 调用方用户信息，userId 必填
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
-        :param FlowIds: 需要查询的流程ID列表，限制最大20个
+        :param FlowIds: 需要查询的流程ID列表，限制最大100个
         :type FlowIds: list of str
-        :param Agent: 应用相关信息
+        :param Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填
         :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         """
         self.Operator = None
         self.FlowIds = None
         self.Agent = None
 
 
@@ -2990,15 +3006,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param FlowIds: 需要查询的流程ID列表，限制最大100个
         :type FlowIds: list of str
-        :param Operator: 调用方用户信息
+        :param Operator: 调用方用户信息，userId 必填
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
         :param Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填
         :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         """
         self.FlowIds = None
         self.Operator = None
         self.Agent = None
@@ -3054,65 +3070,65 @@
 
     def __init__(self):
         r"""
         :param Operator: 调用方用户信息，userId 必填
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
         :param Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填
         :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
+        :param ContentType: 查询内容：0-模板列表及详情（默认），1-仅模板列表
+        :type ContentType: int
+        :param Filters: 搜索条件，具体参考Filter结构体。本接口取值：template-id：按照【 **模板唯一标识** 】进行过滤
+        :type Filters: list of Filter
         :param Offset: 查询偏移位置，默认0
         :type Offset: int
         :param Limit: 查询个数，默认20，最大200
         :type Limit: int
-        :param Filters: 搜索条件，具体参考Filter结构体。本接口取值：template-id：按照【 **模板唯一标识** 】进行过滤
-        :type Filters: list of Filter
         :param ApplicationId: 这个参数跟下面的IsChannel参数配合使用。
 IsChannel=false时，ApplicationId参数不起任何作用。
 IsChannel=true时，ApplicationId为空，查询所有第三方应用集成平台企业模板列表；ApplicationId不为空，查询指定应用下的模板列表
 ApplicationId为空，查询所有应用下的模板列表
         :type ApplicationId: str
         :param IsChannel: 默认为false，查询SaaS模板库列表；
 为true，查询第三方应用集成平台企业模板库管理列表
         :type IsChannel: bool
-        :param ContentType: 查询内容：0-模板列表及详情（默认），1-仅模板列表
-        :type ContentType: int
         :param Organization: 暂未开放
         :type Organization: :class:`tencentcloud.ess.v20201111.models.OrganizationInfo`
         :param GenerateSource: 暂未开放
         :type GenerateSource: int
         """
         self.Operator = None
         self.Agent = None
+        self.ContentType = None
+        self.Filters = None
         self.Offset = None
         self.Limit = None
-        self.Filters = None
         self.ApplicationId = None
         self.IsChannel = None
-        self.ContentType = None
         self.Organization = None
         self.GenerateSource = None
 
 
     def _deserialize(self, params):
         if params.get("Operator") is not None:
             self.Operator = UserInfo()
             self.Operator._deserialize(params.get("Operator"))
         if params.get("Agent") is not None:
             self.Agent = Agent()
             self.Agent._deserialize(params.get("Agent"))
-        self.Offset = params.get("Offset")
-        self.Limit = params.get("Limit")
+        self.ContentType = params.get("ContentType")
         if params.get("Filters") is not None:
             self.Filters = []
             for item in params.get("Filters"):
                 obj = Filter()
                 obj._deserialize(item)
                 self.Filters.append(obj)
+        self.Offset = params.get("Offset")
+        self.Limit = params.get("Limit")
         self.ApplicationId = params.get("ApplicationId")
         self.IsChannel = params.get("IsChannel")
-        self.ContentType = params.get("ContentType")
         if params.get("Organization") is not None:
             self.Organization = OrganizationInfo()
             self.Organization._deserialize(params.get("Organization"))
         self.GenerateSource = params.get("GenerateSource")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
@@ -3127,15 +3143,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param Templates: 模板详情列表
         :type Templates: list of TemplateInfo
-        :param TotalCount: 查询到的总个数
+        :param TotalCount: 查询到的总数
         :type TotalCount: int
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.Templates = None
         self.TotalCount = None
         self.RequestId = None
@@ -3159,31 +3175,37 @@
 
     def __init__(self):
         r"""
         :param Operator: 操作人信息，userId必填
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
         :param Limit: 返回最大数量，最大为20
         :type Limit: int
+        :param Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填
+        :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         :param Filters: 查询过滤实名用户，Key为Status，Values为["IsVerified"]
 根据第三方系统openId过滤查询员工时,Key为StaffOpenId,Values为["OpenId","OpenId",...]
         :type Filters: list of Filter
         :param Offset: 偏移量，默认为0，最大为20000
         :type Offset: int
         """
         self.Operator = None
         self.Limit = None
+        self.Agent = None
         self.Filters = None
         self.Offset = None
 
 
     def _deserialize(self, params):
         if params.get("Operator") is not None:
             self.Operator = UserInfo()
             self.Operator._deserialize(params.get("Operator"))
         self.Limit = params.get("Limit")
+        if params.get("Agent") is not None:
+            self.Agent = Agent()
+            self.Agent._deserialize(params.get("Agent"))
         if params.get("Filters") is not None:
             self.Filters = []
             for item in params.get("Filters"):
                 obj = Filter()
                 obj._deserialize(item)
                 self.Filters.append(obj)
         self.Offset = params.get("Offset")
@@ -3609,15 +3631,15 @@
 class DescribeUserAutoSignStatusRequest(AbstractModel):
     """DescribeUserAutoSignStatus请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param Operator: 操作人信息
+        :param Operator: 操作人信息，UserId必填
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
         :param SceneKey: 自动签场景:
 E_PRESCRIPTION_AUTO_SIGN 电子处方
         :type SceneKey: str
         :param UserInfo: 查询开启状态的用户信息
         :type UserInfo: :class:`tencentcloud.ess.v20201111.models.UserThreeFactor`
         """
@@ -3675,15 +3697,15 @@
 class DisableUserAutoSignRequest(AbstractModel):
     """DisableUserAutoSign请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param Operator: 操作人信息
+        :param Operator: 操作人信息,UserId必填
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
         :param SceneKey: 自动签场景:
 E_PRESCRIPTION_AUTO_SIGN 电子处方
         :type SceneKey: str
         :param UserInfo: 关闭自动签的个人的三要素
         :type UserInfo: :class:`tencentcloud.ess.v20201111.models.UserThreeFactor`
         """
@@ -4541,15 +4563,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param TaskId: 任务Id，通过CreateConvertTaskApi得到
         :type TaskId: str
-        :param Operator: 操作人信息
+        :param Operator: 操作人信息,UserId必填
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
         :param Agent: 应用号信息
         :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         :param Organization: 暂未开放
         :type Organization: :class:`tencentcloud.ess.v20201111.models.OrganizationInfo`
         """
         self.TaskId = None
@@ -4635,15 +4657,15 @@
         :type Name: str
         :param Alias: 成员企业别名
 注意：此字段可能返回 null，表示取不到有效值。
         :type Alias: str
         :param OrganizationId: 成员企业id
 注意：此字段可能返回 null，表示取不到有效值。
         :type OrganizationId: str
-        :param UpdateTime: 更新时间
+        :param UpdateTime: 更新时间，时间戳，单位秒
 注意：此字段可能返回 null，表示取不到有效值。
         :type UpdateTime: int
         :param Status: 成员企业加入集团的当前状态:1-待授权;2-已授权待激活;3-拒绝授权;4-已解除;5-已加入
 注意：此字段可能返回 null，表示取不到有效值。
         :type Status: int
         :param IsMainOrganization: 是否为集团主企业
 注意：此字段可能返回 null，表示取不到有效值。
@@ -4653,21 +4675,21 @@
         :type IdCardNumber: str
         :param AdminInfo: 企业超管信息
 注意：此字段可能返回 null，表示取不到有效值。
         :type AdminInfo: :class:`tencentcloud.ess.v20201111.models.Admin`
         :param License: 企业许可证
 注意：此字段可能返回 null，表示取不到有效值。
         :type License: str
-        :param LicenseExpireTime: 企业许可证过期时间
+        :param LicenseExpireTime: 企业许可证过期时间，时间戳，单位秒
 注意：此字段可能返回 null，表示取不到有效值。
         :type LicenseExpireTime: int
-        :param JoinTime: 成员企业加入集团时间
+        :param JoinTime: 成员企业加入集团时间，时间戳，单位秒
 注意：此字段可能返回 null，表示取不到有效值。
         :type JoinTime: int
-        :param FlowEngineEnable: 是否可以使用审批流引擎
+        :param FlowEngineEnable: 是否使用审批流引擎，true-是，false-否
 注意：此字段可能返回 null，表示取不到有效值。
         :type FlowEngineEnable: bool
         """
         self.Name = None
         self.Alias = None
         self.OrganizationId = None
         self.UpdateTime = None
@@ -4717,15 +4739,15 @@
         :type RoleId: str
         :param RoleName: 角色名
 注意：此字段可能返回 null，表示取不到有效值。
         :type RoleName: str
         :param RoleStatus: 角色状态，1-启用，2-禁用
 注意：此字段可能返回 null，表示取不到有效值。
         :type RoleStatus: int
-        :param IsGroupRole: 是否是集团角色
+        :param IsGroupRole: 是否是集团角色，true-是，false-否
 注意：此字段可能返回 null，表示取不到有效值。
         :type IsGroupRole: bool
         :param SubOrgIdList: 管辖的子企业列表
 注意：此字段可能返回 null，表示取不到有效值。
         :type SubOrgIdList: list of str
         """
         self.RoleId = None
@@ -4845,30 +4867,30 @@
 
     def __init__(self):
         r"""
         :param SealId: 电子印章编号
         :type SealId: str
         :param SealName: 电子印章名称
         :type SealName: str
-        :param CreateOn: 电子印章授权时间戳
+        :param CreateOn: 电子印章授权时间戳，单位秒
         :type CreateOn: int
-        :param Creator: 电子印章授权人
+        :param Creator: 电子印章授权人的UserId
         :type Creator: str
         :param SealPolicyId: 电子印章策略Id
         :type SealPolicyId: str
         :param SealStatus: 印章状态，有以下六种：CHECKING（审核中）SUCCESS（已启用）FAIL（审核拒绝）CHECKING-SADM（待超管审核）DISABLE（已停用）STOPPED（已终止）
         :type SealStatus: str
         :param FailReason: 审核失败原因
 注意：此字段可能返回 null，表示取不到有效值。
         :type FailReason: str
         :param Url: 印章图片url，5分钟内有效
         :type Url: str
-        :param SealType: 印章类型
+        :param SealType: 印章类型,OFFICIAL-企业公章, CONTRACT-合同专用章,ORGANIZATIONSEAL-企业印章(本地上传印章类型),LEGAL_PERSON_SEAL-法人印章
         :type SealType: str
-        :param IsAllTime: 用印申请是否为永久授权
+        :param IsAllTime: 用印申请是否为永久授权，true-是，false-否
         :type IsAllTime: bool
         :param AuthorizedUsers: 授权人列表
 注意：此字段可能返回 null，表示取不到有效值。
         :type AuthorizedUsers: list of AuthorizedUser
         """
         self.SealId = None
         self.SealName = None
@@ -4958,33 +4980,33 @@
         r"""
         :param VerifyResult: 验签结果。0-签名域未签名；1-验签成功； 3-验签失败；4-未找到签名域：文件内没有签名域；5-签名值格式不正确。
         :type VerifyResult: int
         :param SignPlatform: 签署平台，如果文件是在腾讯电子签平台签署，则返回腾讯电子签，如果文件不在腾讯电子签平台签署，则返回其他平台。
         :type SignPlatform: str
         :param SignerName: 签署人名称
         :type SignerName: str
-        :param SignTime: 签署时间
+        :param SignTime: 签署时间戳，单位秒
         :type SignTime: int
         :param SignAlgorithm: 签名算法
         :type SignAlgorithm: str
         :param CertSn: 签名证书序列号
         :type CertSn: str
-        :param CertNotBefore: 证书起始时间
+        :param CertNotBefore: 证书起始时间戳，单位秒
         :type CertNotBefore: int
-        :param CertNotAfter: 证书过期时间
+        :param CertNotAfter: 证书过期时间戳，单位秒
         :type CertNotAfter: int
-        :param ComponentPosX: 签名域横坐标
+        :param ComponentPosX: 签名域横坐标，单位pt
         :type ComponentPosX: float
-        :param ComponentPosY: 签名域纵坐标
+        :param ComponentPosY: 签名域纵坐标，单位pt
         :type ComponentPosY: float
-        :param ComponentWidth: 签名域宽度
+        :param ComponentWidth: 签名域宽度，单位pt
         :type ComponentWidth: float
-        :param ComponentHeight: 签名域高度
+        :param ComponentHeight: 签名域高度，单位pt
         :type ComponentHeight: float
-        :param ComponentPage: 签名域所在页码
+        :param ComponentPage: 签名域所在页码，1～N
         :type ComponentPage: int
         """
         self.VerifyResult = None
         self.SignPlatform = None
         self.SignerName = None
         self.SignTime = None
         self.SignAlgorithm = None
@@ -5036,15 +5058,15 @@
         :type Description: str
         :param RoleName: 角色名称
         :type RoleName: str
         :param RequireValidation: 是否需要验证，默认为false
         :type RequireValidation: bool
         :param RequireSign: 是否需要签署，默认为true
         :type RequireSign: bool
-        :param RoutingOrder: 添加序列
+        :param RoutingOrder: 添加序列，0～N
         :type RoutingOrder: int
         :param RequireDelivery: 是否需要发送，默认为true
         :type RequireDelivery: bool
         :param Email: 邮箱地址
         :type Email: str
         :param Mobile: 电话号码
         :type Mobile: str
@@ -5202,19 +5224,19 @@
 class RemindFlowRecords(AbstractModel):
     """催办接口返回详细信息
 
     """
 
     def __init__(self):
         r"""
-        :param CanRemind: 是否能够催办
+        :param CanRemind: 是否能够催办，true-是，false-否
         :type CanRemind: bool
         :param FlowId: 合同id
         :type FlowId: str
-        :param RemindMessage: 催办详情
+        :param RemindMessage: 催办详情信息
         :type RemindMessage: str
         """
         self.CanRemind = None
         self.FlowId = None
         self.RemindMessage = None
 
 
@@ -5238,15 +5260,15 @@
 
     def __init__(self):
         r"""
         :param QrCodeId: 二维码id
         :type QrCodeId: str
         :param QrCodeUrl: 二维码url
         :type QrCodeUrl: str
-        :param ExpiredTime: 二维码过期时间
+        :param ExpiredTime: 二维码过期时间戳，单位秒
         :type ExpiredTime: int
         """
         self.QrCodeId = None
         self.QrCodeUrl = None
         self.ExpiredTime = None
 
 
@@ -5318,17 +5340,17 @@
 注意：此字段可能返回 null，表示取不到有效值。
         :type Roles: list of StaffRole
         :param Department: 员工部门
 注意：此字段可能返回 null，表示取不到有效值。
         :type Department: :class:`tencentcloud.ess.v20201111.models.Department`
         :param Verified: 员工是否实名
         :type Verified: bool
-        :param CreatedOn: 员工创建时间戳
+        :param CreatedOn: 员工创建时间戳，单位秒
         :type CreatedOn: int
-        :param VerifiedOn: 员工实名时间戳
+        :param VerifiedOn: 员工实名时间戳，单位秒
 注意：此字段可能返回 null，表示取不到有效值。
         :type VerifiedOn: int
         :param QuiteJob: 员工是否离职：0-未离职，1-离职
 注意：此字段可能返回 null，表示取不到有效值。
         :type QuiteJob: int
         :param ReceiveUserId: 员工离职交接人用户id
         :type ReceiveUserId: str
@@ -5573,58 +5595,58 @@
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class TemplateInfo(AbstractModel):
-    """二期接口返回的模板的信息结构
+    """企业模板的信息结构
 
     """
 
     def __init__(self):
         r"""
         :param TemplateId: 模板ID
         :type TemplateId: str
         :param TemplateName: 模板名字
         :type TemplateName: str
         :param Description: 模板描述信息
         :type Description: str
-        :param DocumentResourceIds: 模板关联的资源IDs
+        :param DocumentResourceIds: 模板关联的资源ID列表
         :type DocumentResourceIds: list of str
         :param FileInfos: 返回的文件信息结构
         :type FileInfos: list of FileInfo
-        :param AttachmentResourceIds: 附件关联的资源ID是
+        :param AttachmentResourceIds: 附件关联的资源ID
         :type AttachmentResourceIds: list of str
         :param SignOrder: 签署顺序
         :type SignOrder: list of int
         :param Recipients: 签署参与者的信息
         :type Recipients: list of Recipient
         :param Components: 模板信息结构
         :type Components: list of Component
         :param SignComponents: 签署区模板信息结构
         :type SignComponents: list of Component
         :param Status: 模板状态(-1:不可用；0:草稿态；1:正式态)
         :type Status: int
-        :param Creator: 模板的创建人
+        :param Creator: 模板的创建人UserId
         :type Creator: str
-        :param CreatedOn: 模板创建的时间戳（精确到秒）
+        :param CreatedOn: 模板创建的时间戳，单位秒
         :type CreatedOn: int
         :param Promoter: 发起人角色信息
         :type Promoter: :class:`tencentcloud.ess.v20201111.models.Recipient`
         :param TemplateType: 模板类型
 取值：
 1  静默签,
 3  普通模板
         :type TemplateType: int
         :param Available: 模板可用状态，取值：1启用（默认），2停用
         :type Available: int
-        :param OrganizationId: 模板创建组织id
+        :param OrganizationId: 创建模板的机构id
         :type OrganizationId: str
-        :param PreviewUrl: 模板预览链接
+        :param PreviewUrl: 模板预览链接，有效时间5分钟
 注意：此字段可能返回 null，表示取不到有效值。
         :type PreviewUrl: str
         :param TemplateVersion: 模板版本。默认为空时，全数字字符，初始版本为yyyyMMdd001。
 注意：此字段可能返回 null，表示取不到有效值。
         :type TemplateVersion: str
         :param Published: 模板是否已发布。true-已发布；false-未发布
 注意：此字段可能返回 null，表示取不到有效值。
```

### Comparing `tencentcloud-sdk-python-ess-3.0.905/tencentcloud_sdk_python_ess.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.906/tencentcloud_sdk_python_ess.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.905
+Version: 3.0.906
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.905/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.906/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.905
+Version: 3.0.906
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.905/setup.py` & `tencentcloud-sdk-python-ess-3.0.906/setup.py`

 * *Files identical despite different names*

