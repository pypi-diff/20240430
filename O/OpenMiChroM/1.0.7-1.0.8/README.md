# Comparing `tmp/OpenMiChroM-1.0.7.tar.gz` & `tmp/OpenMiChroM-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpenMiChroM-1.0.7.tar", last modified: Tue Jun 27 17:12:58 2023, max compression
+gzip compressed data, was "OpenMiChroM-1.0.8.tar", last modified: Tue Apr 30 20:18:35 2024, max compression
```

## Comparing `OpenMiChroM-1.0.7.tar` & `OpenMiChroM-1.0.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-06-27 17:12:58.727846 OpenMiChroM-1.0.7/
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     1131 2023-06-27 17:12:29.000000 OpenMiChroM-1.0.7/LICENSE
--rw-rw-r--   0 antonio   (1000) antonio   (1000)       37 2023-06-27 17:12:29.000000 OpenMiChroM-1.0.7/MANIFEST.in
-drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-06-27 17:12:58.727846 OpenMiChroM-1.0.7/OpenMiChroM/
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    98399 2023-06-27 17:12:29.000000 OpenMiChroM-1.0.7/OpenMiChroM/ChromDynamics.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    23952 2023-06-27 17:12:29.000000 OpenMiChroM-1.0.7/OpenMiChroM/CndbTools.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     2541 2023-06-27 17:12:29.000000 OpenMiChroM-1.0.7/OpenMiChroM/Integrators.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)    36993 2023-06-27 17:12:29.000000 OpenMiChroM-1.0.7/OpenMiChroM/Optimization.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      153 2023-06-27 17:12:29.000000 OpenMiChroM-1.0.7/OpenMiChroM/__init__.py
-drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-06-27 17:12:58.727846 OpenMiChroM-1.0.7/OpenMiChroM/share/
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      517 2023-06-27 17:12:29.000000 OpenMiChroM-1.0.7/OpenMiChroM/share/MiChroM.ff
-drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-06-27 17:12:58.727846 OpenMiChroM-1.0.7/OpenMiChroM.egg-info/
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     5691 2023-06-27 17:12:58.000000 OpenMiChroM-1.0.7/OpenMiChroM.egg-info/PKG-INFO
--rw-rw-r--   0 antonio   (1000) antonio   (1000)      476 2023-06-27 17:12:58.000000 OpenMiChroM-1.0.7/OpenMiChroM.egg-info/SOURCES.txt
--rw-rw-r--   0 antonio   (1000) antonio   (1000)        1 2023-06-27 17:12:58.000000 OpenMiChroM-1.0.7/OpenMiChroM.egg-info/dependency_links.txt
--rw-rw-r--   0 antonio   (1000) antonio   (1000)       50 2023-06-27 17:12:58.000000 OpenMiChroM-1.0.7/OpenMiChroM.egg-info/entry_points.txt
--rw-rw-r--   0 antonio   (1000) antonio   (1000)       41 2023-06-27 17:12:58.000000 OpenMiChroM-1.0.7/OpenMiChroM.egg-info/requires.txt
--rw-rw-r--   0 antonio   (1000) antonio   (1000)       18 2023-06-27 17:12:58.000000 OpenMiChroM-1.0.7/OpenMiChroM.egg-info/top_level.txt
--rw-rw-r--   0 antonio   (1000) antonio   (1000)        1 2023-06-27 17:12:34.000000 OpenMiChroM-1.0.7/OpenMiChroM.egg-info/zip-safe
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     5691 2023-06-27 17:12:58.727846 OpenMiChroM-1.0.7/PKG-INFO
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     5089 2023-06-27 17:12:56.000000 OpenMiChroM-1.0.7/README.rst
--rw-rw-r--   0 antonio   (1000) antonio   (1000)       38 2023-06-27 17:12:58.727846 OpenMiChroM-1.0.7/setup.cfg
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     1254 2023-06-27 17:12:29.000000 OpenMiChroM-1.0.7/setup.py
-drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2023-06-27 17:12:58.727846 OpenMiChroM-1.0.7/tests/
--rw-rw-r--   0 antonio   (1000) antonio   (1000)        0 2023-06-27 17:12:29.000000 OpenMiChroM-1.0.7/tests/__init__.py
--rw-rw-r--   0 antonio   (1000) antonio   (1000)     2799 2023-06-27 17:12:29.000000 OpenMiChroM-1.0.7/tests/tests.py
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2024-04-30 20:18:35.850342 OpenMiChroM-1.0.8/
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     1131 2024-04-30 20:17:14.000000 OpenMiChroM-1.0.8/LICENSE
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)       37 2024-04-30 20:17:14.000000 OpenMiChroM-1.0.8/MANIFEST.in
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2024-04-30 20:18:35.846342 OpenMiChroM-1.0.8/OpenMiChroM/
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    99037 2024-04-30 20:17:14.000000 OpenMiChroM-1.0.8/OpenMiChroM/ChromDynamics.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    24237 2024-04-30 20:17:14.000000 OpenMiChroM-1.0.8/OpenMiChroM/CndbTools.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     2914 2024-04-30 20:17:14.000000 OpenMiChroM-1.0.8/OpenMiChroM/Integrators.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    40515 2024-04-30 20:17:14.000000 OpenMiChroM-1.0.8/OpenMiChroM/Optimization.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      202 2024-04-30 20:17:14.000000 OpenMiChroM-1.0.8/OpenMiChroM/__init__.py
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2024-04-30 20:18:35.846342 OpenMiChroM-1.0.8/OpenMiChroM/share/
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      517 2024-04-30 20:17:14.000000 OpenMiChroM-1.0.8/OpenMiChroM/share/MiChroM.ff
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2024-04-30 20:18:35.846342 OpenMiChroM-1.0.8/OpenMiChroM.egg-info/
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     5691 2024-04-30 20:18:35.000000 OpenMiChroM-1.0.8/OpenMiChroM.egg-info/PKG-INFO
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      476 2024-04-30 20:18:35.000000 OpenMiChroM-1.0.8/OpenMiChroM.egg-info/SOURCES.txt
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)        1 2024-04-30 20:18:35.000000 OpenMiChroM-1.0.8/OpenMiChroM.egg-info/dependency_links.txt
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)       50 2024-04-30 20:18:35.000000 OpenMiChroM-1.0.8/OpenMiChroM.egg-info/entry_points.txt
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)       41 2024-04-30 20:18:35.000000 OpenMiChroM-1.0.8/OpenMiChroM.egg-info/requires.txt
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)       18 2024-04-30 20:18:35.000000 OpenMiChroM-1.0.8/OpenMiChroM.egg-info/top_level.txt
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)        1 2024-04-30 20:17:40.000000 OpenMiChroM-1.0.8/OpenMiChroM.egg-info/zip-safe
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     5691 2024-04-30 20:18:35.850342 OpenMiChroM-1.0.8/PKG-INFO
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     5089 2024-04-30 20:18:31.000000 OpenMiChroM-1.0.8/README.rst
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)       38 2024-04-30 20:18:35.850342 OpenMiChroM-1.0.8/setup.cfg
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     1254 2024-04-30 20:17:14.000000 OpenMiChroM-1.0.8/setup.py
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2024-04-30 20:18:35.850342 OpenMiChroM-1.0.8/tests/
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)        0 2024-04-30 20:17:14.000000 OpenMiChroM-1.0.8/tests/__init__.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     2799 2024-04-30 20:17:14.000000 OpenMiChroM-1.0.8/tests/tests.py
```

### Comparing `OpenMiChroM-1.0.7/LICENSE` & `OpenMiChroM-1.0.8/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2020-2023 The Center for Theoretical Biological Physics (CTBP) - Rice University
+Copyright (c) 2020-2024 The Center for Theoretical Biological Physics (CTBP) - Rice University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `OpenMiChroM-1.0.7/OpenMiChroM/ChromDynamics.py` & `OpenMiChroM-1.0.8/OpenMiChroM/ChromDynamics.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
         import simtk.openmm as openmm
         import simtk.unit as units  
 except:
     print('Failed to load OpenMM. Check your configuration.')
 
 
 from sys import stdout
+import warnings
 import numpy as np
 from six import string_types
 import os
 import time
 import random
 import h5py
 import pandas as pd
@@ -330,24 +331,25 @@
         R"""
         Runs automatically to offset the positions if it is an integer (int) variable.
         """
         data = self.getPositions()
         data = data + np.random.randn(*data.shape) * 0.0001
         self.setPositions(data)
         
+
     def getLoops(self, looplists):
         R"""
         Get the loop position (CTFC anchor points) for each chromosome.
         
         .. note:: For Multi-chain simulations, the ordering of the loop list files is important! The order of the files should be the same as used in the other functions.
 
         Args:
 
-            looplists (text file): 
-                A two-column text file containing the index *i* and *j* of a loci pair that form loop interactions.
+            looplists (list[str]): 
+                List with the names of the files containing loop information. Each file should be a two-column text file containing the index *i* and *j* of the loci pairs that forms the loop anchors.
         """
         self.loopPosition = []
         for file, chain in zip(looplists,self.chains):
             aFile = open(file,'r')
             pos = aFile.read().splitlines()
             m = int(chain[0])
             for t in range(len(pos)):
@@ -681,18 +683,21 @@
 
             mu (float, required):
                 Parameter in the probability of crosslink function. (Default value = 3.22).
             rc (float, required):
                 Parameter in the probability of crosslink function, :math:`f(rc) = 0.5`. (Default value = 1.78).
             X (float, required):
                 Loop interaction parameter. (Default value = -1.612990).
-            looplists (file, optional):
-                A two-column text file containing the index *i* and *j* of a loci pair that form loop interactions. (Default value: :code:`None`).
+            looplists (list[str], required): 
+                List with the names of the files containing loop information. Each file should be a two-column text file containing the index *i* and *j* of the loci pairs that forms the loop anchors. (Default value: :code:`None`).
         """
-            
+        
+        if isinstance(looplists, str):
+            looplists = [looplists]
+
         ELoop = "qsi*0.5*(1. + tanh(mu*(rc - r)))"
                 
         Loop = self.mm.CustomBondForce(ELoop)
         
         Loop.addGlobalParameter('mu', mu)  
         Loop.addGlobalParameter('rc', rc) 
         Loop.addGlobalParameter('qsi', X) 
@@ -1069,39 +1074,50 @@
         """
 
         forceName = "FlatBottomHarmonic"
 
         self.removeForce(forceName)
 
 
-    def addAdditionalForce(self, forceFunction, **args):
+    def addAdditionalForce(self, forceFunction, *args, **kwargs):
         R"""
         Add an additional force after the system has already been initialized.
 
         Args:
 
             forceFunciton (function, required):
                 Force function to be added. Example: addSphericalConfinementLJ
             **args (collection of arguments, required):
                 Arguments of the function to add the force. Consult respective documentation.
         """
         
-        assert isinstance(forceFunction, types.MethodType), f"No function with name {forceFunction}! \
-                                                You can only add functions that are defined as a method of the simulation object"
+        # warning for user defined force function
+        if not isinstance(forceFunction, types.MethodType):
+            warnings.warn("Using user defined force function. Make sure to include the new force object in the MiChroM.forceDict dictionary.")
+
         #store old forcedict keys
         oldForceDictKeys = list(self.forceDict.keys())
         
         # call the function --  
         # the force name is added to the forceDict but not yet added to the system
-        forceFunction(**args)
+        forceFunction(*args, **kwargs)
 
         # find the new forceDict name
-        newForceDictKey_list = list(set(oldForceDictKeys)^set(self.forceDict.keys()))
-        assert len(newForceDictKey_list)==1, "The force you are adding is already present! Try removing it first and then add"
-        newForceDictKey = newForceDictKey_list[0]
+        newKeys = list(set(oldForceDictKeys)^set(self.forceDict.keys()))
+        
+        try:
+            newForceDictKey = newKeys.pop()
+        except:
+            newForceDictKey = None
+        finally:
+            if newForceDictKey is None:
+                raise ValueError("No new force in MiChroM.forceDict! The new force is either already present or was not added properly to the force dictionary.")
+            if newKeys:
+                raise ValueError("Force function added multiple new forces in MiChroM! Please break down the function so each force is added separately.")
+        
         force = self.forceDict[newForceDictKey]
         
         # exclusion list
         exc = self.bondsForException
 
         # set all the attributes of the force (see _applyForces)
         if hasattr(force, "addException"):
@@ -2218,15 +2234,15 @@
         forceValues.append(self.context.getState(getEnergy=True).getPotentialEnergy().value_in_unit(units.kilojoules_per_mole)/self.N)
         df = pd.DataFrame(forceValues,forceNames)
         df.columns = ['Values']
         print(df)
 
     def printHeader(self):
         print('{:^96s}'.format("***************************************************************************************"))
-        print('{:^96s}'.format("**** **** *** *** *** *** *** *** OpenMiChroM-1.0.7 *** *** *** *** *** *** **** ****"))
+        print('{:^96s}'.format("**** **** *** *** *** *** *** *** OpenMiChroM-1.0.8 *** *** *** *** *** *** **** ****"))
         print('')
         print('{:^96s}'.format("OpenMiChroM is a Python library for performing chromatin dynamics simulations."))
         print('{:^96s}'.format("OpenMiChroM uses the OpenMM Python API,"))
         print('{:^96s}'.format("employing the MiChroM (Minimal Chromatin Model) energy function."))
         print('{:^96s}'.format("The chromatin dynamics simulations generate an ensemble of 3D chromosomal structures"))
         print('{:^96s}'.format("that are consistent with experimental Hi-C maps, also allows simulations of a single"))
         print('{:^96s}'.format("or multiple chromosome chain using High-Performance Computing "))
@@ -2237,11 +2253,11 @@
         print('{:^96s}'.format("A Scalable Computational Approach for Simulating Complexes of Multiple Chromosomes."))
         print('{:^96s}'.format("Journal of Molecular Biology. doi:10.1016/j.jmb.2020.10.034."))
         print('{:^96s}'.format("and"))
         print('{:^96s}'.format("Oliveira Junior, A. B. et al."))
         print('{:^96s}'.format("Chromosome Modeling on Downsampled Hi-C Maps Enhances the Compartmentalization Signal."))
         print('{:^96s}'.format("J. Phys. Chem. B, doi:10.1021/acs.jpcb.1c04174."))
         print('')
-        print('{:^96s}'.format("Copyright (c) 2023, The OpenMiChroM development team at"))
+        print('{:^96s}'.format("Copyright (c) 2024, The OpenMiChroM development team at"))
         print('{:^96s}'.format("Rice University"))
         print('{:^96s}'.format("***************************************************************************************"))
         stdout.flush()
```

### Comparing `OpenMiChroM-1.0.7/OpenMiChroM/CndbTools.py` & `OpenMiChroM-1.0.8/OpenMiChroM/CndbTools.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         f_name, file_extension = os.path.splitext(filename)
         
         if file_extension == ".ndb":
             filename = self.ndb2cndb(f_name)   
 
         self.cndb = h5py.File(filename, 'r')
         
-        self.ChromSeq = list(self.cndb['types'].asstr())
+        self.ChromSeq = list(self.cndb['types'])
         self.uniqueChromSeq = set(self.ChromSeq)
         
         self.dictChromSeq = {}
         
         for tt in self.uniqueChromSeq:
             self.dictChromSeq[tt] = ([i for i, e in enumerate(self.ChromSeq) if e == tt])
         
@@ -443,24 +443,26 @@
         bin_mids=0.5*(bin_edges[:-1] + bin_edges[1:])
         bin_vols = (4/3)*np.pi*(bin_edges[1:]**3 - bin_edges[:-1]**3)
         num_density = rdp_hist/(xyz.shape[0]*bin_vols)
 
         return (num_density, bin_mids)
 
         
-    def compute_RDP(self, xyz, radius=20.0, bins=200):
+    def compute_RDP(self, xyz, beadSelection=None, radius=20.0, bins=200):
         R"""
         Calculates the RDP - Radial Distribution Probability. Details can be found in the following publications: 
         
             - Oliveira Jr., A.B., Contessoto, V.G., Mello, M.F. and Onuchic, J.N., 2021. A scalable computational approach for simulating complexes of multiple chromosomes. Journal of Molecular Biology, 433(6), p.166700.
             - Di Pierro, M., Zhang, B., Aiden, E.L., Wolynes, P.G. and Onuchic, J.N., 2016. Transferable model for chromosome architecture. Proceedings of the National Academy of Sciences, 113(43), pp.12168-12173.
         
         Args:
-            xyz (:math:`(frames, beadSelection, XYZ)` :class:`numpy.ndarray`, required):
-                Array of the 3D position of the selected beads for different frames extracted by using the :code: `xyz()` function. 
+            xyz (:math:`(frames, XYZ)` :class:`numpy.ndarray`, required):
+                Array of the 3D position of the frames extracted by using the :code: `xyz()` function. 
+            beadSelection (:math:`(beadSelection)` :class:`numpy.ndarray`):
+                The index of the beads to be sliced from `xyz` that you want to compute RDP. Usualy, you can use the internal selection using the :code: `dictChromSeq['types']` with 'types' been the selection that you want. 
             radius (float, required):
                 Radius of the sphere in units of :math:`\sigma` to be considered in the calculations. The radius value should be modified depending on your simulated chromosome length. (Default value = 20.0).
             bins (int, required):
                 Number of slices to be considered as spherical shells. (Default value = 200).
                        
         Returns:
             :math:`(N, 1)` :class:`numpy.ndarray`:
@@ -501,15 +503,15 @@
         n_frames = 0 
         g_rdf = np.zeros(bins)
  
         for i in range(len(xyz)):
             frame = xyz[i]
             centroide = np.mean(frame, axis=0)[None,:][0]
             n_frames += 1
-            g_rdf += calc_gr(centroide, frame, R_nucleus, deltaR)
+            g_rdf += calc_gr(centroide, frame[beadSelection], R_nucleus, deltaR)
         
         Rx = []   
         for i in np.arange(0, int(R_nucleus+deltaR), deltaR):
             Rx.append(i)
         return(Rx, g_rdf/n_frames) 
 
     def traj2HiC(self, xyz, mu=3.22, rc = 1.78):
@@ -544,8 +546,8 @@
                 print("Reading frame {:} of {:}".format(i, len(xyz)))
         
         return(np.divide(P , Ntotal))    
             
         
     def __repr__(self):
         return '<{0}.{1} object at {2}>\nCndb file has {3} frames, with {4} beads and {5} types '.format(
-      self.__module__, type(self).__name__, hex(id(self)), self.Nframes, self.Nbeads, self.uniqueChromSeq)
+      self.__module__, type(self).__name__, hex(id(self)), self.Nframes, self.Nbeads, self.uniqueChromSeq)
```

### Comparing `OpenMiChroM-1.0.7/OpenMiChroM/Integrators.py` & `OpenMiChroM-1.0.8/OpenMiChroM/Integrators.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,14 +7,19 @@
 Hence velocity v of a monomer represents the active force f = gamma * v.
 """
 
 #import modules
 import openmm as omm
 
 class ActiveBrownianIntegrator(omm.CustomIntegrator):
+    R"""
+    The :class:`~.ActiveBrownianIntegrator` class is a custom Brownian integrator. Just like all Brownian integrators there are no velocities, there are only forces and displacements.
+    Here we use the velocities as a proxy to keep track of the active force for each monomer. 
+    Hence velocity v of a monomer represents the active force f = gamma * v.
+    """
     def __init__(self,
                 timestep=0.001, 
                 temperature=120.0,
                 collision_rate=1.0,
                 corr_time=10.0,
                 constraint_tolerance=1e-8,
                  ):
```

### Comparing `OpenMiChroM-1.0.7/OpenMiChroM/Optimization.py` & `OpenMiChroM-1.0.8/OpenMiChroM/Optimization.py`

 * *Files 2% similar despite different names*

```diff
@@ -662,28 +662,123 @@
         return phi
     
     def get_PiPj_sim_IC(self):
         R"""
         Normalizes the cross term of the Hessian by the number of frames in the simulation for the Ideal Chromosome optimization.
         """
         return self.PiPj_IC/self.Nframes
-    
-    def get_HiC_exp(self, filename):
+
+    def knight_ruiz_balance(self,matrix, tol=1e-5, max_iter=100):
+        R"""
+        Perform the Knight-Ruiz matrix balancing.
+        """
+        A = np.array(matrix, dtype=float)
+        n = A.shape[0]
+        row_scaling = np.ones(n)
+        col_scaling = np.ones(n)
+
+        for _ in range(max_iter):
+            row_scaling = np.sqrt(np.sum(A, axis=1))
+            A /= row_scaling[:, None]
+            col_scaling = np.sqrt(np.sum(A, axis=0))
+            A /= col_scaling
+
+            if np.all(np.abs(row_scaling - 1) < tol) and np.all(np.abs(col_scaling - 1) < tol):
+                break
+
+        return A
+
+
+    def normalize_matrix(self,matrix):
+        R"""
+        Normalize the matrix for simulation optimization. Here the first neighbor should have the probability of contact P=1.0.
+        """
+        matrix = np.nan_to_num(matrix, nan=0, posinf=0, neginf=0)
+        np.fill_diagonal(matrix,0.0)
+
+        max_values = np.amax(np.triu(matrix), axis=1)
+        
+        # To avoid division by zero, replace zeros with ones
+        max_values[max_values == 0] = 0.0000001
+        
+        normalized_matrix = np.triu(matrix) / max_values[:, np.newaxis]
+        # return normalized_matrix
+        matrix= normalized_matrix + np.triu(normalized_matrix,k=1).T
+        np.fill_diagonal(matrix,1.0)
+
+        return matrix
+
+
+    def get_HiC_exp(self, HiC, centerRemove=False, centrange=[0,0], norm=False, cutoff_low=0.0, cutoff_high=1.0, KR=False, neighbors=0):
         R"""
         Receives the experimental Hi-C map (Full dense matrix) in a text format and performs the data normalization from Hi-C frequency/counts/reads to probability.
+        
+        Args:
+            HiC (file, required):
+                Experimental Hi-C map (Full dense matrix) in a text format.
+            centerRemove (bool, optional):
+                Whether to set the contact probability of the centromeric region to zero. (Default value: :code:`False`).
+            centrange (list, required if **centerRemove** = :code:`True`)):
+                Range of the centromeric region, *i.e.*, :code:`centrange=[i,j]`, where *i* and *j*  are the initial and final beads in the centromere. (Default value = :code:`[0,0]`).
+            cutoff (float, optional):
+                Cutoff value for reducing the noise in the original data. Values lower than the **cutoff** are considered :math:`0.0`.
         """
-        allmap = np.loadtxt(filename)
 
-        r=np.triu(allmap, k=1)
-        r[np.isinf(r)]= 0.0
-        r[np.isnan(r)]= 0.0
-        r = normalize(r, axis=1, norm='max')
-        rd = np.transpose(r)
-        self.expHiC = r+rd + np.diag(np.ones(len(r)))
-        self.expHiC[self.expHiC<self.cutoff] = 0.0
+        # get the file extension
+        _, file_extension = os.path.splitext(HiC)
+        if file_extension == '.npy':
+            # use np.load if the file is a .npy file
+            allmap = np.load(HiC)
+        else:
+            allmap = np.loadtxt(HiC)
+
+        if KR==True:
+            allmap = knight_ruiz_balance(allmap)
+
+        if norm==True:
+            r=normalize_matrix(allmap)
+
+            for i in range(len(r)-1):
+                maxElem = r[i][i+1]
+                if (maxElem != np.max(r[i])):
+                    for j in range(len(r[i])):
+                        if maxElem != 0.0:
+                            r[i][j] = float(r[i][j] / maxElem)
+                        else:
+                            r[i][j] = 0.0 
+                        if r[i][j] > 1.0:
+                            r[i][j] = 0.5
+
+            rd = np.transpose(r) 
+            self.expHiC = r+rd + np.diag(np.ones(len(r)))
+        else:
+            self.expHiC = allmap
+        
+        if (centerRemove):
+            centrome = range(centrange[0],centrange[1])
+            self.expHiC[centrome,:] = 0.0
+            self.expHiC[:,centrome] = 0.0
+        
+        #remove noise by cutoff 
+
+        if cutoff_low>0.0:
+            self.expHiC[self.expHiC<cutoff_low] = 0.0
+        
+        if cutoff_high<1.0:
+            self.expHiC[self.expHiC>cutoff_high] = 0.0
+
+        # Remove the number of Neighbors to optimize.
+        M=self.expHiC
+        neighbor_mask = np.abs(np.subtract.outer(np.arange(len(M)), np.arange(len(M)))) <= neighbors
+        M[neighbor_mask] = 0.0
+        self.expHiC = M
+
+        self.mask = self.expHiC == 0.0
+
+        self.phi_exp = self.expHiC
 
     def calc_phi_exp_IC(self):
         R"""
         Calculates the contact probability as a function of the genomic distance from the experimental Hi-C for the Ideal Chromosome optimization.
         """
         dmax = self.dend - self.dinit
         phi = np.zeros(dmax)
```

### Comparing `OpenMiChroM-1.0.7/OpenMiChroM/share/MiChroM.ff` & `OpenMiChroM-1.0.8/OpenMiChroM/share/MiChroM.ff`

 * *Files identical despite different names*

### Comparing `OpenMiChroM-1.0.7/OpenMiChroM.egg-info/PKG-INFO` & `OpenMiChroM-1.0.8/OpenMiChroM.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenMiChroM
-Version: 1.0.7
+Version: 1.0.8
 Summary: Open-Michrom lib for chromosome simulations
 Home-page: https://ndb.rice.edu/Open-MiChroM
 Author: Antonio Bento de Oliveira Junior,Vinicius de Godoi Contessoto
 Author-email: antonio.oliveira@rice.edu,contessoto@rice.edu
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `OpenMiChroM-1.0.7/PKG-INFO` & `OpenMiChroM-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenMiChroM
-Version: 1.0.7
+Version: 1.0.8
 Summary: Open-Michrom lib for chromosome simulations
 Home-page: https://ndb.rice.edu/Open-MiChroM
 Author: Antonio Bento de Oliveira Junior,Vinicius de Godoi Contessoto
 Author-email: antonio.oliveira@rice.edu,contessoto@rice.edu
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `OpenMiChroM-1.0.7/README.rst` & `OpenMiChroM-1.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `OpenMiChroM-1.0.7/setup.py` & `OpenMiChroM-1.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from os import path
 
 this_dir = path.abspath(path.dirname(__file__))
 with open(path.join(this_dir, "README.rst")) as f:
     long_description = f.read()
 
-__version__ = "1.0.7"
+__version__ = "1.0.8"
 for line in open(path.join("OpenMiChroM", "__init__.py")):
     if line.startswith("__version__"):
         exec(line.strip())
 
 setup(
     name="OpenMiChroM",
     version=__version__,
```

### Comparing `OpenMiChroM-1.0.7/tests/tests.py` & `OpenMiChroM-1.0.8/tests/tests.py`

 * *Files identical despite different names*

