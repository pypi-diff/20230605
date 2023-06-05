# Comparing `tmp/hh_ui_check-0.1.5.tar.gz` & `tmp/hh_ui_check-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hh_ui_check-0.1.5.tar", max compression
+gzip compressed data, was "hh_ui_check-0.1.6.tar", max compression
```

## Comparing `hh_ui_check-0.1.5.tar` & `hh_ui_check-0.1.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     6273 2023-06-02 05:34:57.983561 hh_ui_check-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-06-02 03:09:39.424775 hh_ui_check-0.1.5/hh_ui_check/__init__.py
--rwxr-xr-x   0        0        0      729 2023-06-05 06:48:39.171611 hh_ui_check-0.1.5/hh_ui_check/__main__.py
--rw-r--r--   0        0        0     3733 2023-06-05 06:42:28.034026 hh_ui_check-0.1.5/hh_ui_check/diff.py
--rw-r--r--   0        0        0     2112 2023-06-05 06:42:32.130634 hh_ui_check-0.1.5/hh_ui_check/hist_compare.py
--rw-r--r--   0        0        0      503 2023-06-05 06:42:35.999893 hh_ui_check-0.1.5/hh_ui_check/horizen.py
--rw-r--r--   0        0        0      607 2023-06-05 06:42:45.982863 hh_ui_check-0.1.5/hh_ui_check/overlapping.py
--rw-r--r--   0        0        0      471 2023-06-05 06:42:23.464798 hh_ui_check-0.1.5/hh_ui_check/substract.py
--rw-r--r--   0        0        0      441 2023-06-05 06:51:05.241298 hh_ui_check-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     6751 1970-01-01 00:00:00.000000 hh_ui_check-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     6436 2023-06-05 07:40:26.333224 hh_ui_check-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-06-02 03:09:39.424775 hh_ui_check-0.1.6/hh_ui_check/__init__.py
+-rwxr-xr-x   0        0        0     1345 2023-06-05 07:37:29.410773 hh_ui_check-0.1.6/hh_ui_check/__main__.py
+-rw-r--r--   0        0        0     3793 2023-06-05 07:35:44.125306 hh_ui_check-0.1.6/hh_ui_check/diff.py
+-rw-r--r--   0        0        0     2112 2023-06-05 07:33:11.573944 hh_ui_check-0.1.6/hh_ui_check/hist_compare.py
+-rw-r--r--   0        0        0      523 2023-06-05 07:33:30.911444 hh_ui_check-0.1.6/hh_ui_check/horizen.py
+-rw-r--r--   0        0        0      627 2023-06-05 07:33:41.444875 hh_ui_check-0.1.6/hh_ui_check/overlapping.py
+-rw-r--r--   0        0        0      491 2023-06-05 07:34:23.893074 hh_ui_check-0.1.6/hh_ui_check/substract.py
+-rw-r--r--   0        0        0      441 2023-06-05 07:38:29.860432 hh_ui_check-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     6914 1970-01-01 00:00:00.000000 hh_ui_check-0.1.6/PKG-INFO
```

### Comparing `hh_ui_check-0.1.5/README.md` & `hh_ui_check-0.1.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -86,7 +86,15 @@
 Show your appreciation to those who have contributed to the project.
 
 ## License
 For open source projects, say how it is licensed.
 
 ## Project status
 If you have run out of energy or time for your project, put a note at the top of the README saying that development has slowed down or stopped completely. Someone may choose to fork your project or volunteer to step in as a maintainer or owner, allowing your project to keep going. You can also make an explicit request for maintainers.
+# 执行命令
+在文件夹里运行 `python -m hh-ui-check`
+
+# 文件夹要求
+内容有 1.png & 2.png
+
+若有子文件夹，子文件里也要有 1.png & 2.png
+
```

### Comparing `hh_ui_check-0.1.5/hh_ui_check/diff.py` & `hh_ui_check-0.1.6/hh_ui_check/diff.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import cv2
 import numpy as np
 
 # 最大要素数量 默认500
 MAX_FEATURES = 500
 GOOD_MATCH_PERCENT = 0.15
 
-def alignImages(im1, im2):
+def alignImages(dirPath, im1, im2):
 
   # im2 is reference and im1 is to be warped to match im2
   # note: numbering is swapped in function
  
   # Convert images to grayscale
   im1Gray = cv2.cvtColor(im1, cv2.COLOR_BGR2GRAY)
   im2Gray = cv2.cvtColor(im2, cv2.COLOR_BGR2GRAY)
@@ -31,15 +31,15 @@
   matches = sorted(matches, key=lambda x: x.distance, reverse=False)
   # Remove not so good matches
   numGoodMatches = int(len(matches) * GOOD_MATCH_PERCENT)
   matches = matches[:numGoodMatches]
  
   # Draw top matches
   imMatches = cv2.drawMatches(im1, keypoints1, im2, keypoints2, matches, None)
-  cv2.imwrite("diff_matches.png", imMatches)
+  cv2.imwrite(dirPath + "/diff_matches.png", imMatches)
    
   # Extract location of good matches
   points1 = np.zeros((len(matches), 2), dtype=np.float32)
   points2 = np.zeros((len(matches), 2), dtype=np.float32)
  
   for i, match in enumerate(matches):
     points1[i, :] = keypoints1[match.queryIdx].pt
@@ -51,20 +51,20 @@
   # Use homography
   height, width, channels = im2.shape
   im1Reg = cv2.warpPerspective(im1, h, (width, height))
    
   return im1Reg, h
  
  
-def getDiffImages(image1, image2):
+def getDiffImages(dirPath, image1, image2):
   hh, ww = image1.shape[:2]
   
   # Aligned image will be stored in imReg. 
   # The estimated homography will be stored in h. 
-  imReg, h = alignImages(image2, image1)
+  imReg, h = alignImages(dirPath, image2, image1)
    
   # Print estimated homography
   # print("Estimated homography : \n",  h)
   
   # Convert images to HSV and get saturation channel
   refSat = cv2.cvtColor(image1, cv2.COLOR_BGR2HSV)[:,:,1]
   imSat = cv2.cvtColor(imReg, cv2.COLOR_BGR2HSV)[:,:,1]
@@ -93,11 +93,11 @@
   result = image1.copy()
   for c in cnts:
       x,y,w,h = cv2.boundingRect(c)
       if x>0 and y>0 and x+w<ww-1 and y+h<hh-1:
         cv2.rectangle(result, (x, y), (x+w, y+h), (0, 0, 255), 2)
 
   # save images
-  cv2.imwrite('diff.png', diff_cleaned)
-  cv2.imwrite('diff_result.png', result)
+  cv2.imwrite(dirPath + '/diff.png', diff_cleaned)
+  cv2.imwrite(dirPath + '/diff_result.png', result)
```

### Comparing `hh_ui_check-0.1.5/hh_ui_check/hist_compare.py` & `hh_ui_check-0.1.6/hh_ui_check/hist_compare.py`

 * *Files identical despite different names*

### Comparing `hh_ui_check-0.1.5/hh_ui_check/overlapping.py` & `hh_ui_check-0.1.6/hh_ui_check/overlapping.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 
 # 两图相减法
 import cv2
 import numpy as np
 
 
-def getOverlapping(image1, image2):
+def getOverlapping(dirPath, image1, image2):
   hh, ww = image1.shape[:2]
   
   hh1, ww1 = image2.shape[:2]
 
   h=max(hh,hh1)
   w=max(ww,ww1)
   org_image=np.ones((h,w,3),dtype=np.uint8)*255
@@ -18,10 +18,10 @@
   org_image[:hh,:ww,:]=image1[:,:,:]
   trans_image[:hh1,:ww1,:]=image2[:,:,:]
 
   # substract_img = trans_image - org_image
   # 权重越大，透明度越低
   overlapping = cv2.addWeighted(org_image, 0.7, trans_image, 0.3, 0)
   # 保存叠加后的图片
-  cv2.imwrite('overlapping.jpg', overlapping)
+  cv2.imwrite(dirPath + '/overlapping.jpg', overlapping)
```

### Comparing `hh_ui_check-0.1.5/PKG-INFO` & `hh_ui_check-0.1.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hh-ui-check
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: 林明超
 Author-email: mingchao.lin@zeekrlife.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -101,8 +101,16 @@
 Show your appreciation to those who have contributed to the project.
 
 ## License
 For open source projects, say how it is licensed.
 
 ## Project status
 If you have run out of energy or time for your project, put a note at the top of the README saying that development has slowed down or stopped completely. Someone may choose to fork your project or volunteer to step in as a maintainer or owner, allowing your project to keep going. You can also make an explicit request for maintainers.
+# 执行命令
+在文件夹里运行 `python -m hh-ui-check`
+
+# 文件夹要求
+内容有 1.png & 2.png
+
+若有子文件夹，子文件里也要有 1.png & 2.png
+
```

