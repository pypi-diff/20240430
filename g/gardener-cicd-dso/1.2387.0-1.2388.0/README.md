# Comparing `tmp/gardener_cicd_dso-1.2387.0.tar.gz` & `tmp/gardener_cicd_dso-1.2388.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gardener_cicd_dso-1.2387.0.tar", last modified: Fri Apr 26 17:05:11 2024, max compression
+gzip compressed data, was "gardener_cicd_dso-1.2388.0.tar", last modified: Tue Apr 30 05:06:03 2024, max compression
```

## Comparing `gardener_cicd_dso-1.2387.0.tar` & `gardener_cicd_dso-1.2388.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 17:05:11.204507 gardener_cicd_dso-1.2387.0/
--rw-r--r--   0 root         (0) root         (0)    11357 2024-04-26 17:04:22.000000 gardener_cicd_dso-1.2387.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      211 2024-04-26 17:05:11.204507 gardener_cicd_dso-1.2387.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2093 2024-04-26 17:04:22.000000 gardener_cicd_dso-1.2387.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 17:05:11.200507 gardener_cicd_dso-1.2387.0/checkmarx/
--rw-r--r--   0 root         (0) root         (0)      132 2024-04-26 17:04:22.000000 gardener_cicd_dso-1.2387.0/checkmarx/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7945 2024-04-26 17:04:22.000000 gardener_cicd_dso-1.2387.0/checkmarx/client.py
--rw-r--r--   0 root         (0) root         (0)     3746 2024-04-26 17:04:22.000000 gardener_cicd_dso-1.2387.0/checkmarx/model.py
--rw-r--r--   0 root         (0) root         (0)     7033 2024-04-26 17:04:22.000000 gardener_cicd_dso-1.2387.0/checkmarx/project.py
--rw-r--r--   0 root         (0) root         (0)     5790 2024-04-26 17:04:22.000000 gardener_cicd_dso-1.2387.0/checkmarx/tablefmt.py
--rw-r--r--   0 root         (0) root         (0)    19358 2024-04-26 17:04:22.000000 gardener_cicd_dso-1.2387.0/checkmarx/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 17:05:11.200507 gardener_cicd_dso-1.2387.0/clamav/
--rw-r--r--   0 root         (0) root         (0)      132 2024-04-26 17:04:22.000000 gardener_cicd_dso-1.2387.0/clamav/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4680 2024-04-26 17:04:22.000000 gardener_cicd_dso-1.2387.0/clamav/client.py
--rw-r--r--   0 root         (0) root         (0)     8427 2024-04-26 17:04:22.000000 gardener_cicd_dso-1.2387.0/clamav/cnudie.py
--rw-r--r--   0 root         (0) root         (0)     2252 2024-04-26 17:04:22.000000 gardener_cicd_dso-1.2387.0/clamav/model.py
--rw-r--r--   0 root         (0) root         (0)     1902 2024-04-26 17:04:22.000000 gardener_cicd_dso-1.2387.0/clamav/report.py
--rw-r--r--   0 root         (0) root         (0)     1083 2024-04-26 17:04:22.000000 gardener_cicd_dso-1.2387.0/clamav/routes.py
--rw-r--r--   0 root         (0) root         (0)     7469 2024-04-26 17:04:22.000000 gardener_cicd_dso-1.2387.0/clamav/scan.py
--rw-r--r--   0 root         (0) root         (0)     5564 2024-04-26 17:04:22.000000 gardener_cicd_dso-1.2387.0/clamav/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 17:05:11.204507 gardener_cicd_dso-1.2387.0/gardener_cicd_dso.egg-info/
--rw-r--r--   0 root         (0) root         (0)      211 2024-04-26 17:05:11.000000 gardener_cicd_dso-1.2387.0/gardener_cicd_dso.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      670 2024-04-26 17:05:11.000000 gardener_cicd_dso-1.2387.0/gardener_cicd_dso.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 17:05:11.000000 gardener_cicd_dso-1.2387.0/gardener_cicd_dso.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       37 2024-04-26 17:05:11.000000 gardener_cicd_dso-1.2387.0/gardener_cicd_dso.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2024-04-26 17:05:11.000000 gardener_cicd_dso-1.2387.0/gardener_cicd_dso.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 17:05:11.204507 gardener_cicd_dso-1.2387.0/protecode/
--rw-r--r--   0 root         (0) root         (0)      132 2024-04-26 17:04:22.000000 gardener_cicd_dso-1.2387.0/protecode/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7653 2024-04-26 17:04:22.000000 gardener_cicd_dso-1.2387.0/protecode/assessments.py
--rw-r--r--   0 root         (0) root         (0)    17319 2024-04-26 17:04:22.000000 gardener_cicd_dso-1.2387.0/protecode/client.py
--rw-r--r--   0 root         (0) root         (0)    10709 2024-04-26 17:04:22.000000 gardener_cicd_dso-1.2387.0/protecode/model.py
--rw-r--r--   0 root         (0) root         (0)     3636 2024-04-26 17:04:22.000000 gardener_cicd_dso-1.2387.0/protecode/rescore.py
--rw-r--r--   0 root         (0) root         (0)    29221 2024-04-26 17:04:22.000000 gardener_cicd_dso-1.2387.0/protecode/scanning.py
--rw-r--r--   0 root         (0) root         (0)     9176 2024-04-26 17:04:22.000000 gardener_cicd_dso-1.2387.0/protecode/util.py
--rw-r--r--   0 root         (0) root         (0)      359 2024-04-26 17:04:22.000000 gardener_cicd_dso-1.2387.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      174 2024-04-26 17:05:11.204507 gardener_cicd_dso-1.2387.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      673 2024-04-26 17:04:22.000000 gardener_cicd_dso-1.2387.0/setup.dso.py
--rw-r--r--   0 root         (0) root         (0)     2174 2024-04-26 17:04:22.000000 gardener_cicd_dso-1.2387.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 05:06:03.121183 gardener_cicd_dso-1.2388.0/
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-04-30 04:58:56.000000 gardener_cicd_dso-1.2388.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      211 2024-04-30 05:06:03.121183 gardener_cicd_dso-1.2388.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2093 2024-04-30 04:58:56.000000 gardener_cicd_dso-1.2388.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 05:06:03.117184 gardener_cicd_dso-1.2388.0/checkmarx/
+-rw-r--r--   0 root         (0) root         (0)      132 2024-04-30 04:58:56.000000 gardener_cicd_dso-1.2388.0/checkmarx/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7945 2024-04-30 04:58:56.000000 gardener_cicd_dso-1.2388.0/checkmarx/client.py
+-rw-r--r--   0 root         (0) root         (0)     3746 2024-04-30 04:58:56.000000 gardener_cicd_dso-1.2388.0/checkmarx/model.py
+-rw-r--r--   0 root         (0) root         (0)     7033 2024-04-30 04:58:56.000000 gardener_cicd_dso-1.2388.0/checkmarx/project.py
+-rw-r--r--   0 root         (0) root         (0)     5790 2024-04-30 04:58:56.000000 gardener_cicd_dso-1.2388.0/checkmarx/tablefmt.py
+-rw-r--r--   0 root         (0) root         (0)    19358 2024-04-30 04:58:56.000000 gardener_cicd_dso-1.2388.0/checkmarx/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 05:06:03.121183 gardener_cicd_dso-1.2388.0/clamav/
+-rw-r--r--   0 root         (0) root         (0)      132 2024-04-30 04:58:56.000000 gardener_cicd_dso-1.2388.0/clamav/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4680 2024-04-30 04:58:56.000000 gardener_cicd_dso-1.2388.0/clamav/client.py
+-rw-r--r--   0 root         (0) root         (0)     8472 2024-04-30 04:58:56.000000 gardener_cicd_dso-1.2388.0/clamav/cnudie.py
+-rw-r--r--   0 root         (0) root         (0)     2252 2024-04-30 04:58:56.000000 gardener_cicd_dso-1.2388.0/clamav/model.py
+-rw-r--r--   0 root         (0) root         (0)     1902 2024-04-30 04:58:56.000000 gardener_cicd_dso-1.2388.0/clamav/report.py
+-rw-r--r--   0 root         (0) root         (0)     1083 2024-04-30 04:58:56.000000 gardener_cicd_dso-1.2388.0/clamav/routes.py
+-rw-r--r--   0 root         (0) root         (0)     7469 2024-04-30 04:58:56.000000 gardener_cicd_dso-1.2388.0/clamav/scan.py
+-rw-r--r--   0 root         (0) root         (0)     5564 2024-04-30 04:58:56.000000 gardener_cicd_dso-1.2388.0/clamav/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 05:06:03.121183 gardener_cicd_dso-1.2388.0/gardener_cicd_dso.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      211 2024-04-30 05:06:03.000000 gardener_cicd_dso-1.2388.0/gardener_cicd_dso.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      670 2024-04-30 05:06:03.000000 gardener_cicd_dso-1.2388.0/gardener_cicd_dso.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 05:06:03.000000 gardener_cicd_dso-1.2388.0/gardener_cicd_dso.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2024-04-30 05:06:03.000000 gardener_cicd_dso-1.2388.0/gardener_cicd_dso.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2024-04-30 05:06:03.000000 gardener_cicd_dso-1.2388.0/gardener_cicd_dso.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 05:06:03.121183 gardener_cicd_dso-1.2388.0/protecode/
+-rw-r--r--   0 root         (0) root         (0)      132 2024-04-30 04:58:56.000000 gardener_cicd_dso-1.2388.0/protecode/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7653 2024-04-30 04:58:56.000000 gardener_cicd_dso-1.2388.0/protecode/assessments.py
+-rw-r--r--   0 root         (0) root         (0)    17319 2024-04-30 04:58:56.000000 gardener_cicd_dso-1.2388.0/protecode/client.py
+-rw-r--r--   0 root         (0) root         (0)    10709 2024-04-30 04:58:56.000000 gardener_cicd_dso-1.2388.0/protecode/model.py
+-rw-r--r--   0 root         (0) root         (0)     3636 2024-04-30 04:58:56.000000 gardener_cicd_dso-1.2388.0/protecode/rescore.py
+-rw-r--r--   0 root         (0) root         (0)    29221 2024-04-30 04:58:56.000000 gardener_cicd_dso-1.2388.0/protecode/scanning.py
+-rw-r--r--   0 root         (0) root         (0)    10915 2024-04-30 04:58:56.000000 gardener_cicd_dso-1.2388.0/protecode/util.py
+-rw-r--r--   0 root         (0) root         (0)      359 2024-04-30 04:58:56.000000 gardener_cicd_dso-1.2388.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      174 2024-04-30 05:06:03.121183 gardener_cicd_dso-1.2388.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      673 2024-04-30 04:58:56.000000 gardener_cicd_dso-1.2388.0/setup.dso.py
+-rw-r--r--   0 root         (0) root         (0)     2174 2024-04-30 04:58:56.000000 gardener_cicd_dso-1.2388.0/setup.py
```

### Comparing `gardener_cicd_dso-1.2387.0/LICENSE` & `gardener_cicd_dso-1.2388.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2387.0/README.md` & `gardener_cicd_dso-1.2388.0/README.md`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2387.0/checkmarx/client.py` & `gardener_cicd_dso-1.2388.0/checkmarx/client.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2387.0/checkmarx/model.py` & `gardener_cicd_dso-1.2388.0/checkmarx/model.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2387.0/checkmarx/project.py` & `gardener_cicd_dso-1.2388.0/checkmarx/project.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2387.0/checkmarx/tablefmt.py` & `gardener_cicd_dso-1.2388.0/checkmarx/tablefmt.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2387.0/checkmarx/util.py` & `gardener_cicd_dso-1.2388.0/checkmarx/util.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2387.0/clamav/client.py` & `gardener_cicd_dso-1.2388.0/clamav/client.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2387.0/clamav/cnudie.py` & `gardener_cicd_dso-1.2388.0/clamav/cnudie.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,15 +234,16 @@
             _scan_result_to_malware_finding(r)
             for r in aggregated_scan_result.findings
         ),
         metadata=dso.model.ClamAVMetadata(
             clamav_version_str=clamav_version_info.clamav_version_str,
             signature_version=clamav_version_info.signature_version,
             virus_definition_timestamp=clamav_version_info.signature_date,
-        )
+        ),
+        severity=gcm.Severity.BLOCKER.name,
     )
 
     return dso.model.ArtefactMetadata(
         artefact=artefact_ref,
         meta=meta,
         data=finding,
         discovery_date=discovery_date,
```

### Comparing `gardener_cicd_dso-1.2387.0/clamav/model.py` & `gardener_cicd_dso-1.2388.0/clamav/model.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2387.0/clamav/report.py` & `gardener_cicd_dso-1.2388.0/clamav/report.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2387.0/clamav/routes.py` & `gardener_cicd_dso-1.2388.0/clamav/routes.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2387.0/clamav/scan.py` & `gardener_cicd_dso-1.2388.0/clamav/scan.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2387.0/clamav/util.py` & `gardener_cicd_dso-1.2388.0/clamav/util.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2387.0/gardener_cicd_dso.egg-info/SOURCES.txt` & `gardener_cicd_dso-1.2388.0/gardener_cicd_dso.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2387.0/protecode/assessments.py` & `gardener_cicd_dso-1.2388.0/protecode/assessments.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2387.0/protecode/client.py` & `gardener_cicd_dso-1.2388.0/protecode/client.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2387.0/protecode/model.py` & `gardener_cicd_dso-1.2388.0/protecode/model.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2387.0/protecode/rescore.py` & `gardener_cicd_dso-1.2388.0/protecode/rescore.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2387.0/protecode/scanning.py` & `gardener_cicd_dso-1.2388.0/protecode/scanning.py`

 * *Files identical despite different names*

### Comparing `gardener_cicd_dso-1.2387.0/protecode/util.py` & `gardener_cicd_dso-1.2388.0/protecode/util.py`

 * *Files 21% similar despite different names*

```diff
@@ -34,27 +34,29 @@
 
     artefact = gcm.artifact_from_node(node=scanned_element)
     artefact_ref = dso.model.component_artefact_id_from_ocm(
         component=scanned_element.component,
         artefact=artefact,
     )
 
+    scan_id = dso.model.BDBAScanId(
+        base_url=scan_result.base_url(),
+        report_url=scan_result.report_url(),
+        product_id=scan_result.product_id(),
+        group_id=scan_result.group_id(),
+    )
+
+    has_license_findings = False
+    has_vulnerability_findings = False
     for package in scan_result.components():
         package_id = dso.model.BDBAPackageId(
             package_name=package.name(),
             package_version=package.version(),
         )
 
-        scan_id = dso.model.BDBAScanId(
-            base_url=scan_result.base_url(),
-            report_url=scan_result.report_url(),
-            product_id=scan_result.product_id(),
-            group_id=scan_result.group_id(),
-        )
-
         filesystem_paths = list({
             dso.model.FilesystemPath(
                 path=path,
                 digest=digest,
             ) for path, digest in iter_filesystem_paths(component=package)
         })
 
@@ -105,14 +107,15 @@
 
             yield dso.model.ArtefactMetadata(
                 artefact=artefact_ref,
                 meta=meta,
                 data=license_finding,
                 discovery_date=discovery_date,
             )
+            has_license_findings = True
 
         meta = dso.model.Metadata(
             datasource=dso.model.Datasource.BDBA,
             type=dso.model.Datatype.VULNERABILITY,
             creation_date=now,
             last_update=now,
         )
@@ -139,14 +142,67 @@
 
             yield dso.model.ArtefactMetadata(
                 artefact=artefact_ref,
                 meta=meta,
                 data=vulnerability_finding,
                 discovery_date=discovery_date,
             )
+            has_vulnerability_findings = True
+
+    if not has_license_findings:
+        # yield dummy finding so that delivery-service can handle "no license findings"-finding
+        meta = dso.model.Metadata(
+            datasource=dso.model.Datasource.BDBA,
+            type=dso.model.Datatype.LICENSE,
+            creation_date=now,
+            last_update=now,
+        )
+
+        dummy_finding = dso.model.LicenseFinding(
+            id=package_id,
+            scan_id=scan_id,
+            severity=gcm.Severity.NONE.name,
+            license=license,
+        )
+
+        yield dso.model.ArtefactMetadata(
+            artefact=artefact_ref,
+            meta=meta,
+            data=dummy_finding,
+            discovery_date=discovery_date,
+        )
+
+    if not has_vulnerability_findings:
+        # yield dummy finding so that delivery-service can handle "no license findings"-finding
+        meta = dso.model.Metadata(
+            datasource=dso.model.Datasource.BDBA,
+            type=dso.model.Datatype.VULNERABILITY,
+            creation_date=now,
+            last_update=now,
+        )
+
+        dummy_finding = dso.model.VulnerabilityFinding(
+            id=dso.model.BDBAPackageId(
+                package_name=None,
+                package_version=None,
+            ),
+            scan_id=scan_id,
+            severity=gcm.Severity.NONE.name,
+            cve=None,
+            cvss_v3_score=-1,
+            cvss=None,
+            summary=None,
+        )
+
+        yield dso.model.ArtefactMetadata(
+            artefact=artefact_ref,
+            meta=meta,
+            data=dummy_finding,
+            discovery_date=discovery_date,
+        )
 
 
 def iter_filesystem_paths(
     component: pm.Component,
     file_type: str | None=None,
 ) -> collections.abc.Generator[tuple[str, str], None, None]:
     for ext_obj in component.extended_objects():
```

### Comparing `gardener_cicd_dso-1.2387.0/setup.dso.py` & `gardener_cicd_dso-1.2388.0/setup.dso.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         return f.read().strip()
 
 
 setuptools.setup(
     name='gardener-cicd-dso',
     version=version(),
     description='Gardener CI/CD DevSecOps',
-    python_requires='>=3.10',
+    python_requires='>=3.11',
     py_modules=modules(),
     packages=[
         'checkmarx',
         'clamav',
         'protecode',
     ],
     package_data={
```

### Comparing `gardener_cicd_dso-1.2387.0/setup.py` & `gardener_cicd_dso-1.2388.0/setup.py`

 * *Files identical despite different names*

