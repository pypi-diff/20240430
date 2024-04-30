# Comparing `tmp/feynamp-0.0.5.12.tar.gz` & `tmp/feynamp-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feynamp-0.0.5.12.tar", max compression
+gzip compressed data, was "feynamp-0.0.9.tar", max compression
```

## Comparing `feynamp-0.0.5.12.tar` & `feynamp-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0    35149 2024-04-04 09:31:27.109037 feynamp-0.0.5.12/LICENSE
--rw-r--r--   0        0        0     1259 2024-04-04 09:31:27.109037 feynamp-0.0.5.12/README.md
--rw-r--r--   0        0        0     1358 2024-04-04 09:31:27.113037 feynamp-0.0.5.12/feynamp/__init__.py
--rw-r--r--   0        0        0     3373 2024-04-04 09:31:27.113037 feynamp-0.0.5.12/feynamp/amplitude.py
--rw-r--r--   0        0        0     1651 2024-04-04 09:31:27.113037 feynamp-0.0.5.12/feynamp/form/__init__.py
--rw-r--r--   0        0        0     2187 2024-04-04 09:31:27.113037 feynamp-0.0.5.12/feynamp/form/color.py
--rw-r--r--   0        0        0     2191 2024-04-04 09:31:27.113037 feynamp-0.0.5.12/feynamp/form/form.py
--rw-r--r--   0        0        0     8567 2024-04-04 09:31:27.113037 feynamp-0.0.5.12/feynamp/form/lorentz.py
--rw-r--r--   0        0        0     7042 2024-04-04 09:31:27.113037 feynamp-0.0.5.12/feynamp/form/momentum.py
--rw-r--r--   0        0        0     1687 2024-04-04 09:31:27.113037 feynamp-0.0.5.12/feynamp/leg.py
--rw-r--r--   0        0        0      149 2024-04-04 09:31:27.113037 feynamp-0.0.5.12/feynamp/log.py
--rw-r--r--   0        0        0      469 2024-04-04 09:31:27.113037 feynamp-0.0.5.12/feynamp/math.py
--rw-r--r--   0        0        0     2029 2024-04-04 09:31:27.113037 feynamp-0.0.5.12/feynamp/momentum.py
--rw-r--r--   0        0        0     1525 2024-04-04 09:31:27.113037 feynamp-0.0.5.12/feynamp/propagator.py
--rw-r--r--   0        0        0      577 2024-04-04 09:31:27.113037 feynamp-0.0.5.12/feynamp/sympy/__init__.py
--rw-r--r--   0        0        0     6324 2024-04-04 09:31:27.113037 feynamp-0.0.5.12/feynamp/sympy/color.py
--rw-r--r--   0        0        0     3383 2024-04-04 09:31:27.113037 feynamp-0.0.5.12/feynamp/sympy/lorentz.py
--rw-r--r--   0        0        0      601 2024-04-04 09:31:27.113037 feynamp-0.0.5.12/feynamp/util.py
--rw-r--r--   0        0        0     6581 2024-04-04 09:31:27.113037 feynamp-0.0.5.12/feynamp/vertex.py
--rw-r--r--   0        0        0     2175 2024-04-04 09:31:27.117037 feynamp-0.0.5.12/pyproject.toml
--rw-r--r--   0        0        0     2021 1970-01-01 00:00:00.000000 feynamp-0.0.5.12/setup.py
--rw-r--r--   0        0        0     1972 1970-01-01 00:00:00.000000 feynamp-0.0.5.12/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-07 08:55:47.679557 feynamp-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1259 2024-04-07 08:55:47.679557 feynamp-0.0.9/README.md
+-rw-r--r--   0        0        0     1376 2024-04-07 08:55:47.699557 feynamp-0.0.9/feynamp/__init__.py
+-rw-r--r--   0        0        0     5022 2024-04-07 08:55:47.699557 feynamp-0.0.9/feynamp/amplitude.py
+-rw-r--r--   0        0        0     1948 2024-04-07 08:55:47.699557 feynamp-0.0.9/feynamp/form/__init__.py
+-rw-r--r--   0        0        0     3787 2024-04-07 08:55:47.699557 feynamp-0.0.9/feynamp/form/color.py
+-rw-r--r--   0        0        0    81814 2024-04-07 08:55:47.699557 feynamp-0.0.9/feynamp/form/colorh.py
+-rw-r--r--   0        0        0     4756 2024-04-07 08:55:47.699557 feynamp-0.0.9/feynamp/form/form.py
+-rw-r--r--   0        0        0     8972 2024-04-07 08:55:47.699557 feynamp-0.0.9/feynamp/form/lorentz.py
+-rw-r--r--   0        0        0     7351 2024-04-07 08:55:47.699557 feynamp-0.0.9/feynamp/form/momentum.py
+-rw-r--r--   0        0        0     1689 2024-04-07 08:55:47.699557 feynamp-0.0.9/feynamp/leg.py
+-rw-r--r--   0        0        0      149 2024-04-07 08:55:47.699557 feynamp-0.0.9/feynamp/log.py
+-rw-r--r--   0        0        0      469 2024-04-07 08:55:47.699557 feynamp-0.0.9/feynamp/math.py
+-rw-r--r--   0        0        0     2029 2024-04-07 08:55:47.699557 feynamp-0.0.9/feynamp/momentum.py
+-rw-r--r--   0        0        0     1560 2024-04-07 08:55:47.699557 feynamp-0.0.9/feynamp/propagator.py
+-rw-r--r--   0        0        0      577 2024-04-07 08:55:47.699557 feynamp-0.0.9/feynamp/sympy/__init__.py
+-rw-r--r--   0        0        0     6324 2024-04-07 08:55:47.699557 feynamp-0.0.9/feynamp/sympy/color.py
+-rw-r--r--   0        0        0     3383 2024-04-07 08:55:47.699557 feynamp-0.0.9/feynamp/sympy/lorentz.py
+-rw-r--r--   0        0        0      601 2024-04-07 08:55:47.699557 feynamp-0.0.9/feynamp/util.py
+-rw-r--r--   0        0        0     6916 2024-04-07 08:55:47.699557 feynamp-0.0.9/feynamp/vertex.py
+-rw-r--r--   0        0        0     2198 2024-04-07 08:55:48.703551 feynamp-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2026 1970-01-01 00:00:00.000000 feynamp-0.0.9/setup.py
+-rw-r--r--   0        0        0     1989 1970-01-01 00:00:00.000000 feynamp-0.0.9/PKG-INFO
```

### Comparing `feynamp-0.0.5.12/LICENSE` & `feynamp-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `feynamp-0.0.5.12/README.md` & `feynamp-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `feynamp-0.0.5.12/feynamp/__init__.py` & `feynamp-0.0.9/feynamp/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .amplitude import feynman_diagram_to_string
+from .amplitude import complex_conjugate, feynman_diagram_to_string
 from .log import debug
 from .propagator import find_propagator_in_model, get_propagator_math
 from .vertex import find_vertex_in_model, get_vertex_math
 
 
 def get_spin_average(fds):
     """
@@ -27,15 +27,15 @@
     Initial quarks produce an averaging by 1/3 each
     Initial gluons produce an averaging by 1/8 each
     """
     r = []
     for leg in fds[0].get_incoming():
         if leg.pdgid == 21:
             r += ["1/8"]
-        elif leg.pdgid in range(1, 7) or -leg.pdgid in range(1, 17):
+        elif leg.pdgid in range(1, 7) or -leg.pdgid in range(1, 7):
             r += ["1/3"]
         elif leg.pdgid == 22:
             r += ["1"]
         elif leg.pdgid == 23:
             r += ["1"]
         elif leg.pdgid in range(11, 19) or -leg.pdgid in range(11, 19):
             r += ["1"]
```

### Comparing `feynamp-0.0.5.12/feynamp/form/__init__.py` & `feynamp-0.0.9/feynamp/form/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,19 +5,20 @@
 import form
 import sympy
 from feynml.feynmandiagram import FeynmanDiagram
 from feynmodel.feyn_model import FeynModel
 
 import feynamp.amplitude as amplitude
 from feynamp import get_color_average, get_spin_average
-from feynamp.form.color import get_color
-from feynamp.form.lorentz import get_gammas, get_polarisation_sums
+from feynamp.form.color import apply_color_parallel
+from feynamp.form.lorentz import get_gammas, get_metrics, get_polarisation_sums
 from feynamp.form.momentum import (
     apply,
     apply_den,
+    apply_parallel,
     get_kinematics,
     get_mandelstamm,
     get_onshell,
 )
 from feynamp.log import debug
 
 # TODO compute squared  functino which coutns legs!!"!!!" and picks right mandelstamm,s
@@ -25,38 +26,46 @@
 
 def compute_squared(fds: List[FeynmanDiagram], fm: FeynModel, tag=False):
     dims = fds[0].get_externals_size()
     for fd in fds:
         assert (
             dims == fd.get_externals_size()
         ), "All FeynmanDiagrams must have the same external legs"
-    s2 = amplitude.square(fds, fm, tag=tag)
+    s2 = amplitude.square_parallel(fds, fm, tag=tag)
     debug(f"{s2=}")
+
+    s2 = apply_color_parallel(s2)
+
     fs = ""
+    fs += get_metrics()
+    # fs += get_color()
+    # fs += get_kinematics()
+    # fs += get_onshell(fds, fm)
+    # fs += get_mandelstamm(fds, fm)
+    # This is where it gets expensive
     fs += get_polarisation_sums(fds, fm)
+    fs += get_kinematics()
+    fs += get_onshell(fds, fm)
     fs += get_gammas()
-    fs += get_color()
     fs += get_kinematics()
     fs += get_onshell(fds, fm)
     fs += get_mandelstamm(fds, fm)
 
-    rs = apply(s2, fs)
+    rs = apply_parallel(s2, fs)
+    rs = " + ".join([f"({r})" for r in rs])
     debug(f"{rs=}")
 
     rr = apply_den(
         rs,
         get_onshell(fds, fm) + get_mandelstamm(fds, fm),
     )
     debug(f"{rr=}")
 
-    ret = sympy.simplify(
-        sympy.parse_expr(
-            rr.replace("Mom_", "")
-            .replace(".", "_")
-            .replace("^", "**")
-            .replace("mss", "s")
-            .replace("msu", "u")
-            .replace("mst", "t")
-        )
-        * sympy.parse_expr("*".join([*get_color_average(fds), *get_spin_average(fds)]))
-    )
+    ret = sympy.parse_expr(
+        rr.replace("Mom_", "")
+        .replace(".", "_")
+        .replace("^", "**")
+        .replace("mss", "s")
+        .replace("msu", "u")
+        .replace("mst", "t")
+    ) * sympy.parse_expr("*".join([*get_color_average(fds), *get_spin_average(fds)]))
     return ret
```

### Comparing `feynamp-0.0.5.12/feynamp/form/lorentz.py` & `feynamp-0.0.9/feynamp/form/lorentz.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,17 +53,14 @@
 endrepeat;
 """
 
 
 # TODO implement collecting of gammas and form calc solving of it
 # idea: GammaCollect(1,spin1,spin2, mu,nu,...) run through and then apply to expression
 gamma_collect = """
-repeat;
-id Metric(Mua?,Mub?) = d_(Mua,Mub);
-endrepeat;
 #do i = 1, 10
 once Gamma(Mux?,Spin1?,Spin2?) = GammaCollect(`i',Spin1,Spin2,Mux);
 repeat;
 id GammaCollect(`i',Spin1?,Spin2?,?mus)*Gamma(Mux?, Spin2?,Spin3?) = GammaCollect(`i',Spin1,Spin3, ?mus, Mux);
 id GammaCollect(`i',Spin1?,Spin2?,?mus)*GammaId(Spin2?,Spin3?) = GammaCollect(`i',Spin1,Spin3, ?mus)*gi_(`i');
 endrepeat;
 id GammaCollect(`i',Spin1?,Spin1?,?mus) = g_(`i',?mus);
@@ -75,21 +72,39 @@
 id GammaIdCollect(`i',Spin1?,Spin2?)*GammaId(Spin2?,Spin3?) = GammaIdCollect(`i',Spin1,Spin3)*gi_(`i');
 endrepeat;
 id GammaIdCollect(`i',Spin1?,Spin1?) = 1;
 trace4, `i';
 #enddo
 """
 
+metrics = """
+* Simplify metrics, here let form handle it 
+repeat;
+id Metric(Mua?,Mub?) = d_(Mua,Mub);
+endrepeat;
+"""
+
+
+def get_metrics():
+    return metrics
+
+
+def apply_metrics(string_expr):
+    s = string_to_form(string_expr)
+    from .color import color_init
+
+    return run(init + color_init + f"Local TMP = {s};" + get_metrics())
+
 
 def get_gammas():
     return new_get_gammas()
 
 
 def new_get_gammas():
-    return get_dirac_trick() + gamma_collect
+    return get_dirac_trick() + get_metrics() + gamma_collect
 
 
 def get_gammas_v1():
     return get_polarisation_sum_v1() + get_dirac_trick() + gammas
 
 
 def apply_gammas(string_expr):
@@ -99,15 +114,19 @@
 
 def get_orthogonal_polarisation_momentum(
     leg: Leg, fds: List[FeynmanDiagram], model: FeynModel
 ):
     for fd in [fds[0]]:
         for fleg in fd.legs:
             p = find_leg_in_model(fd, fleg, model)
-            if is_mass_zero(p) and fleg != leg:
+            if (
+                is_mass_zero(p)
+                and fleg != leg
+                and leg.is_incoming() == fleg.is_incoming()
+            ):
                 mom = insert_momentum(fleg.momentum.name)
                 return mom
     raise ValueError("No orthogonal momentum found")
 
 
 def get_polarisation_sums(fds: List[FeynmanDiagram], model: FeynModel):
     pol_sums = ""
```

### Comparing `feynamp-0.0.5.12/feynamp/form/momentum.py` & `feynamp-0.0.9/feynamp/form/momentum.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 from typing import List
 
 from feynml.feynmandiagram import FeynmanDiagram
 from feynmodel.feyn_model import FeynModel
 
 # from feynamp.form import *
-from feynamp.form.form import init, run, string_to_form
+from feynamp.form.form import init, run, run_parallel, string_to_form
 from feynamp.leg import find_leg_in_model
 from feynamp.log import warning
 from feynamp.momentum import insert_mass, insert_momentum
 
 momenta = """
 repeat;
     id P(Mu1?,Moma?)*P(Mu1?,Momb?) = Moma.Momb;
@@ -47,26 +47,37 @@
 
 
 def apply_denominators(string_expr):
     s = string_to_form(string_expr)
     return run(init + f"Local TMP = {s};" + denominators)
 
 
+def apply_parallel(amps: List[str], operations: str):
+    return run_parallel(init, operations, [string_to_form(a) for a in amps])
+
+
 def apply(string_expr, str_a):
     s = string_to_form(string_expr)
     return run(init + f"Local TMP = {s};" + str_a)
 
 
 def apply_den(string_expr, str_f):
     # re match all Dens
     s = string_expr
+    # find all denominators
     res = re.findall(r"Den\(([a-zA-Z0-9_+*-\.^]+)\)", string_expr)
+
+    # print(string_expr)
+    # print("rDens: ", len(res), res)
+    # only keep unique
+    res = list(set(res))
     if res:
-        for og in res:  # TODO parallelize? each as one var in form?
-            g = apply(og, str_f)
+        new_gs = apply_parallel(res, str_f)
+        # print("Dens: ", len(res), res)
+        for og, g in zip(res, new_gs):
             s = s.replace("Den(" + og + ")", "1/(" + g + ")")
     return s
 
 
 def get_onshell(fds: List[FeynmanDiagram], model: FeynModel):
     if isinstance(fds, FeynmanDiagram):
         warning(
```

### Comparing `feynamp-0.0.5.12/feynamp/leg.py` & `feynamp-0.0.9/feynamp/leg.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     # give particles color vectors to sum over them in the end (or better average)
     # TODO this could be also done as incoming vs outcoming
     if p.color == 8:
         # if particle is a gluon give it a adjoint color function
         ret += f"VA(Glu{p.particle.id},{mom})*"
     if p.color == 3 or p.color == -3:
         # if particle is a quark give it a fundamental color function
-        ret += f"VC(Col{p.particle.id},{mom})*"
+        ret += f"VC(Color{p.particle.id},{mom})*"
 
     if p.spin == 3:
         if leg.is_incoming():
             ret += f"eps(Mu{p.particle.id},Pol{p.particle.id},{mom})"
         else:
             ret += f"eps_star(Mu{p.particle.id},Pol{p.particle.id},{mom})"
     if p.spin == 2:
```

### Comparing `feynamp-0.0.5.12/feynamp/momentum.py` & `feynamp-0.0.9/feynamp/momentum.py`

 * *Files identical despite different names*

### Comparing `feynamp-0.0.5.12/feynamp/propagator.py` & `feynamp-0.0.9/feynamp/propagator.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,25 +13,25 @@
     p = find_propagator_in_model(fd, prop, model)
     if p.particle.momentum is None or p.particle.momentum.name is None:
         raise ValueError("Momentum not set for particle")
     mom = insert_momentum(p.particle.momentum.name)
     mass = insert_mass(p.mass.name)
     ret = ""
     if p.color == 3 or p.color == -3:
-        ret += f"df(ColIn{p.particle.id},ColOut{p.particle.id})*"
+        ret += f"df(ColorIn{p.particle.id},ColorOut{p.particle.id})*"
     if p.color == 8:
         ret += f"da(GluIn{p.particle.id},GluOut{p.particle.id})*"
     # if boson just 1/(p^2-m^2)
     if p.spin == 3:
         # nid = generate_new_id()
         # TODO treate denominators differently for loops etc?
-        ret += f"Metric(MuIn{p.particle.id},MuOut{p.particle.id})*"
+        ret += f"(-1)*complex(0,1)*Metric(MuIn{p.particle.id},MuOut{p.particle.id})*"
     elif p.spin == 2:  # TODO handle plus minus mass for fermions
         nid = generate_new_id()
-        ret += f"(P(Mu{nid},{mom})*Gamma(Mu{nid},SpinIn{p.particle.id},SpinOut{p.particle.id})"
+        ret += f"complex(0,1)*(P(Mu{nid},{mom})*Gamma(Mu{nid},SpinIn{p.particle.id},SpinOut{p.particle.id})"
         ret += f" + {mass}*GammaId(SpinIn{p.particle.id},SpinOut{p.particle.id}))*"
     else:
         raise ValueError("Spin not set for particle")
     return ret + f"Denom({mom},{mass})"
 
 
 def find_propagator_in_model(fd, prop, model):
```

### Comparing `feynamp-0.0.5.12/feynamp/sympy/__init__.py` & `feynamp-0.0.9/feynamp/sympy/__init__.py`

 * *Files identical despite different names*

### Comparing `feynamp-0.0.5.12/feynamp/sympy/color.py` & `feynamp-0.0.9/feynamp/sympy/color.py`

 * *Files identical despite different names*

### Comparing `feynamp-0.0.5.12/feynamp/sympy/lorentz.py` & `feynamp-0.0.9/feynamp/sympy/lorentz.py`

 * *Files identical despite different names*

### Comparing `feynamp-0.0.5.12/feynamp/util.py` & `feynamp-0.0.9/feynamp/util.py`

 * *Files identical despite different names*

### Comparing `feynamp-0.0.5.12/feynamp/vertex.py` & `feynamp-0.0.9/feynamp/vertex.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,24 +4,27 @@
 import numpy as np
 from feynml.connector import Connector
 from feynml.id import generate_new_id
 from feynml.leg import Leg
 from feynml.propagator import Propagator
 from feynml.vertex import Vertex
 
+from feynamp.log import debug, info
 from feynamp.momentum import insert_momentum
 from feynamp.util import safe_index_replace
 
 
 def insert_color_types(s: str):
     """ """
     # We use the non greedy .*? to match multiple occurances individually
-    s = re.sub(r"T\((.*?),(.*?),(.*?)\)", r"T(Glu\1,Col\2,Col\3)", s)
+    # s = re.sub(r"T\((.*?),(.*?),(.*?)\)", r"T(Glu\1,Color\2,Color\3)", s)
+    # TODO do we want this? Or above
+    s = re.sub(r"T\((.*?),(.*?),(.*?)\)", r"T(Color\2,Color\3,Glu\1)", s)
     s = re.sub(r"f\((.*?),(.*?),(.*?)\)", r"f(Glu\1,Glu\2,Glu\3)", s)
-    s = re.sub(r"Identity\((.*?),(.*?)\)", r"Identity(Col\1,Col\2)", s)
+    s = re.sub(r"Identity\((.*?),(.*?)\)", r"Identity(Color\1,Color\2)", s)
     return s
 
 
 def insert_lorentz_types(s: str, connections: List[Connector], vertex: Vertex):
     # We use the non greedy .*? to match multiple occurances individually
     s = re.sub(r"Gamma\((.*?),(.*?),(.*?)\)", r"Gamma(Mu\1,Spin\2,Spin\3)", s)
     s = re.sub(r"ProjP\((.*?),(.*?)\)", r"ProjP(Spin\1,Spin\2)", s)
@@ -32,15 +35,17 @@
     for g in matches:
         # find connection with g[1] id in connections
         repl = None
         for c in connections:
             if c.id == g[1] or "In" + str(c.id) == g[1] or "Out" + str(c.id) == g[1]:
                 # TODO: is this correct?
                 if c.goes_into(vertex):
-                    repl = "P(Mu" + g[0] + "," + insert_momentum(c.momentum.name) + ")"
+                    repl = (
+                        "(P(Mu" + g[0] + "," + insert_momentum(c.momentum.name) + "))"
+                    )
                     break
                 else:
                     repl = (
                         "(-P(Mu" + g[0] + "," + insert_momentum(c.momentum.name) + "))"
                     )
                     break
         if repl is None:
@@ -79,14 +84,16 @@
     v = find_vertex_in_model(fd, vertex, model)
     if v is None:
         raise Exception(f"Vertex {vertex} not found in model")
         # return None
     assert len(v.color) == len(v.lorentz)
     cret = []
     lret = []
+    info(f"{v.color=}")
+    info(f"{v.lorentz=}")
     for j in range(len(v.color)):
         col = v.color[j]
         nid = generate_new_id()
         col = safe_index_replace(col, str(-1), str(nid))
         for i, vv in enumerate(v.particles):
             if isinstance(v.connections[i], Leg):
                 col = safe_index_replace(col, str(i + 1), str(v.connections[i].id))
@@ -101,15 +108,16 @@
                 raise Exception(
                     f"Connection {v.connections[i]} not a leg or propagator"
                 )
         if typed:
             col = insert_color_types(col)
         cret.append(col)
     for k in range(len(v.lorentz)):
-        lor = v.lorentz[j].structure
+        lor = v.lorentz[k].structure
+        debug(f"{lor=}")
         nid = generate_new_id()
         lor = safe_index_replace(lor, str(-1), str(nid))
         for i, vv in enumerate(v.particles):
             if isinstance(v.connections[i], Leg):
                 lor = safe_index_replace(lor, str(i + 1), str(v.connections[i].id))
             elif isinstance(v.connections[i], Propagator):
                 lor = safe_index_replace(
@@ -121,18 +129,19 @@
             else:
                 raise Exception(
                     f"Connection {v.connections[i]} not a leg or propagator"
                 )
         if typed:
             lor = insert_lorentz_types(lor, v.connections, vertex)
         lret.append(lor)
-    ret = []
+    vertex_math = []
     for k, v in v.couplings.items():
-        ret.append((v.value, cret[k[0]], lret[k[1]]))
-    return ret
+        vertex_math.append((v.value, cret[k[0]], lret[k[1]]))
+    debug(f"{vertex_math=}")
+    return vertex_math
 
 
 def find_vertex_in_model(fd, vertex, model):
     """
     Finds the model vertex corresponding to the given FeynmanDiagram vertex
 
     Note: Sorting is to check for the correct particles in a vertex given they can be in any order and have duplicates
```

### Comparing `feynamp-0.0.5.12/pyproject.toml` & `feynamp-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 [tool.poetry]
 name = "feynamp"
-version = "0.0.5.12"
+version = "0.0.9"
 description = "Compute Feynman diagrams"
 authors = ["Alexander Puck Neuwirth <alexander@neuwirth-informatik.de>"]
 readme = "README.md"
 repository = "https://github.com/APN-Pucky/feynamp"
 
 [tool.poetry.dependencies]
 python = "^3.8"
+pqdm = "*"
 sympy = "*"
 python-form = "*"
 
 feynml = ">=0.2.26"
 #feynml = {path= "../feynml", develop = true }
 
 feynmodel = ">=0.0.5"
 #feynmodel = {path= "../feynmodel", develop = true }
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
-equation-database = ">=2024.4.4"
+equation-database = ">=2024.4.5"
 #equation-database = {path="../equation-database", develop = true}
 pytest = "*"
 pytest-cov =  "*"
 pytest-profiling =  "*"
 pytest-line-profiler-apn = ">=0.1.3"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = ">=2.20,<4.0"
+snakeviz = "*"
 ipython =  "*"
 jupyterlab =  "*"
 jupyter = "*"
 pyfeyn2 = ">=2.3.6"
 #pyfeyn2 = {path= "../pyfeyn2", develop = true }
 pyqgraf = ">=0.0.14"
 #pyqgraf = {path= "../pyqgraf", develop = true }
```

### Comparing `feynamp-0.0.5.12/setup.py` & `feynamp-0.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['feynamp', 'feynamp.form', 'feynamp.sympy']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['feynml>=0.2.26', 'feynmodel>=0.0.5', 'python-form', 'sympy']
+['feynml>=0.2.26', 'feynmodel>=0.0.5', 'pqdm', 'python-form', 'sympy']
 
 setup_kwargs = {
     'name': 'feynamp',
-    'version': '0.0.5.12',
+    'version': '0.0.9',
     'description': 'Compute Feynman diagrams',
     'long_description': '# FeynAmp\n\n[![PyPI version][pypi image]][pypi link] [![PyPI version][pypi versions]][pypi link]  ![downloads](https://img.shields.io/pypi/dm/feynamp.svg)\n\n[![test][a t image]][a t link]      [![Coverage Status][c t i]][c t l]  [![Codacy Badge](https://app.codacy.com/project/badge/Coverage/b7192679265b441cb534c9dc06d1b350)](https://app.codacy.com/gh/APN-Pucky/feynamp/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage)   [![Codacy Badge](https://app.codacy.com/project/badge/Grade/b7192679265b441cb534c9dc06d1b350)](https://app.codacy.com/gh/APN-Pucky/feynamp/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)\n\n\n## Related\n\n* Mathematica: FormCalc, FeynCalc\n* Julia: https://arxiv.org/pdf/2310.07634.pdf\n\n[pypi image]: https://badge.fury.io/py/feynamp.svg\n[pypi link]: https://pypi.org/project/feynamp/\n[pypi versions]: https://img.shields.io/pypi/pyversions/feynamp.svg\n\n[a t link]: https://github.com/APN-Pucky/feynamp/actions/workflows/test.yml\n[a t image]: https://github.com/APN-Pucky/feynamp/actions/workflows/test.yml/badge.svg\n\n[c t l]: https://coveralls.io/github/APN-Pucky/feynamp?branch=master\n[c t i]: https://coveralls.io/repos/github/APN-Pucky/feynamp/badge.svg?branch=master\n',
     'author': 'Alexander Puck Neuwirth',
     'author_email': 'alexander@neuwirth-informatik.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/APN-Pucky/feynamp',
```

### Comparing `feynamp-0.0.5.12/PKG-INFO` & `feynamp-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: feynamp
-Version: 0.0.5.12
+Version: 0.0.9
 Summary: Compute Feynman diagrams
 Home-page: https://github.com/APN-Pucky/feynamp
 Author: Alexander Puck Neuwirth
 Author-email: alexander@neuwirth-informatik.de
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: feynml (>=0.2.26)
 Requires-Dist: feynmodel (>=0.0.5)
+Requires-Dist: pqdm
 Requires-Dist: python-form
 Requires-Dist: sympy
 Project-URL: Repository, https://github.com/APN-Pucky/feynamp
 Description-Content-Type: text/markdown
 
 # FeynAmp
```

