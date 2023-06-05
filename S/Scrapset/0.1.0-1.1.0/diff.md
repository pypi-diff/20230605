# Comparing `tmp/Scrapset-0.1.0-py3-none-any.whl.zip` & `tmp/Scrapset-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3734 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat     4483 b- defN 23-Jun-05 15:24 Scrapset/Scrapset.py
+Zip file size: 3749 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat     4485 b- defN 23-Jun-05 15:51 Scrapset/Scrapset.py
 -rw-rw-rw-  2.0 fat       67 b- defN 23-Jun-05 15:28 Scrapset/__init__.py
--rw-rw-rw-  2.0 fat     2763 b- defN 23-Jun-05 15:44 Scrapset-0.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-05 15:44 Scrapset-0.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat      626 b- defN 23-Jun-05 15:44 Scrapset-0.1.0.dist-info/licence.txt
--rw-rw-rw-  2.0 fat        9 b- defN 23-Jun-05 15:44 Scrapset-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      545 b- defN 23-Jun-05 15:44 Scrapset-0.1.0.dist-info/RECORD
-7 files, 8585 bytes uncompressed, 2764 bytes compressed:  67.8%
+-rw-rw-rw-  2.0 fat     2789 b- defN 23-Jun-05 16:08 Scrapset-1.1.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-05 16:08 Scrapset-1.1.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat      632 b- defN 23-Jun-05 16:08 Scrapset-1.1.0.dist-info/licence.txt
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Jun-05 16:08 Scrapset-1.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      545 b- defN 23-Jun-05 16:08 Scrapset-1.1.0.dist-info/RECORD
+7 files, 8619 bytes uncompressed, 2779 bytes compressed:  67.8%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: Scrapset/Scrapset.py
 Comment: 
 
 Filename: Scrapset/__init__.py
 Comment: 
 
-Filename: Scrapset-0.1.0.dist-info/METADATA
+Filename: Scrapset-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: Scrapset-0.1.0.dist-info/WHEEL
+Filename: Scrapset-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: Scrapset-0.1.0.dist-info/licence.txt
+Filename: Scrapset-1.1.0.dist-info/licence.txt
 Comment: 
 
-Filename: Scrapset-0.1.0.dist-info/top_level.txt
+Filename: Scrapset-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: Scrapset-0.1.0.dist-info/RECORD
+Filename: Scrapset-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Scrapset/Scrapset.py

```diff
@@ -47,14 +47,15 @@
                     list_of_dic['all_details'].append(data_set_details)
                     list_of_dic['up_vote'].append(data_set_upvote)
             driver.quit()
             return list_of_dic
         except:
             logging.error("Invalid Url")
 
+
 class DataDotGov:
     def web_driver_chrome(self):
         options = webdriver.ChromeOptions()
         options.add_argument("--verbose")
         options.add_argument('--no-sandbox')
         # options.add_argument('--headless')
         options.add_argument('--disable-gpu')
```

## Comparing `Scrapset-0.1.0.dist-info/METADATA` & `Scrapset-1.1.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: Scrapset
-Version: 0.1.0
-Summary: Scraping Dataset sites
+Version: 1.1.0
+Summary: DataScraper: Effortless Dataset Extraction
 Author: Ibrahim
 Author-email: string2025@gmail.com
 Description-Content-Type: text/markdown
 License-File: licence.txt
 Requires-Dist: selenium
 
 # Dataset Scraper (Scrapset)
 
 
+
 Scrapset is a Python module specifically created for web scraping data from websites like Kaggle and Data.gov. It simplifies the task of extracting dataset information such as titles, upvotes (for Kaggle), and recent views (for Data.gov).
 
 By utilizing the Scrapset module, you can automate the retrieval of dataset details from these platforms. This can be beneficial for various purposes such as data analysis, research, or developing machine learning models. The module employs the Selenium library to interact with the websites and extract the desired data.
 
 With Scrapset, you can quickly and easily scrape dataset information, empowering you to work with valuable data from Kaggle, Data.gov, and similar websites.
 
 
@@ -33,27 +34,29 @@
 Methods:
 web_driver_chrome(): Initializes and returns a Selenium Chrome WebDriver with customized options for scraping Data.gov datasets.
 
 data_set_page(url, last_page, initial_page): Scrapes the titles, recent views, and authors of datasets from Data.gov. The method takes the url of the Data.gov datasets page, the last_page number to scrape up to, and the initial_page number to start scraping from. It returns a dictionary containing the scraped dataset information.
 
 # Example code to extract titles of datasets from Data.gov
 
+
 ```
 
 import kaggle_datasets as m
 import pandas as pd
 df=m.DataDotGov()
 data=df.data_set_page('https://catalog.data.gov',last_page=10,initial_page=5)
 datf=pd.DataFrame(data)
 datf.to_csv('datagov.csv',index=False)
 
 ```
 
 # Example code to extract titles, upvote, Usability index  of datasets from kaggle
 
+
 ```
 
 import kaggle_datasets as m
 import pandas as pd
 df=m.KaggleDataSet()
 data=df.data_set_page('https://kaggle.com',last_page=10,initial_page=5)
 datf=pd.DataFrame(data)
```

## Comparing `Scrapset-0.1.0.dist-info/licence.txt` & `Scrapset-1.1.0.dist-info/licence.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,5 +1,7 @@
 This module is open source and freely available for anyone to use and contribute to. There are no restrictions on the use of this module, and we encourage everyone to take advantage of its features and capabilities.
 
 As the creator of this module, Ibrahim welcomes contributions from the community to help improve and expand its functionality. Whether you are a developer, a data scientist, or just someone who is passionate about technology, you are invited to contribute to this project and help make it even better.
 
-Thank you for your interest in this module, and we look forward to seeing what you can create with it.
+Thank you for your interest in this module, and we look forward to seeing what you can create with it.
+
+
```

## Comparing `Scrapset-0.1.0.dist-info/RECORD` & `Scrapset-1.1.0.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Scrapset/Scrapset.py,sha256=kloQnqJbQlmK6-qObATuhiMwC_5MDJw5NjV-m2iW5n4,4483
+Scrapset/Scrapset.py,sha256=cpgoiFbf14lkLS5DR0X992HwU2r7o3jRc0fAZPiEqeE,4485
 Scrapset/__init__.py,sha256=_WwZDcTXBfm9fjdR6bFA36VcSgVsVmDVrf-fguj1UhQ,67
-Scrapset-0.1.0.dist-info/METADATA,sha256=krUS-8RvvPuKG8-ahimLZ5nt1aDIELkm2fQg5FIHqRE,2763
-Scrapset-0.1.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-Scrapset-0.1.0.dist-info/licence.txt,sha256=zoLuMgX2_oYN9WLdnLbRlgRbmg9hFq5CILuI6mrr9fU,626
-Scrapset-0.1.0.dist-info/top_level.txt,sha256=DZOAmLHm1ITM5F5fGFEDfQ6NnQAwotBcWCwj5PdhqNw,9
-Scrapset-0.1.0.dist-info/RECORD,,
+Scrapset-1.1.0.dist-info/METADATA,sha256=caMjZg0NIBLA_vSWIoAK1ekl-2wmVk0WdGCJ3c7LQEI,2789
+Scrapset-1.1.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+Scrapset-1.1.0.dist-info/licence.txt,sha256=i79SE9-rWtU07j8Skpf29SRVwtEfuu34njYipmNzLGU,632
+Scrapset-1.1.0.dist-info/top_level.txt,sha256=DZOAmLHm1ITM5F5fGFEDfQ6NnQAwotBcWCwj5PdhqNw,9
+Scrapset-1.1.0.dist-info/RECORD,,
```

