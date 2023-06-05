# Comparing `tmp/qwak-sim-2023.1013a0.tar.gz` & `tmp/qwak-sim-2023.1014a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwak-sim-2023.1013a0.tar", last modified: Tue May 16 14:40:52 2023, max compression
+gzip compressed data, was "qwak-sim-2023.1014a0.tar", last modified: Mon Jun  5 16:19:59 2023, max compression
```

## Comparing `qwak-sim-2023.1013a0.tar` & `qwak-sim-2023.1014a0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 14:40:52.384733 qwak-sim-2023.1013a0/
--rw-rw-rw-   0        0        0    35823 2022-04-06 17:13:42.000000 qwak-sim-2023.1013a0/LICENSE
--rw-rw-rw-   0        0        0    44887 2023-05-16 14:40:52.384733 qwak-sim-2023.1013a0/PKG-INFO
--rw-rw-rw-   0        0        0     2997 2023-03-03 16:23:09.000000 qwak-sim-2023.1013a0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 14:40:52.332733 qwak-sim-2023.1013a0/core/
-drwxrwxrwx   0        0        0        0 2023-05-16 14:40:52.350733 qwak-sim-2023.1013a0/core/qwak/
--rw-rw-rw-   0        0        0     3173 2023-01-12 18:57:54.000000 qwak-sim-2023.1013a0/core/qwak/Errors.py
--rw-rw-rw-   0        0        0    19476 2023-01-12 21:11:43.000000 qwak-sim-2023.1013a0/core/qwak/GraphicalQWAK.py
--rw-rw-rw-   0        0        0    18390 2023-05-04 16:33:03.000000 qwak-sim-2023.1013a0/core/qwak/Operator.py
--rw-rw-rw-   0        0        0     9100 2023-05-04 16:33:03.000000 qwak-sim-2023.1013a0/core/qwak/ProbabilityDistribution.py
--rw-rw-rw-   0        0        0     7927 2023-05-04 16:33:03.000000 qwak-sim-2023.1013a0/core/qwak/QuantumWalk.py
--rw-rw-rw-   0        0        0    10903 2023-05-04 16:33:03.000000 qwak-sim-2023.1013a0/core/qwak/State.py
--rw-rw-rw-   0        0        0     5868 2022-09-11 00:13:38.000000 qwak-sim-2023.1013a0/core/qwak/StochasticOperator.py
--rw-rw-rw-   0        0        0     1392 2022-09-11 00:13:38.000000 qwak-sim-2023.1013a0/core/qwak/StochasticProbabilityDistribution.py
--rw-rw-rw-   0        0        0     3282 2022-09-11 00:13:38.000000 qwak-sim-2023.1013a0/core/qwak/StochasticQuantumWalk.py
--rw-rw-rw-   0        0        0     5017 2022-09-11 00:13:38.000000 qwak-sim-2023.1013a0/core/qwak/StochasticQwak.py
--rw-rw-rw-   0        0        0      164 2023-05-16 14:39:40.000000 qwak-sim-2023.1013a0/core/qwak/__init__.py
--rw-rw-rw-   0        0        0    31792 2023-05-16 02:17:11.000000 qwak-sim-2023.1013a0/core/qwak/qwak.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:40:52.372732 qwak-sim-2023.1013a0/core/qwak_sim.egg-info/
--rw-rw-rw-   0        0        0    44887 2023-05-16 14:40:52.000000 qwak-sim-2023.1013a0/core/qwak_sim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      800 2023-05-16 14:40:52.000000 qwak-sim-2023.1013a0/core/qwak_sim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 14:40:52.000000 qwak-sim-2023.1013a0/core/qwak_sim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2023-05-16 14:40:52.000000 qwak-sim-2023.1013a0/core/qwak_sim.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-16 14:40:52.000000 qwak-sim-2023.1013a0/core/qwak_sim.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-16 14:40:52.377733 qwak-sim-2023.1013a0/core/utils/
--rw-rw-rw-   0        0        0     8767 2022-09-26 03:47:41.000000 qwak-sim-2023.1013a0/core/utils/PerfectStateTransfer.py
--rw-rw-rw-   0        0        0       33 2023-05-16 14:39:40.000000 qwak-sim-2023.1013a0/core/utils/__init__.py
--rw-rw-rw-   0        0        0     1081 2023-05-04 16:33:03.000000 qwak-sim-2023.1013a0/core/utils/jsonTools.py
--rw-rw-rw-   0        0        0    16222 2023-05-04 16:33:03.000000 qwak-sim-2023.1013a0/core/utils/plotTools.py
--rw-rw-rw-   0        0        0     1572 2023-05-16 14:39:40.000000 qwak-sim-2023.1013a0/pyproject.toml
--rw-rw-rw-   0        0        0      575 2023-05-16 14:40:52.386733 qwak-sim-2023.1013a0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-16 14:40:52.383217 qwak-sim-2023.1013a0/tests/
--rw-rw-rw-   0        0        0    19690 2023-01-12 20:35:08.000000 qwak-sim-2023.1013a0/tests/test_GraphicalQwakCycle.py
--rw-rw-rw-   0        0        0     9573 2023-05-04 16:33:03.000000 qwak-sim-2023.1013a0/tests/test_QwakComplete.py
--rw-rw-rw-   0        0        0     8030 2023-05-04 16:33:03.000000 qwak-sim-2023.1013a0/tests/test_QwakCycle.py
--rw-rw-rw-   0        0        0     9608 2023-05-04 16:33:03.000000 qwak-sim-2023.1013a0/tests/test_QwakPath.py
--rw-rw-rw-   0        0        0     1960 2022-09-10 23:35:23.000000 qwak-sim-2023.1013a0/tests/test_StochasticQwak.py
+drwxrwxrwx   0        0        0        0 2023-06-05 16:19:59.596982 qwak-sim-2023.1014a0/
+-rw-rw-rw-   0        0        0    35823 2022-04-06 17:13:42.000000 qwak-sim-2023.1014a0/LICENSE
+-rw-rw-rw-   0        0        0    44887 2023-06-05 16:19:59.596982 qwak-sim-2023.1014a0/PKG-INFO
+-rw-rw-rw-   0        0        0     2997 2023-03-03 16:23:09.000000 qwak-sim-2023.1014a0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 16:19:59.533981 qwak-sim-2023.1014a0/core/
+drwxrwxrwx   0        0        0        0 2023-06-05 16:19:59.559981 qwak-sim-2023.1014a0/core/qwak/
+-rw-rw-rw-   0        0        0     3173 2023-01-12 18:57:54.000000 qwak-sim-2023.1014a0/core/qwak/Errors.py
+-rw-rw-rw-   0        0        0    19476 2023-01-12 21:11:43.000000 qwak-sim-2023.1014a0/core/qwak/GraphicalQWAK.py
+-rw-rw-rw-   0        0        0    18452 2023-06-01 20:05:52.000000 qwak-sim-2023.1014a0/core/qwak/Operator.py
+-rw-rw-rw-   0        0        0     9100 2023-05-04 16:33:03.000000 qwak-sim-2023.1014a0/core/qwak/ProbabilityDistribution.py
+-rw-rw-rw-   0        0        0     7927 2023-05-04 16:33:03.000000 qwak-sim-2023.1014a0/core/qwak/QuantumWalk.py
+-rw-rw-rw-   0        0        0    10903 2023-05-04 16:33:03.000000 qwak-sim-2023.1014a0/core/qwak/State.py
+-rw-rw-rw-   0        0        0     5868 2022-09-11 00:13:38.000000 qwak-sim-2023.1014a0/core/qwak/StochasticOperator.py
+-rw-rw-rw-   0        0        0     1392 2022-09-11 00:13:38.000000 qwak-sim-2023.1014a0/core/qwak/StochasticProbabilityDistribution.py
+-rw-rw-rw-   0        0        0     3282 2022-09-11 00:13:38.000000 qwak-sim-2023.1014a0/core/qwak/StochasticQuantumWalk.py
+-rw-rw-rw-   0        0        0     5017 2022-09-11 00:13:38.000000 qwak-sim-2023.1014a0/core/qwak/StochasticQwak.py
+-rw-rw-rw-   0        0        0      164 2023-06-05 16:17:51.000000 qwak-sim-2023.1014a0/core/qwak/__init__.py
+-rw-rw-rw-   0        0        0    32633 2023-06-05 01:48:00.000000 qwak-sim-2023.1014a0/core/qwak/qwak.py
+drwxrwxrwx   0        0        0        0 2023-06-05 16:19:59.582980 qwak-sim-2023.1014a0/core/qwak_sim.egg-info/
+-rw-rw-rw-   0        0        0    44887 2023-06-05 16:19:59.000000 qwak-sim-2023.1014a0/core/qwak_sim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      800 2023-06-05 16:19:59.000000 qwak-sim-2023.1014a0/core/qwak_sim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 16:19:59.000000 qwak-sim-2023.1014a0/core/qwak_sim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2023-06-05 16:19:59.000000 qwak-sim-2023.1014a0/core/qwak_sim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-05 16:19:59.000000 qwak-sim-2023.1014a0/core/qwak_sim.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-05 16:19:59.588982 qwak-sim-2023.1014a0/core/utils/
+-rw-rw-rw-   0        0        0     8937 2023-06-01 20:05:52.000000 qwak-sim-2023.1014a0/core/utils/PerfectStateTransfer.py
+-rw-rw-rw-   0        0        0       33 2023-06-05 16:17:51.000000 qwak-sim-2023.1014a0/core/utils/__init__.py
+-rw-rw-rw-   0        0        0     2730 2023-06-05 16:11:16.000000 qwak-sim-2023.1014a0/core/utils/jsonTools.py
+-rw-rw-rw-   0        0        0    16222 2023-05-04 16:33:03.000000 qwak-sim-2023.1014a0/core/utils/plotTools.py
+-rw-rw-rw-   0        0        0     1572 2023-06-05 16:17:51.000000 qwak-sim-2023.1014a0/pyproject.toml
+-rw-rw-rw-   0        0        0      575 2023-06-05 16:19:59.598985 qwak-sim-2023.1014a0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-05 16:19:59.595982 qwak-sim-2023.1014a0/tests/
+-rw-rw-rw-   0        0        0    19690 2023-01-12 20:35:08.000000 qwak-sim-2023.1014a0/tests/test_GraphicalQwakCycle.py
+-rw-rw-rw-   0        0        0     9573 2023-05-04 16:33:03.000000 qwak-sim-2023.1014a0/tests/test_QwakComplete.py
+-rw-rw-rw-   0        0        0     8030 2023-05-04 16:33:03.000000 qwak-sim-2023.1014a0/tests/test_QwakCycle.py
+-rw-rw-rw-   0        0        0     9608 2023-05-04 16:33:03.000000 qwak-sim-2023.1014a0/tests/test_QwakPath.py
+-rw-rw-rw-   0        0        0     1960 2022-09-10 23:35:23.000000 qwak-sim-2023.1014a0/tests/test_StochasticQwak.py
```

### Comparing `qwak-sim-2023.1013a0/LICENSE` & `qwak-sim-2023.1014a0/LICENSE`

 * *Files identical despite different names*

### Comparing `qwak-sim-2023.1013a0/PKG-INFO` & `qwak-sim-2023.1014a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwak-sim
-Version: 2023.1013a0
+Version: 2023.1014a0
 Summary: Simulate Continuous-Time Quantum Walks
 Home-page: https://github.com/qwchagas/qwak
 Author: Jaime Santos
 Author-email: Jaime Santos <jaimepereirasantos123@gmail.com>, Bruno Chagas <na@na.na>, Rodrigo Chaves <na@na.na>, Lorenzo Buffoni <na@na.na>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

### Comparing `qwak-sim-2023.1013a0/README.md` & `qwak-sim-2023.1014a0/README.md`

 * *Files identical despite different names*

### Comparing `qwak-sim-2023.1013a0/core/qwak/Errors.py` & `qwak-sim-2023.1014a0/core/qwak/Errors.py`

 * *Files identical despite different names*

### Comparing `qwak-sim-2023.1013a0/core/qwak/GraphicalQWAK.py` & `qwak-sim-2023.1014a0/core/qwak/GraphicalQWAK.py`

 * *Files identical despite different names*

### Comparing `qwak-sim-2023.1013a0/core/qwak/Operator.py` & `qwak-sim-2023.1014a0/core/qwak/Operator.py`

 * *Files 2% similar despite different names*

```diff
@@ -375,21 +375,23 @@
         # TODO: Check if numpy is faster for eigenvecs and vals.
         try:
             nodeA = int(nodeA)
             nodeB = int(nodeB)
             if nodeA > nodeB:
                 nodeA, nodeB = swapNodes(nodeA, nodeB)
 
-            symAdj = sp.Matrix(self._hamiltonian.tolist())
-            # Isto já foi calculado.
-            eigenVec, D = symAdj.diagonalize()
-            eigenVal = getEigenVal(D)
+            symAdj = sp.Matrix(self._adjacency)
+            M = self._adjacency
+            P = self._eigenvectors
+            P_inv = np.linalg.inv(P)
+            D = np.matmul(P_inv, np.matmul(M, P))
             isCospec = isStrCospec(symAdj, nodeA, nodeB)
             chRoots, g, delta = checkRoots(
-                symAdj, nodeA, eigenVec, eigenVal)
+                symAdj, nodeA, self._eigenvectors, self._eigenvalues
+                )
             if isCospec and chRoots:
                 result = pi / (g * np.sqrt(delta))
             else:
                 result = -1
             return result
         except ValueError:
             raise MissingNodeInput(
@@ -542,7 +544,8 @@
     #     print(f"init: {initState}")
     #     print(f"Eigenvectors {self._eigenvectors}")
     #     for i in range(len(self._eigenvectors)):
     #         eigenVec = np.transpose(self._eigenvectors[:,i]).conjugate()
     #         ef += np.absolute(np.matmul(eigenVec,initState))**2
     #         print(f"eigenVec: {eigenVec}\t\t eigenVec norm: {np.linalg.norm(eigenVec)}\t\tef : {ef}\n")
     #     return ef
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `qwak-sim-2023.1013a0/core/qwak/ProbabilityDistribution.py` & `qwak-sim-2023.1014a0/core/qwak/ProbabilityDistribution.py`

 * *Files identical despite different names*

### Comparing `qwak-sim-2023.1013a0/core/qwak/QuantumWalk.py` & `qwak-sim-2023.1014a0/core/qwak/QuantumWalk.py`

 * *Files identical despite different names*

### Comparing `qwak-sim-2023.1013a0/core/qwak/State.py` & `qwak-sim-2023.1014a0/core/qwak/State.py`

 * *Files identical despite different names*

### Comparing `qwak-sim-2023.1013a0/core/qwak/StochasticOperator.py` & `qwak-sim-2023.1014a0/core/qwak/StochasticOperator.py`

 * *Files identical despite different names*

### Comparing `qwak-sim-2023.1013a0/core/qwak/StochasticProbabilityDistribution.py` & `qwak-sim-2023.1014a0/core/qwak/StochasticProbabilityDistribution.py`

 * *Files identical despite different names*

### Comparing `qwak-sim-2023.1013a0/core/qwak/StochasticQuantumWalk.py` & `qwak-sim-2023.1014a0/core/qwak/StochasticQuantumWalk.py`

 * *Files identical despite different names*

### Comparing `qwak-sim-2023.1013a0/core/qwak/StochasticQwak.py` & `qwak-sim-2023.1014a0/core/qwak/StochasticQwak.py`

 * *Files identical despite different names*

### Comparing `qwak-sim-2023.1013a0/core/qwak/qwak.py` & `qwak-sim-2023.1014a0/core/qwak/qwak.py`

 * *Files 2% similar despite different names*

```diff
@@ -300,15 +300,15 @@
         Parameters
         ----------
         newGraph : nx.Graph
             New NetworkX graph.
         """
         self._graph = newGraph
         self._n = len(self._graph)
-        self.setDim(self._n, graph=self._graph)
+        # self.setDim(self._n, graph=self._graph)
 
     def getGraph(self) -> nx.Graph:
         """Gets the current graph.
 
         Returns
         -------
         nx.Graph
@@ -832,14 +832,39 @@
 
         """
         try:
             return self._operator.checkPST(fromNode, toNode)
         except MissingNodeInput as err:
             raise err
 
+    def checkPST_sympy(self, fromNode, toNode) -> Union[str, bool]:
+        """Checks if a structure allows for PST between certain nodes.
+
+        Parameters
+        ----------
+        fromNode : _type_
+            Starting node.
+        toNode : _type_
+            Ending node.
+        Returns
+        -------
+        Union([str,bool])
+            _description_
+
+        Raises
+        ------
+        MissingNodeInput
+            Missing input node error.
+
+        """
+        try:
+            return self._operator.checkPST_sympy(fromNode, toNode)
+        except MissingNodeInput as err:
+            raise err
+
     def getTransportEfficiency(self) -> float:
         """Gets the transport efficiency of the quantum walk.
 
         Returns
         -------
         float
             Transport efficiency of the quantum walk.
@@ -887,14 +912,24 @@
         self.setGraph(newQWAK.getGraph())
         self.setDim(newQWAK.getDim(), graph=self._graph)
         self.setInitState(newQWAK.getInitState())
         self.setOperator(newQWAK.getOperator())
         self.setWalk(newQWAK.getWalk())
         self.setProbDist(newQWAK.getProbDist())
 
+    def getQWAKId(self) -> str:
+        """Gets the QWAK instance's ID.
+
+        Returns
+        -------
+        str
+            QWAK instance's ID.
+        """
+        return self._qwakId
+
     def to_json(self, isDynamic=False) -> str:
         """Returns a JSON representation of the QWAK instance
 
         Parameters
         ----------
         isDynamic : bool, optional
             If True, the JSON will contain the timeList, probDistList and
```

### Comparing `qwak-sim-2023.1013a0/core/qwak_sim.egg-info/PKG-INFO` & `qwak-sim-2023.1014a0/core/qwak_sim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwak-sim
-Version: 2023.1013a0
+Version: 2023.1014a0
 Summary: Simulate Continuous-Time Quantum Walks
 Home-page: https://github.com/qwchagas/qwak
 Author: Jaime Santos
 Author-email: Jaime Santos <jaimepereirasantos123@gmail.com>, Bruno Chagas <na@na.na>, Rodrigo Chaves <na@na.na>, Lorenzo Buffoni <na@na.na>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

### Comparing `qwak-sim-2023.1013a0/core/qwak_sim.egg-info/SOURCES.txt` & `qwak-sim-2023.1014a0/core/qwak_sim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qwak-sim-2023.1013a0/core/utils/PerfectStateTransfer.py` & `qwak-sim-2023.1014a0/core/utils/PerfectStateTransfer.py`

 * *Files 7% similar despite different names*

```diff
@@ -117,42 +117,41 @@
             for j in range(int(pow(i, 2)), n + 1, int(pow(i, 2))):
                 isSqrFree[j - 1] = False
     for i in range(n):
         if isSqrFree[i]:
             sqrFreeList.append(i + 1)
     return sqrFreeList
 
-
 def getEigenSupp(a, eigenvec, eigenval):
-    """EigenSupp is responsible for getting the eigenvalue support of the vertice a. The eigenvalue support of the vertice a is
-    all the eigenvalues such that Er a != 0, where a is vector with 1 in the a-th entry and zero in all others and Er is the
-    projection matrix of the eigenvalue r. It returns a list with all those eigenavlues. This is one of the conditions for PST,
-    because we do not need to check for eigenvalues that are not in the eigenvalue support.
+    """Returns the eigenvalue support of the vertex a.
+
+    The eigenvalue support of the vertex a is the set of all eigenvalues such that
+    the projection matrix of the eigenvalue r applied to the vector with 1 in the a-th
+    entry and zero in all others is not zero.
 
     Parameters
     ----------
-    a : _type_
-        _description_
-    eigenvec : _type_
-        _description_
-    eigenval : _type_
-        _description_
+    a : int
+        The index of the vertex.
+    eigenvec : numpy.ndarray
+        The eigenvectors of the graph.
+    eigenval : numpy.ndarray
+        The eigenvalues of the graph.
 
     Returns
     -------
-    _type_
-        _description_
+    list
+        The eigenvalues in the eigenvalue support of the vertex a.
     """
     supp = []
     for i in range(len(eigenval)):
-        if eigenvec.col(i)[a] != 0:
-            supp.append(eigenval[i])
+        if abs(eigenvec[a][i]) > 1e-10:
+            supp.append(round(eigenval[i],5))
     return supp
 
-
 def checkRoots(A, a, eigenvec, eigenval):
     """CheckRoots is responsible for checking the second condition for PST which is that all eigenvalues is the eigenvalue support
     of a must be all integers or all quadratic integers with the format p+qr*Sqrt(delta)/2, with qr changing from eigenvalue to
     to eigenvalue. The frist step is to define h(x) = phi/gcd(phi,phia) that have all its roots in the eigenvalue support of a,
     then its degree k will be crucial.
     First, we check for integer roots in the interval [-n^4,n^4] that the eigenvalues should be. We check by putting the
     value in the loop, i, direct into h(i) and we see if it is equal to zero. If it is, then we check if i is in the
@@ -196,33 +195,35 @@
     quadRoots = 0
     sqrtFreeInt = getSquareFree(int((4 * A**2).trace()))
     p = h.all_coeffs()[1]
     deltaTmp = 0
     for deltaS in sqrtFreeInt:
         q = 0
         while (p + q * sqrt(deltaS) / 2) <= sqrt(int(((A**2).trace()))):
+            # print(f'\np + q * sqrt(deltaS) / 2 = {Float(p + q * sqrt(deltaS) / 2, 3)}\nsupp = {supp}\nCondition: {Float(p + q * sqrt(deltaS) / 2, 3) in supp}\n')
             if (
                 h(p + q * sqrt(deltaS) / 2) == 0
                 and Float(p + q * sqrt(deltaS) / 2, 3) in supp
             ):
                 quadRoots += 1
                 deltaTmp = deltaS
             q += 1
-
+    # print(quadRoots < k, intRoots < k)
     if quadRoots > 0:
         delta = deltaTmp
     if quadRoots < k and intRoots < k:
         return False, 0, 0
     diffs = []
     for i in range(len(supp)):
         diffs.append((max(supp) - supp[i]) / np.sqrt(delta))
 
     g = 0
     for diff in diffs:
-        g = np.gcd(g, diff)
+        # print(f'g = {g}, diff = {diff}')
+        g = np.gcd(Float(g), Float(diff))
     return True, g, delta
 
 
 def swapNodes(nodeA, nodeB):
     """_summary_
 
     Parameters
```

### Comparing `qwak-sim-2023.1013a0/core/utils/plotTools.py` & `qwak-sim-2023.1014a0/core/utils/plotTools.py`

 * *Files identical despite different names*

### Comparing `qwak-sim-2023.1013a0/pyproject.toml` & `qwak-sim-2023.1014a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=54",
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qwak-sim"
-version = "2023.1013-alpha"
+version = "2023.1014-alpha"
 description = "Simulate Continuous-Time Quantum Walks"
 readme = "README.md"
 authors = [{ name = "Jaime Santos", email = "jaimepereirasantos123@gmail.com" },
             { name = "Bruno Chagas", email = "na@na.na" },
             { name = "Rodrigo Chaves", email = "na@na.na" },
             { name = "Lorenzo Buffoni", email = "na@na.na" }]
 license = { file = "LICENSE" }
@@ -38,15 +38,15 @@
 
 [tool.setuptools.packages.find]
 where = ["core"]
 include = ["qwak","utils"]  # alternatively: `exclude = ["additional*"]`
 namespaces = false
 
 [tool.bumpver]
-current_version = "2023.1013-alpha"
+current_version = "2023.1014-alpha"
 version_pattern = "YYYY.BUILD[-TAG]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `qwak-sim-2023.1013a0/setup.cfg` & `qwak-sim-2023.1014a0/setup.cfg`

 * *Files identical despite different names*

### Comparing `qwak-sim-2023.1013a0/tests/test_GraphicalQwakCycle.py` & `qwak-sim-2023.1014a0/tests/test_GraphicalQwakCycle.py`

 * *Files identical despite different names*

### Comparing `qwak-sim-2023.1013a0/tests/test_QwakComplete.py` & `qwak-sim-2023.1014a0/tests/test_QwakComplete.py`

 * *Files identical despite different names*

### Comparing `qwak-sim-2023.1013a0/tests/test_QwakCycle.py` & `qwak-sim-2023.1014a0/tests/test_QwakCycle.py`

 * *Files identical despite different names*

### Comparing `qwak-sim-2023.1013a0/tests/test_QwakPath.py` & `qwak-sim-2023.1014a0/tests/test_QwakPath.py`

 * *Files identical despite different names*

### Comparing `qwak-sim-2023.1013a0/tests/test_StochasticQwak.py` & `qwak-sim-2023.1014a0/tests/test_StochasticQwak.py`

 * *Files identical despite different names*

