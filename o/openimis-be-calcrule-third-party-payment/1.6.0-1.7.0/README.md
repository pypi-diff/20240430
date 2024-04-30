# Comparing `tmp/openimis-be-calcrule-third_party_payment-1.6.0.tar.gz` & `tmp/openimis_be_calcrule_third_party_payment-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-calcrule-third_party_payment-1.6.0.tar", last modified: Sat Dec 16 00:58:00 2023, max compression
+gzip compressed data, was "openimis_be_calcrule_third_party_payment-1.7.0.tar", last modified: Tue Apr 30 09:06:54 2024, max compression
```

## Comparing `openimis-be-calcrule-third_party_payment-1.6.0.tar` & `openimis_be_calcrule_third_party_payment-1.7.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:58:00.653642 openimis-be-calcrule-third_party_payment-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2023-12-16 00:57:49.000000 openimis-be-calcrule-third_party_payment-1.6.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2023-12-16 00:58:00.653642 openimis-be-calcrule-third_party_payment-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      697 2023-12-16 00:57:49.000000 openimis-be-calcrule-third_party_payment-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:58:00.649642 openimis-be-calcrule-third_party_payment-1.6.0/calcrule_third_party_payment/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2023-12-16 00:57:49.000000 openimis-be-calcrule-third_party_payment-1.6.0/calcrule_third_party_payment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-16 00:57:49.000000 openimis-be-calcrule-third_party_payment-1.6.0/calcrule_third_party_payment/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2023-12-16 00:57:49.000000 openimis-be-calcrule-third_party_payment-1.6.0/calcrule_third_party_payment/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)    11174 2023-12-16 00:57:49.000000 openimis-be-calcrule-third_party_payment-1.6.0/calcrule_third_party_payment/calculation_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    11463 2023-12-16 00:57:49.000000 openimis-be-calcrule-third_party_payment-1.6.0/calcrule_third_party_payment/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:58:00.649642 openimis-be-calcrule-third_party_payment-1.6.0/calcrule_third_party_payment/converters/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2023-12-16 00:57:49.000000 openimis-be-calcrule-third_party_payment-1.6.0/calcrule_third_party_payment/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2023-12-16 00:57:49.000000 openimis-be-calcrule-third_party_payment-1.6.0/calcrule_third_party_payment/converters/claim_to_bill_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     2903 2023-12-16 00:57:49.000000 openimis-be-calcrule-third_party_payment-1.6.0/calcrule_third_party_payment/converters/claims_to_bill.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:58:00.649642 openimis-be-calcrule-third_party_payment-1.6.0/calcrule_third_party_payment/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:49.000000 openimis-be-calcrule-third_party_payment-1.6.0/calcrule_third_party_payment/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-12-16 00:57:49.000000 openimis-be-calcrule-third_party_payment-1.6.0/calcrule_third_party_payment/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     9511 2023-12-16 00:57:49.000000 openimis-be-calcrule-third_party_payment-1.6.0/calcrule_third_party_payment/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-12-16 00:57:49.000000 openimis-be-calcrule-third_party_payment-1.6.0/calcrule_third_party_payment/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     5269 2023-12-16 00:57:49.000000 openimis-be-calcrule-third_party_payment-1.6.0/calcrule_third_party_payment/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-16 00:57:49.000000 openimis-be-calcrule-third_party_payment-1.6.0/calcrule_third_party_payment/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:58:00.653642 openimis-be-calcrule-third_party_payment-1.6.0/openimis_be_calcrule_third_party_payment.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2023-12-16 00:58:00.000000 openimis-be-calcrule-third_party_payment-1.6.0/openimis_be_calcrule_third_party_payment.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      966 2023-12-16 00:58:00.000000 openimis-be-calcrule-third_party_payment-1.6.0/openimis_be_calcrule_third_party_payment.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-16 00:58:00.000000 openimis-be-calcrule-third_party_payment-1.6.0/openimis_be_calcrule_third_party_payment.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2023-12-16 00:58:00.000000 openimis-be-calcrule-third_party_payment-1.6.0/openimis_be_calcrule_third_party_payment.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-16 00:58:00.000000 openimis-be-calcrule-third_party_payment-1.6.0/openimis_be_calcrule_third_party_payment.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-16 00:58:00.653642 openimis-be-calcrule-third_party_payment-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2023-12-16 00:58:00.000000 openimis-be-calcrule-third_party_payment-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:54.309049 openimis_be_calcrule_third_party_payment-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-30 09:06:43.000000 openimis_be_calcrule_third_party_payment-1.7.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-30 09:06:54.309049 openimis_be_calcrule_third_party_payment-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-30 09:06:43.000000 openimis_be_calcrule_third_party_payment-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:54.305049 openimis_be_calcrule_third_party_payment-1.7.0/calcrule_third_party_payment/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-30 09:06:43.000000 openimis_be_calcrule_third_party_payment-1.7.0/calcrule_third_party_payment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 09:06:43.000000 openimis_be_calcrule_third_party_payment-1.7.0/calcrule_third_party_payment/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-30 09:06:43.000000 openimis_be_calcrule_third_party_payment-1.7.0/calcrule_third_party_payment/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11295 2024-04-30 09:06:43.000000 openimis_be_calcrule_third_party_payment-1.7.0/calcrule_third_party_payment/calculation_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11463 2024-04-30 09:06:43.000000 openimis_be_calcrule_third_party_payment-1.7.0/calcrule_third_party_payment/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:54.309049 openimis_be_calcrule_third_party_payment-1.7.0/calcrule_third_party_payment/converters/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-30 09:06:43.000000 openimis_be_calcrule_third_party_payment-1.7.0/calcrule_third_party_payment/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-04-30 09:06:43.000000 openimis_be_calcrule_third_party_payment-1.7.0/calcrule_third_party_payment/converters/claim_to_bill_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-04-30 09:06:43.000000 openimis_be_calcrule_third_party_payment-1.7.0/calcrule_third_party_payment/converters/claims_to_bill.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:54.309049 openimis_be_calcrule_third_party_payment-1.7.0/calcrule_third_party_payment/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:43.000000 openimis_be_calcrule_third_party_payment-1.7.0/calcrule_third_party_payment/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 09:06:43.000000 openimis_be_calcrule_third_party_payment-1.7.0/calcrule_third_party_payment/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9525 2024-04-30 09:06:43.000000 openimis_be_calcrule_third_party_payment-1.7.0/calcrule_third_party_payment/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-30 09:06:43.000000 openimis_be_calcrule_third_party_payment-1.7.0/calcrule_third_party_payment/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5269 2024-04-30 09:06:43.000000 openimis_be_calcrule_third_party_payment-1.7.0/calcrule_third_party_payment/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 09:06:43.000000 openimis_be_calcrule_third_party_payment-1.7.0/calcrule_third_party_payment/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:54.309049 openimis_be_calcrule_third_party_payment-1.7.0/openimis_be_calcrule_third_party_payment.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-30 09:06:54.000000 openimis_be_calcrule_third_party_payment-1.7.0/openimis_be_calcrule_third_party_payment.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-30 09:06:54.000000 openimis_be_calcrule_third_party_payment-1.7.0/openimis_be_calcrule_third_party_payment.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:06:54.000000 openimis_be_calcrule_third_party_payment-1.7.0/openimis_be_calcrule_third_party_payment.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-30 09:06:54.000000 openimis_be_calcrule_third_party_payment-1.7.0/openimis_be_calcrule_third_party_payment.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-30 09:06:54.000000 openimis_be_calcrule_third_party_payment-1.7.0/openimis_be_calcrule_third_party_payment.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 09:06:54.309049 openimis_be_calcrule_third_party_payment-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-30 09:06:53.000000 openimis_be_calcrule_third_party_payment-1.7.0/setup.py
```

### Comparing `openimis-be-calcrule-third_party_payment-1.6.0/LICENSE.md` & `openimis_be_calcrule_third_party_payment-1.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule-third_party_payment-1.6.0/PKG-INFO` & `openimis_be_calcrule_third_party_payment-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-calcrule-third_party_payment
-Version: 1.6.0
+Version: 1.7.0
 Summary: The openIMIS Backend calculation rule thirdparty payment reference module.
 Home-page: https://openimis.org/
 Author: Seweryn Niedzielski
 Author-email: sniedzielski@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-calcrule-third_party_payment-1.6.0/README.md` & `openimis_be_calcrule_third_party_payment-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule-third_party_payment-1.6.0/calcrule_third_party_payment/apps.py` & `openimis_be_calcrule_third_party_payment-1.7.0/calcrule_third_party_payment/apps.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule-third_party_payment-1.6.0/calcrule_third_party_payment/calculation_rule.py` & `openimis_be_calcrule_third_party_payment-1.7.0/calcrule_third_party_payment/calculation_rule.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,35 +30,36 @@
 from core.signals import *
 from core import datetime
 from invoice.services import BillService
 
 from product.models import Product
 from calcrule_third_party_payment.converters import ClaimsToBillConverter, ClaimToBillItemConverter
 from core.models import User
-
+import logging
+logger = logging.getLogger(__name__)
 
 class ThirdPartyPaymentCalculationRule(AbsCalculationRule):
     version = 1
     uuid = "0a1b6d54-eef4-4ee6-ac47-2a99cfa5e9a8"
     calculation_rule_name = "payment: fee for service"
     description = DESCRIPTION_CONTRIBUTION_VALUATION
     impacted_class_parameter = CLASS_RULE_PARAM_VALIDATION
     date_valid_from = datetime.datetime(2000, 1, 1)
     date_valid_to = None
     status = "active"
     from_to = FROM_TO
     type = "account_payable"
     sub_type = "third_party_payment"
 
-    signal_get_rule_name = Signal(providing_args=[])
-    signal_get_rule_details = Signal(providing_args=[])
-    signal_get_param = Signal(providing_args=[])
-    signal_get_linked_class = Signal(providing_args=[])
-    signal_calculate_event = Signal(providing_args=[])
-    signal_convert_from_to = Signal(providing_args=[])
+    signal_get_rule_name = Signal([])
+    signal_get_rule_details = Signal([])
+    signal_get_param = Signal([])
+    signal_get_linked_class = Signal([])
+    signal_calculate_event = Signal([])
+    signal_convert_from_to = Signal([])
 
     @classmethod
     def ready(cls):
         now = datetime.datetime.now()
         condition_is_valid = (now >= cls.date_valid_from and now <= cls.date_valid_to) \
             if cls.date_valid_to else (now >= cls.date_valid_from and cls.date_valid_to is None)
         if condition_is_valid:
@@ -163,14 +164,15 @@
             results['user'] = kwargs.get('user', None)
             BillService.bill_create(convert_results=results)
         return results
 
     @classmethod
     def convert_batch(cls, **kwargs):
         work_data = kwargs.get('work_data', None)
+        logger.debug(f"creating bill for br {work_data['created_run']}")
         if work_data:
             user = User.objects.filter(i_user__id=work_data['created_run'].audit_user_id).first()
             # create queryset based on provided params
             claim_queryset = Claim.objects.filter(validity_to=None, batch_run=work_data['created_run'], health_facility__isnull=False)
             claim_br_hf_list = list(claim_queryset.values('batch_run', 'health_facility').distinct())
             for cbh in claim_br_hf_list:
                 claim_queryset_by_br_hf = Claim.objects.filter(
@@ -202,14 +204,16 @@
         if len(products) > 0:
             product = max(products, key=operator.attrgetter('id'))
             bill = ClaimsToBillConverter.to_bill_obj(claims=instance, product=product)
             bill_line_items = []
             for claim in instance.all():
                 bill_line_item = ClaimToBillItemConverter.to_bill_line_item_obj(claim=claim)
                 bill_line_items.append(bill_line_item)
+                ClaimsToBillConverter.build_amounts(bill_line_item, bill)
+            
             return {
                 'bill_data': bill,
                 'bill_data_line': bill_line_items,
                 'type_conversion': 'claims queryset-bill'
             }
 
     @classmethod
```

### Comparing `openimis-be-calcrule-third_party_payment-1.6.0/calcrule_third_party_payment/config.py` & `openimis_be_calcrule_third_party_payment-1.7.0/calcrule_third_party_payment/config.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule-third_party_payment-1.6.0/calcrule_third_party_payment/converters/claim_to_bill_item.py` & `openimis_be_calcrule_third_party_payment-1.7.0/calcrule_third_party_payment/converters/claim_to_bill_item.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,29 +60,29 @@
 
     @classmethod
     def build_quantity(cls, bill_line_item):
         bill_line_item["quantity"] = 1
 
     @classmethod
     def build_unit_price(cls, bill_line_item, claim):
-        bill_line_item["unit_price"] = claim.claimed
+        bill_line_item["unit_price"] = claim.claimed or claim.remunerated
 
     @classmethod
     def build_discount(cls, bill_line_item, claim):
-        if claim.claimed and claim.approved:
-            if claim.claimed >= claim.approved:
-                bill_line_item["deduction"] = claim.claimed - claim.approved
+        if claim.claimed and claim.remunerated:
+            if claim.claimed != claim.remunerated:
+                bill_line_item["deduction"] = claim.claimed - claim.remunerated
 
     @classmethod
     def build_tax(cls, bill_line_item):
         bill_line_item["tax_rate"] = None
         bill_line_item["tax_analysis"] = None
 
     @classmethod
     def build_amounts(cls, bill_line_item):
         if bill_line_item["unit_price"]:
             bill_line_item["amount_net"] = bill_line_item["quantity"] * bill_line_item["unit_price"]
         else:
             bill_line_item["amount_net"] = 0
-        if "discount" in bill_line_item:
+        if "deduction" in bill_line_item:
             bill_line_item["amount_net"] = bill_line_item["amount_net"] - bill_line_item["deduction"]
         bill_line_item["amount_total"] = bill_line_item["amount_net"]
```

### Comparing `openimis-be-calcrule-third_party_payment-1.6.0/calcrule_third_party_payment/converters/claims_to_bill.py` & `openimis_be_calcrule_third_party_payment-1.7.0/calcrule_third_party_payment/converters/claims_to_bill.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,14 +17,15 @@
         cls.build_thirdparty(health_facility, bill)
         cls.build_code(health_facility, product, batch_run, bill)
         cls.build_date_dates(batch_run, bill)
         #cls.build_tax_analysis(bill)
         cls.build_currency(bill)
         cls.build_status(bill)
         cls.build_terms(product, bill)
+        cls.build_init_amounts(bill)
         return bill
 
     @classmethod
     def build_subject(cls, batch_run, bill):
         bill["subject_id"] = batch_run.id
         bill['subject_type'] = ContentType.objects.get_for_model(batch_run)
 
@@ -65,10 +66,21 @@
 
     @classmethod
     def build_terms(cls, product, bill):
         bill["terms"] = product.name
 
     @classmethod
     def build_amounts(cls, line_item, bill_update):
-        bill_update["amount_net"] = line_item["amount_net"]
-        bill_update["amount_total"] = line_item["amount_total"]
-        bill_update["amount_discount"] = 0 if line_item["discount"] else line_item["discount"]
+        
+        bill_update["amount_net"] += line_item["amount_net"]
+        bill_update["amount_total"] += line_item["amount_total"]
+        #bill_update["amount_discount"] += 0 if "discount" in  line_item or not line_item["discount"] else line_item["discount"]
+        #bill_update["amount_deduction"] += 0 if "deduction" in  line_item or not line_item["deduction"] else line_item["deduction"]
+        
+    @classmethod
+    def build_init_amounts(cls, bill_update):
+        
+        bill_update["amount_net"] = 0
+        bill_update["amount_total"] = 0
+        #bill_update["amount_discount"] += 0 if "discount" in  line_item or not line_item["discount"] else line_item["discount"]
+        #bill_update["amount_deduction"] += 0 if "deduction" in  line_item or not line_item["deduction"] else line_item["deduction"]
+
```

### Comparing `openimis-be-calcrule-third_party_payment-1.6.0/calcrule_third_party_payment/tests.py` & `openimis_be_calcrule_third_party_payment-1.7.0/calcrule_third_party_payment/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import calendar
 import datetime
 import decimal
 
-from claim.gql_mutations import validate_and_process_dedrem_claim
+from claim.services import submit_claim, validate_and_process_dedrem_claim
 from claim.models import (
     ClaimDedRem,
     Claim
 )
 from claim.test_helpers import (
     create_test_claim,
     create_test_claimservice,
@@ -170,34 +170,36 @@
             claim1, custom_props={"price_asked": 100, "service_id": service.id, "qty_provided": 2,
                                   "price_origin": ProductItemOrService.ORIGIN_RELATIVE}
         )
         item1 = create_test_claimitem(
             claim1, "A", custom_props={"price_asked": 100, "item_id": item.id, "qty_provided": 3,
                                        "price_origin": ProductItemOrService.ORIGIN_RELATIVE}
         )
-        errors = validate_and_process_dedrem_claim(claim1, self.user, True)
-        _, days_in_month = calendar.monthrange(claim1.validity_from.year, claim1.validity_from.month)
-        # add process stamp for claim to not use the process_stamp with now()
-        claim1.process_stamp = datetime.datetime(claim1.validity_from.year, claim1.validity_from.month,
-                                                 days_in_month - 1)
-        claim1.save()
+        claim1.refresh_from_db()
 
+        class DummyUser:
+            def __init__(self):
+                self.id_for_audit = 1
+        errors = submit_claim(claim1,DummyUser() )
+        errors += validate_and_process_dedrem_claim(claim1, DummyUser(), True)
+        claim1.process_stamp = claim1.validity_from
+        claim1.save()
         self.assertEqual(len(errors), 0)
         self.assertEqual(
             claim1.status,
             Claim.STATUS_PROCESSED,
             "The claim has relative pricing, so should go to PROCESSED rather than VALUATED",
         )
         # Make sure that the dedrem was generated
         dedrem = ClaimDedRem.objects.filter(claim=claim1).first()
         self.assertIsNotNone(dedrem)
         self.assertEquals(dedrem.rem_g, 500)  # 100*2 + 100*3
         # renumerated should be Null
         self.assertEqual(claim1.remunerated, None)
-
+        days_in_month = calendar.monthrange(claim1.validity_from.year, claim1.validity_from.month)[1]
         # When
         end_date = datetime.datetime(claim1.validity_from.year, claim1.validity_from.month, days_in_month)
         batch_run = do_process_batch(
             self.user.id_for_audit,
             test_region.id,
             end_date
         )
@@ -209,16 +211,16 @@
         self.assertNotEqual(item1.price_valuated, item1.price_adjusted)
         self.assertNotEqual(service1.price_valuated, service1.price_adjusted)
         # based on calculation - should be 201.15 per item and service
         # therefore renumerated = 402.30
         self.assertEqual(item1.price_valuated, decimal.Decimal('201.15'))
         self.assertEqual(service1.price_valuated, decimal.Decimal('201.15'))
         self.assertEqual(claim1.remunerated, service1.price_valuated + item1.price_valuated)
-        self.assertNotEqual(Bill.objects.get(subject_id=batch_run.id), None)
-        self.assertNotEqual(BillItem.objects.get(bill__subject_id=batch_run.id), None)
+        self.assertNotEqual(Bill.objects.filter(subject_id=batch_run.id).first(), None)
+        self.assertNotEqual(BillItem.objects.filter(bill__subject_id=batch_run.id).first(), None)
 
         # tearDown
         # dedrem.delete() # already done if the test passed
         premium.delete()
         payer.delete()
         delete_claim_with_itemsvc_dedrem_and_history(claim1)
         policy.insuree_policies.first().delete()
```

### Comparing `openimis-be-calcrule-third_party_payment-1.6.0/calcrule_third_party_payment/utils.py` & `openimis_be_calcrule_third_party_payment-1.7.0/calcrule_third_party_payment/utils.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule-third_party_payment-1.6.0/openimis_be_calcrule_third_party_payment.egg-info/PKG-INFO` & `openimis_be_calcrule_third_party_payment-1.7.0/openimis_be_calcrule_third_party_payment.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: openimis-be-calcrule-third-party-payment
-Version: 1.6.0
+Name: openimis-be-calcrule-third_party_payment
+Version: 1.7.0
 Summary: The openIMIS Backend calculation rule thirdparty payment reference module.
 Home-page: https://openimis.org/
 Author: Seweryn Niedzielski
 Author-email: sniedzielski@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-calcrule-third_party_payment-1.6.0/openimis_be_calcrule_third_party_payment.egg-info/SOURCES.txt` & `openimis_be_calcrule_third_party_payment-1.7.0/openimis_be_calcrule_third_party_payment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule-third_party_payment-1.6.0/setup.py` & `openimis_be_calcrule_third_party_payment-1.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-calcrule-third_party_payment',
-    version='v1.6.0',
+    version='v1.7.0',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend calculation rule thirdparty payment reference module.',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://openimis.org/',
```

