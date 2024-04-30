# Comparing `tmp/dsp_tools-7.1.3.post1.tar.gz` & `tmp/dsp_tools-7.1.3.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsp_tools-7.1.3.post1.tar", max compression
+gzip compressed data, was "dsp_tools-7.1.3.post2.tar", max compression
```

## Comparing `dsp_tools-7.1.3.post1.tar` & `dsp_tools-7.1.3.post2.tar`

### file list

```diff
@@ -1,115 +1,115 @@
--rw-r--r--   0        0        0    35149 2024-04-25 10:13:32.063843 dsp_tools-7.1.3.post1/LICENSE
--rw-r--r--   0        0        0     4941 2024-04-25 10:13:32.079843 dsp_tools-7.1.3.post1/docs/index.md
--rw-r--r--   0        0        0     8375 2024-04-25 10:13:59.179862 dsp_tools-7.1.3.post1/pyproject.toml
--rw-r--r--   0        0        0       41 2024-04-25 10:13:32.079843 dsp_tools-7.1.3.post1/src/dsp_tools/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 10:13:32.079843 dsp_tools-7.1.3.post1/src/dsp_tools/cli/__init__.py
--rw-r--r--   0        0        0     7360 2024-04-25 10:13:32.079843 dsp_tools-7.1.3.post1/src/dsp_tools/cli/call_action.py
--rw-r--r--   0        0        0    12476 2024-04-25 10:13:32.079843 dsp_tools-7.1.3.post1/src/dsp_tools/cli/create_parsers.py
--rw-r--r--   0        0        0     9909 2024-04-25 10:13:32.079843 dsp_tools-7.1.3.post1/src/dsp_tools/cli/entry_point.py
--rw-r--r--   0        0        0        0 2024-04-25 10:13:32.079843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 10:13:32.079843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/excel2json/__init__.py
--rw-r--r--   0        0        0    15987 2024-04-25 10:13:32.079843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/excel2json/lists.py
--rw-r--r--   0        0        0        0 2024-04-25 10:13:32.079843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/excel2json/models/__init__.py
--rw-r--r--   0        0        0     8065 2024-04-25 10:13:32.079843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/excel2json/models/input_error.py
--rw-r--r--   0        0        0      501 2024-04-25 10:13:32.079843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/excel2json/models/list_node_name.py
--rw-r--r--   0        0        0     6313 2024-04-25 10:13:32.079843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/excel2json/project.py
--rw-r--r--   0        0        0    13738 2024-04-25 10:13:32.079843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/excel2json/properties.py
--rw-r--r--   0        0        0    11887 2024-04-25 10:13:32.079843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/excel2json/resources.py
--rw-r--r--   0        0        0    11866 2024-04-25 10:13:32.079843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/excel2json/utils.py
--rw-r--r--   0        0        0      466 2024-04-25 10:13:32.079843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/excel2xml/__init__.py
--rw-r--r--   0        0        0    21324 2024-04-25 10:13:32.079843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/excel2xml/excel2xml_cli.py
--rw-r--r--   0        0        0    76125 2024-04-25 10:13:32.079843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/excel2xml/excel2xml_lib.py
--rw-r--r--   0        0        0     1981 2024-04-25 10:13:32.079843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/excel2xml/propertyelement.py
--rw-r--r--   0        0        0     8275 2024-04-25 10:13:32.079843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/id2iri.py
--rw-r--r--   0        0        0        0 2024-04-25 10:13:32.079843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/ingest_xmlupload/__init__.py
--rw-r--r--   0        0        0     2876 2024-04-25 10:13:32.079843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/ingest_xmlupload/apply_ingest_id.py
--rw-r--r--   0        0        0     2351 2024-04-25 10:13:32.079843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/ingest_xmlupload/upload_xml.py
--rw-r--r--   0        0        0     4891 2024-04-25 10:13:32.079843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/ingest_xmlupload/user_information.py
--rw-r--r--   0        0        0        0 2024-04-25 10:13:32.079843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/project/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 10:13:32.079843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/project/create/__init__.py
--rw-r--r--   0        0        0    45642 2024-04-25 10:13:32.079843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/project/create/project_create.py
--rw-r--r--   0        0        0     8243 2024-04-25 10:13:32.079843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/project/create/project_create_lists.py
--rw-r--r--   0        0        0    21090 2024-04-25 10:13:32.079843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/project/create/project_validate.py
--rw-r--r--   0        0        0     5743 2024-04-25 10:13:32.079843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/project/get.py
--rw-r--r--   0        0        0        0 2024-04-25 10:13:32.079843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/project/models/__init__.py
--rw-r--r--   0        0        0    12173 2024-04-25 10:13:32.079843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/project/models/context.py
--rw-r--r--   0        0        0     8379 2024-04-25 10:13:32.079843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/project/models/group.py
--rw-r--r--   0        0        0      850 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/project/models/helpers.py
--rw-r--r--   0        0        0    14910 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/project/models/listnode.py
--rw-r--r--   0        0        0      245 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/project/models/model.py
--rw-r--r--   0        0        0    12710 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/project/models/ontology.py
--rw-r--r--   0        0        0    11594 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/project/models/project.py
--rw-r--r--   0        0        0      306 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/project/models/project_definition.py
--rw-r--r--   0        0        0    17215 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/project/models/propertyclass.py
--rw-r--r--   0        0        0    28334 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/project/models/resourceclass.py
--rw-r--r--   0        0        0    17030 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/project/models/user.py
--rw-r--r--   0        0        0        0 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/resume_xmlupload/__init__.py
--rw-r--r--   0        0        0     4200 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/resume_xmlupload/resume_xmlupload.py
--rw-r--r--   0        0        0     4177 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/rosetta.py
--rw-r--r--   0        0        0    14112 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/start_stack.py
--rw-r--r--   0        0        0     1134 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/template.py
--rw-r--r--   0        0        0        0 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/__init__.py
--rw-r--r--   0        0        0     2350 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/ark2iri.py
--rw-r--r--   0        0        0    10356 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/check_consistency_with_ontology.py
--rw-r--r--   0        0        0      625 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/iri_resolver.py
--rw-r--r--   0        0        0     3587 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/list_client.py
--rw-r--r--   0        0        0        0 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/models/__init__.py
--rw-r--r--   0        0        0     1334 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/models/formatted_text_value.py
--rw-r--r--   0        0        0     5428 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/models/ontology_lookup_models.py
--rw-r--r--   0        0        0     6752 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/models/ontology_problem_models.py
--rw-r--r--   0        0        0     2388 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/models/permission.py
--rw-r--r--   0        0        0      812 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/models/sipi.py
--rw-r--r--   0        0        0      675 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/models/upload_state.py
--rw-r--r--   0        0        0     2236 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/models/xmlallow.py
--rw-r--r--   0        0        0      548 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/models/xmlbitstream.py
--rw-r--r--   0        0        0     1437 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/models/xmlpermission.py
--rw-r--r--   0        0        0     2026 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/models/xmlproperty.py
--rw-r--r--   0        0        0     5164 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/models/xmlresource.py
--rw-r--r--   0        0        0     4004 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/models/xmlvalue.py
--rw-r--r--   0        0        0     3466 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/ontology_client.py
--rw-r--r--   0        0        0     3063 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/project_client.py
--rw-r--r--   0        0        0     4653 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/read_validate_xml_file.py
--rw-r--r--   0        0        0    13023 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/resource_create_client.py
--rw-r--r--   0        0        0     4585 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/resource_multimedia.py
--rw-r--r--   0        0        0        0 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/stash/__init__.py
--rw-r--r--   0        0        0    12372 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/stash/construct_and_analyze_graph.py
--rw-r--r--   0        0        0     2452 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/stash/graph_models.py
--rw-r--r--   0        0        0     5724 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/stash/stash_circular_references.py
--rw-r--r--   0        0        0     3068 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/stash/stash_models.py
--rw-r--r--   0        0        0     4237 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/stash/upload_stashed_resptr_props.py
--rw-r--r--   0        0        0     7727 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/stash/upload_stashed_xml_texts.py
--rw-r--r--   0        0        0     2175 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/upload_config.py
--rw-r--r--   0        0        0      858 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/write_diagnostic_info.py
--rw-r--r--   0        0        0    22348 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/xmlupload.py
--rw-r--r--   0        0        0        0 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/models/__init__.py
--rw-r--r--   0        0        0      654 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/models/custom_warnings.py
--rw-r--r--   0        0        0     2876 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/models/datetimestamp.py
--rw-r--r--   0        0        0     2536 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/models/exceptions.py
--rw-r--r--   0        0        0     8457 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/models/langstring.py
--rw-r--r--   0        0        0     1777 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/models/projectContext.py
--rw-r--r--   0        0        0        0 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/py.typed
--rw-r--r--   0        0        0     1488 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/resources/0100-template-repo/template.json
--rw-r--r--   0        0        0     1036 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/resources/0100-template-repo/template.xml
--rw-r--r--   0        0        0    24361 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/resources/schema/data.xsd
--rw-r--r--   0        0        0     2770 2024-04-25 10:13:32.083843 dsp_tools-7.1.3.post1/src/dsp_tools/resources/schema/lists-only.json
--rw-r--r--   0        0        0    44347 2024-04-25 10:13:32.087843 dsp_tools-7.1.3.post1/src/dsp_tools/resources/schema/project.json
--rw-r--r--   0        0        0    33977 2024-04-25 10:13:32.087843 dsp_tools-7.1.3.post1/src/dsp_tools/resources/schema/properties-only.json
--rw-r--r--   0        0        0     4341 2024-04-25 10:13:32.087843 dsp_tools-7.1.3.post1/src/dsp_tools/resources/schema/resources-only.json
--rw-r--r--   0        0        0       61 2024-04-25 10:13:32.087843 dsp_tools-7.1.3.post1/src/dsp_tools/resources/start-stack/docker-compose.override.yml
--rw-r--r--   0        0        0     3281 2024-04-25 10:13:32.087843 dsp_tools-7.1.3.post1/src/dsp_tools/resources/start-stack/docker-compose.yml
--rw-r--r--   0        0        0      164 2024-04-25 10:13:32.087843 dsp_tools-7.1.3.post1/src/dsp_tools/resources/start-stack/start-stack-config.yml
--rw-r--r--   0        0        0        0 2024-04-25 10:13:32.087843 dsp_tools-7.1.3.post1/src/dsp_tools/utils/__init__.py
--rw-r--r--   0        0        0     1030 2024-04-25 10:13:32.087843 dsp_tools-7.1.3.post1/src/dsp_tools/utils/connection.py
--rw-r--r--   0        0        0    14126 2024-04-25 10:13:32.087843 dsp_tools-7.1.3.post1/src/dsp_tools/utils/connection_live.py
--rw-r--r--   0        0        0     4554 2024-04-25 10:13:32.087843 dsp_tools-7.1.3.post1/src/dsp_tools/utils/date_util.py
--rw-r--r--   0        0        0      457 2024-04-25 10:13:32.087843 dsp_tools-7.1.3.post1/src/dsp_tools/utils/iri_util.py
--rw-r--r--   0        0        0      893 2024-04-25 10:13:32.087843 dsp_tools-7.1.3.post1/src/dsp_tools/utils/json_ld_util.py
--rw-r--r--   0        0        0     1157 2024-04-25 10:13:32.087843 dsp_tools-7.1.3.post1/src/dsp_tools/utils/logger_config.py
--rw-r--r--   0        0        0      705 2024-04-25 10:13:32.087843 dsp_tools-7.1.3.post1/src/dsp_tools/utils/set_encoder.py
--rw-r--r--   0        0        0     5754 2024-04-25 10:13:32.087843 dsp_tools-7.1.3.post1/src/dsp_tools/utils/shared.py
--rw-r--r--   0        0        0      547 2024-04-25 10:13:32.087843 dsp_tools-7.1.3.post1/src/dsp_tools/utils/uri_util.py
--rw-r--r--   0        0        0      978 2024-04-25 10:13:32.087843 dsp_tools-7.1.3.post1/src/dsp_tools/utils/warnings_config.py
--rw-r--r--   0        0        0     4464 2024-04-25 10:13:32.087843 dsp_tools-7.1.3.post1/src/dsp_tools/utils/xml_utils.py
--rw-r--r--   0        0        0     8219 2024-04-25 10:13:32.087843 dsp_tools-7.1.3.post1/src/dsp_tools/utils/xml_validation.py
--rw-r--r--   0        0        0     2312 2024-04-25 10:13:32.087843 dsp_tools-7.1.3.post1/src/dsp_tools/utils/xml_validation_models.py
--rw-r--r--   0        0        0     6317 1970-01-01 00:00:00.000000 dsp_tools-7.1.3.post1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-30 09:22:39.293393 dsp_tools-7.1.3.post2/LICENSE
+-rw-r--r--   0        0        0     4941 2024-04-30 09:22:39.309393 dsp_tools-7.1.3.post2/docs/index.md
+-rw-r--r--   0        0        0     8375 2024-04-30 09:23:11.253494 dsp_tools-7.1.3.post2/pyproject.toml
+-rw-r--r--   0        0        0       41 2024-04-30 09:22:39.309393 dsp_tools-7.1.3.post2/src/dsp_tools/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 09:22:39.309393 dsp_tools-7.1.3.post2/src/dsp_tools/cli/__init__.py
+-rw-r--r--   0        0        0     7410 2024-04-30 09:22:39.309393 dsp_tools-7.1.3.post2/src/dsp_tools/cli/call_action.py
+-rw-r--r--   0        0        0    12631 2024-04-30 09:22:39.309393 dsp_tools-7.1.3.post2/src/dsp_tools/cli/create_parsers.py
+-rw-r--r--   0        0        0     9909 2024-04-30 09:22:39.309393 dsp_tools-7.1.3.post2/src/dsp_tools/cli/entry_point.py
+-rw-r--r--   0        0        0        0 2024-04-30 09:22:39.309393 dsp_tools-7.1.3.post2/src/dsp_tools/commands/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 09:22:39.309393 dsp_tools-7.1.3.post2/src/dsp_tools/commands/excel2json/__init__.py
+-rw-r--r--   0        0        0    15987 2024-04-30 09:22:39.309393 dsp_tools-7.1.3.post2/src/dsp_tools/commands/excel2json/lists.py
+-rw-r--r--   0        0        0        0 2024-04-30 09:22:39.309393 dsp_tools-7.1.3.post2/src/dsp_tools/commands/excel2json/models/__init__.py
+-rw-r--r--   0        0        0     8065 2024-04-30 09:22:39.309393 dsp_tools-7.1.3.post2/src/dsp_tools/commands/excel2json/models/input_error.py
+-rw-r--r--   0        0        0      501 2024-04-30 09:22:39.309393 dsp_tools-7.1.3.post2/src/dsp_tools/commands/excel2json/models/list_node_name.py
+-rw-r--r--   0        0        0     6313 2024-04-30 09:22:39.309393 dsp_tools-7.1.3.post2/src/dsp_tools/commands/excel2json/project.py
+-rw-r--r--   0        0        0    13738 2024-04-30 09:22:39.309393 dsp_tools-7.1.3.post2/src/dsp_tools/commands/excel2json/properties.py
+-rw-r--r--   0        0        0    11887 2024-04-30 09:22:39.309393 dsp_tools-7.1.3.post2/src/dsp_tools/commands/excel2json/resources.py
+-rw-r--r--   0        0        0    11866 2024-04-30 09:22:39.309393 dsp_tools-7.1.3.post2/src/dsp_tools/commands/excel2json/utils.py
+-rw-r--r--   0        0        0      466 2024-04-30 09:22:39.309393 dsp_tools-7.1.3.post2/src/dsp_tools/commands/excel2xml/__init__.py
+-rw-r--r--   0        0        0    21324 2024-04-30 09:22:39.309393 dsp_tools-7.1.3.post2/src/dsp_tools/commands/excel2xml/excel2xml_cli.py
+-rw-r--r--   0        0        0    76125 2024-04-30 09:22:39.309393 dsp_tools-7.1.3.post2/src/dsp_tools/commands/excel2xml/excel2xml_lib.py
+-rw-r--r--   0        0        0     1981 2024-04-30 09:22:39.309393 dsp_tools-7.1.3.post2/src/dsp_tools/commands/excel2xml/propertyelement.py
+-rw-r--r--   0        0        0     8275 2024-04-30 09:22:39.309393 dsp_tools-7.1.3.post2/src/dsp_tools/commands/id2iri.py
+-rw-r--r--   0        0        0        0 2024-04-30 09:22:39.309393 dsp_tools-7.1.3.post2/src/dsp_tools/commands/ingest_xmlupload/__init__.py
+-rw-r--r--   0        0        0     2876 2024-04-30 09:22:39.309393 dsp_tools-7.1.3.post2/src/dsp_tools/commands/ingest_xmlupload/apply_ingest_id.py
+-rw-r--r--   0        0        0     2351 2024-04-30 09:22:39.309393 dsp_tools-7.1.3.post2/src/dsp_tools/commands/ingest_xmlupload/upload_xml.py
+-rw-r--r--   0        0        0     4891 2024-04-30 09:22:39.309393 dsp_tools-7.1.3.post2/src/dsp_tools/commands/ingest_xmlupload/user_information.py
+-rw-r--r--   0        0        0        0 2024-04-30 09:22:39.309393 dsp_tools-7.1.3.post2/src/dsp_tools/commands/project/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 09:22:39.309393 dsp_tools-7.1.3.post2/src/dsp_tools/commands/project/create/__init__.py
+-rw-r--r--   0        0        0    45642 2024-04-30 09:22:39.309393 dsp_tools-7.1.3.post2/src/dsp_tools/commands/project/create/project_create.py
+-rw-r--r--   0        0        0     8243 2024-04-30 09:22:39.309393 dsp_tools-7.1.3.post2/src/dsp_tools/commands/project/create/project_create_lists.py
+-rw-r--r--   0        0        0    21090 2024-04-30 09:22:39.309393 dsp_tools-7.1.3.post2/src/dsp_tools/commands/project/create/project_validate.py
+-rw-r--r--   0        0        0     5743 2024-04-30 09:22:39.309393 dsp_tools-7.1.3.post2/src/dsp_tools/commands/project/get.py
+-rw-r--r--   0        0        0        0 2024-04-30 09:22:39.309393 dsp_tools-7.1.3.post2/src/dsp_tools/commands/project/models/__init__.py
+-rw-r--r--   0        0        0    12173 2024-04-30 09:22:39.309393 dsp_tools-7.1.3.post2/src/dsp_tools/commands/project/models/context.py
+-rw-r--r--   0        0        0     8379 2024-04-30 09:22:39.309393 dsp_tools-7.1.3.post2/src/dsp_tools/commands/project/models/group.py
+-rw-r--r--   0        0        0      850 2024-04-30 09:22:39.309393 dsp_tools-7.1.3.post2/src/dsp_tools/commands/project/models/helpers.py
+-rw-r--r--   0        0        0    14910 2024-04-30 09:22:39.309393 dsp_tools-7.1.3.post2/src/dsp_tools/commands/project/models/listnode.py
+-rw-r--r--   0        0        0      245 2024-04-30 09:22:39.309393 dsp_tools-7.1.3.post2/src/dsp_tools/commands/project/models/model.py
+-rw-r--r--   0        0        0    12710 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/commands/project/models/ontology.py
+-rw-r--r--   0        0        0    11594 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/commands/project/models/project.py
+-rw-r--r--   0        0        0      306 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/commands/project/models/project_definition.py
+-rw-r--r--   0        0        0    17215 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/commands/project/models/propertyclass.py
+-rw-r--r--   0        0        0    28334 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/commands/project/models/resourceclass.py
+-rw-r--r--   0        0        0    17030 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/commands/project/models/user.py
+-rw-r--r--   0        0        0        0 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/commands/resume_xmlupload/__init__.py
+-rw-r--r--   0        0        0     4200 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/commands/resume_xmlupload/resume_xmlupload.py
+-rw-r--r--   0        0        0     4177 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/commands/rosetta.py
+-rw-r--r--   0        0        0    16102 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/commands/start_stack.py
+-rw-r--r--   0        0        0     1134 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/commands/template.py
+-rw-r--r--   0        0        0        0 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/__init__.py
+-rw-r--r--   0        0        0     2350 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/ark2iri.py
+-rw-r--r--   0        0        0    10356 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/check_consistency_with_ontology.py
+-rw-r--r--   0        0        0      625 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/iri_resolver.py
+-rw-r--r--   0        0        0     3587 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/list_client.py
+-rw-r--r--   0        0        0        0 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/models/__init__.py
+-rw-r--r--   0        0        0     1334 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/models/formatted_text_value.py
+-rw-r--r--   0        0        0     5428 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/models/ontology_lookup_models.py
+-rw-r--r--   0        0        0     6752 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/models/ontology_problem_models.py
+-rw-r--r--   0        0        0     2388 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/models/permission.py
+-rw-r--r--   0        0        0      812 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/models/sipi.py
+-rw-r--r--   0        0        0      675 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/models/upload_state.py
+-rw-r--r--   0        0        0     2236 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/models/xmlallow.py
+-rw-r--r--   0        0        0      548 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/models/xmlbitstream.py
+-rw-r--r--   0        0        0     1437 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/models/xmlpermission.py
+-rw-r--r--   0        0        0     2026 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/models/xmlproperty.py
+-rw-r--r--   0        0        0     5164 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/models/xmlresource.py
+-rw-r--r--   0        0        0     4004 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/models/xmlvalue.py
+-rw-r--r--   0        0        0     3466 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/ontology_client.py
+-rw-r--r--   0        0        0     3063 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/project_client.py
+-rw-r--r--   0        0        0     4653 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/read_validate_xml_file.py
+-rw-r--r--   0        0        0    13023 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/resource_create_client.py
+-rw-r--r--   0        0        0     4585 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/resource_multimedia.py
+-rw-r--r--   0        0        0        0 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/stash/__init__.py
+-rw-r--r--   0        0        0    12372 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/stash/construct_and_analyze_graph.py
+-rw-r--r--   0        0        0     2452 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/stash/graph_models.py
+-rw-r--r--   0        0        0     5724 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/stash/stash_circular_references.py
+-rw-r--r--   0        0        0     3068 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/stash/stash_models.py
+-rw-r--r--   0        0        0     4237 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/stash/upload_stashed_resptr_props.py
+-rw-r--r--   0        0        0     7727 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/stash/upload_stashed_xml_texts.py
+-rw-r--r--   0        0        0     2175 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/upload_config.py
+-rw-r--r--   0        0        0      858 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/write_diagnostic_info.py
+-rw-r--r--   0        0        0    22348 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/xmlupload.py
+-rw-r--r--   0        0        0        0 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/models/__init__.py
+-rw-r--r--   0        0        0      654 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/models/custom_warnings.py
+-rw-r--r--   0        0        0     2876 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/models/datetimestamp.py
+-rw-r--r--   0        0        0     2536 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/models/exceptions.py
+-rw-r--r--   0        0        0     8457 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/models/langstring.py
+-rw-r--r--   0        0        0     1777 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/models/projectContext.py
+-rw-r--r--   0        0        0        0 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/py.typed
+-rw-r--r--   0        0        0     1488 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/resources/0100-template-repo/template.json
+-rw-r--r--   0        0        0     1036 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/resources/0100-template-repo/template.xml
+-rw-r--r--   0        0        0    24361 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/resources/schema/data.xsd
+-rw-r--r--   0        0        0     2770 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/resources/schema/lists-only.json
+-rw-r--r--   0        0        0    44347 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/resources/schema/project.json
+-rw-r--r--   0        0        0    33977 2024-04-30 09:22:39.313392 dsp_tools-7.1.3.post2/src/dsp_tools/resources/schema/properties-only.json
+-rw-r--r--   0        0        0     4341 2024-04-30 09:22:39.317393 dsp_tools-7.1.3.post2/src/dsp_tools/resources/schema/resources-only.json
+-rw-r--r--   0        0        0       61 2024-04-30 09:22:39.317393 dsp_tools-7.1.3.post2/src/dsp_tools/resources/start-stack/docker-compose.override.yml
+-rw-r--r--   0        0        0     3281 2024-04-30 09:22:39.317393 dsp_tools-7.1.3.post2/src/dsp_tools/resources/start-stack/docker-compose.yml
+-rw-r--r--   0        0        0      164 2024-04-30 09:22:39.317393 dsp_tools-7.1.3.post2/src/dsp_tools/resources/start-stack/start-stack-config.yml
+-rw-r--r--   0        0        0        0 2024-04-30 09:22:39.317393 dsp_tools-7.1.3.post2/src/dsp_tools/utils/__init__.py
+-rw-r--r--   0        0        0     1030 2024-04-30 09:22:39.317393 dsp_tools-7.1.3.post2/src/dsp_tools/utils/connection.py
+-rw-r--r--   0        0        0    14126 2024-04-30 09:22:39.317393 dsp_tools-7.1.3.post2/src/dsp_tools/utils/connection_live.py
+-rw-r--r--   0        0        0     4554 2024-04-30 09:22:39.317393 dsp_tools-7.1.3.post2/src/dsp_tools/utils/date_util.py
+-rw-r--r--   0        0        0      457 2024-04-30 09:22:39.317393 dsp_tools-7.1.3.post2/src/dsp_tools/utils/iri_util.py
+-rw-r--r--   0        0        0      893 2024-04-30 09:22:39.317393 dsp_tools-7.1.3.post2/src/dsp_tools/utils/json_ld_util.py
+-rw-r--r--   0        0        0     1157 2024-04-30 09:22:39.317393 dsp_tools-7.1.3.post2/src/dsp_tools/utils/logger_config.py
+-rw-r--r--   0        0        0      705 2024-04-30 09:22:39.317393 dsp_tools-7.1.3.post2/src/dsp_tools/utils/set_encoder.py
+-rw-r--r--   0        0        0     5754 2024-04-30 09:22:39.317393 dsp_tools-7.1.3.post2/src/dsp_tools/utils/shared.py
+-rw-r--r--   0        0        0      547 2024-04-30 09:22:39.317393 dsp_tools-7.1.3.post2/src/dsp_tools/utils/uri_util.py
+-rw-r--r--   0        0        0      978 2024-04-30 09:22:39.317393 dsp_tools-7.1.3.post2/src/dsp_tools/utils/warnings_config.py
+-rw-r--r--   0        0        0     4464 2024-04-30 09:22:39.317393 dsp_tools-7.1.3.post2/src/dsp_tools/utils/xml_utils.py
+-rw-r--r--   0        0        0     8219 2024-04-30 09:22:39.317393 dsp_tools-7.1.3.post2/src/dsp_tools/utils/xml_validation.py
+-rw-r--r--   0        0        0     2312 2024-04-30 09:22:39.317393 dsp_tools-7.1.3.post2/src/dsp_tools/utils/xml_validation_models.py
+-rw-r--r--   0        0        0     6317 1970-01-01 00:00:00.000000 dsp_tools-7.1.3.post2/PKG-INFO
```

### Comparing `dsp_tools-7.1.3.post1/LICENSE` & `dsp_tools-7.1.3.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/docs/index.md` & `dsp_tools-7.1.3.post2/docs/index.md`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/pyproject.toml` & `dsp_tools-7.1.3.post2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # See https://packaging.python.org/en/latest/guides/writing-pyproject-toml/#writing-pyproject-toml
 
 [tool.poetry]
 name = "dsp-tools"
-version = "7.1.3.post1"
+version = "7.1.3.post2"
 description = "DSP-TOOLS is a Python package with a command line interface that helps you interact with a DaSCH service platform (DSP) server."
 authors = ["DaSCH - Swiss National Data and Service Center for the Humanities <info@dasch.swiss>"]
 readme = "docs/index.md"
 license = "GPL-3.0-only"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/cli/call_action.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/cli/call_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,14 +86,15 @@
 def _call_start_stack(args: argparse.Namespace) -> bool:
     stack_handler = StackHandler(
         StackConfiguration(
             max_file_size=args.max_file_size,
             enforce_docker_system_prune=args.prune,
             suppress_docker_system_prune=args.no_prune,
             latest_dev_version=args.latest,
+            upload_test_data=args.with_test_data,
         )
     )
     return stack_handler.start_stack()
 
 
 def _call_excel2xml(args: argparse.Namespace) -> bool:
     success, _ = excel2xml(
```

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/cli/create_parsers.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/cli/create_parsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,14 +104,19 @@
         "--no-prune", action="store_true", help="don't execute 'docker system prune' (and don't ask)"
     )
     subparser.add_argument(
         "--latest",
         action="store_true",
         help="use the latest dev version of DSP-API, from the main branch of the GitHub repository",
     )
+    subparser.add_argument(
+        "--with-test-data",
+        action="store_true",
+        help="initialise the database with built-in test data",
+    )
 
 
 def _add_id2iri(subparsers: _SubParsersAction[ArgumentParser]) -> None:
     subparser = subparsers.add_parser(
         name="id2iri",
         help="Replace internal IDs of an XML file (resptr tags or salsah-links) by IRIs provided in a mapping file.",
     )
```

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/cli/entry_point.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/cli/entry_point.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/excel2json/lists.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/excel2json/lists.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/excel2json/models/input_error.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/excel2json/models/input_error.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/excel2json/project.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/excel2json/project.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/excel2json/properties.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/excel2json/properties.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/excel2json/resources.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/excel2json/resources.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/excel2json/utils.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/excel2json/utils.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/excel2xml/excel2xml_cli.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/excel2xml/excel2xml_cli.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/excel2xml/excel2xml_lib.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/excel2xml/excel2xml_lib.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/excel2xml/propertyelement.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/excel2xml/propertyelement.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/id2iri.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/id2iri.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/ingest_xmlupload/apply_ingest_id.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/ingest_xmlupload/apply_ingest_id.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/ingest_xmlupload/upload_xml.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/ingest_xmlupload/upload_xml.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/ingest_xmlupload/user_information.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/ingest_xmlupload/user_information.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/project/create/project_create.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/project/create/project_create.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/project/create/project_create_lists.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/project/create/project_create_lists.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/project/create/project_validate.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/project/create/project_validate.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/project/get.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/project/get.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/project/models/context.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/project/models/context.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/project/models/group.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/project/models/group.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/project/models/helpers.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/project/models/helpers.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/project/models/listnode.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/project/models/listnode.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/project/models/ontology.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/project/models/ontology.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/project/models/project.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/project/models/project.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/project/models/propertyclass.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/project/models/propertyclass.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/project/models/resourceclass.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/project/models/resourceclass.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/project/models/user.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/project/models/user.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/resume_xmlupload/resume_xmlupload.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/resume_xmlupload/resume_xmlupload.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/rosetta.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/rosetta.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/start_stack.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/start_stack.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,14 +26,15 @@
         latest_dev_version: if True, start DSP-API from repo's main branch, instead of the latest deployed version
     """
 
     max_file_size: Optional[int] = None
     enforce_docker_system_prune: bool = False
     suppress_docker_system_prune: bool = False
     latest_dev_version: bool = False
+    upload_test_data: bool = False
 
     def __post_init__(self) -> None:
         """
         Validate the input parameters passed by the user.
 
         Raises:
             UserError: if one of the parameters is invalid
@@ -232,20 +233,60 @@
                 auth=("admin", "test"),
                 timeout=30,
             )
             if not response.ok:
                 logger.error(f"Cannot start DSP-API: Error when creating graph '{graph}'. response = {vars(response)}")
                 raise UserError(f"Cannot start DSP-API: Error when creating graph '{graph}'")
 
+    def _create_admin_user(self) -> None:
+        """
+        This function adds the default system admin user to the database.
+        The password is the hash for "test".
+
+        Raises:
+            UserError: If the user cannot be created.
+        """
+        graph_prefix = "http://0.0.0.0:3030/knora-test/data?graph="
+        admin_graph = "http://www.knora.org/data/admin"
+        admin_user = """
+        @prefix xsd:         <http://www.w3.org/2001/XMLSchema#> .
+        @prefix rdf:         <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
+        @prefix knora-admin: <http://www.knora.org/ontology/knora-admin#> .
+        
+        <http://rdfh.ch/users/root>
+        rdf:type                         knora-admin:User ;
+        knora-admin:username             "root"^^xsd:string ;
+        knora-admin:email                "root@example.com"^^xsd:string ;
+        knora-admin:givenName            "System"^^xsd:string ;
+        knora-admin:familyName           "Administrator"^^xsd:string ;
+        knora-admin:password             "$2a$12$7XEBehimXN1rbhmVgQsyve08.vtDmKK7VMin4AdgCEtE4DWgfQbTK"^^xsd:string ;
+        knora-admin:phone                "123456"^^xsd:string ;
+        knora-admin:preferredLanguage    "en"^^xsd:string ;
+        knora-admin:status               "true"^^xsd:boolean ;
+        knora-admin:isInSystemAdminGroup "true"^^xsd:boolean .
+        """
+        response = requests.post(
+            graph_prefix + admin_graph,
+            files={"file": ("file.ttl", admin_user, "text/turtle; charset: utf-8")},
+            auth=("admin", "test"),
+            timeout=30,
+        )
+        if not response.ok:
+            logger.error(f"Cannot start DSP-API: Error when creating the admin user. response = {vars(response)}")
+            raise UserError("Cannot start DSP-API: Error when creating the admin user.")
+
     def _initialize_fuseki(self) -> None:
         """
         Create the "knora-test" repository and load some basic ontologies and data into it.
         """
         self._create_knora_test_repo()
-        self._load_data_into_repo()
+        if self.__stack_configuration.upload_test_data:
+            self._load_data_into_repo()
+        else:
+            self._create_admin_user()
 
     def _start_remaining_docker_containers(self) -> None:
         """
         Start the other Docker containers that are not running yet.
         (Fuseki is already running at this point.)
         """
         if self.__stack_configuration.latest_dev_version:
```

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/template.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/template.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/ark2iri.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/ark2iri.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/check_consistency_with_ontology.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/check_consistency_with_ontology.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/iri_resolver.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/iri_resolver.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/list_client.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/list_client.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/models/formatted_text_value.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/models/formatted_text_value.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/models/ontology_lookup_models.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/models/ontology_lookup_models.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/models/ontology_problem_models.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/models/ontology_problem_models.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/models/permission.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/models/permission.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/models/sipi.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/models/sipi.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/models/upload_state.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/models/upload_state.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/models/xmlallow.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/models/xmlallow.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/models/xmlbitstream.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/models/xmlbitstream.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/models/xmlpermission.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/models/xmlpermission.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/models/xmlproperty.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/models/xmlproperty.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/models/xmlresource.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/models/xmlresource.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/models/xmlvalue.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/models/xmlvalue.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/ontology_client.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/ontology_client.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/project_client.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/project_client.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/read_validate_xml_file.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/read_validate_xml_file.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/resource_create_client.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/resource_create_client.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/resource_multimedia.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/resource_multimedia.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/stash/construct_and_analyze_graph.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/stash/construct_and_analyze_graph.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/stash/graph_models.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/stash/graph_models.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/stash/stash_circular_references.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/stash/stash_circular_references.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/stash/stash_models.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/stash/stash_models.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/stash/upload_stashed_resptr_props.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/stash/upload_stashed_resptr_props.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/stash/upload_stashed_xml_texts.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/stash/upload_stashed_xml_texts.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/upload_config.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/upload_config.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/write_diagnostic_info.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/write_diagnostic_info.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/commands/xmlupload/xmlupload.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/commands/xmlupload/xmlupload.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/models/custom_warnings.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/models/custom_warnings.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/models/datetimestamp.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/models/datetimestamp.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/models/exceptions.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/models/exceptions.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/models/langstring.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/models/langstring.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/models/projectContext.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/models/projectContext.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/resources/0100-template-repo/template.json` & `dsp_tools-7.1.3.post2/src/dsp_tools/resources/0100-template-repo/template.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/resources/0100-template-repo/template.xml` & `dsp_tools-7.1.3.post2/src/dsp_tools/resources/0100-template-repo/template.xml`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/resources/schema/data.xsd` & `dsp_tools-7.1.3.post2/src/dsp_tools/resources/schema/data.xsd`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/resources/schema/lists-only.json` & `dsp_tools-7.1.3.post2/src/dsp_tools/resources/schema/lists-only.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/resources/schema/project.json` & `dsp_tools-7.1.3.post2/src/dsp_tools/resources/schema/project.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/resources/schema/properties-only.json` & `dsp_tools-7.1.3.post2/src/dsp_tools/resources/schema/properties-only.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/resources/schema/resources-only.json` & `dsp_tools-7.1.3.post2/src/dsp_tools/resources/schema/resources-only.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/resources/start-stack/docker-compose.yml` & `dsp_tools-7.1.3.post2/src/dsp_tools/resources/start-stack/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/utils/connection.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/utils/connection.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/utils/connection_live.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/utils/connection_live.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/utils/date_util.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/utils/date_util.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/utils/json_ld_util.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/utils/json_ld_util.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/utils/logger_config.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/utils/logger_config.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/utils/set_encoder.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/utils/set_encoder.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/utils/shared.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/utils/shared.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/utils/uri_util.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/utils/uri_util.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/utils/warnings_config.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/utils/warnings_config.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/utils/xml_utils.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/utils/xml_utils.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/utils/xml_validation.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/utils/xml_validation.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/src/dsp_tools/utils/xml_validation_models.py` & `dsp_tools-7.1.3.post2/src/dsp_tools/utils/xml_validation_models.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.3.post1/PKG-INFO` & `dsp_tools-7.1.3.post2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsp-tools
-Version: 7.1.3.post1
+Version: 7.1.3.post2
 Summary: DSP-TOOLS is a Python package with a command line interface that helps you interact with a DaSCH service platform (DSP) server.
 Home-page: https://www.dasch.swiss/
 License: GPL-3.0-only
 Author: DaSCH - Swiss National Data and Service Center for the Humanities
 Author-email: info@dasch.swiss
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

