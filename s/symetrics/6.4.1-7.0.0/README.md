# Comparing `tmp/symetrics-6.4.1.tar.gz` & `tmp/symetrics-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symetrics-6.4.1.tar", last modified: Fri Apr 26 00:42:05 2024, max compression
+gzip compressed data, was "symetrics-7.0.0.tar", last modified: Tue Apr 30 06:08:34 2024, max compression
```

## Comparing `symetrics-6.4.1.tar` & `symetrics-7.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 00:42:05.135994 symetrics-6.4.1/
--rw-rw-rw-   0        0        0     1151 2024-04-26 00:42:05.135994 symetrics-6.4.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-26 00:42:05.135994 symetrics-6.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1640 2024-04-26 00:41:49.000000 symetrics-6.4.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-26 00:42:05.090962 symetrics-6.4.1/symetrics/
--rw-rw-rw-   0        0        0      101 2023-12-09 13:09:42.000000 symetrics-6.4.1/symetrics/__init__.py
--rw-rw-rw-   0        0        0      519 2023-12-09 13:09:33.000000 symetrics-6.4.1/symetrics/dbcontext.py
-drwxrwxrwx   0        0        0        0 2024-04-26 00:42:05.133987 symetrics-6.4.1/symetrics/src/
--rw-rw-rw-   0        0        0       25 2023-10-25 09:08:07.000000 symetrics-6.4.1/symetrics/src/__init__.py
--rw-rw-rw-   0        0        0      967 2024-01-31 08:23:38.000000 symetrics-6.4.1/symetrics/src/datastruct.py
--rw-rw-rw-   0        0        0    20747 2024-04-26 00:35:20.000000 symetrics-6.4.1/symetrics/symetrics_api.py
-drwxrwxrwx   0        0        0        0 2024-04-26 00:42:05.131347 symetrics-6.4.1/symetrics.egg-info/
--rw-rw-rw-   0        0        0     1151 2024-04-26 00:42:04.000000 symetrics-6.4.1/symetrics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2024-04-26 00:42:04.000000 symetrics-6.4.1/symetrics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 00:42:04.000000 symetrics-6.4.1/symetrics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-04-26 00:42:04.000000 symetrics-6.4.1/symetrics.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-26 00:42:04.000000 symetrics-6.4.1/symetrics.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-30 06:08:34.854946 symetrics-7.0.0/
+-rw-rw-rw-   0        0        0     1151 2024-04-30 06:08:34.853939 symetrics-7.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-30 06:08:34.854946 symetrics-7.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1640 2024-04-29 10:26:52.000000 symetrics-7.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 06:08:34.796835 symetrics-7.0.0/symetrics/
+-rw-rw-rw-   0        0        0      101 2023-12-09 13:09:42.000000 symetrics-7.0.0/symetrics/__init__.py
+-rw-rw-rw-   0        0        0      519 2023-12-09 13:09:33.000000 symetrics-7.0.0/symetrics/dbcontext.py
+drwxrwxrwx   0        0        0        0 2024-04-30 06:08:34.852433 symetrics-7.0.0/symetrics/src/
+-rw-rw-rw-   0        0        0       25 2023-10-25 09:08:07.000000 symetrics-7.0.0/symetrics/src/__init__.py
+-rw-rw-rw-   0        0        0      967 2024-01-31 08:23:38.000000 symetrics-7.0.0/symetrics/src/datastruct.py
+-rw-rw-rw-   0        0        0    20402 2024-04-30 06:05:59.000000 symetrics-7.0.0/symetrics/symetrics_api.py
+drwxrwxrwx   0        0        0        0 2024-04-30 06:08:34.850448 symetrics-7.0.0/symetrics.egg-info/
+-rw-rw-rw-   0        0        0     1151 2024-04-30 06:08:34.000000 symetrics-7.0.0/symetrics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2024-04-30 06:08:34.000000 symetrics-7.0.0/symetrics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 06:08:34.000000 symetrics-7.0.0/symetrics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-04-30 06:08:34.000000 symetrics-7.0.0/symetrics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-30 06:08:34.000000 symetrics-7.0.0/symetrics.egg-info/top_level.txt
```

### Comparing `symetrics-6.4.1/PKG-INFO` & `symetrics-7.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symetrics
-Version: 6.4.1
+Version: 7.0.0
 Summary: Symetrics API
 Home-page: https://lbundalian.github.io/symetrics/
 Author: Linnaeus Bundalian
 Author-email: linnaeusbundalian@gmail.com
 Keywords: python,synonymous variants
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
```

### Comparing `symetrics-6.4.1/setup.py` & `symetrics-7.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '6.4.1' 
+VERSION = '7.0.0' 
 DESCRIPTION = 'Symetrics API'
 LONG_DESCRIPTION = '''A package to access SYMETRICS database. 
 SYMETRICS database is a consolidation of metrics for synonymous variants which were derived from a number of computational tools each of which contributing to 
 attribute specific metrics such as SYNVEP for general functional constraints, SpliceAI for splicing effect, SILVA for obtaining GERP++ (phylogenetic related constraints)
 CpG/CpG_Exon, dRSCU/RSCU for codon usage and SURF for rna stability. The package also includes a result of the analysis of the influence of each variants exceeding set threshold
 per metrics defined constituting to a score assigned to a gene'''
 REQUIRED_PACKAGES = [
```

### Comparing `symetrics-6.4.1/symetrics/dbcontext.py` & `symetrics-7.0.0/symetrics/dbcontext.py`

 * *Files identical despite different names*

### Comparing `symetrics-6.4.1/symetrics/src/datastruct.py` & `symetrics-7.0.0/symetrics/src/datastruct.py`

 * *Files identical despite different names*

### Comparing `symetrics-6.4.1/symetrics/symetrics_api.py` & `symetrics-7.0.0/symetrics/symetrics_api.py`

 * *Files 15% similar despite different names*

```diff
@@ -49,23 +49,25 @@
 
 class Symetrics(ISymetrics):
 
     _db = None
     _conn = None
     _collection = None
     _gnomad_db = None
+    _constraints = None
     _collection = None
     
     def __init__(self, cfg) -> None:
 
         with open(cfg, 'r') as file:
             config = json.load(file)
     
-        self._db = DbContext(config['collection']['symetrics']['database'])
-        self._gnomad_db = DbContext(config['collection']['gnomad']['database'])
+        self._db = DbContext(config['collection']['symetrics'])
+        self._gnomad_db = DbContext(config['collection']['gnomad'])
+        self._constraints = DbContext(config['collection']['constraints'])
         self._collection = config
 
     
     def get_silva_score(self,variant: VariantObject):
 
         """
         
@@ -86,20 +88,24 @@
         
         """
 
         silva_scores = None
         try:
             # dont forget silva is hg19
             with self._db as dbhandler:
+                
                 silva_cursor = dbhandler._conn.cursor()
-                #silva_query = f'SELECT "#chrom" AS CHR,pos AS POS,ref AS REF,alt AS ALT,gene AS GENE,"#RSCU" AS RSCU,dRSCU,"#GERP++" AS GERP,"#CpG?" AS CPG,CpG_exon AS CPGX FROM SILVA WHERE "#chrom" = {variant._chr} AND pos = {variant._pos} AND ref = "{variant._ref}" AND alt = "{variant._alt}"'
-                #silva_query = f'SELECT * FROM SILVA WHERE "#chrom" = {variant._chr} AND pos = {variant._pos} AND ref = "{variant._ref}" AND alt = "{variant._alt}"'
-                silva_query = f'SELECT * FROM SILVA_SCORE WHERE CHROM = {variant._chr} AND POS = {variant._pos} AND REF = "{variant._ref}" AND ALT = "{variant._alt}"'
                 
-                silva_cursor.execute(silva_query)
+                silva_query = """
+                        SELECT * FROM SILVA_SCORE 
+                        WHERE CHROM = ? AND POS = ? AND REF = ? AND ALT = ?
+                        """
+                params = (variant._chr, variant._pos, variant._ref, variant._alt)
+
+                silva_cursor.execute(silva_query,params)
                 silva_rows = silva_cursor.fetchall()
                 silva_scores = silva_rows[0]
                 silva_scores = {
                     "CHR": silva_scores[0],
                     "POS": silva_scores[1],
                     "REF": silva_scores[3],
                     "ALT": silva_scores[4],
@@ -141,17 +147,26 @@
 
         """
 
         surf_scores = None
         try:
             # SURF is hg38
             with self._db as dbhandler:
+                
                 surf_cursor = dbhandler._conn.cursor()
-                surf_query = f'SELECT CHR,POS,REF,ALT,GENE,SURF FROM SURF WHERE CHR = {variant._chr} AND POS = {variant._pos} AND REF = "{variant._ref}" AND ALT = "{variant._alt}"'
-                surf_cursor.execute(surf_query)
+                
+                surf_query = """
+                    SELECT CHR, POS, REF, ALT, GENE, SURF
+                    FROM SURF
+                    WHERE CHR = ? AND POS = ? AND REF = ? AND ALT = ?
+                    """
+                
+                params = (variant._chr, variant._pos, variant._ref, variant._alt)
+
+                surf_cursor.execute(surf_query,params)
                 surf_rows = surf_cursor.fetchall()
                 surf_scores = surf_rows[0]
                 surf_scores = {
                     "CHR": surf_scores[0],
                     "POS": surf_scores[1],
                     "REF": surf_scores[2],
                     "ALT": surf_scores[3],
@@ -191,18 +206,29 @@
 
         try:
             # synvep is hg38 (pos_GRCh38) abd hg19 (pos)
             with self._db as dbhandler:
                 synvep_cursor = dbhandler._conn.cursor()
                 synvep_query = ''
                 if variant._genome.name == GenomeReference.hg38.name:
-                    synvep_query = f'SELECT chr as CHR,pos_GRCh38 as POS,ref as REF,alt as ALT, HGNC_gene_symbol as GENE,synVep as SYNVEP FROM SYNVEP WHERE chr = {variant._chr} AND pos_GRCh38 = {variant._pos} AND ref = "{variant._ref}" AND alt = "{variant._alt}"'
-                elif variant._genome.name == GenomeReference.hg19.name:
-                    synvep_query = f'SELECT chr as CHR,pos as POS,ref as REF,alt as ALT, HGNC_gene_symbol as GENE,synVep as SYNVEP FROM SYNVEP WHERE chr = {variant._chr} AND pos_GRCh38 = {variant._pos} AND ref = "{variant._ref}" AND alt = "{variant._alt}"'
-                synvep_cursor.execute(synvep_query)
+                    synvep_query = """
+                        SELECT chr as CHR, pos_GRCh38 as POS, ref as REF, alt as ALT, HGNC_gene_symbol as GENE, synVep as SYNVEP
+                        FROM SYNVEP
+                        WHERE chr = ? AND pos_GRCh38 = ? AND ref = ? AND alt = ?
+                        """    
+                    
+                elif variant._genome.name == GenomeReference.hg19.name:                    
+                    synvep_query = """
+                        SELECT chr as CHR, pos_GRCh38 as POS, ref as REF, alt as ALT, HGNC_gene_symbol as GENE, synVep as SYNVEP
+                        FROM SYNVEP
+                        WHERE chr = ? AND pos = ? AND ref = ? AND alt = ?
+                        """
+                params = (variant._chr, variant._pos, variant._ref, variant._alt)
+                
+                synvep_cursor.execute(synvep_query,params)
                 synvep_rows = synvep_cursor.fetchall()
                 synvep_scores = synvep_rows[0]
                 synvep_scores = {
                     "CHR": synvep_scores[0],
                     "POS": synvep_scores[1],
                     "REF": synvep_scores[2],
                     "ALT": synvep_scores[3],
@@ -238,16 +264,25 @@
         """
                         
         spliceai_score = None
         try:
             # synvep is hg38 (pos_GRCh38) abd hg19 (pos)
             with self._db as dbhandler:
                 spliceai_cursor = dbhandler._conn.cursor()
-                spliceai_query = f'SELECT chr as CHR,pos as POS,ref as REF,alt as ALT, INFO FROM SPLICEAI WHERE chr = {variant._chr} AND pos = {variant._pos} AND ref = "{variant._ref}" AND alt = "{variant._alt}"'
-                spliceai_cursor.execute(spliceai_query)
+                                
+                spliceai_query = """
+                SELECT chr as CHR, pos as POS, ref as REF, alt as ALT, INFO
+                FROM SPLICEAI
+                WHERE chr = ? AND pos = ? AND ref = ? AND alt = ?
+                """
+
+                # Prepare the parameters tuple
+                params = (variant._chr, variant._pos, variant._ref, variant._alt)
+
+                spliceai_cursor.execute(spliceai_query,params)
                 spliceai_rows = spliceai_cursor.fetchall()
                 spliceai_score = pd.DataFrame(spliceai_rows)
                 spliceai_score.columns = ['CHR','POS','REF','ALT','INFO']
                 if not spliceai_score.empty:
                     vcf_header = "ALLELE|SYMBOL|DS_AG|DS_AL|DS_DG|DS_DL|DP_AG|DP_AL|DP_DG|DP_DL"
                     vcf_header = vcf_header.split('|')
                     spliceai_score[vcf_header] = spliceai_score['INFO'].str.split('|', expand=True)
@@ -287,46 +322,43 @@
             >>> symetrics = Symetrics('symetrics.db')
             >>> score = symetrics.get_prop_score(group = 'SYNVEP',gene = 'A1BG')
         
         """
 
         scores = None
         scaler = StandardScaler()
-        synvep_constraints = self._collection['collection']['symetrics']['constraints']
-
+        
 
         if group in MetricsGroup.__members__:
-            match group:
-                case MetricsGroup.SYNVEP.name:
-                    scores = pd.read_csv(synvep_constraints[group])
-                    scaled_scores = scaler.fit_transform(scores[['z']])
-                    scores['scaled_z'] = scaled_scores
-                    scores = scores[scores.GENES ==  gene]
-                    scores = scores[['GENES','pval','fdr','z','scaled_z']]
-                    scores.columns = ['GENE','PVAL','FDR','SYMETRIC_SCORE','NORM_SYMETRIC_SCORE']
-                    scores['GROUP'] = group
-                    scores = scores.to_dict(orient='records')
-                case MetricsGroup.SURF.name:
-                    scores = pd.read_csv(synvep_constraints[group])
-                    scaled_scores = scaler.fit_transform(scores[['z']])
-                    scores['scaled_z'] = scaled_scores
-                    scores = scores[scores.GENES ==  gene]
-                    scores = scores[['GENES','pval','fdr','z','scaled_z']]
-                    scores.columns = ['GENE','PVAL','FDR','SYMETRIC_SCORE','NORM_SYMETRIC_SCORE']
-                    scores['GROUP'] = group
-                    scores = scores.to_dict(orient='records')
-                case _:
-                    scores = pd.read_csv(synvep_constraints[group])
-                    scaled_scores = scaler.fit_transform(scores[['z']])
-                    scores['scaled_z'] = scaled_scores
-                    scores = scores[scores.GENE ==  gene]
-                    scores = scores[['GENE','pval','fdr','z','scaled_z']]
-                    scores.columns = ['GENE','PVAL','FDR','SYMETRIC_SCORE','NORM_SYMETRIC_SCORE']
-                    scores['GROUP'] = group
-                    scores = scores.to_dict(orient='records')
+            scores = None
+            try:
+                with self._constraints as dbhandler:
+                            
+                    cursor = dbhandler._conn.cursor()
+                            
+                    query = f"SELECT GENES as GENE, pval as PVAL, fdr as FDR, z as SYMETRIC_SCORE, norm_z as NORM_SYMETRIC_SCORE FROM GNOMADv4{group} WHERE GENES = ?"
+                            
+                    params = (gene,)
+
+                    cursor.execute(query,params)
+                    rows = cursor.fetchall()
+                    scores = rows[0]
+                    scores = {
+                                "GENE": scores[0],
+                                "PVAL": scores[1],
+                                "FDR": scores[2],
+                                "SYMERIC_SCORE": scores[3],
+                                "NORM_SYMERIC_SCORE": scores[4]
+                    }
+
+            except Error as e:
+                    logging.error(e)
+                    logging.error(f"Connection to {self._constraints} failed")
+                
+                    
         else:
             logging.error(f'Group: {group} is not valid')       
     
         return scores    
     
     def get_gnomad_data(self, variant: VariantObject):
```

### Comparing `symetrics-6.4.1/symetrics.egg-info/PKG-INFO` & `symetrics-7.0.0/symetrics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symetrics
-Version: 6.4.1
+Version: 7.0.0
 Summary: Symetrics API
 Home-page: https://lbundalian.github.io/symetrics/
 Author: Linnaeus Bundalian
 Author-email: linnaeusbundalian@gmail.com
 Keywords: python,synonymous variants
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
```

