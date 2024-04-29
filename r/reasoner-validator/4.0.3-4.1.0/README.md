# Comparing `tmp/reasoner_validator-4.0.3.tar.gz` & `tmp/reasoner_validator-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasoner_validator-4.0.3.tar", max compression
+gzip compressed data, was "reasoner_validator-4.1.0.tar", max compression
```

## Comparing `reasoner_validator-4.0.3.tar` & `reasoner_validator-4.1.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1153 2024-04-27 21:11:06.974750 reasoner_validator-4.0.3/LICENSE
--rw-r--r--   0        0        0    13727 2024-04-27 21:11:06.974750 reasoner_validator-4.0.3/README.md
--rw-r--r--   0        0        0      131 2024-04-27 21:11:06.974750 reasoner_validator-4.0.3/docs/.nojekyll
--rw-r--r--   0        0        0      634 2024-04-27 21:11:06.974750 reasoner_validator-4.0.3/docs/Makefile
--rw-r--r--   0        0        0     2291 2024-04-27 21:11:06.974750 reasoner_validator-4.0.3/docs/conf.py
--rw-r--r--   0        0        0    20365 2024-04-27 21:11:06.974750 reasoner_validator-4.0.3/docs/index.rst
--rw-r--r--   0        0        0      795 2024-04-27 21:11:06.974750 reasoner_validator-4.0.3/docs/make.bat
--rw-r--r--   0        0        0      136 2024-04-27 21:11:06.974750 reasoner_validator-4.0.3/docs/reasoner_validator.biolink.rst
--rw-r--r--   0        0        0      135 2024-04-27 21:11:06.974750 reasoner_validator-4.0.3/docs/reasoner_validator.report.rst
--rw-r--r--   0        0        0      152 2024-04-27 21:11:06.974750 reasoner_validator-4.0.3/docs/reasoner_validator.rst
--rw-r--r--   0        0        0      146 2024-04-27 21:11:06.974750 reasoner_validator-4.0.3/docs/reasoner_validator.trapi.mapping.rst
--rw-r--r--   0        0        0      144 2024-04-27 21:11:06.974750 reasoner_validator-4.0.3/docs/reasoner_validator.trapi.rst
--rw-r--r--   0        0        0      163 2024-04-27 21:11:06.974750 reasoner_validator-4.0.3/docs/reasoner_validator.validation_codes.rst
--rw-r--r--   0        0        0      157 2024-04-27 21:11:06.974750 reasoner_validator-4.0.3/docs/reasoner_validator.versioning.rst
--rw-r--r--   0        0        0    39468 2024-04-27 21:11:06.978750 reasoner_validator-4.0.3/docs/validation_codes_dictionary.md
--rw-r--r--   0        0        0     2299 2024-04-27 21:11:06.978750 reasoner_validator-4.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-27 21:11:06.978750 reasoner_validator-4.0.3/reasoner_validator/__init__.py
--rw-r--r--   0        0        0    85875 2024-04-27 21:11:06.978750 reasoner_validator-4.0.3/reasoner_validator/biolink/__init__.py
--rw-r--r--   0        0        0    43025 2024-04-27 21:11:06.978750 reasoner_validator-4.0.3/reasoner_validator/codes.yaml
--rw-r--r--   0        0        0     1761 2024-04-27 21:11:06.978750 reasoner_validator-4.0.3/reasoner_validator/github.py
--rw-r--r--   0        0        0     3973 2024-04-27 21:11:06.978750 reasoner_validator-4.0.3/reasoner_validator/message.py
--rw-r--r--   0        0        0    46755 2024-04-27 21:11:06.978750 reasoner_validator-4.0.3/reasoner_validator/report.py
--rw-r--r--   0        0        0        0 2024-04-27 21:11:06.978750 reasoner_validator-4.0.3/reasoner_validator/sri/__init__.py
--rw-r--r--   0        0        0     4754 2024-04-27 21:11:06.978750 reasoner_validator-4.0.3/reasoner_validator/sri/util.py
--rw-r--r--   0        0        0    14288 2024-04-27 21:11:06.978750 reasoner_validator-4.0.3/reasoner_validator/trapi/__init__.py
--rw-r--r--   0        0        0     1120 2024-04-27 21:11:06.978750 reasoner_validator-4.0.3/reasoner_validator/trapi/mapping.py
--rw-r--r--   0        0        0    14745 2024-04-27 21:11:06.978750 reasoner_validator-4.0.3/reasoner_validator/validation_codes.py
--rw-r--r--   0        0        0    35564 2024-04-27 21:11:06.978750 reasoner_validator-4.0.3/reasoner_validator/validator.py
--rw-r--r--   0        0        0    11943 2024-04-27 21:11:06.978750 reasoner_validator-4.0.3/reasoner_validator/versioning.py
--rw-r--r--   0        0        0      838 2024-04-27 21:11:06.978750 reasoner_validator-4.0.3/reasoner_validator/versions.yaml
--rw-r--r--   0        0        0     2407 2024-04-27 21:11:06.978750 reasoner_validator-4.0.3/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-04-27 21:11:06.978750 reasoner_validator-4.0.3/tests/conftest.py
--rw-r--r--   0        0        0   138310 2024-04-27 21:11:06.978750 reasoner_validator-4.0.3/tests/test_biolink_compliance_validation.py
--rw-r--r--   0        0        0    62107 2024-04-27 21:11:06.982750 reasoner_validator-4.0.3/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml
--rw-r--r--   0        0        0    41247 2024-04-27 21:11:06.982750 reasoner_validator-4.0.3/tests/test_response_validator.py
--rw-r--r--   0        0        0     6157 2024-04-27 21:11:06.982750 reasoner_validator-4.0.3/tests/test_semver.py
--rw-r--r--   0        0        0     2248 2024-04-27 21:11:06.982750 reasoner_validator-4.0.3/tests/test_trapi_versioning.py
--rw-r--r--   0        0        0    27195 2024-04-27 21:11:06.982750 reasoner_validator-4.0.3/tests/test_validate.py
--rw-r--r--   0        0        0    30223 2024-04-27 21:11:06.982750 reasoner_validator-4.0.3/tests/test_validation_report.py
--rw-r--r--   0        0        0     2734 2024-04-27 21:11:06.982750 reasoner_validator-4.0.3/tests/test_workflows.py
--rw-r--r--   0        0        0    15266 1970-01-01 00:00:00.000000 reasoner_validator-4.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1153 2024-04-29 23:47:45.453401 reasoner_validator-4.1.0/LICENSE
+-rw-r--r--   0        0        0    13727 2024-04-29 23:47:45.453401 reasoner_validator-4.1.0/README.md
+-rw-r--r--   0        0        0      131 2024-04-29 23:47:45.453401 reasoner_validator-4.1.0/docs/.nojekyll
+-rw-r--r--   0        0        0      634 2024-04-29 23:47:45.453401 reasoner_validator-4.1.0/docs/Makefile
+-rw-r--r--   0        0        0     2291 2024-04-29 23:47:45.453401 reasoner_validator-4.1.0/docs/conf.py
+-rw-r--r--   0        0        0    20365 2024-04-29 23:47:45.453401 reasoner_validator-4.1.0/docs/index.rst
+-rw-r--r--   0        0        0      795 2024-04-29 23:47:45.453401 reasoner_validator-4.1.0/docs/make.bat
+-rw-r--r--   0        0        0      136 2024-04-29 23:47:45.453401 reasoner_validator-4.1.0/docs/reasoner_validator.biolink.rst
+-rw-r--r--   0        0        0      135 2024-04-29 23:47:45.453401 reasoner_validator-4.1.0/docs/reasoner_validator.report.rst
+-rw-r--r--   0        0        0      152 2024-04-29 23:47:45.453401 reasoner_validator-4.1.0/docs/reasoner_validator.rst
+-rw-r--r--   0        0        0      146 2024-04-29 23:47:45.453401 reasoner_validator-4.1.0/docs/reasoner_validator.trapi.mapping.rst
+-rw-r--r--   0        0        0      144 2024-04-29 23:47:45.453401 reasoner_validator-4.1.0/docs/reasoner_validator.trapi.rst
+-rw-r--r--   0        0        0      163 2024-04-29 23:47:45.453401 reasoner_validator-4.1.0/docs/reasoner_validator.validation_codes.rst
+-rw-r--r--   0        0        0      157 2024-04-29 23:47:45.453401 reasoner_validator-4.1.0/docs/reasoner_validator.versioning.rst
+-rw-r--r--   0        0        0    42104 2024-04-29 23:47:45.453401 reasoner_validator-4.1.0/docs/validation_codes_dictionary.md
+-rw-r--r--   0        0        0     2299 2024-04-29 23:47:45.457401 reasoner_validator-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-29 23:47:45.457401 reasoner_validator-4.1.0/reasoner_validator/__init__.py
+-rw-r--r--   0        0        0    94021 2024-04-29 23:47:45.457401 reasoner_validator-4.1.0/reasoner_validator/biolink/__init__.py
+-rw-r--r--   0        0        0    45890 2024-04-29 23:47:45.457401 reasoner_validator-4.1.0/reasoner_validator/codes.yaml
+-rw-r--r--   0        0        0     1761 2024-04-29 23:47:45.457401 reasoner_validator-4.1.0/reasoner_validator/github.py
+-rw-r--r--   0        0        0     3973 2024-04-29 23:47:45.457401 reasoner_validator-4.1.0/reasoner_validator/message.py
+-rw-r--r--   0        0        0    46755 2024-04-29 23:47:45.457401 reasoner_validator-4.1.0/reasoner_validator/report.py
+-rw-r--r--   0        0        0        0 2024-04-29 23:47:45.457401 reasoner_validator-4.1.0/reasoner_validator/sri/__init__.py
+-rw-r--r--   0        0        0     4754 2024-04-29 23:47:45.457401 reasoner_validator-4.1.0/reasoner_validator/sri/util.py
+-rw-r--r--   0        0        0    15057 2024-04-29 23:47:45.457401 reasoner_validator-4.1.0/reasoner_validator/trapi/__init__.py
+-rw-r--r--   0        0        0     1120 2024-04-29 23:47:45.457401 reasoner_validator-4.1.0/reasoner_validator/trapi/mapping.py
+-rw-r--r--   0        0        0    14745 2024-04-29 23:47:45.457401 reasoner_validator-4.1.0/reasoner_validator/validation_codes.py
+-rw-r--r--   0        0        0    35576 2024-04-29 23:47:45.457401 reasoner_validator-4.1.0/reasoner_validator/validator.py
+-rw-r--r--   0        0        0    12127 2024-04-29 23:47:45.457401 reasoner_validator-4.1.0/reasoner_validator/versioning.py
+-rw-r--r--   0        0        0      866 2024-04-29 23:47:45.457401 reasoner_validator-4.1.0/reasoner_validator/versions.yaml
+-rw-r--r--   0        0        0     3601 2024-04-29 23:47:45.457401 reasoner_validator-4.1.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 23:47:45.457401 reasoner_validator-4.1.0/tests/conftest.py
+-rw-r--r--   0        0        0   145466 2024-04-29 23:47:45.457401 reasoner_validator-4.1.0/tests/test_biolink_compliance_validation.py
+-rw-r--r--   0        0        0    62107 2024-04-29 23:47:45.461401 reasoner_validator-4.1.0/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml
+-rw-r--r--   0        0        0    41308 2024-04-29 23:47:45.461401 reasoner_validator-4.1.0/tests/test_response_validator.py
+-rw-r--r--   0        0        0     6157 2024-04-29 23:47:45.461401 reasoner_validator-4.1.0/tests/test_semver.py
+-rw-r--r--   0        0        0     2248 2024-04-29 23:47:45.461401 reasoner_validator-4.1.0/tests/test_trapi_versioning.py
+-rw-r--r--   0        0        0    36620 2024-04-29 23:47:45.461401 reasoner_validator-4.1.0/tests/test_validate.py
+-rw-r--r--   0        0        0    30223 2024-04-29 23:47:45.461401 reasoner_validator-4.1.0/tests/test_validation_report.py
+-rw-r--r--   0        0        0     3411 2024-04-29 23:47:45.461401 reasoner_validator-4.1.0/tests/test_workflows.py
+-rw-r--r--   0        0        0    15266 1970-01-01 00:00:00.000000 reasoner_validator-4.1.0/PKG-INFO
```

### Comparing `reasoner_validator-4.0.3/LICENSE` & `reasoner_validator-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.3/README.md` & `reasoner_validator-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.3/docs/Makefile` & `reasoner_validator-4.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.3/docs/conf.py` & `reasoner_validator-4.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.3/docs/index.rst` & `reasoner_validator-4.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.3/docs/make.bat` & `reasoner_validator-4.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.3/docs/validation_codes_dictionary.md` & `reasoner_validator-4.1.0/docs/validation_codes_dictionary.md`

 * *Files 3% similar despite different names*

```diff
@@ -620,23 +620,23 @@
 
 **Description:** The 'attribute_type_id' of a Knowledge graph edge attribute must be a controlled vocabulary term specified by a CURIE!
 
 ### error.knowledge_graph.edge.attribute.value.missing
 
 **Message:** An attribute is missing its 'value' property in Edge
 
-**Context:** identifier
+**Context:** identifier, attribute_id
 
 **Description:** An attribute of a Knowledge graph edge must have a 'value' key with a non-empty associated value!
 
 ### error.knowledge_graph.edge.attribute.value.empty
 
 **Message:** An attribute has an empty value in Edge
 
-**Context:** identifier
+**Context:** identifier, attribute_id
 
 **Description:** The value of an attribute of a Knowledge graph edge must not be empty!
 
 ### error.knowledge_graph.edge.provenance.infores.missing
 
 **Message:** Edge has provenance value which is not a well-formed InfoRes CURIE
 
@@ -688,14 +688,62 @@
 
 **Message:** Validation of qualifier in qualifiers threw an unexpected exception
 
 **Context:** identifier, qualifier_type_id, qualifier_value, reason
 
 **Description:** Validation of a specified 'qualifier_type_id' and 'qualifier_value' failed for a given exceptional reason!
 
+### error.knowledge_graph.edge.knowledge_level.missing
+
+**Message:** Edge is missing its required 'knowledge_level' property!
+
+**Context:** edge_id
+
+**Description:** The 'knowledge_level' slot is required for all edges in knowledge graphs complying with the specified TRAPI and Biolink Model release!
+
+### error.knowledge_graph.edge.knowledge_level.duplicated
+
+**Message:** The 'knowledge_level' slot is duplicated for the given edge!
+
+**Context:** identifier, edge_id
+
+**Description:** Each edge should only have one 'knowledge_level' attribute value. Additional ones are ignored
+
+### error.knowledge_graph.edge.knowledge_level.invalid
+
+**Message:** The indicated 'knowledge_level' slot value is invalid for the given edge!
+
+**Context:** identifier, context
+
+**Description:** Acceptable values of the 'knowledge_level' slot are only as enumerated in the specified Biolink Model
+
+### error.knowledge_graph.edge.agent_type.missing
+
+**Message:** Edge is missing its required 'agent_type' property!
+
+**Context:** identifier
+
+**Description:** The 'agent_type' slot is required for all edges in knowledge graphs complying with the specified Biolink Model release!
+
+### error.knowledge_graph.edge.agent_type.duplicated
+
+**Message:** The 'agent_type' slot is duplicated for the given edge!
+
+**Context:** identifier, edge_id
+
+**Description:** Each edge should only have one 'agent_type' attribute value. Additional ones are ignored.
+
+### error.knowledge_graph.edge.agent_type.invalid
+
+**Message:** The indicated 'agent_type' slot value is invalid for the given edge!
+
+**Context:** identifier, context
+
+**Description:** Acceptable values of the 'agent_type' slot are only as enumerated in the specified Biolink Model
+
 ### error.knowledge_graph.edge.sources.missing
 
 **Message:** Missing 'sources' key for Edge
 
 **Context:** identifier
 
 **Description:** Edge must have a 'sources' key with a non-empty associated value!
@@ -794,14 +842,22 @@
 
 **Context:** identifier
 
 **Description:** Value of the 'resource_role' property in the RetrievalSource of a Knowledge Graph Edge must be a non-empty ResourceRole enum value!
 
 ## Warning
 
+### warning.biolink.element.range.unspecified
+
+**Message:** Undefined slot range specification
+
+**Context:** identifier, context, value
+
+**Description:** Biolink Model error: the range slot of the specified element is missing or its value is not a known enum?
+
 ### warning.trapi.response.status.unknown
 
 **Message:** TRAPI Response has unrecognized status code
 
 **Context:** identifier
 
 **Description:** The TRAPI Response status code should be one of a standardized set of short codes, e.g. Success, QueryNotTraversable, KPsNotAvailable
@@ -1062,14 +1118,30 @@
 
 **Message:** Edge attribute values are missing expected Knowledge Provider provenance
 
 **Context:** edge_id, identifier, kp_source_type
 
 **Description:** Edge attributes of ARAs and KPs should record the infores identifier of their knowledge source provenance with respect to KP.
 
+### warning.knowledge_graph.edge.knowledge_level.missing
+
+**Message:** Edge is missing its required 'knowledge_level' property!
+
+**Context:** edge_id
+
+**Description:** The 'knowledge_level' slot is currently optional but recommended for all edges in knowledge graphs complying with the specified TRAPI and Biolink Model release!
+
+### warning.knowledge_graph.edge.agent_type.missing
+
+**Message:** Edge is missing its required 'agent_type' property!
+
+**Context:** identifier
+
+**Description:** The 'agent_type' slot is currently optional but recommended for all edges in knowledge graphs complying with the specified Biolink Model release!
+
 ## Information
 
 ### info.excluded
 
 **Message:** All test case S-P-O triples from resource test location, or specific user excluded S-P-O triples
 
 **Context:** identifier
```

### Comparing `reasoner_validator-4.0.3/pyproject.toml` & `reasoner_validator-4.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reasoner-validator"
-version = "4.0.3"
+version = "4.1.0"
 description = "Validation tools for Reasoner API"
 authors = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
     "Patrick Wang <patrickelvin@gmail.com>"
 ]
 maintainers = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
```

### Comparing `reasoner_validator-4.0.3/reasoner_validator/biolink/__init__.py` & `reasoner_validator-4.1.0/reasoner_validator/biolink/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 from bmt import Toolkit, utils
 from linkml_runtime.linkml_model import ClassDefinition, Element
 
 from reasoner_validator.sri.util import is_curie
 from reasoner_validator.versioning import SemVer, SemVerError
-from reasoner_validator.message import MESSAGE_CATALOG
+from reasoner_validator.message import MESSAGES_BY_TARGET
 from reasoner_validator.trapi import TRAPISchemaValidator
 from reasoner_validator.report import TRAPIGraphType
 
 import logging
 logger = logging.getLogger(__name__)
 
 pp = PrettyPrinter(indent=4)
@@ -242,22 +242,22 @@
 
     def count_node(self, node_id: str):
         self.nodes[node_id][1] += 1
 
     def has_dangling_nodes(self) -> List[str]:
         return [node_id for node_id, entry in self.nodes.items() if not entry[1]]
 
-    def get_result(self) -> Tuple[str, MESSAGE_CATALOG]:
+    def get_result(self) -> Tuple[str, MESSAGES_BY_TARGET]:
         """
         Get result of validation.
 
         :return: model version of the validation and dictionary of reported validation messages.
         :rtype Tuple[str, Optional[Dict[str, Set[str]]]]
         """
-        return self.bmt.get_model_version(), self.get_messages()
+        return self.bmt.get_model_version(), super().get_all_messages()
 
     def validate_graph_node(self, node_id: str, slots: Dict[str, Any], graph_type: TRAPIGraphType):
         """
         Validate slot properties (mainly 'categories') of a node.
 
         :param node_id: str, identifier of a concept node
         :param slots: Dict, properties of the node
@@ -592,19 +592,111 @@
             self.report(
                 code="warning.knowledge_graph.edge.provenance.multiple_primary",
                 source_trail=source_trail,
                 identifier=edge_id,
                 sources=",".join(found_primary_knowledge_source)
             )
 
-    # TODO: 13-July-2023: Certain attribute_type_id's are slated for future implementation in the Biolink Model
-    #                     but not in the current model release; however, some teams have started to use the terms.
-    #                     We therefore put them on a special "inclusion list" (like the CATEGORY_INCLUSIONS below)
-    #                     to permit them to pass through the validation without any complaints.
-    ATTRIBUTE_TYPE_ID_INCLUSIONS = ["biolink:knowledge_level", "biolink:agent_type"]
+    def validate_slot_value(
+            self,
+            slot_name: str,
+            context: str,
+            found: bool,
+            value: Optional[str]
+    ) -> bool:
+        """
+        Validate the single-valued value of a specified slot of the given knowledge graph entity slot.
+        :param slot_name, str, name of a valid slot, a value for which is to be validated
+        :param context: str, context of the validation (e.g. node or edge id)
+        :param found: bool, current status of slot detection,
+                      Should be true if the slot was already previously seen
+        :param value: Optional[str], the value to be validated
+        :return: bool, True if valid slot and value (validation messages recorded in the BiolinkValidator)
+        """
+        if found:
+            # The slot was already encountered in this element,
+            # hence report the duplication with its value?
+            self.report(
+                code=f"error.knowledge_graph.edge.{slot_name}.duplicated",
+                identifier=context,
+                value=str(value)
+            )
+            # we'll be forgiving here and just assume
+            # that the first slot value was acceptable.
+            return True
+
+        slot_element = self.bmt.get_element(f"biolink:{slot_name}")
+        assert slot_element, f"No such slot {slot_name} element in Biolink Model release {self.biolink_version}"
+
+        # Note: we don't need to check for empty attribute.values
+        # here since done elsewhere in the code base
+
+        # Validate slot value here against the specified slot range Enum
+        if "range" in slot_element and slot_element.range:
+            value_range = slot_element.range
+            if value_range and self.bmt.is_enum(value_range):
+                enum = self.bmt.view.get_enum(value_range)
+                if not self.bmt.is_permissible_value_of_enum(enum.name, value):
+                    self.report(
+                        code=f"error.knowledge_graph.edge.{slot_name}.invalid",
+                        identifier=str(value),
+                        context=context
+                    )
+                    return False
+                else:
+                    # if this passes all the gauntlets, assert
+                    # that the slot and its value were found
+                    return True
+
+        # Catch this as a warning against a missing
+        # Biolink Model element range specification
+        self.report(
+            code=f"warning.biolink.element.range.unspecified",
+            identifier=slot_name,
+            context=context,
+            value=str(value)
+        )
+        return False
+
+    def validate_knowledge_level(
+            self,
+            edge_id: str,
+            found: bool,
+            value: Optional[str]
+    ) -> bool:
+        """
+        Validate the value of a 'knowledge_level' of the given edge.
+        :param edge_id: str, identifier of the edge being validated
+        :param found: bool, current status of slot detection, True if already seen previously (return 'True' value here)
+        :param value: Optional[str], the value to be validated
+        :return: bool, if valid slot and value found (validation messages recorded in the BiolinkValidator)
+        """
+        return self.validate_slot_value(slot_name="knowledge_level", context=edge_id, found=found, value=value)
+
+    def validate_agent_type(
+            self,
+            edge_id: str,
+            found: bool,
+            value: Optional[str]
+    ) -> bool:
+        """
+        Validate the value of a 'agent_type' of the given edge.
+        :param edge_id: str, identifier of the edge being validated
+        :param found: bool, current status of slot detection, True if already seen previously (return 'True' value here)
+        :param value: Optional[str], the value to be validated
+        :return: None (validation messages recorded in the BiolinkValidator)
+        """
+        return self.validate_slot_value(slot_name="agent_type", context=edge_id, found=found, value=value)
+
+    # 13-July-2023: Certain attribute_type_id's are slated for future implementation in the Biolink Model
+    #               but not in the current model release; however, some teams have started to use the terms.
+    #               We therefore put them on a special "inclusion list" (like the CATEGORY_INCLUSIONS below)
+    #               to permit them to pass through the validation without any complaints.
+    # ATTRIBUTE_TYPE_ID_INCLUSIONS = ["biolink:knowledge_level", "biolink:agent_type"]
+    ATTRIBUTE_TYPE_ID_INCLUSIONS = []
 
     def validate_attributes(
             self,
             graph_type: TRAPIGraphType,
             edge_id: str,
             edge: Dict,
             source_trail: Optional[str] = None
@@ -659,15 +751,15 @@
                 code="error.knowledge_graph.edge.attribute.not_array",
                 identifier=edge_id,
                 source_trail=source_trail
             )
         else:
             attributes = edge['attributes']
 
-            # TODO: EDeutsch feedback: maybe we don't need to capture TRAPI 1.3.0 attribute-defined 'sources'
+            # EDeutsch feedback: maybe we don't need to capture TRAPI 1.3.0 attribute-defined 'sources'
             # raise NotImplementedError("Implement capture of 'sources' from TRAPI 1.3.0 attributes!")
             # source_trail = self.build_source_trail(sources) if sources else None
 
             ara_source: Optional[str]
             kp_source: Optional[str]
             kp_source_type: Optional[str]
             ara_source, kp_source, kp_source_type = self.get_target_provenance()
@@ -675,14 +767,18 @@
             # Expecting ARA and KP 'aggregator_knowledge_source' attributes?
             found_ara_knowledge_source = False
             found_kp_knowledge_source = False
 
             # also track primary_knowledge_source attribute cardinality now
             found_primary_knowledge_source: List[str] = list()
 
+            # Track presence of 'knowledge_level' and 'agent_type' attributes
+            found_knowledge_level = False
+            found_agent_type = False
+
             for attribute in attributes:
 
                 # Validate attribute_type_id
                 if 'attribute_type_id' not in attribute:
                     self.report(
                         code="error.knowledge_graph.edge.attribute.type_id.missing",
                         identifier=edge_id,
@@ -690,149 +786,170 @@
                     )
                 elif not attribute['attribute_type_id']:
                     self.report(
                         code="error.knowledge_graph.edge.attribute.type_id.empty",
                         identifier=edge_id,
                         source_trail=source_trail
                     )
-                elif 'value' not in attribute:
-                    self.report(
-                        code="error.knowledge_graph.edge.attribute.value.missing",
-                        identifier=edge_id,
-                        source_trail=source_trail
-                    )
-                elif isinstance(attribute['value'], bool) or isinstance(attribute['value'], Number):
-                    # An attribute value which is a Python bool of value 'False'
-                    # or a numeric value with value zero, is acceptable...
-                    pass
-
-                elif not attribute['value'] or \
-                        str(attribute['value']).upper() in ["N/A", "NONE", "NULL"]:
-                    # ...But not other datatype values deemed 'empty'
-                    self.report(
-                        code="error.knowledge_graph.edge.attribute.value.empty",
-                        identifier=edge_id,
-                        source_trail=source_trail
-                    )
                 else:
                     attribute_type_id: str = attribute['attribute_type_id']
-                    value = attribute['value']
-
-                    # TODO: there seems to be non-uniformity in provenance attribute values for some KP/ARA's
-                    #       in which a value is returned as a Python list (of at least one element?) instead
-                    #       of a string. Here, to ensure full coverage of the attribute values returned,
-                    #       we'll coerce scalar values into a list, then iterate.
-                    if not isinstance(value, List):
-                        value = [value]
-
-                    if not is_curie(attribute_type_id):
+                    if 'value' not in attribute:
                         self.report(
-                            code="error.knowledge_graph.edge.attribute.type_id.not_curie",
-                            identifier=attribute_type_id,
-                            edge_id=edge_id,
+                            code="error.knowledge_graph.edge.attribute.value.missing",
+                            identifier=edge_id,
+                            attribute_id=attribute_type_id,
                             source_trail=source_trail
                         )
-                    elif self.validate_biolink():
-                        # 'attribute_type_id' is a CURIE, but how well does it map?
-                        prefix = attribute_type_id.split(":", 1)[0]
-                        if prefix == 'biolink':
-                            # We will skip further validation of terms in the ATTRIBUTE_TYPE_ID_INCLUSIONS list...
-                            if attribute_type_id not in self.ATTRIBUTE_TYPE_ID_INCLUSIONS:
-
-                                # ... but further validate everything else...
-                                biolink_class = self.validate_element_status(
-                                    graph_type=graph_type,
-                                    context="knowledge_graph.edge.attribute.type_id",
+                    else:
+                        value = attribute['value']
+                        if isinstance(value, bool) or isinstance(value, Number):
+                            # An attribute value which is a Python bool of value 'False'
+                            # or a numeric value with value zero, is acceptable...
+                            pass
+
+                        # ...But not other datatype values deemed 'empty'
+                        elif not value or \
+                                str(value).upper() in ["N/A", "NONE", "NULL"]:
+                            self.report(
+                                code="error.knowledge_graph.edge.attribute.value.empty",
+                                identifier=edge_id,
+                                attribute_id=attribute_type_id,
+                                source_trail=source_trail
+                            )
+                        else:
+                            # TODO: there seems to be non-uniformity in provenance attribute values for some KP/ARA's
+                            #       in which a value is returned as a Python list (of at least one element?) instead
+                            #       of a string. Here, to ensure full coverage of the attribute values returned,
+                            #       we'll coerce scalar values into a list, then iterate.
+                            if not isinstance(value, List):
+                                value = [value]
+
+                            if not is_curie(attribute_type_id):
+                                self.report(
+                                    code="error.knowledge_graph.edge.attribute.type_id.not_curie",
                                     identifier=attribute_type_id,
                                     edge_id=edge_id,
                                     source_trail=source_trail
                                 )
-                                if biolink_class:
-                                    if self.bmt.is_category(name=biolink_class.name):
-                                        self.report(
-                                            code="warning.knowledge_graph.edge.attribute.type_id.is_category",
+                            elif self.validate_biolink():
+                                # 'attribute_type_id' is a CURIE, but how well does it map?
+                                prefix = attribute_type_id.split(":", 1)[0]
+                                if prefix == 'biolink':
+                                    # We will skip further validation of terms
+                                    # in the ATTRIBUTE_TYPE_ID_INCLUSIONS list...
+                                    if attribute_type_id not in self.ATTRIBUTE_TYPE_ID_INCLUSIONS:
+
+                                        # ... but further validate everything else...
+                                        biolink_class = self.validate_element_status(
+                                            graph_type=graph_type,
+                                            context="knowledge_graph.edge.attribute.type_id",
                                             identifier=attribute_type_id,
                                             edge_id=edge_id,
                                             source_trail=source_trail
                                         )
-                                    elif self.bmt.is_predicate(name=biolink_class.name):
-                                        self.report(
-                                            code="warning.knowledge_graph.edge.attribute.type_id.is_predicate",
-                                            identifier=attribute_type_id,
-                                            edge_id=edge_id,
-                                            source_trail=source_trail
-                                        )
-                                    elif not self.bmt.is_association_slot(attribute_type_id):
-                                        self.report(
-                                            code="warning.knowledge_graph.edge.attribute.type_id.not_association_slot",
-                                            identifier=attribute_type_id,
-                                            edge_id=edge_id,
-                                            source_trail=source_trail
-                                        )
-                                    else:
-                                        # attribute_type_id is a Biolink 'association_slot': validate it further...
-
-                                        # TODO: only check knowledge_source provenance here for now.
-                                        #       Are there other association_slots to be validated here too?
-                                        #       For example, once new terms with defined value ranges are published
-                                        #       in the Biolink Model, then perhaps 'value' validation will be feasible.
-
-                                        # Edge provenance tags only recorded in
-                                        # Edge attributes prior to TRAPI 1.4.0-beta
-                                        if not self.minimum_required_trapi_version("1.4.0-beta"):
-
-                                            if attribute_type_id not in \
-                                                    [
-                                                        "biolink:aggregator_knowledge_source",
-                                                        "biolink:primary_knowledge_source",
-
-                                                        # Note: deprecated since Biolink release 3.0.2
-                                                        #       but this is probably caught above in the
-                                                        #       'validate_element_status' method predicate
-                                                        "biolink:original_knowledge_source"
-
-                                                    ]:
-
-                                                # TODO: not interested here in any other
-                                                #       attribute_type_id's at this moment
-                                                continue
-
-                                            # ... now, check the infores values against various expectations
-                                            for infores in value:
-                                                if not infores.startswith("infores:"):
-                                                    self.report(
-                                                        code="error.knowledge_graph.edge.provenance.infores.missing",
-                                                        identifier=str(infores),
-                                                        edge_id=edge_id,
-                                                        source_trail=source_trail
-                                                    )
-                                                else:
-                                                    if attribute_type_id == "biolink:primary_knowledge_source":
-                                                        found_primary_knowledge_source.append(infores)
-
-                                                    if ara_source and \
-                                                       attribute_type_id == "biolink:aggregator_knowledge_source" and \
-                                                       infores == ara_source:
-                                                        found_ara_knowledge_source = True
-                                                    elif kp_source and \
-                                                            attribute_type_id == kp_source_type and \
-                                                            infores == kp_source:
-                                                        found_kp_knowledge_source = True
-
-                        # if not a Biolink model defined attribute term, at least, check if
-                        # the 'attribute_type_id' has a namespace (prefix) known to Biolink.
-                        # We won't call it a hard error, but issue a warning
-                        elif not self.bmt.get_element_by_prefix(attribute_type_id):
-                            self.report(
-                                code="warning.knowledge_graph.edge." +
-                                     "attribute.type_id.non_biolink_prefix",
-                                identifier=attribute_type_id,
-                                edge_id=edge_id,
-                                source_trail=source_trail
-                            )
+                                        if biolink_class:
+                                            if self.bmt.is_category(name=biolink_class.name):
+                                                self.report(
+                                                    code="warning.knowledge_graph.edge.attribute.type_id.is_category",
+                                                    identifier=attribute_type_id,
+                                                    edge_id=edge_id,
+                                                    source_trail=source_trail
+                                                )
+                                            elif self.bmt.is_predicate(name=biolink_class.name):
+                                                self.report(
+                                                    code="warning.knowledge_graph.edge.attribute.type_id.is_predicate",
+                                                    identifier=attribute_type_id,
+                                                    edge_id=edge_id,
+                                                    source_trail=source_trail
+                                                )
+                                            elif not self.bmt.is_association_slot(attribute_type_id):
+                                                self.report(
+                                                    code="warning.knowledge_graph.edge.attribute.type_id.not_association_slot",
+                                                    identifier=attribute_type_id,
+                                                    edge_id=edge_id,
+                                                    source_trail=source_trail
+                                                )
+                                            else:
+                                                # attribute_type_id is a Biolink 'association_slot': validate further...
+
+                                                # TODO: only check knowledge_source provenance here for now.
+                                                #       Are there other association_slots to be validated here too?
+                                                #       For example, once new terms with defined value ranges are published
+                                                #       in the Biolink Model, then perhaps 'value' validation will be feasible.
+
+                                                # Edge provenance tags only recorded in
+                                                # Edge attributes prior to TRAPI 1.4.0-beta
+                                                if not self.minimum_required_trapi_version("1.4.0-beta"):
+
+                                                    if attribute_type_id in \
+                                                            [
+                                                                "biolink:aggregator_knowledge_source",
+                                                                "biolink:primary_knowledge_source",
+
+                                                                # Note: deprecated since Biolink release 3.0.2
+                                                                #       but this is probably caught above in the
+                                                                #       'validate_element_status' method predicate
+                                                                "biolink:original_knowledge_source"
+                                                            ]:
+
+                                                        # ... now, check the infores values against various expectations
+                                                        for infores in value:
+                                                            if not infores.startswith("infores:"):
+                                                                self.report(
+                                                                   code="error.knowledge_graph.edge.provenance.infores.missing",
+                                                                   identifier=str(infores),
+                                                                   edge_id=edge_id,
+                                                                   source_trail=source_trail
+                                                                )
+                                                            else:
+                                                                if attribute_type_id == "biolink:primary_knowledge_source":
+                                                                    found_primary_knowledge_source.append(infores)
+
+                                                                if ara_source and \
+                                                                   attribute_type_id == "biolink:aggregator_knowledge_source" \
+                                                                        and infores == ara_source:
+                                                                    found_ara_knowledge_source = True
+                                                                elif kp_source and \
+                                                                        attribute_type_id == kp_source_type and \
+                                                                        infores == kp_source:
+                                                                    found_kp_knowledge_source = True
+
+                                                # We won't likely care if these shows up in
+                                                # graphs compliant with Biolink earlier than 4.2.0.
+                                                # But we validate their values anyhow...
+
+                                                # We expect at this point that the value should be a single scalar
+                                                value = value[0]
+
+                                                if attribute_type_id == "biolink:knowledge_level":
+                                                    found_knowledge_level = \
+                                                        self.validate_knowledge_level(
+                                                            edge_id=edge_id,
+                                                            found=found_knowledge_level,
+                                                            value=value
+                                                        )
+                                                elif attribute_type_id == "biolink:agent_type":
+                                                    found_agent_type = \
+                                                        self.validate_agent_type(
+                                                            edge_id=edge_id,
+                                                            found=found_agent_type,
+                                                            value=value
+                                                        )
+
+                                # if not a Biolink model defined attribute term, at least, check if
+                                # the 'attribute_type_id' has a namespace (prefix) known to Biolink.
+                                # We won't call it a hard error, but issue a warning
+                                elif not self.bmt.get_element_by_prefix(attribute_type_id):
+                                    self.report(
+                                        code="warning.knowledge_graph.edge." +
+                                             "attribute.type_id.non_biolink_prefix",
+                                        identifier=attribute_type_id,
+                                        edge_id=edge_id,
+                                        source_trail=source_trail
+                                    )
 
             # Edge provenance tags only recorded in Edge attributes prior to TRAPI 1.4.0-beta
             if not self.minimum_required_trapi_version("1.4.0-beta") and self.validate_biolink():
                 # After all the attributes have been scanned,
                 # check for provenance. Treat as warnings for now.
                 # Note that provenance checking is only done when Biolink validation is done
                 # (since the various flags are not properly set above, for the test)
@@ -840,14 +957,43 @@
                     edge_id,
                     ara_source, found_ara_knowledge_source,
                     kp_source, found_kp_knowledge_source, kp_source_type,
                     found_primary_knowledge_source,
                     source_trail=source_trail
                 )
 
+            # Mandatory 'knowledge_level' and 'agent_type'
+            # attributes required in all Biolink Model edges
+            # from Biolink Model release 4.2.0 onwards
+            if self.minimum_required_biolink_version("4.2.0"):
+                if not found_knowledge_level:
+                    # Currently projected to be mandatory only in TRAPI 1.6.0
+                    if self.minimum_required_trapi_version("1.6.0"):
+                        self.report(
+                            code="error.knowledge_graph.edge.knowledge_level.missing",
+                            identifier=edge_id
+                        )
+                    else:
+                        self.report(
+                            code="warning.knowledge_graph.edge.knowledge_level.missing",
+                            identifier=edge_id
+                        )
+                if not found_agent_type:
+                    # Currently projected to be mandatory only in TRAPI 1.6.0
+                    if self.minimum_required_trapi_version("1.6.0"):
+                        self.report(
+                            code="error.knowledge_graph.edge.agent_type.missing",
+                            identifier=edge_id
+                        )
+                    else:
+                        self.report(
+                            code="warning.knowledge_graph.edge.agent_type.missing",
+                            identifier=edge_id
+                        )
+
         return source_trail  # may be 'None' if the required attributes are missing
 
     def validate_attribute_constraints(self, edge_id: str, edge: Dict):
         """
         Validate Query Edge Attributes.
 
         :param edge_id: str, string identifier for the edge (for reporting purposes)
@@ -1012,15 +1158,15 @@
                         qualifiers=qualifier_set
                     )
 
     def validate_infores(self, context: str, edge_id: str, identifier: str) -> bool:
         """
         Validate that the specified identifier is a well-formed Infores CURIE.
         Note that here we also now accept that the identifier can
-        be a semi-colon delimited list of such infores.
+        be a semicolon delimited list of such infores.
 
         :param context: reporting context as specified by a validation code prefix
         :param edge_id: specific edge validated, for the purpose of reporting validation context
         :param identifier: candidate (list of) infores curie(s) to be validated.
         :return:
         """
         code_prefix: str = f"error.knowledge_graph.edge.sources.retrieval_source.{context}.infores"
@@ -1077,15 +1223,15 @@
         #     return False
 
         # Infores validates properly here
         return True
 
     def validate_sources(self, edge_id: str, edge: Dict) -> Optional[str]:
         """
-        Validate (TRAPI 1.4.0-beta ++) Edge.sources provenance.
+        Validate (TRAPI 1.4.0-beta ++) Edge sources provenance.
 
         :param edge_id: str, string identifier for the edge (for reporting purposes)
         :param edge: Dict, the edge object associated with some attributes are expected to be found
         :return: Optional[str], audit trail of knowledge source provenance for a given Edge, as a string.
         """
         sources: Dict[str, List[str]] = dict()
         # we ought not to have to test for the absence of the "sources" tag
@@ -1736,12 +1882,12 @@
         (including Biolink version and parent class dictionary content).
         :return: Dict
         """
         dictionary = TRAPISchemaValidator.to_dict(self)
         dictionary["biolink_version"] = self.get_biolink_version()
         return dictionary
 
-    def report_header(self, title: Optional[str], compact_format: bool) -> str:
-        header: str = TRAPISchemaValidator.report_header(self, title, compact_format)
+    def report_header(self, title: Optional[str] = None, compact_format: bool = True) -> str:
+        header: str = super().report_header(title, compact_format)
         header += " and Biolink Model version " \
                   f"'{str(self.get_biolink_version() if self.get_biolink_version() is not None else 'Default')}'"
         return header
```

### Comparing `reasoner_validator-4.0.3/reasoner_validator/codes.yaml` & `reasoner_validator-4.1.0/reasoner_validator/codes.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -473,19 +473,21 @@
               - identifier
             $description: "The 'attribute_type_id' of a Knowledge graph edge attribute must be a controlled vocabulary term specified by a CURIE!"
         value:
           missing:
             $message: "An attribute is missing its 'value' property in Edge"
             $context:
               - identifier
+              - attribute_id
             $description: "An attribute of a Knowledge graph edge must have a 'value' key with a non-empty associated value!"
           empty:
             $message: "An attribute has an empty value in Edge"
             $context:
               - identifier
+              - attribute_id
             $description: "The value of an attribute of a Knowledge graph edge must not be empty!"
       provenance:
         infores:
           missing:
             $message: "Edge has provenance value which is not a well-formed InfoRes CURIE"
             $context:
               - edge_id
@@ -526,14 +528,50 @@
               $message: "Validation of qualifier in qualifiers threw an unexpected exception"
               $context:
                 - identifier
                 - qualifier_type_id
                 - qualifier_value
                 - reason
               $description: "Validation of a specified 'qualifier_type_id' and 'qualifier_value' failed for a given exceptional reason!"
+      knowledge_level:
+        missing:
+          $message: "Edge is missing its required 'knowledge_level' property!"
+          $context:
+            - edge_id
+          $description: "The 'knowledge_level' slot is required for all edges in knowledge graphs complying with the specified TRAPI and Biolink Model release!"
+        duplicated:
+          $message: "The 'knowledge_level' slot is duplicated for the given edge!"
+          $context:
+            - identifier
+            - edge_id
+          $description: "Each edge should only have one 'knowledge_level' attribute value. Additional ones are ignored"
+        invalid:
+          $message: "The indicated 'knowledge_level' slot value is invalid for the given edge!"
+          $context:
+            - identifier
+            - context
+          $description: "Acceptable values of the 'knowledge_level' slot are only as enumerated in the specified Biolink Model"
+      agent_type:
+        missing:
+          $message: "Edge is missing its required 'agent_type' property!"
+          $context:
+            - identifier
+          $description: "The 'agent_type' slot is required for all edges in knowledge graphs complying with the specified Biolink Model release!"
+        duplicated:
+          $message: "The 'agent_type' slot is duplicated for the given edge!"
+          $context:
+            - identifier
+            - edge_id
+          $description: "Each edge should only have one 'agent_type' attribute value. Additional ones are ignored."
+        invalid:
+          $message: "The indicated 'agent_type' slot value is invalid for the given edge!"
+          $context:
+            - identifier
+            - context
+          $description: "Acceptable values of the 'agent_type' slot are only as enumerated in the specified Biolink Model"
       sources:
         missing:
           $message: "Missing 'sources' key for Edge"
           $context:
             - identifier
           $description: "Edge must have a 'sources' key with a non-empty associated value!"
         empty:
@@ -605,14 +643,24 @@
           resource_role:
             empty:
               $message: "Empty 'resource_role' property in Edge"
               $context:
                 - identifier
               $description: "Value of the 'resource_role' property in the RetrievalSource of a Knowledge Graph Edge must be a non-empty ResourceRole enum value!"
 warning:
+  biolink:
+    element:
+      range:
+        unspecified:
+          $message: "Undefined slot range specification"
+          $context:
+            - identifier
+            - context
+            - value
+          $description: "Biolink Model error: the range slot of the specified element is missing or its value is not a known enum?"
   trapi:
     response:
       status:
         unknown:
           $message: "TRAPI Response has unrecognized status code"
           $context:
             - identifier
@@ -838,14 +886,26 @@
           missing:
             $message: "Edge attribute values are missing expected Knowledge Provider provenance"
             $context:
               - edge_id
               - identifier
               - kp_source_type
             $description: "Edge attributes of ARAs and KPs should record the infores identifier of their knowledge source provenance with respect to KP."
+      knowledge_level:
+        missing:
+          $message: "Edge is missing its required 'knowledge_level' property!"
+          $context:
+            - edge_id
+          $description: "The 'knowledge_level' slot is currently optional but recommended for all edges in knowledge graphs complying with the specified TRAPI and Biolink Model release!"
+      agent_type:
+        missing:
+          $message: "Edge is missing its required 'agent_type' property!"
+          $context:
+            - identifier
+          $description: "The 'agent_type' slot is currently optional but recommended for all edges in knowledge graphs complying with the specified Biolink Model release!"
 info:
   excluded:
     $message: "All test case S-P-O triples from resource test location, or specific user excluded S-P-O triples"
     $context:
       - identifier
     $description: "Check the JSON KP test edge data file for specific 'exclude_tests' directives, either global to the file, or on specific edges."
   compliant:
```

### Comparing `reasoner_validator-4.0.3/reasoner_validator/github.py` & `reasoner_validator-4.1.0/reasoner_validator/github.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.3/reasoner_validator/message.py` & `reasoner_validator-4.1.0/reasoner_validator/message.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.3/reasoner_validator/report.py` & `reasoner_validator-4.1.0/reasoner_validator/report.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.3/reasoner_validator/sri/util.py` & `reasoner_validator-4.1.0/reasoner_validator/sri/util.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.3/reasoner_validator/trapi/__init__.py` & `reasoner_validator-4.1.0/reasoner_validator/trapi/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,18 +34,37 @@
 TRAPI_1_4_0_BETA4_SEMVER = SemVer.from_string("v1.4.0-beta4")
 TRAPI_1_4_0_SEMVER = SemVer.from_string("v1.4.0")
 TRAPI_1_4_0: str = str(TRAPI_1_4_0_SEMVER)
 TRAPI_1_4_1_SEMVER = SemVer.from_string("v1.4.1")
 TRAPI_1_4_1: str = str(TRAPI_1_4_1_SEMVER)
 TRAPI_1_4_2_SEMVER = SemVer.from_string("v1.4.2")
 TRAPI_1_4_2: str = str(TRAPI_1_4_2_SEMVER)
-LATEST_TRAPI_RELEASE_SEMVER: SemVer = TRAPI_1_4_2_SEMVER
-LATEST_TRAPI_RELEASE: str = TRAPI_1_4_2
-LATEST_TRAPI_MAJOR_RELEASE_SEMVER: SemVer = SemVer.from_string("v1.4", core_fields=['major', 'minor'])
-LATEST_TRAPI_MAJOR_RELEASE: str = str(LATEST_TRAPI_MAJOR_RELEASE_SEMVER)
+TRAPI_1_5_0_BETA_SEMVER = SemVer.from_string("v1.5.0-beta")
+TRAPI_1_5_0_BETA: str = str(TRAPI_1_5_0_BETA_SEMVER)
+
+LATEST_TRAPI_RELEASE_SEMVER: SemVer = TRAPI_1_5_0_BETA_SEMVER
+LATEST_TRAPI_RELEASE: str = TRAPI_1_5_0_BETA
+
+LATEST_TRAPI_MAJOR_MINOR_RELEASE: str = "1.5"
+LATEST_TRAPI_MAJOR_MINOR_RELEASE_SEMVER: SemVer = \
+    SemVer.from_string(
+        LATEST_TRAPI_MAJOR_MINOR_RELEASE,
+        core_fields=['major', 'minor'],
+        # generally also suppress extension fields
+        # when just going for MAJOR MINOR release SemVer
+        ext_fields=[]
+    )
+LATEST_TRAPI_MAJOR_MINOR_PATCH_RELEASE_SEMVER: SemVer = \
+    SemVer.from_string(
+        LATEST_TRAPI_RELEASE,
+        # generally also suppress extension fields
+        # when just going for MAJOR MINOR PATCH release SemVer
+        ext_fields=[]
+    )
+LATEST_TRAPI_MAJOR_MINOR_PATCH_RELEASE: str = str(LATEST_TRAPI_MAJOR_MINOR_PATCH_RELEASE_SEMVER)
 
 
 class TRAPIAccessError(RuntimeError):
     pass
 
 
 @lru_cache()
@@ -92,15 +111,17 @@
                     or a git branch name, all referencing a target TRAPI schema.
     :return: loaded TRAPI schema
     """
     mapped_release = get_latest_version(target)
     if mapped_release:
         schema_version = mapped_release
     else:
-        err_msg: str = f"No TRAPI version {target}"
+        err_msg: str = \
+            f"Requested TRAPI version '{target}' is unknown to the system. " + \
+            "Perhaps the project version list needs to be updated and package re-released?"
         logger.error(err_msg)
         raise ValueError(err_msg)
 
     return _load_schema(schema_version)
 
 
 def _output(json, flat=False):
@@ -369,11 +390,11 @@
         :return: Dict
         """
         dictionary = ValidationReporter.to_dict(self)
         dictionary["trapi_version"] = self.get_trapi_version()
         return dictionary
 
     def report_header(self, title: Optional[str] = None, compact_format: bool = True) -> str:
-        header: str = ValidationReporter.report_header(self, title, compact_format)
+        header: str = super().report_header(title, compact_format)
         header += f" validating against TRAPI version " \
                   f"'{str(self.get_trapi_version() if self.get_trapi_version() is not None else 'Default')}'"
         return header
```

### Comparing `reasoner_validator-4.0.3/reasoner_validator/trapi/mapping.py` & `reasoner_validator-4.1.0/reasoner_validator/trapi/mapping.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.3/reasoner_validator/validation_codes.py` & `reasoner_validator-4.1.0/reasoner_validator/validation_codes.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.3/reasoner_validator/validator.py` & `reasoner_validator-4.1.0/reasoner_validator/validator.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from reasoner_validator.biolink import (
     BMTWrapper,
     BiolinkValidator,
     get_biolink_model_toolkit
 )
 
 from reasoner_validator.report import TRAPIGraphType
-from reasoner_validator.trapi import LATEST_TRAPI_RELEASE, LATEST_TRAPI_MAJOR_RELEASE_SEMVER
+from reasoner_validator.trapi import LATEST_TRAPI_RELEASE, LATEST_TRAPI_MAJOR_MINOR_RELEASE_SEMVER
 from reasoner_validator.trapi.mapping import MappingValidator, check_node_edge_mappings
 from reasoner_validator.versioning import SemVer, SemVerError, get_latest_version
 from reasoner_validator.sri.util import get_aliases
 
 import logging
 logger = logging.getLogger(__name__)
 
@@ -63,15 +63,15 @@
         self._is_trapi_1_4: Optional[bool] = None
         self.suppress_empty_data_warnings: bool = suppress_empty_data_warnings
 
     def is_trapi_1_4(self) -> bool:
         assert self.trapi_version
         try:  # try block ... Sanity check: in case the trapi_version is somehow invalid?
             target_major_version: SemVer = SemVer.from_string(self.trapi_version, core_fields=['major', 'minor'])
-            self._is_trapi_1_4 = target_major_version >= LATEST_TRAPI_MAJOR_RELEASE_SEMVER
+            self._is_trapi_1_4 = target_major_version >= LATEST_TRAPI_MAJOR_MINOR_RELEASE_SEMVER
         except SemVerError as sve:
             logger.error(f"Current TRAPI release '{self.trapi_version}' seems invalid: {str(sve)}. Reset to latest?")
             self.trapi_version = LATEST_TRAPI_RELEASE
             self._is_trapi_1_4 = True
         return self._is_trapi_1_4
 
     def sanitize_workflow(self, response: Dict) -> Dict:
```

### Comparing `reasoner_validator-4.0.3/reasoner_validator/versioning.py` & `reasoner_validator-4.1.0/reasoner_validator/versioning.py`

 * *Files 3% similar despite different names*

```diff
@@ -264,26 +264,28 @@
     :param release_tag: (possibly partial) SemVer string, Git branch name,
                         or YAML schema file name identifying a release.
     :return: 'best' latest release of SemVer specification or the YAML file directly returned.
     """
     global _latest
 
     if not release_tag:
+        # the current policy is NOT to second guess if the 'latest' version is needed,
+        # but rather, to rely on project maintainers to update the versions.yaml file.
         return None
     elif release_tag.lower().endswith(".yaml"):
         return release_tag
     elif release_tag in _versions["branches"]:
         # cases in which a branch name is
         # given instead of a release number
         return release_tag
     else:
         # strip any prefix from the release tag to ensure that
         # only the SemVer part is used for the latest version lookup
         release_tag = sub(r'^[^0-9]+', '', release_tag)
-        latest: SemVer = _latest.get(release_tag, None)
+        latest: Optional[SemVer] = _latest.get(release_tag, None)
         return str(latest) if latest else None
 
 
 def _set_preferred_version(release_tag: str, target_release: SemVer):
     global _latest
     latest_4_release_tag: Optional[SemVer] = _latest.get(release_tag, None)
     if not latest_4_release_tag or (target_release >= latest_4_release_tag):
```

### Comparing `reasoner_validator-4.0.3/reasoner_validator/versions.yaml` & `reasoner_validator-4.1.0/reasoner_validator/versions.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 branches:
 - '1.3'
 - '1.4'
+- '1.5'
 - add_sources_to_meta_edge
 - edeutsch-Changlog
 - edeutsch-Message-Response-minitemsnow1
 - edeutsch-Query-message
 - edeutsch-Response
 - edeutsch-analysis
 - edeutsch-bypass_cache
 - edeutsch-bypass-2
+- edeutsch-bypass-norm
 - edeutsch-clarify-nodebinding
 - edeutsch-collection-type
 - edeutsch-eb-auxgraph
 - edeutsch-exclude
 - edeutsch-issue-313
 - edeutsch-log-minitems1
 - edeutsch-logs-minitemsto1
@@ -23,16 +25,16 @@
 - edeutsch-response-fix
 - edeutsch-result-nullmin
 - extended
 - gh-pages
 - master
 - mbrush-patch-1
 - mbrush-patch-2
-- mbrush-patch-3
 releases:
+- v1.5.0-beta
 - v1.4.2
 - v1.4.1
 - v1.4.0
 - v1.4.0-beta4
 - v1.4.0-beta3
 - v1.4.0-beta
 - v1.4.0-beta2
```

### Comparing `reasoner_validator-4.0.3/tests/__init__.py` & `reasoner_validator-4.1.0/tests/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,38 @@
-from typing import Tuple, List
+from typing import Tuple, List, Dict, Any
 from sys import stderr
 from os.path import abspath, dirname, sep
 from copy import deepcopy
 
-from reasoner_validator.trapi import TRAPI_1_3_0, LATEST_TRAPI_RELEASE, LATEST_TRAPI_MAJOR_RELEASE
+from reasoner_validator.trapi import (
+    TRAPI_1_3_0,
+    TRAPI_1_4_2,
+    LATEST_TRAPI_RELEASE,
+    LATEST_TRAPI_MAJOR_MINOR_RELEASE, LATEST_TRAPI_MAJOR_MINOR_PATCH_RELEASE
+)
 
 TESTS_DIRECTORY = abspath(dirname(__file__))
 print(f"Test Directory: {TESTS_DIRECTORY}", file=stderr)
 
 PATCHED_SCHEMA_VERSION = "v1.4.0-beta5"
 PATCHED_140_SCHEMA_FILEPATH = f"{TESTS_DIRECTORY}{sep}test_data{sep}patched_trapi_schema_{PATCHED_SCHEMA_VERSION}.yaml"
 BROKEN_SCHEMA_FILEPATH = f"broken-{PATCHED_SCHEMA_VERSION}.yaml"
 
 PRE_1_4_0_TEST_VERSIONS: List = ["1.2", "1.2.0", "1.3", TRAPI_1_3_0]
-LATEST_TEST_RELEASES: List = ["1", LATEST_TRAPI_MAJOR_RELEASE, LATEST_TRAPI_RELEASE]
+TRAPI_1_4_TEST_VERSIONS: List = ["1.4", TRAPI_1_4_2]
+PRE_1_5_0_TEST_VERSIONS: List = PRE_1_4_0_TEST_VERSIONS + TRAPI_1_4_TEST_VERSIONS
 
-ALL_TEST_VERSIONS: List[str] = PRE_1_4_0_TEST_VERSIONS + LATEST_TEST_RELEASES
+LATEST_TEST_RELEASES: List = [
+    "1",
+    LATEST_TRAPI_MAJOR_MINOR_RELEASE,
+    LATEST_TRAPI_MAJOR_MINOR_PATCH_RELEASE,
+    LATEST_TRAPI_RELEASE
+]
+
+ALL_TEST_VERSIONS: List[str] = PRE_1_5_0_TEST_VERSIONS + LATEST_TEST_RELEASES
 
 
 SIMPLE_SAMPLE_NODES = {
     "NCBIGene:29974": {
         "name": "APOBEC1 complementation factor",
         "categories": [
            "biolink:Gene"
@@ -40,28 +53,41 @@
         "attributes": [],
         "original_attribute_name": "max_phase",
         "value": "FDA Clinical Research Phase 2",
         "value_type_id": "biolink:FDA_approval_status_enum"
     }
 ]
 
+DEFAULT_KL = {
+    "attribute_type_id": "biolink:knowledge_level",
+    "value": "not_provided"
+}
+
+
+DEFAULT_AT = {
+    "attribute_type_id": "biolink:agent_type",
+    "value": "not_provided"
+}
+
+DEFAULT_KL_AND_AT_ATTRIBUTES = [DEFAULT_KL, DEFAULT_AT]
+
 # complete edge dereferencing SAMPLE_NODES_WITH_ATTRIBUTES
 SAMPLE_EDGE_WITH_ATTRIBUTES_AND_SOURCES = {
     "edge_1": {
         "subject": "NCBIGene:29974",
         "predicate": "biolink:physically_interacts_with",
         "object": "PUBCHEM.COMPOUND:597",
         "attributes": [
             {
                 "attribute_source": "infores:hmdb",
                 "attribute_type_id": "biolink:stoichiometry",
                 "value": 2,
                 "attributes": [],
             }
-        ],
+        ] + DEFAULT_KL_AND_AT_ATTRIBUTES,
         "sources": [
             {
                 "resource_id": "infores:molepro",
                 "resource_role": "primary_knowledge_source"
             }
         ]
     }
@@ -70,7 +96,28 @@
 SAMPLE_NODES_WITH_UNUSED_NODE = deepcopy(SIMPLE_SAMPLE_NODES)
 SAMPLE_NODES_WITH_UNUSED_NODE["NCBITaxon:9606"] = {
     "name": "Homo sapiens",
     "categories": [
        "biolink:OrganismTaxon"
     ]
 }
+
+SAMPLE_EDGE_WITH_WITHOUT_ATTRIBUTES = {
+    "edge_1": {
+        "subject": "NCBIGene:29974",
+        "predicate": "biolink:physically_interacts_with",
+        "object": "PUBCHEM.COMPOUND:597",
+        "attributes": [],
+        "sources": [
+            {
+                "resource_id": "infores:molepro",
+                "resource_role": "primary_knowledge_source"
+            }
+        ]
+    }
+}
+
+
+def sample_edge_with_attributes(attributes: List[Dict[str, Any]]) -> Dict[str, Any]:
+    sample_edge = deepcopy(SAMPLE_EDGE_WITH_WITHOUT_ATTRIBUTES)
+    sample_edge["edge_1"]["attributes"] = attributes
+    return sample_edge
```

### Comparing `reasoner_validator-4.0.3/tests/test_biolink_compliance_validation.py` & `reasoner_validator-4.1.0/tests/test_biolink_compliance_validation.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,19 @@
 from reasoner_validator.biolink import BiolinkValidator, get_biolink_model_toolkit
 
 from reasoner_validator.report import TRAPIGraphType
 from tests import (
     SIMPLE_SAMPLE_NODES,
     SAMPLE_NODES_WITH_ATTRIBUTES,
     SAMPLE_EDGE_WITH_ATTRIBUTES_AND_SOURCES,
-    SAMPLE_NODES_WITH_UNUSED_NODE
+    SAMPLE_NODES_WITH_UNUSED_NODE,
+    DEFAULT_KL,
+    DEFAULT_AT,
+    DEFAULT_KL_AND_AT_ATTRIBUTES,
+    sample_edge_with_attributes
 )
 from tests.test_validation_report import check_messages
 
 logger = logging.getLogger(__name__)
 logger.setLevel("DEBUG")
 
 pp = PrettyPrinter(indent=4)
@@ -1217,124 +1221,124 @@
         (
             # Query 3. EDAM-DATA:2526 ought to have an acceptable namespace
             {
                 "attributes": [
                     {
                         "attribute_type_id": "EDAM-DATA:2526",
                         "value": "some-value"
-                    }
-                ]
-            },
-            ""  # Should all pass in TRAPI releases 'default' >= 1.4.0-beta
-        ),
-        (
-            # Query 4. Validating terms in the ATTRIBUTE_TYPE_ID_INCLUSIONS list
-            {
-                "attributes": [
-                    {
-                        "attribute_type_id": "biolink:knowledge_level",
-                        "value": "knowledge_assertion"
                     },
-                    {
-                        "attribute_type_id": "biolink:agent_type",
-                        "value": "manual_agent"
-                    }
-                ]
+                ] + DEFAULT_KL_AND_AT_ATTRIBUTES
             },
             ""  # Should all pass in TRAPI releases 'default' >= 1.4.0-beta
         ),
+        # (
+        #     # Query #. Validating terms in the ATTRIBUTE_TYPE_ID_INCLUSIONS list
+        #     {
+        #         "attributes": [
+        #             {
+        #                 "attribute_type_id": "biolink:knowledge_level",
+        #                 "value": "knowledge_assertion"
+        #             },
+        #             {
+        #                 "attribute_type_id": "biolink:agent_type",
+        #                 "value": "manual_agent"
+        #             }
+        #         ]
+        #     },
+        #     ""  # Should all pass in TRAPI releases 'default' >= 1.4.0-beta
+        # ),
         # Slipping in a few unit tests of the
         # "error.knowledge_graph.edge.attribute.value.empty"
         (
-            # Query 5. Attribute value is numeric (int) and zero
+            # Query 4. Attribute value is numeric (int) and zero
             {
                 "attributes": [
                     {
                         "attribute_type_id": "biolink:Attribute",
                         "value": 0
                     }
-                ]
+                ] + DEFAULT_KL_AND_AT_ATTRIBUTES
             },
             ""   # should pass since 'False' is a valid non-empty attribute value
         ),
         (
-            # Query 6. Attribute value is numeric (float) and zero
+            # Query 5. Attribute value is numeric (float) and zero
             {
                 "attributes": [
                     {
                         "attribute_type_id": "biolink:Attribute",
                         "value": 0.0
                     }
-                ]
+                ] + DEFAULT_KL_AND_AT_ATTRIBUTES
             },
             ""   # should pass since 'False' is a valid non-empty attribute value
         ),
         (
-            # Query 7. Attribute value is explicit boolean 'false'
+            # Query 6. Attribute value is explicit boolean 'false'
             {
                 "attributes": [
                     {
                         "attribute_type_id": "biolink:Attribute",
                         "value": False
                     }
-                ]
+                ] + DEFAULT_KL_AND_AT_ATTRIBUTES
             },
             ""   # should pass since 'False' is a valid non-empty attribute value
         ),
         (
-            # Query 8. Empty string as attribute value
+            # Query 7. Empty string as attribute value
             {
                 "attributes": [
                     {
                         "attribute_type_id": "biolink:Attribute",
                         "value": ""
                     }
-                ]
+                ] + DEFAULT_KL_AND_AT_ATTRIBUTES
             },
             "error.knowledge_graph.edge.attribute.value.empty"
         ),
         (
-            # Query 9. None (JSON 'null'?) as attribute value
+            # Query 8. None (JSON 'null'?) as attribute value
             {
                 "attributes": [
                     {
                         "attribute_type_id": "biolink:Attribute",
                         "value": None
                     }
-                ]
+                ] + DEFAULT_KL_AND_AT_ATTRIBUTES
             },
             "error.knowledge_graph.edge.attribute.value.empty"
         ),
         (
-            # Query 10. Empty array (JSON 'null'?) as attribute value
+            # Query 9. Empty array (JSON 'null'?) as attribute value
             {
                 "attributes": [
                     {
                         "attribute_type_id": "biolink:Attribute",
                         "value": []
                     }
-                ]
+                ] + DEFAULT_KL_AND_AT_ATTRIBUTES
             },
             "error.knowledge_graph.edge.attribute.value.empty"
         ),
         (
-            # Query 11. Empty set/dict (JSON 'null'?) as attribute value
+            # Query 10. Empty set/dict (JSON 'null'?) as attribute value
             {
                 "attributes": [
                     {
                         "attribute_type_id": "biolink:Attribute",
                         "value": {}
                     }
-                ]
+                ] + DEFAULT_KL_AND_AT_ATTRIBUTES
             },
             "error.knowledge_graph.edge.attribute.value.empty"
         )
     ]
 )
-def test_post_1_4_0_trapi_validate_attributes(edge: Dict, validation_code: str):
+def test_latest_trapi_validate_attributes(edge: Dict, validation_code: str):
     validator = BiolinkValidator()
     validator.validate_attributes(
         graph_type=TRAPIGraphType.Knowledge_Graph,
         edge_id="test_validate_attributes unit test",
         edge=edge
     )
     check_messages(validator, validation_code)
@@ -1528,15 +1532,15 @@
             # Query 8. value is the JSON boolean false (Python bool False)
             {
                 "attributes": [
                     {
                         "attribute_type_id": "biolink:aggregator_knowledge_source",
                         "value": False
                     },
-                ]
+                ] + DEFAULT_KL_AND_AT_ATTRIBUTES
             },
             get_ara_test_case(),
             ""
         ),
         (
             # Query 9. An attribute_type_id is not a well-formed CURIE? Should fail?
             {
@@ -1557,18 +1561,20 @@
             },
             get_ara_test_case(),
             # "is not a well-formed CURIE!"
             "error.knowledge_graph.edge.attribute.type_id.not_curie"
         )
     ]
 )
-def test_latest_validate_attributes(edge: Dict, target_provenance: Optional[Dict[str, str]], validation_code: str):
+def test_latest_validate_trapi_attributes_with_target_provenance(
+        edge: Dict,
+        target_provenance: Optional[Dict[str, str]],
+        validation_code: str
+):
     validator = BiolinkValidator(
-        # trapi_version="latest",
-        biolink_version=LATEST_BIOLINK_MODEL_VERSION,
         target_provenance=target_provenance
     )
     validator.validate_attributes(
         graph_type=TRAPIGraphType.Knowledge_Graph,
         edge_id="test_validate_attributes unit test",
         edge=edge
     )
@@ -2356,16 +2362,112 @@
         trapi_version=trapi_version
     )
 
 
 ##################################
 # Validate TRAPI Knowledge Graph #
 ##################################
+def test_validate_duplicate_slot_value():
+    validator = BiolinkValidator(biolink_version="4.2.0")
+    validator.validate_slot_value(
+        slot_name="knowledge_level",
+        context="test_validate_duplicate_slot_value",
+        found=True,
+        value="fake-kl-value"
+    )
+    check_messages(validator, "error.knowledge_graph.edge.knowledge_level.duplicated")
+
+
+def test_validate_unspecified_slot_value_range():
+    validator = BiolinkValidator(biolink_version="4.2.0")
+    validator.validate_slot_value(
+        slot_name="supporting_study_metadata",
+        context="test_validate_unspecified_slot_value_range",
+        found=False,
+        value="fake-kl-value"
+    )
+    check_messages(validator, "warning.biolink.element.range.unspecified")
+
+
+#     def validate_slot_value(
+#             self,
+#             slot_name: str,
+#             context: str,
+#             found: bool,
+#             value: Optional[str]
+#     ):
+@pytest.mark.parametrize(
+    "value,code",
+    [
+        ("not_provided", ""),
+        ("prediction", ""),
+        ("fake-kl-value", "error.knowledge_graph.edge.knowledge_level.invalid")
+    ]
+)
+def test_validate_slot_value(value: Optional[str], code: str):
+    validator = BiolinkValidator(biolink_version="4.2.0")
+    validator.validate_slot_value(
+        slot_name="knowledge_level",
+        context="test_validate_slot_value",
+        found=False,
+        value=value
+    )
+    check_messages(validator, code)
+
+
+# def validate_knowledge_level(
+#             self,
+#             edge_id: str,
+#             found: bool,
+#             value: Optional[str]
+#     ) -> bool:
+@pytest.mark.parametrize(
+    "value,code",
+    [
+        ("not_provided", ""),
+        ("prediction", ""),
+        ("fake-kl-value", "error.knowledge_graph.edge.knowledge_level.invalid")
+    ]
+)
+def test_validate_knowledge_level(value: Optional[str], code: str):
+    validator = BiolinkValidator(biolink_version="4.2.0")
+    validator.validate_knowledge_level(
+        edge_id="test_validate_knowledge_level",
+        found=False,
+        value=value
+    )
+    check_messages(validator, code)
+
+
+# def validate_agent_type(
+#             self,
+#             edge_id: str,
+#             found: bool,
+#             value: Optional[str]
+#     ) -> bool:
+@pytest.mark.parametrize(
+    "value,code",
+    [
+        ("not_provided", ""),
+        ("data_analysis_pipeline", ""),
+        ("fake-kl-value", "error.knowledge_graph.edge.agent_type.invalid")
+    ]
+)
+def test_validate_agent_type(value: Optional[str], code: str):
+    validator = BiolinkValidator(biolink_version="4.2.0")
+    validator.validate_agent_type(
+        edge_id="test_validate_agent_type",
+        found=False,
+        value=value
+    )
+    check_messages(validator, code)
+
+
 @pytest.mark.parametrize(
-    "biolink_version,graph_data,validation_code",
+    "biolink_version,graph_data,code",
     [
         (
             LATEST_BIOLINK_MODEL_VERSION,
 
             # Query 0: Sample full valid TRAPI Knowledge Graph
             {
                 # Sample nodes
@@ -2625,15 +2727,15 @@
                         "predicate": "biolink:physically_interacts_with",
                         "object": "NCBIGene:29974",
                         "attributes": [
                             {
                                 "attribute_type_id": "biolink:stoichiometry",
                                 "value": 2
                             }
-                        ],
+                        ] + DEFAULT_KL_AND_AT_ATTRIBUTES,
                         "sources": [
                             {
                                 "resource_id": "infores:molepro",
                                 "resource_role": "primary_knowledge_source"
                             }
                         ]
                     }
@@ -2662,15 +2764,15 @@
                         "predicate": "biolink:physically_interacts_with",
                         "object": "NCBIGene:29974",
                         "attributes": [
                             {
                                 "attribute_type_id": "biolink:stoichiometry",
                                 "value": 2
                             }
-                        ],
+                        ] + DEFAULT_KL_AND_AT_ATTRIBUTES,
                         "sources": [
                             {
                                 "resource_id": "infores:molepro",
                                 "resource_role": "primary_knowledge_source"
                             }
                         ]
                     }
@@ -2699,15 +2801,15 @@
                         "predicate": "biolink:physically_interacts_with",
                         "object": "NCBIGene:29974",
                         "attributes": [
                             {
                                 "attribute_type_id": "biolink:stoichiometry",
                                 "value": 2
                             }
-                        ],
+                        ] + DEFAULT_KL_AND_AT_ATTRIBUTES,
                         "sources": [
                             {
                                 "resource_id": "infores:molepro",
                                 "resource_role": "primary_knowledge_source"
                             }
                         ]
                     }
@@ -2771,15 +2873,15 @@
                         "predicate": "biolink:physically_interacts_with",
                         "object": "NCBIGene:29974",
                         "attributes": [
                             {
                                 "attribute_type_id": "biolink:stoichiometry",
                                 "value": 2
                             }
-                        ],
+                        ] + DEFAULT_KL_AND_AT_ATTRIBUTES,
                         "sources": [
                             {
                                 "resource_id": "infores:molepro",
                                 "resource_role": "primary_knowledge_source"
                             }
                         ]
                     }
@@ -2798,15 +2900,15 @@
                         "predicate": "biolink:physically_interacts_with",
                         "object": "NCBIGene:29974",
                         "attributes": [
                             {
                                 "attribute_type_id": "biolink:stoichiometry",
                                 "value": 2
                             }
-                        ],
+                        ] + DEFAULT_KL_AND_AT_ATTRIBUTES,
                         "sources": [
                             {
                                 "resource_id": "infores:molepro",
                                 "resource_role": "primary_knowledge_source"
                             }
                         ]
                     }
@@ -2827,15 +2929,15 @@
                         "predicate": "biolink:physically_interacts_with",
                         "object": "PUBCHEM.COMPOUND:597",
                         "attributes": [
                             {
                                 "attribute_type_id": "biolink:stoichiometry",
                                 "value": 2
                             }
-                        ],
+                        ] + DEFAULT_KL_AND_AT_ATTRIBUTES,
                         "sources": [
                             {
                                 "resource_id": "infores:molepro",
                                 "resource_role": "primary_knowledge_source"
                             }
                         ]
                     }
@@ -2854,15 +2956,15 @@
                         "predicate": "biolink:unknown_predicate",
                         "object": "PUBCHEM.COMPOUND:597",
                         "attributes": [
                             {
                                 "attribute_type_id": "biolink:stoichiometry",
                                 "value": 2
                             }
-                        ],
+                        ] + DEFAULT_KL_AND_AT_ATTRIBUTES,
                         "sources": [
                             {
                                 "resource_id": "infores:molepro",
                                 "resource_role": "primary_knowledge_source"
                             }
                         ]
                     }
@@ -2881,15 +2983,15 @@
                         "predicate": "biolink:has_unit",
                         "object": "PUBCHEM.COMPOUND:597",
                         "attributes": [
                             {
                                 "attribute_type_id": "biolink:stoichiometry",
                                 "value": 2
                             }
-                        ],
+                        ] + DEFAULT_KL_AND_AT_ATTRIBUTES,
                         "sources": [
                             {
                                 "resource_id": "infores:molepro",
                                 "resource_role": "primary_knowledge_source"
                             }
                         ]
                     }
@@ -2923,15 +3025,15 @@
                         "predicate": "biolink:increases_amount_or_activity_of",
                         "object": "HGNC:391",
                         "attributes": [
                             {
                                 "attribute_type_id": "biolink:stoichiometry",
                                 "value": 2
                             }
-                        ],
+                        ] + DEFAULT_KL_AND_AT_ATTRIBUTES,
                         "sources": [
                             {
                                 "resource_id": "infores:molepro",
                                 "resource_role": "primary_knowledge_source"
                             }
                         ]
                     }
@@ -2966,15 +3068,15 @@
                         "predicate": "biolink:interacts_with",
                         "object": "HGNC:391",
                         "attributes": [
                             {
                                 "attribute_type_id": "biolink:stoichiometry",
                                 "value": 2
                             }
-                        ],
+                        ] + DEFAULT_KL_AND_AT_ATTRIBUTES,
                         "sources": [
                             {
                                 "resource_id": "infores:molepro",
                                 "resource_role": "primary_knowledge_source"
                             }
                         ]
                     }
@@ -3009,15 +3111,15 @@
                         "predicate": "biolink:contributor",
                         "object": "ORCID:56789",
                         "attributes": [
                             {
                                 "attribute_type_id": "biolink:stoichiometry",
                                 "value": 2
                             }
-                        ],
+                        ] + DEFAULT_KL_AND_AT_ATTRIBUTES,
                         "sources": [
                             {
                                 "resource_id": "infores:molepro",
                                 "resource_role": "primary_knowledge_source"
                             }
                         ]
                     }
@@ -3036,15 +3138,15 @@
                         "predicate": "biolink:affected_by",
                         "object": "PUBCHEM.COMPOUND:597",
                         "attributes": [
                             {
                                 "attribute_type_id": "biolink:stoichiometry",
                                 "value": 2
                             }
-                        ],
+                        ] + DEFAULT_KL_AND_AT_ATTRIBUTES,
                         "sources": [
                             {
                                 "resource_id": "infores:molepro",
                                 "resource_role": "primary_knowledge_source"
                             }
                         ]
                     }
@@ -3063,15 +3165,15 @@
                         "predicate": "biolink:physically_interacts_with",
                         "object": "PUBCHEM.COMPOUND:678",
                         "attributes": [
                             {
                                 "attribute_type_id": "biolink:stoichiometry",
                                 "value": 2
                             }
-                        ],
+                        ] + DEFAULT_KL_AND_AT_ATTRIBUTES,
                         "sources": [
                             {
                                 "resource_id": "infores:molepro",
                                 "resource_role": "primary_knowledge_source"
                             }
                         ]
                     }
@@ -3089,15 +3191,15 @@
                         "subject": "NCBIGene:29974",
                         "predicate": "biolink:physically_interacts_with",
                         "object": "PUBCHEM.COMPOUND:597",
                         "attributes": [
                             {
                                 "value": "some value"
                             }
-                        ],
+                        ] + DEFAULT_KL_AND_AT_ATTRIBUTES,
                         "sources": [
                             {
                                 "resource_id": "infores:molepro",
                                 "resource_role": "primary_knowledge_source"
                             }
                         ]
                     }
@@ -3116,15 +3218,15 @@
                         "predicate": "biolink:physically_interacts_with",
                         "object": "PUBCHEM.COMPOUND:597",
                         "attributes": [
                             {
                                 "attribute_type_id": "biolink:stoichiometry",
                                 # "value": 2
                             }
-                        ],
+                        ] + DEFAULT_KL_AND_AT_ATTRIBUTES,
                         "sources": [
                             {
                                 "resource_id": "infores:molepro",
                                 "resource_role": "primary_knowledge_source"
                             }
                         ]
                     }
@@ -3143,15 +3245,15 @@
                         "predicate": "biolink:physically_interacts_with",
                         "object": "PUBCHEM.COMPOUND:597",
                         "attributes": [
                             {
                                 "attribute_type_id": "not_a_curie",
                                 "value": "some value"
                             }
-                        ],
+                        ] + DEFAULT_KL_AND_AT_ATTRIBUTES,
                         "sources": [
                             {
                                 "resource_id": "infores:molepro",
                                 "resource_role": "primary_knowledge_source"
                             }
                         ]
                     }
@@ -3171,15 +3273,15 @@
                         "predicate": "biolink:physically_interacts_with",
                         "object": "PUBCHEM.COMPOUND:597",
                         "attributes": [
                             {
                                 "attribute_type_id": "biolink:OrganismTaxon",
                                 "value": "9606"
                             }
-                        ],
+                        ] + DEFAULT_KL_AND_AT_ATTRIBUTES,
                         "sources": [
                             {
                                 "resource_id": "infores:molepro",
                                 "resource_role": "primary_knowledge_source"
                             }
                         ]
                     }
@@ -3199,15 +3301,15 @@
                         "predicate": "biolink:physically_interacts_with",
                         "object": "PUBCHEM.COMPOUND:597",
                         "attributes": [
                             {
                                 "attribute_type_id": "biolink:related_to",
                                 "value": "something"
                             }
-                        ],
+                        ] + DEFAULT_KL_AND_AT_ATTRIBUTES,
                         "sources": [
                             {
                                 "resource_id": "infores:molepro",
                                 "resource_role": "primary_knowledge_source"
                             }
                         ]
                     }
@@ -3226,15 +3328,15 @@
                         "predicate": "biolink:physically_interacts_with",
                         "object": "PUBCHEM.COMPOUND:597",
                         "attributes": [
                             {
                                 "attribute_type_id": "biolink:synonym",
                                 "value": "some synonym"
                             }
-                        ],
+                        ] + DEFAULT_KL_AND_AT_ATTRIBUTES,
                         "sources": [
                             {
                                 "resource_id": "infores:molepro",
                                 "resource_role": "primary_knowledge_source"
                             }
                         ]
                     }
@@ -3258,15 +3360,15 @@
                                 "attribute_type_id": "biolink:negated",
                                 "value": "some value"
                             },
                             {
                                 "attribute_type_id": "biolink:stoichiometry",
                                 "value": 2
                             }
-                        ],
+                        ] + DEFAULT_KL_AND_AT_ATTRIBUTES,
                         "sources": [
                             {
                                 "resource_id": "infores:molepro",
                                 "resource_role": "primary_knowledge_source"
                             }
                         ]
                     }
@@ -3285,15 +3387,15 @@
                         "predicate": "biolink:physically_interacts_with",
                         "object": "PUBCHEM.COMPOUND:597",
                         "attributes": [
                             {
                                 "attribute_type_id": "foo:bar",
                                 "value": "some value"
                             }
-                        ],
+                        ] + DEFAULT_KL_AND_AT_ATTRIBUTES,
                         "sources": [
                             {
                                 "resource_id": "infores:molepro",
                                 "resource_role": "primary_knowledge_source"
                             }
                         ]
                     }
@@ -3340,15 +3442,15 @@
                         "predicate": "biolink:physically_interacts_with",
                         "object": "PUBCHEM.COMPOUND:597",
                         "attributes": [
                             {
                                 "attribute_type_id": "foo:bar",
                                 "value": "some value"
                             }
-                        ],
+                        ] + DEFAULT_KL_AND_AT_ATTRIBUTES,
                         "sources": [
                             {
                                 "resource_id": "infores:molepro",
                                 "resource_role": "primary_knowledge_source"
                             }
                         ]
                     }
@@ -3370,15 +3472,15 @@
                         "predicate": "biolink:physically_interacts_with",
                         "object": "PUBCHEM.COMPOUND:597",
                         "attributes": [
                             {
                                 "attribute_type_id": "biolink:synonym",
                                 "value": "some synonym"
                             }
-                        ],
+                        ] + DEFAULT_KL_AND_AT_ATTRIBUTES,
                         "sources": [
                             {
                                 "resource_id": "infores:molepro",
                                 "resource_role": "primary_knowledge_source"
                             }
                         ]
                     }
@@ -3395,25 +3497,123 @@
             {
                 # Sample nodes with extra  unused node
                 'nodes': SAMPLE_NODES_WITH_UNUSED_NODE,
                 # Sample edge
                 'edges': SAMPLE_EDGE_WITH_ATTRIBUTES_AND_SOURCES
             },
             "warning.knowledge_graph.nodes.dangling"
+        ),
+        (
+            LATEST_BIOLINK_MODEL_VERSION,
+
+            # Query 36: Knowledge Graph edge duplicated Knowledge Level
+            {
+                'nodes': SAMPLE_NODES_WITH_ATTRIBUTES,
+                'edges': sample_edge_with_attributes(
+                    attributes=[
+                        DEFAULT_KL,
+                        DEFAULT_KL,
+                        DEFAULT_AT
+                    ]
+                )
+            },
+            "error.knowledge_graph.edge.knowledge_level.duplicated"
+        ),
+        (
+            LATEST_BIOLINK_MODEL_VERSION,
+
+            # Query 37: Knowledge Graph edge missing Knowledge Level
+            {
+                'nodes': SAMPLE_NODES_WITH_ATTRIBUTES,
+                'edges': sample_edge_with_attributes(
+                    attributes=[
+                        DEFAULT_AT
+                    ]
+                )
+            },
+            # This will be a warning for TRAPI 1.5.0 but should become an error in TRAPI 1.6.0
+            "warning.knowledge_graph.edge.knowledge_level.missing"
+        ),
+        (
+            LATEST_BIOLINK_MODEL_VERSION,
+
+            # Query 38: Knowledge Graph edge invalid Knowledge Level
+            {
+                'nodes': SAMPLE_NODES_WITH_ATTRIBUTES,
+                'edges': sample_edge_with_attributes(
+                    attributes=[
+                        {
+                           "attribute_type_id": "biolink:knowledge_level",
+                           "value": "not-a-knowledge-level"
+                        },
+                        DEFAULT_AT
+                    ]
+                )
+            },
+            "error.knowledge_graph.edge.knowledge_level.invalid"
+        ),
+        (
+            LATEST_BIOLINK_MODEL_VERSION,
+
+            # Query 39: Knowledge Graph edge duplicated Agent Type
+            {
+                'nodes': SAMPLE_NODES_WITH_ATTRIBUTES,
+                'edges': sample_edge_with_attributes(
+                    attributes=[
+                        DEFAULT_KL,
+                        DEFAULT_AT,
+                        DEFAULT_AT
+                    ]
+                )
+            },
+            "error.knowledge_graph.edge.agent_type.duplicated"
+        ),
+        (
+            LATEST_BIOLINK_MODEL_VERSION,
+
+            # Query 40: Knowledge Graph edge missing Agent Type
+            {
+                'nodes': SAMPLE_NODES_WITH_ATTRIBUTES,
+                'edges': sample_edge_with_attributes(
+                    attributes=[
+                        DEFAULT_KL
+                    ]
+                )
+            },
+            # This will be a warning for TRAPI 1.5.0 but should become an error in TRAPI 1.6.0
+            "warning.knowledge_graph.edge.agent_type.missing"
+        ),
+        (
+            LATEST_BIOLINK_MODEL_VERSION,
+
+            # Query 41: Knowledge Graph edge invalid Agent Type
+            {
+                'nodes': SAMPLE_NODES_WITH_ATTRIBUTES,
+                'edges': sample_edge_with_attributes(
+                    attributes=[
+                        DEFAULT_KL,
+                        {
+                           "attribute_type_id": "biolink:agent_type",
+                           "value": "not-an-agent-type"
+                        }
+                    ]
+                )
+            },
+            "error.knowledge_graph.edge.agent_type.invalid"
         )
     ]
 )
 def test_check_biolink_model_compliance_of_knowledge_graph(
         biolink_version: str,
         graph_data: Dict,
-        validation_code: str
+        code: str
 ):
     validator = BiolinkValidator(biolink_version=biolink_version)
     validator.check_biolink_model_compliance(graph=graph_data, graph_type=TRAPIGraphType.Knowledge_Graph)
-    check_messages(validator, validation_code)
+    check_messages(validator, code)
 
 
 MESSAGE_EDGE_WITHOUT_ATTRIBUTES = {
     "nodes": SIMPLE_SAMPLE_NODES,
     "edges": {
         "edge_1": {
             "subject": "NCBIGene:29974",
```

### Comparing `reasoner_validator-4.0.3/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml` & `reasoner_validator-4.1.0/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.3/tests/test_response_validator.py` & `reasoner_validator-4.1.0/tests/test_response_validator.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 from dictdiffer import diff
 
 from reasoner_validator.trapi import TRAPI_1_3_0, TRAPI_1_4_2
 from reasoner_validator.validator import TRAPIResponseValidator
 from reasoner_validator.report import TRAPIGraphType
 
-from tests import PATCHED_140_SCHEMA_FILEPATH, SAMPLE_NODES_WITH_ATTRIBUTES
+from tests import PATCHED_140_SCHEMA_FILEPATH, SAMPLE_NODES_WITH_ATTRIBUTES, DEFAULT_KL_AND_AT_ATTRIBUTES
 from tests.test_validation_report import check_messages
 
 
 logger = logging.getLogger(__name__)
 logger.setLevel("DEBUG")
 
 _TEST_QG_1 = {
@@ -60,15 +60,15 @@
                    "attribute_type_id": "biolink:aggregator_knowledge_source",
                    "attributes": [],
                    "description": "Molecular Data Provider",
                    "original_attribute_name": "biolink:aggregator_knowledge_source",
                    "value": "infores:molepro",
                    "value_type_id": "biolink:InformationResource"
                }
-            ],
+            ] + DEFAULT_KL_AND_AT_ATTRIBUTES,
         }
     }
 
 _TEST_KG_1 = {
     "nodes": SAMPLE_NODES_WITH_ATTRIBUTES,
     "edges": _TEST_EDGES_1
 }
```

### Comparing `reasoner_validator-4.0.3/tests/test_semver.py` & `reasoner_validator-4.1.0/tests/test_semver.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.3/tests/test_trapi_versioning.py` & `reasoner_validator-4.1.0/tests/test_trapi_versioning.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.3/tests/test_validate.py` & `reasoner_validator-4.1.0/tests/test_validate.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,16 +3,27 @@
 from typing import Tuple, Dict, Optional
 from copy import deepcopy
 
 import pytest
 
 from jsonschema.exceptions import ValidationError
 
-from reasoner_validator.trapi import TRAPISchemaValidator, openapi_to_jsonschema, load_schema, LATEST_TRAPI_RELEASE
-from tests import LATEST_TEST_RELEASES, PRE_1_4_0_TEST_VERSIONS, ALL_TEST_VERSIONS
+from reasoner_validator.trapi import (
+    TRAPISchemaValidator,
+    openapi_to_jsonschema,
+    load_schema,
+    LATEST_TRAPI_RELEASE,
+    LATEST_TRAPI_MAJOR_MINOR_RELEASE
+)
+from tests import (
+    LATEST_TEST_RELEASES,
+    PRE_1_4_0_TEST_VERSIONS,
+    ALL_TEST_VERSIONS,
+    PRE_1_5_0_TEST_VERSIONS, TRAPI_1_4_TEST_VERSIONS
+)
 
 
 @pytest.mark.parametrize(
     "query",
     [
         (  # query 0
             {
@@ -90,15 +101,15 @@
     assert schema, "TRAPI Schema for ('master') branch is not available?"
 
 
 def test_message():
     reporter = TRAPISchemaValidator(
         default_test="test_message",
         default_target="Test Message",
-        trapi_version="v1.4"
+        trapi_version=LATEST_TRAPI_RELEASE
     )
     assert reporter.get_trapi_version() == LATEST_TRAPI_RELEASE
     assert not reporter.has_messages()
     reporter.report("info.compliant")
     assert reporter.has_messages()
     reporter.dump()
 
@@ -116,16 +127,30 @@
     with pytest.raises(ValidationError):
         validator.validate({
             "foo": {},
             "bar": {},
         }, "Query")
 
 
-@pytest.mark.parametrize("trapi_version", ALL_TEST_VERSIONS)
-def test_edgebinding(trapi_version: str):
+@pytest.mark.parametrize("trapi_version", PRE_1_5_0_TEST_VERSIONS)
+def test_trapi_pre_1_5_edgebinding(trapi_version: str):
+    """Test TRAPIValidator(trapi_version=query).validate_EdgeBinding()."""
+    validator = TRAPISchemaValidator(trapi_version=trapi_version)
+    validator.validate({
+        "id": "hello",
+    }, "EdgeBinding")
+    with pytest.raises(ValidationError):
+        validator.validate({
+            "foo": {},
+        }, "EdgeBinding")
+
+
+@pytest.mark.skip("Test inputs are not yet TRAPI 1.5 compliant")
+@pytest.mark.parametrize("trapi_version", LATEST_TEST_RELEASES)
+def test_trapi_1_5_edgebinding(trapi_version: str):
     """Test TRAPIValidator(trapi_version=query).validate_EdgeBinding()."""
     validator = TRAPISchemaValidator(trapi_version=trapi_version)
     validator.validate({
         "id": "hello",
     }, "EdgeBinding")
     with pytest.raises(ValidationError):
         validator.validate({
@@ -252,16 +277,59 @@
                 "allowlist": ["infores:aragorn"]
             }
         }
     }
 ]
 
 
+@pytest.mark.parametrize("trapi_version", TRAPI_1_4_TEST_VERSIONS)
+def test_pre_1_5_query_latest_trapi_workflow_properties(trapi_version: str):
+    """Test flawed TRAPI Query workflow properties."""
+    validator = TRAPISchemaValidator(trapi_version=trapi_version)
+    query = deepcopy(SAMPLE_QUERY)
+    query["workflow"] = SAMPLE_WORKFLOW_1_3_4
+    validator.validate(query, "Query")
+    with pytest.raises(ValidationError):
+        faulty_query_wf = deepcopy(query)
+        # ...and the 'id' object key should have a schema-defined enum as its value,...
+        faulty_query_wf["workflow"] = [
+            {
+                "id": "not-a-workflow-enum"
+            }
+        ]
+        validator.validate(faulty_query_wf, "Query")
+    with pytest.raises(ValidationError):
+        faulty_query_wf = deepcopy(query)
+        # ...and if 'runner_parameters' key is present and has a non-empty value,
+        # it needs oneOf the "allowlist" or "denylist" keys...
+        faulty_query_wf["workflow"] = [
+            {
+                "id": "sort_results_score",
+                "runner_parameters": {}
+            }
+        ]
+        validator.validate(faulty_query_wf, "Query")
+    with pytest.raises(ValidationError):
+        faulty_query_wf = deepcopy(query)
+        # ...and if 'runner_parameters' object "allowlist" or "denylist"
+        # is present, they must have a non-empty value, of at least one infores CURIE.
+        faulty_query_wf["workflow"] = [
+            {
+                "id": "lookup",
+                "runner_parameters": {
+                    "allowlist": []
+                }
+            }
+        ]
+        validator.validate(faulty_query_wf, "Query")
+
+
+@pytest.mark.skip("Test inputs are not yet TRAPI 1.5 compliant")
 @pytest.mark.parametrize("trapi_version", LATEST_TEST_RELEASES)
-def test_query_latest_trapi_workflow_properties(trapi_version: str):
+def test_1_5_query_latest_trapi_workflow_properties(trapi_version: str):
     """Test flawed TRAPI Query workflow properties."""
     validator = TRAPISchemaValidator(trapi_version=trapi_version)
     query = deepcopy(SAMPLE_QUERY)
     query["workflow"] = SAMPLE_WORKFLOW_1_3_4
     validator.validate(query, "Query")
     with pytest.raises(ValidationError):
         faulty_query_wf = deepcopy(query)
@@ -375,14 +443,160 @@
         validator.validate({
             # missing required: node_bindings, edge_bindings
             "foo": {},
             "bar": {},
         }, "Result")
 
 
+@pytest.mark.parametrize("trapi_version", TRAPI_1_4_TEST_VERSIONS)
+def test_trapi_1_4_message_results_component_validation(trapi_version: str):
+    """Test Message.Results component in TRAPIValidator(trapi_version=query).validate()."""
+    #     Result:
+    #       type: object
+    #       description: >-
+    #         A Result object specifies the nodes and edges in the knowledge graph
+    #         that satisfy the structure or conditions of a user-submitted query
+    #         graph. It must contain a NodeBindings object (list of query graph node
+    #         to knowledge graph node mappings) and an EdgeBindings object (list of
+    #         query graph edge to knowledge graph edge mappings).
+    #       properties:
+    #         node_bindings:
+    #           type: object
+    #           description: >-
+    #             The dictionary of Input Query Graph to Result Knowledge Graph node
+    #             bindings where the dictionary keys are the key identifiers of the
+    #             Query Graph nodes and the associated values of those keys are
+    #             instances of NodeBinding schema type (see below). This value is an
+    #             array of NodeBindings since a given query node may have multiple
+    #             knowledge graph Node bindings in the result.
+    #           additionalProperties:
+    #             type: array
+    #             items:
+    #               $ref: '#/components/schemas/NodeBinding'
+    #         analyses:
+    #           type: array
+    #           description: >-
+    #             The list of all Analysis components that contribute to the result.
+    #             See below for Analysis components.
+    #           items:
+    #             $ref: '#/components/schemas/Analysis'
+    #       additionalProperties: true
+    #       required:
+    #         - node_bindings
+    #         - analyses
+    # where an Analysis object is:
+    #     Analysis:
+    #       type: object
+    #       description: >-
+    #         An analysis is a dictionary that contains information about
+    #         the result tied to a particular service. Each Analysis is
+    #         generated by a single reasoning service, and describes the
+    #         outputs of analyses performed by the reasoner on a particular
+    #         Result (e.g. a result score), along with provenance information
+    #         supporting the analysis (e.g. method or data that supported
+    #         generation of the score).
+    #       properties:
+    #         resource_id:
+    #           $ref: '#/components/schemas/CURIE'
+    #           description: The id of the service generating and using this Anlysis
+    #         score:
+    #           type: number
+    #           format: float
+    #           example: 163.233
+    #           description: >-
+    #             A numerical score associated with this result indicating the
+    #             relevance or confidence of this result relative to others in the
+    #             returned set. Higher MUST be better.
+    #           nullable: true
+    #         edge_bindings:
+    #           type: object
+    #           description: >-
+    #             The dictionary of input Query Graph to Knowledge Graph edge
+    #             bindings where the dictionary keys are the key identifiers of the
+    #             Query Graph edges and the associated values of those keys are
+    #             instances of EdgeBinding schema type (see below). This value is an
+    #             array of EdgeBindings since a given query edge may resolve to
+    #             multiple Knowledge Graph Edges.
+    #           additionalProperties:
+    #             type: array
+    #             items:
+    #               $ref: '#/components/schemas/EdgeBinding'
+    #         support_graphs:
+    #           type: array
+    #           description: >-
+    #             This is a list of references to Auxiliary Graph instances
+    #             that supported the analysis of a Result as performed by the
+    #             reasoning service. Each item in the list is the key of a
+    #             single Auxiliary Graph.
+    #           nullable: true
+    #           items:
+    #             type: string
+    #         scoring_method:
+    #           type: string
+    #           description: >-
+    #             An identifier and link to an explanation for the method used
+    #             to generate the score
+    #           nullable: true
+    #         attributes:
+    #           type: array
+    #           description: >-
+    #             The attributes of this particular Analysis.
+    #           items:
+    #             $ref: '#/components/schemas/Attribute'
+    #           nullable: true
+    #       additionalProperties: true
+    #       required:
+    #         - resource_id
+    #         - edge_bindings
+    validator = TRAPISchemaValidator(trapi_version=trapi_version)
+    sample_message_result = {
+        "node_bindings": {
+            "a": [
+                {
+                    "attributes": None,
+                    "id": "SGD:S000000065",
+                    "qnode_id": "SGD:S000000065",
+                    "query_id": None
+                }
+            ],
+            "b": [
+                {
+                    "attributes": None,
+                    "id": "GO:1905776",
+                    "query_id": None
+                }
+            ]
+        },
+        "analyses": [
+            {
+                "resource_id": "infores:arax",
+                "edge_bindings": {
+                    "ab": [
+                        {
+                            "attributes": None,
+                            "id": "uuid:7884e454-d09c-11ec-b00f-0242ac110002"
+                        }
+                    ]
+                },
+                "score": None
+            }
+        ]
+    }
+
+    validator.validate(sample_message_result, "Result")
+
+    with pytest.raises(ValidationError):
+        validator.validate({
+            # missing required: node_bindings, edge_bindings
+            "foo": {},
+            "bar": {},
+        }, "Result")
+
+
+@pytest.mark.skip("Test inputs are not yet TRAPI 1.5 compliant")
 @pytest.mark.parametrize("trapi_version", LATEST_TEST_RELEASES)
 def test_latest_trapi_message_results_component_validation(trapi_version: str):
     """Test Message.Results component in TRAPIValidator(trapi_version=query).validate()."""
     #     Result:
     #       type: object
     #       description: >-
     #         A Result object specifies the nodes and edges in the knowledge graph
@@ -520,16 +734,37 @@
         validator.validate({
             # missing required: node_bindings, edge_bindings
             "foo": {},
             "bar": {},
         }, "Result")
 
 
-@pytest.mark.parametrize("trapi_version", ALL_TEST_VERSIONS)
-def test_message_node_binding_component_validation(trapi_version: str):
+@pytest.mark.parametrize("trapi_version", PRE_1_5_0_TEST_VERSIONS)
+def test_message_pre_1_5_node_binding_component_validation(trapi_version: str):
+    """Test NodeBinding component in TRAPIValidator(trapi_version=query).validate()."""
+    validator = TRAPISchemaValidator(trapi_version=trapi_version)
+    sample_node_binding = {
+        "id": "SGD:S000000065",
+        # 'qnode_id' is not formally specified in spec, but it is an
+        # example of an additionalProperties: true permitted field
+        "qnode_id": "SGD:S000000065",
+        "query_id": None
+    }
+
+    validator.validate(sample_node_binding, "NodeBinding")
+    with pytest.raises(ValidationError):
+        validator.validate({
+            # missing required: id
+            "foo": {},
+            "bar": {},
+        }, "NodeBinding")
+
+@pytest.mark.skip("Test inputs are not yet TRAPI 1.5 compliant")
+@pytest.mark.parametrize("trapi_version", LATEST_TEST_RELEASES)
+def test_latest_trapi_message_node_binding_component_validation(trapi_version: str):
     """Test NodeBinding component in TRAPIValidator(trapi_version=query).validate()."""
     validator = TRAPISchemaValidator(trapi_version=trapi_version)
     sample_node_binding = {
         "id": "SGD:S000000065",
         # 'qnode_id' is not formally specified in spec, but it is an
         # example of an additionalProperties: true permitted field
         "qnode_id": "SGD:S000000065",
```

### Comparing `reasoner_validator-4.0.3/tests/test_validation_report.py` & `reasoner_validator-4.1.0/tests/test_validation_report.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.3/tests/test_workflows.py` & `reasoner_validator-4.1.0/tests/test_workflows.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Dict
 from itertools import product
 from json import dumps
 
 from reasoner_validator.trapi import TRAPISchemaValidator
 from reasoner_validator.validator import TRAPIResponseValidator
 
-from tests import LATEST_TEST_RELEASES
+from tests import LATEST_TEST_RELEASES, TRAPI_1_4_TEST_VERSIONS
 
 SAMPLE_QUERY_1 = {
     "message": {
         "knowledge_graph": None,
         "query_graph": None,
         "results": None,
     },
@@ -63,18 +63,33 @@
         },
         {
             "id": "lookup"
         }
     ]
 }
 
-QUERY_VERSION = [qv for qv in product(LATEST_TEST_RELEASES, (SAMPLE_QUERY_1, SAMPLE_QUERY_2))]
+TRAPI_1_4_QUERY_VERSION = [qv for qv in product(TRAPI_1_4_TEST_VERSIONS, (SAMPLE_QUERY_1, SAMPLE_QUERY_2))]
 
 
-@pytest.mark.parametrize("trapi_version,query", QUERY_VERSION)
+@pytest.mark.parametrize("trapi_version,query", TRAPI_1_4_QUERY_VERSION)
+def test_trapi_1_4_query_trapi_workflow_properties(trapi_version: str, query: Dict):
+    """Test flawed TRAPI Query workflow properties."""
+
+    print(f"\nTRAPI release: '{trapi_version}'")
+    print(f"Test Workflow: '{dumps(query['workflow'], indent=2)}'")
+
+    validator = TRAPISchemaValidator(trapi_version=trapi_version)
+    validator.validate(query, "Query")
+
+
+TRAPI_LATEST_TRAPI_QUERY_VERSION = [qv for qv in product(LATEST_TEST_RELEASES, (SAMPLE_QUERY_1, SAMPLE_QUERY_2))]
+
+
+@pytest.mark.skip("Test inputs are not yet TRAPI 1.5 compliant")
+@pytest.mark.parametrize("trapi_version,query", TRAPI_LATEST_TRAPI_QUERY_VERSION)
 def test_query_latest_trapi_workflow_properties(trapi_version: str, query: Dict):
     """Test flawed TRAPI Query workflow properties."""
 
     print(f"\nTRAPI release: '{trapi_version}'")
     print(f"Test Workflow: '{dumps(query['workflow'], indent=2)}'")
 
     validator = TRAPISchemaValidator(trapi_version=trapi_version)
```

### Comparing `reasoner_validator-4.0.3/PKG-INFO` & `reasoner_validator-4.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-validator
-Version: 4.0.3
+Version: 4.1.0
 Summary: Validation tools for Reasoner API
 Home-page: https://github.com/NCATSTranslator
 License: MIT
 Keywords: NCATS,Biomedical Data Translator,Translator,ReasonerAPI,TRAPI,validation,Biolink Model
 Author: Richard Bruskiewich
 Author-email: richard.bruskiewich@delphinai.com
 Maintainer: Richard Bruskiewich
```

