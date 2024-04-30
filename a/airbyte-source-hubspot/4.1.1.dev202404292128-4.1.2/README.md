# Comparing `tmp/airbyte_source_hubspot-4.1.1.dev202404292128.tar.gz` & `tmp/airbyte_source_hubspot-4.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_hubspot-4.1.1.dev202404292128.tar", max compression
+gzip compressed data, was "airbyte_source_hubspot-4.1.2.tar", max compression
```

## Comparing `airbyte_source_hubspot-4.1.1.dev202404292128.tar` & `airbyte_source_hubspot-4.1.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     4514 2024-04-29 21:23:44.491945 airbyte_source_hubspot-4.1.1.dev202404292128/README.md
--rw-r--r--   0        0        0      812 2024-04-29 21:28:56.714663 airbyte_source_hubspot-4.1.1.dev202404292128/pyproject.toml
--rw-r--r--   0        0        0      124 2024-04-29 21:23:44.495945 airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/__init__.py
--rw-r--r--   0        0        0      154 2024-04-29 21:23:44.495945 airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/constants.py
--rw-r--r--   0        0        0     1885 2024-04-29 21:23:44.495945 airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/errors.py
--rw-r--r--   0        0        0     3809 2024-04-29 21:23:44.495945 airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/helpers.py
--rw-r--r--   0        0        0      233 2024-04-29 21:23:44.495945 airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/run.py
--rw-r--r--   0        0        0     3343 2024-04-29 21:23:44.495945 airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/schemas/campaigns.json
--rw-r--r--   0        0        0      506 2024-04-29 21:23:44.495945 airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/schemas/companies.json
--rw-r--r--   0        0        0      693 2024-04-29 21:23:44.495945 airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/schemas/companies_property_history.json
--rw-r--r--   0        0        0     3054 2024-04-29 21:23:44.495945 airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/schemas/contact_lists.json
--rw-r--r--   0        0        0      517 2024-04-29 21:23:44.495945 airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/schemas/contacts.json
--rw-r--r--   0        0        0      908 2024-04-29 21:23:44.495945 airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/schemas/contacts_form_submissions.json
--rw-r--r--   0        0        0      471 2024-04-29 21:23:44.495945 airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/schemas/contacts_list_memberships.json
--rw-r--r--   0        0        0     3293 2024-04-29 21:23:44.495945 airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/schemas/contacts_merged_audit.json
--rw-r--r--   0        0        0      986 2024-04-29 21:23:44.495945 airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/schemas/contacts_property_history.json
--rw-r--r--   0        0        0     1553 2024-04-29 21:23:44.495945 airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/schemas/deal_pipelines.json
--rw-r--r--   0        0        0    18485 2024-04-29 21:23:44.495945 airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/schemas/deals.json
--rw-r--r--   0        0        0    18562 2024-04-29 21:23:44.495945 airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/schemas/deals_archived.json
--rw-r--r--   0        0        0      690 2024-04-29 21:23:44.495945 airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/schemas/deals_property_history.json
--rw-r--r--   0        0        0     4792 2024-04-29 21:23:44.495945 airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/schemas/email_events.json
--rw-r--r--   0        0        0      784 2024-04-29 21:23:44.495945 airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/schemas/email_subscriptions.json
--rw-r--r--   0        0        0    18307 2024-04-29 21:23:44.495945 airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/schemas/engagements.json
--rw-r--r--   0        0        0    10057 2024-04-29 21:23:44.495945 airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/schemas/engagements_calls.json
--rw-r--r--   0        0        0    14599 2024-04-29 21:23:44.495945 airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/schemas/engagements_emails.json
--rw-r--r--   0        0        0     9913 2024-04-29 21:23:44.495945 airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/schemas/engagements_meetings.json
--rw-r--r--   0        0        0     6592 2024-04-29 21:23:44.495945 airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/schemas/engagements_notes.json
--rw-r--r--   0        0        0    11391 2024-04-29 21:23:44.495945 airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/schemas/engagements_tasks.json
--rw-r--r--   0        0        0     3087 2024-04-29 21:23:44.495945 airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/schemas/feedback_submissions.json
--rw-r--r--   0        0        0      710 2024-04-29 21:23:44.495945 airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/schemas/form_submissions.json
--rw-r--r--   0        0        0     5053 2024-04-29 21:23:44.495945 airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/schemas/forms.json
--rw-r--r--   0        0        0     2217 2024-04-29 21:23:44.495945 airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/schemas/goals.json
--rw-r--r--   0        0        0      398 2024-04-29 21:23:44.495945 airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/schemas/line_items.json
--rw-r--r--   0        0        0    18730 2024-04-29 21:23:44.495945 airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/schemas/marketing_emails.json
--rw-r--r--   0        0        0      986 2024-04-29 21:23:44.495945 airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/schemas/owners.json
--rw-r--r--   0        0        0      986 2024-04-29 21:23:44.495945 airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/schemas/owners_archived.json
--rw-r--r--   0        0        0      398 2024-04-29 21:23:44.495945 airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/schemas/products.json
--rw-r--r--   0        0        0     3742 2024-04-29 21:23:44.495945 airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/schemas/shared/default_event_properties.json
--rw-r--r--   0        0        0     1264 2024-04-29 21:23:44.495945 airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/schemas/subscription_changes.json
--rw-r--r--   0        0        0     1647 2024-04-29 21:23:44.495945 airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/schemas/ticket_pipelines.json
--rw-r--r--   0        0        0      751 2024-04-29 21:23:44.495945 airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/schemas/tickets.json
--rw-r--r--   0        0        0     3905 2024-04-29 21:23:44.495945 airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/schemas/workflows.json
--rw-r--r--   0        0        0     9781 2024-04-29 21:23:44.495945 airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/source.py
--rw-r--r--   0        0        0     4559 2024-04-29 21:23:44.495945 airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/spec.yaml
--rw-r--r--   0        0        0    99368 2024-04-29 21:23:44.495945 airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/streams.py
--rw-r--r--   0        0        0     5234 1970-01-01 00:00:00.000000 airbyte_source_hubspot-4.1.1.dev202404292128/PKG-INFO
+-rw-r--r--   0        0        0     4514 2024-04-30 13:49:46.239723 airbyte_source_hubspot-4.1.2/README.md
+-rw-r--r--   0        0        0      796 2024-04-30 13:53:39.845750 airbyte_source_hubspot-4.1.2/pyproject.toml
+-rw-r--r--   0        0        0      124 2024-04-30 13:49:46.243723 airbyte_source_hubspot-4.1.2/source_hubspot/__init__.py
+-rw-r--r--   0        0        0      154 2024-04-30 13:49:46.243723 airbyte_source_hubspot-4.1.2/source_hubspot/constants.py
+-rw-r--r--   0        0        0     1885 2024-04-30 13:49:46.243723 airbyte_source_hubspot-4.1.2/source_hubspot/errors.py
+-rw-r--r--   0        0        0     3809 2024-04-30 13:49:46.243723 airbyte_source_hubspot-4.1.2/source_hubspot/helpers.py
+-rw-r--r--   0        0        0      233 2024-04-30 13:49:46.243723 airbyte_source_hubspot-4.1.2/source_hubspot/run.py
+-rw-r--r--   0        0        0     6624 2024-04-30 13:49:46.243723 airbyte_source_hubspot-4.1.2/source_hubspot/schemas/campaigns.json
+-rw-r--r--   0        0        0      905 2024-04-30 13:49:46.243723 airbyte_source_hubspot-4.1.2/source_hubspot/schemas/companies.json
+-rw-r--r--   0        0        0     1415 2024-04-30 13:49:46.243723 airbyte_source_hubspot-4.1.2/source_hubspot/schemas/companies_property_history.json
+-rw-r--r--   0        0        0     6086 2024-04-30 13:49:46.243723 airbyte_source_hubspot-4.1.2/source_hubspot/schemas/contact_lists.json
+-rw-r--r--   0        0        0      933 2024-04-30 13:49:46.243723 airbyte_source_hubspot-4.1.2/source_hubspot/schemas/contacts.json
+-rw-r--r--   0        0        0     1866 2024-04-30 13:49:46.243723 airbyte_source_hubspot-4.1.2/source_hubspot/schemas/contacts_form_submissions.json
+-rw-r--r--   0        0        0     1008 2024-04-30 13:49:46.243723 airbyte_source_hubspot-4.1.2/source_hubspot/schemas/contacts_list_memberships.json
+-rw-r--r--   0        0        0     6620 2024-04-30 13:49:46.243723 airbyte_source_hubspot-4.1.2/source_hubspot/schemas/contacts_merged_audit.json
+-rw-r--r--   0        0        0     2093 2024-04-30 13:49:46.243723 airbyte_source_hubspot-4.1.2/source_hubspot/schemas/contacts_property_history.json
+-rw-r--r--   0        0        0     3046 2024-04-30 13:49:46.243723 airbyte_source_hubspot-4.1.2/source_hubspot/schemas/deal_pipelines.json
+-rw-r--r--   0        0        0    30732 2024-04-30 13:49:46.243723 airbyte_source_hubspot-4.1.2/source_hubspot/schemas/deals.json
+-rw-r--r--   0        0        0    18631 2024-04-30 13:49:46.243723 airbyte_source_hubspot-4.1.2/source_hubspot/schemas/deals_archived.json
+-rw-r--r--   0        0        0     1276 2024-04-30 13:49:46.243723 airbyte_source_hubspot-4.1.2/source_hubspot/schemas/deals_property_history.json
+-rw-r--r--   0        0        0     9554 2024-04-30 13:49:46.243723 airbyte_source_hubspot-4.1.2/source_hubspot/schemas/email_events.json
+-rw-r--r--   0        0        0     1670 2024-04-30 13:49:46.243723 airbyte_source_hubspot-4.1.2/source_hubspot/schemas/email_subscriptions.json
+-rw-r--r--   0        0        0    26695 2024-04-30 13:49:46.243723 airbyte_source_hubspot-4.1.2/source_hubspot/schemas/engagements.json
+-rw-r--r--   0        0        0    18505 2024-04-30 13:49:46.243723 airbyte_source_hubspot-4.1.2/source_hubspot/schemas/engagements_calls.json
+-rw-r--r--   0        0        0    25799 2024-04-30 13:49:46.243723 airbyte_source_hubspot-4.1.2/source_hubspot/schemas/engagements_emails.json
+-rw-r--r--   0        0        0    17798 2024-04-30 13:49:46.243723 airbyte_source_hubspot-4.1.2/source_hubspot/schemas/engagements_meetings.json
+-rw-r--r--   0        0        0    11074 2024-04-30 13:49:46.243723 airbyte_source_hubspot-4.1.2/source_hubspot/schemas/engagements_notes.json
+-rw-r--r--   0        0        0    20314 2024-04-30 13:49:46.243723 airbyte_source_hubspot-4.1.2/source_hubspot/schemas/engagements_tasks.json
+-rw-r--r--   0        0        0     5736 2024-04-30 13:49:46.243723 airbyte_source_hubspot-4.1.2/source_hubspot/schemas/feedback_submissions.json
+-rw-r--r--   0        0        0     1332 2024-04-30 13:49:46.243723 airbyte_source_hubspot-4.1.2/source_hubspot/schemas/form_submissions.json
+-rw-r--r--   0        0        0     8454 2024-04-30 13:49:46.243723 airbyte_source_hubspot-4.1.2/source_hubspot/schemas/forms.json
+-rw-r--r--   0        0        0     3717 2024-04-30 13:49:46.243723 airbyte_source_hubspot-4.1.2/source_hubspot/schemas/goals.json
+-rw-r--r--   0        0        0      692 2024-04-30 13:49:46.243723 airbyte_source_hubspot-4.1.2/source_hubspot/schemas/line_items.json
+-rw-r--r--   0        0        0    24533 2024-04-30 13:49:46.243723 airbyte_source_hubspot-4.1.2/source_hubspot/schemas/marketing_emails.json
+-rw-r--r--   0        0        0     1763 2024-04-30 13:49:46.243723 airbyte_source_hubspot-4.1.2/source_hubspot/schemas/owners.json
+-rw-r--r--   0        0        0     1733 2024-04-30 13:49:46.243723 airbyte_source_hubspot-4.1.2/source_hubspot/schemas/owners_archived.json
+-rw-r--r--   0        0        0      676 2024-04-30 13:49:46.243723 airbyte_source_hubspot-4.1.2/source_hubspot/schemas/products.json
+-rw-r--r--   0        0        0     3742 2024-04-30 13:49:46.243723 airbyte_source_hubspot-4.1.2/source_hubspot/schemas/shared/default_event_properties.json
+-rw-r--r--   0        0        0     2414 2024-04-30 13:49:46.243723 airbyte_source_hubspot-4.1.2/source_hubspot/schemas/subscription_changes.json
+-rw-r--r--   0        0        0     2976 2024-04-30 13:49:46.243723 airbyte_source_hubspot-4.1.2/source_hubspot/schemas/ticket_pipelines.json
+-rw-r--r--   0        0        0     1304 2024-04-30 13:49:46.243723 airbyte_source_hubspot-4.1.2/source_hubspot/schemas/tickets.json
+-rw-r--r--   0        0        0     7534 2024-04-30 13:49:46.243723 airbyte_source_hubspot-4.1.2/source_hubspot/schemas/workflows.json
+-rw-r--r--   0        0        0     9781 2024-04-30 13:49:46.243723 airbyte_source_hubspot-4.1.2/source_hubspot/source.py
+-rw-r--r--   0        0        0     4559 2024-04-30 13:49:46.243723 airbyte_source_hubspot-4.1.2/source_hubspot/spec.yaml
+-rw-r--r--   0        0        0    96417 2024-04-30 13:49:46.243723 airbyte_source_hubspot-4.1.2/source_hubspot/streams.py
+-rw-r--r--   0        0        0     5218 1970-01-01 00:00:00.000000 airbyte_source_hubspot-4.1.2/PKG-INFO
```

### Comparing `airbyte_source_hubspot-4.1.1.dev202404292128/README.md` & `airbyte_source_hubspot-4.1.2/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.1.dev202404292128/pyproject.toml` & `airbyte_source_hubspot-4.1.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "4.1.1.dev202404292128"
+version = "4.1.2"
 name = "airbyte-source-hubspot"
 description = "Source implementation for HubSpot."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "ELv2"
 readme = "README.md"
```

### Comparing `airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/errors.py` & `airbyte_source_hubspot-4.1.2/source_hubspot/errors.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/helpers.py` & `airbyte_source_hubspot-4.1.2/source_hubspot/helpers.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/schemas/campaigns.json` & `airbyte_source_hubspot-4.1.2/source_hubspot/schemas/shared/default_event_properties.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6263020833333334%*

 * *Differences: {"'additionalProperties'": 'True',*

 * * "'properties'": "{'id': {'type': {insert: [(1, 'string')], delete: [1]}}, "*

 * *                 "'properties_hs_asset_description': OrderedDict([('type', ['null', 'string'])]), "*

 * *                 "'properties_hs_asset_type': OrderedDict([('type', ['null', 'string'])]), "*

 * *                 "'properties_hs_browser': OrderedDict([('type', ['null', 'string'])]), "*

 * *                 "'properties_hs_campaign_id': OrderedDict([('type', ['null', 'string'])]), "*

 * *                 "'prop […]*

```diff
@@ -1,295 +1,301 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
+    "additionalProperties": true,
     "properties": {
-        "appId": {
+        "eventType": {
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "appName": {
+        "id": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "contentId": {
+        "objectId": {
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "counters": {
-            "properties": {
-                "bounce": {
-                    "type": [
-                        "null",
-                        "integer"
-                    ]
-                },
-                "click": {
-                    "type": [
-                        "null",
-                        "integer"
-                    ]
-                },
-                "deferred": {
-                    "type": [
-                        "null",
-                        "integer"
-                    ]
-                },
-                "delivered": {
-                    "type": [
-                        "null",
-                        "integer"
-                    ]
-                },
-                "dropped": {
-                    "type": [
-                        "null",
-                        "integer"
-                    ]
-                },
-                "forward": {
-                    "type": [
-                        "null",
-                        "integer"
-                    ]
-                },
-                "mta_dropped": {
-                    "type": [
-                        "null",
-                        "integer"
-                    ]
-                },
-                "open": {
-                    "type": [
-                        "null",
-                        "integer"
-                    ]
-                },
-                "print": {
-                    "type": [
-                        "null",
-                        "integer"
-                    ]
-                },
-                "processed": {
-                    "type": [
-                        "null",
-                        "integer"
-                    ]
-                },
-                "reply": {
-                    "type": [
-                        "null",
-                        "integer"
-                    ]
-                },
-                "sent": {
-                    "type": [
-                        "null",
-                        "integer"
-                    ]
-                },
-                "spamreport": {
-                    "type": [
-                        "null",
-                        "integer"
-                    ]
-                },
-                "statuschange": {
-                    "type": [
-                        "null",
-                        "integer"
-                    ]
-                },
-                "suppressed": {
-                    "type": [
-                        "null",
-                        "integer"
-                    ]
-                },
-                "unsubscribed": {
-                    "type": [
-                        "null",
-                        "integer"
-                    ]
-                }
-            },
+        "objectType": {
             "type": [
                 "null",
-                "object"
+                "string"
             ]
         },
-        "counters_bounce": {
+        "occurredAt": {
+            "format": "date-time",
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "counters_click": {
+        "properties_hs_asset_description": {
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "counters_deferred": {
+        "properties_hs_asset_type": {
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "counters_delivered": {
+        "properties_hs_base_url": {
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "counters_dropped": {
+        "properties_hs_browser": {
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "counters_forward": {
+        "properties_hs_campaign_id": {
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "counters_mta_dropped": {
+        "properties_hs_city": {
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "counters_open": {
+        "properties_hs_country": {
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "counters_print": {
+        "properties_hs_device_name": {
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "counters_processed": {
+        "properties_hs_device_type": {
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "counters_reply": {
+        "properties_hs_document_id": {
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "counters_sent": {
+        "properties_hs_element_class": {
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "counters_spamreport": {
+        "properties_hs_element_id": {
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "counters_statuschange": {
+        "properties_hs_element_text": {
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "counters_suppressed": {
+        "properties_hs_form_correlation_id": {
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "counters_unsubscribed": {
+        "properties_hs_form_id": {
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "id": {
+        "properties_hs_form_type": {
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "lastProcessingFinishedAt": {
+        "properties_hs_language": {
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "lastProcessingStartedAt": {
+        "properties_hs_link_href": {
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "lastProcessingStateChangeAt": {
+        "properties_hs_operating_system": {
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "lastUpdatedTime": {
+        "properties_hs_operating_version": {
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "name": {
+        "properties_hs_page_content_type": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "numIncluded": {
+        "properties_hs_page_id": {
             "type": [
                 "null",
-                "integer"
+                "string"
+            ]
+        },
+        "properties_hs_page_title": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "properties_hs_page_url": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "properties_hs_parent_module_id": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "properties_hs_presentation_id": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "properties_hs_referrer": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "properties_hs_region": {
+            "type": [
+                "null",
+                "string"
             ]
         },
-        "numQueued": {
+        "properties_hs_screen_height": {
             "type": [
                 "null",
-                "integer"
+                "string"
+            ]
+        },
+        "properties_hs_screen_width": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "properties_hs_title": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "properties_hs_touchpoint_source": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "properties_hs_tracking_name": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "properties_hs_url": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "properties_hs_url_domain": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "properties_hs_url_path": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "properties_hs_user_agent": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "properties_hs_user_id": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "properties_hs_utm_campaign": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "properties_hs_utm_content": {
+            "type": [
+                "null",
+                "string"
             ]
         },
-        "processingState": {
+        "properties_hs_utm_medium": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "subType": {
+        "properties_hs_utm_source": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "subject": {
+        "properties_hs_utm_term": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "type": {
+        "properties_hs_visitor_type": {
             "type": [
                 "null",
                 "string"
             ]
         }
     },
     "type": [
```

### Comparing `airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/schemas/contacts_form_submissions.json` & `airbyte_source_hubspot-4.1.2/source_hubspot/schemas/companies_property_history.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.3788377192982456%*

 * *Differences: {"'$schema'": "'http://json-schema.org/draft-07/schema'",*

 * * "'additionalProperties'": 'True',*

 * * "'properties'": "{'timestamp': {'type': {insert: [(1, 'string')], delete: [1]}, 'description': "*

 * *                 "'The date and time when the property update occurred.', 'format': 'date-time', "*

 * *                 "'airbyte_type': 'timestamp_with_timezone'}, 'updatedByUserId': "*

 * *                 "OrderedDict([('description', 'The user ID of the user who initiated the property "*

 * *                 "update.'), ('type',  […]*

```diff
@@ -1,85 +1,68 @@
 {
-    "$schema": "http://json-schema.org/draft-07/schema#",
+    "$schema": "http://json-schema.org/draft-07/schema",
+    "additionalProperties": true,
     "properties": {
-        "canonical-url": {
+        "archived": {
+            "description": "Flag indicating if the company property history record is archived or not.",
             "type": [
                 "null",
-                "string"
-            ]
-        },
-        "canonical-vid": {
-            "type": [
-                "null",
-                "integer"
+                "boolean"
             ]
         },
-        "contact-associated-by": {
-            "items": {
-                "type": [
-                    "null",
-                    "string"
-                ]
-            },
-            "type": [
-                "null",
-                "array"
-            ]
-        },
-        "conversion-id": {
+        "companyId": {
+            "description": "The unique identifier of the company to which the property history record belongs.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "form-id": {
+        "property": {
+            "description": "The specific property that was updated in the company record.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "form-type": {
+        "sourceId": {
+            "description": "The identifier of the source that updated the property in the company record.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "meta-data": {
-            "items": {},
-            "type": [
-                "null",
-                "array"
-            ]
-        },
-        "page-title": {
+        "sourceType": {
+            "description": "The type of the source that updated the property in the company record.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "page-url": {
+        "timestamp": {
+            "airbyte_type": "timestamp_with_timezone",
+            "description": "The date and time when the property update occurred.",
+            "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "portal-id": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "timestamp": {
+        "updatedByUserId": {
+            "description": "The user ID of the user who initiated the property update.",
             "type": [
                 "null",
-                "integer"
+                "number"
             ]
         },
-        "title": {
+        "value": {
+            "description": "The new value of the property after the update.",
             "type": [
                 "null",
                 "string"
             ]
         }
     },
-    "type": "object"
+    "type": [
+        "null",
+        "object"
+    ]
 }
```

### Comparing `airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/schemas/deal_pipelines.json` & `airbyte_source_hubspot-4.1.2/source_hubspot/schemas/subscription_changes.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333333333333334%*

 * *Differences: {"'properties'": "{replace: OrderedDict([('timestamp', OrderedDict([('description', 'Timestamp "*

 * *                 "when the subscription change data was fetched'), ('type', ['null', "*

 * *                 "'integer'])])), ('portalId', OrderedDict([('description', 'ID of the portal "*

 * *                 "related to the subscription changes'), ('type', ['null', 'integer'])])), "*

 * *                 "('recipient', OrderedDict([('description', 'Recipient of the subscription change "*

 * *                 "notification'), ('ty […]*

```diff
@@ -1,112 +1,75 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
     "properties": {
-        "active": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
-        "createdAt": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "default": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
-        "displayOrder": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "label": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "objectType": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "objectTypeId": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "pipelineId": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "stages": {
+        "changes": {
+            "description": "List of all subscription changes",
             "items": {
+                "description": "Details of each subscription change",
                 "properties": {
-                    "active": {
+                    "causedByEvent": {
+                        "description": "Event that triggered the subscription change",
+                        "properties": {
+                            "created": {
+                                "description": "Timestamp when the event that caused the change occurred",
+                                "type": [
+                                    "null",
+                                    "integer"
+                                ]
+                            },
+                            "id": {
+                                "description": "Unique identifier for the event that caused the change",
+                                "type": [
+                                    "null",
+                                    "string"
+                                ]
+                            }
+                        },
                         "type": [
                             "null",
-                            "boolean"
+                            "object"
                         ]
                     },
-                    "createdAt": {
+                    "change": {
+                        "description": "Details of the change that occurred",
                         "type": [
                             "null",
-                            "integer"
+                            "string"
                         ]
                     },
-                    "displayOrder": {
+                    "changeType": {
+                        "description": "Type of change (e.g., add, remove, update)",
                         "type": [
                             "null",
-                            "integer"
+                            "string"
                         ]
                     },
-                    "label": {
+                    "portalId": {
+                        "description": "ID of the portal associated with the subscription change",
                         "type": [
                             "null",
-                            "string"
+                            "integer"
                         ]
                     },
-                    "metadata": {
-                        "properties": {
-                            "isClosed": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "probability": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            }
-                        },
+                    "source": {
+                        "description": "Source of the subscription change",
                         "type": [
                             "null",
-                            "object"
+                            "string"
                         ]
                     },
-                    "stageId": {
+                    "subscriptionId": {
+                        "description": "Unique identifier for the subscription affected by the change",
                         "type": [
                             "null",
-                            "string"
+                            "integer"
                         ]
                     },
-                    "updatedAt": {
+                    "timestamp": {
+                        "description": "Timestamp when the subscription change occurred",
                         "type": [
                             "null",
                             "integer"
                         ]
                     }
                 },
                 "type": [
@@ -115,15 +78,37 @@
                 ]
             },
             "type": [
                 "null",
                 "array"
             ]
         },
-        "updatedAt": {
+        "normalizedEmailId": {
+            "description": "Normalized email identifier associated with the subscription",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "portalId": {
+            "description": "ID of the portal related to the subscription changes",
+            "type": [
+                "null",
+                "integer"
+            ]
+        },
+        "recipient": {
+            "description": "Recipient of the subscription change notification",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "timestamp": {
+            "description": "Timestamp when the subscription change data was fetched",
             "type": [
                 "null",
                 "integer"
             ]
         }
     },
     "type": [
```

### Comparing `airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/schemas/deals.json` & `airbyte_source_hubspot-4.1.2/source_hubspot/schemas/deals_archived.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.996761602286029%*

 * *Differences: {"'properties'": "{'properties': {'properties': {'hs_is_closed': {'type': {insert: [(1, "*

 * *                 "'string')], delete: [1]}}, 'hs_is_closed_won': {'type': {insert: [(1, "*

 * *                 "'string')], delete: [1]}}, "*

 * *                 "'hs_line_item_global_term_hs_discount_percentage_enabled': {'type': {insert: "*

 * *                 "[(1, 'string')], delete: [1]}}, "*

 * *                 "'hs_line_item_global_term_hs_recurring_billing_period_enabled': {'type': "*

 * *                 "{insert: [(1, 'string')], […]*

```diff
@@ -3,14 +3,22 @@
     "properties": {
         "archived": {
             "type": [
                 "null",
                 "boolean"
             ]
         },
+        "archivedAt": {
+            "description": "The date and time when the deal was archived",
+            "format": "date-time",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
         "companies": {
             "items": {
                 "type": [
                     "null",
                     "string"
                 ]
             },
@@ -394,21 +402,21 @@
                         "null",
                         "string"
                     ]
                 },
                 "hs_is_closed": {
                     "type": [
                         "null",
-                        "boolean"
+                        "string"
                     ]
                 },
                 "hs_is_closed_won": {
                     "type": [
                         "null",
-                        "boolean"
+                        "string"
                     ]
                 },
                 "hs_lastmodifieddate": {
                     "format": "date-time",
                     "type": [
                         "null",
                         "string"
@@ -431,51 +439,51 @@
                         "null",
                         "string"
                     ]
                 },
                 "hs_line_item_global_term_hs_discount_percentage_enabled": {
                     "type": [
                         "null",
-                        "boolean"
+                        "string"
                     ]
                 },
                 "hs_line_item_global_term_hs_recurring_billing_period": {
                     "type": [
                         "null",
                         "string"
                     ]
                 },
                 "hs_line_item_global_term_hs_recurring_billing_period_enabled": {
                     "type": [
                         "null",
-                        "boolean"
+                        "string"
                     ]
                 },
                 "hs_line_item_global_term_hs_recurring_billing_start_date": {
                     "type": [
                         "null",
                         "string"
                     ]
                 },
                 "hs_line_item_global_term_hs_recurring_billing_start_date_enabled": {
                     "type": [
                         "null",
-                        "boolean"
+                        "string"
                     ]
                 },
                 "hs_line_item_global_term_recurringbillingfrequency": {
                     "type": [
                         "null",
                         "string"
                     ]
                 },
                 "hs_line_item_global_term_recurringbillingfrequency_enabled": {
                     "type": [
                         "null",
-                        "boolean"
+                        "string"
                     ]
                 },
                 "hs_manual_forecast_category": {
                     "type": [
                         "null",
                         "string"
                     ]
@@ -985,21 +993,21 @@
                 "null",
                 "string"
             ]
         },
         "properties_hs_is_closed": {
             "type": [
                 "null",
-                "boolean"
+                "string"
             ]
         },
         "properties_hs_is_closed_won": {
             "type": [
                 "null",
-                "boolean"
+                "string"
             ]
         },
         "properties_hs_lastmodifieddate": {
             "format": "date-time",
             "type": [
                 "null",
                 "string"
@@ -1022,51 +1030,51 @@
                 "null",
                 "string"
             ]
         },
         "properties_hs_line_item_global_term_hs_discount_percentage_enabled": {
             "type": [
                 "null",
-                "boolean"
+                "string"
             ]
         },
         "properties_hs_line_item_global_term_hs_recurring_billing_period": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "properties_hs_line_item_global_term_hs_recurring_billing_period_enabled": {
             "type": [
                 "null",
-                "boolean"
+                "string"
             ]
         },
         "properties_hs_line_item_global_term_hs_recurring_billing_start_date": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "properties_hs_line_item_global_term_hs_recurring_billing_start_date_enabled": {
             "type": [
                 "null",
-                "boolean"
+                "string"
             ]
         },
         "properties_hs_line_item_global_term_recurringbillingfrequency": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "properties_hs_line_item_global_term_recurringbillingfrequency_enabled": {
             "type": [
                 "null",
-                "boolean"
+                "string"
             ]
         },
         "properties_hs_manual_forecast_category": {
             "type": [
                 "null",
                 "string"
             ]
```

### Comparing `airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/schemas/deals_archived.json` & `airbyte_source_hubspot-4.1.2/source_hubspot/schemas/marketing_emails.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8351685018351684%*

 * *Differences: {"'properties'": "{'id': {'type': {insert: [(1, 'integer')], delete: [1]}}, 'archivedAt': {'type': "*

 * *                 "{insert: [(1, 'integer')], delete: [1]}, 'description': 'Timestamp when the "*

 * *                 "email was archived', delete: ['format']}, 'ab': OrderedDict([('type', ['null', "*

 * *                 "'boolean'])]), 'abHoursToWait': OrderedDict([('type', ['null', 'integer'])]), "*

 * *                 "'abSampleSizeDefault': OrderedDict([('type', ['null', 'string'])]), "*

 * *                 "'abSamplingD […]*

```diff
@@ -1,1256 +1,1646 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
     "properties": {
-        "archived": {
+        "ab": {
             "type": [
                 "null",
                 "boolean"
             ]
         },
-        "archivedAt": {
-            "format": "date-time",
+        "abHoursToWait": {
+            "type": [
+                "null",
+                "integer"
+            ]
+        },
+        "abSampleSizeDefault": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "companies": {
-            "items": {
-                "type": [
-                    "null",
-                    "string"
-                ]
-            },
+        "abSamplingDefault": {
             "type": [
                 "null",
-                "array"
+                "string"
             ]
         },
-        "contacts": {
-            "items": {
-                "type": [
-                    "null",
-                    "string"
-                ]
-            },
+        "abStatus": {
             "type": [
                 "null",
-                "array"
+                "string"
             ]
         },
-        "createdAt": {
-            "format": "date-time",
+        "abSuccessMetric": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "id": {
+        "abTestPercentage": {
+            "type": [
+                "null",
+                "integer"
+            ]
+        },
+        "abVariation": {
+            "type": [
+                "null",
+                "boolean"
+            ]
+        },
+        "absoluteUrl": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "line_items": {
+        "aifeatures": {
+            "type": [
+                "null",
+                "object"
+            ]
+        },
+        "allEmailCampaignIds": {
             "items": {
                 "type": [
                     "null",
-                    "string"
+                    "integer"
                 ]
             },
             "type": [
                 "null",
                 "array"
             ]
         },
-        "properties": {
-            "properties": {
-                "amount": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "amount_in_home_currency": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "closed_lost_reason": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "closed_won_reason": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "closedate": {
-                    "format": "date-time",
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "createdate": {
-                    "format": "date-time",
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "days_to_close": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "dealname": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "dealstage": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "dealtype": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "description": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "engagements_last_meeting_booked": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "engagements_last_meeting_booked_campaign": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "engagements_last_meeting_booked_medium": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "engagements_last_meeting_booked_source": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_acv": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_all_accessible_team_ids": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_all_assigned_business_unit_ids": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_all_owner_ids": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_all_team_ids": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_analytics_source": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_analytics_source_data_1": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_analytics_source_data_2": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_arr": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_closed_amount": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_closed_amount_in_home_currency": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_created_by_user_id": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_createdate": {
-                    "format": "date-time",
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_date_entered_9567448": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_date_entered_9567449": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_date_entered_appointmentscheduled": {
-                    "format": "date-time",
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_date_entered_closedlost": {
-                    "format": "date-time",
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_date_entered_closedwon": {
-                    "format": "date-time",
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_date_entered_contractsent": {
-                    "format": "date-time",
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_date_entered_customclosedwonstage": {
-                    "format": "date-time",
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_date_entered_decisionmakerboughtin": {
-                    "format": "date-time",
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_date_entered_presentationscheduled": {
-                    "format": "date-time",
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_date_entered_qualifiedtobuy": {
-                    "format": "date-time",
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_date_exited_9567448": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_date_exited_9567449": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_date_exited_appointmentscheduled": {
-                    "format": "date-time",
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_date_exited_closedlost": {
-                    "format": "date-time",
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_date_exited_closedwon": {
-                    "format": "date-time",
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_date_exited_contractsent": {
-                    "format": "date-time",
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_date_exited_customclosedwonstage": {
-                    "format": "date-time",
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_date_exited_decisionmakerboughtin": {
-                    "format": "date-time",
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_date_exited_presentationscheduled": {
-                    "format": "date-time",
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_date_exited_qualifiedtobuy": {
-                    "format": "date-time",
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_deal_amount_calculation_preference": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_deal_stage_probability": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_deal_stage_probability_shadow": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_forecast_amount": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_forecast_probability": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_is_closed": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_is_closed_won": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_lastmodifieddate": {
-                    "format": "date-time",
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_latest_meeting_activity": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_likelihood_to_close": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_line_item_global_term_hs_discount_percentage": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_line_item_global_term_hs_discount_percentage_enabled": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_line_item_global_term_hs_recurring_billing_period": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_line_item_global_term_hs_recurring_billing_period_enabled": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_line_item_global_term_hs_recurring_billing_start_date": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_line_item_global_term_hs_recurring_billing_start_date_enabled": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_line_item_global_term_recurringbillingfrequency": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_line_item_global_term_recurringbillingfrequency_enabled": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_manual_forecast_category": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_merged_object_ids": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_mrr": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_next_step": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_num_target_accounts": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_object_id": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_predicted_amount": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_predicted_amount_in_home_currency": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_priority": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_projected_amount": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_projected_amount_in_home_currency": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_sales_email_last_replied": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_tcv": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_unique_creation_key": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_updated_by_user_id": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_user_ids_of_all_notification_followers": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_user_ids_of_all_notification_unfollowers": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_user_ids_of_all_owners": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hubspot_owner_assigneddate": {
-                    "format": "date-time",
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hubspot_owner_id": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hubspot_team_id": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "notes_last_contacted": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "notes_last_updated": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "notes_next_activity_date": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "num_associated_contacts": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "num_contacted_notes": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "num_notes": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "pipeline": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                }
-            },
+        "analyticsPageId": {
             "type": [
                 "null",
-                "object"
+                "string"
             ]
         },
-        "properties_amount": {
+        "analyticsPageType": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_amount_in_home_currency": {
+        "archived": {
             "type": [
                 "null",
-                "string"
+                "boolean"
             ]
         },
-        "properties_closed_lost_reason": {
+        "archivedAt": {
+            "description": "Timestamp when the email was archived",
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "properties_closed_won_reason": {
+        "archivedInDashboard": {
+            "description": "Flag indicating if the email was archived in the dashboard",
             "type": [
                 "null",
-                "string"
+                "boolean"
             ]
         },
-        "properties_closedate": {
-            "format": "date-time",
+        "audienceAccess": {
+            "description": "Information about who has access to view the email",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_createdate": {
-            "format": "date-time",
+        "author": {
+            "description": "Author of the email",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_days_to_close": {
+        "authorAt": {
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "properties_dealname": {
+        "authorName": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_dealstage": {
+        "authorUserId": {
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "properties_dealtype": {
+        "blogEmailType": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_description": {
+        "blogRssSettings": {
+            "description": "Settings related to blog RSS integration",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_engagements_last_meeting_booked": {
+        "campaign": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_engagements_last_meeting_booked_campaign": {
+        "campaignName": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_engagements_last_meeting_booked_medium": {
+        "campaignUtm": {
+            "description": "UTM parameters for campaign tracking",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_engagements_last_meeting_booked_source": {
+        "canSpamSettingsId": {
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "properties_hs_acv": {
+        "categoryId": {
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "properties_hs_all_accessible_team_ids": {
+        "clonedFrom": {
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "properties_hs_all_assigned_business_unit_ids": {
+        "contentAccessRuleIds": {
+            "items": {
+                "type": [
+                    "null",
+                    "integer"
+                ]
+            },
             "type": [
                 "null",
-                "string"
+                "array"
             ]
         },
-        "properties_hs_all_owner_ids": {
+        "contentAccessRuleTypes": {
+            "items": {
+                "type": [
+                    "null",
+                    "string"
+                ]
+            },
             "type": [
                 "null",
-                "string"
+                "array"
             ]
         },
-        "properties_hs_all_team_ids": {
+        "contentTypeCategory": {
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "properties_hs_analytics_source": {
+        "createPage": {
             "type": [
                 "null",
-                "string"
+                "boolean"
             ]
         },
-        "properties_hs_analytics_source_data_1": {
+        "created": {
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "properties_hs_analytics_source_data_2": {
+        "createdById": {
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "properties_hs_arr": {
+        "currentState": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_hs_closed_amount": {
+        "currentlyPublished": {
             "type": [
                 "null",
-                "string"
+                "boolean"
             ]
         },
-        "properties_hs_closed_amount_in_home_currency": {
+        "customReplyTo": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_hs_created_by_user_id": {
+        "customReplyToEnabled": {
             "type": [
                 "null",
-                "string"
+                "boolean"
             ]
         },
-        "properties_hs_createdate": {
-            "format": "date-time",
+        "domain": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_hs_date_entered_9567448": {
+        "emailBody": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_hs_date_entered_9567449": {
+        "emailCampaignGroupId": {
+            "description": "Group ID associated with the email campaign",
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "properties_hs_date_entered_appointmentscheduled": {
-            "format": "date-time",
+        "emailNote": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_hs_date_entered_closedlost": {
-            "format": "date-time",
+        "emailTemplateMode": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_hs_date_entered_closedwon": {
-            "format": "date-time",
+        "emailType": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_hs_date_entered_contractsent": {
-            "format": "date-time",
+        "emailbodyPlaintext": {
+            "description": "Plain text version of the email body",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_hs_date_entered_customclosedwonstage": {
-            "format": "date-time",
+        "feedbackEmailCategory": {
+            "description": "Category for feedback related to the email",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_hs_date_entered_decisionmakerboughtin": {
-            "format": "date-time",
+        "feedbackSurveyId": {
+            "description": "ID of the feedback survey linked to the email",
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "properties_hs_date_entered_presentationscheduled": {
-            "format": "date-time",
+        "flexAreas": {
+            "properties": {
+                "main": {
+                    "properties": {
+                        "boxed": {
+                            "type": [
+                                "null",
+                                "boolean"
+                            ]
+                        },
+                        "isSingleColumnFullWidth": {
+                            "type": [
+                                "null",
+                                "boolean"
+                            ]
+                        },
+                        "sections": {
+                            "items": {
+                                "properties": {
+                                    "columns": {
+                                        "items": {
+                                            "properties": {
+                                                "id": {
+                                                    "type": [
+                                                        "null",
+                                                        "string"
+                                                    ]
+                                                },
+                                                "widgets": {
+                                                    "items": {
+                                                        "type": [
+                                                            "null",
+                                                            "string"
+                                                        ]
+                                                    },
+                                                    "type": [
+                                                        "null",
+                                                        "array"
+                                                    ]
+                                                },
+                                                "width": {
+                                                    "type": [
+                                                        "null",
+                                                        "integer"
+                                                    ]
+                                                }
+                                            },
+                                            "type": [
+                                                "null",
+                                                "object"
+                                            ]
+                                        },
+                                        "type": [
+                                            "null",
+                                            "array"
+                                        ]
+                                    },
+                                    "id": {
+                                        "type": [
+                                            "null",
+                                            "string"
+                                        ]
+                                    },
+                                    "style": {
+                                        "properties": {
+                                            "backgroundColor": {
+                                                "type": [
+                                                    "null",
+                                                    "string"
+                                                ]
+                                            },
+                                            "backgroundType": {
+                                                "type": [
+                                                    "null",
+                                                    "string"
+                                                ]
+                                            },
+                                            "paddingBottom": {
+                                                "type": [
+                                                    "null",
+                                                    "string"
+                                                ]
+                                            },
+                                            "paddingTop": {
+                                                "type": [
+                                                    "null",
+                                                    "string"
+                                                ]
+                                            }
+                                        },
+                                        "type": [
+                                            "null",
+                                            "object"
+                                        ]
+                                    }
+                                },
+                                "type": [
+                                    "null",
+                                    "object"
+                                ]
+                            },
+                            "type": [
+                                "null",
+                                "array"
+                            ]
+                        }
+                    },
+                    "type": [
+                        "null",
+                        "object"
+                    ]
+                }
+            },
             "type": [
                 "null",
-                "string"
+                "object"
             ]
         },
-        "properties_hs_date_entered_qualifiedtobuy": {
-            "format": "date-time",
+        "folderId": {
+            "description": "ID of the folder where the email is stored",
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "properties_hs_date_exited_9567448": {
+        "freezeDate": {
+            "description": "Date when the email content was finalized",
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "properties_hs_date_exited_9567449": {
+        "fromName": {
+            "description": "Name of the sender displayed in the email",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_hs_date_exited_appointmentscheduled": {
-            "format": "date-time",
+        "hasContentAccessRules": {
+            "description": "Indicates if the email has content access rules applied",
             "type": [
                 "null",
-                "string"
+                "boolean"
             ]
         },
-        "properties_hs_date_exited_closedlost": {
-            "format": "date-time",
+        "htmlTitle": {
+            "description": "HTML title of the email",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_hs_date_exited_closedwon": {
-            "format": "date-time",
+        "id": {
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "properties_hs_date_exited_contractsent": {
-            "format": "date-time",
+        "isCreatedFomSandboxSync": {
+            "description": "Flag indicating if the email was created from a sandbox sync",
             "type": [
                 "null",
-                "string"
+                "boolean"
             ]
         },
-        "properties_hs_date_exited_customclosedwonstage": {
-            "format": "date-time",
+        "isGraymailSuppressionEnabled": {
+            "description": "Flag indicating if graymail suppression is enabled for the email",
             "type": [
                 "null",
-                "string"
+                "boolean"
             ]
         },
-        "properties_hs_date_exited_decisionmakerboughtin": {
-            "format": "date-time",
+        "isInstanceLayoutPage": {
+            "description": "Flag indicating if the email is a layout page in an instance",
             "type": [
                 "null",
-                "string"
+                "boolean"
             ]
         },
-        "properties_hs_date_exited_presentationscheduled": {
-            "format": "date-time",
+        "isLocalTimezoneSend": {
+            "description": "Flag indicating if the email is sent based on the local timezone",
             "type": [
                 "null",
-                "string"
+                "boolean"
             ]
         },
-        "properties_hs_date_exited_qualifiedtobuy": {
-            "format": "date-time",
+        "isPublished": {
+            "description": "Flag indicating if the email is published",
             "type": [
                 "null",
-                "string"
+                "boolean"
             ]
         },
-        "properties_hs_deal_amount_calculation_preference": {
+        "isRecipientFatigueSuppressionEnabled": {
+            "description": "Flag indicating if recipient fatigue suppression is enabled",
             "type": [
                 "null",
-                "string"
+                "boolean"
             ]
         },
-        "properties_hs_deal_stage_probability": {
+        "language": {
+            "description": "Language in which the email is written",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_hs_deal_stage_probability_shadow": {
+        "lastEditSessionId": {
+            "description": "Session ID of the last edit made to the email",
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "properties_hs_forecast_amount": {
+        "lastEditUpdateId": {
+            "description": "Update ID of the last edit made to the email",
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "properties_hs_forecast_probability": {
+        "layoutSections": {
+            "description": "Sections within the email layout",
             "type": [
                 "null",
-                "string"
+                "object"
             ]
         },
-        "properties_hs_is_closed": {
+        "leadFlowId": {
+            "description": "ID of the lead flow associated with the email",
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "properties_hs_is_closed_won": {
+        "liveDomain": {
+            "description": "Domain where the live version of the email is hosted",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_hs_lastmodifieddate": {
-            "format": "date-time",
+        "mailingIlsListsExcluded": {
+            "items": {
+                "type": [
+                    "null",
+                    "integer"
+                ]
+            },
             "type": [
                 "null",
-                "string"
+                "array"
             ]
         },
-        "properties_hs_latest_meeting_activity": {
+        "mailingIlsListsIncluded": {
+            "items": {
+                "type": [
+                    "null",
+                    "integer"
+                ]
+            },
             "type": [
                 "null",
-                "string"
+                "array"
             ]
         },
-        "properties_hs_likelihood_to_close": {
+        "mailingListsExcluded": {
+            "items": {
+                "type": [
+                    "null",
+                    "integer"
+                ]
+            },
             "type": [
                 "null",
-                "string"
+                "array"
+            ]
+        },
+        "mailingListsIncluded": {
+            "items": {
+                "type": [
+                    "null",
+                    "integer"
+                ]
+            },
+            "type": [
+                "null",
+                "array"
             ]
         },
-        "properties_hs_line_item_global_term_hs_discount_percentage": {
+        "maxRssEntries": {
+            "description": "Maximum number of RSS entries to include in the email",
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "properties_hs_line_item_global_term_hs_discount_percentage_enabled": {
+        "metaDescription": {
+            "description": "Meta description of the email content",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_hs_line_item_global_term_hs_recurring_billing_period": {
+        "name": {
+            "description": "Name of the email",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_hs_line_item_global_term_hs_recurring_billing_period_enabled": {
+        "pageExpiryEnabled": {
+            "description": "Flag indicating if page expiry is enabled for the email",
             "type": [
                 "null",
-                "string"
+                "boolean"
             ]
         },
-        "properties_hs_line_item_global_term_hs_recurring_billing_start_date": {
+        "pageRedirected": {
+            "description": "Information about page redirection",
             "type": [
                 "null",
-                "string"
+                "boolean"
             ]
         },
-        "properties_hs_line_item_global_term_hs_recurring_billing_start_date_enabled": {
+        "pastMabExperimentIds": {
+            "items": {
+                "type": [
+                    "null",
+                    "string"
+                ]
+            },
             "type": [
                 "null",
-                "string"
+                "array"
             ]
         },
-        "properties_hs_line_item_global_term_recurringbillingfrequency": {
+        "portalId": {
+            "description": "ID of the HubSpot portal associated with the email",
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "properties_hs_line_item_global_term_recurringbillingfrequency_enabled": {
+        "previewKey": {
+            "description": "Key used for email preview",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_hs_manual_forecast_category": {
+        "primaryEmailCampaignId": {
+            "description": "ID of the primary email campaign associated with the email",
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "properties_hs_merged_object_ids": {
+        "processingStatus": {
+            "description": "Status of the email processing",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_hs_mrr": {
+        "publishDate": {
+            "description": "Date when the email is scheduled to be published",
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "properties_hs_next_step": {
+        "publishImmediately": {
+            "description": "Flag indicating if the email should be published immediately",
             "type": [
                 "null",
-                "string"
+                "boolean"
             ]
         },
-        "properties_hs_num_target_accounts": {
+        "publishedAt": {
+            "description": "Timestamp when the email was published",
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "properties_hs_object_id": {
+        "publishedByEmail": {
+            "description": "Email address of the user who published the email",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_hs_predicted_amount": {
+        "publishedById": {
+            "description": "ID of the user who published the email",
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "properties_hs_predicted_amount_in_home_currency": {
+        "publishedByName": {
+            "description": "Name of the user who published the email",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_hs_priority": {
+        "publishedUrl": {
+            "description": "URL where the published email can be accessed",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_hs_projected_amount": {
+        "replyTo": {
+            "description": "Email address for replies to the email",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_hs_projected_amount_in_home_currency": {
+        "resolvedDomain": {
+            "description": "Domain resolved for the email",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_hs_sales_email_last_replied": {
+        "rootMicId": {
+            "description": "Root MIC ID associated with the email",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_hs_tcv": {
+        "rssEmailByText": {
+            "description": "Text content related to RSS emails",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_hs_unique_creation_key": {
+        "rssEmailClickThroughText": {
+            "description": "Text for click-through actions in RSS emails",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_hs_updated_by_user_id": {
+        "rssEmailCommentText": {
+            "description": "Text for comments in RSS emails",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_hs_user_ids_of_all_notification_followers": {
+        "rssEmailEntryTemplateEnabled": {
+            "description": "Flag indicating if the RSS email entry template is enabled",
             "type": [
                 "null",
-                "string"
+                "boolean"
             ]
         },
-        "properties_hs_user_ids_of_all_notification_unfollowers": {
+        "rssEmailImageMaxWidth": {
+            "description": "Maximum width of images in RSS emails",
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "properties_hs_user_ids_of_all_owners": {
+        "rssEmailUrl": {
+            "description": "URL for RSS emails",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_hubspot_owner_assigneddate": {
-            "format": "date-time",
+        "sections": {
+            "description": "Sections within the email",
             "type": [
                 "null",
-                "string"
+                "object"
             ]
         },
-        "properties_hubspot_owner_id": {
+        "securityState": {
+            "description": "Security state of the email",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_hubspot_team_id": {
+        "selected": {
+            "description": "Flag indicating if the email is selected",
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "properties_notes_last_contacted": {
+        "slug": {
+            "description": "Slug associated with the email",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_notes_last_updated": {
+        "smartEmailFields": {
+            "description": "Fields related to smart email features",
             "type": [
                 "null",
-                "string"
+                "object"
             ]
         },
-        "properties_notes_next_activity_date": {
+        "state": {
+            "description": "Current state of the email",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_num_associated_contacts": {
+        "stats": {
+            "properties": {
+                "counters": {
+                    "properties": {
+                        "bounce": {
+                            "type": [
+                                "null",
+                                "integer"
+                            ]
+                        },
+                        "click": {
+                            "type": [
+                                "null",
+                                "integer"
+                            ]
+                        },
+                        "contactslost": {
+                            "type": [
+                                "null",
+                                "integer"
+                            ]
+                        },
+                        "delivered": {
+                            "type": [
+                                "null",
+                                "integer"
+                            ]
+                        },
+                        "dropped": {
+                            "type": [
+                                "null",
+                                "integer"
+                            ]
+                        },
+                        "hardbounced": {
+                            "type": [
+                                "null",
+                                "integer"
+                            ]
+                        },
+                        "notsent": {
+                            "type": [
+                                "null",
+                                "integer"
+                            ]
+                        },
+                        "open": {
+                            "type": [
+                                "null",
+                                "integer"
+                            ]
+                        },
+                        "pending": {
+                            "type": [
+                                "null",
+                                "integer"
+                            ]
+                        },
+                        "reply": {
+                            "type": [
+                                "null",
+                                "integer"
+                            ]
+                        },
+                        "selected": {
+                            "type": [
+                                "null",
+                                "integer"
+                            ]
+                        },
+                        "sent": {
+                            "type": [
+                                "null",
+                                "integer"
+                            ]
+                        },
+                        "softbounced": {
+                            "type": [
+                                "null",
+                                "integer"
+                            ]
+                        },
+                        "spamreport": {
+                            "type": [
+                                "null",
+                                "integer"
+                            ]
+                        },
+                        "suppressed": {
+                            "type": [
+                                "null",
+                                "integer"
+                            ]
+                        },
+                        "unsubscribed": {
+                            "type": [
+                                "null",
+                                "integer"
+                            ]
+                        }
+                    },
+                    "type": [
+                        "null",
+                        "object"
+                    ]
+                },
+                "deviceBreakdown": {
+                    "properties": {
+                        "click_device_type": {
+                            "properties": {
+                                "computer": {
+                                    "type": [
+                                        "null",
+                                        "integer"
+                                    ]
+                                },
+                                "mobile": {
+                                    "type": [
+                                        "null",
+                                        "integer"
+                                    ]
+                                },
+                                "unknown": {
+                                    "type": [
+                                        "null",
+                                        "integer"
+                                    ]
+                                }
+                            },
+                            "type": [
+                                "null",
+                                "object"
+                            ]
+                        },
+                        "open_device_type": {
+                            "properties": {
+                                "computer": {
+                                    "type": [
+                                        "null",
+                                        "integer"
+                                    ]
+                                },
+                                "mobile": {
+                                    "type": [
+                                        "null",
+                                        "integer"
+                                    ]
+                                },
+                                "unknown": {
+                                    "type": [
+                                        "null",
+                                        "integer"
+                                    ]
+                                }
+                            },
+                            "type": [
+                                "null",
+                                "object"
+                            ]
+                        }
+                    },
+                    "type": [
+                        "null",
+                        "object"
+                    ]
+                },
+                "failedToLoad": {
+                    "type": [
+                        "null",
+                        "boolean"
+                    ]
+                },
+                "qualifierStats": {
+                    "type": [
+                        "null",
+                        "object"
+                    ]
+                },
+                "ratios": {
+                    "properties": {
+                        "bounceratio": {
+                            "type": [
+                                "null",
+                                "number"
+                            ]
+                        },
+                        "clickratio": {
+                            "type": [
+                                "null",
+                                "number"
+                            ]
+                        },
+                        "clickthroughratio": {
+                            "type": [
+                                "null",
+                                "number"
+                            ]
+                        },
+                        "contactslostratio": {
+                            "type": [
+                                "null",
+                                "number"
+                            ]
+                        },
+                        "deliveredratio": {
+                            "type": [
+                                "null",
+                                "number"
+                            ]
+                        },
+                        "hardbounceratio": {
+                            "type": [
+                                "null",
+                                "number"
+                            ]
+                        },
+                        "notsentratio": {
+                            "type": [
+                                "null",
+                                "number"
+                            ]
+                        },
+                        "openratio": {
+                            "type": [
+                                "null",
+                                "number"
+                            ]
+                        },
+                        "pendingratio": {
+                            "type": [
+                                "null",
+                                "number"
+                            ]
+                        },
+                        "replyratio": {
+                            "type": [
+                                "null",
+                                "number"
+                            ]
+                        },
+                        "softbounceratio": {
+                            "type": [
+                                "null",
+                                "number"
+                            ]
+                        },
+                        "spamreportratio": {
+                            "type": [
+                                "null",
+                                "number"
+                            ]
+                        },
+                        "unsubscribedratio": {
+                            "type": [
+                                "null",
+                                "number"
+                            ]
+                        }
+                    },
+                    "type": [
+                        "null",
+                        "object"
+                    ]
+                }
+            },
+            "type": [
+                "null",
+                "object"
+            ]
+        },
+        "styleSettings": {
+            "properties": {
+                "background_color": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "background_image": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "background_image_type": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "body_border_color": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "body_border_color_choice": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "body_border_width": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "body_color": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "color_picker_favorite1": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "color_picker_favorite2": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "color_picker_favorite3": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "color_picker_favorite4": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "color_picker_favorite5": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "color_picker_favorite6": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "email_body_padding": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "email_body_width": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "heading_one_font": {
+                    "properties": {
+                        "bold": {
+                            "type": [
+                                "null",
+                                "boolean"
+                            ]
+                        },
+                        "color": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "font": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "font_style": {
+                            "type": [
+                                "null",
+                                "object"
+                            ]
+                        },
+                        "italic": {
+                            "type": [
+                                "null",
+                                "boolean"
+                            ]
+                        },
+                        "size": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "underline": {
+                            "type": [
+                                "null",
+                                "boolean"
+                            ]
+                        }
+                    },
+                    "type": [
+                        "null",
+                        "object"
+                    ]
+                },
+                "heading_two_font": {
+                    "properties": {
+                        "bold": {
+                            "type": [
+                                "null",
+                                "boolean"
+                            ]
+                        },
+                        "color": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "font": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "font_style": {
+                            "type": [
+                                "null",
+                                "object"
+                            ]
+                        },
+                        "italic": {
+                            "type": [
+                                "null",
+                                "boolean"
+                            ]
+                        },
+                        "size": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "underline": {
+                            "type": [
+                                "null",
+                                "boolean"
+                            ]
+                        }
+                    },
+                    "type": [
+                        "null",
+                        "object"
+                    ]
+                },
+                "links_font": {
+                    "properties": {
+                        "bold": {
+                            "type": [
+                                "null",
+                                "boolean"
+                            ]
+                        },
+                        "color": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "font": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "font_style": {
+                            "type": [
+                                "null",
+                                "object"
+                            ]
+                        },
+                        "italic": {
+                            "type": [
+                                "null",
+                                "boolean"
+                            ]
+                        },
+                        "size": {
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "underline": {
+                            "type": [
+                                "null",
+                                "boolean"
+                            ]
+                        }
+                    },
+                    "type": [
+                        "null",
+                        "object"
+                    ]
+                },
+                "primary_accent_color": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "primary_font": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "primary_font_color": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "primary_font_line_height": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "primary_font_size": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "secondary_accent_color": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "secondary_font": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "secondary_font_color": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "secondary_font_line_height": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "secondary_font_size": {
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "use_email_client_default_settings": {
+                    "type": [
+                        "null",
+                        "boolean"
+                    ]
+                },
+                "user_module_defaults": {
+                    "properties": {
+                        "button_email": {
+                            "properties": {
+                                "background_color": {
+                                    "type": [
+                                        "null",
+                                        "string"
+                                    ]
+                                },
+                                "corner_radius": {
+                                    "type": [
+                                        "null",
+                                        "integer"
+                                    ]
+                                },
+                                "font": {
+                                    "type": [
+                                        "null",
+                                        "string"
+                                    ]
+                                },
+                                "font_color": {
+                                    "type": [
+                                        "null",
+                                        "string"
+                                    ]
+                                },
+                                "font_size": {
+                                    "type": [
+                                        "null",
+                                        "integer"
+                                    ]
+                                },
+                                "font_style": {
+                                    "type": [
+                                        "null",
+                                        "object"
+                                    ]
+                                }
+                            },
+                            "type": [
+                                "null",
+                                "object"
+                            ]
+                        },
+                        "email_divider": {
+                            "properties": {
+                                "color": {
+                                    "type": [
+                                        "null",
+                                        "object"
+                                    ]
+                                },
+                                "height": {
+                                    "type": [
+                                        "null",
+                                        "integer"
+                                    ]
+                                },
+                                "line_type": {
+                                    "type": [
+                                        "null",
+                                        "string"
+                                    ]
+                                }
+                            },
+                            "type": [
+                                "null",
+                                "object"
+                            ]
+                        }
+                    },
+                    "type": [
+                        "null",
+                        "object"
+                    ]
+                }
+            },
+            "type": [
+                "null",
+                "object"
+            ]
+        },
+        "subcategory": {
+            "description": "Subcategory to which the email belongs",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_num_contacted_notes": {
+        "subject": {
+            "description": "Subject line of the email",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_num_notes": {
+        "subscription": {
+            "description": "Information about email subscription",
+            "type": [
+                "null",
+                "integer"
+            ]
+        },
+        "subscriptionName": {
+            "description": "Name of the email subscription",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_pipeline": {
+        "teamPerms": {
+            "items": {
+                "type": [
+                    "null",
+                    "string"
+                ]
+            },
+            "type": [
+                "null",
+                "array"
+            ]
+        },
+        "templatePath": {
+            "description": "Path of the email template",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "updatedAt": {
-            "format": "date-time",
+        "transactional": {
+            "description": "Flag indicating if the email is transactional",
+            "type": [
+                "null",
+                "boolean"
+            ]
+        },
+        "translations": {
+            "description": "Translations available for the email",
+            "type": [
+                "null",
+                "object"
+            ]
+        },
+        "unpublishedAt": {
+            "description": "Timestamp when the email was unpublished",
+            "type": [
+                "null",
+                "integer"
+            ]
+        },
+        "updated": {
+            "description": "Timestamp of the last update to the email",
+            "type": [
+                "null",
+                "integer"
+            ]
+        },
+        "updatedById": {
+            "description": "ID of the user who last updated the email",
+            "type": [
+                "null",
+                "integer"
+            ]
+        },
+        "url": {
+            "description": "URL associated with the email",
             "type": [
                 "null",
                 "string"
             ]
+        },
+        "useRssHeadlineAsSubject": {
+            "description": "Flag indicating if the RSS headline should be used as the subject",
+            "type": [
+                "null",
+                "boolean"
+            ]
+        },
+        "userPerms": {
+            "items": {
+                "type": [
+                    "null",
+                    "integer"
+                ]
+            },
+            "type": [
+                "null",
+                "array"
+            ]
+        },
+        "vidsExcluded": {
+            "items": {
+                "type": [
+                    "null",
+                    "integer"
+                ]
+            },
+            "type": [
+                "null",
+                "array"
+            ]
+        },
+        "vidsIncluded": {
+            "items": {
+                "type": [
+                    "null",
+                    "integer"
+                ]
+            },
+            "type": [
+                "null",
+                "array"
+            ]
+        },
+        "visibleToAll": {
+            "description": "Flag indicating if the email is visible to all users",
+            "type": [
+                "null",
+                "boolean"
+            ]
         }
     },
     "type": [
         "null",
         "object"
     ]
 }
```

### Comparing `airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/schemas/deals_property_history.json` & `airbyte_source_hubspot-4.1.2/source_hubspot/schemas/companies.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5078125%*

 * *Differences: {"'$schema'": "'http://json-schema.org/draft-07/schema#'",*

 * * "'properties'": "{'archived': {'description': 'Indicates whether the company is archived or "*

 * *                 "active'}, 'id': OrderedDict([('description', 'Unique identifier for the "*

 * *                 "company'), ('type', ['null', 'string'])]), 'createdAt': "*

 * *                 "OrderedDict([('description', 'Date and time when the company was created'), "*

 * *                 "('type', ['null', 'string']), ('format', 'date-time')]), 'updatedAt': "*

 * *     […]*

```diff
@@ -1,60 +1,50 @@
 {
-    "$schema": "http://json-schema.org/draft-07/schema",
-    "additionalProperties": true,
+    "$schema": "http://json-schema.org/draft-07/schema#",
     "properties": {
         "archived": {
+            "description": "Indicates whether the company is archived or active",
             "type": [
                 "null",
                 "boolean"
             ]
         },
-        "dealId": {
+        "contacts": {
+            "description": "List of contacts associated with the company",
+            "items": {
+                "description": "Details of individual contacts",
+                "type": "string"
+            },
             "type": [
                 "null",
-                "string"
-            ]
-        },
-        "property": {
-            "type": [
-                "null",
-                "string"
+                "array"
             ]
         },
-        "sourceId": {
+        "createdAt": {
+            "description": "Date and time when the company was created",
+            "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "sourceType": {
+        "id": {
+            "description": "Unique identifier for the company",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "timestamp": {
-            "airbyte_type": "timestamp_with_timezone",
+        "updatedAt": {
+            "description": "Date and time when the company was last updated",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
-        },
-        "updatedByUserId": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "value": {
-            "type": [
-                "null",
-                "string"
-            ]
         }
     },
     "type": [
         "null",
         "object"
     ]
 }
```

### Comparing `airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/schemas/engagements_emails.json` & `airbyte_source_hubspot-4.1.2/source_hubspot/schemas/engagements_tasks.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8781129826011513%*

 * *Differences: {"'properties'": "{'id': {'description': 'Unique identifier for the task'}, 'properties': "*

 * *                 "{'properties': {'hs_all_assigned_business_unit_ids': {'description': 'Array of "*

 * *                 "IDs of business units this task is assigned to'}, 'hs_at_mentioned_owner_ids': "*

 * *                 "{'description': 'Array of IDs of owners mentioned in the task'}, "*

 * *                 "'hs_attachment_ids': {'description': 'Array of attachment IDs associated with "*

 * *                 "this task'}, 'hs_body […]*

```diff
@@ -1,1053 +1,946 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
     "properties": {
         "archived": {
+            "description": "Indicates if the task has been archived",
             "type": [
                 "null",
                 "boolean"
             ]
         },
         "companies": {
+            "description": "List of companies associated with the task",
             "items": {
                 "type": [
                     "null",
                     "string"
                 ]
             },
             "type": [
                 "null",
                 "array"
             ]
         },
         "contacts": {
+            "description": "List of contacts associated with the task",
             "items": {
                 "type": [
                     "null",
                     "string"
                 ]
             },
             "type": [
                 "null",
                 "array"
             ]
         },
         "createdAt": {
+            "description": "The date and time when the task was created",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
         "deals": {
+            "description": "List of deals associated with the task",
             "items": {
                 "type": [
                     "null",
                     "string"
                 ]
             },
             "type": [
                 "null",
                 "array"
             ]
         },
         "id": {
+            "description": "Unique identifier for the task",
             "type": [
                 "null",
                 "string"
             ]
         },
         "properties": {
+            "description": "Custom properties associated with the task.",
             "properties": {
                 "hs_all_accessible_team_ids": {
+                    "description": "Array of IDs of teams that have access to this engagement task",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
                 "hs_all_assigned_business_unit_ids": {
+                    "description": "Array of IDs of business units this task is assigned to",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
                 "hs_all_owner_ids": {
+                    "description": "Array of IDs of all owners associated with this task",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
                 "hs_all_team_ids": {
+                    "description": "Array of IDs of all teams associated with this task",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
                 "hs_at_mentioned_owner_ids": {
+                    "description": "Array of IDs of owners mentioned in the task",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
                 "hs_attachment_ids": {
+                    "description": "Array of attachment IDs associated with this task",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
                 "hs_body_preview": {
+                    "description": "Preview of the body content of the task",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
                 "hs_body_preview_html": {
+                    "description": "HTML version of the body content preview",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
                 "hs_body_preview_is_truncated": {
+                    "description": "Indicates if the body preview is truncated",
                     "type": [
                         "null",
                         "boolean"
                     ]
                 },
-                "hs_created_by": {
+                "hs_calendar_event_id": {
+                    "description": "ID of the associated calendar event, if any",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "hs_created_by_user_id": {
+                "hs_created_by": {
+                    "description": "Creator of the task",
                     "type": [
                         "null",
                         "number"
                     ]
                 },
-                "hs_createdate": {
-                    "format": "date-time",
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_direction_and_unique_id": {
+                "hs_created_by_user_id": {
+                    "description": "ID of the user who created the task",
                     "type": [
                         "null",
-                        "string"
+                        "number"
                     ]
                 },
-                "hs_email_attached_video_id": {
+                "hs_createdate": {
+                    "description": "The date and time when the task was created",
+                    "format": "date-time",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "hs_email_attached_video_name": {
+                "hs_engagement_source": {
+                    "description": "Source of the engagement task",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "hs_email_attached_video_opened": {
-                    "type": [
-                        "null",
-                        "boolean"
-                    ]
-                },
-                "hs_email_attached_video_watched": {
-                    "type": [
-                        "null",
-                        "boolean"
-                    ]
-                },
-                "hs_email_bcc_email": {
+                "hs_engagement_source_id": {
+                    "description": "ID of the source of the engagement task",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "hs_email_bcc_firstname": {
+                "hs_follow_up_action": {
+                    "description": "Action to follow up on the task",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "hs_email_bcc_lastname": {
+                "hs_gdpr_deleted": {
+                    "description": "Indicates if the task has been deleted due to GDPR compliance",
                     "type": [
                         "null",
-                        "string"
+                        "boolean"
                     ]
                 },
-                "hs_email_bcc_raw": {
+                "hs_lastmodifieddate": {
+                    "description": "The date and time when the task was last modified",
+                    "format": "date-time",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "hs_email_cc_email": {
+                "hs_merged_object_ids": {
+                    "description": "Array of IDs of merged objects",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "hs_email_cc_firstname": {
+                "hs_modified_by": {
+                    "description": "Last user who modified the task",
                     "type": [
                         "null",
-                        "string"
+                        "number"
                     ]
                 },
-                "hs_email_cc_lastname": {
+                "hs_msteams_message_id": {
+                    "description": "ID of the Microsoft Teams message associated with the task",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "hs_email_cc_raw": {
+                "hs_num_associated_companies": {
+                    "description": "Number of companies associated with the task",
                     "type": [
                         "null",
-                        "string"
+                        "number"
                     ]
                 },
-                "hs_email_direction": {
+                "hs_num_associated_contacts": {
+                    "description": "Number of contacts associated with the task",
                     "type": [
                         "null",
-                        "string"
+                        "number"
                     ]
                 },
-                "hs_email_encoded_email_associations_request": {
+                "hs_num_associated_deals": {
+                    "description": "Number of deals associated with the task",
                     "type": [
                         "null",
-                        "string"
+                        "number"
                     ]
                 },
-                "hs_email_error_message": {
+                "hs_num_associated_queue_objects": {
+                    "description": "Number of queue objects associated with the task",
                     "type": [
                         "null",
-                        "string"
+                        "number"
                     ]
                 },
-                "hs_email_facsimile_send_id": {
+                "hs_num_associated_tickets": {
+                    "description": "Number of tickets associated with the task",
                     "type": [
                         "null",
-                        "string"
+                        "number"
                     ]
                 },
-                "hs_email_from_email": {
+                "hs_object_id": {
+                    "description": "ID of the engagement task object",
                     "type": [
                         "null",
-                        "string"
+                        "number"
                     ]
                 },
-                "hs_email_from_firstname": {
+                "hs_product_name": {
+                    "description": "Name of the product associated with the task",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "hs_email_from_lastname": {
+                "hs_queue_membership_ids": {
+                    "description": "Array of IDs of queue members associated with the task",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "hs_email_from_raw": {
+                "hs_scheduled_tasks": {
+                    "description": "Array of scheduled tasks related to this task",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "hs_email_headers": {
+                "hs_task_body": {
+                    "description": "Full body content of the task",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "hs_email_html": {
+                "hs_task_completion_date": {
+                    "description": "The date and time when the task was completed",
+                    "format": "date-time",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "hs_email_logged_from": {
+                "hs_task_contact_timezone": {
+                    "description": "Timezone of the contact related to the task",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "hs_email_media_processing_status": {
+                "hs_task_for_object_type": {
+                    "description": "Type of object the task is related to",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "hs_email_member_of_forwarded_subthread": {
+                "hs_task_is_all_day": {
+                    "description": "Indicates if the task spans the whole day",
                     "type": [
                         "null",
                         "boolean"
                     ]
                 },
-                "hs_email_message_id": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_email_migrated_via_portal_data_migration": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_email_pending_inline_image_ids": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_email_post_send_status": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_email_recipient_drop_reasons": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_email_send_event_id": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_email_send_event_id_created": {
+                "hs_task_last_contact_outreach": {
+                    "description": "The date and time of the last contact outreach related to the task",
                     "format": "date-time",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "hs_email_sender_email": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_email_sender_firstname": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_email_sender_lastname": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_email_sender_raw": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_email_sent_via": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_email_status": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_email_subject": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_email_text": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_email_thread_id": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_email_to_email": {
+                "hs_task_last_sales_activity_timestamp": {
+                    "description": "The date and time of the last sales activity related to the task",
+                    "format": "date-time",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "hs_email_to_firstname": {
+                "hs_task_priority": {
+                    "description": "Priority level of the task",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "hs_email_to_lastname": {
+                "hs_task_probability_to_complete": {
+                    "description": "Probability of completing the task",
                     "type": [
                         "null",
-                        "string"
+                        "number"
                     ]
                 },
-                "hs_email_to_raw": {
+                "hs_task_relative_reminders": {
+                    "description": "Relative reminders set for the task",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "hs_email_tracker_key": {
+                "hs_task_reminders": {
+                    "description": "Specific reminders set for the task",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "hs_email_validation_skipped": {
+                "hs_task_repeat_interval": {
+                    "description": "Interval for repeating the task",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "hs_engagement_source": {
+                "hs_task_send_default_reminder": {
+                    "description": "Indicates if default reminders should be sent for the task",
                     "type": [
                         "null",
-                        "string"
+                        "boolean"
                     ]
                 },
-                "hs_engagement_source_id": {
+                "hs_task_sequence_enrollment_active": {
+                    "description": "Indicates if the task is part of an active sequence enrollment",
                     "type": [
                         "null",
-                        "string"
+                        "boolean"
                     ]
                 },
-                "hs_follow_up_action": {
+                "hs_task_sequence_step_enrollment_id": {
+                    "description": "ID of the sequence step enrollment related to the task",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "hs_gdpr_deleted": {
+                "hs_task_sequence_step_order": {
+                    "description": "Order of the task within the sequence step",
                     "type": [
                         "null",
-                        "boolean"
+                        "number"
                     ]
                 },
-                "hs_lastmodifieddate": {
-                    "format": "date-time",
+                "hs_task_status": {
+                    "description": "Status of the task",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "hs_merged_object_ids": {
+                "hs_task_subject": {
+                    "description": "Subject of the task",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "hs_modified_by": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_object_id": {
+                "hs_task_template_id": {
+                    "description": "ID of the task template, if any",
                     "type": [
                         "null",
                         "number"
                     ]
                 },
-                "hs_product_name": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_queue_membership_ids": {
+                "hs_task_type": {
+                    "description": "Type of the task",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
                 "hs_timestamp": {
+                    "description": "The timestamp associated with the task",
                     "format": "date-time",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
                 "hs_unique_creation_key": {
+                    "description": "Unique key for task creation",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
                 "hs_unique_id": {
+                    "description": "Unique ID of the task",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
                 "hs_updated_by_user_id": {
+                    "description": "ID of the user who last updated the task",
                     "type": [
                         "null",
                         "number"
                     ]
                 },
                 "hs_user_ids_of_all_notification_followers": {
+                    "description": "Array of user IDs who are followers and receive notifications",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
                 "hs_user_ids_of_all_notification_unfollowers": {
+                    "description": "Array of user IDs who have unfollowed notifications for the task",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
                 "hs_user_ids_of_all_owners": {
+                    "description": "Array of user IDs of all owners",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
                 "hubspot_owner_assigneddate": {
+                    "description": "The date and time when the task was assigned to an owner",
                     "format": "date-time",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
                 "hubspot_owner_id": {
+                    "description": "ID of the owner of the task in HubSpot",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
                 "hubspot_team_id": {
+                    "description": "ID of the team of the task in HubSpot",
                     "type": [
                         "null",
                         "string"
                     ]
                 }
             },
             "type": "object"
         },
         "properties_hs_all_accessible_team_ids": {
+            "description": "List of all team IDs that have access to this task.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "properties_hs_all_assigned_business_unit_ids": {
+            "description": "List of all business unit IDs assigned to this task.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "properties_hs_all_owner_ids": {
+            "description": "List of all user IDs who are owners of this task.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "properties_hs_all_team_ids": {
+            "description": "List of all team IDs assigned to this task.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "properties_hs_at_mentioned_owner_ids": {
+            "description": "List of user IDs mentioned in the task.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "properties_hs_attachment_ids": {
+            "description": "List of attachment IDs associated with the task.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "properties_hs_body_preview": {
+            "description": "Preview of the task body content.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "properties_hs_body_preview_html": {
+            "description": "HTML formatted preview of the task body content.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "properties_hs_body_preview_is_truncated": {
+            "description": "Flag indicating if the body preview is truncated.",
             "type": [
                 "null",
                 "boolean"
             ]
         },
-        "properties_hs_created_by": {
+        "properties_hs_calendar_event_id": {
+            "description": "ID of the calendar event associated with the task.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_hs_created_by_user_id": {
+        "properties_hs_created_by": {
+            "description": "User who created the task.",
             "type": [
                 "null",
                 "number"
             ]
         },
-        "properties_hs_createdate": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_direction_and_unique_id": {
+        "properties_hs_created_by_user_id": {
+            "description": "User ID of the task creator.",
             "type": [
                 "null",
-                "string"
+                "number"
             ]
         },
-        "properties_hs_email_attached_video_id": {
+        "properties_hs_createdate": {
+            "description": "The date and time when the task was created",
+            "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_hs_email_attached_video_name": {
+        "properties_hs_engagement_source": {
+            "description": "Source of the task engagement.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_hs_email_attached_video_opened": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
-        "properties_hs_email_attached_video_watched": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
-        "properties_hs_email_bcc_email": {
+        "properties_hs_engagement_source_id": {
+            "description": "ID of the task engagement source.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_hs_email_bcc_firstname": {
+        "properties_hs_follow_up_action": {
+            "description": "Follow-up action associated with the task.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_hs_email_bcc_lastname": {
+        "properties_hs_gdpr_deleted": {
+            "description": "Flag indicating if the task is deleted due to GDPR compliance.",
             "type": [
                 "null",
-                "string"
+                "boolean"
             ]
         },
-        "properties_hs_email_bcc_raw": {
+        "properties_hs_lastmodifieddate": {
+            "description": "The date and time when the task was last modified",
+            "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_hs_email_cc_email": {
+        "properties_hs_merged_object_ids": {
+            "description": "List of object IDs merged with this task.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_hs_email_cc_firstname": {
+        "properties_hs_modified_by": {
+            "description": "User who last modified the task.",
             "type": [
                 "null",
-                "string"
+                "number"
             ]
         },
-        "properties_hs_email_cc_lastname": {
+        "properties_hs_msteams_message_id": {
+            "description": "ID of the Microsoft Teams message associated with the task.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_hs_email_cc_raw": {
+        "properties_hs_num_associated_companies": {
+            "description": "Number of companies associated with the task.",
             "type": [
                 "null",
-                "string"
+                "number"
             ]
         },
-        "properties_hs_email_direction": {
+        "properties_hs_num_associated_contacts": {
+            "description": "Number of contacts associated with the task.",
             "type": [
                 "null",
-                "string"
+                "number"
             ]
         },
-        "properties_hs_email_encoded_email_associations_request": {
+        "properties_hs_num_associated_deals": {
+            "description": "Number of deals associated with the task.",
             "type": [
                 "null",
-                "string"
+                "number"
             ]
         },
-        "properties_hs_email_error_message": {
+        "properties_hs_num_associated_queue_objects": {
+            "description": "Number of queue objects associated with the task.",
             "type": [
                 "null",
-                "string"
+                "number"
             ]
         },
-        "properties_hs_email_facsimile_send_id": {
+        "properties_hs_num_associated_tickets": {
+            "description": "Number of tickets associated with the task.",
             "type": [
                 "null",
-                "string"
+                "number"
             ]
         },
-        "properties_hs_email_from_email": {
+        "properties_hs_object_id": {
+            "description": "ID of the task object.",
             "type": [
                 "null",
-                "string"
+                "number"
             ]
         },
-        "properties_hs_email_from_firstname": {
+        "properties_hs_product_name": {
+            "description": "Product name associated with the task.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_hs_email_from_lastname": {
+        "properties_hs_queue_membership_ids": {
+            "description": "List of queue membership IDs associated with the task.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_hs_email_from_raw": {
+        "properties_hs_scheduled_tasks": {
+            "description": "Flag indicating if the task is scheduled.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_hs_email_headers": {
+        "properties_hs_task_body": {
+            "description": "Full body content of the task.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_hs_email_html": {
+        "properties_hs_task_completion_date": {
+            "description": "The date and time when the task was completed",
+            "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_hs_email_logged_from": {
+        "properties_hs_task_contact_timezone": {
+            "description": "Time zone of the contact associated with the task.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_hs_email_media_processing_status": {
+        "properties_hs_task_for_object_type": {
+            "description": "Type of object the task is for (e.g., contact, deal).",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_hs_email_member_of_forwarded_subthread": {
+        "properties_hs_task_is_all_day": {
+            "description": "Flag indicating if the task is an all-day task.",
             "type": [
                 "null",
                 "boolean"
             ]
         },
-        "properties_hs_email_message_id": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_email_migrated_via_portal_data_migration": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_email_pending_inline_image_ids": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_email_post_send_status": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_email_recipient_drop_reasons": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_email_send_event_id": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_email_send_event_id_created": {
+        "properties_hs_task_last_contact_outreach": {
+            "description": "The date and time of the last contact outreach related to the task",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_hs_email_sender_email": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_email_sender_firstname": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_email_sender_lastname": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_email_sender_raw": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_email_sent_via": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_email_status": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_email_subject": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_email_text": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_email_thread_id": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_email_to_email": {
+        "properties_hs_task_last_sales_activity_timestamp": {
+            "description": "The date and time of the last sales activity related to the task",
+            "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_hs_email_to_firstname": {
+        "properties_hs_task_priority": {
+            "description": "Priority level of the task.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_hs_email_to_lastname": {
+        "properties_hs_task_probability_to_complete": {
+            "description": "Probability of completing the task.",
             "type": [
                 "null",
-                "string"
+                "number"
             ]
         },
-        "properties_hs_email_to_raw": {
+        "properties_hs_task_relative_reminders": {
+            "description": "List of relative reminders set for the task.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_hs_email_tracker_key": {
+        "properties_hs_task_reminders": {
+            "description": "List of reminders set for the task.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_hs_email_validation_skipped": {
+        "properties_hs_task_repeat_interval": {
+            "description": "Repeat interval for recurring tasks.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_hs_engagement_source": {
+        "properties_hs_task_send_default_reminder": {
+            "description": "Flag indicating if default reminders should be sent for the task.",
             "type": [
                 "null",
-                "string"
+                "boolean"
             ]
         },
-        "properties_hs_engagement_source_id": {
+        "properties_hs_task_sequence_enrollment_active": {
+            "description": "Flag indicating if the task sequence enrollment is active.",
             "type": [
                 "null",
-                "string"
+                "boolean"
             ]
         },
-        "properties_hs_follow_up_action": {
+        "properties_hs_task_sequence_step_enrollment_id": {
+            "description": "ID of the task sequence step enrollment.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_hs_gdpr_deleted": {
+        "properties_hs_task_sequence_step_order": {
+            "description": "Order of the task within the sequence step.",
             "type": [
                 "null",
-                "boolean"
+                "number"
             ]
         },
-        "properties_hs_lastmodifieddate": {
-            "format": "date-time",
+        "properties_hs_task_status": {
+            "description": "Status of the task (e.g., open, closed).",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_hs_merged_object_ids": {
+        "properties_hs_task_subject": {
+            "description": "Subject of the task.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_hs_modified_by": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_object_id": {
+        "properties_hs_task_template_id": {
+            "description": "ID of the task template.",
             "type": [
                 "null",
                 "number"
             ]
         },
-        "properties_hs_product_name": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_queue_membership_ids": {
+        "properties_hs_task_type": {
+            "description": "Type of the task (e.g., call, email).",
             "type": [
                 "null",
                 "string"
             ]
         },
         "properties_hs_timestamp": {
+            "description": "The timestamp associated with the task",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
         "properties_hs_unique_creation_key": {
+            "description": "Unique key for identifying task creation.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "properties_hs_unique_id": {
+            "description": "Unique ID for the task.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "properties_hs_updated_by_user_id": {
+            "description": "User ID of the user who last updated the task.",
             "type": [
                 "null",
                 "number"
             ]
         },
         "properties_hs_user_ids_of_all_notification_followers": {
+            "description": "List of user IDs following notifications for the task.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "properties_hs_user_ids_of_all_notification_unfollowers": {
+            "description": "List of user IDs not following notifications for the task.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "properties_hs_user_ids_of_all_owners": {
+            "description": "List of user IDs who are owners of the task.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "properties_hubspot_owner_assigneddate": {
+            "description": "The date and time when the task was assigned to an owner",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
         "properties_hubspot_owner_id": {
+            "description": "ID of the HubSpot owner associated with the task.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "properties_hubspot_team_id": {
+            "description": "ID of the HubSpot team associated with the task.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "tickets": {
+            "description": "List of tickets associated with the task",
             "items": {
                 "type": [
                     "null",
                     "string"
                 ]
             },
             "type": [
                 "null",
                 "array"
             ]
         },
         "updatedAt": {
+            "description": "The date and time when the task was last updated",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         }
     },
```

### Comparing `airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/schemas/engagements_meetings.json` & `airbyte_source_hubspot-4.1.2/source_hubspot/schemas/forms.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8410947712418301%*

 * *Differences: {"'properties'": "{'id': {'description': 'Unique identifier for the form.'}, 'createdAt': "*

 * *                 "{'description': 'Date and time when the form was created.'}, 'updatedAt': "*

 * *                 "{'description': 'Date and time when the form was last updated.'}, 'archived': "*

 * *                 "{'description': 'Indicates whether the form is archived.'}, 'name': "*

 * *                 "OrderedDict([('description', 'Name of the form.'), ('type', ['null', "*

 * *                 "'string'])]), 'formType': Ordered […]*

```diff
@@ -1,719 +1,423 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
     "properties": {
         "archived": {
+            "description": "Indicates whether the form is archived.",
             "type": [
                 "null",
                 "boolean"
             ]
         },
-        "companies": {
-            "items": {
-                "type": [
-                    "null",
-                    "string"
-                ]
-            },
-            "type": [
-                "null",
-                "array"
-            ]
-        },
-        "contacts": {
-            "items": {
-                "type": [
-                    "null",
-                    "string"
-                ]
-            },
-            "type": [
-                "null",
-                "array"
-            ]
-        },
-        "createdAt": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "deals": {
-            "items": {
-                "type": [
-                    "null",
-                    "string"
-                ]
-            },
-            "type": [
-                "null",
-                "array"
-            ]
-        },
-        "id": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties": {
+        "configuration": {
+            "description": "Configuration settings for the form.",
             "properties": {
-                "hs_activity_type": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_all_accessible_team_ids": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_all_assigned_business_unit_ids": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_all_owner_ids": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_all_team_ids": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_at_mentioned_owner_ids": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_attachment_ids": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_attendee_owner_ids": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_body_preview": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_body_preview_html": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_body_preview_is_truncated": {
+                "allowLinkToResetKnownValues": {
+                    "description": "Allows resetting known values through a link.",
                     "type": [
                         "null",
                         "boolean"
                     ]
                 },
-                "hs_created_by": {
-                    "type": [
-                        "null",
-                        "number"
-                    ]
-                },
-                "hs_created_by_user_id": {
-                    "type": [
-                        "null",
-                        "number"
-                    ]
-                },
-                "hs_createdate": {
-                    "format": "date-time",
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_engagement_source": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_engagement_source_id": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_follow_up_action": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_gdpr_deleted": {
+                "archivable": {
+                    "description": "Indicates whether the form is archivable.",
                     "type": [
                         "null",
                         "boolean"
                     ]
                 },
-                "hs_i_cal_uid": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_internal_meeting_notes": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_lastmodifieddate": {
-                    "format": "date-time",
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_meeting_body": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_meeting_calendar_event_hash": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_meeting_change_id": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_meeting_created_from_link_id": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_meeting_end_time": {
-                    "format": "date-time",
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_meeting_external_url": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_meeting_location": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_meeting_location_type": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_meeting_outcome": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_meeting_pre_meeting_prospect_reminders": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_meeting_source": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_meeting_source_id": {
+                "cloneable": {
+                    "description": "Indicates whether the form is cloneable.",
                     "type": [
                         "null",
-                        "string"
-                    ]
-                },
-                "hs_meeting_start_time": {
-                    "format": "date-time",
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_meeting_title": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_meeting_web_conference_meeting_id": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_merged_object_ids": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hs_modified_by": {
-                    "type": [
-                        "null",
-                        "number"
-                    ]
-                },
-                "hs_object_id": {
-                    "type": [
-                        "null",
-                        "number"
+                        "boolean"
                     ]
                 },
-                "hs_product_name": {
+                "createNewContactForNewEmail": {
+                    "description": "Creates a new contact for a new email.",
                     "type": [
                         "null",
-                        "string"
+                        "boolean"
                     ]
                 },
-                "hs_queue_membership_ids": {
+                "editable": {
+                    "description": "Indicates whether the form is editable.",
                     "type": [
                         "null",
-                        "string"
+                        "boolean"
                     ]
                 },
-                "hs_scheduled_tasks": {
+                "language": {
+                    "description": "Language setting for the form.",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "hs_timestamp": {
-                    "format": "date-time",
+                "lifecycleStages": {
+                    "description": "List of lifecycle stages.",
+                    "items": {
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
                     "type": [
                         "null",
-                        "string"
+                        "array"
                     ]
                 },
-                "hs_unique_creation_key": {
+                "notifyContactOwner": {
+                    "description": "Notification setting for contacting the owner.",
                     "type": [
                         "null",
-                        "string"
+                        "boolean"
                     ]
                 },
-                "hs_unique_id": {
+                "notifyRecipients": {
+                    "description": "Notification setting for recipients.",
                     "type": [
                         "null",
-                        "string"
+                        "array"
                     ]
                 },
-                "hs_updated_by_user_id": {
+                "postSubmitAction": {
+                    "description": "Action to be taken after form submission.",
+                    "properties": {
+                        "type": {
+                            "description": "Type of post-submit action.",
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "value": {
+                            "description": "Value of post-submit action.",
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        }
+                    },
                     "type": [
                         "null",
-                        "number"
+                        "object"
                     ]
                 },
-                "hs_user_ids_of_all_notification_followers": {
+                "prePopulateKnownValues": {
+                    "description": "Pre-populates known values in the form.",
                     "type": [
                         "null",
-                        "string"
+                        "boolean"
                     ]
                 },
-                "hs_user_ids_of_all_notification_unfollowers": {
+                "recaptchaEnabled": {
+                    "description": "Indicates whether reCAPTCHA is enabled.",
                     "type": [
                         "null",
-                        "string"
+                        "boolean"
                     ]
-                },
-                "hs_user_ids_of_all_owners": {
+                }
+            },
+            "type": [
+                "null",
+                "object"
+            ]
+        },
+        "createdAt": {
+            "description": "Date and time when the form was created.",
+            "format": "date-time",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "deletedAt": {
+            "description": "Date and time when the form was deleted.",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "displayOptions": {
+            "description": "Display options for the form.",
+            "properties": {
+                "cssClass": {
+                    "description": "CSS class for styling the form.",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "hubspot_owner_assigneddate": {
-                    "format": "date-time",
+                "renderRawHtml": {
+                    "description": "Indicates whether to render raw HTML.",
                     "type": [
                         "null",
-                        "string"
+                        "boolean"
                     ]
                 },
-                "hubspot_owner_id": {
+                "style": {
+                    "description": "Style settings for the form.",
+                    "properties": {
+                        "backgroundWidth": {
+                            "description": "Background width style.",
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "fontFamily": {
+                            "description": "Font family style.",
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "helpTextColor": {
+                            "description": "Help text color style.",
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "helpTextSize": {
+                            "description": "Help text font size.",
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "labelTextColor": {
+                            "description": "Label text color style.",
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "labelTextSize": {
+                            "description": "Label text font size.",
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "legalConsentTextColor": {
+                            "description": "Legal consent text color style.",
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "legalConsentTextSize": {
+                            "description": "Legal consent text font size.",
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "submitAlignment": {
+                            "description": "Alignment of submit button.",
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "submitColor": {
+                            "description": "Color of submit button.",
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "submitFontColor": {
+                            "description": "Font color of submit button.",
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        },
+                        "submitSize": {
+                            "description": "Size of submit button.",
+                            "type": [
+                                "null",
+                                "string"
+                            ]
+                        }
+                    },
+                    "type": [
+                        "null",
+                        "object"
+                    ]
+                },
+                "submitButtonText": {
+                    "description": "Text for the submit button.",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "hubspot_team_id": {
+                "theme": {
+                    "description": "Theme setting for the form.",
                     "type": [
                         "null",
                         "string"
                     ]
                 }
             },
-            "type": "object"
-        },
-        "properties_hs_activity_type": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_all_accessible_team_ids": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_all_assigned_business_unit_ids": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_all_owner_ids": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_all_team_ids": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_at_mentioned_owner_ids": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_attachment_ids": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_attendee_owner_ids": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_body_preview": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_body_preview_html": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_body_preview_is_truncated": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
-        "properties_hs_created_by": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "properties_hs_created_by_user_id": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "properties_hs_createdate": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_engagement_source": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_engagement_source_id": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_follow_up_action": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_gdpr_deleted": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
-        "properties_hs_i_cal_uid": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_internal_meeting_notes": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_lastmodifieddate": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_meeting_body": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_meeting_calendar_event_hash": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_meeting_change_id": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_meeting_created_from_link_id": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_meeting_end_time": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_meeting_external_url": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_meeting_location": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_meeting_location_type": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_meeting_outcome": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_meeting_pre_meeting_prospect_reminders": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_meeting_source": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_meeting_source_id": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_meeting_start_time": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_meeting_title": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_meeting_web_conference_meeting_id": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_merged_object_ids": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_modified_by": {
             "type": [
                 "null",
-                "number"
+                "object"
             ]
         },
-        "properties_hs_object_id": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "properties_hs_product_name": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_queue_membership_ids": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_scheduled_tasks": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_timestamp": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_unique_creation_key": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_unique_id": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_updated_by_user_id": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "properties_hs_user_ids_of_all_notification_followers": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_user_ids_of_all_notification_unfollowers": {
+        "fieldGroups": {
+            "description": "Groups containing fields of a form.",
+            "items": {
+                "description": "Field groups in the form.",
+                "properties": {
+                    "fields": {
+                        "items": {
+                            "description": "Properties of each field.",
+                            "properties": {
+                                "fieldType": {
+                                    "description": "Type of the field.",
+                                    "type": [
+                                        "null",
+                                        "string"
+                                    ]
+                                },
+                                "hidden": {
+                                    "description": "Indicates whether the field is hidden.",
+                                    "type": [
+                                        "null",
+                                        "boolean"
+                                    ]
+                                },
+                                "label": {
+                                    "description": "Label for the field.",
+                                    "type": [
+                                        "null",
+                                        "string"
+                                    ]
+                                },
+                                "name": {
+                                    "description": "Name of the field.",
+                                    "type": [
+                                        "null",
+                                        "string"
+                                    ]
+                                },
+                                "objectTypeId": {
+                                    "description": "Object type ID for the field.",
+                                    "type": [
+                                        "null",
+                                        "string"
+                                    ]
+                                },
+                                "required": {
+                                    "description": "Indicates whether the field is required.",
+                                    "type": [
+                                        "null",
+                                        "boolean"
+                                    ]
+                                },
+                                "validation": {
+                                    "description": "Validation settings for the field.",
+                                    "properties": {
+                                        "blockedEmailDomains": {
+                                            "description": "List of blocked email domains for validation.",
+                                            "items": {
+                                                "type": [
+                                                    "null",
+                                                    "string"
+                                                ]
+                                            },
+                                            "type": [
+                                                "null",
+                                                "array"
+                                            ]
+                                        },
+                                        "useDefaultBlockList": {
+                                            "description": "Indicates whether to use the default block list for validation.",
+                                            "type": [
+                                                "null",
+                                                "boolean"
+                                            ]
+                                        }
+                                    },
+                                    "type": [
+                                        "null",
+                                        "object"
+                                    ]
+                                }
+                            },
+                            "type": [
+                                "null",
+                                "object"
+                            ]
+                        },
+                        "type": [
+                            "null",
+                            "array"
+                        ]
+                    },
+                    "groupType": {
+                        "description": "Type of field group.",
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "richTextType": {
+                        "description": "Type of rich text.",
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    }
+                },
+                "type": [
+                    "null",
+                    "object"
+                ]
+            },
             "type": [
                 "null",
-                "string"
+                "array"
             ]
         },
-        "properties_hs_user_ids_of_all_owners": {
+        "formType": {
+            "description": "Type of the form.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_hubspot_owner_assigneddate": {
-            "format": "date-time",
+        "id": {
+            "description": "Unique identifier for the form.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "properties_hubspot_owner_id": {
+        "legalConsentOptions": {
+            "description": "Legal consent options for the form.",
             "type": [
                 "null",
-                "string"
+                "object"
             ]
         },
-        "properties_hubspot_team_id": {
+        "name": {
+            "description": "Name of the form.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "tickets": {
-            "items": {
-                "type": [
-                    "null",
-                    "string"
-                ]
-            },
-            "type": [
-                "null",
-                "array"
-            ]
-        },
         "updatedAt": {
+            "description": "Date and time when the form was last updated.",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         }
     },
```

### Comparing `airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/schemas/engagements_notes.json` & `airbyte_source_hubspot-4.1.2/source_hubspot/schemas/feedback_submissions.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8514777131782946%*

 * *Differences: {"'properties'": "{'id': {'description': 'Unique identifier for the feedback submission.'}, "*

 * *                 "'properties': {'type': ['null', 'object'], 'properties': "*

 * *                 "{'hs_all_assigned_business_unit_ids': {'description': 'IDs of business units "*

 * *                 "assigned to the submission.'}, 'hs_created_by_user_id': {'type': {insert: [(1, "*

 * *                 "'string')], delete: [1]}, 'description': 'ID of the user who created the "*

 * *                 "submission.'}, 'hs_createdate': {' […]*

```diff
@@ -1,487 +1,268 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
     "properties": {
         "archived": {
+            "description": "Indicates if the feedback submission is archived or not.",
             "type": [
                 "null",
                 "boolean"
             ]
         },
-        "companies": {
-            "items": {
-                "type": [
-                    "null",
-                    "string"
-                ]
-            },
+        "archivedAt": {
+            "description": "The timestamp when the feedback submission was archived.",
+            "format": "date-time",
             "type": [
                 "null",
-                "array"
+                "string"
             ]
         },
         "contacts": {
+            "description": "List of contacts associated with the feedback submission.",
             "items": {
                 "type": [
                     "null",
                     "string"
                 ]
             },
             "type": [
                 "null",
                 "array"
             ]
         },
         "createdAt": {
+            "description": "The timestamp when the feedback submission was created.",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "deals": {
-            "items": {
-                "type": [
-                    "null",
-                    "string"
-                ]
-            },
-            "type": [
-                "null",
-                "array"
-            ]
-        },
         "id": {
+            "description": "Unique identifier for the feedback submission.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "properties": {
+            "description": "Additional properties related to the feedback submission.",
             "properties": {
                 "hs_all_accessible_team_ids": {
+                    "description": "IDs of teams that have access to the submission.",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
                 "hs_all_assigned_business_unit_ids": {
+                    "description": "IDs of business units assigned to the submission.",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "hs_all_owner_ids": {
+                "hs_contact_email_rollup": {
+                    "description": "Rollup of contact email addresses associated.",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "hs_all_team_ids": {
+                "hs_contact_id": {
+                    "description": "ID of the contact related to the submission.",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "hs_at_mentioned_owner_ids": {
+                "hs_content": {
+                    "description": "Content of the feedback submission.",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "hs_attachment_ids": {
+                "hs_created_by_user_id": {
+                    "description": "ID of the user who created the submission.",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "hs_body_preview": {
+                "hs_createdate": {
+                    "description": "The date when the submission was created.",
+                    "format": "date-time",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "hs_body_preview_html": {
+                "hs_engagement_id": {
+                    "description": "ID of the engagement associated with the submission.",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "hs_body_preview_is_truncated": {
-                    "type": [
-                        "null",
-                        "boolean"
-                    ]
-                },
-                "hs_created_by": {
-                    "type": [
-                        "null",
-                        "number"
-                    ]
-                },
-                "hs_created_by_user_id": {
-                    "type": [
-                        "null",
-                        "number"
-                    ]
-                },
-                "hs_createdate": {
-                    "format": "date-time",
+                "hs_form_guid": {
+                    "description": "GUID of the form used for the submission.",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "hs_engagement_source": {
+                "hs_ingestion_id": {
+                    "description": "ID of the ingestion associated with the submission.",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "hs_engagement_source_id": {
+                "hs_knowledge_article_id": {
+                    "description": "ID of the knowledge article linked.",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "hs_follow_up_action": {
+                "hs_lastmodifieddate": {
+                    "description": "The date when the submission was last modified.",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "hs_gdpr_deleted": {
+                "hs_merged_object_ids": {
+                    "description": "IDs of merged objects related to the submission.",
                     "type": [
                         "null",
-                        "boolean"
+                        "string"
                     ]
                 },
-                "hs_lastmodifieddate": {
-                    "format": "date-time",
+                "hs_object_id": {
+                    "description": "ID of the object associated with the submission.",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "hs_merged_object_ids": {
+                "hs_response_group": {
+                    "description": "The group associated with the response.",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "hs_modified_by": {
+                "hs_submission_name": {
+                    "description": "Name of the feedback submission.",
                     "type": [
                         "null",
-                        "number"
+                        "string"
                     ]
                 },
-                "hs_note_body": {
+                "hs_submission_timestamp": {
+                    "description": "Timestamp of the submission.",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "hs_object_id": {
+                "hs_submission_url": {
+                    "description": "URL of the feedback submission.",
                     "type": [
                         "null",
-                        "number"
+                        "string"
                     ]
                 },
-                "hs_product_name": {
+                "hs_survey_channel": {
+                    "description": "Channel through which the survey was conducted.",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "hs_queue_membership_ids": {
+                "hs_survey_id": {
+                    "description": "ID of the survey associated with the submission.",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "hs_timestamp": {
-                    "format": "date-time",
+                "hs_survey_name": {
+                    "description": "Name of the survey linked to the submission.",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "hs_unique_creation_key": {
+                "hs_survey_type": {
+                    "description": "Type of the survey conducted.",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "hs_unique_id": {
+                "hs_unique_creation_key": {
+                    "description": "Unique key identifying the creation.",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
                 "hs_updated_by_user_id": {
+                    "description": "ID of the user who last updated the submission.",
                     "type": [
                         "null",
-                        "number"
+                        "string"
                     ]
                 },
                 "hs_user_ids_of_all_notification_followers": {
+                    "description": "User IDs of all followers receiving notifications.",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
                 "hs_user_ids_of_all_notification_unfollowers": {
+                    "description": "User IDs of all followers who stopped notifications.",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
                 "hs_user_ids_of_all_owners": {
+                    "description": "User IDs of all owners of the submission.",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "hubspot_owner_assigneddate": {
-                    "format": "date-time",
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "hubspot_owner_id": {
+                "hs_value": {
+                    "description": "Value provided in the feedback submission.",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "hubspot_team_id": {
+                "hs_visitor_id": {
+                    "description": "ID of the visitor associated with the submission.",
                     "type": [
                         "null",
                         "string"
                     ]
                 }
             },
-            "type": "object"
-        },
-        "properties_hs_all_accessible_team_ids": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_all_assigned_business_unit_ids": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_all_owner_ids": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_all_team_ids": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_at_mentioned_owner_ids": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_attachment_ids": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_body_preview": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_body_preview_html": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_body_preview_is_truncated": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
-        "properties_hs_created_by": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "properties_hs_created_by_user_id": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "properties_hs_createdate": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_engagement_source": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_engagement_source_id": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_follow_up_action": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_gdpr_deleted": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
-        "properties_hs_lastmodifieddate": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_merged_object_ids": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_modified_by": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "properties_hs_note_body": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_object_id": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "properties_hs_product_name": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_queue_membership_ids": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_timestamp": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_unique_creation_key": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_unique_id": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_updated_by_user_id": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "properties_hs_user_ids_of_all_notification_followers": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_user_ids_of_all_notification_unfollowers": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hs_user_ids_of_all_owners": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hubspot_owner_assigneddate": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hubspot_owner_id": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "properties_hubspot_team_id": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "tickets": {
-            "items": {
-                "type": [
-                    "null",
-                    "string"
-                ]
-            },
             "type": [
                 "null",
-                "array"
+                "object"
             ]
         },
         "updatedAt": {
+            "description": "The timestamp of the last update made to the feedback submission.",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         }
     },
```

### Comparing `airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/schemas/ticket_pipelines.json` & `airbyte_source_hubspot-4.1.2/source_hubspot/schemas/tickets.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8861111111111111%*

 * *Differences: {"'properties'": "{'id': {'description': 'Unique identifier for the ticket'}, 'archived': "*

 * *                 "{'description': 'Indicates if the ticket is archived or not'}, 'createdAt': "*

 * *                 "{'description': 'Date and time when the ticket was created'}, 'updatedAt': "*

 * *                 "{'description': 'Date and time when the ticket was last updated'}, 'contacts': "*

 * *                 "OrderedDict([('description', 'Contacts associated with the ticket'), ('type', "*

 * *                 "['null', 'arra […]*

```diff
@@ -1,126 +1,76 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
     "properties": {
         "archived": {
+            "description": "Indicates if the ticket is archived or not",
             "type": [
                 "null",
                 "boolean"
             ]
         },
-        "createdAt": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "displayOrder": {
+        "companies": {
+            "description": "Companies associated with the ticket",
+            "items": {
+                "description": "Company data",
+                "type": [
+                    "null",
+                    "string"
+                ]
+            },
             "type": [
                 "null",
-                "integer"
+                "array"
             ]
         },
-        "id": {
+        "contacts": {
+            "description": "Contacts associated with the ticket",
+            "items": {
+                "description": "Contact data",
+                "type": [
+                    "null",
+                    "integer"
+                ]
+            },
             "type": [
                 "null",
-                "string"
+                "array"
             ]
         },
-        "label": {
+        "createdAt": {
+            "description": "Date and time when the ticket was created",
+            "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "stages": {
+        "deals": {
+            "description": "Deals associated with the ticket",
             "items": {
-                "properties": {
-                    "active": {
-                        "type": [
-                            "null",
-                            "boolean"
-                        ]
-                    },
-                    "archived": {
-                        "type": [
-                            "null",
-                            "boolean"
-                        ]
-                    },
-                    "createdAt": {
-                        "format": "date-time",
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "displayOrder": {
-                        "type": [
-                            "null",
-                            "integer"
-                        ]
-                    },
-                    "id": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "label": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "metadata": {
-                        "properties": {
-                            "isClosed": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            },
-                            "ticketState": {
-                                "type": [
-                                    "null",
-                                    "string"
-                                ]
-                            }
-                        },
-                        "type": [
-                            "null",
-                            "object"
-                        ]
-                    },
-                    "updatedAt": {
-                        "format": "date-time",
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    },
-                    "writePermissions": {
-                        "type": [
-                            "null",
-                            "string"
-                        ]
-                    }
-                },
+                "description": "Deal data",
                 "type": [
                     "null",
-                    "object"
+                    "string"
                 ]
             },
             "type": [
                 "null",
                 "array"
             ]
         },
+        "id": {
+            "description": "Unique identifier for the ticket",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
         "updatedAt": {
+            "description": "Date and time when the ticket was last updated",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         }
     },
```

### Comparing `airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/source.py` & `airbyte_source_hubspot-4.1.2/source_hubspot/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/spec.yaml` & `airbyte_source_hubspot-4.1.2/source_hubspot/spec.yaml`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.1.dev202404292128/source_hubspot/streams.py` & `airbyte_source_hubspot-4.1.2/source_hubspot/streams.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 import backoff
 import pendulum as pendulum
 import requests
 from airbyte_cdk.entrypoint import logger
 from airbyte_cdk.models import FailureType, SyncMode
 from airbyte_cdk.sources import Source
-from airbyte_cdk.sources.streams import IncrementalMixin, StateMixin, Stream
+from airbyte_cdk.sources.streams import IncrementalMixin, Stream
 from airbyte_cdk.sources.streams.availability_strategy import AvailabilityStrategy
 from airbyte_cdk.sources.streams.core import StreamData
 from airbyte_cdk.sources.streams.http import HttpStream, HttpSubStream
 from airbyte_cdk.sources.streams.http.availability_strategy import HttpAvailabilityStrategy
 from airbyte_cdk.sources.streams.http.requests_native_auth import Oauth2Authenticator, TokenAuthenticator
 from airbyte_cdk.sources.utils import casing
 from airbyte_cdk.sources.utils.schema_helpers import ResourceSchemaLoader
@@ -1228,15 +1228,15 @@
 
             return {"params": params, "payload": payload}
 
     def stream_slices(
         self, *, sync_mode: SyncMode, cursor_field: List[str] = None, stream_state: Mapping[str, Any] = None
     ) -> Iterable[Optional[Mapping[str, Any]]]:
         self.set_sync(sync_mode, stream_state)
-        return [{}]  # I changed this from [None] since this is a more accurate depiction of what is actually being done. Sync one slice
+        return [None]
 
     def set_sync(self, sync_mode: SyncMode, stream_state):
         self._sync_mode = sync_mode
         if self._sync_mode == SyncMode.incremental:
             if stream_state:
                 if not self._state:
                     self._state = self._start_date
@@ -1357,93 +1357,27 @@
     limit_field = "count"
     primary_key = "listId"
     need_chunk = False
     scopes = {"crm.lists.read"}
     unnest_fields = ["metaData"]
 
 
-class ContactsAllBase(Stream, StateMixin):
+class ContactsAllBase(Stream):
     url = "/contacts/v1/lists/all/contacts/all"
     updated_at_field = "timestamp"
     more_key = "has-more"
     data_field = "contacts"
     page_filter = "vidOffset"
     page_field = "vid-offset"
     primary_key = "canonical-vid"
     scopes = {"crm.objects.contacts.read"}
     properties_scopes = {"crm.schemas.contacts.read"}
     records_field = None
     filter_field = None
     filter_value = None
-    _state = {}
-    limit_field = "count"
-    limit = 100
-    _record_count = 0
-
-    @property
-    def state(self) -> MutableMapping[str, Any]:
-        return self._state
-
-    @state.setter
-    def state(self, value: MutableMapping[str, Any]) -> None:
-        self._state = value
-
-    def read_records(
-        self,
-        sync_mode: SyncMode,
-        cursor_field: List[str] = None,
-        stream_slice: Mapping[str, Any] = None,
-        stream_state: Mapping[str, Any] = None,
-    ) -> Iterable[Mapping[str, Any]]:
-        """
-        This is a specialized read_records for resumable full refresh that only attempts to read a single page of records
-        at a time and updates the state w/ a synthetic cursor based on the Hubspot cursor pagination value `vidOffset`
-        """
-        if self._records_count >= 1800:
-            raise ValueError(f"Failing beause more than 1800 records were read")
-
-        next_page_token = stream_slice
-        logger.info(f"Read in self.state and setting next_page_token to: f{next_page_token}")
-        try:
-            properties = self._property_wrapper
-            if properties and properties.too_many_properties:
-                records, response = self._read_stream_records(
-                    stream_slice=stream_slice,
-                    stream_state=stream_state,
-                    next_page_token=next_page_token,
-                )
-            else:
-                response = self.handle_request(
-                    stream_slice=stream_slice,
-                    stream_state=stream_state,
-                    next_page_token=next_page_token,
-                    properties=properties,
-                )
-                records = self._transform(self.parse_response(response, stream_state=stream_state, stream_slice=stream_slice))
-                
-            records = list(records)
-            self._records_count += records
-
-
-            if self.filter_old_records:
-                records = self._filter_old_records(records)
-            yield from self.record_unnester.unnest(records)
-
-            # todo blai: This is how the gotcha mentioned in the RFR checkpoint reader manifests that the developer must know to
-            #  set state as the empty. Although the state setter expects a real value so maybe this isn't the worst interface
-            self.state = self.next_page_token(response) or {}
-
-            # Always return an empty generator just in case no records were ever yielded
-            yield from []
-        except requests.exceptions.HTTPError as e:
-            response = e.response
-            if response.status_code == HTTPStatus.UNAUTHORIZED:
-                raise AirbyteTracedException("The authentication to HubSpot has expired. Re-authenticate to restore access to HubSpot.")
-            else:
-                raise e
 
     def _transform(self, records: Iterable) -> Iterable:
         for record in super()._transform(records):
             canonical_vid = record.get("canonical-vid")
             for item in record.get(self.records_field, []):
                 yield {"canonical-vid": canonical_vid, **item}
```

### Comparing `airbyte_source_hubspot-4.1.1.dev202404292128/PKG-INFO` & `airbyte_source_hubspot-4.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-hubspot
-Version: 4.1.1.dev202404292128
+Version: 4.1.2
 Summary: Source implementation for HubSpot.
 Home-page: https://airbyte.com
 License: ELv2
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
```

