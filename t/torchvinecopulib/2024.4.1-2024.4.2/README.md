# Comparing `tmp/torchvinecopulib-2024.4.1.tar.gz` & `tmp/torchvinecopulib-2024.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchvinecopulib-2024.4.1.tar", max compression
+gzip compressed data, was "torchvinecopulib-2024.4.2.tar", max compression
```

## Comparing `torchvinecopulib-2024.4.1.tar` & `torchvinecopulib-2024.4.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    35593 2024-03-24 13:40:35.000000 torchvinecopulib-2024.4.1/LICENSE
--rw-r--r--   0        0        0     1481 2024-04-24 08:54:49.541792 torchvinecopulib-2024.4.1/pyproject.toml
--rw-r--r--   0        0        0     5690 2024-04-24 08:54:49.541792 torchvinecopulib-2024.4.1/README.md
--rw-r--r--   0        0        0       97 2024-03-24 13:54:38.000000 torchvinecopulib-2024.4.1/torchvinecopulib/__init__.py
--rw-r--r--   0        0        0      379 2024-03-24 13:54:38.000000 torchvinecopulib-2024.4.1/torchvinecopulib/bicop/__init__.py
--rw-r--r--   0        0        0     9267 2024-03-24 13:54:38.000000 torchvinecopulib-2024.4.1/torchvinecopulib/bicop/_abc.py
--rw-r--r--   0        0        0     1357 2024-03-24 13:54:38.000000 torchvinecopulib-2024.4.1/torchvinecopulib/bicop/_archimedean.py
--rw-r--r--   0        0        0     1949 2024-03-24 13:54:38.000000 torchvinecopulib-2024.4.1/torchvinecopulib/bicop/_clayton.py
--rw-r--r--   0        0        0     8300 2024-03-24 13:54:38.000000 torchvinecopulib-2024.4.1/torchvinecopulib/bicop/_data_bcp.py
--rw-r--r--   0        0        0      414 2024-03-24 13:54:38.000000 torchvinecopulib-2024.4.1/torchvinecopulib/bicop/_elliptical.py
--rw-r--r--   0        0        0     4958 2024-04-24 08:15:26.464746 torchvinecopulib-2024.4.1/torchvinecopulib/bicop/_factory_bcp.py
--rw-r--r--   0        0        0     2837 2024-03-24 13:54:38.000000 torchvinecopulib-2024.4.1/torchvinecopulib/bicop/_frank.py
--rw-r--r--   0        0        0     1676 2024-03-24 13:54:38.000000 torchvinecopulib-2024.4.1/torchvinecopulib/bicop/_gaussian.py
--rw-r--r--   0        0        0     2438 2024-03-24 13:54:38.000000 torchvinecopulib-2024.4.1/torchvinecopulib/bicop/_gumbel.py
--rw-r--r--   0        0        0     1353 2024-03-24 13:54:38.000000 torchvinecopulib-2024.4.1/torchvinecopulib/bicop/_independent.py
--rw-r--r--   0        0        0     3133 2024-04-02 13:53:35.188111 torchvinecopulib-2024.4.1/torchvinecopulib/bicop/_joe.py
--rw-r--r--   0        0        0     3170 2024-04-24 08:21:30.539930 torchvinecopulib-2024.4.1/torchvinecopulib/bicop/_studentt.py
--rw-r--r--   0        0        0    29166 2024-04-24 07:54:05.180351 torchvinecopulib-2024.4.1/torchvinecopulib/util/__init__.py
--rw-r--r--   0        0        0      207 2024-03-24 13:54:42.000000 torchvinecopulib-2024.4.1/torchvinecopulib/vinecop/__init__.py
--rw-r--r--   0        0        0    33223 2024-04-23 08:23:14.413176 torchvinecopulib-2024.4.1/torchvinecopulib/vinecop/_data_vcp.py
--rw-r--r--   0        0        0    25355 2024-04-24 07:53:16.580676 torchvinecopulib-2024.4.1/torchvinecopulib/vinecop/_factory_vcp.py
--rw-r--r--   0        0        0     6831 1970-01-01 00:00:00.000000 torchvinecopulib-2024.4.1/PKG-INFO
+-rw-r--r--   0        0        0    35593 2024-04-27 07:17:40.868884 torchvinecopulib-2024.4.2/LICENSE
+-rw-r--r--   0        0        0     1670 2024-04-30 03:11:55.068293 torchvinecopulib-2024.4.2/pyproject.toml
+-rw-r--r--   0        0        0     5672 2024-04-30 07:21:24.864497 torchvinecopulib-2024.4.2/README.md
+-rw-r--r--   0        0        0       97 2024-04-30 03:35:06.539336 torchvinecopulib-2024.4.2/torchvinecopulib/__init__.py
+-rw-r--r--   0        0        0      529 2024-04-30 03:28:39.037386 torchvinecopulib-2024.4.2/torchvinecopulib/bicop/__init__.py
+-rw-r--r--   0        0        0     9267 2024-04-27 07:17:41.246247 torchvinecopulib-2024.4.2/torchvinecopulib/bicop/_abc.py
+-rw-r--r--   0        0        0     1357 2024-04-27 07:17:41.252249 torchvinecopulib-2024.4.2/torchvinecopulib/bicop/_archimedean.py
+-rw-r--r--   0        0        0     1949 2024-04-27 07:17:41.256246 torchvinecopulib-2024.4.2/torchvinecopulib/bicop/_clayton.py
+-rw-r--r--   0        0        0     8300 2024-04-27 07:17:41.260276 torchvinecopulib-2024.4.2/torchvinecopulib/bicop/_data_bcp.py
+-rw-r--r--   0        0        0      414 2024-03-24 13:54:38.000000 torchvinecopulib-2024.4.2/torchvinecopulib/bicop/_elliptical.py
+-rw-r--r--   0        0        0     4869 2024-04-30 03:54:31.509330 torchvinecopulib-2024.4.2/torchvinecopulib/bicop/_factory_bcp.py
+-rw-r--r--   0        0        0     2881 2024-04-30 02:54:11.474705 torchvinecopulib-2024.4.2/torchvinecopulib/bicop/_frank.py
+-rw-r--r--   0        0        0     1676 2024-04-27 07:17:41.276252 torchvinecopulib-2024.4.2/torchvinecopulib/bicop/_gaussian.py
+-rw-r--r--   0        0        0     2438 2024-04-30 02:54:59.026533 torchvinecopulib-2024.4.2/torchvinecopulib/bicop/_gumbel.py
+-rw-r--r--   0        0        0     1353 2024-03-24 13:54:38.000000 torchvinecopulib-2024.4.2/torchvinecopulib/bicop/_independent.py
+-rw-r--r--   0        0        0     3133 2024-04-30 02:55:12.338411 torchvinecopulib-2024.4.2/torchvinecopulib/bicop/_joe.py
+-rw-r--r--   0        0        0     3170 2024-04-27 07:17:41.289787 torchvinecopulib-2024.4.2/torchvinecopulib/bicop/_studentt.py
+-rw-r--r--   0        0        0    28939 2024-04-30 04:02:06.809730 torchvinecopulib-2024.4.2/torchvinecopulib/util/__init__.py
+-rw-r--r--   0        0        0      207 2024-04-30 07:05:31.177262 torchvinecopulib-2024.4.2/torchvinecopulib/vinecop/__init__.py
+-rw-r--r--   0        0        0    33968 2024-04-30 07:38:57.742190 torchvinecopulib-2024.4.2/torchvinecopulib/vinecop/_data_vcp.py
+-rw-r--r--   0        0        0    26154 2024-04-30 07:39:09.083590 torchvinecopulib-2024.4.2/torchvinecopulib/vinecop/_factory_vcp.py
+-rw-r--r--   0        0        0     6814 1970-01-01 00:00:00.000000 torchvinecopulib-2024.4.2/PKG-INFO
```

### Comparing `torchvinecopulib-2024.4.1/LICENSE` & `torchvinecopulib-2024.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `torchvinecopulib-2024.4.1/pyproject.toml` & `torchvinecopulib-2024.4.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 package-mode = true
 license = "GNU GPLv3"
 name = "torchvinecopulib"
-version = "2024.4.1"
+version = "2024.4.2"
 description = "yet another vine copula library for PyTorch."
 authors = ["Tuoyuan Cheng <cty120120@gmail.com>"]
 maintainers = ["Xiaosheng You <e1204754@u.nus.edu>"]
 readme = "README.md"
 # homepage = ""
 repository = "https://github.com/TY-Cheng/torchvinecopulib"
 documentation = "https://ty-cheng.github.io/torchvinecopulib/"
@@ -17,30 +17,34 @@
     "Operating System :: Microsoft :: Windows :: Windows 10",
     "Operating System :: POSIX :: Linux",
     "Operating System :: MacOS",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering",
 ]
 
+[[tool.poetry.source]]
+name = "pytorch_cu"
+url = "https://download.pytorch.org/whl/cu121"
+priority = "explicit"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 scipy = "*"
-torch = "^2"
+torch = { version = "^2", source = "pytorch_cu" }
 
 
 [tool.poetry.group.all.dependencies]
 matplotlib = "*"
 pot = "*"
 scikit-learn = "*"
 fastkde = "*"
 
 
 [tool.poetry.group.dev.dependencies]
-black = "*"
+black = { version = "*", extras = ["jupyter"] }
 coverage = "*"
 flake8 = "*"
 furo = "*"
 ipykernel = "*"
 matplotlib = "*"
 pandas = "*"
 pot = "*"
```

### Comparing `torchvinecopulib-2024.4.1/README.md` & `torchvinecopulib-2024.4.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -52,17 +52,17 @@
 ```
 
 By `pip` from `./dist/*.whl` or `./dist/*.tar.gz` in this repo.
 Need to use proper file name.
 
 ```bash
 # inside project root folder
-pip install ./dist/torchvinecopulib-2024.4.1-py3-none-any.whl
+pip install ./dist/torchvinecopulib-2024.4.2-py3-none-any.whl
 # or
-pip install ./dist/torchvinecopulib-2024.4.1.tar.gz
+pip install ./dist/torchvinecopulib-2024.4.2.tar.gz
 ```
 
 ## Examples
 
 Visit the `./examples/` folder for `.ipynb` Jupyter notebooks.
 
 ## Documentation
@@ -108,17 +108,16 @@
 - Include a clear and descriptive title and description for your pull request.
 - Make sure all tests pass before submitting the pull request.
 - If your pull request addresses an open issue, reference the issue number in the description using the syntax `#issue_number`.
 - [in-place ops can be slower](https://discuss.pytorch.org/t/are-inplace-operations-faster/61209/4)
 - [torch.jit.script can be slower](https://discuss.pytorch.org/t/why-is-torch-jit-script-slower/120131/6)
 
 ### TODO
-1. non-par bicop
-2. more (non-parametric) `bicop` class in `torch`
-3. potentially deprecating `'mle'` from `mtd_fit`
+1. more (non-parametric) `bicop` class in `torch`
+2. potentially deprecating `'mle'` from `mtd_fit`
 
 ## License
 
 > Copyright (C) 2024 Tuoyuan Cheng, Xiaosheng You, Kan Chen
 >
 > This file is part of torchvinecopulib.
 > torchvinecopulib is free software: you can redistribute it and/or modify
```

### Comparing `torchvinecopulib-2024.4.1/torchvinecopulib/bicop/_abc.py` & `torchvinecopulib-2024.4.2/torchvinecopulib/bicop/_abc.py`

 * *Files identical despite different names*

### Comparing `torchvinecopulib-2024.4.1/torchvinecopulib/bicop/_archimedean.py` & `torchvinecopulib-2024.4.2/torchvinecopulib/bicop/_archimedean.py`

 * *Files identical despite different names*

### Comparing `torchvinecopulib-2024.4.1/torchvinecopulib/bicop/_clayton.py` & `torchvinecopulib-2024.4.2/torchvinecopulib/bicop/_clayton.py`

 * *Files identical despite different names*

### Comparing `torchvinecopulib-2024.4.1/torchvinecopulib/bicop/_data_bcp.py` & `torchvinecopulib-2024.4.2/torchvinecopulib/bicop/_data_bcp.py`

 * *Files identical despite different names*

### Comparing `torchvinecopulib-2024.4.1/torchvinecopulib/bicop/_factory_bcp.py` & `torchvinecopulib-2024.4.2/torchvinecopulib/bicop/_factory_bcp.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,21 +27,23 @@
 
     :param obs_bcp: bivariate copula obs, of shape (num_obs, 2) with values in [0, 1]
     :type obs_bcp: torch.Tensor
     :param tau: Kendall's tau of the observations, defaults to None for the function to estimate
     :type tau: float, optional
     :param thresh_trunc: threshold of Kendall's tau independence test, below which we reject independent bicop, defaults to 0.1
     :type thresh_trunc: float, optional
-    :param mtd_fit: parameter estimation method, either 'itau' (inverse of tau) or 'mle' (maximum likelihood estimation); defaults to "itau"
+    :param mtd_fit: parameter estimation method, either 'itau' (inverse of tau) or
+        'mle' (maximum likelihood estimation); defaults to "itau"
     :type mtd_fit: str, optional
     :param mtd_mle: optimization method for mle as used by scipy.optimize.minimize, defaults to "COBYLA"
     :type mtd_mle: str, optional
     :param mtd_sel: model selection criterion, either 'aic' or 'bic'; defaults to "aic"
     :type mtd_sel: str, optional
-    :param tpl_fam: tuple of str as candidate family names to fit, could be a subset of ('Clayton', 'Frank', 'Gaussian', 'Gumbel', 'Independent', 'Joe', 'StudentT')
+    :param tpl_fam: tuple of str as candidate family names to fit,
+        could be a subset of ('Clayton', 'Frank', 'Gaussian', 'Gumbel', 'Independent', 'Joe', 'StudentT')
     :type tpl_fam: tuple, optional
     :param topk: number of best itau fit taken into further mle, used when mtd_fit is 'mle'; defaults to 2
     :type topk: int, optional
     :raises NotImplementedError: when mtd_fit is neither 'itau' nor 'mle'
     :return: fitted bivariate copula dataclass object
     :rtype: DataBiCop
     """
@@ -89,19 +91,15 @@
             # quit early if 'Independent'
             if i_fam == "Independent":
                 return vec_bcp_data[i_idx]
             # fetch the class
             i_cls = ENUM_FAM_BICOP[i_fam].value
 
             res = minimize(
-                fun=lambda par: i_cls.l_pdf(par=par, obs=obs_bcp, rot=i_rot)
-                .nan_to_num(posinf=0.0, neginf=0.0)
-                .sum()
-                .neg()
-                .item(),
+                fun=lambda par: i_cls.l_pdf(par=par, obs=obs_bcp, rot=i_rot).sum().neg().item(),
                 x0=vec_bcp_data[i_idx].par,
                 bounds=tuple(zip(i_cls._PAR_MIN, i_cls._PAR_MAX)),
                 method=mtd_mle,
             )
             return DataBiCop(
                 fam=i_fam,
                 negloglik=float(res.fun),
```

### Comparing `torchvinecopulib-2024.4.1/torchvinecopulib/bicop/_frank.py` & `torchvinecopulib-2024.4.2/torchvinecopulib/bicop/_frank.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
     @staticmethod
     def hinv1_0(obs: torch.Tensor, par: tuple[float]) -> torch.Tensor:
         """inverse of the first h function, Q(p=v1 | V0=v0)"""
         delta = par[0]
         x = obs[:, [0]]
         return (
-            _g(vec=torch.tensor(1.0), delta=delta)
+            _g(vec=torch.as_tensor(data=1.0, dtype=obs.dtype, device=obs.device), delta=delta)
             / ((-delta * x).exp() / obs[:, [1]] - _g(vec=x, delta=delta))
         ).log1p() / (-delta)
 
     @classmethod
     def l_pdf_0(cls, obs: torch.Tensor, par: tuple[float]) -> torch.Tensor:
         return cls.pdf_0(obs=obs, par=par).log()
```

### Comparing `torchvinecopulib-2024.4.1/torchvinecopulib/bicop/_gaussian.py` & `torchvinecopulib-2024.4.2/torchvinecopulib/bicop/_gaussian.py`

 * *Files identical despite different names*

### Comparing `torchvinecopulib-2024.4.1/torchvinecopulib/bicop/_gumbel.py` & `torchvinecopulib-2024.4.2/torchvinecopulib/bicop/_gumbel.py`

 * *Files identical despite different names*

### Comparing `torchvinecopulib-2024.4.1/torchvinecopulib/bicop/_independent.py` & `torchvinecopulib-2024.4.2/torchvinecopulib/bicop/_independent.py`

 * *Files identical despite different names*

### Comparing `torchvinecopulib-2024.4.1/torchvinecopulib/bicop/_joe.py` & `torchvinecopulib-2024.4.2/torchvinecopulib/bicop/_joe.py`

 * *Files identical despite different names*

### Comparing `torchvinecopulib-2024.4.1/torchvinecopulib/bicop/_studentt.py` & `torchvinecopulib-2024.4.2/torchvinecopulib/bicop/_studentt.py`

 * *Files identical despite different names*

### Comparing `torchvinecopulib-2024.4.1/torchvinecopulib/util/__init__.py` & `torchvinecopulib-2024.4.2/torchvinecopulib/util/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,23 +41,22 @@
 
 def kendall_tau(
     x: torch.Tensor,
     y: torch.Tensor,
     tau_min: float = _TAU_MIN,
     tau_max: float = _TAU_MAX,
 ) -> float:
-    """https://gist.github.com/ili3p/f2b38b898f6eab0d87ec248ea39fde94
-    x,y are both of shape (n, 1)
-    """
+    """x,y are both of shape (n, 1)"""
     res = kendalltau(x.cpu().ravel(), y.cpu().ravel())
     return (max(min(res[0], tau_max), tau_min), res[1])
 
 
 def mutual_info(x: torch.Tensor, y: torch.Tensor, is_sklearn: bool = True) -> float:
     """https://scikit-learn.org/stable/modules/generated/sklearn.feature_selection.mutual_info_regression.html
+
     x,y are both of shape (n, 1)
 
     Purkayastha, S., & Song, P. X. K. (2024).
     fastMI: A fast and consistent copula-based nonparametric estimator of mutual information.
     Journal of Multivariate Analysis, 201, 105270.
     """
     if is_sklearn:
@@ -112,15 +111,16 @@
         ).reciprocal()
     ).item()
 
 
 def chatterjee_xi(x: torch.Tensor, y: torch.Tensor, M: int = 1) -> float:
     """revised Chatterjee's rank correlation coefficient (ξ), taken max to be symmetric
 
-    Chatterjee, S., 2021. A new coefficient of correlation. Journal of the American Statistical Association, 116(536), pp.2009-2022.
+    Chatterjee, S., 2021. A new coefficient of correlation.
+    Journal of the American Statistical Association, 116(536), pp.2009-2022.
 
     Lin, Z. and Han, F., 2023. On boosting the power of Chatterjee’s rank correlation. Biometrika, 110(2), pp.283-299.
     "a large negative value of ξ has only one possible interpretation: the data does not resemble an iid sample."
 
     :param x: obs of shape (n,1)
     :type x: torch.Tensor
     :param y: obs of shape (n,1)
@@ -349,16 +349,14 @@
         .clamp(min=_CDF_MIN, max=_CDF_MAX)
     )
 
 
 # # * Student's t distribution CDF (p), PPF (q), density (d)
 # def inc_beta_reg(vec: torch.Tensor, a: float, b: float) -> torch.Tensor:
 #     # * regularized incomplete beta integral, with a = 0.5, b = nu / 2, vec in [0,1]
-#     # https://stats.stackexchange.com/questions/615961/students-t-cdf-ppf-or-hypergeometric-2f1-or-betainc-using-pytorch
-#     # https://stats.stackexchange.com/questions/52341/formula-to-generate-critical-t-values-for-t-test-instead-of-using-a-look-up-arr
 #     res = torch.empty_like(vec)
 #     if (idx := vec > ((a + 1.0) / (2.0 + a + b))).any():
 #         res[idx] = 1.0 - inc_beta_reg(vec=1.0 - vec[idx], a=b, b=a)
 #     idx = ~idx
 #     x = vec[idx]
 #     qab = a + b
 #     qap = a + 1.0
@@ -532,19 +530,27 @@
     :param nu: the nu parameter, degrees of freedom
     :type nu: float
     :return: cumulative distribution function (CDF) of shape (num_obs, 1), given the observations
     :rtype: torch.Tensor
     """
     h = obs[:, [0]]
     k = obs[:, [1]]
-    rho: torch.Tensor = torch.tensor(rho, dtype=obs.dtype, device=obs.device).clamp(
+    rho: torch.Tensor = torch.as_tensor(
+        data=rho,
+        dtype=obs.dtype,
+        device=obs.device,
+    ).clamp(
         min=_RHO_MIN,
         max=_RHO_MAX,
     )
-    nu: torch.Tensor = torch.tensor(nu, dtype=obs.dtype, device=obs.device).clamp(
+    nu: torch.Tensor = torch.as_tensor(
+        data=nu,
+        dtype=obs.dtype,
+        device=obs.device,
+    ).clamp(
         min=_NU_MIN,
         max=_NU_MAX,
     )
     #
     if nu < 1:
         bvt = pbvnorm(obs=obs, rho=rho)
     else:
@@ -722,23 +728,26 @@
     n_0: int = 1,
     k_1: float = 0.2,
     k_2: float = 2.0,
     j_max: int = 31,
 ) -> float:
     """Solve an arbitrary function for a zero-crossing.
 
-    Oliveira, I.F. and Takahashi, R.H., 2020. An enhancement of the bisection method average performance preserving minmax optimality. ACM Transactions on Mathematical Software (TOMS), 47(1), pp.1-24.
+    Oliveira, I.F. and Takahashi, R.H., 2020.
+    An enhancement of the bisection method average performance preserving minmax optimality.
+    ACM Transactions on Mathematical Software (TOMS), 47(1), pp.1-24.
 
     https://docs.rs/kurbo/0.8.1/kurbo/common/fn.solve_itp.html
 
     https://en.wikipedia.org/wiki/ITP_method
 
     ! It is assumed that f(a) < 0 and f(b) > 0, otherwise unexpected results may occur.
 
-    The ITP method has tuning parameters. This implementation hardwires k2 to 2.0, both because it avoids an expensive floating point exponentiation,
+    The ITP method has tuning parameters. This implementation hardwires k2 to 2.0,
+    both because it avoids an expensive floating point exponentiation,
     and because this value has been tested to work well with curve fitting problems.
 
     The n0 parameter controls the relative impact of the bisection and secant components.
     When it is 0, the number of iterations is guaranteed to be no more than the number required by bisection
     (thus, this method is strictly superior to bisection). However, when the function is smooth,
     a value of 1 gives the secant method more of a chance to engage, so the average number of iterations is likely lower,
     though there can be one more iteration than bisection in the worst case.
```

### Comparing `torchvinecopulib-2024.4.1/torchvinecopulib/vinecop/_data_vcp.py` & `torchvinecopulib-2024.4.2/torchvinecopulib/vinecop/_data_vcp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+import json
 import math
-import pickle
 from abc import ABC
-from dataclasses import dataclass
+from dataclasses import asdict, dataclass
 from operator import itemgetter
 from pathlib import Path
 from pprint import pformat
 
 import numpy as np
 import torch
 
@@ -13,17 +13,23 @@
 @dataclass(slots=True, frozen=True, kw_only=True)
 class DataVineCop(ABC):
     """Dataclass for a vine copula model"""
 
     dct_bcp: dict
     """bivariate copulas, stored as {level: {(vertex_left, vertex_right, frozenset_cond): DataBiCop}}"""
     dct_tree: dict
-    """bivariate dependency measures of edges in trees, stored as {level: {(vertex_left, vertex_right, frozenset_cond): bidep}}"""
+    """
+    bivariate dependency measures of edges in trees,
+    stored as {level: {(vertex_left, vertex_right, frozenset_cond): bidep}}
+    """
     tpl_sim: tuple
-    """the source vertices (pseudo-obs) of simulation paths, read from right to left; some vertices can be given as simulated at the beginning of each simulation workflow"""
+    """
+    the source vertices (pseudo-obs) of simulation paths, read from right to left;
+    some vertices can be given as simulated at the beginning of each simulation workflow
+    """
     mtd_bidep: str
     """method to calculate bivariate dependence"""
 
     @property
     def aic(self) -> float:
         """
 
@@ -41,15 +47,16 @@
         :return: Bayesian information criterion (BIC)
         :rtype: float
         """
         return 2.0 * self.negloglik + self.num_par * math.log(self.num_obs)
 
     @property
     def matrix(self) -> np.array:
-        """structure matrix: upper triangular, in row-major order (each row has a bicop as: vertex_left,...,vertex_right;set_cond)
+        """structure matrix: upper triangular, in row-major order
+        (each row has a bicop as: vertex_left,...,vertex_right;set_cond)
 
         :return: structure matrix
         :rtype: np.array
         """
         # NumPy arrays, like arrays in C, are stored in row-major order by default.
         # In a 2D array, the data is stored row by row: elements in the same row are stored in adjacent memory locations.
         mat = []
@@ -113,19 +120,22 @@
                 return v_l, v_r, s_up, bcp
 
     def _ref_count(
         self,
         tpl_first_vs: tuple[tuple[int, frozenset]] = tuple(),
         tpl_sim: tuple[int] = tuple(),
     ) -> tuple[dict, list[int]]:
-        """reference counting for each vertex during simulation (quant-reg/cond-sim) workflow, for garbage collection (memory release)
+        """reference counting for each vertex during simulation (quant-reg/cond-sim) workflow,
+        for garbage collection (memory release)
 
-        :param tpl_first_vs: tuple of vertices (explicitly arranged in conditioned - conditioning set) that are taken as known at the beginning of a simulation workflow, defaults to tuple()
+        :param tpl_first_vs: tuple of vertices (explicitly arranged in conditioned - conditioning set)
+            that are taken as known at the beginning of a simulation workflow, defaults to tuple()
         :type tpl_first_vs: tuple[tuple[int, frozenset]], optional
-        :param tpl_sim: tuple of vertices in a full simulation workflow, gives flexibility to experienced users, defaults to tuple()
+        :param tpl_sim: tuple of vertices in a full simulation workflow,
+            gives flexibility to experienced users, defaults to tuple()
         :type tpl_sim: tuple[int], optional
         :return: reference counting for each vertex; list of source vertices in this simulation workflow from shallow to deep
         :rtype: tuple[dict, list[int]]
         """
         # * v for vertex, s for condition (frozen)set, read from right to left
         dct_first_vs = {v[0]: v for v in tpl_first_vs}
         lst_source = tpl_sim if tpl_sim else self.tpl_sim
@@ -217,15 +227,16 @@
         is_bcp: bool = True,
         num_digit: int = 2,
         font_size_vertex: int = 8,
         font_size_edge: int = 7,
         f_path: Path = None,
         fig_size: tuple = None,
     ) -> tuple:
-        """draw the vine structure at a given level. Each edge corresponds to a fitted bicop. Each node is a bicop of prev lv (is_bcp=True) or pseudo-obs of the given lv (is_bcp=False).
+        """draw the vine structure at a given level. Each edge corresponds to a fitted bicop.
+        Each node is a bicop of prev lv (is_bcp=True) or pseudo-obs of the given lv (is_bcp=False).
 
         :param lv: level, defaults to 0
         :type lv: int, optional
         :param is_bcp: draw the minimum spanning tree (of prev lv bicops) or pseudo observations, defaults to True
         :type is_bcp: bool, optional
         :param num_digit: number of digits to round for the weights on edges, defaults to 2
         :type num_digit: int, optional
@@ -324,19 +335,23 @@
         self,
         tpl_first_vs: tuple = tuple(),
         tpl_sim: tuple = tuple(),
         font_size_vertex: int = 8,
         f_path: Path = None,
         fig_size: tuple = None,
     ) -> tuple:
-        """draw the directed acyclic graph (DAG) of the vine copula, with pseudo observations and bicops as nodes. The source nodes in simulation workflow are highlighted in yellow.
+        """draw the directed acyclic graph (DAG) of the vine copula, with pseudo observations and bicops as nodes.
+        The source nodes in simulation workflow are highlighted in yellow.
 
-        :param tpl_first_vs: tuple of vertices (explicitly arranged in conditioned - conditioning set) that are taken as already simulated at the beginning of a simulation workflow, affecting the color of nodes, defaults to tuple()
+        :param tpl_first_vs: tuple of vertices (explicitly arranged in conditioned - conditioning set)
+            that are taken as already simulated at the beginning of a simulation workflow,
+            affecting the color of nodes, defaults to tuple()
         :type tpl_first_vs: tuple, optional
-        :param tpl_sim: tuple of vertices in a full simulation workflow, gives flexibility to experienced users, defaults to tuple()
+        :param tpl_sim: tuple of vertices in a full simulation workflow,
+            gives flexibility to experienced users, defaults to tuple()
         :type tpl_sim: tuple, optional
         :param font_size_vertex: font size for vertex labels, defaults to 8
         :type font_size_vertex: int, optional
         :param f_path: file path to save the figure, defaults to None for no saving
         :type f_path: Path, optional
         :param fig_size: figure size, defaults to None
         :type fig_size: tuple, optional
@@ -469,31 +484,45 @@
         :param f_path: file path to save the json file, defaults to './vcp.json'
         :type f_path: Path, optional
         :return: file path where the json file is saved
         :rtype: Path
         """
         f_path = Path(f_path)
         f_path.parent.mkdir(parents=True, exist_ok=True)
+        tmp_json = asdict(self)
+        for lv in tmp_json["dct_bcp"]:
+            tmp_json["dct_bcp"][lv] = {
+                str((key[0], key[1], tuple(key[2]))): val
+                for key, val in tmp_json["dct_bcp"][lv].items()
+            }
+            tmp_json["dct_tree"][lv] = {
+                str((key[0], key[1], tuple(key[2]))): val
+                for key, val in tmp_json["dct_tree"][lv].items()
+            }
         with open(f_path, "w") as file:
-            file.write(self.__repr__())
+            json.dump(
+                obj=tmp_json,
+                fp=file,
+                indent=4,
+            )
         return f_path
 
-    def vcp_to_pkl(self, f_path: Path = Path("./vcp.pkl")) -> Path:
-        """save to a pickle file
+    def vcp_to_pth(self, f_path: Path = Path("./vcp.pth")) -> Path:
+        """save to a pth file
 
         :param self: an instance of the DataVineCop dataclass
-        :param f_path: file path to save the pickle file, defaults to Path('./vcp.pkl')
+        :param f_path: file path to save the pth file, defaults to Path('./vcp.pth')
         :type f_path: Path, optional
-        :return: file path where the pickle file is saved
+        :return: file path where the pth file is saved
         :rtype: Path
         """
         f_path = Path(f_path)
         f_path.parent.mkdir(parents=True, exist_ok=True)
         with open(f_path, "wb") as file:
-            pickle.dump(self, file)
+            torch.save(self, file)
         return f_path
 
     def l_pdf(self, obs_mvcp: torch.Tensor) -> torch.Tensor:
         """log probability density function (PDF) of the multivariate copula
 
         :param self: an instance of the DataVineCop dataclass
         :param obs_mvcp: observation of the multivariate copula, of shape (num_obs, num_dim)
@@ -559,19 +588,21 @@
         return res
 
     def rosenblatt_transform(
         self,
         obs_mvcp: torch.Tensor,
         tpl_sim: tuple = tuple(),
     ) -> torch.Tensor:
-        """Rosenblatt transformation, from the multivariate copula (with dependence) to the uniform multivariate copula (independent), using constructed vine copula
+        """Rosenblatt transformation, from the multivariate copula (with dependence)
+        to the uniform multivariate copula (independent), using constructed vine copula
 
         :param obs_mvcp: observation of the multivariate copula, of shape (num_obs, num_dim)
         :type obs_mvcp: torch.Tensor
-        :param tpl_sim: tuple of vertices (read from right to left) in a full simulation workflow, gives flexibility to experienced users, defaults to tuple()
+        :param tpl_sim: tuple of vertices (read from right to left) in a full simulation workflow,
+            gives flexibility to experienced users, defaults to tuple()
         :type tpl_sim: tuple, optional
         :return: ideally independent uniform multivariate copula, of shape (num_obs, num_dim)
         :rtype: torch.Tensor
         """
         num_dim = self.num_dim
         if not tpl_sim:
             tpl_sim = self.tpl_sim
@@ -636,21 +667,27 @@
         num_sim: int = 1,
         dct_first_vs: dict = {},
         tpl_sim: tuple = tuple(),
         seed: int = 0,
         device: str = "cpu",
         dtype: torch.dtype = torch.float64,
     ) -> torch.Tensor:
-        """full simulation/ quantile-regression/ conditional-simulation using the vine copula. Sequentially for each beginning vertex in the tpl_sim (from right to left, as from shallower lv to deeper lv in the DAG), walk upward by calling hinv until the top vertex (whose cond set is empty) is reached. (Recursively) call hfunc for the other upper vertex if necessary.
+        """full simulation/ quantile-regression/ conditional-simulation using the vine copula.
+        Sequentially for each beginning vertex in the tpl_sim
+        (from right to left, as from shallower lv to deeper lv in the DAG),
+        walk upward by calling hinv until the top vertex (whose cond set is empty) is reached.
+        (Recursively) call hfunc for the other upper vertex if necessary.
 
         :param num_sim: number of simulations; ignored when dct_first_vs is not empty
         :type num_sim: int
-        :param dct_first_vs: dict of {(vertex,cond_set): torch.Tensor(size=(n,1))} in quantile regression/ conditional simulation, where vertices are taken as given already; defaults to {}
+        :param dct_first_vs: dict of {(vertex,cond_set): torch.Tensor(size=(n,1))}
+            in quantile regression/ conditional simulation, where vertices are taken as given already; defaults to {}
         :type dct_first_vs: dict, optional
-        :param tpl_sim: tuple of vertices (read from right to left) in a full simulation workflow, gives flexibility to experienced users, defaults to tuple()
+        :param tpl_sim: tuple of vertices (read from right to left) in a full simulation workflow,
+            gives flexibility to experienced users, defaults to tuple()
         :type tpl_sim: tuple, optional
         :param seed: random seed for torch.manual_seed(), defaults to 0
         :type seed: int, optional
         :param device: device for torch.rand(), defaults to 'cpu'
         :type device: str, optional
         :param dtype: dtype for torch.rand(), defaults to torch.float64
         :type dtype: torch.dtype, optional
@@ -689,15 +726,16 @@
                 (v_r, s_up),
                 (v_down, s_down),
             ):
                 _update_ref_count(v=v, s=s)
 
         def visit_hinv(v_down: int, s_down: frozenset) -> tuple:
             """
-            hinv from (v_down,s_down) (surely exist) and (v_up,s_up) (may not exist yet and recursively call visit_hfunc if necessary)
+            hinv from (v_down,s_down) (surely exist) and (v_up,s_up)
+            (may not exist yet and recursively call visit_hfunc if necessary)
             to (v_down,s_up); then update dct_obs and dct_ref_count and do garbage collection
             """
             # * locate the bicop on upper level that connects the 3 vertices
             v_l, v_r, s_up, bcp = self._loc_bcp(v_down=v_down, s_down=s_down)
             # ! if v_down==v_r then go hinv1([(v_l,s_up), (v_r,s_down)])
             is_down_right = v_down == v_r
             (v_up, hinv) = (v_l, bcp.hinv1) if is_down_right else (v_r, bcp.hinv2)
```

### Comparing `torchvinecopulib-2024.4.1/torchvinecopulib/vinecop/_factory_vcp.py` & `torchvinecopulib-2024.4.2/torchvinecopulib/vinecop/_factory_vcp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,31 @@
-import pickle
-from collections import deque
+import json
+from ast import literal_eval
+from collections import defaultdict, deque
 from itertools import combinations
 from operator import itemgetter
 from pathlib import Path
 from typing import Deque
 
 import numpy as np
 import torch
 
-from ..bicop import bcp_from_obs
+from ..bicop import DataBiCop, bcp_from_obs
 from ..util import ENUM_FUNC_BIDEP
 from ._data_vcp import DataVineCop
 
 
 def _mst_from_edge_rvine(tpl_key_obs: tuple, dct_edge_lv: dict, s_rest: set) -> list:
-    """Construct Kruskal's MAXIMUM spanning tree (MST) from bivariate copula edges, restricted to rvine, using modified disjoint set/ union find.
+    """Construct Kruskal's MAXIMUM spanning tree (MST) from bivariate copula edges,
+    restricted to rvine, using modified disjoint set/ union find.
 
     :param tpl_key_obs: tuple of keys of (pseudo) observations, each key is a tuple of (vertex, cond set)
     :type tpl_key_obs: tuple
-    :param dct_edge_lv: dictionary of edges (vertex_left, vertex_right, cond_set) and corresponding bivariate dependence metric value
+    :param dct_edge_lv: dictionary of edges (vertex_left, vertex_right, cond_set)
+        and corresponding bivariate dependence metric value
     :type dct_edge_lv: dict
     :param s_rest: vertices to be kept deeper in the simulation workflow (static, wont update at each level)
     :type s_rest: set
     :return: list of edges (vertex_l, vertex_r, cond set) in the MST
     :rtype: list
     """
     # * edge2tree, rvine (Kruskal's MST, disjoint set/ union find)
@@ -74,17 +77,19 @@
 def _mst_from_edge_cvine(
     tpl_key_obs: tuple, dct_edge_lv: dict, s_first: set, deq_sim: Deque
 ) -> tuple:
     """Construct Kruskal's MAXIMUM spanning tree (MST) from bivariate copula edges, restricted to cvine
 
     :param tpl_key_obs: tuple of keys of (pseudo) observations, each key is a tuple of (vertex, cond set)
     :type tpl_key_obs: tuple
-    :param dct_edge_lv: dictionary of edges (vertex_left, vertex_right, cond set) and corresponding bivariate dependence metric value
+    :param dct_edge_lv: dictionary of edges (vertex_left, vertex_right, cond set)
+        and corresponding bivariate dependence metric value
     :type dct_edge_lv: dict
-    :param deq_sim: deque of vertices, as simulation workflow (read from right to left, as simulated pseudo-obs vertices from shallowest to deepest level) (dynamically updated at each level)
+    :param deq_sim: deque of vertices, as simulation workflow (read from right to left,
+        as simulated pseudo-obs vertices from shallowest to deepest level) (dynamically updated at each level)
     :type deq_sim: Deque
     :param s_first: set of vertices that are kept shallower in the simulation workflow (dynamically updated at each level)
     :type s_first: set
     :return: list of edges (vertex_left, vertex_right, cond set) in the MST; updated deq_sim; updated s_first
     :rtype: tuple
     """
     # * edge2tree, cvine (MST, restricted to cvine)
@@ -119,15 +124,16 @@
     # update the first set
     s_first -= {v_c}
     # * mst(cvine), deq_sim, s_first
     return mst, deq_sim, s_first
 
 
 def _mst_from_edge_dvine(tpl_key_obs: tuple, dct_edge_lv: dict, s_first: set) -> tuple:
-    """Construct Kruskal's MAXIMUM spanning tree (MST) from bivariate copula edges, restricted to dvine. For dvine the whole struct (and sim flow) is known after lv0, and this func is only called at lv0.
+    """Construct Kruskal's MAXIMUM spanning tree (MST) from bivariate copula edges, restricted to dvine.
+    For dvine the whole struct (and sim flow) is known after lv0, and this func is only called at lv0.
 
     :param tpl_key_obs: tuple of keys of (pseudo) observations, each key is a tuple of (vertex, cond set)
     :type tpl_key_obs: tuple
     :param dct_edge_lv: dictionary of edges (vertex_l, vertex_r, cond set) and corresponding bivariate dependence metric value
     :type dct_edge_lv: dict
     :param s_first: set of vertices that are kept shallower in the simulation workflow
     :type s_first: set
@@ -140,14 +146,15 @@
         # ! only two vertices
         v_head, v_tail = tpl_key_obs
         v_head, v_tail = v_head[0], v_tail[0]
         mst = [(v_head, v_tail, frozenset())]
     else:
         # ! more than two vertices
         import math
+
         from networkx import Graph
         from networkx.algorithms.approximation import threshold_accepting_tsp
 
         dct_cost = {
             (v_l, v_r): math.log1p(1 / max(abs(bidep), 1e-10))
             for (v_l, v_r, s_cond), bidep in dct_edge_lv.items()
         }
@@ -193,15 +200,16 @@
                     v_tail, v_neck, cost = v_nebr, v, i_cost
             mst = [(*sorted((v_head, v_neck)), frozenset())]
             for idx, v in enumerate(tsp[1:-1], start=1):
                 v_l, v_r = sorted((v, tsp[idx + 1]))
                 if {v_l, v_r} != {v_neck, v_tail}:
                     mst.append((v_l, v_r, frozenset()))
         else:
-            # ! both sets have more than one vertex (head-...-neck-body-...-tail, drop head-neck, add neck-body, drop body-tail)
+            # ! both sets have more than one vertex
+            # ! (head-...-neck-body-...-tail, drop head-neck, add neck-body, drop body-tail)
             tsp_first = threshold_accepting_tsp(G.subgraph(s_first), init_cycle="greedy")
             tsp_first.append(tsp_first[1])
             tsp_rest = threshold_accepting_tsp(G.subgraph(s_rest), init_cycle="greedy")
             tsp_rest.append(tsp_rest[1])
             cost = math.inf
             # * loop over two TSPs and pick the combination with min cost
             for idx_neck, _v_neck in enumerate(tsp_first[1:-1], start=1):
@@ -285,50 +293,62 @@
         "Gaussian",
         "Gumbel",
         "Independent",
         "Joe",
     ),
     topk: int = 2,
 ) -> DataVineCop:
-    """Construct a vine copula model from multivariate observations, with structure prescribed by either Dissmann's (MST per level) method or a given matrix. May prioritize some vertices to be first (shallower) in the quantile-regression/conditional-simulation workflow.
+    """Construct a vine copula model from multivariate observations,
+    with structure prescribed by either Dissmann's (MST per level) method or a given matrix.
+    May prioritize some vertices to be first (shallower) in the quantile-regression/conditional-simulation workflow.
 
     :param obs_mvcp: multivariate observations, of shape (num_obs, num_dim)
     :type obs_mvcp: torch.Tensor
-    :param is_Dissmann: whether to use Dissmann's method or follow a given matrix, defaults to True; Dissmann, J., Brechmann, E. C., Czado, C., & Kurowicka, D. (2013). Selecting and estimating regular vine copulae and application to financial returns. Computational Statistics & Data Analysis, 59, 52-69.
+    :param is_Dissmann: whether to use Dissmann's method or follow a given matrix,
+        defaults to True; Dissmann, J., Brechmann, E. C., Czado, C., & Kurowicka, D. (2013).
+        Selecting and estimating regular vine copulae and application to financial returns.
+        Computational Statistics & Data Analysis, 59, 52-69.
     :type is_Dissmann: bool, optional
     :param mtd_vine: one of 'cvine', 'dvine', 'rvine', defaults to "rvine"
     :type mtd_vine: str, optional
-    :param tpl_first: tuple of vertices to be prioritized (kept shallower) in the cond sim workflow. if empty then no priority is set, defaults to tuple()
+    :param tpl_first: tuple of vertices to be prioritized (kept shallower) in the cond sim workflow.
+        if empty then no priority is set, defaults to tuple()
     :type tpl_first: tuple[int], optional
-    :param matrix: a matrix of vine copula structure, of shape (num_dim, num_dim), used when is_Dissmann is False, defaults to None
+    :param matrix: a matrix of vine copula structure, of shape (num_dim, num_dim),
+        used when is_Dissmann is False, defaults to None
     :type matrix: np.ndarray | None, optional
-    :param mtd_bidep: method to calculate bivariate dependence, one of "kendall_tau", "mutual_info", "ferreira_tail_dep_coeff", "chatterjee_xi", "wasserstein_dist_ind", defaults to "chatterjee_xi"
+    :param mtd_bidep: method to calculate bivariate dependence, one of "kendall_tau", "mutual_info",
+        "ferreira_tail_dep_coeff", "chatterjee_xi", "wasserstein_dist_ind", defaults to "chatterjee_xi"
     :type mtd_bidep: str, optional
     :param thresh_trunc: threshold of Kendall's tau independence test, below which we reject independent bicop, defaults to 0.1
     :type thresh_trunc: float, optional
-    :param mtd_fit: method to fit bivariate copula, either 'itau' (inverse of tau) or 'mle' (maximum likelihood estimation); defaults to "itau"
+    :param mtd_fit: method to fit bivariate copula, either 'itau' (inverse of tau) or
+        'mle' (maximum likelihood estimation); defaults to "itau"
     :type mtd_fit: str, optional
     :param mtd_mle: optimization method for mle as used by scipy.optimize.minimize, defaults to "COBYLA"
     :type mtd_mle: str, optional
     :param mtd_sel: bivariate copula model selection criterion, either 'aic' or 'bic'; defaults to "aic"
     :type mtd_sel: str, optional
-    :param tpl_fam: tuple of str as candidate family names to fit bicop, could be a subset of ('Clayton', 'Frank', 'Gaussian', 'Gumbel', 'Independent', 'Joe', 'StudentT'), defaults to ( "Clayton", "Frank", "Gaussian", "Gumbel", "Independent", "Joe")
+    :param tpl_fam: tuple of str as candidate family names to fit bicop,
+        could be a subset of ('Clayton', 'Frank', 'Gaussian', 'Gumbel', 'Independent', 'Joe', 'StudentT'),
+        defaults to ( "Clayton", "Frank", "Gaussian", "Gumbel", "Independent", "Joe")
     :type tpl_fam: tuple[str, ...], optional
     :param topk: number of best "itau" fit taken into further "mle", used when mtd_fit is "mle"; defaults to 2
     :type topk: int, optional
     :raises ValueError: when mtd_vine is not one of 'cvine', 'dvine', 'rvine'
     :return: a constructed DataVineCop object
     :rtype: DataVineCop
     """
     is_kendall_tau = mtd_bidep == "kendall_tau"
     f_bidep = ENUM_FUNC_BIDEP[mtd_bidep]._value_
     num_dim = obs_mvcp.shape[1]
     s_first = set(tpl_first)
     s_rest = set(range(num_dim)) - s_first
-    # ! an object to record the order of sim (read from right to left, as simulated pseudo-obs vertices from shallowest to deepest level)
+    # ! an object to record the order of sim (read from right to left,
+    # ! as simulated pseudo-obs vertices from shallowest to deepest level)
     deq_sim = deque()
     r_D1 = range(num_dim - 1)
     dct_obs = {_: {} for _ in r_D1}
     # * tree is either from Dissmann (MST on edges, needs to record edges) or from matrix
     if is_Dissmann:
         dct_edge = {_: {} for _ in r_D1}
     dct_tree = {_: {} for _ in r_D1}
@@ -497,30 +517,43 @@
     """load a DataVineCop from a json file
 
     :param f_path: path to the json file, defaults to Path("./vcp.json")
     :type f_path: Path, optional
     :return: a DataVineCop object
     :rtype: DataVineCop
     """
-    from ..bicop import DataBiCop
-
     with open(f_path, "r") as file:
-        obj = eval(file.read())
-    return DataVineCop(
-        dct_bcp=obj["dct_bcp"],
-        dct_tree=obj["dct_tree"],
-        tpl_sim=obj["tpl_sim"],
-        mtd_bidep=obj["mtd_bidep"],
-    )
+        tmp_json = json.load(file)
+    #
+    dct_bcp = defaultdict(dict)
+    for lv, i_dct in tmp_json["dct_bcp"].items():
+        for key, val in i_dct.items():
+            v_l, v_r, s_cond = literal_eval(key)
+            s_cond = frozenset(s_cond)
+            val["par"] = tuple(val["par"])
+            dct_bcp[int(lv)][(v_l, v_r, s_cond)] = DataBiCop(**val)
+    tmp_json["dct_bcp"] = dict(dct_bcp)
+    #
+    dct_tree = defaultdict(dict)
+    for lv, i_dct in tmp_json["dct_tree"].items():
+        for key, val in i_dct.items():
+            v_l, v_r, s_cond = literal_eval(key)
+            s_cond = frozenset(s_cond)
+            dct_tree[int(lv)][(v_l, v_r, s_cond)] = val
+    tmp_json["dct_tree"] = dict(dct_tree)
+    #
+    tmp_json["tpl_sim"] = tuple(tmp_json["tpl_sim"])
+    #
+    return DataVineCop(**tmp_json)
 
 
-def vcp_from_pkl(f_path: Path = Path("./vcp.pkl")) -> DataVineCop:
-    """load a DataVineCop from a pickle file
+def vcp_from_pth(f_path: Path = Path("./vcp.pth")) -> DataVineCop:
+    """load a DataVineCop from a pth file
 
-    :param f_path: path to the pickle file, defaults to Path("./vcp.pkl")
+    :param f_path: path to the pth file, defaults to Path("./vcp.pth")
     :type f_path: Path, optional
     :return: a DataVineCop object
     :rtype: DataVineCop
     """
     with open(f_path, "rb") as file:
-        obj = pickle.load(file)
+        obj = torch.load(file)
     return obj
```

### Comparing `torchvinecopulib-2024.4.1/PKG-INFO` & `torchvinecopulib-2024.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchvinecopulib
-Version: 2024.4.1
+Version: 2024.4.2
 Summary: yet another vine copula library for PyTorch.
 Home-page: https://github.com/TY-Cheng/torchvinecopulib
 License: GNU GPLv3
 Keywords: vine copula,copula,torch
 Author: Tuoyuan Cheng
 Author-email: cty120120@gmail.com
 Maintainer: Xiaosheng You
@@ -82,17 +82,17 @@
 ```
 
 By `pip` from `./dist/*.whl` or `./dist/*.tar.gz` in this repo.
 Need to use proper file name.
 
 ```bash
 # inside project root folder
-pip install ./dist/torchvinecopulib-2024.4.1-py3-none-any.whl
+pip install ./dist/torchvinecopulib-2024.4.2-py3-none-any.whl
 # or
-pip install ./dist/torchvinecopulib-2024.4.1.tar.gz
+pip install ./dist/torchvinecopulib-2024.4.2.tar.gz
 ```
 
 ## Examples
 
 Visit the `./examples/` folder for `.ipynb` Jupyter notebooks.
 
 ## Documentation
@@ -138,17 +138,16 @@
 - Include a clear and descriptive title and description for your pull request.
 - Make sure all tests pass before submitting the pull request.
 - If your pull request addresses an open issue, reference the issue number in the description using the syntax `#issue_number`.
 - [in-place ops can be slower](https://discuss.pytorch.org/t/are-inplace-operations-faster/61209/4)
 - [torch.jit.script can be slower](https://discuss.pytorch.org/t/why-is-torch-jit-script-slower/120131/6)
 
 ### TODO
-1. non-par bicop
-2. more (non-parametric) `bicop` class in `torch`
-3. potentially deprecating `'mle'` from `mtd_fit`
+1. more (non-parametric) `bicop` class in `torch`
+2. potentially deprecating `'mle'` from `mtd_fit`
 
 ## License
 
 > Copyright (C) 2024 Tuoyuan Cheng, Xiaosheng You, Kan Chen
 >
 > This file is part of torchvinecopulib.
 > torchvinecopulib is free software: you can redistribute it and/or modify
```

