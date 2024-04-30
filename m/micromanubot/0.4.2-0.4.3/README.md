# Comparing `tmp/micromanubot-0.4.2.tar.gz` & `tmp/micromanubot-0.4.3.tar.gz`

## Comparing `micromanubot-0.4.2.tar` & `micromanubot-0.4.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 micromanubot-0.4.2/.python-version
--rw-r--r--   0        0        0   153295 2020-02-02 00:00:00.000000 micromanubot-0.4.2/main.pdf
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 micromanubot-0.4.2/requirements-dev.lock
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 micromanubot-0.4.2/requirements.lock
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 micromanubot-0.4.2/.github/workflows/python-app.yml
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 micromanubot-0.4.2/src/micromanubot/__init__.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 micromanubot-0.4.2/src/micromanubot/__main__.py
--rw-r--r--   0        0        0    11971 2020-02-02 00:00:00.000000 micromanubot-0.4.2/src/micromanubot/build.py
--rw-r--r--   0        0        0     5342 2020-02-02 00:00:00.000000 micromanubot-0.4.2/src/micromanubot/cite.py
--rw-r--r--   0        0        0     5674 2020-02-02 00:00:00.000000 micromanubot-0.4.2/src/micromanubot/cli.py
--rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 micromanubot-0.4.2/src/micromanubot/config.py
--rw-r--r--   0        0        0     8207 2020-02-02 00:00:00.000000 micromanubot-0.4.2/src/micromanubot/figures.py
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 micromanubot-0.4.2/src/micromanubot/install.py
--rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 micromanubot-0.4.2/src/micromanubot/new.py
--rw-r--r--   0        0        0     4066 2020-02-02 00:00:00.000000 micromanubot-0.4.2/src/micromanubot/pytinytex.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 micromanubot-0.4.2/src/micromanubot/template_data/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 micromanubot-0.4.2/src/micromanubot/template_data/assets/__init__.py
--rw-r--r--   0        0        0     7813 2020-02-02 00:00:00.000000 micromanubot-0.4.2/src/micromanubot/template_data/assets/arxiv.sty
--rw-r--r--   0        0        0    12397 2020-02-02 00:00:00.000000 micromanubot-0.4.2/src/micromanubot/template_data/assets/orcid.pdf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 micromanubot-0.4.2/src/micromanubot/template_data/build/__init__.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 micromanubot-0.4.2/src/micromanubot/template_data/build/main.tex
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 micromanubot-0.4.2/src/micromanubot/template_data/content/1.introduction.tex
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 micromanubot-0.4.2/src/micromanubot/template_data/content/2.results.tex
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 micromanubot-0.4.2/src/micromanubot/template_data/content/3.discussion.tex
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 micromanubot-0.4.2/src/micromanubot/template_data/content/4.methods.tex
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 micromanubot-0.4.2/src/micromanubot/template_data/content/__init__.py
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 micromanubot-0.4.2/src/micromanubot/template_data/content/abstract.tex
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 micromanubot-0.4.2/src/micromanubot/template_data/content/imports.tex
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 micromanubot-0.4.2/src/micromanubot/template_data/content/manual_references.bib
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 micromanubot-0.4.2/src/micromanubot/template_data/content/supplement.tex
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 micromanubot-0.4.2/tests/test_build.py
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 micromanubot-0.4.2/tests/test_cite.py
--rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 micromanubot-0.4.2/tests/test_cli.py
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 micromanubot-0.4.2/tests/test_figures.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 micromanubot-0.4.2/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 micromanubot-0.4.2/LICENSE
--rw-r--r--   0        0        0     5713 2020-02-02 00:00:00.000000 micromanubot-0.4.2/README.md
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 micromanubot-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     6714 2020-02-02 00:00:00.000000 micromanubot-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 micromanubot-0.4.3/.python-version
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 micromanubot-0.4.3/requirements-dev.lock
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 micromanubot-0.4.3/requirements.lock
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 micromanubot-0.4.3/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 micromanubot-0.4.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 micromanubot-0.4.3/src/micromanubot/__init__.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 micromanubot-0.4.3/src/micromanubot/__main__.py
+-rw-r--r--   0        0        0    11971 2020-02-02 00:00:00.000000 micromanubot-0.4.3/src/micromanubot/build.py
+-rw-r--r--   0        0        0     5342 2020-02-02 00:00:00.000000 micromanubot-0.4.3/src/micromanubot/cite.py
+-rw-r--r--   0        0        0     5674 2020-02-02 00:00:00.000000 micromanubot-0.4.3/src/micromanubot/cli.py
+-rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 micromanubot-0.4.3/src/micromanubot/config.py
+-rw-r--r--   0        0        0     8207 2020-02-02 00:00:00.000000 micromanubot-0.4.3/src/micromanubot/figures.py
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 micromanubot-0.4.3/src/micromanubot/install.py
+-rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 micromanubot-0.4.3/src/micromanubot/new.py
+-rw-r--r--   0        0        0     4066 2020-02-02 00:00:00.000000 micromanubot-0.4.3/src/micromanubot/pytinytex.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 micromanubot-0.4.3/src/micromanubot/template_data/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 micromanubot-0.4.3/src/micromanubot/template_data/assets/__init__.py
+-rw-r--r--   0        0        0     7669 2020-02-02 00:00:00.000000 micromanubot-0.4.3/src/micromanubot/template_data/assets/arxiv.sty
+-rw-r--r--   0        0        0    12397 2020-02-02 00:00:00.000000 micromanubot-0.4.3/src/micromanubot/template_data/assets/orcid.pdf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 micromanubot-0.4.3/src/micromanubot/template_data/build/__init__.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 micromanubot-0.4.3/src/micromanubot/template_data/build/main.tex
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 micromanubot-0.4.3/src/micromanubot/template_data/content/1.introduction.tex
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 micromanubot-0.4.3/src/micromanubot/template_data/content/2.results.tex
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 micromanubot-0.4.3/src/micromanubot/template_data/content/3.discussion.tex
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 micromanubot-0.4.3/src/micromanubot/template_data/content/4.methods.tex
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 micromanubot-0.4.3/src/micromanubot/template_data/content/__init__.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 micromanubot-0.4.3/src/micromanubot/template_data/content/abstract.tex
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 micromanubot-0.4.3/src/micromanubot/template_data/content/imports.tex
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 micromanubot-0.4.3/src/micromanubot/template_data/content/manual_references.bib
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 micromanubot-0.4.3/src/micromanubot/template_data/content/supplement.tex
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 micromanubot-0.4.3/tests/test_build.py
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 micromanubot-0.4.3/tests/test_cite.py
+-rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 micromanubot-0.4.3/tests/test_cli.py
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 micromanubot-0.4.3/tests/test_figures.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 micromanubot-0.4.3/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 micromanubot-0.4.3/LICENSE
+-rw-r--r--   0        0        0     5713 2020-02-02 00:00:00.000000 micromanubot-0.4.3/README.md
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 micromanubot-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     6778 2020-02-02 00:00:00.000000 micromanubot-0.4.3/PKG-INFO
```

### Comparing `micromanubot-0.4.2/requirements-dev.lock` & `micromanubot-0.4.3/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.2/requirements.lock` & `micromanubot-0.4.3/requirements.lock`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.2/.github/workflows/python-app.yml` & `micromanubot-0.4.3/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.2/src/micromanubot/build.py` & `micromanubot-0.4.3/src/micromanubot/build.py`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.2/src/micromanubot/cite.py` & `micromanubot-0.4.3/src/micromanubot/cite.py`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.2/src/micromanubot/cli.py` & `micromanubot-0.4.3/src/micromanubot/cli.py`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.2/src/micromanubot/config.py` & `micromanubot-0.4.3/src/micromanubot/config.py`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.2/src/micromanubot/figures.py` & `micromanubot-0.4.3/src/micromanubot/figures.py`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.2/src/micromanubot/install.py` & `micromanubot-0.4.3/src/micromanubot/install.py`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.2/src/micromanubot/new.py` & `micromanubot-0.4.3/src/micromanubot/new.py`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.2/src/micromanubot/pytinytex.py` & `micromanubot-0.4.3/src/micromanubot/pytinytex.py`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.2/src/micromanubot/template_data/assets/arxiv.sty` & `micromanubot-0.4.3/src/micromanubot/template_data/assets/arxiv.sty`

 * *Files 3% similar despite different names*

```diff
@@ -23,24 +23,21 @@
 }
 
 \widowpenalty=10000
 \clubpenalty=10000
 \flushbottom
 \sloppy
 
-\newcommand{\headeright}{A Preprint}
-\newcommand{\undertitle}{A Preprint}
 \newcommand{\shorttitle}{\@title}
 
 \usepackage{fancyhdr}
 \fancyhf{}
 \pagestyle{fancy}
 \renewcommand{\headrulewidth}{0.4pt}
 \fancyheadoffset{0pt}
-\rhead{\scshape \footnotesize \headeright}
 \chead{\shorttitle}
 \cfoot{\thepage}
 
 %Handling Keywords
 \def\keywordname{{\bfseries \emph{Keywords}}}%
 \def\keywords#1{\par\addvspace\medskipamount{\rightskip=0pt plus1cm
 \def\and{\ifhmode\unskip\nobreak\fi\ $\cdot$
@@ -219,15 +216,14 @@
     \hsize\textwidth
     \linewidth\hsize
     \vskip 0.1in
     \@toptitlebar
     \centering
     {\LARGE\sc \@title\par}
     \@bottomtitlebar
-    \textsc{\undertitle}\\
     \vskip 0.1in
     \def\And{%
       \end{tabular}\hfil\linebreak[0]\hfil%
       \begin{tabular}[t]{c}\bf\rule{\z@}{24\p@}\ignorespaces%
     }
     \def\AND{%
       \end{tabular}\hfil\linebreak[4]\hfil%
```

### Comparing `micromanubot-0.4.2/src/micromanubot/template_data/assets/orcid.pdf` & `micromanubot-0.4.3/src/micromanubot/template_data/assets/orcid.pdf`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.2/src/micromanubot/template_data/content/1.introduction.tex` & `micromanubot-0.4.3/src/micromanubot/template_data/content/1.introduction.tex`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.2/src/micromanubot/template_data/content/abstract.tex` & `micromanubot-0.4.3/src/micromanubot/template_data/content/abstract.tex`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.2/src/micromanubot/template_data/content/imports.tex` & `micromanubot-0.4.3/src/micromanubot/template_data/content/imports.tex`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.2/tests/test_build.py` & `micromanubot-0.4.3/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.2/tests/test_cite.py` & `micromanubot-0.4.3/tests/test_cite.py`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.2/tests/test_cli.py` & `micromanubot-0.4.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.2/tests/test_figures.py` & `micromanubot-0.4.3/tests/test_figures.py`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.2/LICENSE` & `micromanubot-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.2/README.md` & `micromanubot-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `micromanubot-0.4.2/pyproject.toml` & `micromanubot-0.4.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "micromanubot"
-version = "0.4.2"
+version = "0.4.3"
 description = "A build tool for academic manuscripts"
 authors = [
     { name = "zietzm", email = "michael.zietz@gmail.com" }
 ]
 dependencies = [
     "tomlkit>=0.12.4",
     "pydantic>=2.7.1",
@@ -26,14 +26,17 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3 :: Only",
 ]
 
+[project.urls]
+Repository = "https://github.com/zietzm/micromanubot"
+
 [project.scripts]
 "umb" = "micromanubot.cli:main"
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
```

### Comparing `micromanubot-0.4.2/PKG-INFO` & `micromanubot-0.4.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.3
 Name: micromanubot
-Version: 0.4.2
+Version: 0.4.3
 Summary: A build tool for academic manuscripts
+Project-URL: Repository, https://github.com/zietzm/micromanubot
 Author-email: zietzm <michael.zietz@gmail.com>
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
```

