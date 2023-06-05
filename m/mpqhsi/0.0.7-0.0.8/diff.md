# Comparing `tmp/mpqhsi-0.0.7.tar.gz` & `tmp/mpqhsi-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpqhsi-0.0.7.tar", last modified: Thu May 18 05:30:49 2023, max compression
+gzip compressed data, was "mpqhsi-0.0.8.tar", last modified: Mon Jun  5 02:37:06 2023, max compression
```

## Comparing `mpqhsi-0.0.7.tar` & `mpqhsi-0.0.8.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 05:30:49.036711 mpqhsi-0.0.7/
--rw-rw-rw-   0        0        0      217 2023-05-18 05:30:49.036711 mpqhsi-0.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-18 05:30:49.026711 mpqhsi-0.0.7/mpqhsi/
--rw-rw-rw-   0        0        0   133632 2023-05-18 05:29:38.000000 mpqhsi-0.0.7/mpqhsi/My_HSI.cp39-win_amd64.pyd
--rw-rw-rw-   0        0        0     5453 2023-05-18 05:28:03.000000 mpqhsi-0.0.7/mpqhsi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 05:30:49.036711 mpqhsi-0.0.7/mpqhsi.egg-info/
--rw-rw-rw-   0        0        0      217 2023-05-18 05:30:48.000000 mpqhsi-0.0.7/mpqhsi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      180 2023-05-18 05:30:48.000000 mpqhsi-0.0.7/mpqhsi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 05:30:48.000000 mpqhsi-0.0.7/mpqhsi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-18 05:30:48.000000 mpqhsi-0.0.7/mpqhsi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 05:30:49.036711 mpqhsi-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      422 2023-05-17 08:24:59.000000 mpqhsi-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 02:37:06.113896 mpqhsi-0.0.8/
+-rw-rw-rw-   0        0        0      217 2023-06-05 02:37:06.113896 mpqhsi-0.0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-05 02:37:06.103892 mpqhsi-0.0.8/mpqhsi/
+-rw-rw-rw-   0        0        0   133632 2023-05-18 05:29:38.000000 mpqhsi-0.0.8/mpqhsi/My_HSI.cp39-win_amd64.pyd
+-rw-rw-rw-   0        0        0     5523 2023-05-18 06:05:00.000000 mpqhsi-0.0.8/mpqhsi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 02:37:06.113896 mpqhsi-0.0.8/mpqhsi.egg-info/
+-rw-rw-rw-   0        0        0      217 2023-06-05 02:37:06.000000 mpqhsi-0.0.8/mpqhsi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2023-06-05 02:37:06.000000 mpqhsi-0.0.8/mpqhsi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 02:37:06.000000 mpqhsi-0.0.8/mpqhsi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-05 02:37:06.000000 mpqhsi-0.0.8/mpqhsi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-05 02:37:06.000000 mpqhsi-0.0.8/mpqhsi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 02:37:06.113896 mpqhsi-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      437 2023-06-05 02:35:30.000000 mpqhsi-0.0.8/setup.py
```

### Comparing `mpqhsi-0.0.7/mpqhsi/__init__.py` & `mpqhsi-0.0.8/mpqhsi/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 def HSI_get_splist_byclick(datacube, channal=3, bands=[10, 20, 30]):
     #####通过该方法可将鼠标点击位置光谱数据以dataframe的形式存在df中########
     df = get_splist_byclick(datacube, channal, bands)
     return df
 
 
 if __name__ == '__main__':
-    from mpqhsi import *
+    import mpqhsi as mhsi
     in_path = './test_data/'
     out_path = './'
     # result = HSI_meandata_make(in_path,out_path,band=80,thre=100)
     # result.to_csv('HSI_ROI_mean_data.csv',encoding='gb2312')
 
     # img = sp.envi.open('../../data/HSI/原始数据/正1-2.hdr', '../../data/HSI/原始数据/正1-2.cube')
     # # HSI_show_one_band(img,band=[70])
@@ -97,22 +97,23 @@
     #                       r"D:\qiaozhiqi\Code\My_init\mpqhsi\mpqhsi-0.0.2\mpqhsi\test_data\反1-1.cube")
 
     # img = HSI_Read_3bands(r"D:\qiaozhiqi\Code\My_init\mpqhsi\mpqhsi-0.0.2\mpqhsi\test_data\反1-1.hdr",
     #                       r"D:\qiaozhiqi\Code\My_init\mpqhsi\mpqhsi-0.0.2\mpqhsi\test_data\反1-1.cube")
 
     name1 = r"D:\qiaozhiqi\Code\My_init\mpqhsi\mpqhsi-0.0.4\mpqhsi\test_data\baishao_2022-11-29_07-51-13\capture\baishao_2022-11-29_07-51-13.hdr"
     name2 = r"D:\qiaozhiqi\Code\My_init\mpqhsi\mpqhsi-0.0.4\mpqhsi\test_data\baishao_2022-11-29_07-51-13\capture\baishao_2022-11-29_07-51-13.raw"
-    datacube = read_datacube(name1,name2)
-    df = HSI_get_splist_byclick(datacube)
-    df.to_csv('s.csv')
+    datacube = mhsi.read_Datacube(name1,name2)
+    df = mhsi.HSI_get_splist_byclick(datacube)
+    df.to_csv('aa.csv')
     # print(datacube[1,1,:].shape)
     # print(read_Data_one_band(name1,name2).shape)
-    # bin = read_Data_one_sp(name1,name2)[0]
+    # bin = read_Data_one_sp(name1,name2,gre_thre=20)[0]
     # ijlist = read_Data_one_sp(name1,name2)[1]
-    # mpqcv.show_img(bin,0)
+    pic = HSI_Read_one_band(name1,name2)
+    mpqcv.save_pic('a.png',pic)
     # print(len(ijlist))
 
     # print(read_Data_one_band(name1,name2,band=[10]).shape)
     # print(read_Data_one_band(name1,name2,band=10).shape)
     # print(type(read_Data_one_band(name1,name2,band=10)))
     # print(img.shape)
     # cv2.imshow('a',img)
```

