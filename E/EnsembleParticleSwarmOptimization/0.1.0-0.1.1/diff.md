# Comparing `tmp/EnsembleParticleSwarmOptimization-0.1.0.tar.gz` & `tmp/EnsembleParticleSwarmOptimization-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EnsembleParticleSwarmOptimization-0.1.0.tar", last modified: Mon Jan 30 15:37:32 2023, max compression
+gzip compressed data, was "EnsembleParticleSwarmOptimization-0.1.1.tar", last modified: Mon Jun  5 16:25:59 2023, max compression
```

## Comparing `EnsembleParticleSwarmOptimization-0.1.0.tar` & `EnsembleParticleSwarmOptimization-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 dxb792   (1939480938) domain users (1734600513)        0 2023-01-30 15:37:32.533697 EnsembleParticleSwarmOptimization-0.1.0/
-drwxr-xr-x   0 dxb792   (1939480938) domain users (1734600513)        0 2023-01-30 15:37:32.533697 EnsembleParticleSwarmOptimization-0.1.0/EnsembleParticleSwarmOptimization.egg-info/
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      661 2023-01-30 15:37:32.000000 EnsembleParticleSwarmOptimization-0.1.0/EnsembleParticleSwarmOptimization.egg-info/PKG-INFO
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      431 2023-01-30 15:37:32.000000 EnsembleParticleSwarmOptimization-0.1.0/EnsembleParticleSwarmOptimization.egg-info/SOURCES.txt
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)        1 2023-01-30 15:37:32.000000 EnsembleParticleSwarmOptimization-0.1.0/EnsembleParticleSwarmOptimization.egg-info/dependency_links.txt
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)       77 2023-01-30 15:37:32.000000 EnsembleParticleSwarmOptimization-0.1.0/EnsembleParticleSwarmOptimization.egg-info/requires.txt
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)        5 2023-01-30 15:37:32.000000 EnsembleParticleSwarmOptimization-0.1.0/EnsembleParticleSwarmOptimization.egg-info/top_level.txt
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      661 2023-01-30 15:37:32.533697 EnsembleParticleSwarmOptimization-0.1.0/PKG-INFO
-drwxr-xr-x   0 dxb792   (1939480938) domain users (1734600513)        0 2023-01-30 15:37:32.533697 EnsembleParticleSwarmOptimization-0.1.0/PySO/
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)    10050 2022-07-01 15:49:40.000000 EnsembleParticleSwarmOptimization-0.1.0/PySO/Clustering_Swarms.py
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)    29614 2023-01-12 14:20:58.000000 EnsembleParticleSwarmOptimization-0.1.0/PySO/HierarchicalSwarmHandler.py
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)    30396 2023-01-30 15:36:02.000000 EnsembleParticleSwarmOptimization-0.1.0/PySO/MWE_Swarm.py
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)     2174 2022-03-28 10:48:24.000000 EnsembleParticleSwarmOptimization-0.1.0/PySO/Model.py
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)     8369 2022-06-29 10:18:27.000000 EnsembleParticleSwarmOptimization-0.1.0/PySO/SwarmHandler.py
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      288 2022-06-29 10:20:13.000000 EnsembleParticleSwarmOptimization-0.1.0/PySO/__init__.py
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)       63 2022-07-04 15:51:30.000000 EnsembleParticleSwarmOptimization-0.1.0/README.md
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)       38 2023-01-30 15:37:32.533697 EnsembleParticleSwarmOptimization-0.1.0/setup.cfg
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      885 2023-01-30 15:36:59.000000 EnsembleParticleSwarmOptimization-0.1.0/setup.py
+drwxr-xr-x   0 dxb792   (1939480938) domain users (1734600513)        0 2023-06-05 16:25:59.965747 EnsembleParticleSwarmOptimization-0.1.1/
+drwxr-xr-x   0 dxb792   (1939480938) domain users (1734600513)        0 2023-06-05 16:25:59.965747 EnsembleParticleSwarmOptimization-0.1.1/EnsembleParticleSwarmOptimization.egg-info/
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      850 2023-06-05 16:25:59.000000 EnsembleParticleSwarmOptimization-0.1.1/EnsembleParticleSwarmOptimization.egg-info/PKG-INFO
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      431 2023-06-05 16:25:59.000000 EnsembleParticleSwarmOptimization-0.1.1/EnsembleParticleSwarmOptimization.egg-info/SOURCES.txt
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)        1 2023-06-05 16:25:59.000000 EnsembleParticleSwarmOptimization-0.1.1/EnsembleParticleSwarmOptimization.egg-info/dependency_links.txt
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)       77 2023-06-05 16:25:59.000000 EnsembleParticleSwarmOptimization-0.1.1/EnsembleParticleSwarmOptimization.egg-info/requires.txt
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)        5 2023-06-05 16:25:59.000000 EnsembleParticleSwarmOptimization-0.1.1/EnsembleParticleSwarmOptimization.egg-info/top_level.txt
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      850 2023-06-05 16:25:59.965747 EnsembleParticleSwarmOptimization-0.1.1/PKG-INFO
+drwxr-xr-x   0 dxb792   (1939480938) domain users (1734600513)        0 2023-06-05 16:25:59.965747 EnsembleParticleSwarmOptimization-0.1.1/PySO/
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)    10064 2023-06-05 15:46:22.000000 EnsembleParticleSwarmOptimization-0.1.1/PySO/Clustering_Swarms.py
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)    34011 2023-06-05 16:01:32.000000 EnsembleParticleSwarmOptimization-0.1.1/PySO/HierarchicalSwarmHandler.py
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)    30396 2023-06-02 15:36:36.000000 EnsembleParticleSwarmOptimization-0.1.1/PySO/MWE_Swarm.py
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)     2174 2023-06-02 15:36:36.000000 EnsembleParticleSwarmOptimization-0.1.1/PySO/Model.py
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)     8369 2023-06-02 15:36:36.000000 EnsembleParticleSwarmOptimization-0.1.1/PySO/SwarmHandler.py
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      288 2023-06-05 16:11:21.000000 EnsembleParticleSwarmOptimization-0.1.1/PySO/__init__.py
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      212 2023-06-05 16:23:57.000000 EnsembleParticleSwarmOptimization-0.1.1/README.md
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)       38 2023-06-05 16:25:59.965747 EnsembleParticleSwarmOptimization-0.1.1/setup.cfg
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      885 2023-06-05 16:11:39.000000 EnsembleParticleSwarmOptimization-0.1.1/setup.py
```

### Comparing `EnsembleParticleSwarmOptimization-0.1.0/EnsembleParticleSwarmOptimization.egg-info/PKG-INFO` & `EnsembleParticleSwarmOptimization-0.1.1/EnsembleParticleSwarmOptimization.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 Metadata-Version: 2.1
 Name: EnsembleParticleSwarmOptimization
-Version: 0.1.0
+Version: 0.1.1
 Summary: Ensemble of particle swarms together with various velocity rules for function optimization
 Home-page: https://github.com/dig07/PySO
 Author: Christopher Moore and Diganta Bandopadhyay
 Author-email: diganta@star.sr.bham.ac.uk
 License: UNKNOWN
 Description: # PySO
         Particle swarm optimizer
         
         Currently under development. 
         
+        ![Multiple Swarm](examples/hierarchical_results/animation_non_periodic.gif)
+        
+        
+        See current To do list here: https://trello.com/b/SEnVSWWd/to-do-list
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `EnsembleParticleSwarmOptimization-0.1.0/PKG-INFO` & `EnsembleParticleSwarmOptimization-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 Metadata-Version: 2.1
 Name: EnsembleParticleSwarmOptimization
-Version: 0.1.0
+Version: 0.1.1
 Summary: Ensemble of particle swarms together with various velocity rules for function optimization
 Home-page: https://github.com/dig07/PySO
 Author: Christopher Moore and Diganta Bandopadhyay
 Author-email: diganta@star.sr.bham.ac.uk
 License: UNKNOWN
 Description: # PySO
         Particle swarm optimizer
         
         Currently under development. 
         
+        ![Multiple Swarm](examples/hierarchical_results/animation_non_periodic.gif)
+        
+        
+        See current To do list here: https://trello.com/b/SEnVSWWd/to-do-list
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `EnsembleParticleSwarmOptimization-0.1.0/PySO/Clustering_Swarms.py` & `EnsembleParticleSwarmOptimization-0.1.1/PySO/Clustering_Swarms.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     I: float
         the inertia of the clustering; i.e. the sum of the squared
         distances between the points and the cluster centres
     membership: array, shape=(n,)
         for each particle, return an int in the range 0, K-1
         identifying the cluster to which it belongs
     """
-    kmeans = KMeans(n_clusters=K)
+    kmeans = KMeans(n_clusters=K,n_init='auto')
     kmeans.fit(X_std)
 
     I = kmeans.inertia_
     memberships = kmeans.labels_
 
     return I, memberships, kmeans
```

### Comparing `EnsembleParticleSwarmOptimization-0.1.0/PySO/HierarchicalSwarmHandler.py` & `EnsembleParticleSwarmOptimization-0.1.1/PySO/HierarchicalSwarmHandler.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,19 @@
                  Minimum_exploration_iterations = 50,
                  Initial_exploration_limit= 150,
                  clustering_indices = None,
                  use_func_vals_in_clustering = False,
                  kick_velocities = True,
                  fitness_veto_fraction = 0.05,
                  max_particles_per_swarm = None,
-                 redraw_velocities_at_segmentation = False):
+                 redraw_velocities_at_segmentation = False,
+                 clustering_min_membership = 5,
+                 clustering_max_clusters = 70,
+                 Tol = 1.0e-2,
+                 Convergence_testing_num_iterations = 50):
         """
 
         REQUIRED INPUTS
         ------
         Hierarchical_models: list,
             list of Hierarchical model objects
         NumSwarms: int
@@ -55,17 +59,17 @@
         ---------------
         Omega: float or list
             the omega parameter for each hierarhical model, inertial coefficient for velocity updating [defaults to .6]
         PhiP: float or list
             the phi_p parameter for each hierarhical model, cognitive coefficient for velocity updating [defaults to .2]
         PhiG: float or list
             the phi_g parameter for each hierarhical model, social coefficient for velocity updating [defaults to .2]
-        MH_fraction: float:
+        MH_fraction: float
             parameter controlling proportion of velocity rule dictated by MCMC, for each hierarchical model [defaults to 0.]
-        Swarm_kwargs: dict,
+        Swarm_kwargs: dict
             dictionary of common arguments between all swarms
         Output: str
             folder in which to save output [defaults to './']
         nPeriodicCheckpoint: int
             number of iterations between printing checkpoints [defaults to 10]
             (Note the swarm will checkpoint its position on every iteration, needed for sampling case)
         Swarm_names: None or list of strings
@@ -77,55 +81,71 @@
         Maxiter: int
             maximum number of iterations the ensemble will run for [defaults to 1e4]
         Resume: bool
             look for resume pkl file on startup and checkpoint during run [defaults to False]
         Maximum_number_of_iterations_per_step: int
             Maximum number of iterations per step
         Minimum_exploration_iterations: int
-            Minimum number of iterations to be done in each step before stall condition evaluated
+            Minimum number of iterations to be done in each step before stall condition evaluated [defaults to 50]
         Initial_exploration_limit: int
-            Minimum number of iterations done in the very first step before stall condition evaluated
+            Minimum number of iterations done in the very first step before stall condition evaluated [defaults to 150]
         clustering_indices: None or list of int
-            Parameter position indexes to use for relabelling/clustering step
+            Parameter position indexes to use for relabelling/clustering step [defaults to all parameters]
         use_func_vals_in_clustering: boolean
             Boolean flag for using function values for clustering or not [defaults to False]
         kick_velocities: boolean
             Boolean flag for reinitialising velocities from position distribution
             on clustering and segmenting [defaults to True]
         fitness_veto_fraction: float
             Fraction of Best swarm position below which we throw away new swarms [defaults to 0.05]
         max_particles_per_swarm: integer
             Maximum number of particles per swarm [defaults to int(total_num_particles/10)]
         redraw_velocities_at_segmentation: Boolean
             Boolean flag indicating if the velocities should be redrawn from swarm position ranges at each segmentation step [defaults to False]
+        clustering_min_membership: int
+            minimum number of particles in each swarm [defaults to 5]
+        clustering_max_clusters: int
+            maximum number of clusters to test for the clustering [defaults to 70]
+        Tol: float
+            the minimum improvement on functionvalue for each swarm that we class as not stalled [defaults to 1e-2]
+        Convergence_testing_num_iterations: int
+            If best swarm value has not improved over this many last iterations (improved past Tol) [defaults to 50]
         """
         assert len(Hierarchical_models)>1, "Please input multiple models for Hierarchical PSO search"
 
         self.Hierarchical_models = Hierarchical_models
 
+        # Ladder for PSO hyper-parameters
         self.Omegas = Omega
         self.PhiPs = PhiP
         self.PhiGs = PhiG
         self.MH_fractions = MH_fraction
 
+        # If PSO hyper-parameters are only a float, replicate them for each step in the ladder
         if type(self.Omegas) == float:
             self.Omegas = [self.Omegas] * len(self.Hierarchical_models)
             self.PhiPs = [self.PhiPs] * len(self.Hierarchical_models)
             self.PhiGs = [self.PhiGs] * len(self.Hierarchical_models)
             self.MH_fractions = [self.MH_fractions] * len(self.Hierarchical_models)
         else:
             assert len(self.Omegas) == len(self.Hierarchical_models), "Please ensure your PSO parameter lists correspond to the correct number of hierarchical steps "
 
-
+        # Parameter names
         self.Model_axis_names = self.Hierarchical_models[1].names
 
+
+        # Number of dimensions
         self.Ndim = len(self.Model_axis_names)
 
         self.NumSwarms = NumSwarms
+
+        # NOTE THIS NAME IS MISLEADING, this is just the total size of the initial swarm
         self.NumParticlesPerSwarm = NumParticlesPerSwarm
+
+        # Common parameters for all swarms
         self.Swarm_kwargs = Swarm_kwargs
 
         self.nPeriodicCheckpoint = nPeriodicCheckpoint
 
         self.BestKnownEnsemblePoint = np.zeros(self.Ndim)
         self.BestKnownEnsembleValue = None
         self.BestCurrentSwarm = None
@@ -133,72 +153,98 @@
         self.Verbose = Verbose
 
         self.SaveEvolution = SaveEvolution
 
         # Refering to the hierarchical steps
         self.Maximum_number_of_iterations_per_step = Maximum_number_of_iterations_per_step
 
+        # Minimum number of iterations the swarms will conduct before they evaluate the stall condition
         self.Minimum_exploration_iterations = Minimum_exploration_iterations
 
+        # Minimum number of iterations for the first model
         self.Initial_exploration_limit = Initial_exploration_limit
 
-
+        # Maximum number of iterations the whole ensemble of swarms will run for
         self.Maxiter = Maxiter
 
+        # UNTESTED RESUME FUNCTIONALITY
         self.Resume = Resume
 
+        # Output directory
         self.Output = Output
 
+        # If we have given then swarm names, otherwise default to numbered list
         self.Swarm_names = Swarm_names
         if self.Swarm_names == None: self.Swarm_names = np.arange(self.NumSwarms) # Defaults to numbered list of swarms
 
-
+        # If the clustering is done only in certain parameters, otherwise cluster in all dimensions (Not including objective function value)
         self.clustering_indices  = clustering_indices
         if self.clustering_indices == None: self.clustering_indices = np.arange(self.Ndim) # Use all parameters by default in clustering
 
+        # If the objective function value is to be used in the clustering process.
         self.use_func_vals_in_clustering = use_func_vals_in_clustering
 
+        # If true, draw new velocities from the new swarms particle positions using a normal distribution [ DEFAULTS TO TRUE ]
+        # If false, use previous particle velocities
         self.kick_velocities = kick_velocities
 
+        # If true, draw new velocities from the new swarms particle positions using a uniform distribution [ DEFAULTS TO FALSE ]
+        # If false, use previous particle velocities
         self.redraw_velocities_at_segmentation = redraw_velocities_at_segmentation
 
+        # self.fitness_veto_fraction * best_objective_function_Val below which we throw swarms away (reassign particles to other swarms)
         self.fitness_veto_fraction = fitness_veto_fraction
 
+        # Maximum particles per swarm, defaults to total particles over 10
         self.max_particles_per_swarm = max_particles_per_swarm
         if self.max_particles_per_swarm == None: self.max_particles_per_swarm = int(self.NumParticlesPerSwarm/10)
 
-        #Initialise swarms
+        # Initialise swarms
         self.InitialiseSwarms()
 
+        # frozen swarms are temporarily held in this dict
         self.frozen_swarms = {}
 
+        # Counts which hierarchical model we are on
         self.Hierarchical_model_counter = 0
 
         # Boolean variable to indicate if all swarms at the current level have stalled
         self.AllStalled = False
 
+        # Variable to check if all swarms have finishing iterating on the last hierarchical model.
         self.swarm_stepping_done = False
 
+        # Clustering parameters (See docstrings)
+        self.clustering_min_membership = clustering_min_membership
+        self.clustering_max_clusters = clustering_max_clusters
+
+        # RESUME FUNCTIONALITY UNTESTED TODO: TEST
         resume_file = os.path.join(self.Output, "PySO_resume.pkl")
 
+        # Stall testing parameters
+        self.Tol = Tol
+        self.Convergence_testing_num_iterations = Convergence_testing_num_iterations
+
         if self.Resume and os.path.exists(resume_file):
             print('Resuming from file {}'.format(resume_file))
             self.ResumeFromCheckpoint()
 
 
     def InitialiseSwarms(self):
         """
         Initialise the swarm points, values and velocities
 
         """
+        # self.Swarms contains all the swarms.
         self.Swarms = {self.Swarm_names[swarm_index]: Swarm(self.Hierarchical_models[0], self.NumParticlesPerSwarm,
                                                             Omega=self.Omegas[0], Phig= self.PhiGs[0], Phip=self.PhiPs[0], Mh_fraction=self.MH_fractions[0],
                                                             **self.Swarm_kwargs)
                        for swarm_index in self.Swarm_names}
 
+        # Computed stability number to check for convergence criteria (might be pointless)
         stability_num = self.stability_check(self.Omegas[0],
                                              self.PhiPs[0],
                                              self.PhiGs[0])
         print('Stability number:', stability_num)
 
         if stability_num <= 0:
             warnings.warn('Stability number is less than 0, initiated swarm is not guranteed to converge!')
@@ -213,21 +259,22 @@
             initial_max_func_vals.append(Swarm_.BestKnownSwarmValue)
 
         self.BestKnownEnsembleValue = np.max(initial_max_func_vals)
         self.BestKnownEnsemblePoint = initial_best_positions[np.argmax(initial_max_func_vals)]
         self.BestCurrentSwarm = list(self.Swarms.keys())[np.argmax(initial_max_func_vals)]
         self.EvolutionCounter = 0
 
-
+        print('Swarm initialisation finished....')
     def EvolveSwarms(self):
         """
         Evolve every swarm through a single iteration
         """
         self.EvolutionCounter += 1
 
+        # TODO: Could probably speed this up by assigning different pools of CPUs to different Swarms
         for name in list(self.Swarms.keys()):
             self.Swarms[name].EvolveSwarm()
 
             if np.max(self.Swarms[name].BestKnownSwarmValue) > self.BestKnownEnsembleValue:
                 self.BestKnownEnsembleValue = np.max(self.Swarms[name].BestKnownSwarmValue)
                 self.BestKnownEnsemblePoint = self.Swarms[name].Points[np.argmax(self.Swarms[name].Values)]
                 self.BestCurrentSwarm = name
@@ -268,36 +315,33 @@
                 # Remove those particles from the frozen swarms datastructure
                 self.frozen_swarms[swarm_index].Points = np.delete(self.frozen_swarms[swarm_index].Points,lowest_fitness_particle_indices,0)
                 self.frozen_swarms[swarm_index].Velocities = np.delete(self.frozen_swarms[swarm_index].Velocities,lowest_fitness_particle_indices,0)
                 self.frozen_swarms[swarm_index].Values = np.delete(self.frozen_swarms[swarm_index].Values,lowest_fitness_particle_indices,0)
                 self.frozen_swarms[swarm_index].BestKnownSwarmPoints = np.delete(self.frozen_swarms[swarm_index].BestKnownPoints,lowest_fitness_particle_indices,0)
                 self.frozen_swarms[swarm_index].BestKnownSwarmValue = np.delete(self.frozen_swarms[swarm_index].BestKnownValues,lowest_fitness_particle_indices,0)
 
-                # if current size is over 25 it will just get bigger once reclustering occurs probably
-
                 print('Swarm ',swarm_index, ' is over the maximum size per swarm, redistributing ',num_particles_in_swarm -
                       self.max_particles_per_swarm,' Particles')
 
         return(num_particles_redistributed)
 
 
 
     def Reallocate_particles(self):
         """Use all particles in current swarms, cluster them based on features and reallocate"""
 
         # Dont want to converge to or explore peaks that are below a certain threshold compared to the best of the entire ensemble
         # But dont want this redistribution to take place on the first "exploratory" swarm
         # Also dont want to redistribute if we are mostly doing MH MCMC velocity rule, as we dont expect strong clustering there
         if self.Hierarchical_model_counter != 0 and self.MH_fractions[self.Hierarchical_model_counter]< 0.1:
+            # this is the TOTAL number of particles to be redistributed to a new swarm
             num_particles_redistributed = self.veto_and_redistribute()
 
         # Extract positions to be used for clustering, only using the indices of parameters that are well measured AND function value     #
         # Feature_array - Particle positions, function values, not all components (Specially not ones well measured)
-        # Chirp mass, distance, sky position, effective spin, time to merger, function values
-
 
         clustering_parameter_positions = np.array([np.take(self.frozen_swarms[swarm_index].Points,self.clustering_indices,axis=1) for swarm_index
                                in self.frozen_swarms.keys()])
 
         clustering_parameter_positions = np.concatenate(clustering_parameter_positions)
 
 
@@ -305,64 +349,70 @@
             clustering_function_values = np.array([self.frozen_swarms[swarm_index].Values for swarm_index
                                                    in self.frozen_swarms.keys()])
             clustering_function_values = np.concatenate(clustering_function_values)
             clustering_features = np.column_stack((clustering_parameter_positions, clustering_function_values))
         else:
             clustering_features = clustering_parameter_positions
 
-
-        K, memberships = Clustering(clustering_features, min_membership=5,max_clusters=70)
+        # min membership is the minimum number of particles per swarm and max clusters is the maximum number of clusters
+        K, memberships = Clustering(clustering_features,min_membership=self.clustering_min_membership,max_clusters=self.clustering_max_clusters)
 
 
         total_particle_positions = np.array([self.frozen_swarms[swarm_index].Points for swarm_index
                                in self.frozen_swarms.keys()])
         total_particle_velocities = np.array([self.frozen_swarms[swarm_index].Velocities for swarm_index
                                in self.frozen_swarms.keys()])
 
         total_particle_velocities = np.concatenate(total_particle_velocities)
         total_particle_positions = np.concatenate(total_particle_positions)
 
         print('Reinitiating swarms with Omega: ',self.Omegas[self.Hierarchical_model_counter+1],
               ' PhiP: ',self.PhiPs[self.Hierarchical_model_counter+1],
               ' PhiG: ',self.PhiGs[self.Hierarchical_model_counter+1])
 
+        # Stability check for convergence (Might be removed)
         stability_num = self.stability_check(self.Omegas[self.Hierarchical_model_counter+1],
                                              self.PhiPs[self.Hierarchical_model_counter+1],
                                              self.PhiGs[self.Hierarchical_model_counter+1])
         print('Stability number:', stability_num)
 
         if stability_num<=0:
             warnings.warn('Stability number is less than 0, initiated swarm is not guranteed to converge!')
 
-
+        # Create each swarm
         for swarm_index in range(K):
 
               swarm_particle_positions = total_particle_positions[np.where(memberships == swarm_index)[0]]
               swarm_particle_velocities = total_particle_velocities[np.where(memberships == swarm_index)[0]]
               self.Swarms[swarm_index] = self.Reinitiate_swarm(swarm_particle_positions, swarm_particle_velocities)
 
-
+        # Check to make sure that we arent on the first segment and there are actually particles to be redistributed (from veto)
+        # Extra swarm for redistributed particles
         if self.Hierarchical_model_counter != 0 and num_particles_redistributed>0:
-            # Redistribute particles from veto step above
+            # Re-distribute particles into a NEW swarm, ie all redistributing particles go into this new swarm (This may not be a good idea in the end)
+
+            # Get all positions from all frozen swarms, which at this stage is ALL swarms (from previous segment)
             parameter_positions = np.array(
-                [self.frozen_swarms[swarm_index].Points  for swarm_index
+                [self.frozen_swarms[swarm_index].Points for swarm_index
                  in self.frozen_swarms.keys()])
 
             parameter_positions = np.concatenate(parameter_positions)
 
-            # Distribute them using covariance matrix of current clusters
+            # Distribute the new swarms positions basically using the centre point of all the current swarms
             cov = np.cov(parameter_positions.T)
             position_mean = np.mean(parameter_positions,axis=0)
             velocity_mean = np.zeros(self.Ndim)
 
             redistributed_particle_positions = np.random.multivariate_normal(position_mean, cov, size=num_particles_redistributed)
             redistributed_particle_velocities = np.random.multivariate_normal(velocity_mean, cov, size=num_particles_redistributed)
 
             # Extra redistributed swarm
             self.Swarms[K] = self.Reinitiate_swarm(redistributed_particle_positions, redistributed_particle_velocities)
+
+        # Empty the frozen swarms dict as we are done with the old swarms
         self.frozen_swarms = {}
         self.AllStalled = False
 
         self.Hierarchical_model_counter += 1
 
     def stability_check(self, Omega, PhiP, PhiG):
         """
@@ -421,49 +471,56 @@
             Omega = self.Omegas[self.Hierarchical_model_counter + 1]
             PhiP = self.PhiPs[self.Hierarchical_model_counter + 1]
             PhiG = self.PhiGs[self.Hierarchical_model_counter + 1]
             MH_fraction = self.MH_fractions[self.Hierarchical_model_counter + 1]
 
         num_particles = positions.shape[0]
 
-        newswarm = Swarm(self.Hierarchical_models[self.Hierarchical_model_counter+ 1],num_particles,
+        newswarm = Swarm(self.Hierarchical_models[self.Hierarchical_model_counter + 1],num_particles,
                          Omega=Omega, Phip=PhiP, Phig=PhiG, Mh_fraction=MH_fraction , **self.Swarm_kwargs)
 
         newswarm.EvolutionCounter = 0
         newswarm.Points = positions
 
-        if self.kick_velocities == True: #and self.Hierarchical_model_counter>0.5*len(self.Hierarchical_models):
+        if self.kick_velocities == True:
             # Kick the reinitialised velocities
             # Regenerate velocities from a normal distribution specified by the covariance of particles in swarm
             vel_cov = np.cov(positions.T)
 
             # Reinitialising velocities with a mean of zero (Shape of mean is 1D with length number of dimensions)
             mean = np.zeros(positions.shape[1])
 
             # Draw velocities from normal distribution specified by position
             newswarm.Velocities = np.random.multivariate_normal(mean, vel_cov, size=num_particles)
         else:
             newswarm.Velocities = velocities
 
+        ## TODO: Need to merge kick_velocity option with redraw_velocities_at_segmentation since they do very similar things
+
         if self.redraw_velocities_at_segmentation == True:
 
+            # Work out the peak to peak of the positions in each axis.
             ptp_vel_bounds = np.ptp(np.array([np.min(positions,axis=0),np.max(positions,axis=0)]).T,axis=1)
 
+            # draw velocities from U[-ptp/2,ptp/2]
             newswarm.Velocities = (ptp_vel_bounds) * np.random.random_sample(size=(num_particles,self.Ndim)) - ptp_vel_bounds/2
 
-
+        # Carry over points from previous models optimization
         newswarm.BestKnownPoints = copy.deepcopy(newswarm.Points)
 
         # Recalculate best personal known values:
         for i in range(newswarm.NumParticles):
+            # TODO: This be paralellized
             newswarm.BestKnownValues[i] = newswarm.Model.log_likelihood(
                 dict(zip(newswarm.Model.names, newswarm.Points[i])))
 
+        # First values for each particle are by definition their best known values
         newswarm.Values = copy.deepcopy(newswarm.BestKnownValues)
 
+        # Best point and swarm value
         newswarm.BestKnownSwarmPoint = newswarm.BestKnownPoints[np.argmax(newswarm.BestKnownValues)]
         newswarm.BestKnownSwarmValue = np.max(newswarm.BestKnownValues)
 
         # Sets up multiprocessing pool for parallel function computations
         newswarm.Pool = Pool(self.Swarm_kwargs['Nthreads'])
 
         return (newswarm)
@@ -523,28 +580,28 @@
 
     def SaveEnsembleEvolution(self):
         """
         At each checkpoint append the evolution of the swarm to the history file
         """
         history_file_path = os.path.join(self.Output, "EnsembleEvolutionHistory.dat")
 
-        # "# particle_number, name1, name2, name3, ..., function_value\n"
+        # "# swarm name, particle_number, name1, name2, name3, ..., function_value\n"
         for swarm_name in list(self.Swarms.keys()):
             for particle_index in range(self.Swarms[swarm_name].NumParticles):
                 string = str(swarm_name) + ","
                 string += str(particle_index) + ","
                 string += np.array2string(self.Swarms[swarm_name].Points[particle_index], separator=',')[1:-1].replace('\n', '')
                 string += ",{}".format(self.Swarms[swarm_name].Values[particle_index])
                 string += ",{}".format(self.Hierarchical_model_counter)
                 string += ",{}\n".format(self.EvolutionCounter)
                 file = open(history_file_path, "a")
                 file.write(string)
                 file.close()
 
-        # All the frozen swarm data
+        # All the frozen swarm data : Might be redundant to store these instead of with a 'frozen' flag but helps with visualisation for now
         for swarm_name in list(self.frozen_swarms.keys()):
             for particle_index in range(self.frozen_swarms[swarm_name].NumParticles):
                 string = str(swarm_name) + ","
                 string += str(particle_index) + ","
                 string += np.array2string(self.frozen_swarms[swarm_name].Points[particle_index], separator=',')[1:-1].replace('\n', '')
                 string += ",{}".format(self.frozen_swarms[swarm_name].Values[particle_index])
                 string += ",{}".format(self.Hierarchical_model_counter)
@@ -556,15 +613,14 @@
         """
         Save the final results to file
         """
         final_swarm_positions = np.concatenate([self.frozen_swarms[swarm_index].Points for swarm_index in list(self.frozen_swarms.keys())])
         final_swarm_values = np.concatenate(np.array([self.frozen_swarms[swarm_index].Values for swarm_index in list(self.frozen_swarms.keys())]))
         final_swarm_positions_filename = os.path.join(self.Output, "final_swarm_positions.txt")
         final_swarm_values_filename = os.path.join(self.Output, "final_swarm_values.txt")
-        final_swarm_values_filename = os.path.join(self.Output, "final_swarm_values.txt")
 
         np.savetxt(final_swarm_positions_filename,final_swarm_positions)
         np.savetxt(final_swarm_values_filename,final_swarm_values)
 
         final_swarm_pickle_filename= os.path.join(self.Output, "final_swarm_pickle.pkl")
         # Dump final swarms into a pickle file
         pickle.dump(self.frozen_swarms.copy(), open(final_swarm_pickle_filename, "wb"))
@@ -581,15 +637,15 @@
 
 
     def check_hierarchical_step(self):
         """
         Checks if any of the swarms meet the condition to switch to the next model
         """
 
-
+        # If all swarms are not stalled yet
         if self.AllStalled == False:
 
             for swarm_index, Swarm_ in zip(list(self.Swarms.keys()),list(self.Swarms.values())):
 
                 # If the mean of the spreads computed across the last 10 iterations has not gotten lower,
                 #   Assume the swarm has stalled and thus conduct a hierarchical step
 
@@ -621,26 +677,29 @@
                     print('\n All swarms stalled! Switching segments from ', str(self.Hierarchical_models[self.Hierarchical_model_counter].segment_number),
                           ' to ', str(self.Hierarchical_models[self.Hierarchical_model_counter+1].segment_number))
                     self.Reallocate_particles()
 
 
     def stall_condition(self,Swarm):
         """
-        Evaluate stall condition for a given swarm
+        Evaluate stall condition for a given swarm.
+
+        Current stall condition is the best swarm value has not increased more than a tolerance (default of 0.01)
+        in the last some number of iterations (defaults to 50). Swarm also stalls if the evolution counter goes over
+        the maximum number of iterations per step.
         """
-        stalled = (((np.mean(Swarm.Spreads[-20:-10]) <= np.mean(Swarm.Spreads[-10:])) and
-         # all(element == Swarm.FuncHistory[-20] for element in Swarm.FuncHistory[-20:]))
-                   (np.abs(Swarm.FuncHistory[-1] - Swarm.FuncHistory[-20]) < 0.01*np.abs(Swarm.FuncHistory[-20]))) or
-                    (Swarm.EvolutionCounter >=  self.Maximum_number_of_iterations_per_step ))
+        stalled = ((np.abs(Swarm.BestKnownSwarmValue - Swarm.FuncHistory[-self.Convergence_testing_num_iterations]) < self.Tol) or
+                    (Swarm.EvolutionCounter >= self.Maximum_number_of_iterations_per_step))
+
         return stalled
 
 
     def Run(self):
         """
-        Run optmisation/sampling for all swarms
+        Run optimisation/sampling for all swarms
         """
         if self.SaveEvolution and self.EvolutionCounter==0:
             self.CreateEvolutionHistoryFile()
             self.SaveEnsembleEvolution()
 
         while self.ContinueCondition() and (self.swarm_stepping_done == False):
             self.EvolveSwarms()
```

### Comparing `EnsembleParticleSwarmOptimization-0.1.0/PySO/MWE_Swarm.py` & `EnsembleParticleSwarmOptimization-0.1.1/PySO/MWE_Swarm.py`

 * *Files identical despite different names*

### Comparing `EnsembleParticleSwarmOptimization-0.1.0/PySO/Model.py` & `EnsembleParticleSwarmOptimization-0.1.1/PySO/Model.py`

 * *Files identical despite different names*

### Comparing `EnsembleParticleSwarmOptimization-0.1.0/PySO/SwarmHandler.py` & `EnsembleParticleSwarmOptimization-0.1.1/PySO/SwarmHandler.py`

 * *Files identical despite different names*

### Comparing `EnsembleParticleSwarmOptimization-0.1.0/setup.py` & `EnsembleParticleSwarmOptimization-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="EnsembleParticleSwarmOptimization",
-    version="0.1.0",
+    version="0.1.1",
     author="Christopher Moore and Diganta Bandopadhyay",
     author_email="diganta@star.sr.bham.ac.uk",
     description="Ensemble of particle swarms together with various velocity rules for function optimization",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dig07/PySO",
     packages=setuptools.find_packages(),
```

