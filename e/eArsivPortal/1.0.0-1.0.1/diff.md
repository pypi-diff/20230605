# Comparing `tmp/eArsivPortal-1.0.0.tar.gz` & `tmp/eArsivPortal-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eArsivPortal-1.0.0.tar", last modified: Mon May 29 16:30:56 2023, max compression
+gzip compressed data, was "eArsivPortal-1.0.1.tar", last modified: Mon Jun  5 07:51:17 2023, max compression
```

## Comparing `eArsivPortal-1.0.0.tar` & `eArsivPortal-1.0.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:30:56.781139 eArsivPortal-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-29 16:30:26.000000 eArsivPortal-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-29 16:30:26.000000 eArsivPortal-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6822 2023-05-29 16:30:56.781139 eArsivPortal-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-05-29 16:30:26.000000 eArsivPortal-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:30:56.781139 eArsivPortal-1.0.0/eArsivPortal/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:30:56.781139 eArsivPortal-1.0.0/eArsivPortal/Core/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-29 16:30:26.000000 eArsivPortal-1.0.0/eArsivPortal/Core/Hatalar.py
--rw-r--r--   0 runner    (1001) docker     (123)     9677 2023-05-29 16:30:26.000000 eArsivPortal-1.0.0/eArsivPortal/Core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:30:56.781139 eArsivPortal-1.0.0/eArsivPortal/Libs/
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-05-29 16:30:26.000000 eArsivPortal-1.0.0/eArsivPortal/Libs/FaturaVer.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-29 16:30:26.000000 eArsivPortal-1.0.0/eArsivPortal/Libs/Oturum.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-29 16:30:26.000000 eArsivPortal-1.0.0/eArsivPortal/Libs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:30:56.781139 eArsivPortal-1.0.0/eArsivPortal/Models/
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-29 16:30:26.000000 eArsivPortal-1.0.0/eArsivPortal/Models/Komutlar.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-29 16:30:26.000000 eArsivPortal-1.0.0/eArsivPortal/Models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-29 16:30:26.000000 eArsivPortal-1.0.0/eArsivPortal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:30:56.781139 eArsivPortal-1.0.0/eArsivPortal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6822 2023-05-29 16:30:56.000000 eArsivPortal-1.0.0/eArsivPortal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-29 16:30:56.000000 eArsivPortal-1.0.0/eArsivPortal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 16:30:56.000000 eArsivPortal-1.0.0/eArsivPortal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-29 16:30:56.000000 eArsivPortal-1.0.0/eArsivPortal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-29 16:30:56.000000 eArsivPortal-1.0.0/eArsivPortal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 16:30:56.785139 eArsivPortal-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-29 16:30:26.000000 eArsivPortal-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:51:17.303589 eArsivPortal-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-05 07:50:48.000000 eArsivPortal-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-05 07:50:48.000000 eArsivPortal-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6907 2023-06-05 07:51:17.303589 eArsivPortal-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-06-05 07:50:48.000000 eArsivPortal-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:51:17.299589 eArsivPortal-1.0.1/eArsivPortal/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:51:17.303589 eArsivPortal-1.0.1/eArsivPortal/Core/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-05 07:50:48.000000 eArsivPortal-1.0.1/eArsivPortal/Core/Hatalar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9672 2023-06-05 07:50:48.000000 eArsivPortal-1.0.1/eArsivPortal/Core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:51:17.303589 eArsivPortal-1.0.1/eArsivPortal/Libs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-06-05 07:50:48.000000 eArsivPortal-1.0.1/eArsivPortal/Libs/FaturaVer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-05 07:50:48.000000 eArsivPortal-1.0.1/eArsivPortal/Libs/Oturum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-05 07:50:48.000000 eArsivPortal-1.0.1/eArsivPortal/Libs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:51:17.303589 eArsivPortal-1.0.1/eArsivPortal/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-05 07:50:48.000000 eArsivPortal-1.0.1/eArsivPortal/Models/Komutlar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-05 07:50:48.000000 eArsivPortal-1.0.1/eArsivPortal/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-05 07:50:48.000000 eArsivPortal-1.0.1/eArsivPortal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:51:17.303589 eArsivPortal-1.0.1/eArsivPortal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6907 2023-06-05 07:51:17.000000 eArsivPortal-1.0.1/eArsivPortal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-05 07:51:17.000000 eArsivPortal-1.0.1/eArsivPortal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 07:51:17.000000 eArsivPortal-1.0.1/eArsivPortal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-05 07:51:17.000000 eArsivPortal-1.0.1/eArsivPortal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-05 07:51:17.000000 eArsivPortal-1.0.1/eArsivPortal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 07:51:17.303589 eArsivPortal-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-05 07:50:48.000000 eArsivPortal-1.0.1/setup.py
```

### Comparing `eArsivPortal-1.0.0/LICENSE` & `eArsivPortal-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `eArsivPortal-1.0.0/PKG-INFO` & `eArsivPortal-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eArsivPortal
-Version: 1.0.0
+Version: 1.0.1
 Summary: GİB e-Arşiv Portal e-Fatura Oluşturucu
 Home-page: https://github.com/keyiflerolsun/eArsivPortal
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: eArsivPortal,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
@@ -182,15 +182,20 @@
 
 #--------------------------------------------------------------#
 
 FaturaSil(mesaj='2 fatura başarıyla silindi.')
 ```
 
 ```python
-portal.gib_sms_onay(faturalar[3], input("SMS Doğrulama Kodu: "))
+imza = portal.gib_imza()
+portal.gib_sms_onay(
+    faturalar = faturalar[3],
+    oid       = imza.oid,
+    sifre     = input("SMS Doğrulama Kodu: ")
+)
 
 #--------------------------------------------------------------#
 
 GibSMSOnay(mesaj='SMS şifreniz doğrulandı, işlem başarılı.')
 ```
 
 ```python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: eArsivPortal Version: 1.0.0 Summary: GÄ°B e-ArÅiv
+Metadata-Version: 2.1 Name: eArsivPortal Version: 1.0.1 Summary: GÄ°B e-ArÅiv
 Portal e-Fatura OluÅturucu Home-page: https://github.com/keyiflerolsun/
 eArsivPortal Author: keyiflerolsun Author-email: keyiflerolsun@gmail.com
 License: GPLv3+ Keywords: eArsivPortal,KekikAkademi,keyiflerolsun Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: GNU General Public License v3 or later (GPLv3+) Classifier: Programming
 Language :: Python :: 3 Requires-Python: >=3.10 Description-Content-Type: text/
 markdown License-File: LICENSE # ð§¾ eArsivPortal [![Boyut](https://
@@ -66,18 +66,19 @@
 onayDurumu='OnaylandÄ±', ettn='8cb401e3-ca6d-442a-8389-c4d87c9eb67c' ) ] ```
 ```python html_fatura = portal.fatura_html( ettn = faturalar[0].ettn
 onay_durumu = faturalar[0].onayDurumu ) with open(f"{faturalar
 [0].aliciUnvanAdSoyad}.html", "w", encoding="utf-8") as dosya: dosya.write
 (html_fatura) ``` ```python portal.fatura_sil( faturalar = [faturalar[0],
 faturalar[1]] aciklama = "Fatura silindi." ) #---------------------------------
 -----------------------------# FaturaSil(mesaj='2 fatura baÅarÄ±yla silindi.')
-``` ```python portal.gib_sms_onay(faturalar[3], input("SMS DoÄrulama Kodu: "))
-#--------------------------------------------------------------# GibSMSOnay
-(mesaj='SMS Åifreniz doÄrulandÄ±, iÅlem baÅarÄ±lÄ±.') ``` ```python
-portal.cikis_yap() ``` ## ð Telif HakkÄ± ve Lisans * *Copyright (C) 2023 by*
-[keyiflerolsun](https://github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL
-PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/
-eArsivPortal/blob/master/LICENSE) *KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ##
-â»ï¸ Ä°letiÅim *Benimle iletiÅime geÃ§mek isterseniz, **Telegram**'dan
-mesaj gÃ¶ndermekten Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ##
-ð¸ BaÄÄ±Å Yap **[âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)**
-*** > **[@KekikAkademi](https://t.me/KekikAkademi)** *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
+``` ```python imza = portal.gib_imza() portal.gib_sms_onay( faturalar =
+faturalar[3], oid = imza.oid, sifre = input("SMS DoÄrulama Kodu: ") ) #-------
+-------------------------------------------------------# GibSMSOnay(mesaj='SMS
+Åifreniz doÄrulandÄ±, iÅlem baÅarÄ±lÄ±.') ``` ```python portal.cikis_yap()
+``` ## ð Telif HakkÄ± ve Lisans * *Copyright (C) 2023 by* [keyiflerolsun]
+(https://github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL PUBLIC LICENSE
+Version 3, 29 June 2007](https://github.com/keyiflerolsun/eArsivPortal/blob/
+master/LICENSE) *KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ## â»ï¸ Ä°letiÅim
+*Benimle iletiÅime geÃ§mek isterseniz, **Telegram**'dan mesaj gÃ¶ndermekten
+Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ## ð¸ BaÄÄ±Å Yap **
+[âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)** *** > **
+[@KekikAkademi](https://t.me/KekikAkademi)** *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
```

### Comparing `eArsivPortal-1.0.0/README.md` & `eArsivPortal-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -166,15 +166,20 @@
 
 #--------------------------------------------------------------#
 
 FaturaSil(mesaj='2 fatura başarıyla silindi.')
 ```
 
 ```python
-portal.gib_sms_onay(faturalar[3], input("SMS Doğrulama Kodu: "))
+imza = portal.gib_imza()
+portal.gib_sms_onay(
+    faturalar = faturalar[3],
+    oid       = imza.oid,
+    sifre     = input("SMS Doğrulama Kodu: ")
+)
 
 #--------------------------------------------------------------#
 
 GibSMSOnay(mesaj='SMS şifreniz doğrulandı, işlem başarılı.')
 ```
 
 ```python
```

#### html2text {}

```diff
@@ -59,18 +59,19 @@
 onayDurumu='OnaylandÄ±', ettn='8cb401e3-ca6d-442a-8389-c4d87c9eb67c' ) ] ```
 ```python html_fatura = portal.fatura_html( ettn = faturalar[0].ettn
 onay_durumu = faturalar[0].onayDurumu ) with open(f"{faturalar
 [0].aliciUnvanAdSoyad}.html", "w", encoding="utf-8") as dosya: dosya.write
 (html_fatura) ``` ```python portal.fatura_sil( faturalar = [faturalar[0],
 faturalar[1]] aciklama = "Fatura silindi." ) #---------------------------------
 -----------------------------# FaturaSil(mesaj='2 fatura baÅarÄ±yla silindi.')
-``` ```python portal.gib_sms_onay(faturalar[3], input("SMS DoÄrulama Kodu: "))
-#--------------------------------------------------------------# GibSMSOnay
-(mesaj='SMS Åifreniz doÄrulandÄ±, iÅlem baÅarÄ±lÄ±.') ``` ```python
-portal.cikis_yap() ``` ## ð Telif HakkÄ± ve Lisans * *Copyright (C) 2023 by*
-[keyiflerolsun](https://github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL
-PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/
-eArsivPortal/blob/master/LICENSE) *KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ##
-â»ï¸ Ä°letiÅim *Benimle iletiÅime geÃ§mek isterseniz, **Telegram**'dan
-mesaj gÃ¶ndermekten Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ##
-ð¸ BaÄÄ±Å Yap **[âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)**
-*** > **[@KekikAkademi](https://t.me/KekikAkademi)** *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
+``` ```python imza = portal.gib_imza() portal.gib_sms_onay( faturalar =
+faturalar[3], oid = imza.oid, sifre = input("SMS DoÄrulama Kodu: ") ) #-------
+-------------------------------------------------------# GibSMSOnay(mesaj='SMS
+Åifreniz doÄrulandÄ±, iÅlem baÅarÄ±lÄ±.') ``` ```python portal.cikis_yap()
+``` ## ð Telif HakkÄ± ve Lisans * *Copyright (C) 2023 by* [keyiflerolsun]
+(https://github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL PUBLIC LICENSE
+Version 3, 29 June 2007](https://github.com/keyiflerolsun/eArsivPortal/blob/
+master/LICENSE) *KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ## â»ï¸ Ä°letiÅim
+*Benimle iletiÅime geÃ§mek isterseniz, **Telegram**'dan mesaj gÃ¶ndermekten
+Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ## ð¸ BaÄÄ±Å Yap **
+[âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)** *** > **
+[@KekikAkademi](https://t.me/KekikAkademi)** *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
```

### Comparing `eArsivPortal-1.0.0/eArsivPortal/Core/__init__.py` & `eArsivPortal-1.0.1/eArsivPortal/Core/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -232,15 +232,15 @@
                 "silinecekler" : self.__fatura_ver(faturalar),
                 "aciklama"     : aciklama
             }
         )
 
         return self.__nesne_ver("FaturaSil", {"mesaj": istek.get("data")})
 
-    def __gib_imza(self) -> BaseModel:
+    def gib_imza(self) -> BaseModel:
         telefon_istek = self.__kod_calistir(
             komut = self.komutlar.TELEFONNO_SORGULA,
             jp    = {}
         )
         telefon_veri = telefon_istek.get("data")
         telefon_no   = telefon_veri.get("telefon")
         if not telefon_no:
@@ -250,24 +250,24 @@
             komut = self.komutlar.SMSSIFRE_GONDER,
             jp    = {
                 "CEPTEL"  : telefon_no,
                 "KCEPTEL" : False,
                 "TIP"     : ""
             }
         )
-        print(f"`{telefon_no}` numarasına SMS gönderildi.")
+        print(f"\n[~] {telefon_no} numarasına SMS gönderildi.\n")
 
         return self.__nesne_ver("GibImza", sms_gonder.get("data"))
 
-    def gib_sms_onay(self, faturalar:list[dict] | dict, sifre:str) -> BaseModel:
+    def gib_sms_onay(self, faturalar:list[dict] | dict, oid:str, sifre:str) -> BaseModel:
         istek = self.__kod_calistir(
             komut = self.komutlar.SMSSIFRE_DOGRULA,
             jp    = {
                 "SIFRE" : sifre,
-                "OID"   : self.__gib_imza().oid,
+                "OID"   : oid,
                 "OPR"   : 1,
                 "DATA"  : self.__fatura_ver(faturalar),
             }
         )
         veri  = istek.get("data")
 
         return self.__nesne_ver("GibSMSOnay", {"mesaj": veri.get("msg")})
```

### Comparing `eArsivPortal-1.0.0/eArsivPortal/Libs/FaturaVer.py` & `eArsivPortal-1.0.1/eArsivPortal/Libs/FaturaVer.py`

 * *Files identical despite different names*

### Comparing `eArsivPortal-1.0.0/eArsivPortal/Libs/Oturum.py` & `eArsivPortal-1.0.1/eArsivPortal/Libs/Oturum.py`

 * *Files identical despite different names*

### Comparing `eArsivPortal-1.0.0/eArsivPortal/Models/Komutlar.py` & `eArsivPortal-1.0.1/eArsivPortal/Models/Komutlar.py`

 * *Files identical despite different names*

### Comparing `eArsivPortal-1.0.0/eArsivPortal.egg-info/PKG-INFO` & `eArsivPortal-1.0.1/eArsivPortal.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eArsivPortal
-Version: 1.0.0
+Version: 1.0.1
 Summary: GİB e-Arşiv Portal e-Fatura Oluşturucu
 Home-page: https://github.com/keyiflerolsun/eArsivPortal
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: eArsivPortal,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
@@ -182,15 +182,20 @@
 
 #--------------------------------------------------------------#
 
 FaturaSil(mesaj='2 fatura başarıyla silindi.')
 ```
 
 ```python
-portal.gib_sms_onay(faturalar[3], input("SMS Doğrulama Kodu: "))
+imza = portal.gib_imza()
+portal.gib_sms_onay(
+    faturalar = faturalar[3],
+    oid       = imza.oid,
+    sifre     = input("SMS Doğrulama Kodu: ")
+)
 
 #--------------------------------------------------------------#
 
 GibSMSOnay(mesaj='SMS şifreniz doğrulandı, işlem başarılı.')
 ```
 
 ```python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: eArsivPortal Version: 1.0.0 Summary: GÄ°B e-ArÅiv
+Metadata-Version: 2.1 Name: eArsivPortal Version: 1.0.1 Summary: GÄ°B e-ArÅiv
 Portal e-Fatura OluÅturucu Home-page: https://github.com/keyiflerolsun/
 eArsivPortal Author: keyiflerolsun Author-email: keyiflerolsun@gmail.com
 License: GPLv3+ Keywords: eArsivPortal,KekikAkademi,keyiflerolsun Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: GNU General Public License v3 or later (GPLv3+) Classifier: Programming
 Language :: Python :: 3 Requires-Python: >=3.10 Description-Content-Type: text/
 markdown License-File: LICENSE # ð§¾ eArsivPortal [![Boyut](https://
@@ -66,18 +66,19 @@
 onayDurumu='OnaylandÄ±', ettn='8cb401e3-ca6d-442a-8389-c4d87c9eb67c' ) ] ```
 ```python html_fatura = portal.fatura_html( ettn = faturalar[0].ettn
 onay_durumu = faturalar[0].onayDurumu ) with open(f"{faturalar
 [0].aliciUnvanAdSoyad}.html", "w", encoding="utf-8") as dosya: dosya.write
 (html_fatura) ``` ```python portal.fatura_sil( faturalar = [faturalar[0],
 faturalar[1]] aciklama = "Fatura silindi." ) #---------------------------------
 -----------------------------# FaturaSil(mesaj='2 fatura baÅarÄ±yla silindi.')
-``` ```python portal.gib_sms_onay(faturalar[3], input("SMS DoÄrulama Kodu: "))
-#--------------------------------------------------------------# GibSMSOnay
-(mesaj='SMS Åifreniz doÄrulandÄ±, iÅlem baÅarÄ±lÄ±.') ``` ```python
-portal.cikis_yap() ``` ## ð Telif HakkÄ± ve Lisans * *Copyright (C) 2023 by*
-[keyiflerolsun](https://github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL
-PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/
-eArsivPortal/blob/master/LICENSE) *KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ##
-â»ï¸ Ä°letiÅim *Benimle iletiÅime geÃ§mek isterseniz, **Telegram**'dan
-mesaj gÃ¶ndermekten Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ##
-ð¸ BaÄÄ±Å Yap **[âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)**
-*** > **[@KekikAkademi](https://t.me/KekikAkademi)** *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
+``` ```python imza = portal.gib_imza() portal.gib_sms_onay( faturalar =
+faturalar[3], oid = imza.oid, sifre = input("SMS DoÄrulama Kodu: ") ) #-------
+-------------------------------------------------------# GibSMSOnay(mesaj='SMS
+Åifreniz doÄrulandÄ±, iÅlem baÅarÄ±lÄ±.') ``` ```python portal.cikis_yap()
+``` ## ð Telif HakkÄ± ve Lisans * *Copyright (C) 2023 by* [keyiflerolsun]
+(https://github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL PUBLIC LICENSE
+Version 3, 29 June 2007](https://github.com/keyiflerolsun/eArsivPortal/blob/
+master/LICENSE) *KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ## â»ï¸ Ä°letiÅim
+*Benimle iletiÅime geÃ§mek isterseniz, **Telegram**'dan mesaj gÃ¶ndermekten
+Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ## ð¸ BaÄÄ±Å Yap **
+[âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)** *** > **
+[@KekikAkademi](https://t.me/KekikAkademi)** *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
```

### Comparing `eArsivPortal-1.0.0/setup.py` & `eArsivPortal-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 from io         import open
 
 setup(
     # ? Genel Bilgiler
     name         = "eArsivPortal",
-    version      = "1.0.0",
+    version      = "1.0.1",
     url          = "https://github.com/keyiflerolsun/eArsivPortal",
     description  = "GİB e-Arşiv Portal e-Fatura Oluşturucu",
     keywords     = ["eArsivPortal", "KekikAkademi", "keyiflerolsun"],
 
     author       = "keyiflerolsun",
     author_email = "keyiflerolsun@gmail.com",
```

