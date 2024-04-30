# Comparing `tmp/polytensor-0.0.3.tar.gz` & `tmp/polytensor-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polytensor-0.0.3.tar", last modified: Thu Feb  1 18:04:02 2024, max compression
+gzip compressed data, was "polytensor-0.0.6.tar", last modified: Tue Apr 30 05:53:23 2024, max compression
```

## Comparing `polytensor-0.0.3.tar` & `polytensor-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 kasner    (1001) kasner    (1001)        0 2024-02-01 18:04:02.225321 polytensor-0.0.3/
--rw-r--r--   0 kasner    (1001) kasner    (1001)     1069 2024-01-25 00:20:52.000000 polytensor-0.0.3/LICENSE
--rw-r--r--   0 kasner    (1001) kasner    (1001)     8307 2024-02-01 18:04:02.225321 polytensor-0.0.3/PKG-INFO
--rw-r--r--   0 kasner    (1001) kasner    (1001)     7716 2024-01-25 00:58:47.000000 polytensor-0.0.3/README.rst
-drwxr-xr-x   0 kasner    (1001) kasner    (1001)        0 2024-02-01 18:04:02.225321 polytensor-0.0.3/polytensor/
--rw-r--r--   0 kasner    (1001) kasner    (1001)       95 2024-01-25 00:20:52.000000 polytensor-0.0.3/polytensor/__init__.py
--rw-r--r--   0 kasner    (1001) kasner    (1001)     1932 2024-01-25 00:20:52.000000 polytensor-0.0.3/polytensor/converters.py
--rw-r--r--   0 kasner    (1001) kasner    (1001)     3615 2024-01-25 00:20:52.000000 polytensor-0.0.3/polytensor/generators.py
--rw-r--r--   0 kasner    (1001) kasner    (1001)     7722 2024-02-01 18:02:59.000000 polytensor-0.0.3/polytensor/polynomial.py
--rw-r--r--   0 kasner    (1001) kasner    (1001)      550 2024-01-25 00:20:52.000000 polytensor-0.0.3/polytensor/serialize.py
-drwxr-xr-x   0 kasner    (1001) kasner    (1001)        0 2024-02-01 18:04:02.225321 polytensor-0.0.3/polytensor.egg-info/
--rw-r--r--   0 kasner    (1001) kasner    (1001)     8307 2024-02-01 18:04:02.000000 polytensor-0.0.3/polytensor.egg-info/PKG-INFO
--rw-r--r--   0 kasner    (1001) kasner    (1001)      437 2024-02-01 18:04:02.000000 polytensor-0.0.3/polytensor.egg-info/SOURCES.txt
--rw-r--r--   0 kasner    (1001) kasner    (1001)        1 2024-02-01 18:04:02.000000 polytensor-0.0.3/polytensor.egg-info/dependency_links.txt
--rw-r--r--   0 kasner    (1001) kasner    (1001)        1 2024-02-01 17:45:55.000000 polytensor-0.0.3/polytensor.egg-info/not-zip-safe
--rw-r--r--   0 kasner    (1001) kasner    (1001)      560 2024-02-01 18:04:02.000000 polytensor-0.0.3/polytensor.egg-info/requires.txt
--rw-r--r--   0 kasner    (1001) kasner    (1001)       11 2024-02-01 18:04:02.000000 polytensor-0.0.3/polytensor.egg-info/top_level.txt
--rw-r--r--   0 kasner    (1001) kasner    (1001)       38 2024-02-01 18:04:02.228654 polytensor-0.0.3/setup.cfg
--rw-r--r--   0 kasner    (1001) kasner    (1001)     1839 2024-02-01 18:03:42.000000 polytensor-0.0.3/setup.py
-drwxr-xr-x   0 kasner    (1001) kasner    (1001)        0 2024-02-01 18:04:02.225321 polytensor-0.0.3/test/
--rw-r--r--   0 kasner    (1001) kasner    (1001)      703 2024-01-25 00:20:52.000000 polytensor-0.0.3/test/testCoefficients.py
--rw-r--r--   0 kasner    (1001) kasner    (1001)     1169 2024-01-25 00:20:52.000000 polytensor-0.0.3/test/testGrad.py
--rw-r--r--   0 kasner    (1001) kasner    (1001)      525 2024-01-25 00:20:52.000000 polytensor-0.0.3/test/testHigherOrder.py
--rw-r--r--   0 kasner    (1001) kasner    (1001)     2204 2024-02-01 18:02:59.000000 polytensor-0.0.3/test/testPackage.py
+drwxr-xr-x   0 blakewilson   (501) staff       (20)        0 2024-04-30 05:53:23.786934 polytensor-0.0.6/
+-rw-r--r--   0 blakewilson   (501) staff       (20)     1069 2024-04-29 16:34:15.000000 polytensor-0.0.6/LICENSE
+-rw-r--r--   0 blakewilson   (501) staff       (20)     8364 2024-04-30 05:53:23.786737 polytensor-0.0.6/PKG-INFO
+-rw-r--r--   0 blakewilson   (501) staff       (20)     7716 2024-04-29 16:34:15.000000 polytensor-0.0.6/README.rst
+drwxr-xr-x   0 blakewilson   (501) staff       (20)        0 2024-04-30 05:53:23.784389 polytensor-0.0.6/polytensor/
+-rw-r--r--   0 blakewilson   (501) staff       (20)       95 2024-04-29 16:34:15.000000 polytensor-0.0.6/polytensor/__init__.py
+-rw-r--r--   0 blakewilson   (501) staff       (20)     1932 2024-04-29 16:34:15.000000 polytensor-0.0.6/polytensor/converters.py
+-rw-r--r--   0 blakewilson   (501) staff       (20)     3158 2024-04-29 16:34:15.000000 polytensor-0.0.6/polytensor/generators.py
+-rw-r--r--   0 blakewilson   (501) staff       (20)     7970 2024-04-30 05:46:53.000000 polytensor-0.0.6/polytensor/polynomial.py
+-rw-r--r--   0 blakewilson   (501) staff       (20)      550 2024-04-29 16:34:15.000000 polytensor-0.0.6/polytensor/serialize.py
+-rw-r--r--   0 blakewilson   (501) staff       (20)     2076 2024-04-29 16:34:15.000000 polytensor-0.0.6/polytensor/validate.py
+drwxr-xr-x   0 blakewilson   (501) staff       (20)        0 2024-04-30 05:53:23.786424 polytensor-0.0.6/polytensor.egg-info/
+-rw-r--r--   0 blakewilson   (501) staff       (20)     8364 2024-04-30 05:53:23.000000 polytensor-0.0.6/polytensor.egg-info/PKG-INFO
+-rw-r--r--   0 blakewilson   (501) staff       (20)      484 2024-04-30 05:53:23.000000 polytensor-0.0.6/polytensor.egg-info/SOURCES.txt
+-rw-r--r--   0 blakewilson   (501) staff       (20)        1 2024-04-30 05:53:23.000000 polytensor-0.0.6/polytensor.egg-info/dependency_links.txt
+-rw-r--r--   0 blakewilson   (501) staff       (20)        1 2024-04-30 05:30:36.000000 polytensor-0.0.6/polytensor.egg-info/not-zip-safe
+-rw-r--r--   0 blakewilson   (501) staff       (20)       27 2024-04-30 05:53:23.000000 polytensor-0.0.6/polytensor.egg-info/requires.txt
+-rw-r--r--   0 blakewilson   (501) staff       (20)       11 2024-04-30 05:53:23.000000 polytensor-0.0.6/polytensor.egg-info/top_level.txt
+-rw-r--r--   0 blakewilson   (501) staff       (20)       38 2024-04-30 05:53:23.786970 polytensor-0.0.6/setup.cfg
+-rw-r--r--   0 blakewilson   (501) staff       (20)     1064 2024-04-30 05:51:15.000000 polytensor-0.0.6/setup.py
+drwxr-xr-x   0 blakewilson   (501) staff       (20)        0 2024-04-30 05:53:23.786088 polytensor-0.0.6/test/
+-rw-r--r--   0 blakewilson   (501) staff       (20)      703 2024-04-29 16:34:15.000000 polytensor-0.0.6/test/testCoefficients.py
+-rw-r--r--   0 blakewilson   (501) staff       (20)     1169 2024-04-29 16:34:15.000000 polytensor-0.0.6/test/testGrad.py
+-rw-r--r--   0 blakewilson   (501) staff       (20)      525 2024-04-29 16:34:15.000000 polytensor-0.0.6/test/testHigherOrder.py
+-rw-r--r--   0 blakewilson   (501) staff       (20)     2233 2024-04-30 05:32:02.000000 polytensor-0.0.6/test/testPackage.py
+-rw-r--r--   0 blakewilson   (501) staff       (20)     1905 2024-04-29 16:34:15.000000 polytensor-0.0.6/test/testSparseDense.py
```

### Comparing `polytensor-0.0.3/LICENSE` & `polytensor-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `polytensor-0.0.3/PKG-INFO` & `polytensor-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: polytensor
-Version: 0.0.3
+Version: 0.0.6
 Home-page: 
 Author: Blake Wilson
 Author-email: wilso692@purdue.edu
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy>=1.25.0
+Requires-Dist: torch>=2.0.0
 
 .. PolyTensor documentation master file, created by
    sphinx-quickstart on Fri Dec 22 09:52:54 2023.
    You can adapt this file completely to your liking, but it should at least
    contain the root `toctree` directive.
 
 .. image:: ./docs/source/_static/icon/moonrabbit.svg
```

### Comparing `polytensor-0.0.3/README.rst` & `polytensor-0.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `polytensor-0.0.3/polytensor/converters.py` & `polytensor-0.0.6/polytensor/converters.py`

 * *Files identical despite different names*

### Comparing `polytensor-0.0.3/polytensor/generators.py` & `polytensor-0.0.6/polytensor/generators.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,14 @@
 import torch
 import random
-import networkx as nx
 from beartype import beartype
 from beartype.typing import List, Callable, Union
 from collections.abc import Iterable
 
 
-def from_networkx(g: nx.Graph, key="weight"):
-    """
-    Converts a networkx graph to a dictionary of terms for a polynomial.
-
-    Args:
-        g : Networkx graph
-        key : Attribute to use for the value of the term
-    """
-    terms = {}
-    for node in list(g.nodes(data=key)):
-        if node[1] is None:
-            raise ValueError(
-                f"Node {node} must have non-None value for attribute {key}"
-            )
-        if node[1] != 0:
-            terms[tuple([node[0]])] = node[1]
-
-    # Convert edges
-    for edge in nx.to_edgelist(g):
-        if edge[1] != 0:
-            terms[edge[:2]] = edge[2]
-
-    return terms
-
-
 @beartype
 def random_combination_generator(iterable: Iterable, k: int):
     """
     Generates random, unique combinations of size k from the iterable.
 
     Source: https://stackoverflow.com/questions/22229796/choose-at-random-from-combinations
 
@@ -90,15 +64,17 @@
     for i, nt in enumerate(num_terms):
         terms.update(
             coeffRandomSampler(n=n, num_terms=nt, degree=i + 1, sample_fn=sample_fn)
         )
     return terms
 
 
-def denseFromSparse(coeffs: dict, num_bits: Union[int, None] = None):
+def denseFromSparse(
+    coeffs: dict, num_bits: Union[int, None] = None, device="cpu", dtype=torch.float
+):
     """
     Generates the coefficients for a dense polynomial from a sparse represention.
 
     Parameters:
         coeffs : Degree of the polynomial
 
     Returns:
@@ -111,25 +87,27 @@
         deg = max(len(k), deg)
         n = max(n, max(k))
     n += 1
 
     if num_bits:
         n = num_bits
 
-    new_coeffs = [torch.nn.Parameter(torch.zeros(1))]
+    new_coeffs = [torch.nn.Parameter(torch.zeros(1, dtype=dtype, device=device))]
 
     for i in range(1, deg + 1):
-        new_coeffs.append(torch.zeros(*([n] * i)))
+        new_coeffs.append(torch.zeros(*([n] * i), dtype=dtype, device=device))
 
     for k, v in coeffs.items():
         new_coeffs[len(k)][k] = v
 
     return new_coeffs
 
 
-def dense(n: int, degree: int):
-    tensors = [torch.nn.Parameter(torch.rand([1]))]
+def dense(n: int, degree: int, device="cuda", dtype=torch.float):
+    tensors = [torch.nn.Parameter(torch.rand([1], device=device, dtype=device))]
 
     for i in range(1, degree + 1):
-        tensors.append(torch.nn.Parameter(torch.rand(*([n] * i))))
+        tensors.append(
+            torch.nn.Parameter(torch.rand(*([n] * i), device=device, dtype=device))
+        )
 
     return tensors
```

### Comparing `polytensor-0.0.3/polytensor/polynomial.py` & `polytensor-0.0.6/polytensor/polynomial.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         coefficients: :math:`s` Stored as a dictionary. Each key represents the monomial variable indices and the value is the coefficient for the term.
 
     """
 
     @beartype
     def __init__(
         self,
-        coefficients: dict[List[int], Union[complex, float, int, torch.Tensor]],
+        coefficients: dict[tuple, Union[complex, float, int, torch.Tensor]],
         device: str = "cpu",
         dtype=torch.float,
         **kwargs,
     ):
         super().__init__()
 
         self.coefficients = coefficients
@@ -124,19 +124,27 @@
         self.coeff_vector = torch.nn.ParameterList()
         self.coeff_map = {}
         for i, term in enumerate(self.coefficients.keys()):
             self.coeff_map[term] = i
             if type(value) not in [torch.Tensor]:
                 self.coeff_vector.append(
                     torch.nn.Parameter(
-                        torch.tensor(self.coefficients[term], dtype=self.dtype)
+                        torch.tensor(
+                            self.coefficients[term],
+                            dtype=self.dtype,
+                            device=self.device,
+                        )
                     )
                 )
             else:
-                self.coeff_vector.append(torch.nn.Parameter(self.coefficients[term]))
+                self.coeff_vector.append(
+                    torch.nn.Parameter(
+                        self.coefficients[term].to(self.dtype).to(self.device)
+                    )
+                )
 
         return True
 
     def __repr__(self):
         return f"SparseCoefficients({self.coefficients})"
 
 
@@ -228,15 +236,15 @@
             terms = torch.nonzero(coefficients[d]).squeeze()
 
             # Check if only one term exists
             if terms.dim() == 1:
                 terms = terms.unsqueeze(0)
 
             for i in range(terms.shape[0]):
-                if (np.diff(terms[i].numpy()) < 0).all():
+                if (np.diff(terms[i].cpu().numpy()) < 0).all():
                     raise ValueError(
                         f"Coefficients {terms[i].numpy()} must be in non-decreasing order."
                     )
 
         return True
 
     def __repr__(self):
```

### Comparing `polytensor-0.0.3/polytensor/serialize.py` & `polytensor-0.0.6/polytensor/serialize.py`

 * *Files identical despite different names*

### Comparing `polytensor-0.0.3/polytensor.egg-info/PKG-INFO` & `polytensor-0.0.6/polytensor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: polytensor
-Version: 0.0.3
+Version: 0.0.6
 Home-page: 
 Author: Blake Wilson
 Author-email: wilso692@purdue.edu
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy>=1.25.0
+Requires-Dist: torch>=2.0.0
 
 .. PolyTensor documentation master file, created by
    sphinx-quickstart on Fri Dec 22 09:52:54 2023.
    You can adapt this file completely to your liking, but it should at least
    contain the root `toctree` directive.
 
 .. image:: ./docs/source/_static/icon/moonrabbit.svg
```

### Comparing `polytensor-0.0.3/test/testCoefficients.py` & `polytensor-0.0.6/test/testCoefficients.py`

 * *Files identical despite different names*

### Comparing `polytensor-0.0.3/test/testGrad.py` & `polytensor-0.0.6/test/testGrad.py`

 * *Files identical despite different names*

### Comparing `polytensor-0.0.3/test/testHigherOrder.py` & `polytensor-0.0.6/test/testHigherOrder.py`

 * *Files identical despite different names*

### Comparing `polytensor-0.0.3/test/testPackage.py` & `polytensor-0.0.6/test/testPackage.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,16 @@
     for _ in range(10):
         num_bits = random.randint(5, 30)
 
         coefficients = polytensor.generators.coeffPUBORandomSampler(
             num_bits, [num_bits, 5, 5, 5], lambda: torch.rand(1)
         )
 
+        print(coefficients)
+
         p = polytensor.SparsePolynomial(coefficients)
 
         x = torch.bernoulli(torch.ones(num_bits) * 0.5)
 
         q = polytensor.DensePolynomial(
             coefficients=polytensor.generators.denseFromSparse(
                 coefficients, num_bits=num_bits
```

