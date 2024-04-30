# Comparing `tmp/diffforms-0.0.21.tar.gz` & `tmp/diffforms-0.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diffforms-0.0.21.tar", last modified: Mon Apr 29 08:52:48 2024, max compression
+gzip compressed data, was "diffforms-0.0.22.tar", last modified: Mon Apr 29 22:16:25 2024, max compression
```

## Comparing `diffforms-0.0.21.tar` & `diffforms-0.0.22.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-29 08:52:48.448162 diffforms-0.0.21/
--rwxrwxrwx   0 root         (0) root         (0)      120 2024-04-25 21:40:15.000000 diffforms-0.0.21/MANIFEST.in
--rwxrwxrwx   0 root         (0) root         (0)      538 2024-04-29 08:52:48.447636 diffforms-0.0.21/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     1479 2024-04-25 21:40:15.000000 diffforms-0.0.21/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-29 08:52:48.443853 diffforms-0.0.21/diffforms/
--rwxrwxrwx   0 root         (0) root         (0)       52 2024-04-25 21:40:15.000000 diffforms-0.0.21/diffforms/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    20230 2024-04-29 08:50:21.000000 diffforms-0.0.21/diffforms/core.py
--rwxrwxrwx   0 root         (0) root         (0)       23 2024-04-29 08:52:40.000000 diffforms-0.0.21/diffforms/release.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-29 08:52:48.447041 diffforms-0.0.21/diffforms.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      538 2024-04-29 08:52:48.000000 diffforms-0.0.21/diffforms.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      272 2024-04-29 08:52:48.000000 diffforms-0.0.21/diffforms.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-29 08:52:48.000000 diffforms-0.0.21/diffforms.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       42 2024-04-29 08:52:48.000000 diffforms-0.0.21/diffforms.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       10 2024-04-29 08:52:48.000000 diffforms-0.0.21/diffforms.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       41 2024-04-25 21:40:15.000000 diffforms-0.0.21/requirements.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2024-04-29 08:52:48.448252 diffforms-0.0.21/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      718 2024-04-25 21:40:15.000000 diffforms-0.0.21/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-29 22:16:25.161721 diffforms-0.0.22/
+-rwxrwxrwx   0 root         (0) root         (0)      120 2024-04-25 21:40:15.000000 diffforms-0.0.22/MANIFEST.in
+-rwxrwxrwx   0 root         (0) root         (0)      538 2024-04-29 22:16:25.160724 diffforms-0.0.22/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     1540 2024-04-29 22:16:05.000000 diffforms-0.0.22/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-29 22:16:25.149290 diffforms-0.0.22/diffforms/
+-rwxrwxrwx   0 root         (0) root         (0)       52 2024-04-25 21:40:15.000000 diffforms-0.0.22/diffforms/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    20224 2024-04-29 22:12:09.000000 diffforms-0.0.22/diffforms/core.py
+-rwxrwxrwx   0 root         (0) root         (0)       23 2024-04-29 22:15:09.000000 diffforms-0.0.22/diffforms/release.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-29 22:16:25.159197 diffforms-0.0.22/diffforms.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      538 2024-04-29 22:16:25.000000 diffforms-0.0.22/diffforms.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      272 2024-04-29 22:16:25.000000 diffforms-0.0.22/diffforms.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-29 22:16:25.000000 diffforms-0.0.22/diffforms.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       42 2024-04-29 22:16:25.000000 diffforms-0.0.22/diffforms.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       10 2024-04-29 22:16:25.000000 diffforms-0.0.22/diffforms.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       41 2024-04-25 21:40:15.000000 diffforms-0.0.22/requirements.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2024-04-29 22:16:25.161811 diffforms-0.0.22/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      718 2024-04-25 21:40:15.000000 diffforms-0.0.22/setup.py
```

### Comparing `diffforms-0.0.21/PKG-INFO` & `diffforms-0.0.22/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffforms
-Version: 0.0.21
+Version: 0.0.22
 Summary: Symbolic differential forms python library
 Home-page: https://github.com/Bone5505/Differential-Forms
 Author: Adam Shaw
 Keywords: differential forms,sympy,polyforms,exterior derivative
 Requires-Dist: wheel>=0.43.0
 Requires-Dist: sympy>=1.12
 Requires-Dist: ipython>=8.19.0
```

### Comparing `diffforms-0.0.21/README.md` & `diffforms-0.0.22/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 =========
 This is the list of possible implementation, in an approximate order of priority (interest to me):
 
 - [X] Differential Forms
 - [X] Exterior Product
 - [X] Simplification of Forms
 - [X] Exterior Differential Operator
-- [ ] Substitution of factors/forms
-- [ ] Vector fields
-- [ ] Generic tensor product
-- [ ] Insertion of vector fields
-- [ ] Hodge star given metric 
+- [ ] Substitution of factors/forms (In Progress)
+- [ ] Vector fields (In Progress)
+- [ ] Generic tensor product (In Progress)
+- [ ] Insertion of vector fields (In Progress)
+- [ ] Hodge star given metric/frame
 
 Dependencies
 ============
 Make sure you have the following python packages:
 
 - wheel (needed for installing through pip)
 - sympy
```

### Comparing `diffforms-0.0.21/diffforms/core.py` & `diffforms-0.0.22/diffforms/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -230,14 +230,15 @@
         return ret
     
     def __mul__(self,other): return WedgeProduct(self,other)
     
     def __rmul__(self,other): return WedgeProduct(other,self)
 
     def __div__(self,other): return WedgeProduct(self,(1/other))
+    def __truediv__(self,other): return WedgeProduct(self,(1/other))
 
     def __radd__(self,other): return self + other
     def __neg__(self):
         ret = DifferentialFormMul()
         ret.forms_list = self.forms_list
         ret.factors = [-f for f in self.factors]
         return ret
@@ -370,16 +371,14 @@
         if isinstance(target,DifferentialForm):
             new_forms_list = []
             new_factors_list = []
             for i in range(len(ret.forms_list)):
                 if target in ret.forms_list[i]:
                     j = ret.forms_list[i].index(target)
                     if isinstance(sub,DifferentialForm):
-                        print(ret.forms_list[i], sub)
-                        print([ret.forms_list[i][:j] + [sub] + ret.forms_list[i][j+1:]])
                         new_forms_list += [ret.forms_list[i][:j] + [sub] + ret.forms_list[i][j+1:]]
                         new_factors_list.append(ret.factors[i])
                     elif isinstance(sub,DifferentialFormMul):
                         for k in range(len(sub.factors)):
                             s = sub.forms_list[k]
                             f = sub.factors[k]
                             new_forms_list+= [ret.forms_list[i][:j] + s + ret.forms_list[i][j+1:]]
@@ -454,20 +453,19 @@
             L = len(self.forms_list[i])
             for perm in permutations(list(range(L)),L):
                 parity = (len(Permutation(perm).full_cyclic_form)-1)%2
                 ret.comps_list += [[self.forms_list[i][p] for p in perm]]
                 ret.factors += [(-1)**parity*self.factors[i]/factorial]
         return ret
 
-
 def d(form):
     if isinstance(form,(DifferentialForm,DifferentialFormMul)):
         return form.d
     
-    elif isinstance(form,(AtomicExpr,Function)):
+    elif isinstance(form,(AtomicExpr,Expr,Function)):
         ret = DifferentialFormMul()
         new_forms_list = []
         new_factors_list = []
         for f in form.free_symbols:
             dform = form.diff(f)
             if dform != 0:
                 new_forms_list += [[DifferentialForm(f,0).d]]
@@ -477,39 +475,39 @@
         ret.factors = new_factors_list
         return ret
 
     raise NotImplementedError
 
 def WedgeProduct(left,right):
     ret = DifferentialFormMul()
-    if isinstance(left,(int,float,Number)):
-        if isinstance(right,(int,float,Number)):
+    if isinstance(left,(int,float,Number,AtomicExpr,Expr)):
+        if isinstance(right,(int,float,Number,AtomicExpr,Expr)):
             return left*right
         elif isinstance(right,DifferentialForm):
             ret.forms_list = [[right]]
             ret.factors = [left]
         elif isinstance(right,DifferentialFormMul):
             ret.forms_list = right.forms_list
             ret.factors = [left*f for f in right.factors]
         else:
             raise NotImplementedError
     elif isinstance(left, DifferentialForm):
-        if isinstance(right,(int,float,Number)):
+        if isinstance(right,(int,float,Number,AtomicExpr,Expr)):
             ret.forms_list = [[left]]
             ret.factors = [right]
         elif isinstance(right,DifferentialForm):
             ret.forms_list = [[left,right]]
             ret.factors = [1]
         elif isinstance(right,DifferentialFormMul):
             ret.forms_list = [[left]+rf for rf in right.forms_list]
             ret.factors = right.factors
         else:
             raise NotImplementedError
     elif isinstance(left,DifferentialFormMul):
-        if isinstance(right,(int,float,Number)):
+        if isinstance(right,(int,float,Number,AtomicExpr,Expr)):
             ret.forms_list = left.forms_list
             ret.factors = [right*f for f in left.factors]
         elif isinstance(right,DifferentialForm):
             ret.forms_list = [lf+[right] for lf in left.forms_list]
             ret.factors = left.factors
         elif isinstance(right,DifferentialFormMul):
             for i in range(len(left.forms_list)):
```

### Comparing `diffforms-0.0.21/diffforms.egg-info/PKG-INFO` & `diffforms-0.0.22/diffforms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffforms
-Version: 0.0.21
+Version: 0.0.22
 Summary: Symbolic differential forms python library
 Home-page: https://github.com/Bone5505/Differential-Forms
 Author: Adam Shaw
 Keywords: differential forms,sympy,polyforms,exterior derivative
 Requires-Dist: wheel>=0.43.0
 Requires-Dist: sympy>=1.12
 Requires-Dist: ipython>=8.19.0
```

### Comparing `diffforms-0.0.21/setup.py` & `diffforms-0.0.22/setup.py`

 * *Files identical despite different names*

