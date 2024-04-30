# Comparing `tmp/nuvla_job_engine-4.0.4.tar.gz` & `tmp/nuvla_job_engine-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nuvla_job_engine-4.0.4.tar", max compression
+gzip compressed data, was "nuvla_job_engine-4.0.5.tar", max compression
```

## Comparing `nuvla_job_engine-4.0.4.tar` & `nuvla_job_engine-4.0.5.tar`

### file list

```diff
@@ -1,109 +1,111 @@
--rw-r--r--   0        0        0    11357 2024-04-04 16:25:48.987583 nuvla_job_engine-4.0.4/LICENSE
--rw-r--r--   0        0        0     4575 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/README.md
--rw-r--r--   0        0        0        0 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/__init__.py
--rw-r--r--   0        0        0       24 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/connector/__init__.py
--rw-r--r--   0        0        0     1340 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/connector/connector.py
--rw-r--r--   0        0        0    11757 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/connector/docker_compose.py
--rw-r--r--   0        0        0    33689 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/connector/docker_machine.py
--rw-r--r--   0        0        0    15017 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/connector/docker_service.py
--rw-r--r--   0        0        0     8401 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/connector/docker_stack.py
--rwxr-xr-x   0        0        0     1412 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/connector/extra/install-rancher.sh
--rw-r--r--   0        0        0     1713 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/connector/extra/k8s-install.sh
--rw-r--r--   0        0        0     1432 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/connector/extra/portainer-k8s.yaml
--rw-r--r--   0        0        0      774 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/connector/extra/portainer-swarm.yaml
--rw-r--r--   0        0        0       68 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/connector/extra/ssh-add-keys.sh
--rw-r--r--   0        0        0    47994 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/connector/kubernetes.py
--rw-r--r--   0        0        0      322 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/connector/machine/__init__.py
--rw-r--r--   0        0        0      641 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/connector/machine/helper.py
--rw-r--r--   0        0        0    11681 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/connector/machine/machine.py
--rw-r--r--   0        0        0    28734 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/connector/nuvlabox.py
--rw-r--r--   0        0        0     5380 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/connector/registry.py
--rw-r--r--   0        0        0     3670 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/connector/utils.py
--rw-r--r--   0        0        0       95 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/__init__.py
--rw-r--r--   0        0        0     1989 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/__init__.py
--rwxr-xr-x   0        0        0     2999 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/application_docker_compose_validate.py
--rwxr-xr-x   0        0        0      320 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/bulk_deployment_set_start.py
--rwxr-xr-x   0        0        0     1686 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/bulk_deployment_set_stop.py
--rwxr-xr-x   0        0        0      322 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/bulk_deployment_set_update.py
--rwxr-xr-x   0        0        0      711 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/bulk_force_delete_deployment.py
--rwxr-xr-x   0        0        0      692 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/bulk_stop_deployment.py
--rwxr-xr-x   0        0        0      908 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/bulk_update_deployment.py
--rwxr-xr-x   0        0        0     1298 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/cancel_children_jobs.py
--rwxr-xr-x   0        0        0     4269 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/coe_provision.py
--rwxr-xr-x   0        0        0     1719 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/coe_start.py
--rwxr-xr-x   0        0        0     1644 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/coe_stop.py
--rwxr-xr-x   0        0        0     2601 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/coe_terminate.py
--rwxr-xr-x   0        0        0     2982 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/component_image_state.py
--rwxr-xr-x   0        0        0     8667 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/credential_check.py
--rw-r--r--   0        0        0     3129 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/dct_check.py
--rw-r--r--   0        0        0     2979 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/deployment_log_fetch.py
--rwxr-xr-x   0        0        0      345 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/deployment_set_delete.py
--rwxr-xr-x   0        0        0      421 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/deployment_set_force_delete.py
--rwxr-xr-x   0        0        0     5402 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/deployment_start.py
--rwxr-xr-x   0        0        0     7298 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/deployment_state.py
--rw-r--r--   0        0        0     3207 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/deployment_stop.py
--rw-r--r--   0        0        0     4010 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/deployment_update.py
--rwxr-xr-x   0        0        0      366 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/dummy_test_action.py
--rw-r--r--   0        0        0      729 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/handle_trial_end.py
--rwxr-xr-x   0        0        0     1051 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/jobs_cleanup.py
--rw-r--r--   0        0        0     3553 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/monitor_bulk_job.py
--rw-r--r--   0        0        0      697 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/notify_coupon_end.py
--rwxr-xr-x   0        0        0     2901 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_add_ssh_key.py
--rwxr-xr-x   0        0        0      692 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_check_api.py
--rwxr-xr-x   0        0        0      867 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_cluster.py
--rwxr-xr-x   0        0        0     2100 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_cluster_cleanup.py
--rwxr-xr-x   0        0        0     4570 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_decommission.py
--rwxr-xr-x   0        0        0     1856 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_disable_stream.py
--rwxr-xr-x   0        0        0     1273 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_enable_stream.py
--rw-r--r--   0        0        0     1453 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_log_fetch.py
--rwxr-xr-x   0        0        0     1232 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_reboot.py
--rwxr-xr-x   0        0        0     4425 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_releases.py
--rwxr-xr-x   0        0        0     1280 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_restart_stream.py
--rwxr-xr-x   0        0        0     2513 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_revoke_ssh_key.py
--rwxr-xr-x   0        0        0     2429 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_scalability_start.py
--rwxr-xr-x   0        0        0     1637 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_update.py
--rw-r--r--   0        0        0      849 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/register_usage_record.py
--rwxr-xr-x   0        0        0     3059 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/service_image_state.py
--rw-r--r--   0        0        0        0 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/utils/__init__.py
--rw-r--r--   0        0        0     1574 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/utils/bulk_action.py
--rwxr-xr-x   0        0        0      854 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/utils/bulk_deployment.py
--rwxr-xr-x   0        0        0     8840 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/utils/bulk_deployment_set_apply.py
--rwxr-xr-x   0        0        0     1289 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/utils/deployment_set_remove.py
--rw-r--r--   0        0        0    11037 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/utils/deployment_utils.py
--rw-r--r--   0        0        0     4009 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/utils/resource_log_fetch.py
--rwxr-xr-x   0        0        0     9633 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/vulnerabilities_database.py
--rw-r--r--   0        0        0     7390 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/base.py
--rw-r--r--   0        0        0     2107 2024-04-04 16:25:48.991583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/distribution.py
--rw-r--r--   0        0        0     1989 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/__init__.py
--rwxr-xr-x   0        0        0     1500 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/component_image_state.py
--rwxr-xr-x   0        0        0     2296 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/deployment_state.py
--rwxr-xr-x   0        0        0     1214 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/deployment_state_new.py
--rwxr-xr-x   0        0        0     2479 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/deployment_state_old.py
--rwxr-xr-x   0        0        0      408 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/dummy_action.py
--rwxr-xr-x   0        0        0     2907 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/handle_trial_end.py
--rwxr-xr-x   0        0        0      440 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/jobs_cleanup.py
--rwxr-xr-x   0        0        0     1803 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/monitor_bulk_jobs.py
--rwxr-xr-x   0        0        0     1754 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/notify_coupon_end.py
--rwxr-xr-x   0        0        0      487 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/nuvlabox_cluster_cleanup.py
--rwxr-xr-x   0        0        0     1435 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/nuvlabox_offline.py
--rwxr-xr-x   0        0        0      475 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/nuvlabox_releases.py
--rwxr-xr-x   0        0        0     1210 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/refresh_customer_subscription_cache.py
--rwxr-xr-x   0        0        0     2464 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/register_usage_record.py
--rwxr-xr-x   0        0        0     3119 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/register_usage_record_new_deployment.py
--rwxr-xr-x   0        0        0     1556 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/service_image_state.py
--rwxr-xr-x   0        0        0      503 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/vulnerabilities_database.py
--rw-r--r--   0        0        0        0 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributor/__init__.py
--rw-r--r--   0        0        0     1400 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributor/distributor.py
--rw-r--r--   0        0        0        0 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/executor/__init__.py
--rw-r--r--   0        0        0     4365 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/executor/executor.py
--rw-r--r--   0        0        0    10814 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/job.py
--rw-r--r--   0        0        0     1975 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/util.py
--rw-r--r--   0        0        0      186 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/job_engine/job/version.py
--rwxr-xr-x   0        0        0     2708 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/scripts/job_deployment_state_push.py
--rwxr-xr-x   0        0        0      208 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/scripts/job_distributor.py
--rwxr-xr-x   0        0        0      197 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/scripts/job_executor.py
--rwxr-xr-x   0        0        0     1967 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/scripts/job_restore.py
--rwxr-xr-x   0        0        0      186 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/nuvla/scripts/pause.py
--rw-r--r--   0        0        0     1221 2024-04-04 16:25:48.995583 nuvla_job_engine-4.0.4/pyproject.toml
--rw-r--r--   0        0        0     5677 1970-01-01 00:00:00.000000 nuvla_job_engine-4.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-30 09:09:30.085070 nuvla_job_engine-4.0.5/LICENSE
+-rw-r--r--   0        0        0     4588 2024-04-30 09:09:30.085070 nuvla_job_engine-4.0.5/README.md
+-rw-r--r--   0        0        0       74 2024-04-30 09:09:30.085070 nuvla_job_engine-4.0.5/nuvla/__init__.py
+-rw-r--r--   0        0        0       24 2024-04-30 09:09:30.085070 nuvla_job_engine-4.0.5/nuvla/job_engine/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 09:09:30.085070 nuvla_job_engine-4.0.5/nuvla/job_engine/connector/__init__.py
+-rw-r--r--   0        0        0     1340 2024-04-30 09:09:30.085070 nuvla_job_engine-4.0.5/nuvla/job_engine/connector/connector.py
+-rw-r--r--   0        0        0    11757 2024-04-30 09:09:30.085070 nuvla_job_engine-4.0.5/nuvla/job_engine/connector/docker_compose.py
+-rw-r--r--   0        0        0    33689 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/connector/docker_machine.py
+-rw-r--r--   0        0        0    15017 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/connector/docker_service.py
+-rw-r--r--   0        0        0     8401 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/connector/docker_stack.py
+-rwxr-xr-x   0        0        0     1412 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/connector/extra/install-rancher.sh
+-rw-r--r--   0        0        0     1713 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/connector/extra/k8s-install.sh
+-rw-r--r--   0        0        0     1432 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/connector/extra/portainer-k8s.yaml
+-rw-r--r--   0        0        0      774 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/connector/extra/portainer-swarm.yaml
+-rw-r--r--   0        0        0       68 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/connector/extra/ssh-add-keys.sh
+-rw-r--r--   0        0        0     2868 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/connector/helm_driver.py
+-rw-r--r--   0        0        0    28909 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/connector/k8s_driver.py
+-rw-r--r--   0        0        0    25028 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/connector/kubernetes.py
+-rw-r--r--   0        0        0      322 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/connector/machine/__init__.py
+-rw-r--r--   0        0        0      641 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/connector/machine/helper.py
+-rw-r--r--   0        0        0    11681 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/connector/machine/machine.py
+-rw-r--r--   0        0        0    28734 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/connector/nuvlabox.py
+-rw-r--r--   0        0        0     5380 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/connector/registry.py
+-rw-r--r--   0        0        0     3668 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/connector/utils.py
+-rw-r--r--   0        0        0       95 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/__init__.py
+-rw-r--r--   0        0        0     1989 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/__init__.py
+-rwxr-xr-x   0        0        0     2999 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/application_docker_compose_validate.py
+-rwxr-xr-x   0        0        0      320 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/bulk_deployment_set_start.py
+-rwxr-xr-x   0        0        0     1686 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/bulk_deployment_set_stop.py
+-rwxr-xr-x   0        0        0      322 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/bulk_deployment_set_update.py
+-rwxr-xr-x   0        0        0      711 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/bulk_force_delete_deployment.py
+-rwxr-xr-x   0        0        0      692 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/bulk_stop_deployment.py
+-rwxr-xr-x   0        0        0      908 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/bulk_update_deployment.py
+-rwxr-xr-x   0        0        0     1298 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/cancel_children_jobs.py
+-rwxr-xr-x   0        0        0     4269 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/coe_provision.py
+-rwxr-xr-x   0        0        0     1719 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/coe_start.py
+-rwxr-xr-x   0        0        0     1644 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/coe_stop.py
+-rwxr-xr-x   0        0        0     2601 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/coe_terminate.py
+-rwxr-xr-x   0        0        0     2982 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/component_image_state.py
+-rwxr-xr-x   0        0        0     8667 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/credential_check.py
+-rw-r--r--   0        0        0     3129 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/dct_check.py
+-rw-r--r--   0        0        0     2831 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/deployment_log_fetch.py
+-rwxr-xr-x   0        0        0      345 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/deployment_set_delete.py
+-rwxr-xr-x   0        0        0      421 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/deployment_set_force_delete.py
+-rwxr-xr-x   0        0        0     5402 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/deployment_start.py
+-rwxr-xr-x   0        0        0     7341 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/deployment_state.py
+-rw-r--r--   0        0        0     3207 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/deployment_stop.py
+-rw-r--r--   0        0        0     4010 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/deployment_update.py
+-rwxr-xr-x   0        0        0      366 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/dummy_test_action.py
+-rw-r--r--   0        0        0      729 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/handle_trial_end.py
+-rwxr-xr-x   0        0        0     1051 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/jobs_cleanup.py
+-rw-r--r--   0        0        0     3553 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/monitor_bulk_job.py
+-rw-r--r--   0        0        0      697 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/notify_coupon_end.py
+-rwxr-xr-x   0        0        0     2803 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_add_ssh_key.py
+-rwxr-xr-x   0        0        0      692 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_check_api.py
+-rwxr-xr-x   0        0        0      867 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_cluster.py
+-rwxr-xr-x   0        0        0     2100 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_cluster_cleanup.py
+-rwxr-xr-x   0        0        0     4570 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_decommission.py
+-rwxr-xr-x   0        0        0     1856 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_disable_stream.py
+-rwxr-xr-x   0        0        0     1273 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_enable_stream.py
+-rw-r--r--   0        0        0     1279 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_log_fetch.py
+-rwxr-xr-x   0        0        0     1247 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_reboot.py
+-rwxr-xr-x   0        0        0     4425 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_releases.py
+-rwxr-xr-x   0        0        0     1280 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_restart_stream.py
+-rwxr-xr-x   0        0        0     2515 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_revoke_ssh_key.py
+-rwxr-xr-x   0        0        0     2429 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_scalability_start.py
+-rwxr-xr-x   0        0        0     1633 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_update.py
+-rw-r--r--   0        0        0      849 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/register_usage_record.py
+-rwxr-xr-x   0        0        0     3059 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/service_image_state.py
+-rw-r--r--   0        0        0        0 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/utils/__init__.py
+-rw-r--r--   0        0        0     1574 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/utils/bulk_action.py
+-rwxr-xr-x   0        0        0      854 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/utils/bulk_deployment.py
+-rwxr-xr-x   0        0        0     8840 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/utils/bulk_deployment_set_apply.py
+-rwxr-xr-x   0        0        0     1289 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/utils/deployment_set_remove.py
+-rw-r--r--   0        0        0    11037 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/utils/deployment_utils.py
+-rw-r--r--   0        0        0     4008 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/utils/resource_log_fetch.py
+-rwxr-xr-x   0        0        0     9633 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/vulnerabilities_database.py
+-rw-r--r--   0        0        0     7390 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/base.py
+-rw-r--r--   0        0        0     2107 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/distribution.py
+-rw-r--r--   0        0        0     1989 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/__init__.py
+-rwxr-xr-x   0        0        0     1500 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/component_image_state.py
+-rwxr-xr-x   0        0        0     2296 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/deployment_state.py
+-rwxr-xr-x   0        0        0     1214 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/deployment_state_new.py
+-rwxr-xr-x   0        0        0     2479 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/deployment_state_old.py
+-rwxr-xr-x   0        0        0      408 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/dummy_action.py
+-rwxr-xr-x   0        0        0     2907 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/handle_trial_end.py
+-rwxr-xr-x   0        0        0      440 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/jobs_cleanup.py
+-rwxr-xr-x   0        0        0     1803 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/monitor_bulk_jobs.py
+-rwxr-xr-x   0        0        0     1754 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/notify_coupon_end.py
+-rwxr-xr-x   0        0        0      487 2024-04-30 09:09:30.093070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/nuvlabox_cluster_cleanup.py
+-rwxr-xr-x   0        0        0     1435 2024-04-30 09:09:30.093070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/nuvlabox_offline.py
+-rwxr-xr-x   0        0        0      475 2024-04-30 09:09:30.093070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/nuvlabox_releases.py
+-rwxr-xr-x   0        0        0     1210 2024-04-30 09:09:30.093070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/refresh_customer_subscription_cache.py
+-rwxr-xr-x   0        0        0     2464 2024-04-30 09:09:30.093070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/register_usage_record.py
+-rwxr-xr-x   0        0        0     3119 2024-04-30 09:09:30.093070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/register_usage_record_new_deployment.py
+-rwxr-xr-x   0        0        0     1556 2024-04-30 09:09:30.093070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/service_image_state.py
+-rwxr-xr-x   0        0        0      503 2024-04-30 09:09:30.093070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/vulnerabilities_database.py
+-rw-r--r--   0        0        0        0 2024-04-30 09:09:30.093070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributor/__init__.py
+-rw-r--r--   0        0        0     1400 2024-04-30 09:09:30.093070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributor/distributor.py
+-rw-r--r--   0        0        0        0 2024-04-30 09:09:30.093070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/executor/__init__.py
+-rw-r--r--   0        0        0     4365 2024-04-30 09:09:30.093070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/executor/executor.py
+-rw-r--r--   0        0        0    10814 2024-04-30 09:09:30.093070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/job.py
+-rw-r--r--   0        0        0     1975 2024-04-30 09:09:30.093070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/util.py
+-rw-r--r--   0        0        0      186 2024-04-30 09:09:30.093070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/version.py
+-rwxr-xr-x   0        0        0     2708 2024-04-30 09:09:30.093070 nuvla_job_engine-4.0.5/nuvla/scripts/job_deployment_state_push.py
+-rwxr-xr-x   0        0        0      208 2024-04-30 09:09:30.093070 nuvla_job_engine-4.0.5/nuvla/scripts/job_distributor.py
+-rwxr-xr-x   0        0        0      197 2024-04-30 09:09:30.093070 nuvla_job_engine-4.0.5/nuvla/scripts/job_executor.py
+-rwxr-xr-x   0        0        0     1967 2024-04-30 09:09:30.093070 nuvla_job_engine-4.0.5/nuvla/scripts/job_restore.py
+-rwxr-xr-x   0        0        0      186 2024-04-30 09:09:30.093070 nuvla_job_engine-4.0.5/nuvla/scripts/pause.py
+-rw-r--r--   0        0        0     1204 2024-04-30 09:09:30.093070 nuvla_job_engine-4.0.5/pyproject.toml
+-rw-r--r--   0        0        0     5632 1970-01-01 00:00:00.000000 nuvla_job_engine-4.0.5/PKG-INFO
```

### Comparing `nuvla_job_engine-4.0.4/LICENSE` & `nuvla_job_engine-4.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/README.md` & `nuvla_job_engine-4.0.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Nuvla Job Engine
 
-[![Build Status](https://github.com/nuvla/job-engine/actions/workflows/main.yml/badge.svg?branch=master)](https://github.com/nuvla/job-engine/actions/workflows/main.yml)
+[![UnitTests and Build Docker Dev. Image](https://github.com/nuvla/job-engine/actions/workflows/devel.yml/badge.svg)](https://github.com/nuvla/job-engine/actions/workflows/devel.yml)
 
 This repository contains the code and configuration for the Job engine, 
 packaged as a Docker container. 
 
 Nuvla job engine use cimi job resource and zookeeper as a locking queue. 
 It's done in a way to be horizontally scalled on different nodes.
```

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/connector/connector.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/connector/connector.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/connector/docker_compose.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/connector/docker_compose.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/connector/docker_machine.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/connector/docker_machine.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/connector/docker_service.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/connector/docker_service.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/connector/docker_stack.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/connector/docker_stack.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/connector/extra/install-rancher.sh` & `nuvla_job_engine-4.0.5/nuvla/job_engine/connector/extra/install-rancher.sh`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/connector/extra/k8s-install.sh` & `nuvla_job_engine-4.0.5/nuvla/job_engine/connector/extra/k8s-install.sh`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/connector/extra/portainer-k8s.yaml` & `nuvla_job_engine-4.0.5/nuvla/job_engine/connector/extra/portainer-k8s.yaml`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/connector/extra/portainer-swarm.yaml` & `nuvla_job_engine-4.0.5/nuvla/job_engine/connector/extra/portainer-swarm.yaml`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/connector/machine/helper.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/connector/machine/helper.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/connector/machine/machine.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/connector/machine/machine.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/connector/nuvlabox.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/connector/nuvlabox.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/connector/registry.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/connector/registry.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/connector/utils.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/connector/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -68,15 +68,15 @@
               'with input: %s',
               timeout, cmd, opt_env, opt_input)
     try:
         result = run(cmd, stdout=PIPE, stderr=stderr, env=opt_env, input=opt_input,
                      timeout=timeout, encoding='UTF-8')
         log.debug('Command result: %s', result)
     except TimeoutExpired:
-        message = 'Command execution timed out after {} seconds'.format(timeout)
+        message = f'Command execution timed out after {timeout} seconds'
         log.exception(message)
         raise Exception(message)
     if result.returncode == 0:
         return result
     else:
         log.exception(result)
         raise Exception(result.stderr)
@@ -89,15 +89,15 @@
 def create_tmp_file(content):
     file = NamedTemporaryFile(delete=True)
     file.write(content.encode())
     file.flush()
     return file
 
 
-def generate_registry_config(registries_auth):
+def generate_registry_config(registries_auth: list):
     auths = {}
     for registry_auth in registries_auth:
         user_pass = registry_auth['username'] + ':' + registry_auth['password']
         auth = base64.b64encode(user_pass.encode('ascii')).decode('utf-8')
         auths['https://' + registry_auth['serveraddress']] = {'auth': auth}
     return json.dumps({'auths': auths})
```

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/__init__.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/application_docker_compose_validate.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/application_docker_compose_validate.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/bulk_deployment_set_stop.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/bulk_deployment_set_stop.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/bulk_force_delete_deployment.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/bulk_force_delete_deployment.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/bulk_stop_deployment.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/bulk_stop_deployment.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/bulk_update_deployment.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/bulk_update_deployment.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/cancel_children_jobs.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/cancel_children_jobs.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/coe_provision.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/coe_provision.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/coe_start.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/coe_start.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/coe_stop.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/coe_stop.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/coe_terminate.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/coe_terminate.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/component_image_state.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/component_image_state.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/credential_check.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/credential_check.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/dct_check.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/dct_check.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/deployment_log_fetch.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/deployment_log_fetch.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,16 +36,14 @@
     @property
     def connector_name(self):
         if not self._connector_name:
             self._connector_name = get_connector_name(self.deployment)
         return self._connector_name
 
     def get_kubernetes_log(self, component, since, lines):
-        self.log.debug(f"Calling the Kubernetes deployment logging...\n\
-            The Connector is set to: {self.connector.__class__.__name__}")
         return self.connector.log(component, since, lines,
                                   namespace=Deployment.uuid(self.deployment))
 
     def get_docker_compose_log(self, component, since, lines):
         module_content = Deployment.module_content(self.deployment)
         return self.connector.log(
             component, since, lines,
```

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/deployment_start.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/deployment_start.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/deployment_state.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/deployment_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,24 +128,23 @@
         services = connector.list(filters={"name": sname})
         if services:
             ports_mapping = connector.extract_vm_ports_mapping(services[0])
             self.api_dpl.update_port_parameters(self.deployment, ports_mapping)
 
     def get_application_state(self):
         kwargs = {}
-        env  = get_env(self.deployment.data)
-        name = Deployment.uuid(self.deployment)
-        connector_name  = get_connector_name(self.deployment)
-        connector_class = get_connector_class(connector_name)
-        connector = initialize_connector(connector_class, self.job, self.deployment)
-
         if Deployment.is_compatibility_docker_compose(self.deployment):
             kwargs['compose_file'] = Deployment.module_content(self.deployment)['docker-compose']
 
-        services = connector.get_services(name, env, **kwargs)
+        connector_name = get_connector_name(self.deployment)
+        connector_class = get_connector_class(connector_name)
+        connector = initialize_connector(connector_class, self.job, self.deployment)
+        services = connector.get_services(Deployment.uuid(self.deployment),
+                                          get_env(self.deployment.data),
+                                          **kwargs)
 
         self.create_update_hostname_output_parameter()
         self.create_update_ips_output_parameters()
 
         self.application_params_update(services)
 
     def do_work(self):
```

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/deployment_stop.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/deployment_stop.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/deployment_update.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/deployment_update.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/handle_trial_end.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/handle_trial_end.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/jobs_cleanup.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/jobs_cleanup.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/monitor_bulk_job.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/monitor_bulk_job.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/notify_coupon_end.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/notify_coupon_end.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_add_ssh_key.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_add_ssh_key.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,51 +29,53 @@
         affected_resources = self.job['affected-resources']
         credential_id = None
         for ar in affected_resources:
             if ar.get('href', '').startswith('credential/'):
                 credential_id = ar.get('href')
                 break
 
-        if credential_id:
-            public_key = self.job.context[credential_id]['public-key']
-            if not self._sanitize_ssh_key(public_key):
-                r = "ssh public key not valid: " + public_key
-                self.job.update_job(status_message=json.dumps(r))
-                return 1
-            self.job.set_progress(10)
-            if os.getenv('KUBERNETES_SERVICE_HOST'):
-                logging.debug('We are using Kubernetes on nuvlabox ID : %s ',nuvlabox_id)
-                connector = K8sSSHKey(api=self.api, nuvlabox_id=nuvlabox_id, job=self.job)
-                connector.handle_ssh_key('add-ssh-key', public_key, credential_id, \
-                    nuvlabox_id=nuvlabox_id)
-            else:
-                connector = NB.NuvlaBox(api=self.api, nuvlabox_id=nuvlabox_id, job=self.job)
-                connector.connect()
-                ssh_keys = connector.nuvlabox.get('ssh-keys', []) 
-                if credential_id not in ssh_keys:
-                    r = connector.nuvlabox_manage_ssh_key('add-ssh-key', public_key)
-
-                    update_payload = ssh_keys + [credential_id]
-
-                    connector.commission({"ssh-keys": update_payload})
-                else:
-                    r = "Requested SSH key has already been added to the \
-                        NuvlaBox in the past. Nothing to do..."
-                self.job.update_job(status_message=json.dumps(r))
-                self.job.set_progress(100)
-        else:
+        if not credential_id:
             raise Exception('Cannot find any reference to an existing credential ID')
 
+        public_key = self.job.context[credential_id]['public-key']
+
+        if not self._is_valid_ssh_key(public_key):
+            r = "SSH public key is not valid: " + public_key
+            self.job.update_job(status_message=json.dumps(r))
+            return 1
+
+        self.job.set_progress(10)
+        if os.getenv('KUBERNETES_SERVICE_HOST'):
+            logging.debug('Using Kubernetes on NuvlaEdge: %s', nuvlabox_id)
+            connector = K8sSSHKey(job=self.job, nuvlabox_id=nuvlabox_id)
+            connector.manage_ssh_key(K8sSSHKey.ACTION_ADD, public_key,
+                                     credential_id, nuvlabox_id=nuvlabox_id)
+        else:
+            connector = NB.NuvlaBox(api=self.api, nuvlabox_id=nuvlabox_id, job=self.job)
+            connector.connect()
+            ssh_keys = connector.nuvlabox.get('ssh-keys', [])
+            if credential_id not in ssh_keys:
+                r = connector.nuvlabox_manage_ssh_key('add-ssh-key', public_key)
+
+                update_payload = ssh_keys + [credential_id]
+
+                connector.commission({"ssh-keys": update_payload})
+            else:
+                r = "Requested SSH key has already been added to the \
+                    NuvlaBox in the past. Nothing to do..."
+            self.job.update_job(status_message=json.dumps(r))
+            self.job.set_progress(100)
+
         return 0
 
-    def _sanitize_ssh_key(self, public_key):
+    def _is_valid_ssh_key(self, public_key):
         """
         function to check that the ssh key string is valid
         
         argument:
         public_key: the public key as a string
         """
-        logging.debug("Checking ssh public key %s ",public_key)
+        logging.debug("Checking ssh public key %s ", public_key)
         return re.match(r'^ssh-\w+\s+\S+(\s+\S+)?$', public_key)
 
     def do_work(self):
         return self.add_ssh_key()
```

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_check_api.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_check_api.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_cluster.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_cluster.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_cluster_cleanup.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_cluster_cleanup.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_decommission.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_decommission.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_disable_stream.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_disable_stream.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_enable_stream.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_enable_stream.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_log_fetch.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_log_fetch.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 import os
 import logging
 
 from ...connector import nuvlabox as nb
-from ...connector import kubernetes as k8
+from ...connector import kubernetes as k8s
 from ..actions import action
 from .utils.resource_log_fetch import ResourceLogFetchJob
 
 action_name = 'fetch_nuvlabox_log'
 
 @action(action_name, True)
 class NuvlaBoxLogFetchJob(ResourceLogFetchJob):
@@ -22,19 +22,15 @@
     @property
     def connector(self):
 
         if not self._connector:
             if os.getenv('KUBERNETES_SERVICE_HOST'):
                 logging.debug("Kubernetes connector used.")
                 try:
-                    self._connector = \
-                        k8.K8sLogging(
-                            api=self.api,
-                            nuvlabox_id=self.resource_log_parent,
-                            job=self.job,)
+                    self._connector = k8s.K8sLogging()
                 except Exception as e:
                     logging.error(f'Kubernetes error:\n{str(e)}')
             else:
                 self._connector = \
                     nb.NuvlaBox(
                         api=self.api,
                         nuvlabox_id=self.resource_log_parent,
```

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_reboot.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_reboot.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,16 +27,16 @@
             ret = self._reboot_docker()
 
         logging.info(f'Reboot action called. Output: {ret}')
 
         return 0
 
     def _reboot_docker(self) -> str:
-        connector = NuvlaBox(api=self.api, \
-            nuvlabox_id=self.job['target-resource']['href'], job=self.job)
+        connector = NuvlaBox(api=self.api, job=self.job,
+                             nuvlabox_id=self.job['target-resource']['href'])
         return connector.reboot()
 
     def _reboot_k8s(self) -> str:
         connector = K8sEdgeMgmt(self.job)
         self.job.set_progress(10)
         ret = connector.reboot()
         self.job.set_progress(90)
```

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_releases.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_releases.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_restart_stream.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_restart_stream.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_revoke_ssh_key.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_revoke_ssh_key.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,18 +35,18 @@
                 credential_id = ar.get('href')
                 break
 
         if credential_id:
             public_key = self.job.context[credential_id]['public-key']
             self.job.set_progress(10)
             if os.getenv('KUBERNETES_SERVICE_HOST'):
-                logging.debug('We are using Kubernetes on nuvlabox ID : %s ',nuvlabox_id)
-                connector = K8sSSHKey(api=self.api, nuvlabox_id=nuvlabox_id, job=self.job)
-                connector.handle_ssh_key('revoke-ssh-key', public_key, \
-                    credential_id, nuvlabox_id=nuvlabox_id)
+                logging.debug('Using Kubernetes on NuvlaEdge: %s', nuvlabox_id)
+                connector = K8sSSHKey(job=self.job, nuvlabox_id=nuvlabox_id)
+                connector.manage_ssh_key(K8sSSHKey.ACTION_REVOKE, public_key,
+                                         credential_id, nuvlabox_id=nuvlabox_id)
             else:
                 connector = NB.NuvlaBox(api=self.api, nuvlabox_id=nuvlabox_id, job=self.job)
                 r = connector.nuvlabox_manage_ssh_key('revoke-ssh-key', public_key)
                 ssh_keys = connector.nuvlabox.get('ssh-keys', [])
                 try:
                     ssh_keys.remove(credential_id)
                     update_payload = {"ssh-keys": ssh_keys}
```

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_scalability_start.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_scalability_start.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/nuvlabox_update.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     def nuvlabox_update(self):
         nuvlabox_id = self.job['target-resource']['href']
 
         logging.info('Updating NuvlaBox {}'.format(nuvlabox_id))
         if os.getenv('KUBERNETES_SERVICE_HOST'):
             logging.debug('Found kubernetes installation.')
-            connector = K8sEdgeMgmt(job=self.job)
+            connector = K8sEdgeMgmt(self.job)
         else:
             logging.info('Found docker installation.')
             connector = NB.NuvlaBox(api=self.api, nuvlabox_id=nuvlabox_id, job=self.job)
         # IMPORTANT BIT THAT MUST CHANGE FOR EVERY NUVLABOX API ACTION
         # in this case, we need to fetch the target NB release
         affected_resources = self.job['affected-resources']
         nb_release_id = None
```

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/register_usage_record.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/register_usage_record.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/service_image_state.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/service_image_state.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/utils/bulk_action.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/utils/bulk_action.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/utils/bulk_deployment.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/utils/bulk_deployment.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/utils/bulk_deployment_set_apply.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/utils/bulk_deployment_set_apply.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/utils/deployment_set_remove.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/utils/deployment_set_remove.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/utils/deployment_utils.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/utils/deployment_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from nuvla.api.resources.base import ResourceNotFound
 
 from ....connector import (docker_service,
                            docker_stack,
                            docker_compose,
                            kubernetes,
                            utils)
-from ....connector.kubernetes import get_kubernetes_local_endpoint
+from ....connector.k8s_driver import get_kubernetes_local_endpoint
 
 
 def get_connector_name(deployment):
     if Deployment.is_component(deployment):
         return 'docker_service'
 
     elif Deployment.is_application(deployment):
```

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/utils/resource_log_fetch.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/utils/resource_log_fetch.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
     def get_component_logs(self, component: str, since: datetime,
                            lines: int) -> str:
 
         self.log.debug(f"Calling get_component_logs...\n\
             Connector is set to: {self.connector.__class__.__name__}")
 
-        return self.connector.log(component, since, lines,)
+        return self.connector.log(component, since, lines)
 
     def get_resource_log(self, log_id: str) -> dict:
         return self.api.get(log_id).data
 
     def update_resource_log(self, log_id: str, resource_log: dict) -> None:
         self.api.edit(log_id, resource_log)
```

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/actions/vulnerabilities_database.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/vulnerabilities_database.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/base.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/base.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/distribution.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/distribution.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/__init__.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/component_image_state.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/component_image_state.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/deployment_state.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/deployment_state.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/deployment_state_new.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/deployment_state_new.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/deployment_state_old.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/deployment_state_old.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/handle_trial_end.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/handle_trial_end.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/monitor_bulk_jobs.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/monitor_bulk_jobs.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/notify_coupon_end.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/notify_coupon_end.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/nuvlabox_offline.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/nuvlabox_offline.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/refresh_customer_subscription_cache.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/refresh_customer_subscription_cache.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/register_usage_record.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/register_usage_record.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/register_usage_record_new_deployment.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/register_usage_record_new_deployment.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributions/service_image_state.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/service_image_state.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/distributor/distributor.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributor/distributor.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/executor/executor.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/executor/executor.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/job.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/job.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/job_engine/job/util.py` & `nuvla_job_engine-4.0.5/nuvla/job_engine/job/util.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/scripts/job_deployment_state_push.py` & `nuvla_job_engine-4.0.5/nuvla/scripts/job_deployment_state_push.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/nuvla/scripts/job_restore.py` & `nuvla_job_engine-4.0.5/nuvla/scripts/job_restore.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.4/pyproject.toml` & `nuvla_job_engine-4.0.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nuvla-job-engine"
-version = "4.0.4"
+version = "4.0.5"
 description = "Nuvla Job Engine."
 license = "Apache-2.0"
 authors = ["SixSq SA <support@sixsq.com>"]
 maintainers = ["Ignacio Penas <nacho@sixsq.com>"]
 readme = "README.md"
 repository = "https://github.com/nuvla/job-engine"
 classifiers = [
@@ -16,28 +16,27 @@
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.11",
         "Topic :: Software Development"]
 packages = [{ include = "nuvla" }]
 
 
 [tool.poetry.dependencies]
-python = "^3.11"
-nuvla-api = "^3.0.9"
+python = ">=3.11,<3.12"
+nuvla-api = "^4"
 docker = "^7.0.0"
 pyyaml = "^6.0.1"
 statsd = "^4.0.1"
 packaging = "^23.2"
 importlib-metadata = "^7.0.1"
 
 
 [tool.poetry.group.server.dependencies]
 elasticsearch = "^7"
 boto3 = "^1.34.40"
 kazoo = "^2.6.0"
-requests = "2.27.1"
 
 
 [tool.poetry.group.test.dependencies]
 mock = "^5.1.0"
 pytest = "^8.0.0"
 pytest-cov = "^4.1.0"
 coverage = "^7.4.1"
```

### Comparing `nuvla_job_engine-4.0.4/PKG-INFO` & `nuvla_job_engine-4.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 Metadata-Version: 2.1
 Name: nuvla-job-engine
-Version: 4.0.4
+Version: 4.0.5
 Summary: Nuvla Job Engine.
 Home-page: https://github.com/nuvla/job-engine
 License: Apache-2.0
 Author: SixSq SA
 Author-email: support@sixsq.com
 Maintainer: Ignacio Penas
 Maintainer-email: nacho@sixsq.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.11,<3.12
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Requires-Dist: docker (>=7.0.0,<8.0.0)
 Requires-Dist: importlib-metadata (>=7.0.1,<8.0.0)
-Requires-Dist: nuvla-api (>=3.0.9,<4.0.0)
+Requires-Dist: nuvla-api (>=4,<5)
 Requires-Dist: packaging (>=23.2,<24.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: statsd (>=4.0.1,<5.0.0)
 Project-URL: Repository, https://github.com/nuvla/job-engine
 Description-Content-Type: text/markdown
 
 # Nuvla Job Engine
 
-[![Build Status](https://github.com/nuvla/job-engine/actions/workflows/main.yml/badge.svg?branch=master)](https://github.com/nuvla/job-engine/actions/workflows/main.yml)
+[![UnitTests and Build Docker Dev. Image](https://github.com/nuvla/job-engine/actions/workflows/devel.yml/badge.svg)](https://github.com/nuvla/job-engine/actions/workflows/devel.yml)
 
 This repository contains the code and configuration for the Job engine, 
 packaged as a Docker container. 
 
 Nuvla job engine use cimi job resource and zookeeper as a locking queue. 
 It's done in a way to be horizontally scalled on different nodes.
```

