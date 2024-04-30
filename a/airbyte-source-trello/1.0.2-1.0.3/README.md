# Comparing `tmp/airbyte-source-trello-1.0.2.tar.gz` & `tmp/airbyte_source_trello-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-source-trello-1.0.2.tar", last modified: Thu Feb  1 08:02:09 2024, max compression
+gzip compressed data, was "airbyte_source_trello-1.0.3.tar", max compression
```

## Comparing `airbyte-source-trello-1.0.2.tar` & `airbyte_source_trello-1.0.3.tar`

### file list

```diff
@@ -1,38 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 08:02:09.449895 airbyte-source-trello-1.0.2/
--rw-r--r--   0 root         (0) root         (0)     4165 2024-02-01 08:02:09.449895 airbyte-source-trello-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3995 2024-02-01 07:53:30.000000 airbyte-source-trello-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 08:02:09.449895 airbyte-source-trello-1.0.2/airbyte_source_trello.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4165 2024-02-01 08:02:09.000000 airbyte-source-trello-1.0.2/airbyte_source_trello.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1027 2024-02-01 08:02:09.000000 airbyte-source-trello-1.0.2/airbyte_source_trello.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-01 08:02:09.000000 airbyte-source-trello-1.0.2/airbyte_source_trello.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2024-02-01 08:02:09.000000 airbyte-source-trello-1.0.2/airbyte_source_trello.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-02-01 08:02:09.000000 airbyte-source-trello-1.0.2/airbyte_source_trello.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       43 2024-02-01 08:02:09.000000 airbyte-source-trello-1.0.2/airbyte_source_trello.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 08:02:09.445895 airbyte-source-trello-1.0.2/integration_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-02-01 07:53:30.000000 airbyte-source-trello-1.0.2/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      479 2024-02-01 07:53:30.000000 airbyte-source-trello-1.0.2/integration_tests/abnormal_state.json
--rw-r--r--   0 root         (0) root         (0)      435 2024-02-01 07:53:30.000000 airbyte-source-trello-1.0.2/integration_tests/acceptance.py
--rw-r--r--   0 root         (0) root         (0)      526 2024-02-01 07:53:30.000000 airbyte-source-trello-1.0.2/integration_tests/catalog.json
--rw-r--r--   0 root         (0) root         (0)     2233 2024-02-01 07:53:30.000000 airbyte-source-trello-1.0.2/integration_tests/configured_catalog.json
--rw-r--r--   0 root         (0) root         (0)       99 2024-02-01 07:53:30.000000 airbyte-source-trello-1.0.2/integration_tests/invalid_config.json
--rw-r--r--   0 root         (0) root         (0)       83 2024-02-01 07:53:30.000000 airbyte-source-trello-1.0.2/integration_tests/sample_config.json
--rw-r--r--   0 root         (0) root         (0)       62 2024-02-01 07:53:30.000000 airbyte-source-trello-1.0.2/integration_tests/sample_state.json
--rw-r--r--   0 root         (0) root         (0)     4034 2024-02-01 08:02:09.449895 airbyte-source-trello-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      916 2024-02-01 08:02:07.000000 airbyte-source-trello-1.0.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 08:02:09.445895 airbyte-source-trello-1.0.2/source_trello/
--rw-r--r--   0 root         (0) root         (0)      124 2024-02-01 07:53:30.000000 airbyte-source-trello-1.0.2/source_trello/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1720 2024-02-01 07:53:30.000000 airbyte-source-trello-1.0.2/source_trello/components.py
--rw-r--r--   0 root         (0) root         (0)     8425 2024-02-01 07:53:30.000000 airbyte-source-trello-1.0.2/source_trello/manifest.yaml
--rw-r--r--   0 root         (0) root         (0)      230 2024-02-01 07:53:30.000000 airbyte-source-trello-1.0.2/source_trello/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 08:02:09.449895 airbyte-source-trello-1.0.2/source_trello/schemas/
--rw-r--r--   0 root         (0) root         (0)     7626 2024-02-01 07:53:30.000000 airbyte-source-trello-1.0.2/source_trello/schemas/actions.json
--rw-r--r--   0 root         (0) root         (0)     5759 2024-02-01 07:53:30.000000 airbyte-source-trello-1.0.2/source_trello/schemas/boards.json
--rw-r--r--   0 root         (0) root         (0)     5775 2024-02-01 07:53:30.000000 airbyte-source-trello-1.0.2/source_trello/schemas/cards.json
--rw-r--r--   0 root         (0) root         (0)    13173 2024-02-01 07:53:30.000000 airbyte-source-trello-1.0.2/source_trello/schemas/checklists.json
--rw-r--r--   0 root         (0) root         (0)      449 2024-02-01 07:53:30.000000 airbyte-source-trello-1.0.2/source_trello/schemas/lists.json
--rw-r--r--   0 root         (0) root         (0)     4549 2024-02-01 07:53:30.000000 airbyte-source-trello-1.0.2/source_trello/schemas/organizations.json
--rw-r--r--   0 root         (0) root         (0)      264 2024-02-01 07:53:30.000000 airbyte-source-trello-1.0.2/source_trello/schemas/users.json
--rw-r--r--   0 root         (0) root         (0)      475 2024-02-01 07:53:30.000000 airbyte-source-trello-1.0.2/source_trello/source.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 08:02:09.449895 airbyte-source-trello-1.0.2/unit_tests/
--rw-r--r--   0 root         (0) root         (0)     1106 2024-02-01 07:53:30.000000 airbyte-source-trello-1.0.2/unit_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2686 2024-02-01 07:53:30.000000 airbyte-source-trello-1.0.2/unit_tests/test_order_ids_partition_router.py
+-rw-r--r--   0        0        0     3995 2024-04-30 17:22:09.000000 airbyte_source_trello-1.0.3/README.md
+-rw-r--r--   0        0        0      737 2024-04-30 17:41:27.491454 airbyte_source_trello-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      124 2024-04-30 17:22:09.000000 airbyte_source_trello-1.0.3/source_trello/__init__.py
+-rw-r--r--   0        0        0     1760 2024-04-30 17:22:09.000000 airbyte_source_trello-1.0.3/source_trello/components.py
+-rw-r--r--   0        0        0     8416 2024-04-30 17:22:09.000000 airbyte_source_trello-1.0.3/source_trello/manifest.yaml
+-rw-r--r--   0        0        0      230 2024-04-30 17:22:09.000000 airbyte_source_trello-1.0.3/source_trello/run.py
+-rw-r--r--   0        0        0     7626 2024-04-30 17:22:09.000000 airbyte_source_trello-1.0.3/source_trello/schemas/actions.json
+-rw-r--r--   0        0        0     5759 2024-04-30 17:22:09.000000 airbyte_source_trello-1.0.3/source_trello/schemas/boards.json
+-rw-r--r--   0        0        0     5775 2024-04-30 17:22:09.000000 airbyte_source_trello-1.0.3/source_trello/schemas/cards.json
+-rw-r--r--   0        0        0    13173 2024-04-30 17:22:09.000000 airbyte_source_trello-1.0.3/source_trello/schemas/checklists.json
+-rw-r--r--   0        0        0      449 2024-04-30 17:22:09.000000 airbyte_source_trello-1.0.3/source_trello/schemas/lists.json
+-rw-r--r--   0        0        0     4549 2024-04-30 17:22:09.000000 airbyte_source_trello-1.0.3/source_trello/schemas/organizations.json
+-rw-r--r--   0        0        0      264 2024-04-30 17:22:09.000000 airbyte_source_trello-1.0.3/source_trello/schemas/users.json
+-rw-r--r--   0        0        0      475 2024-04-30 17:22:09.000000 airbyte_source_trello-1.0.3/source_trello/source.py
+-rw-r--r--   0        0        0     4697 1970-01-01 00:00:00.000000 airbyte_source_trello-1.0.3/PKG-INFO
```

### Comparing `airbyte-source-trello-1.0.2/PKG-INFO` & `airbyte_source_trello-1.0.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,70 +1,67 @@
-Metadata-Version: 2.1
-Name: airbyte-source-trello
-Version: 1.0.2
-Summary: Source implementation for Trello.
-Author: Airbyte
-Author-email: contact@airbyte.io
-Description-Content-Type: text/markdown
-Requires-Dist: airbyte-cdk
-Provides-Extra: tests
-Requires-Dist: requests-mock~=1.9.3; extra == "tests"
-Requires-Dist: pytest~=6.2; extra == "tests"
-Requires-Dist: pytest-mock~=3.6.1; extra == "tests"
-
 # Trello Source
 
 This is the repository for the Trello configuration based source connector.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/trello).
 
+## Local development
 
+#### Create credentials
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/trello)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_trello/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `integration_tests/sample_config.json` for a sample config file.
 
 **If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source trello test creds`
 and place them into `secrets/config.json`.
 
+### Locally running the connector docker image
 
 
+#### Build
 **Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
 ```bash
 airbyte-ci connectors --name=source-trello build
 ```
 
 An image will be built with the tag `airbyte/source-trello:dev`.
 
 **Via `docker build`:**
 ```bash
 docker build -t airbyte/source-trello:dev .
 ```
 
+#### Run
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-trello:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-trello:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-trello:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-trello:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
+## Testing
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-trello test
 ```
 
+### Customizing acceptance Tests
 Customize `acceptance-test-config.yml` file to configure tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
+## Dependency Management
 All of your dependencies should go in `setup.py`, NOT `requirements.txt`. The requirements file is only used to connect internal Airbyte dependencies in the monorepo for local development.
 We split dependencies between two groups, dependencies that are:
 * required for your connector to work need to go to `MAIN_REQUIREMENTS` list.
 * required for the testing need to go to `TEST_REQUIREMENTS` list
 
+### Publishing a new version of the connector
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-trello test`
 2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/trello.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+
```

### Comparing `airbyte-source-trello-1.0.2/README.md` & `airbyte_source_trello-1.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: airbyte-source-trello
+Version: 1.0.3
+Summary: Source implementation for Trello.
+Home-page: https://airbyte.com
+License: MIT
+Author: Airbyte
+Author-email: contact@airbyte.io
+Requires-Python: >=3.9,<3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: airbyte-cdk (>=0,<1)
+Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/trello
+Project-URL: Repository, https://github.com/airbytehq/airbyte
+Description-Content-Type: text/markdown
+
 # Trello Source
 
 This is the repository for the Trello configuration based source connector.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/trello).
 
 ## Local development
 
@@ -61,7 +80,8 @@
 2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/trello.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
 
+
```

### Comparing `airbyte-source-trello-1.0.2/source_trello/components.py` & `airbyte_source_trello-1.0.3/source_trello/components.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         stream_map = {stream_config.stream.name: stream_config.stream for stream_config in self.parent_stream_configs}
 
         board_ids = set(self.config.get("board_ids", []))
         if not board_ids:
             board_ids = self.read_all_boards(stream_boards=stream_map["boards"], stream_organizations=stream_map["organizations"])
 
         for board_id in board_ids:
-            yield {"id": board_id}
+            yield StreamSlice(partition={"id": board_id}, cursor_slice={})
 
     def read_all_boards(self, stream_boards: Stream, stream_organizations: Stream):
         """
         Method to get id of each board in the boards stream,
         get ids of boards associated with each organization in the organizations stream
         and yield each unique board id
         """
```

### Comparing `airbyte-source-trello-1.0.2/source_trello/manifest.yaml` & `airbyte_source_trello-1.0.3/source_trello/manifest.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-version: 0.51.2
+version: 0.85.0
 type: DeclarativeSource
 
 check:
   type: CheckStream
   stream_names:
     - boards
 
@@ -45,16 +45,16 @@
     page_size_option:
       type: RequestOption
       field_name: limit
       inject_into: request_parameter
     pagination_strategy:
       type: CursorPagination
       page_size: 500
-      cursor_value: "{{ (last_records|last)['id'] }}"
-      stop_condition: "{{ not last_records }}"
+      cursor_value: "{{ last_record['id'] }}"
+      stop_condition: "{{ not last_record }}"
   board_id_partition_router:
     - type: CustomPartitionRouter
       class_name: source_trello.components.OrderIdsPartitionRouter
       parent_stream_configs:
         - type: ParentStreamConfig
           parent_key: id
           partition_field: id
```

### Comparing `airbyte-source-trello-1.0.2/source_trello/schemas/actions.json` & `airbyte_source_trello-1.0.3/source_trello/schemas/actions.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-trello-1.0.2/source_trello/schemas/boards.json` & `airbyte_source_trello-1.0.3/source_trello/schemas/boards.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-trello-1.0.2/source_trello/schemas/cards.json` & `airbyte_source_trello-1.0.3/source_trello/schemas/cards.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-trello-1.0.2/source_trello/schemas/checklists.json` & `airbyte_source_trello-1.0.3/source_trello/schemas/checklists.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-trello-1.0.2/source_trello/schemas/organizations.json` & `airbyte_source_trello-1.0.3/source_trello/schemas/organizations.json`

 * *Files identical despite different names*

