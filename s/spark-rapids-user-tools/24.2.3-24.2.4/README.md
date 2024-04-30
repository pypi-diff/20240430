# Comparing `tmp/spark_rapids_user_tools-24.2.3-241_f740195-py3-none-any.whl.zip` & `tmp/spark_rapids_user_tools-24.2.4-248_e093c7c-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,127 +1,130 @@
-Zip file size: 863951 bytes, number of entries: 125
--rw-r--r--  2.0 unx      750 b- defN 24-Apr-24 14:51 spark_rapids_pytools/__init__.py
--rw-r--r--  2.0 unx      992 b- defN 24-Apr-24 14:51 spark_rapids_pytools/build.py
--rw-r--r--  2.0 unx     1450 b- defN 24-Apr-24 14:51 spark_rapids_pytools/wrapper.py
--rw-r--r--  2.0 unx      646 b- defN 24-Apr-24 14:51 spark_rapids_pytools/cloud_api/__init__.py
--rw-r--r--  2.0 unx     8507 b- defN 24-Apr-24 14:51 spark_rapids_pytools/cloud_api/azurestorage.py
--rw-r--r--  2.0 unx    16172 b- defN 24-Apr-24 14:51 spark_rapids_pytools/cloud_api/databricks_aws.py
--rw-r--r--  2.0 unx     1268 b- defN 24-Apr-24 14:51 spark_rapids_pytools/cloud_api/databricks_aws_job.py
--rw-r--r--  2.0 unx    19896 b- defN 24-Apr-24 14:51 spark_rapids_pytools/cloud_api/databricks_azure.py
--rw-r--r--  2.0 unx     2428 b- defN 24-Apr-24 14:51 spark_rapids_pytools/cloud_api/databricks_azure_job.py
--rw-r--r--  2.0 unx    26700 b- defN 24-Apr-24 14:51 spark_rapids_pytools/cloud_api/dataproc.py
--rw-r--r--  2.0 unx     8455 b- defN 24-Apr-24 14:51 spark_rapids_pytools/cloud_api/dataproc_gke.py
--rw-r--r--  2.0 unx      929 b- defN 24-Apr-24 14:51 spark_rapids_pytools/cloud_api/dataproc_gke_job.py
--rw-r--r--  2.0 unx      922 b- defN 24-Apr-24 14:51 spark_rapids_pytools/cloud_api/dataproc_job.py
--rw-r--r--  2.0 unx    22845 b- defN 24-Apr-24 14:51 spark_rapids_pytools/cloud_api/emr.py
--rw-r--r--  2.0 unx     1252 b- defN 24-Apr-24 14:51 spark_rapids_pytools/cloud_api/emr_job.py
--rw-r--r--  2.0 unx     4939 b- defN 24-Apr-24 14:51 spark_rapids_pytools/cloud_api/gstorage.py
--rw-r--r--  2.0 unx    13941 b- defN 24-Apr-24 14:51 spark_rapids_pytools/cloud_api/onprem.py
--rw-r--r--  2.0 unx     4055 b- defN 24-Apr-24 14:51 spark_rapids_pytools/cloud_api/s3storage.py
--rw-r--r--  2.0 unx    52987 b- defN 24-Apr-24 14:51 spark_rapids_pytools/cloud_api/sp_types.py
--rw-r--r--  2.0 unx      658 b- defN 24-Apr-24 14:51 spark_rapids_pytools/common/__init__.py
--rw-r--r--  2.0 unx     3927 b- defN 24-Apr-24 14:51 spark_rapids_pytools/common/cluster_inference.py
--rw-r--r--  2.0 unx      978 b- defN 24-Apr-24 14:51 spark_rapids_pytools/common/exceptions.py
--rw-r--r--  2.0 unx     5119 b- defN 24-Apr-24 14:51 spark_rapids_pytools/common/prop_manager.py
--rw-r--r--  2.0 unx    20141 b- defN 24-Apr-24 14:51 spark_rapids_pytools/common/sys_storage.py
--rw-r--r--  2.0 unx    14532 b- defN 24-Apr-24 14:51 spark_rapids_pytools/common/utilities.py
--rw-r--r--  2.0 unx      659 b- defN 24-Apr-24 14:51 spark_rapids_pytools/pricing/__init__.py
--rw-r--r--  2.0 unx     3429 b- defN 24-Apr-24 14:51 spark_rapids_pytools/pricing/databricks_azure_pricing.py
--rw-r--r--  2.0 unx     3522 b- defN 24-Apr-24 14:51 spark_rapids_pytools/pricing/databricks_pricing.py
--rw-r--r--  2.0 unx     1234 b- defN 24-Apr-24 14:51 spark_rapids_pytools/pricing/dataproc_gke_pricing.py
--rw-r--r--  2.0 unx     4247 b- defN 24-Apr-24 14:51 spark_rapids_pytools/pricing/dataproc_pricing.py
--rw-r--r--  2.0 unx     4747 b- defN 24-Apr-24 14:51 spark_rapids_pytools/pricing/emr_pricing.py
--rw-r--r--  2.0 unx     6698 b- defN 24-Apr-24 14:51 spark_rapids_pytools/pricing/price_provider.py
--rw-r--r--  2.0 unx      666 b- defN 24-Apr-24 14:51 spark_rapids_pytools/rapids/__init__.py
--rw-r--r--  2.0 unx     6026 b- defN 24-Apr-24 14:51 spark_rapids_pytools/rapids/bootstrap.py
--rw-r--r--  2.0 unx     6780 b- defN 24-Apr-24 14:51 spark_rapids_pytools/rapids/diagnostic.py
--rw-r--r--  2.0 unx    10472 b- defN 24-Apr-24 14:51 spark_rapids_pytools/rapids/profiling.py
--rw-r--r--  2.0 unx    58920 b- defN 24-Apr-24 14:51 spark_rapids_pytools/rapids/qualification.py
--rw-r--r--  2.0 unx     5739 b- defN 24-Apr-24 14:51 spark_rapids_pytools/rapids/rapids_job.py
--rw-r--r--  2.0 unx    43836 b- defN 24-Apr-24 14:51 spark_rapids_pytools/rapids/rapids_tool.py
--rw-r--r--  2.0 unx     8938 b- defN 24-Apr-24 14:51 spark_rapids_pytools/rapids/tool_ctxt.py
--rw-r--r--  2.0 unx      273 b- defN 24-Apr-24 14:51 spark_rapids_pytools/resources/bootstrap-conf.yaml
--rw-r--r--  2.0 unx     1073 b- defN 24-Apr-24 14:51 spark_rapids_pytools/resources/cluster-configs.yaml
--rwxr-xr-x  2.0 unx     5816 b- defN 24-Apr-24 14:51 spark_rapids_pytools/resources/collect.sh
--rw-r--r--  2.0 unx    30566 b- defN 24-Apr-24 14:51 spark_rapids_pytools/resources/databricks-premium-catalog.json
--rw-r--r--  2.0 unx    13549 b- defN 24-Apr-24 14:51 spark_rapids_pytools/resources/databricks_aws-configs.json
--rw-r--r--  2.0 unx    11272 b- defN 24-Apr-24 14:51 spark_rapids_pytools/resources/databricks_azure-configs.json
--rw-r--r--  2.0 unx     9280 b- defN 24-Apr-24 14:51 spark_rapids_pytools/resources/dataproc-configs.json
--rw-r--r--  2.0 unx     9069 b- defN 24-Apr-24 14:51 spark_rapids_pytools/resources/dataproc_gke-configs.json
--rw-r--r--  2.0 unx       30 b- defN 24-Apr-24 14:51 spark_rapids_pytools/resources/diagnostic-conf.yaml
--rw-r--r--  2.0 unx    12779 b- defN 24-Apr-24 14:51 spark_rapids_pytools/resources/emr-configs.json
--rw-r--r--  2.0 unx     5159 b- defN 24-Apr-24 14:51 spark_rapids_pytools/resources/onprem-configs.json
--rw-r--r--  2.0 unx    38903 b- defN 24-Apr-24 14:51 spark_rapids_pytools/resources/premium-databricks-azure-catalog.json
--rw-r--r--  2.0 unx     1517 b- defN 24-Apr-24 14:51 spark_rapids_pytools/resources/profiling-conf.yaml
--rw-r--r--  2.0 unx     8101 b- defN 24-Apr-24 14:51 spark_rapids_pytools/resources/qualification-conf.yaml
--rw-r--r--  2.0 unx     7779 b- defN 24-Apr-24 14:51 spark_rapids_pytools/resources/dev/prepackage_mgr.py
--rw-r--r--  2.0 unx     2195 b- defN 24-Apr-24 14:51 spark_rapids_pytools/resources/dev/process_databricks_azure_pricing.py
--rw-r--r--  2.0 unx   405769 b- defN 24-Apr-24 14:51 spark_rapids_pytools/resources/qualx/models/xgboost/databricks-aws.json
--rw-r--r--  2.0 unx   160200 b- defN 24-Apr-24 14:51 spark_rapids_pytools/resources/qualx/models/xgboost/databricks-azure.json
--rw-r--r--  2.0 unx   795042 b- defN 24-Apr-24 14:51 spark_rapids_pytools/resources/qualx/models/xgboost/dataproc.json
--rw-r--r--  2.0 unx   361292 b- defN 24-Apr-24 14:51 spark_rapids_pytools/resources/qualx/models/xgboost/dataproc_2.1-orc.json
--rw-r--r--  2.0 unx   530621 b- defN 24-Apr-24 14:51 spark_rapids_pytools/resources/qualx/models/xgboost/onprem.json
--rw-r--r--  2.0 unx      669 b- defN 24-Apr-24 14:51 spark_rapids_pytools/resources/templates/dataproc-create_gpu_cluster_script.ms
--rw-r--r--  2.0 unx      518 b- defN 24-Apr-24 14:51 spark_rapids_pytools/resources/templates/dataproc-run_bootstrap.ms
--rw-r--r--  2.0 unx      855 b- defN 24-Apr-24 14:51 spark_rapids_pytools/resources/templates/emr-create_gpu_cluster_script.ms
--rw-r--r--  2.0 unx      537 b- defN 24-Apr-24 14:51 spark_rapids_pytools/resources/templates/emr-run_bootstrap.ms
--rw-r--r--  2.0 unx      241 b- defN 24-Apr-24 14:51 spark_rapids_pytools/resources/templates/cluster_template/databricks_aws.ms
--rw-r--r--  2.0 unx      330 b- defN 24-Apr-24 14:51 spark_rapids_pytools/resources/templates/cluster_template/databricks_azure.ms
--rw-r--r--  2.0 unx      626 b- defN 24-Apr-24 14:51 spark_rapids_pytools/resources/templates/cluster_template/dataproc.ms
--rw-r--r--  2.0 unx      759 b- defN 24-Apr-24 14:51 spark_rapids_pytools/resources/templates/cluster_template/emr.ms
--rw-r--r--  2.0 unx      293 b- defN 24-Apr-24 14:51 spark_rapids_pytools/resources/templates/cluster_template/emr_node.ms
--rw-r--r--  2.0 unx      630 b- defN 24-Apr-24 14:51 spark_rapids_pytools/wrappers/__init__.py
--rw-r--r--  2.0 unx    19338 b- defN 24-Apr-24 14:51 spark_rapids_pytools/wrappers/databricks_aws_wrapper.py
--rw-r--r--  2.0 unx    18795 b- defN 24-Apr-24 14:51 spark_rapids_pytools/wrappers/databricks_azure_wrapper.py
--rw-r--r--  2.0 unx     9834 b- defN 24-Apr-24 14:51 spark_rapids_pytools/wrappers/dataproc_gke_wrapper.py
--rw-r--r--  2.0 unx    18774 b- defN 24-Apr-24 14:51 spark_rapids_pytools/wrappers/dataproc_wrapper.py
--rw-r--r--  2.0 unx    19300 b- defN 24-Apr-24 14:51 spark_rapids_pytools/wrappers/emr_wrapper.py
--rw-r--r--  2.0 unx    12518 b- defN 24-Apr-24 14:51 spark_rapids_pytools/wrappers/onprem_wrapper.py
--rw-r--r--  2.0 unx     1008 b- defN 24-Apr-24 14:51 spark_rapids_tools/__init__.py
--rw-r--r--  2.0 unx     5286 b- defN 24-Apr-24 14:51 spark_rapids_tools/enums.py
--rw-r--r--  2.0 unx     2099 b- defN 24-Apr-24 14:51 spark_rapids_tools/exceptions.py
--rw-r--r--  2.0 unx     1167 b- defN 24-Apr-24 14:51 spark_rapids_tools/cloud/__init__.py
--rw-r--r--  2.0 unx     4759 b- defN 24-Apr-24 14:51 spark_rapids_tools/cloud/cluster.py
--rw-r--r--  2.0 unx      649 b- defN 24-Apr-24 14:51 spark_rapids_tools/cloud/databricks/__init__.py
--rw-r--r--  2.0 unx     1808 b- defN 24-Apr-24 14:51 spark_rapids_tools/cloud/databricks/dbcluster.py
--rw-r--r--  2.0 unx      647 b- defN 24-Apr-24 14:51 spark_rapids_tools/cloud/dataproc/__init__.py
--rw-r--r--  2.0 unx     2243 b- defN 24-Apr-24 14:51 spark_rapids_tools/cloud/dataproc/dataproccluster.py
--rw-r--r--  2.0 unx      642 b- defN 24-Apr-24 14:51 spark_rapids_tools/cloud/emr/__init__.py
--rw-r--r--  2.0 unx     1243 b- defN 24-Apr-24 14:51 spark_rapids_tools/cloud/emr/emrcluster.py
--rw-r--r--  2.0 unx      645 b- defN 24-Apr-24 14:51 spark_rapids_tools/cloud/onprem/__init__.py
--rw-r--r--  2.0 unx     1768 b- defN 24-Apr-24 14:51 spark_rapids_tools/cloud/onprem/onpremcluster.py
--rw-r--r--  2.0 unx      706 b- defN 24-Apr-24 14:51 spark_rapids_tools/cmdli/__init__.py
--rw-r--r--  2.0 unx    27691 b- defN 24-Apr-24 14:51 spark_rapids_tools/cmdli/argprocessor.py
--rw-r--r--  2.0 unx    16404 b- defN 24-Apr-24 14:51 spark_rapids_tools/cmdli/tools_cli.py
--rw-r--r--  2.0 unx     1433 b- defN 24-Apr-24 14:51 spark_rapids_tools/storagelib/__init__.py
--rw-r--r--  2.0 unx     5549 b- defN 24-Apr-24 14:51 spark_rapids_tools/storagelib/cspfs.py
--rw-r--r--  2.0 unx    11165 b- defN 24-Apr-24 14:51 spark_rapids_tools/storagelib/csppath.py
--rw-r--r--  2.0 unx      774 b- defN 24-Apr-24 14:51 spark_rapids_tools/storagelib/adls/__init__.py
--rw-r--r--  2.0 unx     1658 b- defN 24-Apr-24 14:51 spark_rapids_tools/storagelib/adls/adlsfs.py
--rw-r--r--  2.0 unx      785 b- defN 24-Apr-24 14:51 spark_rapids_tools/storagelib/adls/adlspath.py
--rw-r--r--  2.0 unx      751 b- defN 24-Apr-24 14:51 spark_rapids_tools/storagelib/gcs/__init__.py
--rw-r--r--  2.0 unx     1528 b- defN 24-Apr-24 14:51 spark_rapids_tools/storagelib/gcs/gcsfs.py
--rw-r--r--  2.0 unx      784 b- defN 24-Apr-24 14:51 spark_rapids_tools/storagelib/gcs/gcspath.py
--rw-r--r--  2.0 unx      755 b- defN 24-Apr-24 14:51 spark_rapids_tools/storagelib/hdfs/__init__.py
--rw-r--r--  2.0 unx     1761 b- defN 24-Apr-24 14:51 spark_rapids_tools/storagelib/hdfs/hdfsfs.py
--rw-r--r--  2.0 unx      784 b- defN 24-Apr-24 14:51 spark_rapids_tools/storagelib/hdfs/hdfspath.py
--rw-r--r--  2.0 unx      760 b- defN 24-Apr-24 14:51 spark_rapids_tools/storagelib/local/__init__.py
--rw-r--r--  2.0 unx      865 b- defN 24-Apr-24 14:51 spark_rapids_tools/storagelib/local/localfs.py
--rw-r--r--  2.0 unx      780 b- defN 24-Apr-24 14:51 spark_rapids_tools/storagelib/local/localpath.py
--rw-r--r--  2.0 unx      726 b- defN 24-Apr-24 14:51 spark_rapids_tools/storagelib/s3/__init__.py
--rw-r--r--  2.0 unx     1732 b- defN 24-Apr-24 14:51 spark_rapids_tools/storagelib/s3/s3fs.py
--rw-r--r--  2.0 unx      776 b- defN 24-Apr-24 14:51 spark_rapids_tools/storagelib/s3/s3path.py
--rw-r--r--  2.0 unx      653 b- defN 24-Apr-24 14:51 spark_rapids_tools/tools/__init__.py
--rw-r--r--  2.0 unx     1096 b- defN 24-Apr-24 14:51 spark_rapids_tools/tools/autotuner.py
--rw-r--r--  2.0 unx    54414 b- defN 24-Apr-24 14:51 spark_rapids_tools/tools/model_xgboost.py
--rw-r--r--  2.0 unx     3284 b- defN 24-Apr-24 14:51 spark_rapids_tools/tools/top_candidates.py
--rw-r--r--  2.0 unx     4081 b- defN 24-Apr-24 14:51 spark_rapids_tools/tools/unsupported_ops_stage_duration.py
--rw-r--r--  2.0 unx      987 b- defN 24-Apr-24 14:51 spark_rapids_tools/utils/__init__.py
--rw-r--r--  2.0 unx     4844 b- defN 24-Apr-24 14:51 spark_rapids_tools/utils/propmanager.py
--rw-r--r--  2.0 unx    12210 b- defN 24-Apr-24 14:51 spark_rapids_tools/utils/util.py
--rw-r--r--  2.0 unx    21086 b- defN 24-Apr-24 14:51 spark_rapids_user_tools-24.2.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     4126 b- defN 24-Apr-24 14:51 spark_rapids_user_tools-24.2.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-24 14:51 spark_rapids_user_tools-24.2.3.dist-info/WHEEL
--rw-r--r--  2.0 unx      133 b- defN 24-Apr-24 14:51 spark_rapids_user_tools-24.2.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       40 b- defN 24-Apr-24 14:51 spark_rapids_user_tools-24.2.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    13035 b- defN 24-Apr-24 14:51 spark_rapids_user_tools-24.2.3.dist-info/RECORD
-125 files, 3136916 bytes uncompressed, 842485 bytes compressed:  73.2%
+Zip file size: 866245 bytes, number of entries: 128
+-rw-r--r--  2.0 unx      755 b- defN 24-Apr-30 11:13 spark_rapids_pytools/__init__.py
+-rw-r--r--  2.0 unx      992 b- defN 24-Apr-30 11:13 spark_rapids_pytools/build.py
+-rw-r--r--  2.0 unx     1450 b- defN 24-Apr-30 11:13 spark_rapids_pytools/wrapper.py
+-rw-r--r--  2.0 unx      646 b- defN 24-Apr-30 11:13 spark_rapids_pytools/cloud_api/__init__.py
+-rw-r--r--  2.0 unx     8507 b- defN 24-Apr-30 11:13 spark_rapids_pytools/cloud_api/azurestorage.py
+-rw-r--r--  2.0 unx    16540 b- defN 24-Apr-30 11:13 spark_rapids_pytools/cloud_api/databricks_aws.py
+-rw-r--r--  2.0 unx     1268 b- defN 24-Apr-30 11:13 spark_rapids_pytools/cloud_api/databricks_aws_job.py
+-rw-r--r--  2.0 unx    19913 b- defN 24-Apr-30 11:13 spark_rapids_pytools/cloud_api/databricks_azure.py
+-rw-r--r--  2.0 unx     2428 b- defN 24-Apr-30 11:13 spark_rapids_pytools/cloud_api/databricks_azure_job.py
+-rw-r--r--  2.0 unx    27376 b- defN 24-Apr-30 11:13 spark_rapids_pytools/cloud_api/dataproc.py
+-rw-r--r--  2.0 unx     8455 b- defN 24-Apr-30 11:13 spark_rapids_pytools/cloud_api/dataproc_gke.py
+-rw-r--r--  2.0 unx      929 b- defN 24-Apr-30 11:13 spark_rapids_pytools/cloud_api/dataproc_gke_job.py
+-rw-r--r--  2.0 unx      922 b- defN 24-Apr-30 11:13 spark_rapids_pytools/cloud_api/dataproc_job.py
+-rw-r--r--  2.0 unx    23288 b- defN 24-Apr-30 11:13 spark_rapids_pytools/cloud_api/emr.py
+-rw-r--r--  2.0 unx     1252 b- defN 24-Apr-30 11:13 spark_rapids_pytools/cloud_api/emr_job.py
+-rw-r--r--  2.0 unx     4939 b- defN 24-Apr-30 11:13 spark_rapids_pytools/cloud_api/gstorage.py
+-rw-r--r--  2.0 unx    13941 b- defN 24-Apr-30 11:13 spark_rapids_pytools/cloud_api/onprem.py
+-rw-r--r--  2.0 unx     4055 b- defN 24-Apr-30 11:13 spark_rapids_pytools/cloud_api/s3storage.py
+-rw-r--r--  2.0 unx    53339 b- defN 24-Apr-30 11:13 spark_rapids_pytools/cloud_api/sp_types.py
+-rw-r--r--  2.0 unx      658 b- defN 24-Apr-30 11:13 spark_rapids_pytools/common/__init__.py
+-rw-r--r--  2.0 unx     3927 b- defN 24-Apr-30 11:13 spark_rapids_pytools/common/cluster_inference.py
+-rw-r--r--  2.0 unx      978 b- defN 24-Apr-30 11:13 spark_rapids_pytools/common/exceptions.py
+-rw-r--r--  2.0 unx     5119 b- defN 24-Apr-30 11:13 spark_rapids_pytools/common/prop_manager.py
+-rw-r--r--  2.0 unx    20141 b- defN 24-Apr-30 11:13 spark_rapids_pytools/common/sys_storage.py
+-rw-r--r--  2.0 unx    14532 b- defN 24-Apr-30 11:13 spark_rapids_pytools/common/utilities.py
+-rw-r--r--  2.0 unx      659 b- defN 24-Apr-30 11:13 spark_rapids_pytools/pricing/__init__.py
+-rw-r--r--  2.0 unx     3429 b- defN 24-Apr-30 11:13 spark_rapids_pytools/pricing/databricks_azure_pricing.py
+-rw-r--r--  2.0 unx     3522 b- defN 24-Apr-30 11:13 spark_rapids_pytools/pricing/databricks_pricing.py
+-rw-r--r--  2.0 unx     1234 b- defN 24-Apr-30 11:13 spark_rapids_pytools/pricing/dataproc_gke_pricing.py
+-rw-r--r--  2.0 unx     4247 b- defN 24-Apr-30 11:13 spark_rapids_pytools/pricing/dataproc_pricing.py
+-rw-r--r--  2.0 unx     4747 b- defN 24-Apr-30 11:13 spark_rapids_pytools/pricing/emr_pricing.py
+-rw-r--r--  2.0 unx     6698 b- defN 24-Apr-30 11:13 spark_rapids_pytools/pricing/price_provider.py
+-rw-r--r--  2.0 unx      666 b- defN 24-Apr-30 11:13 spark_rapids_pytools/rapids/__init__.py
+-rw-r--r--  2.0 unx     6026 b- defN 24-Apr-30 11:13 spark_rapids_pytools/rapids/bootstrap.py
+-rw-r--r--  2.0 unx     6780 b- defN 24-Apr-30 11:13 spark_rapids_pytools/rapids/diagnostic.py
+-rw-r--r--  2.0 unx    10472 b- defN 24-Apr-30 11:13 spark_rapids_pytools/rapids/profiling.py
+-rw-r--r--  2.0 unx    59208 b- defN 24-Apr-30 11:13 spark_rapids_pytools/rapids/qualification.py
+-rw-r--r--  2.0 unx     5739 b- defN 24-Apr-30 11:13 spark_rapids_pytools/rapids/rapids_job.py
+-rw-r--r--  2.0 unx    43836 b- defN 24-Apr-30 11:13 spark_rapids_pytools/rapids/rapids_tool.py
+-rw-r--r--  2.0 unx     8938 b- defN 24-Apr-30 11:13 spark_rapids_pytools/rapids/tool_ctxt.py
+-rw-r--r--  2.0 unx      273 b- defN 24-Apr-30 11:13 spark_rapids_pytools/resources/bootstrap-conf.yaml
+-rw-r--r--  2.0 unx     1073 b- defN 24-Apr-30 11:13 spark_rapids_pytools/resources/cluster-configs.yaml
+-rwxr-xr-x  2.0 unx     5816 b- defN 24-Apr-30 11:13 spark_rapids_pytools/resources/collect.sh
+-rw-r--r--  2.0 unx    30566 b- defN 24-Apr-30 11:13 spark_rapids_pytools/resources/databricks-premium-catalog.json
+-rw-r--r--  2.0 unx    13549 b- defN 24-Apr-30 11:13 spark_rapids_pytools/resources/databricks_aws-configs.json
+-rw-r--r--  2.0 unx    11272 b- defN 24-Apr-30 11:13 spark_rapids_pytools/resources/databricks_azure-configs.json
+-rw-r--r--  2.0 unx     9280 b- defN 24-Apr-30 11:13 spark_rapids_pytools/resources/dataproc-configs.json
+-rw-r--r--  2.0 unx     9069 b- defN 24-Apr-30 11:13 spark_rapids_pytools/resources/dataproc_gke-configs.json
+-rw-r--r--  2.0 unx       30 b- defN 24-Apr-30 11:13 spark_rapids_pytools/resources/diagnostic-conf.yaml
+-rw-r--r--  2.0 unx    12779 b- defN 24-Apr-30 11:13 spark_rapids_pytools/resources/emr-configs.json
+-rw-r--r--  2.0 unx     5159 b- defN 24-Apr-30 11:13 spark_rapids_pytools/resources/onprem-configs.json
+-rw-r--r--  2.0 unx    38903 b- defN 24-Apr-30 11:13 spark_rapids_pytools/resources/premium-databricks-azure-catalog.json
+-rw-r--r--  2.0 unx     1517 b- defN 24-Apr-30 11:13 spark_rapids_pytools/resources/profiling-conf.yaml
+-rw-r--r--  2.0 unx     8164 b- defN 24-Apr-30 11:13 spark_rapids_pytools/resources/qualification-conf.yaml
+-rw-r--r--  2.0 unx     7779 b- defN 24-Apr-30 11:13 spark_rapids_pytools/resources/dev/prepackage_mgr.py
+-rw-r--r--  2.0 unx     2195 b- defN 24-Apr-30 11:13 spark_rapids_pytools/resources/dev/process_databricks_azure_pricing.py
+-rw-r--r--  2.0 unx   405769 b- defN 24-Apr-30 11:13 spark_rapids_pytools/resources/qualx/models/xgboost/databricks-aws.json
+-rw-r--r--  2.0 unx   160200 b- defN 24-Apr-30 11:13 spark_rapids_pytools/resources/qualx/models/xgboost/databricks-azure.json
+-rw-r--r--  2.0 unx   795042 b- defN 24-Apr-30 11:13 spark_rapids_pytools/resources/qualx/models/xgboost/dataproc.json
+-rw-r--r--  2.0 unx   361292 b- defN 24-Apr-30 11:13 spark_rapids_pytools/resources/qualx/models/xgboost/dataproc_2.1-orc.json
+-rw-r--r--  2.0 unx   530621 b- defN 24-Apr-30 11:13 spark_rapids_pytools/resources/qualx/models/xgboost/onprem.json
+-rw-r--r--  2.0 unx      669 b- defN 24-Apr-30 11:13 spark_rapids_pytools/resources/templates/dataproc-create_gpu_cluster_script.ms
+-rw-r--r--  2.0 unx      518 b- defN 24-Apr-30 11:13 spark_rapids_pytools/resources/templates/dataproc-run_bootstrap.ms
+-rw-r--r--  2.0 unx      855 b- defN 24-Apr-30 11:13 spark_rapids_pytools/resources/templates/emr-create_gpu_cluster_script.ms
+-rw-r--r--  2.0 unx      537 b- defN 24-Apr-30 11:13 spark_rapids_pytools/resources/templates/emr-run_bootstrap.ms
+-rw-r--r--  2.0 unx      241 b- defN 24-Apr-30 11:13 spark_rapids_pytools/resources/templates/cluster_template/databricks_aws.ms
+-rw-r--r--  2.0 unx      291 b- defN 24-Apr-30 11:13 spark_rapids_pytools/resources/templates/cluster_template/databricks_azure.ms
+-rw-r--r--  2.0 unx      579 b- defN 24-Apr-30 11:13 spark_rapids_pytools/resources/templates/cluster_template/dataproc.ms
+-rw-r--r--  2.0 unx      759 b- defN 24-Apr-30 11:13 spark_rapids_pytools/resources/templates/cluster_template/emr.ms
+-rw-r--r--  2.0 unx       40 b- defN 24-Apr-30 11:13 spark_rapids_pytools/resources/templates/node_template/databricks_aws.ms
+-rw-r--r--  2.0 unx       40 b- defN 24-Apr-30 11:13 spark_rapids_pytools/resources/templates/node_template/databricks_azure.ms
+-rw-r--r--  2.0 unx      293 b- defN 24-Apr-30 11:13 spark_rapids_pytools/resources/templates/node_template/emr.ms
+-rw-r--r--  2.0 unx      630 b- defN 24-Apr-30 11:13 spark_rapids_pytools/wrappers/__init__.py
+-rw-r--r--  2.0 unx    19338 b- defN 24-Apr-30 11:13 spark_rapids_pytools/wrappers/databricks_aws_wrapper.py
+-rw-r--r--  2.0 unx    18795 b- defN 24-Apr-30 11:13 spark_rapids_pytools/wrappers/databricks_azure_wrapper.py
+-rw-r--r--  2.0 unx     9834 b- defN 24-Apr-30 11:13 spark_rapids_pytools/wrappers/dataproc_gke_wrapper.py
+-rw-r--r--  2.0 unx    18774 b- defN 24-Apr-30 11:13 spark_rapids_pytools/wrappers/dataproc_wrapper.py
+-rw-r--r--  2.0 unx    19300 b- defN 24-Apr-30 11:13 spark_rapids_pytools/wrappers/emr_wrapper.py
+-rw-r--r--  2.0 unx    12518 b- defN 24-Apr-30 11:13 spark_rapids_pytools/wrappers/onprem_wrapper.py
+-rw-r--r--  2.0 unx     1008 b- defN 24-Apr-30 11:13 spark_rapids_tools/__init__.py
+-rw-r--r--  2.0 unx     5286 b- defN 24-Apr-30 11:13 spark_rapids_tools/enums.py
+-rw-r--r--  2.0 unx     2099 b- defN 24-Apr-30 11:13 spark_rapids_tools/exceptions.py
+-rw-r--r--  2.0 unx     1167 b- defN 24-Apr-30 11:13 spark_rapids_tools/cloud/__init__.py
+-rw-r--r--  2.0 unx     4759 b- defN 24-Apr-30 11:13 spark_rapids_tools/cloud/cluster.py
+-rw-r--r--  2.0 unx      649 b- defN 24-Apr-30 11:13 spark_rapids_tools/cloud/databricks/__init__.py
+-rw-r--r--  2.0 unx     1808 b- defN 24-Apr-30 11:13 spark_rapids_tools/cloud/databricks/dbcluster.py
+-rw-r--r--  2.0 unx      647 b- defN 24-Apr-30 11:13 spark_rapids_tools/cloud/dataproc/__init__.py
+-rw-r--r--  2.0 unx     2243 b- defN 24-Apr-30 11:13 spark_rapids_tools/cloud/dataproc/dataproccluster.py
+-rw-r--r--  2.0 unx      642 b- defN 24-Apr-30 11:13 spark_rapids_tools/cloud/emr/__init__.py
+-rw-r--r--  2.0 unx     1243 b- defN 24-Apr-30 11:13 spark_rapids_tools/cloud/emr/emrcluster.py
+-rw-r--r--  2.0 unx      645 b- defN 24-Apr-30 11:13 spark_rapids_tools/cloud/onprem/__init__.py
+-rw-r--r--  2.0 unx     1768 b- defN 24-Apr-30 11:13 spark_rapids_tools/cloud/onprem/onpremcluster.py
+-rw-r--r--  2.0 unx      706 b- defN 24-Apr-30 11:13 spark_rapids_tools/cmdli/__init__.py
+-rw-r--r--  2.0 unx    27691 b- defN 24-Apr-30 11:13 spark_rapids_tools/cmdli/argprocessor.py
+-rw-r--r--  2.0 unx    16404 b- defN 24-Apr-30 11:13 spark_rapids_tools/cmdli/tools_cli.py
+-rw-r--r--  2.0 unx     1433 b- defN 24-Apr-30 11:13 spark_rapids_tools/storagelib/__init__.py
+-rw-r--r--  2.0 unx     5549 b- defN 24-Apr-30 11:13 spark_rapids_tools/storagelib/cspfs.py
+-rw-r--r--  2.0 unx    11165 b- defN 24-Apr-30 11:13 spark_rapids_tools/storagelib/csppath.py
+-rw-r--r--  2.0 unx      774 b- defN 24-Apr-30 11:13 spark_rapids_tools/storagelib/adls/__init__.py
+-rw-r--r--  2.0 unx     1658 b- defN 24-Apr-30 11:13 spark_rapids_tools/storagelib/adls/adlsfs.py
+-rw-r--r--  2.0 unx      785 b- defN 24-Apr-30 11:13 spark_rapids_tools/storagelib/adls/adlspath.py
+-rw-r--r--  2.0 unx      751 b- defN 24-Apr-30 11:13 spark_rapids_tools/storagelib/gcs/__init__.py
+-rw-r--r--  2.0 unx     1528 b- defN 24-Apr-30 11:13 spark_rapids_tools/storagelib/gcs/gcsfs.py
+-rw-r--r--  2.0 unx      784 b- defN 24-Apr-30 11:13 spark_rapids_tools/storagelib/gcs/gcspath.py
+-rw-r--r--  2.0 unx      755 b- defN 24-Apr-30 11:13 spark_rapids_tools/storagelib/hdfs/__init__.py
+-rw-r--r--  2.0 unx     1761 b- defN 24-Apr-30 11:13 spark_rapids_tools/storagelib/hdfs/hdfsfs.py
+-rw-r--r--  2.0 unx      784 b- defN 24-Apr-30 11:13 spark_rapids_tools/storagelib/hdfs/hdfspath.py
+-rw-r--r--  2.0 unx      760 b- defN 24-Apr-30 11:13 spark_rapids_tools/storagelib/local/__init__.py
+-rw-r--r--  2.0 unx      865 b- defN 24-Apr-30 11:13 spark_rapids_tools/storagelib/local/localfs.py
+-rw-r--r--  2.0 unx      780 b- defN 24-Apr-30 11:13 spark_rapids_tools/storagelib/local/localpath.py
+-rw-r--r--  2.0 unx      726 b- defN 24-Apr-30 11:13 spark_rapids_tools/storagelib/s3/__init__.py
+-rw-r--r--  2.0 unx     1732 b- defN 24-Apr-30 11:13 spark_rapids_tools/storagelib/s3/s3fs.py
+-rw-r--r--  2.0 unx      776 b- defN 24-Apr-30 11:13 spark_rapids_tools/storagelib/s3/s3path.py
+-rw-r--r--  2.0 unx      653 b- defN 24-Apr-30 11:13 spark_rapids_tools/tools/__init__.py
+-rw-r--r--  2.0 unx     1096 b- defN 24-Apr-30 11:13 spark_rapids_tools/tools/autotuner.py
+-rw-r--r--  2.0 unx    54414 b- defN 24-Apr-30 11:13 spark_rapids_tools/tools/model_xgboost.py
+-rw-r--r--  2.0 unx     4764 b- defN 24-Apr-30 11:13 spark_rapids_tools/tools/speedup_category.py
+-rw-r--r--  2.0 unx     1714 b- defN 24-Apr-30 11:13 spark_rapids_tools/tools/top_candidates.py
+-rw-r--r--  2.0 unx     4081 b- defN 24-Apr-30 11:13 spark_rapids_tools/tools/unsupported_ops_stage_duration.py
+-rw-r--r--  2.0 unx      987 b- defN 24-Apr-30 11:13 spark_rapids_tools/utils/__init__.py
+-rw-r--r--  2.0 unx     4844 b- defN 24-Apr-30 11:13 spark_rapids_tools/utils/propmanager.py
+-rw-r--r--  2.0 unx    12742 b- defN 24-Apr-30 11:13 spark_rapids_tools/utils/util.py
+-rw-r--r--  2.0 unx    21086 b- defN 24-Apr-30 11:13 spark_rapids_user_tools-24.2.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4126 b- defN 24-Apr-30 11:13 spark_rapids_user_tools-24.2.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-30 11:13 spark_rapids_user_tools-24.2.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx      133 b- defN 24-Apr-30 11:13 spark_rapids_user_tools-24.2.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       40 b- defN 24-Apr-30 11:13 spark_rapids_user_tools-24.2.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    13384 b- defN 24-Apr-30 11:13 spark_rapids_user_tools-24.2.4.dist-info/RECORD
+128 files, 3143197 bytes uncompressed, 844187 bytes compressed:  73.1%
```

## zipnote {}

```diff
@@ -201,15 +201,21 @@
 
 Filename: spark_rapids_pytools/resources/templates/cluster_template/dataproc.ms
 Comment: 
 
 Filename: spark_rapids_pytools/resources/templates/cluster_template/emr.ms
 Comment: 
 
-Filename: spark_rapids_pytools/resources/templates/cluster_template/emr_node.ms
+Filename: spark_rapids_pytools/resources/templates/node_template/databricks_aws.ms
+Comment: 
+
+Filename: spark_rapids_pytools/resources/templates/node_template/databricks_azure.ms
+Comment: 
+
+Filename: spark_rapids_pytools/resources/templates/node_template/emr.ms
 Comment: 
 
 Filename: spark_rapids_pytools/wrappers/__init__.py
 Comment: 
 
 Filename: spark_rapids_pytools/wrappers/databricks_aws_wrapper.py
 Comment: 
@@ -336,14 +342,17 @@
 
 Filename: spark_rapids_tools/tools/autotuner.py
 Comment: 
 
 Filename: spark_rapids_tools/tools/model_xgboost.py
 Comment: 
 
+Filename: spark_rapids_tools/tools/speedup_category.py
+Comment: 
+
 Filename: spark_rapids_tools/tools/top_candidates.py
 Comment: 
 
 Filename: spark_rapids_tools/tools/unsupported_ops_stage_duration.py
 Comment: 
 
 Filename: spark_rapids_tools/utils/__init__.py
@@ -351,26 +360,26 @@
 
 Filename: spark_rapids_tools/utils/propmanager.py
 Comment: 
 
 Filename: spark_rapids_tools/utils/util.py
 Comment: 
 
-Filename: spark_rapids_user_tools-24.2.3.dist-info/LICENSE
+Filename: spark_rapids_user_tools-24.2.4.dist-info/LICENSE
 Comment: 
 
-Filename: spark_rapids_user_tools-24.2.3.dist-info/METADATA
+Filename: spark_rapids_user_tools-24.2.4.dist-info/METADATA
 Comment: 
 
-Filename: spark_rapids_user_tools-24.2.3.dist-info/WHEEL
+Filename: spark_rapids_user_tools-24.2.4.dist-info/WHEEL
 Comment: 
 
-Filename: spark_rapids_user_tools-24.2.3.dist-info/entry_points.txt
+Filename: spark_rapids_user_tools-24.2.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: spark_rapids_user_tools-24.2.3.dist-info/top_level.txt
+Filename: spark_rapids_user_tools-24.2.4.dist-info/top_level.txt
 Comment: 
 
-Filename: spark_rapids_user_tools-24.2.3.dist-info/RECORD
+Filename: spark_rapids_user_tools-24.2.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## spark_rapids_pytools/__init__.py

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2023, NVIDIA CORPORATION.
+# Copyright (c) 2023-2024, NVIDIA CORPORATION.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,9 +12,9 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """init file of the spark_rapids_pytools package."""
 
 from spark_rapids_pytools.build import get_version
 
-VERSION = '24.02.3'
+VERSION = '24.02.4'
 __version__ = get_version(VERSION)
```

## spark_rapids_pytools/cloud_api/databricks_aws.py

```diff
@@ -233,19 +233,23 @@
         # construct master node info when cluster is inactive
         if master_nodes_from_conf is None:
             master_node_type_id = self.props.get_value('driver_node_type_id')
             if master_node_type_id is None:
                 raise RuntimeError('Failed to find master node information from cluster properties')
             master_nodes_from_conf = {'node_id': None}
         # construct worker nodes info when cluster is inactive
-        if worker_nodes_from_conf is None:
-            worker_node_type_id = self.props.get_value('node_type_id')
-            if worker_node_type_id is None:
-                raise RuntimeError('Failed to find worker node information from cluster properties')
-            worker_nodes_from_conf = [{'node_id': None} for i in range(num_workers)]
+        executors_cnt = len(worker_nodes_from_conf) if worker_nodes_from_conf else 0
+        if num_workers != executors_cnt:
+            self.logger.warning('Cluster configuration: `executors` count %d does not match the '
+                                '`num_workers` value %d. Using generated names.', executors_cnt,
+                                num_workers)
+            worker_nodes_from_conf = self.generate_node_configurations(num_workers)
+        if num_workers == 0 and self.props.get_value('node_type_id') is None:
+            # if there are no worker nodes and no node_type_id, then we cannot proceed
+            raise RuntimeError('Failed to find worker node information from cluster properties')
         # create workers array
         worker_nodes: list = []
         for worker_node in worker_nodes_from_conf:
             worker_props = {
                 'Id': worker_node['node_id'],
                 'props': JSONPropertiesContainer(prop_arg=worker_node, file_load=False),
                 # set the node region based on the wrapper defined region
```

## spark_rapids_pytools/cloud_api/databricks_azure.py

```diff
@@ -100,22 +100,14 @@
             hw_info_json = mc_info['SysInfo']
             hw_info_ob = SysInfo(num_cpus=hw_info_json['num_cpus'], cpu_mem=hw_info_json['cpu_mem'])
             gpu_info_json = mc_info['GpuInfo']['GPUs'][0]
             gpu_info_obj = GpuHWInfo(num_gpus=gpu_info_json['Count'], gpu_mem=gpu_info_json['MemoryInfo']['SizeInMiB'])
             gpu_scopes[mc_prof] = NodeHWInfo(sys_info=hw_info_ob, gpu_info=gpu_info_obj)
         return gpu_scopes
 
-    def generate_cluster_configuration(self, render_args: dict):
-        executor_names = ','.join([
-            f'{{"node_id": "12345678900{i}"}}'
-            for i in range(render_args['NUM_EXECUTOR_NODES'])
-        ])
-        render_args['EXECUTOR_NAMES'] = f'[{executor_names}]'
-        return super().generate_cluster_configuration(render_args)
-
 
 @dataclass
 class DBAzureCMDDriver(CMDDriverBase):
     """Represents the command interface that will be used by DATABRICKS_AZURE"""
 
     configs: JSONPropertiesContainer = None
     cache_expiration_secs: int = field(default=604800, init=False)  # update the file once a week
@@ -317,19 +309,23 @@
         # construct driver node info when cluster is inactive
         if driver_nodes_from_conf is None:
             driver_node_type_id = self.props.get_value('driver_node_type_id')
             if driver_node_type_id is None:
                 raise RuntimeError('Failed to find driver node information from cluster properties')
             driver_nodes_from_conf = {'node_id': None}
         # construct worker nodes info when cluster is inactive
-        if worker_nodes_from_conf is None:
-            worker_node_type_id = self.props.get_value('node_type_id')
-            if worker_node_type_id is None:
-                raise RuntimeError('Failed to find worker node information from cluster properties')
-            worker_nodes_from_conf = [{'node_id': None} for i in range(num_workers)]
+        executors_cnt = len(worker_nodes_from_conf) if worker_nodes_from_conf else 0
+        if num_workers != executors_cnt:
+            self.logger.warning('Cluster configuration: `executors` count %d does not match the '
+                                '`num_workers` value %d. Using generated names.', executors_cnt,
+                                num_workers)
+            worker_nodes_from_conf = self.generate_node_configurations(num_workers)
+        if num_workers == 0 and self.props.get_value('node_type_id') is None:
+            # if there are no worker nodes and no node_type_id, then we cannot proceed
+            raise RuntimeError('Failed to find worker node information from cluster properties')
         # create workers array
         worker_nodes: list = []
         for worker_node in worker_nodes_from_conf:
             worker_props = {
                 'Id': worker_node['node_id'],
                 'props': JSONPropertiesContainer(prop_arg=worker_node, file_load=False),
                 # set the node region based on the wrapper defined region
```

## spark_rapids_pytools/cloud_api/dataproc.py

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 
 """Implementation specific to Dataproc"""
 
 import json
 from dataclasses import dataclass, field
-from typing import Any, List
+from typing import Any, List, Union
 
 from spark_rapids_tools import CspEnv
 from spark_rapids_pytools.cloud_api.dataproc_job import DataprocLocalRapidsJob
 from spark_rapids_pytools.cloud_api.gstorage import GStorageDriver
 from spark_rapids_pytools.cloud_api.sp_types import PlatformBase, CMDDriverBase, \
     ClusterBase, ClusterNode, SysInfo, GpuHWInfo, SparkNodeType, ClusterState, GpuDevice, \
     NodeHWInfo, ClusterGetAccessor
@@ -159,16 +159,14 @@
         # TODO: Currently only single series is supported. Change this to a loop when using multiple series.
         series_name, unit_info = list(executors_from_config.items())[0]
         if cores_per_executor in unit_info['vCPUs']:
             return f'{series_name}-{cores_per_executor}'
         return None
 
     def generate_cluster_configuration(self, render_args: dict):
-        executor_names = ','.join([f'"test-node-e{i}"' for i in range(render_args['NUM_EXECUTOR_NODES'])])
-        render_args['EXECUTOR_NAMES'] = f'[{executor_names}]'
         image_version = self.configs.get_value('clusterInference', 'defaultImage')
         render_args['IMAGE'] = f'"{image_version}"'
         render_args['ZONE'] = f'"{self.cli.get_zone()}"'
         return super().generate_cluster_configuration(render_args)
 
 
 @dataclass
@@ -407,15 +405,22 @@
 
     def _init_nodes(self):
         # assume that only one master node
         master_nodes_from_conf = self.props.get_value('config', 'masterConfig', 'instanceNames')
         raw_worker_prop = self.props.get_value_silent('config', 'workerConfig')
         worker_nodes: list = []
         if raw_worker_prop:
-            worker_nodes_from_conf = self.props.get_value('config', 'workerConfig', 'instanceNames')
+            worker_cnt = self.props.get_value('config', 'workerConfig', 'numInstances')
+            worker_nodes_from_conf = self.props.get_value_silent('config', 'workerConfig', 'instanceNames')
+            instance_names_cnt = len(worker_nodes_from_conf) if worker_nodes_from_conf else 0
+            if worker_cnt != instance_names_cnt:
+                self.logger.warning('Cluster configuration: `instanceNames` count %d does not '
+                                    'match the `numInstances` value %d. Using generated names.',
+                                    instance_names_cnt, worker_cnt)
+                worker_nodes_from_conf = self.generate_node_configurations(worker_cnt)
             # create workers array
             for worker_node in worker_nodes_from_conf:
                 worker_props = {
                     'name': worker_node,
                     'props': JSONPropertiesContainer(prop_arg=raw_worker_prop, file_load=False),
                     # set the node zone based on the wrapper defined zone
                     'zone': self.zone
@@ -532,14 +537,21 @@
             'WORKERS_COUNT': self.get_workers_count(),
             'WORKERS_MACHINE': worker_node.instance_type,
             'LOCAL_SSD': 2,
             'GPU_DEVICE': gpu_device_hash.get(gpu_device),
             'GPU_PER_WORKER': gpu_per_machine
         }
 
+    def _generate_node_configuration(self, render_args: dict = None) -> Union[str, dict]:
+        """
+        Overrides to provide the cluster node configuration which is node name
+        in case of Dataproc.
+        """
+        return 'test-node-e'
+
 
 @dataclass
 class DataprocSavingsEstimator(SavingsEstimator):
     """
     A class that calculates the savings based on Dataproc price provider
     """
     def _calculate_group_cost(self, cluster_inst: ClusterGetAccessor, node_type: SparkNodeType):
```

## spark_rapids_pytools/cloud_api/emr.py

```diff
@@ -335,26 +335,32 @@
     def __create_ec2_list_by_group(self, group_arg):
         if isinstance(group_arg, InstanceGroup):
             group_obj = group_arg
             group_id = group_arg.id
         else:
             group_id = group_arg
             group_obj = None
+        render_args = {
+            'INSTANCE_GROUP_ID': f'"{group_id}"',
+            'INSTANCE_TYPE': f'"{group_obj.instance_type}"'
+        }
         if self.is_inferred:
-            # If cluster settings are inferred, create a list of instances with default configuration
-            render_args = {
-                'INSTANCE_GROUP_ID': f'"{group_id}"',
-                'INSTANCE_TYPE': f'"{group_obj.instance_type}"'
-            }
-            node_config = json.loads(self.generate_node_configuration(render_args))
-            instances_list = [node_config for _ in range(group_obj.count)]
+            # If the instance is inferred, generate a default list of node configurations
+            instances_list = self.generate_node_configurations(group_obj.count, render_args)
         else:
             query_args = {'instance-group-id': group_id}
-            raw_instance_list = self.cli.exec_platform_list_cluster_instances(self, query_args=query_args)
-            instances_list = json.loads(raw_instance_list).get('Instances')
+            try:
+                # Fetch cluster instances based on instance group id
+                raw_instance_list = self.cli.exec_platform_list_cluster_instances(self, query_args=query_args)
+                instances_list = json.loads(raw_instance_list).get('Instances')
+            except Exception:  # pylint: disable=broad-except
+                # If instance list creation fails, generate a default list of node configurations
+                self.logger.error('Failed to create configurations for %s instances in group %s. '
+                                  'Using generated names.', group_obj.count, group_id)
+                instances_list = self.generate_node_configurations(group_obj.count, render_args)
         ec2_instances = []
         for raw_inst in instances_list:
             parsed_state = raw_inst['Status']['State']
             ec2_instance = Ec2Instance(
                 id=raw_inst['Id'],
                 ec2_instance_id=raw_inst['Ec2InstanceId'],
                 dns_name=raw_inst['PublicDnsName'],
```

## spark_rapids_pytools/cloud_api/sp_types.py

```diff
@@ -1163,18 +1163,25 @@
 
     def generate_bootstrap_script(self, overridden_args: dict = None) -> str:
         platform_name = CspEnv.pretty_print(self.platform.type_id)
         template_path = Utils.resource_path(f'templates/{platform_name}-run_bootstrap.ms')
         render_args = self._set_render_args_bootstrap_template(overridden_args)
         return TemplateGenerator.render_template_file(template_path, render_args)
 
-    def generate_node_configuration(self, render_args: dict) -> str:
+    def _generate_node_configuration(self, render_args: dict) -> Union[str, dict]:
         platform_name = CspEnv.pretty_print(self.platform.type_id)
-        template_path = Utils.resource_path(f'templates/cluster_template/{platform_name}_node.ms')
-        return TemplateGenerator.render_template_file(template_path, render_args)
+        template_path = Utils.resource_path(f'templates/node_template/{platform_name}.ms')
+        return json.loads(TemplateGenerator.render_template_file(template_path, render_args))
+
+    def generate_node_configurations(self, num_executors: int, render_args: dict = None) -> list:
+        """
+        Generates a list of node configurations for the given number of executors.
+        """
+        node_config = self._generate_node_configuration(render_args)
+        return [node_config for _ in range(num_executors)]
 
 
 @dataclass
 class ClusterReshape(ClusterGetAccessor):
     """
     A class that handles reshaping of the given cluster.
     It takes argument a cluster object and callable methods that defines
```

## spark_rapids_pytools/rapids/qualification.py

```diff
@@ -10,15 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Implementation class representing wrapper around the RAPIDS acceleration Qualification tool."""
 
-import textwrap
 from dataclasses import dataclass, field
 from math import ceil
 from typing import Any, List, Callable
 
 import numpy as np
 import pandas as pd
 from tabulate import tabulate
@@ -28,14 +27,15 @@
 from spark_rapids_pytools.common.sys_storage import FSUtil
 from spark_rapids_pytools.common.utilities import Utils, TemplateGenerator
 from spark_rapids_pytools.pricing.price_provider import SavingsEstimator
 from spark_rapids_pytools.rapids.rapids_job import RapidsJobPropContainer
 from spark_rapids_pytools.rapids.rapids_tool import RapidsJarTool
 from spark_rapids_tools.enums import QualFilterApp, QualGpuClusterReshapeType, QualEstimationModel
 from spark_rapids_tools.tools.model_xgboost import predict
+from spark_rapids_tools.tools.speedup_category import SpeedupCategory
 from spark_rapids_tools.tools.top_candidates import TopCandidates
 from spark_rapids_tools.tools.unsupported_ops_stage_duration import UnsupportedOpsStageDuration
 from spark_rapids_tools.utils.util import Utilities
 
 
 @dataclass
 class QualificationSummary:
@@ -690,16 +690,21 @@
             return QualificationSummary(comments=self.__generate_mc_types_conversion_report())
 
         unsupported_ops_obj = UnsupportedOpsStageDuration(self.ctxt.get_value('local', 'output',
                                                                               'unsupportedOperators'))
         # Calculate unsupported operators stage duration before grouping
         all_apps = unsupported_ops_obj.prepare_apps_with_unsupported_stages(all_apps, unsupported_ops_df)
         apps_pruned_df = self.__remap_columns_and_prune(all_apps)
+        speedup_category_ob = SpeedupCategory(self.ctxt.get_value('local', 'output', 'speedupCategories'))
+        # Calculate the speedup category column
+        apps_pruned_df = speedup_category_ob.build_category_column(apps_pruned_df)
         apps_pruned_df.to_csv(output_files_info['full']['path'], float_format='%.2f')
         apps_grouped_df, group_notes = self.__group_apps_by_name(apps_pruned_df)
+        # Recalculate the speedup category column after grouping
+        apps_grouped_df = speedup_category_ob.build_category_column(apps_grouped_df)
         recommended_apps = self.__get_recommended_apps(apps_grouped_df)
         # if the gpu_reshape_type is set to JOB then, then we should ignore recommended apps
         speedups_irrelevant_flag = self.__recommendation_is_non_standard()
         reshaped_notes = self.__generate_cluster_shape_report()
         report_comments = [group_notes] if group_notes else []
         if reshaped_notes:
             report_comments.append(reshaped_notes)
@@ -759,21 +764,25 @@
             # summary columns depend on the type of the generated report
             selected_cols = self.ctxt.get_value('local', 'output', 'summaryColumns',
                                                 f'savingsReportEnabled{str(savings_report_enabled)}')
             # check if any filters apply
             filter_recommendation_enabled = self.ctxt.get_ctxt('filterApps') == QualFilterApp.SPEEDUPS
             filter_pos_enabled = self.ctxt.get_ctxt('filterApps') == QualFilterApp.SAVINGS
             filter_top_candidate_enabled = self.ctxt.get_ctxt('filterApps') == QualFilterApp.TOP_CANDIDATES
+            squeeze_header_enabled = self.ctxt.get_value('toolOutput', 'stdout', 'summaryReport', 'compactWidth')
+            header_width = self.ctxt.get_value('toolOutput', 'stdout', 'summaryReport', 'columnWidth')
 
             if filter_top_candidate_enabled:
                 # TODO: Ideally we should create instance of TopCandidates as class variable using the filter apps flag.
                 #  This should be refactored along with entire filter apps logic to use more object-oriented design.
                 top_candidates_obj = TopCandidates(self.ctxt.get_value('local', 'output', 'topCandidates'))
                 filtered_apps = top_candidates_obj.filter_apps(raw_df)
-                return top_candidates_obj.prepare_output(filtered_apps)
+                result_df = top_candidates_obj.prepare_output(filtered_apps)
+                # squeeze the header titles if enabled
+                return Utilities.squeeze_df_header(result_df, header_width) if squeeze_header_enabled else result_df
 
             if self.__recommendation_is_non_standard():
                 # During processing of arguments phase, we verified that the filter does not conflict
                 # with the shape recommendation
                 raw_df = self.__remap_cols_for_shape_type(raw_df,
                                                           selected_cols,
                                                           self.ctxt.get_ctxt('gpuClusterShapeRecommendation'))
@@ -805,23 +814,15 @@
                 # convert to seconds
                 for column in df_row[[col for col in df_row.columns if 'Duration' in col]]:
                     df_row[column] = df_row[column].div(1000).round(2)
             # change the header to include time unit
             df_row.columns = df_row.columns.str.replace('Duration',
                                                         f'Duration{time_unit}', regex=False)
             # squeeze the header titles if enabled
-            if self.ctxt.get_value('toolOutput', 'stdout', 'summaryReport', 'compactWidth'):
-                col_w_conf = self.ctxt.get_value('toolOutput', 'stdout', 'summaryReport', 'columnWidth')
-                for column in df_row.columns:
-                    if len(column) > col_w_conf:
-                        new_column_name = textwrap.fill(column, col_w_conf, break_long_words=False)
-                        if new_column_name != column:
-                            df_row.columns = df_row.columns.str.replace(column,
-                                                                        new_column_name, regex=False)
-            return df_row
+            return Utilities.squeeze_df_header(df_row, header_width) if squeeze_header_enabled else df_row
 
         if not self._evaluate_rapids_jar_tool_output_exist():
             return
 
         rapids_output_dir = self.ctxt.get_rapids_output_folder()
         rapids_summary_file = FSUtil.build_path(rapids_output_dir,
                                                 self.ctxt.get_value('toolOutput', 'csv', 'summaryReport', 'fileName'))
```

## spark_rapids_pytools/resources/databricks_azure-configs.json

### Pretty-printed

 * *Similarity: 0.9982638888888888%*

 * *Differences: {"'dependencies'": "{'deployMode': {'LOCAL': {1: {'uri': "*

 * *                   "'https://repo1.maven.org/maven2/org/apache/hadoop/hadoop-azure/3.3.4/hadoop-azure-3.3.4.jar', "*

 * *                   "'md5': '1ec4cbd59548412010fe1515070eef73', 'sha1': "*

 * *                   "'a23f621bca9b2100554150f6b0b521f94b8b419e', 'size': 574116}}}}"}*

```diff
@@ -41,20 +41,20 @@
                     "relativePath": "jars/*",
                     "sha512": "8883c67e0a138069e597f3e7d4edbbd5c3a565d50b28644aad02856a1ec1da7cb92b8f80454ca427118f69459ea326eaa073cf7b1a860c3b796f4b07c2101319",
                     "size": 400395283,
                     "type": "archive",
                     "uri": "https://archive.apache.org/dist/spark/spark-3.5.0/spark-3.5.0-bin-hadoop3.tgz"
                 },
                 {
-                    "md5": "0fb8b8e565fd920fb809220cb2cc5ee7",
+                    "md5": "1ec4cbd59548412010fe1515070eef73",
                     "name": "Hadoop Azure",
-                    "sha1": "24425e7fad3a302715cefd570a0f4bdf3f50bc8e",
-                    "size": 609646,
+                    "sha1": "a23f621bca9b2100554150f6b0b521f94b8b419e",
+                    "size": 574116,
                     "type": "jar",
-                    "uri": "https://repo1.maven.org/maven2/org/apache/hadoop/hadoop-azure/3.3.6/hadoop-azure-3.3.6.jar"
+                    "uri": "https://repo1.maven.org/maven2/org/apache/hadoop/hadoop-azure/3.3.4/hadoop-azure-3.3.4.jar"
                 }
             ],
             "SPARK333-LOCAL": [
                 {
                     "name": "Apache Spark",
                     "relativePath": "jars/*",
                     "sha512": "ebf79c7861f3120d5ed9465fdd8d5302a734ff30713a0454b714bbded7ab9f218b3108dc46a5de4cc2102c86e7be53908f84d2c7a19e59bc75880766eeefeef9",
```

## spark_rapids_pytools/resources/qualification-conf.yaml

```diff
@@ -209,51 +209,54 @@
           - 'Stage ID'
         sum:
           - 'App ID'
           - 'App Duration'
       resultColumnName: 'Unsupported Operators Stage Duration'
       percentResultColumnName: 'Unsupported Operators Stage Duration Percent'
     topCandidates:
+      categoryColumnName: 'Estimated GPU Speedup Category'
       outputColumns:
         - 'App ID'
         - 'App Name'
-        - 'App Duration'
-        - 'Estimated GPU Speedup'
-        - 'Unsupported Operators Stage Duration Percent'
+        - 'Estimated GPU Speedup Category'
+      eligibleCategories:
+        - 'Small'
+        - 'Medium'
+        - 'Large'
       sortingColumns:
         - 'Estimated GPU Speedup'
         - 'Unsupported Operators Stage Duration Percent'
       joinColumns:
         - 'App ID'
         - 'App Name'
         - 'App Duration'
-      ranges:
-          - columnName: 'Estimated GPU Speedup'
-            lowerBound: 1.3
-            upperBound: 1000000.0
-          - columnName: 'Unsupported Operators Stage Duration Percent'
-            lowerBound: 0.0
-            upperBound: 25.0
-      output: # Configs related to output
-        columns:
-          - 'App ID'
-          - 'App Name'
-          - 'Estimated GPU Speedup'
-        remap:
-          - columnName: 'Estimated GPU Speedup'
-            recommendationRanges:
-              - title: 'Small'
-                lowerBound: 1.3
-                upperBound: 2.0
-              - title: 'Medium'
-                lowerBound: 2.0
-                upperBound: 3.0
-              - title: 'Large'
-                lowerBound: 3.0
-                upperBound: 1000000.0
+    speedupCategories:
+      speedupColumnName: 'Estimated GPU Speedup'
+      categoryColumnName: 'Estimated GPU Speedup Category'
+      categories:
+        - title: 'Not Applicable'
+          lowerBound: -1000000.0
+          upperBound: 1.3
+        - title: 'Small'
+          lowerBound: 1.3
+          upperBound: 2.0
+        - title: 'Medium'
+          lowerBound: 2.0
+          upperBound: 3.0
+        - title: 'Large'
+          lowerBound: 3.0
+          upperBound: 1000000.0
+      eligibilityConditions:
+        - columnName: 'Estimated GPU Speedup'
+          lowerBound: 1.3
+          upperBound: 1000000.0
+        - columnName: 'Unsupported Operators Stage Duration Percent'
+          lowerBound: 0.0
+          upperBound: 25.0
+      defaultCategory: 'Not Recommended'
     predictionModel:
       outputDirectory: 'xgboost_predictions'
       files:
         perSql:
           name: 'per_sql.csv'
         perApp:
           name: 'per_app.csv'
```

## spark_rapids_pytools/resources/templates/cluster_template/databricks_azure.ms

```diff
@@ -1,12 +1,11 @@
 {
   "cluster_id": "1234-5678-1234567",
   "driver": {
     "node_id": "1234567890"
   },
-  "executors": {{{ EXECUTOR_NAMES }}},
   "cluster_name": "default-cluster-name",
   "driver_node_type_id": {{{ DRIVER_INSTANCE }}},
   "node_type_id": {{{ EXECUTOR_INSTANCE }}},
   "num_workers": {{ NUM_EXECUTOR_NODES }},
   "state": "TERMINATED"
 }
```

## spark_rapids_pytools/resources/templates/cluster_template/dataproc.ms

```diff
@@ -9,15 +9,14 @@
       "instanceNames": [
         "test-node-d"
       ],
       "machineTypeUri": {{{ DRIVER_INSTANCE }}},
       "numInstances": {{ NUM_DRIVER_NODES }}
     },
     "workerConfig": {
-      "instanceNames": {{{ EXECUTOR_NAMES }}},
       "machineTypeUri": {{{ EXECUTOR_INSTANCE }}},
       "numInstances": {{ NUM_EXECUTOR_NODES }}
     },
     "softwareConfig": {
         "imageVersion": {{{ IMAGE }}}
     }
   },
```

## spark_rapids_tools/tools/top_candidates.py

```diff
@@ -11,16 +11,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Implementation class for Top Candidates logic."""
 
 from dataclasses import dataclass, field
-from typing import Optional
-from functools import partial
 
 import pandas as pd
 
 
 @dataclass
 class TopCandidates:
     """
@@ -28,51 +26,20 @@
     """
     props: dict = field(default=None, init=True)
 
     def filter_apps(self, all_apps: pd.DataFrame) -> pd.DataFrame:
         """
         Generic method to filter applications based on criteria
         """
-        filtered_apps = all_apps[all_apps.apply(self.__filter_single_row, axis=1)]
-        # Select output columns and sort
-        output_columns = self.props.get('outputColumns')
-        sorting_columns = self.props.get('sortingColumns')
-        return filtered_apps[output_columns].sort_values(by=sorting_columns, ascending=False)
-
-    def __filter_single_row(self, single_row: pd.Series) -> bool:
-        """
-        Used to create a filter for based on specified ranges.
-        Example:
-        self.props['ranges'] = [
-            {'columnName': 'colA', 'lowerBound': 18, 'upperBound': 30},
-            {'columnName': 'colB', 'lowerBound': 70, 'upperBound': 100}
-        ]
-        single_row = pd.Series({'colA': 25, 'colB': 85})
-        The function will return True because the colA (25) is within the range (18-30)
-        and the colB (85) is within the range (70-100).
-        """
-        for criteria in self.props.get('ranges'):
-            col_value = single_row[criteria.get('columnName')]
-            if not criteria.get('lowerBound') <= col_value <= criteria.get('upperBound'):
-                return False
-        return True
+        category_col_name = self.props.get('categoryColumnName')
+        eligible_categories = self.props.get('eligibleCategories')
+        # Filter applications based on categories
+        return all_apps[all_apps[category_col_name].isin(eligible_categories)]
 
     def prepare_output(self, all_apps: pd.DataFrame) -> pd.DataFrame:
         """
         Generic method to transform applications for the output
         """
-        output_props = self.props.get('output')
-
-        # Function to remap column values based on recommended ranges
-        def remap_column(col_value, recommended_ranges: dict) -> Optional[str]:
-            for s_range in recommended_ranges:
-                if s_range['lowerBound'] <= col_value < s_range['upperBound']:
-                    return s_range['title']
-            return None
-
-        # Iterate over each entry and apply remapping to respective columns
-        for remap_entry in output_props.get('remap', []):
-            column_name = remap_entry.get('columnName')
-            recommendation_ranges = remap_entry.get('recommendationRanges')
-            remap_func = partial(remap_column, recommended_ranges=recommendation_ranges)
-            all_apps[column_name] = all_apps[column_name].apply(remap_func)
-        return all_apps[output_props.get('columns', [])]
+        output_columns = self.props.get('outputColumns')
+        sorting_columns = self.props.get('sortingColumns')
+        # Sort columns and select output columns
+        return all_apps.sort_values(by=sorting_columns, ascending=False)[output_columns]
```

## spark_rapids_tools/utils/util.py

```diff
@@ -15,14 +15,15 @@
 """Utility and helper methods"""
 
 import os
 import pathlib
 import re
 import ssl
 import sys
+import textwrap
 import urllib
 import xml.etree.ElementTree as elem_tree
 from functools import reduce
 from operator import getitem
 from typing import Any, Optional, ClassVar
 
 import certifi
@@ -294,7 +295,17 @@
                 'rapidsThreads': num_threads_unit
             },
             'profiling': {
                 'jvmMaxHeapSize': prof_heap,
                 'rapidsThreads': prof_threads
             }
         }
+
+    @classmethod
+    def squeeze_df_header(cls, df_row: pd.DataFrame, header_width: int) -> pd.DataFrame:
+        for column in df_row.columns:
+            if len(column) > header_width:
+                new_column_name = textwrap.fill(column, header_width, break_long_words=False)
+                if new_column_name != column:
+                    df_row.columns = df_row.columns.str.replace(column,
+                                                                new_column_name, regex=False)
+        return df_row
```

## Comparing `spark_rapids_user_tools-24.2.3.dist-info/LICENSE` & `spark_rapids_user_tools-24.2.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `spark_rapids_user_tools-24.2.3.dist-info/METADATA` & `spark_rapids_user_tools-24.2.4.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-rapids-user-tools
-Version: 24.2.3
+Version: 24.2.4
 Summary: A simple wrapper process around cloud service providers to run tools for the RAPIDS Accelerator for Apache Spark.
 Author-email: NVIDIA Corporation <spark-rapids-support@nvidia.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

## Comparing `spark_rapids_user_tools-24.2.3.dist-info/RECORD` & `spark_rapids_user_tools-24.2.4.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-spark_rapids_pytools/__init__.py,sha256=lXRJXVOfSrh0nV-M-Ys6VkqXLnb-r3ag83kUH5gje08,750
+spark_rapids_pytools/__init__.py,sha256=qoTSJhmjwxxcpcOdHC7OHvvKIVCVRntQHvJIIi92myI,755
 spark_rapids_pytools/build.py,sha256=Ej4Pc2jPIyeVUUOyC67ZMc6Tj90NKj0DrXyniJc0FnY,992
 spark_rapids_pytools/wrapper.py,sha256=0MurKLBYvNb3UVHy6BUdAAVjEZMRkinN6Us0I0hNn7k,1450
 spark_rapids_pytools/cloud_api/__init__.py,sha256=NQSbmxhLzvnZrf4ltpgCLMjCEERPv5QoYo62LEdDBs8,646
 spark_rapids_pytools/cloud_api/azurestorage.py,sha256=yuFk7H5Y8aY0H5dOmeJBS03uhgS2nah5v0Kw2GJzDnE,8507
-spark_rapids_pytools/cloud_api/databricks_aws.py,sha256=Xm5PbnoiLst7lL92gHAotFRx_MrhfrfxDm8PCPk0C2A,16172
+spark_rapids_pytools/cloud_api/databricks_aws.py,sha256=bS7mULmMYC2l8xfAsE4WBZ2KOYDEqoO_lQyVIke_VuQ,16540
 spark_rapids_pytools/cloud_api/databricks_aws_job.py,sha256=ZNYM2pa8fObRhc9c9VcqCT6HxGJNfHeFhdoVYNek51E,1268
-spark_rapids_pytools/cloud_api/databricks_azure.py,sha256=PlZOunO9dKiVzdRLZHvhtkbIJeGgDcEUm654OiB_RKs,19896
+spark_rapids_pytools/cloud_api/databricks_azure.py,sha256=_JJpeSsVhjrc2kyAEklqcQmUtxXTcAkEd_r4-HMyu3M,19913
 spark_rapids_pytools/cloud_api/databricks_azure_job.py,sha256=u-wOcJXRyFCuEsXQypW8O09O5YQ2pt_gNcOlQjwpXYE,2428
-spark_rapids_pytools/cloud_api/dataproc.py,sha256=bWrQJjQ8r-jKU4dYic_7PAdKesgIOe9XwEomFxH3wQc,26700
+spark_rapids_pytools/cloud_api/dataproc.py,sha256=Ja_tpQD6Mzsaita-1Ebz3pkII2mD2dcDTkQoNiXjfvA,27376
 spark_rapids_pytools/cloud_api/dataproc_gke.py,sha256=3Sggx2S_7uw3XXws5NFPgIccb1fvITx-AFDe9-eSZTM,8455
 spark_rapids_pytools/cloud_api/dataproc_gke_job.py,sha256=GYbpZ5XRkWkmew82W6VcXfR0th5cy_3vSbqSBMPLGrk,929
 spark_rapids_pytools/cloud_api/dataproc_job.py,sha256=VMBbFjUfzF7ZZtwWI5dsc8exiZwkARHQIeWIcY3wZNs,922
-spark_rapids_pytools/cloud_api/emr.py,sha256=BpS67okt4YotuTnjccUGysV1pxn1frfHJD9ViIrw028,22845
+spark_rapids_pytools/cloud_api/emr.py,sha256=YcExhOh98LHxjJ9Nr4Dc2oIWbFRJ8wKAmkGsA5b6r1Q,23288
 spark_rapids_pytools/cloud_api/emr_job.py,sha256=-6VA4HV34BVm_CoxaSh13pDb1pyeYHoRbzWVQFfuT0o,1252
 spark_rapids_pytools/cloud_api/gstorage.py,sha256=88IzLWOzEphCETGQaVN3_U7wUD0M2doDy759WQmNoJI,4939
 spark_rapids_pytools/cloud_api/onprem.py,sha256=KvLe5TEjTVMmPU9Ocb7ptiSUZvir28cNL9AJMy_jEbc,13941
 spark_rapids_pytools/cloud_api/s3storage.py,sha256=cFqZETxWt_3Yagk3UlQt65pM4A0qb6idpbi8kUOK5pE,4055
-spark_rapids_pytools/cloud_api/sp_types.py,sha256=zc1l8peAIHc-MJK6FCH1bsi3N2Hc3QZvD7jVVnzygD8,52987
+spark_rapids_pytools/cloud_api/sp_types.py,sha256=IAxyzyYNBy0jYAibLSgP7D0pEExrLQjwAB3S7TmM4aY,53339
 spark_rapids_pytools/common/__init__.py,sha256=A8h0t211p8t_aATYiwCLWTwTy564kCcZp-HTWKiO4u8,658
 spark_rapids_pytools/common/cluster_inference.py,sha256=s1dhheSeup5OQq_sJ7PEVL5-m4stnqBgnZLbhODGZ74,3927
 spark_rapids_pytools/common/exceptions.py,sha256=CK9PF75hSrRh6qaz0aKoiNqaU78E8OfiNydZ4i6WgoM,978
 spark_rapids_pytools/common/prop_manager.py,sha256=GI4vz5Vjw2Lz0RXJXYKs3o_AwepMNql0klTJ_VhDNkQ,5119
 spark_rapids_pytools/common/sys_storage.py,sha256=knE0ZLCLToFo7r5XfIf0cc6L7rJ2vl2UfcWpMriYRAw,20141
 spark_rapids_pytools/common/utilities.py,sha256=puotuvbPIC5K9N4-E5VgJFZU4f-qpfXoAOz7DF8YzNE,14532
 spark_rapids_pytools/pricing/__init__.py,sha256=Y_IWTtiKulkkoC84SLS8LkRWTi393zeUGHaNogZfOSg,659
@@ -30,48 +30,50 @@
 spark_rapids_pytools/pricing/dataproc_pricing.py,sha256=4-RuYxW9V0K0mqj2mqCJsKEUbvxPXHCwF4AsK1z6UXE,4247
 spark_rapids_pytools/pricing/emr_pricing.py,sha256=9KdPjKSC4RFAg40ZpMHbrVEUXaFWDd9unNNaOcdpROw,4747
 spark_rapids_pytools/pricing/price_provider.py,sha256=fUOt34BZeAvsC3WDTnRRCBwchVV0sfkRJT5aGNQ_sxg,6698
 spark_rapids_pytools/rapids/__init__.py,sha256=xiYk9b76AV_v3fEELcYzXCUPvXQhCD687eJ5RCYQW7M,666
 spark_rapids_pytools/rapids/bootstrap.py,sha256=V2-inHdECJYpPXQMuO1KhWvYIGF8M2fYq7fcXVnwAWo,6026
 spark_rapids_pytools/rapids/diagnostic.py,sha256=481_MjrbCtrpS8RJLyM0MgMFRxVkXqToMFHhriQS26k,6780
 spark_rapids_pytools/rapids/profiling.py,sha256=fnDo7I1kv22iaUChompMMNW6ywlCdTtKEYxTVTZabMg,10472
-spark_rapids_pytools/rapids/qualification.py,sha256=abqtLNIJVX-BzSyjq7FQ8vlNbrXg9CHHqilrX38WOp0,58920
+spark_rapids_pytools/rapids/qualification.py,sha256=Ij2uIW75wnDiMtPQX_Vp9nTW8fNh2PBTb4LfuBFh3iE,59208
 spark_rapids_pytools/rapids/rapids_job.py,sha256=HId6wvfXwsPVb26meKGn_C1PcS68NGT41uNgZZx6vTY,5739
 spark_rapids_pytools/rapids/rapids_tool.py,sha256=4MrN3xLQP4XMOADPXKA2zEynzlQLWTE8kDnGpuQ3Mxg,43836
 spark_rapids_pytools/rapids/tool_ctxt.py,sha256=UFHyD_XnOG80Jj1GQX-MFHAhF5mP9Hth3Fe9wudQqks,8938
 spark_rapids_pytools/resources/bootstrap-conf.yaml,sha256=rqjuQ2gwyOmavD3c8q_mWM5qXCxThczg2ldyjdGwgw4,273
 spark_rapids_pytools/resources/cluster-configs.yaml,sha256=5gklmC6mR1EeKvpeL-m0zrFJGaQnDiBGeXRFGdCoXqM,1073
 spark_rapids_pytools/resources/collect.sh,sha256=53oPX45kkx2sK3EA-CPcPD7GXkv7p6r54uNyyjwzW74,5816
 spark_rapids_pytools/resources/databricks-premium-catalog.json,sha256=XBptMDeu7Abbrv6xC4C1oDuMuEIqnrGEqwrhJFutLJM,30566
 spark_rapids_pytools/resources/databricks_aws-configs.json,sha256=YBotFq2bi2rQV1iUna0aNXVhiXp8VHLV_MpTjSIgvbw,13549
-spark_rapids_pytools/resources/databricks_azure-configs.json,sha256=Zv_SahYEnfVCR2PyiwvqH8FI2AtRGShOGRI_sXwdySg,11272
+spark_rapids_pytools/resources/databricks_azure-configs.json,sha256=kya7pJ59A-ZDyWAnVlozt9WHrcH4E40A0zFkGwCSkz8,11272
 spark_rapids_pytools/resources/dataproc-configs.json,sha256=GxhdwkyyDseM1jiqs25gEZqJzImJcwPCSd5xl3Mqt6U,9280
 spark_rapids_pytools/resources/dataproc_gke-configs.json,sha256=qp5sd3rPC8PUTZAr1gOEM4DV_ZnZ13bnkQLj9PFkx8A,9069
 spark_rapids_pytools/resources/diagnostic-conf.yaml,sha256=vS32UyRhj5ox2MZ8-6EgMjXEWlGeaw9izYiAdAoWpfE,30
 spark_rapids_pytools/resources/emr-configs.json,sha256=2YFA1VCj6oetMNTTFjsAsqxxDV9U2IkYk8RI_EI0i0A,12779
 spark_rapids_pytools/resources/onprem-configs.json,sha256=LQ2uszvZ0nDpK2HhoAUzsHj-5S-tFeXM4kinJLbkiM0,5159
 spark_rapids_pytools/resources/premium-databricks-azure-catalog.json,sha256=KGxUoiNPVTVzQaR3SN_FV9PH80fEnp6JnMhnv2YFOBY,38903
 spark_rapids_pytools/resources/profiling-conf.yaml,sha256=BqY12DJ1tkXDJZLITCaODyGx2KWEWNFmC3COFhIS21o,1517
-spark_rapids_pytools/resources/qualification-conf.yaml,sha256=OKN17xO7K_RsyjMTe4hPX300kyVLKTjEcF4tIuDy8Yc,8101
+spark_rapids_pytools/resources/qualification-conf.yaml,sha256=Nu-EC9TjaahWm4eVcCsY5RQmyO2I28k-73bN5bQv2NM,8164
 spark_rapids_pytools/resources/dev/prepackage_mgr.py,sha256=pHORWIxdDWTWvSi4poTDbPdtd-zY-_46wteqNQULlZo,7779
 spark_rapids_pytools/resources/dev/process_databricks_azure_pricing.py,sha256=lmXGoTdrwdrhh8UO7DSL-kgbLOJP1X0kgJPq6cJfF3U,2195
 spark_rapids_pytools/resources/qualx/models/xgboost/databricks-aws.json,sha256=ZCFDXaUBzW-0RMjzVbUg5RQARR2w21MfeRmMIJfA3oU,405769
 spark_rapids_pytools/resources/qualx/models/xgboost/databricks-azure.json,sha256=4GLZ4J6cV77PnmjQpSlFAJWYXkhqCteNG4yF444smIs,160200
 spark_rapids_pytools/resources/qualx/models/xgboost/dataproc.json,sha256=JzTuXAidAbOUmK0xoJpsMKm1kIU2QCGOp-wyatTAyGQ,795042
 spark_rapids_pytools/resources/qualx/models/xgboost/dataproc_2.1-orc.json,sha256=ZSd34Yy1NiDYjpjPlBubZFSq-Ov9uH4UCGaAcn7Mwq8,361292
 spark_rapids_pytools/resources/qualx/models/xgboost/onprem.json,sha256=Iql4KaLjmk_VZgm9dbmO-qFsqFq-1fV4abaoGcd2S3U,530621
 spark_rapids_pytools/resources/templates/dataproc-create_gpu_cluster_script.ms,sha256=JhgUTLPRlDGr-vHbqYwbmerYAVKcBK8inJ1mGHff_O4,669
 spark_rapids_pytools/resources/templates/dataproc-run_bootstrap.ms,sha256=lmnyouNCpbytpRVZ_YbQ6d6hCl3XaYxqzNomxSJwSSk,518
 spark_rapids_pytools/resources/templates/emr-create_gpu_cluster_script.ms,sha256=UIlW0GcYn2fovtcDNYPUmg99h0zKy-DxXGO-1Lr_xQs,855
 spark_rapids_pytools/resources/templates/emr-run_bootstrap.ms,sha256=7xqXBMIu5Tg02KCq_YN9oLLiE3c8jgWl8BUvFQZODhs,537
 spark_rapids_pytools/resources/templates/cluster_template/databricks_aws.ms,sha256=8TcAd0HOgDsSIbVhhkk2FhfJiGmz83EYxDlyg4_ZBtI,241
-spark_rapids_pytools/resources/templates/cluster_template/databricks_azure.ms,sha256=3ozo3OGzHOfqQSCRsXRiXmb0RVAIczdWqB9zVAVvwb4,330
-spark_rapids_pytools/resources/templates/cluster_template/dataproc.ms,sha256=iDPWxqjhPRlI2pjVbTIJk5zUjGLzWV7LoS-bemOGMaU,626
+spark_rapids_pytools/resources/templates/cluster_template/databricks_azure.ms,sha256=0sVKMfyTRLAPhPlq6EZXHQhRQ3NgQiNkhN8Lxld_v5o,291
+spark_rapids_pytools/resources/templates/cluster_template/dataproc.ms,sha256=ZP44POz4-FuHy7oPBGVHFtIgb7b_HCbkBiE6bupGB2w,579
 spark_rapids_pytools/resources/templates/cluster_template/emr.ms,sha256=vsF6bl07eE-tPRe4z9uknNkCgAIEZTHEXkMQQyt9dJs,759
-spark_rapids_pytools/resources/templates/cluster_template/emr_node.ms,sha256=wkvwpv0eNLTdVvhTD49CCNmhRpQDo6373i-d-dr0uOk,293
+spark_rapids_pytools/resources/templates/node_template/databricks_aws.ms,sha256=mCFoGf_Ebacb3iFSvvlpY36AuqkDfektDYI1Avh4_ws,40
+spark_rapids_pytools/resources/templates/node_template/databricks_azure.ms,sha256=mCFoGf_Ebacb3iFSvvlpY36AuqkDfektDYI1Avh4_ws,40
+spark_rapids_pytools/resources/templates/node_template/emr.ms,sha256=wkvwpv0eNLTdVvhTD49CCNmhRpQDo6373i-d-dr0uOk,293
 spark_rapids_pytools/wrappers/__init__.py,sha256=CQ7Mf-YyBFNl6xmQGsPARv1w5GU3jGliByn5IHCcLkE,630
 spark_rapids_pytools/wrappers/databricks_aws_wrapper.py,sha256=H_vlUCwbjREQRY31p5Hw8lFtvBefuz_EhKJ1FeElY0A,19338
 spark_rapids_pytools/wrappers/databricks_azure_wrapper.py,sha256=lRajc_YFt92vJ0Rocek018wL74CltKKCBV0ewuQVxMA,18795
 spark_rapids_pytools/wrappers/dataproc_gke_wrapper.py,sha256=wjk8HJksf4RtE0si9W_V0Gzy0-IUsZ9epvXwMmAcYDo,9834
 spark_rapids_pytools/wrappers/dataproc_wrapper.py,sha256=f-I5f9E2cAemVXSW31V37MmqSYKUd-VZVUnkf89rxn8,18774
 spark_rapids_pytools/wrappers/emr_wrapper.py,sha256=OBgvCus5WefPd6B_3IM4U_X316iIJHfU2erAPevRG0Q,19300
 spark_rapids_pytools/wrappers/onprem_wrapper.py,sha256=haFjePrP0RquDvDMsbeY3pu0NwYE8w6H7ikCKtAzUbk,12518
@@ -108,18 +110,19 @@
 spark_rapids_tools/storagelib/local/localpath.py,sha256=gJ25FAZ2D_m5y_d5zii-fK73ZFCpiXnBUFimYLq7_X0,780
 spark_rapids_tools/storagelib/s3/__init__.py,sha256=z8CUs721lyZHAG3_Vcg-6gIP9VOPE3V5lEudb2lBnc8,726
 spark_rapids_tools/storagelib/s3/s3fs.py,sha256=vvEFZkLpOIwpW58DNi8atD-GYVv3wJjZVaOhd4g46WI,1732
 spark_rapids_tools/storagelib/s3/s3path.py,sha256=7JtLB5Nl6z1M6TMBGIuyumNKC3wsgkTY06n3J0BceTg,776
 spark_rapids_tools/tools/__init__.py,sha256=xOL1EJyVKvW3o4dCrtqghVhb7kf4Dgjb06x5nli2fXA,653
 spark_rapids_tools/tools/autotuner.py,sha256=nnP-ZN4fnONmKgGIyZV8DY-G0oLD6b4JGuEpLCuPBrc,1096
 spark_rapids_tools/tools/model_xgboost.py,sha256=gwz--J3dilRkzEzVaK7YY8yI5NOdVSndhua7gCprznc,54414
-spark_rapids_tools/tools/top_candidates.py,sha256=LxV5LBSmHcCZ9ddaDKuFOKX5sguujzH0CSD5OSClCCU,3284
+spark_rapids_tools/tools/speedup_category.py,sha256=7pxG5wG4JnugCUD0hpHVrQrRIN423tJd_rcuP4d1DIM,4764
+spark_rapids_tools/tools/top_candidates.py,sha256=NH8d2miKr6v_CfeXdOReb25fc6znO91T6Z4hPYpFE3M,1714
 spark_rapids_tools/tools/unsupported_ops_stage_duration.py,sha256=QeyovcFJsOlPUK-B3pO_cD68xjqVCyHV_HTNYisVfG0,4081
 spark_rapids_tools/utils/__init__.py,sha256=eYOmNcGR_4p8EvM41Jqd2VlnTwck1742DNa_Q_np5VQ,987
 spark_rapids_tools/utils/propmanager.py,sha256=7Cu8Qxi1owWO1cPjHYPyASxos-_iH5J86uYZEyLkrBs,4844
-spark_rapids_tools/utils/util.py,sha256=XgihSlpGv6Jm89wco121B-mKW3t6kbOeohfQw_DbkTk,12210
-spark_rapids_user_tools-24.2.3.dist-info/LICENSE,sha256=RnI8IUCDrXfGVHFfYTsT8OKEuaOtkMGDQOn8foh7D00,21086
-spark_rapids_user_tools-24.2.3.dist-info/METADATA,sha256=LvCE988O1d5FuswhVCRk3InCXdd32vbL87PyKs_lYQk,4126
-spark_rapids_user_tools-24.2.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-spark_rapids_user_tools-24.2.3.dist-info/entry_points.txt,sha256=MvX--wvYR0O5R5ArlTJeaCT3R7auC--PsQAD5haufDM,133
-spark_rapids_user_tools-24.2.3.dist-info/top_level.txt,sha256=OhA3L9VLtMKwE1-Dc8K7lmhLZ7aya3lxG_ifOnYWip8,40
-spark_rapids_user_tools-24.2.3.dist-info/RECORD,,
+spark_rapids_tools/utils/util.py,sha256=F6GtFq_PXkotITKalzhROnRJR-WHVCm54eW3OR9iOsk,12742
+spark_rapids_user_tools-24.2.4.dist-info/LICENSE,sha256=RnI8IUCDrXfGVHFfYTsT8OKEuaOtkMGDQOn8foh7D00,21086
+spark_rapids_user_tools-24.2.4.dist-info/METADATA,sha256=47DWDquc_6R7Ry95LDb-npDyp2U1quK6WiJY9ppZNfs,4126
+spark_rapids_user_tools-24.2.4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+spark_rapids_user_tools-24.2.4.dist-info/entry_points.txt,sha256=MvX--wvYR0O5R5ArlTJeaCT3R7auC--PsQAD5haufDM,133
+spark_rapids_user_tools-24.2.4.dist-info/top_level.txt,sha256=OhA3L9VLtMKwE1-Dc8K7lmhLZ7aya3lxG_ifOnYWip8,40
+spark_rapids_user_tools-24.2.4.dist-info/RECORD,,
```

