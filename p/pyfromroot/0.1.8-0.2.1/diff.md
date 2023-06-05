# Comparing `tmp/pyfromroot-0.1.8.tar.gz` & `tmp/pyfromroot-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfromroot-0.1.8.tar", last modified: Thu Apr  7 14:45:48 2022, max compression
+gzip compressed data, was "pyfromroot-0.2.1.tar", last modified: Mon Jun  5 09:04:28 2023, max compression
```

## Comparing `pyfromroot-0.1.8.tar` & `pyfromroot-0.2.1.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2022-04-07 14:45:48.318258 pyfromroot-0.1.8/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     2329 2022-04-07 14:45:48.314258 pyfromroot-0.1.8/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1376 2022-04-07 14:45:44.000000 pyfromroot-0.1.8/README.md
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2022-04-07 14:45:48.314258 pyfromroot-0.1.8/bin/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1789 2022-04-04 17:20:20.000000 pyfromroot-0.1.8/bin/pyfromroot
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2022-04-07 14:45:48.314258 pyfromroot-0.1.8/pyfromroot/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      253 2022-04-04 17:20:20.000000 pyfromroot-0.1.8/pyfromroot/__init__.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    11542 2022-04-07 14:31:55.000000 pyfromroot-0.1.8/pyfromroot/pr_fit.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     7329 2022-04-07 14:05:10.000000 pyfromroot-0.1.8/pyfromroot/pr_load.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     3641 2022-04-07 13:27:02.000000 pyfromroot-0.1.8/pyfromroot/pr_model_decay.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     6601 2022-04-07 14:26:38.000000 pyfromroot-0.1.8/pyfromroot/pr_model_gpol1.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     4097 2022-04-06 11:57:07.000000 pyfromroot-0.1.8/pyfromroot/pr_model_pocall.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     3945 2022-04-06 11:59:21.000000 pyfromroot-0.1.8/pyfromroot/pr_model_polall.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     5234 2022-04-07 14:40:03.000000 pyfromroot-0.1.8/pyfromroot/pr_zoom.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2301 2022-04-04 17:20:20.000000 pyfromroot-0.1.8/pyfromroot/prj_utils.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     6964 2022-04-05 16:04:41.000000 pyfromroot-0.1.8/pyfromroot/prun.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      565 2022-04-04 17:20:20.000000 pyfromroot-0.1.8/pyfromroot/unitname.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2022-04-07 14:45:47.000000 pyfromroot-0.1.8/pyfromroot/version.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2022-04-07 14:45:48.314258 pyfromroot-0.1.8/pyfromroot.egg-info/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     2329 2022-04-07 14:45:48.000000 pyfromroot-0.1.8/pyfromroot.egg-info/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      496 2022-04-07 14:45:48.000000 pyfromroot-0.1.8/pyfromroot.egg-info/SOURCES.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2022-04-07 14:45:48.000000 pyfromroot-0.1.8/pyfromroot.egg-info/dependency_links.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        5 2022-04-07 14:45:48.000000 pyfromroot-0.1.8/pyfromroot.egg-info/requires.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       11 2022-04-07 14:45:48.000000 pyfromroot-0.1.8/pyfromroot.egg-info/top_level.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2022-04-07 14:45:48.318258 pyfromroot-0.1.8/setup.cfg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1163 2022-04-05 08:32:29.000000 pyfromroot-0.1.8/setup.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-05 09:04:28.873340 pyfromroot-0.2.1/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    10569 2023-06-05 09:04:28.873340 pyfromroot-0.2.1/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    10303 2023-03-15 09:15:20.000000 pyfromroot-0.2.1/README.md
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-05 09:04:28.869340 pyfromroot-0.2.1/bin/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    11413 2023-03-15 09:15:20.000000 pyfromroot-0.2.1/bin/pyfromroot
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-05 09:04:28.873340 pyfromroot-0.2.1/pyfromroot/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      253 2023-03-15 09:15:20.000000 pyfromroot-0.2.1/pyfromroot/__init__.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     3880 2023-03-15 09:15:20.000000 pyfromroot-0.2.1/pyfromroot/pr_draw.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    17383 2023-03-16 17:23:03.000000 pyfromroot-0.2.1/pyfromroot/pr_fit.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     9850 2023-03-15 09:15:20.000000 pyfromroot-0.2.1/pyfromroot/pr_load.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     3678 2023-03-15 09:15:20.000000 pyfromroot-0.2.1/pyfromroot/pr_model_decay.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     9945 2023-03-16 17:21:17.000000 pyfromroot-0.2.1/pyfromroot/pr_model_gpol1.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     5984 2023-03-15 09:15:20.000000 pyfromroot-0.2.1/pyfromroot/pr_model_logxy.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     6835 2023-03-15 09:15:20.000000 pyfromroot-0.2.1/pyfromroot/pr_model_pocall.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     5516 2023-03-15 09:15:20.000000 pyfromroot-0.2.1/pyfromroot/pr_model_polall.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     5407 2023-03-15 09:15:20.000000 pyfromroot-0.2.1/pyfromroot/pr_zoom.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2301 2023-03-15 09:15:20.000000 pyfromroot-0.2.1/pyfromroot/prj_utils.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     8691 2023-03-15 09:15:20.000000 pyfromroot-0.2.1/pyfromroot/prun.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      565 2023-03-15 09:15:20.000000 pyfromroot-0.2.1/pyfromroot/unitname.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-06-05 09:04:28.000000 pyfromroot-0.2.1/pyfromroot/version.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-05 09:04:28.873340 pyfromroot-0.2.1/pyfromroot.egg-info/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    10569 2023-06-05 09:04:28.000000 pyfromroot-0.2.1/pyfromroot.egg-info/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      547 2023-06-05 09:04:28.000000 pyfromroot-0.2.1/pyfromroot.egg-info/SOURCES.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-06-05 09:04:28.000000 pyfromroot-0.2.1/pyfromroot.egg-info/dependency_links.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       54 2023-06-05 09:04:28.000000 pyfromroot-0.2.1/pyfromroot.egg-info/requires.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       11 2023-06-05 09:04:28.000000 pyfromroot-0.2.1/pyfromroot.egg-info/top_level.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-06-05 09:04:28.873340 pyfromroot-0.2.1/setup.cfg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1367 2023-04-03 13:37:30.000000 pyfromroot-0.2.1/setup.py
```

### Comparing `pyfromroot-0.1.8/pyfromroot/pr_fit.py` & `pyfromroot-0.2.1/pyfromroot/pr_fit.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python3
-
+import re
 import ROOT
 import numpy as np
 from array import array
 import random
 import os
 import pandas as pd
 
@@ -17,18 +17,28 @@
 
 # ------------------------- MINUIT PART ----------------
 #  pip3 install iminout  numba_stats numpy
 from iminuit import cost, Minuit
 import iminuit
 from numba_stats import norm, uniform # faster replacements for scipy.stats functions
 
-
 import glob
 
-def main( *args ):
+import time
+
+
+
+
+
+#def main( *args, **kwargs ):
+def main( *args, **kwargs ):
+    """
+ call fit models on histo and TGraphs; returns data_dict if present
+  canvas="fitresult...."
+    """
     if len(args)<1:
         print("X... no object name given  (and no model given too)")
         return
     if len(args)<2:
         print("X... no model given, I try to look for them")
         files = glob.glob("pr_model*.py")
         if len(files)==0:
@@ -37,24 +47,54 @@
         else:
             files = [x for x in files if x.find("pr_model_")>=0]
             files = [x.split("_")[2].split(".")[0] for x in files]
             print(f"i... available  FIT models: \n{files}")
             return
 
 
+
+
+    # I dont go back to previous CANVAS, It is not sure that i is not a PAD
+    # c_orig = None
+    # if ROOT.addressof(ROOT.gPad)!=0:
+    #     #print("\n\n\n\nD... 1FIT   I have a gpad active",ROOT.addressof(ROOT.gPad))
+    #     c_orig = ROOT.gPad.GetCanvas()
+    #     #print("\n\n\n\nD... 1FIT   I have a gpad active",ROOT.addressof(c_orig))
+    # #else:
+    #     #print("\n\n\n\nD...  1FIT I have NONONO gpad active")
+
+    #time.sleep(1)
+
+
     fname = args[0]
-    g_orig = ROOT.gDirectory.FindObject(f"{fname}")
+    g_orig = ROOT.gDirectory.FindObject(fname)
+    if g_orig:
+        print("i... OBJECT FOUND gD ==", g_orig)
+    else:
+        print("X... not found in gD", g_orig)
 
+        print("i... I must search in GetListOfSpecials() ")
+        g_orig = ROOT.gROOT.GetListOfSpecials().FindObject(fname)
+        if g_orig:
+            print("i... OBJECT FOUND LSOS ==", g_orig)
+        else:
+            print("X... OBJECT NOT FOUND LSOS ==", g_orig)
+    #ROOT.gROOT.GetListOfSpecials().ls()
+    #ROOT.gROOT.GetListOfSpecials().ls()
+    #print("DIR:")
+    #ROOT.gDirectory.ls()
+    #print("--------")
 
 
     # - check the object. If None => try to load something
     #        AUTOMATIC LOAD
     #
-    if g_orig==None:
+    if g_orig is None:
         print(f"X... {fname} object doesnot exist in gDirectory")
+        sys.exit(0)
         # - do we try to load it? If it is an actual file
         if os.path.exists(fname):
             print(f"i... BUT file /{fname} exists")
             print(f" ...       trying to unload and load /pr_load/")
             try:
                 sys.modules.pop( "pr_load" )
             except:
@@ -76,41 +116,53 @@
             g_orig = ROOT.gDirectory.FindObject( fname )
 
 
     # MODULE========================================== I call again prun;
 
     shape = args[1]
     polorder = None
+    print(f"fit.main.{shape}")
 
     # print (len(shape))
     # print( shape.find("pol") )
     # print(  shape[-1] )
     # print( [ str(i) for i in range(0,10) ] )
 
+
+
     # POL0-9
+    polorder = 1
     if (len(shape)==4) and (shape.find("pol")==0) and ( shape[-1] in [ str(i) for i in range(0,10) ] ):
-        print("i... POLi model shape  detected")
+        print("i... POLi model shape  DEMANDED")
         polorder = int(shape[-1])
         shape = "polall"
 
     # POC0-9 - chebyshev
     if (len(shape)==4) and (shape.find("poc")==0) and ( shape[-1] in [ str(i) for i in range(0,10) ] ):
-        print("i... POLi model shape  detected")
+        print("i... POLi model shape  DEMANDED")
         polorder = int(shape[-1])
         shape = "pocall"
 
+    # np exp  np log - logxy
+    if (len(shape)==6) and (shape.find("logxy")==0) and ( shape[-1] in [ str(i) for i in range(0,10) ] ):
+        print("i... LOGXYi model  shape  DEMANDED")
+        polorder = int(shape[-1])
+        shape = "logxy"
+
     model_name = f"model_{shape}"
     module = prun.import_module( model_name )
 
 
 
 
     if module is None:
         print(f"X... module {model_name} not found...")
         return
+    #else:
+    #    print(f"                              {model_name}                    LOADED")
     #if not(os.path.exists(f"{model}.py")):
     #    print(f"X... required model file  {model}.py does not exist")
     #    return
 
     #------------------------------ MODEL SHOULD BE LOADED HERE ------
 
     # # UNimport module first - case there was an error there previously
@@ -123,15 +175,14 @@
     # module = importlib.import_module( model )
     #------------------------------------------------------
 
 
 
 
 
-
     print(f"i... extracting /{g_orig.GetName()}/ of type /{g_orig.ClassName()}/")
 
     # -------------------------------   get Arrays -> import to numpy  .asarray
     ishisto = False
 
     if g_orig.ClassName()=="TGraph":
         x=np.asarray( g_orig.GetX() )
@@ -158,39 +209,55 @@
         #   x chan -0.5 to compensate midbin!
         #
         #  NASTY TRICK - x=x-zx1 -> and back...... I cannot converge at 7000chan
         #
         #
         zx1,zx2 = g_orig.GetXaxis().GetFirst(),g_orig.GetXaxis().GetLast()
 
-        x  = np.asarray( np.arange( zx1,  zx2+1 ) ,  np.float64 )
+        x_ = np.arange( 1.0*zx1,  zx2+1.0  )
+        x  = np.asarray( x_ )
         #
         # i have proble with large distances
         #
         #x  = np.asarray( np.arange( zx1-zx1,  zx2+1-zx1 ) ,  np.float64 )
         #x = x + 0.5 # bin center
         y  = np.zeros_like(x)
         dy = np.zeros_like(y)+1
 
+        miner = 1.0
+        for i in range(zx1,zx2+1): # zx1,zx2+1 all range
+            if miner>g_orig.GetBinError(i) and g_orig.GetBinError(i)>0.:
+                miner = g_orig.GetBinError(i)
 
         for i in range(zx1,zx2+1): # zx1,zx2+1 all range
             # i checked that I must -0.5 as bin[0] is underflow
             x[i-zx1] = float(x[i-zx1] - 0.5)
             y[i-zx1] = g_orig.GetBinContent( i)
-            if y[i-zx1]>0:
-                dy[i-zx1]=np.sqrt(y[i-zx1])
+            ddyy = g_orig.GetBinError(i)
+            if ddyy==0:
+                dy[i-zx1] = miner
+            else:
+                dy[i-zx1] = ddyy
+            if y[i-zx1]==0:
+                dy[i-zx1]=miner
+                #dy[i-zx1]=np.sqrt(y[i-zx1])
                 #dy[i-zx1]=10
 
         dx = np.zeros_like(x)
 
+        # NONONO dy[dy==0]=1.0
+        print( list(dy) )
 
-        x = np.array(  x  ,  np.float64)
-        y = np.array(  y  ,  np.float64)
-        dx = np.array(  dx  ,  np.float64)
-        dy = np.array(  dy  ,  np.float64)
+        #x = np.array(  x  ,  np.float64)
+        #y = np.array(  y  ,  np.float64)
+        #dx = np.array(  dx  ,  np.float64)
+        #print( type(dy) )
+        #print( len(dy) )
+        #print( dy )
+        #dy = np.array(  dy  ,  np.float64)
         #dx=np.asarray( g_orig.GetEX() )
         #dy=np.asarray( g_orig.GetEY() )
         #cala = (g_orig.GetXaxis().GetXmax() - g_orig.GetXaxis().GetXmin() )/( g_orig.GetNbinsX() )
         #calb =  g_orig.GetXaxis().GetXmax() - cala*g_orig.GetNbinsX()
 
     #---------------------------------------- DONE with importing TGraphs or histos ----------
 
@@ -203,114 +270,208 @@
 
 
 
     #-*********************************now the MINUIT PART
     #-*********************************now the MINUIT PART
     # x is channels, even if there is a calibration
     #
-    #NOT POSSIBLE....area destorts    #  x = cala*x + calb
+    #NOT POSSIBLE to send calibrated. ....area destorts    #  x = cala*x + calb
+
+    #print( type(dy) )
+    #print( len(dy) )
+    #print(".iii")  crashed !!!!!!!!!!!
+    #print(dy)
     yf = module.main( x,y,dy , polorder )
 
 
 
 
 
 
 
     # --- I can output the results.  I do it for : gpol1
     #print(type(yf))
-
+    xf10 = None
+    yf10 = None
+    #yf = returns.....
     if type(yf) is np.ndarray:
-        print("")
+        print("D...     direct return of yf")
+        yf10 = yf
+        xf10 = x
 
     elif type(yf) is tuple: # ------------ i wanted to get 3 functions (fit,low,high)
+        print("D...     TUPLE return of yf,  upper,lower bound.... not good")
         yf,yf_l,yf_h=yf[0],yf[1],yf[2]
+        yf10 = yf
+        xf10 = x
 
-    elif  type(yf) is dict:
-        print("i... full dict of data return")
+
+    elif  type(yf) is dict: #*------------------------ ALL DATA
+        #print("i... full dict of data return")
         data_dict = yf
+
         #yf_l = data_dict['yf_l']
         #yf_h = data_dict['yf_h']
         yf   = data_dict['yf']
+        yf10 = yf
+        xf10 = x
+
+        if 'yf10' in data_dict:
+            yf10   = data_dict['yf10']
+            xf10   = data_dict['xf10']
 
     else:
         print("X... I am watching the output of the fit module. Unknown. Stop") # just yf values to plot
         return
         #-*********************************now the MINUIT PART
     #-*********************************now the MINUIT PART
 
     #x = x + zx1 # trick to converge
 
 
 
 
+    # ///////////////////////////////////////////////////// plotting results OR QUIT
 
+    # canvasname = "fitresult"
+    #print( "KW:", kwargs.keys() )
+    if "canvas" in kwargs.keys():
+        canvasname = kwargs["canvas"]
+    else:
+        canvasname = None
 
+    if canvasname is None:
+        print("F... RETURN FROM FIT :) no canv")
+        if "data_dict" in locals():
+            return data_dict
+        else:
+            return
     # ///////////////////////////////////////////////////// plotting results
-    cmain = ROOT.gROOT.GetListOfCanvases().FindObject("fitresult")
+
+    cmain = ROOT.gROOT.GetListOfCanvases().FindObject( canvasname )
     if ROOT.addressof(cmain)==0:
-        print("i... creating a new /fitresult/ canvas")
-        cmain = ROOT.TCanvas("fitresult","fitresult",600,800)
-        print("i... creating a new /fitresult/ canvas draw")
+        print(f"i... creating a new /{canvasname}/ canvas")
+        cmain = ROOT.TCanvas(canvasname,canvasname,600,800)
+        print(f"i... creating a new /{canvasname}/ canvas draw")
         cmain.Draw()
-        print("i... creating a new /fitresult/ canvas drawn")
+        cmain.Divide(1,2) # div canvas
+        print(f"i... creating a new /{canvasname}/ canvas drawn")
         #cmain = ROOT.gPad.GetCanvas()  # reset all canvas
 
     cmain.SetFillColor(19)
-    cmain.Clear()
-    print("i... div a new /fitresult/ canvas")
-    cmain.Divide(1,2) # div canvas
+    #cmain.Clear()
+    #print("i... div a new /fitresult/ canvas")
     cmain.cd(1)
 
+
+
     ####g_xy = ROOT.TGraph( len(x) , x.flatten("C"), yf.flatten("C") )
     g_orig.SetMarkerStyle(7) # small circle , no lines...
 
     # if low number of points-plit triagles
     if len(x)<15: g_orig.SetMarkerStyle(22)
     g_orig.Draw() # for histo NOT PAWL;  it works with NO PAWL TGraph too
     ROOT.gPad.Modified()
     ROOT.gPad.Update()
 
+
     #x = x[:5]
     #yf= yf[:5]
     #y = y[:5]
     #print(type(x),  len(x)  , x)
     #print(type(yf), len(yf) , yf)
 
 
-    # --------------------- result plotted ---------------
+
+    # --------------------- resulting fit plotted ---------------
+    magenta = 3
     if ishisto:
         #print(g_orig.GetXaxis().GetXmin()  , g_orig.GetXaxis().GetXmax() )
         cala = (g_orig.GetXaxis().GetXmax() - g_orig.GetXaxis().GetXmin() )/( g_orig.GetNbinsX() )
         calb =  g_orig.GetXaxis().GetXmax() - cala*g_orig.GetNbinsX()
         #print(x)
         x = cala*x + calb
+        xf10 = cala*xf10 + calb # I have a problem with calibration
 
         data_dict["cala"] = cala
         data_dict["calb"] = calb
 
         data_dict["E"] = cala*data_dict["channel"]+calb
         data_dict["dE"] = cala*data_dict["dchannel"]
 
         data_dict["Efwhm"] = cala*data_dict["fwhm"]
 
-        print(f"Energies:  {data_dict['E']:12.2f} +- {data_dict['dE']:8.2f}  fwhm= {data_dict['Efwhm']:4.2f}")
+        data_dict["dEfwhm"] = cala*data_dict["dfwhm"]
+
+
+        # do yourselves somewhere
+        #print(f"Energies:  {data_dict['E']:12.2f} +- {data_dict['dE']:8.2f}  fwhm= {data_dict['Efwhm']:4.2f}")
 
 
+        if abs(data_dict['diff_fit_int_proc'])>1:
+            print("X...  BAD DESCRIPTION - DIFF fit/area MORE THAN 1%")
+            magenta = 2
+        if  not( data_dict['noerror']):
+            print("X...  BAD DESCRIPTION - SOME ERROR OF FIT")
+            magenta = 2
+        if data_dict['area'] <= 2*data_dict['darea']:
+            print("X...  BAD DESCRIPTION - Area error too large")
+            magenta = 2
+        if data_dict['fwhm'] <= 2*data_dict['dfwhm']:
+            print("X...  BAD DESCRIPTION - FWHM error too large")
+            magenta = 2
+
 
         #print(x)
         #print(cala,calb)
-    gf = ROOT.TGraph( len(x) , x.flatten("C"), yf.flatten("C") )
-    gf.SetLineColor(6) # 5 yellow 6 magenta
-    gf.SetLineWidth(2)
+    #-----------------------------------
+
+    if xf10 is None:
+        gf = ROOT.TGraph( len(x) , x.flatten("C"), yf.flatten("C") )
+    else:
+        #print(xf10)
+        #print(yf10)
+        gf = ROOT.TGraph( len(xf10) , xf10.flatten("C"), yf10.flatten("C") )
+
+
+        # specific for efficiency
+        try:
+            position = os.path.splitext( g_orig.GetTitle() )[0]
+            position = int( re.findall(r"\d+", position)[0] )
+            print("i... Title of graph is ",g_orig.GetTitle() , position )
+
+            # writing out tab; with all points --- for efficiency---
+            with open(f"out{position}.tab", "w" ) as f:
+                #f.write( "\n".join( str(yf10).strip("][").split() )+"\n"  )
+                ar2d = np.vstack( (xf10, yf10) ).T
+                #print(ar2d)
+                np.savetxt( f, ar2d )
+            with open("oparams.txt","a") as f:
+                f.write( f"{position}  {data_dict['a']} {data_dict['da']}  {data_dict['b']}   {data_dict['db']}  {data_dict['c']}  {data_dict['dc']}  {data_dict['e']} {data_dict['de']}\n" )
+        except:
+            print(" ... no model output was saved (pr_fit)")
+
+
+    #print(data_dict.keys())
+    #gf.Print()
+    gf.SetLineColor(magenta) # red2/green3 ...   5 yellow 6 magenta
+    gf.SetMarkerColor(magenta) # red2/green3 ...   5 yellow 6 magenta
+    gf.SetMarkerStyle(7) # red2/green3 ...   5 yellow 6 magenta
+    gf.SetLineWidth(1)
     #gf.SetFillStyle(3004)
     #gf.SetFillColor(6)
     #gf.SetFillColorAlpha( 6, 0.05)
     #gf.Draw("sameLF") # i liked to fill gaus F
-    gf.Draw("sameL")
+    gf.Draw("samePL")
+    if ('data_dict' in locals()) and ( 'logy' in data_dict):
+        if data_dict['logy']:
+            ROOT.gPad.SetLogy()
+    if('data_dict' in locals()) and ( 'logx' in data_dict):
+        if data_dict['logx']:
+            ROOT.gPad.SetLogx()
 
 
     # if not ("yf_l" in locals()):
     #     yf_l = yf
     # # --------------------- result plotted ---------------
     # gf_l = ROOT.TGraph( len(x) , x.flatten("C"), yf_l.flatten("C") )
     # gf_l.SetLineColor(6) # 5 yellow
@@ -333,14 +494,16 @@
     ROOT.gPad.Update()
 
 
 
 
 
 
+
+
     cmain.cd(2) # --------second pad --------------------------
     # ------ differences ------------------
     #gfy=np.asarray( gf.GetY() )
     gfy = yf
     diffy = y-gfy
     gf_diff= ROOT.TGraphErrors( len(x) , x.flatten("C"),
                                 diffy.flatten("C"),
@@ -350,47 +513,66 @@
 
     # keep the axes' labels from original graph
 
     newtitle =  f"exp-fit:{g_orig.GetTitle()};{g_orig.GetXaxis().GetTitle()};{g_orig.GetYaxis().GetTitle()}-fit"
     #print(f"NEWTITLE={newtitle}")
     gf_diff.SetTitle( newtitle)
     gf_diff.SetMarkerStyle(7) # small circle , no lines...
-    gf_diff.SetLineColor(4)
+    gf_diff.SetLineColor(4) #
     gf_diff.Draw("PAW")
 
 
     # plotting the red line of perfect fit
 
     zeroy = y-y
     gf_zero= ROOT.TGraph( len(x) , x.flatten("C"), zeroy.flatten("C")  )
-    gf_zero.SetLineColor(2)
+    #gf_zero.SetLineColor(2) # red line at 0
+    gf_zero.SetLineColor(magenta) # CODE FOR RESULT COLOR  line at 0
     gf_zero.Draw("same")
     ROOT.gPad.SetGrid()
     ROOT.gPad.SetLogy( False)
     ROOT.gPad.Modified()
     ROOT.gPad.Update()
 
 
 
+    #  NOT GOING back to original CANVAS here... may be PAD too
+    # if c_orig is not None:
+    #     #print("\n\n\n\nD... going back              ",ROOT.addressof(c_orig))
+    #     #print("\n\n\nD... going back to main TCanvas")
+    #     c_orig.cd()
+    # #else:
+    #     #print("\n\n\nD... NONONO going back to main TCanvas")
+
+        #time.sleep(1)
+
     #-------------------------- I NEED to REGISTER all to be able to display on gPad
 
 
-    prun.register(cmain, "fitresult")
+    prun.register(cmain, canvasname) # REGISTER CANVAS
 
     prun.register(gf, "fit")
     #prun.register(gf_l, "fit_low")
     #prun.register(gf_h, "fit_high")
     prun.register(gf_diff, "fitdiff")
     prun.register(gf_zero, "linezero")
 
+
+
     if "data_dict" in locals():
         return data_dict
     else:
         return
 
 
+
+
+
+
+
+
 if __name__=="__main__":
     Fire(main)
     # update canvas
     #ROOT.gPad.Modified()
     #ROOT.gPad.Update()
     input('press ENTER to end...')
```

### Comparing `pyfromroot-0.1.8/pyfromroot/pr_load.py` & `pyfromroot-0.2.1/pyfromroot/pr_load.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,41 +3,59 @@
 import ROOT
 import numpy as np
 from array import array
 import random
 import os
 import pandas as pd
 
+
 from fire import Fire
 
 #import prun # looks like mutual import, but it is not really
 from  pyfromroot import prun
 
 import ROOT
 import time
+
+
+from  fastnumbers import isfloat
+
+
+
+
 #   the DAT file can contain TAGS:
 #   #COLNAME: frame,x,y     ... column names (selfexplaining)
 #   #LOAD_AS: x,dx,y,dy     ... order of columns  for x,y,dx,dy TGraph(Errors)
 #
 
 
+
+
 def create_histo(df, hpos, cala, calb ):
+    """
+    TH1F * created
+    """
     x = np.array(  df[ df.columns[hpos] ]  ,  np.float64)
     h = ROOT.TH1F( "h", "h", len(df), 0, len(df) )
     bn = 0
     for bc in x:
         bn+=1
         h.SetBinContent(  bn, bc )
     h.GetXaxis().SetLimits( calb, cala*len(df)+calb )
     return h
 
 
 
+
+
+
+
+
 #---------------------------------------------
-def main( *args ):
+def main( *args , **kwargs):
 
     print(f"i... @load: args={args}")
     if len(args)==0:
         print("X... no file given")
         return
 
     fname = args[0]
@@ -61,41 +79,80 @@
 
     else:
         print("D... ok, no argument that would take a priority")
 
 
     # - LOAD_AS x,y,dx,dy CODES for columns and COLNAMES inside the file ---
     #  and handle the priority of ARGS xydxdy ..............
+    # names is nice columns names - xynames is x y dx dy
     names = []
     if xynames is None: xynames = []
     columns = 0
+
+
+    # first try is searching for 10 lines and COLNAME: LOAD_AS
+    #  1st line maybe #COLNAME without pragma?
+    line1st = True
+    line1stascolname = False
+    line1stnames = [] # stays [] if False
+    line1stheader = None # normally no header
+
     with open(fname) as f:
         #print("i... looking the file for COLNAMES: and LOAD_AS:")
         i = 0
         for com in f:
             com = com.strip()
             #print(com)
             i+=1
             if i>10: break
             com=com.strip()
-            if com.find("#")!=0:
+            if com.find("#")<0:
+                if line1st:
+                    line1st = False
+                    columns = com.split()
+                    line1stnames = com.split()
+
+                    # - at least twoONE values are float -> it is not a header
+                    num_floats = 0
+                    for i2 in columns:
+                        if isfloat(i2):
+                            num_floats+=1
+                    if num_floats >= 1:
+                        line1stascolname = False
+                    else:
+                        line1stascolname = True
+
+                        # try:
+                        #     float(i2) # if any of conversions is an error
+                        # except:
+                        #     line1stascolname = True
+
                 columns = len(com.split())
             if com.find("#COLNAME:")==0:
                 names2 = com.split(":")[1].strip().split(",")
                 names = names2
+                print("NAMES == {names}")
 
             if com.find("#LOAD_AS:")==0:
                 # overrides?
                 names2 = com.split(":")[1].strip().split(",")
                 if (len(names2)>1)and( 'x' in names2)and('y' in names2): # x,y at least
                     if len(xynames)==0:
                         xynames = names2
 
 
 
+    print("i... existing # of columns = ", columns)
+    print("i... 1 COLNAME:",names)
+    print("i... ... backup names = ", line1stnames)
+    print("i... 1 LOAD_AS:" ,xynames)
+    if line1stascolname:
+        names = line1stnames
+        line1stheader = 1
+    #print(names,xynames)
     #--- here I must play with CALIB -------------------------------------
     cala = 1
     calb = 0
     for i in xynames:
         if i.find("cala=")==0: cala = float(i.split("=")[-1])
         if i.find("calb=")==0: calb = float(i.split("=")[-1])
 
@@ -109,18 +166,22 @@
 
     # here I do the correct number of columns - BUTBUT later I do the same....
     while len(xynames)<columns:
         xynames.append(f"c_{len(xynames)}")
 
     for i in range(len(xynames)):
         if xynames[i]=="_":xynames[i]=f"col_{i}"
+    for i in range(len(names)):
+        if names[i]=="_":names[i]=f"col_{i}"
 
 
     if len(names)==0: names=xynames
-    if len(names)!=len(xynames): names=xynames
+    if len(names)!=len(xynames):
+        print("!... redoing names",names)
+        names=xynames
 
 
 
     #
     # HERE, all column names should be defined, if available
     # Order is defined by now
     #
@@ -138,106 +199,127 @@
             print("X... try  x,y,dx,dy  or y,x ...." )
             return
         else:
             histo = True
 
 
     # count columns first to be sure it matches the names ;ADD fake colnames
+    print("i... TRYING TO SUGGEST csv structure ............")
+    #print(names)
     df = pd.read_csv(fname, delimiter="\s+", header=None, comment="#", nrows=2)
     i=1
     while len(names) <  df.shape[1]:
         names.append(f"col{i:d}")
         i+=1
-
-    print("TRYING TO SUGGEST............")
-    print(df)
+    print("i... names==",names)
 
     if len(names)!=df.shape[1]:
-        print(f"X... column probl: names={len(names)} i={i} dfcols={df.shape}" )
+        print(f"X... column problem: names={len(names)} i={i} dfcols={df.shape}" )
 
     # read all data now; column names are from COLNAMES or xynames(if not def)
-    df = pd.read_csv(fname, delimiter="\s+", header=None, comment="#", names = names )
+    df = pd.read_csv(fname, delimiter="\s+", header=line1stheader, comment="#", names = names )
+    print("---------------df---------------")
     print(df)
 
     #
     # HERE THE DF SHOULD BE PERFECTLY LOADED with colnames, defined x,y, maybe++
     #
 
-    # ------ graph name in CLING
-    NAME1 = os.path.splitext(fname)[0]
-    print(f"D... graph name = {NAME1}")
 
 
 
     #------------------------------ HISTO OR GRAPH --------------
     if histo:
         hpos = xynames.index('h')
         print(f"i... h position {hpos}")
         print(f"i... hname= {names[hpos]} ")
+        NAME1 = os.path.splitext(fname)[0]
     else:
         xpos = xynames.index('x')
         ypos = xynames.index('y')
         print(f"i... x position {xpos}  y position {ypos}")
         print(f"i... xname= {names[xpos]}  yname= {names[ypos]}")
+        NAME1 = os.path.splitext(fname)[0]+f"_{names[xpos]}_{names[ypos]}"
+    # ------ graph name in CLING - I enhance with variables - move after xpos
+    #  I need to save 2 same graphs:
+    #     - one without any _x_y to be accessible easily
+    #     - one with _x_y that is specific and made accessible after more loads
+    #
+
+
+    NAMEO = os.path.splitext(fname)[0]
+    print(f"D... graph name = {NAMEO}; for multiloads=>{NAME1} ")
 
 
     if histo:
-        g = create_histo(df, hpos, cala, calb)
-        g.Draw()
-        g.SetTitle(f"{NAME1};channel;{names[hpos]}")
-        ROOT.gPad.SetLogy()
-        g.Print()
+        # it will be TH1F
+
+        gontainer = create_histo(df, hpos, cala, calb)
+        #gontainer.Draw()
+        gontainer.SetTitle(f"{NAME1};channel;{names[hpos]}")
+        #ROOT.gPad.SetLogy()
+        gontainer.Print()
+
 
     else:
+        # gontainer will be TGraphErrors
 
         x = np.array(  df[ df.columns[xpos] ]  ,  np.float64)
         y = np.array(  df[ df.columns[ypos] ]  ,  np.float64)
 
         #
         # check if dx and/or dy  given
         #
 
-        if ('dx' in names)and('dy' in names):
+        if ('dx' in xynames)and('dy' in xynames):
             dxpos = xynames.index('dx')
             dypos = xynames.index('dy')
             dx = np.array(  df[ df.columns[dxpos] ]  ,  np.float64)
             dy = np.array(  df[ df.columns[dypos] ]  ,  np.float64)
-            g = ROOT.TGraphErrors( len(x) , x.flatten("C"), y.flatten("C"), dx.flatten("C"), dy.flatten("C") )
-        elif ('dx' in names):
+            gontainer = ROOT.TGraphErrors( len(x) , x.flatten("C"), y.flatten("C"), dx.flatten("C"), dy.flatten("C") )
+        elif ('dx' in xynames):
             dxpos = xynames.index('dx')
             dx = np.array(  df[ df.columns[dxpos] ]  ,  np.float64)
             dy = np.zeros_like(y)
-            g = ROOT.TGraphErrors( len(x) , x.flatten("C"), y.flatten("C"), dx.flatten("C"), dy.flatten("C") )
-        elif ('dy' in names):
+            gontainer = ROOT.TGraphErrors( len(x) , x.flatten("C"), y.flatten("C"), dx.flatten("C"), dy.flatten("C") )
+        elif ('dy' in xynames):
             dypos = xynames.index('dy')
             dy = np.array(  df[ df.columns[dypos] ]  ,  np.float64)
             dx = np.zeros_like(x)
-            g = ROOT.TGraphErrors( len(x) , x.flatten("C"), y.flatten("C"), dx.flatten("C"), dy.flatten("C") )
+            gontainer = ROOT.TGraphErrors( len(x) , x.flatten("C"), y.flatten("C"), dx.flatten("C"), dy.flatten("C") )
         else:
-            g = ROOT.TGraph( len(x) , x.flatten("C"), y.flatten("C") )
+            gontainer = ROOT.TGraph( len(x) , x.flatten("C"), y.flatten("C") )
 
         #
         # PLOT
         #  xpos and ypos are for axis labels
         #
         #g.Print()
         # plot nicely on (maybe new) TCanvas
-        g.SetMarkerStyle(7) # small circle , no lines...
-        g.SetMarkerStyle(1) # small circle , no lines...
-        g.SetMarkerStyle(22) # small...
-        g.SetTitle(f"{NAME1};{names[xpos]};{names[ypos]}")
-        g.Draw("PAW") # no lines...
-
-    # ------------------------------ END OF GRAPH / HISTO ---------------
-    ROOT.gPad.SetGrid()
-    prun.register(g,NAME1)
-    ROOT.gPad.Modified()
-    ROOT.gPad.Update()
+        gontainer.SetMarkerStyle(7) # small circle , no lines...
+        gontainer.SetMarkerStyle(1) # small circle , no lines...
+        gontainer.SetMarkerStyle(22) # small...
+
+        #g.SetName(f"{NAME1}") # done in prun register
+        gontainer.SetTitle(f"{NAME1};{names[xpos]};{names[ypos]}")
+        #gontainer.Draw("PAW") # no lines...
+
+    # ------------------------------ END OF GRAPH / HISTO : common ----------
+    #ROOT.gPad.SetGrid()
+    prun.register(gontainer,NAME1) # register to SPecials with _x_y
+    prun.register(gontainer,NAMEO) # register to SPecials sole simple
+    #ROOT.gPad.Modified()
+    #ROOT.gPad.Update()
 
     return
 
+
+
+
+
+#############################################################################
 if __name__=="__main__":
     Fire(main)
     print("H... close canvas to exit...")
     while ROOT.addressof(ROOT.gPad)!=0:
         time.sleep(0.2)
     #input('press ENTER to end...')
```

### Comparing `pyfromroot-0.1.8/pyfromroot/pr_model_decay.py` & `pyfromroot-0.2.1/pyfromroot/pr_model_decay.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,16 @@
 
 
 
 
 
     # ---- for histograms, use cx...
     print(".............iminuit.............>")
+    if len(x)<3:
+        return None
     c2 = cost.LeastSquares(x, y, dy, model_chi2)
 
 
     m2 = Minuit(c2,
                 a = 1,
                 t12 = 100)
```

### Comparing `pyfromroot-0.1.8/pyfromroot/pr_model_pocall.py` & `pyfromroot-0.2.1/pyfromroot/pr_model_polall.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,91 +3,119 @@
 #  pip3 install iminout  numba_stats numpy
 #
 from iminuit import cost, Minuit
 import iminuit
 from numba_stats import norm, uniform # faster replacements for scipy.stats functions
 import numpy as np
 
+#from termcolor import colored
+from console import fg, fx
+
+import re
+
 
 #
-# I need to go to chebyshev -no good for calibrations....
+# NONONO.... I need to go to chebyshev
 #
 
-def print_errors(m2, chi2dof):
-    """
-    I allow a,b,c,d,...  I have longer decimal places
-    """
-    WID =65
-    print
-    print("_"*WID)
-    zn = ""
-    if chi2dof>1:    zn = "*"
-    print(f" name              value     error{zn}       error%   remark")
-    print("_"*WID)
-    for key in m2.parameters:
-        #if len(key)==1:
-        #    continue
-
-        err = m2.errors[key]
-        val = m2.values[key]
-        if val<0:val=-val
-
-        if chi2dof>1:
-            err = err * np.sqrt(chi2dof)
-
-        print(f"| {key:7} | {val:11.4f} | {err:9.4f}  |  {100*err/val:6.1f}% |", end="")
-        if key=="area":
-            print(f" {100/np.sqrt(val):5.2f}%  (sqrt)|")
-        elif key=="fwhm":
-            print(f" {100*m2.values['fwhm']/m2.values['channel']:5.2f}%  (reso)|")
-        else:
-            print(f"               |")
-
-
-    print("_"*WID)
-    if chi2dof>1: print(f"*... errors WERE scaled up  {np.sqrt(chi2dof):.1f}x     for chi2={chi2dof:.1f} !")
-    print(f"i... Chebyshev parameters are not real! they are for shifted X")
+
+def main(x,y,dy, polorder = None):
+    print("__________________________________________________ poly")
+    #global bin1 # trick for better convergence
+    #bin1 = x[0]
 
 
 
 
-def main(x,y,dy, polorder = None):
-    print("__________________________________________________")
 
-    global bin1 # trick for better convergence
-    bin1 = x[0]
+    def print_errors(m2, chi2dof):
+        """
+        I allow a,b,c,d,...  I have longer decimal places
+        """
+        WID =65
+        print
+        print("_"*WID)
+        zn = ""
+
+        form = "  "
+        xpol = len(m2.parameters)
+        xpolm = len(m2.parameters)
+
+        if chi2dof>1:    zn = "*"
+        print(f" name              value     error{zn}       error%   remark")
+        print("_"*WID)
+        for key in m2.parameters:
+            #if len(key)==1:
+            #    continue
+
+            err = m2.errors[key]
+            val = m2.values[key]
+            # if val<0:val=-val #why the hell this?
+
+            if chi2dof>1:
+                err = err * np.sqrt(chi2dof)
+            if val==0:
+                errproc = None
+            else:
+                errproc = 100*err/val
+                if errproc<0: errproc = -errproc
+
+            print(f"| {key:7} | {val:12.8f} | {err:9.8f}  |  {errproc}% |", end="")
+
+            xpol-=1
+            form=f"{form} {val:.8f}{'*x'*xpol}"
+            if xpol!=0: form+=" +"
+
+
+            if key=="area":
+                print(f" {100/np.sqrt(val):5.2f}%  (sqrt)|")
+            elif key=="fwhm":
+                print(f" {100*m2.values['fwhm']/m2.values['channel']:5.2f}%  (reso)|")
+            else:
+                print(f"               |")
+
+
+        print("_"*WID)
+        if chi2dof>1: print(f"*... errors WERE scaled up  {np.sqrt(chi2dof):.1f}x     for chi2={chi2dof:.1f} !")
+        print("\n",form,"\n") # FORMULA
+        form1 = re.sub("x", f"{x[0]}", form)
+        form2 = re.sub("x", f"{x[-1]}", form)
+        print(   eval(form1) ,"=",form1)
+        print(   eval(form2) ,"=",form2)
+
+
 
 
 
 
     def model_chi20(x,   a):
-        f = np.polynomial.Chebyshev( [a] )(x-bin1)
+        f = a
         return f
     def model_chi21(x,   a,b):
-        f = np.polynomial.Chebyshev( [a,b] )(x-bin1)
+        f = a* x + b
         return f
     def model_chi22(x,   a,b,c):
-        f = np.polynomial.Chebyshev( [a,b,c] )(x-bin1)
+        f = a*x*x + b*x +c
         return f
     def model_chi23(x,   a,b,c,d):
-        f = np.polynomial.Chebyshev( [a,b,c,d] )(x-bin1)
+        f = a*x*x*x + b*x*x +c*x +d
         return f
     def model_chi24(x,   a,b,c,d,e):
-        f = np.polynomial.Chebyshev( [a,b,c,d,e] )(x-bin1)
+        f = a*x*x*x*x + b*x*x*x +c*x*x+d*x+e
         return f
     def model_chi25(x,   a,b,c,d,e,f):
-        f = np.polynomial.Chebyshev( [a,b,c,d,e,f] )(x-bin1)
+        f = a*x*x*x*x*x + b*x*x*x*x +c*x*x*x+d*x*x+e*x+f
         return f
 
 
-
     # ---- for histograms, use cx...
     print(".............iminuit.............>")
     c2 = cost.LeastSquares(x, y, dy, locals()["model_chi2"+str(polorder)] )
 
+
     if polorder==0:
 
         m2 = Minuit(c2,
                     a=y.mean()  )
     elif polorder==1:
 
         m2 = Minuit(c2,
@@ -110,34 +138,38 @@
                     a=0.1**5,b=0.1**4,c=0.1**3, d=0.1**2, e=0.1, f=y.mean() )
     else:
         print("X...  unknown polynomial order to me ")
         return None
 
 
 
+
     # m2.limits["a", "b", "c"] = (0, None)
 
     m2.migrad()       # DO MINIMIZATION <<<<<<<<<<
     #print(m2.errors) # error view
     #print(m2.values) # value view
 
     print(m2.fmin)   #NICE table
     print(m2.params) # NICE table
 
 
 
     # ------ create parameter list on the fly
-    params = [ chr(ord('a')+i) for i in  range(0,polorder+1)]
-    #print(params)
-    params =  [ m2.values[i] for i in params ]
-    #print(params)
+    paramnames = [ chr(ord('a')+i) for i in  range(0,polorder+1)]
+    #paramnames =  list("abce")
+    params =  [ m2.values[i] for i in paramnames ]
+
 
     yf = locals()["model_chi2"+str(polorder)]( x, *params )
 
 
+    xf10 = np.arange( x[0],x[-1], (x[-1]-x[0])/100 )
+    yf10 = locals()["model_chi2"+str(polorder)]( xf10, *params )
+
 
     chi2dof=m2.fval/(len(x) - m2.nfit)
     if False:
         print("   FCN =",m2.fval)
         print(" points=",len(x))
         print("   par = ",m2.nfit)
         print("  Chi2 = ", chi2dof)
@@ -145,10 +177,43 @@
 
     print()
     print(f"i... FIT IS valid ... {m2.valid} ")
     print(f" ... and accurate ... {m2.accurate}")
     #print(f" ... and all ok   ... {NOError}")
 
 
-    print(f"i... Chebyshev parameters are not real! they are for shifted X")
-    print("_________________________________________________")
-    return yf
+    if not(m2.valid):
+        print( f"{fg.red}X... ____________FIT SEEMS NOT  VALID___________ {fg.default}" )
+    elif  not(m2.accurate):
+        print( f"{fg.yellow}X... ____________VALID BUT NOT ACCURATE___________ {fg.default}" )
+    else:
+        print( f"{fg.green}i...    fit seems OK to me {fg.default}" )
+
+    res = {}
+    res['yf'] = yf
+    res['yf10'] = yf10
+    res['xf10'] = xf10
+
+    res['chi2dof'] = chi2dof
+
+    res['valid'] = m2.valid
+    res['accurate'] = m2.accurate
+
+    res['noerror'] = True
+    #------------ the last one is OR ALL
+    if not(m2.valid) or not(m2.accurate):
+        res['noerror'] = False
+
+    res['logx']       = False
+    res['logy']       = False
+
+
+    res['range']    = ( x[0], x[-1] )
+
+    for i in paramnames:
+        res[i] = m2.values[i]
+        res[f"d{i}"] = m2.errors[i]
+
+
+
+    print("_________________________________________________polall")
+    return res
```

### Comparing `pyfromroot-0.1.8/pyfromroot/pr_zoom.py` & `pyfromroot-0.2.1/pyfromroot/pr_zoom.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 
 
 
 def main( *args ):
     """
     I want to zoom:  object(histo) xlow,xhigh
     """
+    display = False # NO DISPLAY HERE
+    #display = True #  DISPLAY HERE
     if len(args)<1:
         print("X... no object name given  (and no model given too)")
         return
     if len(args)<2:
         print("X... no zoom limits  given")
         return
 
@@ -141,40 +143,43 @@
         calb =  g_orig.GetXaxis().GetXmax() - cala*g_orig.GetNbinsX()
         # x = cala*x + calb
 
 
 
     # ///////////////////////////////////////////////////// plotting results
 
-    cmain = ROOT.gPad.GetCanvas()  # reset all canvas
-    cmain.Clear()
+    #cmain = ROOT.gPad.GetCanvas()  # reset all canvas
+    #cmain.Clear()
+    #cmain = ROOT.gPad  # reset JUST THE PAD
+    #cmain.Clear()
     #cmain.Divide(1,1) # div canvas
     #cmain.cd(1)
 
     ####g_xy = ROOT.TGraph( len(x) , x.flatten("C"), yf.flatten("C") )
     x12 = args[1].split(",")
     x12 = [ float(x) for x in x12 ]
 
     if x12[1]<x12[0]:
         dx = x12[1]
         x =  x12[0]
         x12[0] = x-dx
         x12[1] = x+dx
 
-    print(f"i... zooming to ")
+    #print(f"i... zooming to ")
 
 
     g_orig.GetXaxis().SetRangeUser( x12[0] , x12[1]  )
     # zoom works on energies!
     # g_orig.GetXaxis().SetRangeUser( (x12[0] - calb)/cala, (x12[1] - calb)/cala )
 
-    g_orig.SetMarkerStyle(7) # small circle , no lines...
-    g_orig.Draw() # for histo NOT PAWL;  it works with NO PAWL TGraph too
-    ROOT.gPad.Modified()
-    ROOT.gPad.Update()
+    if display:
+        g_orig.SetMarkerStyle(7) # small circle , no lines...
+        g_orig.Draw() # for histo NOT PAWL;  it works with NO PAWL TGraph too
+        ROOT.gPad.Modified()
+        ROOT.gPad.Update()
 
 
 
     #-------------------------- I NEED to REGISTER all to be able to display on gPad
 
 #    prun.register(gf, "fit")
```

### Comparing `pyfromroot-0.1.8/pyfromroot/prj_utils.py` & `pyfromroot-0.2.1/pyfromroot/prj_utils.py`

 * *Files identical despite different names*

### Comparing `pyfromroot-0.1.8/pyfromroot/prun.py` & `pyfromroot-0.2.1/pyfromroot/prun.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,38 +15,42 @@
 def register(obj, NAME ):
     """
     For plotting on current canvas or access from CLING,
  each object has to be registered
     """
     #NAME = "fit"
     obj.SetName(NAME)
+
     # obj.SetTitle(NAME)
     oldg = ROOT.gROOT.GetListOfSpecials().FindObject(NAME)
     if oldg:
+        #print(f"i...    removing existing object {NAME}", end="\r"))
         ROOT.gROOT.GetListOfSpecials().Remove(oldg)
     ROOT.gROOT.GetListOfSpecials().Add(obj)
+    #print(f"i... object NAME={NAME} registered")
+    #ROOT.gROOT.GetListOfSpecials().ls()
     return
 
 
 
 #========================================== functions called from C++
 
 # ---------------------------------------------------------------
 def import_pr_input():
     """
     get the input from TText object and  eventual arguments
     """
     # 1/ get input
     lin = ROOT.gROOT.GetListOfSpecials().FindObject("pr_input")
-    # print(f"P... infput function found - see: {lin}")
 
     # for a case if called from python code
     if ROOT.addressof(lin)==0:
-        print("X... no TText present ... called from python?")
+        print("D... no TText present ... called from python")
         return None,None
+    print(f"P... input function found - see: {lin}", lin.Print() )
 
     inname = lin.GetName()
     intit = lin.GetTitle()
 
     # print(f"P...    title={intit},  name={inname} " )
     params = []
     if intit.find(" ")>0: # space means parameters follow
@@ -70,28 +74,33 @@
     tgt2 = os.path.dirname(os.path.abspath(__file__))
     os.chdir( tgt2 )
     files = glob.glob("pr_*.py")
     if len(files)==0:
         print("X... NO python FILES available (listpy)")
         return None
     # files = [x for x in files if x.find("pr_model_")!=0] # models- I exclude?
-    print(f"i... modules available in REPO:\n          {[ x.rstrip('.py').lstrip('pr_') for x in files]}")
+    #print("REPO:",tgt2) # I forgot to link inside the repo
+    #print("REPO",files)
+    corenames = [ os.path.splitext(x)[0].split("pr_")[1] for x in files]
+    #print(f"i... modules available in REPO:\n          {corenames}")
     files = [ tgt2+"/"+x for x in files ]
     #- GO back from repo
     os.chdir( dirnow )
 
     #print("D... looking current dir")
     filescur = glob.glob("pr_*.py")
     #print(f"i... curdir: {filescur}")
     if len(filescur)==0:
-        print("D... NO python FILES available in current directory (listpy)")
+        asdqwe541 = 1
+        #print("D... NO python FILES available in current directory (listpy)")
         # return None
         #files = filescur
     else:
-        print(f"i... modules available in CURR:\n          {[ x.rstrip('.py').lstrip('pr_') for x in filescur]}")
+        corenames = [ os.path.splitext(x)[0].split("pr_")[1] for x in filescur]
+        #print(f"i... modules available in CURR:\n          {corenames}")
         # files = [x for x in files if x.find("pr_model_")!=0] # models- I exclude?
         files =  files + filescur
 
 
 
 
 
@@ -102,30 +111,34 @@
 # ---------------------------------------------------------------
 def import_module(intit):
 
 
     files = listpy() # get all modules available
 
     if files is None:
-        print("X... no loadable modules found....(import_module)")
+        print("X... no loadable modules found....(@import_module)")
         return None
 
+    # print(files) # all present files
+    # print(intit) # module
     module = None
     for ffile in files:
         # ffile may be with a path....
         construct = ffile
         if len(ffile.split("/"))>1:
             construct = construct.split("/")[-1]
         construct =  construct.lstrip("pr_")
         # print(construct)
         construct =  construct.rstrip("py")[:-1] # prioblem w .py
         # print(construct)
-        #print(f" ...    searching  /{intit}/ in /{ffile}/ <={construct}")
+        ##print(f" ... searching /{intit}/ in /{ffile}/ <={construct}")
+        # this was the last searching
+        #print(f" ... searching /{intit}/ in {ffile} ")
 
-        if (intit== construct):
+        if (intit == construct):
             #print(f"P... got {ffile}")
             #print("i... trying to importlib:", item.GetTitle() )
             # UNimport module first - case there was an error there previously
             unloadname = f"pr_{intit}"
             print(f"i... module /{unloadname}/ ... ", end="")
             try:
                 sys.modules.pop( unloadname ) # ffile[:-3]     f"pr_{construct}")
@@ -148,31 +161,30 @@
 
     return module
 # ---------------------------------------------------------------
 # ---------------------------------------------------------------
 
 #================================================================== MAIN PART
 
-def loadpy( *args ):
+def loadpy( *args, **kwargs ):
     """
     import module - based on the TText object Title created in C++ earlier
     """
     #print("P... in fun listpy")
 
-
     intit, params = import_pr_input()
     #print(f" intit={intit}, params={params}")
 
     if intit is None:
         if len(args)!=2:
-            print("X... I think I am called from python, I need two arguments")
+            print("X... I think I am called from python, but I need two arguments")
             return
         intit = args[0]
         params = args[1].split()
-        print(f"fi... called from python, looking for module /{intit}/; params = /{params}/")
+        print(f"i...  module= /{intit}/; params = /{params}/")
 
 
     # files = listpy()
 
     # if files is None:
     #     print("X... no loadable modules found....(loadpy)")
     #     return
@@ -206,20 +218,63 @@
     #         module = importlib.util.module_from_spec(spec)
     #         spec.loader.exec_module(module)
 
     #         print("i... importing module DONE")
 
     module = import_module(intit)
     # AND run the modules' main()
-    if len(params)>0:
+    if len(params)>0 and len(kwargs)>0:
+        res = module.main( *params, **kwargs)
+    elif len(params)>0:
         res = module.main( *params)
     else:
         res = module.main()
 
 
 
     # print("i... leaving prun.py")
     return res # I cant do better with adding to Specials and gDirectory
     #======================================================================== END
 
     print(f"X... no file like pr_{intit}.py found (loadpy)")
     return
+
+
+
+
+
+
+#============================================ DO / PROCESS (same and better THAN LOADPY) ===
+def do( *args, **kwargs ):
+    """
+    import module - based on the TText object Title created in C++ earlier
+    """
+
+    print("D... args in /DO/", args)
+    intit, params = import_pr_input()  # when called from ROOT. None None when from python
+    print(f" intit={intit}, params={params}")
+
+    if intit is None: # from PYTHON
+        if len(args)!=2:
+            print("X... I think I am called from python, I need two arguments")
+            return
+        intit = args[0]
+        params = args[1].split()
+        print(f"fi... called from python, searching module /{intit}/; params = /{params}/")
+
+
+
+    module = import_module(intit)
+    # AND run the modules' main()
+    if len(params)>0:
+        res = module.main( *params, **kwargs)
+    else:
+        res = module.main()
+
+
+
+    print("i... leaving /DO/")
+    return res # I cant do better with adding to Specials and gDirectory
+    #======================================================================== END
+
+    print(f"X... no file like pr_{intit}.py found (loadpy)")
+    return
```

### Comparing `pyfromroot-0.1.8/pyfromroot/unitname.py` & `pyfromroot-0.2.1/pyfromroot/unitname.py`

 * *Files identical despite different names*

