# Comparing `tmp/casedi-0.0.1.tar.gz` & `tmp/casedi-0.0.2.tar.gz`

## Comparing `casedi-0.0.1.tar` & `casedi-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0   279780 2020-02-02 00:00:00.000000 casedi-0.0.1/casedi.png
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 casedi-0.0.1/casedi/__init__.py
--rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 casedi-0.0.1/casedi/enrichment.py
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 casedi-0.0.1/casedi/expression.py
--rw-r--r--   0        0        0     7290 2020-02-02 00:00:00.000000 casedi-0.0.1/casedi/survival.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 casedi-0.0.1/casedi/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 casedi-0.0.1/docs/conf.py
--rw-r--r--   0        0        0    96894 2020-02-02 00:00:00.000000 casedi-0.0.1/examples/examples.ipynb
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 casedi-0.0.1/tests/test_enrichment.py
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 casedi-0.0.1/tests/test_expression.py
--rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 casedi-0.0.1/tests/test_survival.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 casedi-0.0.1/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 casedi-0.0.1/LICENSE
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 casedi-0.0.1/README.md
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 casedi-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 casedi-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0   279780 2020-02-02 00:00:00.000000 casedi-0.0.2/casedi.png
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 casedi-0.0.2/casedi/__init__.py
+-rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 casedi-0.0.2/casedi/enrichment.py
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 casedi-0.0.2/casedi/expression.py
+-rw-r--r--   0        0        0     7285 2020-02-02 00:00:00.000000 casedi-0.0.2/casedi/survival.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 casedi-0.0.2/casedi/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 casedi-0.0.2/docs/conf.py
+-rw-r--r--   0        0        0    94589 2020-02-02 00:00:00.000000 casedi-0.0.2/examples/examples.ipynb
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 casedi-0.0.2/tests/test_enrichment.py
+-rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 casedi-0.0.2/tests/test_expression.py
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 casedi-0.0.2/tests/test_survival.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 casedi-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 casedi-0.0.2/LICENSE
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 casedi-0.0.2/README.md
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 casedi-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 casedi-0.0.2/PKG-INFO
```

### Comparing `casedi-0.0.1/casedi.png` & `casedi-0.0.2/casedi.png`

 * *Files identical despite different names*

### Comparing `casedi-0.0.1/casedi/enrichment.py` & `casedi-0.0.2/casedi/enrichment.py`

 * *Files identical despite different names*

### Comparing `casedi-0.0.1/casedi/expression.py` & `casedi-0.0.2/casedi/expression.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import scipy
 import pandas as pd
 
-from casedi_test.util import make_matrix
+from casedi.util import make_matrix
 
 def ase_compare_expression(gene, ase_table, expression_table, alternative='two-sided'):
     """Wrapper function for scipy.stats.mannwhitneyu to test expression
     difference between samples showing ASE and BAE using the Mann-Whitney
     U test
     
     Parameters
```

### Comparing `casedi-0.0.1/casedi/survival.py` & `casedi-0.0.2/casedi/survival.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from sksurv.nonparametric import kaplan_meier_estimator
 from sksurv.compare import compare_survival
 import pandas as pd
 import numpy as np
 import matplotlib.pyplot as plt
 
-from casedi_test.util import make_matrix
+from casedi.util import make_matrix
 
 def ase_compare_survival(gene, ase_table, survival_table,  return_stats=False,expression_table=None,plot=False,stratify_expression=None):
     """Wrapper function for sksurv kaplan_meier_estimator and 
     compare_survival that uses log-rank test to compares survival
     between samples showing ASE and BAE. Optionally, compare 
     survival between ASE + high expression and BAE + low expression
     or vice versa.
```

### Comparing `casedi-0.0.1/examples/examples.ipynb` & `casedi-0.0.2/examples/examples.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9677197802197802%*

 * *Differences: {"'cells'": "{0: {delete: ['id']}, 1: {'source': ['from casedi.survival import "*

 * *            "ase_compare_survival\\n', 'from casedi.expression import ase_compare_expression\\n', "*

 * *            "'from casedi.enrichment import ase_compare_groups'], delete: ['id']}, 2: {delete: "*

 * *            "['id']}, 3: {delete: ['id']}, 4: {delete: ['id']}, 5: {delete: ['id']}, 6: {delete: "*

 * *            "['id']}, 7: {delete: ['id']}, 8: {delete: ['id']}, 9: {delete: ['id']}, 10: {delete: "*

 * *            "['id']}, 11: {delete:  […]*

```diff
@@ -1,88 +1,55 @@
 {
     "cells": [
         {
             "cell_type": "code",
             "execution_count": 1,
-            "id": "d9873fbe-4120-4551-b088-ce4af5bcd45d",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import pandas as pd\n",
                 "import numpy as np\n",
                 "import matplotlib.pyplot as plt"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
-            "id": "76f5da9a-e716-458c-903f-618827265e21",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from casedi_test.survival import ase_compare_survival\n",
-                "from casedi_test.expression import ase_compare_expression\n",
-                "from casedi_test.enrichment import ase_compare_groups"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 93,
-            "id": "1e0dd0df-97d1-46de-9bcc-f2d6b68afdae",
-            "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "Defaulting to user installation because normal site-packages is not writeable\n",
-                        "Looking in indexes: https://test.pypi.org/simple/\n",
-                        "Collecting casedi-test\n",
-                        "  Using cached https://test-files.pythonhosted.org/packages/f1/68/210a98a73428c1b8bf57262af3f05a0d1d3b6695dbea310e2a1457dda1f0/casedi_test-0.0.8-py3-none-any.whl (7.8 kB)\n",
-                        "Installing collected packages: casedi-test\n",
-                        "  Attempting uninstall: casedi-test\n",
-                        "    Found existing installation: casedi-test 0.0.7\n",
-                        "    Uninstalling casedi-test-0.0.7:\n",
-                        "      Successfully uninstalled casedi-test-0.0.7\n",
-                        "Successfully installed casedi-test-0.0.8\n"
-                    ]
-                }
-            ],
-            "source": [
-                "!python3 -m pip install --upgrade --force-reinstall --index-url https://test.pypi.org/simple/ --no-deps casedi-test"
+                "from casedi.survival import ase_compare_survival\n",
+                "from casedi.expression import ase_compare_expression\n",
+                "from casedi.enrichment import ase_compare_groups"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "4498138b-3906-42b6-b465-a1028917aee7",
             "metadata": {},
             "source": [
                 "# Examples using CASEDI on toy data"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "620b5f74-9f97-4e75-b54b-336891ab82fe",
             "metadata": {},
             "source": [
                 "## Identifying genes where samples showing ASE show significant outlier expression compared to samples showing BAE"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "1931db45-e511-406a-9def-e8f85fc6890e",
             "metadata": {},
             "source": [
                 "Generating an example table with ASE data for gene A for 20 tumor samples, where half of samples show ASE and half show BAE"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
-            "id": "3f47ccc1-6c8b-4aaf-84d8-4d9aaa1c0d86",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -267,24 +234,22 @@
                 "                         'sampleID': np.arange(0,20,1) \n",
                 "                         })\n",
                 "ase_table"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "1bd89b89-ab10-45db-ac12-a696c7d37a1b",
             "metadata": {},
             "source": [
                 "Generate gene expression table of samples x genes with normalized expression values. Index must match sampleID."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
-            "id": "5e07e2de-5e64-4c95-a058-d08e86540a96",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -425,24 +390,22 @@
                 "expr = np.concatenate([np.random.randint(0,10,10),np.random.randint(5,10,10)])\n",
                 "expression_table = pd.DataFrame({'A': expr})\n",
                 "expression_table"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "34a95cf8-52ba-4894-bcbb-b486f96bcb5e",
             "metadata": {},
             "source": [
                 "Test if samples showing ASE for gene A have different overall expression than samples showing BAE"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
-            "id": "c80b0fe0-3bb9-434b-a233-f692f7f72f8f",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "MannwhitneyuResult(statistic=81.0, pvalue=0.01798403235775862)"
                         ]
@@ -457,32 +420,29 @@
                 "                       ase_table=ase_table,\n",
                 "                       expression_table=expression_table,\n",
                 "                       alternative='two-sided')"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "aac4b104-6f43-4012-bd02-8a8573224def",
             "metadata": {},
             "source": [
                 "## Survival difference between samples showing ASE and BAE"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "68e3da4d-781b-4927-8bdd-c284209a7e1e",
             "metadata": {},
             "source": [
                 "Generate a table with survival times and statuses for each sample. Index must match sampleID. You can use overall survival, progression-free survival, etc."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 6,
-            "id": "cbe43234-7d78-40c9-8eb2-0ef0fa80bf55",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -648,24 +608,22 @@
                 "                               'survival_status': events # 0 for no event, 1 for event\n",
                 "                              })\n",
                 "survival_table"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "5b991eed-9100-4cc8-9b89-345ff66004d1",
             "metadata": {},
             "source": [
                 "Perform log-rank test to test for difference in survival between samples showing ASE and BAE for gene A"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 7,
-            "id": "6439ee1b-4d6e-4285-87ce-693caa6cc322",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "(6.063519058408218, 0.013800242446541905)"
                         ]
@@ -680,24 +638,22 @@
                 "                     ase_table=ase_table,\n",
                 "                     survival_table=survival_table\n",
                 "                     )"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "491cc0fd-fe93-4434-974d-c6b003a257a0",
             "metadata": {},
             "source": [
                 "Plot Kaplan-Meier"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 8,
-            "id": "3e470739-66cb-4e5f-9ab8-26182e268cb0",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "(0.0, 20.0)"
                         ]
@@ -726,24 +682,22 @@
                 "                     plot=True\n",
                 "                     )\n",
                 "plt.xlim(0,20)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "379eda72-ce87-4ffb-b2ae-c33e4b83ecb7",
             "metadata": {},
             "source": [
                 "Further stratify by ASE and high expression"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 9,
-            "id": "4e809ae9-d829-4cd6-975c-210b3570ad29",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "(5.992110651197611, 0.014369998202495463)"
                         ]
@@ -761,15 +715,14 @@
                 "                     expression_table=expression_table,\n",
                 "                     )"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 10,
-            "id": "7435b467-c652-4c4e-964e-e90131489954",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "<matplotlib.legend.Legend at 0x7f1943c709d0>"
                         ]
@@ -800,34 +753,31 @@
                 "                     plot=True\n",
                 "                     )\n",
                 "plt.legend(bbox_to_anchor=(1,1))"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "852e1db5-8517-40a7-beb6-edd80f9a58de",
             "metadata": {},
             "source": [
                 "## Enrichment analysis between two subgroups"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "096d69a9-be58-408c-b784-4ed324ab38d6",
             "metadata": {},
             "source": [
                 "Used to identify ASE associated with a particular mutation, molecular subtype of tumor, tumor stage, etc \n",
                 "\n",
                 "Example: Tumors 0-9 have a gene fusion in gene A and tumors 10-19 do not. Group 1 will be fusion positive tumors, group 2 will be fusion negative tumors"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 11,
-            "id": "69bb6c53-f7c6-4f92-bbfe-1b2d5580ba47",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -1155,15 +1105,14 @@
                 "ase_table = pd.concat([ase_table, gene_B],ignore_index=True)\n",
                 "ase_table"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 12,
-            "id": "be100093-7e43-4ae7-a050-3c17874618fb",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Group1 genes showing ASE:  1\n",
@@ -1256,15 +1205,14 @@
                 "                   testable_fraction=0.1\n",
                 "                   )"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "c1d97336-c690-4988-95d5-237ffb35fd78",
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
@@ -1278,13 +1226,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.5"
+            "version": "3.7.9"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `casedi-0.0.1/tests/test_enrichment.py` & `casedi-0.0.2/tests/test_enrichment.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import unittest
 import pandas as pd
 import numpy as np
 
-from casedi_test.enrichment import ase_compare_groups
+from casedi.enrichment import ase_compare_groups
 
 example_ase_table = pd.DataFrame({'gene': np.repeat('A',20),
                                  'ase': np.concatenate([np.repeat(0,10),np.repeat(1,10)]),
                                  'sampleID': np.arange(0,20,1) 
                                  })
 
 group1 = np.array([])
```

### Comparing `casedi-0.0.1/tests/test_expression.py` & `casedi-0.0.2/tests/test_expression.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import unittest
 import pandas as pd
 import numpy as np
 
-from casedi_test.expression import ase_compare_expression
+from casedi.expression import ase_compare_expression
 
 example_ase_table = pd.DataFrame({'gene': np.repeat('A',20),
                                  'ase': np.concatenate([np.repeat(0,10),np.repeat(1,10)]),
                                  'sampleID': np.arange(0,20,1) 
                                  })
 example_ase_table2 = pd.DataFrame({'gene': np.repeat('A',20),
                                  'ase': np.repeat(0,20), # no ASE samples
```

### Comparing `casedi-0.0.1/tests/test_survival.py` & `casedi-0.0.2/tests/test_survival.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import unittest
 import pandas as pd
 import numpy as np
 
-from casedi_test.survival import ase_compare_survival
+from casedi.survival import ase_compare_survival
 
 example_ase_table = pd.DataFrame({'gene': np.repeat('A',20),
                                  'ase': np.concatenate([np.repeat(0,10),np.repeat(1,10)]),
                                  'sampleID': np.arange(1,21,1) # mismatching sampleID
                                  })
 example_survival_table = pd.DataFrame({'survival_time': np.concatenate([np.repeat(10,10),np.repeat(2,10)]),
                                        'survival_status': np.concatenate([np.repeat(1,10),np.repeat(0,10)]),
```

### Comparing `casedi-0.0.1/.gitignore` & `casedi-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `casedi-0.0.1/LICENSE` & `casedi-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `casedi-0.0.1/README.md` & `casedi-0.0.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 CASEDI is an analysis framework that uses tumor allele-specific expression (ASE) data to prioritize cancer driver genes. CASEDI includes functions to identify genes enriched for ASE between datasets, conduct ASE-stratified survival analysis, and identify genes showing ASE outlier expression.
 
 ## Installation
 
 The latest stable release can be installed from PyPI:
 
 ```python
-pip install --index-url https://test.pypi.org/simple/ --no-deps casedi-test
+pip install casedi
 ```
 You may instead want to use the development version from Github:
 
 ```python
 pip install git+https://https://github.com/maggietsui/casedi.git
 ```
```

### Comparing `casedi-0.0.1/pyproject.toml` & `casedi-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "casedi"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Maggie Tsui", email="margaret.tsui@ucsf.edu" },
 ]
 
 description = "Cancer ASE driver identification (CASEDI)"
 readme = "README.md"
 dependencies = [
```

### Comparing `casedi-0.0.1/PKG-INFO` & `casedi-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: casedi
-Version: 0.0.1
+Version: 0.0.2
 Summary: Cancer ASE driver identification (CASEDI)
 Project-URL: Homepage, https://github.com/maggietsui/CASEDI
 Project-URL: Issues, https://github.com/maggietsui/CASEDI/issues
 Author-email: Maggie Tsui <margaret.tsui@ucsf.edu>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -25,15 +25,15 @@
 CASEDI is an analysis framework that uses tumor allele-specific expression (ASE) data to prioritize cancer driver genes. CASEDI includes functions to identify genes enriched for ASE between datasets, conduct ASE-stratified survival analysis, and identify genes showing ASE outlier expression.
 
 ## Installation
 
 The latest stable release can be installed from PyPI:
 
 ```python
-pip install --index-url https://test.pypi.org/simple/ --no-deps casedi-test
+pip install casedi
 ```
 You may instead want to use the development version from Github:
 
 ```python
 pip install git+https://https://github.com/maggietsui/casedi.git
 ```
```

