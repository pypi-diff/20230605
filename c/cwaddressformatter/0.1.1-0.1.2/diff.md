# Comparing `tmp/cwaddressformatter-0.1.1-py3-none-any.whl.zip` & `tmp/cwaddressformatter-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,16 @@
-Zip file size: 180871 bytes, number of entries: 12
+Zip file size: 182253 bytes, number of entries: 14
+-rw-r--r--  2.0 unx     6148 b- defN 23-Jun-05 03:40 .DS_Store
 -rw-r--r--  2.0 unx      143 b- defN 20-Jun-02 11:32 address_formatter/__init__.py
 -rw-r--r--  2.0 unx     6608 b- defN 20-Jun-02 11:21 address_formatter/main.py
 -rw-r--r--  2.0 unx       18 b- defN 20-Jun-02 11:31 address_formatter/version.py
+-rw-r--r--  2.0 unx     6148 b- defN 23-Jun-05 03:51 cwaddressformatter/.DS_Store
 -rw-r--r--  2.0 unx      143 b- defN 20-Jun-02 11:32 cwaddressformatter/__init__.py
--rw-r--r--  2.0 unx     8150 b- defN 23-Mar-21 02:55 cwaddressformatter/main.py
--rw-r--r--  2.0 unx  1416653 b- defN 22-Dec-02 08:17 cwaddressformatter/opendata111road.csv
--rw-r--r--  2.0 unx       18 b- defN 23-Mar-21 02:55 cwaddressformatter/version.py
--rw-r--r--  2.0 unx     3313 b- defN 23-Mar-21 03:02 cwaddressformatter-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-21 03:02 cwaddressformatter-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       64 b- defN 23-Mar-21 03:02 cwaddressformatter-0.1.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       19 b- defN 23-Mar-21 03:02 cwaddressformatter-0.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1049 b- defN 23-Mar-21 03:02 cwaddressformatter-0.1.1.dist-info/RECORD
-12 files, 1436270 bytes uncompressed, 179081 bytes compressed:  87.5%
+-rw-r--r--  2.0 unx     8714 b- defN 23-Jun-05 08:44 cwaddressformatter/main.py
+-rw-r--r--  2.0 unx  1416702 b- defN 23-Jun-05 03:40 cwaddressformatter/opendata111road.csv
+-rw-r--r--  2.0 unx       18 b- defN 23-Jun-05 08:44 cwaddressformatter/version.py
+-rw-r--r--  2.0 unx     3481 b- defN 23-Jun-05 08:48 cwaddressformatter-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-05 08:48 cwaddressformatter-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       64 b- defN 23-Jun-05 08:48 cwaddressformatter-0.1.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       19 b- defN 23-Jun-05 08:48 cwaddressformatter-0.1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1200 b- defN 23-Jun-05 08:48 cwaddressformatter-0.1.2.dist-info/RECORD
+14 files, 1449498 bytes uncompressed, 180237 bytes compressed:  87.6%
```

## zipnote {}

```diff
@@ -1,37 +1,43 @@
+Filename: .DS_Store
+Comment: 
+
 Filename: address_formatter/__init__.py
 Comment: 
 
 Filename: address_formatter/main.py
 Comment: 
 
 Filename: address_formatter/version.py
 Comment: 
 
+Filename: cwaddressformatter/.DS_Store
+Comment: 
+
 Filename: cwaddressformatter/__init__.py
 Comment: 
 
 Filename: cwaddressformatter/main.py
 Comment: 
 
 Filename: cwaddressformatter/opendata111road.csv
 Comment: 
 
 Filename: cwaddressformatter/version.py
 Comment: 
 
-Filename: cwaddressformatter-0.1.1.dist-info/METADATA
+Filename: cwaddressformatter-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: cwaddressformatter-0.1.1.dist-info/WHEEL
+Filename: cwaddressformatter-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: cwaddressformatter-0.1.1.dist-info/entry_points.txt
+Filename: cwaddressformatter-0.1.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: cwaddressformatter-0.1.1.dist-info/top_level.txt
+Filename: cwaddressformatter-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: cwaddressformatter-0.1.1.dist-info/RECORD
+Filename: cwaddressformatter-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cwaddressformatter/main.py

```diff
@@ -128,15 +128,16 @@
                 else:
                     return address[0:i+1], address[i+1:]
         
     return "", address
 
 
 openRoad = []
-with open('opendata111road.csv', newline='') as csvfile:
+# with open('opendata111road.csv', newline='') as csvfile:
+with open('./CEROAD11107.csv', newline='') as csvfile:
 
   rows = csv.DictReader(csvfile)
 
   # 以迴圈輸出指定欄位
   for row in rows:
     openRoad.append(row['road'])
 
@@ -156,14 +157,16 @@
     road, address = findAdds(address, ("大樓","街","路","大道","城"))
     sec, address = findAdds(address, ("段"))
     lane, address = findAdds(address, ("巷"))
     alley, address = findAdds(address, ("弄"))
     post, address = findAdds(address, ("郵政"))
     no, address = findAdds(address, ("號"))
     floor, address = findAdds(address, ("樓"))
+    if not floor:
+        floor, address = findAdds(address, ("F"))
     room, address = findAdds(address, ("室"))
     dash, address = findAdds(address, ("之"))
     
     # if road == '苓雅一路':
     # print("Address:", original)
     # print("city:", city, "district:", district, "village:", village, "neighbor:", neighbor)
     # print("road:", road,  "sec:", sec, "lane:", lane, "alley:", alley)
@@ -210,38 +213,46 @@
             road = district
 
     if not road and not no:
         # print("PASS")
         return original
 
     sec = digit2zh(sec)
-    lane = zh2digit(lane)
+
+    # 巷弄有些是中文巷名或是根本沒有巷，例如四維巷，改為加上路名，查詢郵局的地址資料
+    if road+lane not in openRoad:        
+        lane = zh2digit(lane)
+    
     alley = zh2digit(alley)
     # floorName = zh2digit(floorName)
     # floorUnit = zh2digit(floorUnit)
     no = zh2digit(no)
     floor = zh2digit(floor)
     def replaceDash(string):
-        # string = string.replace("之", "-")
+        string = string.replace("之", "-")
+        string = string.replace(",", "")
         # string = string.replace("一", "-")
         return string
     address = zh2digit(address)
     # print(room)
+    lane = replaceDash(lane)
     dash = replaceDash(dash)
     no = replaceDash(no)
+    room = replaceDash(room)
 
     # print("no:" , no)
     # if road == '村圓山路':
-    # print("Address:", original)
-    # print("city:", city, "district:", district, "village:", village, "neighbor:", neighbor)
-    # print("road:", road,  "sec:", sec, "lane:", lane, "alley:", alley)
-    # print("no:", no, "floor:", floor, "room:", room, "address:", address, "dash:", dash)
+    print("Address:", original)
+    print("city:", city, "district:", district, "village:", village, "neighbor:", neighbor)
+    print("road:", road,  "sec:", sec, "lane:", lane, "alley:", alley)
+    print("no:", no, "floor:", floor, "room:", room, "address:", address, "dash:", dash)
     # print("")
-    # print(floor)
-    floor = re.sub(r"(\d+)F", "\\1樓", floor, 0, re.MULTILINE)
+    print(floor)
+    floor = re.sub(r"(\d+)\s*F", "\\1樓", floor, 0, re.MULTILINE)
+    print(floor)
     # print(address)
     address = re.sub(r"(\d+)F", "\\1樓", address, 0, re.MULTILINE)
 
     # address = re.sub(r"(\d+)F", "\\1樓", address, 0, re.MULTILINE)
 
     dash = re.sub(r"(\d+)F", "\\1樓", dash, 0, re.MULTILINE)
 
@@ -251,14 +262,15 @@
     # print("address:", address)
 
     
     str = "".join([road, sec, lane, alley, post, no, floor, room, dash, address])
     str = str.replace("（", "(")
     str = str.replace("）", ")")
     str = str.replace("－", "-")
+    str = str.replace("＿", "-")
     str = str.replace("~", "-")
     str = str.replace(" ", "")
     str = str.replace("街街", "街")
     str = str.replace("号", "號")
     str = str.replace("楼", "樓")
     str = str.replace("，", "")
 
@@ -270,10 +282,12 @@
     return str
 
 # print(getAddress("福鎮街43-2號"))
 
 
 if __name__ == '__main__':
     
-    # print(getDeDupeAddress("中安街178巷3号10F"))
-    # print(getDeDupeAddress("中安街178巷3号F"))
+    # print(getDeDupeAddress("永福街141號12樓之1（C3-12F)警衛室代收"))
+    # print(getDeDupeAddress("興隆路三段 327 號 4 F"))
+    
+    # print(getDeDupeAddress("永福街141號12樓之1（C3-12F)警衛室代收"))
     pass
```

## cwaddressformatter/opendata111road.csv

```diff
@@ -23398,14 +23398,15 @@
 新北市,新北市新店區,中央八街
 新北市,新北市新店區,中央三街
 新北市,新北市新店區,中央五街
 新北市,新北市新店區,中央六街
 新北市,新北市新店區,中央四街
 新北市,新北市新店區,中央路
 新北市,新北市新店區,中正路
+新北市,新北市新店區,中正路四維巷
 新北市,新北市新店區,中生路
 新北市,新北市新店區,中華路
 新北市,新北市新店區,中興路
 新北市,新北市新店區,五峯路
 新北市,新北市新店區,太平路
 新北市,新北市新店區,文中路
 新北市,新北市新店區,文化路
```

## cwaddressformatter/version.py

```diff
@@ -1 +1 @@
-VERSION = "0.1.1"
+VERSION = "0.1.2"
```

## Comparing `cwaddressformatter-0.1.1.dist-info/METADATA` & `cwaddressformatter-0.1.2.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cwaddressformatter
-Version: 0.1.1
+Version: 0.1.2
 Summary: Format address using universal pattern
 Home-page: https://github.com/Shihyen/address-formatter
 Author: Shihyen Chen
 Author-email: sun1229@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -21,14 +21,17 @@
 
 # 地址格式規則
 
 https://pypi.org/project/cwaddressformatter/
 
 ## Release Note
 
+### 0.1.2:  20230605 調整邏輯
+1. 更改地址資料庫為郵局版本(2022/07)，理論上更準，修正了「中正路四維巷」這種中文巷名的問題。
+
 ### 0.1.0:  20230307 調整邏輯
 1. F改為樓，應用在dash參數上(-x)
 2. 半型改全型（）-
 
 ### 0.0.8:  20221202 更新路名OpenData 110版
 
 ### 0.0.5: 20221202 文字轉數字機制優化
```

## Comparing `cwaddressformatter-0.1.1.dist-info/RECORD` & `cwaddressformatter-0.1.2.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+.DS_Store,sha256=Nw7Z9jfHM3UWM3oN5V2xGp3obi4oJJqYKEQHYx7qu-w,6148
 address_formatter/__init__.py,sha256=3e8um1-lzVyp4LEDX_nV5yrFnPLEnmDOgCQDRkhXkEY,143
 address_formatter/main.py,sha256=_xHyp9tH1vbFeJoI5fSW3yr-VZ_TTh5M7_R76uRO91A,6608
 address_formatter/version.py,sha256=Q8raD6k02z4DoYniAz3iui5d6EdM1el95SMTLXJbeCA,18
+cwaddressformatter/.DS_Store,sha256=JACaso_PI4pfKHBxlOdqlRqU4OjRSCnlEjOmmIoGAf0,6148
 cwaddressformatter/__init__.py,sha256=3e8um1-lzVyp4LEDX_nV5yrFnPLEnmDOgCQDRkhXkEY,143
-cwaddressformatter/main.py,sha256=hSZTIwSFKxWsY6q9Zb1QdvLV9Jga4c5PlxVeCQTfVRs,8150
-cwaddressformatter/opendata111road.csv,sha256=CpDjO5XYqhxQEBmVg1PWcn1PN5Yc_T0l7xApinkxw34,1416653
-cwaddressformatter/version.py,sha256=K4bqp4JdOs9KHYMltFboNleHcCgvR1V7uAJwB8wlYQw,18
-cwaddressformatter-0.1.1.dist-info/METADATA,sha256=7rMVUPA1Du9ezZsIWlTfBkSCWB7aimr9F4MX8S0NZbc,3313
-cwaddressformatter-0.1.1.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-cwaddressformatter-0.1.1.dist-info/entry_points.txt,sha256=Pd9sw7w4pm-BMSffmkbjCvdtHwd6Fqzizk1tUoacTWM,64
-cwaddressformatter-0.1.1.dist-info/top_level.txt,sha256=8bk29FtgxiLt5rjWSr9mzI7cAeReWxaOiyU1UbYiAeo,19
-cwaddressformatter-0.1.1.dist-info/RECORD,,
+cwaddressformatter/main.py,sha256=SYXr_swxmc3qK0SnwnZUKSU0fAN6c8LN-EbE0lZs8jU,8714
+cwaddressformatter/opendata111road.csv,sha256=qm5hD9pKA9ctJOUYcJXoSmS22vmTOVrY523pEXewX-4,1416702
+cwaddressformatter/version.py,sha256=3ITyQfKn-h4AMdaHk5rHJaliZbCnbLZ7O3QQnAJH8yI,18
+cwaddressformatter-0.1.2.dist-info/METADATA,sha256=4W5Z48FwT6_OvHhDYpk7VvW45zUUlQluO11OiFZdBzo,3481
+cwaddressformatter-0.1.2.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+cwaddressformatter-0.1.2.dist-info/entry_points.txt,sha256=Pd9sw7w4pm-BMSffmkbjCvdtHwd6Fqzizk1tUoacTWM,64
+cwaddressformatter-0.1.2.dist-info/top_level.txt,sha256=8bk29FtgxiLt5rjWSr9mzI7cAeReWxaOiyU1UbYiAeo,19
+cwaddressformatter-0.1.2.dist-info/RECORD,,
```

