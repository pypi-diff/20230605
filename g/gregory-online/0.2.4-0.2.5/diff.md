# Comparing `tmp/gregory_online-0.2.4.tar.gz` & `tmp/gregory_online-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gregory_online-0.2.4.tar", last modified: Fri Jun  2 15:19:40 2023, max compression
+gzip compressed data, was "gregory_online-0.2.5.tar", last modified: Mon Jun  5 09:03:56 2023, max compression
```

## Comparing `gregory_online-0.2.4.tar` & `gregory_online-0.2.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-02 15:19:40.124060 gregory_online-0.2.4/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1814 2023-06-02 15:19:40.124060 gregory_online-0.2.4/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1560 2023-06-02 15:19:34.000000 gregory_online-0.2.4/README.md
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-02 15:19:40.120060 gregory_online-0.2.4/bin/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    49972 2023-06-02 15:19:37.000000 gregory_online-0.2.4/bin/gregory_online
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-02 15:19:40.120060 gregory_online-0.2.4/gregory_online/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      261 2022-09-16 15:11:00.000000 gregory_online-0.2.4/gregory_online/__init__.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     6435 2023-03-17 17:33:40.000000 gregory_online-0.2.4/gregory_online/config.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    12282 2023-06-02 13:02:37.000000 gregory_online-0.2.4/gregory_online/fetchnp.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4527 2023-04-20 14:10:17.000000 gregory_online-0.2.4/gregory_online/histo_analyze.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3955 2023-03-17 17:33:40.000000 gregory_online-0.2.4/gregory_online/histo_displ.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      779 2023-03-17 17:33:40.000000 gregory_online-0.2.4/gregory_online/histo_global_cont.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    13381 2023-05-31 13:39:18.000000 gregory_online-0.2.4/gregory_online/histo_io.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4942 2023-03-17 17:33:40.000000 gregory_online-0.2.4/gregory_online/histo_np_ops.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     5961 2023-04-20 14:10:17.000000 gregory_online-0.2.4/gregory_online/key_enter.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2549 2023-04-20 14:10:17.000000 gregory_online-0.2.4/gregory_online/topbar.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        0 2022-09-16 15:11:00.000000 gregory_online-0.2.4/gregory_online/utilone.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2853 2023-06-02 14:03:44.000000 gregory_online-0.2.4/gregory_online/utils.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-06-02 15:19:39.000000 gregory_online-0.2.4/gregory_online/version.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-02 15:19:40.124060 gregory_online-0.2.4/gregory_online.egg-info/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1814 2023-06-02 15:19:40.000000 gregory_online-0.2.4/gregory_online.egg-info/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      589 2023-06-02 15:19:40.000000 gregory_online-0.2.4/gregory_online.egg-info/SOURCES.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-06-02 15:19:40.000000 gregory_online-0.2.4/gregory_online.egg-info/dependency_links.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       65 2023-06-02 15:19:40.000000 gregory_online-0.2.4/gregory_online.egg-info/requires.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       15 2023-06-02 15:19:40.000000 gregory_online-0.2.4/gregory_online.egg-info/top_level.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-06-02 15:19:40.124060 gregory_online-0.2.4/setup.cfg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1200 2023-06-01 12:16:03.000000 gregory_online-0.2.4/setup.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-05 09:03:56.009804 gregory_online-0.2.5/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     1775 2023-06-05 09:03:56.009804 gregory_online-0.2.5/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     1560 2023-06-02 15:20:26.000000 gregory_online-0.2.5/README.md
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-05 09:03:56.005804 gregory_online-0.2.5/bin/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    50146 2023-06-05 09:03:53.000000 gregory_online-0.2.5/bin/gregory_online
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-05 09:03:56.009804 gregory_online-0.2.5/gregory_online/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      261 2023-03-15 09:15:19.000000 gregory_online-0.2.5/gregory_online/__init__.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     6435 2023-03-15 09:15:19.000000 gregory_online-0.2.5/gregory_online/config.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    12513 2023-06-05 08:52:20.000000 gregory_online-0.2.5/gregory_online/fetchnp.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4527 2023-04-20 08:56:38.000000 gregory_online-0.2.5/gregory_online/histo_analyze.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3957 2023-06-02 15:34:38.000000 gregory_online-0.2.5/gregory_online/histo_displ.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      779 2023-03-16 17:25:56.000000 gregory_online-0.2.5/gregory_online/histo_global_cont.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    13381 2023-06-02 15:20:26.000000 gregory_online-0.2.5/gregory_online/histo_io.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4942 2023-03-17 14:35:05.000000 gregory_online-0.2.5/gregory_online/histo_np_ops.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     5961 2023-04-19 12:31:34.000000 gregory_online-0.2.5/gregory_online/key_enter.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2549 2023-04-19 12:17:44.000000 gregory_online-0.2.5/gregory_online/topbar.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        0 2023-03-15 09:15:19.000000 gregory_online-0.2.5/gregory_online/utilone.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2853 2023-06-02 15:20:26.000000 gregory_online-0.2.5/gregory_online/utils.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-06-05 09:03:55.000000 gregory_online-0.2.5/gregory_online/version.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-05 09:03:56.009804 gregory_online-0.2.5/gregory_online.egg-info/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     1775 2023-06-05 09:03:55.000000 gregory_online-0.2.5/gregory_online.egg-info/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      589 2023-06-05 09:03:55.000000 gregory_online-0.2.5/gregory_online.egg-info/SOURCES.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-06-05 09:03:55.000000 gregory_online-0.2.5/gregory_online.egg-info/dependency_links.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       65 2023-06-05 09:03:55.000000 gregory_online-0.2.5/gregory_online.egg-info/requires.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       15 2023-06-05 09:03:55.000000 gregory_online-0.2.5/gregory_online.egg-info/top_level.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-06-05 09:03:56.009804 gregory_online-0.2.5/setup.cfg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1200 2023-06-02 15:20:26.000000 gregory_online-0.2.5/setup.py
```

### Comparing `gregory_online-0.2.4/PKG-INFO` & `gregory_online-0.2.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: gregory_online
-Version: 0.2.4
+Version: 0.2.5
 Summary: Online watching HTTP server of ROOT on port 9009
-Home-page: UNKNOWN
 Author: me
 Author-email: jaromrax@gmail.com
 License: GPL2
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 Project gregory~online~
 =======================
 
 *experimental code to online survey root spectra from THTTPServer*
 
@@ -79,9 +77,7 @@
   mock~server~.py         
   rebin.py                
   setup.py                
   topbar.py               
   utilone.py              
   version.py              
   ----------------------- ------------------------------
-
-
```

### Comparing `gregory_online-0.2.4/README.md` & `gregory_online-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.4/bin/gregory_online` & `gregory_online-0.2.5/bin/gregory_online`

 * *Files 1% similar despite different names*

```diff
@@ -426,22 +426,24 @@
 
             #if ROOT.gDirectory.FindObject("backg"):
             #    fill_h_with_np(histograms["backg"],"backg")  # No livetime here
 
 
             INFLUX = True
             if INFLUX and len(h1np_diff)>2:
-                just_spesum = h1np_diff[1:-1].sum()
-                # print(just_spesum, h1np_diff)
+                # just_spesum = h1np_diff[1:-1].sum()
+                just_spesum = h1np_diff.sum()
+                # print("D... just_spesum==",just_spesum, h1np_diff, h1np)
                 deadt = 0
                 if  just_spesum !=0:
+                    # print("D... diff[0]==", h1np_diff[0], h1np_diff[1], len(h1np_diff) )
                     deadt = h1np_diff[0]/just_spesum*100
                 if is_float(rate) and is_float(deadt):
                     infvals = f"rate_{spectrumname}={rate:.1f},deadt_{spectrumname}={deadt:.1f}"
-                    #print(infvals)
+                    # print("D...",infvals)
                     influxwrite("test", f"greg",  infvals ) # hostname added automat
 
 
 
 
             # IN ANY CASE... REFRESH ALL CANVASES
             refresh_canvases()
```

### Comparing `gregory_online-0.2.4/gregory_online/config.py` & `gregory_online-0.2.5/gregory_online/config.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.4/gregory_online/fetchnp.py` & `gregory_online-0.2.5/gregory_online/fetchnp.py`

 * *Files 5% similar despite different names*

```diff
@@ -205,15 +205,15 @@
 
         self.xmin = jhis['fXaxis']['fXmin']
         self.xmax = jhis['fXaxis']['fXmax']
 
         #print( jhis.keys() )
         helem = jhis['fArray']
 
-        #print(len(helem) , helem[0], helem[-1] )
+        # print("D... helem in fetch: len,0,1 ...", len(helem) , helem[0], helem[-1] )
 
         self.h1np_prev = 1.0*self.h1np # save  previous
         self.h1np = np.array( helem )
 
         #---------protection in case of  reset
         if self.h1np.sum()< self.h1np_prev.sum():
             print(f"i... {fg.red}RESET? I CLEAN THE PREV. HISTOGRAM{fg.default}")
@@ -224,14 +224,18 @@
 
         if self.first_fetch:
             self.first_fetch = False
             self.h1np_diff = self.h1np*0
         else:
             self.h1np_diff = self.h1np - self.h1np_prev
 
+            # print("D... diff after substract", self.h1np_diff)
+            # print("D... h1np and prev@ substract",  self.h1np, self.h1np_prev)
+            # underflow should be retained
+
         #sum = 0
 
         #self.maximum = max(helem)
 
         #print(f"D... end fetch {sumnow-sumprev}  {sumnow}, {sumprev}")
         return True
 
@@ -288,18 +292,18 @@
             # ---------runtime, that is resistant to clear or no count
             #  HERE I PREPARE REALTIME AND RUNTIME (if no title info available)
             #   - this (together wth get_) can keep self.started  GOOD - TITLEvar works...
 
             if self.started is None:
                 if self.tcp_fetch_time is not None:
                     if self.realtime is not None: # set from TITLE rt=
-                        print(f"D... {fg.yellow}1st tuning of starttime from title realtime{fg.default}")
+                        # print(f"D... {fg.yellow}1st tuning of starttime from title realtime{fg.default}")
                         self.set_started_before( self.realtime + self.tcp_fetch_time/2)
                     else:
-                        print(f"D... {fg.yellow}1st tuning of starttime from runtime{fg.default}")
+                        # print(f"D... {fg.yellow}1st tuning of starttime from runtime{fg.default}")
                         self.set_started_before( self.runtime.total_seconds() + self.tcp_fetch_time/2 ) # guess
 
             if self.realtime is None: # do it from our time
                 if self.started is not None:
                     self.runtime = now - self.started
             else: # DO IT FROM TITLE -
                 self.runtime = dt.timedelta(seconds = self.realtime)
```

### Comparing `gregory_online-0.2.4/gregory_online/histo_analyze.py` & `gregory_online-0.2.5/gregory_online/histo_analyze.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.4/gregory_online/histo_displ.py` & `gregory_online-0.2.5/gregory_online/histo_displ.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
 
         # histograms[hname].SetMarkerStyle(7)
         # histograms[hname].SetLineColor(16)
         # histograms[hname].Draw("EX0")
 
     else:
         #print(f"X... {hname} is NOT there, we run ")
-        fill_h_with_np(h1np,hname, errors=errors, limits_calib=limits_calib, title=title)
+        fill_h_with_np(h1np,hname, errors=errors, limits_calib=limits_calib, title = hname)
         #histograms[hname].Draw("HEX0") # E0 bars, X0 no 0,
 
     histograms[hname].SetMarkerStyle(7)
     histograms[hname].SetLineColor(color)
     if filled:
         histograms[hname].SetFillStyle(3001)
         histograms[hname].SetFillColor(color)
```

### Comparing `gregory_online-0.2.4/gregory_online/histo_global_cont.py` & `gregory_online-0.2.5/gregory_online/histo_global_cont.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.4/gregory_online/histo_io.py` & `gregory_online-0.2.5/gregory_online/histo_io.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.4/gregory_online/histo_np_ops.py` & `gregory_online-0.2.5/gregory_online/histo_np_ops.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.4/gregory_online/key_enter.py` & `gregory_online-0.2.5/gregory_online/key_enter.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.4/gregory_online/topbar.py` & `gregory_online-0.2.5/gregory_online/topbar.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.4/gregory_online/utils.py` & `gregory_online-0.2.5/gregory_online/utils.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.4/gregory_online.egg-info/PKG-INFO` & `gregory_online-0.2.5/gregory_online.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: gregory-online
-Version: 0.2.4
+Version: 0.2.5
 Summary: Online watching HTTP server of ROOT on port 9009
-Home-page: UNKNOWN
 Author: me
 Author-email: jaromrax@gmail.com
 License: GPL2
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 Project gregory~online~
 =======================
 
 *experimental code to online survey root spectra from THTTPServer*
 
@@ -79,9 +77,7 @@
   mock~server~.py         
   rebin.py                
   setup.py                
   topbar.py               
   utilone.py              
   version.py              
   ----------------------- ------------------------------
-
-
```

### Comparing `gregory_online-0.2.4/gregory_online.egg-info/SOURCES.txt` & `gregory_online-0.2.5/gregory_online.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.4/setup.py` & `gregory_online-0.2.5/setup.py`

 * *Files identical despite different names*

