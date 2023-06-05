# Comparing `tmp/chariot-sdk-1.3.0.tar.gz` & `tmp/chariot-sdk-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chariot-sdk-1.3.0.tar", last modified: Fri Mar 31 07:20:23 2023, max compression
+gzip compressed data, was "chariot-sdk-1.3.1.tar", last modified: Mon Jun  5 05:44:44 2023, max compression
```

## Comparing `chariot-sdk-1.3.0.tar` & `chariot-sdk-1.3.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-03-31 07:20:23.241387 chariot-sdk-1.3.0/
--rw-rw-rw-   0        0        0      225 2023-03-23 01:34:20.000000 chariot-sdk-1.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4741 2023-03-31 07:20:23.240388 chariot-sdk-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     4489 2023-03-31 03:48:26.000000 chariot-sdk-1.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-31 07:20:23.215601 chariot-sdk-1.3.0/chariotCore/
--rw-rw-rw-   0        0        0       20 2023-03-22 01:38:55.000000 chariot-sdk-1.3.0/chariotCore/__init__.py
--rw-rw-rw-   0        0        0     5146 2023-03-29 06:48:43.000000 chariot-sdk-1.3.0/chariotCore/main.py
-drwxrwxrwx   0        0        0        0 2023-03-31 07:20:23.222601 chariot-sdk-1.3.0/chariotCore/res/
--rw-rw-rw-   0        0        0      728 2023-03-24 03:56:05.000000 chariot-sdk-1.3.0/chariotCore/res/Dockerfile
-drwxrwxrwx   0        0        0        0 2023-03-31 07:20:23.231821 chariot-sdk-1.3.0/chariotCore/res/SDK/
--rw-rw-rw-   0        0        0       18 2023-03-22 01:39:54.000000 chariot-sdk-1.3.0/chariotCore/res/SDK/__init__.py
--rw-rw-rw-   0        0        0    19623 2023-03-31 03:50:40.000000 chariot-sdk-1.3.0/chariotCore/res/SDK/base.py
--rw-rw-rw-   0        0        0     4295 2023-03-29 02:07:51.000000 chariot-sdk-1.3.0/chariotCore/res/SDK/chariot.py
--rw-rw-rw-   0        0        0     2382 2023-03-30 03:07:22.000000 chariot-sdk-1.3.0/chariotCore/res/SDK/cli.py
--rw-rw-rw-   0        0        0     1982 2023-03-22 01:40:07.000000 chariot-sdk-1.3.0/chariotCore/res/SDK/models.py
--rw-rw-rw-   0        0        0    12157 2023-03-31 07:06:50.000000 chariot-sdk-1.3.0/chariotCore/res/SDK/subassembly.py
--rw-rw-rw-   0        0        0    13910 2023-03-31 07:06:59.000000 chariot-sdk-1.3.0/chariotCore/res/SDK/web.py
--rw-rw-rw-   0        0        0        1 2023-03-22 01:39:01.000000 chariot-sdk-1.3.0/chariotCore/res/__init__.py
--rw-rw-rw-   0        0        0      742 2023-03-31 07:00:07.000000 chariot-sdk-1.3.0/chariotCore/res/config.ini
--rw-rw-rw-   0        0        0    29297 2022-04-11 01:54:53.000000 chariot-sdk-1.3.0/chariotCore/res/icon.png
--rw-rw-rw-   0        0        0      187 2023-03-29 05:45:08.000000 chariot-sdk-1.3.0/chariotCore/res/plugin.spec.yaml
--rw-rw-rw-   0        0        0       73 2023-03-22 01:39:45.000000 chariot-sdk-1.3.0/chariotCore/res/requirements.txt
--rw-rw-rw-   0        0        0    11834 2023-03-29 07:31:33.000000 chariot-sdk-1.3.0/chariotCore/tasks.py
--rw-rw-rw-   0        0        0    33935 2023-03-31 02:41:04.000000 chariot-sdk-1.3.0/chariotCore/templates.py
--rw-rw-rw-   0        0        0    49506 2023-03-29 07:30:00.000000 chariot-sdk-1.3.0/chariotCore/tools.py
-drwxrwxrwx   0        0        0        0 2023-03-31 07:20:23.239390 chariot-sdk-1.3.0/chariot_sdk.egg-info/
--rw-rw-rw-   0        0        0     4741 2023-03-31 07:20:22.000000 chariot-sdk-1.3.0/chariot_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      736 2023-03-31 07:20:22.000000 chariot-sdk-1.3.0/chariot_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-31 07:20:22.000000 chariot-sdk-1.3.0/chariot_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-03-31 07:20:22.000000 chariot-sdk-1.3.0/chariot_sdk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       81 2023-03-31 07:20:22.000000 chariot-sdk-1.3.0/chariot_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-03-31 07:20:22.000000 chariot-sdk-1.3.0/chariot_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-31 07:20:23.241387 chariot-sdk-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1255 2023-03-22 08:34:44.000000 chariot-sdk-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 05:44:44.262516 chariot-sdk-1.3.1/
+-rw-rw-rw-   0        0        0      225 2023-04-06 02:58:21.000000 chariot-sdk-1.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     6048 2023-06-05 05:44:44.261632 chariot-sdk-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5796 2023-06-05 03:58:05.000000 chariot-sdk-1.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 05:44:44.197076 chariot-sdk-1.3.1/chariotCore/
+-rw-rw-rw-   0        0        0       20 2023-04-19 03:33:16.000000 chariot-sdk-1.3.1/chariotCore/__init__.py
+-rw-rw-rw-   0        0        0     5390 2023-04-27 03:57:04.000000 chariot-sdk-1.3.1/chariotCore/main.py
+drwxrwxrwx   0        0        0        0 2023-06-05 05:44:44.205077 chariot-sdk-1.3.1/chariotCore/res/
+-rw-rw-rw-   0        0        0      728 2023-04-19 03:33:43.000000 chariot-sdk-1.3.1/chariotCore/res/Dockerfile
+drwxrwxrwx   0        0        0        0 2023-06-05 05:44:44.222054 chariot-sdk-1.3.1/chariotCore/res/SDK/
+-rw-rw-rw-   0        0        0       18 2023-04-14 04:07:29.000000 chariot-sdk-1.3.1/chariotCore/res/SDK/__init__.py
+-rw-rw-rw-   0        0        0    20196 2023-04-20 02:42:22.000000 chariot-sdk-1.3.1/chariotCore/res/SDK/base.py
+-rw-rw-rw-   0        0        0     4104 2023-04-20 03:52:25.000000 chariot-sdk-1.3.1/chariotCore/res/SDK/chariot.py
+-rw-rw-rw-   0        0        0     2382 2023-04-10 07:11:20.000000 chariot-sdk-1.3.1/chariotCore/res/SDK/cli.py
+-rw-rw-rw-   0        0        0     2641 2023-05-06 10:07:45.000000 chariot-sdk-1.3.1/chariotCore/res/SDK/models.py
+-rw-rw-rw-   0        0        0    12157 2023-04-10 07:11:24.000000 chariot-sdk-1.3.1/chariotCore/res/SDK/subassembly.py
+-rw-rw-rw-   0        0        0    18426 2023-05-12 02:19:25.000000 chariot-sdk-1.3.1/chariotCore/res/SDK/web.py
+-rw-rw-rw-   0        0        0        1 2023-03-22 01:39:01.000000 chariot-sdk-1.3.1/chariotCore/res/__init__.py
+-rw-rw-rw-   0        0        0      712 2023-04-27 08:19:16.000000 chariot-sdk-1.3.1/chariotCore/res/config.ini
+-rw-rw-rw-   0        0        0    29297 2022-04-11 01:54:53.000000 chariot-sdk-1.3.1/chariotCore/res/icon.png
+-rw-rw-rw-   0        0        0      161 2023-04-23 02:20:36.000000 chariot-sdk-1.3.1/chariotCore/res/plugin.spec.yaml
+-rw-rw-rw-   0        0        0       73 2023-03-22 01:39:45.000000 chariot-sdk-1.3.1/chariotCore/res/requirements.txt
+-rw-rw-rw-   0        0        0    12874 2023-04-27 08:17:13.000000 chariot-sdk-1.3.1/chariotCore/tasks.py
+-rw-rw-rw-   0        0        0    29369 2023-05-19 02:36:28.000000 chariot-sdk-1.3.1/chariotCore/templates.py
+-rw-rw-rw-   0        0        0    40487 2023-05-16 06:23:27.000000 chariot-sdk-1.3.1/chariotCore/tools.py
+drwxrwxrwx   0        0        0        0 2023-06-05 05:44:44.260925 chariot-sdk-1.3.1/chariot_sdk.egg-info/
+-rw-rw-rw-   0        0        0     6048 2023-06-05 05:44:44.000000 chariot-sdk-1.3.1/chariot_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      736 2023-06-05 05:44:44.000000 chariot-sdk-1.3.1/chariot_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 05:44:44.000000 chariot-sdk-1.3.1/chariot_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-06-05 05:44:44.000000 chariot-sdk-1.3.1/chariot_sdk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       81 2023-06-05 05:44:44.000000 chariot-sdk-1.3.1/chariot_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-05 05:44:44.000000 chariot-sdk-1.3.1/chariot_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 05:44:44.262516 chariot-sdk-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1255 2023-04-06 02:58:22.000000 chariot-sdk-1.3.1/setup.py
```

### Comparing `chariot-sdk-1.3.0/PKG-INFO` & `chariot-sdk-1.3.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chariot-sdk
-Version: 1.3.0
+Version: 1.3.1
 Summary: Chariot plugin maker
 Home-page: https://pypi.org/
 Author: chariot
 Author-email: chariot@example.com
 License: MIT
 Requires-Python: >=3
 Description-Content-Type: text/markdown
@@ -20,14 +20,31 @@
 - python 3.8+
 
 ### 安装
 > pip install chariot-sdk
 
 ### 更新日志
 
+> 1.3.0 -> 1.3.1
+
+- 修改资产接收器的输出结构，现在资产的key值将决定前端展示的文本
+- 去除yaml文件中的multi_workers、hot_update参数，新增sdk参数用于记录开发插件用的SDK版本，以后千乘将根据sdk参数（版本）来判断插件支持的功能
+- 添加-r命令下测试资产接收器的功能
+- api接口现在会限制测试时接收器的数量为1，在启动下一个接收器时，上一个接收器会被自动关闭（也可以手动关闭接收器）
+- 提高了SDK对插件出现错误时的兼容，从而更好地防范热改动功能引发的SDK崩溃
+- 新增了更多的可能的错误信息日志、
+- 新增对打包不同架构的离线包支持，现在可以在-mki命令后添加平台参数以获得不同架构下的离线包，如chariot-plugin -mki linux/arm64
+- 打包插件现在会在压缩包内自动添加上插件的结构信息和代码信息（plugin.construction.json），以适应将来上线的热改动功能
+- 现在打包好的插件会被放在插件根目录下的builds文件夹内
+- 重构了自动生成插件的功能
+- 重构了获取插件定义数据的功能
+- 修正了一些chariot-plugin -h中的帮助内容
+- 删除testserver测试功能
+- 调整生成插件时的模板文件
+
 > 1.2.10 -> 1.3.0
 
 - 修复了非Debug模式下，debug等级的日志仍然会在某种条件下输出的bug
 - 修复了Debug模式切换后无法切换回去的bug
 - 调整了重载配置行为的位置，修复了原来在完成连接器的运行后才加载配置的bug
 - 新增资产接收器模块，此模块专门用于转发资产相关的信息
 - 新增查询插件使用SDK版本信息接口
```

### Comparing `chariot-sdk-1.3.0/README.md` & `chariot-sdk-1.3.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -9,14 +9,31 @@
 - python 3.8+
 
 ### 安装
 > pip install chariot-sdk
 
 ### 更新日志
 
+> 1.3.0 -> 1.3.1
+
+- 修改资产接收器的输出结构，现在资产的key值将决定前端展示的文本
+- 去除yaml文件中的multi_workers、hot_update参数，新增sdk参数用于记录开发插件用的SDK版本，以后千乘将根据sdk参数（版本）来判断插件支持的功能
+- 添加-r命令下测试资产接收器的功能
+- api接口现在会限制测试时接收器的数量为1，在启动下一个接收器时，上一个接收器会被自动关闭（也可以手动关闭接收器）
+- 提高了SDK对插件出现错误时的兼容，从而更好地防范热改动功能引发的SDK崩溃
+- 新增了更多的可能的错误信息日志、
+- 新增对打包不同架构的离线包支持，现在可以在-mki命令后添加平台参数以获得不同架构下的离线包，如chariot-plugin -mki linux/arm64
+- 打包插件现在会在压缩包内自动添加上插件的结构信息和代码信息（plugin.construction.json），以适应将来上线的热改动功能
+- 现在打包好的插件会被放在插件根目录下的builds文件夹内
+- 重构了自动生成插件的功能
+- 重构了获取插件定义数据的功能
+- 修正了一些chariot-plugin -h中的帮助内容
+- 删除testserver测试功能
+- 调整生成插件时的模板文件
+
 > 1.2.10 -> 1.3.0
 
 - 修复了非Debug模式下，debug等级的日志仍然会在某种条件下输出的bug
 - 修复了Debug模式切换后无法切换回去的bug
 - 调整了重载配置行为的位置，修复了原来在完成连接器的运行后才加载配置的bug
 - 新增资产接收器模块，此模块专门用于转发资产相关的信息
 - 新增查询插件使用SDK版本信息接口
```

### Comparing `chariot-sdk-1.3.0/chariotCore/main.py` & `chariot-sdk-1.3.1/chariotCore/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,38 +9,42 @@
 
     千乘系统插件生成器 v{VERSION}
 
 #   -h, --help              查看帮助信息
 
 #   -v, --version           查看版本
 
-#   -g --generate           生成插件，需要yaml或json类型的插件定义文件路径参数。
-                            建议每次改动插件定义文件时重新生成一次插件。 
-                            注意，重新生成插件会覆盖不同组件的models.py校验文件。
+#   -g --generate           生成插件，需要yaml或json类型的插件定义文件路径参数
+                            建议每次改动插件定义文件时重新生成一次插件
+                            注意，重新生成插件会覆盖不同组件的models.py校验文件
                             使用示例：chariot-plugin -g .\plugin.spec.yaml
                             
-#   -ag, --auto_generate    自动生成高度模板化插件，需要特殊格式的插件定义文件路径。
+#   -ag, --auto_generate    自动生成高度模板化插件，需要特殊格式的插件定义文件路径
                             此方法一般自动调用。
                             
 #   -y, --yaml              在当前工作目录下生成一个yaml模板文件用于编写插件参数
 
-#   -r, --run               运行插件指定功能，需要json格式的数据参数。
-                            注意，此命令会尝试运行完成一个功能的完整流程，并且发送真实请求。
+#   -r, --run               运行插件指定功能，需要json格式的数据参数
+                            注意，此命令会尝试运行完成一个功能的完整流程，并且可能发送真实请求
                             使用示例：chariot-plugin -r tests\example_action.json
                             
 #   -hp, --http             启动api接口，插件以REST服务的形式对外提供服务，用于测试和使用接口
+                            默认启动 4 个API子进程
+                            可通过在-hp命令后加上数字的方式调整启用的进程数
 
-#   -t, --test              测试插件指定功能的连接器(connection)部分，需要json格式的数据参数。
-                            注意，此命令可能会发送真实请求。
+#   -t, --test              测试插件指定功能的连接器(connection)部分，需要json格式的数据参数
+                            注意，此命令可能会发送真实请求
                             使用示例：chariot-plugin -t tests\example_action.json
                             
 #   -tb, --tarball          插件打包，生成在线包，用于在线环境的插件安装，打包后的文件较小
 
-#   -mki, --mkimg           制作成docker镜像，生成离线包，用于离线环境的插件安装。
+#   -mki, --mkimg           制作成docker镜像，生成离线包，用于离线环境的插件安装
                             注意，打包时需要联网，打包后的文件较大
+                            可传入平台参数来决定所使用的架构，如，linux/386，linux/arm64
+                            不填则默认根据当前开发环境的架构进行打包
     """
 
     parser = argparse.ArgumentParser(formatter_class=argparse.RawDescriptionHelpFormatter, description=description)
 
     #   添加命令
     parser.add_argument("-v", "--version", help="查看版本", action='version', version=f"chariot-sdk: {VERSION}")
     parser.add_argument("-g", "--generate",
@@ -60,29 +64,29 @@
                         help="测试连接器",
                         action="append")
     parser.add_argument("-tb", "--tarball",
                         help="生成在线包",
                         action="store_true")
     parser.add_argument("-mki", "--mkimg",
                         help="生成离线包",
-                        action="store_true")
+                        nargs='?', const="", type=str)
 
     #   获取add_argument中action的参数
     args = parser.parse_args()
 
     #   生成插件
     if args.generate:
         #   需要当前工作区的绝对路径和yaml文件的相对路径
         file_path = args.generate[0]
         generate(os.getcwd(), file_path)
 
     #   自动生成插件
     elif args.auto_generate:
         file_path = args.auto_generate[0]
-        autoGenerate(os.getcwd(), file_path)
+        return autoGenerate(os.getcwd(), file_path)
 
     #   在当前工作目录下生成一个yaml模板文件
     elif args.yaml:
         #   需要当前工作区的绝对路径
         generateYaml(os.getcwd())
 
     #   根据tests文件下的json文件内填写的参数，以正常流程(包括使用连接器)运行插件内不同的组件
@@ -101,24 +105,17 @@
         #   需要当前工作区的绝对路径
         if args.http < 0:
             log("error", f"错误的工作进程数量：{args.http}")
             return
         else:
             http(os.getcwd(), args.http)
 
-
-
     #   打包在线包
     elif args.tarball:
         tarball(os.getcwd())
 
     #   打包离线包
-    elif args.mkimg:
-        mkimg(os.getcwd())
-
-    #   启动api测试服务
-    #   **此方法暂时弃用**
-    # elif args.testserver:
-    # testserver(os.getcwd())
+    elif args.mkimg or args.mkimg == "":
+        mkimg(args.mkimg)
 
     else:
         logging.info("输入 chariot-plugin -h 以获取帮助")
```

### Comparing `chariot-sdk-1.3.0/chariotCore/res/Dockerfile` & `chariot-sdk-1.3.1/chariotCore/res/Dockerfile`

 * *Files identical despite different names*

### Comparing `chariot-sdk-1.3.0/chariotCore/res/SDK/base.py` & `chariot-sdk-1.3.1/chariotCore/res/SDK/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -619,7 +619,29 @@
                 else:
                     p_temp[k] = temp
             elif p_temp[k] in ["", {}, None, []]:
                 p_temp.remove(p_temp[k])
                 return popEmpty(p_temp)
         return p_temp
     return p_temp
+
+
+def getPluginData():
+    """
+    #   获取插件定义数据
+    """
+
+    yaml_data_path = os.path.join(os.getcwd(), "plugin.spec.yaml")
+
+    json_data_path = os.path.join(os.getcwd(), "plugin.spec.json")
+
+    if os.path.exists(yaml_data_path):
+        with open(yaml_data_path, "r", encoding="utf-8") as file:
+            plugin_data = yaml.load(file.read(), Loader=yaml.FullLoader)
+        return plugin_data
+
+    elif os.path.exists(json_data_path):
+        plugin_data = json.load(open(json_data_path, "r"))
+        return plugin_data
+
+    else:
+        return None
```

### Comparing `chariot-sdk-1.3.0/chariotCore/res/SDK/chariot.py` & `chariot-sdk-1.3.1/chariotCore/res/SDK/chariot.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 from .base import *
 from .web import runserver
 
-
 ####
 #
 #   这里的方法主要是给开发时测试用的
 #   但事实上，老版本千乘在创建触发器、告警接收器、情报接收器也会通过这里创建
 #
 ####
 
+_modules_dict = {
+    "action": "动作",
+    "trigger": "触发器",
+    "alarm": "告警接收器",
+    "receiver": "情报接收器",
+    "asset": "资产接收器"
+}
+
+_modules_list = ["action", "trigger", "alarm", "receiver", "asset"]
+
 
 def run(data: dict, plugin_object):
     """
     #   运行功能的整个流程
     参数说明：
     data:dict,      #   运行功能时的必要的数据
     plugin_object:PLUGIN,      #   插件集合对象（类位于生成的插件后的根目录下main.py文件内）
@@ -25,46 +34,36 @@
     data_body = data.get("body")
     if not data_body:
         log("error", "body 为空")
         return
 
     log("info", "检测需要运行的组件")
 
-    modules_list = ["action", "trigger", "alarm", "receiver", "asset"]
-
     #   检查json数据是使用在哪个组件上的
-    for module in modules_list:
+    for module in _modules_list:
         if data_body.get(module):
             runModule(data_body[module], data_body, plugin_object, module)
             return
 
     log("info", "未检测到需要运行的组件")
 
 
 def runModule(func_name: str, data: dict, plugin_object, module):
     """
     #   运行功能
     参数说明：
     func_name:str,  #   功能名称（功能ID）
     data:dict,      #   运行功能时的必要的数据
     plugin_object:PLUGIN,      #   插件集合对象（类位于生成的插件后的根目录下main.py文件内）
-    module:str,     #   组件，module = actions,
+    module:str,     #   组件，module = action, trigger, alarm, receiver, asset
 
     出现异常时，会将异常信息放入log，但不会抛出异常
     """
 
-    module_dict = {
-        "action": "动作",
-        "trigger": "触发器",
-        "alarm": "告警接收器",
-        "receiver": "情报接收器",
-        "asset": "资产接收器"
-    }
-
-    log("info", f"运行{module_dict[module]}（{module}）中")
+    log("info", f"运行{_modules_dict[module]}（{module}）中")
 
     plugin_object_dict = {
         "action": plugin_object.actions,
         "trigger": plugin_object.triggers,
         "alarm": plugin_object.alarm_receivers,
         "receiver": plugin_object.indicator_receivers,
         "asset": plugin_object.asset_receivers
@@ -82,54 +81,46 @@
     else:
         #   数据转发URL
         dispatcher_url = data.get("dispatcher").get("url")
         #   缓存服务URL
         cache_url = data.get("dispatcher").get("cache_url")
         func._run(input_data, connection_data, dispatcher_url, cache_url)
 
-    log("info", f"{module_dict[module]}（{module}）运行结束")
+    log("info", f"{_modules_dict[module]}（{module}）运行结束")
 
 
 def test(data: dict, plugin_object):
     """
     #   只运行连接器部分
     参数说明：
     data:dict,      #   运行功能时的必要的json数据
     plugin_object:PLUGIN,      #   插件集合对象（类位于生成的插件后的根目录下main.py文件内）
     """
     #   必要的参数位于data内的body下
     data_body = data.get("body", {})
     connection_data = data_body.get("connection")
 
-    module_dict = {
-        "action": "动作",
-        "trigger": "触发器",
-        "alarm": "告警接收器",
-        "receiver": "情报接收器",
-        "asset": "资产接收器"
-    }
-
     plugin_object_dict = {
         "action": plugin_object.actions,
         "trigger": plugin_object.triggers,
         "alarm": plugin_object.alarm_receivers,
         "receiver": plugin_object.indicator_receivers,
-        "asx set": plugin_object.asset_receivers
+        "asset": plugin_object.asset_receivers
     }
 
     #   检查json数据是使用在哪个组件上的
     modules_list = ["action", "trigger", "alarm", "receiver", "asset"]
 
     #   检查json数据是使用在哪个组件上的
     for module in modules_list:
         if data_body.get(module):
             func_name = data_body[module]
             func = plugin_object_dict[module][func_name]
             func._test(connection_data)
-            log("info", f"{module_dict[module]}（{module}）连接器运行结束")
+            log("info", f"{_modules_dict[module]}（{module}）连接器运行结束")
             return
 
     log("info", "未检测到需要运行的组件")
 
 
 def http(workers=4):
     """
```

### Comparing `chariot-sdk-1.3.0/chariotCore/res/SDK/cli.py` & `chariot-sdk-1.3.1/chariotCore/res/SDK/cli.py`

 * *Files identical despite different names*

### Comparing `chariot-sdk-1.3.0/chariotCore/res/SDK/models.py` & `chariot-sdk-1.3.1/chariotCore/res/SDK/models.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,69 +1,56 @@
-from typing import List
+from typing import List, Literal, Optional
 from pydantic import BaseModel
 
 
-#   插件定义文件结构，用于自动生成插件
-class PLUGIN_CONSTRUCTION(BaseModel):
-    plugin_spec_version: str = "v2"
-    name: str
-    version: str
-    hot_update: bool = True
-    auto_generate: bool = True
-    title: dict
-    description: dict = None
-    vendor: str = "chariot"
-    tags: List[str] = None
-    connection: dict = None
-    actions: dict
-
-
 #   执行数据验证类，用于传入插件数据的验证
 class PLUGIN_TEST_MODEL(BaseModel):
     version: str
     type: str
     body: dict
 
 
-class DISPATCHER(BaseModel):
+#   转发地址和缓存地址
+class DISPATCHER_MODEL(BaseModel):
     url: str = "http://127.0.0.1:10001/transpond"
     cache_url: str = ""
 
 
+#   请求
 class BODY_MODEL(BaseModel):
     meta: dict = {}
     connection: dict = {}
-    dispatcher: DISPATCHER = None
+    dispatcher: DISPATCHER_MODEL = None
     input: dict = {}
     enable_web: bool = False
     config: dict = {}
 
 
 class ACTION_TEST_BODY_MODEL(BODY_MODEL):
     action: str
 
 
 class TRIGGER_TEST_BODY_MODEL(BODY_MODEL):
     trigger: str
-    dispatcher: DISPATCHER
+    dispatcher: DISPATCHER_MODEL
 
 
 class ALARM_RECEIVER_TEST_BODY_MODEL(BODY_MODEL):
     alarm: str
-    dispatcher: DISPATCHER
+    dispatcher: DISPATCHER_MODEL
 
 
 class INDICATOR_RECEIVER_TEST_BODY_MODEL(BODY_MODEL):
     receiver: str
-    dispatcher: DISPATCHER
+    dispatcher: DISPATCHER_MODEL
 
 
 class ASSET_RECEIVER_TEST_BODY_MODEL(BODY_MODEL):
     asset: str
-    dispatcher: DISPATCHER
+    dispatcher: DISPATCHER_MODEL
 
 
 class ACTION_TEST_MODEL(BaseModel):
     version: str = "v3"
     type: str = "action"
     body: ACTION_TEST_BODY_MODEL
 
@@ -86,7 +73,44 @@
     body: INDICATOR_RECEIVER_TEST_BODY_MODEL
 
 
 class ASSET_RECEIVER_TEST_MODEL(BaseModel):
     version: str = "v3"
     type: str = "asset_receiver"
     body: ASSET_RECEIVER_TEST_BODY_MODEL
+
+
+#   插件定义文件结构，用于初始化插件
+class PLUGIN_DATA_MODEL(BaseModel):
+    plugin_spec_version: str = "v3"
+    name: str
+    version: str
+    title: dict
+    sdk: str = "1.3.1"
+    description: dict = None
+    vendor: str = "chariot"
+    tags: List[str] = []
+    types: dict = None
+    connection: dict = None
+    actions: dict = None
+    triggers: dict = None
+    alarm_receivers: dict = None
+    indicator_receivers: dict = None
+    asset_receivers: dict = None
+
+
+class FUNC_SET_MODEL(BaseModel):
+    func_id: str
+    func_code: str
+
+
+class CODE_DICT_MODEL(BaseModel):
+    actions: List[FUNC_SET_MODEL] = []
+    triggers: List[FUNC_SET_MODEL] = []
+    alarm_receivers: List[FUNC_SET_MODEL] = []
+    indicator_receivers: List[FUNC_SET_MODEL] = []
+    asset_receivers: List[FUNC_SET_MODEL] = []
+
+
+class PLUGIN_CONSTRUCTION_MODEL(BaseModel):
+    plugin_data: PLUGIN_DATA_MODEL
+    plugin_code: CODE_DICT_MODEL
```

### Comparing `chariot-sdk-1.3.0/chariotCore/res/SDK/subassembly.py` & `chariot-sdk-1.3.1/chariotCore/res/SDK/subassembly.py`

 * *Files identical despite different names*

### Comparing `chariot-sdk-1.3.0/chariotCore/res/SDK/web.py` & `chariot-sdk-1.3.1/chariotCore/res/SDK/web.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,58 +1,52 @@
+import os
+import yaml
 from fastapi import FastAPI, File, Request
 from fastapi.responses import JSONResponse
 import uvicorn
 import typing
 import multiprocessing
 from . import VERSION
 from .models import *
 from .base import *
 from importlib import reload
+from signal import SIGINT
 
 ####
 #
-#   插件的Rest API服务
+#   插件的API服务
 #   全局变量前面请加下划线，这些变量应该只被web.py内方法调用
-#   **预计在将来某一个版本中被另外一种方法替代** (这行划去)
+#   --预计在将来某一个版本中被另外一种方法替代-- (这行划去)
 #   计划总赶不上变化不是吗
 #
 ####
 
 _rest_server = FastAPI(title="千乘插件API接口", version=VERSION, description="")
 
 
 @_rest_server.post("/actions/{action_name}", tags=["动作"])
 async def actions(action_name, plugin_stdin: typing.Optional[ACTION_TEST_MODEL]):
     """
     #   动作接口
     """
     clearLog(clear_size=1)
 
-    #   在生成插件之后有actions就能成功import了
-    try:
-        import actions
-        #   先初始化并释放一次动作类，以清空缓存
-        actions.modules_dict()[action_name]()
-        #   清空完再reload
-        reload(actions)
-    except:
-        pass
-
-    action = load_module(action_name, "action")
+    action = loadModule(action_name, "actions")
 
     if not action:
-        log("error", f"无法找到功能：{action_name}")
+        log("error", f"无法导入功能：{action_name}")
         content = {
-            "msg": f"无法找到功能：{action_name}"
+            "msg": f"无法导入功能：{action_name}",
+            "status": "False"
         }
-        return JSONResponse(content=content, status_code=404)
+        return JSONResponse(content=content, status_code=400)
 
     #   取出body
     data = plugin_stdin.dict()
-    checkModel(data, models.PLUGIN_TEST_MODEL)
+    checkModel(data, PLUGIN_TEST_MODEL)
     data_body = data.get("body")
 
     #   获取input
     input_data = data_body.get("input")
     connection_data = data_body.get("connection")
 
     #   执行 run 相关操作
@@ -65,271 +59,112 @@
 
 
 @_rest_server.post("/actions/{action_name}/test", tags=["动作"])
 async def actions_test(action_name: str, plugin_stdin: typing.Optional[ACTION_TEST_MODEL]):
     """
     #   动作连接器测试接口
     """
-    return rest_test("action", action_name, plugin_stdin)
-
-
-def load_module(func_name, module):
-    """
-    #   尝试重载各个组件
-    参数说明
-    func_name:str,      #   方法名
-    module:str,         #   组件
-
-    如果无法找到方法或组件则返回None
-    """
-
-    if module == "action":
-        #   在生成插件之后有actions就能成功import了
-        try:
-            import actions
-            #   先初始化并释放一次功能类，以清空缓存
-            actions.modules_dict()[func_name]()
-            #   清空完再reload
-            reload(actions)
-            return actions.modules_dict()[func_name]()
-        except:
-            pass
-
-    elif module == "trigger":
-        #   通过接口创建的接收器进程会重新加载文件，所以无需reload和清缓存
-        try:
-            import triggers
-            return triggers.modules_dict()[func_name]()
-        except:
-            pass
-
-    elif module == "alarm_receiver":
-        try:
-            import alarm_receivers
-            return alarm_receivers.modules_dict()[func_name]()
-        except:
-            pass
-
-    elif module == "indicator_receiver":
-        try:
-            import indicator_receivers
-            return indicator_receivers.modules_dict()[func_name]()
-        except:
-            pass
-
-    elif module == "asset_receiver":
-        try:
-            import asset_receivers
-            return asset_receivers.modules_dict()[func_name]()
-        except:
-            pass
-
-    return None
-
-
-def rest_test(module, func_name, plugin_stdin):
-    """
-    #   通用接收器的连接器测试方法
-    参数说明：
-    module:str,         #   组件，module = action,trigger,alarm_receiver,indicator_receiver,asset_receiver
-    func_name:str,  #   方法名称
-    plugin_stdin:str,   #   接口传入数据
-
-    因为测试连接器流程一样
-    所有使用一个通用方法进行维护
-    """
-
-    clearLog(clear_size=1)
-
-    func = load_module(func_name, module)
-
-    if not func:
-        log("error", f"未找到功能：{func_name}")
-        content = {
-            "msg": "未找到功能：{func_name}"
-        }
-        return JSONResponse(content=content, status_code=404)
-
-    #   取出body
-    data = plugin_stdin.dict()
-    data_body = data.get("body")
-
-    connection_data = data_body.get("connection")
-
-    if data_body.get("config"):
-        log("info", "获取请求中配置信息")
-        loadConfig(data_body["config"])
-    else:
-        log("info", "请求中无配置信息，使用默认配置")
-        loadConfig()
-
-    output = func._test(connection_data)
-
-    if output["body"]["status"] != "True":
-        return JSONResponse(content=output, status_code=500)
-    else:
-        return output
-
-
-def receivers(module, receiver_name, plugin_stdin):
-    """
-    #   通用接收器方法
-    参数说明：
-    module:str,         #   组件，module = trigger,alarm_receiver,indicator_receiver,asset_receiver
-    receiver_name:str,  #   接收器名称
-    plugin_stdin:str,   #   接口传入数据
-
-    因为触发器、告警接收器、情报接收器、资产接收器代码重复率极高（或者可以说一模一样的），
-    因此使用一个通用方法进行维护
-    """
-
-    clearLog(clear_size=1)
-
-    receiver = load_module(receiver_name, module)
-
-    module_dict = {
-        "trigger": "触发器",
-        "indicator_receiver": "情报接收器",
-        "alarm_receiver": "告警接收器",
-        "asset_receiver": "资产接收器"
-    }
-
-    data = plugin_stdin.dict()
-
-    try:
-        #   判断是否存在接收器类型
-        if data.get("type") not in module_dict.keys():
-            log("error", f"不支持的接收器类模块类型（type）：{data.get('type')}")
-            content = {
-                "msg": f"不支持的接收器类模块类型（type）：{data.get('type')}",
-                "tips": f"目前仅支持{list(module_dict.keys())}"
-            }
-            return JSONResponse(content=content, status_code=400)
-
-        #   判断是否存在该接收器
-        if not receiver:
-            log("error", f"不存在的功能：{receiver_name}")
-            content = {
-                "msg": f"不存在的功能：{receiver_name}"
-            }
-            return JSONResponse(content=content, status_code=400)
-
-        #   data中的body部分
-        data_body = data.get("body")
-        #   run输入参数
-        input_data = data_body.get("input")
-        #   连接器参数
-        connection_data = data_body.get("connection")
-        #   转发地址
-        dispatcher_url = data_body.get("dispatcher").get("url")
-        #   缓存地址
-        cache_url = data_body.get("dispatcher").get("cache_url")
-        #   进程创建
-        process = multiprocessing.Process(target=receiver._run,
-                                          args=(input_data, connection_data, dispatcher_url, cache_url,
-                                                data_body.get("config")))
-        #   启动进程
-        process.start()
-
-        from .base import _log_data
-
-        content = {
-            "version": "v1",
-            "type": data["type"],
-            "body": {
-                "status": "True",
-                "log": _log_data,
-                "error_trace": "",
-                "msg": f"{module_dict[data['type']]}已创建完成"
-            }
-        }
-
-        return JSONResponse(content=content, status_code=201)
-
-    except Exception as error:
-
-        from .base import _log_data
-
-        log("error", f"{error}")
-
-        content = {
-            "version": "v1",
-            "type": data["type"],
-            "body": {
-                "status": "False",
-                "log": _log_data,
-                "error_trace": traceback.format_exc(),
-                "msg": f"{module_dict[data['type']]}创建失败"
-            }
-        }
-
-        return JSONResponse(content=content, status_code=500)
+    return rest_test("actions", action_name, plugin_stdin)
 
 
 @_rest_server.post("/triggers/{trigger_name}", tags=["触发器"])
 async def triggers(trigger_name: str, plugin_stdin: typing.Optional[TRIGGER_TEST_MODEL]):
     """
     #   触发器接口
     """
-    return receivers("trigger", trigger_name, plugin_stdin)
+    return createReceivers("triggers", trigger_name, plugin_stdin)
 
 
 @_rest_server.post("/triggers/{trigger_name}/test", tags=["触发器"])
 async def trigger_test(trigger_name: str, plugin_stdin: typing.Optional[TRIGGER_TEST_MODEL]):
     """
     #   触发器连接器测试接口
     """
-    return rest_test("trigger", trigger_name, plugin_stdin)
+    return rest_test("triggers", trigger_name, plugin_stdin)
 
 
 @_rest_server.post("/alarm_receivers/{alarm_receiver_name}", tags=["告警接收器"])
 async def alarm_receivers(alarm_receiver_name: str, plugin_stdin: typing.Optional[ALARM_RECEIVER_TEST_MODEL]):
     """
     #   告警接收器接口
     """
-    return receivers("alarm_receiver", alarm_receiver_name, plugin_stdin)
+    return createReceivers("alarm_receivers", alarm_receiver_name, plugin_stdin)
 
 
 @_rest_server.post("/alarm_receivers/{alarm_receiver_name}/test", tags=["告警接收器"])
 async def alarm_receivers_test(alarm_receiver_name: str,
                                plugin_stdin: typing.Optional[ALARM_RECEIVER_TEST_MODEL]):
     """
     #   告警接收器连接器测试接口
     """
-    return rest_test("alarm_receiver", alarm_receiver_name, plugin_stdin)
+    return rest_test("alarm_receivers", alarm_receiver_name, plugin_stdin)
 
 
 @_rest_server.post("/indicator_receivers/{indicator_receiver_name}", tags=["情报接收器"])
 async def indicator_receivers(indicator_receiver_name: str,
                               plugin_stdin: typing.Optional[INDICATOR_RECEIVER_TEST_MODEL]):
     """
     #   情报接收器接口
     """
-    return receivers("indicator_receiver", indicator_receiver_name, plugin_stdin)
+    return createReceivers("indicator_receivers", indicator_receiver_name, plugin_stdin)
 
 
 @_rest_server.post("/indicator_receivers/{indicator_receiver_name}/test", tags=["情报接收器"])
 async def indicator_receivers_test(indicator_receiver_name: str,
                                    plugin_stdin: typing.Optional[INDICATOR_RECEIVER_TEST_MODEL]):
     """
     #   情报接收器连接器测试接口
     """
-    return rest_test("indicator_receiver", indicator_receiver_name, plugin_stdin)
+    return rest_test("indicator_receivers", indicator_receiver_name, plugin_stdin)
 
 
 @_rest_server.post("/asset_receivers/{asset_receiver_name}", tags=["资产接收器"])
 async def asset_receivers(asset_receiver_name: str,
                           plugin_stdin: typing.Optional[ASSET_RECEIVER_TEST_MODEL]):
-    return receivers("asset_receiver", asset_receiver_name, plugin_stdin)
+    """
+    #   资产接收器接口
+    """
+    return createReceivers("asset_receivers", asset_receiver_name, plugin_stdin)
 
 
 @_rest_server.post("/asset_receivers/{asset_receiver_name}/test", tags=["资产接收器"])
 async def asset_receivers_test(asset_receiver_name: str,
                                plugin_stdin: typing.Optional[ASSET_RECEIVER_TEST_MODEL]):
-    return rest_test("asset_receiver", asset_receiver_name, plugin_stdin)
+    """
+    #   资产接收器连接器测试接口
+    """
+    return rest_test("asset_receivers", asset_receiver_name, plugin_stdin)
+
+
+@_rest_server.post("/shutdown_receivers", tags=["插件编辑"])
+async def shutdown_receivers():
+    """
+    #   关闭接收器
+    """
+    try:
+        pid_data = getLocalCache("receiver_pid")
+        os.kill(pid_data["pid"], SIGINT)
+        log("info", "退出完成")
+
+        setLocalCache({"pid": None}, "receiver_pid")
+
+        content = {
+            "msg": "退出完成"
+        }
+        return JSONResponse(content=content, status_code=200)
+
+    except Exception as error:
+        log("warning", "退出失败，可能没有接收器正在运行？")
+
+        setLocalCache({"pid": None}, "receiver_pid")
+
+        content = {
+            "msg": "退出失败，可能没有接收器正在运行？"
+        }
+        return JSONResponse(content=content, status_code=404)
 
 
 @_rest_server.post("/update_plugin", tags=["插件热更新"])
 async def update_plugin(update_pack: bytes = File()):
     """
     #   上传更新包
     """
@@ -349,33 +184,143 @@
         clearUpdateFile()
         content = {
             "msg": f"更新失败 - {error}"
         }
         return JSONResponse(content=content, status_code=500)
 
 
-@_rest_server.post("/generate_plugin", tags=["插件生成器"])
-async def generate_plugin(plugin_construction: models.PLUGIN_CONSTRUCTION):
+@_rest_server.post("/editor/plugin", tags=["插件编辑"])
+async def post_plugin(plugin_construction: PLUGIN_CONSTRUCTION_MODEL):
     """
-    #   自动生成插件接口
-    #   此接口暂时不可用
-    TODO 修复自动生成插件功能在多进程下的运行
+    #   初始化插件
     """
+
+    clearLog(clear_size=1)
+
+    work_path = os.getcwd()
+
+    plugin_construction = plugin_construction.dict()
+
+    plugin_data = plugin_construction["plugin_data"]
+
+    yaml_path = os.path.join(work_path, "plugin.spec.yaml")
+
+    with open(yaml_path, "w", encoding="utf-8") as file:
+        yaml.dump(plugin_data, file, encoding="utf-8",
+                  allow_unicode=True, sort_keys=False)
+
+    result = os.system("chariot-plugin -ag plugin.spec.yaml")
+
+    if result:
+        content = {
+            "msg": "插件初始化失败，请查看日志以排除错误"
+        }
+        return JSONResponse(content=content, status_code=400)
+
+    codes = plugin_construction["plugin_code"]
+
+    error_dict = {}
+
+    dir_and_code = []
+
+    #   先遍历检查一遍，防止重复或错误操作
+    #   遍历要更新的组件列表的方法和代码
+    for module, func_list in codes.items():
+        #   遍历要更新的方法
+        for func in func_list:
+            module_file_path = os.path.join(work_path, module, (func["func_id"] + ".py"))
+            #   当方法不存在时记录在案
+            if not os.path.exists(module_file_path):
+                try:
+                    error_dict[module].append(func["func_id"])
+                except:
+                    error_dict[module] = []
+                    error_dict[module].append(func["func_id"])
+            else:
+                dir_and_code.append((module_file_path, func["func_code"]))
+
+    #   当有方法不存在时就放弃所有更新
+    if error_dict:
+        content = {
+            "msg": "部分功能未记录在定义文件，已结束插件初始化",
+            "not_found": error_dict
+        }
+        return JSONResponse(content=content, status_code=400)
+
+    try:
+        for func_path, func_code in dir_and_code:
+            with open(func_path, "w", encoding="utf-8") as file:
+                file.write(func_code)
+        return {
+            "msg": "插件生成完成"
+        }
+    except Exception as error:
+        content = {
+            "msg": f"代码写入失败 - {error}"
+        }
+        return JSONResponse(content=content, status_code=500)
+
+
+@_rest_server.get("/editor/plugin", tags=["插件编辑"])
+async def get_plugin():
+    clearLog(clear_size=1)
+
+    work_path = os.getcwd()
+
+    modules_dir = ["actions", "triggers", "alarm_receivers", "indicator_receivers", "asset_receivers"]
+
+    modules_dict = {}
+
+    try:
+
+        for temp_module in modules_dir:
+
+            modules_dict[temp_module] = []
+
+            modules_dir_path = os.path.join(work_path, temp_module)
+
+            if not os.path.exists(modules_dir_path):
+                continue
+
+            module_files = os.listdir(modules_dir_path)
+
+            ignore_files = ["models.py", "__init__.py", "__pycache__"]
+
+            for ignore_file in ignore_files:
+                if ignore_file in module_files:
+                    module_files.pop(module_files.index(ignore_file))
+
+            for module_file in module_files:
+                module_file_path = os.path.join(modules_dir_path, module_file)
+
+                with open(module_file_path, "r", encoding="utf-8") as module_file_code:
+                    modules_dict[temp_module].append({
+                        "func_id": module_file.replace(".py", ""),
+                        "func_code": module_file_code.read()
+                    })
+    except Exception as error:
+        content = {
+            "msg": f"功能代码读取失败 - {error}"
+        }
+        return JSONResponse(content=content, status_code=500)
+
+    plugin_data = getPluginData()
+
+    if not plugin_data:
+        log("error", "插件定义数据不存在")
+        content = {
+            "msg": "插件定义数据不存在"
+        }
+        return JSONResponse(content=content, status_code=404)
+
     return {
-        "msg": "接口暂时停用"
+        "plugin_data": plugin_data,
+        "plugin_code": modules_dict
     }
 
-    # clearLog(clear_size=1)
-    #
-    # data = plugin_construction.dict()
-    #
-    # #   将特殊定义文件放到缓存下，等待SDK调用
-    # setLocalCache(data, "plugin_construction")
-    #
-    # os.system("chariot-plugin -ag {}".format(os.path.join("__sdkcache__", "plugin_construction.chariot-128.sdkc")))
 
 @_rest_server.get("/sdk_version", tags=["插件信息"])
 async def sdk_version():
     """
     #   获取SDK版本
     """
     return {
@@ -385,58 +330,264 @@
 
 @_rest_server.get("/plugin_data", tags=["插件信息"])
 async def get_plugin_data():
     """
     #   获取插件定义数据接口
     """
 
-    json_data_path = os.path.join(os.getcwd(), "plugin.spec.json")
-
-    yaml_data_path = os.path.join(os.getcwd(), "plugin.spec.yaml")
-
-    if os.path.exists(json_data_path):
-        plugin_data = json.load(open(json_data_path, "r"))
-        return plugin_data
+    plugin_data = getPluginData()
 
-    elif os.path.exists(yaml_data_path):
-        with open(yaml_data_path, "r", encoding="utf-8") as file:
-            plugin_data = yaml.load(file.read(), Loader=yaml.FullLoader)
+    if plugin_data:
         return plugin_data
 
     else:
         log("error", "插件定义数据不存在")
         content = {
             "error": "插件定义数据不存在"
         }
         return JSONResponse(content=content, status_code=404)
 
 
 @_rest_server.post("/transpond", tags=["转发数据接收"])
-async def receive_transponded(request: Request):
+async def receive_transpond(request: Request):
     """
     #   测试用接口，用于接收转发的数据
     """
     try:
         data = await request.body()
-        log("info", f"获得转发数据：\n {data.decode()}")
+        log("attention", f"获得转发数据：\n {json.loads(data.decode())}")
         resp_data = {
             "msg": "接收成功",
             "error": ""
         }
         return JSONResponse(content=resp_data)
     except Exception as error:
         resp_data = {
             "msg": "接收失败",
             "error": str(error)
         }
         return JSONResponse(content=resp_data, status_code=500)
 
 
-def runserver(workers=4):
+def loadModule(func_id, module):
+    """
+    #   尝试重载各个组件
+    参数说明
+    func_id:str,      #   方法名
+    module:str,         #   组件
+
+    如果无法找到方法或组件则返回None
+    """
+
+    if module == "actions":
+        #   在生成插件之后有actions就能成功import了
+        try:
+            import actions
+            #   先初始化并释放一次功能类，以清空缓存
+            actions.modules_dict()[func_id]()
+            #   清空完再reload
+            reload(actions)
+            return actions.modules_dict()[func_id]()
+        except:
+            log("error", traceback.format_exc())
+
+    elif module == "triggers":
+        #   通过接口创建的接收器进程会重新加载文件，所以无需reload和清缓存
+        try:
+            import triggers
+            return triggers.modules_dict()[func_id]()
+        except:
+            log("error", traceback.format_exc())
+
+    elif module == "alarm_receivers":
+        try:
+            import alarm_receivers
+            return alarm_receivers.modules_dict()[func_id]()
+        except:
+            log("error", traceback.format_exc())
+
+    elif module == "indicator_receivers":
+        try:
+            import indicator_receivers
+            return indicator_receivers.modules_dict()[func_id]()
+        except:
+            log("error", traceback.format_exc())
+
+    elif module == "asset_receivers":
+        try:
+            import asset_receivers
+            return asset_receivers.modules_dict()[func_id]()
+        except:
+            log("error", traceback.format_exc())
+
+    return None
+
+
+def rest_test(module, func_id, plugin_stdin):
+    """
+    #   通用的连接器测试方法
+    参数说明：
+    module:str,         #   组件，module = action,trigger,alarm_receiver,indicator_receiver,asset_receiver
+    func_id:str,  #   方法id
+    plugin_stdin:str,   #   接口传入数据
+
+    因为测试连接器流程一样
+    所有使用一个通用方法进行维护
+    """
+
+    clearLog(clear_size=1)
+
+    func = loadModule(func_id, module)
+
+    if not func:
+        log("error", f"无法导入功能：{func_id}")
+        content = {
+            "msg": "无法导入功能：{func_id}"
+        }
+        return JSONResponse(content=content, status_code=400)
+
+    #   取出body
+    data = plugin_stdin.dict()
+    data_body = data.get("body")
+
+    connection_data = data_body.get("connection")
+
+    if data_body.get("config"):
+        log("info", "获取请求中配置信息")
+        loadConfig(data_body["config"])
+    else:
+        log("info", "请求中无配置信息，使用默认配置")
+        loadConfig()
+
+    output = func._test(connection_data)
+
+    if output["body"]["status"] != "True":
+        return JSONResponse(content=output, status_code=500)
+    else:
+        return output
+
+
+def createReceivers(module, receiver_name, plugin_stdin):
+    """
+    #   通用接收器方法
+    参数说明：
+    module:str,         #   组件，module = trigger,alarm_receiver,indicator_receiver,asset_receiver
+    receiver_name:str,  #   接收器名称
+    plugin_stdin:str,   #   接口传入数据
+
+    因为触发器、告警接收器、情报接收器、资产接收器代码重复率极高（或者可以说一模一样的），
+    因此使用一个通用方法进行维护
+    """
+
+    clearLog(clear_size=1)
+
+    module_dict = {
+        "triggers": "触发器",
+        "indicator_receivers": "情报接收器",
+        "alarm_receivers": "告警接收器",
+        "asset_receivers": "资产接收器"
+    }
+
+    data = plugin_stdin.dict()
+
+    try:
+
+        plugin_data = getPluginData()
+
+        if not plugin_data.get(module, {}).get(receiver_name):
+            log("error", f"无法在{module_dict[module]}下找到该功能：{receiver_name}")
+            content = {
+                "msg": f"无法在{module_dict[module]}下找到该功能：{receiver_name}"
+            }
+            return JSONResponse(content=content, status_code=404)
+
+        process = multiprocessing.Process(target=receiverProcess, args=(module, receiver_name, data))
+
+        process.start()
+
+        #   先鲨了之前创建的接收器，千乘只允许一个容器跑一个接收器
+        log("attention", "尝试退出之前创建的接收器")
+        try:
+            pid_data = getLocalCache("receiver_pid")
+            os.kill(pid_data["pid"], SIGINT)
+            log("info", "退出完成")
+            log("info", "缓存本次接收器信息")
+            setLocalCache({"pid": process.pid}, "receiver_pid")
+        except:
+            log("warning", "退出失败，第一次创建接收器请忽略此警告")
+            log("info", "缓存本次接收器信息")
+            setLocalCache({"pid": process.pid}, "receiver_pid")
+
+    except Exception as error:
+
+        from .base import _log_data
+
+        log("error", f"{error}")
+
+        content = {
+            "version": "v1",
+            "type": data["type"],
+            "body": {
+                "status": "False",
+                "log": _log_data,
+                "error_trace": traceback.format_exc(),
+                "msg": f"{module_dict[module]}创建失败"
+            }
+        }
+
+        return JSONResponse(content=content, status_code=500)
+
+    from .base import _log_data
+
+    content = {
+        "version": "v1",
+        "type": data["type"],
+        "body": {
+            "status": "True",
+            "log": _log_data,
+            "error_trace": "",
+            "msg": f"{module_dict[module]}已创建完成"
+        }
+    }
+
+    return JSONResponse(content=content, status_code=201)
+
+
+def receiverProcess(module, receiver_name, data):
+    """
+    #   此方法用于创建各类接收器进程
+    参数说明：
+    module:str,         #   组件，module = trigger,alarm_receiver,indicator_receiver,asset_receiver
+    receiver_name:str,  #   接收器名称
+    data:dict,  #   接收的数据
+    """
+
+    receiver = loadModule(receiver_name, module)
+    if not receiver:
+        log("error", f"无法导入功能：{receiver_name}")
+        content = {
+            "msg": f"无法导入功能：{receiver_name}"
+        }
+        return JSONResponse(content=content, status_code=400)
+
+    #   data中的body部分
+    data_body = data.get("body")
+    #   run输入参数
+    input_data = data_body.get("input")
+    #   连接器参数
+    connection_data = data_body.get("connection")
+    #   转发地址
+    dispatcher_url = data_body.get("dispatcher").get("url")
+    #   缓存地址
+    cache_url = data_body.get("dispatcher").get("cache_url")
+
+    receiver._run(input_data, connection_data, dispatcher_url, cache_url, data_body.get("config"))
+
+
+def runserver(workers):
     """
     #   启动api服务
     参数说明：
     workers:int,    #   工作进程数量
     """
-    os.system("")
     log("attention", "在浏览器内输入 http://127.0.0.1:10001/docs 以进行接口测试")
     uvicorn.run("SDK.web:_rest_server", host="0.0.0.0", port=10001, workers=workers)
```

### Comparing `chariot-sdk-1.3.0/chariotCore/res/config.ini` & `chariot-sdk-1.3.1/chariotCore/res/config.ini`

 * *Files 10% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 #	转发线程数量控制
 #	不建议调整，以免发生DDOS
 threads_limit = 5
 
 [ignore]
 #   打包时忽略的根目录下的文件
 #   以逗号分隔多个文件（文件夹）
-ignore = env,venv,tests,.git,.vs,.gitignore,.idea,__sdkcache__,__pycache__,temp_image.tar.gz,temp_plugin.tar.gz
+ignore = env,venv,tests,.git,.vs,.gitignore,.idea,__sdkcache__,__pycache__,builds
```

### Comparing `chariot-sdk-1.3.0/chariotCore/res/icon.png` & `chariot-sdk-1.3.1/chariotCore/res/icon.png`

 * *Files identical despite different names*

### Comparing `chariot-sdk-1.3.0/chariotCore/tasks.py` & `chariot-sdk-1.3.1/chariotCore/tasks.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import json
+import os
+
 from chariotCore import VERSION
 from chariotCore.tools import *
 from chariotCore.templates import *
 import traceback
 import tarfile
 import docker
 
@@ -27,29 +30,14 @@
     ]
 
     try:
 
         #   读取插件定义文件
         data = readGenerateFile(work_path, file_path)
 
-        #   在没有任何功能的数据和非自动生成插件的情况下
-        if not any([data.get(module) for module in modules]):
-            log("info", "未检测到任何功能的数据，需要生成自适应Request插件吗？[Y/N]")
-            if input() != "Y":
-                log("info", "已结束生成")
-                return
-            #   生成基础文件
-            generateBaseFile(work_path)
-            #   生成入口文件 main.py 用于给千乘执行
-            plugin_name = "auto_generator"
-            generateMainFile(work_path, plugin_name, {})
-            #   生成存储热更新包的文件夹，自动生成插件包后将放置在这里
-            generateUpdateFile(work_path)
-            return
-
         #   生成基础文件
         generateBaseFile(work_path)
 
         #   生成tests文件夹
         tests_path = os.path.join(work_path, "tests")
         if not os.path.exists(tests_path):
             os.mkdir(tests_path)
@@ -62,16 +50,19 @@
         if types:
             #   生成自定义类的校验数据
             types_model = generateTypesModel(types)
         else:
             types_model = ""
             log("attention", "未检测到自定义类型，跳过自定义类型校验数据的生成")
 
-        #   生成connection，connection不存在也要生成一份校验数据，因为所有功能执行前默认跑一次连接器
-        connection_params = data.get("connection", {})
+        #   生成connection
+        connection_params = data.get("connection")
+        #   connection不存在也要生成一份校验数据，因为所有功能执行前默认跑一次连接器
+        if not connection_params:
+            connection_params = {}
         #   生成连接器的校验数据
         connection_model = generateConnectionModel(connection_params)
         #   获取参数列表，用于生成功能文件
         connection_keys = list(connection_params.keys())
 
         modules_list_dict = {
             "actions": [],
@@ -86,17 +77,14 @@
             func_class_name_list = generateModule(data, module, types_model, connection_model, connection_keys)
             modules_list_dict[module] = func_class_name_list
 
         #   生成入口文件 main.py
         plugin_name = data.get("name")
         generateMainFile(work_path, plugin_name, modules_list_dict)
 
-        #   生成本地REST测试服务器文件
-        # generateTestServerFile(work_path,actions_list,triggers_list,indicator_receivers_list,alarm_receivers_list)
-
         #   生成帮助文件
         generateHelpFile(data)
 
         #   生成通用文件存储的文件夹
         generateUtilFile(work_path)
 
         #   生成存储热更新包的文件夹
@@ -105,79 +93,108 @@
     except Exception as error:
         log("error", f"{error}\n{traceback.format_exc()}")
         return
 
     log("info", "所有插件文件生成完成")
 
 
-def autoGenerate(work_path, file_path):
+def autoGenerate(work_path, file_path: str):
     """
     #   生成插件
     参数说明：
     work_path:str,    #   当前工作区绝对路径
     file_path:str,    #   特殊定义文件相对路径
 
     #   生成失败时显示错误log，并返回
     """
-    log("info", f"正在使用千乘插件开发工具 v{VERSION} 自动生成插件中")
+
+    modules = [
+        "actions",
+        "triggers",
+        "alarm_receivers",
+        "indicator_receivers",
+        "asset_receivers"
+    ]
 
     try:
 
         log("info", "读取插件数据中")
 
         try:
-            file_readbytes = open(os.path.join(work_path, file_path), "rb").read()
-            data = json.loads(file_readbytes.decode())
+            file_read = open(os.path.join(work_path, file_path), "r", encoding="utf-8").read()
+            if file_path.endswith(".sdkc") or file_path.endswith(".json"):
+                data = json.loads(file_read)
+            elif file_path.endswith(".yaml"):
+                data = yaml.load(file_read, Loader=yaml.FullLoader)
+            else:
+                data = json.loads(file_read)
         except Exception as error:
             raise Exception(f"读取插件数据失败\n  失败原因：{error}")
 
         log("info", "读取完成")
 
         #   生成tests文件夹
         tests_path = os.path.join(work_path, "tests")
         if not os.path.exists(tests_path):
             os.mkdir(tests_path)
 
-        #   转换插件特殊定义文件
-        trans_data = autoGenerateDataTrans(data)
-        #   生成一般插件定义文件
-        autoGeneratePluginSpecFile(trans_data)
-        #   生成校验数据
-        actions_model = generateModelData("actions", trans_data.get("actions"))
-        #   生成连接器校验数据
-        connection_model = generateConnectionModel(trans_data.get("connection", {}))
-        #   组合校验文件数据
-        actions_model = model_header + connection_model + actions_model
-        #   生成校验文件
-        generateModelFile(work_path, "actions", actions_model)
-        #   生成动作文件
-        actions_list = autoGenerateActionsFile(work_path, trans_data)
-        #   生成入口文件 main.py
-        plugin_name = data.get("name")
+        #   生成自定义类
+        types = data.get("types")
+        if types:
+            #   生成自定义类的校验数据
+            types_model = generateTypesModel(types)
+        else:
+            types_model = ""
+            log("attention", "未检测到自定义类型，跳过自定义类型校验数据的生成")
+
+        #   生成connection
+        connection_params = data.get("connection")
+        #   connection不存在也要生成一份校验数据，因为所有功能执行前默认跑一次连接器
+        if not connection_params:
+            connection_params = {}
+        #   生成连接器的校验数据
+        connection_model = generateConnectionModel(connection_params)
+        #   获取参数列表，用于生成功能文件
+        connection_keys = list(connection_params.keys())
+
         modules_list_dict = {
-            "actions": actions_list
+            "actions": [],
+            "triggers": [],
+            "alarm_receivers": [],
+            "indicator_receivers": [],
+            "asset_receivers": []
         }
-        generateMainFile(work_path, plugin_name, modules_list_dict)
 
-        #   生成本地REST测试服务器文件
-        # generateTestServerFile(work_path,actions_list,[],[],[])
+        #   删除老旧文件
+        deleteOldFile(modules_list_dict)
+
+        #   生成组件以及组件属下的功能
+        for module in modules:
+            func_class_name_list = generateModule(data, module, types_model, connection_model, connection_keys)
+            modules_list_dict[module] = func_class_name_list
+
+        #   生成入口文件 main.py
+        plugin_name = data.get("name")
+        generateMainFile(work_path, plugin_name, modules_list_dict)
 
         #   生成帮助文件
         generateHelpFile(data)
 
         #   生成通用文件存储的文件夹
         generateUtilFile(work_path)
 
         #   生成存储热更新包的文件夹
         generateUpdateFile(work_path)
 
     except Exception as error:
-        log("error", error)
-        print(traceback.format_exc())
-        return
+        log("error", f"{error}\n{traceback.format_exc()}")
+        return 1
+
+    log("info", "所有插件文件生成完成")
+    return 0
 
 
 def generateYaml(work_path: str):
     """
     #   在当前工作目录下生成一个yaml模板文件
     参数说明：
     work_path:str,    #   当前工作区绝对路径
@@ -262,34 +279,39 @@
     log("info", "创建在线包中")
 
     tarballOnlinePack()
 
     log("info", "创建完成")
 
 
-def mkimg(work_path: str):
+def mkimg(os_arch: str):
     """
     参数说明：
-    work_path:str,    #   当前工作区绝对路径
+    os_arch:str,    #   平台，不填默认根据目前开发环境进行选择，例如：linux/386，linux/arm64，linux/arm/v7
     """
     log("info", "创建离线包中")
 
+    work_path = os.getcwd()
+
+    #   builds文件夹用于放置构建好的包
+    builds_dir_path = os.path.join(work_path, "builds")
+
     #   需要打包的文件
     #   以元组形式放入 (相对目录, 打包后在压缩包内的文件名)
     #   打包后在压缩包内的文件名为千乘后端规定的
     files_to_tar = [
         ("plugin.spec.yaml", "plugin.spec.yaml"),
         ("icon.png", "icon.png"),
         ("help.md", "help.md"),
     ]
 
     #   临时镜像文件名
     temp_image = "temp_image.tar.gz"
     files_to_tar.append(
-        (temp_image, "plugin.tar.gz")
+        (os.path.join("builds", temp_image), "plugin.tar.gz")
     )
 
     #   临时在线包文件名
     temp_tar = "temp_plugin.tar.gz"
 
     #   创建临时在线包
     #   这里调用此方法是为了利用打包在线包时的忽略不必要文件功能
@@ -297,77 +319,89 @@
     data = tarballOnlinePack(temp_tar)
 
     #   获取插件定义文件中的元数据
     vendor = data["vendor"]
     name = data["name"]
     version = data["version"]
 
-    #   离线包文件名
-    offline_name = f"{vendor}-{name}-{version}-offline.tar.gz"
-
-    #   清除原来可能存在的同版本离线包文件以及打包失败的残留临时文件
-    clear_files = [temp_image, offline_name]
-
-    for file in clear_files:
-        if os.path.exists(file) and not os.path.isdir(os.path.join(work_path, file)):
-            os.remove(file)
-
     #   创建Docker环境
     docker_client = docker.from_env()
 
     #   镜像标签
     tag = f"{vendor}/{name}:{version}"
 
-    temp_plugin_tar = open(os.path.join(work_path, "temp_plugin.tar.gz"), "rb")
+    temp_plugin_tar = open(os.path.join(builds_dir_path, "temp_plugin.tar.gz"), "rb")
 
     log("info", "创建镜像中")
-    docker_client.images.build(fileobj=temp_plugin_tar, pull=True, tag=tag, custom_context=True)
+    docker_client.images.build(fileobj=temp_plugin_tar, pull=True, tag=tag, custom_context=True, platform=os_arch)
     log("info", "创建完成")
 
     temp_plugin_tar.close()
 
     log("info", "缓存镜像至本地")
-    #   根据tag获取镜像
-    image = docker_client.images.get(tag)
-    #   暂存镜像文件
-    with open(os.path.join(work_path, temp_image), "wb") as file:
-        for chunk in image.save(named=True):
-            file.write(chunk)
+    try:
+        temp_image_path = os.path.join(builds_dir_path,temp_image)
+        #   清除可能的残留文件
+        if os.path.exists(temp_image_path):
+            os.remove(temp_image_path)
+        #   根据tag获取镜像
+        image = docker_client.images.get(tag)
+        image_data = image.attrs
+        #   暂存镜像文件
+        with open(temp_image_path, "wb") as file:
+            for chunk in image.save(named=True):
+                file.write(chunk)
+    except Exception as error:
+        raise Exception(f"缓存失败\n{error}")
     log("info", "缓存完成")
 
+    log("info", "创建临时插件结构文件")
+    plugin = {
+        "plugin_data": data,
+        "plugin_code": getAllModulesCode()
+    }
+    with open(os.path.join(work_path, "plugin.construction.json"), "w", encoding="utf-8") as file:
+        json.dump(plugin, file, ensure_ascii=False)
+        files_to_tar.append(("plugin.construction.json", "plugin.construction.json"))
+    log("info", "创建完成")
+
+    #   离线包文件名
+    offline_name = f"{vendor}-" \
+                   f"{name}-" \
+                   f"{version}-" \
+                   f"{(image_data['Os'] + '-') if image_data.get('Os') else ''}" \
+                   f"{(image_data['Architecture'] + '-') if image_data.get('Architecture') else ''}" \
+                   f"{(image_data['Variant'] + '-') if image_data.get('Variant') else ''}" \
+                   f"offline.tar.gz"
+
     log("info", "打包必要文件")
+
     try:
-        with tarfile.open(os.path.join(work_path, offline_name), "w:gz", format=tarfile.GNU_FORMAT) as tar:
+        offline_tar_path = os.path.join(builds_dir_path,offline_name)
+        #   清除可能的残留文件
+        if os.path.exists(offline_tar_path):
+            os.remove(offline_tar_path)
+        with tarfile.open(offline_tar_path, "w:gz", format=tarfile.GNU_FORMAT) as tar:
             for file in files_to_tar:
                 file_path = os.path.join(work_path, file[0])
                 if os.path.exists(file_path):
                     tar.add(file_path, arcname=file[1])
                 else:
                     raise Exception(f"{file}缺失")
     except Exception as error:
-        log("error", f"打包失败\n{error}")
+        raise Exception(f"打包失败\n{error}")
 
-    else:
-        log("info", "打包完成")
-        log("info", "创建离线包完成")
-
-    finally:
-        log("info", "清理临时文件中")
-        clear_files = [temp_image, temp_tar]
-        for file in clear_files:
-            if os.path.exists(file) and not os.path.isdir(os.path.join(work_path, file)):
-                os.remove(file)
-        log("info", "清理完成")
-        return
+    log("info", "打包完成")
+    log("info", "创建离线包完成")
 
-
-def testserver(work_path: str):
-    """
-    **此方法暂时弃用**
-
-    参数说明：
-    work_path:str,    #   当前工作区绝对路径
-    """
-    testserver_path = os.path.join(work_path, "testserver.py")
-
-    cmd = f"python {testserver_path}"
-    os.system(cmd)
+    log("info", "清理临时文件中")
+    clear_files = [
+        os.path.join("builds", temp_image),
+        os.path.join("builds", temp_tar),
+        "plugin.construction.json"
+    ]
+    for file in clear_files:
+        file_path = os.path.join(work_path, file)
+        if os.path.exists(file_path) and not os.path.isdir(file_path):
+            os.remove(file)
+    log("info", "清理完成")
+    return
```

### Comparing `chariot-sdk-1.3.0/chariotCore/templates.py` & `chariot-sdk-1.3.1/chariotCore/templates.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,21 +7,15 @@
 from pydantic import BaseModel
 from typing import *
 
 # 可自行修改增加校验精准度
 
 """
 
-model_template = """
-class {{ className }}(BaseModel):
-    {% if args %}{% for argName, argType in args %}
-    {{ argName }}: {{ argType }}
-    {% endfor %}{% else %}
-    ...
-    {% endif %}"""
+
 
 action_template = """
 from SDK.subassembly import Actions
 from SDK.base import *
 
 from .models import {{ connModel }}, {{ inputModel }}, {{ outputModel }}
 
@@ -43,16 +37,14 @@
         {% if connectionKeys %}{% for key in connectionKeys %}
         {{ key }} = data.get("{{ key }}"){% endfor %}{% else %}
         ...    
         {% endif %}
     
     def run(self, params={}):
         #   write your code
-        #   可调用 popEmpty() 去除载荷中的空参数
-        #   使用 setLocalCache()、getLocalCache() 管理本地缓存
         {% if inputKeys %}{% for key in inputKeys %}
         {{ key }} = params.get("{{ key }}"){% endfor %}{% else %}
         ...
         {% endif %}
 """
 
 triggers_template = """
@@ -79,17 +71,14 @@
         {% if connectionKeys %}{% for key in connectionKeys %}
         {{ key }} = data.get("{{ key }}"){% endfor %}{% else %}
         ...    
         {% endif %}
 
     def run(self, params={}):
         #   write your code
-        #   可调用 popEmpty() 去除载荷中的空参数
-        #   使用 self.setCache() 设置在线缓存
-        #   使用 setLocalCache()、getLocalCache() 管理本地缓存
         #   返回必须使用 self.send({})
         {% if inputKeys %}{% for key in inputKeys %}
         {{ key }} = params.get("{{ key }}"){% endfor %}{% else %}
         ...
         {% endif %}
 """
 
@@ -118,18 +107,15 @@
         {% if connectionKeys %}{% for key in connectionKeys %}
         {{ key }} = data.get("{{ key }}"){% endfor %}{% else %}
         ...    
         {% endif %}
 
     def run(self, params={}):
         #   write your code
-        #   可调用 popEmpty() 去除载荷中的空参数
         #   返回必须使用 self.send({})
-        #   使用 self.setCache() 设置在线缓存
-        #   使用 setLocalCache()、getLocalCache() 管理本地缓存
         {% if inputKeys %}{% for key in inputKeys %}
         {{ key }} = params.get("{{ key }}"){% endfor %}{% else %}
         ...
         {% endif %}
 
 """
 
@@ -197,18 +183,15 @@
         {% if connectionKeys %}{% for key in connectionKeys %}
         {{ key }} = data.get("{{ key }}"){% endfor %}{% else %}
         ...    
         {% endif %}
 
     def run(self, params={}):
         #   write your code
-        #   可调用 popEmpty() 去除载荷中的空参数
         #   返回必须使用 self.send({})
-        #   使用 self.setCache() 设置在线缓存
-        #   使用 setLocalCache()、getLocalCache() 管理本地缓存
         {% if inputKeys %}{% for key in inputKeys %}
         {{ key }} = params.get("{{ key }}"){% endfor %}{% else %}
         ...
         {% endif %}
 
 
 """
@@ -519,61 +502,82 @@
   }
 }
 """
 
 main_template = """#!/usr/bin/env python
 
 from SDK.cli import client
-{% if actions %}
-import actions{% endif %}
-{% if triggers %}
-import triggers{% endif %}
-{% if indicator_receivers %}
-import indicator_receivers{% endif %}
-{% if alarm_receivers %}
-import alarm_receivers{% endif %}
-{% if asset_receivers %}
-import asset_receivers{% endif %}
+from SDK.base import log
+from traceback import format_exc
+
+{% if actions %}try:
+    import actions
+except:
+    log("error",format_exc())
+{% endif %}
+{% if triggers %}try:
+    import triggers
+except:
+    log("error",format_exc())
+{% endif %}
+{% if indicator_receivers %}try:
+    import indicator_receivers
+except:
+    log("error",format_exc())
+{% endif %}
+{% if alarm_receivers %}try:
+    import alarm_receivers
+except:
+    log("error",format_exc())
+{% endif %}
+{% if asset_receivers %}try:
+    import asset_receivers
+except:
+    log("error",format_exc())
+{% endif %}
 
 # 整个程序入口
 
 class {{ pluginName }}(object):
 
     def __init__(self):
 
         self.connection = {}
         self.actions = {}
         self.triggers = {}
         self.indicator_receivers = {}
         self.alarm_receivers = {} 
         self.asset_receivers = {}
         
-        {% for actionClass in actions %}
-        self.add_actions(actions.{{ actionClass }}())
+        {% for actionClass in actions %}try:
+            self.add_actions(actions.{{ actionClass }}())
+        except:
+            pass
         {% endfor %}
-
-        {% for triggerClass in triggers %}
-        self.add_triggers(triggers.{{ triggerClass }}())
+        {% for triggerClass in triggers %}try:
+            self.add_triggers(triggers.{{ triggerClass }}())
+        except:
+            pass
         {% endfor %}
-
-        {% for indicatorReceiverClass in indicator_receivers %}
-        self.add_indicator_receivers(indicator_receivers.{{ indicatorReceiverClass }}())
+        {% for indicatorReceiverClass in indicator_receivers %}try:
+            self.add_indicator_receivers(indicator_receivers.{{ indicatorReceiverClass }}())
+        except:
+            pass
         {% endfor %}
-        
-        {% for alarmReceiverClass in alarm_receivers %}
-        self.add_alarm_receivers(alarm_receivers.{{ alarmReceiverClass }}())
+        {% for alarmReceiverClass in alarm_receivers %}try:
+            self.add_alarm_receivers(alarm_receivers.{{ alarmReceiverClass }}())
+        except:
+            pass
         {% endfor %}
-        
-        {% for assetReceiversClass in asset_receivers %}
-        self.add_asset_receivers(asset_receivers.{{ assetReceiversClass }}())
+        {% for assetReceiversClass in asset_receivers %}try:
+            self.add_asset_receivers(asset_receivers.{{ assetReceiversClass }}())
+        except:
+            pass
         {% endfor %}
         
-    def add_connection(self, connect):
-        self.connection[connect.name] = connect
-
     def add_actions(self, action):
         self.actions[action.name] = action
 
     def add_triggers(self, trigger):
         self.triggers[trigger.name] = trigger
 
     def add_indicator_receivers(self, indicator_receiver):
@@ -594,27 +598,31 @@
     main()
     
 """
 
 init_template = """
 import sys
 from importlib import reload
-{% if module == "actions" %}
+import traceback
+from SDK.base import log
 from .models import *
 reload(models)
-{% endif %}
+
 {% for name, className in init_list %}
-from .{{ name }} import {{ className }}
+try:
+    from .{{ name }} import {{ className }}
+except:
+    log("error",traceback.format_exc())
 {% endfor %}
 
 def modules_dict():
 
     reload(sys.modules[__name__])
-    {% if module == "actions" %}{% for name, className in init_list %}reload({{ name }})
-    {% endfor %}{% endif %}
+    {% for name, className in init_list %}reload({{ name }})
+    {% endfor %}
     return {
         {% for name, className in init_list %}"{{ name }}": {{ className }},
         {% endfor %}
     }
 """
 
 
@@ -1055,14 +1063,22 @@
 {%- endfor %}
 
 {% endfor %}
 
 {% endif %}
 """
 
+model_template = """
+class {{ className }}(BaseModel):
+    {% if args %}{% for argName, argType in args %}
+    {{ argName }}: {{ argType }}
+    {% endfor %}{% else %}
+    ...
+    {% endif %}"""
+
 indicator_receivers_model_types = """
 class Indicator(BaseModel):
     uid: str
     type: str
     value: str
     source: str
     reputation: str
@@ -1178,170 +1194,27 @@
     created_at: str
     updated_at: str
     
 """
 
 alarm_receivers_model_template = """
 class {{ className }}(BaseModel):
-
     alarm: Alarm
     
 """
 
 asset_receivers_model_types = """
 class Asset(BaseModel):
-    servicer: str = ""
-    device_type: str = ""
-    device_id: str = ""
-    name: str = ""
-    public_ipv4: str = ""
-    inner_ipv4: str = ""
-    location: str = ""
-    department: str = ""
-    description: str = ""
-    mac: str = ""
-    model: str = ""
-    os: str = ""
-    cpu: str = ""
-    ram: str = ""
-    kernel_version: str = ""
-    port: str = ""
-    disk: str = ""
-    software: str = ""
-    tag: Optional[List[str]] = []
-    raw: str = ""
-    created_at: str
-    updated_at: str
+    record: dict
+    details: dict
+    device_id: str
+    monitor: dict = {}
+    status: bool
 """
 
 asset_receivers_model_template = """
 class {{ className }}(BaseModel):
-
-    asset: Asset
-    
-"""
-
-testserver_head_template = r"""
-from fastapi import FastAPI,HTTPException
-import uvicorn
-import typing
-import json
-from SDK.base import * 
-
-description = \
-'''
-  欢迎使用 1.2.8 版本SDK提供的全新测试系统。\n
-  相较于之前的版本的 REST 测试接口，这个版本提供了更加详细的功能细分以及测试数据输入指引。\n
-  现在再也不会几个接口测试一大堆功能，一大堆参数还不知道怎么填了。\n
-  
-  Enjoy it!  -- Matthews_K
-
-'''
-test_server = FastAPI(title="Chariot-Plugin Test Server", version="1.2.8", description=description)
-
-"""
-
-testserver_tail_template = """
-def runserver():
-    os.system("")
-    log("attention","在浏览器内输入 http://127.0.0.1:1453/docs 以进行接口测试")
-    log("attention","在浏览器内输入 http://127.0.0.1:1453/redoc 以查看帮助文档")
-    uvicorn.run(test_server,host="127.0.0.1", port=1453)
-
-
-if __name__ == '__main__':
-
-    runserver()
-"""
-
-testserver_actions_template = """
-@test_server.post("/actions/{{ name }}",response_model={{ class_name }}().outputModel,tags=["动作"])
-def action_{{ name }}(connection_data:{{ class_name }}().connModel=None,
-                      input_data:{{ class_name }}().inputModel=None):
-    
-    clearLog()
-
-    connection_data = connection_data.dict()
-
-    input_data = input_data.dict()
-
-    output = {{ class_name }}()._run(input_data,connection_data)
-
-    if output["body"].get("error_trace"):
-        raise HTTPException(500,detail=output["body"]["error_trace"])
-    else:
-        output_data = output["body"]["output"]
-
-    return output_data
-
-"""
-
-testserver_triggers_template = """
-@test_server.post("/triggers/{{ name }}",response_model={{ class_name }}().outputModel,tags=["触发器"])
-def trigger_{{ name }}(dispatcher_url:str="http://127.0.0.1:8000/send",
-                       connection_data:{{ class_name }}().connModel=None,
-                       input_data:{{ class_name }}().inputModel=None):
-    
-    clearLog()
-
-    connection_data = connection_data.dict()
-
-    input_data = input_data.dict()
-
-    output = {{ class_name }}()._run(input_data,connection_data,dispatcher_url)
-
-    if output["body"].get("error_trace"):
-        raise HTTPException(500,detail=output["body"]["error_trace"])
-    else:
-        output_data = output["body"]["output"]
-
-    return output_data
-
-"""
-
-testserver_alarm_receivers_template = """
-@test_server.post("/alarm_receivers/{{ name }}",response_model={{ class_name }}().outputModel,tags=["告警接收器"])
-def alarm_receiver_{{ name }}(dispatcher_url:str="http://127.0.0.1:8000/send",
-                              connection_data:{{ class_name }}().connModel=None,
-                              input_data:{{ class_name }}().inputModel=None):
-    
-    clearLog()
-
-    connection_data = connection_data.dict()
-
-    input_data = input_data.dict()
-
-    output = {{ class_name }}()._run(input_data,connection_data,dispatcher_url)
-
-    if output["body"].get("error_trace"):
-        raise HTTPException(500,detail=output["body"]["error_trace"])
-    else:
-        output_data = output["body"]["output"]
-
-    return output_data
-
-"""
-
-testserver_indicator_receivers_template = """
-@test_server.post("/indicator_receivers/{{ name }}",response_model={{ class_name }}().outputModel,tags=["情报接收器"])
-def indicator_receiver_{{ name }}(dispatcher_url:str="http://127.0.0.1:8000/send",
-                              connection_data:{{ class_name }}().connModel=None,
-                              input_data:{{ class_name }}().inputModel=None):
-    
-    clearLog()
-
-    connection_data = connection_data.dict()
-
-    input_data = input_data.dict()
-
-    output = {{ class_name }}()._run(input_data,connection_data,dispatcher_url)
-
-    if output["body"].get("error_trace"):
-        raise HTTPException(500,detail=output["body"]["error_trace"])
-    else:
-        output_data = output["body"]["output"]
-
-    return output_data
-
+    source: str
+    asset_type: str
+    records: List[Asset] = []
 """
 
-
```

### Comparing `chariot-sdk-1.3.0/chariotCore/tools.py` & `chariot-sdk-1.3.1/chariotCore/tools.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     "boolean": "bool",
     "float": "float",
     "date": "str",
     "object": "dict",
     "password": "str",
     "integer": "int",
     "file": "dict",
+    #   file的类型是一个包含filename和content的字典
     "any": "Any"
 }
 
 module_dict = {
     "actions": "动作",
     "triggers": "触发器",
     "indicator_receivers": "情报接收器",
@@ -593,230 +594,14 @@
     }
 
     func = renderStrTemplate(func_data, module_template_dict[module])
 
     return func, func_data, init
 
 
-def autoGenerateDataTrans(data: dict) -> dict:
-    """
-    #   将用于自动生成插件的插件特殊定义数据重新整理为一般的插件定义数据
-    #   特殊定义文件相较于一般的插件定义文件在每个功能上的input参数下都对各个需要输入的数据进行了分类
-    #   这一举措是为了确定输入的数据属于构成一次请求中的哪一部分
-    参数说明：
-    data:dict,      #   特殊定义文件的数据
-    """
-
-    log("info", "转换插件定义文件中")
-
-    #   深拷贝一份数据用于操作
-    new_data = deepcopy(data)
-
-    #   用于统一化变量名称，以防出现变量名在python中不可用
-    value_id = 0
-
-    #   转换连接器
-    connection_data = data.get("connection", {})
-    new_data["connection"] = {}
-    for value_type in connection_data:
-        for value in connection_data[value_type]:
-            #   构建新的统一参数名和旧参数名的映射
-            connection_data[value_type][value]["@origin"] = value
-            #   把参数属于哪一类也塞进去
-            connection_data[value_type][value]["@type"] = value_type
-            new_data["connection"][f"value_{value_id}"] = connection_data[value_type][value]
-            value_id += 1
-
-    #   用于重新计数
-    value_temp = value_id
-
-    #   转换动作
-    actions_data = data.get("actions")
-
-    #   遍历动作的每一个功能
-    for func in actions_data:
-        new_data["actions"][func]["input"] = {}
-
-        #   有时候GET请求啥参数也没有
-        if not actions_data[func].get("input"):
-            continue
-
-        #   遍历功能的input部分每一个参数分类
-        for value_type in actions_data[func]["input"]:
-            #   遍历每一个参数分类下的参数
-            for value in actions_data[func]["input"][value_type]:
-                #   构建新的统一参数名和旧参数名的映射
-                actions_data[func]["input"][value_type][value]["@origin"] = value
-                #   把参数属于哪一类也塞进去
-                actions_data[func]["input"][value_type][value]["@type"] = value_type
-                new_data["actions"][func]["input"][f"value_{value_id}"] = actions_data[func]["input"][value_type][value]
-                value_id += 1
-
-        value_id = value_temp
-
-    return new_data
-
-
-def autoGeneratePluginSpecFile(data: dict):
-    """
-    #   从特殊定义文件中自动生成一般插件定义文件
-    #   一个插件总得有个定义文件不是吗？
-    参数说明：
-    data:dict,      #   特殊定义文件的数据
-    """
-    with open("plugin.spec.json", "w", encoding="utf-8") as file:
-        json.dump(data, file, ensure_ascii=False)
-
-
-def autoGenerateActionsFile(work_path: str, module_data: dict) -> list:
-    """
-    #   生成请求API专用的动作运行文件
-    #   大部分API接口只需要构造简单的Requests就能直接调用，因此可以高度模板化，减少开发时间
-    #   与“生成所有功能的运行文件”方法不同的是，高度模板化带来的是更多详细参数的需求，其他方面则无太大区别
-    参数说明：
-    work_path:str,    #   当前工作区绝对路径
-    module_data:dict,    #   组件的参数
-    """
-
-    #   用于记录要在初始化文件（__init__.py）中写入的功能导入（import）
-    init_list = []
-
-    #   功能列表 key_list，用于生成入口文件 main.py
-    key_list = []
-
-    #   组件文件夹路径
-    key_path = os.path.join(work_path, "actions")
-
-    #   获取连接器数据
-    connection_url_params_keys = []
-    connection_headers_keys = []
-    connection_params_keys = []
-    connection_body_keys = []
-    connection_files_keys = []
-    connection_ssl_verify = ()
-    for value, value_params in module_data.get("connection", {}).items():
-        if value_params["@type"] == "url_params":
-            connection_url_params_keys.append((value, value_params["@origin"]))
-        elif value_params["@type"] == "headers":
-            connection_headers_keys.append((value, value_params["@origin"]))
-        elif value_params["@type"] == "params":
-            connection_params_keys.append((value, value_params["@origin"]))
-        elif value_params["@type"] == "body":
-            connection_body_keys.append((value, value_params["@origin"]))
-        elif value_params["@type"] == "files":
-            connection_files_keys.append((value, value_params["@origin"]))
-        elif value_params["@type"] == "ssl_verify":
-            connection_ssl_verify = (value, value_params["@origin"])
-
-    #   遍历组件内每一个功能和功能的参数
-    for module_key, params in module_data.get("actions", {}).items():
-        try:
-
-            log("info", rf"生成 actions\{module_key}.py 文件中")
-
-            #   存储用于渲染功能文件内容的数据
-            key_data = {}
-
-            #   功能类名采用全大写
-            key_class_name = module_key.upper() + "_ACTION"
-            key_data["actionsName"] = key_class_name
-
-            init_list.append([module_key, key_class_name])
-
-            #   设定渲染模板
-            key_template = action_rest_template
-            key_test_template = actions_test_template
-
-            #   功能列表，用于生成入口文件 main.py
-            key_list.append(key_class_name)
-
-            #   设置input, output类名
-            input_class_name = module_key.upper() + "_INPUT"
-            output_class_name = module_key.upper() + "_OUTPUT"
-
-            #   获取动作数据
-            run_url_params_keys = []
-            run_headers_keys = []
-            run_params_keys = []
-            run_body_keys = []
-            run_files_keys = []
-            run_ssl_verify = ()
-
-            for value in params["input"]:
-                if params["input"][value]["@type"] == "url_params":
-                    run_url_params_keys.append((value, params["input"][value]["@origin"]))
-                elif params["input"][value]["@type"] == "headers":
-                    run_headers_keys.append((value, params["input"][value]["@origin"]))
-                elif params["input"][value]["@type"] == "params":
-                    run_params_keys.append((value, params["input"][value]["@origin"]))
-                elif params["input"][value]["@type"] == "body":
-                    run_body_keys.append((value, params["input"][value]["@origin"]))
-                elif params["input"][value]["@type"] == "files":
-                    run_files_keys.append((value, params["input"][value]["@origin"]))
-                elif params["input"][value]["@type"] == "ssl_verify":
-                    run_ssl_verify = (value, params["input"][value]["@origin"])
-
-            #   获取请求方式
-            method = params["method"]
-            #   获取URL
-            url = params["url"]
-            #   对URL中的参数进行整理
-            for url_param in connection_url_params_keys:
-                url = str(url).replace("{" + f"{url_param[1]}" + "}", "{self." + url_param[0] + "}")
-            for url_param in run_url_params_keys:
-                url = str(url).replace("{" + url_param[1] + "}", "{self." + url_param[0] + "}")
-
-            #   获取请求体类型
-            body_type = params.get("body_type", None)
-
-            key_data.update({
-                "name": module_key,
-                "inputModel": input_class_name,
-                "outputModel": output_class_name,
-                "connModel": "CONNECTION",
-                "method": method,
-                "url": url,
-                "body_type": body_type,
-                "connection_url_params_keys": connection_url_params_keys,
-                "connection_headers_keys": connection_headers_keys,
-                "connection_params_keys": connection_params_keys,
-                "connection_body_keys": connection_body_keys,
-                "connection_files_keys": connection_files_keys,
-                "connection_ssl_verify": connection_ssl_verify,
-                "run_url_params_keys": run_url_params_keys,
-                "run_headers_keys": run_headers_keys,
-                "run_params_keys": run_params_keys,
-                "run_body_keys": run_body_keys,
-                "run_files_keys": run_files_keys,
-                "run_ssl_verify": run_ssl_verify
-            })
-
-            #   渲染组件内不同功能文件内容
-            key = renderStrTemplate(key_data, key_template)
-
-            file_path = os.path.join(key_path, f"{module_key}.py")
-
-            with open(file_path, "w", encoding="utf-8", newline="\n") as file:
-                file.write(key)
-
-            log("info", rf"actions\{module_key}.py 生成完成")
-
-        except Exception as error:
-            raise Exception(rf"actions\{module_key}.py 生成失败，原因未知：" + f"\n{error}")
-
-        #   生成测试用的json文件
-        generateTestFile(key_data, key_test_template)
-
-    generateInitFile("actions", key_path, init_list)
-
-    log("info", f"{module_dict['actions']}（actions）所有功能生成完成")
-
-    return key_list
-
-
 def generateTestFile(func_data, func_test_template):
     """
     #   生成测试用的json文件
     参数说明：
     func_data:dict,     #   功能的各项参数
     key_test_template:str,  #   需要渲染的测试文件模板
     生成失败时抛出异常
@@ -1004,16 +789,14 @@
 
 def generateHelpFile(yaml_data: dict):
     """
     #   生成帮助文件
     参数说明：
     yaml_data:dict,     #   yaml文件数据
 
-    **此方法生成的文件基本用不上，预计在将来版本删除**
-
     生成失败时抛出异常
     """
 
     log("info", r"生成帮助文件 \help.md 中")
 
     try:
         file_path = os.path.join(os.getcwd(), "help.md")
@@ -1072,102 +855,14 @@
 
     except Exception as error:
         raise Exception(r"热更新源码包存储文件夹 \update 失败，原因未知：" + f"\n{error}")
 
     log("info", r"热更新源码包存储文件夹 \update 生成完成")
 
 
-def generateTestServerFile(work_path: str,
-                           actions_list: list,
-                           triggers_list: list,
-                           indicator_receivers_list: list,
-                           alarm_receivers_list: list):
-    """
-    **此方法暂时弃用**
-
-    #   生成本地REST测试服务器文件
-    参数说明：
-    work_path:str,      #   当前工作区绝对路径
-    actions_list:list,      #   动作列表
-    triggers_list:list,     #   触发器列表
-    indicator_receivers_list:list,      #   情报接收器列表
-    alarm_receivers_list:list,          #   告警接收器列表
-
-    生成失败时抛出异常
-    """
-
-    log("info", r"生成本地REST测试服务器数据文件 \testserver.py 中")
-
-    testserver_file_content = testserver_head_template
-
-    if actions_list:
-
-        testserver_file_content = "\nfrom actions import *" + testserver_file_content
-
-        for action in actions_list:
-            action_data = {
-                "class_name": action,
-                "name": action.replace("_ACTION", "").lower()
-            }
-
-            testserver_file_content += renderStrTemplate(action_data, testserver_actions_template)
-
-    if triggers_list:
-
-        testserver_file_content = "\nfrom triggers import *" + testserver_file_content
-
-        for trigger in triggers_list:
-            trigger_data = {
-                "class_name": trigger,
-                "name": trigger.replace("_TRIGGER", "").lower()
-            }
-
-            testserver_file_content += renderStrTemplate(trigger_data, testserver_triggers_template)
-
-    if indicator_receivers_list:
-
-        testserver_file_content = "\nfrom indicator_receivers import *" + testserver_file_content
-
-        for indicator_receiver in indicator_receivers_list:
-            indicator_receiver_data = {
-                "class_name": indicator_receiver,
-                "name": indicator_receiver.replace("_INDICATOR_RECEIVER", "").lower()
-            }
-
-            testserver_file_content += renderStrTemplate(indicator_receiver_data,
-                                                         testserver_indicator_receivers_template)
-
-    if alarm_receivers_list:
-
-        testserver_file_content = "\nfrom alarm_receivers import *" + testserver_file_content
-
-        for alarm_receiver in alarm_receivers_list:
-            alarm_receiver_data = {
-                "class_name": alarm_receiver,
-                "name": alarm_receiver.replace("_ALARM_RECEIVER", "").lower()
-            }
-
-            testserver_file_content += renderStrTemplate(alarm_receiver_data, testserver_alarm_receivers_template)
-
-    testserver_file_content += testserver_tail_template
-
-    try:
-
-        testserver_file_path = os.path.join(work_path, "testserver.py")
-
-        with open(testserver_file_path, "w", encoding="utf-8") as file:
-
-            file.write(testserver_file_content)
-
-    except Exception as error:
-        raise Exception(rf"本地REST测试服务器数据文件 \testserver.py 生成失败 \n   {error}")
-
-    log("info", r"本地REST测试服务器数据文件 \testserver.py 生成完成")
-
-
 def argsSetupData(param_name: str, params: dict) -> list:
     """
     #   整理构成参数方便调用
     参数说明：
     param_name:str,     #   集合名称（自定义类名称、输入集合名称、输出集合名称）
     params:dict,    #   构成参数
 
@@ -1354,27 +1049,45 @@
     data = readGenerateFile(work_path, "plugin.spec.yaml")
 
     #   获取插件定义文件中的元数据
     vendor = data["vendor"]
     name = data["name"]
     version = data["version"]
 
+    #   builds文件夹用于放置构建好的包
+    builds_dir_path = os.path.join(work_path, "builds")
+
+    if not os.path.exists(builds_dir_path) or not os.path.isdir(builds_dir_path):
+        os.mkdir(builds_dir_path)
+
+
     #   在线包文件名
+    #   当传入在线包名称时，一般是要创建临时在线包
     if pack_name:
         tar_name = pack_name
+    #   当打包在线包时，需要创建临时插件结构文件
     else:
         tar_name = f"{vendor}-{name}-{version}.tar.gz"
 
-    #   排除可能存在的离线包
-    offline_name = f"{vendor}-{name}-{version}-offline.tar.gz"
+        #   打包在线包时，需要保存一个数据整合文件
+        plugin = {
+            "plugin_data": data,
+            "plugin_code": getAllModulesCode()
+        }
+        with open(os.path.join(work_path, "plugin.construction.json"), "w", encoding="utf-8") as file:
+            json.dump(plugin, file, ensure_ascii=False)
 
-    tar = tarfile.open(os.path.join(work_path, tar_name), "w:gz", format=tarfile.GNU_FORMAT)
+    #   创建压缩包
+    tar = tarfile.open(os.path.join(builds_dir_path, tar_name), "w:gz", format=tarfile.GNU_FORMAT)
 
     #   默认排除项
-    ignore = ["__sdkcache__", "__pycache__", offline_name, f"{vendor}-{name}-{version}.tar.gz"]
+    ignore = ["__sdkcache__",
+              "__pycache__",
+              "__temp__",
+              "builds"]
 
     ignore.extend(loadIgnore())
 
     #   去重
     ignore = list(set(ignore))
 
     for file in os.listdir(work_path):
@@ -1382,8 +1095,93 @@
             log("info", f"{file}已忽略")
             continue
         else:
             tar.add(os.path.join(work_path, file), arcname=file)
 
     tar.close()
 
+    #   清除可能存在的临时结构文件
+    if os.path.exists(os.path.join(work_path, "plugin.construction.json")):
+        os.remove(os.path.join(work_path, "plugin.construction.json"))
+
     return data
+
+
+def deleteOldFile(modules_list_dict):
+    """
+    #   删除老旧文件
+    参数说明：
+    modules_list_dict: dict
+    """
+    log("info", "清理旧的文件中")
+
+    work_path = os.getcwd()
+
+    for module, func_id_list in modules_list_dict.items():
+        module_path = os.path.join(work_path, module)
+
+        if os.path.exists(module_path):
+            file_list = os.listdir(module_path)
+
+            ignore_files = ["models.py", "__init__.py", "__pycache__"]
+            for ignore_file in ignore_files:
+                if ignore_file in file_list:
+                    file_list.pop(file_list.index(ignore_file))
+
+            for index in range(len(func_id_list)):
+                func_id_list[index] += ".py"
+
+            #   如果目前一个方法都没有了，直接删文件夹
+            if not func_id_list:
+                shutil.rmtree(module_path)
+                continue
+
+            #   原有方法的集合 减去 目前方法的集合 即为 要删除的方法的集合
+            need_delete = list(set(file_list) - set(func_id_list))
+
+            for file in need_delete:
+                os.remove(os.path.join(work_path, module, file))
+
+        else:
+            continue
+
+    log("info", "清理完成")
+
+
+def getAllModulesCode():
+    """
+    #   获取所有功能的代码
+    """
+
+    work_path = os.getcwd()
+
+    modules_dir = ["actions", "triggers", "alarm_receivers", "indicator_receivers", "asset_receivers"]
+
+    modules_dict = {}
+
+    for temp_module in modules_dir:
+
+        modules_dict[temp_module] = []
+
+        modules_dir_path = os.path.join(work_path, temp_module)
+
+        if not os.path.exists(modules_dir_path):
+            continue
+
+        module_files = os.listdir(modules_dir_path)
+
+        ignore_files = ["models.py", "__init__.py", "__pycache__"]
+
+        for ignore_file in ignore_files:
+            if ignore_file in module_files:
+                module_files.pop(module_files.index(ignore_file))
+
+        for module_file in module_files:
+            module_file_path = os.path.join(modules_dir_path, module_file)
+
+            with open(module_file_path, "r", encoding="utf-8") as module_file_code:
+                modules_dict[temp_module].append({
+                    "func_name": module_file.replace(".py", ""),
+                    "func_code": module_file_code.read()
+                })
+
+    return modules_dict
```

### Comparing `chariot-sdk-1.3.0/chariot_sdk.egg-info/PKG-INFO` & `chariot-sdk-1.3.1/chariot_sdk.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chariot-sdk
-Version: 1.3.0
+Version: 1.3.1
 Summary: Chariot plugin maker
 Home-page: https://pypi.org/
 Author: chariot
 Author-email: chariot@example.com
 License: MIT
 Requires-Python: >=3
 Description-Content-Type: text/markdown
@@ -20,14 +20,31 @@
 - python 3.8+
 
 ### 安装
 > pip install chariot-sdk
 
 ### 更新日志
 
+> 1.3.0 -> 1.3.1
+
+- 修改资产接收器的输出结构，现在资产的key值将决定前端展示的文本
+- 去除yaml文件中的multi_workers、hot_update参数，新增sdk参数用于记录开发插件用的SDK版本，以后千乘将根据sdk参数（版本）来判断插件支持的功能
+- 添加-r命令下测试资产接收器的功能
+- api接口现在会限制测试时接收器的数量为1，在启动下一个接收器时，上一个接收器会被自动关闭（也可以手动关闭接收器）
+- 提高了SDK对插件出现错误时的兼容，从而更好地防范热改动功能引发的SDK崩溃
+- 新增了更多的可能的错误信息日志、
+- 新增对打包不同架构的离线包支持，现在可以在-mki命令后添加平台参数以获得不同架构下的离线包，如chariot-plugin -mki linux/arm64
+- 打包插件现在会在压缩包内自动添加上插件的结构信息和代码信息（plugin.construction.json），以适应将来上线的热改动功能
+- 现在打包好的插件会被放在插件根目录下的builds文件夹内
+- 重构了自动生成插件的功能
+- 重构了获取插件定义数据的功能
+- 修正了一些chariot-plugin -h中的帮助内容
+- 删除testserver测试功能
+- 调整生成插件时的模板文件
+
 > 1.2.10 -> 1.3.0
 
 - 修复了非Debug模式下，debug等级的日志仍然会在某种条件下输出的bug
 - 修复了Debug模式切换后无法切换回去的bug
 - 调整了重载配置行为的位置，修复了原来在完成连接器的运行后才加载配置的bug
 - 新增资产接收器模块，此模块专门用于转发资产相关的信息
 - 新增查询插件使用SDK版本信息接口
```

### Comparing `chariot-sdk-1.3.0/chariot_sdk.egg-info/SOURCES.txt` & `chariot-sdk-1.3.1/chariot_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chariot-sdk-1.3.0/setup.py` & `chariot-sdk-1.3.1/setup.py`

 * *Files identical despite different names*

