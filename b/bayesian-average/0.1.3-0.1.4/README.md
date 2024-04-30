# Comparing `tmp/bayesian_average-0.1.3.tar.gz` & `tmp/bayesian_average-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bayesian_average-0.1.3.tar", last modified: Tue Apr 30 18:26:28 2024, max compression
+gzip compressed data, was "bayesian_average-0.1.4.tar", last modified: Tue Apr 30 20:39:28 2024, max compression
```

## Comparing `bayesian_average-0.1.3.tar` & `bayesian_average-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 martino    (501) staff       (20)        0 2024-04-30 18:26:28.321846 bayesian_average-0.1.3/
--rw-rw-r--   0 martino    (501) staff       (20)     1274 2024-03-28 16:44:26.000000 bayesian_average-0.1.3/LICENSE.txt
--rw-r--r--   0 martino    (501) staff       (20)      253 2024-04-30 18:26:28.321602 bayesian_average-0.1.3/PKG-INFO
--rw-r--r--   0 martino    (501) staff       (20)     2090 2024-04-30 10:50:43.000000 bayesian_average-0.1.3/README.md
-drwxr-xr-x   0 martino    (501) staff       (20)        0 2024-04-30 18:26:28.320687 bayesian_average-0.1.3/bayesian_average/
--rw-rw-r--   0 martino    (501) staff       (20)     1313 2024-04-30 15:27:17.000000 bayesian_average-0.1.3/bayesian_average/__init__.py
--rw-r--r--   0 martino    (501) staff       (20)       21 2024-04-30 13:41:55.000000 bayesian_average-0.1.3/bayesian_average/_version.py
--rw-rw-r--   0 martino    (501) staff       (20)     6499 2024-04-30 14:35:11.000000 bayesian_average-0.1.3/bayesian_average/average.py
-drwxr-xr-x   0 martino    (501) staff       (20)        0 2024-04-30 18:26:28.321390 bayesian_average-0.1.3/bayesian_average.egg-info/
--rw-r--r--   0 martino    (501) staff       (20)      253 2024-04-30 18:26:28.000000 bayesian_average-0.1.3/bayesian_average.egg-info/PKG-INFO
--rw-r--r--   0 martino    (501) staff       (20)      276 2024-04-30 18:26:28.000000 bayesian_average-0.1.3/bayesian_average.egg-info/SOURCES.txt
--rw-r--r--   0 martino    (501) staff       (20)        1 2024-04-30 18:26:28.000000 bayesian_average-0.1.3/bayesian_average.egg-info/dependency_links.txt
--rw-r--r--   0 martino    (501) staff       (20)       17 2024-04-30 18:26:28.000000 bayesian_average-0.1.3/bayesian_average.egg-info/top_level.txt
--rw-r--r--   0 martino    (501) staff       (20)       38 2024-04-30 18:26:28.321888 bayesian_average-0.1.3/setup.cfg
--rw-r--r--   0 martino    (501) staff       (20)      457 2024-04-30 13:20:30.000000 bayesian_average-0.1.3/setup.py
+drwxr-xr-x   0 martino    (501) staff       (20)        0 2024-04-30 20:39:28.838167 bayesian_average-0.1.4/
+-rw-rw-r--   0 martino    (501) staff       (20)     1274 2024-03-28 16:44:26.000000 bayesian_average-0.1.4/LICENSE.txt
+-rw-r--r--   0 martino    (501) staff       (20)     1414 2024-04-30 20:39:28.837957 bayesian_average-0.1.4/PKG-INFO
+-rw-r--r--   0 martino    (501) staff       (20)     3894 2024-04-30 19:25:01.000000 bayesian_average-0.1.4/README.md
+drwxr-xr-x   0 martino    (501) staff       (20)        0 2024-04-30 20:39:28.837158 bayesian_average-0.1.4/bayesian_average/
+-rw-rw-r--   0 martino    (501) staff       (20)     1308 2024-04-30 19:25:55.000000 bayesian_average-0.1.4/bayesian_average/__init__.py
+-rw-r--r--   0 martino    (501) staff       (20)       21 2024-04-30 19:17:04.000000 bayesian_average-0.1.4/bayesian_average/_version.py
+-rw-rw-r--   0 martino    (501) staff       (20)     6563 2024-04-30 20:32:56.000000 bayesian_average-0.1.4/bayesian_average/average.py
+drwxr-xr-x   0 martino    (501) staff       (20)        0 2024-04-30 20:39:28.837765 bayesian_average-0.1.4/bayesian_average.egg-info/
+-rw-r--r--   0 martino    (501) staff       (20)     1414 2024-04-30 20:39:28.000000 bayesian_average-0.1.4/bayesian_average.egg-info/PKG-INFO
+-rw-r--r--   0 martino    (501) staff       (20)      276 2024-04-30 20:39:28.000000 bayesian_average-0.1.4/bayesian_average.egg-info/SOURCES.txt
+-rw-r--r--   0 martino    (501) staff       (20)        1 2024-04-30 20:39:28.000000 bayesian_average-0.1.4/bayesian_average.egg-info/dependency_links.txt
+-rw-r--r--   0 martino    (501) staff       (20)       17 2024-04-30 20:39:28.000000 bayesian_average-0.1.4/bayesian_average.egg-info/top_level.txt
+-rw-r--r--   0 martino    (501) staff       (20)       38 2024-04-30 20:39:28.838206 bayesian_average-0.1.4/setup.cfg
+-rw-r--r--   0 martino    (501) staff       (20)      460 2024-04-30 19:16:24.000000 bayesian_average-0.1.4/setup.py
```

### Comparing `bayesian_average-0.1.3/LICENSE.txt` & `bayesian_average-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bayesian_average-0.1.3/bayesian_average/__init__.py` & `bayesian_average-0.1.4/bayesian_average/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,12 +5,12 @@
 Calculation of robust weigted average from a set of data points and their uncertainties based on Bayesian statistical methods.
 The proposed weighted average is particularly adapted to inconsistent data and for the presence of outliers, which can both false the results of standard methods.
 
 This robust weighted average is based on Bayesian statistics assuming a normal disrtribution for each data point and considering the associated uncertainty $x_i$ values as just a lower bound of the *real* possibly larger uncertainty $\sigma'$.
 It is obtained by the marginalization on $\sigma'$, this result in a modified probability distribution for each $x_i$ that still depens on $\sigma_i$.
 Two different priors are proposed for $\sigma'$: the non informative Jeffreys' prior $p(\sigma') \propto 1/ \sigma'$ (more precisely its limit, see Ref.[1] in README file), and a modified version of it $p(\sigma') \propto 1/ (\sigma')^2$ proposed in Ref.[2] (in README file).
 
-For both priors, the weighted average and its associated uncertainty are obtained numerically using different types of minimisation algorithms.
+For both priors, the weighted average and its associated uncertainty are obtained numerically using `basinhopping` minimisation algorithm.
 
 In addition, the standard (inverse-variance) weighted average is also available for possible comparisons.
 
 """
```

### Comparing `bayesian_average-0.1.3/bayesian_average/average.py` & `bayesian_average-0.1.4/bayesian_average/average.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,39 +16,41 @@
     return av_value, sig_value
 
 def cwa(data, sigma):    
     """
     Conservative weighted average proposed by Sivia in 2004 (see references in README file).
     The priors of the real uncertainty value are proportional to sigma_0/sigma^2, where sigma_0 is the value provided by the user
     The bounds of the prior are [sigma_0, infinite].
-    This is a modified and normalisable version of the non-informative Jeffeys' prior proportional to 1/sigma.
+    This is a modified and normalisable version of the non-informative Jeffeys' prior.
     """
     loglike = np.sum([log((1 - exp(-(x_temp - mu)**2 / (s_temp**2 * 2))) / (x_temp - mu)**2) for x_temp, s_temp in zip(data, sigma)]) #loglikelihood function
     ddloglike = diff(loglike, mu, 2) #second derivative
     negloglike = lambdify(mu, -loglike)
     av_value = basinhopping(negloglike, np.average(data)).x[0] #find minima of negative loglikelihood
     sig_value = 1/sqrt(-ddloglike.subs(mu, av_value)) #calculate sigma        
     return av_value, sig_value
 
 def jwa(data, sigma):    
     """
     Jeffreys weighted average proposed by Trassinelli and Maxton in 2024 (see references in README file).
-    The priors of the real uncertainty value are non-informative Jeffeys' prior proportional to 1/sigma.
+    The priors of the real uncertainty value are non-informative Jeffeys' prior proportional to 1/sigma'.
     Because of the non-normalisability of the final probability distribution, this weighted average results 
-    correspond to the  limit case with prior bounds [sigma_0, sigma_max] with sigma_max -> infinite. 
+    correspond to the  limit case with prior bounds [sigma, sigma_max] with sigma_max -> infinite. 
     The final probability distribution is, however not a proper probability distribution.
     """
     loglike = np.sum([log(erf((x_temp - mu)/(sqrt(2)*s_temp)) / (x_temp-mu)) for x_temp, s_temp in zip(data, sigma)])
     ddloglike = diff(loglike, mu, 2) #second derivative
     negloglike = lambdify(mu, -loglike)
     av_value = basinhopping(negloglike, np.average(data)).x[0] #find minima of negative loglikelihood
     sig_value = 1/sqrt(-ddloglike.subs(mu, av_value)).evalf() #calculate sigma        
     return av_value, sig_value
 
-def plot_average(data, sigma, plot_data = False, wa_val = False, cwa_val = False, jwa_val = True, wa_loglike = False, cwa_loglike = False, jwa_loglike = True, normalize = False):
+def plot_average(data, sigma, plot_data = False, wa_val = False, cwa_val = False, jwa_val = True, 
+                 wa_loglike = False, cwa_loglike = False, jwa_loglike = True, 
+                 legendon = True, normalize = False):
     """
     This is the main plot function of the library.
 
     Three weighted average are available:
         - wa: standard weigted average
         - jwa: Jeffreys weighted average
         - cwa: conservative weighted average
@@ -76,33 +78,33 @@
         if cwa_loglike:
             loglike = np.sum([log(sqrt(2 / pi) * s_temp * (1 - exp(-(x_temp - mu)**2 / (s_temp**2 * 2))) / (x_temp - mu)**2) for x_temp, s_temp in zip(data, sigma)])
             loglike_lam = lambdify(mu, loglike)
             y_plot = loglike_lam(x_plot)
             if normalize:
                 y_plot = (y_plot - min(y_plot))
                 y_plot = y_plot / np.sum(y_plot)
-            plot(x_plot, y_plot, c = 'dodgerblue', label = "Conservative weighted average")
+            plot(x_plot, y_plot, c = 'dodgerblue', label = "Conservative final likelihood")
         if wa_val:
             wa_av, wa_sig = wa(data, sigma)
-            print("Weighted average:", wa_av, "+-", wa_sig)
-            axvline(wa_av, c = "r", label = "Weighted average")
+            print("Standard weighted average:", wa_av, "+-", wa_sig)
+            axvline(wa_av, c = "r", label = "Standard weighted average")
             axvline(wa_av - wa_sig, c='r', ls = "--")
             axvline(wa_av + wa_sig, c='r', ls = "--")
         if wa_loglike:
             loglike = np.sum([log(1/(s_temp * sqrt(2 * pi)) * exp(-(x_temp - mu)**2 / (s_temp**2 * 2))) for x_temp, s_temp in zip(data, sigma)])
             loglike_lam = lambdify(mu, loglike)
             y_plot = loglike_lam(x_plot)
             if normalize:
                 y_plot = (y_plot - min(y_plot))
                 y_plot = y_plot / np.sum(y_plot)
-            plot(x_plot, y_plot, c = 'orange', label = "Weighted average")
+            plot(x_plot, y_plot, c = 'orange', label = "Standard likelihood")
         if jwa_val:
             jeff_av, jeff_sig = jwa(data, sigma)
             print("Jeffreys weighted average:", jeff_av, "+-", jeff_sig)
-            axvline(jeff_av, c = "g", label = "Jeffreys weighted average")
+            axvline(jeff_av, c = "g", label = "Jeffreys final likelihood")
             axvline(jeff_av - jeff_sig, c='g', ls = "--")
             axvline(jeff_av + jeff_sig, c='g', ls = "--")
         if jwa_loglike:
             loglike = np.sum([log(erf((x_temp - mu)/(sqrt(2)*s_temp)) / (x_temp-mu)) for x_temp, s_temp in zip(data, sigma)])
             loglike_lam = lambdify(mu, loglike)
             y_plot = loglike_lam(x_plot)
             if normalize:
@@ -110,13 +112,13 @@
                 y_plot = y_plot / np.sum(y_plot)
             plot(x_plot, y_plot, c = 'lime', label = "Jeffreys weighted average")
         if plot_data:
             y_min, y_max = gca().get_ylim()
             y_dist = y_max - y_min
             y_data = np.linspace(y_min + 0.2 * y_dist, y_min + 0.8 * y_dist, len(data))
             errorbar(data, y_data, xerr = sigma, ls = "", capsize = 3, marker = ".", label = "data", c = "k")
-        legend()
+        if legendon: legend()
         if normalize:
             ylabel("normalized log-likelihood")
         else:
             ylabel("log-likelihood")
         show()
```

