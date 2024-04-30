# Comparing `tmp/stackql_deploy-1.2.0.tar.gz` & `tmp/stackql_deploy-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stackql_deploy-1.2.0.tar", last modified: Tue Apr 23 07:47:22 2024, max compression
+gzip compressed data, was "stackql_deploy-1.5.0.tar", last modified: Tue Apr 30 05:55:00 2024, max compression
```

## Comparing `stackql_deploy-1.2.0.tar` & `stackql_deploy-1.5.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-23 07:47:22.805036 stackql_deploy-1.2.0/
--rwxrwxrwx   0 javen     (1000) javen     (1000)     1071 2024-03-15 01:52:38.000000 stackql_deploy-1.2.0/LICENSE
--rwxrwxrwx   0 javen     (1000) javen     (1000)     9078 2024-04-23 07:47:22.769729 stackql_deploy-1.2.0/PKG-INFO
--rwxrwxrwx   0 javen     (1000) javen     (1000)     8359 2024-04-17 09:11:17.000000 stackql_deploy-1.2.0/README.rst
--rwxrwxrwx   0 javen     (1000) javen     (1000)       38 2024-04-23 07:47:22.808034 stackql_deploy-1.2.0/setup.cfg
--rwxrwxrwx   0 javen     (1000) javen     (1000)     1703 2024-04-23 07:44:56.000000 stackql_deploy-1.2.0/setup.py
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-23 07:47:12.492136 stackql_deploy-1.2.0/stackql_deploy/
--rwxrwxrwx   0 javen     (1000) javen     (1000)       23 2024-04-23 07:44:56.000000 stackql_deploy-1.2.0/stackql_deploy/__init__.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     9131 2024-04-23 00:07:37.000000 stackql_deploy-1.2.0/stackql_deploy/cli.py
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-23 07:47:18.892313 stackql_deploy-1.2.0/stackql_deploy/cmd/
--rwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 23:31:31.000000 stackql_deploy-1.2.0/stackql_deploy/cmd/__init__.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     8160 2024-04-23 00:59:43.000000 stackql_deploy-1.2.0/stackql_deploy/cmd/build.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     3433 2024-04-16 23:17:44.000000 stackql_deploy-1.2.0/stackql_deploy/cmd/teardown.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     2542 2024-04-16 23:17:44.000000 stackql_deploy-1.2.0/stackql_deploy/cmd/test.py
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-23 07:47:22.085803 stackql_deploy-1.2.0/stackql_deploy/lib/
--rwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 23:31:31.000000 stackql_deploy-1.2.0/stackql_deploy/lib/__init__.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)      192 2024-04-20 03:11:50.000000 stackql_deploy-1.2.0/stackql_deploy/lib/bootstrap.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     4061 2024-04-22 20:59:53.000000 stackql_deploy-1.2.0/stackql_deploy/lib/config.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     3985 2024-04-22 21:39:51.000000 stackql_deploy-1.2.0/stackql_deploy/lib/templating.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     6689 2024-04-23 05:16:36.000000 stackql_deploy-1.2.0/stackql_deploy/lib/utils.py
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-23 07:47:22.188839 stackql_deploy-1.2.0/stackql_deploy/templates/
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-23 07:47:22.338029 stackql_deploy-1.2.0/stackql_deploy/templates/stackql_docs/
--rwxrwxrwx   0 javen     (1000) javen     (1000)       62 2024-04-17 05:34:52.000000 stackql_deploy-1.2.0/stackql_deploy/templates/stackql_docs/stackql_example_rg.md.template
--rwxrwxrwx   0 javen     (1000) javen     (1000)      712 2024-04-17 05:34:52.000000 stackql_deploy-1.2.0/stackql_deploy/templates/stackql_manifest.yml.template
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-23 07:47:22.470565 stackql_deploy-1.2.0/stackql_deploy/templates/stackql_resources/
--rwxrwxrwx   0 javen     (1000) javen     (1000)      892 2024-04-17 05:34:52.000000 stackql_deploy-1.2.0/stackql_deploy/templates/stackql_resources/stackql_example_rg.iql.template
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-23 07:47:22.617423 stackql_deploy-1.2.0/stackql_deploy/templates/stackql_tests/
--rwxrwxrwx   0 javen     (1000) javen     (1000)      726 2024-04-17 05:34:52.000000 stackql_deploy-1.2.0/stackql_deploy/templates/stackql_tests/stackql_example_rg.iql.template
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-23 07:47:22.731727 stackql_deploy-1.2.0/stackql_deploy.egg-info/
--rwxrwxrwx   0 javen     (1000) javen     (1000)     9078 2024-04-23 07:47:04.000000 stackql_deploy-1.2.0/stackql_deploy.egg-info/PKG-INFO
--rwxrwxrwx   0 javen     (1000) javen     (1000)      846 2024-04-23 07:47:11.000000 stackql_deploy-1.2.0/stackql_deploy.egg-info/SOURCES.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)        1 2024-04-23 07:47:04.000000 stackql_deploy-1.2.0/stackql_deploy.egg-info/dependency_links.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)       58 2024-04-23 07:47:04.000000 stackql_deploy-1.2.0/stackql_deploy.egg-info/entry_points.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)       44 2024-04-23 07:47:04.000000 stackql_deploy-1.2.0/stackql_deploy.egg-info/requires.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)       15 2024-04-23 07:47:04.000000 stackql_deploy-1.2.0/stackql_deploy.egg-info/top_level.txt
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-30 05:55:00.684119 stackql_deploy-1.5.0/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     1071 2024-03-15 01:52:38.000000 stackql_deploy-1.5.0/LICENSE
+-rwxrwxrwx   0 javen     (1000) javen     (1000)    14058 2024-04-30 05:55:00.668063 stackql_deploy-1.5.0/PKG-INFO
+-rwxrwxrwx   0 javen     (1000) javen     (1000)    13456 2024-04-30 05:54:37.000000 stackql_deploy-1.5.0/README.rst
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       38 2024-04-30 05:55:00.686119 stackql_deploy-1.5.0/setup.cfg
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     1705 2024-04-30 05:26:37.000000 stackql_deploy-1.5.0/setup.py
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-30 05:54:59.798435 stackql_deploy-1.5.0/stackql_deploy/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       23 2024-04-30 05:28:09.000000 stackql_deploy-1.5.0/stackql_deploy/__init__.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     9137 2024-04-29 20:52:47.000000 stackql_deploy-1.5.0/stackql_deploy/cli.py
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-30 05:55:00.140734 stackql_deploy-1.5.0/stackql_deploy/cmd/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 23:31:31.000000 stackql_deploy-1.5.0/stackql_deploy/cmd/__init__.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)    12761 2024-04-30 03:13:03.000000 stackql_deploy-1.5.0/stackql_deploy/cmd/build.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     3435 2024-04-29 20:52:47.000000 stackql_deploy-1.5.0/stackql_deploy/cmd/teardown.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     4757 2024-04-30 03:14:29.000000 stackql_deploy-1.5.0/stackql_deploy/cmd/test.py
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-30 05:55:00.340212 stackql_deploy-1.5.0/stackql_deploy/lib/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 23:31:31.000000 stackql_deploy-1.5.0/stackql_deploy/lib/__init__.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)      192 2024-04-20 03:11:50.000000 stackql_deploy-1.5.0/stackql_deploy/lib/bootstrap.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     4061 2024-04-22 20:59:53.000000 stackql_deploy-1.5.0/stackql_deploy/lib/config.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     3985 2024-04-22 21:39:51.000000 stackql_deploy-1.5.0/stackql_deploy/lib/templating.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     6689 2024-04-23 05:16:36.000000 stackql_deploy-1.5.0/stackql_deploy/lib/utils.py
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-30 05:55:00.383754 stackql_deploy-1.5.0/stackql_deploy/templates/
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-30 05:55:00.432341 stackql_deploy-1.5.0/stackql_deploy/templates/stackql_docs/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       62 2024-04-17 05:34:52.000000 stackql_deploy-1.5.0/stackql_deploy/templates/stackql_docs/stackql_example_rg.md.template
+-rwxrwxrwx   0 javen     (1000) javen     (1000)      712 2024-04-17 05:34:52.000000 stackql_deploy-1.5.0/stackql_deploy/templates/stackql_manifest.yml.template
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-30 05:55:00.478921 stackql_deploy-1.5.0/stackql_deploy/templates/stackql_queries/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)      726 2024-04-17 05:34:52.000000 stackql_deploy-1.5.0/stackql_deploy/templates/stackql_queries/stackql_example_rg.iql.template
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-30 05:55:00.599374 stackql_deploy-1.5.0/stackql_deploy/templates/stackql_resources/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)      892 2024-04-17 05:34:52.000000 stackql_deploy-1.5.0/stackql_deploy/templates/stackql_resources/stackql_example_rg.iql.template
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-30 05:55:00.649118 stackql_deploy-1.5.0/stackql_deploy.egg-info/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)    14058 2024-04-30 05:54:59.000000 stackql_deploy-1.5.0/stackql_deploy.egg-info/PKG-INFO
+-rwxrwxrwx   0 javen     (1000) javen     (1000)      848 2024-04-30 05:54:59.000000 stackql_deploy-1.5.0/stackql_deploy.egg-info/SOURCES.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)        1 2024-04-30 05:54:59.000000 stackql_deploy-1.5.0/stackql_deploy.egg-info/dependency_links.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       58 2024-04-30 05:54:59.000000 stackql_deploy-1.5.0/stackql_deploy.egg-info/entry_points.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       44 2024-04-30 05:54:59.000000 stackql_deploy-1.5.0/stackql_deploy.egg-info/requires.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       15 2024-04-30 05:54:59.000000 stackql_deploy-1.5.0/stackql_deploy.egg-info/top_level.txt
```

### Comparing `stackql_deploy-1.2.0/LICENSE` & `stackql_deploy-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stackql_deploy-1.2.0/PKG-INFO` & `stackql_deploy-1.5.0/README.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,222 +1,314 @@
-Metadata-Version: 2.1
-Name: stackql-deploy
-Version: 1.2.0
-Summary: Model driven resource provisioning and deployment framework using StackQL.
-Home-page: https://github.com/stackql/stackql-deploy
-Author: Jeffrey Aven
-Author-email: javen@stackql.io
-License: MIT
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: License :: OSI Approved :: MIT License
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-Requires-Dist: click
-Requires-Dist: python-dotenv
-Requires-Dist: jinja2
-Requires-Dist: pystackql>=3.6.1
-
-.. image:: https://stackql.io/img/stackql-logo-bold.png
-    :alt: "stackql logo"
-    :target: https://github.com/stackql/stackql
-    :align: center
-
-==========================================================================
-Model driven resource provisioning and deployment framework using StackQL.
-==========================================================================
-
-.. .. image:: https://readthedocs.org/projects/pystackql/badge/?version=latest
-..    :target: https://pystackql.readthedocs.io/en/latest/
-..    :alt: Documentation Status
-
-.. image:: https://img.shields.io/pypi/v/stackql-deploy
-   :target: https://pypi.org/project/stackql-deploy/
-   :alt: PyPI
-
-==============
-
-**stackql-deploy** is a multi-cloud Infrastructure as Code (IaC) framework using `stackql`_, inspired by dbt (data build tool), which manages data transformation workflows in analytics engineering by treating SQL scripts as models that can be built, tested, and materialized incrementally. You can create a similar framework for infrastructure provisioning with StackQL. The goal is to treat infrastructure-as-code (IaC) queries as models that can be deployed, managed, and interconnected.
-
-This ELT/model-based framework to IaC allows you to provision, test, update and teardown multi-cloud stacks similar to how dbt manages data transformation projects, with the benefits of version control, peer review, and automation. This approach enables you to deploy complex, dependent infrastructure components in a reliable and repeatable manner.
-
-The use of StackQL simplifies the interaction with cloud resources by using SQL-like syntax, making it easier to define and execute complex cloud management operations. Resources are provisioned with ``INSERT`` statements and tests are structured around ``SELECT`` statements.
-
-Features include:
-
-- Dynamic state determination (eliminating the need for state files)
-- Simple flow control with rollback capabilities
-- Single code base for multiple target environments
-- SQL-based definitions for resources and tests
-
-How stackql-deploy Works
-------------------------
-
-**stackql-deploy** orchestrates cloud resource provisioning by parsing SQL-like definitions. It determines the necessity of creating or updating resources based on preflight checks, and ensures the creation and correct desired configuration through post-deployment verifications.
-
-.. image:: https://stackql.io/img/blog/stackql-deploy.png
-    :alt: "stackql-deploy"
-    :target: https://github.com/stackql/stackql
-
-Installing from PyPI
---------------------
-
-To install **stackql-deploy** directly from PyPI, run the following command:
-
-.. code-block:: none
-
-    pip install stackql-deploy
-
-This will install the latest version of **stackql-deploy** and its dependencies from the Python Package Index.
-
-Running stackql-deploy
-----------------------
-
-Once installed, use the `build`, `test`, or `teardown` commands as shown here:
-
-.. code-block:: none
-
-    stackql-deploy build prd example_stack -e AZURE_SUBSCRIPTION_ID 00000000-0000-0000-0000-000000000000 --dry-run
-    stackql-deploy build prd example_stack -e AZURE_SUBSCRIPTION_ID 00000000-0000-0000-0000-000000000000
-    stackql-deploy test prd example_stack -e AZURE_SUBSCRIPTION_ID 00000000-0000-0000-0000-000000000000
-    stackql-deploy teardown prd example_stack -e AZURE_SUBSCRIPTION_ID 00000000-0000-0000-0000-000000000000
-
-.. note::
-   ``teardown`` deprovisions resources in reverse order to creation
-
-additional options include:
-
-- ``--dry-run``: perform a dry run of the stack operations.
-- ``--on-failure=rollback``: action on failure: rollback, ignore or error.
-- ``--env-file=.env``: specify an environment variable file.
-- ``-e KEY=value```: pass additional environment variables.
-- ``--log-level`` : logging level (DEBUG, INFO, WARNING, ERROR, CRITICAL), defaults to INFO.
-
-use ``stackql-deploy info`` to show information about the package and environment, for example
-
-.. code-block:: none
-
-    $ stackql-deploy info
-    stackql-deploy version: 1.0.0
-    pystackql version     : 3.5.4
-    stackql version       : v0.5.612
-    stackql binary path   : /mnt/c/LocalGitRepos/stackql/stackql-deploy/stackql
-    platform              : Linux x86_64 (Linux-5.15.133.1-microsoft-standard-WSL2-x86_64-with-glibc2.35), Python 3.10.12
-
-Use the ``--help`` option to see more information about the commands and options available:
-
-.. code-block:: none
-
-    stackql-deploy --help
-
-Project Structure
------------------
-
-**stackql-deploy** uses a modular structure where each component of the infrastructure is defined in separate files, allowing for clear separation of concerns and easy management. This example is based on a stack named ``example_stack``, with a resource named ``monitor_resource_group``.
-
-::
-
-    ├── example_stack
-    │   ├── stackql_docs
-    │   │   └── monitor_resource_group.md
-    │   ├── stackql_manifest.yml
-    │   ├── stackql_resources
-    │   │   └── monitor_resource_group.iql
-    │   └── stackql_tests
-    │       └── monitor_resource_group.iql
-
-.. note::
-   use the ``init`` command to create a new project structure with sample files, for example ``stackql-deploy init example_stack``
-
-Manifest File
--------------
-
-- **Manifest File**: The ``stackql_manifest.yml`` is used to define your stack and manage dependencies between infrastructure components. This file defines which resources need to be provisioned before others and parameterizes resources based on environment variables or other configurations.
-
-.. code-block:: yaml
-
-    version: 1
-    name: example_stack
-    description: oss activity monitor stack
-    providers:
-      - azure
-    globals:
-      - name: subscription_id
-        description: azure subscription id
-        value: "{{ vars.AZURE_SUBSCRIPTION_ID }}"
-      - name: location
-        value: eastus
-      - name: resource_group_name_base
-        value: "activity-monitor"
-    resources:
-      - name: monitor_resource_group
-        description: azure resource group for activity monitor
-        props:
-          - name: resource_group_name
-            description: azure resource group name
-            value: "{{ globals.resource_group_name_base }}-{{ globals.stack_env }}"
-            # OR YOU CAN DO...
-            # values:
-            #   prd:
-            #     value: "activity-monitor-prd"
-            #   sit:
-            #     value: "activity-monitor-sit"
-            #   dev:
-            #     value: "activity-monitor-dev"
-
-
-Resource and Test SQL Files
-----------------------------
-
-These files define the SQL-like commands for creating, updating, and testing the deployment of resources.
-
-**Resource SQL (stackql_resources/monitor_resource_group.iql):**
-
-.. code-block:: sql
-
-    /*+ create */
-    INSERT INTO azure.resources.resource_groups(
-      resourceGroupName,
-      subscriptionId,
-      data__location
-    )
-    SELECT
-      '{{ resource_group_name }}',
-      '{{ subscription_id }}',
-      '{{ location }}'
-
-    /*+ update */
-    UPDATE azure.resources.resource_groups
-    SET data__location = '{{ location }}'
-    WHERE resourceGroupName = '{{ resource_group_name }}'
-      AND subscriptionId = '{{ subscription_id }}'
-
-    /*+ delete */
-    DELETE FROM azure.resources.resource_groups
-    WHERE resourceGroupName = '{{ resource_group_name }}' AND subscriptionId = '{{ subscription_id }}'
-
-**Test SQL (stackql_tests/monitor_resource_group.iql):**
-
-.. code-block:: sql
-
-    /*+ preflight */
-    SELECT COUNT(*) as count FROM azure.resources.resource_groups
-    WHERE subscriptionId = '{{ subscription_id }}'
-    AND resourceGroupName = '{{ resource_group_name }}'
-
-    /*+ postdeploy, retries=5, retry_delay=5 */
-    SELECT COUNT(*) as count FROM azure.resources.resource_groups
-    WHERE subscriptionId = '{{ subscription_id }}'
-    AND resourceGroupName = '{{ resource_group_name }}'
-    AND location = '{{ location }}'
-    AND JSON_EXTRACT(properties, '$.provisioningState') = 'Succeeded'
-
-**stackql-deploy** simplifies cloud resource management by treating infrastructure as flexible, dynamically assessed code.
-
-.. _stackql: https://github.com/stackql/stackql
+.. image:: https://stackql.io/img/stackql-logo-bold.png
+    :alt: "stackql logo"
+    :target: https://github.com/stackql/stackql
+    :align: center
+
+==========================================================================
+Model driven resource provisioning and deployment framework using StackQL.
+==========================================================================
+
+.. .. image:: https://readthedocs.org/projects/pystackql/badge/?version=latest
+..    :target: https://pystackql.readthedocs.io/en/latest/
+..    :alt: Documentation Status
+
+.. image:: https://img.shields.io/pypi/v/stackql-deploy
+   :target: https://pypi.org/project/stackql-deploy/
+   :alt: PyPI
+
+==============
+
+**stackql-deploy** is a multi-cloud Infrastructure as Code (IaC) framework using `stackql`_, inspired by dbt (data build tool), which manages data transformation workflows in analytics engineering by treating SQL scripts as models that can be built, tested, and materialized incrementally. You can create a similar framework for infrastructure provisioning with StackQL. The goal is to treat infrastructure-as-code (IaC) queries as models that can be deployed, managed, and interconnected.
+
+This ELT/model-based framework to IaC allows you to provision, test, update and teardown multi-cloud stacks similar to how dbt manages data transformation projects, with the benefits of version control, peer review, and automation. This approach enables you to deploy complex, dependent infrastructure components in a reliable and repeatable manner.
+
+The use of StackQL simplifies the interaction with cloud resources by using SQL-like syntax, making it easier to define and execute complex cloud management operations. Resources are provisioned with ``INSERT`` statements and tests are structured around ``SELECT`` statements.
+
+Features include:
+
+- Dynamic state determination (eliminating the need for state files)
+- Simple flow control with rollback capabilities
+- Single code base for multiple target environments
+- SQL-based definitions for resources and tests
+
+How stackql-deploy Works
+------------------------
+
+**stackql-deploy** orchestrates cloud resource provisioning by parsing SQL-like definitions. It determines the necessity of creating or updating resources based on preflight checks, and ensures the creation and correct desired configuration through post-deployment verifications.
+
+.. image:: https://stackql.io/img/blog/stackql-deploy.png
+    :alt: "stackql-deploy"
+    :target: https://github.com/stackql/stackql
+
+Installing from PyPI
+--------------------
+
+To install **stackql-deploy** directly from PyPI, run the following command:
+
+.. code-block:: none
+
+    pip install stackql-deploy
+
+This will install the latest version of **stackql-deploy** and its dependencies from the Python Package Index.
+
+Running stackql-deploy
+----------------------
+
+Once installed, use the `build`, `test`, or `teardown` commands as shown here:
+
+.. code-block:: none
+
+    stackql-deploy build prd example_stack -e AZURE_SUBSCRIPTION_ID 00000000-0000-0000-0000-000000000000 --dry-run
+    stackql-deploy build prd example_stack -e AZURE_SUBSCRIPTION_ID 00000000-0000-0000-0000-000000000000
+    stackql-deploy test prd example_stack -e AZURE_SUBSCRIPTION_ID 00000000-0000-0000-0000-000000000000
+    stackql-deploy teardown prd example_stack -e AZURE_SUBSCRIPTION_ID 00000000-0000-0000-0000-000000000000
+
+.. note::
+   ``teardown`` deprovisions resources in reverse order to creation
+
+additional options include:
+
+- ``--dry-run``: perform a dry run of the stack operations.
+- ``--on-failure=rollback``: action on failure: rollback, ignore or error.
+- ``--env-file=.env``: specify an environment variable file.
+- ``-e KEY=value```: pass additional environment variables.
+- ``--log-level`` : logging level (DEBUG, INFO, WARNING, ERROR, CRITICAL), defaults to INFO.
+
+use ``stackql-deploy info`` to show information about the package and environment, for example
+
+.. code-block:: none
+
+    $ stackql-deploy info
+    stackql-deploy version: 1.0.0
+    pystackql version     : 3.5.4
+    stackql version       : v0.5.612
+    stackql binary path   : /mnt/c/LocalGitRepos/stackql/stackql-deploy/stackql
+    platform              : Linux x86_64 (Linux-5.15.133.1-microsoft-standard-WSL2-x86_64-with-glibc2.35), Python 3.10.12
+
+Use the ``--help`` option to see more information about the commands and options available:
+
+.. code-block:: none
+
+    stackql-deploy --help
+
+Project Structure
+-----------------
+
+**stackql-deploy** uses a modular structure where each component of the infrastructure is defined in separate files, allowing for clear separation of concerns and easy management. This example is based on a stack named ``example_stack``, with a resource named ``monitor_resource_group``.
+
+::
+
+    ├── example_stack
+    │   ├── stackql_docs
+    │   │   └── monitor_resource_group.md
+    │   ├── stackql_manifest.yml
+    │   ├── stackql_resources
+    │   │   └── monitor_resource_group.iql
+    │   └── stackql_queries
+    │       └── monitor_resource_group.iql
+
+.. note::
+   use the ``init`` command to create a new project structure with sample files, for example ``stackql-deploy init example_stack``
+
+Manifest File
+-------------
+
+- **Manifest File**: The ``stackql_manifest.yml`` is used to define your stack and manage dependencies between infrastructure components. This file defines which resources need to be provisioned before others and parameterizes resources based on environment variables or other configurations.
+
+- **Providers**: List the cloud service providers that your stack will interact with. Each provider specified in the list will be initialized and made ready for use with the stack.
+
+  .. code-block:: yaml
+
+    providers:
+      - azure
+      - github
+
+- **Globals**: Defines a set of global variables that can be used across the entire stack configuration. These variables can hold values related to environment settings, default configurations, or any commonly used data.
+
+  .. code-block:: yaml
+
+    globals:
+      - name: subscription_id
+        description: azure subscription id
+        value: "{{ vars.AZURE_SUBSCRIPTION_ID }}"
+      - name: location
+        value: eastus
+      ... (additional globals)
+
+- **Resources**: Describes all the infrastructure components, such as networks, compute instances, databases, etc., that make up your stack. Here you can define the resources, their properties, and any dependencies between them.
+
+  .. code-block:: yaml
+
+    resources:
+      - name: resource_group
+        description: azure resource group for activity monitor app
+      - name: storage_account
+        description: azure storage account for activity monitor app
+        ... (additional properties and exports)
+      ...
+
+  Each resource can have the following attributes:
+
+  - **Name**: A unique identifier for the resource within the stack.
+  - **Description**: A brief explanation of the resource's purpose and functionality.
+  - **Type**: (Optional) Specifies the kind of resource (e.g., 'resource', 'query', 'script').
+  - **Props**: (Optional) Lists the properties of the resource that define its configuration.
+  - **Exports**: (Optional) Variables that are exported by this resource which can be used by other resources.
+  - **Protected**: (Optional) A list of sensitive information that should not be logged or exposed outside secure contexts.
+
+- **Scripts**: If your stack involves the execution of scripts for setup, data manipulation, or deployment actions, they are defined under the resources with a type of 'script'.
+
+  .. code-block:: yaml
+
+    - name: install_dependencies
+      type: script
+      run: |
+        pip install pynacl
+    ...
+
+  The script's execution output can be captured and used within the stack or for further processing.
+
+- **Integration with External Systems**: For stacks that interact with external services like GitHub, special resource types like 'query' can be used to fetch data from these services and use it within your deployment.
+
+  .. code-block:: yaml
+
+    - name: get_github_public_key
+      type: query
+      ... (additional properties and exports)
+
+  This can be useful for dynamic configurations based on external state or metadata.
+
+Resource and Test SQL Files
+----------------------------
+
+These files define the SQL-like commands for creating, updating, and testing the deployment of resources.
+
+.. note:: 
+   The SQL files use special **anchors** to indicate operations such as create, update, delete for resources, 
+   and preflight or post-deployment checks for queries. For detailed explanations of these anchors, refer to the 
+   `Resource SQL Anchors`_ and `Query SQL Anchors`_ sections.
+
+**Resource SQL (stackql_resources/monitor_resource_group.iql):**
+
+.. code-block:: sql
+
+    /*+ create */
+    INSERT INTO azure.resources.resource_groups(
+      resourceGroupName,
+      subscriptionId,
+      data__location
+    )
+    SELECT
+      '{{ resource_group_name }}',
+      '{{ subscription_id }}',
+      '{{ location }}'
+
+    /*+ update */
+    UPDATE azure.resources.resource_groups
+    SET data__location = '{{ location }}'
+    WHERE resourceGroupName = '{{ resource_group_name }}'
+      AND subscriptionId = '{{ subscription_id }}'
+
+    /*+ delete */
+    DELETE FROM azure.resources.resource_groups
+    WHERE resourceGroupName = '{{ resource_group_name }}' AND subscriptionId = '{{ subscription_id }}'
+
+**Test SQL (stackql_queries/monitor_resource_group.iql):**
+
+.. code-block:: sql
+
+    /*+ preflight */
+    SELECT COUNT(*) as count FROM azure.storage.accounts
+    WHERE SPLIT_PART(SPLIT_PART(JSON_EXTRACT(properties, '$.primaryEndpoints.blob'), '//', 2), '.', 1) = '{{ storage_account_name }}'
+    AND subscriptionId = '{{ subscription_id }}'
+    AND resourceGroupName = '{{ resource_group_name }}'
+
+    /*+ postdeploy, retries=5, retry_delay=5 */
+    SELECT 
+    COUNT(*) as count
+    FROM azure.storage.accounts
+    WHERE SPLIT_PART(SPLIT_PART(JSON_EXTRACT(properties, '$.primaryEndpoints.blob'), '//', 2), '.', 1) = '{{ storage_account_name }}'
+    AND subscriptionId = '{{ subscription_id }}'
+    AND resourceGroupName = '{{ resource_group_name }}'
+    AND kind = '{{ storage_kind }}'
+    AND JSON_EXTRACT(sku, '$.name') = 'Standard_LRS'
+    AND JSON_EXTRACT(sku, '$.tier') = 'Standard'
+
+    /*+ exports, retries=5, retry_delay=5 */
+    select json_extract(keys, '$[0].value') as storage_account_key 
+    from azure.storage.accounts_keys 
+    WHERE resourceGroupName = '{{ resource_group_name }}' 
+    AND subscriptionId = '{{ subscription_id }}' 
+    AND accountName = '{{ storage_account_name }}'
+
+
+Resource SQL Anchors
+--------------------
+
+Resource SQL files use special anchor comments as directives for the ``stackql-deploy`` tool to indicate the intended operations:
+
+- **/*+ create */**
+  This anchor precedes SQL ``INSERT`` statements for creating new resources.
+
+  .. code-block:: sql
+
+      /*+ create */
+      INSERT INTO azure.resources.resource_groups(
+        resourceGroupName,
+        subscriptionId,
+        data__location
+      )
+      SELECT
+        '{{ resource_group_name }}',
+        '{{ subscription_id }}',
+        '{{ location }}'
+
+- **/*+ createorupdate */**
+  Specifies an operation to either create a new resource or update an existing one.
+
+- **/*+ update */**
+  Marks SQL ``UPDATE`` statements intended to modify existing resources.
+
+- **/*+ delete */**
+  Tags SQL ``DELETE`` statements for removing resources from the environment.
+
+Query SQL Anchors
+-----------------
+
+Query SQL files contain SQL statements for testing and validation with the following anchors:
+
+- **/*+ preflight */**
+  Used to perform initial checks before a deployment.
+
+  .. code-block:: sql
+
+      /*+ preflight */
+      SELECT COUNT(*) as count FROM azure.resources.resource_groups
+      WHERE subscriptionId = '{{ subscription_id }}'
+      AND resourceGroupName = '{{ resource_group_name }}'
+
+- **/*+ postdeploy, retries=5, retry_delay=5 */**
+  Post-deployment checks to confirm the success of the operation, with optional ``retries`` and ``retry_delay`` parameters.
+
+  .. code-block:: sql
+
+      /*+ postdeploy, retries=5, retry_delay=5 */
+      SELECT COUNT(*) as count FROM azure.resources.resource_groups
+      WHERE subscriptionId = '{{ subscription_id }}'
+      AND resourceGroupName = '{{ resource_group_name }}'
+      AND location = '{{ location }}'
+      AND JSON_EXTRACT(properties, '$.provisioningState') = 'Succeeded'
+
+- **/*+ exports, retries=5, retry_delay=5 */**
+  Extracts and exports information after a deployment. Similar to post-deploy checks but specifically for exporting data.
+
+
+.. note::
+   The following parameters are used to control the behavior of retry mechanisms in SQL operations:
+
+   - **``retries``** (optional, integer): Defines the number of times a query should be retried upon failure.
+   - **``retry_delay``** (optional, integer): Sets the delay in seconds between each retry attempt.
+
+
+**stackql-deploy** simplifies cloud resource management by treating infrastructure as flexible, dynamically assessed code.
+
+.. _stackql: https://github.com/stackql/stackql
```

### Comparing `stackql_deploy-1.2.0/setup.py` & `stackql_deploy-1.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,29 @@
     readme = f.read()
 
 # with open('LICENSE', encoding='utf-8') as f:
 #     license_text = f.read()
 
 setup(
     name='stackql-deploy',
-    version='1.2.0',
+    version='1.5.0',
     description='Model driven resource provisioning and deployment framework using StackQL.',
     long_description=readme,
     long_description_content_type='text/x-rst',
     author='Jeffrey Aven',
     author_email='javen@stackql.io',
     url='https://github.com/stackql/stackql-deploy',
     license='MIT',
     packages=find_packages(),
     package_data={
         'stackql_deploy': [
             'templates/*.template',
             'templates/stackql_docs/*.template',
             'templates/stackql_resources/*.template',
-            'templates/stackql_tests/*.template',
+            'templates/stackql_queries/*.template',
         ],
     },    
     include_package_data=True,
     install_requires=[
         'click', 
         'python-dotenv',
         'jinja2',
```

### Comparing `stackql_deploy-1.2.0/stackql_deploy/cli.py` & `stackql_deploy-1.5.0/stackql_deploy/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,28 +176,28 @@
 #
 
 def create_project_structure(stack_name):
     base_path = os.path.join(os.getcwd(), stack_name)
     if os.path.exists(base_path):
         raise click.ClickException(f"Directory '{stack_name}' already exists.")
     
-    directories = ['stackql_docs', 'stackql_resources', 'stackql_tests']
+    directories = ['stackql_docs', 'stackql_resources', 'stackql_queries']
     for directory in directories:
         os.makedirs(os.path.join(base_path, directory), exist_ok=True)
     
     template_base_path = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'templates')
     env = Environment(loader=FileSystemLoader(template_base_path))
 
     logger.debug(f"template base path: {template_base_path}")
 
     template_files = {
         'stackql_manifest.yml.template': os.path.join(base_path, 'stackql_manifest.yml'),
         'stackql_docs/stackql_example_rg.md.template': os.path.join(base_path,'stackql_docs', 'stackql_example_rg.md'),
         'stackql_resources/stackql_example_rg.iql.template': os.path.join(base_path,'stackql_resources', 'stackql_example_rg.iql'),
-        'stackql_tests/stackql_example_rg.iql.template': os.path.join(base_path,'stackql_tests', 'stackql_example_rg.iql')
+        'stackql_queries/stackql_example_rg.iql.template': os.path.join(base_path,'stackql_queries', 'stackql_example_rg.iql')
     }
     
     for template_name, output_name in template_files.items():
         logger.debug(f"template name: {template_name}")
         logger.debug(f"template output name: {output_name}")
         template = env.get_template(template_name)
         rendered_content = template.render(stack_name=stack_name)
```

### Comparing `stackql_deploy-1.2.0/stackql_deploy/cmd/teardown.py` & `stackql_deploy-1.5.0/stackql_deploy/cmd/teardown.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
             # get full context
             full_context = get_full_context(self.env, self.global_context, resource, self.logger)    
 
             # get resource queries
             resource_queries, resource_query_options = get_queries(self.env, self.stack_dir, 'stackql_resources', resource, full_context, True, self.logger)
 
             # get resource queries
-            test_queries, test_query_options = get_queries(self.env, self.stack_dir, 'stackql_tests', resource, full_context, False, self.logger)
+            test_queries, test_query_options = get_queries(self.env, self.stack_dir, 'stackql_queries', resource, full_context, False, self.logger)
 
             delete_query = None
 
             if 'delete' in resource_queries:
                 delete_query = resource_queries['delete']
 
             preflight_query = None
```

### Comparing `stackql_deploy-1.2.0/stackql_deploy/lib/config.py` & `stackql_deploy-1.5.0/stackql_deploy/lib/config.py`

 * *Files identical despite different names*

### Comparing `stackql_deploy-1.2.0/stackql_deploy/lib/templating.py` & `stackql_deploy-1.5.0/stackql_deploy/lib/templating.py`

 * *Files identical despite different names*

### Comparing `stackql_deploy-1.2.0/stackql_deploy/lib/utils.py` & `stackql_deploy-1.5.0/stackql_deploy/lib/utils.py`

 * *Files identical despite different names*

### Comparing `stackql_deploy-1.2.0/stackql_deploy/templates/stackql_manifest.yml.template` & `stackql_deploy-1.5.0/stackql_deploy/templates/stackql_manifest.yml.template`

 * *Files identical despite different names*

### Comparing `stackql_deploy-1.2.0/stackql_deploy/templates/stackql_resources/stackql_example_rg.iql.template` & `stackql_deploy-1.5.0/stackql_deploy/templates/stackql_resources/stackql_example_rg.iql.template`

 * *Files identical despite different names*

### Comparing `stackql_deploy-1.2.0/stackql_deploy/templates/stackql_tests/stackql_example_rg.iql.template` & `stackql_deploy-1.5.0/stackql_deploy/templates/stackql_queries/stackql_example_rg.iql.template`

 * *Files identical despite different names*

### Comparing `stackql_deploy-1.2.0/stackql_deploy.egg-info/SOURCES.txt` & `stackql_deploy-1.5.0/stackql_deploy.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -16,9 +16,9 @@
 stackql_deploy/lib/__init__.py
 stackql_deploy/lib/bootstrap.py
 stackql_deploy/lib/config.py
 stackql_deploy/lib/templating.py
 stackql_deploy/lib/utils.py
 stackql_deploy/templates/stackql_manifest.yml.template
 stackql_deploy/templates/stackql_docs/stackql_example_rg.md.template
-stackql_deploy/templates/stackql_resources/stackql_example_rg.iql.template
-stackql_deploy/templates/stackql_tests/stackql_example_rg.iql.template
+stackql_deploy/templates/stackql_queries/stackql_example_rg.iql.template
+stackql_deploy/templates/stackql_resources/stackql_example_rg.iql.template
```

