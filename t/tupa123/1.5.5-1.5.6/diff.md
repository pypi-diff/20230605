# Comparing `tmp/tupa123-1.5.5.tar.gz` & `tmp/tupa123-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tupa123-1.5.5.tar", last modified: Thu Jun  1 18:58:01 2023, max compression
+gzip compressed data, was "tupa123-1.5.6.tar", last modified: Mon Jun  5 19:09:13 2023, max compression
```

## Comparing `tupa123-1.5.5.tar` & `tupa123-1.5.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 18:58:01.871468 tupa123-1.5.5/
--rw-rw-rw-   0        0        0     1101 2023-03-27 13:05:36.000000 tupa123-1.5.5/LICENSE.txt
--rw-rw-rw-   0        0        0     2352 2023-06-01 18:58:01.870604 tupa123-1.5.5/PKG-INFO
--rw-rw-rw-   0        0        0     1876 2023-04-18 13:58:59.000000 tupa123-1.5.5/README.md
--rw-rw-rw-   0        0        0       42 2023-06-01 18:58:01.871468 tupa123-1.5.5/setup.cfg
--rw-rw-rw-   0        0        0      839 2023-06-01 18:57:23.000000 tupa123-1.5.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:58:01.850541 tupa123-1.5.5/tupa12/
--rw-rw-rw-   0        0        0       23 2023-05-30 20:43:01.000000 tupa123-1.5.5/tupa12/__init__.py
--rw-rw-rw-   0        0        0    50693 2023-06-01 18:56:11.000000 tupa123-1.5.5/tupa12/tupa12.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:58:01.858125 tupa123-1.5.5/tupa123/
--rw-rw-rw-   0        0        0       24 2023-05-30 20:42:30.000000 tupa123-1.5.5/tupa123/__init__.py
--rw-rw-rw-   0        0        0   172319 2023-05-29 13:46:41.000000 tupa123-1.5.5/tupa123/machine1.txt
--rw-rw-rw-   0        0        0    89863 2023-06-01 18:56:09.000000 tupa123-1.5.5/tupa123/tupa123.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:58:01.868579 tupa123-1.5.5/tupa123.egg-info/
--rw-rw-rw-   0        0        0     2352 2023-06-01 18:58:01.000000 tupa123-1.5.5/tupa123.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2023-06-01 18:58:01.000000 tupa123-1.5.5/tupa123.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 18:58:01.000000 tupa123-1.5.5/tupa123.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-06-01 18:58:01.000000 tupa123-1.5.5/tupa123.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-01 18:58:01.000000 tupa123-1.5.5/tupa123.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-05 19:09:13.115947 tupa123-1.5.6/
+-rw-rw-rw-   0        0        0     1101 2023-03-27 13:05:36.000000 tupa123-1.5.6/LICENSE.txt
+-rw-rw-rw-   0        0        0     2352 2023-06-05 19:09:13.115947 tupa123-1.5.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1876 2023-04-18 13:58:59.000000 tupa123-1.5.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-05 19:09:13.116937 tupa123-1.5.6/setup.cfg
+-rw-rw-rw-   0        0        0      839 2023-06-05 19:07:46.000000 tupa123-1.5.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 19:09:13.096828 tupa123-1.5.6/tupa12/
+-rw-rw-rw-   0        0        0       23 2023-05-30 20:43:01.000000 tupa123-1.5.6/tupa12/__init__.py
+-rw-rw-rw-   0        0        0    54180 2023-06-05 16:54:03.000000 tupa123-1.5.6/tupa12/tupa12.py
+drwxrwxrwx   0        0        0        0 2023-06-05 19:09:13.105082 tupa123-1.5.6/tupa123/
+-rw-rw-rw-   0        0        0       24 2023-05-30 20:42:30.000000 tupa123-1.5.6/tupa123/__init__.py
+-rw-rw-rw-   0        0        0   172319 2023-05-29 13:46:41.000000 tupa123-1.5.6/tupa123/machine1.txt
+-rw-rw-rw-   0        0        0    94064 2023-06-05 18:09:11.000000 tupa123-1.5.6/tupa123/tupa123.py
+drwxrwxrwx   0        0        0        0 2023-06-05 19:09:13.113922 tupa123-1.5.6/tupa123.egg-info/
+-rw-rw-rw-   0        0        0     2352 2023-06-05 19:09:12.000000 tupa123-1.5.6/tupa123.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2023-06-05 19:09:13.000000 tupa123-1.5.6/tupa123.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 19:09:12.000000 tupa123-1.5.6/tupa123.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-06-05 19:09:12.000000 tupa123-1.5.6/tupa123.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-05 19:09:12.000000 tupa123-1.5.6/tupa123.egg-info/top_level.txt
```

### Comparing `tupa123-1.5.5/LICENSE.txt` & `tupa123-1.5.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tupa123-1.5.5/PKG-INFO` & `tupa123-1.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tupa123
-Version: 1.5.5
+Version: 1.5.6
 Summary: fully connected neural network with four layers
 Author: Leandro Schemmer
 Author-email: leandro.schemmer@gmail.com
 License: MIT
 Keywords: artificial-intelligence neural-networks four-layers regression regression-analysis classification-algorithms tupa123 deep-learning machine-learning data-science artificial-neural-network open-source
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `tupa123-1.5.5/README.md` & `tupa123-1.5.6/README.md`

 * *Files identical despite different names*

### Comparing `tupa123-1.5.5/setup.py` & `tupa123-1.5.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='tupa123',
-    version='1.5.5',
+    version='1.5.6',
     license = 'MIT',
     license_files=('LICENSE.txt',),
     packages=['tupa123', 'tupa12'],
     package_data={'tupa123': ['machine1.txt'],},    
     install_requires=['numpy','matplotlib','pandas','opencv-python'],    
     author='Leandro Schemmer',
     author_email='leandro.schemmer@gmail.com',
```

### Comparing `tupa123-1.5.5/tupa12/tupa12.py` & `tupa123-1.5.6/tupa12/tupa12.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,25 +15,24 @@
 
 
 
 #Neural network 3 layers--------------------------------------------------------------------------------------------------------------------
 class nnet3:
 
     #global variables-------------------------------------------------------------------------
-    def __init__ (self, norma=1, coef=0, normout=1, nn1c=1, nn2c=5, nn3c=1, rate=0.01, epochs=1000, fa2c=5, fa3c=0, cost=0, regu=0, namenet='', shift=1, iteconv=0, conv=0, sbw=1, c1=2, txt=0, sdnoise=0, c2=0.01, c3=1.33):
+    def __init__ (self, norma=1, normout=1, nn1c=1, nn2c=5, nn3c=1, rate=0.01, epochs=1000, fa2c=5, fa3c=0, cost=0, regu=0, namenet='', shift=1, iteconv=0, conv=0, sbw=1, c1=2, txt=0, sdnoise=0, c2=0.01, c3=1.33):
         
         self.nn1c=nn1c
         self.nn2c=nn2c
         self.nn3c=nn3c
         self.rate=rate
         self.epochs=epochs
         self.fa2c=fa2c
         self.fa3c=fa3c
         self.norma=norma
-        self.coef=coef
         self.normout=normout
         self.cost=cost
         self.regu=regu
         self.namenet=namenet
         self.shift=shift
         self.iteconv=iteconv
         self.conv=conv
@@ -49,126 +48,244 @@
 ###############################################################
 ###############################################################
 #########  Auxliar function to normalization   ################
 ###############################################################
 ###############################################################
 
 
-
-    #data normalization by calculating maximums and minimums-----------------------------------------------
+    #data normalization by calculating maximums and minimums, inlet------------------------------------------
     def Normalize(self, data, maxiname, mininame, medianame, desvioname):          
 
         #=-1, standardization
         #=0, do anything
         #=1, between 0 and 1
-        #=2, between -1 and 1 
-        #=3, log(x+coef)
-        #=4, log(x+coef)  between 0 and 1
-        #=5, log(x+coef)  between -1 and 1
-        #=6, log(x+coef)  and standardization
-
-        if (self.norma>=3): 
-            data = np.log(data + self.coef)
-        normalized = data*1
-        
+        #=2, between -1 and 1
+        #=3, divide by the average
+        #=4, divide by the average and -1 to centralize in zero
+       
         vetormax = np.max(data,0) 
         vetormin = np.min(data,0)
-                
+
         if self.shift>1: #aplica o esticamento se tiver
             vetormax=np.where(vetormax < 0, vetormax*(1/self.shift), vetormax*self.shift)
             vetormin=np.where(vetormin < 0, vetormin*self.shift, vetormin*(1/self.shift))
 
         vetormed = (vetormax+vetormin)/2
         media = np.mean(data,0)
         desvio = np.std(data,0)        
+
+        if (self.norma==0):
+            normalized = data *1
                                     
-        if (self.norma==1) or (self.norma==4):
+        if (self.norma==1):
             vetoraux = (vetormax - vetormin)
             vetoraux = np.where(vetoraux==0, 1 , vetoraux)
             normalized = (data - vetormin) / vetoraux
             
-        if (self.norma==2) or (self.norma==5):
+        if (self.norma==2):
             vetoraux = (vetormax - vetormed)
             vetoraux = np.where(vetoraux==0, 1 , vetoraux)
             normalized = (data - vetormed) / vetoraux
 
-        if (self.norma==6) or (self.norma==-1):
+        if (self.norma==-1):
             vetoraux = desvio
             vetoraux = np.where(vetoraux==0, 1 , vetoraux)
             normalized = (data - media)/vetoraux
 
+        if (self.norma==3):
+            normalized = data / media
+
+        if (self.norma==4):
+            normalized = (data / media)-1
+
+
         np.save(maxiname, vetormax)
         np.save(mininame, vetormin)
         np.save(medianame, media)
         np.save(desvioname, desvio)
         
         return normalized
 
 
 
+    #data normalization by calculating maximums and minimums, outlet------------------------------------------
+    def Normalizeout(self, data, maxiname, mininame, medianame, desvioname):          
+
+        #=-1, standardization
+        #=0, do anything
+        #=1, between 0 and 1
+        #=2, between -1 and 1 
+        
+        vetormax = np.max(data,0) 
+        vetormin = np.min(data,0)
+
+        if self.shift>1: #aplica o esticamento se tiver
+            vetormax=np.where(vetormax < 0, vetormax*(1/self.shift), vetormax*self.shift)
+            vetormin=np.where(vetormin < 0, vetormin*self.shift, vetormin*(1/self.shift))
+
+        vetormed = (vetormax+vetormin)/2
+        media = np.mean(data,0)
+        desvio = np.std(data,0)
+        
+        if (self.normout==0):
+            normalized = data *1
+                                    
+        if (self.normout==1):
+            vetoraux = (vetormax - vetormin)
+            vetoraux = np.where(vetoraux==0, 1 , vetoraux)
+            normalized = (data - vetormin) / vetoraux
+            
+        if (self.normout==2):
+            vetoraux = (vetormax - vetormed)
+            vetoraux = np.where(vetoraux==0, 1 , vetoraux)
+            normalized = (data - vetormed) / vetoraux
+
+        if (self.normout==-1):
+            vetoraux = desvio
+            vetoraux = np.where(vetoraux==0, 1 , vetoraux)
+            normalized = (data - media)/vetoraux
+
+        if (self.normout==3):
+            normalized = data / media
+
+        if (self.normout==4):
+            normalized = (data / media)-1
 
+        np.save(maxiname, vetormax)
+        np.save(mininame, vetormin)
+        np.save(medianame, media)
+        np.save(desvioname, desvio)
+        
+        return normalized
 
 
     #normalizing the data by entering maximums and minimums-----------------------------------------------
     def Normalize2(self, data, maxiname, mininame, medianame, desvioname):         
 
         vetormax = np.load(maxiname) 
         vetormin = np.load(mininame) 
         vetormed = (vetormax+vetormin)/2
         media = np.load(medianame)
         desvio = np.load(desvioname)  
 
-        if (self.norma>=3): 
-            data = np.log(data + self.coef)
-        normalized = data*1
+        normalized = data*1 #==0, não faz nada
+
+        if (self.norma==0):
+            normalized = data *1
                                                 
-        if (self.norma==1) or (self.norma==4):  
+        if (self.norma==1):  
             normalized = (data - vetormin) / (vetormax - vetormin)
             
-        if (self.norma==2) or (self.norma==5):    
+        if (self.norma==2):    
             normalized = (data - vetormed) / (vetormax - vetormed)                                 
 
-        if (self.norma==6) or (self.norma==-1):
+        if (self.norma==-1):
             normalized = (data - media)/desvio
-            
+
+        if (self.norma==3):
+            normalized = data / media
+
+        if (self.norma==4):
+            normalized = (data / media)-1
+        
         return normalized
 
 
+    #normalizing the data by entering maximums and minimums-----------------------------------------------
+    def Normalize2out(self, data, maxiname, mininame, medianame, desvioname):         
+
+        vetormax = np.load(maxiname) 
+        vetormin = np.load(mininame) 
+        vetormed = (vetormax+vetormin)/2
+        media = np.load(medianame)
+        desvio = np.load(desvioname)  
+
+        normalized = data*1 #==0, não faz nada
+
+        if (self.normout==0):
+            normalized = data *1
+                                                
+        if (self.normout==1):  
+            normalized = (data - vetormin) / (vetormax - vetormin)
+            
+        if (self.normout==2):    
+            normalized = (data - vetormed) / (vetormax - vetormed)                                 
+
+        if (self.normout==-1):
+            normalized = (data - media)/desvio
 
+        if (self.normout==3):
+            normalized = data / media
 
+        if (self.normout==4):
+            normalized = (data / media)-1
+        
+        return normalized
 
 
 
-    #data denormalization-------------------------------------------------------------------
+    #data denormalization by entering maximums and minimums--------------------------------------------
     def DesNormalize(self, normalized, maxiname, mininame, medianame, desvioname):         
 
         vetormax = np.load(maxiname) 
         vetormin = np.load(mininame) 
         vetormed = (vetormax+vetormin)/2
         media = np.load(medianame)
         desvio = np.load(desvioname) 
         
-        desnorma = normalized*1
+        desnorma = normalized*1 #==0, nada
                             
-        if (self.norma==1) or (self.norma==4):  
+        if (self.norma==1):  
             desnorma = normalized * (vetormax - vetormin) + vetormin
             
-        if (self.norma==2) or (self.norma==5):  
+        if (self.norma==2):  
             desnorma = normalized * (vetormax - vetormed) + vetormed
 
-        if (self.norma==6) or (self.norma==-1):          
+        if (self.norma==-1):          
             desnorma = normalized*desvio + media
 
-        if (self.norma>=3): 
-            desnorma = np.exp(desnorma) - self.coef
-                               
+        if (self.norma==3): 
+            desnorma = normalized*media
+
+        if (self.norma==4):
+            desnorma = (normalized+1)*media
+                           
         return desnorma
 
 
 
+    #data denormalization by entering maximums and minimums--------------------------------------------
+    def DesNormalizeout(self, normalized, maxiname, mininame, medianame, desvioname):         
+
+        vetormax = np.load(maxiname) 
+        vetormin = np.load(mininame) 
+        vetormed = (vetormax+vetormin)/2
+        media = np.load(medianame)
+        desvio = np.load(desvioname) 
+        
+        desnorma = normalized*1 #==0, nada
+                            
+        if (self.normout==1):  
+            desnorma = normalized * (vetormax - vetormin) + vetormin
+            
+        if (self.normout==2):  
+            desnorma = normalized * (vetormax - vetormed) + vetormed
+
+        if (self.normout==-1):          
+            desnorma = normalized*desvio + media
+
+        if (self.normout==3): 
+            desnorma = normalized*media
+
+        if (self.normout==4):
+            desnorma = (normalized+1)*media
+                           
+        return desnorma
+
+
 
 ###############################################################
 ###############################################################
 ################ Activation functions   #######################
 ###############################################################
 ###############################################################
 
@@ -448,23 +565,20 @@
             B3 = -0.1 + 2*0.1*(np.random.rand(self.nn3c))  
             P12 = -0.1 + 2*0.1*(np.random.rand(self.nn1c,self.nn2c))
             P23 = -0.1 + 2*0.1*(np.random.rand(self.nn2c,self.nn3c))
 
 
         #Normaliza os parametros-------------------------
         matX = self.Normalize(matX,nomepasta + "vmax_in.npy",nomepasta + "vmin_in.npy",nomepasta + "media_in.npy",nomepasta + "desvio_in.npy")                
-        if (self.normout==1):
-            matY = self.Normalize(matY,nomepasta + "vmax_out.npy",nomepasta + "vmin_out.npy",nomepasta + "media_out.npy",nomepasta + "desvio_out.npy")
+        matY = self.Normalizeout(matY,nomepasta + "vmax_out.npy",nomepasta + "vmin_out.npy",nomepasta + "media_out.npy",nomepasta + "desvio_out.npy")
 
-        #Para validacao cruzada, normaliza em função do conjunto padrão de dados de correção dos pesos
+        #Para validacao cruzada se houver------
         if (len(matX2)>1):
             matX2 = self.Normalize2(matX2,nomepasta + "vmax_in.npy",nomepasta + "vmin_in.npy",nomepasta + "media_in.npy",nomepasta + "desvio_in.npy") 
-            if (self.normout==1):
-                matY2 = self.Normalize2(matY2,nomepasta + "vmax_in.npy",nomepasta + "vmin_in.npy",nomepasta + "media_in.npy",nomepasta + "desvio_in.npy") 
-
+            matY2 = self.Normalize2out(matY2,nomepasta + "vmax_out.npy",nomepasta + "vmin_out.npy",nomepasta + "media_out.npy",nomepasta + "desvio_out.npy") 
 
 
         #Processo de aprendizado------------------------------------------------------------
                 
         VetorErro = [0]
         MenorErro = 999999999
         
@@ -738,24 +852,20 @@
             B3 = -0.1 + 2*0.1*(np.random.rand(self.nn3c))   
             P12 = -0.1 + 2*0.1*(np.random.rand(self.nn1c,self.nn2c))
             P23 = -0.1 + 2*0.1*(np.random.rand(self.nn2c,self.nn3c))
 
 
         #Normaliza os parametros-------------------------
         matX = self.Normalize(matX,nomepasta + "vmax_in.npy",nomepasta + "vmin_in.npy",nomepasta + "media_in.npy",nomepasta + "desvio_in.npy")                
-        if (self.normout==1):
-            matY = self.Normalize(matY,nomepasta + "vmax_out.npy",nomepasta + "vmin_out.npy",nomepasta + "media_out.npy",nomepasta + "desvio_out.npy")
+        matY = self.Normalizeout(matY,nomepasta + "vmax_out.npy",nomepasta + "vmin_out.npy",nomepasta + "media_out.npy",nomepasta + "desvio_out.npy")
 
-        #Para validacao cruzada, normaliza em função do conjunto padrão de dados de correção dos pesos
+        #Para validacao cruzada se houver------
         if (len(matX2)>1):
             matX2 = self.Normalize2(matX2,nomepasta + "vmax_in.npy",nomepasta + "vmin_in.npy",nomepasta + "media_in.npy",nomepasta + "desvio_in.npy") 
-            if (self.normout==1):
-                matY2 = self.Normalize2(matY2,nomepasta + "vmax_in.npy",nomepasta + "vmin_in.npy",nomepasta + "media_in.npy",nomepasta + "desvio_in.npy") 
-
-
+            matY2 = self.Normalize2out(matY2,nomepasta + "vmax_out.npy",nomepasta + "vmin_out.npy",nomepasta + "media_out.npy",nomepasta + "desvio_out.npy") 
 
 
         #Processo de aprendizado------------------------------------------------------------
 
         VetorErro = [0]
         MenorErro = 999999999
 
@@ -1016,24 +1126,23 @@
         except: #Inicializa randomicamente-------------------------------
 
             B2 = -0.1 + 2*0.1*(np.random.rand(self.nn2c))
             B3 = -0.1 + 2*0.1*(np.random.rand(self.nn3c))  
             P12 = -0.1 + 2*0.1*(np.random.rand(self.nn1c,self.nn2c))
             P23 = -0.1 + 2*0.1*(np.random.rand(self.nn2c,self.nn3c))
 
+
         #Normaliza os parametros-------------------------
         matX = self.Normalize(matX,nomepasta + "vmax_in.npy",nomepasta + "vmin_in.npy",nomepasta + "media_in.npy",nomepasta + "desvio_in.npy")                
-        if (self.normout==1):
-            matY = self.Normalize(matY,nomepasta + "vmax_out.npy",nomepasta + "vmin_out.npy",nomepasta + "media_out.npy",nomepasta + "desvio_out.npy")
+        matY = self.Normalizeout(matY,nomepasta + "vmax_out.npy",nomepasta + "vmin_out.npy",nomepasta + "media_out.npy",nomepasta + "desvio_out.npy")
 
-        #Para validacao cruzada, normaliza em função do conjunto padrão de dados de correção dos pesos
+        #Para validacao cruzada se houver------
         if (len(matX2)>1):
             matX2 = self.Normalize2(matX2,nomepasta + "vmax_in.npy",nomepasta + "vmin_in.npy",nomepasta + "media_in.npy",nomepasta + "desvio_in.npy") 
-            if (self.normout==1):
-                matY2 = self.Normalize2(matY2,nomepasta + "vmax_out.npy",nomepasta + "vmin_out.npy",nomepasta + "media_out.npy",nomepasta + "desvio_out.npy")
+            matY2 = self.Normalize2out(matY2,nomepasta + "vmax_out.npy",nomepasta + "vmin_out.npy",nomepasta + "media_out.npy",nomepasta + "desvio_out.npy") 
 
 
         #Processo de aprendizado------------------------------------------------------------
 
         VetorErro = [0]
         MenorErro = 999999999
 
@@ -1290,16 +1399,15 @@
 
             c3 = np.dot(c2,P23)- B3
             c3 = self.Activation(self.fa3c,c3)       
 
             # saida----------------------------
             Calculated[caso][:] = c3[:]
 
-        if (self.normout==1):            
-            Calculated = self.DesNormalize(Calculated, nomepasta + "vmax_out.npy", nomepasta + "vmin_out.npy",nomepasta + "media_out.npy",nomepasta + "desvio_out.npy") 
+        Calculated = self.DesNormalizeout(Calculated, nomepasta + "vmax_out.npy", nomepasta + "vmin_out.npy",nomepasta + "media_out.npy",nomepasta + "desvio_out.npy") 
 
         if (self.txt!=0): #print txt out data
              np.savetxt(nomepasta + "out.txt", Calculated)
 
         return Calculated
```

### Comparing `tupa123-1.5.5/tupa123/machine1.txt` & `tupa123-1.5.6/tupa123/machine1.txt`

 * *Files identical despite different names*

### Comparing `tupa123-1.5.5/tupa123/tupa123.py` & `tupa123-1.5.6/tupa123/tupa123.py`

 * *Files 6% similar despite different names*

```diff
@@ -659,27 +659,49 @@
 #faz a normalização entrando especificamente os valores maximos e minimos e um formato de lista
 def Norma(data, vetormax, vetormin):
     vetormax2 = np.array(vetormax)
     vetormin2 = np.array(vetormin)    
     normalized = (data - vetormin2) / (vetormax2 - vetormin2)
     return normalized
 
-def DesNorma(data, vetormax, vetormin):
+def Desnorma(data, vetormax, vetormin):
     vetormax2 = np.array(vetormax)
     vetormin2 = np.array(vetormin) 
     denormalized = data * (vetormax2 - vetormin2) + vetormin2
     return denormalized
 
 
 
 
+#compressão logaritmica, dado um vetor de 0 a n por variável
+def Compress(data, vetorlog):
+    a,b = data.shape
+    for i in range(0, a):
+        for j in range(0, b):
+            comando = vetorlog[j]
+            if (comando > 0):
+                for k in range(comando):
+                    data[i][j] = np.log10(data[i][j])
+    return data
 
 
 
 
+#descompressão logaritmica, dado um vetor de 0 a n por variável
+def Decompress(data, vetorlog):
+    a,b = data.shape
+    for i in range(0, a):
+        for j in range(0, b):
+            comando = vetorlog[j]
+            if (comando > 0):
+                for k in range(comando):
+                    data[i][j] =10**(data[i][j])
+    return data
+
+
 
 
 
 ###############################################################
 ###############################################################
 #########  Gaussian Expansion   ###############################
 ###############################################################
@@ -767,27 +789,26 @@
 
 
 
 #Neural network 4 layers--------------------------------------------------------------------------------------------------------------------
 class nnet4:
 
     #global variables-------------------------------------------------------------------------
-    def __init__ (self, norma=1, coef=0, normout=1, nn1c=1, nn2c=5, nn3c=5, nn4c=1, rate=0.01, epochs=1000, fa2c=5, fa3c=5, fa4c=0, cost=0, regu=0, namenet='', shift=1, iteconv=0, conv=0, sbw=1, c1=2, txt=0, sdnoise=0, c2=0.01, c3=1.33):
+    def __init__ (self, norma=1, normout=1, nn1c=1, nn2c=5, nn3c=5, nn4c=1, rate=0.01, epochs=1000, fa2c=5, fa3c=5, fa4c=0, cost=0, regu=0, namenet='', shift=1, iteconv=0, conv=0, sbw=1, c1=2, txt=0, sdnoise=0, c2=0.01, c3=1.33):
         
         self.nn1c=nn1c
         self.nn2c=nn2c
         self.nn3c=nn3c
         self.nn4c=nn4c
         self.rate=rate
         self.epochs=epochs
         self.fa2c=fa2c
         self.fa3c=fa3c
         self.fa4c=fa4c
         self.norma=norma
-        self.coef=coef
         self.normout=normout
         self.cost=cost
         self.regu=regu
         self.namenet=namenet
         self.shift=shift
         self.iteconv=iteconv
         self.conv=conv
@@ -804,125 +825,244 @@
 ###############################################################
 #########  Auxliar function to normalization   ################
 ###############################################################
 ###############################################################
 
 
 
-    #data normalization by calculating maximums and minimums-----------------------------------------------
+    #data normalization by calculating maximums and minimums, inlet------------------------------------------
     def Normalize(self, data, maxiname, mininame, medianame, desvioname):          
 
         #=-1, standardization
         #=0, do anything
         #=1, between 0 and 1
-        #=2, between -1 and 1 
-        #=3, log(x+coef)
-        #=4, log(x+coef)  between 0 and 1
-        #=5, log(x+coef)  between -1 and 1
-        #=6, log(x+coef)  and standardization
-
-        if (self.norma>=3): 
-            data = np.log(data + self.coef)
-        normalized = data*1
-        
+        #=2, between -1 and 1
+        #=3, divide by the average
+        #=4, divide by the average and -1 to centralize in zero
+       
         vetormax = np.max(data,0) 
         vetormin = np.min(data,0)
-                
+
         if self.shift>1: #aplica o esticamento se tiver
             vetormax=np.where(vetormax < 0, vetormax*(1/self.shift), vetormax*self.shift)
             vetormin=np.where(vetormin < 0, vetormin*self.shift, vetormin*(1/self.shift))
 
         vetormed = (vetormax+vetormin)/2
         media = np.mean(data,0)
         desvio = np.std(data,0)        
+
+        if (self.norma==0):
+            normalized = data *1
                                     
-        if (self.norma==1) or (self.norma==4):
+        if (self.norma==1):
             vetoraux = (vetormax - vetormin)
             vetoraux = np.where(vetoraux==0, 1 , vetoraux)
             normalized = (data - vetormin) / vetoraux
             
-        if (self.norma==2) or (self.norma==5):
+        if (self.norma==2):
             vetoraux = (vetormax - vetormed)
             vetoraux = np.where(vetoraux==0, 1 , vetoraux)
             normalized = (data - vetormed) / vetoraux
 
-        if (self.norma==6) or (self.norma==-1):
+        if (self.norma==-1):
             vetoraux = desvio
             vetoraux = np.where(vetoraux==0, 1 , vetoraux)
             normalized = (data - media)/vetoraux
 
+        if (self.norma==3):
+            normalized = data / media
+
+        if (self.norma==4):
+            normalized = (data / media)-1
+
+
         np.save(maxiname, vetormax)
         np.save(mininame, vetormin)
         np.save(medianame, media)
         np.save(desvioname, desvio)
         
         return normalized
 
 
 
+    #data normalization by calculating maximums and minimums, outlet------------------------------------------
+    def Normalizeout(self, data, maxiname, mininame, medianame, desvioname):          
+
+        #=-1, standardization
+        #=0, do anything
+        #=1, between 0 and 1
+        #=2, between -1 and 1 
+        
+        vetormax = np.max(data,0) 
+        vetormin = np.min(data,0)
+
+        if self.shift>1: #aplica o esticamento se tiver
+            vetormax=np.where(vetormax < 0, vetormax*(1/self.shift), vetormax*self.shift)
+            vetormin=np.where(vetormin < 0, vetormin*self.shift, vetormin*(1/self.shift))
+
+        vetormed = (vetormax+vetormin)/2
+        media = np.mean(data,0)
+        desvio = np.std(data,0)
+        
+        if (self.normout==0):
+            normalized = data *1
+                                    
+        if (self.normout==1):
+            vetoraux = (vetormax - vetormin)
+            vetoraux = np.where(vetoraux==0, 1 , vetoraux)
+            normalized = (data - vetormin) / vetoraux
+            
+        if (self.normout==2):
+            vetoraux = (vetormax - vetormed)
+            vetoraux = np.where(vetoraux==0, 1 , vetoraux)
+            normalized = (data - vetormed) / vetoraux
+
+        if (self.normout==-1):
+            vetoraux = desvio
+            vetoraux = np.where(vetoraux==0, 1 , vetoraux)
+            normalized = (data - media)/vetoraux
+
+        if (self.normout==3):
+            normalized = data / media
+
+        if (self.normout==4):
+            normalized = (data / media)-1
 
+        np.save(maxiname, vetormax)
+        np.save(mininame, vetormin)
+        np.save(medianame, media)
+        np.save(desvioname, desvio)
+        
+        return normalized
 
 
     #normalizing the data by entering maximums and minimums-----------------------------------------------
     def Normalize2(self, data, maxiname, mininame, medianame, desvioname):         
 
         vetormax = np.load(maxiname) 
         vetormin = np.load(mininame) 
         vetormed = (vetormax+vetormin)/2
         media = np.load(medianame)
         desvio = np.load(desvioname)  
 
-        if (self.norma>=3): 
-            data = np.log(data + self.coef)
-        normalized = data*1
+        normalized = data*1 #==0, não faz nada
+
+        if (self.norma==0):
+            normalized = data *1
                                                 
-        if (self.norma==1) or (self.norma==4):  
+        if (self.norma==1):  
             normalized = (data - vetormin) / (vetormax - vetormin)
             
-        if (self.norma==2) or (self.norma==5):    
+        if (self.norma==2):    
             normalized = (data - vetormed) / (vetormax - vetormed)                                 
 
-        if (self.norma==6) or (self.norma==-1):
+        if (self.norma==-1):
             normalized = (data - media)/desvio
-            
+
+        if (self.norma==3):
+            normalized = data / media
+
+        if (self.norma==4):
+            normalized = (data / media)-1
+        
         return normalized
 
 
+    #normalizing the data by entering maximums and minimums-----------------------------------------------
+    def Normalize2out(self, data, maxiname, mininame, medianame, desvioname):         
+
+        vetormax = np.load(maxiname) 
+        vetormin = np.load(mininame) 
+        vetormed = (vetormax+vetormin)/2
+        media = np.load(medianame)
+        desvio = np.load(desvioname)  
+
+        normalized = data*1 #==0, não faz nada
+
+        if (self.normout==0):
+            normalized = data *1
+                                                
+        if (self.normout==1):  
+            normalized = (data - vetormin) / (vetormax - vetormin)
+            
+        if (self.normout==2):    
+            normalized = (data - vetormed) / (vetormax - vetormed)                                 
+
+        if (self.normout==-1):
+            normalized = (data - media)/desvio
 
+        if (self.normout==3):
+            normalized = data / media
 
+        if (self.normout==4):
+            normalized = (data / media)-1
+        
+        return normalized
 
 
 
-    #data denormalization-------------------------------------------------------------------
+    #data denormalization by entering maximums and minimums--------------------------------------------
     def DesNormalize(self, normalized, maxiname, mininame, medianame, desvioname):         
 
         vetormax = np.load(maxiname) 
         vetormin = np.load(mininame) 
         vetormed = (vetormax+vetormin)/2
         media = np.load(medianame)
         desvio = np.load(desvioname) 
         
-        desnorma = normalized*1
+        desnorma = normalized*1 #==0, nada
                             
-        if (self.norma==1) or (self.norma==4):  
+        if (self.norma==1):  
             desnorma = normalized * (vetormax - vetormin) + vetormin
             
-        if (self.norma==2) or (self.norma==5):  
+        if (self.norma==2):  
             desnorma = normalized * (vetormax - vetormed) + vetormed
 
-        if (self.norma==6) or (self.norma==-1):          
+        if (self.norma==-1):          
             desnorma = normalized*desvio + media
 
-        if (self.norma>=3): 
-            desnorma = np.exp(desnorma) - self.coef
-                               
+        if (self.norma==3): 
+            desnorma = normalized*media
+
+        if (self.norma==4):
+            desnorma = (normalized+1)*media
+                           
         return desnorma
 
 
 
+    #data denormalization by entering maximums and minimums--------------------------------------------
+    def DesNormalizeout(self, normalized, maxiname, mininame, medianame, desvioname):         
+
+        vetormax = np.load(maxiname) 
+        vetormin = np.load(mininame) 
+        vetormed = (vetormax+vetormin)/2
+        media = np.load(medianame)
+        desvio = np.load(desvioname) 
+        
+        desnorma = normalized*1 #==0, nada
+                            
+        if (self.normout==1):  
+            desnorma = normalized * (vetormax - vetormin) + vetormin
+            
+        if (self.normout==2):  
+            desnorma = normalized * (vetormax - vetormed) + vetormed
+
+        if (self.normout==-1):          
+            desnorma = normalized*desvio + media
+
+        if (self.normout==3): 
+            desnorma = normalized*media
+
+        if (self.normout==4):
+            desnorma = (normalized+1)*media
+                           
+        return desnorma
+
+
 
 ###############################################################
 ###############################################################
 ################ Activation functions   #######################
 ###############################################################
 ###############################################################
 
@@ -1219,23 +1359,20 @@
             P12 = -0.1 + 2*0.1*(np.random.rand(self.nn1c,self.nn2c))
             P23 = -0.1 + 2*0.1*(np.random.rand(self.nn2c,self.nn3c))
             P34 = -0.1 + 2*0.1*(np.random.rand(self.nn3c,self.nn4c))
 
 
         #Normaliza os parametros-------------------------
         matX = self.Normalize(matX,nomepasta + "vmax_in.npy",nomepasta + "vmin_in.npy",nomepasta + "media_in.npy",nomepasta + "desvio_in.npy")                
-        if (self.normout==1):
-            matY = self.Normalize(matY,nomepasta + "vmax_out.npy",nomepasta + "vmin_out.npy",nomepasta + "media_out.npy",nomepasta + "desvio_out.npy")
+        matY = self.Normalizeout(matY,nomepasta + "vmax_out.npy",nomepasta + "vmin_out.npy",nomepasta + "media_out.npy",nomepasta + "desvio_out.npy")
 
-        #Para validacao cruzada, normaliza em função do conjunto padrão de dados de correção dos pesos
+        #Para validacao cruzada se houver------
         if (len(matX2)>1):
             matX2 = self.Normalize2(matX2,nomepasta + "vmax_in.npy",nomepasta + "vmin_in.npy",nomepasta + "media_in.npy",nomepasta + "desvio_in.npy") 
-            if (self.normout==1):
-                matY2 = self.Normalize2(matY2,nomepasta + "vmax_in.npy",nomepasta + "vmin_in.npy",nomepasta + "media_in.npy",nomepasta + "desvio_in.npy") 
-
+            matY2 = self.Normalize2out(matY2,nomepasta + "vmax_out.npy",nomepasta + "vmin_out.npy",nomepasta + "media_out.npy",nomepasta + "desvio_out.npy") 
 
 
         #Processo de aprendizado------------------------------------------------------------
                 
         VetorErro = [0]
         MenorErro = 999999999
         
@@ -1553,23 +1690,20 @@
             P12 = -0.1 + 2*0.1*(np.random.rand(self.nn1c,self.nn2c))
             P23 = -0.1 + 2*0.1*(np.random.rand(self.nn2c,self.nn3c))
             P34 = -0.1 + 2*0.1*(np.random.rand(self.nn3c,self.nn4c))
 
 
         #Normaliza os parametros-------------------------
         matX = self.Normalize(matX,nomepasta + "vmax_in.npy",nomepasta + "vmin_in.npy",nomepasta + "media_in.npy",nomepasta + "desvio_in.npy")                
-        if (self.normout==1):
-            matY = self.Normalize(matY,nomepasta + "vmax_out.npy",nomepasta + "vmin_out.npy",nomepasta + "media_out.npy",nomepasta + "desvio_out.npy")
+        matY = self.Normalizeout(matY,nomepasta + "vmax_out.npy",nomepasta + "vmin_out.npy",nomepasta + "media_out.npy",nomepasta + "desvio_out.npy")
 
-        #Para validacao cruzada, normaliza em função do conjunto padrão de dados de correção dos pesos
+        #Para validacao cruzada se houver------
         if (len(matX2)>1):
             matX2 = self.Normalize2(matX2,nomepasta + "vmax_in.npy",nomepasta + "vmin_in.npy",nomepasta + "media_in.npy",nomepasta + "desvio_in.npy") 
-            if (self.normout==1):
-                matY2 = self.Normalize2(matY2,nomepasta + "vmax_in.npy",nomepasta + "vmin_in.npy",nomepasta + "media_in.npy",nomepasta + "desvio_in.npy") 
-
+            matY2 = self.Normalize2out(matY2,nomepasta + "vmax_out.npy",nomepasta + "vmin_out.npy",nomepasta + "media_out.npy",nomepasta + "desvio_out.npy") 
 
 
 
         #Processo de aprendizado------------------------------------------------------------
 
         VetorErro = [0]
         MenorErro = 999999999
@@ -1873,23 +2007,20 @@
             P12 = -0.1 + 2*0.1*(np.random.rand(self.nn1c,self.nn2c))
             P23 = -0.1 + 2*0.1*(np.random.rand(self.nn2c,self.nn3c))
             P34 = -0.1 + 2*0.1*(np.random.rand(self.nn3c,self.nn4c))
 
 
         #Normaliza os parametros-------------------------
         matX = self.Normalize(matX,nomepasta + "vmax_in.npy",nomepasta + "vmin_in.npy",nomepasta + "media_in.npy",nomepasta + "desvio_in.npy")                
-        if (self.normout==1):
-            matY = self.Normalize(matY,nomepasta + "vmax_out.npy",nomepasta + "vmin_out.npy",nomepasta + "media_out.npy",nomepasta + "desvio_out.npy")
+        matY = self.Normalizeout(matY,nomepasta + "vmax_out.npy",nomepasta + "vmin_out.npy",nomepasta + "media_out.npy",nomepasta + "desvio_out.npy")
 
-        #Para validacao cruzada, normaliza em função do conjunto padrão de dados de correção dos pesos
+        #Para validacao cruzada se houver------
         if (len(matX2)>1):
             matX2 = self.Normalize2(matX2,nomepasta + "vmax_in.npy",nomepasta + "vmin_in.npy",nomepasta + "media_in.npy",nomepasta + "desvio_in.npy") 
-            if (self.normout==1):
-                matY2 = self.Normalize2(matY2,nomepasta + "vmax_out.npy",nomepasta + "vmin_out.npy",nomepasta + "media_out.npy",nomepasta + "desvio_out.npy")
-
+            matY2 = self.Normalize2out(matY2,nomepasta + "vmax_out.npy",nomepasta + "vmin_out.npy",nomepasta + "media_out.npy",nomepasta + "desvio_out.npy") 
 
 
         #Processo de aprendizado------------------------------------------------------------
 
         VetorErro = [0]
         MenorErro = 999999999
 
@@ -2185,16 +2316,15 @@
         
             c4 = np.dot(c3,P34)- B4
             c4 = self.Activation(self.fa4c,c4)         
 
             # saida----------------------------
             Calculated[caso][:] = c4[:]
 
-        if (self.normout==1):            
-            Calculated = self.DesNormalize(Calculated, nomepasta + "vmax_out.npy", nomepasta + "vmin_out.npy",nomepasta + "media_out.npy",nomepasta + "desvio_out.npy") 
+        Calculated = self.DesNormalizeout(Calculated, nomepasta + "vmax_out.npy", nomepasta + "vmin_out.npy",nomepasta + "media_out.npy",nomepasta + "desvio_out.npy") 
 
         if (self.txt!=0): #print txt out data
              np.savetxt(nomepasta + "out.txt", Calculated)
 
         return Calculated
```

### Comparing `tupa123-1.5.5/tupa123.egg-info/PKG-INFO` & `tupa123-1.5.6/tupa123.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tupa123
-Version: 1.5.5
+Version: 1.5.6
 Summary: fully connected neural network with four layers
 Author: Leandro Schemmer
 Author-email: leandro.schemmer@gmail.com
 License: MIT
 Keywords: artificial-intelligence neural-networks four-layers regression regression-analysis classification-algorithms tupa123 deep-learning machine-learning data-science artificial-neural-network open-source
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

