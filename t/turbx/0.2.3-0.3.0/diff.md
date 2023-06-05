# Comparing `tmp/turbx-0.2.3.tar.gz` & `tmp/turbx-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbx-0.2.3.tar", last modified: Fri Apr 21 16:14:18 2023, max compression
+gzip compressed data, was "turbx-0.3.0.tar", last modified: Mon Jun  5 13:53:04 2023, max compression
```

## Comparing `turbx-0.2.3.tar` & `turbx-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 iagappel  (1000) iagappel  (1000)        0 2023-04-21 16:14:18.676028 turbx-0.2.3/
--rwxrwxr-x   0 iagappel  (1000) iagappel  (1000)     1065 2022-06-30 12:13:09.000000 turbx-0.2.3/LICENSE
--rw-r--r--   0 iagappel  (1000) iagappel  (1000)     2353 2023-04-21 16:14:18.676028 turbx-0.2.3/PKG-INFO
--rwxrwxr-x   0 iagappel  (1000) iagappel  (1000)     1072 2023-04-15 18:45:25.000000 turbx-0.2.3/README.md
--rw-r--r--   0 iagappel  (1000) iagappel  (1000)       38 2023-04-21 16:14:18.676028 turbx-0.2.3/setup.cfg
--rwxrwxr-x   0 iagappel  (1000) iagappel  (1000)     2295 2023-04-21 16:13:23.000000 turbx-0.2.3/setup.py
-drwxr-xr-x   0 iagappel  (1000) iagappel  (1000)        0 2023-04-21 16:14:18.676028 turbx-0.2.3/turbx/
--rwxrwxr-x   0 iagappel  (1000) iagappel  (1000)     3154 2023-04-15 18:44:32.000000 turbx-0.2.3/turbx/__init__.py
--rwxrwxr-x   0 iagappel  (1000) iagappel  (1000)  1145346 2023-04-21 16:06:44.000000 turbx-0.2.3/turbx/turbx.py
-drwxr-xr-x   0 iagappel  (1000) iagappel  (1000)        0 2023-04-21 16:14:18.676028 turbx-0.2.3/turbx.egg-info/
--rw-r--r--   0 iagappel  (1000) iagappel  (1000)     2353 2023-04-21 16:14:18.000000 turbx-0.2.3/turbx.egg-info/PKG-INFO
--rw-r--r--   0 iagappel  (1000) iagappel  (1000)      203 2023-04-21 16:14:18.000000 turbx-0.2.3/turbx.egg-info/SOURCES.txt
--rw-r--r--   0 iagappel  (1000) iagappel  (1000)        1 2023-04-21 16:14:18.000000 turbx-0.2.3/turbx.egg-info/dependency_links.txt
--rw-r--r--   0 iagappel  (1000) iagappel  (1000)      143 2023-04-21 16:14:18.000000 turbx-0.2.3/turbx.egg-info/requires.txt
--rw-r--r--   0 iagappel  (1000) iagappel  (1000)        6 2023-04-21 16:14:18.000000 turbx-0.2.3/turbx.egg-info/top_level.txt
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-06-05 13:53:04.442429 turbx-0.3.0/
+-rwxrwxr-x   0 jason     (1000) jason     (1000)     1065 2022-06-30 12:13:09.000000 turbx-0.3.0/LICENSE
+-rw-rw-r--   0 jason     (1000) jason     (1000)     2353 2023-06-05 13:53:04.442429 turbx-0.3.0/PKG-INFO
+-rwxrwxr-x   0 jason     (1000) jason     (1000)     1072 2023-04-15 18:45:25.000000 turbx-0.3.0/README.md
+-rw-rw-r--   0 jason     (1000) jason     (1000)       38 2023-06-05 13:53:04.442429 turbx-0.3.0/setup.cfg
+-rwxrwxr-x   0 jason     (1000) jason     (1000)     2295 2023-06-05 13:43:40.000000 turbx-0.3.0/setup.py
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-06-05 13:53:04.438429 turbx-0.3.0/turbx/
+-rwxrwxr-x   0 jason     (1000) jason     (1000)     3260 2023-06-05 13:43:21.000000 turbx-0.3.0/turbx/__init__.py
+-rwxrwxr-x   0 jason     (1000) jason     (1000)  1170945 2023-06-05 13:37:28.000000 turbx-0.3.0/turbx/turbx.py
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-06-05 13:53:04.442429 turbx-0.3.0/turbx.egg-info/
+-rw-rw-r--   0 jason     (1000) jason     (1000)     2353 2023-06-05 13:53:04.000000 turbx-0.3.0/turbx.egg-info/PKG-INFO
+-rw-rw-r--   0 jason     (1000) jason     (1000)      203 2023-06-05 13:53:04.000000 turbx-0.3.0/turbx.egg-info/SOURCES.txt
+-rw-rw-r--   0 jason     (1000) jason     (1000)        1 2023-06-05 13:53:04.000000 turbx-0.3.0/turbx.egg-info/dependency_links.txt
+-rw-rw-r--   0 jason     (1000) jason     (1000)      143 2023-06-05 13:53:04.000000 turbx-0.3.0/turbx.egg-info/requires.txt
+-rw-rw-r--   0 jason     (1000) jason     (1000)        6 2023-06-05 13:53:04.000000 turbx-0.3.0/turbx.egg-info/top_level.txt
```

### Comparing `turbx-0.2.3/LICENSE` & `turbx-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `turbx-0.2.3/PKG-INFO` & `turbx-0.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turbx
-Version: 0.2.3
+Version: 0.3.0
 Summary: Extensible toolkit for analyzing turbulent flow datasets
 Home-page: https://github.com/iagappel/turbx
 Author: Jason A
 Maintainer: Jason A
 License: MIT
 Keywords: scientific computing,statistics,simulation,turbulence,turbulent flows,direct numerical simulation,DNS,parallel,visualization
 Platform: any
```

### Comparing `turbx-0.2.3/README.md` & `turbx-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `turbx-0.2.3/setup.py` & `turbx-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name='turbx',
-    version='0.2.3',
+    version='0.3.0',
     description='Extensible toolkit for analyzing turbulent flow datasets',
     
     long_description=long_description,
     long_description_content_type='text/markdown',
     
     url='https://github.com/iagappel/turbx',
     author='Jason A',
```

### Comparing `turbx-0.2.3/turbx/__init__.py` & `turbx-0.3.0/turbx/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 '''
 turbx
 
 Extensible toolkit for analyzing turbulent flow datasets
 '''
 
-__version__ = '0.2.2'
+__version__ = '0.3.0'
 __author__ = 'Jason A'
 
 from .turbx import cgd
 from .turbx import rgd
 from .turbx import eas4
 from .turbx import ztmd
 from .turbx import lpd
 from .turbx import spd
 
+from .turbx import h5_chunk_sizer
 from .turbx import h5_visititems_print_attrs
 from .turbx import h5_visit_container
 
 from .turbx import eas3
 
 from .turbx import curve_fitter
 
@@ -31,14 +32,15 @@
 from .turbx import interp_1d
 from .turbx import fd_coeff_calculator
 from .turbx import gradient
 from .turbx import get_metric_tensor_3d
 from .turbx import get_metric_tensor_2d
 from .turbx import get_grid_quality_metrics_2d
 from .turbx import smoothstep
+from .turbx import stretch_1d_cluster_ends
 
 from .turbx import rect_to_cyl
 from .turbx import cyl_to_rect
 from .turbx import rotate_2d
 
 from .turbx import get_grad
 from .turbx import get_curl
@@ -69,14 +71,15 @@
 
 __all__ = ['cgd',
            'rgd',
            'eas4',
            'ztmd',
            'lpd',
            'spd',
+           'h5_chunk_sizer',
            'h5_visititems_print_attrs',
            'h5_visit_container',
            'eas3',
            'curve_fitter',
            'Blasius_solution',
            'freestream_parameters',
            'calc_bl_edge_1d',
```

### Comparing `turbx-0.2.3/turbx/turbx.py` & `turbx-0.3.0/turbx/turbx.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,25 +31,28 @@
 import skimage
 from skimage import color
 
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 import cmocean, colorcet, cmasher
 
+import colorspacious
+from colorspacious import cspace_converter
+
 # import vtk
 # from vtk.util import numpy_support
 
 ## required for EAS3
 import struct
 
 '''
 ========================================================================
 
 turbx: an extensible toolkit for analyzing turbulent flow datasets
---> version Spring 2023
+--> version Summer 2023
 
 $> wget https://raw.githubusercontent.com/iagappel/turbx/main/turbx/turbx.py
 $> git clone git@gitlab.iag.uni-stuttgart.de:transi/turbx.git
 $> git clone git@github.com:iagappel/turbx.git
 
 h5py Documentation:
 https://docs.h5py.org/_/downloads/en/3.8.0/pdf/
@@ -112,57 +115,72 @@
             kwargs.pop('driver')
         if ( not self.usingmpi ) and ('comm' in kwargs):
             kwargs.pop('comm')
         
         ## | mpiexec --mca io romio321 -n $NP python3 ...
         ## | mpiexec --mca io ompio -n $NP python3 ...
         ## | ompi_info --> print ompi settings ('MCA io' gives io implementation options)
-        ## | export ROMIO_FSTYPE_FORCE="lustre:" --> force Lustre driver over UFS --> causes crash
+        ## | export ROMIO_FSTYPE_FORCE="lustre:" --> force Lustre driver over UFS when using romio --> causes crash
         ## | export ROMIO_FSTYPE_FORCE="ufs:"
         ## | export ROMIO_PRINT_HINTS=1 --> show available hints
         
-        ## determine MPI info / hints
+        ## https://doku.lrz.de/best-practices-hints-and-optimizations-for-io-10747318.html
+        
+        ## OMPIO
+        ## export OMPI_MCA_sharedfp=^lockedfile,individual
+        ## mpiexec --mca io ompio -n $NP python3 script.py
+        
+        ## set ROMIO hints, passed through 'mpi_info' dict
         if self.usingmpi:
             if ('info' in kwargs):
                 self.mpi_info = kwargs['info']
             else:
                 mpi_info = MPI.Info.Create()
                 ##
                 mpi_info.Set('romio_ds_write' , 'disable'   )
                 mpi_info.Set('romio_ds_read'  , 'disable'   )
                 mpi_info.Set('romio_cb_read'  , 'automatic' )
                 mpi_info.Set('romio_cb_write' , 'automatic' )
                 #mpi_info.Set('romio_cb_read'  , 'enable' )
                 #mpi_info.Set('romio_cb_write' , 'enable' )
-                mpi_info.Set('cb_buffer_size' , str(int(round(16*1024**2))) ) ## 16 [MB]
+                #mpi_info.Set('cb_buffer_size' , str(int(round(16*1024**2))) ) ## 16 [MB]
+                mpi_info.Set('cb_buffer_size' , str(int(round(32*1024**2))) ) ## 32 [MB]
+                ##
+                #mpi_info.Set('romio_no_indep_rw' , 'true' ) ## Deferred open + only collective I/O 
+                #mpi_info.Set('cb_nodes' , str(int(round(1*self.n_ranks))) )
                 ##
                 kwargs['info'] = mpi_info
                 self.mpi_info = mpi_info
         
         ## | rdcc_nbytes:
         ## | ------------
         ## | Integer setting the total size of the raw data chunk cache for this dataset in bytes.
         ## | In most cases increasing this number will improve performance, as long as you have 
         ## | enough free memory. The default size is 1 MB
         
         ## --> gets passed to H5Pset_chunk_cache
         if ('rdcc_nbytes' not in kwargs):
-            kwargs['rdcc_nbytes'] = int(16*1024**2) ## 16 [MB]
+            kwargs['rdcc_nbytes'] = int(32*1024**2) ## 32 [MB]
+            #kwargs['rdcc_nbytes'] = int(16*1024**2) ## 16 [MB]
         
         ## | rdcc_nslots:
         ## | ------------
         ## | Integer defining the number of chunk slots in the raw data chunk cache for this dataset.
         
         ## if ('rdcc_nslots' not in kwargs):
         ##     kwargs['rdcc_nslots'] = 521
         
         ## cgd() unique kwargs (not h5py.File kwargs) --> pop() rather than get()
         verbose = kwargs.pop('verbose',False)
         force   = kwargs.pop('force',False)
         
+        # === initialize file on FS
+        
+        ## if file open mode is 'w', the file exists, and force is False
+        ## --> raise error
         if (self.open_mode == 'w') and (force is False) and os.path.isfile(self.fname):
             if (self.rank==0):
                 print('\n'+72*'-')
                 print(self.fname+' already exists! opening with \'w\' would overwrite.\n')
                 openModeInfoStr = '''
                                   r       --> Read only, file must exist
                                   r+      --> Read/write, file must exist
@@ -178,38 +196,29 @@
                 print(textwrap.indent(textwrap.dedent(openModeInfoStr), 2*' ').strip('\n'))
                 print(72*'-'+'\n')
             
             if (self.comm is not None):
                 self.comm.Barrier()
             raise FileExistsError()
         
-        ## remove file, touch, stripe
-        elif (self.open_mode == 'w') and (force is True) and os.path.isfile(self.fname):
+        ## if file open mode is 'w', the file exists, and force is True
+        ## --> delete, touch, chmod, stripe
+        if (self.open_mode == 'w') and (force is True) and os.path.isfile(self.fname):
             if (self.rank==0):
                 os.remove(self.fname)
                 Path(self.fname).touch()
+                os.chmod(self.fname, int('640', base=8))
                 if shutil.which('lfs') is not None:
-                    return_code = subprocess.call('lfs migrate --stripe-count 16 --stripe-size 16M %s > /dev/null 2>&1'%self.fname, shell=True)
-                else:
-                    #print('striping with lfs not permitted on this filesystem')
-                    pass
-        
-        ## touch, stripe
-        elif (self.open_mode == 'w') and not os.path.isfile(self.fname):
-            if (self.rank==0):
-                Path(self.fname).touch()
-                if shutil.which('lfs') is not None:
-                    return_code = subprocess.call('lfs migrate --stripe-count 16 --stripe-size 16M %s > /dev/null 2>&1'%self.fname, shell=True)
+                    return_code = subprocess.call(f'lfs migrate --stripe-count 16 --stripe-size 16M {self.fname} > /dev/null 2>&1', shell=True)
+                    if (return_code != 0):
+                        raise ValueError('lfs migrate failed')
                 else:
                     #print('striping with lfs not permitted on this filesystem')
                     pass
         
-        else:
-            pass
-        
         if (self.comm is not None):
             self.comm.Barrier()
         
         ## call actual h5py.File.__init__()
         super(cgd, self).__init__(*args, **kwargs)
         self.get_header(verbose=verbose, read_grid=read_grid)
     
@@ -777,15 +786,15 @@
                     if verbose: print('broadcasted y')
                 
                 if ( hf_eas4.gmode_dim3==5 ) and ( z.shape != (nx,ny,nz) ):
                     z = np.broadcast_to(z, (nx,ny,nz))
                     if verbose: print('broadcasted z')
             
             shape  = (nz,ny,nx)
-            chunks = rgd.chunk_sizer(nxi=shape, constraint=(None,None,None), size_kb=chunk_kb, base=2, data_byte=8)
+            chunks = h5_chunk_sizer(nxi=shape, constraint=(None,None,None), size_kb=chunk_kb, base=4, itemsize=8)
             
             # === write coord arrays
             
             if ('dims/x' in self):
                 del self['dims/x']
             if ('dims/y' in self):
                 del self['dims/y']
@@ -993,15 +1002,15 @@
                 ## 1D
                 #self.create_dataset('dims/x', data=x)
                 #self.create_dataset('dims/y', data=y)
                 #self.create_dataset('dims/z', data=z)
                 
                 ## 3D
                 shape  = (nz,ny,nx)
-                chunks = rgd.chunk_sizer(nxi=shape, constraint=(None,None,None), size_kb=chunk_kb, base=2, data_byte=8)
+                chunks = h5_chunk_sizer(nxi=shape, constraint=(None,None,None), size_kb=chunk_kb, base=4, itemsize=8)
                 
                 ## if (x is not None) and (y is not None) and (z is not None):
                 ##     if self.usingmpi: self.comm.Barrier()
                 ##     t_start = timeit.default_timer()
                 ##     dset = self.create_dataset('dims/x', data=x.T, shape=shape, chunks=chunks)
                 ##     dset = self.create_dataset('dims/y', data=y.T, shape=shape, chunks=chunks)
                 ##     dset = self.create_dataset('dims/z', data=z.T, shape=shape, chunks=chunks)
@@ -1317,15 +1326,15 @@
         
         # === initialize datasets
         for scalar in self.scalars:
             if verbose:
                 even_print('initializing data/%s'%(scalar,),'%0.2f [GB]'%(data_gb,))
             
             shape  = (self.nt,self.nz,self.ny,self.nx)
-            chunks = rgd.chunk_sizer(nxi=shape, constraint=(1,None,None,None), size_kb=chunk_kb, base=2)
+            chunks = h5_chunk_sizer(nxi=shape, constraint=(1,None,None,None), size_kb=chunk_kb, base=4, itemsize=4)
             
             dset = self.create_dataset('data/%s'%scalar, 
                                        shape=shape, 
                                        dtype=np.float32,
                                        chunks=chunks)
             
             chunk_kb_ = np.prod(dset.chunks)*4 / 1024. ## actual
@@ -2006,15 +2015,15 @@
                         raise ValueError
                     dtype = np.dtype(np.float32)
                     float_bytes = dtype.itemsize
                 else:
                     raise ValueError
                 
                 shape  = (nz,ny,nx)
-                chunks = rgd.chunk_sizer(nxi=shape, constraint=(None,None,None), size_kb=chunk_kb, base=2, data_byte=float_bytes)
+                chunks = h5_chunk_sizer(nxi=shape, constraint=(None,None,None), size_kb=chunk_kb, base=4, itemsize=float_bytes)
                 
                 dset = hf_tgt.create_dataset( 'dims/x', 
                                               shape=shape, 
                                               dtype=dtype,
                                               chunks=chunks )
                 
                 dset = hf_tgt.create_dataset( 'dims/y', 
@@ -2057,26 +2066,23 @@
                 # ===
                 
                 ## time 'chunks' split (number of timesteps to read / write at a time)
                 ctl_ = np.array_split(tfi,ct)
                 ctl = [[b[0],b[-1]+1] for b in ctl_ ]
                 
                 shape  = (nt,nz,ny,nx) ## target
-                #chunks = cgd.chunk_sizer(nxi=shape, constraint=(1,None,None,None), size_kb=chunk_kb, base=2)
-                
                 hf_tgt.scalars = []
-                #data_gb = 4*nx*ny*nz*nt / 1024**3
                 
                 ## initialize scalar datasets
                 t_start = timeit.default_timer()
                 for scalar in hf_src.scalars:
                     
                     dtype = hf_src.scalars_dtypes_dict[scalar]
                     float_bytes = dtype.itemsize
-                    chunks = rgd.chunk_sizer(nxi=shape, constraint=(1,None,None,None), size_kb=chunk_kb, base=2, data_byte=float_bytes)
+                    chunks = h5_chunk_sizer(nxi=shape, constraint=(1,None,None,None), size_kb=chunk_kb, base=4, itemsize=float_bytes)
                     data_gb = float_bytes * nx * ny * nz * nt / 1024**3
                     
                     if (scalar in scalars):
                         if verbose:
                             even_print('initializing data/%s'%(scalar,),'%0.1f [GB]'%(data_gb,))
                         dset = hf_tgt.create_dataset('data/%s'%scalar,
                                                        shape=shape,
@@ -2370,15 +2376,15 @@
         # self.x = x
         # self.y = y
         # self.z = z
         
         # === write coord arrays
         
         shape  = (nz,ny,nx)
-        chunks = rgd.chunk_sizer(nxi=shape, constraint=(None,None,None), size_kb=chunk_kb, base=2, data_byte=8)
+        chunks = h5_chunk_sizer(nxi=shape, constraint=(None,None,None), size_kb=chunk_kb, base=4, itemsize=8)
         
         # === write coordinate datasets (independent)
         
         # dset = self.create_dataset('dims/x', data=x.T, shape=shape, chunks=chunks)
         # dset = self.create_dataset('dims/y', data=y.T, shape=shape, chunks=chunks)
         # dset = self.create_dataset('dims/z', data=z.T, shape=shape, chunks=chunks)
         
@@ -2441,15 +2447,15 @@
         if self.usingmpi: self.comm.Barrier()
         t_delta = timeit.default_timer() - t_start
         if verbose: even_print('write: dims/z','%0.2f [GB]  %0.3f [s]  %0.3f [GB/s]'%(data_gb,t_delta,(data_gb/t_delta)))
         
         # ===
         
         shape  = (self.nt,self.nz,self.ny,self.nx)
-        chunks = rgd.chunk_sizer(nxi=shape, constraint=(1,None,None,None), size_kb=chunk_kb, base=2, data_byte=4)
+        chunks = h5_chunk_sizer(nxi=shape, constraint=(1,None,None,None), size_kb=chunk_kb, base=4, itemsize=4)
         
         ## initialize
         data_gb = 4*nx*ny*nz*nt / 1024.**3
         for scalar in ['u','v','w']:
             if ('data/%s'%scalar in self):
                 del self['data/%s'%scalar]
             if verbose:
@@ -2677,15 +2683,15 @@
             
             if verbose: print(72*'-')
             
             # === initialize mean datasets
             for scalar in self.scalars:
                 
                 shape  = (1,self.nz,self.ny,self.nx)
-                chunks = rgd.chunk_sizer(nxi=shape, constraint=(1,None,None,None), size_kb=chunk_kb, base=2)
+                chunks = h5_chunk_sizer(nxi=shape, constraint=(1,None,None,None), size_kb=chunk_kb, base=4, itemsize=4)
                 
                 if reynolds:
                     
                     ## do the Re mean of all scalars in file, regardless whether explicitly in scalars_re or not
                     #if scalar in scalars_re:
                     if True:
                         
@@ -2702,14 +2708,15 @@
                         
                         chunk_kb_ = np.prod(dset.chunks)*4 / 1024. ## actual
                         if verbose:
                             even_print('chunk shape (t,z,y,x)','%s'%str(dset.chunks))
                             even_print('chunk size','%i [KB]'%int(round(chunk_kb_)))
                 
                 if favre:
+                    
                     if (scalar in scalars_fv):
                         if ('data/%s_fv'%scalar in hf_mean):
                             del hf_mean['data/%s_fv'%scalar]
                         if (self.rank==0):
                             even_print('initializing data/%s_fv'%(scalar,),'%0.3f [GB]'%(data_gb_mean,))
                         dset = hf_mean.create_dataset('data/%s_fv'%scalar,
                                                       shape=shape,
@@ -2724,14 +2731,15 @@
                             even_print('chunk size','%i [KB]'%int(round(chunk_kb_)))
             
             if self.usingmpi: self.comm.Barrier()
             if verbose: print(72*'-')
             
             # === read rho
             if favre:
+                
                 dset = self['data/rho']
                 if self.usingmpi: self.comm.Barrier()
                 t_start = timeit.default_timer()
                 if self.usingmpi: 
                     with dset.collective:
                         #rho = dset[:,rz1:rz2,ry1:ry2,rx1:rx2].T
                         rho = dset[ti_min:,rz1:rz2,ry1:ry2,rx1:rx2].T
@@ -2841,15 +2849,14 @@
         if verbose: print(72*'-')
         if verbose: even_print('time read',format_time_string(t_read))
         if verbose: even_print('time write',format_time_string(t_write))
         if verbose: even_print(fn_cgd_mean, '%0.2f [GB]'%(os.path.getsize(fn_cgd_mean)/1024**3))
         if verbose: even_print('read total avg', '%0.2f [GB]  %0.3f [s]  %0.3f [GB/s]'%(data_gb_read,t_read,(data_gb_read/t_read)))
         if verbose: even_print('write total avg', '%0.2f [GB]  %0.3f [s]  %0.3f [GB/s]'%(data_gb_write,t_write,(data_gb_write/t_write)))
         if verbose: print(72*'-')
-        #if verbose: print('\n'+72*'-')
         if verbose: print('total time : cgd.get_mean() : %s'%format_time_string((timeit.default_timer() - t_start_func)))
         if verbose: print(72*'-')
         return
     
     def add_mean_dimensional_data_xpln(self, **kwargs):
         '''
         get dimensionalized mean data for [x]/[s1] plane
@@ -2901,15 +2908,15 @@
         if verbose: even_print('nx','%i'%self.nx)
         if verbose: even_print('ny','%i'%self.ny)
         if verbose: even_print('nz','%i'%self.nz)
         if verbose: even_print('nt','%i'%self.nt)
         if verbose: even_print('ngp','%0.1f [M]'%(self.ngp/1e6,))
         if verbose: print(72*'-')
         
-        ## read in 3D coordinate arrays, then dimensinoalize [m]
+        ## read in 3D coordinate arrays, then dimensionalize [m]
         x = np.copy( self['dims/x'][()].T * self.lchar )
         y = np.copy( self['dims/y'][()].T * self.lchar )
         z = np.copy( self['dims/z'][()].T * self.lchar )
         nx = self.nx
         ny = self.ny
         nz = self.nz
         
@@ -3160,14 +3167,16 @@
                                              u_edge=u1_edge,
                                              nu_wall=nu_wall,
                                             )
         
         # === add to file
         
         gn = 'data_dim'
+        
+        ## if group already exists, delete it entirely
         if (gn in self):
             del self[gn]
         
         ## 1D
         self.create_dataset(f'{gn}/psvel' , data=psvel, chunks=None)
         self.create_dataset(f'{gn}/utang' , data=utang, chunks=None)
         self.create_dataset(f'{gn}/rho'   , data=rho,   chunks=None)
@@ -3207,16 +3216,15 @@
         self.create_dataset(f'{gn}/sc_l_out'   , data=sc_l_out   , chunks=None)
         self.create_dataset(f'{gn}/sc_t_out'   , data=sc_t_out   , chunks=None)
         
         ## add integrated quantities (all 0D)
         for key,val in dd.items():
             self.create_dataset(f'{gn}/{key}', data=val, chunks=None)
         
-        # === report
-        
+        ## report
         if verbose:
             print(72*'-')
             even_print('Re_τ'                      , '%0.1f'%dd['Re_tau']            )
             even_print('Re_θ'                      , '%0.1f'%dd['Re_theta']          )
             even_print('θ'                         , '%0.5e [m]'%dd['theta_cmp']     )
             even_print('δ*'                        , '%0.5e [m]'%dd['dstar_cmp']     )
             even_print('H12'                       , '%0.5f'%dd['H12']               )
@@ -3419,28 +3427,29 @@
         
         # ===
         
         comm_cgd_prime = MPI.COMM_WORLD
         
         with cgd(fn_cgd_prime, 'w', force=force, driver=self.driver, comm=self.comm) as hf_prime:
             
-            ## initialize CGD file
+            ## initialize prime cgd from cgd
             hf_prime.init_from_cgd(self.fname, rx=rx,ry=ry,rz=rz, chunk_kb=chunk_kb)
             
             ## add top-level attributes
             #hf_prime.attrs['fclass'] = 'cgd'
             hf_prime.attrs['fsubtype'] = 'prime'
             
             #shape  = (self.nt,self.nz,self.ny,self.nx)
             shape  = (nt_prime,self.nz,self.ny,self.nx)
-            chunks = rgd.chunk_sizer(nxi=shape, constraint=(1,None,None,None), size_kb=chunk_kb, base=2)
+            chunks = h5_chunk_sizer(nxi=shape, constraint=(1,None,None,None), size_kb=chunk_kb, base=4, itemsize=4)
             
             # === initialize prime datasets + rho
             
             if copy_rho:
+                
                 if verbose:
                     even_print('initializing data/rho','%0.1f [GB]'%(data_gb,))
                 dset = hf_prime.create_dataset('data/rho',
                                                shape=shape,
                                                dtype=np.float32,
                                                chunks=chunks)
                 
@@ -3909,43 +3918,46 @@
                     print('rank %04d : rx1=%i rx2=%i ry1=%i ry2=%i rz1=%i rz2=%i'%(self.rank, rx1,rx2, ry1,ry2, rz1,rz2))
                     sys.stdout.flush()
         
         if self.usingmpi: self.comm.Barrier()
         
         # ===
         
+        dtype = self['data/u'].dtype
+        itemsize = dtype.itemsize
+        
         data_gb = 4*self.nx*self.ny*self.nz*self.nt / 1024**3
         
         shape  = (self.nt,self.nz,self.ny,self.nx)
-        chunks = rgd.chunk_sizer(nxi=shape, constraint=(1,None,None,None), size_kb=chunk_kb, base=2)
+        chunks = h5_chunk_sizer(nxi=shape, constraint=(1,None,None,None), size_kb=chunk_kb, base=4, itemsize=itemsize)
         
         # === initialize 4D arrays in HDF5
         
         if save_lambda2:
             if verbose: even_print('initializing data/lambda2','%0.2f [GB]'%(data_gb,))
             if ('data/lambda2' in self):
                 del self['data/lambda2']
             dset = self.create_dataset('data/lambda2', 
                                         shape=shape, 
-                                        dtype=self['data/u'].dtype,
+                                        dtype=dtype,
                                         chunks=chunks,
                                         )
             
             chunk_kb_ = np.prod(dset.chunks)*4 / 1024. ## actual
             if verbose:
                 even_print('chunk shape (t,z,y,x)','%s'%str(dset.chunks))
                 even_print('chunk size','%i [KB]'%int(round(chunk_kb_)))
         
         if save_Q:
             if verbose: even_print('initializing data/Q','%0.2f [GB]'%(data_gb,))
             if ('data/Q' in self):
                 del self['data/Q']
             dset = self.create_dataset('data/Q', 
                                         shape=shape, 
-                                        dtype=self['data/u'].dtype,
+                                        dtype=dtype,
                                         chunks=chunks,
                                         )
             
             chunk_kb_ = np.prod(dset.chunks)*4 / 1024. ## actual
             if verbose:
                 even_print('chunk shape (t,z,y,x)','%s'%str(dset.chunks))
                 even_print('chunk size','%i [KB]'%int(round(chunk_kb_)))
@@ -4450,15 +4462,15 @@
         #vtang = np.broadcast_to(vtang[:,:,np.newaxis,np.newaxis,:], (nxr,nyr,nzr,1,2))
         #vnorm = np.broadcast_to(vnorm[:,:,np.newaxis,np.newaxis,:], (nxr,nyr,nzr,1,2))
         
         # ===
         
         data_gb = 4*self.nx*self.ny*self.nz*self.nt / 1024**3
         shape  = (self.nt,self.nz,self.ny,self.nx)
-        chunks = rgd.chunk_sizer(nxi=shape, constraint=(1,None,None,None), size_kb=chunk_kb, base=2, data_byte=4)
+        chunks = h5_chunk_sizer(nxi=shape, constraint=(1,None,None,None), size_kb=chunk_kb, base=4, itemsize=4)
         
         for scalar in ['utang','unorm']:
             
             if verbose:
                 even_print(f'initializing data/{scalar}','%0.1f [GB]'%(data_gb,))
             if (f'data/{scalar}' in self):
                 del self[f'data/{scalar}']
@@ -4728,21 +4740,40 @@
             if (t4d[0]!=0):
                 rx1, rx2 = rx1-n_overlap, rx2
                 xA += n_overlap
                 xB += n_overlap
             if (t4d[0]!=rx-1):
                 rx1, rx2 = rx1, rx2+n_overlap
             
-            ## overlap in [y]
+            ## ## overlap in [y]
+            ## if (t4d[1]!=0):
+            ##     ry1, ry2 = ry1-n_overlap, ry2
+            ##     yA += n_overlap
+            ##     yB += n_overlap
+            ## if (t4d[1]!=ry-1):
+            ##     ry1, ry2 = ry1, ry2+n_overlap
+            
+            ## overlap in [y] --> TODO: needs checking
             if (t4d[1]!=0):
-                ry1, ry2 = ry1-n_overlap, ry2
+                ry1 = ry1-n_overlap
+                #ry2 = ry2
                 yA += n_overlap
                 yB += n_overlap
             if (t4d[1]!=ry-1):
-                ry1, ry2 = ry1, ry2+n_overlap
+                #ry1 = ry1
+                ry2 = min(ry2+n_overlap,self.ny)
+            
+            if (ry2>self.ny):
+                #raise IndexError
+                print('ry2>self.ny')
+                self.comm.Abort(1)
+            if (ry1<0):
+                #raise IndexError
+                print('ry1<0')
+                self.comm.Abort(1)
             
             ## overlap in [z]
             if (t4d[2]!=0):
                 rz1, rz2 = rz1-n_overlap, rz2
                 zA += n_overlap
                 zB += n_overlap
             if (t4d[2]!=rz-1):
@@ -4774,15 +4805,15 @@
         # vtang = np.broadcast_to(vtang[:,:,np.newaxis,:], (nxr,nyr,nzr,2))
         # vnorm = np.broadcast_to(vnorm[:,:,np.newaxis,:], (nxr,nyr,nzr,2))
         
         # ===
         
         data_gb = 4*self.nx*self.ny*self.nz*self.nt / 1024**3
         shape  = (self.nt,self.nz,self.ny,self.nx)
-        chunks = rgd.chunk_sizer(nxi=shape, constraint=(1,None,None,None), size_kb=chunk_kb, base=2, data_byte=4)
+        chunks = h5_chunk_sizer(nxi=shape, constraint=(1,None,None,None), size_kb=chunk_kb, base=4, itemsize=4)
         
         # === initialize 4D arrays in HDF5
         
         for dsn in ['vort_x','vort_y','vort_z']:
             if verbose: even_print(f'initializing data/{dsn}','%0.2f [GB]'%(data_gb,))
             if (f'data/{dsn}' in self):
                 del self[f'data/{dsn}']
@@ -5236,14 +5267,15 @@
         
         # === extend the rank ranges (spatial range overlap)
         
         if self.usingmpi:
             
             n_overlap = stencil_npts_one_side + 3
             
+            ## default start:end indices for local-->global write
             xA = 0
             xB = nxr
             yA = 0
             yB = nyr
             zA = 0
             zB = nzr
             
@@ -5256,21 +5288,40 @@
             if (t4d[0]!=0):
                 rx1, rx2 = rx1-n_overlap, rx2
                 xA += n_overlap
                 xB += n_overlap
             if (t4d[0]!=rx-1):
                 rx1, rx2 = rx1, rx2+n_overlap
             
-            ## overlap in [y]
+            ## ## overlap in [y]
+            ## if (t4d[1]!=0):
+            ##     ry1, ry2 = ry1-n_overlap, ry2
+            ##     yA += n_overlap
+            ##     yB += n_overlap
+            ## if (t4d[1]!=ry-1):
+            ##     ry1, ry2 = ry1, ry2+n_overlap
+            
+            ## overlap in [y] --> TODO: needs checking
             if (t4d[1]!=0):
-                ry1, ry2 = ry1-n_overlap, ry2
+                ry1 = ry1-n_overlap
+                #ry2 = ry2
                 yA += n_overlap
                 yB += n_overlap
             if (t4d[1]!=ry-1):
-                ry1, ry2 = ry1, ry2+n_overlap
+                #ry1 = ry1
+                ry2 = min(ry2+n_overlap,self.ny)
+            
+            if (ry2>self.ny):
+                #raise IndexError
+                print('ry2>self.ny')
+                self.comm.Abort(1)
+            if (ry1<0):
+                #raise IndexError
+                print('ry1<0')
+                self.comm.Abort(1)
             
             ## overlap in [z]
             if (t4d[2]!=0):
                 rz1, rz2 = rz1-n_overlap, rz2
                 zA += n_overlap
                 zB += n_overlap
             if (t4d[2]!=rz-1):
@@ -5285,45 +5336,56 @@
         if self.usingmpi and False:
             for ri in range(self.n_ranks):
                 self.comm.Barrier()
                 if (self.rank == ri):
                     print('rank %04d : rx1=%i rx2=%i ry1=%i ry2=%i rz1=%i rz2=%i'%(self.rank, rx1,rx2, ry1,ry2, rz1,rz2))
                     sys.stdout.flush()
         
+        #time.sleep(1)
+        #if verbose: print('')
         if self.usingmpi: self.comm.Barrier()
         
         # ===
         
         dset = self['dims/snorm']
         snorm = np.copy( dset[ry1:ry2] )
         
-        ## read rank-local tang/norm basis vectos vtang & vnorm
+        ## read rank-local tang/norm basis vectors vtang & vnorm
         dset = self['csys/vtang']
         vtang = np.copy( dset[rx1:rx2,ry1:ry2,:] )
         dset = self['csys/vnorm']
         vnorm = np.copy( dset[rx1:rx2,ry1:ry2,:] )
         
         ## convert vtang,vnorm (nx,ny,2) --> (nx,ny,nz,3)
         vtang3d = np.zeros((nxr,nyr,nzr,3), dtype=np.float64)
         vnorm3d = np.zeros((nxr,nyr,nzr,3), dtype=np.float64)
         vspan3d = np.zeros((nxr,nyr,nzr,3), dtype=np.float64)
         
         vtang3d[:,:,:,:2] = vtang[:,:,np.newaxis,:]
         vnorm3d[:,:,:,:2] = vnorm[:,:,np.newaxis,:]
         vspan3d[:,:,:,-1] = 1.
         
+        if self.usingmpi: self.comm.Barrier()
+        
         # ===
         
         data_gb = 4*self.nx*self.ny*self.nz*self.nt / 1024**3
         shape  = (self.nt,self.nz,self.ny,self.nx)
-        chunks = rgd.chunk_sizer(nxi=shape, constraint=(1,None,None,None), size_kb=chunk_kb, base=2, data_byte=4)
+        
+        constraint = (1,None,None,None)
+        base = 4
+        
+        # constraint = (None,-1,1,-1)
+        # base = 64
+        
+        chunks = h5_chunk_sizer(nxi=shape, constraint=constraint, size_kb=chunk_kb, base=base, itemsize=4)
         
         # === initialize 4D arrays in HDF5
         
-        for dsn in ['vort_tang']: #, 'vort_tang_bak']:
+        for dsn in ['vort_tang']:
             if verbose: even_print(f'initializing data/{dsn}','%0.2f [GB]'%(data_gb,))
             if (f'data/{dsn}' in self):
                 del self[f'data/{dsn}']
             dset = self.create_dataset( f'data/{dsn}',
                                         shape=shape,
                                         dtype=np.float32,
                                         chunks=chunks,
@@ -5791,24 +5853,25 @@
         if verbose: even_print('nx','%i'%self.nx)
         if verbose: even_print('ny','%i'%self.ny)
         if verbose: even_print('nz','%i'%self.nz)
         if verbose: even_print('nt','%i'%self.nt)
         if verbose: even_print('ngp','%0.1f [M]'%(self.ngp/1e6,))
         if verbose: print(72*'-')
         
+        ## 0D scalars
         lchar   = self.lchar   ; data['lchar']   = lchar
         U_inf   = self.U_inf   ; data['U_inf']   = U_inf
         rho_inf = self.rho_inf ; data['rho_inf'] = rho_inf
         T_inf   = self.T_inf   ; data['T_inf']   = T_inf
         
         #data['M_inf'] = self.M_inf
         data['Ma'] = self.Ma
         data['Pr'] = self.Pr
         
-        ## read in 3D coordinate arrays, then dimensinoalize [m]
+        ## read in 3D coordinate arrays, then dimensionalize [m]
         ## every ranks gets full grid
         x = np.copy( self['dims/x'][()].T * self.lchar )
         y = np.copy( self['dims/y'][()].T * self.lchar )
         z = np.copy( self['dims/z'][()].T * self.lchar )
         
         nx = self.nx ; data['nx'] = nx
         ny = self.ny ; data['ny'] = ny
@@ -6363,18 +6426,16 @@
                 else:
                     if verbose: even_print(dsn,'not found')
             
             if verbose: print(72*'-')
             
             ## initialize datasets
             data_gb = (self.nx * self.nz) * 4 / 1024**3
-            #shape  = (self.nt,self.nz,self.nx)
-            #chunks = rgd.chunk_sizer(nxi=shape, constraint=(1,None,None), size_kb=chunk_kb, base=2, data_byte=4)
             shape  = (self.nx,self.nz,self.nt)
-            chunks = rgd.chunk_sizer(nxi=shape, constraint=(None,None,1), size_kb=chunk_kb, base=2, data_byte=4)
+            chunks = h5_chunk_sizer(nxi=shape, constraint=(None,None,1), size_kb=chunk_kb, base=4, itemsize=4)
             
             scalars_spd = [ 'tau_u1_s2', 'tau_u3_s2', 'T','rho','mu','nu','u_tau','p' ]
             
             for scalar in scalars_spd:
                 
                 if verbose:
                     even_print(f'initializing data/{scalar}','%0.1f [GB]'%(data_gb,))
@@ -6791,15 +6852,15 @@
                 dsn = f'data/{scalar}'
                 dset = self[dsn]
                 dtype = dset.dtype
                 float_bytes = dtype.itemsize
                 
                 #shape  = (self.ny,self.nz,self.nt)
                 shape  = (ni,nj,nt)
-                chunks = rgd.chunk_sizer(nxi=shape, constraint=(None,None,1), size_kb=chunk_kb, base=2, data_byte=float_bytes)
+                chunks = h5_chunk_sizer(nxi=shape, constraint=(None,None,1), size_kb=chunk_kb, base=4, itemsize=float_bytes)
                 
                 data_gb = np.prod(shape) * float_bytes / 1024**3
                 
                 if verbose:
                     even_print(f'initializing {dsn}','%0.1f [GB]'%(data_gb,))
                 if (dsn in hfspd):
                     del hfspd[dsn]
@@ -6877,14 +6938,328 @@
         
         if verbose: print(72*'-')
         if verbose: print('total time : turbx.export_polydata_xpln() : %s'%format_time_string((timeit.default_timer() - t_start_func)))
         if verbose: print(72*'-')
         
         return
     
+    def export_polydata_zpln(self, fn_spd=None, **kwargs):
+        '''
+        get 2D [x,y] quantities of a reduced I/O volume which is thin in the [z]/[s3] direction
+        and export structured polydata (SPD) file
+        '''
+        
+        if (self.rank==0):
+            verbose = True
+        else:
+            verbose = False
+        
+        rx = kwargs.get('rx',1)
+        ry = kwargs.get('ry',1)
+        rz = kwargs.get('rz',1)
+        ct = kwargs.get('ct',1) ## n chunks [t]
+        
+        chunk_kb = kwargs.get('chunk_kb',4*1024) ## 4 [MB]
+        force    = kwargs.get('force',False)
+        
+        acc = kwargs.get('acc',4)
+        edge_stencil = kwargs.get('edge_stencil','full')
+        
+        if verbose: print('\n'+'cgd.export_polydata_zpln()'+'\n'+72*'-')
+        t_start_func = timeit.default_timer()
+        
+        ## check
+        if not ('data/utang' in self) and self.curvilinear:
+            raise ValueError('data/utang not in hdf5')
+        if not ('data/unorm' in self) and self.curvilinear:
+            raise ValueError('data/unorm not in hdf5')
+        if not ('dims/snorm' in self) and self.curvilinear:
+            raise ValueError('dims/snorm not in hdf5')
+        if not ('dims/stang' in self) and self.curvilinear:
+            raise ValueError('dims/stang not in hdf5')
+        
+        if (rx*ry*rz != self.n_ranks):
+            raise AssertionError('rx*ry*rz != self.n_ranks')
+        if (rz!=1):
+            raise AssertionError('rz!=1')
+        if (rx>self.nx):
+            raise AssertionError('rx>self.nx')
+        if (ry>self.ny):
+            raise AssertionError('ry>self.ny')
+        
+        if verbose: even_print('rx','%i'%rx)
+        if verbose: even_print('ry','%i'%ry)
+        if verbose: print(72*'-')
+        
+        ## get size of infile
+        fsize = os.path.getsize(self.fname)/1024**3
+        if verbose: even_print(os.path.basename(self.fname),'%0.1f [GB]'%fsize)
+        if verbose: even_print('nx','%i'%self.nx)
+        if verbose: even_print('ny','%i'%self.ny)
+        if verbose: even_print('nz','%i'%self.nz)
+        if verbose: even_print('nt','%i'%self.nt)
+        if verbose: even_print('ngp','%0.1f [M]'%(self.ngp/1e6,))
+        if verbose: print(72*'-')
+        
+        ## polydata file name (for writing)
+        if (fn_spd is None):
+            fname_path = os.path.dirname(self.fname)
+            fname_base = os.path.basename(self.fname)
+            fname_root, fname_ext = os.path.splitext(fname_base)
+            fname_spd_h5_base = fname_root+'_polydata.h5'
+            #fn_spd = os.path.join(fname_path, fname_spd_h5_base)
+            fn_spd = str(PurePosixPath(fname_path, fname_spd_h5_base))
+            #fn_spd = Path(fname_path, fname_spd_h5_base)
+        
+        # === ranks
+        
+        if self.usingmpi:
+            
+            comm4d = self.comm.Create_cart(dims=[rx,ry,rz], periods=[False,False,False], reorder=False)
+            t4d = comm4d.Get_coords(self.rank)
+            
+            rxl_ = np.array_split(np.arange(self.nx,dtype=np.int64),min(rx,self.nx))
+            ryl_ = np.array_split(np.arange(self.ny,dtype=np.int64),min(ry,self.ny))
+            rzl_ = np.array_split(np.arange(self.nz,dtype=np.int64),min(rz,self.nz))
+            #rtl_ = np.array_split(np.arange(self.nt,dtype=np.int64),min(rt,self.nt))
+            
+            rxl = [[b[0],b[-1]+1] for b in rxl_ ]
+            ryl = [[b[0],b[-1]+1] for b in ryl_ ]
+            rzl = [[b[0],b[-1]+1] for b in rzl_ ]
+            #rtl = [[b[0],b[-1]+1] for b in rtl_ ]
+            
+            rx1, rx2 = rxl[t4d[0]]; nxr = rx2 - rx1
+            ry1, ry2 = ryl[t4d[1]]; nyr = ry2 - ry1
+            rz1, rz2 = rzl[t4d[2]]; nzr = rz2 - rz1
+            #rt1, rt2 = rtl[t4d[3]]; ntr = rt2 - rt1
+        
+        else:
+            
+            nxr = self.nx
+            nyr = self.ny
+            nzr = self.nz
+            #ntr = self.nt
+        
+        ri1 = rx1
+        ri2 = rx2
+        rj1 = ry1
+        rj2 = ry2
+        
+        ## [t] chunks
+        ctl_ = np.array_split(np.arange(self.nt),min(ct,self.nt))
+        ctl  = [[b[0],b[-1]+1] for b in ctl_ ]
+        
+        data_gb = (self.ny * self.nz) * 4 / 1024**3
+        
+        ## get [snorm] or [y]
+        if ('dims/snorm' in self):
+            dset = self['dims/snorm']
+            snorm = np.copy( dset[ry1:ry2] )
+        else:
+            if self.rectilinear:
+                dset = self['dims/y']
+                snorm = np.copy( dset[0,ry1:ry2,0].T )
+            else:
+                raise ValueError
+        
+        ## get [stang] or [x]
+        if ('dims/stang' in self):
+            dset = self['dims/stang']
+            stang = np.copy( dset[rx1:rx2] )
+        else:
+            if self.rectilinear:
+                dset = self['dims/x']
+                stang = np.copy( dset[rx1:rx2,ry1:ry2,0].T )
+            else:
+                raise ValueError
+        
+        ## get middle-most [z] index
+        zi = self.nz // 2
+        
+        ## 3D polydata grid coordinates : shape (nx,ny,3)
+        xyz = np.zeros((self.nx, self.ny, 3))
+        xyz[:,:,0] = np.copy(self['dims/x'][zi,:,:]).T
+        xyz[:,:,1] = np.copy(self['dims/y'][zi,:,:]).T
+        xyz[:,:,2] = np.copy(self['dims/z'][zi,:,:]).T
+        
+        ## open & initialize polydata (SPD) file
+        if verbose: even_print('surface polydata (spd) .h5', fn_spd)
+        with spd(fn_spd, 'w', force=force, driver=self.driver, comm=MPI.COMM_WORLD) as hfspd:
+            
+            ## add attributes from CGD to SPD
+            ## this doesnt work because CGD does not use attributes for its metadata as of writing this func
+            # for key,val in self.attrs.items():
+            #     hfspd.attrs[key] = val
+            
+            ## add attributes from CGD to SPD
+            for key in self.udef:
+                hfspd.attrs[key] = self.udef[key]
+            #for key in self.udef_deriv:
+            #    hfspd.attrs[key] = self.udef_deriv[key]
+            
+            ## add time vector from CGD to SPD
+            dsn = f'dims/t'
+            if (dsn in hfspd):
+                del hfspd[dsn]
+            data = np.copy(self[dsn][()])
+            ds = hfspd.create_dataset(dsn, data=data, chunks=None) ## no transpose!
+            if verbose: even_print(dsn,'%s'%str(ds.shape))
+            
+            ## add 3D polydata grid coordinates : shape (nx,nz,3)
+            dsn = f'dims/xyz'
+            if (dsn in hfspd):
+                del hfspd[dsn]
+            ds = hfspd.create_dataset(dsn, data=xyz, chunks=None) ## no transpose!
+            if verbose: even_print(dsn,'%s'%str(ds.shape))
+            
+            ni = self.nx
+            nj = self.ny
+            nt = self.nt
+            hfspd.attrs['ni'] = ni
+            hfspd.attrs['nj'] = nj
+            hfspd.attrs['n_quads'] = ( ni - 1 ) * ( nj - 1 )
+            hfspd.attrs['n_pts'] = ni * nj
+            hfspd.attrs['nt'] = nt
+            
+            if verbose: print(72*'-')
+            hfspd.get_header(verbose=verbose)
+            if verbose: print(72*'-')
+            
+            ## add additional [dims/<>] dsets
+            for dsn in [ 'dims/stang', 'dims/snorm', 'dims/crv_R' ]:
+                if (dsn in self):
+                    if (dsn in hfspd):
+                        del hfspd[dsn]
+                    data = np.copy(self[dsn][()])
+                    
+                    if (data.shape==(self.nx,)):
+                        data = np.array( [data[xi] ], dtype=data.dtype )
+                        if (data.ndim!=1):
+                            raise ValueError
+                    
+                    ds = hfspd.create_dataset(dsn, data=data, chunks=None)
+                    if verbose: even_print(dsn,'%s'%str(ds.shape))
+                else:
+                    if verbose: even_print(dsn,'not found')
+            
+            ## add additional [csys/<>] dsets
+            for dsn in [ 'csys/vtang', 'csys/vnorm' ]:
+                if (dsn in self):
+                    if (dsn in hfspd):
+                        del hfspd[dsn]
+                    data = np.copy(self[dsn][xi,:,:])
+                    
+                    if (data.ndim!=3):
+                        data = data[np.newaxis,:,:]
+                    if (data.ndim!=3):
+                        raise ValueError
+                    
+                    ds = hfspd.create_dataset(dsn, data=data, chunks=None)
+                    if verbose: even_print(dsn,'%s'%str(ds.shape))
+                else:
+                    if verbose: even_print(dsn,'not found')
+            
+            if verbose: print(72*'-')
+            
+            ## initialize datasets
+            for scalar in self.scalars:
+                
+                dsn = f'data/{scalar}'
+                dset = self[dsn]
+                dtype = dset.dtype
+                float_bytes = dtype.itemsize
+                
+                #shape  = (self.ny,self.nz,self.nt)
+                shape  = (ni,nj,nt)
+                chunks = h5_chunk_sizer(nxi=shape, constraint=(None,None,1), size_kb=chunk_kb, base=4, itemsize=float_bytes)
+                
+                data_gb = np.prod(shape) * float_bytes / 1024**3
+                
+                if verbose:
+                    even_print(f'initializing {dsn}','%0.1f [GB]'%(data_gb,))
+                if (dsn in hfspd):
+                    del hfspd[dsn]
+                dset = hfspd.create_dataset( dsn,
+                                             shape=shape,
+                                             dtype=dtype,
+                                             chunks=chunks )
+                
+                chunk_kb_ = np.prod(dset.chunks)*4 / 1024. ## actual
+                if verbose:
+                    even_print('chunk shape (i,j,t)','%s'%str(dset.chunks))
+                    even_print('chunk size','%i [KB]'%int(round(chunk_kb_)))
+        
+        if verbose: print(72*'-')
+        
+        # === main loop
+        
+        data_gb_read  = 0.
+        data_gb_write = 0.
+        t_read  = 0.
+        t_write = 0.
+        
+        with spd(fn_spd, 'a', driver=self.driver, comm=MPI.COMM_WORLD) as hfspd:
+            
+            if verbose:
+                progress_bar = tqdm(total=ct*self.n_scalars, ncols=100, desc='export spd', leave=False, file=sys.stdout)
+            
+            for scalar in self.scalars:
+                
+                dsn = f'data/{scalar}'
+                
+                dset_src = self[dsn]
+                dset_tgt = hfspd[dsn]
+                
+                dtype = dset_src.dtype
+                float_bytes = dtype.itemsize
+                
+                for ctl_ in ctl:
+                    ct1, ct2 = ctl_
+                    ntc = ct2 - ct1
+                    
+                    ## read
+                    self.comm.Barrier()
+                    t_start = timeit.default_timer()
+                    with dset_src.collective:
+                        data = np.copy( dset_src[ct1:ct2,zi,ry1:ry2,rx1:rx2].T )
+                    self.comm.Barrier()
+                    t_delta = timeit.default_timer() - t_start
+                    data_gb = float_bytes * ni * nj * ntc / 1024**3
+                    
+                    t_read       += t_delta
+                    data_gb_read += data_gb
+                    
+                    if verbose:
+                        tqdm.write(even_print(f'read: {scalar}', '%0.3f [GB]  %0.3f [s]  %0.3f [GB/s]'%(data_gb,t_delta,(data_gb/t_delta)), s=True))
+                    
+                    ## write
+                    hfspd.comm.Barrier()
+                    t_start = timeit.default_timer()
+                    with dset_tgt.collective:
+                        dset_tgt[ri1:ri2,rj1:rj2,ct1:ct2] = data
+                    hfspd.comm.Barrier()
+                    t_delta = timeit.default_timer() - t_start
+                    data_gb = float_bytes * ni * nj * ntc / 1024**3
+                    
+                    t_write       += t_delta
+                    data_gb_write += data_gb
+                    
+                    if verbose:
+                        tqdm.write(even_print(f'write: {scalar}', '%0.3f [GB]  %0.3f [s]  %0.3f [GB/s]'%(data_gb,t_delta,(data_gb/t_delta)), s=True))
+                    
+                    if verbose: progress_bar.update()
+            
+            if verbose: progress_bar.close()
+        
+        if verbose: print(72*'-')
+        if verbose: print('total time : turbx.export_polydata_zpln() : %s'%format_time_string((timeit.default_timer() - t_start_func)))
+        if verbose: print(72*'-')
+        
+        return
+    
     # ===
     
     def check_grid_validity_z(self,):
         '''
         check grid validity for CGD file (in [z] direction)
         - monotonically increasing
         - no Δ=0
@@ -7359,15 +7734,15 @@
     │
     └-─ data/<<scalar>> --> 4D [t,z,y,x]
     
     '''
     
     def __init__(self, *args, **kwargs):
         
-        self.fname, openMode = args
+        self.fname, self.open_mode = args
         
         self.fname_path = os.path.dirname(self.fname)
         self.fname_base = os.path.basename(self.fname)
         self.fname_root, self.fname_ext = os.path.splitext(self.fname_base)
         
         ## default to libver='latest' if none provided
         if ('libver' not in kwargs):
@@ -7389,67 +7764,85 @@
             self.n_ranks = self.comm.Get_size()
             self.rank    = self.comm.Get_rank()
         else:
             self.comm    = None
             self.n_ranks = 1
             self.rank    = 0
         
+        stripe_count   = kwargs.pop('stripe_count'   , 32 )
+        stripe_size_mb = kwargs.pop('stripe_size_mb' , 8  )
+        
         ## if not using MPI, remove 'driver' and 'comm' from kwargs
         if ( not self.usingmpi ) and ('driver' in kwargs):
             kwargs.pop('driver')
         if ( not self.usingmpi ) and ('comm' in kwargs):
             kwargs.pop('comm')
         
         ## | mpiexec --mca io romio321 -n $NP python3 ...
         ## | mpiexec --mca io ompio -n $NP python3 ...
         ## | ompi_info --> print ompi settings ('MCA io' gives io implementation options)
-        ## | export ROMIO_FSTYPE_FORCE="lustre:" --> force Lustre driver over UFS --> causes crash
+        ## | export ROMIO_FSTYPE_FORCE="lustre:" --> force Lustre driver over UFS when using romio --> causes crash
         ## | export ROMIO_FSTYPE_FORCE="ufs:"
         ## | export ROMIO_PRINT_HINTS=1 --> show available hints
         
-        ## determine MPI info / hints
+        ## https://doku.lrz.de/best-practices-hints-and-optimizations-for-io-10747318.html
+        
+        ## OMPIO
+        ## export OMPI_MCA_sharedfp=^lockedfile,individual
+        ## mpiexec --mca io ompio -n $NP python3 script.py
+        
+        ## set ROMIO hints, passed through 'mpi_info' dict
         if self.usingmpi:
             if ('info' in kwargs):
                 self.mpi_info = kwargs['info']
             else:
                 mpi_info = MPI.Info.Create()
                 ##
                 mpi_info.Set('romio_ds_write' , 'disable'   )
                 mpi_info.Set('romio_ds_read'  , 'disable'   )
                 mpi_info.Set('romio_cb_read'  , 'automatic' )
                 mpi_info.Set('romio_cb_write' , 'automatic' )
                 #mpi_info.Set('romio_cb_read'  , 'enable' )
                 #mpi_info.Set('romio_cb_write' , 'enable' )
                 mpi_info.Set('cb_buffer_size' , str(int(round(16*1024**2))) ) ## 16 [MB]
+                #mpi_info.Set('cb_buffer_size' , str(int(round(32*1024**2))) ) ## 32 [MB]
+                ##
+                #mpi_info.Set('romio_no_indep_rw' , 'true' ) ## Deferred open + only collective I/O 
+                #mpi_info.Set('cb_nodes' , str(int(round(1*self.n_ranks))) )
                 ##
                 kwargs['info'] = mpi_info
                 self.mpi_info = mpi_info
         
         ## | rdcc_nbytes:
         ## | ------------
         ## | Integer setting the total size of the raw data chunk cache for this dataset in bytes.
         ## | In most cases increasing this number will improve performance, as long as you have 
         ## | enough free memory. The default size is 1 MB
         
         ## --> gets passed to H5Pset_chunk_cache
         if ('rdcc_nbytes' not in kwargs):
+            #kwargs['rdcc_nbytes'] = int(32*1024**2) ## 32 [MB]
             kwargs['rdcc_nbytes'] = int(16*1024**2) ## 16 [MB]
         
         ## | rdcc_nslots:
         ## | ------------
         ## | Integer defining the number of chunk slots in the raw data chunk cache for this dataset.
         
         ## if ('rdcc_nslots' not in kwargs):
         ##     kwargs['rdcc_nslots'] = 521
         
         ## rgd() unique kwargs (not h5py.File kwargs) --> pop() rather than get()
         verbose = kwargs.pop('verbose',False)
         force   = kwargs.pop('force',False)
         
-        if (openMode == 'w') and (force is False) and os.path.isfile(self.fname):
+        # === initialize file on FS
+        
+        ## if file open mode is 'w', the file exists, and force is False
+        ## --> raise error
+        if (self.open_mode == 'w') and (force is False) and os.path.isfile(self.fname):
             if (self.rank==0):
                 print('\n'+72*'-')
                 print(self.fname+' already exists! opening with \'w\' would overwrite.\n')
                 openModeInfoStr = '''
                                   r       --> Read only, file must exist
                                   r+      --> Read/write, file must exist
                                   w       --> Create file, truncate if exists
@@ -7464,38 +7857,30 @@
                 print(textwrap.indent(textwrap.dedent(openModeInfoStr), 2*' ').strip('\n'))
                 print(72*'-'+'\n')
             
             if (self.comm is not None):
                 self.comm.Barrier()
             raise FileExistsError()
         
-        ## remove file, touch, stripe
-        elif (openMode == 'w') and (force is True) and os.path.isfile(self.fname):
+        ## if file open mode is 'w', the file exists, and force is True
+        ## --> delete, touch, chmod, stripe
+        if (self.open_mode == 'w') and (force is True) and os.path.isfile(self.fname):
             if (self.rank==0):
                 os.remove(self.fname)
                 Path(self.fname).touch()
+                os.chmod(self.fname, int('640', base=8))
                 if shutil.which('lfs') is not None:
-                    return_code = subprocess.call('lfs migrate --stripe-count 16 --stripe-size 16M %s > /dev/null 2>&1'%self.fname, shell=True)
+                    cmd_str_lfs_migrate = f'lfs migrate --stripe-count {stripe_count:d} --stripe-size {stripe_size_mb:d}M {self.fname} > /dev/null 2>&1'
+                    return_code = subprocess.call(cmd_str_lfs_migrate, shell=True)
+                    if (return_code != 0):
+                        raise ValueError('lfs migrate failed')
                 else:
                     #print('striping with lfs not permitted on this filesystem')
                     pass
         
-        ## touch, stripe
-        elif (openMode == 'w') and not os.path.isfile(self.fname):
-            if (self.rank==0):
-                Path(self.fname).touch()
-                if shutil.which('lfs') is not None:
-                    return_code = subprocess.call('lfs migrate --stripe-count 16 --stripe-size 16M %s > /dev/null 2>&1'%self.fname, shell=True)
-                else:
-                    #print('striping with lfs not permitted on this filesystem')
-                    pass
-        
-        else:
-            pass
-        
         if (self.comm is not None):
             self.comm.Barrier()
         
         ## call actual h5py.File.__init__()
         super(rgd, self).__init__(*args, **kwargs)
         self.get_header(verbose=verbose)
     
@@ -7524,24 +7909,35 @@
             if exception_type is not None:
                 print(72*'-')
         return super(rgd, self).__exit__()
     
     def get_header(self,**kwargs):
         '''
         initialize header attributes of RGD class instance
+        --> this gets called automatically upon opening the file
         '''
         
         verbose = kwargs.get('verbose',True)
         
         if (self.rank!=0):
             verbose=False
         
         # === attrs
         if ('duration_avg' in self.attrs.keys()):
             self.duration_avg = self.attrs['duration_avg']
+        # if ('rectilinear' in self.attrs.keys()):
+        #     self.rectilinear = self.attrs['rectilinear']
+        # if ('curvilinear' in self.attrs.keys()):
+        #     self.curvilinear = self.attrs['curvilinear']
+        
+        ## these should be set in the (init_from_() funcs)
+        if ('fclass' in self.attrs.keys()):
+            self.fclass = self.attrs['fclass'] ## 'rgd','cgd',...
+        if ('fsubtype' in self.attrs.keys()):
+            self.fsubtype = self.attrs['fsubtype'] ## 'unsteady','mean','prime',...
         
         # === udef
         
         if ('header' in self):
             
             udef_real = np.copy(self['header/udef_real'][:])
             udef_char = np.copy(self['header/udef_char'][:]) ## the unpacked numpy array of |S128 encoded fixed-length character objects
@@ -7558,15 +7954,15 @@
             self.p_inf       = self.udef['p_inf']
             self.T_inf       = self.udef['T_inf']
             self.C_Suth      = self.udef['C_Suth']
             self.S_Suth      = self.udef['S_Suth']
             self.mu_Suth_ref = self.udef['mu_Suth_ref']
             self.T_Suth_ref  = self.udef['T_Suth_ref']
             
-            if verbose: print(72*'-')
+            #if verbose: print(72*'-')
             if verbose: even_print('Ma'          , '%0.2f [-]'           % self.Ma          )
             if verbose: even_print('Re'          , '%0.1f [-]'           % self.Re          )
             if verbose: even_print('Pr'          , '%0.3f [-]'           % self.Pr          )
             if verbose: even_print('T_inf'       , '%0.3f [K]'           % self.T_inf       )
             if verbose: even_print('p_inf'       , '%0.1f [Pa]'          % self.p_inf       )
             if verbose: even_print('kappa'       , '%0.3f [-]'           % self.kappa       )
             if verbose: even_print('R'           , '%0.3f [J/(kg·K)]'    % self.R           )
@@ -7579,15 +7975,15 @@
             
             rho_inf = self.rho_inf = self.p_inf/(self.R * self.T_inf)
             mu_inf  = self.mu_inf  = 14.58e-7*self.T_inf**1.5/(self.T_inf+110.4)
             nu_inf  = self.nu_inf  = self.mu_inf/self.rho_inf
             a_inf   = self.a_inf   = np.sqrt(self.kappa*self.R*self.T_inf)
             U_inf   = self.U_inf   = self.Ma*self.a_inf
             cp      = self.cp      = self.R*self.kappa/(self.kappa-1.)
-            cv      = self.cv      = self.cp/self.kappa                         
+            cv      = self.cv      = self.cp/self.kappa
             r       = self.r       = self.Pr**(1/3)
             Tw      = self.Tw      = self.T_inf
             Taw     = self.Taw     = self.T_inf + self.r*self.U_inf**2/(2*self.cp)
             lchar   = self.lchar   = self.Re*self.nu_inf/self.U_inf
             
             tchar   = self.tchar = self.lchar / self.U_inf
             uchar   = self.uchar = self.U_inf
@@ -7601,15 +7997,16 @@
             if verbose: even_print('cp'      , '%0.3f [J/(kg·K)]' % self.cp      )
             if verbose: even_print('cv'      , '%0.3f [J/(kg·K)]' % self.cv      )
             if verbose: even_print('r'       , '%0.6f [-]'        % self.r       )
             if verbose: even_print('Tw'      , '%0.3f [K]'        % self.Tw      )
             if verbose: even_print('Taw'     , '%0.3f [K]'        % self.Taw     )
             if verbose: even_print('lchar'   , '%0.6E [m]'        % self.lchar   )
             if verbose: even_print('tchar'   , '%0.6E [s]'        % self.tchar   )
-            if verbose: print(72*'-'+'\n')
+            if verbose: print(72*'-')
+            #if verbose: print(72*'-'+'\n')
             
             # === write the 'derived' udef variables to a dict attribute of the RGD instance
             udef_char_deriv = ['rho_inf', 'mu_inf', 'nu_inf', 'a_inf', 'U_inf', 'cp', 'cv', 'r', 'Tw', 'Taw', 'lchar']
             udef_real_deriv = [ rho_inf,   mu_inf,   nu_inf,   a_inf,   U_inf,   cp,   cv,   r,   Tw,   Taw,   lchar ]
             self.udef_deriv = dict(zip(udef_char_deriv, udef_real_deriv))
         
         else:
@@ -7623,15 +8020,15 @@
             y   = self.y   = np.copy(self['dims/y'][:])
             z   = self.z   = np.copy(self['dims/z'][:])
             nx  = self.nx  = x.size
             ny  = self.ny  = y.size
             nz  = self.nz  = z.size
             ngp = self.ngp = nx*ny*nz
             
-            if verbose: print(72*'-')
+            #if verbose: print(72*'-')
             if verbose: even_print('nx', '%i'%nx )
             if verbose: even_print('ny', '%i'%ny )
             if verbose: even_print('nz', '%i'%nz )
             if verbose: even_print('ngp', '%i'%ngp )
             if verbose: print(72*'-')
             
             if verbose: even_print('x_min', '%0.2f'%x.min())
@@ -7642,15 +8039,16 @@
             if verbose: even_print('y_max', '%0.2f'%y.max())
             if (self.ny>2):
                 if verbose: even_print('dy begin : end', '%0.3E : %0.3E'%( (y[1]-y[0]), (y[-1]-y[-2]) ))
             if verbose: even_print('z_min', '%0.2f'%z.min())
             if verbose: even_print('z_max', '%0.2f'%z.max())
             if (self.nz>2):
                 if verbose: even_print('dz begin : end', '%0.3E : %0.3E'%( (z[1]-z[0]), (z[-1]-z[-2]) ))
-            if verbose: print(72*'-'+'\n')
+            #if verbose: print(72*'-'+'\n')
+            if verbose: print(72*'-')
         
         else:
             pass
         
         # === 1D grid filters
         
         self.hasGridFilter=False
@@ -7703,21 +8101,21 @@
         else:
             self.t  = np.array([], dtype=np.float64)
             self.ti = np.array([], dtype=np.int64)
             self.nt = nt = 0
             self.dt = 0.
             self.duration = duration = 0.
         
-        if verbose: print(72*'-')
+        #if verbose: print(72*'-')
         if verbose: even_print('nt', '%i'%self.nt )
         if verbose: even_print('dt', '%0.6f'%self.dt)
         if verbose: even_print('duration', '%0.2f'%self.duration )
         if hasattr(self, 'duration_avg'):
             if verbose: even_print('duration_avg', '%0.2f'%self.duration_avg )
-        if verbose: print(72*'-'+'\n')
+        #if verbose: print(72*'-'+'\n')
         
         # === ts group names & scalars
         
         if ('data' in self):
             self.scalars = list(self['data'].keys()) ## 4D : string names of scalars : ['u','v','w'],...
             self.n_scalars = len(self.scalars)
             self.scalars_dtypes = []
@@ -7725,92 +8123,18 @@
                 self.scalars_dtypes.append(self[f'data/{scalar}'].dtype)
             self.scalars_dtypes_dict = dict(zip(self.scalars, self.scalars_dtypes)) ## dict {<<scalar>>: <<dtype>>}
         else:
             self.scalars = []
             self.n_scalars = 0
             self.scalars_dtypes = []
             self.scalars_dtypes_dict = dict(zip(self.scalars, self.scalars_dtypes))
+        
         return
     
-    # === I/O funcs
-    
-    @staticmethod
-    def chunk_sizer(nxi, **kwargs):
-        '''
-        solve for an appropriate HDF5 chunk size based on dims
-        '''
-        
-        size_kb     = kwargs.get('size_kb'    , 1024) ## target chunk size [KB]
-        data_byte   = kwargs.get('data_byte'  , 4)    ## dtype size [B]
-        constraint  = kwargs.get('constraint' , None) ## nxi constraints (fixed )
-        base        = kwargs.get('base'       , 1)
-        
-        if not hasattr(nxi, '__iter__'):
-            raise AssertionError('\'nxi\' must be an iterable')
-        if constraint is None:
-            constraint = [None for i in range(len(nxi))]
-        if not hasattr(constraint, '__iter__'):
-            raise AssertionError('\'constraint\' must be an iterable')
-        if not (len(nxi)==len(constraint)):
-            raise ValueError('nxi and constraint must have same size')
-        if not isinstance(base, int):
-            raise TypeError('\'base\' must be type int')
-        
-        if False: ## increment divisor on all axes
-            
-            div=2
-            cc=-1
-            while True:
-                cc+=1
-                chunks=[]
-                for i in range(len(nxi)):
-                    if constraint[i] is not None:
-                        chunks.append(constraint[i])
-                    else:
-                        aa = max(math.ceil(nxi[i]/div),1)
-                        bb = max(nxi[i]//div,1)
-                        if (bb==1):
-                            chunks.append(1)
-                        else:
-                            chunks.append(aa)
-                
-                chunk_size_kb = np.prod(chunks)*data_byte / 1024.
-                #print('chunk size %0.1f [KB]'%chunk_size_kb)
-                
-                if (chunk_size_kb<=size_kb):
-                    break
-                else:
-                    div+=1
-                
-                if (cc>int(1e5)):
-                    raise RuntimeError('max iterations in rgd.chunk_sizer()')
-        
-        if True: ## increment divisor on largest axis
-            
-            nxi_ = [n for n in nxi] ## copy
-            div  = [1 for i in range(len(nxi))]
-            i_flexible = [i for i in range(len(nxi)) if constraint[i] is None]
-            while True:
-                chunks = [ max(math.ceil(nxi_[i]/div[i]),1) if (constraint[i] is None) else constraint[i] for i in range(len(nxi))]
-                
-                chunk_size_kb = np.prod(chunks)*data_byte / 1024.
-                #print('chunk size %0.1f [KB]'%chunk_size_kb)
-                
-                if (chunk_size_kb<=size_kb):
-                    break
-                else:
-                    aa = [i for i, j in enumerate(chunks) if (constraint[i] is None)]
-                    bb = [j for i, j in enumerate(chunks) if (constraint[i] is None)]
-                    i_gt = aa[np.argmax(bb)]
-                    if (base==1):
-                        div[i_gt] += 1
-                    else:
-                        div[i_gt] *= base
-        
-        return tuple(chunks)
+    # === I/O
     
     def init_from_eas4(self, fn_eas4, **kwargs):
         '''
         initialize an RGD from an EAS4 (NS3D output format)
         -----
         - x_min/max xi_min/max : min/max coord/index
         - stride filters (sx,sy,sz)
@@ -7844,24 +8168,28 @@
         yi_min = kwargs.get('yi_min',None)
         zi_min = kwargs.get('zi_min',None)
         
         xi_max = kwargs.get('xi_max',None)
         yi_max = kwargs.get('yi_max',None)
         zi_max = kwargs.get('zi_max',None)
         
+        ## set default attributes
+        self.attrs['fsubtype'] = 'unsteady'
+        self.attrs['fclass']   = 'rgd'
+        
         if verbose: print('\n'+'rgd.init_from_eas4()'+'\n'+72*'-')
         t_start_func = timeit.default_timer()
         
         # even_print('infile', os.path.basename(fn_eas4))
         # even_print('infile size', '%0.2f [GB]'%(os.path.getsize(fn_eas4)/1024**3))
         # even_print('outfile', self.fname)
         
-        if verbose: print('>>> infile : %s'%fn_eas4)
-        if verbose: print('>>> infile size : %0.2f [GB]'%(os.path.getsize(fn_eas4)/1024**3))
-        if verbose: print('>>> outfile : %s'%self.fname)
+        if verbose: even_print('infile', os.path.basename(fn_eas4))
+        if verbose: even_print('infile size', '%0.2f [GB]'%(os.path.getsize(fn_eas4)/1024**3))
+        if verbose: even_print('outfile', self.fname)
         
         with eas4(fn_eas4, 'r', verbose=False, driver=self.driver, comm=self.comm) as hf_eas4:
             
             if verbose: even_print( 'gmode dim1' , '%i / %s'%( hf_eas4.gmode_dim1_orig, gmode_dict[hf_eas4.gmode_dim1_orig] ) )
             if verbose: even_print( 'gmode dim2' , '%i / %s'%( hf_eas4.gmode_dim2_orig, gmode_dict[hf_eas4.gmode_dim2_orig] ) )
             if verbose: even_print( 'gmode dim3' , '%i / %s'%( hf_eas4.gmode_dim3_orig, gmode_dict[hf_eas4.gmode_dim3_orig] ) )
             
@@ -7953,15 +8281,15 @@
                     if verbose: even_print('xi_min', '%i'%xi_min)
                     for c in xfi:
                         if (xi_min<0) and (c>=(nx+xi_min)): ## support negative indexing
                             xfi_.append(c)
                         elif (xi_min>=0) and (c>=xi_min):
                             xfi_.append(c)
                     xfi=np.array(xfi_, dtype=np.int64)
-
+                
                 if (xi_max is not None):
                     
                     xfi_ = []
                     if verbose: even_print('xi_max', '%i'%xi_max)
                     for c in xfi:
                         if (xi_max<0) and (c<=(nx+xi_max)): ## support negative indexing
                             xfi_.append(c)
@@ -7975,15 +8303,15 @@
                     if verbose: even_print('yi_min', '%i'%yi_min)
                     for c in yfi:
                         if (yi_min<0) and (c>=(ny+yi_min)): ## support negative indexing
                             yfi_.append(c)
                         elif (yi_min>=0) and (c>=yi_min):
                             yfi_.append(c)
                     yfi=np.array(yfi_, dtype=np.int64)
-
+                
                 if (yi_max is not None):
                     
                     yfi_ = []
                     if verbose: even_print('yi_max', '%i'%yi_max)
                     for c in yfi:
                         if (yi_max<0) and (c<=(ny+yi_max)): ## support negative indexing
                             yfi_.append(c)
@@ -7997,15 +8325,15 @@
                     if verbose: even_print('zi_min', '%i'%zi_min)
                     for c in zfi:
                         if (zi_min<0) and (c>=(nz+zi_min)): ## support negative indexing
                             zfi_.append(c)
                         elif (zi_min>=0) and (c>=zi_min):
                             zfi_.append(c)
                     zfi=np.array(zfi_, dtype=np.int64)
-
+                
                 if (zi_max is not None):
                     
                     zfi_ = []
                     if verbose: even_print('zi_max', '%i'%zi_max)
                     for c in zfi:
                         if (zi_max<0) and (c<=(nz+zi_max)): ## support negative indexing
                             zfi_.append(c)
@@ -8066,19 +8394,19 @@
                 ###     print('>>> grid filter is present')
                 ### else:
                 ###     print('>>> no grid filter present')
                 
                 # === (over)write coord vecs if filter present
                 if self.hasGridFilter:
                     
-                    nx = x.size    
-                    ny = y.size    
-                    nz = z.size    
-                    ngp = nx*ny*nz 
-                    #nt = t.size   
+                    nx = x.size
+                    ny = y.size
+                    nz = z.size
+                    ngp = nx*ny*nz
+                    #nt = t.size
                     
                     if verbose: even_print('nx',  '%i'%nx  )
                     if verbose: even_print('ny',  '%i'%ny  )
                     if verbose: even_print('nz',  '%i'%nz  )
                     if verbose: even_print('ngp', '%i'%ngp )
                     #if verbose: even_print('nt', '%i'%nt )
                     
@@ -8108,31 +8436,42 @@
                     #print('>>> size of 3D coord arrays : %0.2f [GB]'%size3DCoordArrays)
                     if (size3DCoordArrays < 100): ## if less than 100 [MB]
                         xxx, yyy, zzz = np.meshgrid(x, y, z, indexing='ij')
                         self.create_dataset('dims/xxx', data=xxx.T)
                         self.create_dataset('dims/yyy', data=yyy.T)
                         self.create_dataset('dims/zzz', data=zzz.T)
         
-        if hasFilters: print(72*'-'+'\n')
+        if verbose: print(72*'-')
         self.get_header(verbose=True)
+        if verbose: print(72*'-')
+        
         return
     
     def init_from_rgd(self, fn_rgd, **kwargs):
         '''
         initialize an RGD from an RGD (copy over header data & coordinate data)
         '''
         
         t_info = kwargs.get('t_info',True)
+        #chunk_kb = kwargs.get('chunk_kb',4*1024) ## 4 [MB]
         
         verbose = kwargs.get('verbose',True)
         if (self.rank!=0):
             verbose=False
         
+        ## set default attributes: fsubtype, fclass
+        self.attrs['fsubtype'] = 'unsteady'
+        self.attrs['fclass']   = 'rgd'
+        
         with rgd(fn_rgd, 'r', driver=self.driver, comm=self.comm) as hf_ref:
             
+            ## copy over fsubtype
+            if hasattr(hf_ref,'fsubtype'):
+                self.attrs['fsubtype'] = hf_ref.fsubtype
+            
             # === copy over header info if needed
             
             if all([('header/udef_real' in self),('header/udef_char' in self)]):
                 raise ValueError('udef already present')
             else:
                 udef         = hf_ref.udef
                 udef_real    = list(udef.values())
@@ -8171,14 +8510,23 @@
                 self.nt = self.t.size
                 self.create_dataset('dims/t', data=hf_ref.t)
             else:
                 t = np.array([0.], dtype=np.float64)
                 if ('dims/t' in self):
                     del self['dims/t']
                 self.create_dataset('dims/t', data=t)
+            
+            # ===
+            
+            ## copy over [data_dim/<>] dsets if present
+            if ('data_dim' in hf_ref):
+                for dsn in hf_ref['data_dim'].keys():
+                    data = np.copy( hf_ref[f'data_dim/{dsn}'][()] ) 
+                    self.create_dataset(f'data_dim/{dsn}', data=data, chunks=None)
+                    if self.usingmpi: self.comm.Barrier()
         
         self.get_header(verbose=False)
         return
     
     def import_eas4(self, fn_eas4_list, **kwargs):
         '''
         import data from a series of EAS4 files to a RGD
@@ -8198,45 +8546,54 @@
         t_start_func = timeit.default_timer()
         
         ti_min = kwargs.get('ti_min',None)
         ti_max = kwargs.get('ti_max',None)
         tt_min = kwargs.get('tt_min',None)
         tt_max = kwargs.get('tt_max',None)
         
-        chunk_kb = kwargs.get('chunk_kb',4*1024) ## default chunk size 4 [MB]
+        chunk_kb         = kwargs.get('chunk_kb',4*1024) ## h5 chunk size: default 4 [MB]
+        chunk_constraint = kwargs.get('chunk_constraint',None) ## the 'constraint' parameter for sizing h5 chunks
+        chunk_base       = kwargs.get('chunk_base',None)
         
         ## float precision when copying
         ## default is 'single' i.e. cast data to single
         ## 'same' will preserve the floating point precision from the EAS4 file
         prec = kwargs.get('prec',None)
         if (prec is None):
             prec = 'single'
         elif (prec=='single'):
             pass
         elif (prec=='same'):
             pass
         else:
             raise ValueError('prec not set correctly')
         
-        # === check for an often made mistake
+        ## HDF5 chunk parameters (t,z,y,x)
+        if (chunk_constraint is None):
+            chunk_constraint = (1,None,None,None) ## single [t] convention
+            #chunk_constraint = (None,-1,1,-1) ## single [y] convention
+        if (chunk_base is None):
+            chunk_base = 4
+        
+        ## check for an often made mistake
         ts_min = kwargs.get('ts_min',None)
         ts_max = kwargs.get('ts_max',None)
         if (ts_min is not None):
             raise AssertionError('ts_min is not an option --> did you mean ti_min or tt_min?')
         if (ts_max is not None):
             raise AssertionError('ts_max is not an option --> did you mean ti_max or tt_max?')
         
-        # === check that iterable of EAS4 files is OK
+        ## check that iterable of EAS4 files is OK
         if not hasattr(fn_eas4_list, '__iter__'):
             raise AssertionError('first arg \'fn_eas4_list\' must be iterable')
         for fn_eas4 in fn_eas4_list:
             if not os.path.isfile(fn_eas4):
                 raise FileNotFoundError('%s not found!'%fn_eas4)
         
-        # === ranks
+        ## ranks
         rx = kwargs.get('rx',1)
         ry = kwargs.get('ry',1)
         rz = kwargs.get('rz',1)
         rt = kwargs.get('rt',1)
         
         if (rx*ry*rz*rt != self.n_ranks):
             raise AssertionError('rx*ry*rz*rt != self.n_ranks')
@@ -8421,16 +8778,16 @@
             dtype = self.scalars_dtypes_dict[scalar]
             float_bytes = dtype.itemsize
             data_gb = float_bytes*self.nt*self.nz*self.ny*self.nx / 1024**3
             
             if verbose:
                 even_print('initializing data/%s'%(scalar,),'%0.2f [GB]'%(data_gb,))
             
-            shape  = (self.nt,self.nz,self.ny,self.nx)
-            chunks = rgd.chunk_sizer(nxi=shape, constraint=(1,None,None,None), size_kb=chunk_kb, base=2, data_byte=float_bytes)
+            shape = (self.nt,self.nz,self.ny,self.nx)
+            chunks = h5_chunk_sizer(nxi=shape, constraint=chunk_constraint, size_kb=chunk_kb, base=chunk_base, itemsize=float_bytes)
             
             dset = self.create_dataset('data/%s'%scalar, 
                                        shape=shape, 
                                        dtype=dtype,
                                        chunks=chunks)
             
             chunk_kb_ = np.prod(dset.chunks)*float_bytes / 1024. ## actual
@@ -8604,45 +8961,55 @@
         t_start_func = timeit.default_timer()
         
         rx       = kwargs.get('rx',1)
         ry       = kwargs.get('ry',1)
         rz       = kwargs.get('rz',1)
         rt       = kwargs.get('rt',1)
         force    = kwargs.get('force',False) ## overwrite or raise error if exists
-        chunk_kb = kwargs.get('chunk_kb',4*1024) ## 4 [MB]
         ti_min   = kwargs.get('ti_min',None)
         ti_max   = kwargs.get('ti_max',None)
         scalars  = kwargs.get('scalars',None)
-        ##
+        
+        chunk_kb         = kwargs.get('chunk_kb',4*1024) ## h5 chunk size: default 4 [MB]
+        chunk_constraint = kwargs.get('chunk_constraint',None) ## the 'constraint' parameter for sizing h5 chunks
+        chunk_base       = kwargs.get('chunk_base',None)
+        
         xi_min = kwargs.get('xi_min',None) ## 4D coordinate 
         xi_max = kwargs.get('xi_max',None)
         yi_min = kwargs.get('yi_min',None)
         yi_max = kwargs.get('yi_max',None)
         zi_min = kwargs.get('zi_min',None)
         zi_max = kwargs.get('zi_max',None)
         ti_min = kwargs.get('ti_min',None)
         ti_max = kwargs.get('ti_max',None)
-        ##
+        
         ct = kwargs.get('ct',1) ## 'chunks' in time
         
         if (rt!=1):
             raise AssertionError('rt!=1')
         if (rx*ry*rz!=n_ranks):
             raise AssertionError('rx*ry*rz!=n_ranks')
         if not os.path.isfile(fn_rgd_src):
             raise FileNotFoundError('%s not found!'%fn_rgd_src)
         if os.path.isfile(fn_rgd_tgt) and not force:
             raise FileExistsError('%s already exists. delete it or use \'force=True\' kwarg'%fn_rgd_tgt)
         
+        ## HDF5 chunk parameters
+        if (chunk_constraint is None):
+            chunk_constraint = (1,None,None,None) ## single [t] convention
+            #chunk_constraint = (None,-1,1,-1) ## single [y] convention
+        if (chunk_base is None):
+            chunk_base = 4
+        
         # ===
         
         with rgd(fn_rgd_src, 'r', comm=MPI.COMM_WORLD, driver='mpio', libver='latest') as hf_src:
             with rgd(fn_rgd_tgt, 'w', comm=MPI.COMM_WORLD, driver='mpio', libver='latest', force=force) as hf_tgt:
                 
-                ## copy over header info
+                ## copy over header info (source --> target)
                 hf_tgt.init_from_rgd(fn_rgd_src)
                 
                 if (scalars is None):
                     scalars = hf_src.scalars
                 
                 if verbose:
                     even_print('fn_rgd_src' , fn_rgd_src )
@@ -8899,35 +9266,34 @@
                 #rt2_ = rt2 - ti[ti_min]
                 
                 ## time 'chunks' split (number of timesteps to read / write at a time)
                 ctl_ = np.array_split(tfi,ct)
                 ctl = [[b[0],b[-1]+1] for b in ctl_ ]
                 
                 shape  = (nt,nz,ny,nx) ## target
-                #chunks = rgd.chunk_sizer(nxi=shape, constraint=(1,None,None,None), size_kb=chunk_kb, base=2)
-                
                 hf_tgt.scalars = []
                 #data_gb = 4*nx*ny*nz*nt / 1024**3
                 
                 ## initialize datasets
                 t_start = timeit.default_timer()
                 for scalar in hf_src.scalars:
                     
                     dtype = hf_src.scalars_dtypes_dict[scalar]
                     float_bytes = dtype.itemsize
-                    chunks = rgd.chunk_sizer(nxi=shape, constraint=(1,None,None,None), size_kb=chunk_kb, base=2, data_byte=float_bytes)
+                    
+                    chunks = h5_chunk_sizer(nxi=shape, constraint=chunk_constraint, size_kb=chunk_kb, base=chunk_base, itemsize=float_bytes)
                     data_gb = float_bytes * nx * ny * nz * nt / 1024**3
                     
                     if (scalar in scalars):
                         if verbose:
                             even_print('initializing data/%s'%(scalar,),'%0.1f [GB]'%(data_gb,))
                         dset = hf_tgt.create_dataset('data/%s'%scalar,
-                                                       shape=shape,
-                                                       dtype=dtype,
-                                                       chunks=chunks)
+                                                     shape=shape,
+                                                     dtype=dtype,
+                                                     chunks=chunks)
                         hf_tgt.scalars.append(scalar)
                         
                         chunk_kb_ = np.prod(dset.chunks)*float_bytes / 1024. ## actual
                         if verbose:
                             even_print('chunk shape (t,z,y,x)','%s'%str(dset.chunks))
                             even_print('chunk size','%i [KB]'%int(round(chunk_kb_)))
                 
@@ -9022,15 +9388,15 @@
         delete scalars from RGD 
         '''
         pass
         return
     
     def read(self,**kwargs):
         '''
-        a convenience func to read all data from file & return structured array
+        read data from file & return structured array
         '''
         
         verbose_master = kwargs.get('verbose',True)
         
         if (self.rank==0):
             verbose = True
         else:
@@ -9199,15 +9565,15 @@
         ## write dims
         self.create_dataset('dims/x', data=x)
         self.create_dataset('dims/y', data=y)
         self.create_dataset('dims/z', data=z)
         self.create_dataset('dims/t', data=t)
         
         shape  = (self.nt,self.nz,self.ny,self.nx)
-        chunks = rgd.chunk_sizer(nxi=shape, constraint=(1,None,None,None), size_kb=chunk_kb, base=2)
+        chunks = h5_chunk_sizer(nxi=shape, constraint=(1,None,None,None), size_kb=chunk_kb, base=4, itemsize=4)
         
         ## initialize
         data_gb = 4*nx*ny*nz*nt / 1024.**3
         for scalar in ['u','v','w']:
             if ('data/%s'%scalar in self):
                 del self['data/%s'%scalar]
             if verbose:
@@ -9298,23 +9664,32 @@
         t_start_func = timeit.default_timer()
         
         rx = kwargs.get('rx',1)
         ry = kwargs.get('ry',1)
         rz = kwargs.get('rz',1)
         rt = kwargs.get('rt',1)
         
-        chunk_kb = kwargs.get('chunk_kb',4*1024) ## 4 [MB]
+        chunk_kb         = kwargs.get('chunk_kb',4*1024) ## h5 chunk size: default 4 [MB]
+        chunk_constraint = kwargs.get('chunk_constraint',None) ## the 'constraint' parameter for sizing h5 chunks
+        chunk_base       = kwargs.get('chunk_base',None)
         
         self.nx = nx = kwargs.get('nx',128)
         self.ny = ny = kwargs.get('ny',128)
         self.nz = nz = kwargs.get('nz',128)
         self.nt = nt = kwargs.get('nt',128)
         
-        data_gb = 3 * 4*nx*ny*nz*nt / 1024.**3
+        #data_gb = 3 * 4*nx*ny*nz*nt / 1024.**3
+        data_gb = 1 * 4*nx*ny*nz*nt / 1024.**3
+        
         if verbose: even_print(self.fname, '%0.2f [GB]'%(data_gb,))
+        if verbose: even_print('nx','%i'%self.nx)
+        if verbose: even_print('ny','%i'%self.ny)
+        if verbose: even_print('nz','%i'%self.nz)
+        if verbose: even_print('nt','%i'%self.nt)
+        if verbose: print(72*'-')
         
         self.x = x = np.linspace(0., 2*np.pi, nx, dtype=np.float32)
         self.y = y = np.linspace(0., 2*np.pi, ny, dtype=np.float32)
         self.z = z = np.linspace(0., 2*np.pi, nz, dtype=np.float32)
         #self.t = t = np.linspace(0., 10.,     nt, dtype=np.float32)
         self.t = t = 0.1 * np.arange(nt, dtype=np.float32)
         
@@ -9347,23 +9722,25 @@
         else:
             nxr = nx
             nyr = ny
             nzr = nz
             ntr = nt
         
         ## write dims (independent)
-        self.create_dataset('dims/x', data=x)
-        self.create_dataset('dims/y', data=y)
-        self.create_dataset('dims/z', data=z)
-        self.create_dataset('dims/t', data=t)
+        self.create_dataset('dims/x', data=x, chunks=None)
+        self.create_dataset('dims/y', data=y, chunks=None)
+        self.create_dataset('dims/z', data=z, chunks=None)
+        self.create_dataset('dims/t', data=t, chunks=None)
         
         shape  = (self.nt,self.nz,self.ny,self.nx)
-        chunks = rgd.chunk_sizer(nxi=shape, constraint=(1,None,None,None), size_kb=chunk_kb, base=2)
+        float_bytes = 4
+        chunks = h5_chunk_sizer(nxi=shape, constraint=chunk_constraint, size_kb=chunk_kb, base=chunk_base, itemsize=float_bytes)
         
-        self.scalars = ['u','v','w']
+        #self.scalars = ['u','v','w']
+        self.scalars = ['u']
         self.scalars_dtypes = [np.float32 for s in self.scalars]
         
         ## initialize datasets
         data_gb = 4*nx*ny*nz*nt / 1024.**3
         self.usingmpi: self.comm.Barrier()
         t_start = timeit.default_timer()
         for scalar in self.scalars:
@@ -9422,26 +9799,25 @@
                 even_print('write: %s'%(scalar,), '%0.2f [GB]  %0.3f [s]  %0.3f [GB/s]'%(data_gb,t_delta,(data_gb/t_delta)))
         
         if verbose: print(72*'-')
         if verbose: even_print('time initialize',format_time_string(t_initialize))
         if verbose: even_print('write total', '%0.2f [GB]  %0.3f [s]  %0.3f [GB/s]'%(data_gb_write,t_write,(data_gb_write/t_write)))
         if verbose: even_print(self.fname, '%0.2f [GB]'%(os.path.getsize(self.fname)/1024**3))
         if verbose: print(72*'-')
-        
-        if verbose: print('\n'+72*'-')
         if verbose: print('total time : rgd.populate_white_noise() : %s'%format_time_string((timeit.default_timer() - t_start_func)))
         if verbose: print(72*'-')
         
         return
     
-    # === post-processing
+    # === averaging
     
     def get_mean(self, **kwargs):
         '''
         get mean in [t] --> leaves [x,y,z,1]
+        --> save to new RGD file
         '''
         
         if (self.rank==0):
             verbose = True
         else:
             verbose = False
         
@@ -9458,15 +9834,24 @@
         #sfm         = kwargs.get('scalars',None) ## scalars to take (for mean)
         ti_min       = kwargs.get('ti_min',None)
         favre        = kwargs.get('favre',True)
         reynolds     = kwargs.get('reynolds',True)
         ##
         force        = kwargs.get('force',False)
         
-        chunk_kb     = kwargs.get('chunk_kb',4*1024) ## 4 [MB]
+        chunk_kb         = kwargs.get('chunk_kb',4*1024) ## h5 chunk size: default 4 [MB]
+        chunk_constraint = kwargs.get('chunk_constraint',None) ## the 'constraint' parameter for sizing h5 chunks
+        chunk_base       = kwargs.get('chunk_base',None)
+        
+        ## HDF5 chunk parameters (t,z,y,x)
+        if (chunk_constraint is None):
+            chunk_constraint = (1,None,None,None) ## single [t] convention
+            #chunk_constraint = (None,-1,1,-1) ## single [y] convention
+        if (chunk_base is None):
+            chunk_base = 4
         
         if (rx*ry*rz != self.n_ranks):
             raise AssertionError('rx*ry*rz != self.n_ranks')
         if (rx>self.nx):
             raise AssertionError('rx>self.nx')
         if (ry>self.ny):
             raise AssertionError('ry>self.ny')
@@ -9529,81 +9914,88 @@
             ti_for_avg = np.copy( self.ti )
         
         nt_avg       = ti_for_avg.shape[0]
         t_avg_start  = self.t[ti_for_avg[0]]
         t_avg_end    = self.t[ti_for_avg[-1]]
         duration_avg = t_avg_end - t_avg_start
         
+        ## assert constant Δt, later attach dt as attribute to mean file
+        dt0 = np.diff(self.t)[0]
+        if not np.all(np.isclose(np.diff(self.t), dt0, rtol=1e-7)):
+            raise ValueError
+        
         if verbose: even_print('n timesteps avg','%i/%i'%(nt_avg,self.nt))
         if verbose: even_print('t index avg start','%i'%(ti_for_avg[0],))
         if verbose: even_print('t index avg end','%i'%(ti_for_avg[-1],))
         if verbose: even_print('t avg start','%0.2f [-]'%(t_avg_start,))
         if verbose: even_print('t avg end','%0.2f [-]'%(t_avg_end,))
         if verbose: even_print('duration avg','%0.2f [-]'%(duration_avg,))
-        if verbose: print(72*'-')
+        if verbose: even_print('Δt','%0.2f [-]'%(dt0,))
+        #if verbose: print(72*'-')
         
         ## performance
         t_read = 0.
         t_write = 0.
         data_gb_read = 0.
         data_gb_write = 0.
         
         ##data_gb      = 4*self.nx*self.ny*self.nz*self.nt / 1024**3
         #data_gb      = 4*self.nx*self.ny*self.nz*nt_avg / 1024**3
         #data_gb_mean = 4*self.nx*self.ny*self.nz*1      / 1024**3
         
         scalars_re = ['u','v','w','p','T','rho']
         scalars_fv = ['u','v','w','p','T','rho']
         
-        ## check if constant Δt (if so, attach dt attribute to mean file)
-        dt0_ = np.diff(self.t)[0]
-        if np.all(np.isclose(np.diff(self.t), dt0_, rtol=1e-7)):
-            dt0 = dt0_
-        else:
-            dt0 = None
-        dt0_ = None; del dt0_
-        
         #with rgd(fn_rgd_mean, 'w', force=force, driver='mpio', comm=MPI.COMM_WORLD) as hf_mean:
         with rgd(fn_rgd_mean, 'w', force=force, driver=self.driver, comm=self.comm) as hf_mean:
             
+            ## initialize the mean file from the opened unsteady rgd file
+            hf_mean.init_from_rgd(self.fname)
+            
+            ## set some top-level attributes
             hf_mean.attrs['duration_avg'] = duration_avg ## duration of mean
             #hf_mean.attrs['duration_avg'] = self.duration
-            
             hf_mean.attrs['dt'] = dt0
+            #hf_mean.attrs['fclass'] = 'rgd'
+            hf_mean.attrs['fsubtype'] = 'mean'
             
-            hf_mean.init_from_rgd(self.fname) ## initialize the mean rgd file from the rgd file
+            if verbose: print(72*'-')
             
             # === initialize mean datasets
             for scalar in self.scalars:
                 
                 dtype = self.scalars_dtypes_dict[scalar]
                 float_bytes = self.scalars_dtypes_dict[scalar].itemsize
                 
                 data_gb_mean = float_bytes*self.nx*self.ny*self.nz*1 / 1024**3
                 
                 shape  = (1,self.nz,self.ny,self.nx)
-                chunks = rgd.chunk_sizer(nxi=shape, constraint=(1,None,None,None), size_kb=chunk_kb, base=2, data_byte=float_bytes)
+                chunks = h5_chunk_sizer(nxi=shape, constraint=chunk_constraint, size_kb=chunk_kb, base=chunk_base, itemsize=float_bytes)
                 
                 if reynolds:
                     
-                    if ('data/%s'%scalar in hf_mean):
-                        del hf_mean['data/%s'%scalar]
-                    if verbose:
-                        even_print( f'initializing data/{scalar}' , f'{data_gb_mean:0.3f} [GB]' )
-                    dset = hf_mean.create_dataset(f'data/{scalar}',
-                                                  shape=shape,
-                                                  dtype=dtype,
-                                                  chunks=chunks,
-                                                  )
-                    hf_mean.scalars.append('data/%s'%scalar)
-                    
-                    chunk_kb_ = np.prod(dset.chunks)*float_bytes / 1024. ## actual
-                    if verbose:
-                        even_print('chunk shape (t,z,y,x)','%s'%str(dset.chunks))
-                        even_print('chunk size','%i [KB]'%int(round(chunk_kb_)))
+                    ## do the Re mean of all scalars in file, regardless whether explicitly in scalars_re or not
+                    #if scalar in scalars_re:
+                    if True:
+                        
+                        if ('data/%s'%scalar in hf_mean):
+                            del hf_mean['data/%s'%scalar]
+                        if verbose:
+                            even_print( f'initializing data/{scalar}' , f'{data_gb_mean:0.3f} [GB]' )
+                        dset = hf_mean.create_dataset(f'data/{scalar}',
+                                                      shape=shape,
+                                                      dtype=dtype,
+                                                      chunks=chunks,
+                                                      )
+                        hf_mean.scalars.append('data/%s'%scalar)
+                        
+                        chunk_kb_ = np.prod(dset.chunks)*float_bytes / 1024. ## actual
+                        if verbose:
+                            even_print('chunk shape (t,z,y,x)','%s'%str(dset.chunks))
+                            even_print('chunk size','%i [KB]'%int(round(chunk_kb_)))
                 
                 if favre:
                     
                     if (scalar in scalars_fv):
                         if ('data/%s_fv'%scalar in hf_mean):
                             del hf_mean['data/%s_fv'%scalar]
                         if verbose:
@@ -9623,14 +10015,15 @@
             if self.usingmpi: self.comm.Barrier()
             if verbose: print(72*'-')
             
             # === read rho
             if favre:
                 
                 dset = self['data/rho']
+                
                 dtype = self.scalars_dtypes_dict['rho']
                 if (dtype!=dset.dtype):
                     raise ValueError
                 float_bytes = self.scalars_dtypes_dict[scalar].itemsize
                 
                 if self.usingmpi: self.comm.Barrier()
                 t_start = timeit.default_timer()
@@ -9760,15 +10153,14 @@
                             txt = even_print('write: %s_fv'%scalar, '%0.2f [GB]  %0.2f [s]  %0.3f [GB/s]'%(data_gb_mean,t_delta,(data_gb_mean/t_delta)), s=True)
                             tqdm.write(txt)
                         
                         t_write       += t_delta
                         data_gb_write += data_gb_mean
             
             if self.usingmpi: self.comm.Barrier()
-            if verbose: print(72*'-')
             
             # === replace dims/t array --> take last time of series
             t = np.array([self.t[-1]],dtype=np.float64)
             if ('dims/t' in hf_mean):
                 del hf_mean['dims/t']
             hf_mean.create_dataset('dims/t', data=t)
             
@@ -9778,33 +10170,383 @@
         if verbose: print(72*'-')
         if verbose: even_print('time read',format_time_string(t_read))
         if verbose: even_print('time write',format_time_string(t_write))
         if verbose: even_print(fn_rgd_mean, '%0.2f [GB]'%(os.path.getsize(fn_rgd_mean)/1024**3))
         if verbose: even_print('read total avg', '%0.2f [GB]  %0.3f [s]  %0.3f [GB/s]'%(data_gb_read,t_read,(data_gb_read/t_read)))
         if verbose: even_print('write total avg', '%0.2f [GB]  %0.3f [s]  %0.3f [GB/s]'%(data_gb_write,t_write,(data_gb_write/t_write)))
         if verbose: print(72*'-')
-        
-        if verbose: print('\n'+72*'-')
         if verbose: print('total time : rgd.get_mean() : %s'%format_time_string((timeit.default_timer() - t_start_func)))
         if verbose: print(72*'-')
         return
     
+    def add_mean_dimensional_data_xpln(self, **kwargs):
+        '''
+        get dimensionalized mean data for [x] plane
+        --> save to existing RGD file with fsubtype=mean
+        - assumes volume which is thin in [x] direction
+        - an RGD which is the output of rgd.get_mean() should be opened here
+        - not parallel
+        '''
+        
+        verbose = kwargs.get('verbose',True)
+        epsilon = kwargs.get('epsilon',5e-4)
+        
+        if (self.rank==0):
+            verbose = True
+        else:
+            verbose = False
+        
+        if verbose: print('\n'+'rgd.add_mean_dimensional_data_xpln()'+'\n'+72*'-')
+        t_start_func = timeit.default_timer()
+        
+        ## this func is not parallel
+        if self.usingmpi:
+            raise NotImplementedError('rgd.add_mean_dimensional_data_xpln() is not a parallel function')
+        
+        ## 'r' and 'w' open modes are not allowed
+        if not (self.open_mode=='a') or (self.open_mode=='r+'):
+            raise ValueError(f'open mode is {self.open_mode}')
+        
+        ## assert that this is a mean flow file ( i.e. output from cgd.get_mean() )
+        if (self.fsubtype!='mean'):
+            print(self.fsubtype)
+            raise ValueError
+        
+        ## get size of infile
+        fsize = os.path.getsize(self.fname)/1024**3
+        if verbose: even_print(os.path.basename(self.fname),'%0.1f [GB]'%fsize)
+        if verbose: even_print('nx','%i'%self.nx)
+        if verbose: even_print('ny','%i'%self.ny)
+        if verbose: even_print('nz','%i'%self.nz)
+        if verbose: even_print('nt','%i'%self.nt)
+        if verbose: even_print('ngp','%0.1f [M]'%(self.ngp/1e6,))
+        if verbose: print(72*'-')
+        
+        ## read in 1D coordinate arrays, then dimensinoalize [m]
+        x = np.copy( self['dims/x'][()] * self.lchar )
+        y = np.copy( self['dims/y'][()] * self.lchar )
+        z = np.copy( self['dims/z'][()] * self.lchar )
+        nx = self.nx
+        ny = self.ny
+        nz = self.nz
+        
+        if (x.ndim!=1):
+            raise ValueError
+        if (y.ndim!=1):
+            raise ValueError
+        if (z.ndim!=1):
+            raise ValueError
+        
+        ## check if constant Δz (calculate Δz+ later)
+        dz0 = np.diff(z)[0]
+        if not np.all(np.isclose(np.diff(z), dz0, rtol=1e-7)):
+            raise NotImplementedError
+        
+        ## check if mean rgd has attr 'dt'
+        if ('dt' in self.attrs.keys()):
+            dt = self.attrs['dt']
+            if (dt is not None):
+                dt *= self.tchar
+        else:
+            raise ValueError
+        
+        if verbose: even_print('Δt/tchar','%0.8f'%(dt/self.tchar))
+        if verbose: even_print('Δt','%0.3e [s]'%(dt,))
+        if verbose: even_print('duration/tchar','%0.1f'%(self.duration_avg,))
+        if verbose: even_print('duration','%0.3e [s]'%(self.duration_avg*self.tchar,))
+        if verbose: print(72*'-')
+        
+        ## re-dimensionalize
+        u   =  self.U_inf                     * np.copy( self['data/u'][()].T   )
+        v   =  self.U_inf                     * np.copy( self['data/v'][()].T   )
+        w   =  self.U_inf                     * np.copy( self['data/w'][()].T   )
+        rho =  self.rho_inf                   * np.copy( self['data/rho'][()].T )
+        p   =  (self.rho_inf * self.U_inf**2) * np.copy( self['data/p'][()].T   )
+        T   =  self.T_inf                     * np.copy( self['data/T'][()].T   )
+        
+        # mu1 = (14.58e-7 * T**1.5) / ( T + 110.4 )
+        # mu2 = self.mu_Suth_ref * ( T / self.T_Suth_ref )**(3/2) * (self.T_Suth_ref+self.S_Suth)/(T+self.S_Suth)
+        # mu3 = self.C_Suth * T**(3/2) / (T + self.S_Suth)
+        # np.testing.assert_allclose(mu1, mu2, rtol=1e-14, atol=1e-14)
+        # np.testing.assert_allclose(mu2, mu3, rtol=1e-14, atol=1e-14)
+        # mu = np.copy(mu3)
+        
+        mu = self.C_Suth * T**(3/2) / (T + self.S_Suth)
+        nu = mu / rho
+        
+        # === average in [z] --> leave 2D [x,y]
+        
+        u     = np.squeeze( np.mean( u     , axis=2, dtype=np.float64).astype(np.float32) )
+        v     = np.squeeze( np.mean( v     , axis=2, dtype=np.float64).astype(np.float32) )
+        w     = np.squeeze( np.mean( w     , axis=2, dtype=np.float64).astype(np.float32) )
+        rho   = np.squeeze( np.mean( rho   , axis=2, dtype=np.float64).astype(np.float32) )
+        p     = np.squeeze( np.mean( p     , axis=2, dtype=np.float64).astype(np.float32) )
+        T     = np.squeeze( np.mean( T     , axis=2, dtype=np.float64).astype(np.float32) )
+        #utang = np.squeeze( np.mean( utang , axis=2, dtype=np.float64).astype(np.float32) )
+        #unorm = np.squeeze( np.mean( unorm , axis=2, dtype=np.float64).astype(np.float32) )
+        mu    = np.squeeze( np.mean( mu    , axis=2, dtype=np.float64).astype(np.float32) )
+        nu    = np.squeeze( np.mean( nu    , axis=2, dtype=np.float64).astype(np.float32) )
+        
+        ## determine finite difference order / size of central stencil 
+        if (nx<3):
+            raise ValueError('dx[] not possible because nx<3')
+        elif (nx>=3) and (nx<5):
+            acc = 2
+        elif (nx>=5) and (nx<7):
+            acc = 4
+        elif (nx>=7):
+            acc = 6
+        else:
+            raise ValueError('this should never happen')
+        
+        edge_stencil = 'half'
+        if verbose: even_print('acc','%i'%acc)
+        if verbose: even_print('edge_stencil',edge_stencil)
+        
+        # === get gradients & vort_z
+        
+        ddx_u = gradient(u, x, axis=0, acc=acc, edge_stencil=edge_stencil, d=1, no_warn=True)
+        ddy_u = gradient(u, y, axis=1, acc=acc, edge_stencil=edge_stencil, d=1, no_warn=True)
+        
+        ddx_v = gradient(v, x, axis=0, acc=acc, edge_stencil=edge_stencil, d=1, no_warn=True)
+        ddy_v = gradient(v, y, axis=1, acc=acc, edge_stencil=edge_stencil, d=1, no_warn=True)
+        
+        ## dimensional [1/s]
+        vort_z = ddx_v - ddy_u
+        
+        # ===
+        
+        ## [y] gradients --> yields 1D in [y]
+        ddy_u   = gradient(u   , y, axis=1, acc=acc, edge_stencil=edge_stencil)
+        ddy_v   = gradient(v   , y, axis=1, acc=acc, edge_stencil=edge_stencil)
+        ddy_T   = gradient(T   , y, axis=1, acc=acc, edge_stencil=edge_stencil)
+        ddy_p   = gradient(p   , y, axis=1, acc=acc, edge_stencil=edge_stencil)
+        ddy_rho = gradient(rho , y, axis=1, acc=acc, edge_stencil=edge_stencil)
+        
+        ## wall quantities --> mean over [x] --> leave 0D float
+        ddy_u_wall  = float( np.mean( ddy_u[:,0] ) )
+        ddy_T_wall  = float( np.mean( ddy_T[:,0] ) )
+        rho_wall    = float( np.mean( rho[:,0]   ) )
+        nu_wall     = float( np.mean( nu[:,0]    ) )
+        mu_wall     = float( np.mean( mu[:,0]    ) )
+        T_wall      = float( np.mean( T[:,0]     ) )
+        tau_wall    = mu_wall * ddy_u_wall
+        q_wall      = self.cp * mu_wall / self.Pr * ddy_T_wall ## wall heat flux (?)
+        
+        ## friction velocity
+        u_tau  = np.sqrt(tau_wall/rho_wall)
+        #y_plus = np.copy( s2 * u_tau / nu_wall )
+        
+        # === populate 1D & 2D arrays using calc_bl_edge_1d(), calc_d99_1d()
+        
+        psvel = np.zeros((nx,ny), dtype=np.float64)
+        
+        psvel_edge = np.zeros((nx,), dtype=np.float64)
+        u_edge     = np.zeros((nx,), dtype=np.float64)
+        rho_edge   = np.zeros((nx,), dtype=np.float64)
+        mu_edge    = np.zeros((nx,), dtype=np.float64)
+        nu_edge    = np.zeros((nx,), dtype=np.float64)
+        T_edge     = np.zeros((nx,), dtype=np.float64)
+        
+        y_edge = np.zeros((nx,), dtype=np.float64)
+        d99    = np.zeros((nx,), dtype=np.float64)
+        
+        u_99   = np.zeros((nx,), dtype=np.float64)
+        
+        for i in range(nx):
+            
+            vort_z_ = np.copy( vort_z[i,:] )
+            psvel_  = sp.integrate.cumulative_trapezoid(-1*vort_z_, y, initial=0.)
+            psvel[i,:] = psvel_
+            
+            ## get edge
+            y_edge_ = calc_bl_edge_1d( y=y, psvel=psvel_, ynorm=self.lchar, acc=acc, edge_stencil=edge_stencil, epsilon=epsilon )
+            #aa = ( y_edge_ - y.min() ) / ( y.max() - y.min() )
+            #tqdm.write(f'{aa:0.9f}')
+            y_edge[i] = y_edge_
+            
+            ## interpolate at edge
+            psvel_edge_ = sp.interpolate.interp1d(y, psvel_ , kind='cubic', bounds_error=True)(y_edge_)
+            psvel_edge_ = float(psvel_edge_)
+            psvel_edge[i] = psvel_edge_
+            
+            u_edge[i]   = sp.interpolate.interp1d(y, u[i,:]   , kind='cubic', bounds_error=True)(y_edge_)
+            rho_edge[i] = sp.interpolate.interp1d(y, rho[i,:] , kind='cubic', bounds_error=True)(y_edge_)
+            mu_edge[i]  = sp.interpolate.interp1d(y, mu[i,:]  , kind='cubic', bounds_error=True)(y_edge_)
+            nu_edge[i]  = sp.interpolate.interp1d(y, nu[i,:]  , kind='cubic', bounds_error=True)(y_edge_)
+            T_edge[i]   = sp.interpolate.interp1d(y, T[i,:]   , kind='cubic', bounds_error=True)(y_edge_)
+            
+            ## get d99
+            d99_ = calc_d99_1d( y=y, y_edge=y_edge_, psvel=psvel_, psvel_edge=psvel_edge_ )
+            d99_ = float(d99_)
+            d99[i] = d99_
+            
+            u_99[i] = sp.interpolate.interp1d(y, u[i,:], kind='cubic', bounds_error=True)(d99_)
+        
+        # === avg in [x]/[s1] --> leave [y]/[s2]
+        
+        psvel = np.mean( psvel , axis=0 )
+        u     = np.mean( u     , axis=0 )
+        rho   = np.mean( rho   , axis=0 )
+        
+        psvel_edge  = np.mean( psvel_edge )
+        u_edge      = np.mean( u_edge     )
+        rho_edge    = np.mean( rho_edge   )
+        mu_edge     = np.mean( mu_edge    )
+        nu_edge     = np.mean( nu_edge    )
+        T_edge      = np.mean( T_edge     )
+        
+        y_edge      = np.mean( y_edge     )
+        d99         = np.mean( d99        )
+        
+        u_99        = np.mean( u_99      )
+        
+        sc_l_out = d99
+        sc_u_out = u_99
+        sc_t_out = d99/u_99
+        np.testing.assert_allclose(sc_t_out, sc_l_out/sc_u_out, rtol=1e-14, atol=1e-14)
+        
+        sc_u_in = u_tau
+        sc_l_in = nu_wall / u_tau
+        sc_t_in = nu_wall / u_tau**2
+        np.testing.assert_allclose(sc_t_in, sc_l_in/sc_u_in, rtol=1e-14, atol=1e-14)
+        
+        t_meas = self.duration_avg * (self.lchar / self.U_inf)
+        t_eddy = t_meas / (d99/u_tau)
+        
+        # === get 0D BL integral quantities
+        
+        dd = calc_bl_integral_quantities_1d( y=y,
+                                             u=u,
+                                             rho=rho,
+                                             u_tau=u_tau,
+                                             d99=d99,
+                                             y_edge=y_edge,
+                                             rho_edge=rho_edge,
+                                             nu_edge=nu_edge,
+                                             u_edge=u_edge,
+                                             nu_wall=nu_wall,
+                                            )
+        
+        # === add to file
+        
+        gn = 'data_dim'
+        
+        ## if group already exists in file, delete it entirely
+        if (gn in self):
+            del self[gn]
+        
+        ## 1D
+        self.create_dataset(f'{gn}/psvel' , data=psvel , chunks=None)
+        self.create_dataset(f'{gn}/u'     , data=u     , chunks=None)
+        self.create_dataset(f'{gn}/rho'   , data=rho   , chunks=None)
+        
+        self.create_dataset(f'{gn}/ddy_u'   , data=ddy_u   , chunks=None)
+        self.create_dataset(f'{gn}/ddy_v'   , data=ddy_v   , chunks=None)
+        self.create_dataset(f'{gn}/ddy_T'   , data=ddy_T   , chunks=None)
+        self.create_dataset(f'{gn}/ddy_p'   , data=ddy_p   , chunks=None)
+        self.create_dataset(f'{gn}/ddy_rho' , data=ddy_rho , chunks=None)
+        
+        self.create_dataset(f'{gn}/z1d' , data=z , chunks=None)
+        self.create_dataset(f'{gn}/z'   , data=z , chunks=None)
+        
+        ## 0D
+        self.create_dataset(f'{gn}/dz0'        , data=dz0 , chunks=None)
+        self.create_dataset(f'{gn}/dt'         , data=dt  , chunks=None)
+        
+        self.create_dataset(f'{gn}/y_edge'     , data=y_edge    , chunks=None)
+        self.create_dataset(f'{gn}/d99'        , data=d99       , chunks=None)
+        self.create_dataset(f'{gn}/u_99'       , data=u_99      , chunks=None)
+        
+        self.create_dataset(f'{gn}/psvel_edge' , data=psvel_edge , chunks=None)
+        self.create_dataset(f'{gn}/u_edge'     , data=u_edge     , chunks=None)
+        self.create_dataset(f'{gn}/rho_edge'   , data=rho_edge   , chunks=None)
+        self.create_dataset(f'{gn}/mu_edge'    , data=mu_edge    , chunks=None)
+        self.create_dataset(f'{gn}/nu_edge'    , data=nu_edge    , chunks=None)
+        self.create_dataset(f'{gn}/T_edge'     , data=T_edge     , chunks=None)
+        
+        self.create_dataset(f'{gn}/u_tau'      , data=u_tau      , chunks=None)
+        
+        self.create_dataset(f'{gn}/ddy_u_wall' , data=ddy_u_wall , chunks=None )
+        self.create_dataset(f'{gn}/ddy_T_wall' , data=ddy_T_wall , chunks=None )
+        self.create_dataset(f'{gn}/rho_wall'   , data=rho_wall   , chunks=None )
+        self.create_dataset(f'{gn}/nu_wall'    , data=nu_wall    , chunks=None )
+        self.create_dataset(f'{gn}/mu_wall'    , data=mu_wall    , chunks=None )
+        self.create_dataset(f'{gn}/T_wall'     , data=T_wall     , chunks=None )
+        self.create_dataset(f'{gn}/tau_wall'   , data=tau_wall   , chunks=None )
+        self.create_dataset(f'{gn}/q_wall'     , data=q_wall     , chunks=None )
+        
+        self.create_dataset(f'{gn}/sc_u_in'    , data=sc_u_in    , chunks=None)
+        self.create_dataset(f'{gn}/sc_l_in'    , data=sc_l_in    , chunks=None)
+        self.create_dataset(f'{gn}/sc_t_in'    , data=sc_t_in    , chunks=None)
+        self.create_dataset(f'{gn}/sc_u_out'   , data=sc_u_out   , chunks=None)
+        self.create_dataset(f'{gn}/sc_l_out'   , data=sc_l_out   , chunks=None)
+        self.create_dataset(f'{gn}/sc_t_out'   , data=sc_t_out   , chunks=None)
+        
+        ## add integrated quantities (all 0D)
+        for key,val in dd.items():
+            self.create_dataset(f'{gn}/{key}', data=val, chunks=None)
+        
+        ## report
+        if verbose:
+            print(72*'-')
+            even_print('Re_τ'                      , '%0.1f'%dd['Re_tau']            )
+            even_print('Re_θ'                      , '%0.1f'%dd['Re_theta']          )
+            even_print('θ'                         , '%0.5e [m]'%dd['theta_cmp']     )
+            even_print('δ*'                        , '%0.5e [m]'%dd['dstar_cmp']     )
+            even_print('H12'                       , '%0.5f'%dd['H12']               )
+            ##
+            even_print('δ99'                       , '%0.5e [m]'%d99                 )
+            even_print('θ/δ99'                     , '%0.5f'%(dd['theta_cmp']/d99)   )
+            even_print('δ*/δ99'                    , '%0.5f'%(dd['dstar_cmp']/d99)   )
+            even_print('u_τ'                       , '%0.3f [m/s]'%u_tau             )
+            even_print('ν_wall'                    , '%0.5e [m²/s]'%nu_wall          )
+            even_print('τ_wall'                    , '%0.5e [Pa]'%tau_wall           )
+            even_print('τ_wall/q_inf'              , '%0.5e'%(tau_wall/(self.rho_inf*self.U_inf**2)) )
+            even_print('cf = 2·τ_wall/q_edge'      , '%0.5e'%(2*tau_wall/(rho_edge*u_edge**2)) )
+            even_print('t_meas'                    , '%0.5e [s]'%t_meas              )
+            even_print('t_meas/tchar'              , '%0.1f'%(t_meas/self.tchar)     )
+            even_print('t_eddy = t_meas/(δ99/u_τ)' , '%0.2f'%t_eddy                  )
+            even_print('t_meas/(δ99/u_99)'         , '%0.2f'%(t_meas/(d99/u_99))     )
+            even_print('t_meas/(20·δ99/u_99)'      , '%0.2f'%(t_meas/(20*d99/u_99))  )
+            print(72*'-')
+            even_print('sc_u_in = u_τ'               , '%0.5e [m/s]'%(sc_u_in,)  )
+            even_print('sc_l_in = δ_ν = ν_wall/u_τ'  , '%0.5e [m]'%(sc_l_in,)    )
+            even_print('sc_t_in = t_ν = ν_wall/u_τ²' , '%0.5e [s]'%(sc_t_in,)    )
+            even_print('sc_u_out = u_99'             , '%0.5e [m/s]'%(sc_u_out,) )
+            even_print('sc_l_out = δ99'              , '%0.5e [m]'%(sc_l_out,)   )
+            even_print('sc_t_out = δ99/u_99'         , '%0.5e [s]'%(sc_t_out,)   )
+        
+        # ===
+        
+        if verbose: print(72*'-')
+        if verbose: print('total time : rgd.add_mean_dimensional_data_xpln() : %s'%format_time_string((timeit.default_timer() - t_start_func)))
+        if verbose: print(72*'-')
+        
+        return
+    
+    # === unsteady
+    
     def get_prime(self, **kwargs):
         '''
         get mean-removed (prime) variables in [t]
         -----
         XI  : Reynolds primes : mean(XI)=0
         XII : Favre primes    : mean(ρ·XII)=0 --> mean(XII)≠0 !!
         '''
         
         if (self.rank==0):
             verbose = True
         else:
             verbose = False
         
+        ## assert that the opened RGD has fsubtype 'unsteady'
+        if (self.fsubtype!='unsteady'):
+            raise ValueError
+        
         if verbose: print('\n'+'rgd.get_prime()'+'\n'+72*'-')
         t_start_func = timeit.default_timer()
         
         rx = kwargs.get('rx',1)
         ry = kwargs.get('ry',1)
         rz = kwargs.get('rz',1)
         #rt = kwargs.get('rt',1)
@@ -9813,15 +10555,26 @@
         fn_rgd_mean  = kwargs.get('fn_rgd_mean',None)
         fn_rgd_prime = kwargs.get('fn_rgd_prime',None)
         sfp          = kwargs.get('scalars',None) ## scalars (for prime)
         favre        = kwargs.get('favre',True)
         reynolds     = kwargs.get('reynolds',True)
         force        = kwargs.get('force',False)
         
-        chunk_kb     = kwargs.get('chunk_kb',4*1024) ## 4 [MB]
+        chunk_kb         = kwargs.get('chunk_kb',4*1024) ## h5 chunk size: default 4 [MB]
+        chunk_constraint = kwargs.get('chunk_constraint',None) ## the 'constraint' parameter for sizing h5 chunks
+        chunk_base       = kwargs.get('chunk_base',None)
+        
+        ti_min = kwargs.get('ti_min',None)
+        
+        ## HDF5 chunk parameters (t,z,y,x)
+        if (chunk_constraint is None):
+            chunk_constraint = (1,None,None,None) ## single [t] convention
+            #chunk_constraint = (None,-1,1,-1) ## single [y] convention
+        if (chunk_base is None):
+            chunk_base = 4
         
         ## if writing Favre primes, copy over ρ --> mean(ρ·XII)=0 / mean(XII)≠0 !!
         if favre:
             copy_rho = True
         else:
             copy_rho = False
         
@@ -9829,14 +10582,17 @@
             raise AssertionError('rx*ry*rz != self.n_ranks')
         if (rx>self.nx):
             raise AssertionError('rx>self.nx')
         if (ry>self.ny):
             raise AssertionError('ry>self.ny')
         if (rz>self.nz):
             raise AssertionError('rz>self.nz')
+        if (ti_min is not None):
+            if not isinstance(ti_min, int):
+                raise TypeError('ti_min must be type int')
         
         if (sfp is None):
             sfp = self.scalars
         
         # === ranks
         
         if self.usingmpi:
@@ -9859,16 +10615,28 @@
             #rt1, rt2 = rtl[t4d[3]]; ntr = rt2 - rt1
         else:
             nxr = self.nx
             nyr = self.ny
             nzr = self.nz
             #ntr = self.nt
         
+        # === get times to take for prime
+        if (ti_min is not None):
+            ti_for_prime = np.copy( self.ti[ti_min:] )
+        else:
+            ti_for_prime = np.copy( self.ti )
+        
+        nt_prime       = ti_for_prime.shape[0]
+        t_prime_start  = self.t[ti_for_prime[0]]
+        t_prime_end    = self.t[ti_for_prime[-1]]
+        duration_prime = t_prime_end - t_prime_start
+        
         # === chunks
-        ctl_ = np.array_split(np.arange(self.nt),min(ct,self.nt))
+        #ctl_ = np.array_split(np.arange(self.nt),min(ct,self.nt))
+        ctl_ = np.array_split(ti_for_prime,min(ct,nt_prime))
         ctl  = [[b[0],b[-1]+1] for b in ctl_ ]
         
         # === mean file name (for reading)
         if (fn_rgd_mean is None):
             fname_path = os.path.dirname(self.fname)
             fname_base = os.path.basename(self.fname)
             fname_root, fname_ext = os.path.splitext(fname_base)
@@ -9894,22 +10662,35 @@
         if verbose: even_print('fn_rgd_mean'     , fn_rgd_mean   )
         if verbose: even_print('fn_rgd_prime'    , fn_rgd_prime  )
         if verbose: even_print('do Favre avg'    , str(favre)    )
         if verbose: even_print('do Reynolds avg' , str(reynolds) )
         if verbose: even_print('copy rho'        , str(copy_rho) )
         if verbose: even_print('ct'              , '%i'%ct       )
         if verbose: print(72*'-')
+        if verbose: even_print('nx','%i'%self.nx)
+        if verbose: even_print('ny','%i'%self.ny)
+        if verbose: even_print('nz','%i'%self.nz)
+        if verbose: even_print('nt','%i'%self.nt)
+        if verbose: print(72*'-')
+        if verbose: even_print('n timesteps prime','%i/%i'%(nt_prime,self.nt))
+        if verbose: even_print('t index prime start','%i'%(ti_for_prime[0],))
+        if verbose: even_print('t index prime end','%i'%(ti_for_prime[-1],))
+        if verbose: even_print('t prime start','%0.2f [-]'%(t_prime_start,))
+        if verbose: even_print('t prime end','%0.2f [-]'%(t_prime_end,))
+        if verbose: even_print('duration prime','%0.2f [-]'%(duration_prime,))
+        if verbose: print(72*'-')
         
         t_read = 0.
         t_write = 0.
         data_gb_read = 0.
         data_gb_write = 0.
         
         #data_gb      = 4*self.nx*self.ny*self.nz*self.nt / 1024**3
-        #data_gb_mean = 4*self.nx*self.ny*self.nz*1       / 1024**3
+        data_gb      = 4*self.nx*self.ny*self.nz*nt_prime / 1024**3
+        data_gb_mean = 4*self.nx*self.ny*self.nz*1       / 1024**3
         
         scalars_re = ['u','v','w','T','p','rho']
         scalars_fv = ['u','v','w','T'] ## p'' and ρ'' are never really needed
         
         scalars_re_ = []
         for scalar in scalars_re:
             if (scalar in self.scalars) and (scalar in sfp):
@@ -9927,33 +10708,39 @@
         comm_rgd_prime = MPI.COMM_WORLD
         
         with rgd(fn_rgd_prime, 'w', force=force, driver=self.driver, comm=self.comm) as hf_prime:
             
             ## initialize prime rgd from rgd
             hf_prime.init_from_rgd(self.fname)
             
+            ## add top-level attributes
+            #hf_prime.attrs['fclass'] = 'rgd'
+            hf_prime.attrs['fsubtype'] = 'prime'
+            
+            #shape  = (self.nt,self.nz,self.ny,self.nx)
+            shape  = (nt_prime,self.nz,self.ny,self.nx)
+            
             ## determine dtypes for prime file
             for scalar in self.scalars:
                 dset = self[f'data/{scalar}']
                 dtype = dset.dtype
                 if reynolds and (scalar in scalars_re):
                     hf_prime.scalars_dtypes_dict[f'{scalar}I'] = dtype
                 if favre and (scalar in scalars_fv):
                     hf_prime.scalars_dtypes_dict[f'{scalar}II'] = dtype
             
-            shape  = (self.nt,self.nz,self.ny,self.nx)
-            
             # === initialize prime datasets + rho
             
             if copy_rho:
                 
                 dtype = self.scalars_dtypes_dict['rho']
                 float_bytes = dtype.itemsize
-                chunks = rgd.chunk_sizer(nxi=shape, constraint=(1,None,None,None), size_kb=chunk_kb, base=2, data_byte=float_bytes)
-                data_gb = float_bytes*self.nx*self.ny*self.nz*self.nt / 1024**3
+                chunks = h5_chunk_sizer(nxi=shape, constraint=chunk_constraint, size_kb=chunk_kb, base=chunk_base, itemsize=float_bytes)
+                #data_gb = float_bytes*self.nx*self.ny*self.nz*self.nt / 1024**3
+                data_gb = float_bytes*self.nx*self.ny*self.nz*nt_prime / 1024**3
                 
                 if verbose:
                     even_print('initializing data/rho','%0.1f [GB]'%(data_gb,))
                 
                 dset = hf_prime.create_dataset('data/rho',
                                                shape=shape,
                                                dtype=dtype,
@@ -9967,51 +10754,53 @@
             for scalar in self.scalars:
                 
                 if reynolds:
                     if (scalar in scalars_re):
                         
                         dtype = hf_prime.scalars_dtypes_dict[f'{scalar}I']
                         float_bytes = dtype.itemsize
-                        chunks = rgd.chunk_sizer(nxi=shape, constraint=(1,None,None,None), size_kb=chunk_kb, base=2, data_byte=float_bytes)
-                        data_gb = float_bytes*self.nx*self.ny*self.nz*self.nt / 1024**3
+                        chunks = h5_chunk_sizer(nxi=shape, constraint=chunk_constraint, size_kb=chunk_kb, base=chunk_base, itemsize=float_bytes)
+                        #data_gb = float_bytes*self.nx*self.ny*self.nz*self.nt / 1024**3
+                        data_gb = float_bytes*self.nx*self.ny*self.nz*nt_prime / 1024**3
                         
                         ## if ('data/%sI'%scalar in hf_prime):
                         ##     del hf_prime['data/%sI'%scalar]
                         if verbose:
                             even_print('initializing data/%sI'%(scalar,),'%0.1f [GB]'%(data_gb,))
                         
                         dset = hf_prime.create_dataset(f'data/{scalar}I',
                                                        shape=shape,
                                                        dtype=dtype,
                                                        chunks=chunks)
-                        hf_prime.scalars.append(f'data/{scalar}I')
+                        hf_prime.scalars.append(f'{scalar}I')
                         
                         chunk_kb_ = np.prod(dset.chunks)*float_bytes / 1024. ## actual
                         if verbose:
                             even_print('chunk shape (t,z,y,x)','%s'%str(dset.chunks))
                             even_print('chunk size','%i [KB]'%int(round(chunk_kb_)))
                 
                 if favre:
                     if (scalar in scalars_fv):
                         
                         dtype = hf_prime.scalars_dtypes_dict[f'{scalar}II']
                         float_bytes = dtype.itemsize
-                        chunks = rgd.chunk_sizer(nxi=shape, constraint=(1,None,None,None), size_kb=chunk_kb, base=2, data_byte=float_bytes)
-                        data_gb = float_bytes*self.nx*self.ny*self.nz*self.nt / 1024**3
+                        chunks = h5_chunk_sizer(nxi=shape, constraint=chunk_constraint, size_kb=chunk_kb, base=chunk_base, itemsize=float_bytes)
+                        #data_gb = float_bytes*self.nx*self.ny*self.nz*self.nt / 1024**3
+                        data_gb = float_bytes*self.nx*self.ny*self.nz*nt_prime / 1024**3
                         
                         ## if ('data/%sII'%scalar in hf_prime):
                         ##     del hf_prime['data/%sII'%scalar]
                         if verbose:
                             even_print('initializing data/%sII'%(scalar,),'%0.1f [GB]'%(data_gb,))
                         
                         dset = hf_prime.create_dataset(f'data/{scalar}II',
                                                        shape=shape,
                                                        dtype=dtype,
                                                        chunks=chunks)
-                        hf_prime.scalars.append(f'data/{scalar}II')
+                        hf_prime.scalars.append(f'{scalar}II')
                         
                         chunk_kb_ = np.prod(dset.chunks)*float_bytes / 1024. ## actual
                         if verbose:
                             even_print('chunk shape (t,z,y,x)','%s'%str(dset.chunks))
                             even_print('chunk size','%i [KB]'%int(round(chunk_kb_)))
             
             if hf_prime.usingmpi: comm_rgd_prime.Barrier()
@@ -10029,21 +10818,56 @@
                 if (scalar in scalars_fv) and favre:
                     n_pbar += 1
             
             comm_rgd_mean = MPI.COMM_WORLD
             
             with rgd(fn_rgd_mean, 'r', driver=self.driver, comm=self.comm) as hf_mean:
                 
+                ## copy over 'data_dim' from mean file
+                if ('data_dim' in hf_mean):
+                    grp = hf_mean['data_dim']
+                    for dsn in grp.keys():
+                        ds = hf_mean[f'data_dim/{dsn}']
+                        data = np.copy(ds[()])
+                        #if (f'data_dim/{dsn}' in hf_prime):
+                        #    del hf_prime[f'data_dim/{dsn}']
+                        
+                        #if self.usingmpi:
+                        #    with dset.collective:
+                        #        hf_prime.create_dataset(f'data_dim/{dsn}', data=data, chunks=None)
+                        #else:
+                        #    hf_prime.create_dataset(f'data_dim/{dsn}', data=data, chunks=None)
+                        
+                        hf_prime.create_dataset(f'data_dim/{dsn}', data=data, chunks=None)
+                    
+                    if verbose:
+                        even_print('data_dim copied to prime',str(True))
+                else:
+                    if verbose:
+                        even_print('data_dim copied to prime',str(False))
+                
                 if verbose:
                     progress_bar = tqdm(total=ct*n_pbar, ncols=100, desc='prime', leave=False, file=sys.stdout)
                 
                 for ctl_ in ctl:
                     ct1, ct2 = ctl_
                     ntc = ct2 - ct1
                     
+                    #if verbose: tqdm.write(f'ct1,ct2 = {ct1:d},{ct2:d}')
+                    #if verbose: tqdm.write(f'ntc = {ntc:d}')
+                    
+                    ## chunk range for writing to file (offset from read if using ti_min)
+                    if (ti_min is not None):
+                        #ct1w,ct2w = ct1-ti_min, ct2-ti_min ## doesnt work for (-) ti_min
+                        ct1w,ct2w = ct1-ti_for_prime[0], ct2-ti_for_prime[0]
+                    else:
+                        ct1w,ct2w = ct1,ct2
+                    
+                    #if verbose: tqdm.write(f'ct1w,ct2w = {ct1w:d},{ct2w:d}')
+                    
                     if favre or copy_rho:
                         
                         ## read rho
                         dset = self['data/rho']
                         dtype = dset.dtype
                         float_bytes = dtype.itemsize
                         data_gb = float_bytes*self.nx*self.ny*self.nz*ntc / 1024**3
@@ -10071,17 +10895,19 @@
                         float_bytes = dtype.itemsize
                         data_gb = float_bytes*self.nx*self.ny*self.nz*ntc / 1024**3
                         
                         if hf_prime.usingmpi: hf_prime.comm.Barrier()
                         t_start = timeit.default_timer()
                         if self.usingmpi:
                             with dset.collective:
-                                dset[ct1:ct2,rz1:rz2,ry1:ry2,rx1:rx2] = rho.T
+                                #dset[ct1:ct2,rz1:rz2,ry1:ry2,rx1:rx2] = rho.T
+                                dset[ct1w:ct2w,rz1:rz2,ry1:ry2,rx1:rx2] = rho.T
                         else:
-                            dset[ct1:ct2,:,:,:] = rho.T
+                            #dset[ct1:ct2,:,:,:] = rho.T
+                            dset[ct1w:ct2w,:,:,:] = rho.T
                         if hf_prime.usingmpi: hf_prime.comm.Barrier()
                         t_delta = timeit.default_timer() - t_start
                         
                         t_write       += t_delta
                         data_gb_write += data_gb
                         
                         if verbose:
@@ -10164,17 +10990,19 @@
                                 float_bytes = dtype.itemsize
                                 data_gb = float_bytes * hf_prime.nx * hf_prime.ny * hf_prime.nz * ntc / 1024**3
                                 
                                 if hf_prime.usingmpi: hf_prime.comm.Barrier()
                                 t_start = timeit.default_timer()
                                 if hf_prime.usingmpi:
                                     with dset.collective:
-                                        dset[ct1:ct2,rz1:rz2,ry1:ry2,rx1:rx2] = data_prime_re.T
+                                        #dset[ct1:ct2,rz1:rz2,ry1:ry2,rx1:rx2] = data_prime_re.T
+                                        dset[ct1w:ct2w,rz1:rz2,ry1:ry2,rx1:rx2] = data_prime_re.T
                                 else:
-                                    dset[ct1:ct2,:,:,:] = data_prime_re.T
+                                    #dset[ct1:ct2,:,:,:] = data_prime_re.T
+                                    dset[ct1w:ct2w,:,:,:] = data_prime_re.T
                                 if hf_prime.usingmpi: hf_prime.comm.Barrier()
                                 t_delta = timeit.default_timer() - t_start
                                 
                                 t_write       += t_delta
                                 data_gb_write += data_gb
                                 
                                 if verbose:
@@ -10217,17 +11045,19 @@
                                 float_bytes = dtype.itemsize
                                 data_gb = float_bytes * hf_prime.nx * hf_prime.ny * hf_prime.nz * ntc / 1024**3
                                 
                                 if hf_prime.usingmpi: hf_prime.comm.Barrier()
                                 t_start = timeit.default_timer()
                                 if hf_prime.usingmpi:
                                     with dset.collective:
-                                        dset[ct1:ct2,rz1:rz2,ry1:ry2,rx1:rx2] = data_prime_fv.T
+                                        #dset[ct1:ct2,rz1:rz2,ry1:ry2,rx1:rx2] = data_prime_fv.T
+                                        dset[ct1w:ct2w,rz1:rz2,ry1:ry2,rx1:rx2] = data_prime_fv.T
                                 else:
-                                    dset[ct1:ct2,:,:,:] = data_prime_fv.T
+                                    #dset[ct1:ct2,:,:,:] = data_prime_fv.T
+                                    dset[ct1w:ct2w,:,:,:] = data_prime_fv.T
                                 if hf_prime.usingmpi: hf_prime.comm.Barrier()
                                 t_delta = timeit.default_timer() - t_start
                                 
                                 t_write       += t_delta
                                 data_gb_write += data_gb
                                 
                                 if verbose:
@@ -10241,801 +11071,38 @@
                         if self.usingmpi: self.comm.Barrier()
                         if hf_prime.usingmpi: comm_rgd_prime.Barrier()
                         if hf_mean.usingmpi: comm_rgd_mean.Barrier()
                 
                 if verbose:
                     progress_bar.close()
             
+            # === replace dims/t array in prime file (if ti_min was given)
+            if (ti_min is not None):
+                t = np.copy( self.t[ti_min:] )
+                if ('dims/t' in hf_prime):
+                    del hf_prime['dims/t']
+                hf_prime.create_dataset('dims/t', data=t)
+            
             if hf_mean.usingmpi: comm_rgd_mean.Barrier()
         if hf_prime.usingmpi: comm_rgd_prime.Barrier()
         if self.usingmpi: self.comm.Barrier()
         
         # ===
         
-        #if verbose: print(72*'-')
+        if verbose: print(72*'-')
         if verbose: even_print('time read',format_time_string(t_read))
         if verbose: even_print('time write',format_time_string(t_write))
         if verbose: even_print(fn_rgd_prime, '%0.2f [GB]'%(os.path.getsize(fn_rgd_prime)/1024**3))
         if verbose: even_print('read total avg', '%0.2f [GB]  %0.3f [s]  %0.3f [GB/s]'%(data_gb_read,t_read,(data_gb_read/t_read)))
         if verbose: even_print('write total avg', '%0.2f [GB]  %0.3f [s]  %0.3f [GB/s]'%(data_gb_write,t_write,(data_gb_write/t_write)))
         if verbose: print(72*'-')
         if verbose: print('total time : rgd.get_prime() : %s'%format_time_string((timeit.default_timer() - t_start_func)))
         if verbose: print(72*'-')
         return
     
-    def get_mean_dim(self, **kwargs):
-        '''
-        get dimensionalized [x,z] mean
-        '''
-        
-        if (self.rank==0):
-            verbose = True
-        else:
-            verbose = False
-        
-        if verbose: print('\n'+'rgd.get_mean_dim()'+'\n'+72*'-')
-        t_start_func = timeit.default_timer()
-        
-        rx = kwargs.get('rx',1)
-        ry = kwargs.get('ry',1)
-        rz = kwargs.get('rz',1)
-        rt = kwargs.get('rt',1)
-        
-        xi1ss = kwargs.get('xi1ss',0) ## only relevant for when nx > N
-        xi2ss = kwargs.get('xi2ss',-1)
-        
-        ## always only one rank in y and t!!!
-        if (ry != 1):
-            raise AssertionError('ry != 1')
-        if (rt != 1):
-            raise AssertionError('rt != 1')
-        
-        if (rx*rz != self.n_ranks):
-            raise AssertionError('rx*rz != self.n_ranks')
-        if (self.nt != 1):
-            raise AssertionError('self.nt != 1 --> rgd.get_mean_dim() should only be run on mean files, i.e. output from rgd.get_mean()')
-        if (rx>self.nx):
-            raise AssertionError('rx>self.nx')
-        if (rz>self.nz):
-            raise AssertionError('rz>self.nz')
-        
-        if self.usingmpi:
-            
-            comm4d = self.comm.Create_cart(dims=[rx,ry,rz,rt], periods=[False,False,False,False], reorder=False)
-            t4d = comm4d.Get_coords(self.rank)
-            
-            rxl_ = np.array_split(np.array(range(self.nx),dtype=np.int64),min(rx,self.nx))
-            #ryl_ = np.array_split(np.array(range(self.ny),dtype=np.int64),min(ry,self.ny))
-            rzl_ = np.array_split(np.array(range(self.nz),dtype=np.int64),min(rz,self.nz))
-            #rtl_ = np.array_split(np.array(range(self.nt),dtype=np.int64),min(rt,self.nt))
-            
-            rxl = [[b[0],b[-1]+1] for b in rxl_ ]
-            #ryl = [[b[0],b[-1]+1] for b in ryl_ ]
-            rzl = [[b[0],b[-1]+1] for b in rzl_ ]
-            #rtl = [[b[0],b[-1]+1] for b in rtl_ ]
-            
-            rx1, rx2 = rxl[t4d[0]]; nxr = rx2 - rx1
-            #ry1, ry2 = ryl[t4d[1]]; nyr = ry2 - ry1
-            rz1, rz2 = rzl[t4d[2]]; nzr = rz2 - rz1
-            #rt1, rt2 = rtl[t4d[3]]; ntr = rt2 - rt1
-            
-            nyr = self.ny
-        
-        else:
-            
-            nxr = self.nx
-            nyr = self.ny
-            nzr = self.nz
-            #ntr = self.nt
-        
-        fn_dat_mean_dim  = kwargs.get('fn_dat_mean_dim',None)
-        #fn_h5_mean_dim   = kwargs.get('fn_h5_mean_dim',None)
-        
-        # === mean (dim) file name (for writing) : .dat
-        if (fn_dat_mean_dim is None):
-            fname_path = os.path.dirname(self.fname)
-            fname_base = os.path.basename(self.fname)
-            fname_root, fname_ext = os.path.splitext(fname_base)
-            #fname_root = re.findall('io\S+_mpi_[0-9]+', fname_root)[0]
-            #fname_dat_mean_base = fname_root+'_mean_dim.dat'
-            fname_dat_mean_base = fname_root+'_dim.dat'
-            fn_dat_mean_dim = str(PurePosixPath(fname_path, fname_dat_mean_base))
-        
-        # # === mean (dim) file name (for writing) : .h5
-        # if (fn_h5_mean_dim is None):
-        #     fname_path = os.path.dirname(self.fname)
-        #     fname_base = os.path.basename(self.fname)
-        #     fname_root, fname_ext = os.path.splitext(fname_base)
-        #     fname_h5_mean_base = fname_root+'_dim.h5'
-        #     fn_h5_mean_dim = str(PurePosixPath(fname_path, fname_h5_mean_base))
-        
-        if verbose: even_print('fn_rgd_mean'     , self.fname       )
-        if verbose: even_print('fn_dat_mean_dim' , fn_dat_mean_dim  )
-        if verbose: print(72*'-')
-        
-        # ===
-        
-        data = {} ## the container dict that will be returned
-        
-        nx = self.nx ; data['nx'] = nx
-        ny = self.ny ; data['ny'] = ny
-        nz = self.nz ; data['nz'] = nz
-        
-        # === write all header attributes (and derived ones)
-        for key in self.udef:
-            data[key] = self.udef[key]
-        for key in self.udef_deriv:
-            data[key] = self.udef_deriv[key]
-        
-        xs = np.copy(self.x) ; data['xs'] = xs ## dimensionless (inlet)
-        ys = np.copy(self.y) ; data['ys'] = ys ## dimensionless (inlet)
-        zs = np.copy(self.z) ; data['zs'] = zs ## dimensionless (inlet)
-        
-        x = self.x * self.lchar ; data['x'] = x ## dimensional [m]
-        y = self.y * self.lchar ; data['y'] = y ## dimensional [m]
-        z = self.z * self.lchar ; data['z'] = z ## dimensional [m]
-        
-        ## check if constant Δz (calculate Δz+ later)
-        dz0_ = np.diff(z)[0]
-        if np.all(np.isclose(np.diff(z), dz0_, rtol=1e-7)):
-            dz0 = dz0_
-        else:
-            dz0 = None
-        dz0_ = None; del dz0_
-        data['dz0'] = dz0
-        
-        ## check if mean rgd has attr 'dt'
-        if ('dt' in self.attrs.keys()):
-            dt = self.attrs['dt']
-            if (dt is not None):
-                dt *= self.tchar
-            data['dt'] = dt
-        
-        # === 5D [scalar][x,y,z,t] structured array
-        data_scalar = np.zeros(shape=(nxr, self.ny, nzr, 1), dtype={'names':self.scalars, 'formats':self.scalars_dtypes})
-        
-        for scalar in self.scalars:
-            
-            dset = self[f'data/{scalar}']
-            dtype = self.scalars_dtypes_dict[scalar]
-            if (dset.dtype!=dtype):
-                raise ValueError
-            float_bytes = dtype.itemsize
-            
-            if self.usingmpi: self.comm.Barrier()
-            t_start = timeit.default_timer()
-            if self.usingmpi: 
-                with dset.collective:
-                    data_scalar[scalar] = dset[:,rz1:rz2,:,rx1:rx2].T
-            else:
-                data_scalar[scalar] = dset[()].T
-            if self.usingmpi: self.comm.Barrier()
-            t_delta = timeit.default_timer() - t_start
-            
-            data_gb = float_bytes * self.nx * self.ny * self.nz * self.nt / 1024**3
-            
-            if (self.rank==0):
-                even_print('read: %s'%scalar, '%0.3f [GB]  %0.3f [s]  %0.3f [GB/s]'%(data_gb,t_delta,(data_gb/t_delta)))
-        
-        # === dimensionalize
-        
-        u   =  self.U_inf                     * np.squeeze(np.copy(data_scalar['u'])   ) ; data['u']   = u
-        v   =  self.U_inf                     * np.squeeze(np.copy(data_scalar['v'])   ) ; data['v']   = v
-        w   =  self.U_inf                     * np.squeeze(np.copy(data_scalar['w'])   ) ; data['w']   = w
-        rho =  self.rho_inf                   * np.squeeze(np.copy(data_scalar['rho']) ) ; data['rho'] = rho
-        p   =  (self.rho_inf * self.U_inf**2) * np.squeeze(np.copy(data_scalar['p'])   ) ; data['p']   = p
-        T   =  self.T_inf                     * np.squeeze(np.copy(data_scalar['T'])   ) ; data['T']   = T
-        
-        umag = np.sqrt(u**2+v**2+w**2) ; data['umag'] = umag
-        mflux = umag*rho               ; data['mflux'] = mflux
-        
-        mu = (14.58e-7 * T**1.5) / (T+110.4)      ; data['mu']  = mu
-        M  = u / np.sqrt(self.kappa * self.R * T) ; data['M']   = M
-        nu = mu / rho                             ; data['nu']  = nu
-        
-        # === get gradients
-        
-        if True:
-            
-            ## dudx   = np.zeros(shape=(nxr,ny,nzr), dtype=np.float64)
-            ## dvdx   = np.zeros(shape=(nxr,ny,nzr), dtype=np.float64)
-            ## dTdx   = np.zeros(shape=(nxr,ny,nzr), dtype=np.float64)
-            ## dpdx   = np.zeros(shape=(nxr,ny,nzr), dtype=np.float64)
-            ## drhodx = np.zeros(shape=(nxr,ny,nzr), dtype=np.float64)
-            
-            dudy   = np.zeros(shape=(nxr,ny,nzr), dtype=np.float64)
-            dvdy   = np.zeros(shape=(nxr,ny,nzr), dtype=np.float64)
-            dTdy   = np.zeros(shape=(nxr,ny,nzr), dtype=np.float64)
-            dpdy   = np.zeros(shape=(nxr,ny,nzr), dtype=np.float64)
-            drhody = np.zeros(shape=(nxr,ny,nzr), dtype=np.float64)
-            
-            acc = 6
-            edge_stencil = 'half'
-            
-            ## y-gradients
-            if verbose: progress_bar = tqdm(total=(nxr*nzr), ncols=100, desc='grad', leave=False, file=sys.stdout)
-            for i in range(nxr):
-                for k in range(nzr):
-                    
-                    if True: ## these do not need to be 1D for rectilinear grids
-                        dudy[i,:,k]   = gradient(u[i,:,k]   , y, acc=acc, edge_stencil=edge_stencil)
-                        dvdy[i,:,k]   = gradient(v[i,:,k]   , y, acc=acc, edge_stencil=edge_stencil)
-                        dTdy[i,:,k]   = gradient(T[i,:,k]   , y, acc=acc, edge_stencil=edge_stencil)
-                        dpdy[i,:,k]   = gradient(p[i,:,k]   , y, acc=acc, edge_stencil=edge_stencil)
-                        drhody[i,:,k] = gradient(rho[i,:,k] , y, acc=acc, edge_stencil=edge_stencil)
-                    
-                    if False:
-                        dudy[i,:,k]   = sp.interpolate.CubicSpline(y,   u[i,:,k], bc_type='natural')(y,1)
-                        dvdy[i,:,k]   = sp.interpolate.CubicSpline(y,   v[i,:,k], bc_type='natural')(y,1)
-                        dTdy[i,:,k]   = sp.interpolate.CubicSpline(y,   T[i,:,k], bc_type='natural')(y,1)
-                        dpdy[i,:,k]   = sp.interpolate.CubicSpline(y,   p[i,:,k], bc_type='natural')(y,1)
-                        drhody[i,:,k] = sp.interpolate.CubicSpline(y, rho[i,:,k], bc_type='natural')(y,1)
-                    
-                    if False:
-                        dudy[i,:,k]   = sp.interpolate.pchip(y,   u[i,:,k])(y,1)
-                        dvdy[i,:,k]   = sp.interpolate.pchip(y,   v[i,:,k])(y,1)
-                        dTdy[i,:,k]   = sp.interpolate.pchip(y,   T[i,:,k])(y,1)
-                        dpdy[i,:,k]   = sp.interpolate.pchip(y,   p[i,:,k])(y,1)
-                        drhody[i,:,k] = sp.interpolate.pchip(y, rho[i,:,k])(y,1)
-                    
-                    if verbose: progress_bar.update()
-            
-            ## x-gradients --> only need for pseudovel --> not available (currently) in MPI implementation
-            if False:
-                for j in range(self.ny):
-                    for k in range(nzr):
-                        
-                        if True:
-                            dudx[:,j,k]   = sp.interpolate.CubicSpline(x,   u[:,j,k], bc_type='natural')(x,1)
-                            dvdx[:,j,k]   = sp.interpolate.CubicSpline(x,   v[:,j,k], bc_type='natural')(x,1)
-                            dTdx[:,j,k]   = sp.interpolate.CubicSpline(x,   T[:,j,k], bc_type='natural')(x,1)
-                            dpdx[:,j,k]   = sp.interpolate.CubicSpline(x,   p[:,j,k], bc_type='natural')(x,1)
-                            drhodx[:,j,k] = sp.interpolate.CubicSpline(x, rho[:,j,k], bc_type='natural')(x,1)
-                        
-                        if False:
-                            dudx[:,j,k]   = sp.interpolate.pchip(x,   u[:,j,k])(x,1)
-                            dvdx[:,j,k]   = sp.interpolate.pchip(x,   v[:,j,k])(x,1)
-                            dTdx[:,j,k]   = sp.interpolate.pchip(x,   T[:,j,k])(x,1)
-                            dpdx[:,j,k]   = sp.interpolate.pchip(x,   p[:,j,k])(x,1)
-                            drhodx[:,j,k] = sp.interpolate.pchip(x, rho[:,j,k])(x,1)
-                    
-                    if verbose: progress_bar.update()
-            if verbose: progress_bar.close()
-        
-        # else: ## lower order gradients
-        #     
-        #     if True:
-        #         dudy   = np.gradient(u,   y, edge_order=2, axis=1)
-        #         dvdy   = np.gradient(v,   y, edge_order=2, axis=1)
-        #         dpdy   = np.gradient(p,   y, edge_order=2, axis=1)
-        #         dTdy   = np.gradient(T,   y, edge_order=2, axis=1)
-        #         drhody = np.gradient(rho, y, edge_order=2, axis=1)
-        #     
-        #     if False:
-        #         dudx   = np.gradient(u,   x, edge_order=2, axis=0)
-        #         dvdx   = np.gradient(v,   x, edge_order=2, axis=0)
-        #         dpdx   = np.gradient(p,   x, edge_order=2, axis=0)
-        #         dTdx   = np.gradient(T,   x, edge_order=2, axis=0)
-        #         drhodx = np.gradient(rho, x, edge_order=2, axis=0)
-        
-        # ===
-        
-        if False: # no x-gradients
-            data['dudx']   = dudx  
-            data['dvdx']   = dvdx  
-            data['dTdx']   = dTdx  
-            data['dpdx']   = dpdx  
-            data['drhodx'] = drhodx
-        
-        data['dudy']   = dudy
-        data['dvdy']   = dvdy
-        data['dTdy']   = dTdy
-        data['dpdy']   = dpdy
-        data['drhody'] = drhody
-        
-        # ===
-        
-        if False:
-            vort_z = dvdx - dudy
-            data['vort_z'] = vort_z
-        
-        ## wall-adjacent values
-        dudy_wall = np.squeeze(dudy[:,0,:])
-        rho_wall  = np.squeeze(rho[:,0,:])
-        nu_wall   = np.squeeze(nu[:,0,:])
-        mu_wall   = np.squeeze(mu[:,0,:])
-        T_wall    = np.squeeze(T[:,0,:])
-        tau_wall  = mu_wall * dudy_wall
-        q_wall    = self.cp * mu_wall / self.Pr * np.squeeze(dTdy[:,0,:]) ### wall heat flux
-        
-        data['dudy_wall'] = dudy_wall
-        data['rho_wall']  = rho_wall
-        data['nu_wall']   = nu_wall
-        data['mu_wall']   = mu_wall
-        data['T_wall']    = T_wall
-        data['tau_wall']  = tau_wall
-        data['q_wall']    = q_wall
-        
-        u_tau  = np.sqrt(tau_wall/rho_wall)
-        y_plus = y[np.newaxis,:,np.newaxis] * u_tau[:,np.newaxis,:] / nu_wall[:,np.newaxis,:]
-        u_plus = u / u_tau[:,np.newaxis,:]
-        
-        data['u_tau']  = u_tau
-        data['y_plus'] = y_plus
-        data['u_plus'] = u_plus
-        
-        # === BL edge & 99 values
-        
-        j_edge     = np.zeros(shape=(nxr,nzr), dtype=np.int32)
-        y_edge     = np.zeros(shape=(nxr,nzr), dtype=np.float64)
-        u_edge     = np.zeros(shape=(nxr,nzr), dtype=np.float64)
-        v_edge     = np.zeros(shape=(nxr,nzr), dtype=np.float64)
-        w_edge     = np.zeros(shape=(nxr,nzr), dtype=np.float64)
-        T_edge     = np.zeros(shape=(nxr,nzr), dtype=np.float64)
-        p_edge     = np.zeros(shape=(nxr,nzr), dtype=np.float64)
-        rho_edge   = np.zeros(shape=(nxr,nzr), dtype=np.float64)
-        nu_edge    = np.zeros(shape=(nxr,nzr), dtype=np.float64)
-        #psvel_edge = np.zeros(shape=(nxr,nzr), dtype=np.float64)
-        M_edge     = np.zeros(shape=(nxr,nzr), dtype=np.float64)
-        
-        d99        = np.zeros(shape=(nxr,nzr), dtype=np.float64) ## δ₉₉ --> interpolated
-        d99j       = np.zeros(shape=(nxr,nzr), dtype=np.int32)   ## closest y-index to δ₉₉
-        d99g       = np.zeros(shape=(nxr,nzr), dtype=np.float64) ## δ₉₉ at nearest grid point
-        
-        u99        = np.zeros(shape=(nxr,nzr), dtype=np.float64)
-        v99        = np.zeros(shape=(nxr,nzr), dtype=np.float64)
-        w99        = np.zeros(shape=(nxr,nzr), dtype=np.float64)
-        T99        = np.zeros(shape=(nxr,nzr), dtype=np.float64)
-        p99        = np.zeros(shape=(nxr,nzr), dtype=np.float64)
-        rho99      = np.zeros(shape=(nxr,nzr), dtype=np.float64)
-        nu99       = np.zeros(shape=(nxr,nzr), dtype=np.float64)
-        #psvel99    = np.zeros(shape=(nxr,nzr), dtype=np.float64)
-        M99        = np.zeros(shape=(nxr,nzr), dtype=np.float64)
-        
-        # === get pseudo-velocity (wall-normal integration of z-vorticity)
-        if False:
-            psvel = np.zeros(shape=(nxr,nyr,nzr), dtype=np.float64)
-            if verbose: progress_bar = tqdm(total=(nxr*nzr), ncols=100, desc='psvel', leave=False, file=sys.stdout)
-            for i in range(nxr):
-                for k in range(nzr):
-                    psvel[i,:,k] = sp.integrate.cumulative_trapezoid(-1*vort_z[i,:,k], y, initial=0.)
-                    if verbose: progress_bar.update()
-            if verbose: progress_bar.close()
-            
-            psvel_ddy = np.zeros(shape=(nxr,nyr,nzr), dtype=np.float64)
-            if verbose: progress_bar = tqdm(total=(nxr*nzr), ncols=100, desc='psvel_ddy', leave=False, file=sys.stdout)
-            for i in range(nxr):
-                for k in range(nzr):
-                    psvel_ddy[i,:,k] = sp.interpolate.CubicSpline(y,psvel[i,:,k],bc_type='natural')(y,1)
-                    if verbose: progress_bar.update()
-            if verbose: progress_bar.close()
-            
-            data['psvel']     = psvel
-            data['psvel_ddy'] = psvel_ddy
-        
-        ## This parameter becomes incredibly hard to tune for different Ma, etc
-        ## - If large:
-        ##    - The ddx(j_edge) is relatively smooth, BUT it's still in a region where the gradient is still (relatively high)
-        ##       --> it is, after all, no longer really the 'edge'
-        ##    - This results in the 99 values and their dependents (i.e. Re_theta) having digital 'steps'
-        ## - If small:
-        ##    - The 99 values are relatively smooth BUT...
-        ##    - The ddx(j_edge) can be 'shock-like' and very uneven, usually producing single jumps in 99 values
-        ## - The solution:
-        ##    - First use large epsilon, THEN find point in between that point and the top boundary
-        
-        #epsilon = 1e-6
-        epsilon = 1e-3
-        
-        ## u criteria
-        if True:
-            j_edge_3 = np.zeros(shape=(nx,nz), dtype=np.int32)
-            if verbose: progress_bar = tqdm(total=(nxr*nzr), ncols=100, desc='umax', leave=False, file=sys.stdout)
-            for i in range(nxr):
-                for k in range(nzr):
-                    umax=u[i,:,k].max()
-                    for j in range(nyr):
-                        if math.isclose(u[i,j,k], umax, rel_tol=epsilon):
-                            #j_edge_3[i,k] = j
-                            j_edge_3[i,k] = np.abs(y-(y[j]+(1/8)*(y.max()-y[j]))).argmin() ## split difference to bound (distance)
-                            break
-                        if (u[i,j,k]>umax):
-                            j_edge_3[i,k] = j-1
-                            break
-                    if verbose: progress_bar.update()
-            if verbose: progress_bar.close()
-        
-        ## umag criteria
-        if False:
-            j_edge_4 = np.zeros(shape=(nx,nz), dtype=np.int32)
-            if verbose: progress_bar = tqdm(total=(nxr*nzr), ncols=100, desc='umagmax', leave=False, file=sys.stdout)
-            for i in range(nxr):
-                for k in range(nzr):
-                    umagmax=umag[i,:,k].max()
-                    for j in range(nyr):
-                        if math.isclose(umag[i,j,k], umagmax, rel_tol=epsilon):
-                            j_edge_4[i,k] = j
-                            break
-                        if (umag[i,j,k]>umagmax):
-                            j_edge_4[i,k] = j-1
-                            break
-                    if verbose: progress_bar.update()
-            if verbose: progress_bar.close()
-        
-        ## mass flux criteria
-        if False:
-            j_edge_5 = np.zeros(shape=(nx,nz), dtype=np.int32)
-            if verbose: progress_bar = tqdm(total=(nxr*nzr), ncols=100, desc='mfluxmax', leave=False, file=sys.stdout)
-            for i in range(nxr):
-                for k in range(nzr):
-                    mfluxmax = mflux[i,:,k].max()
-                    for j in range(nyr):
-                        if math.isclose(mflux[i,j,k], mfluxmax, rel_tol=epsilon):
-                            j_edge_5[i,k] = j
-                            break
-                        if (mflux[i,j,k]>mfluxmax):
-                            j_edge_5[i,k] = j-1
-                            break
-                    if verbose: progress_bar.update()
-            if verbose: progress_bar.close()
-        
-        j_edge = j_edge_3
-        #j_edge = np.amin(np.stack((j_edge_3,j_edge_4,j_edge_5)), axis=0) ## minimum of collective minima : shape [nx,nz]
-        
-        # === populate edge arrays (always grid snapped)
-        
-        for i in range(nxr):
-            for k in range(nzr):
-                je              =   j_edge[i,k]
-                y_edge[i,k]     =         y[je]
-                u_edge[i,k]     =     u[i,je,k]
-                v_edge[i,k]     =     v[i,je,k]
-                w_edge[i,k]     =     w[i,je,k]
-                T_edge[i,k]     =     T[i,je,k]
-                p_edge[i,k]     =     p[i,je,k]
-                rho_edge[i,k]   =   rho[i,je,k]
-                nu_edge[i,k]    =    nu[i,je,k]
-                #psvel_edge[i,k] = psvel[i,je,k]
-                M_edge[i,k]     =     M[i,je,k]
-        
-        data['j_edge']     = j_edge
-        data['y_edge']     = y_edge
-        data['u_edge']     = u_edge
-        data['v_edge']     = v_edge
-        data['w_edge']     = w_edge
-        data['T_edge']     = T_edge
-        data['p_edge']     = p_edge
-        data['rho_edge']   = rho_edge
-        data['nu_edge']    = nu_edge
-        #data['psvel_edge'] = psvel_edge
-        data['M_edge']     = M_edge
-        
-        # ===
-        
-        if verbose: progress_bar = tqdm(total=(nxr*nzr), ncols=100, desc='δ99', leave=False, file=sys.stdout)
-        for i in range(nxr):
-            for k in range(nzr):
-                
-                ## populate d99 arrays with default 'grid-snapped' values
-                for j in range(nyr):
-                    
-                    if False:
-                        if (psvel[i,j,k] >= 0.99*psvel_edge[i,k]):
-                            d99j[i,k] =   j-1
-                            d99[i,k]  = y[j-1]
-                            d99g[i,k] = y[j-1] ## at grid
-                            break
-                    
-                    if True:
-                        if (u[i,j,k] >= 0.99*u_edge[i,k]):
-                            d99j[i,k] =   j-1
-                            d99[i,k]  = y[j-1]
-                            d99g[i,k] = y[j-1] ## at grid
-                            break
-                
-                # === use spline interpolation to find d99
-                
-                je = j_edge[i,k]+5 ## add points for interpolation
-                
-                if False:
-                    psvel_spl = sp.interpolate.CubicSpline(y[:je],psvel[i,:je,k]-(0.99*psvel_edge[i,k]),bc_type='natural')
-                    roots = psvel_spl.roots(discontinuity=False, extrapolate=False)
-                
-                if True:
-                    u_spl = sp.interpolate.CubicSpline(y[:je],u[i,:je,k]-(0.99*u_edge[i,k]),bc_type='natural')
-                    roots = u_spl.roots(discontinuity=False, extrapolate=False)
-                    #u_spl = sp.interpolate.pchip(y[:je],u[i,:je,k]-(0.99*u_edge[i,k]))
-                    #roots = u_spl.roots(extrapolate=False,discontinuity=False)
-                
-                # === populate d99 with root, recalculate & overwrite index/snap values
-                
-                if (roots.size>0):
-                    d99_ = roots[0] ## lowest (and usually only) root
-                    if (d99_<y_edge[i,k]): ## dont let it be greater than max location
-                        d99[i,k]  =   d99_
-                        d99j[i,k] =   np.abs(y-d99_).argmin()  ## closest index to interped value
-                        d99g[i,k] = y[np.abs(y-d99_).argmin()] ## d99 at nearest grid point (overwrite)
-                    else:
-                        raise ValueError('root is > max! : xi=%i'%i)
-                else:
-                    d99_ = d99[i,k]
-                    #raise ValueError('no root found at xi=%i'%i)
-                    print('WARNING: no root was found --> taking grid snapped value')
-                    print('-->check turbx.rgd.get_mean_dim()')
-                
-                # === get other quantities @ d99
-                
-                u99[i,k]     = sp.interpolate.interp1d(y[:je],     u[i,:je,k] )(d99_)
-                rho99[i,k]   = sp.interpolate.interp1d(y[:je],   rho[i,:je,k] )(d99_)
-                nu99[i,k]    = sp.interpolate.interp1d(y[:je],    nu[i,:je,k] )(d99_)
-                T99[i,k]     = sp.interpolate.interp1d(y[:je],     T[i,:je,k] )(d99_)
-                p99[i,k]     = sp.interpolate.interp1d(y[:je],     p[i,:je,k] )(d99_)
-                v99[i,k]     = sp.interpolate.interp1d(y[:je],     v[i,:je,k] )(d99_)
-                w99[i,k]     = sp.interpolate.interp1d(y[:je],     w[i,:je,k] )(d99_)
-                #psvel99[i,k] = sp.interpolate.interp1d(y[:je], psvel[i,:je,k] )(d99_)
-                M99[i,k]     = sp.interpolate.interp1d(y[:je],     M[i,:je,k] )(d99_)
-                
-                if verbose: progress_bar.update()
-        if verbose: progress_bar.close()
-        
-        data['u99']     = u99
-        data['rho99']   = rho99
-        data['nu99']    = nu99
-        data['T99']     = T99
-        data['p99']     = p99
-        data['v99']     = v99
-        data['w99']     = w99
-        #data['psvel99'] = psvel99
-        data['M99']     = M99
-        
-        data['d99']     = d99
-        data['d99j']    = d99j
-        data['d99g']    = d99g
-        
-        if True:
-            sc_l_in  = nu_wall / u_tau
-            sc_u_in  = u_tau
-            sc_t_in  = nu_wall / u_tau**2
-            sc_l_out = d99
-            sc_u_out = u99
-            sc_t_out = d99/u99
-            
-            data['sc_l_in']  = sc_l_in
-            data['sc_u_in']  = sc_u_in
-            data['sc_t_in']  = sc_t_in
-            data['sc_l_out'] = sc_l_out
-            data['sc_u_out'] = sc_u_out
-            data['sc_t_out'] = sc_t_out
-        
-        # === θ, δ*, Re_θ, Re_τ
-        
-        Re_theta      = np.zeros(shape=(nxr,nzr), dtype=np.float64)
-        Re_theta_wall = np.zeros(shape=(nxr,nzr), dtype=np.float64)
-        Re_tau        = np.zeros(shape=(nxr,nzr), dtype=np.float64)
-        Re_d99        = np.zeros(shape=(nxr,nzr), dtype=np.float64)
-        Re_x          = np.zeros(shape=(nxr,nzr), dtype=np.float64)
-        H12           = np.zeros(shape=(nxr,nzr), dtype=np.float64)
-        H12_inc       = np.zeros(shape=(nxr,nzr), dtype=np.float64)
-        theta         = np.zeros(shape=(nxr,nzr), dtype=np.float64)
-        dstar         = np.zeros(shape=(nxr,nzr), dtype=np.float64)
-        
-        u_vd = np.zeros(shape=(nxr,ny,nzr), dtype=np.float64) ## Van Driest scaled u
-        
-        if verbose: progress_bar = tqdm(total=(nxr*nzr), ncols=100, desc='Re,θ,δ*', leave=False, file=sys.stdout)
-        for i in range(nxr):
-            for k in range(nzr):
-                je   = j_edge[i,k]
-                yl   = np.copy(     y[:je+1]   )
-                ul   = np.copy(   u[i,:je+1,k] )
-                rhol = np.copy( rho[i,:je+1,k] )
-                
-                integrand_theta_inc = (ul/u_edge[i,k])*(1-(ul/u_edge[i,k]))
-                integrand_dstar_inc = 1-(ul/u_edge[i,k])
-                theta_inc           = sp.integrate.trapezoid(integrand_theta_inc, x=yl)
-                dstar_inc           = sp.integrate.trapezoid(integrand_dstar_inc, x=yl)
-                
-                integrand_theta_cmp = (ul*rhol)/(u_edge[i,k]*rho_edge[i,k])*(1-(ul/u_edge[i,k]))
-                integrand_dstar_cmp = (1-((ul*rhol)/(u_edge[i,k]*rho_edge[i,k])))
-                theta_cmp           = sp.integrate.trapezoid(integrand_theta_cmp, x=yl)
-                dstar_cmp           = sp.integrate.trapezoid(integrand_dstar_cmp, x=yl)
-                
-                integrand_u_vd   = np.sqrt(T_wall[i,k]/T[i,:,k])
-                u_vd[i,:,k]      = sp.integrate.cumulative_trapezoid(integrand_u_vd, u[i,:,k], initial=0)
-                
-                theta[i,k]         = theta_cmp
-                dstar[i,k]         = dstar_cmp
-                H12[i,k]           = dstar_cmp/theta_cmp
-                H12_inc[i,k]       = dstar_inc/theta_inc
-                Re_tau[i,k]        = d99[i,k]*u_tau[i,k]/nu_wall[i,k]
-                Re_theta[i,k]      = theta_cmp*u_edge[i,k]/nu_edge[i,k]
-                Re_theta_wall[i,k] = rho_edge[i,k]*theta_cmp*u_edge[i,k]/mu_wall[i,k]
-                Re_d99[i,k]        = d99[i,k]*u_edge[i,k]/nu_edge[i,k]
-                Re_x[i,k]          = u_edge[i,k]*(x[i]-x[0])/nu_edge[i,k]
-                
-                if verbose: progress_bar.update()
-        if verbose: progress_bar.close()
-        
-        # ===
-        
-        data['Re_theta']      = Re_theta
-        data['Re_theta_wall'] = Re_theta_wall
-        data['Re_tau']        = Re_tau
-        data['Re_d99']        = Re_d99
-        data['Re_x']          = Re_x
-        data['H12']           = H12
-        data['H12_inc']       = H12_inc
-        data['theta']         = theta
-        data['dstar']         = dstar
-        
-        u_plus_vd = u_vd / u_tau[:,np.newaxis,:] ## Van Driest scaled velocity (wall units)
-        data['u_plus_vd'] = u_plus_vd
-        
-        # === gather/bcast the averaged data (it's small)
-        
-        if self.usingmpi:
-            
-            data2 = {}
-            for key,val in data.items():
-                
-                if isinstance(data[key], np.ndarray) and (data[key].shape==(nxr,nyr,nzr)):
-                    data2[key] = np.zeros((self.nx,self.ny,self.nz), dtype=data[key].dtype)
-                    arr = self.comm.gather([rx1,rx2,rz1,rz2, np.copy(val)], root=0)
-                    arr = self.comm.bcast(arr, root=0)
-                    for i in range(len(arr)):
-                        data2[key][arr[i][0]:arr[i][1],:,arr[i][2]:arr[i][3]] = arr[i][-1]
-                
-                elif isinstance(data[key], np.ndarray) and (data[key].shape==(nxr,nzr)):
-                    data2[key] = np.zeros((self.nx,self.nz), dtype=data[key].dtype)
-                    arr = self.comm.gather([rx1,rx2,rz1,rz2, np.copy(val)], root=0)
-                    arr = self.comm.bcast(arr, root=0)
-                    for i in range(len(arr)):
-                        data2[key][arr[i][0]:arr[i][1],arr[i][2]:arr[i][3]] = arr[i][-1]
-                
-                else:
-                    data2[key] = val
-                
-                self.comm.Barrier()
-            
-            data = None; del data
-            data = data2
-            
-            # ===
-            
-            if False: ## to check
-                for key,val in data.items():
-                    if (self.rank==0):
-                        if isinstance(data[key], np.ndarray):
-                            print('%s: %s'%(key, str(data[key].shape)))
-                        else:
-                            print('%s: %s'%(key, type(data[key])))
-        
-        # === report dimensional scales
-        
-        if verbose: print(72*'-')
-        
-        t_meas = self.duration_avg * (self.lchar / self.U_inf)
-        
-        if (nx<=20): ## if negligibly thin in [x] --> usually only the case for x-stripes
-            
-            d99_avg      = np.mean(data['d99'],      axis=(0,1)) ## avg in [x,z] --> leave 0D scalar
-            u99_avg      = np.mean(data['u99'],      axis=(0,1))
-            nu_wall_avg  = np.mean(data['nu_wall'],  axis=(0,1))
-            u_tau_avg    = np.mean(data['u_tau'],    axis=(0,1))
-            Re_tau_avg   = np.mean(data['Re_tau'],   axis=(0,1))
-            Re_theta_avg = np.mean(data['Re_theta'], axis=(0,1))
-            t_eddy = t_meas / (d99_avg/u_tau_avg)
-            
-            sc_l_in_avg  = np.mean(data['sc_l_in']  , axis=(0,1), dtype=np.float64)
-            sc_l_out_avg = np.mean(data['sc_l_out'] , axis=(0,1), dtype=np.float64)
-            sc_t_in_avg  = np.mean(data['sc_t_in']  , axis=(0,1), dtype=np.float64)
-            sc_t_out_avg = np.mean(data['sc_t_out'] , axis=(0,1), dtype=np.float64)
-            
-            if verbose:
-                even_print('Re_τ'                      , '%0.1f'%Re_tau_avg                    )
-                even_print('Re_θ'                      , '%0.1f'%Re_theta_avg                  )
-                even_print('δ99'                       , '%0.5e [m]'%d99_avg                   )
-                even_print('u_τ'                       , '%0.3f [m/s]'%u_tau_avg               )
-                even_print('ν_wall'                    , '%0.5e [m²/s]'%nu_wall_avg            )
-                even_print('t_meas'                    , '%0.5e [s]'%t_meas                    )
-                even_print('t_meas/(δ99/u_τ) = t_eddy' , '%0.2f'%t_eddy                        )
-                even_print('t_meas/(δ99/u99)'          , '%0.2f'%(t_meas/(d99_avg/u99_avg))    )
-                even_print('t_meas/(20·δ99/u99)'       , '%0.2f'%(t_meas/(20*d99_avg/u99_avg)) )
-                
-                if ( dz0 is not None ):
-                    even_print('Δz+' , '%0.3f'%(dz0/sc_l_in_avg) )
-                if ( dt is not None ):
-                    even_print('Δt+' , '%0.3f'%(dt/sc_t_in_avg) )
-        
-        else:
-            
-            d99_x       = np.mean(data['d99']      , axis=(1,)) ## avg in [z] --> leave [x]
-            u99_x       = np.mean(data['u99']      , axis=(1,))
-            nu_wall_x   = np.mean(data['nu_wall']  , axis=(1,))
-            u_tau_x     = np.mean(data['u_tau']    , axis=(1,))
-            Re_tau_x    = np.mean(data['Re_tau']   , axis=(1,))
-            Re_theta_x  = np.mean(data['Re_theta'] , axis=(1,))
-            sc_l_in_x   = np.mean(data['sc_l_in']  , axis=(1,))
-            sc_u_in_x   = np.mean(data['sc_u_in']  , axis=(1,))
-            sc_t_in_x   = np.mean(data['sc_t_in']  , axis=(1,))
-            sc_l_out_x  = np.mean(data['sc_l_out'] , axis=(1,))
-            sc_u_out_x  = np.mean(data['sc_u_out'] , axis=(1,))
-            sc_t_out_x  = np.mean(data['sc_t_out'] , axis=(1,))
-            
-            d99_x_end   = d99_x[xi2ss]
-            u_tau_x_end = u_tau_x[xi2ss]
-            u99_x_end   = u99_x[xi2ss]
-            x_range     = x[xi2ss]-x[xi1ss]
-            z_range     = z[xi2ss]-z[xi1ss]
-            t_eddy_end  = t_meas / ( d99_x_end / u_tau_x_end)
-            
-            sc_l_in_growth_fac   = (sc_l_in_x[xi2ss]  - sc_l_in_x[xi1ss])  / sc_l_in_x[xi2ss]
-            sc_u_in_growth_fac   = (sc_u_in_x[xi2ss]  - sc_u_in_x[xi1ss])  / sc_u_in_x[xi2ss]
-            sc_t_in_growth_fac   = (sc_t_in_x[xi2ss]  - sc_t_in_x[xi1ss])  / sc_t_in_x[xi2ss]
-            sc_l_out_growth_fac  = (sc_l_out_x[xi2ss] - sc_l_out_x[xi1ss]) / sc_l_out_x[xi2ss]
-            sc_u_out_growth_fac  = (sc_u_out_x[xi2ss] - sc_u_out_x[xi1ss]) / sc_u_out_x[xi2ss]
-            sc_t_out_growth_fac  = (sc_t_out_x[xi2ss] - sc_t_out_x[xi1ss]) / sc_t_out_x[xi2ss]
-            
-            if verbose:
-                even_print( 'xi1ss', '%i'%xi1ss )
-                even_print( 'xi2ss', '%i'%xi2ss )
-                ##
-                even_print( 'x min:max' , '%0.5e : %0.5e'%(x.min(),x.max()) )
-                even_print( 'y min:max' , '%0.5e : %0.5e'%(y.min(),y.max()) )
-                even_print( 'z min:max' , '%0.5e : %0.5e'%(z.min(),z.max()) )
-                ##
-                even_print( 'x/lchar min:max' , '%0.6f : %0.6f'%(x.min()/self.lchar , x.max()/self.lchar) )
-                even_print( 'y/lchar min:max' , '%0.6f : %0.6f'%(y.min()/self.lchar , y.max()/self.lchar) )
-                even_print( 'z/lchar min:max' , '%0.6f : %0.6f'%(z.min()/self.lchar , z.max()/self.lchar) )
-                ##
-                even_print( 'x_range', '%0.5e [m]'%x_range )
-                even_print( 'x_range/lchar', '%0.2f'%(x_range/self.lchar) )
-                even_print( 'x_range/δ99 @ end', '%0.2f'%(x_range/d99_x_end) )
-                even_print( 'z_range/δ99 @ end', '%0.2f'%(z_range/d99_x_end) )
-                ##
-                print(72*'-')
-                even_print( 'rdiff(x) : ℓ_in  = ν_wall/u_τ'  , '%+0.6f'%sc_l_in_growth_fac  )
-                even_print( 'rdiff(x) : u_in  = u_τ'         , '%+0.6f'%sc_u_in_growth_fac  )
-                even_print( 'rdiff(x) : t_in  = ν_wall/u_τ²' , '%+0.6f'%sc_t_in_growth_fac  )
-                even_print( 'rdiff(x) : ℓ_out = δ99'         , '%+0.6f'%sc_l_out_growth_fac )
-                even_print( 'rdiff(x) : u_out = u99'         , '%+0.6f'%sc_u_out_growth_fac )
-                even_print( 'rdiff(x) : t_out = d99/u99'     , '%+0.6f'%sc_t_out_growth_fac )
-                ##
-                print(72*'-')
-                even_print('Re_τ @ end'   , '%0.1f'%Re_tau_x[xi2ss] )
-                even_print('Re_θ @ end'   , '%0.1f'%Re_theta_x[xi2ss] )
-                even_print('δ99 @ end'    , '%0.5e [m]'%d99_x[xi2ss] )
-                even_print('u_τ @ end'    , '%0.3f [m/s]'%u_tau_x[xi2ss] )
-                even_print('ν_wall @ end' , '%0.5e [m²/s]'%nu_wall_x[xi2ss] )
-                print(72*'-')
-                ##
-                even_print('t_meas'                                , '%0.5e [s]'%t_meas )
-                even_print('t_meas/(δ99/u_τ) = t_eddy @ end'       , '%0.2f'%t_eddy_end )
-                even_print('t_meas/(δ99/u99) @ end'                , '%0.2f'%(t_meas/(d99_x_end/u99_x_end)) )
-                even_print('t_meas/(20·δ99/u99) @ end'             , '%0.2f'%(t_meas/(20*d99_x_end/u99_x_end)) )
-                even_print('t_meas/(x_range/U_inf) = n flowpasses' , '%0.2f'%(t_meas/(x_range/self.U_inf)) )
-        
-        if verbose: print(72*'-')
-        
-        # ===
-        
-        if (self.rank==0):
-            with open(fn_dat_mean_dim,'wb') as f:
-                pickle.dump(data,f,protocol=4)
-            size = os.path.getsize(fn_dat_mean_dim)
-        
-        if self.usingmpi: self.comm.Barrier()
-        if verbose: even_print(fn_dat_mean_dim, '%0.2f [GB]'%(os.path.getsize(fn_dat_mean_dim)/1024**3))
-        if verbose: print(72*'-')
-        
-        if verbose: print('\n'+72*'-')
-        if verbose: print('total time : rgd.get_mean_dim() : %s'%format_time_string((timeit.default_timer() - t_start_func)))
-        if verbose: print(72*'-')
-        
-        return
-    
     def calc_lambda2(self, **kwargs):
         '''
         calculate λ-2 & Q
         Jeong & Hussain (1996) : https://doi.org/10.1017/S0022112095000462
         '''
         
         if (self.rank==0):
@@ -11212,15 +11279,15 @@
         #dtype = self.scalars_dtypes_dict['u']
         dset = self['data/u']
         dtype = dset.dtype
         float_bytes = dtype.itemsize
         data_gb = float_bytes*self.nt*self.nz*self.ny*self.nx / 1024**3
         
         shape  = (self.nt,self.nz,self.ny,self.nx)
-        chunks = rgd.chunk_sizer(nxi=shape, constraint=(1,None,None,None), size_kb=chunk_kb, base=2, data_byte=float_bytes)
+        chunks = h5_chunk_sizer(nxi=shape, constraint=(1,None,None,None), size_kb=chunk_kb, base=4, itemsize=float_bytes)
         
         # === initialize 4D arrays in HDF5
         
         if save_lambda2:
             if verbose: even_print('initializing data/lambda2','%0.2f [GB]'%(data_gb,))
             if ('data/lambda2' in self):
                 del self['data/lambda2']
@@ -11486,14 +11553,586 @@
         #if verbose: print('\n'+72*'-')
         if verbose: print(72*'-')
         if verbose: print('total time : turbx.rgd.calc_lambda2() : %s'%format_time_string((timeit.default_timer() - t_start_func)))
         if verbose: print(72*'-')
         
         return
     
+    # ===
+    
+    def calc_high_order_stats(self,**kwargs):
+        '''
+        calculate high-order statistical quantities
+        - skewness
+        - kurtosis / 'flatness'
+        - probability distribution function (PDF)
+        '''
+        
+        if (self.rank==0):
+            verbose = True
+        else:
+            verbose = False
+        
+        ## assert that the opened RGD has fsubtype 'unsteady'
+        if (self.fsubtype!='unsteady'):
+            raise ValueError
+        
+        if verbose: print('\n'+'rgd.calc_high_order_stats()'+'\n'+72*'-')
+        t_start_func = timeit.default_timer()
+        
+        rx = kwargs.get('rx',1)
+        ry = kwargs.get('ry',1)
+        rz = kwargs.get('rz',1)
+        rt = kwargs.get('rt',1)
+        
+        fn_dat_hos  = kwargs.get('fn_dat_hos',None) ## hos = 'high-order stats'
+        fn_rgd_mean = kwargs.get('fn_rgd_mean',None)
+        n_bins      = kwargs.get('n_bins',1024) ## n bins for histogram (PDF) calculation
+        
+        ## for now only distribute data in [y] --> allows [x,z] mean before Send/Recv
+        if (rx!=1):
+            raise AssertionError('rx!=1')
+        if (rz!=1):
+            raise AssertionError('rz!=1')
+        if (rt!=1):
+            raise AssertionError('rt!=1')
+        
+        if (rx*ry*rz*rt != self.n_ranks):
+            raise AssertionError('rx*ry*rz*rt != self.n_ranks')
+        if (rx>self.nx):
+            raise AssertionError('rx>self.nx')
+        if (ry>self.ny):
+            raise AssertionError('ry>self.ny')
+        if (rz>self.nz):
+            raise AssertionError('rz>self.nz')
+        if (rt>self.nt):
+            raise AssertionError('rt>self.nt')
+        
+        # ===
+        
+        #comm4d = self.comm.Create_cart(dims=[rx,ry,ry,rt], periods=[False,False,False,False], reorder=False)
+        #t4d = comm4d.Get_coords(self.rank)
+        
+        #rxl_ = np.array_split(np.array(range(self.nx),dtype=np.int64),min(rx,self.nx))
+        ryl_ = np.array_split(np.array(range(self.ny),dtype=np.int64),min(ry,self.ny))
+        #rzl_ = np.array_split(np.array(range(self.nz),dtype=np.int64),min(rz,self.nz))
+        #rtl_ = np.array_split(np.array(range(self.nt),dtype=np.int64),min(rt,self.nt))
+
+        #rxl = [[b[0],b[-1]+1] for b in rxl_ ]
+        ryl = [[b[0],b[-1]+1] for b in ryl_ ]
+        #rzl = [[b[0],b[-1]+1] for b in rzl_ ]
+        #rtl = [[b[0],b[-1]+1] for b in rtl_ ]
+        
+        #rx1, rx2 = rxl[t4d[0]]; nxr = rx2 - rx1
+        #ry1, ry2 = ryl[t4d[1]]; nyr = ry2 - ry1
+        #rz1, rz2 = rzl[t4d[2]]; nzr = rz2 - rz1
+        #rt1, rt2 = rtl[t4d[3]]; ntr = rt2 - rt1
+        
+        ry1,ry2 = ryl[self.rank]; nyr = ry2 - ry1
+        
+        # === mean file name (for reading)
+        if (fn_rgd_mean is None):
+            fname_path = os.path.dirname(self.fname)
+            fname_base = os.path.basename(self.fname)
+            fname_root, fname_ext = os.path.splitext(fname_base)
+            fname_mean_h5_base = fname_root+'_mean.h5'
+            #fn_rgd_mean = os.path.join(fname_path, fname_mean_h5_base)
+            fn_rgd_mean = str(PurePosixPath(fname_path, fname_mean_h5_base))
+            #fn_rgd_mean = Path(fname_path, fname_mean_h5_base)
+        
+        # # === mean (dimensional) file name (for reading) : .dat
+        # if (fn_dat_mean_dim is None):
+        #     fname_path = os.path.dirname(self.fname)
+        #     fname_base = os.path.basename(self.fname)
+        #     fname_root, fname_ext = os.path.splitext(fname_base)
+        #     fname_root = re.findall('io\S+_mpi_[0-9]+', fname_root)[0]
+        #     fname_dat_mean_base = fname_root+'_mean_dim.dat'
+        #     fn_dat_mean_dim = str(PurePosixPath(fname_path, fname_dat_mean_base))
+        
+        # === high-order stats ('hos') file name (for writing) : dat
+        if (fn_dat_hos is None):
+            fname_path = os.path.dirname(self.fname)
+            fname_base = os.path.basename(self.fname)
+            fname_root, fname_ext = os.path.splitext(fname_base)
+            fname_root = re.findall('io\S+_mpi_[0-9]+', fname_root)[0]
+            fname_hos_dat_base = fname_root+'_hos.dat'
+            fn_dat_hos = str(PurePosixPath(fname_path, fname_hos_dat_base))
+        
+        # ===
+        
+        if verbose: even_print( 'fn_rgd_mean'  , fn_rgd_mean )
+        if verbose: even_print( 'fn_rgd'       , self.fname  )
+        if verbose: even_print( 'fn_dat_hos'   , fn_dat_hos  )
+        if verbose: print(72*'-')
+        
+        # if not os.path.isfile(fn_dat_mean_dim):
+        #     raise FileNotFoundError('%s not found!'%fn_dat_mean_dim)
+        
+        if False: ## open mean (dimensional) data : .dat
+            
+            with open(fn_dat_mean_dim,'rb') as f:
+                data_mean_dim = pickle.load(f)
+            fmd = type('foo', (object,), data_mean_dim)
+            
+            self.comm.Barrier()
+            
+            ## the data dictionary to be pickled later
+            data = {}
+            
+            ## 2D dimensional quantities --> [x,z]
+            u_tau    = fmd.u_tau    # ; data['u_tau']    = u_tau
+            nu_wall  = fmd.nu_wall  # ; data['nu_wall']  = nu_wall
+            rho_wall = fmd.rho_wall # ; data['rho_wall'] = rho_wall
+            d99      = fmd.d99      # ; data['d99']      = d99
+            u99      = fmd.u99      # ; data['u99']      = u99
+            Re_tau   = fmd.Re_tau   # ; data['Re_tau']   = Re_tau
+            Re_theta = fmd.Re_theta # ; data['Re_theta'] = Re_theta
+            
+            ## mean [x,z] --> leave 0D scalar
+            u_tau_avg    = np.mean(fmd.u_tau    , axis=(0,1)) ; data['u_tau_avg']    = u_tau_avg
+            nu_wall_avg  = np.mean(fmd.nu_wall  , axis=(0,1)) ; data['nu_wall_avg']  = nu_wall_avg
+            rho_wall_avg = np.mean(fmd.rho_wall , axis=(0,1)) ; data['rho_wall_avg'] = rho_wall_avg
+            d99_avg      = np.mean(fmd.d99      , axis=(0,1)) ; data['d99_avg']      = d99_avg
+            u99_avg      = np.mean(fmd.u99      , axis=(0,1)) ; data['u99_avg']      = u99_avg
+            Re_tau_avg   = np.mean(fmd.Re_tau   , axis=(0,1)) ; data['Re_tau_avg']   = Re_tau_avg
+            Re_theta_avg = np.mean(fmd.Re_theta , axis=(0,1)) ; data['Re_theta_avg'] = Re_theta_avg
+            
+            ## mean [x,z] --> leave 1D [y]
+            rho_avg = np.mean(fmd.rho,axis=(0,2))
+            data['rho_avg'] = rho_avg
+            
+            # === 2D inner scales --> [x,z]
+            sc_l_in = nu_wall / u_tau
+            sc_u_in = u_tau
+            sc_t_in = nu_wall / u_tau**2
+            
+            # === 2D outer scales --> [x,z]
+            sc_l_out = d99
+            sc_u_out = u99
+            sc_t_out = d99/u99
+            
+            # === check
+            np.testing.assert_allclose(fmd.lchar   , self.lchar   , rtol=1e-8)
+            np.testing.assert_allclose(fmd.U_inf   , self.U_inf   , rtol=1e-8)
+            np.testing.assert_allclose(fmd.rho_inf , self.rho_inf , rtol=1e-8)
+            np.testing.assert_allclose(fmd.T_inf   , self.T_inf   , rtol=1e-8)
+            np.testing.assert_allclose(fmd.nx      , self.nx      , rtol=1e-8)
+            np.testing.assert_allclose(fmd.ny      , self.ny      , rtol=1e-8)
+            np.testing.assert_allclose(fmd.nz      , self.nz      , rtol=1e-8)
+            np.testing.assert_allclose(fmd.xs      , self.x       , rtol=1e-8)
+            np.testing.assert_allclose(fmd.ys      , self.y       , rtol=1e-8)
+            np.testing.assert_allclose(fmd.zs      , self.z       , rtol=1e-8)
+            
+            lchar   = self.lchar   ; data['lchar']   = lchar
+            U_inf   = self.U_inf   ; data['U_inf']   = U_inf
+            rho_inf = self.rho_inf ; data['rho_inf'] = rho_inf
+            T_inf   = self.T_inf   ; data['T_inf']   = T_inf
+            
+            data['Ma'] = self.Ma
+            data['Pr'] = self.Pr
+            
+            nx = self.nx ; data['nx'] = nx
+            ny = self.ny ; data['ny'] = ny
+            nz = self.nz ; data['nz'] = nz
+            nt = self.nt ; data['nt'] = nt
+            
+            ## dimless (inlet)
+            xd = self.x
+            yd = self.y
+            zd = self.z
+            td = self.t
+            
+            ## dimensional [m] / [s]
+            x      = self.x * lchar
+            y      = self.y * lchar
+            z      = self.z * lchar
+            t      = self.t * (lchar/U_inf)
+            t_meas = t[-1]-t[0]
+            dt     = self.dt * (lchar/U_inf)
+            
+            data['x'] = x
+            data['y'] = y
+            data['z'] = z
+            data['t'] = t
+            data['t_meas'] = t_meas
+            data['dt'] = dt
+            
+            np.testing.assert_equal(nx,x.size)
+            np.testing.assert_equal(ny,y.size)
+            np.testing.assert_equal(nz,z.size)
+            np.testing.assert_equal(nt,t.size)
+            np.testing.assert_allclose(dt, t[1]-t[0], rtol=1e-8)
+            
+            # === report
+            if verbose:
+                even_print('nx'     , '%i'        %nx     )
+                even_print('ny'     , '%i'        %ny     )
+                even_print('nz'     , '%i'        %nz     )
+                even_print('nt'     , '%i'        %nt     )
+                even_print('dt'     , '%0.5e [s]' %dt     )
+                even_print('t_meas' , '%0.5e [s]' %t_meas )
+                print(72*'-')
+            
+            if verbose:
+                even_print('Re_τ'   , '%0.1f'         % Re_tau_avg   )
+                even_print('Re_θ'   , '%0.1f'         % Re_theta_avg )
+                even_print('δ99'    , '%0.5e [m]'     % d99_avg      )
+                even_print('U_inf'  , '%0.3f [m/s]'   % U_inf        )
+                even_print('u_τ'    , '%0.3f [m/s]'   % u_tau_avg    )
+                even_print('ν_wall' , '%0.5e [m²/s]'  % nu_wall_avg  )
+                even_print('ρ_wall' , '%0.6f [kg/m³]' % rho_wall_avg  )
+                print(72*'-')
+            
+            t_eddy = t_meas / ( d99_avg / u_tau_avg )
+            
+            if verbose:
+                even_print('t_meas/(δ99/u_τ) = t_eddy' , '%0.2f'%t_eddy)
+                even_print('t_meas/(δ99/u99)'          , '%0.2f'%(t_meas/(d99_avg/u99_avg)))
+                even_print('t_meas/(20·δ99/u99)'       , '%0.2f'%(t_meas/(20*d99_avg/u99_avg)))
+                print(72*'-')
+        
+        self.comm.Barrier()
+        
+        ## the data dictionary to be pickled later
+        data = {}
+        
+        if True: ## open mean (dimensional) data : from mean .h5
+            
+            with rgd(fn_rgd_mean, 'r', driver=self.driver, comm=self.comm) as hf_mean:
+                
+                ## assert that the opened RGD has fsubtype 'mean'
+                if (hf_mean.fsubtype!='mean'):
+                    raise ValueError
+                
+                ## assert that 'data_dim' is present in mean file
+                if ('data_dim' not in hf_mean):
+                    raise ValueError(f'group data_dim not present in {fn_rgd_mean}')
+                
+                ## put all data from 'data_dim' into the dictionary data which will be pickled at the end
+                for dsn in hf_mean['data_dim'].keys():
+                    d_ = np.copy( hf_mean[f'data_dim/{dsn}'][()] )
+                    if (d_.ndim == 0):
+                        d_ = float(d_)
+                    data[dsn] = d_
+                
+                ## 1D
+                rho_avg = np.copy( hf_mean['data_dim/rho'][()] )
+                u_avg   = np.copy( hf_mean['data_dim/u'][()]   )
+                
+                ## 0D
+                u_tau    = float( hf_mean['data_dim/u_tau'][()]    )
+                nu_wall  = float( hf_mean['data_dim/nu_wall'][()]  )
+                rho_wall = float( hf_mean['data_dim/rho_wall'][()] )
+                d99      = float( hf_mean['data_dim/d99'][()]      )
+                u_99     = float( hf_mean['data_dim/u_99'][()]     )
+                Re_tau   = float( hf_mean['data_dim/Re_tau'][()]   )
+                Re_theta = float( hf_mean['data_dim/Re_theta'][()] )
+                sc_u_in  = float( hf_mean['data_dim/sc_u_in'][()]  )
+                sc_l_in  = float( hf_mean['data_dim/sc_l_in'][()]  )
+                sc_t_in  = float( hf_mean['data_dim/sc_t_in'][()]  )
+                sc_u_out = float( hf_mean['data_dim/sc_u_out'][()] )
+                sc_l_out = float( hf_mean['data_dim/sc_l_out'][()] )
+                sc_t_out = float( hf_mean['data_dim/sc_t_out'][()] )
+                
+                ## these are recalculated and checked in next step
+                z1d_ = np.copy( hf_mean['data_dim/z1d'][()] )
+                dz0_ = np.copy( hf_mean['data_dim/dz0'][()] )
+                dt_  = np.copy( hf_mean['data_dim/dt'][()]  )
+        
+        ## get size of infile
+        fsize = os.path.getsize(self.fname)/1024**3
+        if verbose: even_print(os.path.basename(self.fname),'%0.1f [GB]'%fsize)
+        if verbose: even_print('nx','%i'%self.nx)
+        if verbose: even_print('ny','%i'%self.ny)
+        if verbose: even_print('nz','%i'%self.nz)
+        if verbose: even_print('nt','%i'%self.nt)
+        if verbose: even_print('ngp','%0.1f [M]'%(self.ngp/1e6,))
+        if verbose: print(72*'-')
+        
+        ## 0D scalars
+        lchar   = self.lchar   ; data['lchar']   = lchar
+        U_inf   = self.U_inf   ; data['U_inf']   = U_inf
+        rho_inf = self.rho_inf ; data['rho_inf'] = rho_inf
+        T_inf   = self.T_inf   ; data['T_inf']   = T_inf
+        
+        #data['M_inf'] = self.M_inf
+        data['Ma'] = self.Ma
+        data['Pr'] = self.Pr
+        
+        ## read in 1D coordinate arrays, then re-dimensionalize [m]
+        x = np.copy( self['dims/x'][()] * self.lchar )
+        y = np.copy( self['dims/y'][()] * self.lchar )
+        z = np.copy( self['dims/z'][()] * self.lchar )
+        
+        nx = self.nx ; data['nx'] = nx
+        ny = self.ny ; data['ny'] = ny
+        nz = self.nz ; data['nz'] = nz
+        nt = self.nt ; data['nt'] = nt
+        
+        t = np.copy( self['dims/t'][()] * self.tchar )
+        
+        # ## dimless (inlet/characteristic)
+        # xd = self.x
+        # yd = self.y
+        # zd = self.z
+        # td = self.t
+        
+        ## redimensionalize coordinates --> [m],[s],[m/s],etc.
+        x      = self.x * lchar
+        y      = self.y * lchar
+        z      = self.z * lchar
+        t      = self.t * (lchar/U_inf)
+        t_meas = t[-1]-t[0]
+        dt     = self.dt * (lchar/U_inf)
+        
+        z1d = np.copy(z)
+        
+        ## check if constant Δz (calculate Δz+ later)
+        dz0 = np.diff(z1d)[0]
+        if not np.all(np.isclose(np.diff(z1d), dz0, rtol=1e-7)):
+            raise NotImplementedError
+        
+        ## dimensional [s]
+        dt = self.dt * self.tchar
+        np.testing.assert_allclose(dt, t[1]-t[0], rtol=1e-14, atol=1e-14)
+        
+        t_meas = self.duration * self.tchar
+        np.testing.assert_allclose(t_meas, t.max()-t.min(), rtol=1e-14, atol=1e-14)
+        
+        ## check against values in 'data_dim' (imported above)
+        np.testing.assert_allclose(dt  , dt_  , rtol=1e-14, atol=1e-14)
+        np.testing.assert_allclose(dz0 , dz0_ , rtol=1e-14, atol=1e-14)
+        np.testing.assert_allclose(z1d , z1d_ , rtol=1e-14, atol=1e-14)
+        
+        zrange = z1d.max() - z1d.min()
+        #zrange = z[-1]-z[0]
+        
+        data['x'] = x
+        data['y'] = y
+        data['z'] = z
+        #data['z1d'] = z1d
+        
+        data['t'] = t
+        data['t_meas'] = t_meas
+        data['dt'] = dt
+        data['dz0'] = dz0
+        data['zrange'] = zrange
+        
+        if verbose: even_print('Δt/tchar','%0.8f'%(dt/self.tchar))
+        if verbose: even_print('Δt','%0.3e [s]'%(dt,))
+        if verbose: even_print('duration/tchar','%0.1f'%(self.duration,))
+        if verbose: even_print('duration','%0.3e [s]'%(self.duration*self.tchar,))
+        if verbose: print(72*'-')
+        
+        ## report
+        if verbose:
+            even_print('dt'     , '%0.5e [s]' % dt      )
+            even_print('t_meas' , '%0.5e [s]' % t_meas  )
+            even_print('dz0'    , '%0.5e [m]' % dz0     )
+            even_print('zrange' , '%0.5e [m]' % zrange  )
+            print(72*'-')
+        
+        ## report
+        if verbose:
+            even_print('Re_τ'    , '%0.1f'        % Re_tau    )
+            even_print('Re_θ'    , '%0.1f'        % Re_theta  )
+            even_print('δ99'     , '%0.5e [m]'    % d99       )
+            even_print('δ_ν=(ν_wall/u_τ)' , '%0.5e [m]' % sc_l_in )
+            even_print('U_inf'  , '%0.3f [m/s]'   % self.U_inf )
+            even_print('u_τ'    , '%0.3f [m/s]'   % u_tau     )
+            even_print('ν_wall' , '%0.5e [m²/s]'  % nu_wall   )
+            even_print('ρ_wall' , '%0.6f [kg/m³]' % rho_wall  )
+            ##
+            even_print('Δz+'        , '%0.3f'%(dz0/sc_l_in) )
+            even_print('zrange/δ99' , '%0.3f'%(zrange/d99)  )
+            even_print('Δt+'        , '%0.3f'%(dt/sc_t_in)  )
+            print(72*'-')
+        
+        t_eddy = t_meas / ( d99 / u_tau )
+        
+        if verbose:
+            even_print('t_meas/(δ99/u_τ) = t_eddy' , '%0.2f'%t_eddy)
+            even_print('t_meas/(δ99/u99)'          , '%0.2f'%(t_meas/(d99/u_99)))
+            even_print('t_meas/(20·δ99/u99)'       , '%0.2f'%(t_meas/(20*d99/u_99)))
+        
+        # ===
+        
+        scalars = [ 'u', 'v', 'w', 'T' ]
+        scalars_dtypes = [ self.scalars_dtypes_dict[s] for s in scalars ]
+        n_scalars = len(scalars)
+        
+        ## dtype of unsteady data (currently must be all same dtype)
+        if np.all( [ (dtp==np.float32) for dtp in scalars_dtypes ] ):
+            dtype_unsteady = np.float32
+            float_bytes = 4
+        elif np.all( [ (dtp==np.float64) for dtp in scalars_dtypes ] ):
+            dtype_unsteady = np.float64
+            float_bytes = 8
+        else:
+            raise NotImplementedError('primes dont all have same dtype --> needs update')
+        
+        ## initialize buffers
+        hos_scalars = [ f'{s}_mean'    for s in scalars ] + \
+                      [ f'{s}I_median' for s in scalars ] + \
+                      [ f'{s}_std'     for s in scalars ] + \
+                      [ f'{s}_skew'    for s in scalars ] + \
+                      [ f'{s}_kurt'    for s in scalars ]
+        
+        hos_scalars_dtypes = [ np.float64 for s in hos_scalars ]
+        #hos                = np.zeros(shape=(self.nx, nyr, self.nz) , dtype={'names':hos_scalars, 'formats':hos_scalars_dtypes})
+        hos                = np.zeros(shape=(nyr,) , dtype={'names':hos_scalars, 'formats':hos_scalars_dtypes})
+        
+        hist_scalars = [ '%s'%(s,) for s in scalars ]
+        hist_scalars_dtypes = [ np.float64 for s in hist_scalars ]
+        hist = np.zeros(shape=(nyr, n_bins) , dtype={'names':hist_scalars, 'formats':hist_scalars_dtypes})
+        
+        bins_scalars = [ '%s'%(s,) for s in scalars ]
+        bins_scalars_dtypes = [ np.float64 for s in bins_scalars ]
+        bins = np.zeros(shape=(nyr, n_bins+1) , dtype={'names':bins_scalars, 'formats':bins_scalars_dtypes})
+        
+        ## check memory
+        mem_total_gb = psutil.virtual_memory().total/1024**3
+        mem_avail_gb = psutil.virtual_memory().available/1024**3
+        mem_free_gb  = psutil.virtual_memory().free/1024**3
+        if verbose:
+            even_print('mem total',     '%0.1f [GB]'%(mem_total_gb,))
+            even_print('mem available', '%0.1f [GB] / %0.1f[%%]'%(mem_avail_gb,(100*mem_avail_gb/mem_total_gb)))
+            even_print('mem free',      '%0.1f [GB] / %0.1f[%%]'%(mem_free_gb,(100*mem_free_gb/mem_total_gb)))
+            print(72*'-')
+        
+        ## main loop
+        self.comm.Barrier()
+        if verbose: progress_bar = tqdm(total=n_scalars*nyr, ncols=100, desc='high order stats', leave=False, file=sys.stdout)
+        
+        for s in scalars:
+            
+            #data_unsteady = np.zeros(shape=(nx, nyr, nz, nt), dtype={'names':scalars, 'formats':scalars_dtypes})
+            data_unsteady = np.zeros(shape=(nx, nyr, nz, nt), dtype=dtype_unsteady)
+            
+            ## read prime data
+            dset = self[f'data/{s}']
+            self.comm.Barrier()
+            t_start = timeit.default_timer()
+            if self.usingmpi:
+                with dset.collective:
+                    data_unsteady[:,:,:,:] = np.copy( dset[:,:,ry1:ry2,:].T )
+            else:
+                data_unsteady[:,:,:,:] = np.copy( dset[()].T )
+            self.comm.Barrier()
+            t_delta = timeit.default_timer() - t_start
+            data_gb = float_bytes * self.nx * self.ny * self.nz * self.nt / 1024**3
+            if verbose:
+                tqdm.write(even_print(f'read: {s}', '%0.3f [GB]  %0.3f [s]  %0.3f [GB/s]'%(data_gb,t_delta,(data_gb/t_delta)), s=True))
+            
+            ## redimensionalize prime data
+            if s in ['u','v','w', 'uI','vI','wI', 'uII','vII','wII']:
+                data_unsteady *= U_inf
+            elif s in ['r_uII','r_vII','r_wII']:
+                data_unsteady *= (U_inf*rho_inf)
+            elif s in ['T','TI','TII']:
+                data_unsteady *= T_inf
+            elif s in ['r_TII']:
+                data_unsteady *= (T_inf*rho_inf)
+            elif s in ['rho','rhoI']:
+                data_unsteady *= rho_inf
+            elif s in ['p','pI','pII']:
+                data_unsteady *= (rho_inf * U_inf**2)
+            else:
+                raise ValueError('condition needed for redimensionalizing \'%s\''%var)
+            
+            for yi in range(nyr):
+                
+                ## all [x,z,t] at this [y]
+                d        = np.copy( data_unsteady[:,yi,:,:] ).astype(np.float64).ravel()
+                d_mean   = np.mean( d , dtype=np.float64 )
+                dI       = np.copy( d - d_mean )
+                
+                dI_median = np.median( dI )
+                
+                hist_ , bin_edges_ = np.histogram( dI , bins=n_bins , density=True )
+                hist[s][yi,:] = hist_
+                bins[s][yi,:] = bin_edges_
+                
+                #d_var = np.mean( dI**2 ) ## = d.std()**2
+                d_std = np.sqrt( np.mean( dI**2 , dtype=np.float64 ) ) ## = d.std()
+                
+                ## kurtosis can be checked against scipy implementation
+                ## sp.stats.kurtosis(d,fisher=False)
+                
+                if np.isclose(d_std, 0., atol=1e-08):
+                    d_skew = 0.
+                    d_kurt = 0.
+                else:
+                    d_skew = np.mean( dI**3 , dtype=np.float64 ) / d_std**3
+                    d_kurt = np.mean( dI**4 , dtype=np.float64 ) / d_std**4
+                
+                hos[f'{s}I_median'][yi] = dI_median
+                hos[f'{s}_mean'][yi]    = d_mean
+                hos[f'{s}_std'][yi]     = d_std
+                hos[f'{s}_skew'][yi]    = d_skew
+                hos[f'{s}_kurt'][yi]    = d_kurt
+                
+                if verbose: progress_bar.update()
+        
+        self.comm.Barrier()
+        if verbose:
+            progress_bar.close()
+            print(72*'-')
+        
+        # === average in [x,z], leave [y] --> not needed if stats are calculated over [x,z,t] per [y]
+        
+        ## hos_ = np.zeros(shape=(nyr,) , dtype={'names':hos_scalars, 'formats':hos_scalars_dtypes})
+        ## for tag in hos_scalars:
+        ##     hos_[tag] = np.mean( hos[tag] , axis=(0,2) , dtype=np.float64 )
+        ## hos = np.copy( hos_ )
+        ## self.comm.Barrier()
+        
+        # === gather
+        
+        G = self.comm.gather([ self.rank, hos, hist, bins ], root=0)
+        G = self.comm.bcast(G, root=0)
+        
+        hos  = np.zeros( (ny,)         , dtype={'names':hos_scalars  , 'formats':hos_scalars_dtypes}  )
+        hist = np.zeros( (ny,n_bins)   , dtype={'names':hist_scalars , 'formats':hist_scalars_dtypes} )
+        bins = np.zeros( (ny,n_bins+1) , dtype={'names':bins_scalars , 'formats':bins_scalars_dtypes} )
+        
+        for ri in range(self.n_ranks):
+            j = ri
+            for GG in G:
+                if (GG[0]==ri):
+                    for tag in hos_scalars:
+                        hos[tag][ryl[j][0]:ryl[j][1],] = GG[1][tag]
+                    for tag in hist_scalars:
+                        hist[tag][ryl[j][0]:ryl[j][1],:] = GG[2][tag]
+                    for tag in bins_scalars:
+                        bins[tag][ryl[j][0]:ryl[j][1],:] = GG[3][tag]
+                else:
+                    pass
+        
+        # === save results
+        if (self.rank==0):
+            
+            data['hos']  = hos
+            data['hist'] = hist
+            data['bins'] = bins
+            
+            with open(fn_dat_hos,'wb') as f:
+                pickle.dump(data, f, protocol=4)
+            print('--w-> %s : %0.2f [MB]'%(fn_dat_hos,os.path.getsize(fn_dat_hos)/1024**2))
+        
+        # ===
+        
+        self.comm.Barrier()
+        
+        if verbose: print(72*'-')
+        if verbose: print('total time : rgd.calc_high_order_stats() : %s'%format_time_string((timeit.default_timer() - t_start_func)))
+        if verbose: print(72*'-')
+        
+        return
+    
     def calc_turb_spectrum_time(self, **kwargs):
         '''
         calculate FFT in [t] (frequency) at every [x,y,z], avg in [x,z]
         - designed for analyzing unsteady, thin planes in [x]
         '''
         
         if (self.rank==0):
@@ -11531,15 +12170,15 @@
         if (ry>self.ny):
             raise AssertionError('ry>self.ny')
         if (rz>self.nz):
             raise AssertionError('rz>self.nz')
         if (rt>self.nt):
             raise AssertionError('rt>self.nt')
         
-        # === distribute 4D data over ranks
+        # === distribute 4D data over ranks --> here only in [y]
         
         #comm4d = self.comm.Create_cart(dims=[rx,ry,ry,rt], periods=[False,False,False,False], reorder=False)
         #t4d = comm4d.Get_coords(self.rank)
         
         #rxl_ = np.array_split(np.arange(self.nx,dtype=np.int64),min(rx,self.nx))
         ryl_ = np.array_split(np.arange(self.ny,dtype=np.int64),min(ry,self.ny))
         #rzl_ = np.array_split(np.arange(self.nz,dtype=np.int64),min(rz,self.nz))
@@ -11553,212 +12192,222 @@
         #rx1, rx2 = rxl[t4d[0]]; nxr = rx2 - rx1
         #ry1, ry2 = ryl[t4d[1]]; nyr = ry2 - ry1
         #rz1, rz2 = rzl[t4d[2]]; nzr = rz2 - rz1
         #rt1, rt2 = rtl[t4d[3]]; ntr = rt2 - rt1
         
         ry1,ry2 = ryl[self.rank]; nyr = ry2 - ry1
         
-        # === mean (dimensional) file name (for reading) : .dat
-        if (fn_dat_mean_dim is None):
-            fname_path = os.path.dirname(self.fname)
-            fname_base = os.path.basename(self.fname)
-            fname_root, fname_ext = os.path.splitext(fname_base)
-            fname_root = re.findall('io\S+_mpi_[0-9]+', fname_root)[0]
-            fname_dat_mean_base = fname_root+'_mean_dim.dat'
-            fn_dat_mean_dim = str(PurePosixPath(fname_path, fname_dat_mean_base))
+        # # === mean (dimensional) file name (for reading) : .dat
+        # if (fn_dat_mean_dim is None):
+        #     fname_path = os.path.dirname(self.fname)
+        #     fname_base = os.path.basename(self.fname)
+        #     fname_root, fname_ext = os.path.splitext(fname_base)
+        #     fname_root = re.findall('io\S+_mpi_[0-9]+', fname_root)[0]
+        #     fname_dat_mean_base = fname_root+'_mean_dim.dat'
+        #     fn_dat_mean_dim = str(PurePosixPath(fname_path, fname_dat_mean_base))
         
         # === fft file name (for writing) : dat
         if (fn_dat_fft is None):
             fname_path = os.path.dirname(self.fname)
             fname_base = os.path.basename(self.fname)
             fname_root, fname_ext = os.path.splitext(fname_base)
             fname_root = re.findall('io\S+_mpi_[0-9]+', fname_root)[0]
             fname_fft_dat_base = fname_root+'_turb_spec_time.dat'
             fn_dat_fft = str(PurePosixPath(fname_path, fname_fft_dat_base))
         
         if verbose: even_print('fn_rgd_prime'    , self.fname       )
-        if verbose: even_print('fn_dat_mean_dim' , fn_dat_mean_dim  )
+        #if verbose: even_print('fn_dat_mean_dim' , fn_dat_mean_dim  )
         if verbose: even_print('fn_dat_fft'      , fn_dat_fft       )
         if verbose: print(72*'-')
         
-        if not os.path.isfile(fn_dat_mean_dim):
-            raise FileNotFoundError('%s not found!'%fn_dat_mean_dim)
+        #if not os.path.isfile(fn_dat_mean_dim):
+        #    raise FileNotFoundError('%s not found!'%fn_dat_mean_dim)
         
-        # === read in data (mean dim) --> every rank gets full [x,z]
-        with open(fn_dat_mean_dim,'rb') as f:
-            data_mean_dim = pickle.load(f)
-        fmd = type('foo', (object,), data_mean_dim)
+        # # === read in data (mean dim) --> every rank gets full [x,z]
+        # with open(fn_dat_mean_dim,'rb') as f:
+        #     data_mean_dim = pickle.load(f)
+        # fmd = type('foo', (object,), data_mean_dim)
         
         self.comm.Barrier()
         
         ## the data dictionary to be pickled later
         data = {}
         
-        ## 2D dimensional quantities --> [x,z]
-        u_tau    = fmd.u_tau    # ; data['u_tau']    = u_tau
-        nu_wall  = fmd.nu_wall  # ; data['nu_wall']  = nu_wall
-        rho_wall = fmd.rho_wall # ; data['rho_wall'] = rho_wall
-        d99      = fmd.d99      # ; data['d99']      = d99
-        u99      = fmd.u99      # ; data['u99']      = u99
-        Re_tau   = fmd.Re_tau   # ; data['Re_tau']   = Re_tau
-        Re_theta = fmd.Re_theta # ; data['Re_theta'] = Re_theta
-        
-        ## mean [x,z] --> leave 0D scalar
-        u_tau_avg    = np.mean(fmd.u_tau    , axis=(0,1)) ; data['u_tau_avg']    = u_tau_avg
-        nu_wall_avg  = np.mean(fmd.nu_wall  , axis=(0,1)) ; data['nu_wall_avg']  = nu_wall_avg
-        rho_wall_avg = np.mean(fmd.rho_wall , axis=(0,1)) ; data['rho_wall_avg'] = rho_wall_avg
-        d99_avg      = np.mean(fmd.d99      , axis=(0,1)) ; data['d99_avg']      = d99_avg
-        u99_avg      = np.mean(fmd.u99      , axis=(0,1)) ; data['u99_avg']      = u99_avg
-        Re_tau_avg   = np.mean(fmd.Re_tau   , axis=(0,1)) ; data['Re_tau_avg']   = Re_tau_avg
-        Re_theta_avg = np.mean(fmd.Re_theta , axis=(0,1)) ; data['Re_theta_avg'] = Re_theta_avg
-        
-        ## mean [x,z] --> leave 1D [y]
-        rho_avg = np.mean(fmd.rho,axis=(0,2))
-        data['rho_avg'] = rho_avg
+        if ('data_dim' not in self):
+            raise ValueError('group data_dim not present')
         
-        # === 2D inner scales --> [x,z]
-        sc_l_in = nu_wall / u_tau
-        sc_u_in = u_tau
-        sc_t_in = nu_wall / u_tau**2
+        ## put all data from 'data_dim' into the dictionary data which will be pickled at the end
+        for dsn in self['data_dim'].keys():
+            d_ = np.copy( self[f'data_dim/{dsn}'][()] )
+            if (d_.ndim == 0):
+                d_ = float(d_)
+            data[dsn] = d_
         
-        # === 2D outer scales --> [x,z]
-        sc_l_out = d99
-        sc_u_out = u99
-        sc_t_out = d99/u99
+        ## 1D
+        rho_avg = np.copy( self['data_dim/rho'][()] )
+        u_avg   = np.copy( self['data_dim/u'][()]   )
+        
+        ## 0D
+        u_tau    = float( self['data_dim/u_tau'][()]    )
+        nu_wall  = float( self['data_dim/nu_wall'][()]  )
+        rho_wall = float( self['data_dim/rho_wall'][()] )
+        d99      = float( self['data_dim/d99'][()]      )
+        u_99     = float( self['data_dim/u_99'][()]     )
+        Re_tau   = float( self['data_dim/Re_tau'][()]   )
+        Re_theta = float( self['data_dim/Re_theta'][()] )
+        sc_u_in  = float( self['data_dim/sc_u_in'][()]  )
+        sc_l_in  = float( self['data_dim/sc_l_in'][()]  )
+        sc_t_in  = float( self['data_dim/sc_t_in'][()]  )
+        sc_u_out = float( self['data_dim/sc_u_out'][()] )
+        sc_l_out = float( self['data_dim/sc_l_out'][()] )
+        sc_t_out = float( self['data_dim/sc_t_out'][()] )
+        
+        ## these are recalculated and checked in next step
+        z1d_ = np.copy( self['data_dim/z1d'][()] )
+        dz0_ = np.copy( self['data_dim/dz0'][()] )
+        dt_  = np.copy( self['data_dim/dt'][()]  )
+        
+        # ===
         
-        np.testing.assert_allclose( fmd.sc_l_in  , sc_l_in  , rtol=1e-14 )
-        np.testing.assert_allclose( fmd.sc_l_out , sc_l_out , rtol=1e-14 )
-        np.testing.assert_allclose( fmd.sc_u_in  , sc_u_in  , rtol=1e-14 )
-        np.testing.assert_allclose( fmd.sc_u_out , sc_u_out , rtol=1e-14 )
-        np.testing.assert_allclose( fmd.sc_t_in  , sc_t_in  , rtol=1e-14 )
-        np.testing.assert_allclose( fmd.sc_t_out , sc_t_out , rtol=1e-14 )
-        
-        sc_l_in_avg  = np.mean(sc_l_in  , axis=(0,1))
-        sc_l_out_avg = np.mean(sc_l_out , axis=(0,1))
-        sc_u_in_avg  = np.mean(sc_u_in  , axis=(0,1))
-        sc_u_out_avg = np.mean(sc_u_out , axis=(0,1))
-        sc_t_in_avg  = np.mean(sc_t_in  , axis=(0,1))
-        sc_t_out_avg = np.mean(sc_t_out , axis=(0,1))
-        
-        # === check
-        np.testing.assert_allclose( fmd.lchar   , self.lchar   , rtol=1e-14 )
-        np.testing.assert_allclose( fmd.U_inf   , self.U_inf   , rtol=1e-14 )
-        np.testing.assert_allclose( fmd.rho_inf , self.rho_inf , rtol=1e-14 )
-        np.testing.assert_allclose( fmd.T_inf   , self.T_inf   , rtol=1e-14 )
-        np.testing.assert_allclose( fmd.nx      , self.nx      , rtol=1e-14 )
-        np.testing.assert_allclose( fmd.ny      , self.ny      , rtol=1e-14 )
-        np.testing.assert_allclose( fmd.nz      , self.nz      , rtol=1e-14 )
-        np.testing.assert_allclose( fmd.xs      , self.x       , rtol=1e-14 )
-        np.testing.assert_allclose( fmd.ys      , self.y       , rtol=1e-14 )
-        np.testing.assert_allclose( fmd.zs      , self.z       , rtol=1e-14 )
+        ## get size of infile
+        fsize = os.path.getsize(self.fname)/1024**3
+        if verbose: even_print(os.path.basename(self.fname),'%0.1f [GB]'%fsize)
+        if verbose: even_print('nx','%i'%self.nx)
+        if verbose: even_print('ny','%i'%self.ny)
+        if verbose: even_print('nz','%i'%self.nz)
+        if verbose: even_print('nt','%i'%self.nt)
+        if verbose: even_print('ngp','%0.1f [M]'%(self.ngp/1e6,))
+        if verbose: print(72*'-')
         
+        ## 0D scalars
         lchar   = self.lchar   ; data['lchar']   = lchar
         U_inf   = self.U_inf   ; data['U_inf']   = U_inf
         rho_inf = self.rho_inf ; data['rho_inf'] = rho_inf
         T_inf   = self.T_inf   ; data['T_inf']   = T_inf
         
         data['Ma'] = self.Ma
         data['Pr'] = self.Pr
         
+        ## read in 1D coordinate arrays, then re-dimensionalize [m]
+        x = np.copy( self['dims/x'][()] * self.lchar )
+        y = np.copy( self['dims/y'][()] * self.lchar )
+        z = np.copy( self['dims/z'][()] * self.lchar )
+        
         nx = self.nx ; data['nx'] = nx
         ny = self.ny ; data['ny'] = ny
         nz = self.nz ; data['nz'] = nz
         nt = self.nt ; data['nt'] = nt
         
-        ## dimless (inlet)
-        xd = self.x
-        yd = self.y
-        zd = self.z
-        td = self.t
+        # ## dimless (inlet/characteristic)
+        # xd = self.x
+        # yd = self.y
+        # zd = self.z
+        # td = self.t
         
-        ## dimensional [m] / [s]
+        ## redimensionalize coordinates --> [m],[s],[m/s],etc.
         x      = self.x * lchar
         y      = self.y * lchar
         z      = self.z * lchar
         t      = self.t * (lchar/U_inf)
         t_meas = t[-1]-t[0]
         dt     = self.dt * (lchar/U_inf)
         
+        z1d = np.copy(z)
+        
         ## check if constant Δz (calculate Δz+ later)
-        dz0_ = np.diff(z)[0]
-        if np.all(np.isclose(np.diff(z), dz0_, rtol=1e-7)):
-            dz0 = dz0_
-        else:
-            dz0 = None
-        dz0_ = None; del dz0_
-        data['dz0'] = dz0
+        dz0 = np.diff(z1d)[0]
+        if not np.all(np.isclose(np.diff(z1d), dz0, rtol=1e-7)):
+            raise NotImplementedError
+        
+        ## dimensional [s]
+        dt = self.dt * self.tchar
+        np.testing.assert_allclose(dt, t[1]-t[0], rtol=1e-14, atol=1e-14)
+        
+        t_meas = self.duration * self.tchar
+        np.testing.assert_allclose(t_meas, t.max()-t.min(), rtol=1e-14, atol=1e-14)
+        
+        ## check against values in 'data_dim' (imported above)
+        np.testing.assert_allclose(dt  , dt_  , rtol=1e-14, atol=1e-14)
+        np.testing.assert_allclose(dz0 , dz0_ , rtol=1e-14, atol=1e-14)
+        np.testing.assert_allclose(z1d , z1d_ , rtol=1e-14, atol=1e-14)
+        
+        zrange = z[-1]-z[0]
         
         data['x'] = x
         data['y'] = y
         data['z'] = z
+        #data['z1d'] = z1d
+        
         data['t'] = t
         data['t_meas'] = t_meas
         data['dt'] = dt
+        data['dz0'] = dz0
+        data['zrange'] = zrange
         
-        np.testing.assert_equal(nx,x.size)
-        np.testing.assert_equal(ny,y.size)
-        np.testing.assert_equal(nz,z.size)
-        np.testing.assert_equal(nt,t.size)
-        np.testing.assert_allclose(dt, t[1]-t[0], rtol=1e-8)
+        if verbose: even_print('Δt/tchar','%0.8f'%(dt/self.tchar))
+        if verbose: even_print('Δt','%0.3e [s]'%(dt,))
+        if verbose: even_print('duration/tchar','%0.1f'%(self.duration,))
+        if verbose: even_print('duration','%0.3e [s]'%(self.duration*self.tchar,))
+        if verbose: print(72*'-')
         
-        # === report
+        ## report
         if verbose:
-            even_print('nx'     , '%i'        %nx     )
-            even_print('ny'     , '%i'        %ny     )
-            even_print('nz'     , '%i'        %nz     )
-            even_print('nt'     , '%i'        %nt     )
-            even_print('dt'     , '%0.5e [s]' %dt     )
-            even_print('t_meas' , '%0.5e [s]' %t_meas )
+            even_print('dt'     , '%0.5e [s]' % dt      )
+            even_print('t_meas' , '%0.5e [s]' % t_meas  )
+            even_print('dz0'    , '%0.5e [m]' % dz0     )
+            even_print('zrange' , '%0.5e [m]' % zrange  )
             print(72*'-')
         
+        ## report
         if verbose:
-            even_print('Re_τ'    , '%0.1f'        % Re_tau_avg    )
-            even_print('Re_θ'    , '%0.1f'        % Re_theta_avg  )
-            even_print('δ99'     , '%0.5e [m]'    % d99_avg       )
-            even_print('δ_ν=(ν_wall/u_τ)' , '%0.5e [m]' % sc_l_in_avg )
-            even_print('U_inf'  , '%0.3f [m/s]'   % U_inf         )
-            even_print('u_τ'    , '%0.3f [m/s]'   % u_tau_avg     )
-            even_print('ν_wall' , '%0.5e [m²/s]'  % nu_wall_avg   )
-            even_print('ρ_wall' , '%0.6f [kg/m³]' % rho_wall_avg  )
+            even_print('Re_τ'    , '%0.1f'        % Re_tau    )
+            even_print('Re_θ'    , '%0.1f'        % Re_theta  )
+            even_print('δ99'     , '%0.5e [m]'    % d99       )
+            even_print('δ_ν=(ν_wall/u_τ)' , '%0.5e [m]' % sc_l_in )
+            even_print('U_inf'  , '%0.3f [m/s]'   % self.U_inf )
+            even_print('u_τ'    , '%0.3f [m/s]'   % u_tau     )
+            even_print('ν_wall' , '%0.5e [m²/s]'  % nu_wall   )
+            even_print('ρ_wall' , '%0.6f [kg/m³]' % rho_wall  )
             ##
-            even_print( 'Δz+' , '%0.3f'%(dz0/sc_l_in_avg) )
-            even_print( 'Δt+' , '%0.3f'%(dt/sc_t_in_avg) )
+            even_print( 'Δz+'        , '%0.3f'%(dz0/sc_l_in) )
+            even_print( 'zrange/δ99' , '%0.3f'%(zrange/d99)  )
+            even_print( 'Δt+'        , '%0.3f'%(dt/sc_t_in)  )
             print(72*'-')
         
-        t_eddy = t_meas / ( d99_avg / u_tau_avg )
+        t_eddy = t_meas / ( d99 / u_tau )
         
         if verbose:
             even_print('t_meas/(δ99/u_τ) = t_eddy' , '%0.2f'%t_eddy)
-            even_print('t_meas/(δ99/u99)'          , '%0.2f'%(t_meas/(d99_avg/u99_avg)))
-            even_print('t_meas/(20·δ99/u99)'       , '%0.2f'%(t_meas/(20*d99_avg/u99_avg)))
+            even_print('t_meas/(δ99/u99)'          , '%0.2f'%(t_meas/(d99/u_99)))
+            even_print('t_meas/(20·δ99/u99)'       , '%0.2f'%(t_meas/(20*d99/u_99)))
             print(72*'-')
         
-        # === establish windowing
+        ## establish fft (time) windowing
         win_len, overlap = get_overlapping_window_size(nt, n_win, overlap_fac_nom)
         overlap_fac = overlap / win_len
         tw, n_win, n_pad = get_overlapping_windows(t, win_len, overlap)
         
         data['win_len']     = win_len
         data['overlap_fac'] = overlap_fac
         data['overlap']     = overlap
         data['n_win']       = n_win
         
         t_meas_per_win = (win_len-1)*dt
-        t_eddy_per_win = t_meas_per_win / (d99_avg/u_tau_avg)
+        t_eddy_per_win = t_meas_per_win / (d99/u_tau)
         
         data['t_eddy_per_win'] = t_eddy_per_win
         
         if verbose:
             even_print('overlap_fac (nominal)' , '%0.5f'%overlap_fac_nom    )
             even_print('n_win'                 , '%i'%n_win                 )
             even_print('win_len'               , '%i'%win_len               )
             even_print('overlap'               , '%i'%overlap               )
             even_print('overlap_fac'           , '%0.5f'%overlap_fac        )
             even_print('n_pad'                 , '%i'%n_pad                 )
-            even_print('t_win/(δ99/u_τ)'       , '%0.2f [-]'%t_eddy_per_win )
+            even_print('t_win/(δ99/u_τ)'       , '%0.3f [-]'%t_eddy_per_win )
             print(72*'-')
         
         # === get frequency vector --> here for short time FFT!
         freq_full = sp.fft.fftfreq(n=win_len, d=dt)
         fp        = np.where(freq_full>0)
         freq      = np.copy(freq_full[fp])
         df        = freq[1]-freq[0]
@@ -11770,154 +12419,140 @@
         
         if verbose:
             even_print('freq min','%0.1f [Hz]'%freq.min())
             even_print('freq max','%0.1f [Hz]'%freq.max())
             even_print('df','%0.1f [Hz]'%df)
             even_print('nf','%i'%nf)
             
-            # freq_plus = freq * np.mean(sc_t_in, axis=(0,1)) ## [?]
-            # df_plus   = df   * np.mean(sc_t_in, axis=(0,1)) ## [?]
-            # even_print('freq+ min','%0.5e [-]'%freq_plus.min())
-            # even_print('freq+ max','%0.5f [-]'%freq_plus.max())
-            # even_print('df+','%0.5e [-]'%df_plus)
-            
-            period_eddy = (1/freq) / np.mean((d99/u_tau), axis=(0,1))
-            period_plus = (1/freq) / np.mean(sc_t_in,     axis=(0,1))
-            even_print('period+ min'     , '%0.5e [-]'%period_plus.min())
-            even_print('period+ max'     , '%0.5f [-]'%period_plus.max())
-            even_print('period eddy min' , '%0.5e [-]'%period_eddy.min())
-            even_print('period eddy max' , '%0.5f [-]'%period_eddy.max())
+            period_eddy = (1/freq) / (d99/u_tau)
+            period_plus = (1/freq) / sc_t_in
+            even_print('min : period+ = (1/f)/(ν_wall/u_τ²)'   , '%0.5f [-]'%period_plus.min())
+            even_print('max : period+ = (1/f)/(ν_wall/u_τ²)'   , '%0.5f [-]'%period_plus.max())
+            even_print('min : period_eddy = (1/f)/(d99/u_tau)' , '%0.5e [-]'%period_eddy.min())
+            even_print('max : period_eddy = (1/f)/(d99/u_tau)' , '%0.5f [-]'%period_eddy.max())
             
             print(72*'-')
         
-        # === kx, λx
+        self.comm.Barrier()
+        
+        # === wavenumber kx, λx
+        
+        # λx = u/f
+        # kx = 2·π·f/u
+        # ---
+        # λx/δ99
+        # λx+ = λx/(ν/u_tau)
+        # kx·δ99
+        # kx+ = (2·π·f/u)·(ν/u_tau)
         
         na = np.newaxis
         
         ## prevent zeros since later we divide by wall u to get kx
-        #fmd.u = np.maximum(fmd.u, np.ones_like(fmd.u)*1e-8)
-        fmd.u[:,0,:] = fmd.u[:,1,:]*1e-4
+        u_avg[0] = u_avg[1]*1e-6
         
-        # eps=1e-6
-        # fmd.u[:,0,:] = np.maximum( 1e-4*fmd.u[:,1,:] , eps*np.ones_like(fmd.u[:,1,:]) )
+        ## kx = 2·π·f/u --> [y,f]
+        kx = (2*np.pi*freq[na,:]/u_avg[:,na])
         
-        ## kx
-        kx = (2*np.pi*freq[na,na,na,:]/fmd.u[:,:,:,na])
-        kx = np.mean(kx, axis=(0,2)) ## avg in [x,z] --> [y,f]
-        
-        # ## kx·δ99 --> dimless outer
-        # kxd = (2*np.pi*freq[na,na,na,:]/fmd.u[:,:,:,na]) * sc_l_out[:,na,:,na]
-        # kxd = np.mean(kxd, axis=(0,2)) ## avg in [x,z] --> [y,f]
-        
-        # ## kx+ --> dimless inner
-        # kxp = (2*np.pi*freq[na,na,na,:]/fmd.u[:,:,:,na]) * sc_l_in[:,na,:,na]
-        # kxp = np.mean(kxp, axis=(0,2)) ## avg in [x,z] --> [y,f]
-        
-        ## λx
-        lx = (fmd.u[:,:,:,na]/freq[na,na,na,:])
-        lx = np.mean(lx, axis=(0,2)) ## avg in [x,z] --> [y,f]
-        
-        # ## λx/δ99 --> dimless outer
-        # lxd = (fmd.u[:,:,:,na]/freq[na,na,na,:]) / sc_l_out[:,na,:,na]
-        # lxd = np.mean(lxd, axis=(0,2)) ## avg in [x,z] --> [y,f]
-        
-        # ## λx+ = λx/(ν/u_tau) --> dimless inner
-        # lxp = (fmd.u[:,:,:,na]/freq[na,na,na,:]) / sc_l_in[:,na,:,na]
-        # lxp = np.mean(lxp, axis=(0,2)) ## avg in [x,z] --> [y,f]
+        ## λx = u/f --> [y,f]
+        lx = (u_avg[:,na]/freq[na,:])
         
         data['kx']  = kx
-        # data['kxp'] = kxp
-        # data['kxd'] = kxd
         data['lx']  = lx
-        # data['lxp'] = lxp
-        # data['lxd'] = lxd
         
         # === read in data (prime) --> still dimless (char)
         
-        scalars = [ 'uI','vI','wI' , 'rho','uII','vII','wII' ]
-        #scalars = [ 'uI' ]
+        scalars = [ 'uI','vI','wI' , 'rho', 'uII','vII','wII' ]
         
         ## [var1, var2, density_scaling]
         fft_combis = [
                      [ 'uI'  , 'uI'  , False ],
                      [ 'vI'  , 'vI'  , False ],
                      [ 'wI'  , 'wI'  , False ],
                      [ 'uI'  , 'vI'  , False ],
+                     [ 'uI'  , 'wI'  , False ],
+                     [ 'vI'  , 'wI'  , False ],
                      [ 'uII' , 'uII' , True  ],
                      [ 'vII' , 'vII' , True  ],
                      [ 'wII' , 'wII' , True  ],
                      [ 'uII' , 'vII' , True  ],
+                     [ 'uII' , 'wII' , True  ],
+                     [ 'vII' , 'wII' , True  ],
                      ]
         
-        scalars_dtypes = [ self.scalars_dtypes_dict[s] for s in scalars ]
+        if verbose:
+            even_print('n turb spectrum (time) scalar combinations' , '%i'%(len(fft_combis),))
+            print(72*'-')
         
-        ## dtype of prime data (currently must be all same dtype)
-        if np.all( [ (dtp==np.float32) for dtp in scalars_dtypes ] ):
-            dtype_primes = np.float32
-        elif np.all( [ (dtp==np.float64) for dtp in scalars_dtypes ] ):
-            dtype_primes = np.float64
-        else:
-            raise NotImplementedError
+        ## decide if mass density will be needed
+        read_density = False
+        for cc in fft_combis:
+            scalar_L, scalar_R, density_scaling = cc
+            if density_scaling:
+                read_density = True
+                break
         
-        ## 5D [scalar][x,y,z,t] structured array
-        data_prime = np.zeros(shape=(self.nx, nyr, self.nz, self.nt), dtype={'names':scalars, 'formats':scalars_dtypes})
+        if verbose:
+            even_print('read ρ', str(read_density))
         
-        for scalar in scalars:
+        ## confirm 'rho' is not in locals
+        if read_density and ('rho' in locals()):
+            raise ValueError('rho alread in locals... check')
+        
+        if read_density:
             
-            dset = self[f'data/{scalar}']
-            dtype = dset.dtype
-            float_bytes = dtype.itemsize
+            ## buffer for rho ( !! NOT rhoI !! ) --> this is read from 'prime' file
+            rho = np.zeros(shape=(nx, nyr, nz, nt), dtype=np.float32)
             
+            dset = self['data/rho']
             self.comm.Barrier()
             t_start = timeit.default_timer()
-            with dset.collective:
-                data_prime[scalar] = np.copy( dset[:,:,ry1:ry2,:].T )
+            if self.usingmpi:
+                with dset.collective:
+                    rho[:,:,:,:] = dset[:,:,ry1:ry2,:].T
+            else:
+                rho[:,:,:,:] = dset[()].T
             self.comm.Barrier()
             t_delta = timeit.default_timer() - t_start
-            
-            data_gb = float_bytes * self.nx * self.ny * self.nz * self.nt / 1024**3
-            
+            data_gb = 4 * self.nx * self.ny * self.nz * self.nt / 1024**3
             if verbose:
-                even_print('read: %s'%scalar, '%0.3f [GB]  %0.3f [s]  %0.3f [GB/s]'%(data_gb,t_delta,(data_gb/t_delta)))
+                even_print( 'read: rho','%0.3f [GB]  %0.3f [s]  %0.3f [GB/s]'%(data_gb,t_delta,(data_gb/t_delta)))
+            
+            ## re-dimensionalize rho
+            rho *= rho_inf
         
-        # === redimensionalize prime data
+        # ===
         
-        for var in data_prime.dtype.names:
-            if var in ['u','v','w', 'uI','vI','wI', 'uII','vII','wII']:
-                data_prime[var] *= U_inf
-            elif var in ['r_uII','r_vII','r_wII']:
-                data_prime[var] *= (U_inf*rho_inf)
-            elif var in ['T','TI','TII']:
-                data_prime[var] *= T_inf
-            elif var in ['r_TII']:
-                data_prime[var] *= (T_inf*rho_inf)
-            elif var in ['rho','rhoI']:
-                data_prime[var] *= rho_inf
-            elif var in ['p','pI','pII']:
-                data_prime[var] *= (rho_inf * U_inf**2)
-            else:
-                raise ValueError('condition needed for redimensionalizing \'%s\''%var)
+        scalars_dtypes = [ self.scalars_dtypes_dict[s] for s in scalars ]
+        
+        ## dtype of prime data (currently must be all same dtype)
+        if np.all( [ (dtp==np.float32) for dtp in scalars_dtypes ] ):
+            dtype_primes = np.float32
+        elif np.all( [ (dtp==np.float64) for dtp in scalars_dtypes ] ):
+            dtype_primes = np.float64
+        else:
+            raise NotImplementedError('primes dont all have same dtype --> needs update')
         
         ## force the ∫PSD == (co)variance
         ## this usually represents about a 1-2% power correction which comes about due to 
         ##   non-stationarity of windowed data
         normalize_psd_by_cov = False
         
-        ## initialize buffers
-        Euu_scalars         = [ '%s%s'%(cc[0],cc[1]) for cc in fft_combis ]
-        Euu_scalars_dtypes  = [ dtype_primes for s in Euu_scalars ]
-        Euu                 = np.zeros(shape=(self.nx, nyr, self.nz, nf) , dtype={'names':Euu_scalars, 'formats':Euu_scalars_dtypes})
-        uIuI_avg            = np.zeros(shape=(self.nx, nyr, self.nz)     , dtype={'names':Euu_scalars, 'formats':Euu_scalars_dtypes})
+        Euu_scalars        = [ '%s%s'%(cc[0],cc[1]) for cc in fft_combis ]
+        Euu_scalars_dtypes = [ dtype_primes for s in Euu_scalars ]
+        
+        ## buffers
+        Euu_avg  = np.zeros(shape=(nyr, nf) , dtype={'names':Euu_scalars, 'formats':Euu_scalars_dtypes})
+        uIuI_avg = np.zeros(shape=(nyr,   ) , dtype={'names':Euu_scalars, 'formats':Euu_scalars_dtypes})
         if normalize_psd_by_cov:
             energy_norm_fac_arr = np.zeros(shape=(self.nx, nyr, self.nz) , dtype={'names':Euu_scalars, 'formats':Euu_scalars_dtypes}) ## just for monitoring
         
         ## check memory
-        mem_total_gb = psutil.virtual_memory().total/1024**3
-        mem_avail_gb = psutil.virtual_memory().available/1024**3
-        mem_free_gb  = psutil.virtual_memory().free/1024**3
+        mem_total_gb = psutil.virtual_memory().total     / 1024**3
+        mem_avail_gb = psutil.virtual_memory().available / 1024**3
+        mem_free_gb  = psutil.virtual_memory().free      / 1024**3
         if verbose:
             even_print('mem total',     '%0.1f [GB]'%(mem_total_gb,))
             even_print('mem available', '%0.1f [GB] / %0.1f[%%]'%(mem_avail_gb,(100*mem_avail_gb/mem_total_gb)))
             even_print('mem free',      '%0.1f [GB] / %0.1f[%%]'%(mem_free_gb,(100*mem_free_gb/mem_total_gb)))
         
         ## the window function
         window_type = 'tukey'
@@ -11927,67 +12562,130 @@
             window = np.ones(win_len, dtype=np.float64)
         if verbose:
             even_print('window type', '\'%s\''%str(window_type))
         
         ## sum of sqrt of window: needed for power normalization
         sum_sqrt_win = np.sum(np.sqrt(window))
         
-        # === main loop
+        if verbose:
+            even_print('sum(sqrt(window)) / win_len', '%0.5f'%(sum_sqrt_win/win_len))
         
+        if verbose:
+            print(72*'-')
+        
+        ## main loop --> turbulent spectrum in [Δt] at every [x,y,z]
         self.comm.Barrier()
-        if verbose: progress_bar = tqdm(total=self.nx*nyr*self.nz, ncols=100, desc='fft', leave=False)
-        for xi in range(self.nx):
-            for yi in range(nyr):
-                for zi in range(self.nz):
-                    for cci,cc in enumerate(fft_combis):
-                        
-                        tag = Euu_scalars[cci]
-                        ccL,ccR,density_scaling = cc
-                        
-                        uL = np.copy( data_prime[ccL][xi,yi,zi,:] )
-                        uR = np.copy( data_prime[ccR][xi,yi,zi,:] )
+        if verbose:
+            progress_bar = tqdm(total=len(fft_combis)*nx*nyr*nz, ncols=100, desc='calc_turb_spectrum_time()', leave=False, file=sys.stdout)
+        
+        for cci,cc in enumerate(fft_combis):
+            
+            scalar_L, scalar_R, density_scaling = cc
+            tag = '%s%s'%(scalar_L, scalar_R)
+            
+            ## check if autocorrelation, in which case don't read twice
+            if (scalar_L==scalar_R):
+                scalars = [ scalar_L ]
+            else:
+                scalars = [ scalar_L, scalar_R ]
+            
+            scalars_dtypes = [ self.scalars_dtypes_dict[s] for s in scalars ]
+            
+            ## prime data buffer
+            ## 5D [scalar][x,y,z,t] structured array
+            data_prime = np.zeros(shape=(nx, nyr, nz, nt), dtype={'names':scalars, 'formats':scalars_dtypes})
+            
+            ## unsteady data buffers
+            Euu  = np.zeros(shape=(self.nx, nyr, self.nz, nf), dtype=np.float32)
+            uIuI = np.zeros(shape=(self.nx, nyr, self.nz),     dtype=np.float32)
+            
+            ## read prime data
+            for scalar in scalars:
+                dset = self['data/%s'%scalar]
+                self.comm.Barrier()
+                t_start = timeit.default_timer()
+                if self.usingmpi:
+                    with dset.collective:
+                        data_prime[scalar][:,:,:,:] = np.copy( dset[:,:,ry1:ry2,:].T )
+                else:
+                    data_prime[scalar][:,:,:,:] = np.copy( dset[()].T )
+                self.comm.Barrier()
+                t_delta = timeit.default_timer() - t_start
+                data_gb = 4 * self.nx * self.ny * self.nz * self.nt / 1024**3
+                if verbose:
+                    tqdm.write(even_print('read: %s'%scalar, '%0.3f [GB]  %0.3f [s]  %0.3f [GB/s]'%(data_gb,t_delta,(data_gb/t_delta)), s=True))
+            
+            ## redimensionalize prime data
+            for var in data_prime.dtype.names:
+                if var in ['u','v','w', 'uI','vI','wI', 'uII','vII','wII']:
+                    data_prime[var] *= U_inf
+                elif var in ['r_uII','r_vII','r_wII']:
+                    data_prime[var] *= (U_inf*rho_inf)
+                elif var in ['T','TI','TII']:
+                    data_prime[var] *= T_inf
+                elif var in ['r_TII']:
+                    data_prime[var] *= (T_inf*rho_inf)
+                elif var in ['rho','rhoI']:
+                    data_prime[var] *= rho_inf
+                elif var in ['p','pI','pII']:
+                    data_prime[var] *= (rho_inf * U_inf**2)
+                else:
+                    raise ValueError('condition needed for redimensionalizing \'%s\''%var)
+            
+            ## print names of components being cross-correlated
+            if verbose:
+                if density_scaling:
+                    fancy_tag = '<ρ·%s,ρ·%s>'%(scalar_L,scalar_R)
+                else:
+                    fancy_tag = '<%s,%s>'%(scalar_L,scalar_R)
+                tqdm.write(even_print('running Δt fft calc', fancy_tag, s=True))
+            
+            for xi in range(nx):
+                for yi in range(nyr):
+                    for zi in range(nz):
                         
-                        if ('rho' in data_prime.dtype.names):
-                            
-                            #rho     = np.copy( data_prime['rho'][xi,yi,:,ti] )
-                            rho     = np.copy( data_prime['rho'][xi,yi,zi,:] )
-                            rho_avg = np.mean( rho, dtype=np.float64 )
-                            
-                            #if (rho.dtype==np.float32):
-                            #    rho_avg = np.copy(rho_avg.astype(np.float32))
+                        uL = np.copy( data_prime[scalar_L][xi,yi,zi,:] )
+                        uR = np.copy( data_prime[scalar_R][xi,yi,zi,:] )
                         
+                        if density_scaling:
+                            rho1d = np.copy( rho[xi,yi,zi,:] )
+                            rho_avg = np.mean( rho1d, dtype=np.float64 )
                         else:
-                            rho     = None
+                            rho1d   = None
                             rho_avg = None
                         
                         # ===
                         
                         if density_scaling:
-                            uIuI_avg_ijk = np.mean(uL*uR*rho, dtype=np.float64) / rho_avg
-                            #if (dtype_primes==np.float32):
-                            #    uIuI_avg_ijk = np.copy( uIuI_avg_ijk.astype(np.float32) )
+                            uIuI_ijk = np.mean(uL*uR*rho1d, dtype=np.float64) / rho_avg
                         else:
-                            uIuI_avg_ijk = np.mean(uL*uR, dtype=np.float64)
+                            uIuI_ijk = np.mean(uL*uR, dtype=np.float64)
                         
-                        uIuI_avg[tag][xi,yi,zi] = uIuI_avg_ijk
+                        ## write to buffer
+                        uIuI[xi,yi,zi] = uIuI_ijk
                         
                         ## window time series into several overlapping windows
-                        uL,  nw, n_pad = get_overlapping_windows(uL,  win_len, overlap)
-                        uR,  nw, n_pad = get_overlapping_windows(uR,  win_len, overlap)
-                        rho, nw, n_pad = get_overlapping_windows(rho, win_len, overlap)
+                        uL, nw, n_pad = get_overlapping_windows(uL, win_len, overlap)
+                        uR, nw, n_pad = get_overlapping_windows(uR, win_len, overlap)
+                        if density_scaling:
+                            rho1d, _, _ = get_overlapping_windows(rho1d, win_len, overlap)
+                        else:
+                            rho1d = None
                         
-                        ## do fft for each segment
+                        ## STFT buffer
                         Euu_ijk = np.zeros((nw,nf), dtype=dtype_primes)
+                        
+                        ## do fft for each segment
                         for wi in range(nw):
                             if density_scaling:
-                                ui    = np.copy( uL[wi,:] * rho[wi,:] )
-                                uj    = np.copy( uR[wi,:] * rho[wi,:] )
+                                ui = np.copy( uL[wi,:] * rho1d[wi,:] )
+                                uj = np.copy( uR[wi,:] * rho1d[wi,:] )
                             else:
-                                ui    = np.copy( uL[wi,:] )
-                                uj    = np.copy( uR[wi,:] )
+                                ui = np.copy( uL[wi,:] )
+                                uj = np.copy( uR[wi,:] )
                             n     = ui.size
                             #A_ui = sp.fft.fft(ui)[fp] / n
                             #A_uj = sp.fft.fft(uj)[fp] / n
                             ui   *= window
                             uj   *= window
                             #ui  -= np.mean(ui) ## de-trend
                             #uj  -= np.mean(uj)
@@ -12000,102 +12698,70 @@
                         
                         ## divide off mean mass density
                         if density_scaling:
                             Euu_ijk /= rho_avg**2
                         
                         ## normalize such that ∫PSD=(co)variance
                         if normalize_psd_by_cov:
-                            if (uIuI_avg_ijk!=0.):
-                                energy_norm_fac = np.sum(df*Euu_ijk) / uIuI_avg_ijk
+                            if (uIuI_ijk!=0.):
+                                energy_norm_fac = np.sum(df*Euu_ijk) / uIuI_ijk
                             else:
                                 energy_norm_fac = 1.
                             Euu_ijk /= energy_norm_fac
-                            energy_norm_fac_arr[tag][xi,yi,zi] = energy_norm_fac
+                            energy_norm_fac_arr[xi,yi,zi] = energy_norm_fac
                         
-                        ## write
-                        Euu[tag][xi,yi,zi,:] = Euu_ijk
-                    
-                    if verbose: progress_bar.update()
-        if verbose: progress_bar.close()
-        
-        ## report energy normalization factors --> tmp,only rank 0 currently!
-        if normalize_psd_by_cov:
-            if verbose: print(72*'-')
-            for tag in Euu_scalars:
-                energy_norm_fac_min = energy_norm_fac_arr[tag].min()
-                energy_norm_fac_max = energy_norm_fac_arr[tag].max()
-                energy_norm_fac_avg = np.mean(energy_norm_fac_arr[tag], axis=(0,1,2), dtype=np.float64) ##.astype(np.float32)
-                if verbose:
-                    even_print('energy norm min/max/avg : %s'%tag, '%0.4f / %0.4f / %0.4f'%(energy_norm_fac_min,energy_norm_fac_max,energy_norm_fac_avg))
-            energy_norm_fac_arr = None ; del energy_norm_fac_arr
-        
-        # === average in [x,z] --> leave [y,f]
-        
-        Euu_      = np.zeros(shape=(nyr,nf) , dtype={'names':Euu_scalars, 'formats':Euu_scalars_dtypes})
-        uIuI_avg_ = np.zeros(shape=(nyr,)   , dtype={'names':Euu_scalars, 'formats':Euu_scalars_dtypes})
-        self.comm.Barrier()
+                        ## write to buffer
+                        Euu[xi,yi,zi,:] = Euu_ijk
+                        
+                        if verbose: progress_bar.update()
+            
+            ## average in [x,z]
+            Euu_avg[tag]  = np.mean( Euu  , axis=(0,2) , dtype=np.float64)
+            uIuI_avg[tag] = np.mean( uIuI , axis=(0,2) , dtype=np.float64)
+            
+            ## barrier per FFT scalar pair
+            self.comm.Barrier()
         
-        for tag in Euu_scalars:
-            Euu_[tag]      = np.mean( Euu[tag]      , axis=(0,2) , dtype=np.float64) #.astype(np.float32) ## avg in [x,z] --> leave [y,f]
-            uIuI_avg_[tag] = np.mean( uIuI_avg[tag] , axis=(0,2) , dtype=np.float64) #.astype(np.float32) ## avg in [x,z] --> leave [y]
-        Euu      = np.copy( Euu_ )
-        uIuI_avg = np.copy( uIuI_avg_ )
-        self.comm.Barrier()
+        if verbose: progress_bar.close()
         
         # === gather all results
         # --> arrays are very small at this point, just do 'lazy' gather/bcast, dont worry about buffers etc
         
-        G = self.comm.gather([self.rank, 
-                              Euu, uIuI_avg ], root=0)
+        G = self.comm.gather([ self.rank, np.copy(Euu_avg), np.copy(uIuI_avg) ], root=0)
         G = self.comm.bcast(G, root=0)
         
-        Euu      = np.zeros( (ny,nf) , dtype={'names':Euu_scalars, 'formats':Euu_scalars_dtypes})
+        Euu_avg  = np.zeros( (ny,nf) , dtype={'names':Euu_scalars, 'formats':Euu_scalars_dtypes})
         uIuI_avg = np.zeros( (ny,)   , dtype={'names':Euu_scalars, 'formats':Euu_scalars_dtypes})
         
         for ri in range(self.n_ranks):
             j = ri
             for GG in G:
                 if (GG[0]==ri):
                     for tag in Euu_scalars:
-                        Euu[tag][ryl[j][0]:ryl[j][1],:]    = GG[1][tag]
-                        uIuI_avg[tag][ryl[j][0]:ryl[j][1]] = GG[2][tag]
+                        Euu_avg[tag][ryl[j][0]:ryl[j][1],:] = GG[1][tag]
+                        uIuI_avg[tag][ryl[j][0]:ryl[j][1]]  = GG[2][tag]
                 else:
                     pass
         if verbose: print(72*'-')
         
         # === save results
         if (self.rank==0):
             
-            data['Euu']      = Euu
-            data['uIuI_avg'] = uIuI_avg
-            
-            ## avg in [x,z] --> leave 0D scalar
-            sc_l_in  = np.mean(sc_l_in  , axis=(0,1) , dtype=np.float64) #.astype(np.float32)
-            sc_u_in  = np.mean(sc_u_in  , axis=(0,1) , dtype=np.float64) #.astype(np.float32)
-            sc_t_in  = np.mean(sc_t_in  , axis=(0,1) , dtype=np.float64) #.astype(np.float32)
-            sc_l_out = np.mean(sc_l_out , axis=(0,1) , dtype=np.float64) #.astype(np.float32)
-            sc_u_out = np.mean(sc_u_out , axis=(0,1) , dtype=np.float64) #.astype(np.float32)
-            sc_t_out = np.mean(sc_t_out , axis=(0,1) , dtype=np.float64) #.astype(np.float32)
-            
-            data['sc_l_in']  = sc_l_in
-            data['sc_u_in']  = sc_u_in
-            data['sc_t_in']  = sc_t_in
-            data['sc_l_out'] = sc_l_out
-            data['sc_u_out'] = sc_u_out
-            data['sc_t_out'] = sc_t_out
+            data['Euu']  = Euu_avg
+            data['uIuI'] = uIuI_avg
             
             with open(fn_dat_fft,'wb') as f:
                 pickle.dump(data, f, protocol=4)
             print('--w-> %s : %0.2f [MB]'%(fn_dat_fft,os.path.getsize(fn_dat_fft)/1024**2))
         
         # ===
         
         self.comm.Barrier()
         
-        if verbose: print('\n'+72*'-')
+        if verbose: print(72*'-')
         if verbose: print('total time : rgd.calc_turb_spectrum_time() : %s'%format_time_string((timeit.default_timer() - t_start_func)))
         if verbose: print(72*'-')
         
         return
     
     def calc_turb_spectrum_span(self, **kwargs):
         '''
@@ -12135,15 +12801,15 @@
         if (ry>self.ny):
             raise AssertionError('ry>self.ny')
         if (rz>self.nz):
             raise AssertionError('rz>self.nz')
         if (rt>self.nt):
             raise AssertionError('rt>self.nt')
         
-        # === distribute 4D data over ranks
+        # === distribute 4D data over ranks --> here only in [y]
         
         #comm4d = self.comm.Create_cart(dims=[rx,ry,ry,rt], periods=[False,False,False,False], reorder=False)
         #t4d = comm4d.Get_coords(self.rank)
         
         #rxl_ = np.array_split(np.arange(self.nx,dtype=np.int64),min(rx,self.nx))
         ryl_ = np.array_split(np.arange(self.ny,dtype=np.int64),min(ry,self.ny))
         #rzl_ = np.array_split(np.arange(self.nz,dtype=np.int64),min(rz,self.nz))
@@ -12157,196 +12823,203 @@
         #rx1, rx2 = rxl[t4d[0]]; nxr = rx2 - rx1
         #ry1, ry2 = ryl[t4d[1]]; nyr = ry2 - ry1
         #rz1, rz2 = rzl[t4d[2]]; nzr = rz2 - rz1
         #rt1, rt2 = rtl[t4d[3]]; ntr = rt2 - rt1
         
         ry1,ry2 = ryl[self.rank]; nyr = ry2 - ry1
         
-        # === mean (dimensional) file name (for reading) : .dat
-        if (fn_dat_mean_dim is None):
-            fname_path = os.path.dirname(self.fname)
-            fname_base = os.path.basename(self.fname)
-            fname_root, fname_ext = os.path.splitext(fname_base)
-            fname_root = re.findall('io\S+_mpi_[0-9]+', fname_root)[0]
-            fname_dat_mean_base = fname_root+'_mean_dim.dat'
-            fn_dat_mean_dim = str(PurePosixPath(fname_path, fname_dat_mean_base))
+        # # === mean (dimensional) file name (for reading) : .dat
+        # if (fn_dat_mean_dim is None):
+        #     fname_path = os.path.dirname(self.fname)
+        #     fname_base = os.path.basename(self.fname)
+        #     fname_root, fname_ext = os.path.splitext(fname_base)
+        #     fname_root = re.findall('io\S+_mpi_[0-9]+', fname_root)[0]
+        #     fname_dat_mean_base = fname_root+'_mean_dim.dat'
+        #     fn_dat_mean_dim = str(PurePosixPath(fname_path, fname_dat_mean_base))
         
         # === fft file name (for writing) : dat
         if (fn_dat_fft is None):
             fname_path = os.path.dirname(self.fname)
             fname_base = os.path.basename(self.fname)
             fname_root, fname_ext = os.path.splitext(fname_base)
             fname_root = re.findall('io\S+_mpi_[0-9]+', fname_root)[0]
             fname_fft_dat_base = fname_root+'_turb_spec_span.dat'
             fn_dat_fft = str(PurePosixPath(fname_path, fname_fft_dat_base))
         
         if verbose: even_print('fn_rgd_prime'    , self.fname       )
-        if verbose: even_print('fn_dat_mean_dim' , fn_dat_mean_dim  )
+        #if verbose: even_print('fn_dat_mean_dim' , fn_dat_mean_dim  )
         if verbose: even_print('fn_dat_fft'      , fn_dat_fft       )
         if verbose: print(72*'-')
         
-        if not os.path.isfile(fn_dat_mean_dim):
-            raise FileNotFoundError('%s not found!'%fn_dat_mean_dim)
+        #if not os.path.isfile(fn_dat_mean_dim):
+        #    raise FileNotFoundError('%s not found!'%fn_dat_mean_dim)
         
-        # === read in data (mean dim) --> every rank gets full [x,z]
-        with open(fn_dat_mean_dim,'rb') as f:
-            data_mean_dim = pickle.load(f)
-        fmd = type('foo', (object,), data_mean_dim)
+        # # === read in data (mean dim) --> every rank gets full [x,z]
+        # with open(fn_dat_mean_dim,'rb') as f:
+        #     data_mean_dim = pickle.load(f)
+        # fmd = type('foo', (object,), data_mean_dim)
         
         self.comm.Barrier()
         
         ## the data dictionary to be pickled later
         data = {}
         
-        ## 2D dimensional quantities --> [x,z]
-        u_tau    = fmd.u_tau    # ; data['u_tau']    = u_tau
-        nu_wall  = fmd.nu_wall  # ; data['nu_wall']  = nu_wall
-        rho_wall = fmd.rho_wall # ; data['rho_wall'] = rho_wall
-        d99      = fmd.d99      # ; data['d99']      = d99
-        u99      = fmd.u99      # ; data['u99']      = u99
-        Re_tau   = fmd.Re_tau   # ; data['Re_tau']   = Re_tau
-        Re_theta = fmd.Re_theta # ; data['Re_theta'] = Re_theta
-        
-        ## mean [x,z] --> leave 0D scalar
-        u_tau_avg    = np.mean(fmd.u_tau    , axis=(0,1)) ; data['u_tau_avg']    = u_tau_avg
-        nu_wall_avg  = np.mean(fmd.nu_wall  , axis=(0,1)) ; data['nu_wall_avg']  = nu_wall_avg
-        rho_wall_avg = np.mean(fmd.rho_wall , axis=(0,1)) ; data['rho_wall_avg'] = rho_wall_avg
-        d99_avg      = np.mean(fmd.d99      , axis=(0,1)) ; data['d99_avg']      = d99_avg
-        u99_avg      = np.mean(fmd.u99      , axis=(0,1)) ; data['u99_avg']      = u99_avg
-        Re_tau_avg   = np.mean(fmd.Re_tau   , axis=(0,1)) ; data['Re_tau_avg']   = Re_tau_avg
-        Re_theta_avg = np.mean(fmd.Re_theta , axis=(0,1)) ; data['Re_theta_avg'] = Re_theta_avg
-        
-        ## mean [x,z] --> leave 1D [y]
-        rho_avg = np.mean(fmd.rho,axis=(0,2))
-        data['rho_avg'] = rho_avg
+        if ('data_dim' not in self):
+            raise ValueError('group data_dim not present')
         
-        # === 2D inner scales --> [x,z]
-        sc_l_in = nu_wall / u_tau
-        sc_u_in = u_tau
-        sc_t_in = nu_wall / u_tau**2
+        ## put all data from 'data_dim' into the dictionary data which will be pickled at the end
+        for dsn in self['data_dim'].keys():
+            d_ = np.copy( self[f'data_dim/{dsn}'][()] )
+            if (d_.ndim == 0):
+                d_ = float(d_)
+            data[dsn] = d_
         
-        # === 2D outer scales --> [x,z]
-        sc_l_out = d99
-        sc_u_out = u99
-        sc_t_out = d99/u99
+        ## 1D
+        rho_avg = np.copy( self['data_dim/rho'][()] )
+        u_avg   = np.copy( self['data_dim/u'][()]   )
         
-        np.testing.assert_allclose( fmd.sc_l_in  , sc_l_in  , rtol=1e-14 )
-        np.testing.assert_allclose( fmd.sc_l_out , sc_l_out , rtol=1e-14 )
-        np.testing.assert_allclose( fmd.sc_u_in  , sc_u_in  , rtol=1e-14 )
-        np.testing.assert_allclose( fmd.sc_u_out , sc_u_out , rtol=1e-14 )
-        np.testing.assert_allclose( fmd.sc_t_in  , sc_t_in  , rtol=1e-14 )
-        np.testing.assert_allclose( fmd.sc_t_out , sc_t_out , rtol=1e-14 )
-        
-        sc_l_in_avg  = np.mean(sc_l_in  , axis=(0,1))
-        sc_l_out_avg = np.mean(sc_l_out , axis=(0,1))
-        sc_u_in_avg  = np.mean(sc_u_in  , axis=(0,1))
-        sc_u_out_avg = np.mean(sc_u_out , axis=(0,1))
-        sc_t_in_avg  = np.mean(sc_t_in  , axis=(0,1))
-        sc_t_out_avg = np.mean(sc_t_out , axis=(0,1))
-        
-        # === check
-        np.testing.assert_allclose( fmd.lchar   , self.lchar   , rtol=1e-14 )
-        np.testing.assert_allclose( fmd.U_inf   , self.U_inf   , rtol=1e-14 )
-        np.testing.assert_allclose( fmd.rho_inf , self.rho_inf , rtol=1e-14 )
-        np.testing.assert_allclose( fmd.T_inf   , self.T_inf   , rtol=1e-14 )
-        np.testing.assert_allclose( fmd.nx      , self.nx      , rtol=1e-14 )
-        np.testing.assert_allclose( fmd.ny      , self.ny      , rtol=1e-14 )
-        np.testing.assert_allclose( fmd.nz      , self.nz      , rtol=1e-14 )
-        np.testing.assert_allclose( fmd.xs      , self.x       , rtol=1e-14 )
-        np.testing.assert_allclose( fmd.ys      , self.y       , rtol=1e-14 )
-        np.testing.assert_allclose( fmd.zs      , self.z       , rtol=1e-14 )
+        ## 0D
+        u_tau    = float( self['data_dim/u_tau'][()]    )
+        nu_wall  = float( self['data_dim/nu_wall'][()]  )
+        rho_wall = float( self['data_dim/rho_wall'][()] )
+        d99      = float( self['data_dim/d99'][()]      )
+        u_99     = float( self['data_dim/u_99'][()]     )
+        Re_tau   = float( self['data_dim/Re_tau'][()]   )
+        Re_theta = float( self['data_dim/Re_theta'][()] )
+        sc_u_in  = float( self['data_dim/sc_u_in'][()]  )
+        sc_l_in  = float( self['data_dim/sc_l_in'][()]  )
+        sc_t_in  = float( self['data_dim/sc_t_in'][()]  )
+        sc_u_out = float( self['data_dim/sc_u_out'][()] )
+        sc_l_out = float( self['data_dim/sc_l_out'][()] )
+        sc_t_out = float( self['data_dim/sc_t_out'][()] )
+        
+        ## these are recalculated and checked in next step
+        z1d_ = np.copy( self['data_dim/z1d'][()] )
+        dz0_ = np.copy( self['data_dim/dz0'][()] )
+        dt_  = np.copy( self['data_dim/dt'][()]  )
+        
+        # ===
+        
+        ## get size of infile
+        fsize = os.path.getsize(self.fname)/1024**3
+        if verbose: even_print(os.path.basename(self.fname),'%0.1f [GB]'%fsize)
+        if verbose: even_print('nx','%i'%self.nx)
+        if verbose: even_print('ny','%i'%self.ny)
+        if verbose: even_print('nz','%i'%self.nz)
+        if verbose: even_print('nt','%i'%self.nt)
+        if verbose: even_print('ngp','%0.1f [M]'%(self.ngp/1e6,))
+        if verbose: print(72*'-')
         
+        ## 0D scalars
         lchar   = self.lchar   ; data['lchar']   = lchar
         U_inf   = self.U_inf   ; data['U_inf']   = U_inf
         rho_inf = self.rho_inf ; data['rho_inf'] = rho_inf
         T_inf   = self.T_inf   ; data['T_inf']   = T_inf
         
+        #data['M_inf'] = self.M_inf
         data['Ma'] = self.Ma
         data['Pr'] = self.Pr
         
+        ## read in 1D coordinate arrays, then re-dimensionalize [m]
+        x = np.copy( self['dims/x'][()] * self.lchar )
+        y = np.copy( self['dims/y'][()] * self.lchar )
+        z = np.copy( self['dims/z'][()] * self.lchar )
+        
         nx = self.nx ; data['nx'] = nx
         ny = self.ny ; data['ny'] = ny
         nz = self.nz ; data['nz'] = nz
         nt = self.nt ; data['nt'] = nt
         
-        ## dimless (inlet)
-        xd = self.x
-        yd = self.y
-        zd = self.z
-        td = self.t
+        t = np.copy( self['dims/t'][()] * self.tchar )
         
-        ## dimensional [m] / [s]
+        # ## dimless (inlet/characteristic)
+        # xd = self.x
+        # yd = self.y
+        # zd = self.z
+        # td = self.t
+        
+        ## redimensionalize coordinates --> [m],[s],[m/s],etc.
         x      = self.x * lchar
         y      = self.y * lchar
         z      = self.z * lchar
         t      = self.t * (lchar/U_inf)
         t_meas = t[-1]-t[0]
         dt     = self.dt * (lchar/U_inf)
         
-        # dz0 = z[ 1]-z[0]
+        z1d = np.copy(z)
         
         ## check if constant Δz (calculate Δz+ later)
-        dz0_ = np.diff(z)[0]
-        if np.all(np.isclose(np.diff(z), dz0_, rtol=1e-7)):
-            dz0 = dz0_
-        else:
-            raise ValueError
+        dz0 = np.diff(z1d)[0]
+        if not np.all(np.isclose(np.diff(z1d), dz0, rtol=1e-7)):
+            raise NotImplementedError
         
-        zrange = z[-1]-z[0]
+        ## dimensional [s]
+        dt = self.dt * self.tchar
+        np.testing.assert_allclose(dt, t[1]-t[0], rtol=1e-14, atol=1e-14)
+        
+        t_meas = self.duration * self.tchar
+        np.testing.assert_allclose(t_meas, t.max()-t.min(), rtol=1e-14, atol=1e-14)
+        
+        ## check against values in 'data_dim' (imported above)
+        np.testing.assert_allclose(dt  , dt_  , rtol=1e-14, atol=1e-14)
+        np.testing.assert_allclose(dz0 , dz0_ , rtol=1e-14, atol=1e-14)
+        np.testing.assert_allclose(z1d , z1d_ , rtol=1e-14, atol=1e-14)
+        
+        zrange = z1d.max() - z1d.min()
         
         data['x'] = x
         data['y'] = y
         data['z'] = z
+        #data['z1d'] = z1d
+        
         data['t'] = t
         data['t_meas'] = t_meas
         data['dt'] = dt
         data['dz0'] = dz0
         data['zrange'] = zrange
         
-        np.testing.assert_equal(nx,x.size)
-        np.testing.assert_equal(ny,y.size)
-        np.testing.assert_equal(nz,z.size)
-        np.testing.assert_equal(nt,t.size)
-        np.testing.assert_allclose(dt, t[1]-t[0], rtol=1e-8)
+        if verbose: even_print('Δt/tchar','%0.8f'%(dt/self.tchar))
+        if verbose: even_print('Δt','%0.3e [s]'%(dt,))
+        if verbose: even_print('duration/tchar','%0.1f'%(self.duration,))
+        if verbose: even_print('duration','%0.3e [s]'%(self.duration*self.tchar,))
+        if verbose: print(72*'-')
         
-        # === report
+        ## report
         if verbose:
-            even_print('nx'     , '%i'        %nx     )
-            even_print('ny'     , '%i'        %ny     )
-            even_print('nz'     , '%i'        %nz     )
-            even_print('nt'     , '%i'        %nt     )
-            even_print('dt'     , '%0.5e [s]' %dt     )
-            even_print('t_meas' , '%0.5e [s]' %t_meas )
-            even_print('dz0'    , '%0.5e [m]' %dz0     )
-            even_print('zrange' , '%0.5e [m]' %zrange  )
+            even_print('dt'     , '%0.5e [s]' % dt      )
+            even_print('t_meas' , '%0.5e [s]' % t_meas  )
+            even_print('dz0'    , '%0.5e [m]' % dz0     )
+            even_print('zrange' , '%0.5e [m]' % zrange  )
             print(72*'-')
         
+        ## report
         if verbose:
-            even_print('Re_τ'    , '%0.1f'        % Re_tau_avg    )
-            even_print('Re_θ'    , '%0.1f'        % Re_theta_avg  )
-            even_print('δ99'     , '%0.5e [m]'    % d99_avg       )
-            even_print('δ_ν=(ν_wall/u_τ)' , '%0.5e [m]' % sc_l_in_avg )
-            even_print('U_inf'  , '%0.3f [m/s]'   % U_inf         )
-            even_print('u_τ'    , '%0.3f [m/s]'   % u_tau_avg     )
-            even_print('ν_wall' , '%0.5e [m²/s]'  % nu_wall_avg   )
-            even_print('ρ_wall' , '%0.6f [kg/m³]' % rho_wall_avg  )
+            even_print('Re_τ'    , '%0.1f'        % Re_tau    )
+            even_print('Re_θ'    , '%0.1f'        % Re_theta  )
+            even_print('δ99'     , '%0.5e [m]'    % d99       )
+            even_print('δ_ν=(ν_wall/u_τ)' , '%0.5e [m]' % sc_l_in )
+            even_print('U_inf'  , '%0.3f [m/s]'   % self.U_inf )
+            even_print('u_τ'    , '%0.3f [m/s]'   % u_tau     )
+            even_print('ν_wall' , '%0.5e [m²/s]'  % nu_wall   )
+            even_print('ρ_wall' , '%0.6f [kg/m³]' % rho_wall  )
             ##
-            even_print( 'Δz+' , '%0.3f'%(dz0/sc_l_in_avg) )
-            even_print( 'Δt+' , '%0.3f'%(dt/sc_t_in_avg) )
+            even_print( 'Δz+'        , '%0.3f'%(dz0/sc_l_in) )
+            even_print( 'zrange/δ99' , '%0.3f'%(zrange/d99)  )
+            even_print( 'Δt+'        , '%0.3f'%(dt/sc_t_in)  )
             print(72*'-')
         
         # t_eddy = t_meas / ( d99_avg / u_tau_avg )
         # 
         # if verbose:
         #     even_print('t_meas/(δ99/u_τ) = t_eddy' , '%0.2f'%t_eddy)
         #     even_print('t_meas/(δ99/u99)'          , '%0.2f'%(t_meas/(d99_avg/u99_avg)))
         #     even_print('t_meas/(20·δ99/u99)'       , '%0.2f'%(t_meas/(20*d99_avg/u99_avg)))
         #     print(72*'-')
         
-        # === get wavenumber vector
+        ## get wavenumber vector
         kz_full = sp.fft.fftfreq(n=nz, d=dz0) * ( 2 * np.pi )
         kzp     = np.where(kz_full>0)
         kz      = np.copy(kz_full[kzp])
         dkz     = kz[1]-kz[0]
         nkz     = kz.size
         
         data['kz']  = kz
@@ -12355,103 +13028,109 @@
         
         if verbose:
             even_print('kz min','%0.1f [1/m]'%kz.min())
             even_print('kz max','%0.1f [1/m]'%kz.max())
             even_print('dkz','%0.1f [1/m]'%dkz)
             even_print('nkz','%i'%nkz)
             
-            kz_inner = np.copy( kz * sc_l_in_avg  )
-            kz_outer = np.copy( kz * sc_l_out_avg )
+            kz_inner = np.copy( kz * sc_l_in  )
+            kz_outer = np.copy( kz * sc_l_out )
             
             even_print('(kz·δ_ν) min' , '%0.5e [-]'%kz_inner.min())
             even_print('(kz·δ_ν) max' , '%0.5f [-]'%kz_inner.max())
-            even_print('(kz·δ99) min' , '%0.5e [-]'%kz_outer.min())
-            even_print('(kz·δ99) max' , '%0.5f [-]'%kz_outer.max())
+            even_print('(kz·δ99) min' , '%0.5f [-]'%kz_outer.min())
+            even_print('(kz·δ99) max' , '%0.5e [-]'%kz_outer.max())
             
             print(72*'-')
         
         # === read in data (prime) --> still dimless (char)
         
-        scalars = [ 'uI','vI','wI' , 'rho','uII','vII','wII' ]
-        #scalars = [ 'uI' ]
-        scalars_dtypes = [self.scalars_dtypes_dict[s] for s in scalars]
+        scalars = [ 'uI','vI','wI' , 'rho', 'uII','vII','wII' ]
+        scalars_dtypes = [ self.scalars_dtypes_dict[s] for s in scalars ]
         
         ## [var1, var2, density_scaling]
         fft_combis = [
                      [ 'uI'  , 'uI'  , False ],
                      [ 'vI'  , 'vI'  , False ],
                      [ 'wI'  , 'wI'  , False ],
                      [ 'uI'  , 'vI'  , False ],
+                     [ 'uI'  , 'wI'  , False ],
+                     [ 'vI'  , 'wI'  , False ],
                      [ 'uII' , 'uII' , True  ],
                      [ 'vII' , 'vII' , True  ],
                      [ 'wII' , 'wII' , True  ],
                      [ 'uII' , 'vII' , True  ],
+                     [ 'uII' , 'wII' , True  ],
+                     [ 'vII' , 'wII' , True  ],
                      ]
         
-        scalars_dtypes = [ self.scalars_dtypes_dict[s] for s in scalars ]
+        if verbose:
+            even_print('n turb spectrum (span) scalar combinations' , '%i'%(len(fft_combis),))
+            print(72*'-')
         
-        ## dtype of prime data (currently must be all same dtype)
-        if np.all( [ (dtp==np.float32) for dtp in scalars_dtypes ] ):
-            dtype_primes = np.float32
-        elif np.all( [ (dtp==np.float64) for dtp in scalars_dtypes ] ):
-            dtype_primes = np.float64
-        else:
-            raise NotImplementedError
+        ## decide if mass density will be needed
+        read_density = False
+        for cc in fft_combis:
+            scalar_L, scalar_R, density_scaling = cc
+            if density_scaling:
+                read_density = True
+                break
         
-        ## 5D [scalar][x,y,z,t] structured array
-        data_prime = np.zeros(shape=(self.nx, nyr, self.nz, self.nt), dtype={'names':scalars, 'formats':scalars_dtypes})
+        if verbose:
+            even_print('read ρ', str(read_density))
         
-        for scalar in scalars:
+        ## confirm 'rho' is not in locals
+        if read_density and ('rho' in locals()):
+            raise ValueError('rho alread in locals... check')
+        
+        if read_density:
             
-            dset = self[f'data/{scalar}']
-            dtype = dset.dtype
-            float_bytes = dtype.itemsize
+            ## buffer for rho ( !! NOT rhoI !! ) --> this is read from 'prime' file
+            rho = np.zeros(shape=(nx, nyr, nz, nt), dtype=np.float32)
             
+            dset = self['data/rho']
             self.comm.Barrier()
             t_start = timeit.default_timer()
-            with dset.collective:
-                data_prime[scalar] = np.copy( dset[:,:,ry1:ry2,:].T )
+            if self.usingmpi:
+                with dset.collective:
+                    rho[:,:,:,:] = np.copy( dset[:,:,ry1:ry2,:].T )
+            else:
+                rho[:,:,:,:] = np.copy( dset[()].T )
             self.comm.Barrier()
             t_delta = timeit.default_timer() - t_start
-            
-            data_gb = float_bytes * self.nx * self.ny * self.nz * self.nt / 1024**3
-            
+            data_gb = 4 * self.nx * self.ny * self.nz * self.nt / 1024**3
             if verbose:
-                even_print('read: %s'%scalar, '%0.3f [GB]  %0.3f [s]  %0.3f [GB/s]'%(data_gb,t_delta,(data_gb/t_delta)))
+                even_print( 'read: rho','%0.3f [GB]  %0.3f [s]  %0.3f [GB/s]'%(data_gb,t_delta,(data_gb/t_delta)))
+            
+            ## re-dimensionalize rho
+            rho *= rho_inf
         
-        # === redimensionalize prime data
+        # ===
         
-        for var in data_prime.dtype.names:
-            if var in ['u','v','w', 'uI','vI','wI', 'uII','vII','wII']:
-                data_prime[var] *= U_inf
-            elif var in ['r_uII','r_vII','r_wII']:
-                data_prime[var] *= (U_inf*rho_inf)
-            elif var in ['T','TI','TII']:
-                data_prime[var] *= T_inf
-            elif var in ['r_TII']:
-                data_prime[var] *= (T_inf*rho_inf)
-            elif var in ['rho','rhoI']:
-                data_prime[var] *= rho_inf
-            elif var in ['p','pI','pII']:
-                data_prime[var] *= (rho_inf * U_inf**2)
-            else:
-                raise ValueError('condition needed for redimensionalizing \'%s\''%var)
+        ## dtype of prime data (currently must be all same dtype)
+        if np.all( [ (dtp==np.float32) for dtp in scalars_dtypes ] ):
+            dtype_primes = np.float32
+        elif np.all( [ (dtp==np.float64) for dtp in scalars_dtypes ] ):
+            dtype_primes = np.float64
+        else:
+            raise NotImplementedError
         
         ## force the ∫PSD == (co)variance
         ## this usually represents about a 1-2% power correction which comes about due to 
         ##   non-stationarity of windowed data
         normalize_psd_by_cov = False
         
-        ## initialize buffers
-        Euu_scalars         = [ '%s%s'%(cc[0],cc[1]) for cc in fft_combis ]
-        Euu_scalars_dtypes  = [ dtype_primes for s in Euu_scalars ]
-        Euu                 = np.zeros(shape=(self.nx, nyr, self.nt, nkz) , dtype={'names':Euu_scalars, 'formats':Euu_scalars_dtypes})
-        uIuI_avg            = np.zeros(shape=(self.nx, nyr, self.nt)      , dtype={'names':Euu_scalars, 'formats':Euu_scalars_dtypes})
+        Euu_scalars        = [ '%s%s'%(cc[0],cc[1]) for cc in fft_combis ]
+        Euu_scalars_dtypes = [ dtype_primes for s in Euu_scalars ]
+        
+        ## buffers (for averaged data)
+        Euu_avg  = np.zeros(shape=(nyr, nkz) , dtype={'names':Euu_scalars, 'formats':Euu_scalars_dtypes})
+        uIuI_avg = np.zeros(shape=(nyr,    ) , dtype={'names':Euu_scalars, 'formats':Euu_scalars_dtypes})
         if normalize_psd_by_cov:
-            energy_norm_fac_arr = np.zeros(shape=(self.nx, nyr, self.nt) , dtype={'names':Euu_scalars, 'formats':Euu_scalars_dtypes}) ## just for monitoring
+            energy_norm_fac_arr = np.zeros(shape=(self.nx, nyr, self.nz) , dtype={'names':Euu_scalars, 'formats':Euu_scalars_dtypes}) ## just for monitoring
         
         ## check memory
         mem_total_gb = psutil.virtual_memory().total/1024**3
         mem_avail_gb = psutil.virtual_memory().available/1024**3
         mem_free_gb  = psutil.virtual_memory().free/1024**3
         if verbose:
             even_print('mem total',     '%0.1f [GB]'%(mem_total_gb,))
@@ -12469,48 +13148,117 @@
             window = np.ones(win_len, dtype=np.float64)
         if verbose:
             even_print('window type', '\'%s\''%str(window_type))
         
         ## sum of sqrt of window: needed for power normalization
         sum_sqrt_win = np.sum(np.sqrt(window))
         
+        if verbose:
+            even_print('sum(sqrt(window)) / win_len', '%0.5f'%(sum_sqrt_win/win_len))
+        
+        if verbose:
+            print(72*'-')
+        
         # === main loop
         
+        ## main loop --> turbulent spectrum in [Δz] at every [x,y,t]
         self.comm.Barrier()
-        if verbose: progress_bar = tqdm(total=self.nx*nyr*self.nt, ncols=100, desc='fft', leave=False)
-        for xi in range(self.nx):
-            for yi in range(nyr):
-                for ti in range(self.nt):
-                    for cci,cc in enumerate(fft_combis):
-                        
-                        tag = Euu_scalars[cci]
-                        ccL,ccR,density_scaling = cc
+        if verbose:
+            progress_bar = tqdm(total=len(fft_combis)*nx*nyr*nt, ncols=100, desc='calc_turb_spectrum_span()', leave=False, file=sys.stdout)
+        
+        for cci,cc in enumerate(fft_combis):
+            
+            scalar_L, scalar_R, density_scaling = cc
+            tag = '%s%s'%(scalar_L, scalar_R)
+            
+            ## check if autocorrelation, in which case don't read twice
+            if (scalar_L==scalar_R):
+                scalars = [ scalar_L ]
+            else:
+                scalars = [ scalar_L, scalar_R ]
+            
+            scalars_dtypes = [ self.scalars_dtypes_dict[s] for s in scalars ]
+            
+            ## prime data buffer
+            ## 5D [scalar][x,y,z,t] structured array
+            data_prime = np.zeros(shape=(nx, nyr, nz, nt), dtype={'names':scalars, 'formats':scalars_dtypes})
+            
+            ## unsteady data buffers
+            Euu  = np.zeros(shape=(self.nx, nyr, self.nt, nkz), dtype=np.float32)
+            uIuI = np.zeros(shape=(self.nx, nyr, self.nt),      dtype=np.float32)
+            
+            ## read prime data
+            for scalar in scalars:
+                dset = self['data/%s'%scalar]
+                self.comm.Barrier()
+                t_start = timeit.default_timer()
+                if self.usingmpi:
+                    with dset.collective:
+                        data_prime[scalar][:,:,:,:] = np.copy( dset[:,:,ry1:ry2,:].T )
+                else:
+                    data_prime[scalar][:,:,:,:] = np.copy( dset[()].T )
+                self.comm.Barrier()
+                t_delta = timeit.default_timer() - t_start
+                data_gb = 4 * self.nx * self.ny * self.nz * self.nt / 1024**3
+                if verbose:
+                    tqdm.write(even_print('read: %s'%scalar, '%0.3f [GB]  %0.3f [s]  %0.3f [GB/s]'%(data_gb,t_delta,(data_gb/t_delta)), s=True))
+            
+            ## redimensionalize prime data
+            for var in data_prime.dtype.names:
+                if var in ['u','v','w', 'uI','vI','wI', 'uII','vII','wII']:
+                    data_prime[var] *= U_inf
+                elif var in ['r_uII','r_vII','r_wII']:
+                    data_prime[var] *= (U_inf*rho_inf)
+                elif var in ['T','TI','TII']:
+                    data_prime[var] *= T_inf
+                elif var in ['r_TII']:
+                    data_prime[var] *= (T_inf*rho_inf)
+                elif var in ['rho','rhoI']:
+                    data_prime[var] *= rho_inf
+                elif var in ['p','pI','pII']:
+                    data_prime[var] *= (rho_inf * U_inf**2)
+                else:
+                    raise ValueError('condition needed for redimensionalizing \'%s\''%var)
+            
+            ## print names of components being cross-correlated
+            if verbose:
+                if density_scaling:
+                    fancy_tag = '<ρ·%s,ρ·%s>'%(scalar_L,scalar_R)
+                else:
+                    fancy_tag = '<%s,%s>'%(scalar_L,scalar_R)
+                tqdm.write(even_print('running Δz fft calc', fancy_tag, s=True))
+            
+            for xi in range(self.nx):
+                for yi in range(nyr):
+                    for ti in range(self.nt):
                         
-                        uL = np.copy( data_prime[ccL][xi,yi,:,ti] )
-                        uR = np.copy( data_prime[ccR][xi,yi,:,ti] )
+                        uL = np.copy( data_prime[scalar_L][xi,yi,:,ti] )
+                        uR = np.copy( data_prime[scalar_R][xi,yi,:,ti] )
                         
-                        if ('rho' in data_prime.dtype.names):
-                            rho     = np.copy( data_prime['rho'][xi,yi,:,ti] )
-                            rho_avg = np.mean( rho, dtype=np.float64 )
+                        if density_scaling:
+                            #rho1d = np.copy( rho[xi,yi,zi,:] )
+                            rho1d = np.copy( rho[xi,yi,:,ti] )
+                            rho_avg = np.mean( rho1d, dtype=np.float64 )
                         else:
-                            rho     = None
+                            rho1d   = None
                             rho_avg = None
                         
                         # ===
                         
                         if density_scaling:
-                            uIuI_avg_ijk = np.mean(uL*uR*rho, dtype=np.float64) / rho_avg
+                            uIuI_ijk = np.mean(uL*uR*rho1d, dtype=np.float64) / rho_avg
                         else:
-                            uIuI_avg_ijk = np.mean(uL*uR,     dtype=np.float64)
+                            uIuI_ijk = np.mean(uL*uR, dtype=np.float64)
                         
-                        uIuI_avg[tag][xi,yi,ti] = uIuI_avg_ijk
+                        ## write to buffer
+                        uIuI[xi,yi,ti] = uIuI_ijk
                         
                         if density_scaling:
-                            ui = np.copy( uL * rho )
-                            uj = np.copy( uR * rho )
+                            ui = np.copy( uL * rho1d )
+                            uj = np.copy( uR * rho1d )
                         else:
                             ui = np.copy( uL )
                             uj = np.copy( uR )
                         
                         n     = ui.size
                         #A_ui = sp.fft.fft(ui)[fp] / n
                         #A_uj = sp.fft.fft(uj)[fp] / n
@@ -12524,107 +13272,83 @@
                         
                         ## divide off mean mass density
                         if density_scaling:
                             Euu_ijk /= rho_avg**2
                         
                         ## normalize such that ∫PSD=(co)variance
                         if normalize_psd_by_cov:
-                            if (uIuI_avg_ijk!=0.):
-                                energy_norm_fac = np.sum(dkz*Euu_ijk) / uIuI_avg_ijk
+                            if (uIuI_ijk!=0.):
+                                energy_norm_fac = np.sum(dkz*Euu_ijk) / uIuI_ijk
                             else:
                                 energy_norm_fac = 1.
                             Euu_ijk /= energy_norm_fac
-                            energy_norm_fac_arr[tag][xi,yi,ti] = energy_norm_fac
+                            energy_norm_fac_arr[xi,yi,ti] = energy_norm_fac
                         
-                        ## write
-                        Euu[tag][xi,yi,ti,:] = Euu_ijk
-                    
-                    if verbose: progress_bar.update()
-        if verbose: progress_bar.close()
-        
-        ## report energy normalization factors --> tmp,only rank 0 currently!
-        if normalize_psd_by_cov:
-            if verbose: print(72*'-')
-            for tag in Euu_scalars:
-                energy_norm_fac_min = energy_norm_fac_arr[tag].min()
-                energy_norm_fac_max = energy_norm_fac_arr[tag].max()
-                energy_norm_fac_avg = np.mean(energy_norm_fac_arr[tag], axis=(0,1,2), dtype=np.float64)
-                if verbose:
-                    even_print('energy norm min/max/avg : %s'%tag, '%0.4f / %0.4f / %0.4f'%(energy_norm_fac_min,energy_norm_fac_max,energy_norm_fac_avg))
-            energy_norm_fac_arr = None ; del energy_norm_fac_arr
-        
-        # === average in [x,t] --> leave [y,kz]
-        
-        Euu_      = np.zeros(shape=(nyr,nkz) , dtype={'names':Euu_scalars, 'formats':Euu_scalars_dtypes})
-        uIuI_avg_ = np.zeros(shape=(nyr,)    , dtype={'names':Euu_scalars, 'formats':Euu_scalars_dtypes})
-        self.comm.Barrier()
+                        ## write to buffer
+                        Euu[xi,yi,ti,:] = Euu_ijk
+                        
+                        if verbose: progress_bar.update()
+            
+            ## average in [x,t] --> leave [y,kz]
+            Euu_avg[tag]  = np.mean( Euu  , axis=(0,2) , dtype=np.float64)
+            uIuI_avg[tag] = np.mean( uIuI , axis=(0,2) , dtype=np.float64)
+            
+            ## barrier per FFT scalar pair
+            self.comm.Barrier()
         
-        for tag in Euu_scalars:
-            Euu_[tag]      = np.mean( Euu[tag]      , axis=(0,2) , dtype=np.float64) #.astype(np.float32) ## avg in [x,t] --> leave [y,kz]
-            uIuI_avg_[tag] = np.mean( uIuI_avg[tag] , axis=(0,2) , dtype=np.float64) #.astype(np.float32) ## avg in [x,t] --> leave [y]
-        Euu      = np.copy( Euu_ )
-        uIuI_avg = np.copy( uIuI_avg_ )
-        self.comm.Barrier()
+        if verbose: progress_bar.close()
         
         # === gather all results
         # --> arrays are very small at this point, just do 'lazy' gather/bcast, dont worry about buffers etc
         
-        G = self.comm.gather([self.rank, 
-                              Euu, uIuI_avg ], root=0)
+        G = self.comm.gather([ self.rank, np.copy(Euu_avg), np.copy(uIuI_avg) ], root=0)
         G = self.comm.bcast(G, root=0)
         
-        Euu      = np.zeros( (ny,nkz) , dtype={'names':Euu_scalars, 'formats':Euu_scalars_dtypes})
+        Euu_avg  = np.zeros( (ny,nkz) , dtype={'names':Euu_scalars, 'formats':Euu_scalars_dtypes})
         uIuI_avg = np.zeros( (ny,)    , dtype={'names':Euu_scalars, 'formats':Euu_scalars_dtypes})
         
         for ri in range(self.n_ranks):
             j = ri
             for GG in G:
                 if (GG[0]==ri):
                     for tag in Euu_scalars:
-                        Euu[tag][ryl[j][0]:ryl[j][1],:]    = GG[1][tag]
-                        uIuI_avg[tag][ryl[j][0]:ryl[j][1]] = GG[2][tag]
+                        Euu_avg[tag][ryl[j][0]:ryl[j][1],:] = GG[1][tag]
+                        uIuI_avg[tag][ryl[j][0]:ryl[j][1]]  = GG[2][tag]
                 else:
                     pass
         if verbose: print(72*'-')
         
         # === save results
         if (self.rank==0):
             
-            data['Euu']      = Euu
+            data['Euu']      = Euu_avg
             data['uIuI_avg'] = uIuI_avg
             
-            ## avg in [x,z] --> leave 0D scalar
-            sc_l_in  = np.mean(sc_l_in  , axis=(0,1) , dtype=np.float64) #.astype(np.float32)
-            sc_u_in  = np.mean(sc_u_in  , axis=(0,1) , dtype=np.float64) #.astype(np.float32)
-            sc_t_in  = np.mean(sc_t_in  , axis=(0,1) , dtype=np.float64) #.astype(np.float32)
-            sc_l_out = np.mean(sc_l_out , axis=(0,1) , dtype=np.float64) #.astype(np.float32)
-            sc_u_out = np.mean(sc_u_out , axis=(0,1) , dtype=np.float64) #.astype(np.float32)
-            sc_t_out = np.mean(sc_t_out , axis=(0,1) , dtype=np.float64) #.astype(np.float32)
-            
-            data['sc_l_in']  = sc_l_in
-            data['sc_u_in']  = sc_u_in
-            data['sc_t_in']  = sc_t_in
-            data['sc_l_out'] = sc_l_out
-            data['sc_u_out'] = sc_u_out
-            data['sc_t_out'] = sc_t_out
-            
             with open(fn_dat_fft,'wb') as f:
                 pickle.dump(data, f, protocol=4)
             print('--w-> %s : %0.2f [MB]'%(fn_dat_fft,os.path.getsize(fn_dat_fft)/1024**2))
         
         # ===
         
         self.comm.Barrier()
         
-        if verbose: print('\n'+72*'-')
+        if verbose: print(72*'-')
         if verbose: print('total time : rgd.calc_turb_spectrum_span() : %s'%format_time_string((timeit.default_timer() - t_start_func)))
         if verbose: print(72*'-')
         
         return
     
+    def calc_turb_spectrum_2d_span_time(self, **kwargs):
+        '''
+        calculate 2D FFT in [z,t] at every [x,y], avg in [x]
+        - designed for analyzing unsteady, thin planes in [x]
+        '''
+        pass
+        return
+    
     def calc_ccor_time(self, **kwargs):
         '''
         calculate cross-correlation in [t] and avg in [x,z] --> leave [y,Δt]
         - designed for analyzing unsteady, thin planes in [x]
         '''
         if (self.rank==0):
             verbose = True
@@ -12679,217 +13403,226 @@
         #rx1, rx2 = rxl[t4d[0]]; nxr = rx2 - rx1
         #ry1, ry2 = ryl[t4d[1]]; nyr = ry2 - ry1
         #rz1, rz2 = rzl[t4d[2]]; nzr = rz2 - rz1
         #rt1, rt2 = rtl[t4d[3]]; ntr = rt2 - rt1
         
         ry1,ry2 = ryl[self.rank]; nyr = ry2 - ry1
         
-        # === mean dimensional file name (for reading) : .dat
-        if (fn_dat_mean_dim is None):
-            fname_path = os.path.dirname(self.fname)
-            fname_base = os.path.basename(self.fname)
-            fname_root, fname_ext = os.path.splitext(fname_base)
-            fname_root = re.findall('io\S+_mpi_[0-9]+', fname_root)[0]
-            fname_dat_mean_base = fname_root+'_mean_dim.dat'
-            fn_dat_mean_dim = str(PurePosixPath(fname_path, fname_dat_mean_base))
+        # # === mean dimensional file name (for reading) : .dat
+        # if (fn_dat_mean_dim is None):
+        #     fname_path = os.path.dirname(self.fname)
+        #     fname_base = os.path.basename(self.fname)
+        #     fname_root, fname_ext = os.path.splitext(fname_base)
+        #     fname_root = re.findall('io\S+_mpi_[0-9]+', fname_root)[0]
+        #     fname_dat_mean_base = fname_root+'_mean_dim.dat'
+        #     fn_dat_mean_dim = str(PurePosixPath(fname_path, fname_dat_mean_base))
         
         # === cross-correlation file name (for writing) : dat
         if (fn_dat_ccor_time is None):
             fname_path = os.path.dirname(self.fname)
             fname_base = os.path.basename(self.fname)
             fname_root, fname_ext = os.path.splitext(fname_base)
             fname_root = re.findall('io\S+_mpi_[0-9]+', fname_root)[0]
             fname_ccor_time_dat_base = fname_root+'_ccor_time.dat'
             fn_dat_ccor_time = str(PurePosixPath(fname_path, fname_ccor_time_dat_base))
         
         if verbose: even_print('fn_rgd_prime'     , self.fname       )
-        if verbose: even_print('fn_dat_mean_dim'  , fn_dat_mean_dim  )
+        #if verbose: even_print('fn_dat_mean_dim'  , fn_dat_mean_dim  )
         if verbose: even_print('fn_dat_ccor_time' , fn_dat_ccor_time )
         if verbose: print(72*'-')
         
-        if not os.path.isfile(fn_dat_mean_dim):
-            raise FileNotFoundError('%s not found!'%fn_dat_mean_dim)
+        #if not os.path.isfile(fn_dat_mean_dim):
+        #    raise FileNotFoundError('%s not found!'%fn_dat_mean_dim)
         
-        # === read in data (mean dim) --> every rank gets full [x,z]
-        with open(fn_dat_mean_dim,'rb') as f:
-            data_mean_dim = pickle.load(f)
-        fmd = type('foo', (object,), data_mean_dim)
+        # # === read in data (mean dim) --> every rank gets full [x,z]
+        # with open(fn_dat_mean_dim,'rb') as f:
+        #     data_mean_dim = pickle.load(f)
+        # fmd = type('foo', (object,), data_mean_dim)
         
         self.comm.Barrier()
         
         ## the data dictionary to be pickled later
         data = {}
         
-        ## 2D dimensional quantities --> [x,z]
-        u_tau    = fmd.u_tau    # ; data['u_tau']    = u_tau
-        nu_wall  = fmd.nu_wall  # ; data['nu_wall']  = nu_wall
-        rho_wall = fmd.rho_wall # ; data['rho_wall'] = rho_wall
-        d99      = fmd.d99      # ; data['d99']      = d99
-        u99      = fmd.u99      # ; data['u99']      = u99
-        Re_tau   = fmd.Re_tau   # ; data['Re_tau']   = Re_tau
-        Re_theta = fmd.Re_theta # ; data['Re_theta'] = Re_theta
-        
-        ## mean [x,z] --> leave 0D scalar
-        u_tau_avg    = np.mean(fmd.u_tau    , axis=(0,1)) ; data['u_tau_avg']    = u_tau_avg
-        nu_wall_avg  = np.mean(fmd.nu_wall  , axis=(0,1)) ; data['nu_wall_avg']  = nu_wall_avg
-        rho_wall_avg = np.mean(fmd.rho_wall , axis=(0,1)) ; data['rho_wall_avg'] = rho_wall_avg
-        d99_avg      = np.mean(fmd.d99      , axis=(0,1)) ; data['d99_avg']      = d99_avg
-        u99_avg      = np.mean(fmd.u99      , axis=(0,1)) ; data['u99_avg']      = u99_avg
-        Re_tau_avg   = np.mean(fmd.Re_tau   , axis=(0,1)) ; data['Re_tau_avg']   = Re_tau_avg
-        Re_theta_avg = np.mean(fmd.Re_theta , axis=(0,1)) ; data['Re_theta_avg'] = Re_theta_avg
-        
-        ## mean [x,z] --> leave 1D [y]
-        rho_avg = np.mean(fmd.rho,axis=(0,2))
-        data['rho_avg'] = rho_avg
+        if ('data_dim' not in self):
+            raise ValueError('group data_dim not present')
         
-        # === 2D inner scales --> [x,z]
-        sc_l_in = nu_wall / u_tau
-        sc_u_in = u_tau
-        sc_t_in = nu_wall / u_tau**2
+        ## put all data from 'data_dim' into the dictionary data which will be pickled at the end
+        for dsn in self['data_dim'].keys():
+            d_ = np.copy( self[f'data_dim/{dsn}'][()] )
+            if (d_.ndim == 0):
+                d_ = float(d_)
+            data[dsn] = d_
         
-        # === 2D outer scales --> [x,z]
-        sc_l_out = d99
-        sc_u_out = u99
-        sc_t_out = d99/u99
+        ## 1D
+        rho_avg = np.copy( self['data_dim/rho'][()] )
+        u_avg   = np.copy( self['data_dim/u'][()]   )
+        
+        ## 0D
+        u_tau    = float( self['data_dim/u_tau'][()]    )
+        nu_wall  = float( self['data_dim/nu_wall'][()]  )
+        rho_wall = float( self['data_dim/rho_wall'][()] )
+        d99      = float( self['data_dim/d99'][()]      )
+        u_99     = float( self['data_dim/u_99'][()]     )
+        Re_tau   = float( self['data_dim/Re_tau'][()]   )
+        Re_theta = float( self['data_dim/Re_theta'][()] )
+        sc_u_in  = float( self['data_dim/sc_u_in'][()]  )
+        sc_l_in  = float( self['data_dim/sc_l_in'][()]  )
+        sc_t_in  = float( self['data_dim/sc_t_in'][()]  )
+        sc_u_out = float( self['data_dim/sc_u_out'][()] )
+        sc_l_out = float( self['data_dim/sc_l_out'][()] )
+        sc_t_out = float( self['data_dim/sc_t_out'][()] )
         
-        np.testing.assert_allclose( fmd.sc_l_in  , sc_l_in  , rtol=1e-14 )
-        np.testing.assert_allclose( fmd.sc_l_out , sc_l_out , rtol=1e-14 )
-        np.testing.assert_allclose( fmd.sc_u_in  , sc_u_in  , rtol=1e-14 )
-        np.testing.assert_allclose( fmd.sc_u_out , sc_u_out , rtol=1e-14 )
-        np.testing.assert_allclose( fmd.sc_t_in  , sc_t_in  , rtol=1e-14 )
-        np.testing.assert_allclose( fmd.sc_t_out , sc_t_out , rtol=1e-14 )
-        
-        ## mean [x,z] --> leave 0D scalar
-        sc_l_in_avg  = np.mean(sc_l_in  , axis=(0,1))
-        sc_l_out_avg = np.mean(sc_l_out , axis=(0,1))
-        sc_u_in_avg  = np.mean(sc_u_in  , axis=(0,1))
-        sc_u_out_avg = np.mean(sc_u_out , axis=(0,1))
-        sc_t_in_avg  = np.mean(sc_t_in  , axis=(0,1))
-        sc_t_out_avg = np.mean(sc_t_out , axis=(0,1))
-        
-        # === check
-        np.testing.assert_allclose(fmd.lchar   , self.lchar   , rtol=1e-8)
-        np.testing.assert_allclose(fmd.U_inf   , self.U_inf   , rtol=1e-8)
-        np.testing.assert_allclose(fmd.rho_inf , self.rho_inf , rtol=1e-8)
-        np.testing.assert_allclose(fmd.T_inf   , self.T_inf   , rtol=1e-8)
-        np.testing.assert_allclose(fmd.nx      , self.nx      , rtol=1e-8)
-        np.testing.assert_allclose(fmd.ny      , self.ny      , rtol=1e-8)
-        np.testing.assert_allclose(fmd.nz      , self.nz      , rtol=1e-8)
-        np.testing.assert_allclose(fmd.xs      , self.x       , rtol=1e-8)
-        np.testing.assert_allclose(fmd.ys      , self.y       , rtol=1e-8)
-        np.testing.assert_allclose(fmd.zs      , self.z       , rtol=1e-8)
+        ## these are recalculated and checked in next step
+        z1d_ = np.copy( self['data_dim/z1d'][()] )
+        dz0_ = np.copy( self['data_dim/dz0'][()] )
+        dt_  = np.copy( self['data_dim/dt'][()]  )
         
+        # ===
+        
+        ## get size of infile
+        fsize = os.path.getsize(self.fname)/1024**3
+        if verbose: even_print(os.path.basename(self.fname),'%0.1f [GB]'%fsize)
+        if verbose: even_print('nx','%i'%self.nx)
+        if verbose: even_print('ny','%i'%self.ny)
+        if verbose: even_print('nz','%i'%self.nz)
+        if verbose: even_print('nt','%i'%self.nt)
+        if verbose: even_print('ngp','%0.1f [M]'%(self.ngp/1e6,))
+        if verbose: print(72*'-')
+        
+        ## 0D scalars
         lchar   = self.lchar   ; data['lchar']   = lchar
         U_inf   = self.U_inf   ; data['U_inf']   = U_inf
         rho_inf = self.rho_inf ; data['rho_inf'] = rho_inf
         T_inf   = self.T_inf   ; data['T_inf']   = T_inf
         
         data['Ma'] = self.Ma
         data['Pr'] = self.Pr
         
+        ## read in 1D coordinate arrays, then re-dimensionalize [m]
+        x = np.copy( self['dims/x'][()] * self.lchar )
+        y = np.copy( self['dims/y'][()] * self.lchar )
+        z = np.copy( self['dims/z'][()] * self.lchar )
+        
         nx = self.nx ; data['nx'] = nx
         ny = self.ny ; data['ny'] = ny
         nz = self.nz ; data['nz'] = nz
         nt = self.nt ; data['nt'] = nt
         
-        ## dimless (inlet)
-        xd = self.x
-        yd = self.y
-        zd = self.z
-        td = self.t
+        # ## dimless (inlet/characteristic)
+        # xd = self.x
+        # yd = self.y
+        # zd = self.z
+        # td = self.t
         
         ## dimensional [m] / [s]
         x      = self.x * lchar 
         y      = self.y * lchar
         z      = self.z * lchar
         t      = self.t * (lchar/U_inf)
         t_meas = t[-1]-t[0]
         dt     = self.dt * (lchar/U_inf)
         
+        z1d = np.copy(z)
+        
         ## check if constant Δz (calculate Δz+ later)
-        dz0_ = np.diff(z)[0]
-        if np.all(np.isclose(np.diff(z), dz0_, rtol=1e-7)):
-            dz0 = dz0_
-        else:
-            raise ValueError
+        dz0 = np.diff(z1d)[0]
+        if not np.all(np.isclose(np.diff(z1d), dz0, rtol=1e-7)):
+            raise NotImplementedError
+        
+        ## dimensional [s]
+        dt = self.dt * self.tchar
+        np.testing.assert_allclose(dt, t[1]-t[0], rtol=1e-14, atol=1e-14)
+        
+        t_meas = self.duration * self.tchar
+        np.testing.assert_allclose(t_meas, t.max()-t.min(), rtol=1e-14, atol=1e-14)
+        
+        ## check against values in 'data_dim' (imported above)
+        np.testing.assert_allclose(dt  , dt_  , rtol=1e-14, atol=1e-14)
+        np.testing.assert_allclose(dz0 , dz0_ , rtol=1e-14, atol=1e-14)
+        np.testing.assert_allclose(z1d , z1d_ , rtol=1e-14, atol=1e-14)
         
         zrange = z[-1]-z[0]
         
         data['x'] = x
         data['y'] = y
         data['z'] = z
+        #data['z1d'] = z1d
+        
         data['t'] = t
         data['t_meas'] = t_meas
         data['dt'] = dt
         data['dz0'] = dz0
         data['zrange'] = zrange
         
-        np.testing.assert_equal(nx,x.size)
-        np.testing.assert_equal(ny,y.size)
-        np.testing.assert_equal(nz,z.size)
-        np.testing.assert_equal(nt,t.size)
-        np.testing.assert_allclose(dt, t[1]-t[0], rtol=1e-8)
+        if verbose: even_print('Δt/tchar','%0.8f'%(dt/self.tchar))
+        if verbose: even_print('Δt','%0.3e [s]'%(dt,))
+        if verbose: even_print('duration/tchar','%0.1f'%(self.duration,))
+        if verbose: even_print('duration','%0.3e [s]'%(self.duration*self.tchar,))
+        if verbose: print(72*'-')
         
-        # === report
+        ## report
         if verbose:
-            even_print('nx'     , '%i'        %nx     )
-            even_print('ny'     , '%i'        %ny     )
-            even_print('nz'     , '%i'        %nz     )
-            even_print('nt'     , '%i'        %nt     )
-            even_print('dt'     , '%0.5e [s]' %dt     )
-            even_print('t_meas' , '%0.5e [s]' %t_meas )
-            even_print('dz0'    , '%0.5e [m]' %dz0     )
-            even_print('zrange' , '%0.5e [m]' %zrange  )
+            even_print('dt'     , '%0.5e [s]' % dt      )
+            even_print('t_meas' , '%0.5e [s]' % t_meas  )
+            even_print('dz0'    , '%0.5e [m]' % dz0     )
+            even_print('zrange' , '%0.5e [m]' % zrange  )
             print(72*'-')
         
+        ## report
         if verbose:
-            even_print('Re_τ'   , '%0.1f'         % Re_tau_avg    )
-            even_print('Re_θ'   , '%0.1f'         % Re_theta_avg  )
-            even_print('δ99'    , '%0.5e [m]'     % d99_avg       )
-            even_print('δ_ν=(ν_wall/u_τ)' , '%0.5e [m]' % sc_l_in_avg )
-            even_print('U_inf'  , '%0.3f [m/s]'   % U_inf         )
-            even_print('u_τ'    , '%0.3f [m/s]'   % u_tau_avg     )
-            even_print('ν_wall' , '%0.5e [m²/s]'  % nu_wall_avg   )
-            even_print('ρ_wall' , '%0.6f [kg/m³]' % rho_wall_avg  )
+            even_print('Re_τ'    , '%0.1f'        % Re_tau    )
+            even_print('Re_θ'    , '%0.1f'        % Re_theta  )
+            even_print('δ99'     , '%0.5e [m]'    % d99       )
+            even_print('δ_ν=(ν_wall/u_τ)' , '%0.5e [m]' % sc_l_in )
+            even_print('U_inf'  , '%0.3f [m/s]'   % self.U_inf )
+            even_print('u_τ'    , '%0.3f [m/s]'   % u_tau     )
+            even_print('ν_wall' , '%0.5e [m²/s]'  % nu_wall   )
+            even_print('ρ_wall' , '%0.6f [kg/m³]' % rho_wall  )
             ##
-            even_print( 'Δz+'        , '%0.3f'%(dz0/sc_l_in_avg) )
-            even_print( 'zrange/δ99' , '%0.3f'%(zrange/d99_avg)  )
-            even_print( 'Δt+'        , '%0.3f'%(dt/sc_t_in_avg)  )
+            even_print( 'Δz+'        , '%0.3f'%(dz0/sc_l_in) )
+            even_print( 'zrange/δ99' , '%0.3f'%(zrange/d99)  )
+            even_print( 'Δt+'        , '%0.3f'%(dt/sc_t_in)  )
             print(72*'-')
         
-        t_eddy = t_meas / (d99_avg/u_tau_avg)
+        t_eddy = t_meas / ( d99 / u_tau )
         
         if verbose:
             even_print('t_meas/(δ99/u_τ) = t_eddy' , '%0.2f'%t_eddy)
-            even_print('t_meas/(δ99/u99)'          , '%0.2f'%(t_meas/(d99_avg/u99_avg)))
-            even_print('t_meas/(20·δ99/u99)'       , '%0.2f'%(t_meas/(20*d99_avg/u99_avg)))
+            even_print('t_meas/(δ99/u99)'          , '%0.2f'%(t_meas/(d99/u_99)))
+            even_print('t_meas/(20·δ99/u99)'       , '%0.2f'%(t_meas/(20*d99/u_99)))
         
-        ## get lags & n lags
+        ## get lags
         lags,_  = ccor( np.ones(nt,dtype=np.float32) , np.ones(nt,dtype=np.float32), get_lags=True )
         n_lags_ = nt*2-1
         n_lags  = lags.shape[0]
         if (n_lags!=n_lags_):
             raise AssertionError('possible problem with lags calc --> check!')
         
+        data['lags'] = lags
+        data['n_lags'] = n_lags
+        
         if verbose:
             even_print('n lags (Δt)' , '%i'%(n_lags,))
         
         ## [var1, var2, density_scaling]
         R_combis = [
                    [ 'uI'  , 'uI'  , False ],
                    [ 'vI'  , 'vI'  , False ],
                    [ 'wI'  , 'wI'  , False ],
                    [ 'uI'  , 'vI'  , False ],
                    [ 'uI'  , 'TI'  , False ],
+                   [ 'vI'  , 'TI'  , False ],
                    [ 'TI'  , 'TI'  , False ],
                    [ 'uII' , 'uII' , True  ],
                    [ 'vII' , 'vII' , True  ],
                    [ 'wII' , 'wII' , True  ],
                    [ 'uII' , 'vII' , True  ],
                    [ 'uII' , 'TII' , True  ],
+                   [ 'vII' , 'TII' , True  ],
                    [ 'TII' , 'TII' , True  ],
                    ]
         
         if verbose:
             even_print('n ccor (Δt) scalar combinations' , '%i'%(len(R_combis),))
             print(72*'-')
         
@@ -12897,28 +13630,34 @@
         read_density = False
         for cc in R_combis:
             scalar_L, scalar_R, density_scaling = cc
             if density_scaling:
                 read_density = True
                 break
         
-        ## read density
+        if verbose:
+            even_print('read ρ', str(read_density))
+        
+        ## confirm 'rho' is not in locals
         if read_density and ('rho' in locals()):
             raise ValueError('rho alread in locals... check')
         
         if read_density:
             
             ## buffer for rho (NOT rhoI) --> this is read from 'prime' file
             rho = np.zeros(shape=(nx, nyr, nz, nt), dtype=np.float32)
             
             dset = self['data/rho']
             self.comm.Barrier()
             t_start = timeit.default_timer()
-            with dset.collective:
-                rho[:,:,:,:] = dset[:,:,ry1:ry2,:].T
+            if self.usingmpi:
+                with dset.collective:
+                    rho[:,:,:,:] = dset[:,:,ry1:ry2,:].T
+            else:
+                rho[:,:,:,:] = dset[()].T
             self.comm.Barrier()
             t_delta = timeit.default_timer() - t_start
             data_gb = 4 * self.nx * self.ny * self.nz * self.nt / 1024**3
             if verbose:
                 even_print( 'read: rho','%0.3f [GB]  %0.3f [s]  %0.3f [GB/s]'%(data_gb,t_delta,(data_gb/t_delta)))
             
             ## re-dimensionalize rho
@@ -13002,17 +13741,21 @@
                     fancy_tag = '<%s,%s>'%(scalar_L,scalar_R)
                 tqdm.write(even_print('running Δt cross-correlation calc', fancy_tag, s=True))
             
             for xi in range(nx):
                 for yi in range(nyr):
                     for zi in range(nz):
                         
-                        uL    = np.copy( data_prime[scalar_L][xi,yi,zi,:]   )
-                        uR    = np.copy( data_prime[scalar_R][xi,yi,zi,:]   )
-                        rho1d = np.copy( rho[xi,yi,zi,:] )
+                        uL = np.copy( data_prime[scalar_L][xi,yi,zi,:]   )
+                        uR = np.copy( data_prime[scalar_R][xi,yi,zi,:]   )
+                        
+                        if density_scaling:
+                            rho1d = np.copy( rho[xi,yi,zi,:] )
+                        else:
+                            rho1d = None
                         
                         if density_scaling:
                             data_R[xi,yi,zi,:] = ccor( rho1d*uL , rho1d*uR )
                         else:
                             data_R[xi,yi,zi,:] = ccor( uL , uR )
                         
                         if verbose: progress_bar.update()
@@ -13071,28 +13814,14 @@
         # === save results
         
         if (self.rank==0):
             
             data['R']    = R ## the main cross-correlation data array
             data['lags'] = lags
             
-            sc_l_in  = np.mean(sc_l_in  , axis=(0,1) , dtype=np.float64) #.astype(np.float32) ## avg in [x,z] --> leave 0D scalar
-            sc_u_in  = np.mean(sc_u_in  , axis=(0,1) , dtype=np.float64) #.astype(np.float32)
-            sc_t_in  = np.mean(sc_t_in  , axis=(0,1) , dtype=np.float64) #.astype(np.float32)
-            sc_l_out = np.mean(sc_l_out , axis=(0,1) , dtype=np.float64) #.astype(np.float32)
-            sc_u_out = np.mean(sc_u_out , axis=(0,1) , dtype=np.float64) #.astype(np.float32)
-            sc_t_out = np.mean(sc_t_out , axis=(0,1) , dtype=np.float64) #.astype(np.float32)
-            
-            data['sc_l_in']  = sc_l_in
-            data['sc_u_in']  = sc_u_in
-            data['sc_t_in']  = sc_t_in
-            data['sc_l_out'] = sc_l_out
-            data['sc_u_out'] = sc_u_out
-            data['sc_t_out'] = sc_t_out
-            
             with open(fn_dat_ccor_time,'wb') as f:
                 pickle.dump(data, f, protocol=4)
             print('--w-> %s : %0.2f [MB]'%(fn_dat_ccor_time,os.path.getsize(fn_dat_ccor_time)/1024**2))
         
         # ===
         
         self.comm.Barrier()
@@ -13119,15 +13848,15 @@
         
         rx = kwargs.get('rx',1)
         ry = kwargs.get('ry',1)
         rz = kwargs.get('rz',1)
         rt = kwargs.get('rt',1)
         
         fn_dat_ccor_span = kwargs.get('fn_dat_ccor_span',None)
-        fn_dat_mean_dim  = kwargs.get('fn_dat_mean_dim',None)
+        #fn_dat_mean_dim  = kwargs.get('fn_dat_mean_dim',None)
         
         ## for now only distribute data in [y]
         if (rx!=1):
             raise AssertionError('rx!=1')
         if (rz!=1):
             raise AssertionError('rz!=1')
         if (rt!=1):
@@ -13162,195 +13891,203 @@
         #rx1, rx2 = rxl[t4d[0]]; nxr = rx2 - rx1
         #ry1, ry2 = ryl[t4d[1]]; nyr = ry2 - ry1
         #rz1, rz2 = rzl[t4d[2]]; nzr = rz2 - rz1
         #rt1, rt2 = rtl[t4d[3]]; ntr = rt2 - rt1
         
         ry1,ry2 = ryl[self.rank]; nyr = ry2 - ry1
         
-        # === mean dimensional file name (for reading) : .dat
-        if (fn_dat_mean_dim is None):
-            fname_path = os.path.dirname(self.fname)
-            fname_base = os.path.basename(self.fname)
-            fname_root, fname_ext = os.path.splitext(fname_base)
-            fname_root = re.findall('io\S+_mpi_[0-9]+', fname_root)[0]
-            fname_dat_mean_base = fname_root+'_mean_dim.dat'
-            fn_dat_mean_dim = str(PurePosixPath(fname_path, fname_dat_mean_base))
+        # # === mean dimensional file name (for reading) : .dat
+        # if (fn_dat_mean_dim is None):
+        #     fname_path = os.path.dirname(self.fname)
+        #     fname_base = os.path.basename(self.fname)
+        #     fname_root, fname_ext = os.path.splitext(fname_base)
+        #     fname_root = re.findall('io\S+_mpi_[0-9]+', fname_root)[0]
+        #     fname_dat_mean_base = fname_root+'_mean_dim.dat'
+        #     fn_dat_mean_dim = str(PurePosixPath(fname_path, fname_dat_mean_base))
         
         # === cross-correlation file name (for writing) : dat
         if (fn_dat_ccor_span is None):
             fname_path = os.path.dirname(self.fname)
             fname_base = os.path.basename(self.fname)
             fname_root, fname_ext = os.path.splitext(fname_base)
             fname_root = re.findall('io\S+_mpi_[0-9]+', fname_root)[0]
             fname_ccor_span_dat_base = fname_root+'_ccor_span.dat'
             fn_dat_ccor_span = str(PurePosixPath(fname_path, fname_ccor_span_dat_base))
         
         if verbose: even_print('fn_rgd_prime'     , self.fname       )
-        if verbose: even_print('fn_dat_mean_dim'  , fn_dat_mean_dim  )
+        #if verbose: even_print('fn_dat_mean_dim'  , fn_dat_mean_dim  )
         if verbose: even_print('fn_dat_ccor_span' , fn_dat_ccor_span )
         if verbose: print(72*'-')
         
-        if not os.path.isfile(fn_dat_mean_dim):
-            raise FileNotFoundError('%s not found!'%fn_dat_mean_dim)
+        # if not os.path.isfile(fn_dat_mean_dim):
+        #     raise FileNotFoundError('%s not found!'%fn_dat_mean_dim)
         
-        # === read in data (mean dim) --> every rank gets full [x,z]
-        with open(fn_dat_mean_dim,'rb') as f:
-            data_mean_dim = pickle.load(f)
-        fmd = type('foo', (object,), data_mean_dim)
+        # # === read in data (mean dim) --> every rank gets full [x,z]
+        # with open(fn_dat_mean_dim,'rb') as f:
+        #     data_mean_dim = pickle.load(f)
+        # fmd = type('foo', (object,), data_mean_dim)
         
         self.comm.Barrier()
         
         ## the data dictionary to be pickled later
         data = {}
         
-        ## 2D dimensional quantities --> [x,z]
-        u_tau    = fmd.u_tau    # ; data['u_tau']    = u_tau
-        nu_wall  = fmd.nu_wall  # ; data['nu_wall']  = nu_wall
-        rho_wall = fmd.rho_wall # ; data['rho_wall'] = rho_wall
-        d99      = fmd.d99      # ; data['d99']      = d99
-        u99      = fmd.u99      # ; data['u99']      = u99
-        Re_tau   = fmd.Re_tau   # ; data['Re_tau']   = Re_tau
-        Re_theta = fmd.Re_theta # ; data['Re_theta'] = Re_theta
-        
-        ## mean [x,z] --> leave 0D scalar
-        u_tau_avg    = np.mean(fmd.u_tau    , axis=(0,1)) ; data['u_tau_avg']    = u_tau_avg
-        nu_wall_avg  = np.mean(fmd.nu_wall  , axis=(0,1)) ; data['nu_wall_avg']  = nu_wall_avg
-        rho_wall_avg = np.mean(fmd.rho_wall , axis=(0,1)) ; data['rho_wall_avg'] = rho_wall_avg
-        d99_avg      = np.mean(fmd.d99      , axis=(0,1)) ; data['d99_avg']      = d99_avg
-        u99_avg      = np.mean(fmd.u99      , axis=(0,1)) ; data['u99_avg']      = u99_avg
-        Re_tau_avg   = np.mean(fmd.Re_tau   , axis=(0,1)) ; data['Re_tau_avg']   = Re_tau_avg
-        Re_theta_avg = np.mean(fmd.Re_theta , axis=(0,1)) ; data['Re_theta_avg'] = Re_theta_avg
-        
-        ## mean [x,z] --> leave 1D [y]
-        rho_avg = np.mean(fmd.rho,axis=(0,2))
-        data['rho_avg'] = rho_avg
+        if ('data_dim' not in self):
+            raise ValueError('group data_dim not present')
         
-        # === 2D inner scales --> [x,z]
-        sc_l_in = nu_wall / u_tau
-        sc_u_in = u_tau
-        sc_t_in = nu_wall / u_tau**2
+        ## put all data from 'data_dim' into the dictionary data which will be pickled at the end
+        for dsn in self['data_dim'].keys():
+            d_ = np.copy( self[f'data_dim/{dsn}'][()] )
+            if (d_.ndim == 0):
+                d_ = float(d_)
+            data[dsn] = d_
         
-        # === 2D outer scales --> [x,z]
-        sc_l_out = d99
-        sc_u_out = u99
-        sc_t_out = d99/u99
+        ## 1D
+        rho_avg = np.copy( self['data_dim/rho'][()] )
+        u_avg   = np.copy( self['data_dim/u'][()]   )
         
-        np.testing.assert_allclose( fmd.sc_l_in  , sc_l_in  , rtol=1e-14 )
-        np.testing.assert_allclose( fmd.sc_l_out , sc_l_out , rtol=1e-14 )
-        np.testing.assert_allclose( fmd.sc_u_in  , sc_u_in  , rtol=1e-14 )
-        np.testing.assert_allclose( fmd.sc_u_out , sc_u_out , rtol=1e-14 )
-        np.testing.assert_allclose( fmd.sc_t_in  , sc_t_in  , rtol=1e-14 )
-        np.testing.assert_allclose( fmd.sc_t_out , sc_t_out , rtol=1e-14 )
-        
-        ## mean [x,z] --> leave 0D scalar
-        sc_l_in_avg  = np.mean(sc_l_in  , axis=(0,1))
-        sc_l_out_avg = np.mean(sc_l_out , axis=(0,1))
-        sc_u_in_avg  = np.mean(sc_u_in  , axis=(0,1))
-        sc_u_out_avg = np.mean(sc_u_out , axis=(0,1))
-        sc_t_in_avg  = np.mean(sc_t_in  , axis=(0,1))
-        sc_t_out_avg = np.mean(sc_t_out , axis=(0,1))
-        
-        # === check
-        np.testing.assert_allclose(fmd.lchar   , self.lchar   , rtol=1e-8)
-        np.testing.assert_allclose(fmd.U_inf   , self.U_inf   , rtol=1e-8)
-        np.testing.assert_allclose(fmd.rho_inf , self.rho_inf , rtol=1e-8)
-        np.testing.assert_allclose(fmd.T_inf   , self.T_inf   , rtol=1e-8)
-        np.testing.assert_allclose(fmd.nx      , self.nx      , rtol=1e-8)
-        np.testing.assert_allclose(fmd.ny      , self.ny      , rtol=1e-8)
-        np.testing.assert_allclose(fmd.nz      , self.nz      , rtol=1e-8)
-        np.testing.assert_allclose(fmd.xs      , self.x       , rtol=1e-8)
-        np.testing.assert_allclose(fmd.ys      , self.y       , rtol=1e-8)
-        np.testing.assert_allclose(fmd.zs      , self.z       , rtol=1e-8)
+        ## 0D
+        u_tau    = float( self['data_dim/u_tau'][()]    )
+        nu_wall  = float( self['data_dim/nu_wall'][()]  )
+        rho_wall = float( self['data_dim/rho_wall'][()] )
+        d99      = float( self['data_dim/d99'][()]      )
+        u_99     = float( self['data_dim/u_99'][()]     )
+        Re_tau   = float( self['data_dim/Re_tau'][()]   )
+        Re_theta = float( self['data_dim/Re_theta'][()] )
+        sc_u_in  = float( self['data_dim/sc_u_in'][()]  )
+        sc_l_in  = float( self['data_dim/sc_l_in'][()]  )
+        sc_t_in  = float( self['data_dim/sc_t_in'][()]  )
+        sc_u_out = float( self['data_dim/sc_u_out'][()] )
+        sc_l_out = float( self['data_dim/sc_l_out'][()] )
+        sc_t_out = float( self['data_dim/sc_t_out'][()] )
         
+        ## these are recalculated and checked in next step
+        z1d_ = np.copy( self['data_dim/z1d'][()] )
+        dz0_ = np.copy( self['data_dim/dz0'][()] )
+        dt_  = np.copy( self['data_dim/dt'][()]  )
+        
+        # ===
+        
+        ## get size of infile
+        fsize = os.path.getsize(self.fname)/1024**3
+        if verbose: even_print(os.path.basename(self.fname),'%0.1f [GB]'%fsize)
+        if verbose: even_print('nx','%i'%self.nx)
+        if verbose: even_print('ny','%i'%self.ny)
+        if verbose: even_print('nz','%i'%self.nz)
+        if verbose: even_print('nt','%i'%self.nt)
+        if verbose: even_print('ngp','%0.1f [M]'%(self.ngp/1e6,))
+        if verbose: print(72*'-')
+        
+        ## 0D scalars
         lchar   = self.lchar   ; data['lchar']   = lchar
         U_inf   = self.U_inf   ; data['U_inf']   = U_inf
         rho_inf = self.rho_inf ; data['rho_inf'] = rho_inf
         T_inf   = self.T_inf   ; data['T_inf']   = T_inf
         
+        #data['M_inf'] = self.M_inf
         data['Ma'] = self.Ma
         data['Pr'] = self.Pr
         
+        ## read in 1D coordinate arrays, then re-dimensionalize [m]
+        x = np.copy( self['dims/x'][()] * self.lchar )
+        y = np.copy( self['dims/y'][()] * self.lchar )
+        z = np.copy( self['dims/z'][()] * self.lchar )
+        
         nx = self.nx ; data['nx'] = nx
         ny = self.ny ; data['ny'] = ny
         nz = self.nz ; data['nz'] = nz
         nt = self.nt ; data['nt'] = nt
         
-        ## dimless (inlet)
-        xd = self.x
-        yd = self.y
-        zd = self.z
-        td = self.t
+        t = np.copy( self['dims/t'][()] * self.tchar )
         
-        ## dimensional [m] / [s]
-        x      = self.x * lchar 
+        # ## dimless (inlet/characteristic)
+        # xd = self.x
+        # yd = self.y
+        # zd = self.z
+        # td = self.t
+        
+        ## redimensionalize coordinates --> [m],[s],[m/s],etc.
+        x      = self.x * lchar
         y      = self.y * lchar
         z      = self.z * lchar
         t      = self.t * (lchar/U_inf)
         t_meas = t[-1]-t[0]
         dt     = self.dt * (lchar/U_inf)
         
+        z1d = np.copy(z)
+        
         ## check if constant Δz (calculate Δz+ later)
-        dz0_ = np.diff(z)[0]
-        if np.all(np.isclose(np.diff(z), dz0_, rtol=1e-7)):
-            dz0 = dz0_
-        else:
-            raise ValueError
+        dz0 = np.diff(z1d)[0]
+        if not np.all(np.isclose(np.diff(z1d), dz0, rtol=1e-7)):
+            raise NotImplementedError
         
-        zrange = z[-1]-z[0]
+        ## dimensional [s]
+        dt = self.dt * self.tchar
+        np.testing.assert_allclose(dt, t[1]-t[0], rtol=1e-14, atol=1e-14)
+        
+        t_meas = self.duration * self.tchar
+        np.testing.assert_allclose(t_meas, t.max()-t.min(), rtol=1e-14, atol=1e-14)
+        
+        ## check against values in 'data_dim' (imported above)
+        np.testing.assert_allclose(dt  , dt_  , rtol=1e-14, atol=1e-14)
+        np.testing.assert_allclose(dz0 , dz0_ , rtol=1e-14, atol=1e-14)
+        np.testing.assert_allclose(z1d , z1d_ , rtol=1e-14, atol=1e-14)
+        
+        zrange = z1d.max() - z1d.min()
+        #zrange = z[-1]-z[0]
         
         data['x'] = x
         data['y'] = y
         data['z'] = z
+        #data['z1d'] = z1d
+        
         data['t'] = t
         data['t_meas'] = t_meas
         data['dt'] = dt
         data['dz0'] = dz0
         data['zrange'] = zrange
         
-        np.testing.assert_equal(nx,x.size)
-        np.testing.assert_equal(ny,y.size)
-        np.testing.assert_equal(nz,z.size)
-        np.testing.assert_equal(nt,t.size)
-        np.testing.assert_allclose(dt, t[1]-t[0], rtol=1e-8)
+        if verbose: even_print('Δt/tchar','%0.8f'%(dt/self.tchar))
+        if verbose: even_print('Δt','%0.3e [s]'%(dt,))
+        if verbose: even_print('duration/tchar','%0.1f'%(self.duration,))
+        if verbose: even_print('duration','%0.3e [s]'%(self.duration*self.tchar,))
+        if verbose: print(72*'-')
         
-        # === report
+        ## report
         if verbose:
-            even_print('nx'     , '%i'        %nx     )
-            even_print('ny'     , '%i'        %ny     )
-            even_print('nz'     , '%i'        %nz     )
-            even_print('nt'     , '%i'        %nt     )
-            even_print('dt'     , '%0.5e [s]' %dt     )
-            even_print('t_meas' , '%0.5e [s]' %t_meas )
-            even_print('dz0'    , '%0.5e [m]' %dz0     )
-            even_print('zrange' , '%0.5e [m]' %zrange  )
+            even_print('dt'     , '%0.5e [s]' % dt      )
+            even_print('t_meas' , '%0.5e [s]' % t_meas  )
+            even_print('dz0'    , '%0.5e [m]' % dz0     )
+            even_print('zrange' , '%0.5e [m]' % zrange  )
             print(72*'-')
         
+        ## report
         if verbose:
-            even_print('Re_τ'   , '%0.1f'         % Re_tau_avg    )
-            even_print('Re_θ'   , '%0.1f'         % Re_theta_avg  )
-            even_print('δ99'    , '%0.5e [m]'     % d99_avg       )
-            even_print('δ_ν=(ν_wall/u_τ)' , '%0.5e [m]' % sc_l_in_avg )
-            even_print('U_inf'  , '%0.3f [m/s]'   % U_inf         )
-            even_print('u_τ'    , '%0.3f [m/s]'   % u_tau_avg     )
-            even_print('ν_wall' , '%0.5e [m²/s]'  % nu_wall_avg   )
-            even_print('ρ_wall' , '%0.6f [kg/m³]' % rho_wall_avg  )
+            even_print('Re_τ'    , '%0.1f'        % Re_tau    )
+            even_print('Re_θ'    , '%0.1f'        % Re_theta  )
+            even_print('δ99'     , '%0.5e [m]'    % d99       )
+            even_print('δ_ν=(ν_wall/u_τ)' , '%0.5e [m]' % sc_l_in )
+            even_print('U_inf'  , '%0.3f [m/s]'   % self.U_inf )
+            even_print('u_τ'    , '%0.3f [m/s]'   % u_tau     )
+            even_print('ν_wall' , '%0.5e [m²/s]'  % nu_wall   )
+            even_print('ρ_wall' , '%0.6f [kg/m³]' % rho_wall  )
             ##
-            even_print( 'Δz+'        , '%0.3f'%(dz0/sc_l_in_avg) )
-            even_print( 'zrange/δ99' , '%0.3f'%(zrange/d99_avg)  )
-            even_print( 'Δt+'        , '%0.3f'%(dt/sc_t_in_avg)  )
+            even_print( 'Δz+'        , '%0.3f'%(dz0/sc_l_in) )
+            even_print( 'zrange/δ99' , '%0.3f'%(zrange/d99)  )
+            even_print( 'Δt+'        , '%0.3f'%(dt/sc_t_in)  )
             print(72*'-')
         
-        t_eddy = t_meas / (d99_avg/u_tau_avg)
+        t_eddy = t_meas / ( d99 / u_tau )
         
         if verbose:
             even_print('t_meas/(δ99/u_τ) = t_eddy' , '%0.2f'%t_eddy)
-            even_print('t_meas/(δ99/u99)'          , '%0.2f'%(t_meas/(d99_avg/u99_avg)))
-            even_print('t_meas/(20·δ99/u99)'       , '%0.2f'%(t_meas/(20*d99_avg/u99_avg)))
+            even_print('t_meas/(δ99/u99)'          , '%0.2f'%(t_meas/(d99/u_99)))
+            even_print('t_meas/(20·δ99/u99)'       , '%0.2f'%(t_meas/(20*d99/u_99)))
         
-        ## get lags & n lags
+        ## get lags
         lags,_  = ccor( np.ones(nz,dtype=np.float32) , np.ones(nz,dtype=np.float32), get_lags=True )
         n_lags_ = nz*2-1
         n_lags  = lags.shape[0]
         if (n_lags!=n_lags_):
             raise AssertionError('possible problem with lags calc --> check!')
         
         if verbose:
@@ -13359,20 +14096,22 @@
         ## [var1, var2, density_scaling]
         R_combis = [
                    [ 'uI'  , 'uI'  , False ],
                    [ 'vI'  , 'vI'  , False ],
                    [ 'wI'  , 'wI'  , False ],
                    [ 'uI'  , 'vI'  , False ],
                    [ 'uI'  , 'TI'  , False ],
+                   [ 'vI'  , 'TI'  , False ],
                    [ 'TI'  , 'TI'  , False ],
                    [ 'uII' , 'uII' , True  ],
                    [ 'vII' , 'vII' , True  ],
                    [ 'wII' , 'wII' , True  ],
                    [ 'uII' , 'vII' , True  ],
                    [ 'uII' , 'TII' , True  ],
+                   [ 'vII' , 'TII' , True  ],
                    [ 'TII' , 'TII' , True  ],
                    ]
         
         if verbose:
             even_print('n ccor (Δz) scalar combinations' , '%i'%(len(R_combis),))
             print(72*'-')
         
@@ -13380,15 +14119,18 @@
         read_density = False
         for cc in R_combis:
             scalar_L, scalar_R, density_scaling = cc
             if density_scaling:
                 read_density = True
                 break
         
-        ## read density
+        if verbose:
+            even_print('read ρ', str(read_density))
+        
+        ## confirm 'rho' is not in locals
         if read_density and ('rho' in locals()):
             raise ValueError('rho alread in locals... check')
         
         if read_density:
             
             ## buffer for rho (NOT rhoI) --> this is read from 'prime' file
             rho = np.zeros(shape=(nx, nyr, nz, nt), dtype=np.float32)
@@ -13485,17 +14227,21 @@
                     fancy_tag = '<%s,%s>'%(scalar_L,scalar_R)
                 tqdm.write(even_print('running Δz cross-correlation calc', fancy_tag, s=True))
             
             for xi in range(nx):
                 for yi in range(nyr):
                     for ti in range(nt):
                         
-                        uL    = np.copy( data_prime[scalar_L][xi,yi,:,ti]   )
-                        uR    = np.copy( data_prime[scalar_R][xi,yi,:,ti]   )
-                        rho1d = np.copy( rho[xi,yi,:,ti] )
+                        uL = np.copy( data_prime[scalar_L][xi,yi,:,ti]   )
+                        uR = np.copy( data_prime[scalar_R][xi,yi,:,ti]   )
+                        
+                        if density_scaling:
+                            rho1d = np.copy( rho[xi,yi,:,ti] )
+                        else:
+                            rho1d = None
                         
                         if density_scaling:
                             data_R[xi,yi,:,ti] = ccor( rho1d*uL , rho1d*uR )
                         else:
                             data_R[xi,yi,:,ti] = ccor( uL , uR )
                         
                         if verbose: progress_bar.update()
@@ -13554,28 +14300,14 @@
         # === save results
         
         if (self.rank==0):
             
             data['R']    = R ## the main cross-correlation data array
             data['lags'] = lags
             
-            sc_l_in  = np.mean(sc_l_in  , axis=(0,1) , dtype=np.float64) #.astype(np.float32) ## avg in [x,z] --> leave 0D scalar
-            sc_u_in  = np.mean(sc_u_in  , axis=(0,1) , dtype=np.float64) #.astype(np.float32)
-            sc_t_in  = np.mean(sc_t_in  , axis=(0,1) , dtype=np.float64) #.astype(np.float32)
-            sc_l_out = np.mean(sc_l_out , axis=(0,1) , dtype=np.float64) #.astype(np.float32)
-            sc_u_out = np.mean(sc_u_out , axis=(0,1) , dtype=np.float64) #.astype(np.float32)
-            sc_t_out = np.mean(sc_t_out , axis=(0,1) , dtype=np.float64) #.astype(np.float32)
-            
-            data['sc_l_in']  = sc_l_in
-            data['sc_u_in']  = sc_u_in
-            data['sc_t_in']  = sc_t_in
-            data['sc_l_out'] = sc_l_out
-            data['sc_u_out'] = sc_u_out
-            data['sc_t_out'] = sc_t_out
-            
             with open(fn_dat_ccor_span,'wb') as f:
                 pickle.dump(data, f, protocol=4)
             print('--w-> %s : %0.2f [MB]'%(fn_dat_ccor_span,os.path.getsize(fn_dat_ccor_span)/1024**2))
         
         # ===
         
         self.comm.Barrier()
@@ -13585,45 +14317,79 @@
         if verbose: print('total time : rgd.calc_ccor_span() : %s'%format_time_string((timeit.default_timer() - t_start_func)))
         if verbose: print(72*'-')
         
         return
     
     def calc_turb_budget(self, **kwargs):
         '''
-        calculate turbulent kinetic energy (k) budget
+        calculate budget of turbulent kinetic energy (k)
+        -----
+        - parallelized over time [t] dimension
+        - dimensional [SI]
+        - designed for analyzing unsteady, thin planes in [x]
+        - requires that get_prime() and get_mean() were run on unsteady RGD
+        - requires that get_prime() was run with favre=True
+        - currently does NOT work in serial mode (parallel only)
+        -----
+        SI units of terms are [kg/(m·s³)] or [kg m^-1 s^-3]
+        normalize from SI with
+        * nu_wall / u_tau**4 / rho_wall --> *[ kg^-1 m s^3]
+        or
+        / ( u_tau**4 * rho_wall / nu_wall ) --> /[kg m^-1 s^-3]
+        -----
+        Gaurini, S., Moser, R., Shariff, K., & Wray, A. (2000).
+        Direct numerical simulation of a supersonic turbulent boundary layer at Mach 2.5.
+        Journal of Fluid Mechanics, 414, 1-33.
+        doi:10.1017/S0022112000008466
         -----
-        --> dimensional [SI]
-        --> requires that get_prime() was run with option favre=True
+        Pirozzoli, S., Grasso, F., & Gatski, T. B. (2004).
+        Direct numerical simulation and analysis of a spatially evolving supersonic turbulent boundary layer at M= 2.25.
+        Physics of fluids, 16(3), 530-545.
+        doi:10.1063/1.1637604
         '''
         
         if (self.rank==0):
             verbose = True
         else:
             verbose = False
         
         if verbose: print('\n'+'rgd.calc_turb_budget()'+'\n'+72*'-')
         t_start_func = timeit.default_timer()
         
+        if (self.fsubtype!='unsteady'):
+            raise ValueError
+        
+        if ( not self.usingmpi ):
+            raise ValueError('rgd.calc_turb_budget() currently only works in MPI mode')
+        
         rx = kwargs.get('rx',1)
         ry = kwargs.get('ry',1)
         rz = kwargs.get('rz',1)
         rt = kwargs.get('rt',1)
         
-        force                   = kwargs.get('force',False)
-        chunk_kb                = kwargs.get('chunk_kb',4*1024) ## 4 [MB]
-        hiOrder                 = kwargs.get('hiOrder',False)
-        #fn_rgd                 = kwargs.get('fn_rgd',None) ## self
-        fn_rgd_mean             = kwargs.get('fn_rgd_mean',None)
-        fn_rgd_prime            = kwargs.get('fn_rgd_prime',None)
-        fn_rgd_turb_budget      = kwargs.get('fn_rgd_turb_budget',None)
-        fn_rgd_turb_budget_mean = kwargs.get('fn_rgd_turb_budget_mean',None)
-        ##
-        save_unsteady           = kwargs.get('save_unsteady',False)
+        ct = kwargs.get('ct',1)
         
-        ## for now only distribute data in [y]
+        force = kwargs.get('force',False)
+        
+        fn_rgd_mean        = kwargs.get('fn_rgd_mean',None)
+        fn_rgd_prime       = kwargs.get('fn_rgd_prime',None)
+        fn_rgd_turb_budget = kwargs.get('fn_rgd_turb_budget',None)
+        fn_rgd_turb_budget = kwargs.get('fn_rgd_turb_budget',None)
+        fn_dat_turb_budget = kwargs.get('fn_dat_turb_budget',None)
+        
+        #save_unsteady = kwargs.get('save_unsteady',False)
+        
+        acc          = kwargs.get('acc', 6)
+        edge_stencil = kwargs.get('edge_stencil', 'half')
+        
+        chunk_kb         = kwargs.get('chunk_kb',4*1024) ## h5 chunk size: default 4 [MB]
+        chunk_constraint = kwargs.get('chunk_constraint',None) ## the 'constraint' parameter for sizing h5 chunks
+        chunk_base       = kwargs.get('chunk_base',None)
+        
+        ## for now only distribute data in [t]
         if (rx!=1):
             raise AssertionError('rx!=1')
         if (ry!=1):
             raise AssertionError('ry!=1')
         if (rz!=1):
             raise AssertionError('rz!=1')
         
@@ -13643,27 +14409,59 @@
         #comm4d = self.comm.Create_cart(dims=[rx,ry,ry,rt], periods=[False,False,False,False], reorder=False)
         #t4d = comm4d.Get_coords(self.rank)
         
         #rxl_ = np.array_split(np.array(range(self.nx),dtype=np.int64),min(rx,self.nx))
         #ryl_ = np.array_split(np.array(range(self.ny),dtype=np.int64),min(ry,self.ny))
         #rzl_ = np.array_split(np.array(range(self.nz),dtype=np.int64),min(rz,self.nz))
         rtl_ = np.array_split(np.array(range(self.nt),dtype=np.int64),min(rt,self.nt))
-
+        
         #rxl = [[b[0],b[-1]+1] for b in rxl_ ]
         #ryl = [[b[0],b[-1]+1] for b in ryl_ ]
         #rzl = [[b[0],b[-1]+1] for b in rzl_ ]
         rtl = [[b[0],b[-1]+1] for b in rtl_ ]
         
         #rx1, rx2 = rxl[t4d[0]]; nxr = rx2 - rx1
         #ry1, ry2 = ryl[t4d[1]]; nyr = ry2 - ry1
         #rz1, rz2 = rzl[t4d[2]]; nzr = rz2 - rz1
         #rt1, rt2 = rtl[t4d[3]]; ntr = rt2 - rt1
         
         rt1,rt2 = rtl[self.rank]; ntr = rt2 - rt1
         
+        # === [t] sub chunk range --> ctl = list of ranges in rt1:rt2
+        ctl_ = np.array_split( np.arange(rt1,rt2) , min(ct,ntr) )
+        ctl = [[b[0],b[-1]+1] for b in ctl_ ]
+        
+        ## check that no sub ranges are <=1
+        for a_ in [ ctl_[1]-ctl_[0] for ctl_ in ctl ]:
+            if (a_ <= 1):
+                raise ValueError
+        
+        ## the average sub [t] chunk size on this rank
+        avg_chunk_nt = np.mean( [ ctl_[1]-ctl_[0] for ctl_ in ctl ] )
+        
+        if True: ## check that [t] sub-chunk ranges are correct
+            
+            mytimeindices = []
+            for ctl_ in ctl:
+                ct1, ct2 = ctl_
+                mytimeindices += [ ti_ for ti_ in self.ti[ct1:ct2] ]
+            
+            G = self.comm.gather([ self.rank , mytimeindices ], root=0)
+            G = self.comm.bcast(G, root=0)
+            
+            alltimeindices = []
+            for G_ in G:
+                alltimeindices += G_[1]
+            alltimeindices = np.array( sorted(alltimeindices), dtype=np.int64 )
+            
+            if not np.array_equal( alltimeindices , self.ti ):
+                raise AssertionError
+            if not np.array_equal( alltimeindices , np.arange(self.nt, dtype=np.int64) ):
+                raise AssertionError
+        
         # === mean file name (for reading)
         if (fn_rgd_mean is None):
             fname_path = os.path.dirname(self.fname)
             fname_base = os.path.basename(self.fname)
             fname_root, fname_ext = os.path.splitext(fname_base)
             fname_mean_h5_base = fname_root+'_mean.h5'
             #fn_rgd_mean = os.path.join(fname_path, fname_mean_h5_base)
@@ -13682,94 +14480,71 @@
             #fn_rgd_prime = os.path.join(fname_path, fname_prime_h5_base)
             fn_rgd_prime = str(PurePosixPath(fname_path, fname_prime_h5_base))
             #fn_rgd_prime = Path(fname_path, fname_prime_h5_base)
         
         if not os.path.isfile(fn_rgd_prime):
             raise FileNotFoundError('%s not found!'%fn_rgd_prime)
         
-        # === turb_budget file name (for writing)
+        # === turb_budget .h5 file name (for writing)
         if (fn_rgd_turb_budget is None):
             fname_path = os.path.dirname(self.fname)
             fname_base = os.path.basename(self.fname)
             fname_root, fname_ext = os.path.splitext(fname_base)
-            fname_turb_budget_h5_base = fname_root+'_turb_budget.h5'
-            #fn_rgd_turb_budget = os.path.join(fname_path, fname_turb_budget_h5_base)
-            fn_rgd_turb_budget = str(PurePosixPath(fname_path, fname_turb_budget_h5_base))
-            #fn_rgd_turb_budget = Path(fname_path, fname_turb_budget_h5_base)
+            fn_rgd_turb_budget_base = fname_root+'_turb_budget.h5'
+            fn_rgd_turb_budget = str(PurePosixPath(fname_path, fn_rgd_turb_budget_base))
         
         if os.path.isfile(fn_rgd_turb_budget) and (force is False):
-            raise FileNotFoundError('%s already present & force=False'%fn_rgd_turb_budget)
+            raise ValueError(f'{fn_rgd_turb_budget} already present & force=False')
         
-        # === turb_budget (mean) file name (for writing)
-        if (fn_rgd_turb_budget_mean is None):
+        # === turb_budget .dat file name (for writing)
+        if (fn_dat_turb_budget is None):
             fname_path = os.path.dirname(self.fname)
             fname_base = os.path.basename(self.fname)
             fname_root, fname_ext = os.path.splitext(fname_base)
-            fn_rgd_turb_budget_mean_base = fname_root+'_turb_budget_mean.h5'
-            fn_rgd_turb_budget_mean = str(PurePosixPath(fname_path, fn_rgd_turb_budget_mean_base))
-        
-        if os.path.isfile(fn_rgd_turb_budget_mean) and (force is False):
-            raise FileNotFoundError('%s already present & force=False'%fn_rgd_turb_budget_mean)
+            fn_dat_turb_budget_base = fname_root+'_turb_budget.dat'
+            fn_dat_turb_budget = str(PurePosixPath(fname_path, fn_dat_turb_budget_base))
         
-        if verbose: even_print('fn_rgd'       , self.fname   )
-        if verbose: even_print('fn_rgd_mean'  , fn_rgd_mean  )
-        if verbose: even_print('fn_rgd_prime' , fn_rgd_prime )
+        if verbose: even_print('fn_rgd'             , self.fname         )
+        if verbose: even_print('fn_rgd_mean'        , fn_rgd_mean        )
+        if verbose: even_print('fn_rgd_prime'       , fn_rgd_prime       )
         if verbose: even_print('fn_rgd_turb_budget' , fn_rgd_turb_budget )
-        if verbose: even_print('fn_rgd_turb_budget_mean' , fn_rgd_turb_budget_mean )
+        if verbose: even_print('fn_dat_turb_budget' , fn_dat_turb_budget )
         if verbose: print(72*'-')
         
         # ===
         
         if verbose: even_print('nx' , '%i'%self.nx)
         if verbose: even_print('ny' , '%i'%self.ny)
         if verbose: even_print('nz' , '%i'%self.nz)
         if verbose: even_print('nt' , '%i'%self.nt)
-        if verbose: even_print('save_unsteady', str(save_unsteady))
+        #if verbose: even_print('save_unsteady', str(save_unsteady))
+        if verbose: print(72*'-')
+        if verbose: even_print('rt' , '%i'%rt)
+        if verbose: even_print('ct' , '%i'%ct)
+        if verbose: even_print('ntr' , '%i'%ntr)
+        if verbose: even_print('avg [t] chunk nt' , '%0.2f'%avg_chunk_nt)
         if verbose: print(72*'-')
         
         # === init outfiles
         
-        ## unsteady turb budget
-        if save_unsteady:
+        ## initialize file: turbulent kinetic energy budget, averaged
+        with rgd(fn_rgd_turb_budget, 'w', force=force, driver='mpio', comm=self.comm) as f1:
             
-            with rgd(fn_rgd_turb_budget, 'w', force=force, driver='mpio', comm=self.comm, libver='latest') as f1:
-                f1.init_from_rgd(self.fname)
-                
-                shape = (f1.nt,f1.nz,f1.ny,f1.nx)
-                chunks = rgd.chunk_sizer(nxi=shape, constraint=(1,None,None,None), size_kb=chunk_kb, base=2)
-                
-                data_gb = 4*f1.nt*f1.nz*f1.ny*f1.nx / 1024**3
-                
-                for dss in ['unsteady_production','unsteady_dissipation','unsteady_transport','unsteady_diffusion','unsteady_p_dilatation','unsteady_p_diffusion']:
-                    
-                    if verbose:
-                        even_print('initializing data/%s'%(dss,),'%0.1f [GB]'%(data_gb,))
-                    
-                    dset = f1.create_dataset('data/%s'%dss, 
-                                             shape=shape, 
-                                             dtype=np.float32,
-                                             chunks=chunks)
-                    
-                    chunk_kb_ = np.prod(dset.chunks)*4 / 1024. ## actual
-                    if verbose:
-                        even_print('chunk shape (t,z,y,x)','%s'%str(dset.chunks))
-                        even_print('chunk size','%i [KB]'%int(round(chunk_kb_)))
-            
-            if verbose: print(72*'-')
-        
-        ## avg turb budget
-        with rgd(fn_rgd_turb_budget_mean, 'w', force=force, driver='mpio', comm=self.comm, libver='latest') as f1:
+            f1.init_from_rgd(self.fname, t_info=False)
             
-            f1.attrs['duration_avg'] = self.t[-1] - self.t[0] ## add attribute for duration of mean
+            ## set some top-level attributes
+            #f1.attrs['duration_avg'] = duration_avg ## duration of mean
+            f1.attrs['duration_avg'] = self.t[-1] - self.t[0]
             #f1_mean.attrs['duration_avg'] = self.duration
-            
-            f1.init_from_rgd(self.fname, t_info=False)
+            f1.attrs['dt'] = self.t[1] - self.t[0]
+            #f1.attrs['fclass'] = 'rgd'
+            f1.attrs['fsubtype'] = 'mean'
             
             shape = (1,f1.nz,f1.ny,f1.nx)
-            chunks = rgd.chunk_sizer(nxi=shape, constraint=(1,None,None,None), size_kb=chunk_kb, base=2)
+            chunks = h5_chunk_sizer(nxi=shape, constraint=chunk_constraint, size_kb=chunk_kb, base=chunk_base, itemsize=4)
             
             data_gb = 4*1*f1.nz*f1.ny*f1.nx / 1024**3
             
             for dss in ['production','dissipation','transport','diffusion','p_dilatation','p_diffusion']:
                 
                 if verbose:
                     even_print('initializing data/%s'%(dss,),'%0.1f [GB]'%(data_gb,))
@@ -13795,1007 +14570,798 @@
         if verbose: print(72*'-')
         
         self.comm.Barrier()
         
         # ===
         
         ## with rgd(fn_rgd, 'r', driver='mpio', comm=comm, verbose=False) as hf_rgd: #self
-        with rgd(fn_rgd_prime, 'r', driver='mpio', comm=self.comm, libver='latest') as hf_prime:
-            with rgd(fn_rgd_mean, 'r', driver='mpio', comm=self.comm, libver='latest') as hf_mean:
-                
-                lchar   = self.lchar
-                U_inf   = self.U_inf
-                rho_inf = self.rho_inf
-                T_inf   = self.T_inf
-                ## p_inf = self.p_inf  ## should not be used for redimensionalization of p
-                
-                x = lchar * self.x
-                y = lchar * self.y
-                z = lchar * self.z
-                
-                nx = self.nx
-                ny = self.ny
-                nz = self.nz
-                nt = self.nt
-                
-                u_re = U_inf * hf_mean['data/u'][0,:,:,:].T
-                v_re = U_inf * hf_mean['data/v'][0,:,:,:].T
-                w_re = U_inf * hf_mean['data/w'][0,:,:,:].T
-                u_fv = U_inf * hf_mean['data/u_fv'][0,:,:,:].T
-                v_fv = U_inf * hf_mean['data/v_fv'][0,:,:,:].T
-                w_fv = U_inf * hf_mean['data/w_fv'][0,:,:,:].T
-                
-                dudx_ij_fv = get_grad(u_fv, v_fv, w_fv, x, y, z, do_stack=False, hiOrder=hiOrder, verbose=False)
-                dudx_ij_re = get_grad(u_re, v_re, w_re, x, y, z, do_stack=False, hiOrder=hiOrder, verbose=False)
-                
-                dudx_fv = dudx_ij_fv['dadx'][:,:,:,np.newaxis] ; dudx_re = dudx_ij_re['dadx'][:,:,:,np.newaxis]
-                dudy_fv = dudx_ij_fv['dady'][:,:,:,np.newaxis] ; dudy_re = dudx_ij_re['dady'][:,:,:,np.newaxis]
-                dudz_fv = dudx_ij_fv['dadz'][:,:,:,np.newaxis] ; dudz_re = dudx_ij_re['dadz'][:,:,:,np.newaxis]
-                dvdx_fv = dudx_ij_fv['dbdx'][:,:,:,np.newaxis] ; dvdx_re = dudx_ij_re['dbdx'][:,:,:,np.newaxis]
-                dvdy_fv = dudx_ij_fv['dbdy'][:,:,:,np.newaxis] ; dvdy_re = dudx_ij_re['dbdy'][:,:,:,np.newaxis]
-                dvdz_fv = dudx_ij_fv['dbdz'][:,:,:,np.newaxis] ; dvdz_re = dudx_ij_re['dbdz'][:,:,:,np.newaxis]
-                dwdx_fv = dudx_ij_fv['dcdx'][:,:,:,np.newaxis] ; dwdx_re = dudx_ij_re['dcdx'][:,:,:,np.newaxis]
-                dwdy_fv = dudx_ij_fv['dcdy'][:,:,:,np.newaxis] ; dwdy_re = dudx_ij_re['dcdy'][:,:,:,np.newaxis]
-                dwdz_fv = dudx_ij_fv['dcdz'][:,:,:,np.newaxis] ; dwdz_re = dudx_ij_re['dcdz'][:,:,:,np.newaxis]
-                
-                # === do read
-                ss1 = ['u','v','w','p','T','rho']
-                ss2 = ['uI','vI','wI','uII','vII','wII','pI','TI','rhoI']
+        with rgd(fn_rgd_prime, 'r', driver='mpio', comm=self.comm) as hf_prime:
+            with rgd(fn_rgd_mean, 'r', driver='mpio', comm=self.comm) as hf_mean:
                 
-                formats = [np.float32 for s in ss1+ss2]
-                dd = np.zeros(shape=(nx,ny,nz,ntr), dtype={'names':ss1+ss2, 'formats':formats}, order='C')
+                np.testing.assert_allclose(hf_prime.t, self.t, atol=1e-14, rtol=1e-14)
                 
-                for ss in ss1:
-                    dset = self['data/%s'%ss]
-                    self.comm.Barrier()
-                    t_start = timeit.default_timer()
-                    with dset.collective:
-                        dd[ss] = dset[rt1:rt2,:,:,:].T
-                    self.comm.Barrier()
-                    t_delta = timeit.default_timer() - t_start
-                    data_gb = 4*nx*ny*nz*nt/1024**3
-                    if verbose:
-                        even_print('read: %s'%ss, '%0.3f [GB]  %0.3f [s]  %0.3f [GB/s]'%(data_gb,t_delta,(data_gb/t_delta)))
+                np.testing.assert_allclose(hf_prime.x, self.x, atol=1e-14, rtol=1e-14)
+                np.testing.assert_allclose(hf_prime.y, self.y, atol=1e-14, rtol=1e-14)
+                np.testing.assert_allclose(hf_prime.z, self.z, atol=1e-14, rtol=1e-14)
+                
+                np.testing.assert_allclose(hf_prime.x, hf_mean.x, atol=1e-14, rtol=1e-14)
+                np.testing.assert_allclose(hf_prime.y, hf_mean.y, atol=1e-14, rtol=1e-14)
+                np.testing.assert_allclose(hf_prime.z, hf_mean.z, atol=1e-14, rtol=1e-14)
+                
+                np.testing.assert_allclose( hf_prime.lchar   , hf_mean.lchar   , atol=1e-14, rtol=1e-14 )
+                np.testing.assert_allclose( hf_prime.lchar   , self.lchar      , atol=1e-14, rtol=1e-14 )
+                np.testing.assert_allclose( hf_prime.U_inf   , hf_mean.U_inf   , atol=1e-14, rtol=1e-14 )
+                np.testing.assert_allclose( hf_prime.U_inf   , self.U_inf      , atol=1e-14, rtol=1e-14 )
+                np.testing.assert_allclose( hf_prime.T_inf   , hf_mean.T_inf   , atol=1e-14, rtol=1e-14 )
+                np.testing.assert_allclose( hf_prime.T_inf   , self.T_inf      , atol=1e-14, rtol=1e-14 )
+                np.testing.assert_allclose( hf_prime.rho_inf , hf_mean.rho_inf , atol=1e-14, rtol=1e-14 )
+                np.testing.assert_allclose( hf_prime.rho_inf , self.rho_inf    , atol=1e-14, rtol=1e-14 )
                 
-                for ss in ss2:
-                    dset = hf_prime['data/%s'%ss]
-                    self.comm.Barrier()
-                    t_start = timeit.default_timer()
-                    with dset.collective:
-                        dd[ss] = dset[rt1:rt2,:,:,:].T
-                    self.comm.Barrier()
-                    t_delta = timeit.default_timer() - t_start
-                    data_gb = 4*nx*ny*nz*nt/1024**3
-                    if verbose:
-                        even_print('read: %s'%ss, '%0.3f [GB]  %0.3f [s]  %0.3f [GB/s]'%(data_gb,t_delta,(data_gb/t_delta)))
-                
-                if verbose: print(72*'-')
-                
-                data_gb = dd.nbytes / 1024**3
-                if verbose:
-                    tqdm.write(even_print('data_gb (rank)', '%0.1f [GB]'%data_gb, s=True))
-                
-                mem_avail_gb = psutil.virtual_memory().available/1024**3
-                mem_free_gb  = psutil.virtual_memory().free/1024**3
-                if verbose:
-                    tqdm.write(even_print('mem free', '%0.1f [GB]'%mem_free_gb, s=True))
-                
-                # === dimensionalize
+                # ===
                 
-                u    = dd['u']   * U_inf
-                v    = dd['v']   * U_inf
-                w    = dd['w']   * U_inf
-                uI   = dd['uI']  * U_inf
-                vI   = dd['vI']  * U_inf
-                wI   = dd['wI']  * U_inf
-                uII  = dd['uII'] * U_inf
-                vII  = dd['vII'] * U_inf
-                wII  = dd['wII'] * U_inf
-                
-                rho  = dd['rho']  * rho_inf
-                rhoI = dd['rhoI'] * rho_inf
-                p    = dd['p']    * (rho_inf * U_inf**2)
-                pI   = dd['pI']   * (rho_inf * U_inf**2)
-                T    = dd['T']    * T_inf
-                TI   = dd['TI']   * T_inf
+                if (hf_prime.fsubtype!='prime'):
+                    raise ValueError
+                if (hf_mean.fsubtype!='mean'):
+                    raise ValueError
                 
-                mu  = np.copy(14.58e-7*T**1.5/(T+110.4))
+                data = {} ## dict to be output to .dat file
                 
-                dd = None
-                del dd
+                if ('data_dim' not in hf_mean):
+                    raise ValueError('group data_dim not present')
                 
-                # === get gradients
+                ## put all data from 'data_dim' into the dictionary data which will be pickled at the end
+                for dsn in hf_mean['data_dim'].keys():
+                    d_ = np.copy( hf_mean[f'data_dim/{dsn}'][()] )
+                    if (d_.ndim == 0):
+                        d_ = float(d_)
+                    data[dsn] = d_
                 
-                t_start = timeit.default_timer()
+                ## 1D
+                #rho_avg = np.copy( hf_mean['data_dim/rho'][()] )
+                #u_avg   = np.copy( hf_mean['data_dim/u'][()]   )
+                #v_avg   = np.copy( hf_mean['data_dim/v'][()]   )
+                #w_avg   = np.copy( hf_mean['data_dim/w'][()]   )
+                #T_avg   = np.copy( hf_mean['data_dim/T'][()]   )
+                #p_avg   = np.copy( hf_mean['data_dim/p'][()]   )
+                
+                ## 0D
+                u_tau    = float( hf_mean['data_dim/u_tau'][()]    )
+                nu_wall  = float( hf_mean['data_dim/nu_wall'][()]  )
+                rho_wall = float( hf_mean['data_dim/rho_wall'][()] )
+                T_wall   = float( hf_mean['data_dim/T_wall'][()]   )
+                d99      = float( hf_mean['data_dim/d99'][()]      )
+                u_99     = float( hf_mean['data_dim/u_99'][()]     )
+                Re_tau   = float( hf_mean['data_dim/Re_tau'][()]   )
+                Re_theta = float( hf_mean['data_dim/Re_theta'][()] )
+                sc_u_in  = float( hf_mean['data_dim/sc_u_in'][()]  )
+                sc_l_in  = float( hf_mean['data_dim/sc_l_in'][()]  )
+                sc_t_in  = float( hf_mean['data_dim/sc_t_in'][()]  )
+                sc_u_out = float( hf_mean['data_dim/sc_u_out'][()] )
+                sc_l_out = float( hf_mean['data_dim/sc_l_out'][()] )
+                sc_t_out = float( hf_mean['data_dim/sc_t_out'][()] )
+                
+                ## 0D scalars
+                lchar   = self.lchar   ; data['lchar']   = lchar
+                U_inf   = self.U_inf   ; data['U_inf']   = U_inf
+                rho_inf = self.rho_inf ; data['rho_inf'] = rho_inf
+                T_inf   = self.T_inf   ; data['T_inf']   = T_inf
+                
+                #data['M_inf'] = self.M_inf
+                data['Ma'] = self.Ma
+                data['Pr'] = self.Pr
+                
+                ## read in 1D coordinate arrays, then re-dimensionalize [m]
+                x = np.copy( self['dims/x'][()] * self.lchar )
+                y = np.copy( self['dims/y'][()] * self.lchar )
+                z = np.copy( self['dims/z'][()] * self.lchar )
+                t = np.copy( self['dims/t'][()] * self.tchar )
+                
+                ## dimensional [s]
+                dt = self.dt * self.tchar
+                np.testing.assert_allclose(dt, t[1]-t[0], rtol=1e-14, atol=1e-14)
+                
+                t_meas = self.duration * self.tchar
+                np.testing.assert_allclose(t_meas, t.max()-t.min(), rtol=1e-14, atol=1e-14)
+                
+                t_eddy = t_meas / ( d99 / u_tau )
+                
+                ## check if constant Δz (calculate Δz+ later)
+                dz0 = np.diff(z)[0]
+                if not np.all(np.isclose(np.diff(z), dz0, rtol=1e-7)):
+                    raise NotImplementedError
+                np.testing.assert_allclose(dz0, z[1]-z[0], rtol=1e-14, atol=1e-14)
                 
-                dudx   = np.gradient(u,   x, edge_order=2, axis=0)
-                dudy   = np.gradient(u,   y, edge_order=2, axis=1)
-                dudz   = np.gradient(u,   z, edge_order=2, axis=2)
-                dvdx   = np.gradient(v,   x, edge_order=2, axis=0)
-                dvdy   = np.gradient(v,   y, edge_order=2, axis=1)
-                dvdz   = np.gradient(v,   z, edge_order=2, axis=2)
-                dwdx   = np.gradient(w,   x, edge_order=2, axis=0)
-                dwdy   = np.gradient(w,   y, edge_order=2, axis=1)
-                dwdz   = np.gradient(w,   z, edge_order=2, axis=2)
-                ##
-                duIdx  = np.gradient(uI,  x, edge_order=2, axis=0)
-                duIdy  = np.gradient(uI,  y, edge_order=2, axis=1)
-                duIdz  = np.gradient(uI,  z, edge_order=2, axis=2)
-                dvIdx  = np.gradient(vI,  x, edge_order=2, axis=0)
-                dvIdy  = np.gradient(vI,  y, edge_order=2, axis=1)
-                dvIdz  = np.gradient(vI,  z, edge_order=2, axis=2)
-                dwIdx  = np.gradient(wI,  x, edge_order=2, axis=0)
-                dwIdy  = np.gradient(wI,  y, edge_order=2, axis=1)
-                dwIdz  = np.gradient(wI,  z, edge_order=2, axis=2)
-                ##
-                duIIdx = np.gradient(uII, x, edge_order=2, axis=0)
-                duIIdy = np.gradient(uII, y, edge_order=2, axis=1)
-                duIIdz = np.gradient(uII, z, edge_order=2, axis=2)
-                dvIIdx = np.gradient(vII, x, edge_order=2, axis=0)
-                dvIIdy = np.gradient(vII, y, edge_order=2, axis=1)
-                dvIIdz = np.gradient(vII, z, edge_order=2, axis=2)
-                dwIIdx = np.gradient(wII, x, edge_order=2, axis=0)
-                dwIIdy = np.gradient(wII, y, edge_order=2, axis=1)
-                dwIIdz = np.gradient(wII, z, edge_order=2, axis=2)
+                zrange = z.max() - z.min()
+                np.testing.assert_allclose(zrange, z[-1]-z[0], rtol=1e-14, atol=1e-14)
                 
-                t_delta = timeit.default_timer() - t_start
+                nx = self.nx ; data['nx'] = nx
+                ny = self.ny ; data['ny'] = ny
+                nz = self.nz ; data['nz'] = nz
+                nt = self.nt ; data['nt'] = nt
+                
+                ## add data to dict that gets output
+                data['x'] = x
+                data['y'] = y
+                data['z'] = z
+                data['t'] = t
+                data['t_meas'] = t_meas
+                data['dt'] = dt
+                data['dz0'] = dz0
+                data['zrange'] = zrange
+                
+                if verbose: even_print('Δt/tchar','%0.8f'%(dt/self.tchar))
+                if verbose: even_print('Δt','%0.3e [s]'%(dt,))
+                if verbose: even_print('duration/tchar','%0.1f'%(self.duration,))
+                if verbose: even_print('duration','%0.3e [s]'%(self.duration*self.tchar,))
+                if verbose: print(72*'-')
                 
+                ## report
                 if verbose:
-                    tqdm.write(even_print('get gradients', format_time_string(t_delta), s=True))
+                    even_print('dt'     , '%0.5e [s]' % dt      )
+                    even_print('t_meas' , '%0.5e [s]' % t_meas  )
+                    even_print('dz0'    , '%0.5e [m]' % dz0     )
+                    even_print('zrange' , '%0.5e [m]' % zrange  )
+                    print(72*'-')
                 
-                self.comm.Barrier()
-                mem_avail_gb = psutil.virtual_memory().available/1024**3
-                mem_free_gb  = psutil.virtual_memory().free/1024**3
+                ## report
                 if verbose:
-                    tqdm.write(even_print('mem available', '%0.1f [GB]'%mem_avail_gb, s=True))
-                    tqdm.write(even_print('mem free',      '%0.1f [GB]'%mem_free_gb,  s=True))
-                
-                # === stack into tensors
+                    even_print('Re_τ'    , '%0.1f'        % Re_tau    )
+                    even_print('Re_θ'    , '%0.1f'        % Re_theta  )
+                    even_print('δ99'     , '%0.5e [m]'    % d99       )
+                    even_print('δ_ν=(ν_wall/u_τ)' , '%0.5e [m]' % sc_l_in )
+                    even_print('U_inf'  , '%0.3f [m/s]'   % self.U_inf )
+                    even_print('u_τ'    , '%0.3f [m/s]'   % u_tau     )
+                    even_print('ν_wall' , '%0.5e [m²/s]'  % nu_wall   )
+                    even_print('ρ_wall' , '%0.6f [kg/m³]' % rho_wall  )
+                    ##
+                    even_print( 'Δz+'        , '%0.3f'%(dz0/sc_l_in) )
+                    even_print( 'zrange/δ99' , '%0.3f'%(zrange/d99)  )
+                    even_print( 'Δt+'        , '%0.3f'%(dt/sc_t_in)  )
+                    print(72*'-')
                 
-                t_start = timeit.default_timer()
+                ## report
+                if verbose:
+                    even_print('t_meas/(δ99/u_τ) = t_eddy' , '%0.2f'%t_eddy)
+                    even_print('t_meas/(δ99/u99)'          , '%0.2f'%(t_meas/(d99/u_99)))
+                    even_print('t_meas/(20·δ99/u99)'       , '%0.2f'%(t_meas/(20*d99/u_99)))
+                    print(72*'-')
                 
-                uI_i  = np.copy(np.stack((uI,  vI,  wI ), axis=-1))
-                uII_i = np.copy(np.stack((uII, vII, wII), axis=-1))
+                # ===
                 
-                duIdx_ij = np.stack((np.stack((duIdx, duIdy, duIdz), axis=4),
-                                     np.stack((dvIdx, dvIdy, dvIdz), axis=4),
-                                     np.stack((dwIdx, dwIdy, dwIdz), axis=4)), axis=5)
-                
-                duIIdx_ij = np.stack((np.stack((duIIdx, duIIdy, duIIdz), axis=4),
-                                      np.stack((dvIIdx, dvIIdy, dvIIdz), axis=4),
-                                      np.stack((dwIIdx, dwIIdy, dwIIdz), axis=4)), axis=5)
+                ## copy AVG [u,v,w] into memory
+                u_re = np.copy( U_inf * hf_mean['data/u'][0,:,:,:].T    )
+                v_re = np.copy( U_inf * hf_mean['data/v'][0,:,:,:].T    )
+                w_re = np.copy( U_inf * hf_mean['data/w'][0,:,:,:].T    )
+                u_fv = np.copy( U_inf * hf_mean['data/u_fv'][0,:,:,:].T )
+                v_fv = np.copy( U_inf * hf_mean['data/v_fv'][0,:,:,:].T )
+                w_fv = np.copy( U_inf * hf_mean['data/w_fv'][0,:,:,:].T )
+                
+                ## get Reynolds avg strain tensor elements
+                dudx_re = gradient( u=u_re , x=x , axis=0 , acc=acc , edge_stencil=edge_stencil )[:,:,:,np.newaxis]
+                dudy_re = gradient( u=u_re , x=y , axis=1 , acc=acc , edge_stencil=edge_stencil )[:,:,:,np.newaxis]
+                dudz_re = gradient( u=u_re , x=z , axis=2 , acc=acc , edge_stencil=edge_stencil )[:,:,:,np.newaxis]
+                dvdx_re = gradient( u=v_re , x=x , axis=0 , acc=acc , edge_stencil=edge_stencil )[:,:,:,np.newaxis]
+                dvdy_re = gradient( u=v_re , x=y , axis=1 , acc=acc , edge_stencil=edge_stencil )[:,:,:,np.newaxis]
+                dvdz_re = gradient( u=v_re , x=z , axis=2 , acc=acc , edge_stencil=edge_stencil )[:,:,:,np.newaxis]
+                dwdx_re = gradient( u=w_re , x=x , axis=0 , acc=acc , edge_stencil=edge_stencil )[:,:,:,np.newaxis]
+                dwdy_re = gradient( u=w_re , x=y , axis=1 , acc=acc , edge_stencil=edge_stencil )[:,:,:,np.newaxis]
+                dwdz_re = gradient( u=w_re , x=z , axis=2 , acc=acc , edge_stencil=edge_stencil )[:,:,:,np.newaxis]
+                
+                ## get Favre avg strain tensor elements
+                dudx_fv = gradient( u=u_fv , x=x , axis=0 , acc=acc , edge_stencil=edge_stencil )[:,:,:,np.newaxis]
+                dudy_fv = gradient( u=u_fv , x=y , axis=1 , acc=acc , edge_stencil=edge_stencil )[:,:,:,np.newaxis]
+                dudz_fv = gradient( u=u_fv , x=z , axis=2 , acc=acc , edge_stencil=edge_stencil )[:,:,:,np.newaxis]
+                dvdx_fv = gradient( u=v_fv , x=x , axis=0 , acc=acc , edge_stencil=edge_stencil )[:,:,:,np.newaxis]
+                dvdy_fv = gradient( u=v_fv , x=y , axis=1 , acc=acc , edge_stencil=edge_stencil )[:,:,:,np.newaxis]
+                dvdz_fv = gradient( u=v_fv , x=z , axis=2 , acc=acc , edge_stencil=edge_stencil )[:,:,:,np.newaxis]
+                dwdx_fv = gradient( u=w_fv , x=x , axis=0 , acc=acc , edge_stencil=edge_stencil )[:,:,:,np.newaxis]
+                dwdy_fv = gradient( u=w_fv , x=y , axis=1 , acc=acc , edge_stencil=edge_stencil )[:,:,:,np.newaxis]
+                dwdz_fv = gradient( u=w_fv , x=z , axis=2 , acc=acc , edge_stencil=edge_stencil )[:,:,:,np.newaxis]
+                
+                ## accumulators for per-timestep sum, at end gets multiplied by (1/nt) to get average
+                unsteady_production_sum   = np.zeros((nx,ny,nz,1), dtype=np.float64, order='C')
+                unsteady_dissipation_sum  = np.zeros((nx,ny,nz,1), dtype=np.float64, order='C')
+                unsteady_transport_sum    = np.zeros((nx,ny,nz,1), dtype=np.float64, order='C')
+                unsteady_diffusion_sum    = np.zeros((nx,ny,nz,1), dtype=np.float64, order='C')
+                unsteady_p_diffusion_sum  = np.zeros((nx,ny,nz,1), dtype=np.float64, order='C')
+                unsteady_p_dilatation_sum = np.zeros((nx,ny,nz,1), dtype=np.float64, order='C')
                 
-                t_delta = timeit.default_timer() - t_start
-                if verbose:
-                    tqdm.write(even_print('tensor stacking',format_time_string(t_delta), s=True))
+                # === main loop (iterate through sub-ranges within rank-distributed [t] range)
                 
-                self.comm.Barrier()
-                mem_avail_gb = psutil.virtual_memory().available/1024**3
-                mem_free_gb  = psutil.virtual_memory().free/1024**3
+                ## main loop --> cross-correlation in [Δz] at every [x,y,t]
                 if verbose:
-                    tqdm.write(even_print('mem available', '%0.1f [GB]'%mem_avail_gb, s=True))
-                    tqdm.write(even_print('mem free',      '%0.1f [GB]'%mem_free_gb,  s=True))
+                    progress_bar = tqdm(total=ct, ncols=100, desc='turb budget', leave=False, file=sys.stdout)
                 
-                # === production
-                if True:
+                ct_counter=0
+                for ctl_ in ctl:
+                    ct_counter += 1
+                    ct1, ct2 = ctl_
+                    ntc = ct2 - ct1
                     
-                    if verbose: print(72*'-')
-                    t_start = timeit.default_timer()
+                    if (ct>1):
+                        if verbose:
+                            mesg = f'[t] sub chunk {ct_counter:d}/{ct:d}'
+                            tqdm.write( mesg )
+                            tqdm.write( '-'*len(mesg) )
+                    
+                    # === read unsteady data
+                    
+                    ss1 = ['u','v','w','T','rho'] ## 'p'
+                    ss2 = ['uI','vI','wI', 'uII','vII','wII', 'pI'] ## 'TI','rhoI'
+                    
+                    formats = [ np.float32 for s in ss1+ss2 ]
+                    #shape = (nx,ny,nz,ntr)
+                    shape = (nx,ny,nz,ntc)
+                    dd = np.zeros(shape=shape, dtype={'names':ss1+ss2, 'formats':formats}, order='C')
                     
-                    r_uII_uII = rho*uII*uII
-                    r_uII_vII = rho*uII*vII
-                    r_uII_wII = rho*uII*wII
-                    
-                    r_vII_uII = rho*vII*uII
-                    r_vII_vII = rho*vII*vII
-                    r_vII_wII = rho*vII*wII
-                    
-                    r_wII_uII = rho*wII*uII
-                    r_wII_vII = rho*wII*vII
-                    r_wII_wII = rho*wII*wII
-                    
-                    ## unsteady_production_ = - ( r_uII_uII * dudx_fv + r_uII_vII * dudy_fv + r_uII_wII * dudz_fv \
-                    ##                          + r_uII_vII * dvdx_fv + r_vII_vII * dvdy_fv + r_vII_wII * dvdz_fv \
-                    ##                          + r_uII_wII * dwdx_fv + r_vII_wII * dwdy_fv + r_wII_wII * dwdz_fv )
-                    
-                    r_uIIuII_ij = np.stack((np.stack((r_uII_uII, r_uII_vII, r_uII_wII), axis=4),
-                                            np.stack((r_vII_uII, r_vII_vII, r_vII_wII), axis=4),
-                                            np.stack((r_wII_uII, r_wII_vII, r_wII_wII), axis=4)), axis=5)
-                    
-                    dudx_fv_ij = np.stack((np.stack((dudx_fv, dudy_fv, dudz_fv), axis=4),
-                                           np.stack((dvdx_fv, dvdy_fv, dvdz_fv), axis=4),
-                                           np.stack((dwdx_fv, dwdy_fv, dwdz_fv), axis=4)), axis=5)
+                    for ss in ss1:
+                        dset = self['data/%s'%ss]
+                        self.comm.Barrier()
+                        t_start = timeit.default_timer()
+                        with dset.collective:
+                            #dd[ss] = dset[rt1:rt2,:,:,:].T
+                            dd[ss] = dset[ct1:ct2,:,:,:].T
+                        self.comm.Barrier()
+                        t_delta = timeit.default_timer() - t_start
+                        #data_gb = 4*nx*ny*nz*nt/1024**3
+                        data_gb = self.n_ranks * 4*nx*ny*nz*ntc/1024**3 ## approximate!
+                        if verbose:
+                            tqdm.write( even_print('read: %s'%ss, '%0.3f [GB]  %0.3f [s]  %0.3f [GB/s]'%(data_gb,t_delta,(data_gb/t_delta)), s=True) )
                     
-                    unsteady_production = -1*np.einsum('xyztij,xyztij->xyzt', r_uIIuII_ij, dudx_fv_ij)
+                    for ss in ss2:
+                        dset = hf_prime['data/%s'%ss]
+                        self.comm.Barrier()
+                        t_start = timeit.default_timer()
+                        with dset.collective:
+                            #dd[ss] = dset[rt1:rt2,:,:,:].T
+                            dd[ss] = dset[ct1:ct2,:,:,:].T
+                        self.comm.Barrier()
+                        t_delta = timeit.default_timer() - t_start
+                        #data_gb = 4*nx*ny*nz*nt/1024**3
+                        data_gb = self.n_ranks * 4*nx*ny*nz*ntc/1024**3 ## approximate!
+                        if verbose:
+                            tqdm.write( even_print('read: %s'%ss, '%0.3f [GB]  %0.3f [s]  %0.3f [GB/s]'%(data_gb,t_delta,(data_gb/t_delta)), s=True) )
                     
-                    ## np.testing.assert_allclose(unsteady_production, unsteady_production_, atol=20000)
-                    ## print('check passed : np.einsum()')
+                    if verbose: tqdm.write(72*'-')
                     
-                    t_delta = timeit.default_timer() - t_start
-                    if verbose:
-                        tqdm.write(even_print('production', format_time_string(t_delta), s=True))
+                    # ===
                     
-                    # === do avg
-                    t_start = timeit.default_timer()
-                    unsteady_production_sum   = np.zeros((nx,ny,nz,1), dtype=np.float64, order='C')
-                    unsteady_production_sum_i = np.sum(unsteady_production, axis=3, keepdims=True, dtype=np.float64)
-                    self.comm.Reduce([unsteady_production_sum_i, MPI.DOUBLE], [unsteady_production_sum, MPI.DOUBLE], op=MPI.SUM, root=0)
-                    if (self.rank==0):
-                        production = ((1/nt)*unsteady_production_sum).astype(np.float32)
-                    t_delta = timeit.default_timer() - t_start
+                    data_gb = dd.nbytes / 1024**3
                     if verbose:
-                        tqdm.write(even_print('t avg production', format_time_string(t_delta),s=True))
-                    
-                    # === write avg
-                    with rgd(fn_rgd_turb_budget_mean, 'a', driver='mpio', comm=self.comm, libver='latest') as f1:
-                        if (self.rank==0):
-                            f1['data/production'][:,:,:,:] = production.T
-                    self.comm.Barrier()
-                    
-                    # === write unsteady data
-                    if save_unsteady:
-                        with rgd(fn_rgd_turb_budget, 'a', driver='mpio', comm=self.comm, libver='latest') as f1:
-                            dset = f1['data/unsteady_production']
-                            self.comm.Barrier()
-                            t_start = timeit.default_timer()
-                            with dset.collective:
-                                dset[rt1:rt2,:,:,:] = unsteady_production.T
-                            t_delta = timeit.default_timer() - t_start
-                            data_gb = 4*nx*ny*nz*nt/1024**3
-                            if verbose:
-                                even_print('write: unsteady production', '%0.3f [GB]  %0.3f [s]  %0.3f [GB/s]'%(data_gb,t_delta,(data_gb/t_delta)))
-                    
-                    # === release mem
-                    r_uII_uII           = None; del r_uII_uII
-                    r_uII_vII           = None; del r_uII_vII
-                    r_uII_wII           = None; del r_uII_wII
-                    r_vII_uII           = None; del r_vII_uII
-                    r_vII_vII           = None; del r_vII_vII
-                    r_vII_wII           = None; del r_vII_wII
-                    r_wII_uII           = None; del r_wII_uII
-                    r_wII_vII           = None; del r_wII_vII
-                    r_wII_wII           = None; del r_wII_wII
-                    r_uIIuII_ij         = None; del r_uIIuII_ij
-                    dudx_fv_ij          = None; del dudx_fv_ij
-                    unsteady_production = None; del unsteady_production
+                        tqdm.write(even_print('data_gb (rank)', '%0.1f [GB]'%data_gb, s=True))
                     
-                    self.comm.Barrier()
                     mem_avail_gb = psutil.virtual_memory().available/1024**3
                     mem_free_gb  = psutil.virtual_memory().free/1024**3
                     if verbose:
-                        tqdm.write(even_print('mem available', '%0.1f [GB]'%mem_avail_gb, s=True))
-                        tqdm.write(even_print('mem free',      '%0.1f [GB]'%mem_free_gb,  s=True))
-                
-                # === dissipation ε
-                if True:
+                        tqdm.write(even_print('mem free', '%0.1f [GB]'%mem_free_gb, s=True))
                     
-                    if verbose: print(72*'-')
-                    t_start = timeit.default_timer()
-                    
-                    duIIdx_ij_duIdx_ij = np.einsum('xyztij,xyztij->xyzt', duIIdx_ij, duIdx_ij)
-                    duIIdx_ij_duIdx_ji = np.einsum('xyztij,xyztji->xyzt', duIIdx_ij, duIdx_ij)
+                    # === redimensionalize the unsteady data
                     
-                    ## # === from pp_turbulent_budget.F90
-                    ## unsteady_dissipation_ = mu * ( (duIdx + duIdx) * duIIdx  +  (duIdy + dvIdx) * duIIdy  +  (duIdz + dwIdx) * duIIdz \
-                    ##                              + (dvIdx + duIdy) * dvIIdx  +  (dvIdy + dvIdy) * dvIIdy  +  (dvIdz + dwIdy) * dvIIdz \
-                    ##                              + (dwIdx + duIdz) * dwIIdx  +  (dwIdy + dvIdz) * dwIIdy  +  (dwIdz + dwIdz) * dwIIdz )
+                    u    = np.copy( dd['u']   * U_inf )
+                    v    = np.copy( dd['v']   * U_inf )
+                    w    = np.copy( dd['w']   * U_inf )
+                    uI   = np.copy( dd['uI']  * U_inf )
+                    vI   = np.copy( dd['vI']  * U_inf )
+                    wI   = np.copy( dd['wI']  * U_inf )
+                    uII  = np.copy( dd['uII'] * U_inf )
+                    vII  = np.copy( dd['vII'] * U_inf )
+                    wII  = np.copy( dd['wII'] * U_inf )
+                    
+                    rho  = np.copy( dd['rho']  * rho_inf              )
+                    #rhoI = np.copy( dd['rhoI'] * rho_inf              )
+                    #p    = np.copy( dd['p']    * (rho_inf * U_inf**2) )
+                    pI   = np.copy( dd['pI']   * (rho_inf * U_inf**2) )
+                    T    = np.copy( dd['T']    * T_inf                )
+                    #TI   = np.copy( dd['TI']   * T_inf                )
+                    
+                    #mu = np.copy(14.58e-7*T**1.5/(T+110.4))
+                    mu = self.C_Suth * T**(3/2) / (T + self.S_Suth)
+                    nu = mu / rho
                     
-                    unsteady_dissipation = mu*(duIIdx_ij_duIdx_ij + duIIdx_ij_duIdx_ji)
+                    dd = None ; del dd
                     
-                    ## np.testing.assert_allclose(unsteady_dissipation, unsteady_dissipation_, rtol=1e-4)
-                    ## print('check passed : np.einsum() : dissipation')
-                    
-                    t_delta = timeit.default_timer() - t_start
-                    if verbose:
-                        tqdm.write(even_print('dissipation', format_time_string(t_delta),s=True))
+                    # === get gradients
                     
-                    # === do avg
                     t_start = timeit.default_timer()
-                    unsteady_dissipation_sum   = np.zeros((nx,ny,nz,1), dtype=np.float64, order='C')
-                    unsteady_dissipation_sum_i = np.sum(unsteady_dissipation, axis=3, keepdims=True, dtype=np.float64)
-                    self.comm.Reduce([unsteady_dissipation_sum_i, MPI.DOUBLE], [unsteady_dissipation_sum, MPI.DOUBLE], op=MPI.SUM, root=0)
-                    if (self.rank==0):
-                        dissipation = ((1/nt)*unsteady_dissipation_sum).astype(np.float32)
-                    t_delta = timeit.default_timer() - t_start
-                    if verbose:
-                        tqdm.write(even_print('t avg dissipation', format_time_string(t_delta),s=True))
                     
-                    # === write avg
-                    with rgd(fn_rgd_turb_budget_mean, 'a', driver='mpio', comm=self.comm, libver='latest') as f1:
-                        if (self.rank==0):
-                            f1['data/dissipation'][:,:,:,:] = dissipation.T
-                    self.comm.Barrier()
+                    ## numpy.gradient() --> low order, maximally O2
+                    # dudx   = np.gradient(u,   x, edge_order=2, axis=0)
+                    # dudy   = np.gradient(u,   y, edge_order=2, axis=1)
+                    # dudz   = np.gradient(u,   z, edge_order=2, axis=2)
+                    # dvdx   = np.gradient(v,   x, edge_order=2, axis=0)
+                    # dvdy   = np.gradient(v,   y, edge_order=2, axis=1)
+                    # dvdz   = np.gradient(v,   z, edge_order=2, axis=2)
+                    # dwdx   = np.gradient(w,   x, edge_order=2, axis=0)
+                    # dwdy   = np.gradient(w,   y, edge_order=2, axis=1)
+                    # dwdz   = np.gradient(w,   z, edge_order=2, axis=2)
+                    # ##
+                    # duIdx  = np.gradient(uI,  x, edge_order=2, axis=0)
+                    # duIdy  = np.gradient(uI,  y, edge_order=2, axis=1)
+                    # duIdz  = np.gradient(uI,  z, edge_order=2, axis=2)
+                    # dvIdx  = np.gradient(vI,  x, edge_order=2, axis=0)
+                    # dvIdy  = np.gradient(vI,  y, edge_order=2, axis=1)
+                    # dvIdz  = np.gradient(vI,  z, edge_order=2, axis=2)
+                    # dwIdx  = np.gradient(wI,  x, edge_order=2, axis=0)
+                    # dwIdy  = np.gradient(wI,  y, edge_order=2, axis=1)
+                    # dwIdz  = np.gradient(wI,  z, edge_order=2, axis=2)
+                    # ##
+                    # duIIdx = np.gradient(uII, x, edge_order=2, axis=0)
+                    # duIIdy = np.gradient(uII, y, edge_order=2, axis=1)
+                    # duIIdz = np.gradient(uII, z, edge_order=2, axis=2)
+                    # dvIIdx = np.gradient(vII, x, edge_order=2, axis=0)
+                    # dvIIdy = np.gradient(vII, y, edge_order=2, axis=1)
+                    # dvIIdz = np.gradient(vII, z, edge_order=2, axis=2)
+                    # dwIIdx = np.gradient(wII, x, edge_order=2, axis=0)
+                    # dwIIdy = np.gradient(wII, y, edge_order=2, axis=1)
+                    # dwIIdz = np.gradient(wII, z, edge_order=2, axis=2)
+                    
+                    ## turbx.gradient() --> high order
+                    ## get unsteady strain tensor elements
+                    dudx   = gradient(u, x, acc=acc, edge_stencil=edge_stencil, axis=0)
+                    dudy   = gradient(u, y, acc=acc, edge_stencil=edge_stencil, axis=1)
+                    dudz   = gradient(u, z, acc=acc, edge_stencil=edge_stencil, axis=2)
+                    dvdx   = gradient(v, x, acc=acc, edge_stencil=edge_stencil, axis=0)
+                    dvdy   = gradient(v, y, acc=acc, edge_stencil=edge_stencil, axis=1)
+                    dvdz   = gradient(v, z, acc=acc, edge_stencil=edge_stencil, axis=2)
+                    dwdx   = gradient(w, x, acc=acc, edge_stencil=edge_stencil, axis=0)
+                    dwdy   = gradient(w, y, acc=acc, edge_stencil=edge_stencil, axis=1)
+                    dwdz   = gradient(w, z, acc=acc, edge_stencil=edge_stencil, axis=2)
+                    ##
+                    duIdx  = gradient(uI, x, acc=acc, edge_stencil=edge_stencil, axis=0)
+                    duIdy  = gradient(uI, y, acc=acc, edge_stencil=edge_stencil, axis=1)
+                    duIdz  = gradient(uI, z, acc=acc, edge_stencil=edge_stencil, axis=2)
+                    dvIdx  = gradient(vI, x, acc=acc, edge_stencil=edge_stencil, axis=0)
+                    dvIdy  = gradient(vI, y, acc=acc, edge_stencil=edge_stencil, axis=1)
+                    dvIdz  = gradient(vI, z, acc=acc, edge_stencil=edge_stencil, axis=2)
+                    dwIdx  = gradient(wI, x, acc=acc, edge_stencil=edge_stencil, axis=0)
+                    dwIdy  = gradient(wI, y, acc=acc, edge_stencil=edge_stencil, axis=1)
+                    dwIdz  = gradient(wI, z, acc=acc, edge_stencil=edge_stencil, axis=2)
+                    ##
+                    duIIdx = gradient(uII, x, acc=acc, edge_stencil=edge_stencil, axis=0)
+                    duIIdy = gradient(uII, y, acc=acc, edge_stencil=edge_stencil, axis=1)
+                    duIIdz = gradient(uII, z, acc=acc, edge_stencil=edge_stencil, axis=2)
+                    dvIIdx = gradient(vII, x, acc=acc, edge_stencil=edge_stencil, axis=0)
+                    dvIIdy = gradient(vII, y, acc=acc, edge_stencil=edge_stencil, axis=1)
+                    dvIIdz = gradient(vII, z, acc=acc, edge_stencil=edge_stencil, axis=2)
+                    dwIIdx = gradient(wII, x, acc=acc, edge_stencil=edge_stencil, axis=0)
+                    dwIIdy = gradient(wII, y, acc=acc, edge_stencil=edge_stencil, axis=1)
+                    dwIIdz = gradient(wII, z, acc=acc, edge_stencil=edge_stencil, axis=2)
                     
-                    # === write unsteady data
-                    if save_unsteady:
-                        with rgd(fn_rgd_turb_budget, 'a', driver='mpio', comm=self.comm, libver='latest') as f1:
-                            dset = f1['data/unsteady_dissipation']
-                            self.comm.Barrier()
-                            t_start = timeit.default_timer()
-                            with dset.collective:
-                                dset[rt1:rt2,:,:,:] = unsteady_dissipation.T
-                            t_delta = timeit.default_timer() - t_start
-                            data_gb = 4*nx*ny*nz*nt/1024**3
-                            if verbose:
-                                even_print('write: unsteady dissipation', '%0.3f [GB]  %0.3f [s]  %0.3f [GB/s]'%(data_gb,t_delta,(data_gb/t_delta)))
+                    t_delta = timeit.default_timer() - t_start
                     
-                    # === release mem
-                    duIIdx_ij_duIdx_ij   = None; del duIIdx_ij_duIdx_ij
-                    duIIdx_ij_duIdx_ji   = None; del duIIdx_ij_duIdx_ji
-                    unsteady_dissipation = None; del unsteady_dissipation
+                    if verbose:
+                        tqdm.write(even_print('get gradients', format_time_string(t_delta), s=True))
                     
                     self.comm.Barrier()
                     mem_avail_gb = psutil.virtual_memory().available/1024**3
                     mem_free_gb  = psutil.virtual_memory().free/1024**3
                     if verbose:
                         tqdm.write(even_print('mem available', '%0.1f [GB]'%mem_avail_gb, s=True))
                         tqdm.write(even_print('mem free',      '%0.1f [GB]'%mem_free_gb,  s=True))
-                
-                # === transport
-                if True:
                     
-                    if verbose: print(72*'-')
+                    # === stack velocities into vectors, fluctuating strains into (Re stress) tensor
+                    
                     t_start = timeit.default_timer()
                     
-                    tc = np.einsum('xyzt,xyzti,xyzti,xyztj->xyztj', rho, uII_i, uII_i, uII_i) ## triple correlation
-                    tc_ddx = np.gradient(tc, x, axis=0, edge_order=2)
-                    tc_ddy = np.gradient(tc, y, axis=1, edge_order=2)
-                    tc_ddz = np.gradient(tc, z, axis=2, edge_order=2)
-                    unsteady_transport = -0.5*(tc_ddx[:,:,:,:,0] + tc_ddy[:,:,:,:,1] + tc_ddz[:,:,:,:,2])
+                    uI_i  = np.copy(np.stack((uI,  vI,  wI ), axis=-1))
+                    uII_i = np.copy(np.stack((uII, vII, wII), axis=-1))
                     
-                    t_delta = timeit.default_timer() - t_start
-                    if verbose:
-                        tqdm.write(even_print('transport', format_time_string(t_delta),s=True))
+                    duIdx_ij = np.copy( np.stack((np.stack((duIdx, duIdy, duIdz), axis=4),
+                                                  np.stack((dvIdx, dvIdy, dvIdz), axis=4),
+                                                  np.stack((dwIdx, dwIdy, dwIdz), axis=4)), axis=5) )
+                    
+                    duIIdx_ij = np.copy( np.stack((np.stack((duIIdx, duIIdy, duIIdz), axis=4),
+                                                   np.stack((dvIIdx, dvIIdy, dvIIdz), axis=4),
+                                                   np.stack((dwIIdx, dwIIdy, dwIIdz), axis=4)), axis=5) )
                     
-                    # === do avg
-                    t_start = timeit.default_timer()
-                    unsteady_transport_sum   = np.zeros((nx,ny,nz,1), dtype=np.float64, order='C')
-                    unsteady_transport_sum_i = np.sum(unsteady_transport, axis=3, keepdims=True, dtype=np.float64)
-                    self.comm.Reduce([unsteady_transport_sum_i, MPI.DOUBLE], [unsteady_transport_sum, MPI.DOUBLE], op=MPI.SUM, root=0)
-                    if (self.rank==0):
-                        transport = ( (1/nt)*unsteady_transport_sum ).astype(np.float32)
                     t_delta = timeit.default_timer() - t_start
                     if verbose:
-                        tqdm.write(even_print('t avg transport', format_time_string(t_delta),s=True))
-                    
-                    # === write avg
-                    with rgd(fn_rgd_turb_budget_mean, 'a', driver='mpio', comm=self.comm, libver='latest') as f1:
-                        if (self.rank==0):
-                            f1['data/transport'][:,:,:,:] = transport.T
-                    self.comm.Barrier()
-                    
-                    # === write unsteady data
-                    if save_unsteady:
-                        with rgd(fn_rgd_turb_budget, 'a', driver='mpio', comm=self.comm, libver='latest') as f1:
-                            dset = f1['data/unsteady_transport']
-                            self.comm.Barrier()
-                            t_start = timeit.default_timer()
-                            with dset.collective:
-                                dset[rt1:rt2,:,:,:] = unsteady_transport.T
-                            t_delta = timeit.default_timer() - t_start
-                            data_gb = 4*nx*ny*nz*nt/1024**3
-                            if verbose:
-                                even_print('write: unsteady transport', '%0.3f [GB]  %0.3f [s]  %0.3f [GB/s]'%(data_gb,t_delta,(data_gb/t_delta)))
-                    
-                    # === release mem
-                    tc     = None; del tc
-                    tc_ddx = None; del tc_ddx
-                    tc_ddy = None; del tc_ddy
-                    tc_ddz = None; del tc_ddz
-                    unsteady_transport = None; del unsteady_transport
+                        tqdm.write(even_print('tensor stacking',format_time_string(t_delta), s=True))
                     
                     self.comm.Barrier()
                     mem_avail_gb = psutil.virtual_memory().available/1024**3
                     mem_free_gb  = psutil.virtual_memory().free/1024**3
                     if verbose:
                         tqdm.write(even_print('mem available', '%0.1f [GB]'%mem_avail_gb, s=True))
                         tqdm.write(even_print('mem free',      '%0.1f [GB]'%mem_free_gb,  s=True))
-                
-                # === (viscous) diffusion
-                if True:
-                    
-                    if verbose: print(72*'-')
-                    t_start = timeit.default_timer()
-                    
-                    omega_ij = duIdx_ij + np.transpose(duIdx_ij, axes=(0,1,2,3,5,4))
                     
-                    if False:
+                    # === production : P
+                    if True:
+                        
+                        if verbose: tqdm.write(72*'-')
+                        t_start = timeit.default_timer()
                         
-                        omega_ij_2 = np.stack((np.stack(((duIdx+duIdx), (dvIdx+duIdy), (dwIdx+duIdz)), axis=4),
-                                               np.stack(((duIdy+dvIdx), (dvIdy+dvIdy), (dwIdy+dvIdz)), axis=4),
-                                               np.stack(((duIdz+dwIdx), (dvIdz+dwIdy), (dwIdz+dwIdz)), axis=4)), axis=5)
+                        r_uII_uII = rho*uII*uII
+                        r_uII_vII = rho*uII*vII
+                        r_uII_wII = rho*uII*wII
+                        
+                        r_vII_uII = rho*vII*uII
+                        r_vII_vII = rho*vII*vII
+                        r_vII_wII = rho*vII*wII
+                        
+                        r_wII_uII = rho*wII*uII
+                        r_wII_vII = rho*wII*vII
+                        r_wII_wII = rho*wII*wII
+                        
+                        ## unsteady_production_ = - ( r_uII_uII * dudx_fv + r_uII_vII * dudy_fv + r_uII_wII * dudz_fv \
+                        ##                          + r_uII_vII * dvdx_fv + r_vII_vII * dvdy_fv + r_vII_wII * dvdz_fv \
+                        ##                          + r_uII_wII * dwdx_fv + r_vII_wII * dwdy_fv + r_wII_wII * dwdz_fv )
+                        
+                        r_uIIuII_ij = np.stack((np.stack((r_uII_uII, r_uII_vII, r_uII_wII), axis=4),
+                                                np.stack((r_vII_uII, r_vII_vII, r_vII_wII), axis=4),
+                                                np.stack((r_wII_uII, r_wII_vII, r_wII_wII), axis=4)), axis=5)
+                        
+                        dudx_fv_ij = np.stack((np.stack((dudx_fv, dudy_fv, dudz_fv), axis=4),
+                                               np.stack((dvdx_fv, dvdy_fv, dvdz_fv), axis=4),
+                                               np.stack((dwdx_fv, dwdy_fv, dwdz_fv), axis=4)), axis=5)
                         
-                        np.testing.assert_allclose(omega_ij, omega_ij_2, rtol=1e-8)
+                        unsteady_production = -1*np.einsum('xyztij,xyztij->xyzt', r_uIIuII_ij, dudx_fv_ij)
                         
+                        ## np.testing.assert_allclose(unsteady_production, unsteady_production_, atol=20000)
+                        ## print('check passed : np.einsum()')
+                        
+                        t_delta = timeit.default_timer() - t_start
                         if verbose:
-                            print('check passed : np.einsum()')
-                    
-                    ## ## this one is likely wrong
-                    ## omega_ij = np.stack((np.stack(((duIdx+duIdx), (dvIdx+duIdy), (dwIdx+duIdz)), axis=4),
-                    ##                      np.stack(((duIdy+duIdx), (dvIdy+duIdy), (dwIdy+duIdz)), axis=4),
-                    ##                      np.stack(((duIdz+duIdx), (dvIdz+duIdy), (dwIdz+duIdz)), axis=4)), axis=5)
-                    
-                    A = np.einsum('xyzt,xyzti,xyztij->xyztj', mu, uI_i, omega_ij)
-                    A_ddx = np.gradient(A[:,:,:,:,0], x, axis=0, edge_order=2)
-                    A_ddy = np.gradient(A[:,:,:,:,1], y, axis=1, edge_order=2)
-                    A_ddz = np.gradient(A[:,:,:,:,2], z, axis=2, edge_order=2)
-                    unsteady_diffusion = A_ddx + A_ddy + A_ddz
-                    
-                    t_delta = timeit.default_timer() - t_start
-                    if verbose:
-                        tqdm.write(even_print('diffusion', format_time_string(t_delta),s=True))
+                            tqdm.write(even_print('calc production', format_time_string(t_delta), s=True))
+                        
+                        self.comm.Barrier()
+                        
+                        ## combine sums across ranks for this [t] chunk
+                        unsteady_production_sum_i   = np.sum(unsteady_production, axis=3, keepdims=True, dtype=np.float64)
+                        unsteady_production_sum_buf = np.zeros((nx,ny,nz,1), dtype=np.float64, order='C')
+                        self.comm.Reduce([unsteady_production_sum_i, MPI.DOUBLE],
+                                         [unsteady_production_sum_buf, MPI.DOUBLE],
+                                         op=MPI.SUM,
+                                         root=0)
+                        
+                        ## add aggregated sum (across ranks) to the total accumulator
+                        unsteady_production_sum += unsteady_production_sum_buf
+                        
+                        # === release mem
+                        r_uII_uII           = None; del r_uII_uII
+                        r_uII_vII           = None; del r_uII_vII
+                        r_uII_wII           = None; del r_uII_wII
+                        r_vII_uII           = None; del r_vII_uII
+                        r_vII_vII           = None; del r_vII_vII
+                        r_vII_wII           = None; del r_vII_wII
+                        r_wII_uII           = None; del r_wII_uII
+                        r_wII_vII           = None; del r_wII_vII
+                        r_wII_wII           = None; del r_wII_wII
+                        r_uIIuII_ij         = None; del r_uIIuII_ij
+                        dudx_fv_ij          = None; del dudx_fv_ij
+                        unsteady_production = None; del unsteady_production
+                        
+                        self.comm.Barrier()
+                        mem_avail_gb = psutil.virtual_memory().available/1024**3
+                        mem_free_gb  = psutil.virtual_memory().free/1024**3
+                        if verbose:
+                            tqdm.write(even_print('mem available', '%0.1f [GB]'%mem_avail_gb, s=True))
+                            tqdm.write(even_print('mem free',      '%0.1f [GB]'%mem_free_gb,  s=True))
                     
-                    # === do avg
-                    t_start = timeit.default_timer()
-                    unsteady_diffusion_sum   = np.zeros((nx,ny,nz,1), dtype=np.float64, order='C')
-                    unsteady_diffusion_sum_i = np.sum(unsteady_diffusion, axis=3, keepdims=True, dtype=np.float64)
-                    self.comm.Reduce([unsteady_diffusion_sum_i, MPI.DOUBLE], [unsteady_diffusion_sum, MPI.DOUBLE], op=MPI.SUM, root=0)
-                    if (self.rank==0):
-                        diffusion = ( (1/nt)*unsteady_diffusion_sum ).astype(np.float32)
-                    t_delta = timeit.default_timer() - t_start
-                    if verbose:
-                        tqdm.write(even_print('t avg diffusion', format_time_string(t_delta),s=True))
+                    # === dissipation : ϕ,ε
+                    if True:
+                        
+                        if verbose: tqdm.write(72*'-')
+                        t_start = timeit.default_timer()
+                        
+                        duIIdx_ij_duIdx_ij = np.einsum('xyztij,xyztij->xyzt', duIIdx_ij, duIdx_ij)
+                        duIIdx_ij_duIdx_ji = np.einsum('xyztij,xyztji->xyzt', duIIdx_ij, duIdx_ij)
+                        
+                        ## # === from pp_turbulent_budget.F90
+                        ## unsteady_dissipation_ = mu * ( (duIdx + duIdx) * duIIdx  +  (duIdy + dvIdx) * duIIdy  +  (duIdz + dwIdx) * duIIdz \
+                        ##                              + (dvIdx + duIdy) * dvIIdx  +  (dvIdy + dvIdy) * dvIIdy  +  (dvIdz + dwIdy) * dvIIdz \
+                        ##                              + (dwIdx + duIdz) * dwIIdx  +  (dwIdy + dvIdz) * dwIIdy  +  (dwIdz + dwIdz) * dwIIdz )
+                        
+                        unsteady_dissipation = mu*(duIIdx_ij_duIdx_ij + duIIdx_ij_duIdx_ji)
+                        
+                        ## np.testing.assert_allclose(unsteady_dissipation, unsteady_dissipation_, rtol=1e-4)
+                        ## print('check passed : np.einsum() : dissipation')
+                        
+                        t_delta = timeit.default_timer() - t_start
+                        if verbose:
+                            tqdm.write(even_print('calc dissipation', format_time_string(t_delta),s=True))
+                        
+                        self.comm.Barrier()
+                        
+                        ## combine sums across ranks for this [t] chunk
+                        unsteady_dissipation_sum_i   = np.sum(unsteady_dissipation, axis=3, keepdims=True, dtype=np.float64)
+                        unsteady_dissipation_sum_buf = np.zeros((nx,ny,nz,1), dtype=np.float64, order='C')
+                        self.comm.Reduce([unsteady_dissipation_sum_i, MPI.DOUBLE],
+                                         [unsteady_dissipation_sum_buf, MPI.DOUBLE],
+                                         op=MPI.SUM,
+                                         root=0)
+                        
+                        ## add aggregated sum (across ranks) to the total accumulator
+                        unsteady_dissipation_sum += unsteady_dissipation_sum_buf
+                        
+                        ## release mem
+                        duIIdx_ij_duIdx_ij   = None; del duIIdx_ij_duIdx_ij
+                        duIIdx_ij_duIdx_ji   = None; del duIIdx_ij_duIdx_ji
+                        unsteady_dissipation = None; del unsteady_dissipation
+                        
+                        self.comm.Barrier()
+                        mem_avail_gb = psutil.virtual_memory().available/1024**3
+                        mem_free_gb  = psutil.virtual_memory().free/1024**3
+                        if verbose:
+                            tqdm.write(even_print('mem available', '%0.1f [GB]'%mem_avail_gb, s=True))
+                            tqdm.write(even_print('mem free',      '%0.1f [GB]'%mem_free_gb,  s=True))
                     
-                    # === write avg
-                    with rgd(fn_rgd_turb_budget_mean, 'a', driver='mpio', comm=self.comm, libver='latest') as f1:
-                        if (self.rank==0):
-                            f1['data/diffusion'][:,:,:,:] = diffusion.T
-                    self.comm.Barrier()
+                    # === transport : T
+                    if True:
+                        
+                        if verbose: tqdm.write(72*'-')
+                        t_start = timeit.default_timer()
+                        
+                        ## triple correlation
+                        tc = np.einsum('xyzt,xyzti,xyzti,xyztj->xyztj', rho, uII_i, uII_i, uII_i)
+                        
+                        #tc_ddx = np.gradient(tc, x, axis=0, edge_order=2)
+                        #tc_ddy = np.gradient(tc, y, axis=1, edge_order=2)
+                        #tc_ddz = np.gradient(tc, z, axis=2, edge_order=2)
+                        
+                        tc_ddx = gradient(tc, x, axis=0, acc=acc, edge_stencil=edge_stencil)
+                        tc_ddy = gradient(tc, y, axis=1, acc=acc, edge_stencil=edge_stencil)
+                        tc_ddz = gradient(tc, z, axis=2, acc=acc, edge_stencil=edge_stencil)
+                        
+                        unsteady_transport = -0.5*(tc_ddx[:,:,:,:,0] + tc_ddy[:,:,:,:,1] + tc_ddz[:,:,:,:,2])
+                        
+                        t_delta = timeit.default_timer() - t_start
+                        if verbose:
+                            tqdm.write(even_print('calc transport', format_time_string(t_delta),s=True))
+                        
+                        ## combine sums across ranks for this [t] chunk
+                        unsteady_transport_sum_i   = np.sum(unsteady_transport, axis=3, keepdims=True, dtype=np.float64)
+                        unsteady_transport_sum_buf = np.zeros((nx,ny,nz,1), dtype=np.float64, order='C')
+                        self.comm.Reduce([unsteady_transport_sum_i, MPI.DOUBLE],
+                                         [unsteady_transport_sum_buf, MPI.DOUBLE],
+                                         op=MPI.SUM,
+                                         root=0)
+                        
+                        self.comm.Barrier()
+                        
+                        ## add aggregated sum (across ranks) to the total accumulator
+                        unsteady_transport_sum += unsteady_transport_sum_buf
+                        
+                        ## release mem
+                        tc     = None; del tc
+                        tc_ddx = None; del tc_ddx
+                        tc_ddy = None; del tc_ddy
+                        tc_ddz = None; del tc_ddz
+                        unsteady_transport = None; del unsteady_transport
+                        
+                        self.comm.Barrier()
+                        mem_avail_gb = psutil.virtual_memory().available/1024**3
+                        mem_free_gb  = psutil.virtual_memory().free/1024**3
+                        if verbose:
+                            tqdm.write(even_print('mem available', '%0.1f [GB]'%mem_avail_gb, s=True))
+                            tqdm.write(even_print('mem free',      '%0.1f [GB]'%mem_free_gb,  s=True))
                     
-                    # === write unsteady data
-                    if save_unsteady:
-                        with rgd(fn_rgd_turb_budget, 'a', driver='mpio', comm=self.comm, libver='latest') as f1:
-                            dset = f1['data/unsteady_diffusion']
-                            self.comm.Barrier()
-                            t_start = timeit.default_timer()
-                            with dset.collective:
-                                dset[rt1:rt2,:,:,:] = unsteady_diffusion.T
-                            t_delta = timeit.default_timer() - t_start
-                            data_gb = 4*nx*ny*nz*nt/1024**3
+                    # === viscous diffusion : D
+                    if True:
+                        
+                        if verbose: tqdm.write(72*'-')
+                        t_start = timeit.default_timer()
+                        
+                        omega_ij = duIdx_ij + np.transpose(duIdx_ij, axes=(0,1,2,3,5,4))
+                        
+                        if False:
+                            
+                            omega_ij_2 = np.stack((np.stack(((duIdx+duIdx), (dvIdx+duIdy), (dwIdx+duIdz)), axis=4),
+                                                   np.stack(((duIdy+dvIdx), (dvIdy+dvIdy), (dwIdy+dvIdz)), axis=4),
+                                                   np.stack(((duIdz+dwIdx), (dvIdz+dwIdy), (dwIdz+dwIdz)), axis=4)), axis=5)
+                            
+                            np.testing.assert_allclose(omega_ij, omega_ij_2, rtol=1e-8)
+                            
                             if verbose:
-                                even_print('write: unsteady diffusion', '%0.3f [GB]  %0.3f [s]  %0.3f [GB/s]'%(data_gb,t_delta,(data_gb/t_delta)))
-                    
-                    # === release mem
-                    omega_ij = None; del omega_ij
-                    A        = None; del A
-                    A_ddx    = None; del A_ddx
-                    A_ddy    = None; del A_ddy
-                    A_ddz    = None; del A_ddz
-                    unsteady_diffusion = None; del unsteady_diffusion
-                    
-                    self.comm.Barrier()
-                    mem_avail_gb = psutil.virtual_memory().available/1024**3
-                    mem_free_gb  = psutil.virtual_memory().free/1024**3
-                    if verbose:
-                        tqdm.write(even_print('mem available', '%0.1f [GB]'%mem_avail_gb, s=True))
-                        tqdm.write(even_print('mem free',      '%0.1f [GB]'%mem_free_gb,  s=True))
-                
-                # === pressure diffusion
-                if True:
-                    
-                    if verbose: print(72*'-')
-                    t_start = timeit.default_timer()
-                    
-                    A = np.einsum('xyzti,xyzt->xyzti', uII_i, pI)
-                    A_ddx = np.gradient(A[:,:,:,:,0], x, axis=0, edge_order=2)
-                    A_ddy = np.gradient(A[:,:,:,:,1], y, axis=1, edge_order=2)
-                    A_ddz = np.gradient(A[:,:,:,:,2], z, axis=2, edge_order=2)
-                    unsteady_p_diffusion = A_ddx + A_ddy + A_ddz
-                    
-                    t_delta = timeit.default_timer() - t_start
-                    if verbose:
-                        tqdm.write(even_print('p_diffusion', format_time_string(t_delta),s=True))
+                                print('check passed : omega_ij')
+                        
+                        ## ## this one is likely wrong
+                        ## omega_ij = np.stack((np.stack(((duIdx+duIdx), (dvIdx+duIdy), (dwIdx+duIdz)), axis=4),
+                        ##                      np.stack(((duIdy+duIdx), (dvIdy+duIdy), (dwIdy+duIdz)), axis=4),
+                        ##                      np.stack(((duIdz+duIdx), (dvIdz+duIdy), (dwIdz+duIdz)), axis=4)), axis=5)
+                        
+                        A = np.einsum('xyzt,xyzti,xyztij->xyztj', mu, uI_i, omega_ij)
+                        
+                        # A_ddx = np.gradient(A[:,:,:,:,0], x, axis=0, edge_order=2)
+                        # A_ddy = np.gradient(A[:,:,:,:,1], y, axis=1, edge_order=2)
+                        # A_ddz = np.gradient(A[:,:,:,:,2], z, axis=2, edge_order=2)
+                        
+                        A_ddx = gradient(A[:,:,:,:,0], x, axis=0, acc=acc, edge_stencil=edge_stencil)
+                        A_ddy = gradient(A[:,:,:,:,1], y, axis=1, acc=acc, edge_stencil=edge_stencil)
+                        A_ddz = gradient(A[:,:,:,:,2], z, axis=2, acc=acc, edge_stencil=edge_stencil)
+                        
+                        unsteady_diffusion = A_ddx + A_ddy + A_ddz
+                        
+                        t_delta = timeit.default_timer() - t_start
+                        if verbose:
+                            tqdm.write(even_print('calc diffusion', format_time_string(t_delta),s=True))
+                        
+                        self.comm.Barrier()
+                        
+                        ## combine sums across ranks for this [t] chunk
+                        unsteady_diffusion_sum_i   = np.sum(unsteady_diffusion, axis=3, keepdims=True, dtype=np.float64)
+                        unsteady_diffusion_sum_buf = np.zeros((nx,ny,nz,1), dtype=np.float64, order='C')
+                        self.comm.Reduce([unsteady_diffusion_sum_i, MPI.DOUBLE],
+                                         [unsteady_diffusion_sum_buf, MPI.DOUBLE],
+                                         op=MPI.SUM,
+                                         root=0)
+                        
+                        ## add aggregated sum (across ranks) to the total accumulator
+                        unsteady_diffusion_sum += unsteady_diffusion_sum_buf
+                        
+                        ## release mem
+                        omega_ij = None; del omega_ij
+                        A        = None; del A
+                        A_ddx    = None; del A_ddx
+                        A_ddy    = None; del A_ddy
+                        A_ddz    = None; del A_ddz
+                        unsteady_diffusion = None; del unsteady_diffusion
+                        
+                        self.comm.Barrier()
+                        mem_avail_gb = psutil.virtual_memory().available/1024**3
+                        mem_free_gb  = psutil.virtual_memory().free/1024**3
+                        if verbose:
+                            tqdm.write(even_print('mem available', '%0.1f [GB]'%mem_avail_gb, s=True))
+                            tqdm.write(even_print('mem free',      '%0.1f [GB]'%mem_free_gb,  s=True))
                     
-                    # === do avg
-                    t_start = timeit.default_timer()
-                    unsteady_p_diffusion_sum   = np.zeros((nx,ny,nz,1), dtype=np.float64, order='C')
-                    unsteady_p_diffusion_sum_i = np.sum(unsteady_p_diffusion, axis=3, keepdims=True, dtype=np.float64)
-                    self.comm.Reduce([unsteady_p_diffusion_sum_i, MPI.DOUBLE], [unsteady_p_diffusion_sum, MPI.DOUBLE], op=MPI.SUM, root=0)
-                    if (self.rank==0):
-                        p_diffusion = ( (1/nt)*unsteady_p_diffusion_sum ).astype(np.float32)
-                    t_delta = timeit.default_timer() - t_start
-                    if verbose:
-                        tqdm.write(even_print('t avg p_diffusion', format_time_string(t_delta),s=True))
+                    # === pressure diffusion
+                    if True:
+                        
+                        if verbose: tqdm.write(72*'-')
+                        t_start = timeit.default_timer()
+                        
+                        A = np.einsum('xyzti,xyzt->xyzti', uII_i, pI)
+                        
+                        #A_ddx = np.gradient(A[:,:,:,:,0], x, axis=0, edge_order=2)
+                        #A_ddy = np.gradient(A[:,:,:,:,1], y, axis=1, edge_order=2)
+                        #A_ddz = np.gradient(A[:,:,:,:,2], z, axis=2, edge_order=2)
+                        
+                        A_ddx = gradient(A[:,:,:,:,0], x, axis=0, acc=acc, edge_stencil=edge_stencil)
+                        A_ddy = gradient(A[:,:,:,:,1], y, axis=1, acc=acc, edge_stencil=edge_stencil)
+                        A_ddz = gradient(A[:,:,:,:,2], z, axis=2, acc=acc, edge_stencil=edge_stencil)
+                        
+                        unsteady_p_diffusion = A_ddx + A_ddy + A_ddz
+                        
+                        t_delta = timeit.default_timer() - t_start
+                        if verbose:
+                            tqdm.write(even_print('calc p_diffusion', format_time_string(t_delta),s=True))
+                        
+                        self.comm.Barrier()
+                        
+                        ## combine sums across ranks for this [t] chunk
+                        unsteady_p_diffusion_sum_i   = np.sum(unsteady_p_diffusion, axis=3, keepdims=True, dtype=np.float64)
+                        unsteady_p_diffusion_sum_buf = np.zeros((nx,ny,nz,1), dtype=np.float64, order='C')
+                        self.comm.Reduce([unsteady_p_diffusion_sum_i, MPI.DOUBLE],
+                                         [unsteady_p_diffusion_sum_buf, MPI.DOUBLE],
+                                         op=MPI.SUM,
+                                         root=0)
+                        
+                        ## add aggregated sum (across ranks) to the total accumulator
+                        unsteady_p_diffusion_sum += unsteady_p_diffusion_sum_buf
+                        
+                        # === release mem
+                        A        = None; del A
+                        A_ddx    = None; del A_ddx
+                        A_ddy    = None; del A_ddy
+                        A_ddz    = None; del A_ddz
+                        unsteady_p_diffusion = None; del unsteady_p_diffusion
+                        
+                        self.comm.Barrier()
+                        mem_avail_gb = psutil.virtual_memory().available/1024**3
+                        mem_free_gb  = psutil.virtual_memory().free/1024**3
+                        if verbose:
+                            tqdm.write(even_print('mem available', '%0.1f [GB]'%mem_avail_gb, s=True))
+                            tqdm.write(even_print('mem free',      '%0.1f [GB]'%mem_free_gb,  s=True))
                     
-                    # === write avg
-                    with rgd(fn_rgd_turb_budget_mean, 'a', driver='mpio', comm=self.comm, libver='latest') as f1:
-                        if (self.rank==0):
-                            f1['data/p_diffusion'][:,:,:,:] = p_diffusion.T
-                    self.comm.Barrier()
+                    # === pressure dilatation
+                    if True:
+                        
+                        if verbose: tqdm.write(72*'-')
+                        t_start = timeit.default_timer()
+                        
+                        # A = np.einsum('xyzt,xyzti->xyzti', pI, uII_i)
+                        # A_ddx = np.gradient(A[:,:,:,:,0], x, axis=0, edge_order=2)
+                        # A_ddy = np.gradient(A[:,:,:,:,1], y, axis=1, edge_order=2)
+                        # A_ddz = np.gradient(A[:,:,:,:,2], z, axis=2, edge_order=2)
+                        # unsteady_p_dilatation = A_ddx + A_ddy + A_ddz
+                        
+                        unsteady_p_dilatation = pI * ( duIIdx + dvIIdy + dwIIdz )
+                        
+                        t_delta = timeit.default_timer() - t_start
+                        if verbose:
+                            tqdm.write(even_print('calc p_dilatation', format_time_string(t_delta),s=True))
+                        
+                        self.comm.Barrier()
+                        
+                        ## combine sums across ranks for this [t] chunk
+                        unsteady_p_dilatation_sum_i   = np.sum(unsteady_p_dilatation, axis=3, keepdims=True, dtype=np.float64)
+                        unsteady_p_dilatation_sum_buf = np.zeros((nx,ny,nz,1), dtype=np.float64, order='C')
+                        self.comm.Reduce([unsteady_p_dilatation_sum_i, MPI.DOUBLE],
+                                         [unsteady_p_dilatation_sum_buf, MPI.DOUBLE],
+                                         op=MPI.SUM,
+                                         root=0)
+                        
+                        ## add aggregated sum (across ranks) to the total accumulator
+                        unsteady_p_dilatation_sum += unsteady_p_dilatation_sum_buf
+                        
+                        ## release mem
+                        unsteady_p_dilatation = None
+                        del unsteady_p_dilatation
+                        
+                        self.comm.Barrier()
+                        mem_avail_gb = psutil.virtual_memory().available/1024**3
+                        mem_free_gb  = psutil.virtual_memory().free/1024**3
+                        if verbose:
+                            tqdm.write(even_print('mem available', '%0.1f [GB]'%mem_avail_gb, s=True))
+                            tqdm.write(even_print('mem free',      '%0.1f [GB]'%mem_free_gb,  s=True))
                     
-                    # === write unsteady data
-                    if save_unsteady:
-                        with rgd(fn_rgd_turb_budget, 'a', driver='mpio', comm=self.comm, libver='latest') as f1:
-                            dset = f1['data/unsteady_p_diffusion']
-                            self.comm.Barrier()
-                            t_start = timeit.default_timer()
-                            with dset.collective:
-                                dset[rt1:rt2,:,:,:] = unsteady_p_diffusion.T
-                            t_delta = timeit.default_timer() - t_start
-                            data_gb = 4*nx*ny*nz*nt/1024**3
-                            if verbose:
-                                even_print('write: unsteady p diffusion', '%0.3f [GB]  %0.3f [s]  %0.3f [GB/s]'%(data_gb,t_delta,(data_gb/t_delta)))
+                    ## manual garbage collect
+                    #gc.collect()
+                    #self.comm.Barrier()
                     
-                    # === release mem
-                    A        = None; del A
-                    A_ddx    = None; del A_ddx
-                    A_ddy    = None; del A_ddy
-                    A_ddz    = None; del A_ddz
-                    unsteady_p_diffusion = None; del unsteady_p_diffusion
+                    if verbose: progress_bar.update()
                     
-                    self.comm.Barrier()
-                    mem_avail_gb = psutil.virtual_memory().available/1024**3
-                    mem_free_gb  = psutil.virtual_memory().free/1024**3
-                    if verbose:
-                        tqdm.write(even_print('mem available', '%0.1f [GB]'%mem_avail_gb, s=True))
-                        tqdm.write(even_print('mem free',      '%0.1f [GB]'%mem_free_gb,  s=True))
+                    if verbose: tqdm.write(72*'-')
                 
-                # === pressure dilatation
-                if True:
-                    
-                    if verbose: print(72*'-')
-                    t_start = timeit.default_timer()
-                    
-                    # A = np.einsum('xyzt,xyzti->xyzti', pI, uII_i)
-                    # A_ddx = np.gradient(A[:,:,:,:,0], x, axis=0, edge_order=2)
-                    # A_ddy = np.gradient(A[:,:,:,:,1], y, axis=1, edge_order=2)
-                    # A_ddz = np.gradient(A[:,:,:,:,2], z, axis=2, edge_order=2)
-                    # unsteady_p_dilatation = A_ddx + A_ddy + A_ddz
-                    
-                    unsteady_p_dilatation = pI * ( duIIdx + dvIIdy + dwIIdz )
-                    
-                    t_delta = timeit.default_timer() - t_start
-                    if verbose:
-                        tqdm.write(even_print('p_dilatation', format_time_string(t_delta),s=True))
-                    
-                    # === do avg
-                    t_start = timeit.default_timer()
-                    unsteady_p_dilatation_sum   = np.zeros((nx,ny,nz,1), dtype=np.float64, order='C')
-                    unsteady_p_dilatation_sum_i = np.sum(unsteady_p_dilatation, axis=3, keepdims=True, dtype=np.float64)
-                    self.comm.Reduce([unsteady_p_dilatation_sum_i, MPI.DOUBLE], [unsteady_p_dilatation_sum, MPI.DOUBLE], op=MPI.SUM, root=0)
-                    if (self.rank==0):
-                        p_dilatation = ( (1/nt)*unsteady_p_dilatation_sum ).astype(np.float32)
-                    t_delta = timeit.default_timer() - t_start
-                    if verbose:
-                        tqdm.write(even_print('t avg p_dilatation', format_time_string(t_delta),s=True))
-                    
-                    # === write avg
-                    with rgd(fn_rgd_turb_budget_mean, 'a', driver='mpio', comm=self.comm, libver='latest') as f1:
-                        if (self.rank==0):
-                            f1['data/p_dilatation'][:,:,:,:] = p_dilatation.T
-                    self.comm.Barrier()
-                    
-                    # === write unsteady data
-                    if save_unsteady:
-                        with rgd(fn_rgd_turb_budget, 'a', driver='mpio', comm=self.comm, libver='latest') as f1:
-                            dset = f1['data/unsteady_p_dilatation']
-                            self.comm.Barrier()
-                            t_start = timeit.default_timer()
-                            with dset.collective:
-                                dset[rt1:rt2,:,:,:] = unsteady_p_dilatation.T
-                            t_delta = timeit.default_timer() - t_start
-                            data_gb = 4*nx*ny*nz*nt/1024**3
-                            if verbose:
-                                even_print('write: unsteady p dilatation', '%0.3f [GB]  %0.3f [s]  %0.3f [GB/s]'%(data_gb,t_delta,(data_gb/t_delta)))
-                    
-                    # === release mem
-                    unsteady_p_dilatation = None; del unsteady_p_dilatation
-                    
-                    self.comm.Barrier()
-                    mem_avail_gb = psutil.virtual_memory().available/1024**3
-                    mem_free_gb  = psutil.virtual_memory().free/1024**3
-                    if verbose:
-                        tqdm.write(even_print('mem available', '%0.1f [GB]'%mem_avail_gb, s=True))
-                        tqdm.write(even_print('mem free',      '%0.1f [GB]'%mem_free_gb,  s=True))
-        
-        if verbose: print(72*'-')
-        
-        # === make .xdmf
-        
-        if save_unsteady:
-            with rgd(fn_rgd_turb_budget, 'r', driver='mpio', comm=self.comm, libver='latest') as f1:
-                f1.make_xdmf()
-        with rgd(fn_rgd_turb_budget_mean, 'r', driver='mpio', comm=self.comm, libver='latest') as f1:
-            f1.make_xdmf()
+                if verbose: progress_bar.close()
         
-        # ===
+        # === multiply accumulators by (1/n) to get [t] avg --> leave [x,y,z]
         
+        if (self.rank==0):
+            production   = np.copy( ((1/nt) * unsteady_production_sum   ) )
+            dissipation  = np.copy( ((1/nt) * unsteady_dissipation_sum  ) )
+            transport    = np.copy( ((1/nt) * unsteady_transport_sum    ) )
+            diffusion    = np.copy( ((1/nt) * unsteady_diffusion_sum    ) )
+            p_diffusion  = np.copy( ((1/nt) * unsteady_p_diffusion_sum  ) )
+            p_dilatation = np.copy( ((1/nt) * unsteady_p_dilatation_sum ) )
         self.comm.Barrier()
-        if verbose: print('\n'+72*'-')
-        if verbose: print('total time : rgd.calc_turb_budget() : %s'%format_time_string((timeit.default_timer() - t_start_func)))
-        if verbose: print(72*'-')
         
-        return
-    
-    def calc_high_order_stats(self,**kwargs):
-        '''
-        calculate skewness, kurtosis ('flatness'), probability distribution function (PDF)
-        '''
+        # === write to HDF5 --> [x,y,z,1]
         
+        #with rgd(fn_rgd_turb_budget, 'a', driver='mpio', comm=self.comm, libver='latest') as f1:
         if (self.rank==0):
-            verbose = True
-        else:
-            verbose = False
-        
-        if verbose: print('\n'+'rgd.calc_high_order_stats()'+'\n'+72*'-')
-        t_start_func = timeit.default_timer()
-        
-        rx = kwargs.get('rx',1)
-        ry = kwargs.get('ry',1)
-        rz = kwargs.get('rz',1)
-        rt = kwargs.get('rt',1)
-        
-        fn_dat_hos      = kwargs.get('fn_dat_hos',None) ## hos = 'high-order stats'
-        fn_dat_mean_dim = kwargs.get('fn_dat_mean_dim',None)
-        
-        ## for now only distribute data in [y] --> allows [x,z] mean before Send/Recv
-        if (rx!=1):
-            raise AssertionError('rx!=1')
-        if (rz!=1):
-            raise AssertionError('rz!=1')
-        if (rt!=1):
-            raise AssertionError('rt!=1')
-        
-        if (rx*ry*rz*rt != self.n_ranks):
-            raise AssertionError('rx*ry*rz*rt != self.n_ranks')
-        if (rx>self.nx):
-            raise AssertionError('rx>self.nx')
-        if (ry>self.ny):
-            raise AssertionError('ry>self.ny')
-        if (rz>self.nz):
-            raise AssertionError('rz>self.nz')
-        if (rt>self.nt):
-            raise AssertionError('rt>self.nt')
-        
-        # ===
-        
-        #comm4d = self.comm.Create_cart(dims=[rx,ry,ry,rt], periods=[False,False,False,False], reorder=False)
-        #t4d = comm4d.Get_coords(self.rank)
-        
-        #rxl_ = np.array_split(np.array(range(self.nx),dtype=np.int64),min(rx,self.nx))
-        ryl_ = np.array_split(np.array(range(self.ny),dtype=np.int64),min(ry,self.ny))
-        #rzl_ = np.array_split(np.array(range(self.nz),dtype=np.int64),min(rz,self.nz))
-        #rtl_ = np.array_split(np.array(range(self.nt),dtype=np.int64),min(rt,self.nt))
-
-        #rxl = [[b[0],b[-1]+1] for b in rxl_ ]
-        ryl = [[b[0],b[-1]+1] for b in ryl_ ]
-        #rzl = [[b[0],b[-1]+1] for b in rzl_ ]
-        #rtl = [[b[0],b[-1]+1] for b in rtl_ ]
-        
-        #rx1, rx2 = rxl[t4d[0]]; nxr = rx2 - rx1
-        #ry1, ry2 = ryl[t4d[1]]; nyr = ry2 - ry1
-        #rz1, rz2 = rzl[t4d[2]]; nzr = rz2 - rz1
-        #rt1, rt2 = rtl[t4d[3]]; ntr = rt2 - rt1
-        
-        ry1,ry2 = ryl[self.rank]; nyr = ry2 - ry1
-        
-        # === mean (dimensional) file name (for reading) : .dat
-        if (fn_dat_mean_dim is None):
-            fname_path = os.path.dirname(self.fname)
-            fname_base = os.path.basename(self.fname)
-            fname_root, fname_ext = os.path.splitext(fname_base)
-            fname_root = re.findall('io\S+_mpi_[0-9]+', fname_root)[0]
-            fname_dat_mean_base = fname_root+'_mean_dim.dat'
-            fn_dat_mean_dim = str(PurePosixPath(fname_path, fname_dat_mean_base))
-        
-        # === high-order stats ('hos') file name (for writing) : dat
-        if (fn_dat_hos is None):
-            fname_path = os.path.dirname(self.fname)
-            fname_base = os.path.basename(self.fname)
-            fname_root, fname_ext = os.path.splitext(fname_base)
-            fname_root = re.findall('io\S+_mpi_[0-9]+', fname_root)[0]
-            fname_hos_dat_base = fname_root+'_hos.dat'
-            fn_dat_hos = str(PurePosixPath(fname_path, fname_hos_dat_base))
-        
-        # ===
-        
-        if verbose: even_print('fn_rgd'     , self.fname )
-        if verbose: even_print('fn_dat_hos' , fn_dat_hos )
-        if verbose: print(72*'-')
-
-        if not os.path.isfile(fn_dat_mean_dim):
-            raise FileNotFoundError('%s not found!'%fn_dat_mean_dim)
-        
-        if True: ## open mean (dimensional) data
-            
-            with open(fn_dat_mean_dim,'rb') as f:
-                data_mean_dim = pickle.load(f)
-            fmd = type('foo', (object,), data_mean_dim)
-
-            self.comm.Barrier()
-            
-            ## the data dictionary to be pickled later
-            data = {}
-            
-            ## 2D dimensional quantities --> [x,z]
-            u_tau    = fmd.u_tau    # ; data['u_tau']    = u_tau
-            nu_wall  = fmd.nu_wall  # ; data['nu_wall']  = nu_wall
-            rho_wall = fmd.rho_wall # ; data['rho_wall'] = rho_wall
-            d99      = fmd.d99      # ; data['d99']      = d99
-            u99      = fmd.u99      # ; data['u99']      = u99
-            Re_tau   = fmd.Re_tau   # ; data['Re_tau']   = Re_tau
-            Re_theta = fmd.Re_theta # ; data['Re_theta'] = Re_theta
-            
-            ## mean [x,z] --> leave 0D scalar
-            u_tau_avg    = np.mean(fmd.u_tau    , axis=(0,1)) ; data['u_tau_avg']    = u_tau_avg
-            nu_wall_avg  = np.mean(fmd.nu_wall  , axis=(0,1)) ; data['nu_wall_avg']  = nu_wall_avg
-            rho_wall_avg = np.mean(fmd.rho_wall , axis=(0,1)) ; data['rho_wall_avg'] = rho_wall_avg
-            d99_avg      = np.mean(fmd.d99      , axis=(0,1)) ; data['d99_avg']      = d99_avg
-            u99_avg      = np.mean(fmd.u99      , axis=(0,1)) ; data['u99_avg']      = u99_avg
-            Re_tau_avg   = np.mean(fmd.Re_tau   , axis=(0,1)) ; data['Re_tau_avg']   = Re_tau_avg
-            Re_theta_avg = np.mean(fmd.Re_theta , axis=(0,1)) ; data['Re_theta_avg'] = Re_theta_avg
-            
-            ## mean [x,z] --> leave 1D [y]
-            rho_avg = np.mean(fmd.rho,axis=(0,2))
-            data['rho_avg'] = rho_avg
-            
-            # === 2D inner scales --> [x,z]
-            sc_l_in = nu_wall / u_tau
-            sc_u_in = u_tau
-            sc_t_in = nu_wall / u_tau**2
-            
-            # === 2D outer scales --> [x,z]
-            sc_l_out = d99
-            sc_u_out = u99
-            sc_t_out = d99/u99
-            
-            # === check
-            np.testing.assert_allclose(fmd.lchar   , self.lchar   , rtol=1e-8)
-            np.testing.assert_allclose(fmd.U_inf   , self.U_inf   , rtol=1e-8)
-            np.testing.assert_allclose(fmd.rho_inf , self.rho_inf , rtol=1e-8)
-            np.testing.assert_allclose(fmd.T_inf   , self.T_inf   , rtol=1e-8)
-            np.testing.assert_allclose(fmd.nx      , self.nx      , rtol=1e-8)
-            np.testing.assert_allclose(fmd.ny      , self.ny      , rtol=1e-8)
-            np.testing.assert_allclose(fmd.nz      , self.nz      , rtol=1e-8)
-            np.testing.assert_allclose(fmd.xs      , self.x       , rtol=1e-8)
-            np.testing.assert_allclose(fmd.ys      , self.y       , rtol=1e-8)
-            np.testing.assert_allclose(fmd.zs      , self.z       , rtol=1e-8)
-            
-            lchar   = self.lchar   ; data['lchar']   = lchar
-            U_inf   = self.U_inf   ; data['U_inf']   = U_inf
-            rho_inf = self.rho_inf ; data['rho_inf'] = rho_inf
-            T_inf   = self.T_inf   ; data['T_inf']   = T_inf
-            
-            data['Ma'] = self.Ma
-            data['Pr'] = self.Pr
-            
-            nx = self.nx ; data['nx'] = nx
-            ny = self.ny ; data['ny'] = ny
-            nz = self.nz ; data['nz'] = nz
-            nt = self.nt ; data['nt'] = nt
-
-            ## dimless (inlet)
-            xd = self.x
-            yd = self.y
-            zd = self.z
-            td = self.t
-            
-            ## dimensional [m] / [s]
-            x      = self.x * lchar
-            y      = self.y * lchar
-            z      = self.z * lchar
-            t      = self.t * (lchar/U_inf)
-            t_meas = t[-1]-t[0]
-            dt     = self.dt * (lchar/U_inf)
-            
-            data['x'] = x
-            data['y'] = y
-            data['z'] = z
-            data['t'] = t
-            data['t_meas'] = t_meas
-            data['dt'] = dt
-            
-            np.testing.assert_equal(nx,x.size)
-            np.testing.assert_equal(ny,y.size)
-            np.testing.assert_equal(nz,z.size)
-            np.testing.assert_equal(nt,t.size)
-            np.testing.assert_allclose(dt, t[1]-t[0], rtol=1e-8)
-            
-            # === report
-            if verbose:
-                even_print('nx'     , '%i'        %nx     )
-                even_print('ny'     , '%i'        %ny     )
-                even_print('nz'     , '%i'        %nz     )
-                even_print('nt'     , '%i'        %nt     )
-                even_print('dt'     , '%0.5e [s]' %dt     )
-                even_print('t_meas' , '%0.5e [s]' %t_meas )
-                print(72*'-')
-            
-            if verbose:
-                even_print('Re_τ'   , '%0.1f'         % Re_tau_avg   )
-                even_print('Re_θ'   , '%0.1f'         % Re_theta_avg )
-                even_print('δ99'    , '%0.5e [m]'     % d99_avg      )
-                even_print('U_inf'  , '%0.3f [m/s]'   % U_inf        )
-                even_print('u_τ'    , '%0.3f [m/s]'   % u_tau_avg    )
-                even_print('ν_wall' , '%0.5e [m²/s]'  % nu_wall_avg  )
-                even_print('ρ_wall' , '%0.6f [kg/m³]' % rho_wall_avg  )
-                print(72*'-')
-            
-            t_eddy = t_meas / ( d99_avg / u_tau_avg )
-            
-            if verbose:
-                even_print('t_meas/(δ99/u_τ) = t_eddy' , '%0.2f'%t_eddy)
-                even_print('t_meas/(δ99/u99)'          , '%0.2f'%(t_meas/(d99_avg/u99_avg)))
-                even_print('t_meas/(20·δ99/u99)'       , '%0.2f'%(t_meas/(20*d99_avg/u99_avg)))
-                print(72*'-')
-        
-        if True: ## read RGD data & dimensionalize
-            
-            scalars = [ 'u','T' ] ## 'v','w','p','rho'
-            scalars_dtypes = [self.scalars_dtypes_dict[s] for s in scalars]
-            
-            ## 5D [scalar][x,y,z,t] structured array
-            data_prime = np.zeros(shape=(self.nx, nyr, self.nz, self.nt), dtype={'names':scalars, 'formats':scalars_dtypes})
-            
-            for scalar in scalars:
-                dset = self['data/%s'%scalar]
-                self.comm.Barrier()
-                t_start = timeit.default_timer()
-                with dset.collective:
-                    data_prime[scalar] = dset[:,:,ry1:ry2,:].T
-                self.comm.Barrier()
-                t_delta = timeit.default_timer() - t_start
-                data_gb = 4 * self.nx * self.ny * self.nz * self.nt / 1024**3
-                if verbose:
-                    even_print('read: %s'%scalar, '%0.3f [GB]  %0.3f [s]  %0.3f [GB/s]'%(data_gb,t_delta,(data_gb/t_delta)))
-            
-            # === redimensionalize prime data
-            
-            for var in data_prime.dtype.names:
-                if var in ['u','v','w', 'uI','vI','wI', 'uII','vII','wII']:
-                    data_prime[var] *= U_inf
-                elif var in ['r_uII','r_vII','r_wII']:
-                    data_prime[var] *= (U_inf*rho_inf)
-                elif var in ['T','TI','TII']:
-                    data_prime[var] *= T_inf
-                elif var in ['r_TII']:
-                    data_prime[var] *= (T_inf*rho_inf)
-                elif var in ['rho','rhoI']:
-                    data_prime[var] *= rho_inf
-                elif var in ['p','pI','pII']:
-                    data_prime[var] *= (rho_inf * U_inf**2)
-                else:
-                    raise ValueError('condition needed for redimensionalizing \'%s\''%var)
-        
-        ## initialize buffers
-        hos_scalars = [ '%s_mean'%(s,)    for s in scalars ] + \
-                      [ '%sI_median'%(s,) for s in scalars ] + \
-                      [ '%s_std'%(s,)     for s in scalars ] + \
-                      [ '%s_skew'%(s,)    for s in scalars ] + \
-                      [ '%s_kurt'%(s,)    for s in scalars ]
-        
-        hos_scalars_dtypes = [ np.float64 for s in hos_scalars ]
-        #hos                = np.zeros(shape=(self.nx, nyr, self.nz) , dtype={'names':hos_scalars, 'formats':hos_scalars_dtypes})
-        hos                = np.zeros(shape=(nyr,) , dtype={'names':hos_scalars, 'formats':hos_scalars_dtypes})
-        
-        n_bins = 1000
-        
-        hist_scalars = [ '%s'%(s,) for s in scalars ]
-        hist_scalars_dtypes = [ np.float64 for s in hist_scalars ]
-        hist = np.zeros(shape=(nyr, n_bins) , dtype={'names':hist_scalars, 'formats':hist_scalars_dtypes})
-        
-        bins_scalars = [ '%s'%(s,) for s in scalars ]
-        bins_scalars_dtypes = [ np.float64 for s in bins_scalars ]
-        bins = np.zeros(shape=(nyr, n_bins+1) , dtype={'names':bins_scalars, 'formats':bins_scalars_dtypes})
-        
-        ## check memory
-        mem_total_gb = psutil.virtual_memory().total/1024**3
-        mem_avail_gb = psutil.virtual_memory().available/1024**3
-        mem_free_gb  = psutil.virtual_memory().free/1024**3
-        if verbose:
-            even_print('mem total',     '%0.1f [GB]'%(mem_total_gb,))
-            even_print('mem available', '%0.1f [GB] / %0.1f[%%]'%(mem_avail_gb,(100*mem_avail_gb/mem_total_gb)))
-            even_print('mem free',      '%0.1f [GB] / %0.1f[%%]'%(mem_free_gb,(100*mem_free_gb/mem_total_gb)))
-            print(72*'-')
-        
-        ## main loop
-        self.comm.Barrier()
-        #if verbose: progress_bar = tqdm(total=self.nx*nyr*self.nz, ncols=100, desc='high order stats', leave=False)
-        if verbose: progress_bar = tqdm(total=nyr, ncols=100, desc='high order stats', leave=False)
-        for yi in range(nyr):
-            for s in scalars:
-                
-                ## all [x,z,t] at this [y]
-                d        = np.copy( data_prime[s][:,yi,:,:] ).astype(np.float64).ravel()
-                d_mean   = np.mean( d , dtype=np.float64 )
-                
-                dI        = d - d_mean
-                dI_median = np.median( dI )
-                
-                hist_ , bin_edges_ = np.histogram( dI , bins=n_bins , density=True )
-                hist[s][yi,:] = hist_
-                bins[s][yi,:] = bin_edges_
-                
-                #d_var  = np.mean( dI**2 ) ## = d.std()**2
-                d_std  = np.sqrt( np.mean( dI**2 , dtype=np.float64 ) ) ## = d.std()
-                
-                if np.isclose(d_std, 0., atol=1e-08):
-                    d_skew = 0.
-                    d_kurt = 0.
-                else:
-                    d_skew = np.mean( dI**3 , dtype=np.float64 ) / d_std**3
-                    d_kurt = np.mean( dI**4 , dtype=np.float64 ) / d_std**4 ## = sp.stats.kurtosis(d,fisher=False)
-                
-                hos['%sI_median'%s][yi] = dI_median
-                hos['%s_mean'%s][yi]    = d_mean
-                hos['%s_std'%s][yi]     = d_std
-                hos['%s_skew'%s][yi]    = d_skew
-                hos['%s_kurt'%s][yi]    = d_kurt
-                
-                if verbose: progress_bar.update()
-        if verbose:
-            progress_bar.close()
+            with rgd(fn_rgd_turb_budget, 'a') as f1:
+                f1['data/production'][:,:,:,:]   = production.T.astype(np.float32)
+                f1['data/dissipation'][:,:,:,:]  = dissipation.T.astype(np.float32)
+                f1['data/transport'][:,:,:,:]    = transport.T.astype(np.float32)
+                f1['data/diffusion'][:,:,:,:]    = diffusion.T.astype(np.float32)
+                f1['data/p_diffusion'][:,:,:,:]  = p_diffusion.T.astype(np.float32)
+                f1['data/p_dilatation'][:,:,:,:] = p_dilatation.T.astype(np.float32)
         self.comm.Barrier()
         
-        # === average in [x,z], leave [y] --> not needed if stats are calculated over [x,z,t] per [y]
-        
-        ## hos_ = np.zeros(shape=(nyr,) , dtype={'names':hos_scalars, 'formats':hos_scalars_dtypes})
-        ## for tag in hos_scalars:
-        ##     hos_[tag] = np.mean( hos[tag] , axis=(0,2) , dtype=np.float64 )
-        ## hos = np.copy( hos_ )
-        ## self.comm.Barrier()
-        
-        # === gather
-        
-        G = self.comm.gather([ self.rank, hos, hist, bins ], root=0)
-        G = self.comm.bcast(G, root=0)
-        
-        hos  = np.zeros( (ny,)         , dtype={'names':hos_scalars  , 'formats':hos_scalars_dtypes}  )
-        hist = np.zeros( (ny,n_bins)   , dtype={'names':hist_scalars , 'formats':hist_scalars_dtypes} )
-        bins = np.zeros( (ny,n_bins+1) , dtype={'names':bins_scalars , 'formats':bins_scalars_dtypes} )
-        
-        for ri in range(self.n_ranks):
-            j = ri
-            for GG in G:
-                if (GG[0]==ri):
-                    for tag in hos_scalars:
-                        hos[tag][ryl[j][0]:ryl[j][1],] = GG[1][tag]
-                    for tag in hist_scalars:
-                        hist[tag][ryl[j][0]:ryl[j][1],:] = GG[2][tag]
-                    for tag in bins_scalars:
-                        bins[tag][ryl[j][0]:ryl[j][1],:] = GG[3][tag]
-                else:
-                    pass
+        # === write to .dat --> pre-average in [x,y], leaving [y]
         
-        # === save results
         if (self.rank==0):
             
-            data['hos']  = hos
-            data['hist'] = hist
-            data['bins'] = bins
-            
-            sc_l_in  = np.mean(sc_l_in  , axis=(0,1) , dtype=np.float64).astype(np.float32) ## avg in [x,z] --> leave 0D scalar
-            sc_u_in  = np.mean(sc_u_in  , axis=(0,1) , dtype=np.float64).astype(np.float32)
-            sc_t_in  = np.mean(sc_t_in  , axis=(0,1) , dtype=np.float64).astype(np.float32)
-            sc_l_out = np.mean(sc_l_out , axis=(0,1) , dtype=np.float64).astype(np.float32)
-            sc_u_out = np.mean(sc_u_out , axis=(0,1) , dtype=np.float64).astype(np.float32)
-            sc_t_out = np.mean(sc_t_out , axis=(0,1) , dtype=np.float64).astype(np.float32)
-            
-            data['sc_l_in']  = sc_l_in
-            data['sc_l_out'] = sc_l_out
-            data['sc_t_in']  = sc_t_in
-            data['sc_t_out'] = sc_t_out
-            data['sc_u_in']  = sc_u_in
-            data['sc_u_out'] = sc_u_out
-            
-            with open(fn_dat_hos,'wb') as f:
-                pickle.dump(data, f, protocol=4)
-            print('--w-> %s : %0.2f [MB]'%(fn_dat_hos,os.path.getsize(fn_dat_hos)/1024**2))
+            ## avg in [x,z] --> leave [y]
+            data['production']   = np.copy( np.squeeze( np.mean( production   , axis=(0,2) , dtype=np.float64 ) ) )
+            data['dissipation']  = np.copy( np.squeeze( np.mean( dissipation  , axis=(0,2) , dtype=np.float64 ) ) )
+            data['transport']    = np.copy( np.squeeze( np.mean( transport    , axis=(0,2) , dtype=np.float64 ) ) )
+            data['diffusion']    = np.copy( np.squeeze( np.mean( diffusion    , axis=(0,2) , dtype=np.float64 ) ) )
+            data['p_diffusion']  = np.copy( np.squeeze( np.mean( p_diffusion  , axis=(0,2) , dtype=np.float64 ) ) )
+            data['p_dilatation'] = np.copy( np.squeeze( np.mean( p_dilatation , axis=(0,2) , dtype=np.float64 ) ) )
+            
+            with open(fn_dat_turb_budget,'wb') as f1:
+                pickle.dump(data, f1, protocol=4)
+            print('--w-> %s : %0.2f [MB]'%(fn_dat_turb_budget,os.path.getsize(fn_dat_turb_budget)/1024**2))
+        self.comm.Barrier()
         
         # ===
         
-        self.comm.Barrier()
-        
-        if verbose: print('\n'+72*'-')
-        if verbose: print('total time : rgd.calc_high_order_stats() : %s'%format_time_string((timeit.default_timer() - t_start_func)))
         if verbose: print(72*'-')
+        if verbose: print('total time : rgd.calc_turb_budget() : %s'%format_time_string((timeit.default_timer() - t_start_func)))
+        if verbose: print(72*'-')
+        
+        ## make .xdmf
+        with rgd(fn_rgd_turb_budget, 'r', driver='mpio', comm=self.comm, libver='latest') as f1:
+            f1.make_xdmf()
         
         return
     
-    # === Eulerian to Lagrangian transform --> 'converts' RGD to LPD
+    # === time integration / particle tracking : generate LPD
     
     def time_integrate(self, **kwargs):
         '''
         do Lagrangian-frame time integration of [u,v,w] field
         -----
         --> output LPD (Lagrangian Particle Data) file / lpd() instance
         '''
@@ -15216,29 +15782,32 @@
             
             ## 'self' passed here is RGD / h5py.File instance
             ## this copies over all the header info from the RGD: U_inf, lchar, etc
             hf_lpd.init_from_rgd(self, t_info=False)
             
             ## shape & HDF5 chunk scheme for datasets
             shape = (npts_all_ts, ntc-1)
-            chunks = rgd.chunk_sizer(nxi=shape, constraint=(None,1), size_kb=chunk_kb, base=2)
             
             scalars = [ 'x','y','z', 
                         'u','v','w', 
                         't','id'     ]
             
             scalars_dtype = [ np.float64, np.float64, np.float64, 
                               np.float32, np.float32, np.float32, 
                               np.float64, np.int64                 ]
             
             for si in range(len(scalars)):
                 
                 scalar       = scalars[si]
                 scalar_dtype = scalars_dtype[si]
                 
+                itemsize = np.dtype(scalar_dtype).itemsize
+                
+                chunks = h5_chunk_sizer(nxi=shape, constraint=(None,1), size_kb=chunk_kb, base=2, itemsize=itemsize)
+                
                 if verbose:
                     even_print('initializing',scalar)
                 
                 if ('data/%s'%scalar in hf_lpd):
                     del hf_lpd['data/%s'%scalar]
                 dset = hf_lpd.create_dataset('data/%s'%scalar, 
                                           shape=shape, 
@@ -16085,17 +16654,17 @@
         self.fname_root, self.fname_ext = os.path.splitext(self.fname_base)
         
         ## default to libver='latest' if none provided
         if ('libver' not in kwargs):
             kwargs['libver'] = 'latest'
         
         if (openMode!='r'):
-            raise ValueError('turbx.eas4(): opening EAS4 in anything but read mode \'r\' is discouraged!')
+            raise ValueError('turbx.eas4(): opening EAS4 in anything but read mode \'r\' is not allowed!')
         
-        ## catch possible user error
+        ## catch possible user error --> user tries to open non-EAS4 with turbx.eas4()
         if (self.fname_ext!='.eas'):
             raise ValueError('turbx.eas4() should not be used to open non-EAS4 files')
         
         ## determine if using mpi
         if ('driver' in kwargs) and (kwargs['driver']=='mpio'):
             self.usingmpi = True
         else:
@@ -20388,15 +20957,15 @@
         cpl_ = np.array_split(np.arange(rp1, rp2, dtype=np.int64), n_chunks )
         cpl  = [[b[0],b[-1]+1] for b in cpl_ ]
         
         # === initialize (new) datasets
         
         ## shape & HDF5 chunk scheme for datasets
         shape = (self.npts, self.nt)
-        chunks = rgd.chunk_sizer(nxi=shape, constraint=(None,1), size_kb=chunk_kb, base=2)
+        chunks = h5_chunk_sizer(nxi=shape, constraint=(None,1), size_kb=chunk_kb, base=4, itemsize=4)
         
         scalars_in         = ['u','v','w','t','id']
         scalars_in_dtypes  = [self.scalars_dtypes_dict[s] for s in scalars_in]
         
         scalars_out        = ['ax','ay','az', 'jx','jy','jz']
         scalars_out_dtypes = [np.float32 for i in scalars_out]
         
@@ -20823,15 +21392,21 @@
             self.n_ranks = self.comm.Get_size()
             self.rank    = self.comm.Get_rank()
         else:
             self.comm    = None
             self.n_ranks = 1
             self.rank    = 0
         
-        ## determine MPI info / hints
+        ## if not using MPI, remove 'driver' and 'comm' from kwargs
+        if ( not self.usingmpi ) and ('driver' in kwargs):
+            kwargs.pop('driver')
+        if ( not self.usingmpi ) and ('comm' in kwargs):
+            kwargs.pop('comm')
+        
+        ## set ROMIO hints, passed through 'mpi_info' dict
         if self.usingmpi:
             if ('info' in kwargs):
                 self.mpi_info = kwargs['info']
             else:
                 mpi_info = MPI.Info.Create()
                 ##
                 mpi_info.Set('romio_ds_write' , 'disable'   )
@@ -20844,65 +21419,60 @@
                 ##
                 kwargs['info'] = mpi_info
                 self.mpi_info = mpi_info
         
         if ('rdcc_nbytes' not in kwargs):
             kwargs['rdcc_nbytes'] = int(16*1024**2) ## 16 [MB]
         
-        ## ztmd() unique kwargs (not h5py.File kwargs) --> pop() rather than get()
+        ## spd() unique kwargs (not h5py.File kwargs) --> pop() rather than get()
         verbose = kwargs.pop('verbose',False)
         force   = kwargs.pop('force',False)
         
+        # === initialize file on FS
+        
+        ## if file open mode is 'w', the file exists, and force is False
+        ## --> raise error
         if (self.open_mode == 'w') and (force is False) and os.path.isfile(self.fname):
             if (self.rank==0):
                 print('\n'+72*'-')
                 print(self.fname+' already exists! opening with \'w\' would overwrite.\n')
                 openModeInfoStr = '''
                                   r       --> Read only, file must exist
                                   r+      --> Read/write, file must exist
                                   w       --> Create file, truncate if exists
                                   w- or x --> Create file, fail if exists
                                   a       --> Read/write if exists, create otherwise
                                   
                                   or use force=True arg:
                                   
-                                  >>> with ztmd(<<fname>>,'w',force=True) as f:
+                                  >>> with spd(<<fname>>,'w',force=True) as f:
                                   >>>     ...
                                   '''
                 print(textwrap.indent(textwrap.dedent(openModeInfoStr), 2*' ').strip('\n'))
                 print(72*'-'+'\n')
             
             if (self.comm is not None):
                 self.comm.Barrier()
             raise FileExistsError()
         
-        ## remove file, touch, stripe
-        elif (self.open_mode == 'w') and (force is True) and os.path.isfile(self.fname):
+        ## if file open mode is 'w', the file exists, and force is True
+        ## --> delete, touch, chmod, stripe
+        if (self.open_mode == 'w') and (force is True) and os.path.isfile(self.fname):
             if (self.rank==0):
                 os.remove(self.fname)
                 Path(self.fname).touch()
+                os.chmod(self.fname, int('640', base=8))
                 if shutil.which('lfs') is not None:
-                    return_code = subprocess.call('lfs migrate --stripe-count 16 --stripe-size 16M %s > /dev/null 2>&1'%self.fname, shell=True)
+                    return_code = subprocess.call(f'lfs migrate --stripe-count 16 --stripe-size 16M {self.fname} > /dev/null 2>&1', shell=True)
+                    if (return_code != 0):
+                        raise ValueError('lfs migrate failed')
                 else:
                     #print('striping with lfs not permitted on this filesystem')
                     pass
         
-        ## touch, stripe
-        elif (self.open_mode == 'w') and not os.path.isfile(self.fname):
-            if (self.rank==0):
-                Path(self.fname).touch()
-                if shutil.which('lfs') is not None:
-                    return_code = subprocess.call('lfs migrate --stripe-count 16 --stripe-size 16M %s > /dev/null 2>&1'%self.fname, shell=True)
-                else:
-                    #print('striping with lfs not permitted on this filesystem')
-                    pass
-        
-        else:
-            pass
-        
         if (self.comm is not None):
             self.comm.Barrier()
         
         self.mod_avail_tqdm = ('tqdm' in sys.modules)
         
         ## call actual h5py.File.__init__()
         super(spd, self).__init__(*args, **kwargs)
@@ -21334,15 +21904,15 @@
         dsn = 'dims_unstruct/quads'
         if (dsn in self):
             del self[dsn]
         
         shape = quads.shape
         dtype = quads.dtype
         itemsize = quads.dtype.itemsize
-        chunks = rgd.chunk_sizer(nxi=shape, constraint=(None,None), size_kb=chunk_kb, base=2, data_byte=itemsize)
+        chunks = h5_chunk_sizer(nxi=shape, constraint=(None,None), size_kb=chunk_kb, base=4, itemsize=itemsize)
         ds = self.create_dataset(dsn,
                                  shape=shape,
                                  chunks=chunks,
                                  dtype=dtype )
         
         chunk_kb_ = np.prod(ds.chunks)*itemsize / 1024. ## actual
         if verbose:
@@ -21365,15 +21935,15 @@
         dsn = 'dims_unstruct/pts'
         if (dsn in self):
             del self[dsn]
         
         shape = pts.shape
         dtype = pts.dtype
         itemsize = pts.dtype.itemsize
-        chunks = rgd.chunk_sizer(nxi=shape, constraint=(None,None), size_kb=chunk_kb, base=2, data_byte=itemsize)
+        chunks = h5_chunk_sizer(nxi=shape, constraint=(None,None), size_kb=chunk_kb, base=4, itemsize=itemsize)
         ds = self.create_dataset(dsn,
                                  shape=shape,
                                  chunks=chunks,
                                  dtype=dtype )
         
         chunk_kb_ = np.prod(ds.chunks)*itemsize / 1024. ## actual
         if verbose:
@@ -21395,15 +21965,15 @@
             
             dsn = f'data/{scalar}'
             dtype = self[dsn].dtype
             itemsize = pts.dtype.itemsize
             
             ## initialize data_unstruct/<scalar> datasets
             shape = (ni*nj,nt)
-            chunks = rgd.chunk_sizer(nxi=shape, constraint=(None,1), size_kb=chunk_kb, base=2, data_byte=itemsize)
+            chunks = h5_chunk_sizer(nxi=shape, constraint=(None,1), size_kb=chunk_kb, base=4, itemsize=itemsize)
             
             dsn = f'data_unstruct/{scalar}'
             if (dsn in self):
                 del self[dsn]
             
             ds = self.create_dataset(dsn,
                                      shape=shape,
@@ -21612,15 +22182,15 @@
                 dsn = f'dims/xyz'
                 dset = hf_src[dsn]
                 dtype = dset.dtype
                 float_bytes = dtype.itemsize
                 with dset.collective:
                     xyz = np.copy( dset[ri1:ri2,rj1:rj2,:] )
                 shape  = (ni,nj,3)
-                chunks = rgd.chunk_sizer(nxi=shape, constraint=(None,None,3), size_kb=chunk_kb, base=2, data_byte=float_bytes)
+                chunks = h5_chunk_sizer(nxi=shape, constraint=(None,None,3), size_kb=chunk_kb, base=4, itemsize=float_bytes)
                 data_gb = float_bytes * ni * nj / 1024**3
                 if verbose:
                     even_print(f'initializing {dsn}','%0.1f [GB]'%(data_gb,))
                 dset = hf_tgt.create_dataset(dsn, dtype=xyz.dtype, shape=shape, chunks=chunks)
                 chunk_kb_ = np.prod(dset.chunks)*float_bytes / 1024. ## actual
                 if verbose:
                     even_print('chunk shape (i,j,3)',str(dset.chunks))
@@ -21665,15 +22235,15 @@
                     dsn = f'data/{scalar}'
                     ds = hf_src[dsn]
                     dtype = ds.dtype
                     float_bytes = dtype.itemsize
                     
                     data_gb = ni * nj * nt * float_bytes / 1024**3
                     shape   = (ni,nj,nt)
-                    chunks  = rgd.chunk_sizer(nxi=shape, constraint=(None,None,1), size_kb=chunk_kb, base=2, data_byte=float_bytes)
+                    chunks  = h5_chunk_sizer(nxi=shape, constraint=(None,None,1), size_kb=chunk_kb, base=4, itemsize=float_bytes)
                     
                     if verbose:
                         even_print(f'initializing data/{scalar}','%0.1f [GB]'%(data_gb,))
                     if (dsn in hf_tgt):
                         del hf_tgt[dsn]
                     dset = hf_tgt.create_dataset(dsn,
                                                  shape=shape,
@@ -21937,14 +22507,105 @@
         if verbose: print('--w-> %s'%fname_xdmf_base)
         
         return
 
 # meta HDF5 & h5py
 # ======================================================================
 
+def h5_chunk_sizer(nxi, **kwargs):
+    '''
+    solve for HDF5 dataset chunk size
+    -----
+    nxi --> an iterable (tuple,list,etc.) containing the target shape of the full HDF5 dataset
+    constraint --> an iterable with arguments <int> , None , 'full'/-1
+    -----
+    constraint = (1,None,None,None) ## [t] convention
+    constraint = (None,-1,1,-1) ## [y] convention
+    '''
+    
+    size_kb    = kwargs.get('size_kb'    , 2*1024 ) ## target chunk size in [KB] --> default = 2 [MB]
+    itemsize   = kwargs.get('itemsize'   , 4      ) ## dtype.itemsize --> default single precision i.e. 4 [B]
+    constraint = kwargs.get('constraint' , None   ) ## iterable of nxi constraints --> int,None,'full'/-1
+    base       = kwargs.get('base'       , 2      ) ## axis chunk size = ceil[size/(<int>*base)] where <int> is incremented
+    
+    ## check inputs
+    if not hasattr(nxi, '__iter__'):
+        raise AssertionError('\'nxi\' must be an iterable')
+    if constraint is None:
+        constraint = [ None for i in range(len(nxi)) ]
+    if not hasattr(constraint, '__iter__'):
+        raise AssertionError('\'constraint\' must be an iterable')
+    if not (len(nxi)==len(constraint)):
+        raise ValueError('nxi and constraint must have same size')
+    if not isinstance(base, int):
+        raise TypeError('\'base\' must be type int')
+    
+    if True: ## increment divisor on largest axis, with divisor=<int>*base
+        
+        nxi_ = [ n for n in nxi ] ## copy the input shape
+        div = [ 1 for i in range(len(nxi)) ] ## divisor vector, initialize with int ones
+        i_flexible = [ i for i in range(len(nxi)) if constraint[i] is None ] ## list of axes indices which are 'flexible'
+        
+        while True:
+            
+            #div_last = div ## no! pointer, not a copy
+            div_last = [ div[i] for i in range(len(nxi)) ]
+            
+            chunks = []
+            for i in range(len(nxi)):
+                if (constraint[i] is None): ## axis is 'flexible', so divide by divisor
+                    cas = max( int(round(nxi_[i]/div[i])) , 1 ) ## chunk axis shape is solved for
+                elif (constraint[i] == 'full') or (constraint[i] == -1):
+                    cas = nxi_[i] ## chunk axis shape is == dset axis shape
+                else:
+                    
+                    ## this axis is neither 'flexible' nor 'full', so
+                    ## assert that the constraint is a positive integer
+                    if not isinstance(constraint[i], int):
+                        raise ValueError('constraint[%i]=%s is not type int'%(i,str(constraint[i])))
+                    if not (constraint[i]>0):
+                        raise ValueError('constraint[%i]=%i is not >0'%(i,constraint[i]))
+                    
+                    cas = constraint[i] ## chunk axis shape is just the constraint
+                
+                chunks.append(cas)
+            
+            ## there are no flexible axes --> exit loop
+            if len(i_flexible)==0:
+                break
+            
+            ## the current size of a chunk, given 
+            chunk_size_kb = np.prod(chunks)*itemsize / 1024.
+            # print('chunk size %0.1f [KB]'%chunk_size_kb)
+            
+            if ( chunk_size_kb <= size_kb ): ## if chunk size is < target, then break
+                break
+            else: ## otherwise, increase the divisor of the greatest 'flexible' axis
+                
+                ## get index of (flexible) axis with greatest size
+                aa = [ i for i, j in enumerate(chunks) if (constraint[i] is None) ]
+                bb = [ j for i, j in enumerate(chunks) if (constraint[i] is None) ]
+                i_gt = aa[np.argmax(bb)]
+                
+                ## get new divisor
+                if (div[i_gt]==1) and (base!=1):
+                    div[i_gt] = 0
+                div[i_gt] += base
+            
+            # print(f'div = {str(tuple(div))}')
+            # print(f'div_last = {str(tuple(div_last))}')
+            # print(f'chunks = {str(tuple(chunks))}')
+            # print('---')
+            
+            ## check if in infinite loop (divisor not being updated)
+            if (div_last is not None) and (div == div_last):
+                raise ValueError('invalid parameters for h5_chunk_sizer() : constraint=%s, size_kb=%i, base=%i'%(str(constraint),size_kb,base))
+    
+    return tuple(chunks)
+
 def h5_visititems_print_attrs(name, obj):
     '''
     callable for input to h5py.Group.visititems() to print names & attributes
     '''
     n_slashes = name.count('/')
     shift = n_slashes*2*' '
     item_name = name.split('/')[-1]
@@ -22872,18 +23533,18 @@
         raise ValueError
     if (y_edge<y.min()):
         raise ValueError
     
     ny = y.shape[0]
     
     rho_edge_ = sp.interpolate.interp1d(y, rho, kind='cubic', bounds_error=True)(y_edge)
-    np.testing.assert_allclose(rho_edge, rho_edge_, rtol=1e-7)
+    np.testing.assert_allclose(rho_edge, rho_edge_, rtol=1e-5)
     
     u_edge_ = sp.interpolate.interp1d(y, u, kind='cubic', bounds_error=True)(y_edge)
-    np.testing.assert_allclose(u_edge, u_edge_, rtol=1e-7)
+    np.testing.assert_allclose(u_edge, u_edge_, rtol=1e-5)
     
     # ===
     
     integrand_theta_cmp = (u*rho)/(u_edge*rho_edge)*(1-(u/u_edge))
     integrand_dstar_cmp = (1-((u*rho)/(u_edge*rho_edge)))
     
     theta_cmp_     = sp.integrate.cumulative_trapezoid(y=integrand_theta_cmp, x=y, initial=0.)
```

### Comparing `turbx-0.2.3/turbx.egg-info/PKG-INFO` & `turbx-0.3.0/turbx.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turbx
-Version: 0.2.3
+Version: 0.3.0
 Summary: Extensible toolkit for analyzing turbulent flow datasets
 Home-page: https://github.com/iagappel/turbx
 Author: Jason A
 Maintainer: Jason A
 License: MIT
 Keywords: scientific computing,statistics,simulation,turbulence,turbulent flows,direct numerical simulation,DNS,parallel,visualization
 Platform: any
```

