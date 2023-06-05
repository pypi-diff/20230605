# Comparing `tmp/vasp_suite-1.1.3.tar.gz` & `tmp/vasp_suite-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vasp_suite-1.1.3.tar", last modified: Wed May 24 10:25:33 2023, max compression
+gzip compressed data, was "vasp_suite-1.2.0.tar", last modified: Mon Jun  5 12:34:49 2023, max compression
```

## Comparing `vasp_suite-1.1.3.tar` & `vasp_suite-1.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 10:25:33.230555 vasp_suite-1.1.3/
--rw-rw-rw-   0 root         (0) root         (0)    35079 2023-05-24 10:25:20.000000 vasp_suite-1.1.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3381 2023-05-24 10:25:33.229555 vasp_suite-1.1.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2933 2023-05-24 10:25:20.000000 vasp_suite-1.1.3/README.md
--rw-rw-rw-   0 root         (0) root         (0)      174 2023-05-24 10:25:20.000000 vasp_suite-1.1.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-24 10:25:33.230555 vasp_suite-1.1.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1371 2023-05-24 10:25:30.000000 vasp_suite-1.1.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 10:25:33.228555 vasp_suite-1.1.3/vasp_suite/
--rw-rw-rw-   0 root         (0) root         (0)      119 2023-05-24 10:25:20.000000 vasp_suite-1.1.3/vasp_suite/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      105 2023-05-24 10:25:30.000000 vasp_suite-1.1.3/vasp_suite/__version__.py
--rw-rw-rw-   0 root         (0) root         (0)    10765 2023-05-24 10:25:20.000000 vasp_suite-1.1.3/vasp_suite/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     3470 2023-05-24 10:25:20.000000 vasp_suite-1.1.3/vasp_suite/core.py
--rw-rw-rw-   0 root         (0) root         (0)    16932 2023-05-24 10:25:20.000000 vasp_suite-1.1.3/vasp_suite/ewald.py
--rw-rw-rw-   0 root         (0) root         (0)     2922 2023-05-24 10:25:20.000000 vasp_suite-1.1.3/vasp_suite/input.py
--rw-rw-rw-   0 root         (0) root         (0)    16913 2023-05-24 10:25:20.000000 vasp_suite-1.1.3/vasp_suite/structure.py
--rw-rw-rw-   0 root         (0) root         (0)     1711 2023-05-24 10:25:20.000000 vasp_suite-1.1.3/vasp_suite/submission.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 10:25:33.229555 vasp_suite-1.1.3/vasp_suite.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3381 2023-05-24 10:25:33.000000 vasp_suite-1.1.3/vasp_suite.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      422 2023-05-24 10:25:33.000000 vasp_suite-1.1.3/vasp_suite.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 10:25:33.000000 vasp_suite-1.1.3/vasp_suite.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2023-05-24 10:25:33.000000 vasp_suite-1.1.3/vasp_suite.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-24 10:25:33.000000 vasp_suite-1.1.3/vasp_suite.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-05-24 10:25:33.000000 vasp_suite-1.1.3/vasp_suite.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:34:49.911475 vasp_suite-1.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)    35079 2023-06-05 12:34:36.000000 vasp_suite-1.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3381 2023-06-05 12:34:49.911475 vasp_suite-1.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2933 2023-06-05 12:34:36.000000 vasp_suite-1.2.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      174 2023-06-05 12:34:36.000000 vasp_suite-1.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-05 12:34:49.911475 vasp_suite-1.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1371 2023-06-05 12:34:47.000000 vasp_suite-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:34:49.909475 vasp_suite-1.2.0/vasp_suite/
+-rw-rw-rw-   0 root         (0) root         (0)      119 2023-06-05 12:34:36.000000 vasp_suite-1.2.0/vasp_suite/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      105 2023-06-05 12:34:47.000000 vasp_suite-1.2.0/vasp_suite/__version__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16162 2023-06-05 12:34:36.000000 vasp_suite-1.2.0/vasp_suite/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     4855 2023-06-05 12:34:36.000000 vasp_suite-1.2.0/vasp_suite/core.py
+-rwxrwxrwx   0 root         (0) root         (0)    17643 2023-06-05 12:34:36.000000 vasp_suite-1.2.0/vasp_suite/ewald.py
+-rw-rw-rw-   0 root         (0) root         (0)     2936 2023-06-05 12:34:36.000000 vasp_suite-1.2.0/vasp_suite/input.py
+-rw-rw-rw-   0 root         (0) root         (0)    20176 2023-06-05 12:34:36.000000 vasp_suite-1.2.0/vasp_suite/structure.py
+-rw-rw-rw-   0 root         (0) root         (0)     1711 2023-06-05 12:34:36.000000 vasp_suite-1.2.0/vasp_suite/submission.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:34:49.910475 vasp_suite-1.2.0/vasp_suite.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3381 2023-06-05 12:34:49.000000 vasp_suite-1.2.0/vasp_suite.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      422 2023-06-05 12:34:49.000000 vasp_suite-1.2.0/vasp_suite.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 12:34:49.000000 vasp_suite-1.2.0/vasp_suite.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2023-06-05 12:34:49.000000 vasp_suite-1.2.0/vasp_suite.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-05 12:34:49.000000 vasp_suite-1.2.0/vasp_suite.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-06-05 12:34:49.000000 vasp_suite-1.2.0/vasp_suite.egg-info/top_level.txt
```

### Comparing `vasp_suite-1.1.3/LICENSE` & `vasp_suite-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.1.3/PKG-INFO` & `vasp_suite-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vasp_suite
-Version: 1.1.3
+Version: 1.2.0
 Summary: A package for creating and handling input files for vasp
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `vasp_suite-1.1.3/README.md` & `vasp_suite-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.1.3/setup.py` & `vasp_suite-1.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #! /usr/bin/env python3
 # -*- coding: utf-8 -*-
 # pylint: disable=line-too-long,missing-module-docstring,exec-used
 import setuptools
 
 # DO NOT EDIT THIS NUMBER!
 # It is changed automatically by python-semantic-release
-__version__ = "1.1.3"
+__version__ = "1.2.0"
 
 with open('README.md', 'r') as file:
     long_description = file.read()
 
 setuptools.setup(
     name='vasp_suite',
     version=__version__,
```

### Comparing `vasp_suite-1.1.3/vasp_suite/core.py` & `vasp_suite-1.2.0/vasp_suite/core.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 # Imports 
 import numpy as np 
 import os
 from . import structure 
 from . import input 
 from . import submission
+from . import ewald
 
 # Functions 
 
 def generate_input(filename: str, calculation: str) -> None:
     '''
     Generates Input files for VASP Calculations.
     '''
@@ -83,14 +84,70 @@
 def generate_kpoints(mesh: list) -> None:
     with open('KPOINTS', 'w') as f:
         f.write(f'''Regular {mesh[0]} {mesh[1]} {mesh[2]} gamma centred mesh \n''')
         f.write('0\nGamma\n')
         f.write(f'{mesh[0]} {mesh[1]} {mesh[2]}\n')
         f.write('0 0 0')
 
+def convert_cif(filename: str) -> None:
+    '''
+    Converts a cif file to a POSCAR file.
+    '''
+    _s = structure.Structure(filename)
+    _s.CIF_reader()
+    _s.write_poscar()
+
+def qm_region(filename: str, atom: str):
+    '''
+    Generates a qm region for a non-molecular crystal
+    '''
+    _s = structure.Structure(filename)
+    _s.Vasp_reader()
+    _s._find_index(atom)
+    _s.Const_shift(_s.vector)
+    _s.Supercell([2, 2, 2])
+    _s._type = 'Cartesian'
+    _s.Const_shift(-np.array([0.5, 0.5, 0.5]))
+    _s.Cart_coords()
+    _s._build_region()
+    _s.write_xyz()
+
+    
+
+def Ewald(
+        filename: str,
+        qm_region: str,
+        charges: str,
+        atom: str,
+        n: list,
+        expansion: np.ndarray,
+        r_cut: float,
+        bound: float,
+        verbose: int,
+        ) -> None:
+    '''
+    Generates a xfield input file for molcas calulations using the Ewald summation.
+    '''
+    _e = ewald.Ewald(qm_region, filename, charges, atom, n, r_cut, expansion, bound, verbose)
+    _e.Calculate_Ewald()
+    _e.Create_Zones()
+    _e.Fitting()
+
+def potential_plot(
+        filename: str,
+        xy_grid: int,
+        n_points: int,
+        n_contours: int,
+        ) -> None:
+    '''
+    Generates a potential plot from a molcas xfield output file.
+    '''
+    pot = ewald.Potential(filename, xy_grid, n_points, n_contours)
+    pot.Plot()
+
 def create_input_configurations() -> None:
     '''
     Creates input configurations for VASP calculations.
     '''
     if not os.path.exists(os.path.expanduser('~/.vasp_suite_configs')):
         os.mkdir(os.path.expanduser('~/.vasp_suite_configs'))
```

### Comparing `vasp_suite-1.1.3/vasp_suite/input.py` & `vasp_suite-1.2.0/vasp_suite/input.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,30 +29,31 @@
         #else:
         #    raise Warning('Unknown hostname. Generation of POTCAR file not possible.')
 
 
     def _INCAR(self):
         config = cp.ConfigParser()
         input_file = os.path.join(os.path.expanduser('~'), '.vasp_suite_configs', f'''{self.configuration}.ini''')
-        print(os.path.join(os.path.expanduser('~'), '.vasp_suite_configs', f'''{self.configuration}.ini'''))
         config.read(input_file)
-        print(config.sections())
         with open('INCAR', 'w') as f:
             for section in config.sections():
                 for key in config[section]:
                     key = key.upper()
                     f.write(f'''{key} = {config[section][key]}\n''')
 
     def _POTCAR(self):
-        pseudo = self.pseudopotentials 
+        pseudo = self.pseudopotentials
         potpaw = ['H', 'He', 'Li_sv', 'Be', 'B', 'C', 'N', 'O', 'F', 'Ne', 'Na_pv', 'Mg', 'Al', 'Si', 'P', 'S', 'Cl', 'Ar', 'K_sv', 'Ca_sv', 'Sc_sv', 'Ti_sv', 'V_sv', 'Cr_pv', 'Mn_pv', 'Fe', 'Co', 'Ni', 'Cu', 'Zn', 'Ga_d', 'Ge_d', 'As', 'Se', 'Br', 'Kr', 'Rb_sv', 'Sr_sv', 'Y_sv', 'Zr_sv', 'Nb_sv', 'Mo_sv', 'Tc_pv', 'Ru_pv', 'Rh_pv', 'Pd', 'Ag', 'Cd', 'In_d', 'Sn_d', 'Sb', 'Te', 'I', 'Xe', 'Cs_sv', 'Ba_sv', 'La', 'Ce_3', 'Nd_3', 'Pm_3', 'Sm_3', 'Eu_2', 'Gd_3', 'Tb_3', 'Dy_3', 'Ho_3', 'Er_3', 'Tm_3', 'Yb_2', 'Lu_3', 'Hf_pv', 'Ta_pv', 'W_sv', 'Re', 'Os', 'Ir', 'Pt', 'Au', 'Hg', 'Tl_d', 'Pb_d', 'Bi_d', 'Po_d', 'At', 'Rn', 'Fr_sv', 'Ra_sv', 'Ac', 'Th', 'Pa', 'U', 'Np', 'Pu', 'Am', 'Cm']
-        atoms = self._s.atoms 
+        atoms = self._s.atoms
+        order = list(range(len(atoms)))
 
-        files = [x for x in potpaw if x.split('_')[0] in atoms]
-        cwd = os.getcwd() 
+        files = [(x, x.split('_')) for x in potpaw if x.split('_')[0] in atoms]
+        files.sort(key=lambda x: order.index(atoms.index(x[1])))
+        files = [x[0] for x in files]
+        cwd = os.getcwd()
 
         with open('POTCAR', 'w') as f:
             os.system(f'''module load vasp''')
             os.chdir(pseudo)
             for file in files:
                 os.chdir(str(file))
                 with open('POTCAR', 'r') as g:
```

### Comparing `vasp_suite-1.1.3/vasp_suite/structure.py` & `vasp_suite-1.2.0/vasp_suite/structure.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
  # Imports 
 import re
 import os
 import numpy as np 
 import scipy as sp 
 from functools import wraps 
 from time import perf_counter
+from ase import io
 
 def timer(func):
     '''
     A decorator function to time functions.
     '''
     @wraps(func)
     def wrapper(*args, **kwargs):
@@ -58,14 +59,47 @@
        self.bv: np.ndarray = np.array([b1, b2, b3])
 
        # Generate atom list 
        atom_list = [f'{symbol} '*num for symbol, num in zip(self.atoms, self.natoms)]
        atom_list = ' '.join(atom_list).split()
        self._atom_list = atom_list
 
+       # calculate the volume of the unit cell 
+       self.V = np.dot(a1, np.cross(a2, a3)) 
+
+    def CIF_reader(self) -> None:
+        '''
+        Reads a .cif file and initializes it into the structure class.
+        '''
+        data = io.read(self.filename) 
+        self.name = data.get_chemical_formula()
+        self.scale = 1
+        self.av = data.cell.array
+        self._atom_list = data.get_chemical_symbols() 
+        self._N = len(self._atom_list)
+        self._type = 'direct'
+        self.coords = data.get_scaled_positions()
+
+        # convert atom list into atoms and natoms 
+        atom_list = self._atom_list 
+        atoms = list(set(atom_list)) 
+        natoms = [atom_list.count(x) for x in atoms] 
+        self.atoms = atoms 
+        self.natoms = natoms 
+
+        # Calculate reciprocal lattice vectors 
+        a1, a2, a3 = self.av 
+        b1 = 2 * np.pi * np.cross(a2, a3) / (a1@np.cross(a2,a3))
+        b2 = 2 * np.pi * np.cross(a3, a1) / (a2@np.cross(a3,a1))
+        b3 = 2 * np.pi * np.cross(a1, a2) / (a3@np.cross(a1,a2)) 
+        self.bv: np.ndarray = np.array([b1, b2, b3])
+
+        # calculate the volume of the unit cell 
+        self.V = np.dot(a1, np.cross(a2, a3))
+
     @property
     def get_name(self):
         '''
         Getter for name
         '''
         print(f'Name: {self.name}')
         return self.name
@@ -95,23 +129,36 @@
 
     def Supercell(self, n: list) -> None: 
         '''
         Creates a supercell of size n1 x n2 x n3. 
         '''
         coords = self.coords
         n1, n2, n3 = n 
-        supercell = np.array([[x[0]+a, x[1]+b, x[2]+c] for x in coords for a in range(n1) for b in range(n2) for c in range(n3)]) 
-        supercell /= n
-        self.av = self.av * n
-        self.coords = supercell 
+        av = self.av
+        self.orig_av = av
         atom_list = self._atom_list
-        atom_list = np.array([(f'{x} ' * 8).split() for x in atom_list])
-        atom_list = atom_list.flatten().reshape(-1,1)
+
+        _n1 = list(range(n[0]))
+        _n2 = list(range(n[1]))
+        _n3 = list(range(n[2]))
+        _n = np.array([[_n1[i], _n2[j], _n3[k]] for i in range(len(_n1)) for j in range(len(_n2)) for k in range(len(_n3))])
+        coords = np.array([coord + _n[i] for i in range(len(_n)) for coord in coords], dtype=float)
+
+        for i in range(len(coords)):
+            coords[i, 0] = coords[i, 0] / n[0]
+            coords[i, 1] = coords[i, 1] / n[1]
+            coords[i, 2] = coords[i, 2] / n[2]
+
+        av[0], av[1], av[2] = av[0] * n[0], av[1] * n[1], av[2] * n[2]
+        atom_list = [atom_list] * np.prod(n)
+        atom_list = np.array(atom_list).flatten()
+
+        self.coords = coords
+        self.av = av 
         self._atom_list = atom_list
-        self.natoms = [x*n1*n2*n3 for x in self.natoms]
 
     def Const_shift(self, vector: np.ndarray) -> np.ndarray:
         '''
         Shifts the structure by a constant vector. 
         '''
         coords = self.coords 
         coords += vector 
@@ -179,14 +226,59 @@
         enmax = [float(re.findall(r'ENMAX = ([0-9]+.[0-9]+)', x)[0]) for x in lines if 'ENMAX' in x] 
         encut = max(enmax) * 1.3 
         encut = round(encut / 50) * 50 
         encut_list = [x for x in range(encut - 300, encut + 300, 50)]
         self.encut = encut_list
         return np.array(encut_list)
 
+    def _find_index(self, atom: str):
+        '''
+        finds the index of the supplied atom in the coords and then returns the index of the atom in the atom_list 
+        '''
+        atom = re.split(r'(\d+)', atom)
+        for ind, symb in enumerate(self.atoms):
+            if symb == atom[0]:
+                atom_index = ind
+
+        _prev = np.sum(self.natoms[:atom_index])
+        location = _prev + int(atom[1]) - 1
+        vector = - self.coords[location]
+
+        self.vector = vector
+
+    def _build_region(self):
+        coords = self.cart_coords
+        atom_list = self._atom_list
+        atom_list = np.array(atom_list).reshape(-1,1)
+        coords = np.concatenate((atom_list, coords), axis=1)
+        a1, a2, a3 = self.orig_av
+        a1, a2, a3 = np.linalg.norm(a1), np.linalg.norm(a2), np.linalg.norm(a3)
+        a = np.min([a1, a2, a3])
+
+        # build a region around the atom of shape a1 x a2 x a3
+        region = np.array([coords[i] for i in range(len(coords)) if np.linalg.norm(coords[i, 1:]) < a/2])
+        coords = np.array(region[:, 1:], dtype=float)
+        atom_list = region[:, 0]
+        self.cart_coords = coords
+        self._atom_list = atom_list
+        self.name = self.name + '_qm'
+
+    def write_xyz(self):
+        '''
+        Writes an xyz file
+        '''
+        coords = self.cart_coords
+        atom_list = self._atom_list 
+        name = self.name
+
+        with open(f'{name}.xyz', 'w') as f:
+            f.write(f'{len(coords)}\n\n')
+            for i in range(len(coords)):
+                f.write(f'{atom_list[i]} {coords[i,0]} {coords[i,1]} {coords[i,2]}\n')
+
     def write_poscar(self):
         '''
         Writes POSCAR file. 
         '''
         with open('POSCAR', 'w') as f:
             f.write(f'{self.name}\n')
             f.write(f'{self.scale}\n')
@@ -283,19 +375,22 @@
 
     def Create_defect(self):
         '''
         Creates defects in the stucture
         '''
         structures = []
         for structure in self._structures:
-            for i in range(len(structure)-1):
-                if structure[i][0] == self.dopant:
-                    structure = np.delete(structure, i, axis=0)
-                    structures.append(structure)
-                    
+            for i in range(len(structure)):
+                try:
+                    if structure[i][0] == self.dopant:
+                        structure = np.delete(structure, i, axis=0)
+                        structures.append(structure)
+                except:
+                    pass
+
         self._structures = np.array(structures)
 
     def write_poscars(self) -> None:
         '''
         Writes the doped structures to POSCAR files.
         '''
         name: str = self._s.name 
@@ -502,8 +597,7 @@
             total_coords = np.unique(total_coords, axis=0)
             if len(total_coords) == len(asymm_unit):
                 searching = False
             else: 
                 asymm_unit = total_coords
         self.asymm_unit = asymm_unit
         self._write_xyz()
-
```

### Comparing `vasp_suite-1.1.3/vasp_suite/submission.py` & `vasp_suite-1.2.0/vasp_suite/submission.py`

 * *Files identical despite different names*

### Comparing `vasp_suite-1.1.3/vasp_suite.egg-info/PKG-INFO` & `vasp_suite-1.2.0/vasp_suite.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vasp-suite
-Version: 1.1.3
+Version: 1.2.0
 Summary: A package for creating and handling input files for vasp
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

