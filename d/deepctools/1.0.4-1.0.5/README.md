# Comparing `tmp/deepctools-1.0.4.tar.gz` & `tmp/deepctools-1.0.5.tar.gz`

## Comparing `deepctools-1.0.4.tar` & `deepctools-1.0.5.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 deepctools-1.0.4/.pypirc
--rw-r--r--   0        0        0    22042 2020-02-02 00:00:00.000000 deepctools-1.0.4/src/deepctools/DeePCtools.py
--rw-r--r--   0        0        0    14413 2020-02-02 00:00:00.000000 deepctools-1.0.4/src/deepctools/Modeltools.py
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 deepctools-1.0.4/src/deepctools/__init__.py
--rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 deepctools-1.0.4/src/deepctools/util.py
--rw-r--r--   0        0        0     8393 2020-02-02 00:00:00.000000 deepctools-1.0.4/tests/tutorial.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 deepctools-1.0.4/.gitignore
--rw-r--r--   0        0        0    10918 2020-02-02 00:00:00.000000 deepctools-1.0.4/LICENSE
--rw-r--r--   0        0        0     7098 2020-02-02 00:00:00.000000 deepctools-1.0.4/README.md
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 deepctools-1.0.4/pyproject.toml
--rw-r--r--   0        0        0    20463 2020-02-02 00:00:00.000000 deepctools-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0    23574 2020-02-02 00:00:00.000000 deepctools-1.0.5/src/deepctools/DeePCtools.py
+-rw-r--r--   0        0        0    14413 2020-02-02 00:00:00.000000 deepctools-1.0.5/src/deepctools/Modeltools.py
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 deepctools-1.0.5/src/deepctools/__init__.py
+-rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 deepctools-1.0.5/src/deepctools/util.py
+-rw-r--r--   0        0        0    15185 2020-02-02 00:00:00.000000 deepctools-1.0.5/tests/tutorial.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 deepctools-1.0.5/.gitignore
+-rw-r--r--   0        0        0    10918 2020-02-02 00:00:00.000000 deepctools-1.0.5/LICENSE
+-rw-r--r--   0        0        0     7159 2020-02-02 00:00:00.000000 deepctools-1.0.5/README.md
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 deepctools-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0    20524 2020-02-02 00:00:00.000000 deepctools-1.0.5/PKG-INFO
```

### Comparing `deepctools-1.0.4/src/deepctools/DeePCtools.py` & `deepctools-1.0.5/src/deepctools/DeePCtools.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,31 +50,34 @@
                         Functions                |                            Usage
             initialize_DeePCsolver(uloss, opts)  |  construct DeePC solver
             initialize_RDeePCsolver(uloss, opts) |  construct Robust DeePC solver
             solver_step(uini, yini)    |  solve the optimization problem one step
          ----------------------------------------------------------------------------------------------------------
     """
 
-    def __init__(self, u_dim, y_dim, T, Tini, Np, ys, ud, yd, Q, R, us=None, lambda_g=None, lambda_y=None,
-                 ineqconidx=None, ineqconbd=None):
+    def __init__(self, u_dim, y_dim, T, Tini, Np, ud, yd, Q, R, lambda_g=None, lambda_y=None,
+                 sp_change=False, us=None, ys=None, ineqconidx=None, ineqconbd=None):
         """
             ------Initialize the system parameters and DeePC config------
                  u_dim: [int]             |  the dimension of control inputs
                  y_dim: [int]             |  the dimension of controlled outputs
                      T: [int]             |  the length of offline collected data
                   Tini: [int]             |  the initialization length of the online loop
                     Np: [int]             |  the length of predicted future trajectories
-                    us: [array]           |  set-point of u;  size (1, u_dim)
-                    ys: [array]           |  set-point of y;  size (1, y_dim)
                     ud: [array]           |  history data collected offline to construct Hankel matrix; size (T, u_dim)
                     yd: [array]           |  history data collected offline to construct Hankel matrix; size (T, u_dim)
                      Q: [array]           |  the weighting matrix of controlled outputs y
                      R: [array]           |  the weighting matrix of control inputs u
               lambda_y: [array]           |  the weighting matrix of mismatch of controlled output y
               lambda_g: [array]           |  the weighting matrix of norm of operator g
+             sp_change: [bool]            |  whether the set-point of u and y change during control, 
+                                          |      if True, uref, yref will be parameters of the optimization problem
+                                          |      if False, can just give ys, us
+                    us: [array]           |  set-point of u;  size (1, u_dim), if sp_change=False, can just define us, ys
+                    ys: [array]           |  set-point of y;  size (1, y_dim), if sp_change=False, can just define us, ys
             ineqconidx: [dict|[str,list]] |  specify the wanted constraints for u and y, if None, no constraints
                                           |      e.g., only have constraints on u2, u3, {'u': [1,2]}; 'y' as well
              ineqconbd: [dict|[str,list]] |  specify the bounds for u and y, should be consistent with "ineqconidx"
                                           |      e.g., bound on u2, u3, {'lbu': [1,0], 'ubu': [10,5]}; lby, uby as well
         """
 
         self.u_dim = u_dim
@@ -85,18 +88,21 @@
         self.g_dim = T - Tini - Np + 1
         self.Q = Q
         self.R = R
         self.lambda_g = lambda_g
         self.lambda_y = lambda_y
         self.us = us
         self.ys = ys
-        self.yref = np.tile(ys, (Np, 1)).reshape(-1, 1)
-        self.uref = None
-        if us.any():
-            self.uref = np.tile(us, (Np, 1)).reshape(-1, 1)
+        self.sp_change = sp_change
+        if not sp_change:
+            self.yref = np.tile(ys, (Np, 1)).reshape(-1, 1)
+            if us.any():
+                self.uref = np.tile(us, (Np, 1)).reshape(-1, 1)
+            else:
+                self.uref = None
 
         self.Hud = util.hankel(ud, Tini + Np)
         self.Hyd = util.hankel(yd, Tini + Np)
         self.Up = self.Hud[:self.u_dim * self.Tini, :]
         self.Uf = self.Hud[self.u_dim * self.Tini:, :]
         self.Yp = self.Hyd[:self.y_dim * self.Tini, :]
         self.Yf = self.Hyd[self.y_dim * self.Tini:, :]
@@ -125,25 +131,26 @@
             Uf, Yf             |  (dim*Np, T-L+1)
             uref, yref         |  (dim*Np, 1)
             Q, R               |  (dim*Np, dim*Np)
             lambda_g           |  (T-L+1, T-L+1)
             lambda_y           |  (dim*Tini, dim*Tini)
             ------------------------------------------------------------
             Persistently Excitation condition:
-                g_dim >= u_dim * (Tini + Np): to satisfy
-                and the Hankel matrix of ud should be full row rank
-                which is u_dim * (Tini + Np)
+                1. g_dim >= u_dim * (Tini + Np)
+                2. the Hankel matrix of ud should be full row rank
+                   which is u_dim * (Tini + Np)
             ------------------------------------------------------------
         """
         self._checkshape(self.Up, tuple([self.u_dim * self.Tini, self.g_dim]))
         self._checkshape(self.Yp, tuple([self.y_dim * self.Tini, self.g_dim]))
         self._checkshape(self.Uf, tuple([self.u_dim * self.Np, self.g_dim]))
         self._checkshape(self.Yf, tuple([self.y_dim * self.Np, self.g_dim]))
-        self._checkshape(self.uref, tuple([self.u_dim * self.Np, 1]))
-        self._checkshape(self.yref, tuple([self.y_dim * self.Np, 1]))
+        if not self.sp_change:
+            self._checkshape(self.uref, tuple([self.u_dim * self.Np, 1]))
+            self._checkshape(self.yref, tuple([self.y_dim * self.Np, 1]))
         self._checkshape(self.Q, tuple([self.y_dim * self.Np, self.y_dim * self.Np]))
         self._checkshape(self.R, tuple([self.u_dim * self.Np, self.u_dim * self.Np]))
         self._checkshape(self.lambda_g, tuple([self.g_dim, self.g_dim]))
         self._checkshape(self.lambda_y, tuple([self.y_dim * self.Tini, self.y_dim * self.Tini]))
 
         # Check PE condition
         if self.g_dim < self.u_dim * (self.Tini + self.Np):
@@ -155,14 +162,15 @@
 
     def _checkshape(self, x, x_shape):
         """Check if the variable has the correct shape"""
         if x is not None:
             if x.shape != x_shape:
                 raise ValueError(f'Inconsistent detected: {x.shape} != {x_shape}!')
 
+
     def _init_ineq_cons(self, ineqconidx=None, ineqconbd=None):
         """
             Obtain Hankel matrix that used for the inequality constrained variables
                            lbc <= Hc * g <= ubc
             return  Hc, lbc, ubc
         """
         if ineqconidx is None:
@@ -192,33 +200,41 @@
                 ubc_list.append(np.tile(ub, self.Np))
 
             Hc = np.concatenate(Hc_list)
             lbc = np.concatenate(lbc_list).flatten()
             ubc = np.concatenate(ubc_list).flatten()
         return Hc, lbc.tolist(), ubc.tolist()
 
+
     def _init_variables(self):
         """
             Initialize variables of DeePC and RDeePC design
                    parameters: uini, yini   |   updated each iteration
             optimizing_target: g            |   decision variable
         """
         ## define casadi variables
-        self.parameters = ctools.struct_symSX([
-            (
-                ctools.entry('uini', shape=tuple([self.u_dim * self.Tini, 1])),
-                ctools.entry('yini', shape=tuple([self.y_dim * self.Tini, 1]))
-            )
-        ])
-
         self.optimizing_target = ctools.struct_symSX([
             (
                 ctools.entry('g', shape=tuple([self.g_dim, 1]))
             )
         ])
+        
+        parameters = [
+                ctools.entry('uini', shape=tuple([self.u_dim * self.Tini, 1])),
+                ctools.entry('yini', shape=tuple([self.y_dim * self.Tini, 1]))
+        ]
+        
+        if self.sp_change:
+            parameters.extend([
+                ctools.entry('uref', shape=tuple([self.u_dim * self.Np, 1])),
+                ctools.entry('yref', shape=tuple([self.y_dim * self.Np, 1])),
+            ])  
+        
+        self.parameters = ctools.struct_symSX(parameters)
+
 
     @timer
     def init_DeePCsolver(self, uloss='u', opts={}):
         """
                               Formulate NLP solver for: DeePC design
             Initialize CasADi nlp solver, !!! only need to formulate the nlp problem at the first time !!!
             treat the updated variables as parameters of the nlp problem
@@ -253,45 +269,49 @@
         print('>> DeePC design formulating')
         if uloss not in ["u", "uus", "du"]:
             raise ValueError("uloss should be one of: 'u', 'uus', 'du'!")
         if self.g_dim <= (self.u_dim + self.y_dim) * self.Tini:
             raise ValueError(f'NLP do not have enough degrees of freedom | Should: g_dim >= (u_dim + y_dim) * Tini, but got: {self.g_dim} <= {(self.u_dim + self.y_dim) * self.Tini}!')
 
         # define parameters and decision variable
-        uini, yini = self.parameters[...]
+        if self.sp_change:
+            uini, yini, uref, yref = self.parameters[...]
+        else:
+            uini, yini = self.parameters[...]
+            uref, yref = self.uref, self.yref
         g, = self.optimizing_target[...]  # data are stored in list [], notice that ',' cannot be missed
 
         ## J  =  || Uf * g - ys ||_Q^2 + || uloss ||_R^2
         ## s.t.   Up * g = uini
         ##        Yp * g = yini
         ##        ulb <= u <= uub
 
         ## objective function in QP form
         if uloss == 'u':
             ## QP problem
             H = self.Yf.T @ self.Q @ self.Yf + self.Uf.T @ self.R @ self.Uf
-            f = - self.Yf.T @ self.Q @ self.yref  # - self.Uf.T @ self.R @ uref
+            f = - self.Yf.T @ self.Q @ yref  # - self.Uf.T @ self.R @ uref
             obj = 0.5 * cs.mtimes(cs.mtimes(g.T, H), g) + cs.mtimes(f.T, g)
 
         if uloss == 'uus':
-            if self.uref is None:
+            if self.sp_change is False and self.uref is None:
                 raise ValueError("Do not give value of 'us', but required in objective function 'u-us'!")
             ## QP problem
             H = self.Yf.T @ self.Q @ self.Yf + self.Uf.T @ self.R @ self.Uf
-            f = - self.Yf.T @ self.Q @ self.yref - self.Uf.T @ self.R @ self.uref
+            f = - self.Yf.T @ self.Q @ yref - self.Uf.T @ self.R @ uref
             obj = 0.5 * cs.mtimes(cs.mtimes(g.T, H), g) + cs.mtimes(f.T, g)
 
         if uloss == 'du':
             ## Not a QP problem
             u_cur = cs.mtimes(self.Uf, g)
             u_prev = cs.vertcat(uini[-self.u_dim:], cs.mtimes(self.Uf, g)[:-self.u_dim])
             du = u_cur - u_prev
 
             y = cs.mtimes(self.Yf, g)
-            y_loss = y - self.yref
+            y_loss = y - yref
             obj = cs.mtimes(cs.mtimes(y_loss.T, self.Q), y_loss) + cs.mtimes(cs.mtimes(du.T, self.R), du)
 
         #### constrains
         C = []
         lbc, ubc = [], []
         # equal constrains:  Up * g = uini, Yp * g = yini
         C += [cs.mtimes(self.Up, g) - uini]
@@ -356,44 +376,48 @@
             raise ValueError(
                 "Do not give value of 'lambda_g' or 'lambda_y', but required in objective function for Robust DeePC!")
         if self.g_dim <= self.u_dim * self.Tini:
             raise ValueError(f'NLP do not have enough degrees of freedom | Should: g_dim >= u_dim * Tini, but got: {self.g_dim} <= {self.u_dim * self.Tini}!')
 
 
         # define parameters and decision variable
-        uini, yini = self.parameters[...]
+        if self.sp_change:
+            uini, yini, uref, yref = self.parameters[...]
+        else:
+            uini, yini = self.parameters[...]
+            uref, yref = self.uref, self.yref
         g, = self.optimizing_target[...]  # data are stored in list [], notice that ',' cannot be missed
 
         ## J  =  || Uf * g - ys ||_Q^2 + || uloss ||_R^2 + lambda_y || Yp * g - yini||_2^2 + lambda_g || g ||_2^2
         ## s.t.   Up * g = uini
         ##        ulb <= u <= uub
 
         ## objective function
         if uloss == 'u':
             ## QP problem
             H = self.Yf.T @ self.Q @ self.Yf + self.Uf.T @ self.R @ self.Uf + self.Yp.T @ self.lambda_y @ self.Yp + self.lambda_g
-            f = - self.Yp.T @ self.lambda_y @ yini - self.Yf.T @ self.Q @ self.yref  # - self.Uf.T @ self.R @ uref
+            f = - self.Yp.T @ self.lambda_y @ yini - self.Yf.T @ self.Q @ yref  # - self.Uf.T @ self.R @ uref
             obj = 0.5 * cs.mtimes(cs.mtimes(g.T, H), g) + cs.mtimes(f.T, g)
 
         if uloss == 'uus':
-            if self.uref is None:
+            if self.sp_change is False and self.uref is None:
                 raise ValueError("Do not give value of 'us', but required in objective function 'u-us'!")
             ## QP problem
             H = self.Yf.T @ self.Q @ self.Yf + self.Uf.T @ self.R @ self.Uf + self.Yp.T @ self.lambda_y @ self.Yp + self.lambda_g
-            f = - self.Yp.T @ self.lambda_y @ yini - self.Yf.T @ self.Q @ self.yref - self.Uf.T @ self.R @ self.uref
+            f = - self.Yp.T @ self.lambda_y @ yini - self.Yf.T @ self.Q @ yref - self.Uf.T @ self.R @ uref
             obj = 0.5 * cs.mtimes(cs.mtimes(g.T, H), g) + cs.mtimes(f.T, g)
 
         if uloss == 'du':
             ## Not a QP problem
             u_cur = cs.mtimes(self.Uf, g)
             u_prev = cs.vertcat(uini[-self.u_dim:], cs.mtimes(self.Uf, g)[:-self.u_dim])
             du = u_cur - u_prev
 
             y = cs.mtimes(self.Yf, g)
-            y_loss = y - self.yref
+            y_loss = y - yref
 
             sigma_y = cs.mtimes(self.Yp, g) - yini
             obj = cs.mtimes(cs.mtimes(y_loss.T, self.Q), y_loss) + cs.mtimes(cs.mtimes(du.T, self.R), du) + cs.mtimes(
                 cs.mtimes(g.T, self.lambda_g), g) + cs.mtimes(cs.mtimes(sigma_y.T, self.lambda_y), sigma_y)
 
         #### constrains
         C = []
@@ -411,27 +435,34 @@
 
         # formulate the nlp prolbem
         nlp_prob = {'f': obj, 'x': self.optimizing_target, 'p': self.parameters, 'g': cs.vertcat(*C)}
 
         self.solver = cs.nlpsol('solver', 'ipopt', nlp_prob, opts)
         self.lbc = lbc
         self.ubc = ubc
+        
 
-    def solver_step(self, uini, yini):
+    def solver_step(self, uini, yini, uref=None, yref=None):
         """
             solver solve the nlp for one time
             uini, yini:  [array]   | (dim*Tini, 1)
+            uref, yref:  [array]   | (dim*Np, 1) if sp_change=True
               g0_guess:  [array]   | (T-L+1, 1)
             return:
                 u_opt:  the optimized control input for the next Np steps
                  g_op:  the optimized operator g
                   t_s:  solving time
         """
-        parameters = np.concatenate((uini, yini))
-        g0_guess = np.linalg.pinv(np.concatenate((self.Up, self.Yp), axis=0)) @ parameters
+        if self.sp_change:
+            if uref is None or yref is None:
+                raise ValueError("Do not give value of 'uref' or 'yref', but required in objective function!")
+            parameters = np.concatenate((uini, yini, uref, yref))
+        else:
+            parameters = np.concatenate((uini, yini))
+        g0_guess = np.linalg.pinv(np.concatenate((self.Up, self.Yp), axis=0)) @ np.concatenate((uini, yini))
 
         t_ = time.time()
         sol = self.solver(x0=g0_guess, p=parameters, lbg=self.lbc, ubg=self.ubc)
         t_s = time.time() - t_
 
         g_opt = sol['x'].full().ravel()
         u_opt = np.matmul(self.Uf, g_opt)
```

### Comparing `deepctools-1.0.4/src/deepctools/Modeltools.py` & `deepctools-1.0.5/src/deepctools/Modeltools.py`

 * *Files identical despite different names*

### Comparing `deepctools-1.0.4/src/deepctools/__init__.py` & `deepctools-1.0.5/src/deepctools/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,12 +32,12 @@
         % (casadi.__version__, _MIN_CASADI_VERSION))
 elif _getVersion(casadi.__version__) > _getVersion(_MAX_CASADI_VERSION):
     raise ImportError("casadi version %s is too new (must be <=%s)"
         % (casadi.__version__, _MAX_CASADI_VERSION))
 
 # Add modules and some specific functions.
 # from . import DeePCtools
-from .util import hankel
+from .util import hankel, data_to_step
 from .DeePCtools import deepctools
 from .Modeltools import getCasadiFunc, DiscreteSimulator
```

### Comparing `deepctools-1.0.4/src/deepctools/util.py` & `deepctools-1.0.5/src/deepctools/util.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Name: setup.py
+Name: util.py
 Author: Xuewen Zhang
 Date:at 13/04/2024
 version: 1.0.0
 Description: utils of deepctools
 """
 import casadi as cs
 import numpy as np
@@ -74,8 +74,36 @@
     while j < M:  # For some reason, a for loop creates problems here.
         k1 = f(x, *par)
         k2 = f(x + k1 * h / 2, *par)
         k3 = f(x + k2 * h / 2, *par)
         k4 = f(x + k3 * h, *par)
         x = x + (k1 + 2 * k2 + 2 * k3 + k4) * h / 6
         j += 1
-    return x
+    return x
+
+
+def data_to_step(x, t=None):
+        """
+            Transform the sequential data to step data
+            data: (data_size, x_dim)
+            t: (data_size)
+        """
+
+        x = x.T
+        dim, n = x.shape
+        x_step = np.zeros((dim, 2*n))
+
+        for i in range(n):
+            x_step[:, 2 * i] = x[:, i]
+            x_step[:, 2 * i + 1] = x[:, i]
+
+        if t is not None:
+            t_step = np.zeros(2*len(t))
+            for i in range(len(t)):
+                t_step[2 * i] = t[i]
+                t_step[2 * i + 1] = t[i]
+            ts = t[1]-t[0]
+            t_step = t_step[1:]
+            t_step = np.concatenate((t_step, np.array([t_step[-1] + ts])))
+            return x_step.T, t_step
+        else:
+            return x_step.T
```

### Comparing `deepctools-1.0.4/LICENSE` & `deepctools-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `deepctools-1.0.4/README.md` & `deepctools-1.0.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
 Formulate and solve the DeePC problem, including **DeePC** and **Robust DeePC** design.
 
 Construct the nlp solver for DeePC using CasADi IPOPT sovler, only formulate the solver once at the first beginning. 
 
 In the online loop, no need to reformulate the NLP problem which saves lots of computational time.
 
-Each iteration, only need provide updated parameters: $u_{ini}$, $y_{ini}$.
+Each iteration, only need provide updated parameters: $u_{ini}$, $y_{ini}$ (, $u_{ref}$, $y_{ref}$ if set-point changes during control).
 
 > Objective function: $J = \Vert y - y^r \Vert_Q^2 + \Vert u_{loss} \Vert_R^2 + \mathcal{o}(\sigma_y, g)$
 
 > $u_{loss}$ can be:
 
 ```       
         'u': u
```

### Comparing `deepctools-1.0.4/pyproject.toml` & `deepctools-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "deepctools"
-version = "1.0.4"
+version = "1.0.5"
 authors = [
   { name="Xuewen Zhang", email="xuewen.zhang741@outlook.com"}
 ]
 maintainers = [
   { name="Xuewen Zhang", email="xuewen.zhang741@outlook.com"}
 ]
 dependencies = [
```

### Comparing `deepctools-1.0.4/PKG-INFO` & `deepctools-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: deepctools
-Version: 1.0.4
+Version: 1.0.5
 Summary: A wrapped package for Data-enabled predictive control (DeePC) implementation. Including DeePC and Robust DeePC design with multiple objective functions.
 Project-URL: Homepage, https://github.com/QiYuan-Zhang/DeePCtools
 Project-URL: Issues, https://github.com/QiYuan-Zhang/DeePCtools/issues
 Project-URL: Introduction, https://qiyuan-zhang.github.io/my-toolbox/2024/04/15/Developed-deepctools.html
 Author-email: Xuewen Zhang <xuewen.zhang741@outlook.com>
 Maintainer-email: Xuewen Zhang <xuewen.zhang741@outlook.com>
 License:                                 Apache License
@@ -274,15 +274,15 @@
 
 Formulate and solve the DeePC problem, including **DeePC** and **Robust DeePC** design.
 
 Construct the nlp solver for DeePC using CasADi IPOPT sovler, only formulate the solver once at the first beginning. 
 
 In the online loop, no need to reformulate the NLP problem which saves lots of computational time.
 
-Each iteration, only need provide updated parameters: $u_{ini}$, $y_{ini}$.
+Each iteration, only need provide updated parameters: $u_{ini}$, $y_{ini}$ (, $u_{ref}$, $y_{ref}$ if set-point changes during control).
 
 > Objective function: $J = \Vert y - y^r \Vert_Q^2 + \Vert u_{loss} \Vert_R^2 + \mathcal{o}(\sigma_y, g)$
 
 > $u_{loss}$ can be:
 
 ```       
         'u': u
```

