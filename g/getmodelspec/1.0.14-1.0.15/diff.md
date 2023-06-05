# Comparing `tmp/getmodelspec-1.0.14.tar.gz` & `tmp/getmodelspec-1.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\getmodelspec-1.0.14.tar", last modified: Mon Jun  5 11:22:04 2023, max compression
+gzip compressed data, was "dist\getmodelspec-1.0.15.tar", last modified: Mon Jun  5 15:48:15 2023, max compression
```

## Comparing `getmodelspec-1.0.14.tar` & `getmodelspec-1.0.15.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 11:22:04.000000 getmodelspec-1.0.14/
--rw-rw-rw-   0        0        0      126 2023-06-05 11:22:04.000000 getmodelspec-1.0.14/PKG-INFO
--rw-rw-rw-   0        0        0       61 2023-06-04 23:49:21.000000 getmodelspec-1.0.14/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 11:22:04.000000 getmodelspec-1.0.14/getmodelspec/
--rw-rw-rw-   0        0        0      117 2023-06-05 07:20:46.000000 getmodelspec-1.0.14/getmodelspec/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 11:22:04.000000 getmodelspec-1.0.14/getmodelspec/src/
--rw-rw-rw-   0        0        0        0 2023-06-05 07:20:11.000000 getmodelspec-1.0.14/getmodelspec/src/__init__.py
--rw-rw-rw-   0        0        0     8327 2023-06-05 11:15:14.000000 getmodelspec-1.0.14/getmodelspec/src/sony.py
-drwxrwxrwx   0        0        0        0 2023-06-05 11:22:04.000000 getmodelspec-1.0.14/getmodelspec/tools/
--rw-rw-rw-   0        0        0        0 2023-06-05 07:20:04.000000 getmodelspec-1.0.14/getmodelspec/tools/__init__.py
--rw-rw-rw-   0        0        0      906 2023-06-05 11:15:14.000000 getmodelspec-1.0.14/getmodelspec/tools/webdriver.py
-drwxrwxrwx   0        0        0        0 2023-06-05 11:22:04.000000 getmodelspec-1.0.14/getmodelspec.egg-info/
--rw-rw-rw-   0        0        0      126 2023-06-05 11:22:04.000000 getmodelspec-1.0.14/getmodelspec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      378 2023-06-05 11:22:04.000000 getmodelspec-1.0.14/getmodelspec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 11:22:04.000000 getmodelspec-1.0.14/getmodelspec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-05 11:22:04.000000 getmodelspec-1.0.14/getmodelspec.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       13 2023-06-05 11:22:04.000000 getmodelspec-1.0.14/getmodelspec.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-05 11:22:04.000000 getmodelspec-1.0.14/getmodelspec.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 11:22:04.000000 getmodelspec-1.0.14/setup.cfg
--rw-rw-rw-   0        0        0      413 2023-06-05 11:21:48.000000 getmodelspec-1.0.14/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:48:15.000000 getmodelspec-1.0.15/
+-rw-rw-rw-   0        0        0      126 2023-06-05 15:48:15.000000 getmodelspec-1.0.15/PKG-INFO
+-rw-rw-rw-   0        0        0       61 2023-06-04 23:49:21.000000 getmodelspec-1.0.15/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 15:48:15.000000 getmodelspec-1.0.15/getmodelspec/
+-rw-rw-rw-   0        0        0      117 2023-06-05 07:20:46.000000 getmodelspec-1.0.15/getmodelspec/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:48:15.000000 getmodelspec-1.0.15/getmodelspec/src/
+-rw-rw-rw-   0        0        0        0 2023-06-05 07:20:11.000000 getmodelspec-1.0.15/getmodelspec/src/__init__.py
+-rw-rw-rw-   0        0        0     9866 2023-06-05 15:47:40.000000 getmodelspec-1.0.15/getmodelspec/src/sony.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:48:15.000000 getmodelspec-1.0.15/getmodelspec/tools/
+-rw-rw-rw-   0        0        0        0 2023-06-05 07:20:04.000000 getmodelspec-1.0.15/getmodelspec/tools/__init__.py
+-rw-rw-rw-   0        0        0      906 2023-06-05 14:59:18.000000 getmodelspec-1.0.15/getmodelspec/tools/webdriver.py
+drwxrwxrwx   0        0        0        0 2023-06-05 15:48:15.000000 getmodelspec-1.0.15/getmodelspec.egg-info/
+-rw-rw-rw-   0        0        0      126 2023-06-05 15:48:15.000000 getmodelspec-1.0.15/getmodelspec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      378 2023-06-05 15:48:15.000000 getmodelspec-1.0.15/getmodelspec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 15:48:15.000000 getmodelspec-1.0.15/getmodelspec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-05 15:48:15.000000 getmodelspec-1.0.15/getmodelspec.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       13 2023-06-05 15:48:15.000000 getmodelspec-1.0.15/getmodelspec.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-05 15:48:15.000000 getmodelspec-1.0.15/getmodelspec.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 15:48:15.000000 getmodelspec-1.0.15/setup.cfg
+-rw-rw-rw-   0        0        0      413 2023-06-05 15:47:57.000000 getmodelspec-1.0.15/setup.py
```

### Comparing `getmodelspec-1.0.14/getmodelspec/src/sony.py` & `getmodelspec-1.0.15/getmodelspec/src/sony.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,46 +16,57 @@
 class GetSONY:
     def __init__(self):
         self.watingTime = 5
         pass
 
     def getModels(self) -> pd.DataFrame:
         #
-        # ## 메인 페이지에서 시리즈를 추출
-        # seriesUrls = self.getPage1st(url= 'https://electronics.sony.com/tv-video/televisions/c/all-tvs')
+        ## 메인 페이지에서 시리즈를 추출
+        seriesUrls = self.getPage1st(url= 'https://electronics.sony.com/tv-video/televisions/c/all-tvs')
+
+        # ==========================================================================
+        self.backUp(seriesUrls, "seriesUrls")
+        # ==========================================================================
+
+        ## 서브 시리즈 페이지에서 모델을 추출
+        dictAllSeries = {}
+        for url in seriesUrls:
+            dictSeries = self.getPage2nd(url=url)
+            print(dictSeries)
+            dictAllSeries.update(dictSeries)
+        print("Number of all Series:", len(dictAllSeries))
+        #
         #
         # # ==========================================================================
-        # self.backUp(seriesUrls, "seriesUrls")
+        self.backUp(dictAllSeries, "dictAllSeries")
+        # with open(f"dictAllSeries.pickle", "rb") as file:
+        #     dictAllSeries = pickle.load(file)
+
+        # dictAllSeries = {"y":"https://electronics.sony.com/tv-video/televisions/all-tvs/p/kd43x80k",
+        #                 "w":"https://electronics.sony.com/tv-video/televisions/all-tvs/p/kd85x80k",
+        #                  "c":"https://electronics.sony.com/tv-video/televisions/all-tvs/p/xr65x90l",
+        #                  "a":"https://electronics.sony.com/tv-video/televisions/all-tvs/p/xr98x90l",
+        #                  "h": "https://electronics.sony.com/tv-video/televisions/all-tvs/p/xr75x90l",
+        #                  "b":"https://electronics.sony.com/tv-video/televisions/all-tvs/p/xr65x90ck",
+        #                  "t": "https://electronics.sony.com/tv-video/televisions/all-tvs/p/xr55x90l"}
         # # ==========================================================================
-        #
-        # ## 서브 시리즈 페이지에서 모델을 추출
-        # dictAllSeries = {}
-        # for url in seriesUrls:
-        #     dictSeries = self.getPage2nd(url=url)
-        #     print(dictSeries)
-        #     dictAllSeries.update(dictSeries)
-        # print("Number of all Series:", len(dictAllSeries))
-        # #
-        # #
-        # # # ==========================================================================
-        # self.backUp(dictAllSeries, "dictAllSeries")
-        with open(f"dictAllSeries.pickle", "rb") as file:
-            dictAllSeries = pickle.load(file)
-
-        # dictAllSeries = {"w":"https://electronics.sony.com/tv-video/televisions/all-tvs/p/kd85x80k", "c":"https://electronics.sony.com/tv-video/televisions/all-tvs/p/xr55x90l ", "a":"https://electronics.sony.com/tv-video/televisions/all-tvs/p/xr85x90l", "b":"https://electronics.sony.com/tv-video/televisions/all-tvs/p/xr98x90l"}
-        # ==========================================================================
 
         ## 모든 모델 리스트를 추출
         dictModels = {}
         for model_url in dictAllSeries.values():
             print(model_url)
-            try:
-                dictModels.update(self.getPage3rd(model_url))
-            except Exception as e:
-                print(model_url, f"\n getPage3rd error ({e})")
+            dictModels.update(self.getPage3rd(model_url))
+            # for cntTry in range(5):
+            #     try:
+            #         dictModels.update(self.getPage3rd(model_url))
+            #         break
+            #     except Exception as e:
+            #         print(model_url, f"{cntTry} try \n getPage3rd error")
+            #         pass
+
         dfModels = pd.DataFrame.from_dict(dictModels, orient="index")
         return dfModels
 
     ###=====================get info main page====================================##
     def getPage1st(self, url:str) -> set:
         set_mainSeries = set()
         scrolling_cnt: int = 10
@@ -79,15 +90,14 @@
     ###=====================get info Sub page====================================##
     def getPage2nd(self, url:str) -> dict:
         dictSeries = {}
 
         wd = WebDriver.get_crome()
         wd.get(url=url)
         self.waitingPage(5)
-
         elements = wd.find_elements(By.CLASS_NAME, 'custom-variant-selector__item')  ## 시리즈의 모든 인치 모델 가져 옴
 
         for element in elements:
             try:
                 element_url = element.get_attribute('href')
                 label = self.getNamefromURL(element_url)
                 dictSeries[label]=element_url # url 만 저장 함
@@ -96,83 +106,99 @@
                 pass
         wd.quit()
         print(f"Number of SONY {self.getNamefromURL(url)[4:]} series:", len(dictSeries))
         return dictSeries
 
     ###======================final stage===============================##
     def getPage3rd(self, url:str) -> dict:
-        dictSpec = {}
 
-        wd = WebDriver.get_crome()
-        wd.get(url=url)
-        wait = WebDriverWait(wd, self.watingTime)
-        self.waitingPage(5)
+        for cntTry in range(5):
+            try:
+                dictSpec = {}
+                wd = WebDriver.get_crome()
+                wd.get(url=url)
+                wait = WebDriverWait(wd, self.watingTime)
+                # self.waitingPage(1)
+
+                #모델 정보 확인
+                model = wait.until(EC.presence_of_element_located((By.CLASS_NAME, 'product-intro__code'))).text.replace("Model: ", "")
+                dictSpec["Descr"] = wait.until(EC.presence_of_element_located((By.CLASS_NAME, 'product-intro__title'))).text.strip()
 
-        #모델 정보 확인
-        model = wait.until(EC.presence_of_element_located((By.CLASS_NAME, 'product-intro__code'))).text.replace("Model: ", "")
-        dictSpec["Descr"] = wait.until(EC.presence_of_element_located((By.CLASS_NAME, 'product-intro__title'))).text.strip()
-
-        #가격 정보 확인
-        try: dictSpec["price"] = wait.until(EC.presence_of_element_located((By.CLASS_NAME, 'custom-product-summary__price'))).text
-        except Exception as e:
-            print("price error", e)
-            dictSpec["price"] = ""
-
-        # print(dictSpec["price"])
-
-        #이미지 정보 및 url 저장
-        dictSpec["src_url"] = url
-        dictSpec["Img_url"] = wait.until(EC.presence_of_element_located((By.XPATH, '//app-custom-cx-media//img'))).get_attribute('src')
-# ====
-
-        # 스크롤 다운
-        for i in range(25):
-            ActionChains(wd).key_down(Keys.DOWN).perform()
-        self.waitingPage(5)
+                #가격 정보 확인
+                try: dictSpec["price"] = wait.until(EC.presence_of_element_located((By.CLASS_NAME, 'custom-product-summary__price'))).text
+                except Exception as e:
+                    print("price error")
+                    dictSpec["price"] = ""
 
-        # print("spec open")
-        # spec 열기
-        click_element = wd.find_element(By.XPATH, '//*[@id="PDPSpecificationsLink"]/cx-icon')
-        # click_element = wd.find_elements(By.CSS_SELECTOR, ".cx-icon.black_plus")[0]
-        ActionChains(wd).move_to_element(click_element).click().perform()
-        self.waitingPage(5)
+                #이미지 정보 및 url 저장
+                dictSpec["src_url"] = url
+                dictSpec["Img_url"] = wait.until(EC.presence_of_element_located((By.XPATH, '//app-custom-cx-media//img'))).get_attribute('src')
+
+
+                # print("spec open")
+                # spec 열기
+                # for cnt in range(20):
+                #     try:
+                #         click_element = wd.find_element(By.ID, "PDPSpecificationsLink")
+                #         click_element.click()
+                #         break
+                #     except Exception as e:
+                #         ActionChains(wd).key_down(Keys.DOWN).perform()
+                # print(f"try to open spec: {cnt}")
+                element_openSpec = wd.find_element(By.ID, "PDPSpecificationsLink")
+                element_openSpec.click()
+                # wd.find_element(By.ID, "PDPSpecificationsLink").click()
+                self.waitingPage(1)
+
+                # print("see more")
+                # 클래스에 매칭되는 see_more 요소 모두
+                # for cnt in range(20):
+                #     try:
+                #         click_element = wd.find_element(By.CLASS_NAME, 'sony-btn.sony-btn--primary--inverse')
+                #         click_element.click()
+                #         break
+                #     except Exception as e:
+                #         ActionChains(wd).key_down(Keys.DOWN).perform()
+                # print(f"try to open pop: {cnt}")
+
+                try:
+                    element_seeMore = wd.find_element(By.XPATH, '//*[@id="PDPOveriewLink"]/div[1]/div/div/div[2]/div/app-product-specification/div/div[2]/div[3]/button')
+                    element_seeMore.click()
+                except:
+                    element_seeMore = wd.find_element(By.XPATH, '//*[@id="PDPOveriewLink"]/div[1]/div/div/div[2]/div/app-product-specification/div/div[2]/div[2]/button')
+                    element_seeMore.click()
+                self.waitingPage(1)
+
+
+                # print("pop up")
+                #스펙 팝업 창의 스크롤 선택 후 클릭: 팝업 창으로 이동
+                wd.find_element(By.ID, "ngb-nav-0-panel").click()
+
+                # print("get info")
+                #스펙 팝업 창의 스펙 가져오기
+                for cnt in range(15):
+                    elements = wd.find_elements(By.CLASS_NAME, "full-specifications__specifications-single-card__sub-list")
+                    for element in elements:
+                        soup = BeautifulSoup(element.get_attribute("innerHTML"), 'html.parser')
+                        dictSpec.update(self.SoupToDict(soup))
+                    ActionChains(wd).key_down(Keys.PAGE_DOWN).perform()
+                # self.waitingPage(1)
+
+                wd.quit()
+                dictModel = {model: dictSpec}
+                print(f"{model}\n", dictModel)
+                return dictModel
 
-        # 스크롤 다운
-        for i in range(20):
-            ActionChains(wd).key_down(Keys.DOWN).perform()
-        self.waitingPage(10)
-
-        # print("see more")
-        # 클래스에 매칭되는 see_more 요소 모두
-        click_element = wd.find_element(By.XPATH, '//*[@id="PDPOveriewLink"]/div[1]/div/div/div[2]/div/app-product-specification/div/div[2]/div[3]/button')
-        # click_element = wd.find_elements(By.CSS_SELECTOR, '.cx-icon.see-more-features.atom-icon-arrow-down-blue')[1]  # 두 번째 요소 클릭
-        click_element.click()
-        self.waitingPage(5)
+            except Exception as e:
+                print(f"getPage3rd error: {model} try {cntTry+1}/5")
+                wd.quit()
+                pass
 
-        # print("pop up")
-        #스펙 팝업 창의 스크롤 선택 후 클릭: 팝업 창으로 이동
-        scroll_element = wd.find_element(By.CLASS_NAME, "ps__rail-y")
-        scroll_element.click()
-
-        # print("get info")
-        #스펙 팝업 창의 스펙 가져오기
-        for i in range(15):
-            elements = wd.find_elements(By.CLASS_NAME, "full-specifications__specifications-single-card__sub-list")
-            for element in elements:
-                soup = BeautifulSoup(element.get_attribute("innerHTML"), 'html.parser')
-                dictSpec.update(self.SoupToDict(soup))
 
-            ActionChains(wd).key_down(Keys.PAGE_DOWN).perform()
-            time.sleep(1)
-            # wd.find_element(By.TAG_NAME, 'body').send_keys(Keys.PAGE_DOWN)
-        wd.quit()
 
-        dictModel = {model: dictSpec}
-        print(f"{model}\n", dictModel)
-        return dictModel
 
 # ===============================
 
     def getNamefromURL(self, url):
         """
         마지막 / 이후 문자만 가져 옴
         """
```

### Comparing `getmodelspec-1.0.14/getmodelspec/tools/webdriver.py` & `getmodelspec-1.0.15/getmodelspec/tools/webdriver.py`

 * *Files identical despite different names*

