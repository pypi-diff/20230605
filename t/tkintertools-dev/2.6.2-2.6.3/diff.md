# Comparing `tmp/tkintertools-dev-2.6.2.tar.gz` & `tmp/tkintertools-dev-2.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkintertools-dev-2.6.2.tar", last modified: Fri May 26 12:10:48 2023, max compression
+gzip compressed data, was "tkintertools-dev-2.6.3.tar", last modified: Mon Jun  5 17:10:00 2023, max compression
```

## Comparing `tkintertools-dev-2.6.2.tar` & `tkintertools-dev-2.6.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 12:10:48.146677 tkintertools-dev-2.6.2/
--rw-rw-rw-   0        0        0     7548 2023-05-20 23:03:00.000000 tkintertools-dev-2.6.2/LICENSE
--rw-rw-rw-   0        0        0    24785 2023-05-26 12:10:48.144676 tkintertools-dev-2.6.2/PKG-INFO
--rw-rw-rw-   0        0        0    24276 2023-05-26 12:08:22.000000 tkintertools-dev-2.6.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-26 12:10:48.146677 tkintertools-dev-2.6.2/setup.cfg
--rw-rw-rw-   0        0        0     1210 2023-05-26 12:10:07.000000 tkintertools-dev-2.6.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-26 12:10:48.138692 tkintertools-dev-2.6.2/tkintertools/
--rw-rw-rw-   0        0        0     1852 2023-05-26 05:11:00.000000 tkintertools-dev-2.6.2/tkintertools/__init__.py
--rw-rw-rw-   0        0        0    60774 2023-05-26 05:03:13.000000 tkintertools-dev-2.6.2/tkintertools/__main__.py
--rw-rw-rw-   0        0        0     1295 2023-05-22 14:06:44.000000 tkintertools-dev-2.6.2/tkintertools/constants.py
--rw-rw-rw-   0        0        0     9992 2023-05-26 12:02:58.000000 tkintertools-dev-2.6.2/tkintertools/tools_3d.py
-drwxrwxrwx   0        0        0        0 2023-05-26 12:10:48.143674 tkintertools-dev-2.6.2/tkintertools_dev.egg-info/
--rw-rw-rw-   0        0        0    24785 2023-05-26 12:10:47.000000 tkintertools-dev-2.6.2/tkintertools_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-05-26 12:10:48.000000 tkintertools-dev-2.6.2/tkintertools_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 12:10:47.000000 tkintertools-dev-2.6.2/tkintertools_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-26 12:10:47.000000 tkintertools-dev-2.6.2/tkintertools_dev.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-05 17:10:00.511235 tkintertools-dev-2.6.3/
+-rw-rw-rw-   0        0        0     7548 2023-05-27 20:59:02.000000 tkintertools-dev-2.6.3/LICENSE
+-rw-rw-rw-   0        0        0    28175 2023-06-05 17:10:00.509223 tkintertools-dev-2.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0    27670 2023-06-05 16:18:37.000000 tkintertools-dev-2.6.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-05 17:10:00.512236 tkintertools-dev-2.6.3/setup.cfg
+-rw-rw-rw-   0        0        0     1216 2023-05-30 16:20:05.000000 tkintertools-dev-2.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 17:10:00.498001 tkintertools-dev-2.6.3/tkintertools/
+-rw-rw-rw-   0        0        0     2922 2023-06-05 17:07:12.000000 tkintertools-dev-2.6.3/tkintertools/__init__.py
+-rw-rw-rw-   0        0        0    60866 2023-06-05 13:14:52.000000 tkintertools-dev-2.6.3/tkintertools/__main__.py
+-rw-rw-rw-   0        0        0     2136 2023-06-05 17:00:41.000000 tkintertools-dev-2.6.3/tkintertools/constants.py
+-rw-rw-rw-   0        0        0    14759 2023-06-05 13:09:11.000000 tkintertools-dev-2.6.3/tkintertools/tools_3d.py
+drwxrwxrwx   0        0        0        0 2023-06-05 17:10:00.505011 tkintertools-dev-2.6.3/tkintertools_dev.egg-info/
+-rw-rw-rw-   0        0        0    28175 2023-06-05 17:10:00.000000 tkintertools-dev-2.6.3/tkintertools_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-06-05 17:10:00.000000 tkintertools-dev-2.6.3/tkintertools_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 17:10:00.000000 tkintertools-dev-2.6.3/tkintertools_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-05 17:10:00.000000 tkintertools-dev-2.6.3/tkintertools_dev.egg-info/top_level.txt
```

### Comparing `tkintertools-dev-2.6.2/LICENSE` & `tkintertools-dev-2.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tkintertools-dev-2.6.2/PKG-INFO` & `tkintertools-dev-2.6.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,89 +1,184 @@
-Metadata-Version: 2.1
-Name: tkintertools-dev
-Version: 2.6.2
-Summary: An auxiliary module of the tkinder module
-Home-page: https://gitcode.net/weixin_62651706/tkintertools
-Author: Xiaokang2022
-Author-email: 2951256653@qq.com
-License: MulanPSL-2.0
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <div align="center">
     <h1>🚀tkintertools🚀</h1>
     <p><img height="120px" alt="logo.png"
-        src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/tkintertools.png" />
+        src="./tkintertools.png" />
     </p>
     <p>The <code>tkintertools</code> module is an auxiliary module of the <code>tkinter</code> module</p>
     <p><code>tkintertools</code> 模块是 <code>tkinter</code> 模块的辅助模块</p>
     <p>
         <a href="./tkintertools/__init__.py">
-            <img src="https://img.shields.io/badge/Version-2.6.1-blue" alt="latest version" />
+            <img src="https://img.shields.io/badge/Version-2.6.2-blue" alt="latest version" />
         </a>
         <a href="./LICENSE">
             <img src="https://img.shields.io/badge/License-Mulan PSL v2-green" alt="License" />
         </a>
         <a href="./CHANGELOG.md">
-            <img src="https://img.shields.io/badge/ChangeLog-2023/05/26-orange" alt="ChangeLog" />
+            <img src="https://img.shields.io/badge/ChangeLog-2023/06/06-orange" alt="ChangeLog" />
         </a>
         <a href="./TODO.md">
-            <img src="https://img.shields.io/badge/ToDos-10-yellow" alt="ToDos" />
+            <img src="https://img.shields.io/badge/ToDos-13-yellow" alt="ToDos" />
         </a>
         <a href="https://pypistats.org/packages/tkintertools">
             <img src="https://img.shields.io/badge/Downloads-3k-purple" alt="Downloads" />
         </a>
     </p>
     <p>
         <a href="mailto:2951256653@qq.com">
             <img src="https://img.shields.io/badge/Email-2951256653@qq.com-cyan" alt="Email" />
         </a>
         <a href="https://xiaokang2022.blog.csdn.net">
             <img src="https://img.shields.io/badge/Blog-小康2022@CSDN-red" alt="Blog" />
         </a>
-        <a href="https://gitcode.net/weixin_62651706">
+        <a href="https://github.com/Xiaokang2022">
             <img src="https://img.shields.io/badge/Author-小康2022-white" alt="Author" />
         </a>
     </p>
 </div>
 
 Installation/模块安装
 -----------------------
 
 ### Stable version/稳定版本
 
-* Version/版本 : 2.6.1
-* Release Date/发布日期 : 2023/05/21
+* Version/版本 : 2.6.2
+* Release Date/发布日期 : 2023/05/30
 
 ```
-pip install tkintertools==2.6.1
+pip install tkintertools==2.6.2
 ```
 或者
 ```
 pip install tkintertools
 ```
 
-这个是目前的最新版，比较稳定，bug 没有那么多，推荐使用这个。  
+这个是目前的最新稳定版，比较稳定，bug 没有那么多，推荐使用这个。  
 稳定版有文档可以查看，有 issue 我会去查看并尝试解决 issue。
 
 ### Development version/开发版本
 
-* Version/版本 : 2.6.2
-* Release Date/发布日期 : 2023/05/26
+* Version/版本 : 2.6.3
+* Release Date/发布日期 : 2023/06/06
 
 ```
-pip install tkintertools-dev==2.6.2
+pip install tkintertools-dev==2.6.3
 ```
 
-这个是作者正在开发的版本，有新功能，但不能保证稳定，bug 可能会比较多。  
+这个是我正在开发的版本，有新功能，但不能保证稳定，bug 可能会比较多。  
 开发版本没有对应的文档，大家可以在 issue 中提出建议，我会适当采纳一些并在开发版本中更改或实现。
 
+News/最新功能
+------------
+
+最新版的`tkintertools`为`2.6.2`，新增一项极为强大的功能：3d绘图！  
+同时修复一些bug，优化了一部分代码，提升了一部分性能。
+
+通过以下代码来使用3d绘图功能：
+
+```python
+from tkintertools import tools_3d as t3d
+import tkintertools.tools_3d as t3d
+# 两种引入方式都可以
+```
+
+子模块: [tools_3d.py](./tkintertools/tools_3d.py)
+
+目前3d绘图功能还比较简陋，仅能绘制点、线、面以及直边的空间几何体，对于曲边的空间几何体还在开发中！  
+以下是一个使用3d绘图的示例：
+
+在这个示例中，按住鼠标左键可以旋转几何体，按住鼠标右键可以平移几何体，滚动鼠标滚轮可以缩放几何体！  
+x、y 和 z 轴分别是红色、绿色和蓝色的线。
+
+![3d绘图](./docs/images/3d.png)
+
+<details><summary><b>源代码</b></summary>
+
+```python
+import random
+import tkinter
+
+import tkintertools as tkt
+from tkintertools import tools_3d as t3d
+
+root = tkt.Tk('tools_3d', 1280, 720)
+canvas = t3d.Canvas_3D(root, 1280, 720, 0, 0)
+
+geos = []  # type: list[t3d.Geometry]
+origin = t3d.Point(canvas, [0, 0, 0], size=5)  # 原点
+axes = [t3d.Line(canvas, [0, 0, 0], [100, 0, 0], width=3, fill='red'),  # 创建坐标轴
+        t3d.Line(canvas, [0, 0, 0], [0, 100, 0], width=3, fill='green'),
+        t3d.Line(canvas, [0, 0, 0], [0, 0, -100], width=3, fill='blue')]
+
+for _ in range(8):
+    # 创建正方体
+    cube = t3d.Cuboid(
+        canvas, *random.sample(range(-200, 200), 3), *random.sample(range(50, 100), 3))
+    geos.append(cube)
+    # 创建四面体
+    x, y, z = random.sample(range(-200, 200), 3)
+    tetr = t3d.Tetrahedron(
+        canvas, *[[x+random.randint(-100, 100), y+random.randint(-100, 100), z+random.randint(-100, 100)] for _ in range(4)])
+    geos.append(tetr)
+
+
+def translate(event, flag=False, _cache=[]):
+    # type: (tkinter.Event, bool, list[float]) -> None
+    """ 平移事件 """
+    if flag:
+        _cache[:] = [event.x, event.y]
+        return
+    dx = (event.x - _cache[0]) / 6
+    dy = (event.y - _cache[1]) / 6
+    _cache[:] = [event.x, event.y]
+    for axis in axes:
+        axis.translate(0, 6*dx, 6*dy)
+        axis.update()
+    for geo in geos:
+        geo.translate(0, dx, dy)
+        geo.update()
+    origin.translate(0, 6*dx, 6*dy)
+    origin.update()
+
+
+def rotate(event, flag=False, _cache=[]):  # type: (tkinter.Event, bool, list[float]) -> None
+    """ 旋转事件 """
+    if flag:
+        _cache[:] = [event.x, event.y]
+        return
+    dy = (event.x - _cache[0]) / 200
+    dx = (_cache[1] - event.y) / 200
+    _cache[:] = [event.x, event.y]
+    for axis in axes:
+        axis.rotate(0, 6*dx, 6*dy, center=origin.coords)
+        axis.update()
+    for geo in geos:
+        geo.rotate(0, dx, dy, center=origin.coords)
+        geo.update()
+
+
+def scale(event):  # type: (tkinter.Event) -> None
+    """ 缩放事件 """
+    k = 1.01 if event.delta > 0 else 0.99
+    for geo in geos:
+        geo.scale(k, k, k)
+        geo.update()
+
+
+root.bind('<Button-1>', lambda event: rotate(event, True))
+root.bind('<B1-Motion>', rotate)
+root.bind('<Button-3>', lambda event: translate(event, True))
+root.bind('<B3-Motion>', translate)
+root.bind('<MouseWheel>', scale)
+root.mainloop()
+```
+
+</details>
+
+更多更新信息请见：[CHANGELOG.md](./CHANGELOG.md)
+
 Description/模块说明
 ----------------------
 
 tkintertools 是一款基于 tkinter 模块的二次开发的界面编程模块，它完全没有使用任何第三方模块和库的，同时，它也没有任何依赖包，它的功能完全由内置模块和函数实现，而且，它还是跨平台的！它和 tkinter 最大的不同在于，它的控件并非真实的控件，而是在 tkinter 模块中 Canvas 对象中绘制而成的，这就赋予了 tkintertools 控件一些在 tkinter 中没有的特性，列举如下：
 
 * 控件背景可以是透明的（实际上是没有背景颜色）
 * 控件的样式可以是自定义的（比如按钮有圆角）
@@ -580,17 +675,17 @@
 
 ![exam3_1.png](docs/examples/exam3_1.png)
 ![exam3_2.png](docs/examples/exam3_2.png)
 
 More/更多
 ---------
 
-> GitCode:  
-> https://gitcode.net/weixin_62651706/tkintertools
+> GitHub:  
+> https://github.com/Xiaokang2022/tkintertools
 
-> GitHub(Mirror/镜像):  
-> https://github.com/XiaoKang2022-CSDN/tkintertools
+> GitCode(Mirror/镜像):  
+> https://gitcode.net/weixin_62651706/tkintertools
 
-> Column/专栏:  
-> https://blog.csdn.net/weixin_62651706/category_11600888.html
+> Gitee(Mirror/镜像):  
+> https://gitee.com/xiaokang-2022/tkintertools
 
 还有更多内容请在 [源代码](./tkintertools/) 中探索！
```

#### html2text {}

```diff
@@ -1,33 +1,66 @@
-Metadata-Version: 2.1 Name: tkintertools-dev Version: 2.6.2 Summary: An
-auxiliary module of the tkinder module Home-page: https://gitcode.net/
-weixin_62651706/tkintertools Author: Xiaokang2022 Author-email:
-2951256653@qq.com License: MulanPSL-2.0 Classifier: Programming Language ::
-Python :: 3 Classifier: License :: OSI Approved :: Mulan Permissive Software
-License v2 (MulanPSL-2.0) Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown License-File: LICENSE
                       ****** ðtkintertoolsð ******
                                   [logo.png]
      The tkintertools module is an auxiliary module of the tkinter module
              tkintertools æ¨¡åæ¯ tkinter æ¨¡åçè¾å©æ¨¡å
           [latest_version] [License] [ChangeLog] [ToDos] [Downloads]
                             [Email] [Blog] [Author]
 Installation/æ¨¡åå®è£ ----------------------- ### Stable version/
-ç¨³å®çæ¬ * Version/çæ¬ : 2.6.1 * Release Date/åå¸æ¥æ : 2023/05/21
-``` pip install tkintertools==2.6.1 ``` æè ``` pip install tkintertools ```
-è¿ä¸ªæ¯ç®åçææ°çï¼æ¯è¾ç¨³å®ï¼bug
+ç¨³å®çæ¬ * Version/çæ¬ : 2.6.2 * Release Date/åå¸æ¥æ : 2023/05/30
+``` pip install tkintertools==2.6.2 ``` æè ``` pip install tkintertools ```
+è¿ä¸ªæ¯ç®åçææ°ç¨³å®çï¼æ¯è¾ç¨³å®ï¼bug
 æ²¡æé£ä¹å¤ï¼æ¨èä½¿ç¨è¿ä¸ªã ç¨³å®çæææ¡£å¯ä»¥æ¥çï¼æ
 issue æä¼å»æ¥çå¹¶å°è¯è§£å³ issueã ### Development version/
-å¼åçæ¬ * Version/çæ¬ : 2.6.2 * Release Date/åå¸æ¥æ : 2023/05/26
-``` pip install tkintertools-dev==2.6.2 ```
-è¿ä¸ªæ¯ä½èæ­£å¨å¼åççæ¬ï¼ææ°åè½ï¼ä½ä¸è½ä¿è¯ç¨³å®ï¼bug
+å¼åçæ¬ * Version/çæ¬ : 2.6.3 * Release Date/åå¸æ¥æ : 2023/06/06
+``` pip install tkintertools-dev==2.6.3 ```
+è¿ä¸ªæ¯ææ­£å¨å¼åççæ¬ï¼ææ°åè½ï¼ä½ä¸è½ä¿è¯ç¨³å®ï¼bug
 å¯è½ä¼æ¯è¾å¤ã å¼åçæ¬æ²¡æå¯¹åºçææ¡£ï¼å¤§å®¶å¯ä»¥å¨ issue
 ä¸­æåºå»ºè®®ï¼æä¼éå½éçº³ä¸äºå¹¶å¨å¼åçæ¬ä¸­æ´æ¹æå®ç°ã
-Description/æ¨¡åè¯´æ ---------------------- tkintertools æ¯ä¸æ¬¾åºäº
-tkinter
+News/ææ°åè½ -----------
+-
+ææ°çç`tkintertools`ä¸º`2.6.2`ï¼æ°å¢ä¸é¡¹æä¸ºå¼ºå¤§çåè½ï¼3dç»å¾ï¼
+åæ¶ä¿®å¤ä¸äºbugï¼ä¼åäºä¸é¨åä»£ç ï¼æåäºä¸é¨åæ§è½ã
+éè¿ä»¥ä¸ä»£ç æ¥ä½¿ç¨3dç»å¾åè½ï¼ ```python from tkintertools import
+tools_3d as t3d import tkintertools.tools_3d as t3d #
+ä¸¤ç§å¼å¥æ¹å¼é½å¯ä»¥ ``` å­æ¨¡å: [tools_3d.py](./tkintertools/
+tools_3d.py)
+ç®å3dç»å¾åè½è¿æ¯è¾ç®éï¼ä»è½ç»å¶ç¹ãçº¿ãé¢ä»¥åç´è¾¹çç©ºé´å ä½ä½ï¼å¯¹äºæ²è¾¹çç©ºé´å ä½ä½è¿å¨å¼åä¸­ï¼
+ä»¥ä¸æ¯ä¸ä¸ªä½¿ç¨3dç»å¾çç¤ºä¾ï¼
+å¨è¿ä¸ªç¤ºä¾ä¸­ï¼æä½é¼ æ å·¦é®å¯ä»¥æè½¬å ä½ä½ï¼æä½é¼ æ å³é®å¯ä»¥å¹³ç§»å ä½ä½ï¼æ»å¨é¼ æ æ»è½®å¯ä»¥ç¼©æ¾å ä½ä½ï¼
+xãy å z è½´åå«æ¯çº¢è²ãç»¿è²åèè²ççº¿ã ![3dç»å¾](./docs/
+images/3d.png) æºä»£ç  ```python import random import tkinter import
+tkintertools as tkt from tkintertools import tools_3d as t3d root = tkt.Tk
+('tools_3d', 1280, 720) canvas = t3d.Canvas_3D(root, 1280, 720, 0, 0) geos = []
+# type: list[t3d.Geometry] origin = t3d.Point(canvas, [0, 0, 0], size=5) #
+åç¹ axes = [t3d.Line(canvas, [0, 0, 0], [100, 0, 0], width=3, fill='red'), #
+åå»ºåæ è½´ t3d.Line(canvas, [0, 0, 0], [0, 100, 0], width=3,
+fill='green'), t3d.Line(canvas, [0, 0, 0], [0, 0, -100], width=3, fill='blue')]
+for _ in range(8): # åå»ºæ­£æ¹ä½ cube = t3d.Cuboid( canvas, *random.sample
+(range(-200, 200), 3), *random.sample(range(50, 100), 3)) geos.append(cube) #
+åå»ºåé¢ä½ x, y, z = random.sample(range(-200, 200), 3) tetr =
+t3d.Tetrahedron( canvas, *[[x+random.randint(-100, 100), y+random.randint(-100,
+100), z+random.randint(-100, 100)] for _ in range(4)]) geos.append(tetr) def
+translate(event, flag=False, _cache=[]): # type: (tkinter.Event, bool, list
+[float]) -> None """ å¹³ç§»äºä»¶ """ if flag: _cache[:] = [event.x, event.y]
+return dx = (event.x - _cache[0]) / 6 dy = (event.y - _cache[1]) / 6 _cache[:
+] = [event.x, event.y] for axis in axes: axis.translate(0, 6*dx, 6*dy)
+axis.update() for geo in geos: geo.translate(0, dx, dy) geo.update()
+origin.translate(0, 6*dx, 6*dy) origin.update() def rotate(event, flag=False,
+_cache=[]): # type: (tkinter.Event, bool, list[float]) -> None """ æè½¬äºä»¶
+""" if flag: _cache[:] = [event.x, event.y] return dy = (event.x - _cache[0]) /
+200 dx = (_cache[1] - event.y) / 200 _cache[:] = [event.x, event.y] for axis in
+axes: axis.rotate(0, 6*dx, 6*dy, center=origin.coords) axis.update() for geo in
+geos: geo.rotate(0, dx, dy, center=origin.coords) geo.update() def scale
+(event): # type: (tkinter.Event) -> None """ ç¼©æ¾äºä»¶ """ k = 1.01 if
+event.delta > 0 else 0.99 for geo in geos: geo.scale(k, k, k) geo.update()
+root.bind('', lambda event: rotate(event, True)) root.bind('', rotate)
+root.bind('', lambda event: translate(event, True)) root.bind('', translate)
+root.bind('', scale) root.mainloop() ```  æ´å¤æ´æ°ä¿¡æ¯è¯·è§ï¼
+[CHANGELOG.md](./CHANGELOG.md) Description/æ¨¡åè¯´æ ---------------------
+- tkintertools æ¯ä¸æ¬¾åºäº tkinter
 æ¨¡åçäºæ¬¡å¼åççé¢ç¼ç¨æ¨¡åï¼å®å®å¨æ²¡æä½¿ç¨ä»»ä½ç¬¬ä¸æ¹æ¨¡åååºçï¼åæ¶ï¼å®ä¹æ²¡æä»»ä½ä¾èµåï¼å®çåè½å®å¨ç±åç½®æ¨¡ååå½æ°å®ç°ï¼èä¸ï¼å®è¿æ¯è·¨å¹³å°çï¼å®å
 tkinter æå¤§çä¸åå¨äºï¼å®çæ§ä»¶å¹¶éçå®çæ§ä»¶ï¼èæ¯å¨
 tkinter æ¨¡åä¸­ Canvas å¯¹è±¡ä¸­ç»å¶èæçï¼è¿å°±èµäºäº
 tkintertools æ§ä»¶ä¸äºå¨ tkinter ä¸­æ²¡æçç¹æ§ï¼åä¸¾å¦ä¸ï¼ *
 æ§ä»¶èæ¯å¯ä»¥æ¯éæçï¼å®éä¸æ¯æ²¡æèæ¯é¢è²ï¼ *
 æ§ä»¶çæ ·å¼å¯ä»¥æ¯èªå®ä¹çï¼æ¯å¦æé®æåè§ï¼ *
 æ§ä»¶çåå»ºéåº¦è¿å¤§äº tkinter çæ§ä»¶ï¼é¤äº Canvas æ§ä»¶ï¼
@@ -255,11 +288,11 @@
 ### ç®æç»å½çé¢ * æç« é¾æ¥: ææ  * ä»£ç ä»åº: https://
 gitcode.net/weixin_62651706/tester * ç¨åºä¸è½½: ææ  * æ¨èææ°:
 ððð è¿ä¸ªæ¡ä¾ä½¿ç¨äºææ°ç¨³å®çç tkintertools-
 v2.6.0ï¼çé¢éå¸¸ç¨³å®ï¼å ä¹æ²¡æ bugï¼å®å¨éç¨ tkintertools
 çæ§ä»¶ï¼é¢å¼å¾é«ï¼çé¢éå¸¸æµçãä½ç°äº tkintertools
 æ¨¡åä¸ tkinter æ¨¡åç¸æ¯å¨æ§è½ä¸çä¼è¶æ§ï¼ ![exam3_1.png](docs/
 examples/exam3_1.png) ![exam3_2.png](docs/examples/exam3_2.png) More/æ´å¤ ---
------- > GitCode: > https://gitcode.net/weixin_62651706/tkintertools > GitHub
-(Mirror/éå): > https://github.com/XiaoKang2022-CSDN/tkintertools > Column/
-ä¸æ : > https://blog.csdn.net/weixin_62651706/category_11600888.html
+------ > GitHub: > https://github.com/Xiaokang2022/tkintertools > GitCode
+(Mirror/éå): > https://gitcode.net/weixin_62651706/tkintertools > Gitee
+(Mirror/éå): > https://gitee.com/xiaokang-2022/tkintertools
 è¿ææ´å¤åå®¹è¯·å¨ [æºä»£ç ](./tkintertools/) ä¸­æ¢ç´¢ï¼
```

### Comparing `tkintertools-dev-2.6.2/README.md` & `tkintertools-dev-2.6.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,75 +1,198 @@
+Metadata-Version: 2.1
+Name: tkintertools-dev
+Version: 2.6.3
+Summary: An auxiliary module of the tkinder module
+Home-page: https://github.com/Xiaokang2022/tkintertools
+Author: Xiaokang2022
+Author-email: 2951256653@qq.com
+License: MulanPSL-2.0
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <div align="center">
     <h1>🚀tkintertools🚀</h1>
     <p><img height="120px" alt="logo.png"
-        src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/tkintertools.png" />
+        src="./tkintertools.png" />
     </p>
     <p>The <code>tkintertools</code> module is an auxiliary module of the <code>tkinter</code> module</p>
     <p><code>tkintertools</code> 模块是 <code>tkinter</code> 模块的辅助模块</p>
     <p>
         <a href="./tkintertools/__init__.py">
-            <img src="https://img.shields.io/badge/Version-2.6.1-blue" alt="latest version" />
+            <img src="https://img.shields.io/badge/Version-2.6.2-blue" alt="latest version" />
         </a>
         <a href="./LICENSE">
             <img src="https://img.shields.io/badge/License-Mulan PSL v2-green" alt="License" />
         </a>
         <a href="./CHANGELOG.md">
-            <img src="https://img.shields.io/badge/ChangeLog-2023/05/26-orange" alt="ChangeLog" />
+            <img src="https://img.shields.io/badge/ChangeLog-2023/06/06-orange" alt="ChangeLog" />
         </a>
         <a href="./TODO.md">
-            <img src="https://img.shields.io/badge/ToDos-10-yellow" alt="ToDos" />
+            <img src="https://img.shields.io/badge/ToDos-13-yellow" alt="ToDos" />
         </a>
         <a href="https://pypistats.org/packages/tkintertools">
             <img src="https://img.shields.io/badge/Downloads-3k-purple" alt="Downloads" />
         </a>
     </p>
     <p>
         <a href="mailto:2951256653@qq.com">
             <img src="https://img.shields.io/badge/Email-2951256653@qq.com-cyan" alt="Email" />
         </a>
         <a href="https://xiaokang2022.blog.csdn.net">
             <img src="https://img.shields.io/badge/Blog-小康2022@CSDN-red" alt="Blog" />
         </a>
-        <a href="https://gitcode.net/weixin_62651706">
+        <a href="https://github.com/Xiaokang2022">
             <img src="https://img.shields.io/badge/Author-小康2022-white" alt="Author" />
         </a>
     </p>
 </div>
 
 Installation/模块安装
 -----------------------
 
 ### Stable version/稳定版本
 
-* Version/版本 : 2.6.1
-* Release Date/发布日期 : 2023/05/21
+* Version/版本 : 2.6.2
+* Release Date/发布日期 : 2023/05/30
 
 ```
-pip install tkintertools==2.6.1
+pip install tkintertools==2.6.2
 ```
 或者
 ```
 pip install tkintertools
 ```
 
-这个是目前的最新版，比较稳定，bug 没有那么多，推荐使用这个。  
+这个是目前的最新稳定版，比较稳定，bug 没有那么多，推荐使用这个。  
 稳定版有文档可以查看，有 issue 我会去查看并尝试解决 issue。
 
 ### Development version/开发版本
 
-* Version/版本 : 2.6.2
-* Release Date/发布日期 : 2023/05/26
+* Version/版本 : 2.6.3
+* Release Date/发布日期 : 2023/06/06
 
 ```
-pip install tkintertools-dev==2.6.2
+pip install tkintertools-dev==2.6.3
 ```
 
-这个是作者正在开发的版本，有新功能，但不能保证稳定，bug 可能会比较多。  
+这个是我正在开发的版本，有新功能，但不能保证稳定，bug 可能会比较多。  
 开发版本没有对应的文档，大家可以在 issue 中提出建议，我会适当采纳一些并在开发版本中更改或实现。
 
+News/最新功能
+------------
+
+最新版的`tkintertools`为`2.6.2`，新增一项极为强大的功能：3d绘图！  
+同时修复一些bug，优化了一部分代码，提升了一部分性能。
+
+通过以下代码来使用3d绘图功能：
+
+```python
+from tkintertools import tools_3d as t3d
+import tkintertools.tools_3d as t3d
+# 两种引入方式都可以
+```
+
+子模块: [tools_3d.py](./tkintertools/tools_3d.py)
+
+目前3d绘图功能还比较简陋，仅能绘制点、线、面以及直边的空间几何体，对于曲边的空间几何体还在开发中！  
+以下是一个使用3d绘图的示例：
+
+在这个示例中，按住鼠标左键可以旋转几何体，按住鼠标右键可以平移几何体，滚动鼠标滚轮可以缩放几何体！  
+x、y 和 z 轴分别是红色、绿色和蓝色的线。
+
+![3d绘图](./docs/images/3d.png)
+
+<details><summary><b>源代码</b></summary>
+
+```python
+import random
+import tkinter
+
+import tkintertools as tkt
+from tkintertools import tools_3d as t3d
+
+root = tkt.Tk('tools_3d', 1280, 720)
+canvas = t3d.Canvas_3D(root, 1280, 720, 0, 0)
+
+geos = []  # type: list[t3d.Geometry]
+origin = t3d.Point(canvas, [0, 0, 0], size=5)  # 原点
+axes = [t3d.Line(canvas, [0, 0, 0], [100, 0, 0], width=3, fill='red'),  # 创建坐标轴
+        t3d.Line(canvas, [0, 0, 0], [0, 100, 0], width=3, fill='green'),
+        t3d.Line(canvas, [0, 0, 0], [0, 0, -100], width=3, fill='blue')]
+
+for _ in range(8):
+    # 创建正方体
+    cube = t3d.Cuboid(
+        canvas, *random.sample(range(-200, 200), 3), *random.sample(range(50, 100), 3))
+    geos.append(cube)
+    # 创建四面体
+    x, y, z = random.sample(range(-200, 200), 3)
+    tetr = t3d.Tetrahedron(
+        canvas, *[[x+random.randint(-100, 100), y+random.randint(-100, 100), z+random.randint(-100, 100)] for _ in range(4)])
+    geos.append(tetr)
+
+
+def translate(event, flag=False, _cache=[]):
+    # type: (tkinter.Event, bool, list[float]) -> None
+    """ 平移事件 """
+    if flag:
+        _cache[:] = [event.x, event.y]
+        return
+    dx = (event.x - _cache[0]) / 6
+    dy = (event.y - _cache[1]) / 6
+    _cache[:] = [event.x, event.y]
+    for axis in axes:
+        axis.translate(0, 6*dx, 6*dy)
+        axis.update()
+    for geo in geos:
+        geo.translate(0, dx, dy)
+        geo.update()
+    origin.translate(0, 6*dx, 6*dy)
+    origin.update()
+
+
+def rotate(event, flag=False, _cache=[]):  # type: (tkinter.Event, bool, list[float]) -> None
+    """ 旋转事件 """
+    if flag:
+        _cache[:] = [event.x, event.y]
+        return
+    dy = (event.x - _cache[0]) / 200
+    dx = (_cache[1] - event.y) / 200
+    _cache[:] = [event.x, event.y]
+    for axis in axes:
+        axis.rotate(0, 6*dx, 6*dy, center=origin.coords)
+        axis.update()
+    for geo in geos:
+        geo.rotate(0, dx, dy, center=origin.coords)
+        geo.update()
+
+
+def scale(event):  # type: (tkinter.Event) -> None
+    """ 缩放事件 """
+    k = 1.01 if event.delta > 0 else 0.99
+    for geo in geos:
+        geo.scale(k, k, k)
+        geo.update()
+
+
+root.bind('<Button-1>', lambda event: rotate(event, True))
+root.bind('<B1-Motion>', rotate)
+root.bind('<Button-3>', lambda event: translate(event, True))
+root.bind('<B3-Motion>', translate)
+root.bind('<MouseWheel>', scale)
+root.mainloop()
+```
+
+</details>
+
+更多更新信息请见：[CHANGELOG.md](./CHANGELOG.md)
+
 Description/模块说明
 ----------------------
 
 tkintertools 是一款基于 tkinter 模块的二次开发的界面编程模块，它完全没有使用任何第三方模块和库的，同时，它也没有任何依赖包，它的功能完全由内置模块和函数实现，而且，它还是跨平台的！它和 tkinter 最大的不同在于，它的控件并非真实的控件，而是在 tkinter 模块中 Canvas 对象中绘制而成的，这就赋予了 tkintertools 控件一些在 tkinter 中没有的特性，列举如下：
 
 * 控件背景可以是透明的（实际上是没有背景颜色）
 * 控件的样式可以是自定义的（比如按钮有圆角）
@@ -566,17 +689,17 @@
 
 ![exam3_1.png](docs/examples/exam3_1.png)
 ![exam3_2.png](docs/examples/exam3_2.png)
 
 More/更多
 ---------
 
-> GitCode:  
-> https://gitcode.net/weixin_62651706/tkintertools
+> GitHub:  
+> https://github.com/Xiaokang2022/tkintertools
 
-> GitHub(Mirror/镜像):  
-> https://github.com/XiaoKang2022-CSDN/tkintertools
+> GitCode(Mirror/镜像):  
+> https://gitcode.net/weixin_62651706/tkintertools
 
-> Column/专栏:  
-> https://blog.csdn.net/weixin_62651706/category_11600888.html
+> Gitee(Mirror/镜像):  
+> https://gitee.com/xiaokang-2022/tkintertools
 
 还有更多内容请在 [源代码](./tkintertools/) 中探索！
```

#### html2text {}

```diff
@@ -1,26 +1,73 @@
+Metadata-Version: 2.1 Name: tkintertools-dev Version: 2.6.3 Summary: An
+auxiliary module of the tkinder module Home-page: https://github.com/
+Xiaokang2022/tkintertools Author: Xiaokang2022 Author-email: 2951256653@qq.com
+License: MulanPSL-2.0 Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Mulan Permissive Software License v2
+(MulanPSL-2.0) Classifier: Operating System :: OS Independent Description-
+Content-Type: text/markdown License-File: LICENSE
                       ****** ðtkintertoolsð ******
                                   [logo.png]
      The tkintertools module is an auxiliary module of the tkinter module
              tkintertools æ¨¡åæ¯ tkinter æ¨¡åçè¾å©æ¨¡å
           [latest_version] [License] [ChangeLog] [ToDos] [Downloads]
                             [Email] [Blog] [Author]
 Installation/æ¨¡åå®è£ ----------------------- ### Stable version/
-ç¨³å®çæ¬ * Version/çæ¬ : 2.6.1 * Release Date/åå¸æ¥æ : 2023/05/21
-``` pip install tkintertools==2.6.1 ``` æè ``` pip install tkintertools ```
-è¿ä¸ªæ¯ç®åçææ°çï¼æ¯è¾ç¨³å®ï¼bug
+ç¨³å®çæ¬ * Version/çæ¬ : 2.6.2 * Release Date/åå¸æ¥æ : 2023/05/30
+``` pip install tkintertools==2.6.2 ``` æè ``` pip install tkintertools ```
+è¿ä¸ªæ¯ç®åçææ°ç¨³å®çï¼æ¯è¾ç¨³å®ï¼bug
 æ²¡æé£ä¹å¤ï¼æ¨èä½¿ç¨è¿ä¸ªã ç¨³å®çæææ¡£å¯ä»¥æ¥çï¼æ
 issue æä¼å»æ¥çå¹¶å°è¯è§£å³ issueã ### Development version/
-å¼åçæ¬ * Version/çæ¬ : 2.6.2 * Release Date/åå¸æ¥æ : 2023/05/26
-``` pip install tkintertools-dev==2.6.2 ```
-è¿ä¸ªæ¯ä½èæ­£å¨å¼åççæ¬ï¼ææ°åè½ï¼ä½ä¸è½ä¿è¯ç¨³å®ï¼bug
+å¼åçæ¬ * Version/çæ¬ : 2.6.3 * Release Date/åå¸æ¥æ : 2023/06/06
+``` pip install tkintertools-dev==2.6.3 ```
+è¿ä¸ªæ¯ææ­£å¨å¼åççæ¬ï¼ææ°åè½ï¼ä½ä¸è½ä¿è¯ç¨³å®ï¼bug
 å¯è½ä¼æ¯è¾å¤ã å¼åçæ¬æ²¡æå¯¹åºçææ¡£ï¼å¤§å®¶å¯ä»¥å¨ issue
 ä¸­æåºå»ºè®®ï¼æä¼éå½éçº³ä¸äºå¹¶å¨å¼åçæ¬ä¸­æ´æ¹æå®ç°ã
-Description/æ¨¡åè¯´æ ---------------------- tkintertools æ¯ä¸æ¬¾åºäº
-tkinter
+News/ææ°åè½ -----------
+-
+ææ°çç`tkintertools`ä¸º`2.6.2`ï¼æ°å¢ä¸é¡¹æä¸ºå¼ºå¤§çåè½ï¼3dç»å¾ï¼
+åæ¶ä¿®å¤ä¸äºbugï¼ä¼åäºä¸é¨åä»£ç ï¼æåäºä¸é¨åæ§è½ã
+éè¿ä»¥ä¸ä»£ç æ¥ä½¿ç¨3dç»å¾åè½ï¼ ```python from tkintertools import
+tools_3d as t3d import tkintertools.tools_3d as t3d #
+ä¸¤ç§å¼å¥æ¹å¼é½å¯ä»¥ ``` å­æ¨¡å: [tools_3d.py](./tkintertools/
+tools_3d.py)
+ç®å3dç»å¾åè½è¿æ¯è¾ç®éï¼ä»è½ç»å¶ç¹ãçº¿ãé¢ä»¥åç´è¾¹çç©ºé´å ä½ä½ï¼å¯¹äºæ²è¾¹çç©ºé´å ä½ä½è¿å¨å¼åä¸­ï¼
+ä»¥ä¸æ¯ä¸ä¸ªä½¿ç¨3dç»å¾çç¤ºä¾ï¼
+å¨è¿ä¸ªç¤ºä¾ä¸­ï¼æä½é¼ æ å·¦é®å¯ä»¥æè½¬å ä½ä½ï¼æä½é¼ æ å³é®å¯ä»¥å¹³ç§»å ä½ä½ï¼æ»å¨é¼ æ æ»è½®å¯ä»¥ç¼©æ¾å ä½ä½ï¼
+xãy å z è½´åå«æ¯çº¢è²ãç»¿è²åèè²ççº¿ã ![3dç»å¾](./docs/
+images/3d.png) æºä»£ç  ```python import random import tkinter import
+tkintertools as tkt from tkintertools import tools_3d as t3d root = tkt.Tk
+('tools_3d', 1280, 720) canvas = t3d.Canvas_3D(root, 1280, 720, 0, 0) geos = []
+# type: list[t3d.Geometry] origin = t3d.Point(canvas, [0, 0, 0], size=5) #
+åç¹ axes = [t3d.Line(canvas, [0, 0, 0], [100, 0, 0], width=3, fill='red'), #
+åå»ºåæ è½´ t3d.Line(canvas, [0, 0, 0], [0, 100, 0], width=3,
+fill='green'), t3d.Line(canvas, [0, 0, 0], [0, 0, -100], width=3, fill='blue')]
+for _ in range(8): # åå»ºæ­£æ¹ä½ cube = t3d.Cuboid( canvas, *random.sample
+(range(-200, 200), 3), *random.sample(range(50, 100), 3)) geos.append(cube) #
+åå»ºåé¢ä½ x, y, z = random.sample(range(-200, 200), 3) tetr =
+t3d.Tetrahedron( canvas, *[[x+random.randint(-100, 100), y+random.randint(-100,
+100), z+random.randint(-100, 100)] for _ in range(4)]) geos.append(tetr) def
+translate(event, flag=False, _cache=[]): # type: (tkinter.Event, bool, list
+[float]) -> None """ å¹³ç§»äºä»¶ """ if flag: _cache[:] = [event.x, event.y]
+return dx = (event.x - _cache[0]) / 6 dy = (event.y - _cache[1]) / 6 _cache[:
+] = [event.x, event.y] for axis in axes: axis.translate(0, 6*dx, 6*dy)
+axis.update() for geo in geos: geo.translate(0, dx, dy) geo.update()
+origin.translate(0, 6*dx, 6*dy) origin.update() def rotate(event, flag=False,
+_cache=[]): # type: (tkinter.Event, bool, list[float]) -> None """ æè½¬äºä»¶
+""" if flag: _cache[:] = [event.x, event.y] return dy = (event.x - _cache[0]) /
+200 dx = (_cache[1] - event.y) / 200 _cache[:] = [event.x, event.y] for axis in
+axes: axis.rotate(0, 6*dx, 6*dy, center=origin.coords) axis.update() for geo in
+geos: geo.rotate(0, dx, dy, center=origin.coords) geo.update() def scale
+(event): # type: (tkinter.Event) -> None """ ç¼©æ¾äºä»¶ """ k = 1.01 if
+event.delta > 0 else 0.99 for geo in geos: geo.scale(k, k, k) geo.update()
+root.bind('', lambda event: rotate(event, True)) root.bind('', rotate)
+root.bind('', lambda event: translate(event, True)) root.bind('', translate)
+root.bind('', scale) root.mainloop() ```  æ´å¤æ´æ°ä¿¡æ¯è¯·è§ï¼
+[CHANGELOG.md](./CHANGELOG.md) Description/æ¨¡åè¯´æ ---------------------
+- tkintertools æ¯ä¸æ¬¾åºäº tkinter
 æ¨¡åçäºæ¬¡å¼åççé¢ç¼ç¨æ¨¡åï¼å®å®å¨æ²¡æä½¿ç¨ä»»ä½ç¬¬ä¸æ¹æ¨¡åååºçï¼åæ¶ï¼å®ä¹æ²¡æä»»ä½ä¾èµåï¼å®çåè½å®å¨ç±åç½®æ¨¡ååå½æ°å®ç°ï¼èä¸ï¼å®è¿æ¯è·¨å¹³å°çï¼å®å
 tkinter æå¤§çä¸åå¨äºï¼å®çæ§ä»¶å¹¶éçå®çæ§ä»¶ï¼èæ¯å¨
 tkinter æ¨¡åä¸­ Canvas å¯¹è±¡ä¸­ç»å¶èæçï¼è¿å°±èµäºäº
 tkintertools æ§ä»¶ä¸äºå¨ tkinter ä¸­æ²¡æçç¹æ§ï¼åä¸¾å¦ä¸ï¼ *
 æ§ä»¶èæ¯å¯ä»¥æ¯éæçï¼å®éä¸æ¯æ²¡æèæ¯é¢è²ï¼ *
 æ§ä»¶çæ ·å¼å¯ä»¥æ¯èªå®ä¹çï¼æ¯å¦æé®æåè§ï¼ *
 æ§ä»¶çåå»ºéåº¦è¿å¤§äº tkinter çæ§ä»¶ï¼é¤äº Canvas æ§ä»¶ï¼
@@ -248,11 +295,11 @@
 ### ç®æç»å½çé¢ * æç« é¾æ¥: ææ  * ä»£ç ä»åº: https://
 gitcode.net/weixin_62651706/tester * ç¨åºä¸è½½: ææ  * æ¨èææ°:
 ððð è¿ä¸ªæ¡ä¾ä½¿ç¨äºææ°ç¨³å®çç tkintertools-
 v2.6.0ï¼çé¢éå¸¸ç¨³å®ï¼å ä¹æ²¡æ bugï¼å®å¨éç¨ tkintertools
 çæ§ä»¶ï¼é¢å¼å¾é«ï¼çé¢éå¸¸æµçãä½ç°äº tkintertools
 æ¨¡åä¸ tkinter æ¨¡åç¸æ¯å¨æ§è½ä¸çä¼è¶æ§ï¼ ![exam3_1.png](docs/
 examples/exam3_1.png) ![exam3_2.png](docs/examples/exam3_2.png) More/æ´å¤ ---
------- > GitCode: > https://gitcode.net/weixin_62651706/tkintertools > GitHub
-(Mirror/éå): > https://github.com/XiaoKang2022-CSDN/tkintertools > Column/
-ä¸æ : > https://blog.csdn.net/weixin_62651706/category_11600888.html
+------ > GitHub: > https://github.com/Xiaokang2022/tkintertools > GitCode
+(Mirror/éå): > https://gitcode.net/weixin_62651706/tkintertools > Gitee
+(Mirror/éå): > https://gitee.com/xiaokang-2022/tkintertools
 è¿ææ´å¤åå®¹è¯·å¨ [æºä»£ç ](./tkintertools/) ä¸­æ¢ç´¢ï¼
```

### Comparing `tkintertools-dev-2.6.2/setup.py` & `tkintertools-dev-2.6.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 """ 上传 pypi """
 
 import setuptools
 
 
 setuptools.setup(
     name='tkintertools-dev',
-    version="2.6.2",
+    version="2.6.3",
     author='Xiaokang2022',
     license='MulanPSL-2.0',
     author_email='2951256653@qq.com',
     description='An auxiliary module of the tkinder module',
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
-    url='https://gitcode.net/weixin_62651706/tkintertools',
+    url='https://github.com/Xiaokang2022/tkintertools',
     packages=setuptools.find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)',
         'Operating System :: OS Independent',
     ],
 )
 
 # python -m pip install --user --upgrade setuptools wheel [检查更新]
 
 # python setup.py sdist bdist_wheel [打包]
-# twine upload dist/* [上传]
+# python -m twine upload dist/* [上传]
 
 # pip install -U pypistats [数据分析]
 # pip install socksio [数据分析]
 
 # pypistats overall tkintertools [数据分析]
 # pypistats recent tkintertools
 # pypistats system tkintertools
```

### Comparing `tkintertools-dev-2.6.2/tkintertools/__main__.py` & `tkintertools-dev-2.6.3/tkintertools/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,15 +222,17 @@
         `rate_y`: 纵向缩放比率，默认值同上\n
         """
         if not rate_x:
             rate_x = self.master.width[1]/self.master.width[0]/self.rx
         if not rate_y:
             rate_y = self.master.height[1]/self.master.height[0]/self.ry
 
-        if self.keep:  # 维持比例
+        rate_x_pos, rate_y_pos = rate_x, rate_y  # 避免受 keep 影响
+
+        if self.keep is True:  # 维持比例
             rx = rate_x*self.master.width[1]/self.master.width[0]/self.rx
             ry = rate_y*self.master.height[1]/self.master.height[0]/self.ry
             rate_x = rate_y = min(rx, ry)
 
         # 更新画布的位置及大小的数据
         self.width[1] *= rate_x
         self.height[1] *= rate_y
@@ -238,16 +240,16 @@
         temp_y, self.ry = self.ry, self.height[1]/self.height[0]
 
         place_info = self.place_info()
         tkinter.Canvas.place(  # 更新画布的位置及大小
             self,
             width=self.width[1],
             height=self.height[1],
-            x=float(place_info['x'])*rate_x,
-            y=float(place_info['y'])*rate_y)
+            x=float(place_info['x'])*rate_x_pos,
+            y=float(place_info['y'])*rate_y_pos)
 
         for widget in self._widget:  # 更新子画布控件的子虚拟画布控件位置数据
             widget.x1 *= rate_x
             widget.x2 *= rate_x
             widget.y1 *= rate_y
             widget.y2 *= rate_y
```

### Comparing `tkintertools-dev-2.6.2/tkintertools/constants.py` & `tkintertools-dev-2.6.3/tkintertools/constants.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,56 +1,97 @@
 """ All constants """
 
-import sys
+import platform
+
+SYSTEM = platform.system()
+""" Operating System """
 
 PROCESS_SYSTEM_DPI_AWARE = 1
-""" default DPI aware """
+""" Default DPI aware """
 
 
 COLOR_BUTTON_FILL = '#E1E1E1', '#E5F1FB', '#CCE4F7', '#E0E0E0'
-""" default button fill color """
+""" Default button fill color """
 
 COLOR_BUTTON_OUTLINE = '#C0C0C0', '#288CDB', '#4884B4', '#D0D0D0'
-""" default button outline color """
+""" Default button outline color """
 
 COLOR_TEXT_FILL = '#FFFFFF', '#FFFFFF', '#FFFFFF', '#E0E0E0'
-""" default text widget fill color """
+""" Default text widget fill color """
 
 COLOR_TEXT_OUTLINE = '#C0C0C0', '#414141', '#288CDB', '#D0D0D0'
-""" default text widget outline color """
+""" Default text widget outline color """
 
 COLOR_TEXT = '#000000', '#000000', '#000000', '#A3A3A3'
-""" default text color """
+""" Default text color """
 
 COLOR_NONE = '', '', '', ''
-""" default transparent color tuple """
+""" Default transparent color tuple """
 
 COLOR_BAR = '#E1E1E1', '#06b025'
-""" default progress bar color """
+""" Default progress bar color """
 
 BACKGROUND = '#F1F1F1'
-""" default Canvas background color """
+""" Default Canvas background color """
 
 
 BORDERWIDTH = 1
-""" default widget borderwidth """
+""" Default widget borderwidth """
 
 CURSOR = '│'
 """ text cursor """
 
-FONT = 'Microsoft YaHei' if sys.platform == 'win32' else 'DejaVu Sans' if sys.platform == 'linux' else 'Arial'
-""" default font """
+FONT = 'Microsoft YaHei' if SYSTEM == 'Windows' else 'DejaVu Sans' if SYSTEM == 'linux' else 'Arial'
+""" Default font """
 
 SIZE = 20
-""" default font size """
+""" Default font size """
 
 LIMIT = -1
-""" default widget text length limit """
+""" Default widget text length limit """
 
-RADIUS = 0
-""" default widget fillet radius """
+RADIUS = 0 if SYSTEM == 'Windows' and int(
+    platform.version()[-5:]) < 22000 else 4
+""" Default widget fillet radius """
 
 FRAMES = 60
-""" default move frame rate """
+""" Default move frame rate """
 
 TICK = '✓'
-""" default checkbox symbol """
+""" Default checkbox symbol """
+
+
+CFG_3D = 500, None, None
+""" Default 3D configuration """
+
+
+COLOR_POINT_FILL = '#000000'
+""" Default point fill color """
+
+COLOR_POINT_OUTLINE = '#000000'
+""" Default point outline color """
+
+COLOR_LINE_FILL = '#000000'
+""" Default line fill color """
+
+COLOR_SIDE_FILL = ''
+""" Default side fill color """
+
+COLOR_SIDE_OUTLINE = '#000000'
+""" Default side outline color """
+
+POINT_SIZE = 1
+""" Default point size """
+
+POINT_WIDTH = 1
+""" Default point width """
+
+LINE_WDITH = 1
+""" Default line width """
+
+SIDE_WIDTH = 1
+""" Default side width """
+
+
+if __name__ == '__main__':
+    print(', '.join(name for name in globals()
+          if '__' not in name and name.isupper()))
```

### Comparing `tkintertools-dev-2.6.2/tkintertools/tools_3d.py` & `tkintertools-dev-2.6.3/tkintertools/tools_3d.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,198 +1,363 @@
 """ 3D support """
 
 import math  # 数学支持
 import statistics  # 数据统计
-import tkinter  # 基础模块
 from typing import Iterable  # 类型提示
 
-import tkintertools  # 类型提示
+from .__main__ import Canvas, Tk, Toplevel  # 继承和类型提示
+from .constants import *
 
 
-def _cross(
-    matrix,  # type: list[list[float]]
-    vector,  # type: list[float]
-):  # type: (...) -> list[float]
-    """ 转换矩阵 """
-    for i in range(3):
-        matrix[0][i] = sum(matrix[i][j]*vector[j] for j in range(3))
-    return matrix[0]
+class Canvas_3D(Canvas):
+    """ 3D画布，支持3d绘图 """
 
+    def __init__(
+        self,
+        master,  # type: Tk | Toplevel
+        width,  # type: int
+        height,  # type: int
+        x=None,  # type: int | None
+        y=None,  # type: int | None
+        *,
+        lock=True,  # type: bool
+        expand=True,  # type: bool
+        keep=True,  # type: bool
+        cfg_3d=CFG_3D,  # type: Iterable[float, float | None, float | None]
+        **kw
+    ):  # type: (...) -> None
+        """
+        `master`: 父控件\n
+        `width`: 画布宽度\n
+        `height`: 画布高度\n
+        `x`: 画布左上角的横坐标\n
+        `y`: 画布左上角的纵坐标\n
+        `lock`: 画布内控件的功能锁，False 时功能暂时失效\n
+        `expand`: 画布内控件是否能缩放\n
+        `keep`: 画布比例是否保持不变\n
+        `cfg_3d`: 3d绘图的配置，一个包含三个值的列表，[相机距离，横坐标偏移，纵坐标偏移]，默认值相机距离500，图像居中\n
+        `**kw`: 与 tkinter.Canvas 类的参数相同\n
+        """
+        Canvas.__init__(self, master, width, height, x, y,
+                        lock=lock, expand=expand, keep=keep)
+        self.distance = cfg_3d[0]
+        self.dx = width / 2 if cfg_3d[1] is None else cfg_3d[1]
+        self.dy = height / 2 if cfg_3d[2] is None else cfg_3d[2]
+        self._items_3d = []  # type: list[Point | Line | Side | Geometry]
+
+    def items_3d(self):  # type: () -> tuple[Point | Line | Side | Geometry]
+        """ 返回`Canvas_3d`类的`items_3d`元组 """
+        return tuple(self._items_3d)
 
-class Point:
+
+class _Point:
     """ 点 """
 
     def __init__(self, coords):  # type: (list[float]) -> None
-        self.coords = list(coords)  # 利用列表引用
+        self.coords = coords  # 利用列表引用
 
-    def translate(self, dx=0, dy=0, dz=0):  # type: (float, float, float) -> Point
+    def translate(self, dx=0, dy=0, dz=0):  # type: (float, float, float) -> None
         """ 平移 """
         self.coords[0] += dx
         self.coords[1] += dy
         self.coords[2] += dz
-        return self
 
-    def rotate(self, dx=0, dy=0, dz=0):  # type: (float, float, float) -> Point
+    def rotate(self, dx=1, dy=1, dz=1, *, center=[0, 0, 0]):
+        # type: (float, float, float, ..., Iterable[float]) -> None
         """ 旋转 """
-        sa, sb, sc = math.sin(dx), math.sin(dy), math.sin(dz)
-        ca, cb, cc = math.cos(dx), math.cos(dy), math.cos(dz)
-        M = [[cc*cb, cc*sb*sa-sc*ca, cc*sb*ca+sc*sa],
-             [sc*cb, sc*sb*sa+cc*ca, sc*sb*ca-cc*sa],
-             [-sb,   cb*sa,          cb*ca]]
-        self.coords[0], self.coords[1], self.coords[2] = _cross(M, self.coords)
-        return self
+        sx, sy, sz = math.sin(dx), math.sin(dy), math.sin(dz)
+        cx, cy, cz = math.cos(dx), math.cos(dy), math.cos(dz)
+
+        matrix = [[cz*cy, cz*sy*sx-sz*cx, cz*sy*cx+sz*sx],
+                  [sz*cy, sz*sy*sx+cz*cx, sz*sy*cx-cz*sx],
+                  [-sy,   cy*sx,          cy*cx]]
+
+        for i in range(3):
+            matrix[0][i] = center[i] + \
+                sum(matrix[i][j]*(self.coords[j]-center[j]) for j in range(3))
+
+        self.coords[:] = matrix[0]
+
+    def scale(self, kx=1, ky=1, kz=1, *, center=None):
+        # type: (float, float, float, ..., Iterable[float] | None) -> None
+        """ 缩放 """
+        for i, k in zip(range(3), (kx, ky, kz)):
+            self.coords[i] += (self.coords[i] - center[i]) * (k - 1)
 
     def project(self, distance):  # type: (float) -> list[float]
         """ 投影 """
         try:
-            coefficient = distance/(distance - self.coords[0])
-        except:
+            k = distance/(distance - self.coords[0])
+        except ZeroDivisionError:
             return [distance, distance]
-        return [self.coords[1]*coefficient, self.coords[2]*coefficient]
+        return [self.coords[1]*k, self.coords[2]*k]
 
 
-class Line:
+class _Line:
     """ 线 """
 
     def __init__(
         self,
-        x1,  # type: float
-        y1,  # type: float
-        z1,  # type: float
-        x2,  # type: float
-        y2,  # type: float
-        z2,  # type: float
+        point1,  # type: list[float]
+        point2,  # type: list[float]
     ):  # type: (...) -> None
-        self.coords = [[x1, y1, z1], [x2, y2, z2]]
-        self.points = [Point(coord) for coord in self.coords]
+        self.coords = [point1, point2]
+        self.points = [_Point(point) for point in self.coords]
 
-    def translate(self, dx=0, dy=0, dz=0):  # type: (float, float, float) -> Line
+    def translate(self, dx=0, dy=0, dz=0):  # type: (float, float, float) -> None
         """ 平移 """
         for point in self.points:
             point.translate(dx, dy, dz)
-        return self
 
-    def rotate(self, dx=0, dy=0, dz=0):  # type: (float, float, float) -> Line
+    def rotate(self, dx=1, dy=1, dz=1, *, center=[0, 0, 0]):
+        # type: (float, float, float, ..., Iterable[float]) -> None
         """ 旋转 """
         for point in self.points:
-            point.rotate(dx, dy, dz)
-        return self
+            point.rotate(dx, dy, dz, center=center)
+
+    def scale(self, kx=1, ky=1, kz=1, *, center=None):
+        # type: (float, float, float, ..., Iterable[float] | None) -> None
+        """ 缩放 """
+        if center is None:
+            center = [statistics.mean(axis) for axis in zip(*self.coords)]
+        for point in self.points:
+            point.scale(kx, ky, kz, center=center)
 
     def project(self, distance):  # type: (float) -> list[list[float]]
         """ 投影 """
         return [point.project(distance) for point in self.points]
 
 
-class Side:
+class _Side:
     """ 面 """
 
-    def __init__(self, *coords):  # type: (list[float]) -> None
-        self.coords = list(coords)
-        self.lines = [Line(*coords[ind-1], *coords[ind])
-                      for ind in range(len(coords))]
+    def __init__(self, *points):  # type: (list[float]) -> None
+        self.coords = list(points)
+        self.lines = [_Line(points[ind-1], points[ind])
+                      for ind in range(len(points))]
 
-    def translate(self, dx=0, dy=0, dz=0):  # type: (float, float, float) -> Side
+    def translate(self, dx=0, dy=0, dz=0):  # type: (float, float, float) -> None
         """ 平移 """
-        for line in self.lines:
-            line.translate(dx, dy, dz)
-        return self
+        for point in set(point for line in self.lines for point in line.points):
+            point.translate(dx, dy, dz)
 
-    def rotate(self, dx=0, dy=0, dz=0):  # type: (float, float, float) -> Side
+    def rotate(self, dx=1, dy=1, dz=1, *, center=[0, 0, 0]):
+        # type: (float, float, float, ..., Iterable[float]) -> None
         """ 旋转 """
-        for line in self.lines:
-            line.rotate(dx, dy, dz)
-        return self
+        for point in set(point for line in self.lines for point in line.points):
+            point.rotate(dx, dy, dz, center=center)
+
+    def scale(self, kx=1, ky=1, kz=1, *, center=None):
+        # type: (float, float, float, ..., Iterable[float] | None) -> None
+        """ 缩放 """
+        if center is None:
+            center = [statistics.mean(axis) for axis in zip(*self.coords)]
+        for point in set(point for line in self.lines for point in line.points):
+            point.scale(kx, ky, kz, center=center)
 
     def project(self, distance):  # type: (float) -> list[list[list[float]]]
         """ 投影 """
         return [line.project(distance) for line in self.lines]
 
 
+class Point(_Point):
+    """ 点 """
+
+    def __init__(
+        self,
+        canvas,  # type: Canvas_3D
+        coords,  # type: list[float]
+        *,
+        size=POINT_SIZE,  # type: float
+        width=POINT_WIDTH,  # type: float
+        fill=COLOR_POINT_FILL,  # type: str
+        outline=COLOR_POINT_OUTLINE,  # type: str
+    ):  # type: (...) -> None
+        """
+        `canvas`: 父画布\n
+        `coords`: 点的空间坐标\n
+        `size`: 点的大小\n
+        `width`: 点轮廓的宽度\n
+        `fill`: 点内部的填充颜色\n
+        `outline`: 点轮廓的颜色\n
+        """
+        _Point.__init__(self, coords)
+        canvas._items_3d.append(self)
+        self.canvas = canvas
+        self.size = size
+        self.width = width
+        self.fill = fill
+        self.item = canvas.create_oval(
+            -1, -1, -1, -1, fill=fill, outline=outline, width=width)
+        self.update()
+
+    def update(self) -> None:
+        """ 更新 """
+        x, y = self.project(self.canvas.distance)
+        kx, ky = self.canvas.rx, self.canvas.ry
+        x += self.canvas.dx
+        y += self.canvas.dy
+        self.canvas.coords(
+            self.item, (x-self.size)*kx, (y-self.size)*ky, (x+self.size)*kx, (y+self.size)*ky)
+
+
+class Line(_Line):
+    """ 线 """
+
+    def __init__(
+        self,
+        canvas,  # type: Canvas_3D
+        point1,  # type: list[float]
+        point2,  # type: list[float]
+        *,
+        width=LINE_WDITH,  # type: float
+        fill=COLOR_LINE_FILL,  # type: str
+    ):  # type: (...) -> None
+        """
+        `canvas`: 父画布\n
+        `point1`: 起点坐标\n
+        `point2`: 终点坐标\n
+        `width`: 线的宽度\n
+        `fill`: 线的颜色\n
+        """
+        _Line.__init__(self, point1, point2)
+        canvas._items_3d.append(self)
+        self.canvas = canvas
+        self.width = width
+        self.fill = fill
+        self.item = canvas.create_line(-1, -1, -1, -1, width=width, fill=fill)
+        self.update()
+
+    def update(self) -> None:
+        """ 更新 """
+        kx, ky = self.canvas.rx, self.canvas.ry
+        data = self.project(self.canvas.distance)
+        for point in data:
+            point[0] += self.canvas.dx
+            point[1] += self.canvas.dy
+        self.canvas.coords(
+            self.item, *[coord*(ky if i else kx) for point in data for i, coord in enumerate(point)])
+
+
+class Side(_Side):
+    """ 面 """
+
+    def __init__(
+        self,
+        canvas,  # type: Canvas_3D
+        *points,  # type: list[float]
+        width=SIDE_WIDTH,  # type: float
+        fill=COLOR_SIDE_FILL,  # type: str
+        outline=COLOR_SIDE_OUTLINE,  # type: str
+    ):  # type: (...) -> None
+        """
+        `canvas`: 父画布\n
+        `points`: 各点的空间坐标\n
+        `width`: 面轮廓的宽度\n
+        `fill`: 面内部的填充颜色\n
+        `outline`: 面轮廓的颜色\n
+        """
+        _Side.__init__(self, *points)
+        canvas._items_3d.append(self)
+        self.canvas = canvas
+        self.width = width
+        self.fill = fill
+        self.outline = outline
+        self.item = canvas.create_polygon(-1, -1, -1, -1,
+                                          width=width, fill=fill, outline=outline)
+        self.update()
+
+    def update(self) -> None:
+        """ 更新 """
+        kx, ky = self.canvas.rx, self.canvas.ry
+        data = self.project(self.canvas.distance)
+        for line in data:
+            for point in line:
+                point[0] += self.canvas.dx
+                point[1] += self.canvas.dy
+        self.canvas.coords(
+            self.item, *[coord*(ky if i else kx) for line in data for point in line for i, coord in enumerate(point)])
+
+
 class Geometry:
     """ 几何体 """
 
-    def __init__(self, canvas, *sides):  # type: (tkintertools.Canvas, Side) -> None
+    def __init__(self, canvas, *sides):  # type: (Canvas_3D, _Side) -> None
         """
         `canvas`: 显示的画布\n
-        `size`: 平面类`Side`\n
+        `sides`: 平面类`Side`\n
         """
+        canvas._items_3d.append(self)
         self.canvas = canvas
         self.coords = []  # type: list[list[float]]
         self.sides = []  # type: list[Side]
-        self.items = []  # type: list[tkinter._CanvasItemId]
         if sides:
             self.append(*sides)
 
     def translate(self, dx=0, dy=0, dz=0):  # type: (float, float, float) -> None
-        """ 平移 """
-        for side in self.sides:
-            side.translate(dx, dy, dz)
+        """
+        平移\n
+        `dx`: x轴方向位移距离\n
+        `dy`: y轴方向位移距离\n
+        `dz`: z轴方向位移距离\n
+        """
+        for point in set(point for side in self.sides for line in side.lines for point in line.points):
+            point.translate(dx, dy, dz)
 
-    def rotate(self, dx=0, dy=0, dz=0):  # type: (float, float, float) -> None
-        """ 旋转 """
-        for side in self.sides:
-            side.rotate(dx, dy, dz)
+    def rotate(self, dx=1, dy=1, dz=1, *, center=[0, 0, 0]):
+        # type: (float, float, float, ..., Iterable[float]) -> None
+        """
+        旋转\n
+        `dx`: 绕x轴方向旋转角度\n
+        `dy`: 绕y轴方向旋转角度\n
+        `dz`: 绕z轴方向旋转角度\n
+        `center`: 旋转中心\n
+        """
+        for point in set(point for side in self.sides for line in side.lines for point in line.points):
+            point.rotate(dx, dy, dz, center=center)
+
+    def scale(self, kx=1, ky=1, kz=1, *, center=None):
+        # type: (float, float, float, ..., Iterable[float] | None) -> None
+        """
+        缩放\n
+        `kx`: x轴方向缩放比例\n
+        `ky`: y轴方向缩放比例\n
+        `kz`: z轴方向缩放比例\n
+        `center`: 缩放中心，默认为几何中心\n
+        """
+        if center is None:
+            # NOTE: 对凹面几何体无效
+            center = [statistics.mean(axis) for axis in zip(*self.coords)]
+        for point in set(point for side in self.sides for line in side.lines for point in line.points):
+            point.scale(kx, ky, kz, center=center)
 
-    def center(self):  # type: () -> tuple[float, float, float]
-        """ 几何中心 """  # NOTE: 对凹面几何体无效
-        data = list(zip(*self.coords))  # 转置
-        x_c = statistics.mean(data[0])
-        y_c = statistics.mean(data[1])
-        z_c = statistics.mean(data[2])
-        return x_c, y_c, z_c
+    def update(self):  # type: () -> None
+        """ 更新几何体 """
+        for side in self.sides:
+            side.update()
 
     def append(self, *sides):  # type: (Side) -> None
-        """ 添加面 """
+        """
+        添加面\n
+        `sides`: `Side`类\n
+        """
         for side in sides:
             for line in side.lines:
                 for point in line.points:
                     if point not in self.coords:
                         self.coords.append(point)
             self.sides.append(side)
 
-    def update(self, distance, dx=0, dy=0):  # type: (float, float, float) -> None
-        """ 更新几何体 """
-        c = 0
-        for side in self.sides:
-            coords = side.project(distance)
-            for coord in coords:
-
-                k = []
-
-                for lst in coord:
-                    if dx or dy:
-                        lst[0] += 640
-                        lst[1] += 360
-                    k.append(lst[0])
-                    k.append(lst[1])
-
-                self.canvas.coords(self.items[c], k)
-                c += 1
-
-    def draw(self, distance, dx=0, dy=0):  # type: (float, float, float) -> None
-        """ 绘制 """
-        for side in self.sides:
-            coords = side.project(distance)
-            for coord in coords:
-
-                if dx or dy:
-                    for lst in coord:
-                        lst[0] += dx
-                        lst[1] += dy
-
-                self.items.append(self.canvas.create_polygon(
-                    *coord, outline='black'))
-
 
 class Cuboid(Geometry):
     """ 长方体 """
 
     def __init__(
         self,
-        canvas,  # type: tkintertools.Canvas
+        canvas,  # type: Canvas_3D
         x,  # type: float
         y,  # type: float
         z,  # type: float
         length,  # type: float
         width,  # type: float
         height,  # type: float
     ):  # type: (...) -> None
@@ -207,36 +372,35 @@
         """
         self.canvas = canvas
         self.coords = [[x+l, y+w, z+h]
                        for l in (0, length)
                        for w in (0, width)
                        for h in (0, height)]
         self.sides = [
-            Side(self.coords[0], self.coords[1],
+            Side(canvas, self.coords[0], self.coords[1],
                  self.coords[3], self.coords[2]),
-            Side(self.coords[0], self.coords[1],
+            Side(canvas, self.coords[0], self.coords[1],
                  self.coords[5], self.coords[4]),
-            Side(self.coords[0], self.coords[2],
+            Side(canvas, self.coords[0], self.coords[2],
                  self.coords[6], self.coords[4]),
-            Side(self.coords[1], self.coords[3],
+            Side(canvas, self.coords[1], self.coords[3],
                  self.coords[7], self.coords[5]),
-            Side(self.coords[2], self.coords[3],
+            Side(canvas, self.coords[2], self.coords[3],
                  self.coords[7], self.coords[6]),
-            Side(self.coords[4], self.coords[5],
+            Side(canvas, self.coords[4], self.coords[5],
                  self.coords[7], self.coords[6]),
         ]
-        self.items = []  # type: list[tkinter._CanvasItemId]
 
 
 class Tetrahedron(Geometry):
     """ 四面体 """
 
     def __init__(
         self,
-        canvas,  # type: tkintertools.Canvas
+        canvas,  # type: Canvas_3D
         p1,  # type: Iterable[float]
         p2,  # type: Iterable[float]
         p3,  # type: Iterable[float]
         p4,  # type: Iterable[float]
     ):  # type: (...) -> None
         """
         `canvas`: 父画布\n
@@ -244,66 +408,12 @@
         `p2`: 第二个顶点\n
         `p3`: 第三个顶点\n
         `p4`: 第四个顶点\n
         """
         self.canvas = canvas
         self.coords = [list(p1), list(p2), list(p3), list(p4)]
         self.sides = [
-            Side(p1, p2, p3),
-            Side(p1, p2, p4),
-            Side(p1, p3, p4),
-            Side(p2, p3, p4),
+            Side(canvas, self.coords[0], self.coords[1], self.coords[2]),
+            Side(canvas, self.coords[0], self.coords[1], self.coords[3]),
+            Side(canvas, self.coords[0], self.coords[2], self.coords[3]),
+            Side(canvas, self.coords[1], self.coords[2], self.coords[3]),
         ]
-        self.items = []  # type: list[tkinter._CanvasItemId]
-
-
-ORIGIN = Point((0,)*3)
-""" 原点 """
-
-LINE_X = Line(0, 0, 0, 1, 0, 0)
-""" X 轴单位直线 """
-LINE_Y = Line(0, 0, 0, 0, 1, 0)
-""" Y 轴单位直线 """
-LINE_Z = Line(0, 0, 0, 0, 0, 1)
-""" Z 轴单位直线 """
-
-SIDE_YZ = Side((0, 1, 1), (0, 1, -1), (0, -1, -1), (0, -1, 1))
-""" 垂直 X 轴单位平面 """
-SIDE_ZX = Side((1, 0, 1), (1, 0, -1), (-1, 0, -1), (-1, 0, 1))
-""" 垂直 Y 轴单位平面 """
-SIDE_XY = Side((1, 1, 0), (1, -1, 0), (-1, -1, 0), (-1, 1, 0))
-""" 垂直 Z 轴单位平面 """
-
-
-# class Ellipsoid:
-#     """ 椭球体 """
-
-#     def __init__(
-#         self,
-#         x,  # type: float
-#         y,  # type: float
-#         z,  # type: float
-#         length,  # type: float
-#         width,  # type: float
-#         height  # type: float
-#     ):  # type: (...) -> None
-#         self.coords = [[x+l, y+w, z+h]
-#                        for l in (0, length)
-#                        for w in (0, width)
-#                        for h in (0, height)]
-#         self.points = [Point(coord) for coord in self.coords]
-
-#     def translate(self, dx=0, dy=0, dz=0):  # type: (float, float, float) -> None
-#         """ 平移 """
-#         for point in self.points:
-#             point.translate(dx, dy, dz)
-
-#     def rotate(self, dx=0, dy=0, dz=0):  # type: (float, float, float) -> None
-#         """ 旋转 """
-#         for point in self.points:
-#             point.rotate(dx, dy, dz)
-
-#     # type: (float) -> tuple[list[float], list[float]]
-#     def project(self, distance):
-#         """ 投影 """
-#         coefficient = distance/(distance - self.coords[0])
-#         return [self.coords[1]*coefficient, self.coords[2]*coefficient]
```

### Comparing `tkintertools-dev-2.6.2/tkintertools_dev.egg-info/PKG-INFO` & `tkintertools-dev-2.6.3/tkintertools_dev.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,89 +1,198 @@
 Metadata-Version: 2.1
 Name: tkintertools-dev
-Version: 2.6.2
+Version: 2.6.3
 Summary: An auxiliary module of the tkinder module
-Home-page: https://gitcode.net/weixin_62651706/tkintertools
+Home-page: https://github.com/Xiaokang2022/tkintertools
 Author: Xiaokang2022
 Author-email: 2951256653@qq.com
 License: MulanPSL-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
     <h1>🚀tkintertools🚀</h1>
     <p><img height="120px" alt="logo.png"
-        src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/tkintertools.png" />
+        src="./tkintertools.png" />
     </p>
     <p>The <code>tkintertools</code> module is an auxiliary module of the <code>tkinter</code> module</p>
     <p><code>tkintertools</code> 模块是 <code>tkinter</code> 模块的辅助模块</p>
     <p>
         <a href="./tkintertools/__init__.py">
-            <img src="https://img.shields.io/badge/Version-2.6.1-blue" alt="latest version" />
+            <img src="https://img.shields.io/badge/Version-2.6.2-blue" alt="latest version" />
         </a>
         <a href="./LICENSE">
             <img src="https://img.shields.io/badge/License-Mulan PSL v2-green" alt="License" />
         </a>
         <a href="./CHANGELOG.md">
-            <img src="https://img.shields.io/badge/ChangeLog-2023/05/26-orange" alt="ChangeLog" />
+            <img src="https://img.shields.io/badge/ChangeLog-2023/06/06-orange" alt="ChangeLog" />
         </a>
         <a href="./TODO.md">
-            <img src="https://img.shields.io/badge/ToDos-10-yellow" alt="ToDos" />
+            <img src="https://img.shields.io/badge/ToDos-13-yellow" alt="ToDos" />
         </a>
         <a href="https://pypistats.org/packages/tkintertools">
             <img src="https://img.shields.io/badge/Downloads-3k-purple" alt="Downloads" />
         </a>
     </p>
     <p>
         <a href="mailto:2951256653@qq.com">
             <img src="https://img.shields.io/badge/Email-2951256653@qq.com-cyan" alt="Email" />
         </a>
         <a href="https://xiaokang2022.blog.csdn.net">
             <img src="https://img.shields.io/badge/Blog-小康2022@CSDN-red" alt="Blog" />
         </a>
-        <a href="https://gitcode.net/weixin_62651706">
+        <a href="https://github.com/Xiaokang2022">
             <img src="https://img.shields.io/badge/Author-小康2022-white" alt="Author" />
         </a>
     </p>
 </div>
 
 Installation/模块安装
 -----------------------
 
 ### Stable version/稳定版本
 
-* Version/版本 : 2.6.1
-* Release Date/发布日期 : 2023/05/21
+* Version/版本 : 2.6.2
+* Release Date/发布日期 : 2023/05/30
 
 ```
-pip install tkintertools==2.6.1
+pip install tkintertools==2.6.2
 ```
 或者
 ```
 pip install tkintertools
 ```
 
-这个是目前的最新版，比较稳定，bug 没有那么多，推荐使用这个。  
+这个是目前的最新稳定版，比较稳定，bug 没有那么多，推荐使用这个。  
 稳定版有文档可以查看，有 issue 我会去查看并尝试解决 issue。
 
 ### Development version/开发版本
 
-* Version/版本 : 2.6.2
-* Release Date/发布日期 : 2023/05/26
+* Version/版本 : 2.6.3
+* Release Date/发布日期 : 2023/06/06
 
 ```
-pip install tkintertools-dev==2.6.2
+pip install tkintertools-dev==2.6.3
 ```
 
-这个是作者正在开发的版本，有新功能，但不能保证稳定，bug 可能会比较多。  
+这个是我正在开发的版本，有新功能，但不能保证稳定，bug 可能会比较多。  
 开发版本没有对应的文档，大家可以在 issue 中提出建议，我会适当采纳一些并在开发版本中更改或实现。
 
+News/最新功能
+------------
+
+最新版的`tkintertools`为`2.6.2`，新增一项极为强大的功能：3d绘图！  
+同时修复一些bug，优化了一部分代码，提升了一部分性能。
+
+通过以下代码来使用3d绘图功能：
+
+```python
+from tkintertools import tools_3d as t3d
+import tkintertools.tools_3d as t3d
+# 两种引入方式都可以
+```
+
+子模块: [tools_3d.py](./tkintertools/tools_3d.py)
+
+目前3d绘图功能还比较简陋，仅能绘制点、线、面以及直边的空间几何体，对于曲边的空间几何体还在开发中！  
+以下是一个使用3d绘图的示例：
+
+在这个示例中，按住鼠标左键可以旋转几何体，按住鼠标右键可以平移几何体，滚动鼠标滚轮可以缩放几何体！  
+x、y 和 z 轴分别是红色、绿色和蓝色的线。
+
+![3d绘图](./docs/images/3d.png)
+
+<details><summary><b>源代码</b></summary>
+
+```python
+import random
+import tkinter
+
+import tkintertools as tkt
+from tkintertools import tools_3d as t3d
+
+root = tkt.Tk('tools_3d', 1280, 720)
+canvas = t3d.Canvas_3D(root, 1280, 720, 0, 0)
+
+geos = []  # type: list[t3d.Geometry]
+origin = t3d.Point(canvas, [0, 0, 0], size=5)  # 原点
+axes = [t3d.Line(canvas, [0, 0, 0], [100, 0, 0], width=3, fill='red'),  # 创建坐标轴
+        t3d.Line(canvas, [0, 0, 0], [0, 100, 0], width=3, fill='green'),
+        t3d.Line(canvas, [0, 0, 0], [0, 0, -100], width=3, fill='blue')]
+
+for _ in range(8):
+    # 创建正方体
+    cube = t3d.Cuboid(
+        canvas, *random.sample(range(-200, 200), 3), *random.sample(range(50, 100), 3))
+    geos.append(cube)
+    # 创建四面体
+    x, y, z = random.sample(range(-200, 200), 3)
+    tetr = t3d.Tetrahedron(
+        canvas, *[[x+random.randint(-100, 100), y+random.randint(-100, 100), z+random.randint(-100, 100)] for _ in range(4)])
+    geos.append(tetr)
+
+
+def translate(event, flag=False, _cache=[]):
+    # type: (tkinter.Event, bool, list[float]) -> None
+    """ 平移事件 """
+    if flag:
+        _cache[:] = [event.x, event.y]
+        return
+    dx = (event.x - _cache[0]) / 6
+    dy = (event.y - _cache[1]) / 6
+    _cache[:] = [event.x, event.y]
+    for axis in axes:
+        axis.translate(0, 6*dx, 6*dy)
+        axis.update()
+    for geo in geos:
+        geo.translate(0, dx, dy)
+        geo.update()
+    origin.translate(0, 6*dx, 6*dy)
+    origin.update()
+
+
+def rotate(event, flag=False, _cache=[]):  # type: (tkinter.Event, bool, list[float]) -> None
+    """ 旋转事件 """
+    if flag:
+        _cache[:] = [event.x, event.y]
+        return
+    dy = (event.x - _cache[0]) / 200
+    dx = (_cache[1] - event.y) / 200
+    _cache[:] = [event.x, event.y]
+    for axis in axes:
+        axis.rotate(0, 6*dx, 6*dy, center=origin.coords)
+        axis.update()
+    for geo in geos:
+        geo.rotate(0, dx, dy, center=origin.coords)
+        geo.update()
+
+
+def scale(event):  # type: (tkinter.Event) -> None
+    """ 缩放事件 """
+    k = 1.01 if event.delta > 0 else 0.99
+    for geo in geos:
+        geo.scale(k, k, k)
+        geo.update()
+
+
+root.bind('<Button-1>', lambda event: rotate(event, True))
+root.bind('<B1-Motion>', rotate)
+root.bind('<Button-3>', lambda event: translate(event, True))
+root.bind('<B3-Motion>', translate)
+root.bind('<MouseWheel>', scale)
+root.mainloop()
+```
+
+</details>
+
+更多更新信息请见：[CHANGELOG.md](./CHANGELOG.md)
+
 Description/模块说明
 ----------------------
 
 tkintertools 是一款基于 tkinter 模块的二次开发的界面编程模块，它完全没有使用任何第三方模块和库的，同时，它也没有任何依赖包，它的功能完全由内置模块和函数实现，而且，它还是跨平台的！它和 tkinter 最大的不同在于，它的控件并非真实的控件，而是在 tkinter 模块中 Canvas 对象中绘制而成的，这就赋予了 tkintertools 控件一些在 tkinter 中没有的特性，列举如下：
 
 * 控件背景可以是透明的（实际上是没有背景颜色）
 * 控件的样式可以是自定义的（比如按钮有圆角）
@@ -580,17 +689,17 @@
 
 ![exam3_1.png](docs/examples/exam3_1.png)
 ![exam3_2.png](docs/examples/exam3_2.png)
 
 More/更多
 ---------
 
-> GitCode:  
-> https://gitcode.net/weixin_62651706/tkintertools
+> GitHub:  
+> https://github.com/Xiaokang2022/tkintertools
 
-> GitHub(Mirror/镜像):  
-> https://github.com/XiaoKang2022-CSDN/tkintertools
+> GitCode(Mirror/镜像):  
+> https://gitcode.net/weixin_62651706/tkintertools
 
-> Column/专栏:  
-> https://blog.csdn.net/weixin_62651706/category_11600888.html
+> Gitee(Mirror/镜像):  
+> https://gitee.com/xiaokang-2022/tkintertools
 
 还有更多内容请在 [源代码](./tkintertools/) 中探索！
```

#### html2text {}

```diff
@@ -1,33 +1,73 @@
-Metadata-Version: 2.1 Name: tkintertools-dev Version: 2.6.2 Summary: An
-auxiliary module of the tkinder module Home-page: https://gitcode.net/
-weixin_62651706/tkintertools Author: Xiaokang2022 Author-email:
-2951256653@qq.com License: MulanPSL-2.0 Classifier: Programming Language ::
-Python :: 3 Classifier: License :: OSI Approved :: Mulan Permissive Software
-License v2 (MulanPSL-2.0) Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown License-File: LICENSE
+Metadata-Version: 2.1 Name: tkintertools-dev Version: 2.6.3 Summary: An
+auxiliary module of the tkinder module Home-page: https://github.com/
+Xiaokang2022/tkintertools Author: Xiaokang2022 Author-email: 2951256653@qq.com
+License: MulanPSL-2.0 Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Mulan Permissive Software License v2
+(MulanPSL-2.0) Classifier: Operating System :: OS Independent Description-
+Content-Type: text/markdown License-File: LICENSE
                       ****** ðtkintertoolsð ******
                                   [logo.png]
      The tkintertools module is an auxiliary module of the tkinter module
              tkintertools æ¨¡åæ¯ tkinter æ¨¡åçè¾å©æ¨¡å
           [latest_version] [License] [ChangeLog] [ToDos] [Downloads]
                             [Email] [Blog] [Author]
 Installation/æ¨¡åå®è£ ----------------------- ### Stable version/
-ç¨³å®çæ¬ * Version/çæ¬ : 2.6.1 * Release Date/åå¸æ¥æ : 2023/05/21
-``` pip install tkintertools==2.6.1 ``` æè ``` pip install tkintertools ```
-è¿ä¸ªæ¯ç®åçææ°çï¼æ¯è¾ç¨³å®ï¼bug
+ç¨³å®çæ¬ * Version/çæ¬ : 2.6.2 * Release Date/åå¸æ¥æ : 2023/05/30
+``` pip install tkintertools==2.6.2 ``` æè ``` pip install tkintertools ```
+è¿ä¸ªæ¯ç®åçææ°ç¨³å®çï¼æ¯è¾ç¨³å®ï¼bug
 æ²¡æé£ä¹å¤ï¼æ¨èä½¿ç¨è¿ä¸ªã ç¨³å®çæææ¡£å¯ä»¥æ¥çï¼æ
 issue æä¼å»æ¥çå¹¶å°è¯è§£å³ issueã ### Development version/
-å¼åçæ¬ * Version/çæ¬ : 2.6.2 * Release Date/åå¸æ¥æ : 2023/05/26
-``` pip install tkintertools-dev==2.6.2 ```
-è¿ä¸ªæ¯ä½èæ­£å¨å¼åççæ¬ï¼ææ°åè½ï¼ä½ä¸è½ä¿è¯ç¨³å®ï¼bug
+å¼åçæ¬ * Version/çæ¬ : 2.6.3 * Release Date/åå¸æ¥æ : 2023/06/06
+``` pip install tkintertools-dev==2.6.3 ```
+è¿ä¸ªæ¯ææ­£å¨å¼åççæ¬ï¼ææ°åè½ï¼ä½ä¸è½ä¿è¯ç¨³å®ï¼bug
 å¯è½ä¼æ¯è¾å¤ã å¼åçæ¬æ²¡æå¯¹åºçææ¡£ï¼å¤§å®¶å¯ä»¥å¨ issue
 ä¸­æåºå»ºè®®ï¼æä¼éå½éçº³ä¸äºå¹¶å¨å¼åçæ¬ä¸­æ´æ¹æå®ç°ã
-Description/æ¨¡åè¯´æ ---------------------- tkintertools æ¯ä¸æ¬¾åºäº
-tkinter
+News/ææ°åè½ -----------
+-
+ææ°çç`tkintertools`ä¸º`2.6.2`ï¼æ°å¢ä¸é¡¹æä¸ºå¼ºå¤§çåè½ï¼3dç»å¾ï¼
+åæ¶ä¿®å¤ä¸äºbugï¼ä¼åäºä¸é¨åä»£ç ï¼æåäºä¸é¨åæ§è½ã
+éè¿ä»¥ä¸ä»£ç æ¥ä½¿ç¨3dç»å¾åè½ï¼ ```python from tkintertools import
+tools_3d as t3d import tkintertools.tools_3d as t3d #
+ä¸¤ç§å¼å¥æ¹å¼é½å¯ä»¥ ``` å­æ¨¡å: [tools_3d.py](./tkintertools/
+tools_3d.py)
+ç®å3dç»å¾åè½è¿æ¯è¾ç®éï¼ä»è½ç»å¶ç¹ãçº¿ãé¢ä»¥åç´è¾¹çç©ºé´å ä½ä½ï¼å¯¹äºæ²è¾¹çç©ºé´å ä½ä½è¿å¨å¼åä¸­ï¼
+ä»¥ä¸æ¯ä¸ä¸ªä½¿ç¨3dç»å¾çç¤ºä¾ï¼
+å¨è¿ä¸ªç¤ºä¾ä¸­ï¼æä½é¼ æ å·¦é®å¯ä»¥æè½¬å ä½ä½ï¼æä½é¼ æ å³é®å¯ä»¥å¹³ç§»å ä½ä½ï¼æ»å¨é¼ æ æ»è½®å¯ä»¥ç¼©æ¾å ä½ä½ï¼
+xãy å z è½´åå«æ¯çº¢è²ãç»¿è²åèè²ççº¿ã ![3dç»å¾](./docs/
+images/3d.png) æºä»£ç  ```python import random import tkinter import
+tkintertools as tkt from tkintertools import tools_3d as t3d root = tkt.Tk
+('tools_3d', 1280, 720) canvas = t3d.Canvas_3D(root, 1280, 720, 0, 0) geos = []
+# type: list[t3d.Geometry] origin = t3d.Point(canvas, [0, 0, 0], size=5) #
+åç¹ axes = [t3d.Line(canvas, [0, 0, 0], [100, 0, 0], width=3, fill='red'), #
+åå»ºåæ è½´ t3d.Line(canvas, [0, 0, 0], [0, 100, 0], width=3,
+fill='green'), t3d.Line(canvas, [0, 0, 0], [0, 0, -100], width=3, fill='blue')]
+for _ in range(8): # åå»ºæ­£æ¹ä½ cube = t3d.Cuboid( canvas, *random.sample
+(range(-200, 200), 3), *random.sample(range(50, 100), 3)) geos.append(cube) #
+åå»ºåé¢ä½ x, y, z = random.sample(range(-200, 200), 3) tetr =
+t3d.Tetrahedron( canvas, *[[x+random.randint(-100, 100), y+random.randint(-100,
+100), z+random.randint(-100, 100)] for _ in range(4)]) geos.append(tetr) def
+translate(event, flag=False, _cache=[]): # type: (tkinter.Event, bool, list
+[float]) -> None """ å¹³ç§»äºä»¶ """ if flag: _cache[:] = [event.x, event.y]
+return dx = (event.x - _cache[0]) / 6 dy = (event.y - _cache[1]) / 6 _cache[:
+] = [event.x, event.y] for axis in axes: axis.translate(0, 6*dx, 6*dy)
+axis.update() for geo in geos: geo.translate(0, dx, dy) geo.update()
+origin.translate(0, 6*dx, 6*dy) origin.update() def rotate(event, flag=False,
+_cache=[]): # type: (tkinter.Event, bool, list[float]) -> None """ æè½¬äºä»¶
+""" if flag: _cache[:] = [event.x, event.y] return dy = (event.x - _cache[0]) /
+200 dx = (_cache[1] - event.y) / 200 _cache[:] = [event.x, event.y] for axis in
+axes: axis.rotate(0, 6*dx, 6*dy, center=origin.coords) axis.update() for geo in
+geos: geo.rotate(0, dx, dy, center=origin.coords) geo.update() def scale
+(event): # type: (tkinter.Event) -> None """ ç¼©æ¾äºä»¶ """ k = 1.01 if
+event.delta > 0 else 0.99 for geo in geos: geo.scale(k, k, k) geo.update()
+root.bind('', lambda event: rotate(event, True)) root.bind('', rotate)
+root.bind('', lambda event: translate(event, True)) root.bind('', translate)
+root.bind('', scale) root.mainloop() ```  æ´å¤æ´æ°ä¿¡æ¯è¯·è§ï¼
+[CHANGELOG.md](./CHANGELOG.md) Description/æ¨¡åè¯´æ ---------------------
+- tkintertools æ¯ä¸æ¬¾åºäº tkinter
 æ¨¡åçäºæ¬¡å¼åççé¢ç¼ç¨æ¨¡åï¼å®å®å¨æ²¡æä½¿ç¨ä»»ä½ç¬¬ä¸æ¹æ¨¡åååºçï¼åæ¶ï¼å®ä¹æ²¡æä»»ä½ä¾èµåï¼å®çåè½å®å¨ç±åç½®æ¨¡ååå½æ°å®ç°ï¼èä¸ï¼å®è¿æ¯è·¨å¹³å°çï¼å®å
 tkinter æå¤§çä¸åå¨äºï¼å®çæ§ä»¶å¹¶éçå®çæ§ä»¶ï¼èæ¯å¨
 tkinter æ¨¡åä¸­ Canvas å¯¹è±¡ä¸­ç»å¶èæçï¼è¿å°±èµäºäº
 tkintertools æ§ä»¶ä¸äºå¨ tkinter ä¸­æ²¡æçç¹æ§ï¼åä¸¾å¦ä¸ï¼ *
 æ§ä»¶èæ¯å¯ä»¥æ¯éæçï¼å®éä¸æ¯æ²¡æèæ¯é¢è²ï¼ *
 æ§ä»¶çæ ·å¼å¯ä»¥æ¯èªå®ä¹çï¼æ¯å¦æé®æåè§ï¼ *
 æ§ä»¶çåå»ºéåº¦è¿å¤§äº tkinter çæ§ä»¶ï¼é¤äº Canvas æ§ä»¶ï¼
@@ -255,11 +295,11 @@
 ### ç®æç»å½çé¢ * æç« é¾æ¥: ææ  * ä»£ç ä»åº: https://
 gitcode.net/weixin_62651706/tester * ç¨åºä¸è½½: ææ  * æ¨èææ°:
 ððð è¿ä¸ªæ¡ä¾ä½¿ç¨äºææ°ç¨³å®çç tkintertools-
 v2.6.0ï¼çé¢éå¸¸ç¨³å®ï¼å ä¹æ²¡æ bugï¼å®å¨éç¨ tkintertools
 çæ§ä»¶ï¼é¢å¼å¾é«ï¼çé¢éå¸¸æµçãä½ç°äº tkintertools
 æ¨¡åä¸ tkinter æ¨¡åç¸æ¯å¨æ§è½ä¸çä¼è¶æ§ï¼ ![exam3_1.png](docs/
 examples/exam3_1.png) ![exam3_2.png](docs/examples/exam3_2.png) More/æ´å¤ ---
------- > GitCode: > https://gitcode.net/weixin_62651706/tkintertools > GitHub
-(Mirror/éå): > https://github.com/XiaoKang2022-CSDN/tkintertools > Column/
-ä¸æ : > https://blog.csdn.net/weixin_62651706/category_11600888.html
+------ > GitHub: > https://github.com/Xiaokang2022/tkintertools > GitCode
+(Mirror/éå): > https://gitcode.net/weixin_62651706/tkintertools > Gitee
+(Mirror/éå): > https://gitee.com/xiaokang-2022/tkintertools
 è¿ææ´å¤åå®¹è¯·å¨ [æºä»£ç ](./tkintertools/) ä¸­æ¢ç´¢ï¼
```

