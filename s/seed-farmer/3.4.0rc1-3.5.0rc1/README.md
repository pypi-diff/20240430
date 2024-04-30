# Comparing `tmp/seed_farmer-3.4.0rc1-py3-none-any.whl.zip` & `tmp/seed_farmer-3.5.0rc1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 101204 bytes, number of entries: 61
--rw-r--r--  2.0 unx     5729 b- defN 24-Apr-01 21:08 seedfarmer/__init__.py
+Zip file size: 102084 bytes, number of entries: 61
+-rw-r--r--  2.0 unx     5982 b- defN 24-Apr-30 20:13 seedfarmer/__init__.py
 -rw-r--r--  2.0 unx     8397 b- defN 24-Apr-01 21:08 seedfarmer/__main__.py
 -rw-r--r--  2.0 unx      829 b- defN 23-Oct-30 21:20 seedfarmer/__metadata__.py
 -rw-r--r--  2.0 unx     5330 b- defN 24-Apr-01 21:08 seedfarmer/checksum.py
 -rw-r--r--  2.0 unx      865 b- defN 24-Apr-01 21:08 seedfarmer/messages.py
 -rw-r--r--  2.0 unx     7740 b- defN 24-Apr-01 21:08 seedfarmer/output_utils.py
--rw-r--r--  2.0 unx     6330 b- defN 24-Apr-01 21:08 seedfarmer/utils.py
+-rw-r--r--  2.0 unx     7531 b- defN 24-Apr-30 20:13 seedfarmer/utils.py
 -rw-r--r--  2.0 unx     1133 b- defN 23-Oct-30 21:20 seedfarmer/cli_groups/__init__.py
 -rw-r--r--  2.0 unx     6918 b- defN 24-Apr-01 21:08 seedfarmer/cli_groups/_bootstrap_group.py
 -rw-r--r--  2.0 unx     2752 b- defN 23-Oct-30 21:20 seedfarmer/cli_groups/_init_group.py
 -rw-r--r--  2.0 unx    22403 b- defN 24-Apr-01 21:08 seedfarmer/cli_groups/_list_group.py
 -rw-r--r--  2.0 unx     4034 b- defN 24-Apr-01 21:08 seedfarmer/cli_groups/_manage_metadata_group.py
 -rw-r--r--  2.0 unx     1452 b- defN 24-Apr-01 21:08 seedfarmer/cli_groups/_project_group.py
 -rw-r--r--  2.0 unx     4328 b- defN 24-Apr-01 21:08 seedfarmer/cli_groups/_remove_group.py
@@ -29,35 +29,35 @@
 -rw-r--r--  2.0 unx     1760 b- defN 24-Apr-01 21:08 seedfarmer/mgmt/build_info.py
 -rw-r--r--  2.0 unx    26894 b- defN 24-Apr-01 21:08 seedfarmer/mgmt/deploy_utils.py
 -rw-r--r--  2.0 unx     3969 b- defN 24-Apr-01 21:08 seedfarmer/mgmt/git_support.py
 -rw-r--r--  2.0 unx     7365 b- defN 24-Apr-08 17:16 seedfarmer/mgmt/metadata_support.py
 -rw-r--r--  2.0 unx    27311 b- defN 24-Apr-01 21:08 seedfarmer/mgmt/module_info.py
 -rw-r--r--  2.0 unx     3892 b- defN 23-Oct-30 21:20 seedfarmer/mgmt/module_init.py
 -rw-r--r--  2.0 unx     1085 b- defN 23-Oct-30 21:20 seedfarmer/models/__init__.py
--rw-r--r--  2.0 unx     1534 b- defN 24-Apr-01 21:08 seedfarmer/models/_base.py
--rw-r--r--  2.0 unx     2563 b- defN 23-Oct-30 21:20 seedfarmer/models/_deploy_spec.py
--rw-r--r--  2.0 unx     1101 b- defN 24-Apr-01 21:08 seedfarmer/models/_project_spec.py
+-rw-r--r--  2.0 unx     1967 b- defN 24-Apr-30 20:13 seedfarmer/models/_base.py
+-rw-r--r--  2.0 unx     2643 b- defN 24-Apr-30 20:13 seedfarmer/models/_deploy_spec.py
+-rw-r--r--  2.0 unx     1560 b- defN 24-Apr-30 20:13 seedfarmer/models/_project_spec.py
 -rw-r--r--  2.0 unx     2220 b- defN 24-Apr-01 21:08 seedfarmer/models/deploy_responses.py
 -rw-r--r--  2.0 unx     1154 b- defN 23-Oct-30 21:20 seedfarmer/models/manifests/__init__.py
--rw-r--r--  2.0 unx    17967 b- defN 24-Apr-19 16:59 seedfarmer/models/manifests/_deployment_manifest.py
--rw-r--r--  2.0 unx     4101 b- defN 24-Apr-19 16:59 seedfarmer/models/manifests/_module_manifest.py
+-rw-r--r--  2.0 unx    18074 b- defN 24-Apr-30 20:13 seedfarmer/models/manifests/_deployment_manifest.py
+-rw-r--r--  2.0 unx     4213 b- defN 24-Apr-30 20:13 seedfarmer/models/manifests/_module_manifest.py
 -rw-r--r--  2.0 unx      766 b- defN 24-Apr-19 16:59 seedfarmer/models/transfer/__init__.py
 -rw-r--r--  2.0 unx     2756 b- defN 24-Apr-19 16:59 seedfarmer/models/transfer/_module_deploy_object.py
 -rw-r--r--  2.0 unx     5718 b- defN 23-Oct-30 21:20 seedfarmer/resources/deployment_role.template
 -rw-r--r--  2.0 unx     2619 b- defN 23-Oct-30 21:20 seedfarmer/resources/projectpolicy.yaml
 -rw-r--r--  2.0 unx     1426 b- defN 23-Oct-30 21:20 seedfarmer/resources/toolchain_role.template
 -rw-r--r--  2.0 unx     1076 b- defN 23-Oct-30 21:20 seedfarmer/services/__init__.py
 -rw-r--r--  2.0 unx     1255 b- defN 23-Oct-30 21:20 seedfarmer/services/_codebuild.py
 -rw-r--r--  2.0 unx     5582 b- defN 23-Oct-30 21:20 seedfarmer/services/_iam.py
 -rw-r--r--  2.0 unx     1826 b- defN 23-Oct-30 21:20 seedfarmer/services/_secrets_manager.py
 -rw-r--r--  2.0 unx     4912 b- defN 24-Apr-01 21:08 seedfarmer/services/_service_utils.py
 -rw-r--r--  2.0 unx     6263 b- defN 23-Oct-30 21:20 seedfarmer/services/_ssm.py
 -rw-r--r--  2.0 unx    10737 b- defN 24-Apr-01 21:08 seedfarmer/services/session_manager.py
--rw-r--r--  2.0 unx    10174 b- defN 24-Apr-19 17:47 seed_farmer-3.4.0rc1.dist-info/LICENSE
--rw-r--r--  2.0 unx     3158 b- defN 24-Apr-19 17:47 seed_farmer-3.4.0rc1.dist-info/METADATA
--rw-r--r--  2.0 unx       67 b- defN 24-Apr-19 17:47 seed_farmer-3.4.0rc1.dist-info/NOTICE
--rw-r--r--  2.0 unx        9 b- defN 24-Apr-19 17:47 seed_farmer-3.4.0rc1.dist-info/VERSION
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-19 17:47 seed_farmer-3.4.0rc1.dist-info/WHEEL
--rw-r--r--  2.0 unx       57 b- defN 24-Apr-19 17:47 seed_farmer-3.4.0rc1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 24-Apr-19 17:47 seed_farmer-3.4.0rc1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     5586 b- defN 24-Apr-19 17:47 seed_farmer-3.4.0rc1.dist-info/RECORD
-61 files, 358938 bytes uncompressed, 92206 bytes compressed:  74.3%
+-rw-r--r--  2.0 unx    10174 b- defN 24-Apr-30 20:16 seed_farmer-3.5.0rc1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3155 b- defN 24-Apr-30 20:16 seed_farmer-3.5.0rc1.dist-info/METADATA
+-rw-r--r--  2.0 unx       67 b- defN 24-Apr-30 20:16 seed_farmer-3.5.0rc1.dist-info/NOTICE
+-rw-r--r--  2.0 unx        9 b- defN 24-Apr-30 20:16 seed_farmer-3.5.0rc1.dist-info/VERSION
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-30 20:16 seed_farmer-3.5.0rc1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       57 b- defN 24-Apr-30 20:16 seed_farmer-3.5.0rc1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 24-Apr-30 20:16 seed_farmer-3.5.0rc1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     5586 b- defN 24-Apr-30 20:16 seed_farmer-3.5.0rc1.dist-info/RECORD
+61 files, 361580 bytes uncompressed, 93086 bytes compressed:  74.3%
```

## zipnote {}

```diff
@@ -153,32 +153,32 @@
 
 Filename: seedfarmer/services/_ssm.py
 Comment: 
 
 Filename: seedfarmer/services/session_manager.py
 Comment: 
 
-Filename: seed_farmer-3.4.0rc1.dist-info/LICENSE
+Filename: seed_farmer-3.5.0rc1.dist-info/LICENSE
 Comment: 
 
-Filename: seed_farmer-3.4.0rc1.dist-info/METADATA
+Filename: seed_farmer-3.5.0rc1.dist-info/METADATA
 Comment: 
 
-Filename: seed_farmer-3.4.0rc1.dist-info/NOTICE
+Filename: seed_farmer-3.5.0rc1.dist-info/NOTICE
 Comment: 
 
-Filename: seed_farmer-3.4.0rc1.dist-info/VERSION
+Filename: seed_farmer-3.5.0rc1.dist-info/VERSION
 Comment: 
 
-Filename: seed_farmer-3.4.0rc1.dist-info/WHEEL
+Filename: seed_farmer-3.5.0rc1.dist-info/WHEEL
 Comment: 
 
-Filename: seed_farmer-3.4.0rc1.dist-info/entry_points.txt
+Filename: seed_farmer-3.5.0rc1.dist-info/entry_points.txt
 Comment: 
 
-Filename: seed_farmer-3.4.0rc1.dist-info/top_level.txt
+Filename: seed_farmer-3.5.0rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: seed_farmer-3.4.0rc1.dist-info/RECORD
+Filename: seed_farmer-3.5.0rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## seedfarmer/__init__.py

```diff
@@ -133,9 +133,15 @@
 
     @property
     def PROJECT_POLICY_PATH(self) -> str:
         if self._project_spec is None:
             self._load_config_data()
         return str(cast(ProjectSpec, self._project_spec).project_policy_path)
 
+    @property
+    def MANIFEST_VALIDATION_FAIL_ON_UNKNOWN_FIELDS(self) -> bool:
+        if self._project_spec is None:
+            self._load_config_data()
+        return cast(ProjectSpec, self._project_spec).manifest_validation_fail_on_unknown_fields
+
 
 config = Config()
```

## seedfarmer/utils.py

```diff
@@ -11,21 +11,23 @@
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
 import hashlib
 import logging
 import os
+import re
 from typing import Any, Dict, List, Optional
 
 import humps
 import yaml
 from boto3 import Session
 from dotenv import dotenv_values, load_dotenv
 
+import seedfarmer.errors
 from seedfarmer.services._service_utils import get_region, get_sts_identity_info
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
 NoDatesSafeLoader = yaml.SafeLoader
 
 
@@ -188,7 +190,38 @@
 def remove_nulls(payload: Dict[str, Any]) -> Dict[str, Any]:
     if isinstance(payload, dict):
         return {k: remove_nulls(v) for k, v in payload.items() if v is not None}
     elif isinstance(payload, list):
         return [remove_nulls(v) for v in payload]
     else:
         return payload
+
+
+def batch_replace_env(payload: Dict[str, Any]) -> Dict[str, Any]:
+    pattern = r"\${(.*?)}"
+
+    def replace_str(value: str) -> str:
+        matches = re.findall(pattern, value)
+        for match in matches:
+            try:
+                return value.replace("${" + match + "}", os.environ[match.strip()])
+            except KeyError:
+                raise seedfarmer.errors.InvalidManifestError(
+                    f"The environment variable ({match.strip()}) is not available"
+                )
+        return value
+
+    def recurse_elements(working_element: Any) -> Any:
+        if isinstance(working_element, dict):
+            for key, value in working_element.items():
+                if isinstance(value, str):
+                    working_element[key] = replace_str(value)
+                elif isinstance(value, list):
+                    for item in value:
+                        recurse_elements(item)
+                elif isinstance(value, dict) and key not in ["deploy_spec"]:
+                    recurse_elements(value)
+            return working_element
+        return working_element
+
+    payload = recurse_elements(payload)
+    return payload
```

## seedfarmer/models/_base.py

```diff
@@ -11,25 +11,36 @@
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
 from typing import Optional, cast
 
 import humps
-from pydantic import BaseModel, ConfigDict
+from pydantic import BaseModel, ConfigDict, model_validator
+
+from seedfarmer.errors.seedfarmer_errors import InvalidManifestError
 
 
 def to_camel(string: str) -> str:
     return cast(str, humps.camelize(string))  # type: ignore
 
 
 class CamelModel(BaseModel):
     # TODO[pydantic]: The following keys were removed: `underscore_attrs_are_private`.
     # Check https://docs.pydantic.dev/dev-v2/migration/#changes-to-config for more information.
-    model_config = ConfigDict(alias_generator=to_camel, populate_by_name=True)
+    model_config = ConfigDict(alias_generator=to_camel, populate_by_name=True, extra="allow")
+
+    @model_validator(mode="after")
+    def check_for_extra_fields(self) -> "CamelModel":
+        from seedfarmer import config
+
+        if config.MANIFEST_VALIDATION_FAIL_ON_UNKNOWN_FIELDS and self.model_extra:
+            raise InvalidManifestError(f"The following keys are not allowed: {self.model_extra}")
+
+        return self
 
 
 class ModuleRef(CamelModel):
     name: str
     group: str
     key: Optional[str] = None
```

## seedfarmer/models/_deploy_spec.py

```diff
@@ -38,28 +38,28 @@
 class BuildPhases(CamelModel):
     """
     BuildPhases
     This object has the individual commands for each of the define build phases:
     install, pre_build,  build, post_build
     """
 
-    install: BuildPhase = BuildPhase()
-    pre_build: BuildPhase = BuildPhase()
-    build: BuildPhase = BuildPhase()
-    post_build: BuildPhase = BuildPhase()
+    install: BuildPhase = BuildPhase.model_construct()
+    pre_build: BuildPhase = BuildPhase.model_construct()
+    build: BuildPhase = BuildPhase.model_construct()
+    post_build: BuildPhase = BuildPhase.model_construct()
 
 
 class ExecutionType(CamelModel):
     """
     ExecutionType
     This an object that contains the Build Phases object for the destroy or deploy
     object of the DeploySpec
     """
 
-    phases: BuildPhases = BuildPhases()
+    phases: BuildPhases = BuildPhases.model_construct()
 
 
 class DeploySpec(CamelModel):
     """
     DeploySpec
     This represents the commands passed to CodeSeeder that will be executed
     on behalf of the module to be built.
```

## seedfarmer/models/_project_spec.py

```diff
@@ -10,21 +10,32 @@
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
 from typing import Optional, Union
 
+from pydantic import model_validator
+
+from seedfarmer.errors.seedfarmer_errors import InvalidManifestError
 from seedfarmer.models._base import CamelModel
 
 
 class ProjectSpec(CamelModel):
     """
     ProjectSpec
     This represents the project configuration specification. This class is
     typically populated from the project's top-level seedfarmer.yaml file.
     """
 
     project: str
     description: Optional[str] = None
     project_policy_path: Optional[str] = None
     seedfarmer_version: Optional[Union[int, str]] = None
+    manifest_validation_fail_on_unknown_fields: bool = False
+
+    @model_validator(mode="after")
+    def check_for_extra_fields(self) -> "ProjectSpec":
+        if self.manifest_validation_fail_on_unknown_fields and self.model_extra:
+            raise InvalidManifestError(f"The following keys are not allowed: {self.model_extra}")
+
+        return self
```

## seedfarmer/models/manifests/_deployment_manifest.py

```diff
@@ -173,14 +173,17 @@
     _account_alias_index: Dict[str, TargetAccountMapping] = PrivateAttr(default_factory=dict)
     _account_id_index: Dict[str, TargetAccountMapping] = PrivateAttr(default_factory=dict)
     _accounts_regions: Optional[List[Dict[str, str]]] = PrivateAttr(default=None)
     _module_index: Dict[Tuple[str, str], ModuleManifest] = PrivateAttr(default_factory=dict)
     _partition: Optional[str] = PrivateAttr(default="aws")
 
     def __init__(self, **kwargs: Any) -> None:
+        from seedfarmer.utils import batch_replace_env
+
+        kwargs = batch_replace_env(payload=kwargs)
         super().__init__(**kwargs)
 
         if self.name is None and self.name_generator is None:
             raise seedfarmer.errors.InvalidManifestError("One of 'name' or 'name_generator' is required")
 
         if self.name is not None and self.name_generator is not None:
             raise seedfarmer.errors.InvalidManifestError("Only one of 'name' or 'name_generator' can be specified")
```

## seedfarmer/models/manifests/_module_manifest.py

```diff
@@ -97,16 +97,20 @@
     data_files: Optional[List[DataFile]] = None
     commit_hash: SkipJsonSchema[Optional[str]] = None
     npm_mirror: Optional[str] = None
     pypi_mirror: Optional[str] = None
     _target_account_id: Optional[str] = PrivateAttr(default=None)
     _local_path: Optional[str] = PrivateAttr(default=None)
 
-    def __init__(self, **data: Any) -> None:
-        super().__init__(**data)
+    def __init__(self, **kwargs: Any) -> None:
+
+        from seedfarmer.utils import batch_replace_env
+
+        kwargs = batch_replace_env(payload=kwargs)
+        super().__init__(**kwargs)
         self._local_path = self.path
 
     def set_target_account_id(self, account_id: str) -> None:
         self._target_account_id = account_id
 
     def get_target_account_id(self) -> Optional[str]:
         return self._target_account_id
```

## Comparing `seed_farmer-3.4.0rc1.dist-info/LICENSE` & `seed_farmer-3.5.0rc1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `seed_farmer-3.4.0rc1.dist-info/METADATA` & `seed_farmer-3.5.0rc1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seed-farmer
-Version: 3.4.0rc1
+Version: 3.5.0rc1
 Summary: The AWS Professional Services CLI tool SeedFarmer for GitOps support with AWS_CodeSeeder
 Home-page: https://github.com/awslabs/seed-farmer
 Author: AWS Professional Services
 Author-email: aws-proserve-opensource@amazon.com
 License: Apache License 2.0
 Project-URL: Org Site, https://aws.amazon.com/professional-services/
 Keywords: aws,cdk
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.8,<3.12
 Description-Content-Type: text/markdown
-Requires-Dist: aws-codeseeder (~=0.12.0rc1)
+Requires-Dist: aws-codeseeder (~=0.12.0)
 Requires-Dist: cookiecutter (~=2.1.0)
 Requires-Dist: pyhumps (~=3.5.0)
 Requires-Dist: pydantic (~=2.5.3)
 Requires-Dist: executor (~=23.2)
 Requires-Dist: typing-extensions (>=4.6.3)
 Requires-Dist: rich (~=12.4.0)
 Requires-Dist: requests (<2.32,>=2.28)
```

## Comparing `seed_farmer-3.4.0rc1.dist-info/RECORD` & `seed_farmer-3.5.0rc1.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-seedfarmer/__init__.py,sha256=abDAABPBGxrYDo-J5EH4zbKKomqlbqFeHhUPwUhQCvE,5729
+seedfarmer/__init__.py,sha256=4DBVG1odt2Tk6Xz9oZJqiV2tzipyJEDyn_nx0b2-FO4,5982
 seedfarmer/__main__.py,sha256=O8a2kjTMT3kOF4yMep1c7zQPJCFBNYtTWlXBUDFDh6k,8397
 seedfarmer/__metadata__.py,sha256=EvOaiIYE0aSQGrYmmphPD624zAhgFRJqfZjmXMwnfrY,829
 seedfarmer/checksum.py,sha256=37xO9wogJhRSMOCilqr32NwHoAc0MesNhT5lTt_3q9M,5330
 seedfarmer/messages.py,sha256=07ik62SYrKFHhWahVJo5H1mRwygYaoBA7YBRMfHnpXI,865
 seedfarmer/output_utils.py,sha256=l0cbh7ZjDuwpEdyvFLQMAR-0EQPnPOl1l4RigcxNeHk,7740
-seedfarmer/utils.py,sha256=qXEgOhpMJdm82jUqYdfFeHK8yW3BPfeTUf9vzl_AQHs,6330
+seedfarmer/utils.py,sha256=BV796DJv-n8YNYfq_DVusXp45LTbIOkzCImXOwSnsGU,7531
 seedfarmer/cli_groups/__init__.py,sha256=DcoiPjEiE_j8TWJg5xd3QHmrjGpNN578zveAINBAcH8,1133
 seedfarmer/cli_groups/_bootstrap_group.py,sha256=v6-yjjLPnGgYUwk5fBfk49fJ1_FW6lyqP-Fw1olTUpw,6918
 seedfarmer/cli_groups/_init_group.py,sha256=cuwpXTTj2tT8fwrwhBwboiDD6GQVPmXuocTbGNMF80Y,2752
 seedfarmer/cli_groups/_list_group.py,sha256=At5vz8tVGO8uF8rouu3jjf_DK-G1eiEl7SXVhZkChAs,22403
 seedfarmer/cli_groups/_manage_metadata_group.py,sha256=BwL-g1VPRDNG2mb4LmRxa7fmLRgo1UOXPUyb9G5l1Ew,4034
 seedfarmer/cli_groups/_project_group.py,sha256=L4ySaHwxVFN9o2jmLGbeGxFGuqzPEytWE_7xb0UX1Y8,1452
 seedfarmer/cli_groups/_remove_group.py,sha256=0v6RAhXIjhTaes-uCuciE_R0SfsuyCKLjR2x9qlaX1k,4328
@@ -28,34 +28,34 @@
 seedfarmer/mgmt/build_info.py,sha256=hHf9ywy7s3-p2hiqw40BlmG1gToGh0ClvZRqQlvZ1Fo,1760
 seedfarmer/mgmt/deploy_utils.py,sha256=_TVsKjhd_xzrqsTSFCJFMldceyo-04a8RGBoKiJ_6ng,26894
 seedfarmer/mgmt/git_support.py,sha256=WRQKruyKG6iyBoK40y73vI1FC5Ye_Pu6yz0-EYIh8-E,3969
 seedfarmer/mgmt/metadata_support.py,sha256=JLVyriTLIKiqfwjSpo-dNyXfmwS_vAIvF_psU4Mf054,7365
 seedfarmer/mgmt/module_info.py,sha256=Kd9Y_X-k4_ePH7ZCHeBWE8miMN5qDn3tWwGQn_6Aa0A,27311
 seedfarmer/mgmt/module_init.py,sha256=vw6rAXmcj_JnQQoyiro1R6VC3YDtlKLJfQ3y0XisQNo,3892
 seedfarmer/models/__init__.py,sha256=_ZJ4lA83cCB4ZgxqhrfK9gj8AbyHHzd2O_OoDqMCbrs,1085
-seedfarmer/models/_base.py,sha256=VTErybBRA82czXceUP9xA9kCUqEgAinovRtTsXE5Ztg,1534
-seedfarmer/models/_deploy_spec.py,sha256=fJfDKexpyKje1bMKb8l_qbaEM3ycXQdcV77YsR78jN0,2563
-seedfarmer/models/_project_spec.py,sha256=rRwWd0p-376VRmAsY2drS244d5oB3yYupLcs2HahOzc,1101
+seedfarmer/models/_base.py,sha256=BLFvDPjGsT5qfBaWL_QaH4CIKVKfX-9kwBFn5U7CV8w,1967
+seedfarmer/models/_deploy_spec.py,sha256=JQ_3QitqkQrmgwyecxK4rJDI4s6ppE6t0im4pYGRD5w,2643
+seedfarmer/models/_project_spec.py,sha256=YkhdSAIqqc5i3VAarClljx4J7-SPapmpQLycjXb0ZcI,1560
 seedfarmer/models/deploy_responses.py,sha256=U4cHkbZP0Arw_9TS6i1jjpLA0NiGjfzkvP_dSjpMTiM,2220
 seedfarmer/models/manifests/__init__.py,sha256=vcDfpmYs7VeYT-vbMBiC7UvKWFKQJT-w4qdZKAewuvg,1154
-seedfarmer/models/manifests/_deployment_manifest.py,sha256=MHGqm3umnuRfQpZgFTGI6UvqZZLE29Cl3a4kzDwFzG8,17967
-seedfarmer/models/manifests/_module_manifest.py,sha256=nPiLApLp-FHWCWFoXoBW3Qe6O4BUkwLI4uB-4jaS3KA,4101
+seedfarmer/models/manifests/_deployment_manifest.py,sha256=0zVtRYtmA2mHaEQqeOKbki1ItoEuzVvqCeaa-Ny-ulU,18074
+seedfarmer/models/manifests/_module_manifest.py,sha256=pR2u98lTA1egiLPLM91JlpqHhrWwXOfQ5PEe4j3nrQA,4213
 seedfarmer/models/transfer/__init__.py,sha256=tstFBjkaA8qJW3fRz86YewrSakEI5Vn6z2goTOgtMSY,766
 seedfarmer/models/transfer/_module_deploy_object.py,sha256=oUdopmoTVlPRRqgI26C944XCPpjuwSnC6IQOvYWlrEc,2756
 seedfarmer/resources/deployment_role.template,sha256=isqPpJYTVEJtkutQg3a7Y0Mm4lgj7HlFcV_mV8HPrrc,5718
 seedfarmer/resources/projectpolicy.yaml,sha256=-OGN5C_U9zW974XC1a-JPXEsu-tB3NVwJC6DSLNlvqQ,2619
 seedfarmer/resources/toolchain_role.template,sha256=VGx7W2EV2aNpjq2PVqWPX5fbJDxqEH_TwinjWGX922k,1426
 seedfarmer/services/__init__.py,sha256=wlJZVbu4wE4HCnUqDEd_3kq9vjnr3bc9oRTZNbw8OgM,1076
 seedfarmer/services/_codebuild.py,sha256=VY1NXRgPRR1hxAvQMmSHvMqjbZid9ICzHe6xpRYT5kM,1255
 seedfarmer/services/_iam.py,sha256=XfadcMMpHjZYTtZwhcMB1QWQzyDfnzZKdSPnUuNt0hA,5582
 seedfarmer/services/_secrets_manager.py,sha256=0rOvZmiHIiEYiTRJ1HJNn_4emt3NEWZ2_OgqDdxf9VU,1826
 seedfarmer/services/_service_utils.py,sha256=C2IqAcVqx6izxZyck9edfJsC0YXXvIFJ5qLkx6mG2lQ,4912
 seedfarmer/services/_ssm.py,sha256=WNVj5rKxv7USOACfJuLmB-Qmn7KEtmlBNV5BuPxGaTg,6263
 seedfarmer/services/session_manager.py,sha256=Ca9i1FiMtJGhFN7LJ1IZ_76MFC4ohZIPSsShVtxRgkc,10737
-seed_farmer-3.4.0rc1.dist-info/LICENSE,sha256=DVQuDIgE45qn836wDaWnYhSdxoLXgpRRKH4RuTjpRZQ,10174
-seed_farmer-3.4.0rc1.dist-info/METADATA,sha256=JSlCgW2pe7saAkt0MZOEGbfCTYS17ymfPTHa4pOfzOQ,3158
-seed_farmer-3.4.0rc1.dist-info/NOTICE,sha256=1CkO1kwu3Q_OHYTj-d-yiBJA_lNN73a4zSntavaD4oc,67
-seed_farmer-3.4.0rc1.dist-info/VERSION,sha256=K_kOFjPj5pQI8vgEKksw-u-R4ci5-2vk8ZY1jFqx3R0,9
-seed_farmer-3.4.0rc1.dist-info/WHEEL,sha256=00yskusixUoUt5ob_CiUp6LsnN5lqzTJpoqOFg_FVIc,92
-seed_farmer-3.4.0rc1.dist-info/entry_points.txt,sha256=lxdm6KJKOs-cDkQ5snOEfpWM5xG9lplmKTC-15LyheI,57
-seed_farmer-3.4.0rc1.dist-info/top_level.txt,sha256=znpV4OtUGmKGq4kQZ2cE_o9NxJgWxaM6dhPr1trkK0o,11
-seed_farmer-3.4.0rc1.dist-info/RECORD,,
+seed_farmer-3.5.0rc1.dist-info/LICENSE,sha256=DVQuDIgE45qn836wDaWnYhSdxoLXgpRRKH4RuTjpRZQ,10174
+seed_farmer-3.5.0rc1.dist-info/METADATA,sha256=ZFOhBb2kngIgVwCBq7YS-okPYJNGEoBd-bxG3_05LF0,3155
+seed_farmer-3.5.0rc1.dist-info/NOTICE,sha256=1CkO1kwu3Q_OHYTj-d-yiBJA_lNN73a4zSntavaD4oc,67
+seed_farmer-3.5.0rc1.dist-info/VERSION,sha256=pno45hi9Z8jShdp9qQWTOaj5_WRTEBJ4nToJ2534jmk,9
+seed_farmer-3.5.0rc1.dist-info/WHEEL,sha256=00yskusixUoUt5ob_CiUp6LsnN5lqzTJpoqOFg_FVIc,92
+seed_farmer-3.5.0rc1.dist-info/entry_points.txt,sha256=lxdm6KJKOs-cDkQ5snOEfpWM5xG9lplmKTC-15LyheI,57
+seed_farmer-3.5.0rc1.dist-info/top_level.txt,sha256=znpV4OtUGmKGq4kQZ2cE_o9NxJgWxaM6dhPr1trkK0o,11
+seed_farmer-3.5.0rc1.dist-info/RECORD,,
```

