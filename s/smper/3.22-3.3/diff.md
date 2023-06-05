# Comparing `tmp/smper-3.22.tar.gz` & `tmp/smper-3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smper-3.22.tar", last modified: Sat Jun  3 14:33:40 2023, max compression
+gzip compressed data, was "smper-3.3.tar", last modified: Mon Jun  5 11:56:42 2023, max compression
```

## Comparing `smper-3.22.tar` & `smper-3.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-03 14:33:40.099843 smper-3.22/
--rw-r--r--   0 parlorsky   (501) staff       (20)      168 2023-06-03 14:33:40.099660 smper-3.22/PKG-INFO
--rw-r--r--   0 parlorsky   (501) staff       (20)       12 2023-01-19 23:10:33.000000 smper-3.22/README.md
--rw-r--r--   0 parlorsky   (501) staff       (20)       38 2023-06-03 14:33:40.099902 smper-3.22/setup.cfg
--rw-r--r--   0 parlorsky   (501) staff       (20)      421 2023-06-03 14:33:37.000000 smper-3.22/setup.py
-drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-03 14:33:40.097731 smper-3.22/src/
-drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-03 14:33:40.098488 smper-3.22/src/smper/
--rw-r--r--   0 parlorsky   (501) staff       (20)        0 2023-01-19 23:12:11.000000 smper-3.22/src/smper/__init__.py
--rw-r--r--   0 parlorsky   (501) staff       (20)     5986 2023-06-03 14:33:20.000000 smper-3.22/src/smper/smper.py
-drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-03 14:33:40.099453 smper-3.22/src/smper.egg-info/
--rw-r--r--   0 parlorsky   (501) staff       (20)      168 2023-06-03 14:33:40.000000 smper-3.22/src/smper.egg-info/PKG-INFO
--rw-r--r--   0 parlorsky   (501) staff       (20)      223 2023-06-03 14:33:40.000000 smper-3.22/src/smper.egg-info/SOURCES.txt
--rw-r--r--   0 parlorsky   (501) staff       (20)        1 2023-06-03 14:33:40.000000 smper-3.22/src/smper.egg-info/dependency_links.txt
--rw-r--r--   0 parlorsky   (501) staff       (20)        1 2023-01-22 20:56:54.000000 smper-3.22/src/smper.egg-info/not-zip-safe
--rw-r--r--   0 parlorsky   (501) staff       (20)        6 2023-06-03 14:33:40.000000 smper-3.22/src/smper.egg-info/top_level.txt
+drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-05 11:56:42.529217 smper-3.3/
+-rw-r--r--   0 parlorsky   (501) staff       (20)      167 2023-06-05 11:56:42.529028 smper-3.3/PKG-INFO
+-rw-r--r--   0 parlorsky   (501) staff       (20)       12 2023-01-19 23:10:33.000000 smper-3.3/README.md
+-rw-r--r--   0 parlorsky   (501) staff       (20)       38 2023-06-05 11:56:42.529287 smper-3.3/setup.cfg
+-rw-r--r--   0 parlorsky   (501) staff       (20)      420 2023-06-05 11:56:39.000000 smper-3.3/setup.py
+drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-05 11:56:42.527069 smper-3.3/src/
+drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-05 11:56:42.527895 smper-3.3/src/smper/
+-rw-r--r--   0 parlorsky   (501) staff       (20)        0 2023-01-19 23:12:11.000000 smper-3.3/src/smper/__init__.py
+-rw-r--r--   0 parlorsky   (501) staff       (20)     5971 2023-06-05 11:55:29.000000 smper-3.3/src/smper/smper.py
+drwxr-xr-x   0 parlorsky   (501) staff       (20)        0 2023-06-05 11:56:42.528805 smper-3.3/src/smper.egg-info/
+-rw-r--r--   0 parlorsky   (501) staff       (20)      167 2023-06-05 11:56:42.000000 smper-3.3/src/smper.egg-info/PKG-INFO
+-rw-r--r--   0 parlorsky   (501) staff       (20)      223 2023-06-05 11:56:42.000000 smper-3.3/src/smper.egg-info/SOURCES.txt
+-rw-r--r--   0 parlorsky   (501) staff       (20)        1 2023-06-05 11:56:42.000000 smper-3.3/src/smper.egg-info/dependency_links.txt
+-rw-r--r--   0 parlorsky   (501) staff       (20)        1 2023-01-22 20:56:54.000000 smper-3.3/src/smper.egg-info/not-zip-safe
+-rw-r--r--   0 parlorsky   (501) staff       (20)        6 2023-06-05 11:56:42.000000 smper-3.3/src/smper.egg-info/top_level.txt
```

### Comparing `smper-3.22/src/smper/smper.py` & `smper-3.3/src/smper/smper.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,124 +1,129 @@
 import os.path
 
 
 class rv:
     def discrete(number):
         sklad = {1:\
-"import numpy as np\n \
-from scipy.stats import * \n \
-from tqdm import tqdm\n \
-from sympy import *\n \
-import matplotlib.pyplot as plt\n \
-import itertools as it\n \
-from scipy import integrate\n \
-from scipy.special import *\n \
+"import numpy as np\n\
+from scipy.stats import *\n\
+from tqdm import tqdm\n\
+from sympy import *\n\
+import matplotlib.pyplot as plt\n\
+import itertools as it\n\
+from scipy import integrate\n\
+from scipy.special import *\n\
 import random",
                 2: "\
-a,b = 4,7\n \
-def f(x):\n \
-    if a <= x <= b:\n \
-        return ваша функция\n \
-    return 0\n \
-C = 1/integrate.quad(f,a,b)[0]\n \
-матожидание:\n \
-def f_C(x):\n \
-    if 4 <= x <= 7:\n \
-        return x*С*(ваша функция)\n \
-    return 0\n \
-Ex = integrate.quad(f_C,a,b)[0]  \n \
-def f_C_sq(x): \n \
-    if 4 <= x <= 7: \n \
-        return (x)**2 * C *(ваша функция)\n \
-    return 0\n \
-(integrate.quad(f_C_sq,a,b)[0] - Ex**2)**0.5\n \
-class distrbution(rv_continuous):\n \
-    def _pdf(self, x):\n \
-        return C * f(x)\n \
-d = distrbution()\n \
-quant = 0.8\n \
-d.ppf(quant)\n",
+a,b = 4,7\n\
+def f(x):\n\
+    if a <= x <= b:\n\
+        return ваша функция\n\
+    return 0\n\
+C = 1/integrate.quad(f,a,b)[0]\n\
+print(C)\n\
+#матожидание:\n\
+def f_C(x):\n\
+    if 4 <= x <= 7:\n\
+        return x*С*(ваша функция)\n\
+    return 0\n\
+Ex = integrate.quad(f_C,a,b)[0]\n\
+print(Ex)\n\
+def f_C_sq(x):\n\
+    if 4 <= x <= 7:\n\
+        return (x)**2 * C *(ваша функция)\n\
+    return 0\n\
+print((integrate.quad(f_C_sq,a,b)[0] - Ex**2)**0.5)\n\
+class distrbution(rv_continuous):\n\
+    def _pdf(self, x):\n\
+        return C * f(x)\n\
+d = distrbution()\n\
+quant = 0.8\n\
+print(d.ppf(quant))\n",
                 3:"\
-def Y(x):\n \
-    return функция\n \
-a,b = 4,8\n \
-dlin = b-a\n \
-def f(x):\n \
-    if a <= x <= b:\n \
-        return Y\n \
-    return 0\n \
-Ex = integrate.quad(f,a,b)[0] * 1/dlin\n \
-def f_s(x):\n \
-    if a <= x <= b:\n \
-        return (Y)**2\n \
-    return 0\n \
-std = (integrate.quad(f_s,a,b)[0] * 1/dlin - (Ex)**2)**0.5\n \
-асимметрия:\n \
-def f_sk(x):\n \
-    if a <= x <= b:\n \
-        return ((Y - Ex)/std)**3\n \
-    return 0\n \
-skew = integrate.quad(f_sk,a,b)[0] * 1/dlin\n \
-квантиль:\n \
-quant = 0.8\n \
-q = a + quant * dlin\n \
-Y(q)\n",
+def Y(x):\n\
+    return функция\n\
+a,b = 4,8\n\
+dlin = b-a\n\
+def f(x):\n\
+    if a <= x <= b:\n\
+        return Y\n\
+    return 0\n\
+Ex = integrate.quad(f,a,b)[0] * 1/dlin\n\
+print(Ex)\n\
+def f_s(x):\n\
+    if a <= x <= b:\n\
+        return (Y)**2\n\
+    return 0\n\
+std = (integrate.quad(f_s,a,b)[0] * 1/dlin - (Ex)**2)**0.5\n\
+print(std)\n\
+асимметрия:\n\
+def f_sk(x):\n\
+    if a <= x <= b:\n\
+        return ((Y - Ex)/std)**3\n\
+    return 0\n\
+skew = integrate.quad(f_sk,a,b)[0] * 1/dlin\n\
+print(skew)\n\
+квантиль:\n\
+quant = 0.8\n\
+q = a + quant * dlin\n\
+print(Y(q))\n",
                 4: "\
-from scipy.stats import multivariate_normal, norm\n \
-# для нормального (-7; 17; 81; 16; 0.6) найдите\n \
-# P((x - 4)(y - 3) < 0)\n \
-# ЗНАК МЕНЬШЕ\n \
-a = -7; b = 17; c = 81; d = 16; e = 0.6\n \
-mu = np.array([a, b])\n \
-Cov = np.array([[c, e * np.sqrt(c) * np.sqrt(d)], [e * np.sqrt(c) * np.sqrt(d), d]])\n \
-\n \
-W = multivariate_normal(mu, Cov)\n \
-X = norm(a, np.sqrt(c))\n \
-Y = norm(b, np.sqrt(d))\n \
-x = 4; y = 3\n \
+from scipy.stats import multivariate_normal, norm\n\
+# для нормального (-7; 17; 81; 16; 0.6) найдите\n\
+# P((x - 4)(y - 3) < 0)\n\
+# ЗНАК МЕНЬШЕ\n\
+a = -7; b = 17; c = 81; d = 16; e = 0.6\n\
+mu = np.array([a, b])\n\
+Cov = np.array([[c, e * np.sqrt(c) * np.sqrt(d)], [e * np.sqrt(c) * np.sqrt(d), d]])\n\
+\n\
+W = multivariate_normal(mu, Cov)\n\
+X = norm(a, np.sqrt(c))\n\
+Y = norm(b, np.sqrt(d))\n\
+x = 4; y = 3\n\
 print(X.cdf(x) - W.cdf([x, y]))\n",
                 
                 5: "\
-from scipy.stats import multivariate_normal, norm\n \
-# для нормального (-4; 4; 64; 81; -0.31) найдите\n \
-# P((x - 8)(x - 10)(y - 1) < 0)\n \
-# ЗНАК МЕНЬШЕ\n \
-a = -4; b = 4; c = 64; d = 81; e = -0.31\n \
-mu = np.array([a, b])\n \
-Cov = np.array([[c, e * np.sqrt(c) * np.sqrt(d)], [e * np.sqrt(c) * np.sqrt(d), d]])\n \
-W = multivariate_normal(mu, Cov)\n \
-X = norm(a, np.sqrt(c))\n \
-Y = norm(b, np.sqrt(d))\n \
-x1 = 8; x2 = 10; y = 1\n \
-Pa = W.cdf([x1, y])\n \
-Pb = X.cdf(x2) - X.cdf(x1) - (W.cdf([x2, y]) - W.cdf([x1, y]))\n \
-Pc = Y.cdf(y) - W.cdf([x2, y])\n \
+from scipy.stats import multivariate_normal, norm\n\
+# для нормального (-4; 4; 64; 81; -0.31) найдите\n\
+# P((x - 8)(x - 10)(y - 1) < 0)\n\
+# ЗНАК МЕНЬШЕ\n\
+a = -4; b = 4; c = 64; d = 81; e = -0.31\n\
+mu = np.array([a, b])\n\
+Cov = np.array([[c, e * np.sqrt(c) * np.sqrt(d)], [e * np.sqrt(c) * np.sqrt(d), d]])\n\
+W = multivariate_normal(mu, Cov)\n\
+X = norm(a, np.sqrt(c))\n\
+Y = norm(b, np.sqrt(d))\n\
+x1 = 8; x2 = 10; y = 1\n\
+Pa = W.cdf([x1, y])\n\
+Pb = X.cdf(x2) - X.cdf(x1) - (W.cdf([x2, y]) - W.cdf([x1, y]))\n\
+Pc = Y.cdf(y) - W.cdf([x2, y])\n\
 print(Pa + Pb + Pc)\n",
                 
                 6: "\
-from sympy import *\n \
-import numpy as np\n \
-init_printing()\n \
-from fractions import Fraction\n \
-def dr(x):\n \
-    return Fraction(x).limit_denominator()\n \
-# выражение 18 / pi * E**(-30*x**2 - 48*x*y + 8*x - 30*y**2 - 5*y - 85/24)\n \
-x, y = symbols('x y')\n \
-prim = 18 / pi * E**(-30*x**2 - 48*x*y + 8*x - 30*y**2 - 5*y - 85/24)\n \
-integ_y = simplify(integrate(prim, (x, -np.inf, np.inf)))\n \
-integ_x = simplify(integrate(prim, (y, -np.inf, np.inf)))\n \
-Ey = float(simplify(integrate(integ_y * y, (y, -np.inf, np.inf))))\n \
-Ex = float(simplify(integrate(integ_x * x, (x, -np.inf, np.inf))))\n \
-print(dr(Ex), dr(Ey))\n \
-Varx = float(simplify(integrate(x**2 *integ_x, (x, -np.inf, np.inf))) - Ex ** 2)\n \
-Vary = float(simplify(integrate(y ** 2 *integ_y, (y, -np.inf, np.inf))) - Ey ** 2)\n \
-print(dr(Varx), dr(Vary))\n \
-Cov = float(simplify(integrate(simplify(integrate((x - Ex) * (y - Ey) * prim, (x, -np.inf, np.inf))), (y, -np.inf, np.inf))))\n \
-print(dr(Cov))\n \
-p = Cov / (np.sqrt(Varx) * np.sqrt(Vary))\n \
+from sympy import *\n\
+import numpy as np\n\
+init_printing()\n\
+from fractions import Fraction\n\
+def dr(x):\n\
+    return Fraction(x).limit_denominator()\n\
+# выражение 18 / pi * E**(-30*x**2 - 48*x*y + 8*x - 30*y**2 - 5*y - 85/24)\n\
+x, y = symbols('x y')\n\
+prim = 18 / pi * E**(-30*x**2 - 48*x*y + 8*x - 30*y**2 - 5*y - 85/24)\n\
+integ_y = simplify(integrate(prim, (x, -np.inf, np.inf)))\n\
+integ_x = simplify(integrate(prim, (y, -np.inf, np.inf)))\n\
+Ey = float(simplify(integrate(integ_y * y, (y, -np.inf, np.inf))))\n\
+Ex = float(simplify(integrate(integ_x * x, (x, -np.inf, np.inf))))\n\
+print(dr(Ex), dr(Ey))\n\
+Varx = float(simplify(integrate(x**2 *integ_x, (x, -np.inf, np.inf))) - Ex ** 2)\n\
+Vary = float(simplify(integrate(y ** 2 *integ_y, (y, -np.inf, np.inf))) - Ey ** 2)\n\
+print(dr(Varx), dr(Vary))\n\
+Cov = float(simplify(integrate(simplify(integrate((x - Ex) * (y - Ey) * prim, (x, -np.inf, np.inf))), (y, -np.inf, np.inf))))\n\
+print(dr(Cov))\n\
+p = Cov / (np.sqrt(Varx) * np.sqrt(Vary))\n\
 print(dr(p))\n"}
         print(sklad[number])
     
     def cont(number):
         sklad = {1:'imports', 
                 2:"Абсолютно непрерывная случайная величина X\
 может принимать значения только в отрезке [5,10]\
```

