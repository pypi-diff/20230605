# Comparing `tmp/dgpsi-2.1b0.tar.gz` & `tmp/dgpsi-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dgpsi-2.1b0.tar", last modified: Thu Jul 28 00:09:34 2022, max compression
+gzip compressed data, was "dgpsi-2.2.0.tar", last modified: Mon Jun  5 00:37:53 2023, max compression
```

## Comparing `dgpsi-2.1b0.tar` & `dgpsi-2.2.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 00:09:34.241818 dgpsi-2.1b0/
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-07-28 00:09:24.000000 dgpsi-2.1b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4245 2022-07-28 00:09:34.241818 dgpsi-2.1b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3794 2022-07-28 00:09:24.000000 dgpsi-2.1b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 00:09:34.241818 dgpsi-2.1b0/dgpsi/
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-07-28 00:09:24.000000 dgpsi-2.1b0/dgpsi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12624 2022-07-28 00:09:24.000000 dgpsi-2.1b0/dgpsi/dgp.py
--rw-r--r--   0 runner    (1001) docker     (121)    17355 2022-07-28 00:09:24.000000 dgpsi-2.1b0/dgpsi/emulation.py
--rw-r--r--   0 runner    (1001) docker     (121)    16355 2022-07-28 00:09:24.000000 dgpsi-2.1b0/dgpsi/functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     4967 2022-07-28 00:09:24.000000 dgpsi-2.1b0/dgpsi/gp.py
--rw-r--r--   0 runner    (1001) docker     (121)     5168 2022-07-28 00:09:24.000000 dgpsi-2.1b0/dgpsi/imputation.py
--rw-r--r--   0 runner    (1001) docker     (121)    24965 2022-07-28 00:09:24.000000 dgpsi-2.1b0/dgpsi/kernel_class.py
--rw-r--r--   0 runner    (1001) docker     (121)     8469 2022-07-28 00:09:24.000000 dgpsi-2.1b0/dgpsi/likelihood_class.py
--rw-r--r--   0 runner    (1001) docker     (121)    25264 2022-07-28 00:09:24.000000 dgpsi-2.1b0/dgpsi/linkgp.py
--rw-r--r--   0 runner    (1001) docker     (121)     2072 2022-07-28 00:09:24.000000 dgpsi-2.1b0/dgpsi/synthetic.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-28 00:09:34.241818 dgpsi-2.1b0/dgpsi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4245 2022-07-28 00:09:34.000000 dgpsi-2.1b0/dgpsi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      354 2022-07-28 00:09:34.000000 dgpsi-2.1b0/dgpsi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-28 00:09:34.000000 dgpsi-2.1b0/dgpsi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      241 2022-07-28 00:09:34.000000 dgpsi-2.1b0/dgpsi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-07-28 00:09:34.000000 dgpsi-2.1b0/dgpsi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-28 00:09:34.241818 dgpsi-2.1b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1342 2022-07-28 00:09:24.000000 dgpsi-2.1b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:37:53.368122 dgpsi-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-05 00:37:43.000000 dgpsi-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-06-05 00:37:53.368122 dgpsi-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-06-05 00:37:43.000000 dgpsi-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:37:53.364122 dgpsi-2.2.0/dgpsi/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-05 00:37:43.000000 dgpsi-2.2.0/dgpsi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24853 2023-06-05 00:37:43.000000 dgpsi-2.2.0/dgpsi/dgp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38814 2023-06-05 00:37:43.000000 dgpsi-2.2.0/dgpsi/emulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19692 2023-06-05 00:37:43.000000 dgpsi-2.2.0/dgpsi/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12773 2023-06-05 00:37:43.000000 dgpsi-2.2.0/dgpsi/gp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-06-05 00:37:43.000000 dgpsi-2.2.0/dgpsi/imputation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31002 2023-06-05 00:37:43.000000 dgpsi-2.2.0/dgpsi/kernel_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9643 2023-06-05 00:37:43.000000 dgpsi-2.2.0/dgpsi/likelihood_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28996 2023-06-05 00:37:43.000000 dgpsi-2.2.0/dgpsi/linkgp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-05 00:37:43.000000 dgpsi-2.2.0/dgpsi/synthetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11086 2023-06-05 00:37:43.000000 dgpsi-2.2.0/dgpsi/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 00:37:53.368122 dgpsi-2.2.0/dgpsi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-06-05 00:37:53.000000 dgpsi-2.2.0/dgpsi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-05 00:37:53.000000 dgpsi-2.2.0/dgpsi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 00:37:53.000000 dgpsi-2.2.0/dgpsi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-05 00:37:53.000000 dgpsi-2.2.0/dgpsi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-05 00:37:53.000000 dgpsi-2.2.0/dgpsi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 00:37:53.368122 dgpsi-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-05 00:37:43.000000 dgpsi-2.2.0/setup.py
```

### Comparing `dgpsi-2.1b0/LICENSE` & `dgpsi-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dgpsi-2.1b0/dgpsi/functions.py` & `dgpsi-2.2.0/dgpsi/functions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,14 @@
 from numba import jit, vectorize, float64, prange, config
 import numpy as np
 from math import erf, exp, sqrt, pi
 from numpy.random import randn
+from scipy.linalg import pinvh
 import itertools
-from dill import dump, load
 config.THREADING_LAYER = 'workqueue'
-######Save and Load Emulators#######
-def write(emu, pkl_file):
-    """Save the constructed emulator to a pkl file.
-    
-    Args:
-        emu (class): an emulator class. For GP, it is the 'gp' class after training. 
-            For DGP, it is the 'emulator' class. For linked GP/DGP, it is the 'lgp' class.
-        pkl_file (strings): specifies the path to and the name of the pkl file to which
-            the emulator is saved.
-    """
-    dump(emu, open(pkl_file+".pkl","wb"))
-
-
-def read(pkl_file):
-    """Load the pkl file that stores the emulator.
-    
-    Args:
-        pkl_file (strings): specifies the path to and the name of the pkl file where
-            the emulator is stored.
-    
-    Returns:
-        class: an emulator class. For GP, it is the 'gp' class. For DGP, it is the 'emulator' class. 
-            For linked GP/DGP, it is the 'lgp' class.
-    """
-    emu = load(open(pkl_file+".pkl", "rb"))
-    return emu
-
 #######functions for optim#########
 @jit(nopython=True,cache=True)
 def pdist_matern_coef(X):
     n = X.shape[0]
     out_size = np.int((n * (n - 1)) / 2)
     dm = np.empty(out_size)
     k = 0
@@ -173,79 +146,231 @@
     const = np.pi**(-0.5*N)
     xn = np.array(list(itertools.product(*(x,)*N)))
     wn = np.prod(np.array(list(itertools.product(*(w,)*N))), 1)[:, None]
     fn = sqrt(2.0)*(np.sqrt(var[:,None])*xn) + mu[:,None]
     llik=fct(y[:,None],fn)
     return np.sum(np.exp(np.log((wn * const)[None,:]) + llik), axis=1)
 
+######Inverse Sweep for LOO######
+@jit(nopython=True,cache=True)
+def inv_swp(X,k):
+    T = np.empty_like(X)
+    n = len(X)
+    mask=np.ones(n,dtype=np.bool8)
+    mask[k]=False
+    d = -1/X[k,k]
+    #T[:,k] = X[:,k] * d
+    #T[k,:] = X[k,:] * d
+    for i in range(n):
+        for j in range(i+1):
+            if i!=k and j!=k:
+                temp = d * X[i,k] * X[k,j]
+                if i==j:
+                    T[i,j] = X[i,j] + temp
+                else:
+                    T[i,j] = X[i,j] + temp 
+                    T[j,i] = X[j,i] + temp
+    #T[k,k] = d
+    return T[:,mask][mask,:]
+
+######MICE smooth pred var calculation######
+def mice_var(x, x_extra, kernel, nugget_s):
+    """Calculate smoothed predictive variances of the GP using the candidate design set.
+    """
+    kernel.input=x[:,kernel.input_dim]
+    if kernel.connect is not None:
+        kernel.global_input=x_extra[:,kernel.connect]
+    kernel.nugget=max(nugget_s,kernel.nugget)
+    R=kernel.k_matrix()
+    Rinv=pinvh(R,check_finite=False)
+    sigma2 = (1/np.diag(Rinv)).reshape(-1,1)
+    sigma2 = kernel.scale*sigma2
+    return sigma2
+
 ######functions for predictions########
+@jit(nopython=True,cache=True)
+def Pmatrix(X):
+    N,D=np.shape(X)
+    P=np.empty((D,N,N))
+    for d in range(D):
+        for k in range(N):
+            for l in range(k+1):
+                temp = X[k,d]+X[l,d]
+                if k==l:
+                    P[d,k,l] = temp
+                else:
+                    P[d,k,l] = temp
+                    P[d,l,k] = temp
+    return P
+
+def cond_mean(x,z,w1,global_w1,Rinv_y,length,name):
+    """Make GP predictions.
+    """
+    if z is not None:
+        x=np.concatenate((x, z),1)
+        w1=np.concatenate((w1, global_w1),1)
+    r=k_one_vec(w1,x,length,name)
+    m=np.dot(Rinv_y, r)
+    return m
+
 #@jit(nopython=True,cache=True,fastmath=True)
 def gp(x,z,w1,global_w1,Rinv,Rinv_y,scale,length,nugget,name):
     """Make GP predictions.
     """
     if z is not None:
         x=np.concatenate((x, z),1)
         w1=np.concatenate((w1, global_w1),1)
     r=k_one_vec(w1,x,length,name)
     Rinv_r=np.dot(Rinv,r)
     r_Rinv_r=np.sum(r*Rinv_r,axis=0)
     v=np.abs(scale*(1+nugget-r_Rinv_r))
     #m=np.sum(r*Rinv_y,axis=0) 
-    m=(r.T@Rinv_y).flatten()
+    m=np.dot(Rinv_y, r)
     return m, v
 
 #@jit(nopython=True,cache=True,fastmath=True)
-def link_gp(m,v,z,w1,global_w1,Rinv,Rinv_y,scale,length,nugget,name,nb_parallel):
+def link_gp(m,v,z,w1,global_w1,Rinv,Rinv_y,R2sexp,Psexp,scale,length,nugget,name,nb_parallel):
     """Make linked GP predictions.
     """
+    if name=='sexp':
+        m_new, v_new = link_gp_sexp(m,v,z,w1,global_w1,Rinv,Rinv_y,R2sexp,Psexp,scale,length,nugget)
+    else:
+        M=len(m)
+        m_new=np.empty((M))
+        v_new=np.empty((M))
+        if z is not None:
+            Dw=np.shape(w1)[1]
+            Dz=np.shape(z)[1]
+            if len(length)==1:
+                length=length*np.ones(Dw+Dz)
+            Iz=k_one_vec(z,global_w1,length[-Dz::],'matern2.5')
+        else:
+            Dw=np.shape(w1)[1]
+            if len(length)==1:
+                length=length*np.ones(Dw)
+        for i in range(M):
+            mi=m[i]
+            vi=v[i]
+            if z is not None:
+                #zi=np.expand_dims(z[i,:],axis=0)
+                Izi=Iz[i]
+                if nb_parallel:
+                    I,J=IJ_parallel(w1,mi,vi,length[:-Dz])
+                else:
+                    I,J=IJ(w1,mi,vi,length[:-Dz])
+                #Iz_T=np.expand_dims(Iz.flatten(),axis=0)
+                Jzi=np.outer(Izi,Izi)
+                I,J=I*Izi,J*Jzi
+            else:
+                if nb_parallel:
+                    I,J=IJ_parallel(w1,mi,vi,length)
+                else:
+                    I,J=IJ(w1,mi,vi,length)
+            #tr_RinvJ=np.sum(Rinv*J)
+            tr_RinvJ=trace_sum(Rinv,J)
+            #IRinv_y=np.sum(I*Rinv_y)
+            IRinv_y=np.dot(I,Rinv_y)
+            m_new[i]=IRinv_y
+            #v_new[i]=np.abs(np.sum(np.sum(Rinv_y*J,axis=0)*Rinv_y.flatten())-IRinv_y**2+scale*(1+nugget-tr_RinvJ))
+            #v_new[i]=np.abs(Rinv_y.T@J@Rinv_y-IRinv_y**2+scale*(1+nugget-tr_RinvJ))
+            v_new[i]=np.abs(quad(J,Rinv_y)-IRinv_y**2+scale*(1+nugget-tr_RinvJ))
+    return m_new,v_new
+
+@jit(nopython=True,cache=True,fastmath=True)
+def link_gp_sexp(m,v,z,w1,global_w1,Rinv,Rinv_y,R2sexp,Psexp,scale,length,nugget):
+    """Make linked GP predictions for sexp kernels.
+    """
     M=len(m)
-    m_new=np.empty((M,1))
-    v_new=np.empty((M,1))
+    v_new=np.empty((M))
     if z is not None:
         Dw=np.shape(w1)[1]
         Dz=np.shape(z)[1]
         if len(length)==1:
             length=length*np.ones(Dw+Dz)
+        Iz=k_one_vec(z,global_w1,length[-Dz::],'sexp')
+        I=I_sexp(w1,m,v,length[:-Dz])
+        I*=Iz
     else:
         Dw=np.shape(w1)[1]
         if len(length)==1:
             length=length*np.ones(Dw)
+        I=I_sexp(w1,m,v,length)
+    IRinv_y=np.dot(I,Rinv_y)  
     for i in range(M):
-        mi=m[i,:]
-        vi=v[i,:]
+        mi=m[i]
+        vi=v[i]
         if z is not None:
-            zi=np.expand_dims(z[i,:],axis=0)
-            if nb_parallel:
-                I,J=IJ_parallel(w1,mi,vi,length[:-Dz],name)
-            else:
-                I,J=IJ(w1,mi,vi,length[:-Dz],name)
-            Iz=k_one_vec(global_w1,zi,length[-Dz::],name)
-            #Iz_T=np.expand_dims(Iz.flatten(),axis=0)
-            Jz=np.dot(Iz,Iz.T)
-            I,J=I*Iz,J*Jz
+            J=J_sexp(w1,mi,vi,length[:-Dz],Psexp,R2sexp)
+            Izi=Iz[i]
+            Jzi=np.outer(Izi,Izi)
+            J*=Jzi
         else:
-            I,J=IJ(w1,mi,vi,length,name)
-        tr_RinvJ=np.sum(Rinv*J)
-        #IRinv_y=np.sum(I*Rinv_y)
-        IRinv_y=I.T@Rinv_y
-        m_new[i]=IRinv_y
-        #v_new[i]=np.abs(np.sum(np.sum(Rinv_y*J,axis=0)*Rinv_y.flatten())-IRinv_y**2+scale*(1+nugget-tr_RinvJ))
-        v_new[i]=np.abs(Rinv_y.T@J@Rinv_y-IRinv_y**2+scale*(1+nugget-tr_RinvJ))
-    return m_new.flatten(),v_new.flatten()
+            J=J_sexp(w1,mi,vi,length,Psexp,R2sexp)
+        tr_RinvJ=trace_sum(Rinv,J)
+        v_new[i]=np.abs(quad(J,Rinv_y)-IRinv_y[i]**2+scale*(1+nugget-tr_RinvJ)).item()
+    return IRinv_y,v_new
+
+@jit(nopython=True,cache=True,fastmath=True)
+def I_sexp(X,z_m,z_v,length):
+    v_l=1/(1+2*z_v/length**2)
+    X_l=X/length
+    m_l=z_m/length
+    cross1=np.dot(X_l**2,v_l.T)
+    cross2=2*np.dot(X_l,(m_l*v_l).T)
+    L_z=np.sum(m_l**2*v_l,axis=1)
+    coef = 0.5*np.sum(np.log(v_l),axis=1)
+    dist=coef-cross1+cross2-L_z
+    I=np.exp(dist.T)
+    return I
+
+@jit(nopython=True,cache=True,fastmath=True)
+def J_sexp(X,z_m,z_v,length,Psexp,R2sexp):
+    X=X.T
+    d=len(X)
+    vli=z_v/length**2
+    mli=z_m/length
+    J=R2sexp.copy()
+    for i in range(d):
+        J*=1/np.sqrt(1+4*vli[i])*np.exp(-(Psexp[i]-2*mli[i])**2/(2+8*vli[i]))
+    return J
+
+@jit(nopython=True,cache=True,fastmath=True)
+def trace_sum(A,B):
+    n = len(A)
+    a = 0
+    for k in range(n):
+        for l in range(k+1):
+            if k==l:
+                a += A[k,l]*B[k,l]
+            else:
+                a += 2*A[k,l]*B[k,l]
+    return a
+
+@jit(nopython=True,cache=True,fastmath=True)
+def quad(A,B):
+    n = len(A)
+    a = 0
+    for k in range(n):
+        for l in range(k+1):
+            if k==l:
+                a += A[k,l]*B[k]**2
+            else:
+                a += 2*A[k,l]*B[l]*B[k]
+    return a
 
 @jit(nopython=True,cache=True,fastmath=True)
 def k_one_vec(X,z,length,name):
     """Compute cross-correlation matrix between the testing and training input data.
     """
     if name=='sexp':
         X_l=X/length
         z_l=z/length
         L_X=np.expand_dims(np.sum(X_l**2,axis=1),axis=1)
-        L_z=np.expand_dims(np.sum(z_l**2,axis=1,),axis=1)
-        dis2=L_X-2*np.dot(X_l,z_l.T)+L_z.T
+        L_z=np.sum(z_l**2,axis=1)
+        dis2=L_X-2*np.dot(X_l,z_l.T)+L_z
         k=np.exp(-dis2)
     elif name=='matern2.5':
         n=np.shape(X)[0]
         d=np.shape(X)[1]
         m=len(z)
         X_l=np.expand_dims((X/length).T,axis=2)
         z_l=np.expand_dims((z/length).T,axis=2)
@@ -256,59 +381,59 @@
             k1*=(1+sqrt(5)*dis+5/3*dis**2)
             k2+=dis
         k2=np.exp(-sqrt(5)*k2)
         k=k1*k2
     return k
 
 @jit(nopython=True,cache=True,parallel=True)
-def IJ_parallel(X,z_m,z_v,length,name):
+def IJ_parallel(X,z_m,z_v,length):
     """Compute I and J involved in linked GP predictions.
     """
     n = X.shape[0]
-    if name=='sexp':
-        X_z=X-z_m
-        I=np.ones((n,1))
-        J=np.ones((n,n))
-        for i in prange(n):
-            I[i]=I_sexp_parallel(z_v,length,X_z[i])
-            for j in range(i+1):
-                temp = J_sexp_parallel(z_v,length,X_z[i],X_z[j])
-                if i==j:
-                    J[i,j]=temp
-                else:
-                    J[i,j], J[j,i]=temp, temp
-    elif name=='matern2.5':
-        zX=z_m-X
-        muA, muB=zX-sqrt(5)*z_v/length, zX+sqrt(5)*z_v/length
-        I=np.ones((n,1))
-        J=np.ones((n,n))
-        for i in prange(n):
-            I[i]=I_matern_parallel(z_v,length,muA[i],muB[i],zX[i])
-            for j in range(i+1):
-                temp = J_matern_parallel(z_m, z_v, length, X[i], X[j], zX[i], zX[j])
-                if i==j:
-                    J[i,j]=temp
-                else:
-                    J[i,j], J[j,i]=temp, temp 
+#    if name=='sexp':
+#        X_z=X-z_m
+#        I=np.ones((n,1))
+#        J=np.ones((n,n))
+#        for i in prange(n):
+#            I[i]=I_sexp_parallel(z_v,length,X_z[i])
+#            for j in range(i+1):
+#                temp = J_sexp_parallel(z_v,length,X_z[i],X_z[j])
+#                if i==j:
+#                    J[i,j]=temp
+#                else:
+#                    J[i,j], J[j,i]=temp, temp
+#    elif name=='matern2.5':
+    zX=z_m-X
+    muA, muB=zX-sqrt(5)*z_v/length, zX+sqrt(5)*z_v/length
+    I=np.ones((n))
+    J=np.ones((n,n))
+    for i in prange(n):
+        I[i]=I_matern_parallel(z_v,length,muA[i],muB[i],zX[i])
+        for j in range(i+1):
+            temp = J_matern_parallel(z_m, z_v, length, X[i], X[j], zX[i], zX[j])
+            if i==j:
+                J[i,j]=temp
+            else:
+                J[i,j], J[j,i]=temp, temp 
     return I,J
 
-@jit(nopython=True,cache=True)
-def I_sexp_parallel(z_v,length,X_zi):
-    Id=1
-    for d in range(len(length)):
-        Id*=1/np.sqrt(1+2*z_v[d]/length[d]**2)*np.exp(-X_zi[d]**2/(2*z_v[d]+length[d]**2))
-    return Id
+#@jit(nopython=True,cache=True)
+#def I_sexp_parallel(z_v,length,X_zi):
+#    Id=1
+#    for d in range(len(length)):
+#        Id*=1/np.sqrt(1+2*z_v[d]/length[d]**2)*np.exp(-X_zi[d]**2/(2*z_v[d]+length[d]**2))
+#    return Id
 
-@jit(nopython=True,cache=True)
-def J_sexp_parallel(z_v,length,X_zi,X_zj):
-    Jd=1
-    for d in range(len(length)):
-        dis1, dis2 = (X_zi[d]+X_zj[d])**2, (X_zi[d]-X_zj[d])**2
-        Jd*=1/np.sqrt(1+4*z_v[d]/length[d]**2)*np.exp(-dis1/(2*length[d]**2+8*z_v[d])-dis2/(2*length[d]**2))
-    return Jd
+#@jit(nopython=True,cache=True)
+#def J_sexp_parallel(z_v,length,X_zi,X_zj):
+#    Jd=1
+#    for d in range(len(length)):
+#        dis1, dis2 = (X_zi[d]+X_zj[d])**2, (X_zi[d]-X_zj[d])**2
+#        Jd*=1/np.sqrt(1+4*z_v[d]/length[d]**2)*np.exp(-dis1/(2*length[d]**2+8*z_v[d])-dis2/(2*length[d]**2))
+#    return Jd
 
 @jit(nopython=True,cache=True)
 def I_matern_parallel(z_v,length,muA,muB,zXi):
     Id=1
     for d in range(len(length)):
         if z_v[d]!=0:
             Id*=np.exp((5*z_v[d]-2*sqrt(5)*length[d]*zXi[d])/(2*length[d]**2))* \
@@ -330,68 +455,68 @@
         else:
             Idi=(1+sqrt(5)*np.abs(zXi[d])/length[d]+5*zXi[d]**2/(3*length[d]**2))*np.exp(-sqrt(5)*np.abs(zXi[d])/length[d])
             Idj=(1+sqrt(5)*np.abs(zXj[d])/length[d]+5*zXj[d]**2/(3*length[d]**2))*np.exp(-sqrt(5)*np.abs(zXj[d])/length[d])
             J_d*=(Idi*Idj)
     return J_d
 
 @jit(nopython=True,cache=True,fastmath=True)
-def IJ(X,z_m,z_v,length,name):
+def IJ(X,z_m,z_v,length):
     """Compute I and J involved in linked GP predictions.
     """
     n,d=X.shape
-    if name=='sexp':
-        X_z=(X-z_m).T
-        I=np.ones((n))
-        J=np.ones((n,n))
-        for i in range(d):
-            I*=1/np.sqrt(1+2*z_v[i]/length[i]**2)*np.exp(-X_z[i]**2/(2*z_v[i]+length[i]**2))
+#    if name=='sexp':
+#        X_z=(X-z_m).T
+#        I=np.ones((n))
+#        J=np.ones((n,n))
+#        for i in range(d):
+#            I*=1/np.sqrt(1+2*z_v[i]/length[i]**2)*np.exp(-X_z[i]**2/(2*z_v[i]+length[i]**2))
+#            for k in range(n):
+#                for l in range(k+1):
+#                    temp = J_sexp(z_v[i],length[i],X_z[i,k],X_z[i,l])
+#                    if k==l:
+#                        J[k,l]*=temp
+#                    else:
+#                        J[k,l]*=temp
+#                        J[l,k]*=temp
+#        return I.reshape(-1,1),J
+#    elif name=='matern2.5':
+    zX=z_m-X
+    muA=(zX-sqrt(5)*z_v/length).T
+    muB=(zX+sqrt(5)*z_v/length).T
+    zX=zX.T
+    X=X.T
+    I=np.ones((n))
+    J=np.ones((n,n))
+    for i in range(d):    
+        if z_v[i]!=0:
+            I*=np.exp((5*z_v[i]-2*sqrt(5)*length[i]*zX[i])/(2*length[i]**2))* \
+                ((1+sqrt(5)*muA[i]/length[i]+5*(muA[i]**2+z_v[i])/(3*length[i]**2))*pnorm(muA[i]/sqrt(z_v[i]))+ \
+                (sqrt(5)+(5*muA[i])/(3*length[i]))*sqrt(0.5*z_v[i]/pi)/length[i]*np.exp(-0.5*muA[i]**2/z_v[i]))+ \
+                np.exp((5*z_v[i]+2*sqrt(5)*length[i]*zX[i])/(2*length[i]**2))* \
+                ((1-sqrt(5)*muB[i]/length[i]+5*(muB[i]**2+z_v[i])/(3*length[i]**2))*pnorm(-muB[i]/sqrt(z_v[i]))+ \
+                (sqrt(5)-(5*muB[i])/(3*length[i]))*sqrt(0.5*z_v[i]/pi)/length[i]*np.exp(-0.5*muB[i]**2/z_v[i]))
             for k in range(n):
                 for l in range(k+1):
-                    temp = J_sexp(z_v[i],length[i],X_z[i,k],X_z[i,l])
-                    if k==l:
-                        J[k,l]*=temp
+                    J_lk=Jd(X[i,l],X[i,k],z_m[i],z_v[i],length[i])
+                    if l==k:
+                        J[l,k]*=J_lk
                     else:
-                        J[k,l]*=temp
-                        J[l,k]*=temp
-        return I.reshape(-1,1),J
-    elif name=='matern2.5':
-        zX=z_m-X
-        muA=(zX-sqrt(5)*z_v/length).T.reshape((d,n,1))
-        muB=(zX+sqrt(5)*z_v/length).T.reshape((d,n,1))
-        zX=zX.T.reshape((d,n,1))
-        X=X.T.reshape((d,n,1))
-        I=np.ones((n,1))
-        J=np.ones((n,n))
-        for i in range(d):    
-            if z_v[i]!=0:
-                I*=np.exp((5*z_v[i]-2*sqrt(5)*length[i]*zX[i])/(2*length[i]**2))* \
-                    ((1+sqrt(5)*muA[i]/length[i]+5*(muA[i]**2+z_v[i])/(3*length[i]**2))*pnorm(muA[i]/sqrt(z_v[i]))+ \
-                    (sqrt(5)+(5*muA[i])/(3*length[i]))*sqrt(0.5*z_v[i]/pi)/length[i]*np.exp(-0.5*muA[i]**2/z_v[i]))+ \
-                   np.exp((5*z_v[i]+2*sqrt(5)*length[i]*zX[i])/(2*length[i]**2))* \
-                    ((1-sqrt(5)*muB[i]/length[i]+5*(muB[i]**2+z_v[i])/(3*length[i]**2))*pnorm(-muB[i]/sqrt(z_v[i]))+ \
-                    (sqrt(5)-(5*muB[i])/(3*length[i]))*sqrt(0.5*z_v[i]/pi)/length[i]*np.exp(-0.5*muB[i]**2/z_v[i]))
-                for k in range(n):
-                    for l in range(k+1):
-                        J_lk=Jd(X[i][l][0],X[i][k][0],z_m[i],z_v[i],length[i])
-                        if l==k:
-                            J[l,k]*=J_lk
-                        else:
-                            J[l,k]*=J_lk
-                            J[k,l]*=J_lk
-            else:
-                Id=(1+sqrt(5)*np.abs(zX[i])/length[i]+5*zX[i]**2/(3*length[i]**2))*np.exp(-sqrt(5)*np.abs(zX[i])/length[i])
-                I*=Id
-                J*=np.dot(Id,Id.T)
-        return I,J
+                        J[l,k]*=J_lk
+                        J[k,l]*=J_lk
+        else:
+            Id=(1+sqrt(5)*np.abs(zX[i])/length[i]+5*zX[i]**2/(3*length[i]**2))*np.exp(-sqrt(5)*np.abs(zX[i])/length[i])
+            I*=Id
+            J*=np.outer(Id,Id)
+    return I,J
 
-@jit(nopython=True,cache=True,fastmath=True)
-def J_sexp(z_v,length,X_zi,X_zj):
-    dis1, dis2 = (X_zi+X_zj)**2, (X_zi-X_zj)**2
-    Jd=1/sqrt(1+4*z_v/length**2)*exp(-dis1/(2*length**2+8*z_v)-dis2/(2*length**2))
-    return Jd
+#@jit(nopython=True,cache=True,fastmath=True)
+#def J_sexp(z_v,length,X_zi,X_zj):
+#    dis1, dis2 = (X_zi+X_zj)**2, (X_zi-X_zj)**2
+#    Jd=1/sqrt(1+4*z_v/length**2)*exp(-dis1/(2*length**2+8*z_v)-dis2/(2*length**2))
+#    return Jd
 
 @vectorize([float64(float64)],nopython=True,cache=True,fastmath=True)
 def pnorm(x):
     """Compute standard normal CDF.
     """
     return 0.5*(1+erf(x/sqrt(2)))
```

### Comparing `dgpsi-2.1b0/dgpsi/kernel_class.py` & `dgpsi-2.2.0/dgpsi/kernel_class.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,140 +1,167 @@
 import numpy as np
 from numpy.random import randn, uniform, standard_t
+from numpy.linalg import LinAlgError
 from math import sqrt, pi
 from scipy.optimize import minimize, Bounds
 from scipy.linalg import cho_solve, pinvh
 from scipy.spatial.distance import pdist, squareform
-from .functions import gp, link_gp, pdist_matern_one, pdist_matern_multi, pdist_matern_coef, fod_exp, Z_fct
+from .functions import Pmatrix, gp, link_gp, pdist_matern_one, pdist_matern_multi, pdist_matern_coef, fod_exp, Z_fct, inv_swp
 
 class kernel:
     """
     Class that defines the GPs in the DGP hierarchy.
 
-        Args:
-            length (ndarray): a numpy 1d-array, whose length equals to:
-                1. one if the lengthscales in the kernel function are assumed same across input dimensions;
+    Args:
+        length (ndarray): a numpy 1d-array, whose length equals to:
+
+                1. either one if the lengthscales in the kernel function are assumed same across input dimensions; or
                 2. the total number of input dimensions, which is the sum of the number of feeding GPs 
-                in the last layer (defined by the argument 'input_dim') and the number of connected global
-                input dimensions (defined by the argument 'connect'), if the lengthscales in the kernel function 
-                are assumed different across input dimensions.
-            scale (float, optional): the variance of a GP. Defaults to 1..
-            nugget (float, optional): the nugget term of a GP. Defaults to 1e-6.
-            name (str, optional): kernel function to be used. Either 'sexp' for squared exponential kernel or
-                'matern2.5' for Matern2.5 kernel. Defaults to 'sexp'.
-            prior_name (str, optional): prior class. Either gamma ('ga') or inverse gamma ('inv_ga') distribution for 
-                the lengthscales and nugget term. Set None to disable the prior. Defaults to 'ga'.
-            prior_coef (ndarray, optional): a numpy 1d-array that contains two values specifying the shape and rate 
-                parameters of gamma prior, shape and scale parameters of inverse gamma prior. Defaults to np.array([1.6,0.3]).
-            nugget_est (bool, optional): set to True to estimate nugget term or to False to fix the nugget term as specified
-                by the argument 'nugget'. If set to True, the value set to the argument 'nugget' is used as the initial
-                value. Defaults to False.
-            scale_est (bool, optional): set to True to estimate the variance or to False to fix the variance as specified
-                by the argument 'scale'. Defaults to False.
-            input_dim (ndarray, optional): a numpy 1d-array that contains the indices of GPs in the last layer
-                   whose outputs (or the indices of dimensions in the global input if the GP is in the first layer)
-                   feed into the GP. When set to None, all outputs from GPs of last layer (or all global input 
-                   dimensions) feed into the GP. Defaults to None.
-            connect (ndarray, optional): a numpy 1d-array that contains the indices of dimensions in the global
-                input connecting to the GP as additional input dimensions to the input obtained from the output of
-                GPs in the last layer (as determined by the argument 'input_dim'). When set to None, no global input
-                connection is implemented. Defaults to None. When the kernel class is used in GP/DGP emulators for linked
-                emulation and some input dimensions to the computer models are not connected to some feeding computer models, 
-                set 'connect' to a 1d-array of indices of these external global input dimensions, and accordingly, set 
-                'input_dim' to a 1d-array of indices of the remaining input dimensions that are connected to the feeding 
-                computer models.                   
-
-        Attributes:
-            type (str): identifies that the kernel is a GP.
-            g (function): a function giving the log probability density function of gamma or inverse gamma distribution 
-                ignoring the constant part.
-            gfod (function): a function giving the first order derivative of g with respect to the log-transformed 
-                lengthscales and nugget. 
-            para_path (ndarray): a numpy 2d-array that contains the trace of model parameters. Each row is a 
-                parameter estimate produced by one SEM iteration. The model parameters in each row are ordered as 
-                follow: np.array([scale estimate, lengthscale estimate (whose length>=1), nugget estimate]).
-            global_input (ndarray): a numpy 2d-array that contains the connect global input dimensions determined 
-                by the argument 'connect'. The value of the attribute is assigned during the initialisation of 
-                'dgp' class. If 'connect' is set to None, this attribute is also None. 
-            input (ndarray): a numpy 2d-array (each row as a data point and each column as a data dimension) that 
-                contains the input training data (according to the argument 'input_dim') to the GP. The value of 
-                this attribute is assigned during the initialisation of 'dgp' class. 
-            output (ndarray): a numpy 2d-array with only one column that contains the output training data to the GP.
-                The value of this attribute is assigned during the initialisation of 'dgp' class.
-            rep (ndarray): a numpy 1d-array used to re-construct repetitions in the data according to the repetitions 
-                in the global input, i.e., rep is assigned during the initialisation of 'dgp' class if one input position 
-                has multiple outputs. Otherwise, it is None. Defaults to None. 
-            Rinv (ndarray): a numpy 2d-array that stores the inversion of correlation matrix. Defaults to None.
-            Rinv_y (ndarray): a numpy 2d-array that stores the product of correlation matrix inverse and the output Y. Defaults to None.
-            rff (bool): indicates weather random Fourier features are used. Defaults to None.
-            D (int): the dimension of input data to the GP node. Defaults to None.
-            M (int): the number of features in random Fourier approximation. Defaults to None.
-            W (ndarray): a 2d-array (M, D) sampled to construct the Fourier approximation to the kernel matrix. Defaults to None.
-            b (ndarray): a 1d-array (D,) sampled to construct the Fourier approximation to the kernel matrix. Defaults to None.
-
-        Remarks:
-        For linked GP inference, when creating kernel classes for GP nodes in each layer, 
-            1. The 'connect' argument of the kernel class is set at its default None and not used because one needs 
-                to explicitly specify the external inputs to each GP using the Z argument of lgp class;
-            2. The 'global_input' attribute in the kernel class no longer contains dimensions of global input to the 
-                GPs in the first layer, as in DGP inference. Instead it contains external inputs 
-                provided in the Z argument;
-            3. The 'input_dim' argument in the kernel class needs to be specified explicitly by the user to let the 
-                inference know which GPs in the last layer are feeding GPs. We do not implement the default setting, like 
-                in the DGP case, that a GP is connected to all GPs in the last layers. Thus, one has to supply the 'input_dim' 
-                argument a full GP node index in the last layer of all GPs in the last layer are feeding the GP that the kernel
-                class represent. For example, if one is creating a GP that has its local input produced by all 4 GPs in the 
-                last layer, then one needs to assign np.arange(4) to the 'input_dim' argument explicitly.
-        """
+                   in the last layer (defined by the argument **input_dim**) and the number of connected global
+                   input dimensions (defined by the argument **connect**), if the lengthscales in the kernel function 
+                   are assumed different across input dimensions.
+        scale (float, optional): the variance of a GP. Defaults to `1`.
+        nugget (float, optional): the nugget term of a GP. Defaults to `1e-6`.
+        name (str, optional): kernel function to be used. Either `sexp` for squared exponential kernel or
+            `matern2.5` for Matern2.5 kernel. Defaults to `sexp`.
+        prior_name (str, optional): prior options for the lengthscales and nugget term. Either gamma (`ga`), inverse gamma (`inv_ga`) or the reference
+            prior (`ref`) for the lengthscales and nugget term. Set `None` to disable the prior. Defaults to `ga`.
+        prior_coef (ndarray, optional): if **prior_name** is either `ga` or `inv_ga`, it is a numpy 1d-array that contains two values specifying the shape 
+            and rate parameters of gamma prior, or shape and scale parameters of inverse gamma prior. If  **prior_name** is `ref`, it is a numpy 1d-array
+            that gives the value of the coefficient **a** in the reference prior. When set to `None`, it defaults to ``np.array([1.6,0.3])`` for gamma or 
+            inverse gamma priors. When set to the reference prior, it defaults to ``np.array([0.2])``. Defaults to `None`.
+        bds (ndarray, optional): a numpy 1d-array of length two that gives the lower and upper bounds of the lengthscales. Default to `None`.
+        nugget_est (bool, optional): set to `True` to estimate nugget term or to `False` to fix the nugget term as specified
+            by the argument **nugget**. If set to `True`, the value set to the argument **nugget** is used as the initial
+            value. Defaults to `False`.
+        scale_est (bool, optional): set to `True` to estimate the variance or to `False` to fix the variance as specified
+            by the argument **scale**. Defaults to `False`.
+        input_dim (ndarray, optional): a numpy 1d-array that contains either
+
+                1. the indices of GPs in the feeding layer whose outputs feed into the GP; or
+                2. the indices of dimensions in the global input if the GP is in the first layer. 
+            When set to `None`, 
+            
+                1. all outputs from GPs in the feeding layer; or 
+                2. all global input dimensions feed into the GP. 
+            Defaults to `None`.
+        connect (ndarray, optional): a numpy 1d-array that contains the indices of dimensions in the global
+            input connecting to the GP as additional input dimensions to the input obtained from the output of
+            GPs in the feeding layer (as determined by the argument **input_dim**). When set to `None`, no global input
+            connection is implemented. Defaults to `None`. When the kernel class is used in GP/DGP emulators for linked
+            emulation and some input dimensions to the computer models are not connected to some feeding computer models, 
+            set **connect** to a 1d-array of indices of these external global input dimensions, and accordingly, set 
+            **input_dim** to a 1d-array of indices of the remaining input dimensions that are connected to the feeding 
+            computer models.                   
+
+    Attributes:
+        type (str): identifies that the kernel is a GP.
+        g (function): a function giving the log probability density function of gamma or inverse gamma distribution 
+            ignoring the constant part.
+        gfod (function): a function giving the first order derivative of **g** with respect to the log-transformed 
+            lengthscales and nugget. 
+        para_path (ndarray): a numpy 2d-array that contains the trace of model parameters. Each row is a 
+            parameter estimate produced by one SEM iteration. The model parameters in each row are ordered as 
+            follow: ``np.array([scale estimate, lengthscale estimate (whose length>=1), nugget estimate])``.
+        global_input (ndarray): a numpy 2d-array that contains the connect global input dimensions determined 
+            by the argument **connect**. The value of the attribute is assigned during the initialisation of 
+            :class:`.dgp` class. If **connect** is set to `None`, this attribute is also `None`. 
+        input (ndarray): a numpy 2d-array (each row as a data point and each column as a data dimension) that 
+            contains the input training data (according to the argument **input_dim**) to the GP. The value of 
+            this attribute is assigned during the initialisation of :class:`.dgp` class. 
+        output (ndarray): a numpy 2d-array with only one column that contains the output training data to the GP.
+            The value of this attribute is assigned during the initialisation of :class:`.dgp` class.
+        rep (ndarray): a numpy 1d-array used to re-construct repetitions in the data according to the repetitions 
+            in the global input, i.e., rep is assigned during the initialisation of :class:`.dgp` class if one input position 
+            has multiple outputs. Otherwise, it is `None`. Defaults to `None`. 
+        Rinv (ndarray): a numpy 2d-array that stores the inversion of correlation matrix. Defaults to `None`.
+        Rinv_y (ndarray): a numpy 1d-array that stores the product of correlation matrix inverse and the output Y. Defaults to `None`.
+        rff (bool): indicates weather random Fourier features are used. Defaults to `None`.
+        D (int): the dimension of input data to the GP node. Defaults to `None`.
+        M (int): the number of features in random Fourier approximation. Defaults to `None`.
+        W (ndarray): a 2d-array (M, D) sampled to construct the Fourier approximation to the kernel matrix. Defaults to `None`.
+        b (ndarray): a 1d-array (D,) sampled to construct the Fourier approximation to the kernel matrix. Defaults to `None`.
+    """
 
-    def __init__(self, length, scale=1., nugget=1e-6, name='sexp', prior_name='ga', prior_coef=np.array([1.6,0.3]), nugget_est=False, scale_est=False, input_dim=None, connect=None):
+    def __init__(self, length, scale=1., nugget=1e-6, name='sexp', prior_name='ga', prior_coef=None, bds=None, nugget_est=False, scale_est=False, input_dim=None, connect=None):
         self.type='gp'
         self.length=length
         self.scale=np.atleast_1d(scale)
         self.nugget=np.atleast_1d(nugget)
         self.name=name
         self.prior_name=prior_name
-        self.prior_coef=prior_coef
         if self.prior_name=='ga':
+            if prior_coef is None:
+                self.prior_coef=np.array([1.6,0.3])
+            else:
+                self.prior_coef=prior_coef
             self.g=lambda x: (self.prior_coef[0]-1)*np.log(x)-self.prior_coef[1]*x
             self.gfod=lambda x: (self.prior_coef[0]-1)-self.prior_coef[1]*x
         elif self.prior_name=='inv_ga':
+            if prior_coef is None:
+                self.prior_coef=np.array([1.6,0.3])
+            else:
+                self.prior_coef=prior_coef
             self.g=lambda x: -(self.prior_coef[0]+1)*np.log(x)-self.prior_coef[1]/x
             self.gfod=lambda x: -(self.prior_coef[0]+1)+self.prior_coef[1]/x
+        elif self.prior_name=='ref':
+            if prior_coef is None:
+                self.prior_coef=np.array([0.2])
+            else:
+                self.prior_coef=prior_coef
+            self.cl=None
         self.nugget_est=nugget_est
         self.scale_est=scale_est
         self.input_dim=input_dim
         self.connect=connect
         self.para_path=np.atleast_2d(np.concatenate((self.scale,self.length,self.nugget)))
         self.global_input=None
         self.input=None
         self.output=None
         self.rep=None
         self.Rinv=None
         self.Rinv_y=None
+        self.R2sexp=None
+        self.Psexp=None
         self.rff=None
         self.D=None
         self.M=None
         self.W=None
         self.b=None
+        self.bds=bds
+
+    def compute_cl(self):
+        if len(self.length)==1:
+            if self.global_input is not None:
+                X=np.concatenate((self.input, self.global_input),1)
+            else:
+                X=self.input
+            dists = pdist(X, metric="euclidean")
+            self.cl=np.max(dists)/len(self.output)
+        else:
+            input_range = np.max(self.input,axis=0)-np.min(self.input,axis=0)
+            if self.global_input is not None:
+                g_input_range = np.max(self.global_input,axis=0)-np.min(self.global_input,axis=0)
+                input_range = np.concatenate((input_range, g_input_range))
+            self.cl=input_range/len(self.output)**(1/len(self.length))
 
     def sample_basis(self):
-        """Sample W and b to construct random Fourier approximations to correlation matrices.
+        """Sample **W** and **b** to construct random Fourier approximations to correlation matrices.
         """
         if self.name=='sexp':
             self.W=sqrt(2)*randn(self.M,self.D)
         elif self.name=='matern2.5':
             self.W=standard_t(5,size=(self.M,self.D))
         self.b=uniform(0,2*pi,size=self.M)
 
     def log_t(self):
         """Log transform the model parameters (lengthscales and nugget).
 
         Returns:
-            ndarray: a numpy 1d-array of log-transformed model paramters
+            ndarray: a numpy 1d-array of log-transformed model parameters
         """
         if self.nugget_est:
             log_theta=np.log(np.concatenate((self.length,self.nugget)))
         else:
             log_theta=np.log(self.length)
         return log_theta
 
@@ -154,32 +181,33 @@
             K=self.k_matrix()
             L=np.linalg.cholesky(K)
             YKinvY=(self.output).T@cho_solve((L, True), self.output, check_finite=False)
             new_scale=YKinvY/len(self.output)
             self.scale=new_scale.flatten()
             
     def k_matrix(self,fod_eval=False):
-        """Compute the correlation matrix and/or first order derivatives of the correlation matrix 
-            wrt log-transformed lengthscales and nugget.
+        """Compute the correlation matrix and/or first order derivatives of the correlation matrix wrt log-transformed lengthscales and nugget.
         
         Args:
             fod_eval (bool): indicates if the gradient information is also computed along with the correlation
-                matrix. Defaults to False. 
+                matrix. Defaults to `False`. 
 
         Returns:
-            K (ndarray): a numpy 2d-array as the correlation matrix.
-            fod (ndarray): a numpy 3d-array that contains the first order derivatives of the correlation matrix 
-                wrt log-transformed lengthscales and nugget. The length of the array equals to the total number 
-                of model parameters (i.e., the total number of lengthscales and nugget).
+            ndarray_or_tuple: 
+                1. If **fod_eval** = `False`, a numpy 2d-array *K* is returned as the correlation matrix.
+                2. If **fod_eval** = `True`, a tuple is returned. It includes *K* and fod, a numpy 3d-array that contains the first order derivatives of the correlation matrix 
+                   wrt log-transformed lengthscales and nugget. The length of the array equals to the total number 
+                   of model parameters (i.e., the total number of lengthscales and nugget).
         """
         n=len(self.input)
         if self.global_input is not None:
             X=np.concatenate((self.input, self.global_input),1)
         else:
             X=self.input
+        #with np.errstate(divide='ignore'):
         X_l=X/self.length
         if self.name=='sexp':
             dists = pdist(X_l, metric="sqeuclidean")
             K = squareform(np.exp(-dists))
             if fod_eval:
                 if len(self.length)==1:
                     fod=np.expand_dims(squareform(2*dists)*K,axis=0)
@@ -209,29 +237,42 @@
     
     def log_prior(self):
         """Compute the value of log priors specified to the lengthscales and nugget. 
 
         Returns:
             ndarray: a numpy 1d-array giving the sum of log priors of the lengthscales and nugget. 
         """
-        lp=np.sum(self.g(self.length),keepdims=True)
-        if self.nugget_est:
-            lp+=self.g(self.nugget)
+        if self.prior_name=='ref':
+            a, b=self.prior_coef[0], self.prior_coef[1]
+            t=np.sum(self.cl/self.length)+self.nugget
+            lp=a*np.log(t)-b*t
+        else:
+            lp=np.sum(self.g(self.length),keepdims=True)
+            if self.nugget_est:
+                lp+=self.g(self.nugget)
         return lp
 
     def log_prior_fod(self):
         """Compute the first order derivatives of log priors wrt the log-transformed lengthscales and nugget.
 
         Returns:
             ndarray: a numpy 1d-array (whose length equal to the total number of lengthscales and nugget)
-                giving the first order derivatives of log priors wrt the log-transformed lengthscales and nugget.
+            giving the first order derivatives of log priors wrt the log-transformed lengthscales and nugget.
         """
-        fod=self.gfod(self.length)
-        if self.nugget_est:
-            fod=np.concatenate((fod,self.gfod(self.nugget)))
+        if self.prior_name=='ref':
+            a, b=self.prior_coef[0], self.prior_coef[1]
+            t=np.sum(self.cl/self.length)+self.nugget
+            fod=(b-a/t)*self.cl/self.length
+            if self.nugget_est:
+                fod_nugget=(a/t-b)*self.nugget
+                fod=np.concatenate((fod,fod_nugget))
+        else:  
+            fod=self.gfod(self.length)
+            if self.nugget_est:
+                fod=np.concatenate((fod,self.gfod(self.nugget)))
         return fod
 
     def llik(self,x):
         """Compute the negative log-likelihood function of the GP.
 
         Args:
             x (ndarray): a numpy 1d-array that contains the values of log-transformed model parameters: 
@@ -248,15 +289,15 @@
         YKinvY=(self.output).T@cho_solve((L, True), self.output, check_finite=False)
         if self.scale_est:
             scale=YKinvY/n
             neg_llik=0.5*(logdet+n*np.log(scale))
         else:
             neg_llik=0.5*(logdet+YKinvY/self.scale) 
         neg_llik=neg_llik.flatten()
-        if self.prior_name!=None:
+        if self.prior_name is not None:
             neg_llik=neg_llik-self.log_prior()
         return neg_llik
     
     def llik_rff(self,x):
         """Compute the negative log-likelihood function of the GP under RFF.
 
         Args:
@@ -280,29 +321,29 @@
         quad=np.dot(self.output.T,self.output)-np.sum(Zt_y*cho_solve((L, True), Zt_y, check_finite=False))
         if self.scale_est:
             scale=quad/(n*self.nugget)
             neg_llik=0.5*(logdet+n*np.log(scale)+(n-self.M)*np.log(self.nugget))
         else:
             neg_llik=0.5*(logdet+quad/(self.scale*self.nugget)+(n-self.M)*np.log(self.nugget)) 
         neg_llik=neg_llik.flatten()
-        if self.prior_name!=None:
+        if self.prior_name is not None:
             neg_llik=neg_llik-self.log_prior()
         return neg_llik
 
     def llik_der(self,x):
         """Compute first order derivatives of the negative log-likelihood function wrt log-transformed model parameters.
 
         Args:
             x (ndarray): a numpy 1d-array that contains the values of log-transformed model parameters: 
                 log-transformed lengthscales followed by the log-transformed nugget.
 
         Returns:
             ndarray: a numpy 1d-array (whose length equal to the total number of lengthscales and nugget)
-                that contains first order derivatives of the negative log-likelihood function wrt log-transformed 
-                lengthscales and nugget.
+            that contains first order derivatives of the negative log-likelihood function wrt log-transformed 
+            lengthscales and nugget.
         """
         self.update(x)
         n=len(self.output)
         K,Kt=self.k_matrix(fod_eval=True)
         KinvKt=np.linalg.solve(K,Kt)
         tr_KinvKt=np.trace(KinvKt,axis1=1, axis2=2)
         L=np.linalg.cholesky(K)
@@ -312,24 +353,27 @@
         P2=0.5*YKinvKtKinvY
         if self.scale_est:
             YKinvY=(self.output).T@KinvY
             scale=(YKinvY/n).flatten()
             neg_St=-P1-P2/scale
         else:
             neg_St=-P1-P2/self.scale
-        if self.prior_name!=None:
+        if self.prior_name is not None:
             neg_St=neg_St-self.log_prior_fod()
         return neg_St
 
     def log_likelihood_func(self):
         cov=self.scale*self.k_matrix()
         L=np.linalg.cholesky(cov)
         logdet=2*np.sum(np.log(np.abs(np.diag(L))))
         quad=(self.output).T@cho_solve((L, True), self.output, check_finite=False)
         llik=-0.5*(logdet+quad)
+        if self.prior_name=='ref':
+            self.compute_cl()
+            llik+=self.log_prior()
         return llik
 
     def log_likelihood_func_rff(self):
         """Compute Gaussian log-likelihood function using random Fourier features (RFF).
         """
         if self.connect is not None:
             X=np.concatenate((self.input,self.global_input),1)
@@ -339,134 +383,222 @@
         cov=np.dot(Z.T,Z)+self.nugget*np.identity(self.M)
         L=np.linalg.cholesky(cov)
         logdet=2*np.sum(np.log(np.abs(np.diag(L))))
         Zt_y=np.dot(Z.T,self.output)
         quad=-np.sum(Zt_y*cho_solve((L, True), Zt_y, check_finite=False))/(self.scale*self.nugget)
         #quad=-(Zt_y.T@cho_solve((L, True), Zt_y, check_finite=False))/(self.scale*self.nugget)
         llik=-0.5*(logdet+quad)
+        if self.prior_name=='ref':
+            self.compute_cl()
+            llik+=self.log_prior()
         return llik
 
     def maximise(self, method='L-BFGS-B'):
         """Optimise and update model parameters by minimising the negative log-likelihood function.
 
         Args:
-            method (str, optional): optimisation algorithm. Defaults to 'L-BFGS-B'.
+            method (str, optional): optimisation algorithm. Defaults to `L-BFGS-B`.
         """
         initial_theta_trans=self.log_t()
         if self.nugget_est:
             if self.rff:
-                lb=np.concatenate((-5.*np.ones(len(initial_theta_trans)-1),np.log([1e-8])))
-                ub=5.*np.ones(len(initial_theta_trans))
+                if self.bds is None:
+                    lb=np.concatenate((-5.*np.ones(len(initial_theta_trans)-1),np.log([1e-8])))
+                    ub=5.*np.ones(len(initial_theta_trans))
+                else:
+                    with np.errstate(divide='ignore'):
+                        lb=np.concatenate((np.log(self.bds[0])*np.ones(len(initial_theta_trans)-1),np.log([1e-8])))
+                    ub=np.concatenate((np.log(self.bds[1])*np.ones(len(initial_theta_trans)-1),5.))
                 bd=Bounds(lb, ub)
-                _ = minimize(self.llik_rff, initial_theta_trans, method=method, bounds=bd, options={'maxiter': 100, 'maxfun': 125})
+                _ = minimize(self.llik_rff, initial_theta_trans, method=method, bounds=bd, options={'maxiter': 100, 'maxfun': np.max((30,20+5*self.D))})
             else:
-                lb=np.concatenate((-np.inf*np.ones(len(initial_theta_trans)-1),np.log([1e-8])))
-                ub=np.inf*np.ones(len(initial_theta_trans))
+                if self.bds is None:
+                    lb=np.concatenate((-np.inf*np.ones(len(initial_theta_trans)-1),np.log([1e-8])))
+                    if self.prior_name=='ref':
+                        ub=np.concatenate((13.*np.ones(len(initial_theta_trans)-1), [np.inf]))
+                    else:
+                        ub=np.inf*np.ones(len(initial_theta_trans))
+                else:
+                    with np.errstate(divide='ignore'):
+                        lb=np.concatenate((np.log(self.bds[0])*np.ones(len(initial_theta_trans)-1),np.log([1e-8])))
+                    ub=np.concatenate((np.log(self.bds[1])*np.ones(len(initial_theta_trans)-1),[np.inf]))
                 bd=Bounds(lb, ub)
-                _ = minimize(self.llik, initial_theta_trans, method=method, jac=self.llik_der, bounds=bd, options={'maxiter': 100, 'maxfun': 125})
+                _ = minimize(self.llik, initial_theta_trans, method=method, jac=self.llik_der, bounds=bd, options={'maxiter': 100, 'maxfun': np.max((30,20+5*self.D))})
         else:
             if self.rff:
-                lb=-5.*np.ones(len(initial_theta_trans))
-                ub=5.*np.ones(len(initial_theta_trans))
+                if self.bds is None:
+                    lb=-5.*np.ones(len(initial_theta_trans))
+                    ub=5.*np.ones(len(initial_theta_trans))
+                else:
+                    with np.errstate(divide='ignore'):
+                        lb=np.log(self.bds[0])*np.ones(len(initial_theta_trans))
+                    ub=np.log(self.bds[1])*np.ones(len(initial_theta_trans))
                 bd=Bounds(lb, ub)
-                _ = minimize(self.llik_rff, initial_theta_trans, method=method, bounds=bd, options={'maxiter': 100, 'maxfun': 125})
+                _ = minimize(self.llik_rff, initial_theta_trans, method=method, bounds=bd, options={'maxiter': 100, 'maxfun': np.max((30,20+5*self.D))})
             else:
-                _ = minimize(self.llik, initial_theta_trans, method=method, jac=self.llik_der, options={'maxiter': 100, 'maxfun': 125})
+                if self.bds is None:
+                    if self.prior_name=='ref':
+                        lb=-np.inf*np.ones(len(initial_theta_trans))
+                        ub=13.*np.ones(len(initial_theta_trans))
+                        bd=Bounds(lb, ub)
+                        _ = minimize(self.llik, initial_theta_trans, method=method, jac=self.llik_der, bounds=bd, options={'maxiter': 100, 'maxfun': np.max((30,20+5*self.D))})
+                    else:
+                        _ = minimize(self.llik, initial_theta_trans, method=method, jac=self.llik_der, options={'maxiter': 100, 'maxfun': np.max((30,20+5*self.D))})
+                else:
+                    with np.errstate(divide='ignore'):
+                        lb=np.log(self.bds[0])*np.ones(len(initial_theta_trans))
+                    ub=np.log(self.bds[1])*np.ones(len(initial_theta_trans))
+                    bd=Bounds(lb, ub)
+                    _ = minimize(self.llik, initial_theta_trans, method=method, jac=self.llik_der, bounds=bd, options={'maxiter': 100, 'maxfun': np.max((30,20+5*self.D))})
         self.add_to_path()
         
     def add_to_path(self):
-        """Add updated model parameter estimates to the class attribute 'para_path'.
+        """Add updated model parameter estimates to the class attribute **para_path**.
         """
         para=np.concatenate((self.scale,self.length,self.nugget))
         self.para_path=np.vstack((self.para_path,para))
 
     def gp_prediction(self,x,z):
         """Make GP predictions. 
 
         Args:
             x (ndarray): a numpy 2d-array that contains the input testing data (whose rows correspond to testing
                 data points and columns correspond to testing data dimensions) with the number of columns same as 
-                the 'input' attribute.
+                the **input** attribute.
             z (ndarray): a numpy 2d-array that contains additional input testing data (with the same number of 
-                columns of the 'global_input' attribute) from the global testing input if the argument 'connect' 
-                is not None. Set to None if the argument 'connect' is None. 
+                columns of the **global_input** attribute) from the global testing input if the argument **connect** 
+                is not `None`. Set to None if the argument **connect** is `None`. 
 
         Returns:
             tuple: a tuple of two 1d-arrays giving the means and variances at the testing input data positions. 
         """
         m,v=gp(x,z,self.input,self.global_input,self.Rinv,self.Rinv_y,self.scale,self.length,self.nugget,self.name)
         return m,v
 
     def linkgp_prediction(self,m,v,z,nb_parallel):
         """Make linked GP predictions. 
 
         Args:
             m (ndarray): a numpy 2d-array that contains predictive means of testing outputs from the GPs in the last 
                 layer. The number of rows equals to the number of testing positions and the number of columns equals to the 
-                length of the argument 'input_dim'. If the argument 'input_dim' is None, then the number of columns equals 
+                length of the argument **input_dim**. If the argument **input_dim** is `None`, then the number of columns equals 
                 to the number of GPs in the last layer.
             v (ndarray): a numpy 2d-array that contains predictive variances of testing outputs from the GPs in the last 
-                layer. It has the same shape of 'm'.
+                layer. It has the same shape of **m**.
             z (ndarray): a numpy 2d-array that contains additional input testing data (with the same number of 
-                columns of the 'global_input' attribute) from the global testing input if the argument 'connect' 
-                is not None. Set to None if the argument 'connect' is None. 
-            nb_parallel (bool): whether to use Numba's multi-threading to accelerate the predictions.
+                columns of the **global_input** attribute) from the global testing input if the argument **connect** 
+                is not `None`. Set to `None` if the argument **connect** is `None`. 
+            nb_parallel (bool): whether to use *Numba*'s multi-threading to accelerate the predictions.
 
         Returns:
             tuple: a tuple of two 1d-arrays giving the means and variances at the testing input data positions (that are 
-                represented by predictive means and variances).
+            represented by predictive means and variances).
         """
-        m,v=link_gp(m,v,z,self.input,self.global_input,self.Rinv,self.Rinv_y,self.scale,self.length,self.nugget,self.name,nb_parallel)
+        m,v=link_gp(m,v,z,self.input,self.global_input,self.Rinv,self.Rinv_y,self.R2sexp,self.Psexp,self.scale,self.length,self.nugget,self.name,nb_parallel)
         return m,v
 
     def linkgp_prediction_full(self,m,v,m_z,v_z,z,nb_parallel):
         """Make linked GP predictions with additional input also generated by GPs/DGPs. 
 
         Args:
             m (ndarray): a numpy 2d-array that contains predictive means of testing outputs from the GPs in the last 
                 layer. The number of rows equals to the number of testing positions and the number of columns equals to the 
-                length of the argument 'input_dim'. If the argument 'input_dim' is None, then the number of columns equals 
+                length of the argument **input_dim**. If the argument **input_dim** is `None`, then the number of columns equals 
                 to the number of GPs in the last layer.
             v (ndarray): a numpy 2d-array that contains predictive variances of testing outputs from the GPs in the last 
-                layer. It has the same shape of 'm'.
+                layer. It has the same shape of **m**.
             m_z (ndarray): a numpy 2d-array that contains predictive means of additional input testing data from GPs.
             v_z (ndarray): a numpy 2d-array that contains predictive variances of additional input testing data from GPs.
             z (ndarray): a numpy 2d-array that contains additional input testing data from the global testing input that are
-                not from GPs. Set to None if the argument 'connect' is None. 
-            nb_parallel (bool): whether to use Numba's multi-threading to accelerate the predictions.
+                not from GPs. Set to `None` if the argument **connect** is None. 
+            nb_parallel (bool): whether to use *Numba*'s multi-threading to accelerate the predictions.
 
         Returns:
             tuple: a tuple of two 1d-arrays giving the means and variances at the testing input data positions (that are 
-                represented by predictive means and variances).
+            represented by predictive means and variances).
         """
         m=np.concatenate((m,m_z),axis=1)
         v=np.concatenate((v,v_z),axis=1)
         idx1=np.arange(np.shape(m_z)[1])
         idx2=np.arange(np.shape(m_z)[1],np.shape(self.global_input)[1])
         overall_input=np.concatenate((self.input,self.global_input[:,idx1]),axis=1)
-        m,v=link_gp(m,v,z,overall_input,self.global_input[:,idx2],self.Rinv,self.Rinv_y,self.scale,self.length,self.nugget,self.name,nb_parallel)
+        if self.name=='sexp':
+            if len(self.length)==1:
+                global_input_l=self.global_input[:,idx1]/self.length
+            else:
+                D=np.shape(self.input)[1]
+                global_input_l=self.global_input[:,idx1]/(self.length[D::][idx1])
+            dists = pdist(global_input_l, metric="sqeuclidean")
+            R2sexp_global = squareform(np.exp(-dists/2))
+            np.fill_diagonal(R2sexp_global, 1)
+            R2sexp = self.R2sexp*R2sexp_global
+            Psexp_global = Pmatrix(global_input_l)
+            Psexp = np.concatenate((self.Psexp,Psexp_global),axis=0)
+        else:
+            R2sexp, Psexp = self.R2sexp, self.Psexp
+        m,v=link_gp(m,v,z,overall_input,self.global_input[:,idx2],self.Rinv,self.Rinv_y,R2sexp,Psexp,self.scale,self.length,self.nugget,self.name,nb_parallel)
         return m,v
 
     def compute_stats(self):
         """Compute and store key statistics for the GP predictions
         """
         R=self.k_matrix()
         #U, s, Vh = np.linalg.svd(R)
         #self.Rinv=Vh.T@np.diag(s**-1)@U.T
         #L=np.linalg.cholesky(R)
         #self.Rinv_y=cho_solve((L, True), self.output, check_finite=False)
-        self.Rinv=pinvh(R,check_finite=False)
-        self.Rinv_y=np.dot(self.Rinv,self.output)
+        #self.Rinv=pinvh(R,check_finite=False)
+        #self.Rinv_y=np.dot(self.Rinv,self.output).flatten()
+        try:
+            L=np.linalg.cholesky(R)
+            self.Rinv=cho_solve((L, True), np.eye(len(R)), check_finite=False)
+            self.Rinv_y=cho_solve((L, True), self.output, check_finite=False).flatten()
+        except LinAlgError:
+            self.Rinv=pinvh(R,check_finite=False)
+            self.Rinv_y=np.dot(self.Rinv,self.output).flatten()
+        if self.name=='sexp':
+            if self.global_input is None:
+                X_l=self.input/self.length
+            else:
+                if len(self.length)==1:
+                    X_l=self.input/self.length
+                else:
+                    D=np.shape(self.input)[1]
+                    X_l=self.input/self.length[:D]
+            dists = pdist(X_l, metric="sqeuclidean")
+            self.R2sexp = squareform(np.exp(-dists/2))
+            np.fill_diagonal(self.R2sexp, 1)
+            self.Psexp = Pmatrix(X_l)
+
+    def cv_stats(self, i):
+        """Compute the inversion for the LOO.
+        """
+        if self.rep is not None:
+            R=self.k_matrix()
+            idx = self.rep!=i
+            R_loo_i = R[idx,:][:,idx]
+            #LOOinv = pinvh(R_loo_i,check_finite=False)
+            try:
+                L=np.linalg.cholesky(R_loo_i)
+                LOOinv = cho_solve((L, True), np.eye(len(R_loo_i)), check_finite=False)
+            except LinAlgError:
+                LOOinv = pinvh(R_loo_i,check_finite=False)
+        else:
+            LOOinv = inv_swp(self.Rinv, i)
+        return(LOOinv)
+
 
 def combine(*layers):
-    """Combine layers into one list as a DGP structure.
+    """Combine layers into one list as a DGP or linked (D)GP structure.
 
     Args:
-        *layers (list): a sequence of lists, each of which contains the GPs (defined by the kernel class) in that layer.
+        layers (list): a sequence of lists, each of which contains the GP nodes (defined by the :class:`.kernel` class), 
+            likelihood nodes (e.g., defined by the :class:`.Poisson` class), or containers (defined by the :class:`.container` class)
+            in that layer.
 
     Returns:
-        list: a list of layers defining the DGP structure.
+        list: a list of layers defining the DGP or linked (D)GP structure.
     """
     all_layer=[]
     for layer in layers:
         all_layer.append(layer)
     return all_layer
```

### Comparing `dgpsi-2.1b0/dgpsi/likelihood_class.py` & `dgpsi-2.2.0/dgpsi/likelihood_class.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import numpy as np
 from scipy.special import loggamma
 from scipy.linalg import cho_solve
 from .functions import fmvn_mu
 
 class Poisson:
-    """Class to implement Poisson likelihood. It (and all likelihoods below) can only be added as the final
-       layer of the DGP+likelihood model.
+    """Class to implement Poisson likelihood. It can only be added as the final layer of a DGP model.
 
-        Args:
-            input_dim (ndarray, optional): a numpy 1d-array that contains the indices of GPs in the last 
-            layer whose outputs feed into the likelihood node. When set to None, all outputs from GPs of 
-            last layer feed into the likelihood node. Defaults to None.
-
-        Attributes:
-            type (str): identifies that the node is a likelihood node;
-            input (ndarray): a numpy 2d-array (each row as a data point and each column as a likelihood parameter from the
-                DGP part) that contains the input data (according to the argument 'input_dim') to the likelihood node. The value of 
-                this attribute is assigned during the initialisation of 'dgp' class. 
-            output (ndarray): a numpy 2d-array with only one column that contains the output data to the likelihood node.
-                The value of this attribute is assigned during the initialisation of 'dgp' class.
-            exact_post_idx (ndarray): a numpy 1d-array that indicates the indices of the likelihood parameters that allow closed-form
-               conditional posterior distributions. Defaults to None.
-            rep (ndarray): a numpy 1d-array used to re-construct repetitions in the data according to the repetitions in the global input,
-                i.e., rep is assigned during the initialisation of 'dgp' class if one input position has multiple outputs. Otherwise, it is
-                None. Defaults to None. 
+    Args:
+        input_dim (ndarray, optional): a numpy 1d-array of length one that contains the indices of one GP in the feeding 
+            layer whose outputs feed into the likelihood node. When set to `None`, all outputs from GPs of 
+            the feeding layer feed into the likelihood node, and in this case one needs to ensure there is only one GP node specified
+            in the feeding layer. Defaults to `None`.
+
+    Attributes:
+        type (str): identifies that the node is a likelihood node;
+        input (ndarray): a numpy 2d-array (each row as a data point and each column as a likelihood parameter from the
+            DGP part) that contains the input data (according to the argument **input_dim**) to the likelihood node. The value of 
+            this attribute is assigned during the initialisation of :class:`.dgp` class. 
+        output (ndarray): a numpy 2d-array with only one column that contains the output data to the likelihood node.
+            The value of this attribute is assigned during the initialisation of :class:`.dgp` class.
+        exact_post_idx (ndarray): a numpy 1d-array that indicates the indices of the likelihood parameters that allow closed-form
+            conditional posterior distributions. Defaults to `None`.
+        rep (ndarray): a numpy 1d-array used to re-construct repetitions in the data according to the repetitions in the global input,
+            i.e., rep is assigned during the initialisation of :class:`.dgp` class if one input position has multiple outputs. Otherwise, it is
+            `None`. Defaults to `None`. 
     """
     def __init__(self, input_dim=None):
         self.type='likelihood'
         self.name='Poisson'
         self.input=None
         self.output=None
         self.input_dim=input_dim
@@ -45,36 +45,35 @@
         return llik
     
     @staticmethod
     def pllik(y,f):
         """The predicted log-likelihood function of Poisson distribution.
 
         Args:
-            y (ndarray): a numpy 3d-array of output data with shape (N,1,1), where N is the number of output data points.
-            f (ndarray): a numpy 3d-array of sample points with shape (N,S,Q), where S is the number of sample points and 
-                         Q is the number of parameters in the distribution (e.g., Q=1 for Poisson distribution).
+            y (ndarray): a numpy 3d-array of output data with shape ``(N,1,1)``, where *N* is the number of output data points.
+            f (ndarray): a numpy 3d-array of sample points with shape ``(N,S,Q)``, where *S* is the number of sample points and 
+                *Q* is the number of parameters in the distribution (e.g., *Q* = `1` for Poisson distribution).
 
         Returns:
-            ndarray: a numpy 3d-array of log-likelihood for given f.
+            ndarray: a numpy 3d-array of log-likelihood for given **f**.
         """
         pllik=y*f-np.exp(f)-loggamma(y+1)
         return pllik
 
     @staticmethod    
     def prediction(m,v):
-        """Compute mean and variance of the DGP+Poisson model given the predictive
-           mean and variance of DGP model for Poisson parameter.
+        """Compute mean and variance of the DGP+Poisson model given the predictive mean and variance of DGP model for Poisson parameter.
         
         Args:
             m (ndarray): a numpy 2d-array of predictive mean from the DGP model for the Poisson parameter.
             v (ndarray): a numpy 2d-array of predictive variance from the DGP model for the Poisson parameter.
 
         Returns:
             tuple: a tuple of two 1d-arrays giving the means and variances at the testing input data positions (that are 
-                represented by predictive means and variances).
+            represented by predictive means and variances).
         """
         y_mean=np.exp(m+v/2)
         y_var=np.exp(m+v/2)+(np.exp(v)-1)*np.exp(2*m+v)
         return y_mean.flatten(),y_var.flatten()
     
     def sampling(self,f_sample):
         """Generate samples of DGP+Poisson model given samples of DGP model for the Poisson parameter.
@@ -85,14 +84,22 @@
         Returns:
             tuple: a tuple of one 1d-arrays giving samples at the testing input data positions.
         """
         y_sample=np.random.poisson(np.exp(f_sample))
         return y_sample.flatten()
 
 class Hetero:
+    """Class to implement Heteroskedastic Gaussian likelihood. It can only be added as the final layer of a DGP model.
+
+    Args:
+        input_dim (ndarray, optional): a numpy 1d-array of length two that contains the indices of two GPs in the feeding 
+            layer whose outputs feed into the likelihood node. When set to `None`, all outputs from GPs of 
+            the feeding layer feed into the likelihood node, and in this case one needs to ensure there are only two GP nodes specified
+            in the feeding layer. Defaults to `None`.
+    """
     def __init__(self, input_dim=None):
         self.type='likelihood'
         self.name='Hetero'
         self.input=None
         self.output=None
         self.input_dim=input_dim
         self.exact_post_idx=np.array([0])
@@ -140,36 +147,44 @@
             #f_mu=np.random.default_rng().multivariate_normal(mean=mu,cov=cov,check_valid='ignore')
             f_mu=fmvn_mu(mu,cov)
             return f_mu
     
     @staticmethod
     def post_het1(v,Gamma,y_mask):
         """Calculate the conditional posterior mean and covariance of the mean 
-            of the heteroskedastic Gaussian likelihood when there are no repetitions
-            in the training data.
+           of the heteroskedastic Gaussian likelihood when there are no repetitions
+           in the training data.
         """
         L=np.linalg.cholesky(Gamma+v)
         #mu=np.sum(v*cho_solve((L, True), y_mask, check_finite=False),axis=1)
         mu=(v@cho_solve((L, True), y_mask, check_finite=False)).flatten()
         cov=v@cho_solve((L, True), Gamma, check_finite=False)
         return mu, cov
 
     @staticmethod
     def post_het2(v,Gamma,v_mask,V_mask,y_mask):
         """Calculate the conditional posterior mean and covariance of the mean 
-            of the heteroskedastic Gaussian likelihood when there are repetitions
-            in the training data.
+           of the heteroskedastic Gaussian likelihood when there are repetitions
+           in the training data.
         """
         L=np.linalg.cholesky(Gamma+V_mask)
         #mu=np.sum(v_mask.T*cho_solve((L, True), y_mask, check_finite=False),axis=1)
         mu=(v_mask.T@cho_solve((L, True), y_mask, check_finite=False)).flatten()
         cov=v-v_mask.T@cho_solve((L, True), v_mask, check_finite=False)
         return mu, cov    
 
 class NegBin:
+    """Class to implement Negative Binomial likelihood. It can only be added as the final layer of a DGP model.
+
+    Args:
+        input_dim (ndarray, optional): a numpy 1d-array of length two that contains the indices of two GPs in the feeding 
+            layer whose outputs feed into the likelihood node. When set to `None`, all outputs from GPs of 
+            the feeding layer feed into the likelihood node, and in this case one needs to ensure there are only two GP nodes specified
+            in the feeding layer. Defaults to `None`.
+    """
     def __init__(self, input_dim=None):
         self.type='likelihood'
         self.name='NegBin'
         self.input=None
         self.output=None
         self.input_dim=input_dim
         self.exact_post_idx=None
```

### Comparing `dgpsi-2.1b0/dgpsi/linkgp.py` & `dgpsi-2.2.0/dgpsi/linkgp.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,62 +8,78 @@
 
 class container:
     """
     Class to contain the trained GP or DGP emulator of a computer model for linked (D)GP emulation.
 
     Args:
         structure (list): a list that contains the trained structure of GP or DGP of a computer model. For GP, 
-            this is the list exported from the 'export' method of the gp class. For DGP, this is the list exported 
-            from the 'estimate' method of the dgp class.
-        local_input_idx (ndarray): a numpy 1d-array that specifies the indices of outputs (a 2d-array) 
-            produced by all models in the feeding layer that are input to the model emulated by the GP or DGP
-            represented by the 'structure' argument. The indices should be ordered in such a way that the extracted
-            output from the feeding layer is sorted in the same order as the training input used for the GP/DGP 
-            emulation of the computer model that the 'structure' argument represents. When the model is in the first
-            layer, 'local_input_idx' gives the indices of its input in the global testing input set, see 'predict' 
-            method of 'lgp' class for descriptions of the global testing input set. Defaults to None. When the
-            argument is None, one needs to set its value using the 'set_local_input' method of the class. 
+            this is the list exported from the :meth:`.export` method of the :class:`.gp` class. For DGP, this is the list exported 
+            from the :meth:`.estimate` of the :class:`.dgp` class.
+        local_input_idx (ndarray_or_list): a numpy 1d-array or a list:
+
+            1. If **local_input_idx** is a 1d-array, it specifies the indices of outputs (a 2d-array) 
+               produced by all emulators in the feeding layer that are input to the emulator
+               represented by the **structure** argument. The indices should be ordered in such a way that the extracted
+               output from the feeding layer is sorted in the same order as the training input used for the GP/DGP 
+               emulator that the **structure** argument represents. When the emulator is in the first
+               layer, **local_input_idx** gives the indices of its input in the global testing input set, see :meth:`.lgp.predict`
+               for descriptions of the global testing input set. 
+            2. If **local_input_idx** is a list, the emulator must be in layer 2 or deeper layers. The list should have a number 
+               (the same number of preceding layers, e.g., when an emulator is in the second layer, the list is of length 1) of elements. Each
+               element is a 1d-array that specifies the indices of outputs produced by all emulators in the corresponding layer 
+               that feed to the emulator represented by the **structure** argument. If there is no output connections from a certain layer,
+               set `None` instead in the list. 
+               
+            Defaults to `None`. When the argument is `None`, one needs to set its value using the :meth:`.set_local_input`. 
+        block (bool, optional): whether to use the blocked (layer-wise) ESS for the imputations. Defaults to `True`.
     """
-    def __init__(self, structure, local_input_idx=None):
+    def __init__(self, structure, local_input_idx=None, block=True):
         if len(structure)==1:
             self.type='gp'
             self.structure=structure[0]
         else:
             self.type='dgp'
             self.structure=structure
-            self.imp=imputer(self.structure)
+            self.imp=imputer(self.structure, block)
             self.imp.sample(burnin=50)
         self.local_input_idx=local_input_idx
 
     def set_local_input(self, idx):
-        """Set the 'local_input_idx' argument if it is not set when the class is constructed.
+        """Set the **local_input_idx** argument if it is not set when the class is constructed.
+
+        Remark: 
+           This method is useful when different models are emulated by different teams. Each team can create the container
+           of their model even without knowing how different models are connected together. When this information is available and
+           containers of different emulators are collected, the connections between emulators can then be set by assigning
+           values to **local_input_idx** of each container with this method.
         """
         self.local_input_idx=idx
 
 class lgp:
     """
     Class to store a system of GP and DGP emulators for predictions. 
 
     Args:
-        all_layer (list): a list contains L (the number of layers of a systems of computer models) sub-lists, 
+        all_layer (list): a list contains *L* (the number of layers of a systems of computer models) sub-lists, 
             each of which represents a layer and contains the GP/DGP emulators of computer models represented by 
-            the 'container' class. The sub-lists are placed in the list in the same order of the specified computer
+            the :class:`.container` class. The sub-lists are placed in the list in the same order of the specified computer
             model system.
         N (int): the number of imputation to produce the predictions. Increase the value to account for more 
-            imputation uncertainties. If the system consists only GP emulators, 'N' is set to 1 automatically. 
-            Defaults to 50.
-        nb_parallel (bool, optional): whether to use Numba's multi-threading to accelerate the predictions. Defaults to False.
+            imputation uncertainties. If the system consists only GP emulators, **N** is set to `1` automatically. 
+            Defaults to `50`.
+        nb_parallel (bool, optional): whether to use *Numba*'s multi-threading to accelerate the predictions. Defaults to `False`.
     """
     def __init__(self, all_layer, N=50, nb_parallel=False):
         self.nb_parallel=nb_parallel
         self.L=len(all_layer)
+        self.all_layer=all_layer
         self.num_model=[]
         for l in range(1,self.L):
             self.num_model.append(len(all_layer[l]))
-        if np.sum([[cont.type=='dgp' for cont in all_layer[l]] for l in range(self.L)])==0:
+        if np.sum(np.concatenate([[cont.type=='dgp' for cont in all_layer[l]] for l in range(self.L)]))==0:
             N=1
         self.all_layer_set=[]
         for _ in range(N):
             one_imputation=[]
             for l in range(self.L):
                 layer=[]
                 for cont in all_layer[l]:
@@ -73,29 +89,28 @@
                         (cont.imp).sample()
                         (cont.imp).key_stats()
                         layer.append(copy.deepcopy(cont))
                 one_imputation.append(layer)
             self.all_layer_set.append(one_imputation)
 
     def set_nb_parallel(self,nb_parallel):
-        """Set 'self.nb_parallel' to the bool value given by 'nb_parallel'. This method is useful to change 'self.nb_parallel'
-            when the lgp class has already been built.
+        """Set 'self.nb_parallel' to the bool value given by **nb_parallel**. This method is useful to change **self.nb_parallel**
+            when the :class:`.lgp` class has already been built.
         """
         self.nb_parallel=nb_parallel
     
     def ppredict(self,x,method='mean_var',full_layer=False,sample_size=50,chunk_num=None,core_num=None):
         """Implement parallel predictions from the trained DGP model.
 
         Args:
-            x, method, full_layer, sample_size: see descriptions of the method `predict`.
-            chunk_num (int, optional): the number of chunks that the testing input array 'x' will be divided into. 
-                Defaults to None. If not specified, the number of chunks will be determined by dividing the input
-                array into chunks with max 200 input positions. 
-            core_num (int, optional): the number of cores/workers to be used. Defaults to None. If not specified, 
-                the number of cores is set to (max physical cores available - 1).
+            x, method, full_layer, sample_size: see descriptions of the method :meth:`.lgp.predict`.
+            chunk_num (int, optional): the number of chunks that the testing input array **x** will be divided into. 
+                Defaults to `None`. If not specified, the number of chunks is set to **core_num**. 
+            core_num (int, optional): the number of cores/workers to be used. Defaults to `None`. If not specified, 
+                the number of cores is set to ``(max physical cores available - 1)``.
 
         Returns:
             Same as the method `predict`.
         """
         if platform.system()=='Darwin':
             ctx._force_start_method('forkserver')
         if core_num==None:
@@ -112,15 +127,15 @@
                 for l in range(self.L):
                     if l==0:
                         z=[[element] for element in np.array_split(x[l],chunk_num)]
                     else:
                         z_l=x[l]
                         z_m=[[]]*chunk_num
                         for m in range(len(z_l)):
-                            if z_l[m]==None:
+                            if z_l[m] is None:
                                 z_m=[i+j for i, j in zip(z_m,[[None]]*chunk_num)]
                             else:
                                 z_m=[i+[j] for i, j in zip(z_m,np.array_split(z_l[m],chunk_num))]
                         z=[i+[j] for i,j in zip(z,z_m)]
         elif not isinstance(x, list):
             z=np.array_split(x,chunk_num)
         with Pool(core_num) as pool:
@@ -148,61 +163,65 @@
             else:
                 return list(np.concatenate(worker,axis=1) for worker in zip(*res))
 
     def predict(self,x,method='mean_var',full_layer=False,sample_size=50):
         """Implement predictions from the linked (D)GP model.
 
         Args:
-            x Union[ndarray, list]: a numpy 2d-array or a list:
-                1. If x is a 2d-array, it is the global testing input set to the computer models in the first layer where 
-                    each rows are input testing data points and columns are input dimensions across all computer models in 
-                    the first layer of the system. In this case, it is assumed that 'x' is the only global input to the computer 
-                    system, i.e., there are no external global input to computer models in layers other than the first layer.
-                2. If x is a list, it has L (the number of layers of a systems of computer models) elements. The first element
-                    is a numpy 2d-array that represents the global testing input set to the computer models in the first layer. 
-                    The remaining L-1 elements are L-1 sub-lists, each of which contains a number (same as the number of computer
-                    models in the corresponding layer) of numpy 2d-arrays (rows being testing points and columns being input 
-                    dimensions) that represent the external global testing input to the computer models in the corresponding layer. 
-                    The order of 2d-arrays in each sub-list must be the same order of the emulators placed in the corresponding layer
-                    of 'all_layer' argument to 'lgp' class. If there is no external global input to a certain computer model of the 
-                    system, set None in the corresponding sub-list (i.e., layer) of 'x'.   
-            method (str, optional): the prediction approach: mean-variance ('mean_var') or sampling 
-                ('sampling') approach. Defaults to 'mean_var'.
-            full_layer (bool, optional): whether to output the predictions from all GP/DGP emulators in the system. Defaults to False.
-            sample_size (int, optional): the number of samples to draw for each given imputation in 'sampling' method.
-                Defaults to 50.
+            x (ndarray_or_list): a numpy 2d-array or a list.
+            
+                1. If **x** is a 2d-array, it is the global testing input set to the computer emulators in the first layer where 
+                   each rows are input testing data points and columns are input dimensions across all computer emulators in 
+                   the first layer of the system. In this case, it is assumed that **x** is the only global input to the computer 
+                   system, i.e., there are no external global input to computer emulators in layers other than the first layer.
+                2. If **x** is a list, it has *L* (the number of layers of a systems of emulators) elements. The first element
+                   is a numpy 2d-array that represents the global testing input set to the computer emulators in the first layer. 
+                   The remaining *L-1* elements are *L-1* sub-lists, each of which contains a number (same as the number of computer
+                   emulators in the corresponding layer) of numpy 2d-arrays (rows being testing points and columns being input 
+                   dimensions) that represent the external global testing input to the computer models in the corresponding layer. 
+                   The order of 2d-arrays in each sub-list must be the same order of the emulators placed in the corresponding layer
+                   of **all_layer** argument to :class:`.lgp` class. If there is no external global input to a certain computer emulator of the 
+                   system, set `None` in the corresponding sub-list (i.e., layer) of **x**.   
+            method (str, optional): the prediction approach: mean-variance (`mean_var`) or sampling 
+                (`sampling`) approach. Defaults to `mean_var`.
+            full_layer (bool, optional): whether to output the predictions from all GP/DGP emulators in the system. Defaults to `False`.
+            sample_size (int, optional): the number of samples to draw for each given imputation if **method** = '`sampling`'.
+                Defaults to `50`.
             
         Returns:
-            Union[tuple, list]: 
-                if the argument method='mean_var', a tuple is returned:
-                    1. If full_layer=False, the tuple contains two lists, one for the predictive means 
-                        and another for the predictive variances. Each list contains a number (same number of computer models in the
-                        final layer of the system) of numpy 2d-arrays. Each 2d-array has its rows corresponding to global testing 
-                        positions and columns corresponding to GP/DGP (or DGP+likelihood) output dimensions of the associated computer
-                        model in the final layer;
-                    2. If full_layer=True, the tuple contains two lists, one for the predictive means 
-                        and another for the predictive variances. Each list contains L (i.e., the number of layers of the emulated system) 
-                        sub-lists. Each sub-list represents a layer and contains a number (same number of computer models in the corresponding 
-                        layer of the system) of numpy 2d-arrays. Each array has its rows corresponding to global testing positions and columns 
-                        corresponding to GP/DGP (or DGP+likelihood in case of the final layer) output dimensions of the associated computer
-                        model in the corresponding layer.
-                if the argument method='sampling', a list is returned:
-                    1. If full_layer=False, the list contains a number (same number of computer models in the final layer of the system) of numpy 
-                        3d-arrays. Each array corresponds to a computer model in the final layer, and has its 0-axis corresponding to the output 
-                        dimensions of the GP/DGP (or DGP+likelihood) emulators, 1-axis corresponding to global testing positions, and 2-axis 
-                        corresponding to samples of size 'N' imputations * 'sample_size';
-                    2. If full_layer=True, the list contains L (i.e., the number of layers of the emulated system) sub-lists. Each sub-list 
-                        represents a layer and contains a number (same number of computer models in the corresponding layer of the system) of 
-                        numpy 3d-arrays. Each array corresponds to a computer model in the associated layer, and has its 0-axis corresponding 
-                        to the output dimensions of the GP/DGP (or DGP+likelihood in case of the final layer) emulators, 1-axis corresponding 
-                        to global testing positions, and 2-axis corresponding to samples of size 'N' imputations * 'sample_size'.
+            tuple_or_list: 
+                if the argument **method** = '`mean_var`', a tuple is returned:
+
+                    1. If **full_layer** = `False`, the tuple contains two lists, one for the predictive means 
+                       and another for the predictive variances. Each list contains a number (same number of emulators in the
+                       final layer of the system) of numpy 2d-arrays. Each 2d-array has its rows corresponding to global testing 
+                       positions and columns corresponding to output dimensions of the associated emulator in the final layer;
+                    2. If **full_layer** = `True`, the tuple contains two lists, one for the predictive means 
+                       and another for the predictive variances. Each list contains *L* (i.e., the number of layers of the emulated system) 
+                       sub-lists. Each sub-list represents a layer and contains a number (same number of emulators in the corresponding 
+                       layer of the system) of numpy 2d-arrays. Each array has its rows corresponding to global testing positions and columns 
+                       corresponding to output dimensions of the associated GP/DGP emulator in the corresponding layer.
+                if the argument **method** = '`sampling`', a list is returned:
+                    
+                    1. If **full_layer** = `False`, the list contains a number (same number of emulators in the final layer of the system) of numpy 
+                       3d-arrays. Each array corresponds to an emulator in the final layer, and has its 0-axis corresponding to the output 
+                       dimensions of the GP/DGP emulator, 1-axis corresponding to global testing positions, and 2-axis 
+                       corresponding to samples of size **N** * **sample_size**;
+                    2. If **full_layer** = `True`, the list contains *L* (i.e., the number of layers of the emulated system) sub-lists. Each sub-list 
+                       represents a layer and contains a number (same number of emulators in the corresponding layer of the system) of 
+                       numpy 3d-arrays. Each array corresponds to an emulator in the associated layer, and has its 0-axis corresponding 
+                       to the output dimensions of the GP/DGP emulators, 1-axis corresponding to global testing positions, and 2-axis 
+                       corresponding to samples of size **N** * **sample_size**.
+
         """
         if isinstance(x, list) and len(x)!=self.L:
             raise Exception('When test input is given as a list, it must contain global inputs to the all layers (even with no global inputs to internal layers). Set None as the global input to the internal models if they have no global inputs.')
         elif not isinstance(x, list):
+            if x.ndim==1:
+                raise Exception('The testing input has to be a numpy 2d-array.')
             x=[x]
             for num in self.num_model:
                 x.append([None]*num) 
         if method=='mean_var':
             sample_size=1
         mean_pred=[]
         variance_pred=[]
@@ -226,14 +245,16 @@
                 else:
                     m_l,v_l=[], []
                     if method=='sampling':
                         sample_l=[]
                 if l==0:
                     for k in range(n_model):
                         model=layer[k]
+                        if isinstance(model.local_input_idx, list):
+                            raise Exception('When an emulator is in the first layer, local_input_idx must be a 1d-array.') 
                         input_lk=x[l][:,model.local_input_idx]
                         if model.type=='gp':
                             m_lk, v_lk = self.gp_pred(input_lk,None,None,None,model.structure,self.nb_parallel)
                         elif model.type=='dgp':
                             _, _, m_lk, v_lk = self.dgp_pred(input_lk,None,None,None,model.structure,self.nb_parallel)
                         m_l.append(m_lk)
                         v_l.append(v_lk)
@@ -243,20 +264,34 @@
                             sample_l.append(sample_lk.transpose(2,1,0))
                     if full_layer:
                         if method=='mean_var':
                             mean_pred_oneN.append(m_l)
                             variance_pred_oneN.append(v_l)
                         elif method=='sampling':
                             sample_pred_oneN.append(sample_l)
-                    m_l_next, v_l_next=np.concatenate(m_l,axis=1), np.concatenate(v_l,axis=1)
+                    m_l_next, v_l_next=[np.concatenate(m_l,axis=1)], [np.concatenate(v_l,axis=1)]
                 elif l==self.L-1:
                     for k in range(n_model):
                         model=layer[k]
+                        if isinstance(model.local_input_idx, list):
+                            if len(model.local_input_idx)!=self.L-1:
+                                raise Exception('local_input_idx should be a list that has length of %i.' % (self.L-1))
+                            else:
+                                local_input_idx = model.local_input_idx
+                        else:
+                            local_input_idx=[None]*(self.L-2)
+                            local_input_idx.append(model.local_input_idx)
                         external_input_lk=x[l][k]
-                        m_input_lk, v_input_lk = m_l_next[:,model.local_input_idx], v_l_next[:,model.local_input_idx]
+                        m_input_lk, v_input_lk = [], []
+                        for i in range(l):
+                            idx = local_input_idx[i]
+                            if idx is not None:
+                                m_input_lk.append( m_l_next[i][:,idx] )
+                                v_input_lk.append( v_l_next[i][:,idx] )
+                        m_input_lk, v_input_lk = np.concatenate(m_input_lk, axis=1), np.concatenate(v_input_lk, axis=1)
                         if model.type=='gp':
                             m_lk, v_lk=self.gp_pred(None,m_input_lk,v_input_lk,external_input_lk,model.structure,self.nb_parallel)
                             if method=='sampling':
                                 row_num, col_num = np.shape(m_lk)
                                 sample_lk=np.random.normal(m_lk,np.sqrt(v_lk),size=(sample_size, row_num, col_num)).transpose(2,1,0)
                         elif model.type=='dgp':
                             m_one_before_lk, v_one_before_lk, m_lk, v_lk = self.dgp_pred(None,m_input_lk,v_input_lk,external_input_lk,model.structure,self.nb_parallel)
@@ -279,16 +314,30 @@
                             mean_pred_oneN.append(m_last_layer)
                             variance_pred_oneN.append(v_last_layer)
                         elif method=='sampling':
                             sample_pred_oneN.append(sample_last_layer)
                 else:
                     for k in range(n_model):
                         model=layer[k]
+                        if isinstance(model.local_input_idx, list):
+                            if len(model.local_input_idx)!=l:
+                                raise Exception('local_input_idx should be a list that has length of %i.' % (l))
+                            else:
+                                local_input_idx = model.local_input_idx
+                        else:
+                            local_input_idx=[None]*(l-1)
+                            local_input_idx.append(model.local_input_idx)
                         external_input_lk=x[l][k]
-                        m_input_lk, v_input_lk = m_l_next[:,model.local_input_idx], v_l_next[:,model.local_input_idx]
+                        m_input_lk, v_input_lk = [], []
+                        for i in range(l):
+                            idx = local_input_idx[i]
+                            if idx is not None:
+                                m_input_lk.append( m_l_next[i][:,idx] )
+                                v_input_lk.append( v_l_next[i][:,idx] )
+                        m_input_lk, v_input_lk = np.concatenate(m_input_lk, axis=1), np.concatenate(v_input_lk, axis=1)
                         if model.type=='gp':
                             m_lk, v_lk = self.gp_pred(None,m_input_lk,v_input_lk,external_input_lk,model.structure,self.nb_parallel)
                         elif model.type=='dgp':
                             _, _, m_lk, v_lk = self.dgp_pred(None,m_input_lk,v_input_lk,external_input_lk,model.structure,self.nb_parallel)
                         m_l.append(m_lk)
                         v_l.append(v_lk)
                         if method=='sampling' and full_layer:
@@ -297,15 +346,16 @@
                             sample_l.append(sample_lk.transpose(2,1,0))
                     if full_layer:
                         if method=='mean_var':
                             mean_pred_oneN.append(m_l)
                             variance_pred_oneN.append(v_l)
                         elif method=='sampling':
                             sample_pred_oneN.append(sample_l)
-                    m_l_next, v_l_next=np.concatenate(m_l,axis=1), np.concatenate(v_l,axis=1)
+                    m_l_next.append(np.concatenate(m_l,axis=1))
+                    v_l_next.append(np.concatenate(v_l,axis=1))
             if full_layer:
                 if method=='mean_var':
                     mean_pred.append(mean_pred_oneN)
                     variance_pred.append(variance_pred_oneN)
                 elif method=='sampling':
                     sample_pred.append(sample_pred_oneN)
             else:
@@ -344,14 +394,16 @@
         """Compute predictive mean and variance from a DGP (DGP+likelihood) emulator when the testing input is either deterministic or normally distributed.
         """
         if x is None:
             M=len(m)
         else:
             M=len(x)
         L=len(structure)
+        internal_idx=structure[0][0].input_dim
+        external_idx=structure[0][0].connect
         for l in range(L):
             layer=structure[l]
             n_kerenl=len(layer)
             if l==L-1:
                 likelihood_gp_mean=np.empty((M,n_kerenl))
                 likelihood_gp_var=np.empty((M,n_kerenl))
             else:
@@ -369,22 +421,26 @@
             elif l==L-1:
                 for k in range(n_kerenl):
                     kernel=layer[k]
                     m_k_in,v_k_in=overall_test_input_mean[:,kernel.input_dim],overall_test_input_var[:,kernel.input_dim]
                     if kernel.type=='gp':
                         if kernel.connect is not None:
                             if x is None:
-                                D=np.shape(m)[1]
-                                idx1,idx2=kernel.connect[kernel.connect<=(D-1)],kernel.connect[kernel.connect>(D-1)]
-                                if idx1.size==0:
-                                    m_k,v_k=kernel.linkgp_prediction(m=m_k_in,v=v_k_in,z=z[:,idx2-D],nb_parallel=nb_parallel)
-                                elif idx2.size==0:
-                                    m_k,v_k=kernel.linkgp_prediction_full(m=m_k_in,v=v_k_in,m_z=m[:,idx1],v_z=v[:,idx1],z=None,nb_parallel=nb_parallel)
+                                if external_idx is None:
+                                    idx=np.where(kernel.connect[:, None] == internal_idx[None, :])[1]
+                                    m_k,v_k=kernel.linkgp_prediction_full(m=m_k_in,v=v_k_in,m_z=m[:,idx],v_z=v[:,idx],z=None,nb_parallel=nb_parallel)
                                 else:
-                                    m_k,v_k=kernel.linkgp_prediction_full(m=m_k_in,v=v_k_in,m_z=m[:,idx1],v_z=v[:,idx1],z=z[:,idx2-D],nb_parallel=nb_parallel)
+                                    idx1 = np.where(kernel.connect[:, None] == internal_idx[None, :])[1]
+                                    idx2 = np.where(kernel.connect[:, None] == external_idx[None, :])[1]
+                                    if idx1.size==0:
+                                        m_k,v_k=kernel.linkgp_prediction(m=m_k_in,v=v_k_in,z=z[:,idx2],nb_parallel=nb_parallel)
+                                    elif idx2.size==0:
+                                        m_k,v_k=kernel.linkgp_prediction_full(m=m_k_in,v=v_k_in,m_z=m[:,idx1],v_z=v[:,idx1],z=None,nb_parallel=nb_parallel)
+                                    else:
+                                        m_k,v_k=kernel.linkgp_prediction_full(m=m_k_in,v=v_k_in,m_z=m[:,idx1],v_z=v[:,idx1],z=z[:,idx2],nb_parallel=nb_parallel)
                             else:
                                 m_k,v_k=kernel.linkgp_prediction(m=m_k_in,v=v_k_in,z=x[:,kernel.connect],nb_parallel=nb_parallel)
                         else:
                             m_k,v_k=kernel.linkgp_prediction(m=m_k_in,v=v_k_in,z=None,nb_parallel=nb_parallel)
                         likelihood_gp_mean[:,k],likelihood_gp_var[:,k]=m_k,v_k
                     elif kernel.type=='likelihood':
                         m_k,v_k=kernel.prediction(m=m_k_in,v=v_k_in)
```

### Comparing `dgpsi-2.1b0/dgpsi/synthetic.py` & `dgpsi-2.2.0/dgpsi/synthetic.py`

 * *Files identical despite different names*

### Comparing `dgpsi-2.1b0/setup.py` & `dgpsi-2.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 
-VERSION = '2.1-beta'
+VERSION = '2.2.0'
 PACKAGE_NAME = 'dgpsi'
 AUTHOR = 'Deyu Ming'
 AUTHOR_EMAIL = 'deyu.ming.16@ucl.ac.uk'
 URL = 'https://github.com/mingdeyu/DGP'
 
 LICENSE = 'MIT'
-DESCRIPTION = 'Deep Gaussian Process Emulation using Stochastic Imputation'
+DESCRIPTION = 'Deep and Linked Gaussian Process Emulations using Stochastic Imputation'
 LONG_DESCRIPTION = (here / 'README.md').read_text(encoding='utf-8')
 
 INSTALL_REQUIRES = [
       'numpy>=1.18.2',
       'numba>=0.51.2',
       'matplotlib>=3.2.1',
       'tqdm>=4.50.2',
@@ -23,15 +23,16 @@
       'jupyter>=1.0.0',
       'dill>=0.3.2',
       'pathos>=0.2.9',
       'psutil>=5.8.0',
       'cython>=0.29.30',
       'pybind11>=2.10.0',
       'pythran>=0.11.0',
-      'scikit-build>=0.15.0'
+      'scikit-build>=0.15.0',
+      'tabulate>=0.8.7'
 ]
 
 setup(name=PACKAGE_NAME,
       version=VERSION,
       description=DESCRIPTION,
       long_description=LONG_DESCRIPTION,
       long_description_content_type='text/markdown',
```

