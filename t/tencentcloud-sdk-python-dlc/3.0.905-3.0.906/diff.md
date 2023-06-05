# Comparing `tmp/tencentcloud-sdk-python-dlc-3.0.905.tar.gz` & `tmp/tencentcloud-sdk-python-dlc-3.0.906.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dlc-3.0.905.tar", last modified: Fri Jun  2 00:26:57 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dlc-3.0.906.tar", last modified: Mon Jun  5 00:33:02 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dlc-3.0.905.tar` & `tencentcloud-sdk-python-dlc-3.0.906.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:26:57.000000 tencentcloud-sdk-python-dlc-3.0.905/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-02 00:26:57.000000 tencentcloud-sdk-python-dlc-3.0.905/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:26:57.000000 tencentcloud-sdk-python-dlc-3.0.905/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:26:57.000000 tencentcloud-sdk-python-dlc-3.0.905/tencentcloud/dlc/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 00:26:57.000000 tencentcloud-sdk-python-dlc-3.0.905/tencentcloud/dlc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:26:57.000000 tencentcloud-sdk-python-dlc-3.0.905/tencentcloud/dlc/v20210125/
--rw-r--r--   0 root         (0) root         (0)    81336 2023-06-02 00:26:57.000000 tencentcloud-sdk-python-dlc-3.0.905/tencentcloud/dlc/v20210125/dlc_client.py
--rw-r--r--   0 root         (0) root         (0)    11538 2023-06-02 00:26:57.000000 tencentcloud-sdk-python-dlc-3.0.905/tencentcloud/dlc/v20210125/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 00:26:57.000000 tencentcloud-sdk-python-dlc-3.0.905/tencentcloud/dlc/v20210125/__init__.py
--rw-r--r--   0 root         (0) root         (0)   333828 2023-06-02 00:26:57.000000 tencentcloud-sdk-python-dlc-3.0.905/tencentcloud/dlc/v20210125/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-02 00:26:57.000000 tencentcloud-sdk-python-dlc-3.0.905/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-02 00:26:57.000000 tencentcloud-sdk-python-dlc-3.0.905/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-02 00:26:57.000000 tencentcloud-sdk-python-dlc-3.0.905/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:26:57.000000 tencentcloud-sdk-python-dlc-3.0.905/tencentcloud_sdk_python_dlc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 00:26:57.000000 tencentcloud-sdk-python-dlc-3.0.905/tencentcloud_sdk_python_dlc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-02 00:26:57.000000 tencentcloud-sdk-python-dlc-3.0.905/tencentcloud_sdk_python_dlc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-02 00:26:57.000000 tencentcloud-sdk-python-dlc-3.0.905/tencentcloud_sdk_python_dlc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-02 00:26:57.000000 tencentcloud-sdk-python-dlc-3.0.905/tencentcloud_sdk_python_dlc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-02 00:26:57.000000 tencentcloud-sdk-python-dlc-3.0.905/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:33:02.000000 tencentcloud-sdk-python-dlc-3.0.906/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-05 00:33:02.000000 tencentcloud-sdk-python-dlc-3.0.906/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:33:02.000000 tencentcloud-sdk-python-dlc-3.0.906/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:33:02.000000 tencentcloud-sdk-python-dlc-3.0.906/tencentcloud/dlc/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:33:02.000000 tencentcloud-sdk-python-dlc-3.0.906/tencentcloud/dlc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:33:02.000000 tencentcloud-sdk-python-dlc-3.0.906/tencentcloud/dlc/v20210125/
+-rw-r--r--   0 root         (0) root         (0)    81336 2023-06-05 00:33:02.000000 tencentcloud-sdk-python-dlc-3.0.906/tencentcloud/dlc/v20210125/dlc_client.py
+-rw-r--r--   0 root         (0) root         (0)    11538 2023-06-05 00:33:02.000000 tencentcloud-sdk-python-dlc-3.0.906/tencentcloud/dlc/v20210125/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:33:02.000000 tencentcloud-sdk-python-dlc-3.0.906/tencentcloud/dlc/v20210125/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   340367 2023-06-05 00:33:02.000000 tencentcloud-sdk-python-dlc-3.0.906/tencentcloud/dlc/v20210125/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-05 00:33:02.000000 tencentcloud-sdk-python-dlc-3.0.906/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-05 00:33:02.000000 tencentcloud-sdk-python-dlc-3.0.906/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-05 00:33:02.000000 tencentcloud-sdk-python-dlc-3.0.906/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:33:02.000000 tencentcloud-sdk-python-dlc-3.0.906/tencentcloud_sdk_python_dlc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 00:33:02.000000 tencentcloud-sdk-python-dlc-3.0.906/tencentcloud_sdk_python_dlc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-05 00:33:02.000000 tencentcloud-sdk-python-dlc-3.0.906/tencentcloud_sdk_python_dlc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-05 00:33:02.000000 tencentcloud-sdk-python-dlc-3.0.906/tencentcloud_sdk_python_dlc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-05 00:33:02.000000 tencentcloud-sdk-python-dlc-3.0.906/tencentcloud_sdk_python_dlc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-05 00:33:02.000000 tencentcloud-sdk-python-dlc-3.0.906/setup.cfg
```

### Comparing `tencentcloud-sdk-python-dlc-3.0.905/README.rst` & `tencentcloud-sdk-python-dlc-3.0.906/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dlc-3.0.905/tencentcloud/dlc/v20210125/dlc_client.py` & `tencentcloud-sdk-python-dlc-3.0.906/tencentcloud/dlc/v20210125/dlc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dlc-3.0.905/tencentcloud/dlc/v20210125/errorcodes.py` & `tencentcloud-sdk-python-dlc-3.0.906/tencentcloud/dlc/v20210125/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dlc-3.0.905/tencentcloud/dlc/v20210125/models.py` & `tencentcloud-sdk-python-dlc-3.0.906/tencentcloud/dlc/v20210125/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1204,14 +1204,16 @@
         :type ImageVersionName: str
         :param MainClusterName: 主集群名称
         :type MainClusterName: str
         :param ElasticSwitch: spark jar 包年包月集群是否开启弹性
         :type ElasticSwitch: bool
         :param ElasticLimit: spark jar 包年包月集群弹性上限
         :type ElasticLimit: int
+        :param SessionResourceTemplate: spark作业集群session资源配置模板
+        :type SessionResourceTemplate: :class:`tencentcloud.dlc.v20210125.models.SessionResourceTemplate`
         """
         self.EngineType = None
         self.DataEngineName = None
         self.ClusterType = None
         self.Mode = None
         self.AutoResume = None
         self.MinClusters = None
@@ -1234,14 +1236,15 @@
         self.AutoSuspendTime = None
         self.ResourceType = None
         self.DataEngineConfigPairs = None
         self.ImageVersionName = None
         self.MainClusterName = None
         self.ElasticSwitch = None
         self.ElasticLimit = None
+        self.SessionResourceTemplate = None
 
 
     def _deserialize(self, params):
         self.EngineType = params.get("EngineType")
         self.DataEngineName = params.get("DataEngineName")
         self.ClusterType = params.get("ClusterType")
         self.Mode = params.get("Mode")
@@ -1278,14 +1281,17 @@
                 obj = DataEngineConfigPair()
                 obj._deserialize(item)
                 self.DataEngineConfigPairs.append(obj)
         self.ImageVersionName = params.get("ImageVersionName")
         self.MainClusterName = params.get("MainClusterName")
         self.ElasticSwitch = params.get("ElasticSwitch")
         self.ElasticLimit = params.get("ElasticLimit")
+        if params.get("SessionResourceTemplate") is not None:
+            self.SessionResourceTemplate = SessionResourceTemplate()
+            self.SessionResourceTemplate._deserialize(params.get("SessionResourceTemplate"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -1961,14 +1967,16 @@
         :type SparkImage: str
         :param SparkImageVersion: Spark Image 版本名称
         :type SparkImageVersion: str
         :param AppExecutorMaxNumbers: 指定的Executor数量（最大值），默认为1，当开启动态分配有效，若未开启，则该值等于AppExecutorNums
         :type AppExecutorMaxNumbers: int
         :param SessionId: 关联dlc查询脚本id
         :type SessionId: str
+        :param IsInherit: 任务资源配置是否继承集群模板，0（默认）不继承，1：继承
+        :type IsInherit: int
         """
         self.AppName = None
         self.AppType = None
         self.DataEngine = None
         self.AppFile = None
         self.RoleArn = None
         self.AppDriverSize = None
@@ -1989,14 +1997,15 @@
         self.AppPythonFiles = None
         self.IsLocalArchives = None
         self.AppArchives = None
         self.SparkImage = None
         self.SparkImageVersion = None
         self.AppExecutorMaxNumbers = None
         self.SessionId = None
+        self.IsInherit = None
 
 
     def _deserialize(self, params):
         self.AppName = params.get("AppName")
         self.AppType = params.get("AppType")
         self.DataEngine = params.get("DataEngine")
         self.AppFile = params.get("AppFile")
@@ -2019,14 +2028,15 @@
         self.AppPythonFiles = params.get("AppPythonFiles")
         self.IsLocalArchives = params.get("IsLocalArchives")
         self.AppArchives = params.get("AppArchives")
         self.SparkImage = params.get("SparkImage")
         self.SparkImageVersion = params.get("SparkImageVersion")
         self.AppExecutorMaxNumbers = params.get("AppExecutorMaxNumbers")
         self.SessionId = params.get("SessionId")
+        self.IsInherit = params.get("IsInherit")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -3183,14 +3193,32 @@
         :type StartStandbyCluster: bool
         :param ElasticSwitch: spark jar 包年包月集群是否开启弹性
 注意：此字段可能返回 null，表示取不到有效值。
         :type ElasticSwitch: bool
         :param ElasticLimit: spark jar 包年包月集群弹性上限
 注意：此字段可能返回 null，表示取不到有效值。
         :type ElasticLimit: int
+        :param DefaultHouse: 是否为默认引擎
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DefaultHouse: bool
+        :param MaxConcurrency: 单个集群任务最大并发数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type MaxConcurrency: int
+        :param TolerableQueueTime: 任务排队上限时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TolerableQueueTime: int
+        :param UserAppId: 用户appid
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UserAppId: int
+        :param UserUin: 用户uin
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UserUin: str
+        :param SessionResourceTemplate: SessionResourceTemplate
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SessionResourceTemplate: :class:`tencentcloud.dlc.v20210125.models.SessionResourceTemplate`
         """
         self.DataEngineName = None
         self.EngineType = None
         self.ClusterType = None
         self.QuotaId = None
         self.State = None
         self.CreateTime = None
@@ -3223,14 +3251,20 @@
         self.ResourceType = None
         self.ImageVersionId = None
         self.ChildImageVersionId = None
         self.ImageVersionName = None
         self.StartStandbyCluster = None
         self.ElasticSwitch = None
         self.ElasticLimit = None
+        self.DefaultHouse = None
+        self.MaxConcurrency = None
+        self.TolerableQueueTime = None
+        self.UserAppId = None
+        self.UserUin = None
+        self.SessionResourceTemplate = None
 
 
     def _deserialize(self, params):
         self.DataEngineName = params.get("DataEngineName")
         self.EngineType = params.get("EngineType")
         self.ClusterType = params.get("ClusterType")
         self.QuotaId = params.get("QuotaId")
@@ -3277,14 +3311,22 @@
         self.ResourceType = params.get("ResourceType")
         self.ImageVersionId = params.get("ImageVersionId")
         self.ChildImageVersionId = params.get("ChildImageVersionId")
         self.ImageVersionName = params.get("ImageVersionName")
         self.StartStandbyCluster = params.get("StartStandbyCluster")
         self.ElasticSwitch = params.get("ElasticSwitch")
         self.ElasticLimit = params.get("ElasticLimit")
+        self.DefaultHouse = params.get("DefaultHouse")
+        self.MaxConcurrency = params.get("MaxConcurrency")
+        self.TolerableQueueTime = params.get("TolerableQueueTime")
+        self.UserAppId = params.get("UserAppId")
+        self.UserUin = params.get("UserUin")
+        if params.get("SessionResourceTemplate") is not None:
+            self.SessionResourceTemplate = SessionResourceTemplate()
+            self.SessionResourceTemplate._deserialize(params.get("SessionResourceTemplate"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -3455,15 +3497,15 @@
         :type UserAlias: str
         :param UserSubUin: 建库用户ID
 注意：此字段可能返回 null，表示取不到有效值。
         :type UserSubUin: str
         :param GovernPolicy: 数据治理配置项
 注意：此字段可能返回 null，表示取不到有效值。
         :type GovernPolicy: :class:`tencentcloud.dlc.v20210125.models.DataGovernPolicy`
-        :param DatabaseId: 数据库ID
+        :param DatabaseId: 数据库ID（无效字段）
 注意：此字段可能返回 null，表示取不到有效值。
         :type DatabaseId: str
         """
         self.DatabaseName = None
         self.Comment = None
         self.Properties = None
         self.CreateTime = None
@@ -6682,14 +6724,16 @@
         :type SparkImage: str
         :param SparkImageVersion: Spark Image 版本名称
         :type SparkImageVersion: str
         :param AppExecutorMaxNumbers: 指定的Executor数量（最大值），默认为1，当开启动态分配有效，若未开启，则该值等于AppExecutorNums
         :type AppExecutorMaxNumbers: int
         :param SessionId: 关联dlc查询脚本
         :type SessionId: str
+        :param IsInherit: 任务资源配置是否继承集群配置模板：0（默认）不继承、1：继承
+        :type IsInherit: int
         """
         self.AppName = None
         self.AppType = None
         self.DataEngine = None
         self.AppFile = None
         self.RoleArn = None
         self.AppDriverSize = None
@@ -6711,14 +6755,15 @@
         self.DataSource = None
         self.IsLocalArchives = None
         self.AppArchives = None
         self.SparkImage = None
         self.SparkImageVersion = None
         self.AppExecutorMaxNumbers = None
         self.SessionId = None
+        self.IsInherit = None
 
 
     def _deserialize(self, params):
         self.AppName = params.get("AppName")
         self.AppType = params.get("AppType")
         self.DataEngine = params.get("DataEngine")
         self.AppFile = params.get("AppFile")
@@ -6742,14 +6787,15 @@
         self.DataSource = params.get("DataSource")
         self.IsLocalArchives = params.get("IsLocalArchives")
         self.AppArchives = params.get("AppArchives")
         self.SparkImage = params.get("SparkImage")
         self.SparkImageVersion = params.get("SparkImageVersion")
         self.AppExecutorMaxNumbers = params.get("AppExecutorMaxNumbers")
         self.SessionId = params.get("SessionId")
+        self.IsInherit = params.get("IsInherit")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -7601,14 +7647,54 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class SessionResourceTemplate(AbstractModel):
+    """Spark批作业集群Session资源配置模板；
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DriverSize: driver规格：small,medium,large,xlarge；内存型(引擎类型)：m.small,m.medium,m.large,m.xlarge
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DriverSize: str
+        :param ExecutorSize: executor规格：small,medium,large,xlarge；内存型(引擎类型)：m.small,m.medium,m.large,m.xlarge
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ExecutorSize: str
+        :param ExecutorNums: 指定executor数量，最小值为1，最大值小于集群规格
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ExecutorNums: int
+        :param ExecutorMaxNumbers: 指定executor max数量（动态配置场景下），最小值为1，最大值小于集群规格（当ExecutorMaxNumbers小于ExecutorNums时，改值设定为ExecutorNums）
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ExecutorMaxNumbers: int
+        """
+        self.DriverSize = None
+        self.ExecutorSize = None
+        self.ExecutorNums = None
+        self.ExecutorMaxNumbers = None
+
+
+    def _deserialize(self, params):
+        self.DriverSize = params.get("DriverSize")
+        self.ExecutorSize = params.get("ExecutorSize")
+        self.ExecutorNums = params.get("ExecutorNums")
+        self.ExecutorMaxNumbers = params.get("ExecutorMaxNumbers")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class SparkJobInfo(AbstractModel):
     """spark作业详情。
 
     """
 
     def __init__(self):
         r"""
@@ -7701,14 +7787,17 @@
         :type SessionId: str
         :param DataEngineClusterType: spark_emr_livy
 注意：此字段可能返回 null，表示取不到有效值。
         :type DataEngineClusterType: str
         :param DataEngineImageVersion: Spark 3.2-EMR
 注意：此字段可能返回 null，表示取不到有效值。
         :type DataEngineImageVersion: str
+        :param IsInherit: 任务资源配置是否继承集群模板，0（默认）不继承，1：继承
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IsInherit: int
         """
         self.JobId = None
         self.JobName = None
         self.JobType = None
         self.DataEngine = None
         self.Eni = None
         self.IsLocal = None
@@ -7741,14 +7830,15 @@
         self.TaskNum = None
         self.DataEngineStatus = None
         self.JobExecutorMaxNumbers = None
         self.SparkImageVersion = None
         self.SessionId = None
         self.DataEngineClusterType = None
         self.DataEngineImageVersion = None
+        self.IsInherit = None
 
 
     def _deserialize(self, params):
         self.JobId = params.get("JobId")
         self.JobName = params.get("JobName")
         self.JobType = params.get("JobType")
         self.DataEngine = params.get("DataEngine")
@@ -7785,14 +7875,15 @@
         self.TaskNum = params.get("TaskNum")
         self.DataEngineStatus = params.get("DataEngineStatus")
         self.JobExecutorMaxNumbers = params.get("JobExecutorMaxNumbers")
         self.SparkImageVersion = params.get("SparkImageVersion")
         self.SessionId = params.get("SessionId")
         self.DataEngineClusterType = params.get("DataEngineClusterType")
         self.DataEngineImageVersion = params.get("DataEngineImageVersion")
+        self.IsInherit = params.get("IsInherit")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -8349,25 +8440,29 @@
         :type InputFormat: str
         :param StorageSize: 数据表存储大小（单位：Byte）
 注意：此字段可能返回 null，表示取不到有效值。
         :type StorageSize: int
         :param RecordCount: 数据表行数
 注意：此字段可能返回 null，表示取不到有效值。
         :type RecordCount: int
+        :param MapMaterializedViewName: xxxx
+注意：此字段可能返回 null，表示取不到有效值。
+        :type MapMaterializedViewName: str
         """
         self.TableBaseInfo = None
         self.Columns = None
         self.Partitions = None
         self.Location = None
         self.Properties = None
         self.ModifiedTime = None
         self.CreateTime = None
         self.InputFormat = None
         self.StorageSize = None
         self.RecordCount = None
+        self.MapMaterializedViewName = None
 
 
     def _deserialize(self, params):
         if params.get("TableBaseInfo") is not None:
             self.TableBaseInfo = TableBaseInfo()
             self.TableBaseInfo._deserialize(params.get("TableBaseInfo"))
         if params.get("Columns") is not None:
@@ -8390,14 +8485,15 @@
                 obj._deserialize(item)
                 self.Properties.append(obj)
         self.ModifiedTime = params.get("ModifiedTime")
         self.CreateTime = params.get("CreateTime")
         self.InputFormat = params.get("InputFormat")
         self.StorageSize = params.get("StorageSize")
         self.RecordCount = params.get("RecordCount")
+        self.MapMaterializedViewName = params.get("MapMaterializedViewName")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -8549,14 +8645,29 @@
         :type UiUrl: str
         :param TotalTime: 任务耗时，单位： ms
 注意：此字段可能返回 null，表示取不到有效值。
         :type TotalTime: int
         :param CmdArgs: spark app job执行task的程序入口参数
 注意：此字段可能返回 null，表示取不到有效值。
         :type CmdArgs: str
+        :param ImageVersion: 集群镜像大版本名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ImageVersion: str
+        :param DriverSize: driver规格：small,medium,large,xlarge；内存型(引擎类型)：m.small,m.medium,m.large,m.xlarge
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DriverSize: str
+        :param ExecutorSize: executor规格：small,medium,large,xlarge；内存型(引擎类型)：m.small,m.medium,m.large,m.xlarge
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ExecutorSize: str
+        :param ExecutorNums: 指定executor数量，最小值为1，最大值小于集群规格
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ExecutorNums: int
+        :param ExecutorMaxNumbers: 指定executor max数量（动态配置场景下），最小值为1，最大值小于集群规格（当ExecutorMaxNumbers小于ExecutorNums时，改值设定为ExecutorNums）
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ExecutorMaxNumbers: int
         """
         self.DatabaseName = None
         self.DataAmount = None
         self.Id = None
         self.UsedTime = None
         self.OutputPath = None
         self.CreateTime = None
@@ -8582,14 +8693,19 @@
         self.UserAlias = None
         self.SparkJobName = None
         self.SparkJobId = None
         self.SparkJobFile = None
         self.UiUrl = None
         self.TotalTime = None
         self.CmdArgs = None
+        self.ImageVersion = None
+        self.DriverSize = None
+        self.ExecutorSize = None
+        self.ExecutorNums = None
+        self.ExecutorMaxNumbers = None
 
 
     def _deserialize(self, params):
         self.DatabaseName = params.get("DatabaseName")
         self.DataAmount = params.get("DataAmount")
         self.Id = params.get("Id")
         self.UsedTime = params.get("UsedTime")
@@ -8617,14 +8733,19 @@
         self.UserAlias = params.get("UserAlias")
         self.SparkJobName = params.get("SparkJobName")
         self.SparkJobId = params.get("SparkJobId")
         self.SparkJobFile = params.get("SparkJobFile")
         self.UiUrl = params.get("UiUrl")
         self.TotalTime = params.get("TotalTime")
         self.CmdArgs = params.get("CmdArgs")
+        self.ImageVersion = params.get("ImageVersion")
+        self.DriverSize = params.get("DriverSize")
+        self.ExecutorSize = params.get("ExecutorSize")
+        self.ExecutorNums = params.get("ExecutorNums")
+        self.ExecutorMaxNumbers = params.get("ExecutorMaxNumbers")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-dlc-3.0.905/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dlc-3.0.906/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-dlc-3.0.905/PKG-INFO` & `tencentcloud-sdk-python-dlc-3.0.906/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dlc
-Version: 3.0.905
+Version: 3.0.906
 Summary: Tencent Cloud Dlc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dlc-3.0.905/setup.py` & `tencentcloud-sdk-python-dlc-3.0.906/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dlc-3.0.905/tencentcloud_sdk_python_dlc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dlc-3.0.906/tencentcloud_sdk_python_dlc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dlc
-Version: 3.0.905
+Version: 3.0.906
 Summary: Tencent Cloud Dlc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

