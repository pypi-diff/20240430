# Comparing `tmp/openimis-be-claim_batch-1.6.0.tar.gz` & `tmp/openimis_be_claim_batch-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-claim_batch-1.6.0.tar", last modified: Sat Dec 16 00:57:21 2023, max compression
+gzip compressed data, was "openimis_be_claim_batch-1.7.0.tar", last modified: Tue Apr 30 09:05:57 2024, max compression
```

## Comparing `openimis-be-claim_batch-1.6.0.tar` & `openimis_be_claim_batch-1.7.0.tar`

### file list

```diff
@@ -1,40 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:21.879864 openimis-be-claim_batch-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2023-12-16 00:57:13.000000 openimis-be-claim_batch-1.6.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-16 00:57:13.000000 openimis-be-claim_batch-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      868 2023-12-16 00:57:21.879864 openimis-be-claim_batch-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2023-12-16 00:57:13.000000 openimis-be-claim_batch-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:21.875864 openimis-be-claim_batch-1.6.0/claim_batch/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-12-16 00:57:13.000000 openimis-be-claim_batch-1.6.0/claim_batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-16 00:57:13.000000 openimis-be-claim_batch-1.6.0/claim_batch/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2023-12-16 00:57:13.000000 openimis-be-claim_batch-1.6.0/claim_batch/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:21.879864 openimis-be-claim_batch-1.6.0/claim_batch/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2023-12-16 00:57:13.000000 openimis-be-claim_batch-1.6.0/claim_batch/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2023-12-16 00:57:13.000000 openimis-be-claim_batch-1.6.0/claim_batch/migrations/0002_capitationpayment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2023-12-16 00:57:13.000000 openimis-be-claim_batch-1.6.0/claim_batch/migrations/0003_capitationpayment_for_legacy_batch_runs.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2023-12-16 00:57:13.000000 openimis-be-claim_batch-1.6.0/claim_batch/migrations/0004_delete_capitationpayment.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2023-12-16 00:57:13.000000 openimis-be-claim_batch-1.6.0/claim_batch/migrations/0005_capitationpayment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5735 2023-12-16 00:57:13.000000 openimis-be-claim_batch-1.6.0/claim_batch/migrations/0006_capitationpayment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2023-12-16 00:57:13.000000 openimis-be-claim_batch-1.6.0/claim_batch/migrations/0007_update_django_scheme_with_missing_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2023-12-16 00:57:13.000000 openimis-be-claim_batch-1.6.0/claim_batch/migrations/0008_set_managed_to_true.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:13.000000 openimis-be-claim_batch-1.6.0/claim_batch/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8041 2023-12-16 00:57:13.000000 openimis-be-claim_batch-1.6.0/claim_batch/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:21.879864 openimis-be-claim_batch-1.6.0/claim_batch/reports/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:13.000000 openimis-be-claim_batch-1.6.0/claim_batch/reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   137336 2023-12-16 00:57:13.000000 openimis-be-claim_batch-1.6.0/claim_batch/reports/pbc_H.py
--rw-r--r--   0 runner    (1001) docker     (127)   136833 2023-12-16 00:57:13.000000 openimis-be-claim_batch-1.6.0/claim_batch/reports/pbc_P.py
--rw-r--r--   0 runner    (1001) docker     (127)    53878 2023-12-16 00:57:13.000000 openimis-be-claim_batch-1.6.0/claim_batch/reports/pbh.py
--rw-r--r--   0 runner    (1001) docker     (127)    53904 2023-12-16 00:57:13.000000 openimis-be-claim_batch-1.6.0/claim_batch/reports/pbp.py
--rw-r--r--   0 runner    (1001) docker     (127)     7417 2023-12-16 00:57:13.000000 openimis-be-claim_batch-1.6.0/claim_batch/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    30420 2023-12-16 00:57:13.000000 openimis-be-claim_batch-1.6.0/claim_batch/services.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2023-12-16 00:57:13.000000 openimis-be-claim_batch-1.6.0/claim_batch/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6976 2023-12-16 00:57:13.000000 openimis-be-claim_batch-1.6.0/claim_batch/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-16 00:57:13.000000 openimis-be-claim_batch-1.6.0/claim_batch/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2023-12-16 00:57:13.000000 openimis-be-claim_batch-1.6.0/claim_batch/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:21.879864 openimis-be-claim_batch-1.6.0/openimis_be_claim_batch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      868 2023-12-16 00:57:21.000000 openimis-be-claim_batch-1.6.0/openimis_be_claim_batch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2023-12-16 00:57:21.000000 openimis-be-claim_batch-1.6.0/openimis_be_claim_batch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-16 00:57:21.000000 openimis-be-claim_batch-1.6.0/openimis_be_claim_batch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-16 00:57:21.000000 openimis-be-claim_batch-1.6.0/openimis_be_claim_batch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-12-16 00:57:21.000000 openimis-be-claim_batch-1.6.0/openimis_be_claim_batch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-16 00:57:21.879864 openimis-be-claim_batch-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2023-12-16 00:57:21.000000 openimis-be-claim_batch-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:57.049707 openimis_be_claim_batch-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-30 09:05:45.000000 openimis_be_claim_batch-1.7.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-30 09:05:45.000000 openimis_be_claim_batch-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-30 09:05:57.049707 openimis_be_claim_batch-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-30 09:05:45.000000 openimis_be_claim_batch-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:57.045707 openimis_be_claim_batch-1.7.0/claim_batch/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 09:05:45.000000 openimis_be_claim_batch-1.7.0/claim_batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-30 09:05:45.000000 openimis_be_claim_batch-1.7.0/claim_batch/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-30 09:05:45.000000 openimis_be_claim_batch-1.7.0/claim_batch/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:57.045707 openimis_be_claim_batch-1.7.0/claim_batch/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-30 09:05:45.000000 openimis_be_claim_batch-1.7.0/claim_batch/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-30 09:05:45.000000 openimis_be_claim_batch-1.7.0/claim_batch/migrations/0002_capitationpayment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-30 09:05:45.000000 openimis_be_claim_batch-1.7.0/claim_batch/migrations/0003_capitationpayment_for_legacy_batch_runs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-30 09:05:45.000000 openimis_be_claim_batch-1.7.0/claim_batch/migrations/0004_delete_capitationpayment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-30 09:05:45.000000 openimis_be_claim_batch-1.7.0/claim_batch/migrations/0005_capitationpayment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5735 2024-04-30 09:05:45.000000 openimis_be_claim_batch-1.7.0/claim_batch/migrations/0006_capitationpayment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-30 09:05:45.000000 openimis_be_claim_batch-1.7.0/claim_batch/migrations/0007_update_django_scheme_with_missing_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-30 09:05:45.000000 openimis_be_claim_batch-1.7.0/claim_batch/migrations/0008_set_managed_to_true.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:45.000000 openimis_be_claim_batch-1.7.0/claim_batch/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8041 2024-04-30 09:05:45.000000 openimis_be_claim_batch-1.7.0/claim_batch/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:57.045707 openimis_be_claim_batch-1.7.0/claim_batch/reports/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:45.000000 openimis_be_claim_batch-1.7.0/claim_batch/reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   137336 2024-04-30 09:05:45.000000 openimis_be_claim_batch-1.7.0/claim_batch/reports/pbc_H.py
+-rw-r--r--   0 runner    (1001) docker     (127)   136833 2024-04-30 09:05:45.000000 openimis_be_claim_batch-1.7.0/claim_batch/reports/pbc_P.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53878 2024-04-30 09:05:45.000000 openimis_be_claim_batch-1.7.0/claim_batch/reports/pbh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53904 2024-04-30 09:05:45.000000 openimis_be_claim_batch-1.7.0/claim_batch/reports/pbp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7417 2024-04-30 09:05:45.000000 openimis_be_claim_batch-1.7.0/claim_batch/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30907 2024-04-30 09:05:45.000000 openimis_be_claim_batch-1.7.0/claim_batch/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-30 09:05:45.000000 openimis_be_claim_batch-1.7.0/claim_batch/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:57.045707 openimis_be_claim_batch-1.7.0/claim_batch/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:45.000000 openimis_be_claim_batch-1.7.0/claim_batch/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6990 2024-04-30 09:05:45.000000 openimis_be_claim_batch-1.7.0/claim_batch/tests/test_graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7223 2024-04-30 09:05:45.000000 openimis_be_claim_batch-1.7.0/claim_batch/tests/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-30 09:05:45.000000 openimis_be_claim_batch-1.7.0/claim_batch/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-04-30 09:05:45.000000 openimis_be_claim_batch-1.7.0/claim_batch/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:57.049707 openimis_be_claim_batch-1.7.0/openimis_be_claim_batch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-30 09:05:57.000000 openimis_be_claim_batch-1.7.0/openimis_be_claim_batch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-30 09:05:57.000000 openimis_be_claim_batch-1.7.0/openimis_be_claim_batch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:05:57.000000 openimis_be_claim_batch-1.7.0/openimis_be_claim_batch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-30 09:05:57.000000 openimis_be_claim_batch-1.7.0/openimis_be_claim_batch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-30 09:05:57.000000 openimis_be_claim_batch-1.7.0/openimis_be_claim_batch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 09:05:57.049707 openimis_be_claim_batch-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-30 09:05:56.000000 openimis_be_claim_batch-1.7.0/setup.py
```

### Comparing `openimis-be-claim_batch-1.6.0/LICENSE.md` & `openimis_be_claim_batch-1.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis-be-claim_batch-1.6.0/PKG-INFO` & `openimis_be_claim_batch-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-claim_batch
-Version: 1.6.0
+Version: 1.7.0
 Summary: The openIMIS Backend Claim Batch reference module.
 Home-page: https://openimis.org/
 Author: Xavier Gillmann
 Author-email: xgillmann@bluesquarehub.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-claim_batch-1.6.0/README.md` & `openimis_be_claim_batch-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `openimis-be-claim_batch-1.6.0/claim_batch/apps.py` & `openimis_be_claim_batch-1.7.0/claim_batch/apps.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim_batch-1.6.0/claim_batch/migrations/0001_initial.py` & `openimis_be_claim_batch-1.7.0/claim_batch/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim_batch-1.6.0/claim_batch/migrations/0003_capitationpayment_for_legacy_batch_runs.py` & `openimis_be_claim_batch-1.7.0/claim_batch/migrations/0003_capitationpayment_for_legacy_batch_runs.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim_batch-1.6.0/claim_batch/migrations/0006_capitationpayment.py` & `openimis_be_claim_batch-1.7.0/claim_batch/migrations/0006_capitationpayment.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim_batch-1.6.0/claim_batch/migrations/0007_update_django_scheme_with_missing_fields.py` & `openimis_be_claim_batch-1.7.0/claim_batch/migrations/0007_update_django_scheme_with_missing_fields.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim_batch-1.6.0/claim_batch/migrations/0008_set_managed_to_true.py` & `openimis_be_claim_batch-1.7.0/claim_batch/migrations/0008_set_managed_to_true.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim_batch-1.6.0/claim_batch/models.py` & `openimis_be_claim_batch-1.7.0/claim_batch/models.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim_batch-1.6.0/claim_batch/reports/pbc_H.py` & `openimis_be_claim_batch-1.7.0/claim_batch/reports/pbc_H.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim_batch-1.6.0/claim_batch/reports/pbc_P.py` & `openimis_be_claim_batch-1.7.0/claim_batch/reports/pbc_P.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim_batch-1.6.0/claim_batch/reports/pbh.py` & `openimis_be_claim_batch-1.7.0/claim_batch/reports/pbh.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim_batch-1.6.0/claim_batch/reports/pbp.py` & `openimis_be_claim_batch-1.7.0/claim_batch/reports/pbp.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim_batch-1.6.0/claim_batch/schema.py` & `openimis_be_claim_batch-1.7.0/claim_batch/schema.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim_batch-1.6.0/claim_batch/services.py` & `openimis_be_claim_batch-1.7.0/claim_batch/services.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 import pandas as pd
 from django.contrib.admin.options import get_content_type_for_model
 from django.contrib.contenttypes.models import ContentType
 
 import core
 
 from datetime import date
-from django.db import connection, transaction
-from django.db.models import Value, F, Sum, Q, Prefetch, Count, Subquery, OuterRef, FloatField
-from django.db.models.functions import Coalesce, ExtractMonth, ExtractYear
+from django.db import connection, transaction, DatabaseError
+from django.db.models import Value, F, Sum, Q, Prefetch, Count, Subquery, OuterRef, FloatField, TextField
+from django.db.models.functions import Coalesce, ExtractMonth, ExtractYear, Cast
 from django.utils.translation import gettext as _
 
 from calculation.services import run_calculation_rules, get_calculation_object
 from claim.models import ClaimItem, Claim, ClaimService, ClaimDetail
 from claim_batch.models import BatchRun, RelativeIndex, RelativeDistribution
 from contribution.models import Premium
 from contribution_plan.models import PaymentPlan
@@ -138,21 +138,22 @@
 @transaction.atomic
 def process_batch(audit_user_id, location_id, period, year):
     # declare table tblClaimsIDs
     if location_id == -1:
         location_id = None
 
     # Transactional stuff
-    already_run_batch = BatchRun.objects \
-        .filter(run_year=year) \
-        .filter(run_month=period) \
-        .annotate(nn_location_id=Coalesce("location_id", Value(-1))) \
-        .filter(nn_location_id=-1 if location_id is None else location_id) \
-        .filter(validity_to__isnull=True).values("id").first()
+    queryset = BatchRun.objects \
+        .filter(run_year=year,run_month=period,*core.utils.filter_validity())
+    if location_id is None:
+        queryset=queryset.filter(location_id__isnull = True)
+    else:
+        queryset=queryset.filter(location__id = location_id)
 
+    already_run_batch = queryset.values("id").first()
     if already_run_batch:
         return [str(ProcessBatchSubmitError(2))]
     _, days_in_month = calendar.monthrange(year, period)
     end_date = datetime.datetime(year, period, days_in_month)
     now = datetime.datetime.now()
     # TODO - double check this condition
     # if end_date < now:
@@ -192,35 +193,35 @@
     year = end_date.year
     logger.debug("do_process_batch location %s for %s/%s", location_id, period, year)
 
     from core.utils import TimeUtils
     created_run = BatchRun.objects.create(location_id=location_id, run_year=year, run_month=period,
                                           run_date=TimeUtils.now(), audit_user_id=audit_user_id,
                                           validity_from=TimeUtils.now())
-    logger.debug("do_process_batch created run: %s", created_run.id)
+    logger.debug(f"do_process_batch created run: {created_run.id}" )
 
     # 0 prepare the batch run :  does it really make sense
     # per location ? (Ideally per pool but the notion doesn't exist yet)
     # 0.1 get all product concerned, all product that have are configured for the location
     # init start dates
     start_date = None
 
     # period_quarter = period - 2 if period % 3 == 0 else 0
     # period_sem = period - 5 if period % 6 == 0 else 0
 
     products = get_product_queryset(end_date, location_id)
     # 1 per product (Ideally per pool but the notion doesn't exist yet)
     if products:
         for product in products:
-            logger.debug("do_process_batch creating work_data for batch run process")
+            logger.debug(f"do_process_batch creating batch run process for product {product.code}-{product.name}")
             work_data = {"created_run": created_run, "product": product, "end_date": end_date}
-            logger.debug("do_process_batch created work_data for batch run process")
-            allocated_contribution = {}
+            allocated_contribution = None
             # 1.2 get all the payment plan per product
             work_data["payment_plans"] = get_payment_plan_queryset(product, end_date)
+            logger.debug(f"{len(work_data['payment_plans'])} payment plan found")
             # valuate the claims
             # 5 Generate BatchPayment per product (Ideally per pool but the notion doesn't exist yet)
             trigger_calculation_based_on_context(
                 "BatchValuate", work_data, end_date, product, location_id, allocated_contribution, audit_user_id
             )
             # 5.1 filter a calculation valid for batchRun with context BatchPayment (got via 0.2)
             # 54.2 Execute the converter per product/batch run/claim (not claims)
@@ -235,40 +236,47 @@
 
 
 def trigger_calculation_based_on_context(
         context, work_data, end_date, product,
         location_id, allocated_contribution, user_id
 ):
     if work_data["payment_plans"]:
+        
         for payment_plan in work_data["payment_plans"]:
+            logger.debug(f"Starting evaluating payment plan {payment_plan.code}")
             start_date = get_start_date(end_date, payment_plan.periodicity)
             # run only when it makes sense based on periodicitiy
             if start_date is not None:
                 allocated_contribution, work_data = update_work_data(
                     work_data, product, start_date, end_date, allocated_contribution
                 )
                 calculation = get_calculation_object(payment_plan.calculation)
                 if calculation is not None:
                     rcr = calculation.calculate_if_active_for_object(
                         payment_plan, context=context,
                         work_data=work_data, audit_user_id=user_id,
                         location_id=location_id, start_date=start_date, end_date=end_date
                     )
                     if rcr:
-                        logger.debug("conversion processed for: %s", rcr[0][0])
+                        logger.debug("conversion processed for: %s", str(rcr))
+                    else:
+                        logger.debug(f"No conversion done for {payment_plan.code}")
+                else:
+                    logger.debug(f"Calulation nof found for {payment_plan.code}")
 
 
 def update_work_data(work_data, product, start_date, end_date, allocated_contribution=None):
     work_data["start_date"] = start_date
-    # 1.3 generate queryset
+# 1.3 generate queryset
     work_data["items"] = get_items_queryset(product, start_date, end_date)
     work_data["services"] = get_services_queryset(product, start_date, end_date)
     work_data["contributions"] = get_contribution_queryset(product, start_date, end_date)
     work_data['claims'] = get_claim_queryset(product, start_date, end_date)
     work_data['bill_payments'] = get_bill_payment_queryset(product, start_date, end_date)
+    
     work_data['invoice_payments'] = get_invoice_payment_queryset(product, start_date, end_date)
     if allocated_contribution is None:
         allocated_contribution = {}
     start_date_str = str(start_date)
     if start_date_str not in allocated_contribution:
         allocated_contribution[start_date_str] = get_allocated_premium(
             get_allocated_contribution_queryset(product, start_date, end_date), start_date, end_date)
@@ -339,37 +347,43 @@
     return Premium.objects \
         .filter(validity_to__isnull=True) \
         .filter(created_date__range=(start_date, end_date)) \
         .filter(policy__product=product)
 
 
 def get_bill_payment_queryset(product, start_date, end_date):
-    return BillPayment.objects \
-        .filter(is_deleted=False) \
-        .filter(date_created__range=(start_date, end_date)) \
-        .filter(bill__line_items_bill__in=BillItem.objects
-                .filter(is_deleted=False)
-                .filter(line_type=get_content_type_for_model(Premium))
-                .filter(line_id__in=Premium.objects
+    # need to get the invoice with lines that match premium for that product
+
+    
+    qs = BillPayment.objects.filter(is_deleted=False)\
+        .filter(date_created__gte=start_date, date_created__lt=end_date)\
+        .filter(bill__line_items_bill__line_type=get_content_type_for_model(Premium),
+                bill__line_items_bill__line_id__in=Subquery(Premium.objects
                         .filter(validity_to__isnull=True)
                         .filter(policy__product=product)
-                        .values_list('id', flat=True)))
+                        .annotate(as_str=Cast('id', TextField())).values('as_str')
+                        
+                    ))
+    return qs
 
 
 def get_invoice_payment_queryset(product, start_date, end_date):
-    return InvoicePayment.objects \
-        .filter(is_deleted=False) \
-        .filter(date_created__range=(start_date, end_date)) \
-        .filter(invoice__line_items__in=InvoiceLineItem.objects
-                .filter(is_deleted=False)
-                .filter(line_type=get_content_type_for_model(Premium))
-                .filter(line_id__in=Premium.objects
+    
+    qs = InvoicePayment.objects.filter(is_deleted=False)\
+    .filter(date_created__gte=start_date, date_created__lt=end_date)\
+    .filter(invoice__line_items__line_type=get_content_type_for_model(Premium),
+                invoice__line_items__line_id__in=Subquery(Premium.objects
                         .filter(validity_to__isnull=True)
                         .filter(policy__product=product)
-                        .values_list('id', flat=True)))
+                        .annotate(as_str=Cast('id', TextField())).values('as_str')
+                    ))
+    return qs
+
+            
+        
 
 
 def get_allocated_premium(premiums, start_date, end_date):
     # Calculate allcated contributions
     # go trough the contribution and find the allocated contribution
     allocated_premiums = 0
     for premium in premiums:
```

### Comparing `openimis-be-claim_batch-1.6.0/claim_batch/test_helpers.py` & `openimis_be_claim_batch-1.7.0/claim_batch/test_helpers.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim_batch-1.6.0/claim_batch/tests.py` & `openimis_be_claim_batch-1.7.0/claim_batch/tests/tests.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 import calendar
 import datetime
 
-from claim.gql_mutations import validate_and_process_dedrem_claim
+from claim.services import submit_claim, validate_and_process_dedrem_claim
 from claim.models import ClaimDedRem, Claim
 from claim.test_helpers import (
     create_test_claim,
     create_test_claimservice,
     create_test_claimitem,
     delete_claim_with_itemsvc_dedrem_and_history,
 )
-from claim_batch.services import do_process_batch
+from claim_batch.services import do_process_batch, process_batch
 from contribution.test_helpers import create_test_payer, create_test_premium
 from contribution_plan.models import PaymentPlan
 from contribution_plan.tests.helpers import create_test_payment_plan
 from core.services import create_or_update_interactive_user, create_or_update_core_user
 from django.test import TestCase
 from insuree.test_helpers import create_test_insuree
 from medical.test_helpers import create_test_service, create_test_item
 from medical_pricelist.test_helpers import (
     add_service_to_hf_pricelist,
     add_item_to_hf_pricelist,
 )
 from policy.test_helpers import create_test_policy
-from product.models import ProductItemOrService
 from product.test_helpers import (
     create_test_product,
     create_test_product_service,
     create_test_product_item,
 )
+from product.models import ProductItemOrService
+
 
 
 _TEST_USER_NAME = "test_batch_run"
 _TEST_USER_PASSWORD = "test_batch_run"
 _TEST_DATA_USER = {
     "username": _TEST_USER_NAME,
     "last_name": _TEST_USER_NAME,
@@ -121,21 +122,25 @@
         premium = create_test_premium(
             policy_id=policy.id, custom_props={"payer_id": payer.id}
         )
         pricelist_detail1 = add_service_to_hf_pricelist(service)
         pricelist_detail2 = add_item_to_hf_pricelist(item)
 
         claim1 = create_test_claim({"insuree_id": insuree.id})
+
         service1 = create_test_claimservice(
             claim1, custom_props={"service_id": service.id, "qty_provided": 2, "price_origin": ProductItemOrService.ORIGIN_RELATIVE}
         )
         item1 = create_test_claimitem(
             claim1, "A", custom_props={"item_id": item.id, "qty_provided": 3, "price_origin": ProductItemOrService.ORIGIN_RELATIVE}
         )
-        errors = validate_and_process_dedrem_claim(claim1, self.user, True)
+        claim1.refresh_from_db()
+        errors = []
+        errors += submit_claim(claim1, self.user)
+        errors += validate_and_process_dedrem_claim(claim1, self.user, True)
         _, days_in_month = calendar.monthrange(claim1.validity_from.year, claim1.validity_from.month)
         # add process stamp for claim to not use the process_stamp with now()
         claim1.process_stamp = datetime.datetime(claim1.validity_from.year, claim1.validity_from.month, days_in_month-1)
         claim1.save()
 
         self.assertEqual(len(errors), 0)
         self.assertEqual(
@@ -146,19 +151,20 @@
         # Make sure that the dedrem was generated
         dedrem = ClaimDedRem.objects.filter(claim=claim1).first()
         self.assertIsNotNone(dedrem)
         self.assertEquals(dedrem.rem_g, 500)  # 100*2 + 100*3
 
         # When
         end_date = datetime.datetime(claim1.validity_from.year, claim1.validity_from.month, days_in_month)
-
-        do_process_batch(
+        # run batch (audit_user_id, location_id, period, year):
+        process_batch(
             self.user.id_for_audit,
             None,
-            end_date
+            claim1.validity_from.month,
+            claim1.validity_from.year
         )
 
         claim1.refresh_from_db()
         item1.refresh_from_db()
         service1.refresh_from_db()
 
         self.assertEquals(claim1.status, Claim.STATUS_VALUATED)
```

### Comparing `openimis-be-claim_batch-1.6.0/claim_batch/views.py` & `openimis_be_claim_batch-1.7.0/claim_batch/views.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim_batch-1.6.0/openimis_be_claim_batch.egg-info/PKG-INFO` & `openimis_be_claim_batch-1.7.0/openimis_be_claim_batch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: openimis-be-claim-batch
-Version: 1.6.0
+Name: openimis-be-claim_batch
+Version: 1.7.0
 Summary: The openIMIS Backend Claim Batch reference module.
 Home-page: https://openimis.org/
 Author: Xavier Gillmann
 Author-email: xgillmann@bluesquarehub.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-claim_batch-1.6.0/openimis_be_claim_batch.egg-info/SOURCES.txt` & `openimis_be_claim_batch-1.7.0/openimis_be_claim_batch.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 claim_batch/__init__.py
 claim_batch/admin.py
 claim_batch/apps.py
 claim_batch/models.py
 claim_batch/schema.py
 claim_batch/services.py
 claim_batch/test_helpers.py
-claim_batch/tests.py
 claim_batch/urls.py
 claim_batch/views.py
 claim_batch/migrations/0001_initial.py
 claim_batch/migrations/0002_capitationpayment.py
 claim_batch/migrations/0003_capitationpayment_for_legacy_batch_runs.py
 claim_batch/migrations/0004_delete_capitationpayment.py
 claim_batch/migrations/0005_capitationpayment.py
@@ -22,12 +21,15 @@
 claim_batch/migrations/0008_set_managed_to_true.py
 claim_batch/migrations/__init__.py
 claim_batch/reports/__init__.py
 claim_batch/reports/pbc_H.py
 claim_batch/reports/pbc_P.py
 claim_batch/reports/pbh.py
 claim_batch/reports/pbp.py
+claim_batch/tests/__init__.py
+claim_batch/tests/test_graphql.py
+claim_batch/tests/tests.py
 openimis_be_claim_batch.egg-info/PKG-INFO
 openimis_be_claim_batch.egg-info/SOURCES.txt
 openimis_be_claim_batch.egg-info/dependency_links.txt
 openimis_be_claim_batch.egg-info/requires.txt
 openimis_be_claim_batch.egg-info/top_level.txt
```

### Comparing `openimis-be-claim_batch-1.6.0/setup.py` & `openimis_be_claim_batch-1.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-claim_batch',
-    version='v1.6.0',
+    version='v1.7.0',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend Claim Batch reference module.',
     # long_description=README,
     url='https://openimis.org/',
     author='Xavier Gillmann',
```

