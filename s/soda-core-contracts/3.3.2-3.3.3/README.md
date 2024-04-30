# Comparing `tmp/soda_core_contracts-3.3.2.tar.gz` & `tmp/soda_core_contracts-3.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda_core_contracts-3.3.2.tar", last modified: Wed Apr 24 15:25:53 2024, max compression
+gzip compressed data, was "soda_core_contracts-3.3.3.tar", last modified: Tue Apr 30 11:50:24 2024, max compression
```

## Comparing `soda_core_contracts-3.3.2.tar` & `soda_core_contracts-3.3.3.tar`

### file list

```diff
@@ -1,23 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:25:53.827670 soda_core_contracts-3.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-24 15:25:53.827670 soda_core_contracts-3.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-24 15:25:40.000000 soda_core_contracts-3.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 15:25:53.827670 soda_core_contracts-3.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-24 15:25:40.000000 soda_core_contracts-3.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:25:53.823670 soda_core_contracts-3.3.2/soda/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:25:53.823670 soda_core_contracts-3.3.2/soda/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)     8771 2024-04-24 15:25:40.000000 soda_core_contracts-3.3.2/soda/contracts/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    34107 2024-04-24 15:25:40.000000 soda_core_contracts-3.3.2/soda/contracts/contract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:25:53.827670 soda_core_contracts-3.3.2/soda/contracts/impl/
--rw-r--r--   0 runner    (1001) docker     (127)    32025 2024-04-24 15:25:40.000000 soda_core_contracts-3.3.2/soda/contracts/impl/contract_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-24 15:25:40.000000 soda_core_contracts-3.3.2/soda/contracts/impl/json_schema_verifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-04-24 15:25:40.000000 soda_core_contracts-3.3.2/soda/contracts/impl/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-24 15:25:40.000000 soda_core_contracts-3.3.2/soda/contracts/impl/variable_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)    13414 2024-04-24 15:25:40.000000 soda_core_contracts-3.3.2/soda/contracts/impl/yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     6364 2024-04-24 15:25:40.000000 soda_core_contracts-3.3.2/soda/contracts/soda_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    12339 2024-04-24 15:25:40.000000 soda_core_contracts-3.3.2/soda/contracts/soda_data_contract_json_schema_1_0_0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:25:53.827670 soda_core_contracts-3.3.2/soda_core_contracts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-24 15:25:53.000000 soda_core_contracts-3.3.2/soda_core_contracts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-24 15:25:53.000000 soda_core_contracts-3.3.2/soda_core_contracts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 15:25:53.000000 soda_core_contracts-3.3.2/soda_core_contracts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-24 15:25:53.000000 soda_core_contracts-3.3.2/soda_core_contracts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-24 15:25:53.000000 soda_core_contracts-3.3.2/soda_core_contracts.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:50:24.556819 soda_core_contracts-3.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-30 11:50:24.556819 soda_core_contracts-3.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-30 11:50:11.000000 soda_core_contracts-3.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 11:50:24.556819 soda_core_contracts-3.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-30 11:50:11.000000 soda_core_contracts-3.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:50:24.552819 soda_core_contracts-3.3.3/soda/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:50:24.556819 soda_core_contracts-3.3.3/soda/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)    34525 2024-04-30 11:50:11.000000 soda_core_contracts-3.3.3/soda/contracts/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24749 2024-04-30 11:50:11.000000 soda_core_contracts-3.3.3/soda/contracts/contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12454 2024-04-30 11:50:11.000000 soda_core_contracts-3.3.3/soda/contracts/contract_verification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:50:24.556819 soda_core_contracts-3.3.3/soda/contracts/impl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-30 11:50:11.000000 soda_core_contracts-3.3.3/soda/contracts/impl/consistent_hash_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-30 11:50:11.000000 soda_core_contracts-3.3.3/soda/contracts/impl/contract_verification_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-30 11:50:11.000000 soda_core_contracts-3.3.3/soda/contracts/impl/json_schema_verifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-04-30 11:50:11.000000 soda_core_contracts-3.3.3/soda/contracts/impl/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-30 11:50:11.000000 soda_core_contracts-3.3.3/soda/contracts/impl/soda_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-30 11:50:11.000000 soda_core_contracts-3.3.3/soda/contracts/impl/variable_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4844 2024-04-30 11:50:11.000000 soda_core_contracts-3.3.3/soda/contracts/impl/warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11188 2024-04-30 11:50:11.000000 soda_core_contracts-3.3.3/soda/contracts/impl/yaml_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12961 2024-04-30 11:50:11.000000 soda_core_contracts-3.3.3/soda/contracts/soda_data_contract_json_schema_1_0_0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:50:24.556819 soda_core_contracts-3.3.3/soda_core_contracts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-30 11:50:24.000000 soda_core_contracts-3.3.3/soda_core_contracts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-30 11:50:24.000000 soda_core_contracts-3.3.3/soda_core_contracts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 11:50:24.000000 soda_core_contracts-3.3.3/soda_core_contracts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-30 11:50:24.000000 soda_core_contracts-3.3.3/soda_core_contracts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-30 11:50:24.000000 soda_core_contracts-3.3.3/soda_core_contracts.egg-info/top_level.txt
```

### Comparing `soda_core_contracts-3.3.2/soda/contracts/contract.py` & `soda_core_contracts-3.3.3/soda/contracts/check.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,364 +2,67 @@
 
 import dataclasses
 import logging
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from enum import Enum
 from numbers import Number
-from textwrap import indent
-from typing import Dict, List
+from typing import Dict
 
-from soda.cloud.soda_cloud import SodaCloud
-from soda.common import logs as soda_core_logs
 from soda.scan import Scan
-from soda.scan import logger as scan_logger
 
-from soda.contracts import soda_cloud as contract_soda_cloud
-from soda.contracts.connection import SodaException
-from soda.contracts.impl.logs import Location, Log, LogLevel, Logs
-from soda.contracts.impl.yaml import YamlObject, YamlWriter
+from soda.contracts.impl.consistent_hash_builder import ConsistentHashBuilder
+from soda.contracts.impl.logs import Location, Logs
+from soda.contracts.impl.yaml_helper import QuotingSerializer, YamlFile, YamlHelper
 
 logger = logging.getLogger(__name__)
 
 
-class Contract:
-
-    @classmethod
-    def from_yaml_str(
-        cls, contract_yaml_str: str, variables: dict[str, str] | None = None, schedule: str | None = None
-    ) -> Contract:
-        """
-        Build a contract from a YAML string
-        """
-        from soda.contracts.impl.contract_parser import ContractParser
-
-        contract_parser: ContractParser = ContractParser()
-        return contract_parser.parse_contract(
-            contract_yaml_str=contract_yaml_str, variables=variables, schedule=schedule
-        )
-
-    @classmethod
-    def from_yaml_file(
-        cls, file_path: str, variables: dict[str, str] | None = None, schedule: str | None = None
-    ) -> Contract:
-        """
-        Build a contract from a YAML file.
-        Raises OSError in case the file_path cannot be opened like e.g.
-        FileNotFoundError or PermissionError
-        """
-        with open(file_path) as f:
-            contract_yaml_str = f.read()
-            return cls.from_yaml_str(contract_yaml_str=contract_yaml_str, variables=variables, schedule=schedule)
+class Check(ABC):
 
     def __init__(
         self,
-        schedule: str | None,
-        dataset: str,
-        sql_filter: str | None,
-        schema: str | None,
-        checks: List[Check],
-        contract_yaml_str: str,
-        variables: dict[str, str] | None,
         logs: Logs,
+        contract_file: YamlFile,
+        warehouse: str,
+        schema: str | None,
+        dataset: str,
+        check_type: str,
+        check_yaml: dict,
     ):
-        """
-        Consider using Contract.from_yaml_str(contract_yaml_str) instead as that is more stable API.
-        """
-        self.schedule: str | None = schedule
-        self.dataset: str = dataset
-        self.sql_filter: str | None = sql_filter
-        self.schema: str | None = schema
-        self.checks: List[Check] = checks
-        self.contract_yaml_str: str = contract_yaml_str
-        self.variables: dict[str, str] | None = variables
-        # The initial logs will contain the logs of contract parser.  If there are error logs, these error logs
-        # will cause a SodaException to be raised at the end of the Contract.verify method
-        # See also adr/03_exceptions_vs_error_logs.md
         self.logs: Logs = logs
-        self.sodacl_yaml_str: str | None = None
-
-    def verify(self, connection: Connection, soda_cloud: contract_soda_cloud.SodaCloud | None = None) -> ContractResult:
-        """
-        Verifies if the data in the dataset matches the contract.
-        """
-
-        scan = Scan()
-
-        scan_logs = soda_core_logs.Logs(logger=scan_logger)
-        scan_logs.verbose = True
-
-        sodacl_yaml_str: str | None = None
-        try:
-            sodacl_yaml_str = self.generate_sodacl_yaml_str(self.logs)
-            logger.debug(sodacl_yaml_str)
-
-            if sodacl_yaml_str and hasattr(connection, "data_source"):
-                scan._logs = scan_logs
-
-                # This assumes the connection is a DataSourceConnection
-                data_source = connection.data_source
-                # Execute the contract SodaCL in a scan
-                scan.set_data_source_name(data_source.data_source_name)
-                scan_definition_name = (
-                    f"dataset://{connection.name}/{self.schema}/{self.dataset}"
-                    if self.schema
-                    else f"dataset://{connection.name}/{self.dataset}"
-                )
-                scan._data_source_manager.data_sources[data_source.data_source_name] = data_source
-
-                if soda_cloud:
-                    scan.set_scan_definition_name(scan_definition_name)
-                    scan._configuration.soda_cloud = SodaCloud(
-                        host=soda_cloud.host,
-                        api_key_id=soda_cloud.api_key_id,
-                        api_key_secret=soda_cloud.api_key_secret,
-                        token=soda_cloud.token,
-                        port=soda_cloud.port,
-                        logs=scan_logs,
-                        scheme=soda_cloud.scheme,
-                    )
-
-                if self.variables:
-                    scan.add_variables(self.variables)
-
-                # noinspection PyProtectedMember
-                scan.add_sodacl_yaml_str(sodacl_yaml_str)
-                scan.execute()
-
-        except Exception as e:
-            self.logs.error(f"Data contract verification error: {e}", exception=e)
-
-        if soda_cloud:
-            # If SodaCloud is configured, the logs are copied into the contract result and
-            # at the end of this method, a SodaException is raised if there are error logs.
-            self.logs.logs.extend(soda_cloud.logs.logs)
-        if connection:
-            # The connection logs are copied into the contract result and at the end of this
-            # method, a SodaException is raised if there are error logs.
-            self.logs.logs.extend(connection.logs.logs)
-        # The scan warning and error logs are copied into self.logs and at the end of this
-        # method, a SodaException is raised if there are error logs.
-        self.append_scan_warning_and_error_logs(scan_logs)
-
-        contract_result: ContractResult = ContractResult(
-            contract=self, sodacl_yaml_str=sodacl_yaml_str, logs=self.logs, scan=scan
-        )
-        if contract_result.failed():
-            raise SodaException(contract_result=contract_result)
-
-        return contract_result
-
-    def append_scan_warning_and_error_logs(self, scan_logs: soda_core_logs.Logs) -> None:
-        level_map = {
-            soda_core_logs.LogLevel.ERROR: LogLevel.ERROR,
-            soda_core_logs.LogLevel.WARNING: LogLevel.WARNING,
-            soda_core_logs.LogLevel.INFO: LogLevel.INFO,
-            soda_core_logs.LogLevel.DEBUG: LogLevel.DEBUG,
-        }
-        for scan_log in scan_logs.logs:
-            if scan_log.level in [soda_core_logs.LogLevel.ERROR, soda_core_logs.LogLevel.WARNING]:
-                contracts_location: Location = (
-                    Location(line=scan_log.location.line, column=scan_log.location.col)
-                    if scan_log.location is not None
-                    else None
-                )
-                contracts_level: LogLevel = level_map[scan_log.level]
-                self.logs._log(
-                    Log(
-                        level=contracts_level,
-                        message=f"SodaCL: {scan_log.message}",
-                        location=contracts_location,
-                        exception=scan_log.exception,
-                    )
-                )
-
-    def generate_sodacl_yaml_str(self, logs: Logs) -> str:
-        # Serialize the SodaCL YAML object to a YAML string
-        sodacl_checks: list = []
-        sodacl_yaml_object: dict = (
-            {
-                f"filter {self.dataset} [filter]": {"where": self.sql_filter},
-                f"checks for {self.dataset} [filter]": sodacl_checks,
-            }
-            if self.sql_filter
-            else {f"checks for {self.dataset}": sodacl_checks}
-        )
-
-        for check in self.checks:
-            sodacl_check = check.to_sodacl_check()
-            if sodacl_check is not None:
-                sodacl_checks.append(sodacl_check)
-        yaml_writer: YamlWriter = YamlWriter(logs)
-        return yaml_writer.write_to_yaml_str(sodacl_yaml_object)
-
-
-@dataclass
-class ContractResult:
-    """
-    This is the immutable data structure containing all the results from a single contract verification.
-    This includes any potential execution errors as well as the results of all the checks performed.
-    """
-
-    contract: Contract
-    sodacl_yaml_str: str | None
-    # self.logs combines all the logs of the contract verification with the logs of the Connection parsing,
-    # connection usage, SodaCloud parsing and usage (if used) and contract parsing.
-    # At the end of the verify method a SodaException is raised if there are any error logs or check failures.
-    # See also adr/03_exceptions_vs_error_logs.md
-    logs: Logs
-    check_results: List[CheckResult]
-
-    def __init__(self, contract: Contract, sodacl_yaml_str: str | None, logs: Logs, scan: Scan):
-        self.contract = contract
-        self.sodacl_yaml_str = sodacl_yaml_str
-        # See also adr/03_exceptions_vs_error_logs.md
-        self.logs: Logs = Logs(logs)
-        self.check_results: List[CheckResult] = []
-
-        contract_checks_by_id: dict[str, Check] = {check.identity: check for check in contract.checks}
-
-        schema_check: SchemaCheck | None = next((c for c in contract.checks if isinstance(c, SchemaCheck)), None)
-
-        scan_metrics_by_id: dict[str, dict] = {
-            scan_metric["identity"]: scan_metric for scan_metric in scan.scan_results.get("metrics", [])
-        }
-
-        scan_checks = scan.scan_results.get("checks")
-        if isinstance(scan_checks, list):
-            for scan_check in scan_checks:
-                contract_check: Check | None = None
-                if scan_check.get("name") == "Schema Check" and scan_check.get("type") == "generic":
-                    contract_check = schema_check
-                else:
-                    contract_check_id = scan_check.get("contract_check_id")
-                    if isinstance(contract_check_id, str):
-                        contract_check = contract_checks_by_id[contract_check_id]
-
-                assert contract_check is not None, "Contract scan check matching failed :("
-
-                scan_check_metric_ids = scan_check.get("metrics")
-                scan_check_metrics = [
-                    scan_metrics_by_id.get(check_metric_id) for check_metric_id in scan_check_metric_ids
-                ]
-                scan_check_metrics_by_name = {
-                    scan_check_metric.get("metricName"): scan_check_metric for scan_check_metric in scan_check_metrics
-                }
-                check_result = contract_check.create_check_result(
-                    scan_check=scan_check, scan_check_metrics_by_name=scan_check_metrics_by_name, scan=scan
-                )
-                self.check_results.append(check_result)
-
-    def failed(self) -> bool:
-        return self.has_execution_errors() or self.has_check_failures()
-
-    def passed(self) -> bool:
-        return not self.failed()
-
-    def has_execution_errors(self):
-        return self.logs.has_errors()
-
-    def has_check_failures(self):
-        return any(check.outcome == CheckOutcome.FAIL for check in self.check_results)
-
-    def __str__(self) -> str:
-        error_texts_list: List[str] = [str(error) for error in self.logs.get_errors()]
-
-        check_failure_message_list: list[str] = []
-        for check_result in self.check_results:
-            if check_result.outcome == CheckOutcome.FAIL:
-                result_str_lines = check_result.get_contract_result_str_lines()
-                check_failure_message_list.extend(result_str_lines)
-
-        if not error_texts_list and not check_failure_message_list:
-            return "All is good. No checks failed. No contract execution errors."
-
-        errors_summary_text = f"{len(error_texts_list)} execution error"
-        if len(error_texts_list) != 1:
-            errors_summary_text = f"{errors_summary_text}s"
-
-        checks_summary_text = f"{len(check_failure_message_list)} check failure"
-        if len(check_failure_message_list) != 1:
-            checks_summary_text = f"{checks_summary_text}s"
-
-        parts = [f"{checks_summary_text} and {errors_summary_text}"]
-        if error_texts_list:
-            error_lines_text: str = indent("\n".join(error_texts_list), "  ")
-            parts.append(f"Errors: \n{error_lines_text}")
-
-        if check_failure_message_list:
-            parts.append("\n".join(check_failure_message_list))
-
-        return "\n".join(parts)
-
-
-@dataclass
-class Check(ABC):
-
-    schedule: str | None
-    dataset: str
-    column: str | None
-    type: str
-
-    # User defined name as in the contract.  None if not specified in the contract.
-    name: str | None
-
-    # Check identifier used to correlate the sodacl check results with this contract check object when parsing
-    # scan results.  Also used as correlation id in Soda Cloud to match subsequent results for the same check.
-    # Composite key created from schedule, dataset, column, type and identity_suffix.
-    identity: str | None
-
-    location: Location | None
+        self.contract_file: YamlFile = contract_file
+        self.warehouse: str = warehouse
+        self.schema: str | None = schema
+        self.dataset: str = dataset
+        self.type: str = check_type
+        self.check_yaml: dict = check_yaml
+        self.identity: str = self._create_identity()
+        self.skip: bool = False
 
     @abstractmethod
     def to_sodacl_check(self) -> str | dict | None:
         pass
 
     @abstractmethod
     def create_check_result(
         self, scan_check: dict[str, dict], scan_check_metrics_by_name: dict[str, dict], scan: Scan
     ) -> CheckResult:
         pass
 
-    @classmethod
-    def create_check_identity(
-        cls,
-        schedule: str | None,
-        dataset: str,
-        column: str | None,
-        check_type: str,
-        check_identity_suffix: str | None,
-        check_location: Location | None,
-        checks: dict[str, Check],
-        logs: Logs,
-    ) -> str:
-        opt_schedule_part = f"//{schedule}" if schedule else ""
-        opt_column_part = f"/{column}" if column else ""
-        opt_check_identity_suffix_part = f"/{check_identity_suffix}" if check_identity_suffix else ""
-        check_identity = f"{opt_schedule_part}/{dataset}{opt_column_part}/{check_type}{opt_check_identity_suffix_part}"
-
-        other_check: Check = checks.get(check_identity)
-        if other_check:
-            logs.error(f"Duplicate check identity '{check_identity}': {other_check.location} and {check_location}")
-            suffix_index: int = 2
-            while check_identity in checks:
-                opt_check_identity_suffix_part = (
-                    f"/{check_identity_suffix}_{suffix_index}" if check_identity_suffix else f"/{suffix_index}"
-                )
-                check_identity = (
-                    f"{opt_schedule_part}/{dataset}{opt_column_part}/{check_type}{opt_check_identity_suffix_part}"
-                )
-                suffix_index = suffix_index + 1
-        return check_identity
+    @abstractmethod
+    def _create_identity(self) -> str:
+        pass
 
 
-@dataclass
 class CheckResult:
-    check: Check
-    outcome: CheckOutcome
+
+    def __init__(self, check: Check, outcome: CheckOutcome):
+        self.check: Check = check
+        self.outcome: CheckOutcome = outcome
 
     def __str__(self) -> str:
         return "\n".join(self.get_contract_result_str_lines())
 
     @abstractmethod
     def get_contract_result_str_lines(self) -> list[str]:
         """
@@ -375,24 +78,68 @@
         if self.outcome == CheckOutcome.FAIL:
             return "FAILED"
         if self.outcome == CheckOutcome.PASS:
             return "passed"
         return "unverified"
 
 
-@dataclass
 class SchemaCheck(Check):
 
-    columns: dict[str, str | None]
-    optional_columns: list[str]
+    def __init__(
+        self, logs: Logs, contract_file: YamlFile, warehouse: str, schema: str | None, dataset: str, yaml_contract: dict
+    ):
+        super().__init__(
+            logs=logs,
+            contract_file=contract_file,
+            warehouse=warehouse,
+            schema=schema,
+            dataset=dataset,
+            check_type="schema",
+            check_yaml=yaml_contract,
+        )
+
+        self.columns: dict[str, str] = {}
+        self.optional_columns: list[str] = []
+
+        yaml_helper = YamlHelper(logs=self.logs, yaml_file=self.contract_file)
+        extra_columns: str | None = yaml_helper.read_string_opt(yaml_contract, "extra_columns")
+        self.extra_columns_allowed: bool = "allowed" == extra_columns
+
+        yaml_columns: list | None = yaml_helper.read_list(yaml_contract, "columns")
+        if yaml_columns:
+            for yaml_column in yaml_columns:
+                column_name: str | None = yaml_helper.read_string(yaml_column, "name")
+                data_type: str | None = yaml_helper.read_string_opt(yaml_column, "data_type")
+                if column_name:
+                    self.columns[column_name] = data_type
+
+                is_column_optional = yaml_helper.read_bool_opt(yaml_column, "optional", default_value=False)
+                if is_column_optional:
+                    self.optional_columns.append(column_name)
+
+    def _create_identity(self) -> str:
+        return (
+            ConsistentHashBuilder()
+            .add_property("warehouse", self.warehouse)
+            .add_property("schema", self.schema)
+            .add_property("dataset", self.dataset)
+            .add_property("type", self.type)
+            .get_hash()
+        )
 
     def to_sodacl_check(self) -> str | dict | None:
-        schema_fail_dict = {"when mismatching columns": self.columns}
+        column_names: dict[str, str | None] = {
+            QuotingSerializer.quote(column_name): data_type for column_name, data_type in self.columns.items()
+        }
+        schema_fail_dict = {"when mismatching columns": column_names}
         if self.optional_columns:
-            schema_fail_dict["with optional columns"] = self.optional_columns
+            optional_column_names: list[str] = [
+                QuotingSerializer.quote(column_name) for column_name in self.optional_columns
+            ]
+            schema_fail_dict["with optional columns"] = optional_column_names
         return {"schema": {"fail": schema_fail_dict}}
 
     def create_check_result(self, scan_check: dict[str, dict], scan_check_metrics_by_name: dict[str, dict], scan: Scan):
         scan_measured_schema: list[dict] = scan_check_metrics_by_name.get("schema").get("value")
         measured_schema = {c.get("columnName"): c.get("sourceDataType") for c in scan_measured_schema}
 
         diagnostics = scan_check.get("diagnostics", {})
@@ -416,21 +163,30 @@
             measured_schema=measured_schema,
             columns_not_allowed_and_present=columns_not_allowed_and_present,
             columns_required_and_not_present=columns_required_and_not_present,
             columns_having_wrong_type=columns_having_wrong_type,
         )
 
 
-@dataclass
 class SchemaCheckResult(CheckResult):
 
-    measured_schema: Dict[str, str]
-    columns_not_allowed_and_present: list[str] | None
-    columns_required_and_not_present: list[str] | None
-    columns_having_wrong_type: list[DataTypeMismatch] | None
+    def __init__(
+        self,
+        check: Check,
+        outcome: CheckOutcome,
+        measured_schema: Dict[str, str],
+        columns_not_allowed_and_present: list[str] | None,
+        columns_required_and_not_present: list[str] | None,
+        columns_having_wrong_type: list[DataTypeMismatch] | None,
+    ):
+        super().__init__(check, outcome)
+        self.measured_schema: Dict[str, str] = measured_schema
+        self.columns_not_allowed_and_present: list[str] | None = columns_not_allowed_and_present
+        self.columns_required_and_not_present: list[str] | None = columns_required_and_not_present
+        self.columns_having_wrong_type: list[DataTypeMismatch] | None = columns_having_wrong_type
 
     def get_contract_result_str_lines(self) -> list[str]:
         schema_check: SchemaCheck = self.check
         expected_schema: str = ",".join(
             [
                 f"{c.get('name')}{c.get('optional')}{c.get('type')}"
                 for c in [
@@ -462,143 +218,399 @@
                 for data_type_mismatch in self.columns_having_wrong_type
             ]
         )
         return lines
 
 
 @dataclass
-class NumericMetricCheck(Check):
+class CheckArgs:
+    logs: Logs
+    contract_file: YamlFile
+    warehouse: str
+    schema: str | None
+    dataset: str
+    filter: str | None
+    check_type: str
+    check_yaml: dict
+    check_name: str | None
+    check_name_was: str | None
+    check_filter_sql: str | None
+    threshold: Threshold
+    location: Location
+    yaml_helper: YamlHelper
+    column: str | None = None
+    missing_configurations: MissingConfigurations | None = None
+    valid_configurations: ValidConfigurations | None = None
 
-    metric: str
-    check_yaml_object: YamlObject
-    missing_configurations: MissingConfigurations | None
-    valid_configurations: ValidConfigurations | None
-    threshold: NumericThreshold | None
 
-    def to_sodacl_check(self) -> str | dict | None:
-        sodacl_check_line = self.get_sodacl_check_line()
+class CheckFactory(ABC):
+    @abstractmethod
+    def create_check(self, check_args: CheckArgs) -> Check | None:
+        pass
+
+
+class AbstractCheck(Check, ABC):
+
+    threshold_keys = [
+        "must_be_greater_than",
+        "must_be_greater_than_or_equal_to",
+        "must_be_less_than",
+        "must_be_less_than_or_equal_to",
+        "must_be",
+        "must_not_be",
+        "must_be_between",
+        "must_be_not_between",
+    ]
+
+    validity_keys = [
+        "invalid_values",
+        "invalid_format",
+        "invalid_regex_sql",
+        "valid_values",
+        "valid_format",
+        "valid_regex_sql",
+        "valid_min",
+        "valid_max",
+        "valid_length",
+        "valid_min_length",
+        "valid_max_length",
+        "valid_values_reference_data",
+    ]
+
+    def __init__(self, check_args: CheckArgs):
+        # name is initialized before super constructor because it's used in the _create_identity
+        self.name: str | None = check_args.check_name
+        # column is initialized before super constructor because it's used in the _create_identity
+        self.column: str | None = check_args.column
+        super().__init__(
+            logs=check_args.logs,
+            contract_file=check_args.contract_file,
+            warehouse=check_args.warehouse,
+            schema=check_args.schema,
+            dataset=check_args.dataset,
+            check_type=check_args.check_type,
+            check_yaml=check_args.check_yaml,
+        )
+        self.name_was: str | None = check_args.check_name_was
+        self.filter_sql: str | None = check_args.check_filter_sql
+        self.missing_configurations: MissingConfigurations = check_args.missing_configurations
+        self.valid_configurations: ValidConfigurations = check_args.valid_configurations
+        self.threshold: Threshold = check_args.threshold
+        self.location: Location = check_args.location
+
+    def _create_identity(self) -> str:
+        return self._create_identity_with_name(self.name)
 
-        sodacl_check_configs = {"contract check id": self.identity}
+    def _create_identity_with_name(self, name: str) -> str:
+        return (
+            ConsistentHashBuilder()
+            .add_property("warehouse", self.warehouse)
+            .add_property("schema", self.schema)
+            .add_property("dataset", self.dataset)
+            .add_property("column", self.column)
+            .add_property("type", self.type)
+            .add_property("name", name)
+            .get_hash()
+        )
 
+    def _create_sodacl_check_configs(self, check_specific_configs: dict | None = None) -> dict:
+        check_configs: dict = {"identity": self.identity}
         if self.name:
-            sodacl_check_configs["name"] = self.name
+            check_configs["name"] = self.name
+        if self.name_was:
+            identity_was: str = self._create_identity_with_name(self.name_was)
+            check_configs["identity_was"] = identity_was
+        if self.filter_sql:
+            check_configs["filter"] = self.filter_sql
+        if isinstance(check_specific_configs, dict):
+            for key, value in check_specific_configs.items():
+                if value is not None:
+                    check_configs[key] = value
+        return check_configs
+
+
+class MissingCheckFactory(CheckFactory):
+    def create_check(self, check_args: CheckArgs) -> Check | None:
+        check_type = check_args.check_type
+        if check_type in ["no_missing_values", "missing_count", "missing_percent"]:
+            threshold = check_args.threshold
+            metric = check_type
+            if check_type == "no_missing_values":
+                metric = "missing_count"
+                if threshold and not threshold.is_empty():
+                    check_args.logs.error("Check type 'no_missing_values' does not allow for threshold keys must_...")
+                else:
+                    check_args.threshold = Threshold(equal=0)
+            elif not threshold or threshold.is_empty():
+                check_args.logs.error(f"Check type '{check_type}' requires threshold configuration")
+            return MetricCheck(check_args=check_args, metric=metric)
+
+
+class InvalidCheckFactory(CheckFactory):
+    def create_check(self, check_args: CheckArgs) -> Check | None:
+        check_type = check_args.check_type
+        if check_type not in ["no_invalid_values", "invalid_count", "invalid_percent"]:
+            return None
+
+        metric = "invalid_count" if check_type == "no_invalid_values" else check_type
+        valid_configurations: ValidConfigurations = check_args.valid_configurations
+        if valid_configurations and valid_configurations.valid_values_reference_data:
+            return ReferenceDataCheck(check_args=check_args, metric=metric)
+
+        threshold: Threshold | None = check_args.threshold
+        if check_type == "no_invalid_values":
+            if threshold and not threshold.is_empty():
+                check_args.logs.error("Check type 'no_invalid_values' does not allow for threshold keys must_...")
+            else:
+                check_args.threshold = Threshold(equal=0)
+        elif not threshold or threshold.is_empty():
+            check_args.logs.error(f"Check type '{check_type}' requires threshold configuration")
+
+        if not valid_configurations or not valid_configurations.has_non_reference_data_configs():
+            check_args.logs.error(
+                f"Check type '{check_type}' must have a validity configuration like {AbstractCheck.validity_keys}"
+            )
+        return MetricCheck(check_args=check_args, metric=metric)
+
+
+class DuplicateCheckFactory(CheckFactory):
+    def create_check(self, check_args: CheckArgs) -> Check | None:
+        check_type = check_args.check_type
+        if check_type in ["no_duplicate_values", "duplicate_count", "duplicate_percent"]:
+            threshold: Threshold | None = check_args.threshold
+            metric = check_type
+            if check_type == "no_duplicate_values":
+                metric = "duplicate_count"
+                if threshold and not threshold.is_empty():
+                    check_args.logs.error("Check type 'no_duplicate_values' does not allow for threshold keys must_...")
+                else:
+                    check_args.threshold = Threshold(equal=0)
+            elif not threshold or threshold.is_empty():
+                check_args.logs.error(f"Check type '{check_type}' requires threshold configuration")
+
+            return self.create_duplicate_check(check_args=check_args, metric=metric)
+
+    def create_duplicate_check(self, check_args: CheckArgs, metric: str):
+        return MetricCheck(check_args=check_args, metric=metric)
+
+
+class SqlFunctionCheckFactory(CheckFactory):
+    def create_check(self, check_args: CheckArgs) -> Check | None:
+        metric: str = check_args.check_type
+        return MetricCheck(check_args=check_args, metric=metric)
+
+
+class RowCountCheckFactory(CheckFactory):
+
+    def create_check(self, check_args: CheckArgs) -> Check | None:
+        check_type: str = check_args.check_type
+        if check_type in ["row_count", "rows_exist"]:
+            threshold = check_args.threshold
+            metric: str = check_type
+            if check_type == "rows_exist":
+                metric = "row_count"
+                if not threshold.is_empty():
+                    check_args.logs.error(
+                        "Check type 'rows_exist' does not allow for threshold keys must_...",
+                        location=check_args.location,
+                    )
+                check_args.threshold = Threshold(greater_than=0)
+            elif threshold.is_empty():
+                check_args.logs.error(
+                    (
+                        f"Check type '{check_type}' requires threshold configuration "
+                        f"with keys like {AbstractCheck.threshold_keys}"
+                    ),
+                    location=check_args.location,
+                )
+            return MetricCheck(check_args=check_args, metric=metric)
+
+
+class MetricCheck(AbstractCheck):
+
+    def __init__(self, check_args: CheckArgs, metric: str):
+        super().__init__(check_args)
+        self.metric: str = metric
+
+    def to_sodacl_check(self) -> str | dict | None:
+        sodacl_check_line = self.get_sodacl_check_line()
+        sodacl_check_configs = self._create_sodacl_check_configs()
 
         if self.valid_configurations:
             sodacl_check_configs.update(self.valid_configurations.to_sodacl_check_configs_dict())
         if self.missing_configurations:
             sodacl_check_configs.update(self.missing_configurations.to_sodacl_check_configs_dict())
 
         return {sodacl_check_line: sodacl_check_configs}
 
     def create_check_result(self, scan_check: dict[str, dict], scan_check_metrics_by_name: dict[str, dict], scan: Scan):
-        scan_metric_dict: dict
         if "(" in self.metric:
             scan_metric_name = self.metric[: self.metric.index("(")]
             scan_metric_dict = scan_check_metrics_by_name.get(scan_metric_name, None)
         else:
             scan_metric_dict = scan_check_metrics_by_name.get(self.metric, None)
         metric_value: Number = scan_metric_dict.get("value") if scan_metric_dict else None
-        return NumericMetricCheckResult(
+        return MetricCheckResult(
             check=self, outcome=CheckOutcome.from_scan_check(scan_check), metric_value=metric_value
         )
 
     def get_sodacl_check_line(self) -> str:
         sodacl_metric = self.get_sodacl_metric()
         sodacl_threshold: str = self.threshold.get_sodacl_threshold() if self.threshold else ""
         return f"{sodacl_metric} {sodacl_threshold}"
 
     def get_sodacl_metric(self) -> str:
-        return f"{self.metric}({self.column})" if self.column else self.metric
+        column_name: str = QuotingSerializer.quote(self.column)
+        return f"{self.metric}({column_name})" if column_name else self.metric
 
     def get_sodacl_threshold(self) -> str:
         return self.threshold.get_sodacl_threshold() if self.threshold else "?"
 
     def get_metric_str(self) -> str:
         return self.get_sodacl_metric()
 
     def get_expected_str(self) -> str:
         return f"{self.get_metric_str()} {self.get_sodacl_threshold()}"
 
 
-@dataclass
-class NumericMetricCheckResult(CheckResult):
-    metric_value: Number
+class MetricCheckResult(CheckResult):
+    def __init__(
+        self,
+        check: Check,
+        outcome: CheckOutcome,
+        metric_value: Number,
+    ):
+        super().__init__(check, outcome)
+        self.metric_value: Number = metric_value
 
     def get_contract_result_str_lines(self) -> list[str]:
         return [
             self.get_outcome_and_name_line(),
             f"  Expected {self.check.get_expected_str()}",
             f"  Actual {self.check.get_metric_str() } was {self.metric_value}",
         ]
 
 
-@dataclass
-class DuplicateCheck(NumericMetricCheck):
-    columns: list[str]
+class ReferenceDataCheck(MetricCheck):
 
-    def get_sodacl_metric(self) -> str:
-        column_str = self.column if self.column else ", ".join(self.columns)
-        return f"{self.metric}({column_str})"
-
-
-@dataclass
-class InvalidReferenceCheck(NumericMetricCheck):
-
-    valid_values_reference_data: ValidValuesReferenceData
+    def __init__(self, metric: str, check_args: CheckArgs):
+        super().__init__(check_args=check_args, metric=metric)
+        self.valid_values_reference_data: ValidValuesReferenceData = (
+            check_args.valid_configurations.valid_values_reference_data
+        )
 
     def to_sodacl_check(self) -> str | dict | None:
-        sodacl_check_configs = {"contract check id": self.identity}
-
-        if self.name:
-            sodacl_check_configs["name"] = self.name
+        sodacl_check_configs = self._create_sodacl_check_configs()
 
         if self.valid_configurations:
             sodacl_check_configs.update(self.valid_configurations.to_sodacl_check_configs_dict())
         if self.missing_configurations:
             sodacl_check_configs.update(self.missing_configurations.to_sodacl_check_configs_dict())
 
         sodacl_check_line: str = (
-            f"values in ({self.column}) must exist in {self.valid_values_reference_data.dataset} ({self.valid_values_reference_data.column})"
+            f"values in ({QuotingSerializer.quote(self.column)}) "
+            f"must exist in {QuotingSerializer.quote(self.valid_values_reference_data.dataset)} "
+            f"({QuotingSerializer.quote(self.valid_values_reference_data.column)})"
         )
 
         return {sodacl_check_line: sodacl_check_configs}
 
     def create_check_result(self, scan_check: dict[str, dict], scan_check_metrics_by_name: dict[str, dict], scan: Scan):
         scan_metric_dict = scan_check_metrics_by_name.get("reference", {})
         value: Number = scan_metric_dict.get("value")
-        return NumericMetricCheckResult(
-            check=self, outcome=CheckOutcome.from_scan_check(scan_check), metric_value=value
+        return MetricCheckResult(check=self, outcome=CheckOutcome.from_scan_check(scan_check), metric_value=value)
+
+
+class UserDefinedMetricExpressionCheckFactory(CheckFactory):
+    def create_check(self, check_args: CheckArgs) -> Check | None:
+        check_type: str = check_args.check_type
+        if check_type == "metric_expression":
+            return UserDefinedMetricExpressionCheck(check_args)
+
+
+class UserDefinedMetricExpressionCheck(MetricCheck):
+    def __init__(self, check_args: CheckArgs):
+        check_yaml = check_args.check_yaml
+        metric: str = check_args.yaml_helper.read_string_opt(check_yaml, "metric")
+        super().__init__(check_args=check_args, metric=metric)
+        self.expression_sql: str = check_yaml.get("expression_sql")
+
+    def to_sodacl_check(self) -> str | dict | None:
+        sodacl_check_configs = self._create_sodacl_check_configs({f"{self.metric} expression": self.expression_sql})
+
+        sodacl_checkline_threshold = self.threshold.get_sodacl_threshold()
+        sodacl_check_line = f"{self.get_sodacl_metric()} {sodacl_checkline_threshold}"
+
+        return {sodacl_check_line: sodacl_check_configs}
+
+    def create_check_result(self, scan_check: dict[str, dict], scan_check_metrics_by_name: dict[str, dict], scan: Scan):
+        scan_metric_dict: dict = scan_check_metrics_by_name.get(self.metric, None)
+        metric_value: Number = scan_metric_dict.get("value") if scan_metric_dict else None
+        return MetricCheckResult(
+            check=self, outcome=CheckOutcome.from_scan_check(scan_check), metric_value=metric_value
         )
 
 
-@dataclass
-class FreshnessCheck(Check):
+class UserDefinedMetricQueryCheckFactory(CheckFactory):
+    def create_check(self, check_args: CheckArgs) -> Check | None:
+        check_type: str = check_args.check_type
+        if check_type == "metric_query":
+            return UserDefinedMetricQueryCheck(check_args)
+
+
+class UserDefinedMetricQueryCheck(MetricCheck):
+
+    def __init__(self, check_args: CheckArgs):
+        check_yaml = check_args.check_yaml
+        metric: str = check_args.yaml_helper.read_string(check_yaml, "metric")
+        super().__init__(check_args=check_args, metric=metric)
+        self.query_sql: str = check_args.yaml_helper.read_string(check_yaml, "query_sql")
+
+    def to_sodacl_check(self) -> str | dict | None:
+        sodacl_check_configs = self._create_sodacl_check_configs({f"{self.metric} query": self.query_sql})
+
+        sodacl_check_line: str = self.get_sodacl_check_line()
+
+        return {sodacl_check_line: sodacl_check_configs}
+
+    def create_check_result(self, scan_check: dict[str, dict], scan_check_metrics_by_name: dict[str, dict], scan: Scan):
+        scan_metric_dict: dict = scan_check_metrics_by_name.get(self.get_sodacl_check_line(), None)
+        metric_value: Number = scan_metric_dict.get("value") if scan_metric_dict else None
+
+        return MetricCheckResult(
+            check=self, outcome=CheckOutcome.from_scan_check(scan_check), metric_value=metric_value
+        )
+
+
+class FreshnessCheckFactory(CheckFactory):
+    def create_check(self, check_args: CheckArgs) -> Check | None:
+        check_type = check_args.check_type
+        if check_type.startswith("freshness_"):
+            return FreshnessCheck(check_args)
 
-    column: str | None
-    check_yaml_object: YamlObject
-    threshold: NumericThreshold | None
+
+class FreshnessCheck(AbstractCheck):
+
+    def __init__(self, check_args: CheckArgs):
+        super().__init__(check_args)
 
     def get_definition_line(self) -> str:
-        return f"freshness({self.column}) {self.threshold.get_sodacl_threshold()}{self.get_sodacl_time_unit()}"
+        column_name: str = QuotingSerializer.quote(self.column)
+        return f"freshness({column_name}) {self.threshold.get_sodacl_threshold()}{self.get_sodacl_time_unit()}"
 
     def get_sodacl_time_unit(self) -> str:
         sodacl_time_unit_by_check_type = {
             "freshness_in_days": "d",
             "freshness_in_hours": "h",
             "freshness_in_minutes": "m",
         }
         return sodacl_time_unit_by_check_type.get(self.type)
 
     def to_sodacl_check(self) -> str | dict | None:
-        sodacl_check_configs = {
-            "contract check id": self.identity,
-        }
-        if self.name:
-            sodacl_check_configs["name"] = self.name
-
+        sodacl_check_configs = self._create_sodacl_check_configs()
         sodacl_check_line: str = self.get_definition_line()
         return {sodacl_check_line: sodacl_check_configs}
 
     def create_check_result(self, scan_check: dict[str, dict], scan_check_metrics_by_name: dict[str, dict], scan: Scan):
         diagnostics: dict = scan_check["diagnostics"]
         freshness = diagnostics["freshness"]
         freshness_column_max_value = diagnostics["maxColumnTimestamp"]
@@ -613,86 +625,70 @@
             freshness_column_max_value=freshness_column_max_value,
             freshness_column_max_value_utc=freshness_column_max_value_utc,
             now=now,
             now_utc=now_utc,
         )
 
 
-@dataclass
 class FreshnessCheckResult(CheckResult):
-    freshness: str
-    freshness_column_max_value: str
-    freshness_column_max_value_utc: str
-    now: str
-    now_utc: str
+
+    def __init__(
+        self,
+        check: Check,
+        outcome: CheckOutcome,
+        freshness: str,
+        freshness_column_max_value: str,
+        freshness_column_max_value_utc: str,
+        now: str,
+        now_utc: str,
+    ):
+        super().__init__(
+            check=check,
+            outcome=outcome,
+        )
+        self.freshness: str = freshness
+        self.freshness_column_max_value: str = freshness_column_max_value
+        self.freshness_column_max_value_utc: str = freshness_column_max_value_utc
+        self.now: str = now
+        self.now_utc: str = now_utc
 
     def get_contract_result_str_lines(self) -> list[str]:
         assert isinstance(self.check, FreshnessCheck)
         return [
             self.get_outcome_and_name_line(),
             f"  Expected {self.check.get_definition_line()}",
             f"  Actual freshness({self.check.column}) was {self.freshness}",
             f"  Max value in column was ...... {self.freshness_column_max_value}",
             f"  Max value in column in UTC was {self.freshness_column_max_value_utc}",
             f"  Now was ...................... {self.now}",
             f"  Now in UTC was ............... {self.now_utc}",
         ]
 
 
-@dataclass
-class UserDefinedMetricSqlExpressionCheck(NumericMetricCheck):
-
-    metric_sql_expression: str
-
-    def to_sodacl_check(self) -> str | dict | None:
-
-        sodacl_check_configs = {
-            "contract check id": self.identity,
-            f"{self.metric} expression": self.metric_sql_expression,
-        }
-        if self.name:
-            sodacl_check_configs["name"] = self.name
-
-        sodacl_checkline_threshold = self.threshold.get_sodacl_threshold()
-        sodacl_check_line = f"{self.get_sodacl_metric()} {sodacl_checkline_threshold}"
-
-        return {sodacl_check_line: sodacl_check_configs}
-
-    def create_check_result(self, scan_check: dict[str, dict], scan_check_metrics_by_name: dict[str, dict], scan: Scan):
-        scan_metric_dict: dict = scan_check_metrics_by_name.get(self.metric, None)
-        metric_value: Number = scan_metric_dict.get("value") if scan_metric_dict else None
-        return NumericMetricCheckResult(
-            check=self, outcome=CheckOutcome.from_scan_check(scan_check), metric_value=metric_value
-        )
-
-
-@dataclass
-class UserDefinedMetricSqlQueryCheck(NumericMetricCheck):
-
-    metric_sql_query: str
+class MultiColumnDuplicateCheckFactory(DuplicateCheckFactory):
 
-    def to_sodacl_check(self) -> str | dict | None:
-        sodacl_check_configs = {
-            "contract check id": self.identity,
-            f"{self.metric} query": self.metric_sql_query,
-        }
-        if self.name:
-            sodacl_check_configs["name"] = self.name
+    def create_duplicate_check(self, check_args: CheckArgs, metric: str):
+        columns: list[str] = check_args.yaml_helper.read_list_of_strings(check_args.check_yaml, "columns")
+        return MultiColumnDuplicateCheck(check_args=check_args, metric=metric, columns=columns)
 
-        sodacl_check_line: str = self.get_sodacl_check_line()
 
-        return {sodacl_check_line: sodacl_check_configs}
+class MultiColumnDuplicateCheck(MetricCheck):
 
-    def create_check_result(self, scan_check: dict[str, dict], scan_check_metrics_by_name: dict[str, dict], scan: Scan):
-        scan_metric_dict: dict = scan_check_metrics_by_name.get(self.get_sodacl_check_line(), None)
-        metric_value: Number = scan_metric_dict.get("value") if scan_metric_dict else None
+    def __init__(self, check_args: CheckArgs, metric: str, columns: list[str]):
+        super().__init__(check_args=check_args, metric=metric)
+        self.columns: list[str] = columns
 
-        return NumericMetricCheckResult(
-            check=self, outcome=CheckOutcome.from_scan_check(scan_check), metric_value=metric_value
-        )
+    def get_sodacl_metric(self) -> str:
+        # https://sodadata.slack.com/archives/C02J6Q493PY/p1714052722844239
+        # column_str = (
+        #     QuotingSerializer.quote(self.column) if self.column
+        #     else ", ".join([QuotingSerializer.quote(column_name) for column_name in self.columns])
+        # )
+        column_str = self.column if self.column else ", ".join(self.columns)
+        return f"{self.metric}({column_str})"
 
 
 class CheckOutcome(Enum):
     PASS = "pass"
     FAIL = "fail"
     UNKNOWN = "unknown"
 
@@ -711,39 +707,39 @@
     column: str
     expected_data_type: str
     actual_data_type: str
 
 
 def dataclass_object_to_sodacl_dict(dataclass_object: object) -> dict:
     def translate_to_sodacl_key(key: str) -> str:
-        if "sql_" in key:
-            key = key.replace("sql_", "")
+        if "_sql" in key:
+            key = key.replace("_sql", "")
         return key.replace("_", " ")
 
     dict_factory = lambda x: {translate_to_sodacl_key(k): v for (k, v) in x if v is not None}
     return dataclasses.asdict(dataclass_object, dict_factory=dict_factory)
 
 
 @dataclass
 class MissingConfigurations:
     missing_values: list[str] | list[Number] | None
-    missing_sql_regex: str | None
+    missing_regex_sql: str | None
 
     def to_sodacl_check_configs_dict(self) -> dict:
         return dataclass_object_to_sodacl_dict(self)
 
 
 @dataclass
 class ValidConfigurations:
     invalid_values: list[str] | list[Number] | None
     invalid_format: str | None
-    invalid_sql_regex: str | None
+    invalid_regex_sql: str | None
     valid_values: list[str] | list[Number] | None
     valid_format: str | None
-    valid_sql_regex: str | None
+    valid_regex_sql: str | None
     valid_min: Number | None
     valid_max: Number | None
     valid_length: int | None
     valid_min_length: int | None
     valid_max_length: int | None
     valid_values_reference_data: ValidValuesReferenceData | None
 
@@ -752,18 +748,18 @@
         sodacl_check_configs_dict.pop("valid values reference data", None)
         return sodacl_check_configs_dict
 
     def has_non_reference_data_configs(self) -> bool:
         return (
             self.invalid_values is not None
             or self.invalid_format is not None
-            or self.invalid_sql_regex is not None
+            or self.invalid_regex_sql is not None
             or self.valid_values is not None
             or self.valid_format is not None
-            or self.valid_sql_regex is not None
+            or self.valid_regex_sql is not None
             or self.valid_min is not None
             or self.valid_max is not None
             or self.valid_length is not None
             or self.valid_min_length is not None
             or self.valid_max_length is not None
         )
 
@@ -771,15 +767,15 @@
 @dataclass
 class ValidValuesReferenceData:
     dataset: str
     column: str
 
 
 @dataclass
-class NumericThreshold:
+class Threshold:
     """
     The threshold is exceeded when any of the member field conditions is True.
     To be interpreted as a check fails when the metric value is ...greater_than or ...less_than etc...
     """
 
     greater_than: Number | None = None
     greater_than_or_equal: Number | None = None
@@ -791,15 +787,15 @@
     not_between: Range | None = None
 
     def get_sodacl_threshold(self) -> str:
         greater_bound: Number | None = (
             self.greater_than if self.greater_than is not None else self.greater_than_or_equal
         )
         less_bound: Number | None = self.less_than if self.less_than is not None else self.less_than_or_equal
-        if greater_bound is not None and less_bound is not None:
+        if isinstance(greater_bound, Number) and isinstance(less_bound, Number):
             if greater_bound > less_bound:
                 return self.sodacl_threshold(
                     is_not_between=True,
                     lower_bound=less_bound,
                     lower_bound_included=self.less_than is not None,
                     upper_bound=greater_bound,
                     upper_bound_included=self.greater_than is not None,
```

### Comparing `soda_core_contracts-3.3.2/soda/contracts/impl/json_schema_verifier.py` & `soda_core_contracts-3.3.3/soda/contracts/impl/json_schema_verifier.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,17 +7,15 @@
 from soda.contracts.impl.logs import Logs
 
 
 class ValidatorLoader:
 
     @classmethod
     def load_json_schema_validator(cls) -> Draft7Validator:
-        this_file_path: str = __file__
         suffix = "/impl/json_schema_verifier.py"
-        assert this_file_path.endswith(suffix)
         contracts_dir = __file__[: -len(suffix)]
         contract_schema_json_file_path = f"{contracts_dir}/soda_data_contract_json_schema_1_0_0.json"
         with open(contract_schema_json_file_path) as f:
             contract_schema_json_str = f.read()
             schema_dict = json.loads(contract_schema_json_str)
             return Draft7Validator(schema_dict)
```

### Comparing `soda_core_contracts-3.3.2/soda/contracts/impl/logs.py` & `soda_core_contracts-3.3.3/soda/contracts/impl/logs.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from textwrap import indent
 from typing import List
 
 
 @dataclass
 class Location:
 
-    file: str | None = (None,)
-    line: int | None = (None,)
-    column: int | None = None
+    file_path: str | None
+    line: int | None
+    column: int | None
 
     def __str__(self):
         parts = [
-            f"file={self.file}" if self.file else None,
             f"line={self.line}" if self.line is not None else None,
             f"column={self.column}" if self.column is not None else None,
+            f"file={self.file_path}" if self.file_path is not None else None,
         ]
         parts = [p for p in parts if p is not None]
         return ",".join(parts)
 
     def __hash__(self) -> int:
         return hash((self.line, self.column))
 
@@ -68,32 +68,33 @@
     @classmethod
     def error(cls, message: str, location: Location | None = None, exception: BaseException | None = None) -> Log:
         return Log(level=LogLevel.ERROR, message=message, location=location, exception=exception)
 
 
 class Logs:
 
+    # See also adr/03_exceptions_vs_error_logs.md
+
     def __init__(self, logs: Logs | None = None):
         self.logs: List[Log] = []
         if logs is not None:
             self.logs = logs.logs.copy()
 
     def __str__(self) -> str:
         return "\n".join([str(log) for log in self.logs])
 
-    def assert_no_errors(self) -> None:
-        if self.has_errors():
-            errors_lines: List[str] = [str(log) for log in self.logs if log.level == LogLevel.ERROR]
-            error_text = "\n".join(errors_lines)
-            error_word = "error: " if len(self.logs) == 1 else "errors:\n"
-            raise AssertionError(f"Connection {error_word}{error_text}")
-
     def has_errors(self) -> bool:
         return any(log.level == LogLevel.ERROR for log in self.logs)
 
+    def get_errors_str(self) -> str:
+        errors_lines: List[str] = [str(log) for log in self.logs if log.level == LogLevel.ERROR]
+        error_text = "\n".join(errors_lines)
+        error_word = "Error: " if len(self.logs) == 1 else "Errors:\n"
+        return f"{error_word}{error_text}"
+
     def get_errors(self) -> List[Log]:
         return [log for log in self.logs if log.level == LogLevel.ERROR]
 
     def error(self, message: str, location: Location | None = None, exception: BaseException | None = None) -> None:
         self._log(Log(LogLevel.ERROR, message, location, exception))
 
     def _log(self, log: Log) -> None:
```

### Comparing `soda_core_contracts-3.3.2/soda/contracts/impl/variable_resolver.py` & `soda_core_contracts-3.3.3/soda/contracts/impl/variable_resolver.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,13 +17,13 @@
     def resolve(self, text: str) -> str:
         return re.sub(
             pattern=r"\$\{([a-zA-Z_][a-zA-Z_0-9]*)\}",
             repl=lambda m: self._resolve_variable(m.group(1).strip()),
             string=text,
         )
 
-    def _resolve_variable(self, variable_name: str, variables: Dict[str, str] | None = None) -> str:
+    def _resolve_variable(self, variable_name: str) -> str:
         if self.variables is not None and variable_name in self.variables:
             return self.variables[variable_name]
         if variable_name in os.environ:
             return os.getenv(variable_name)
-        self.logs.error(f"Variable '{variable_name}' not configured as environment variable")
+        self.logs.error(f"Variable '{variable_name}' not defined in the variables nor as environment variable")
```

### Comparing `soda_core_contracts-3.3.2/soda/contracts/soda_data_contract_json_schema_1_0_0.json` & `soda_core_contracts-3.3.3/soda/contracts/soda_data_contract_json_schema_1_0_0.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9764384920634921%*

 * *Differences: {"'$defs'": "{'check': {'properties': {'missing_regex_sql': OrderedDict([('description', "*

 * *            "'Customized SQL regex to identify missing values. The flavor of regex depends on the "*

 * *            'SQL engine / warehouse. NULL is always considered missing so that does not have to be '*

 * *            "specified. Implies a missing_count check in Soda.'), ('type', 'string')]), "*

 * *            "'valid_regex_sql': OrderedDict([('description', 'A SQL regular expression that "*

 * *            'matches valid values. I […]*

```diff
@@ -1,34 +1,34 @@
 {
     "$defs": {
         "check": {
             "properties": {
-                "filter_sql_expression": {
-                    "description": "Specifies a sql expression filter that should be applied on the metric",
+                "filter_sql": {
+                    "description": "[Not yet supported] Specifies a sql expression filter that should be applied on the metric",
                     "type": "string"
                 },
                 "invalid_format": {
                     "$ref": "#/$defs/format",
                     "description": "A named regular expression that specifies invalid values."
                 },
-                "invalid_sql_regex": {
+                "invalid_regex_sql": {
                     "description": "A regular expression that specifies valid values.",
                     "type": "string"
                 },
                 "invalid_values": {
                     "description": "A list of valid values. Only supports all strings or all numbers. Implies an invalid_count check in Soda.",
                     "items": {
                         "type": [
                             "number",
                             "string"
                         ]
                     },
                     "type": "array"
                 },
-                "missing_sql_regex": {
+                "missing_regex_sql": {
                     "description": "Customized SQL regex to identify missing values. The flavor of regex depends on the SQL engine / warehouse. NULL is always considered missing so that does not have to be specified. Implies a missing_count check in Soda.",
                     "type": "string"
                 },
                 "missing_values": {
                     "description": "Customized list of missing values. NULL is always considered missing so that does not have to be specified. If no customization is needed, consider specifying not_null:true instead. Implies a missing_count check in Soda.",
                     "items": {
                         "type": [
@@ -135,15 +135,15 @@
                     "description": "The minimum allowed value. Only for numeric data types or text types with a numeric format. Implies an invalid_count check in Soda.",
                     "type": "integer"
                 },
                 "valid_min_length": {
                     "description": "The minimum length of values. Only for text data types. Implies an invalid_count check in Soda.",
                     "type": "integer"
                 },
-                "valid_sql_regex": {
+                "valid_regex_sql": {
                     "description": "A SQL regular expression that matches valid values. Implies a valid_count check in Soda. All (in)valid_* configs are combined in a single invalid_count check.",
                     "type": "string"
                 },
                 "valid_values": {
                     "description": "A list of valid values. Only supports all strings or all numbers. Implies an invalid_count check in Soda.",
                     "items": {
                         "type": [
@@ -226,15 +226,15 @@
             "description": "A list of checks for this dataset executed by a Soda",
             "items": {
                 "$ref": "#/$defs/check"
             },
             "type": "array"
         },
         "columns": {
-            "description": "The schema",
+            "description": "The list of columns, also known as 'the schema' of the dataset.",
             "items": {
                 "properties": {
                     "checks": {
                         "description": "Checks for this column",
                         "items": {
                             "$ref": "#/$defs/check"
                         },
@@ -307,20 +307,34 @@
             "type": "array"
         },
         "dataset": {
             "description": "The name of the dataset",
             "type": "string"
         },
         "description": {
-            "description": "The description of the dataset.  What does each row represent?",
+            "description": "The description of the dataset",
             "type": "string"
         },
         "owner": {
-            "description": "Contact person for this contract. Email address.",
-            "format": "email",
+            "description": "The contact details for the person or team responsible for producing this dataset",
+            "properties": {
+                "email": {
+                    "description": "The email of the person or group responsible for producing this dataset",
+                    "format": "email",
+                    "type": "string"
+                }
+            },
+            "type": "object"
+        },
+        "schema": {
+            "description": "The name of the schema within the data source (on bigquery, this schema property this refers to a dataset)",
+            "type": "string"
+        },
+        "warehouse": {
+            "description": "The name of the warehouse",
             "type": "string"
         }
     },
     "required": [
         "dataset",
         "columns"
     ],
```

### Comparing `soda_core_contracts-3.3.2/soda_core_contracts.egg-info/SOURCES.txt` & `soda_core_contracts-3.3.3/soda_core_contracts.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 README.md
 setup.py
-soda/contracts/connection.py
+soda/contracts/check.py
 soda/contracts/contract.py
-soda/contracts/soda_cloud.py
+soda/contracts/contract_verification.py
 soda/contracts/soda_data_contract_json_schema_1_0_0.json
-soda/contracts/impl/contract_parser.py
+soda/contracts/impl/consistent_hash_builder.py
+soda/contracts/impl/contract_verification_impl.py
 soda/contracts/impl/json_schema_verifier.py
 soda/contracts/impl/logs.py
+soda/contracts/impl/soda_cloud.py
 soda/contracts/impl/variable_resolver.py
-soda/contracts/impl/yaml.py
+soda/contracts/impl/warehouse.py
+soda/contracts/impl/yaml_helper.py
 soda_core_contracts.egg-info/PKG-INFO
 soda_core_contracts.egg-info/SOURCES.txt
 soda_core_contracts.egg-info/dependency_links.txt
 soda_core_contracts.egg-info/requires.txt
 soda_core_contracts.egg-info/top_level.txt
```

