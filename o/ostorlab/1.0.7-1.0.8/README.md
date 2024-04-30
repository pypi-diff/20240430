# Comparing `tmp/ostorlab-1.0.7.tar.gz` & `tmp/ostorlab-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ostorlab-1.0.7.tar", last modified: Fri Apr 19 13:17:53 2024, max compression
+gzip compressed data, was "ostorlab-1.0.8.tar", last modified: Tue Apr 30 12:08:02 2024, max compression
```

## Comparing `ostorlab-1.0.7.tar` & `ostorlab-1.0.8.tar`

### file list

```diff
@@ -1,1480 +1,1464 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.125478 ostorlab-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-19 13:17:38.000000 ostorlab-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14982 2024-04-19 13:17:53.125478 ostorlab-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12872 2024-04-19 13:17:38.000000 ostorlab-1.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-04-19 13:17:53.125478 ostorlab-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-19 13:17:38.000000 ostorlab-1.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.901477 ostorlab-1.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.945477 ostorlab-1.0.7/src/ostorlab/
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.945477 ostorlab-1.0.7/src/ostorlab/agent/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21209 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.945477 ostorlab-1.0.7/src/ostorlab/agent/kb/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.949477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.921477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.913477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.901477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.949477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_DEBUG/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_DEBUG/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_DEBUG/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_DEBUG/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.949477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_ELF_NOTPROTECTED/
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_ELF_NOTPROTECTED/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_ELF_NOTPROTECTED/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_ELF_NOTPROTECTED/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.949477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_INSECURE_NETWORK_SECURITY_CONFIG/
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_INSECURE_NETWORK_SECURITY_CONFIG/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_INSECURE_NETWORK_SECURITY_CONFIG/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_INSECURE_NETWORK_SECURITY_CONFIG/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.949477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_NOT_OBFUSCATED/
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_NOT_OBFUSCATED/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_NOT_OBFUSCATED/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_NOT_OBFUSCATED/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.905477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.949477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_FILE_PROVIDER_PERMISSIVE_EXTERNAL_PATH/
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_FILE_PROVIDER_PERMISSIVE_EXTERNAL_PATH/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_FILE_PROVIDER_PERMISSIVE_EXTERNAL_PATH/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_FILE_PROVIDER_PERMISSIVE_EXTERNAL_PATH/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.949477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_INSECURE_EXEC_CMD/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_INSECURE_EXEC_CMD/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_INSECURE_EXEC_CMD/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_INSECURE_EXEC_CMD/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.949477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_NOTIFICATION_SPOOFING/
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_NOTIFICATION_SPOOFING/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_NOTIFICATION_SPOOFING/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_NOTIFICATION_SPOOFING/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.949477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_WIFI_API_PII/
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_WIFI_API_PII/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_WIFI_API_PII/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_WIFI_API_PII/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.953477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/INSECURE_PACKAGE_CONTEXT/
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/INSECURE_PACKAGE_CONTEXT/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/INSECURE_PACKAGE_CONTEXT/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/INSECURE_PACKAGE_CONTEXT/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.905477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_IMPORTANT/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.953477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_IMPORTANT/APK_EXPORTED/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_IMPORTANT/APK_EXPORTED/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_IMPORTANT/APK_EXPORTED/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_IMPORTANT/APK_EXPORTED/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.953477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_IMPORTANT/APK_SCREENSHOT_DISABLED/
--rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_IMPORTANT/APK_SCREENSHOT_DISABLED/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_IMPORTANT/APK_SCREENSHOT_DISABLED/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_IMPORTANT/APK_SCREENSHOT_DISABLED/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.909477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.953477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_ANALYZE_JNI_ELF/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_ANALYZE_JNI_ELF/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_ANALYZE_JNI_ELF/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_ANALYZE_JNI_ELF/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.953477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_ATTACK_SURFACE/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_ATTACK_SURFACE/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_ATTACK_SURFACE/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_ATTACK_SURFACE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.953477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_CERTIFICAT_INFO/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_CERTIFICAT_INFO/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_CERTIFICAT_INFO/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_CERTIFICAT_INFO/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.953477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_CLASSES/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_CLASSES/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_CLASSES/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_CLASSES/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.953477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_CONST_STRINGS/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_CONST_STRINGS/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_CONST_STRINGS/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_CONST_STRINGS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.957477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_CODE_LOAD/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_CODE_LOAD/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_CODE_LOAD/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_CODE_LOAD/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.957477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_COMMAND_EXEC/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_COMMAND_EXEC/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_COMMAND_EXEC/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_COMMAND_EXEC/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.957477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_CRYPTO/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_CRYPTO/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_CRYPTO/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_CRYPTO/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.957477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_FILESYSTEM/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_FILESYSTEM/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_FILESYSTEM/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_FILESYSTEM/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.957477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_HASH/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_HASH/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_HASH/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_HASH/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.957477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_HTTP/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_HTTP/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_HTTP/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_HTTP/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.957477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_INTENT/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_INTENT/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_INTENT/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_INTENT/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.957477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_IPC/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_IPC/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_IPC/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_IPC/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.961477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_LOGGING/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_LOGGING/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_LOGGING/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_LOGGING/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.961477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_PROCESS/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_PROCESS/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_PROCESS/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_PROCESS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.961477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SERIALIZATION/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SERIALIZATION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SERIALIZATION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SERIALIZATION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.961477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SHARED_PREFERENCES/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SHARED_PREFERENCES/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SHARED_PREFERENCES/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SHARED_PREFERENCES/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.961477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SQLITE/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SQLITE/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SQLITE/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SQLITE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.961477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SSL_PINNING/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SSL_PINNING/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SSL_PINNING/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SSL_PINNING/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.961477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_TLS/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_TLS/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_TLS/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_TLS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.961477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_WEBVIEW/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_WEBVIEW/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_WEBVIEW/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_WEBVIEW/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.961477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_FILEOBSERVER_IMPL/
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_FILEOBSERVER_IMPL/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_FILEOBSERVER_IMPL/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_FILEOBSERVER_IMPL/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.965477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_FILE_LIST/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_FILE_LIST/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_FILE_LIST/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_FILE_LIST/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.965477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_HARDCODED_SQLS/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_HARDCODED_SQLS/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_HARDCODED_SQLS/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_HARDCODED_SQLS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.965477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_HARDCODED_URLS/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_HARDCODED_URLS/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_HARDCODED_URLS/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_HARDCODED_URLS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.965477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_LIST_PERMISSIONS/
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_LIST_PERMISSIONS/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_LIST_PERMISSIONS/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_LIST_PERMISSIONS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.965477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_MANIFEST/
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_MANIFEST/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_MANIFEST/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_MANIFEST/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.965477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_OBFUSCTAED/
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_OBFUSCTAED/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_OBFUSCTAED/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_OBFUSCTAED/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.965477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_WEBVIEWCLIENT_IMPL/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_WEBVIEWCLIENT_IMPL/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_WEBVIEWCLIENT_IMPL/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_WEBVIEWCLIENT_IMPL/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.965477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/BROADCAST_RECEIVER_DYNAMIC_REGISTRATION/
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/BROADCAST_RECEIVER_DYNAMIC_REGISTRATION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/BROADCAST_RECEIVER_DYNAMIC_REGISTRATION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/BROADCAST_RECEIVER_DYNAMIC_REGISTRATION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.969477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_ANDROIDSECURITY/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_ANDROIDSECURITY/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_ANDROIDSECURITY/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_ANDROIDSECURITY/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.969477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_BLUETOOTH/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_BLUETOOTH/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_BLUETOOTH/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_BLUETOOTH/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.969477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_CRYPTO/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_CRYPTO/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_CRYPTO/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_CRYPTO/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.969477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_DELETE_FILE/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_DELETE_FILE/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_DELETE_FILE/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_DELETE_FILE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.969477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_DYNAMIC_CODE_LOADING/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_DYNAMIC_CODE_LOADING/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_DYNAMIC_CODE_LOADING/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_DYNAMIC_CODE_LOADING/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.969477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_EXEC/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_EXEC/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_EXEC/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_EXEC/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.969477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_EXTERNAL_STORAGE/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_EXTERNAL_STORAGE/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_EXTERNAL_STORAGE/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_EXTERNAL_STORAGE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.969477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_IPC/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_IPC/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_IPC/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_IPC/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.969477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_LOG/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_LOG/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_LOG/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_LOG/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.973477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_NATIVE/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_NATIVE/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_NATIVE/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_NATIVE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.973477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_RANDOM/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_RANDOM/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_RANDOM/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_RANDOM/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.973477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_REFLECTION/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_REFLECTION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_REFLECTION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_REFLECTION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.973477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_SOCKET/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_SOCKET/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_SOCKET/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_SOCKET/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.973477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_SQL/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_SQL/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_SQL/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_SQL/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.973477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_SSLTLS/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_SSLTLS/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_SSLTLS/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_SSLTLS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.973477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_WEBVIEW/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_WEBVIEW/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_WEBVIEW/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_WEBVIEW/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.973477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_XML/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_XML/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_XML/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_XML/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.977477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_ZIP/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_ZIP/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_ZIP/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_ZIP/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.977477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/EXPANSION_APK/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/EXPANSION_APK/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/EXPANSION_APK/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/EXPANSION_APK/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.909477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.977477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_DEBUG_SYMBOL_PRESENT/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_DEBUG_SYMBOL_PRESENT/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_DEBUG_SYMBOL_PRESENT/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_DEBUG_SYMBOL_PRESENT/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.977477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_FACEBOOK_REACT_DEV_SETTINGS_ENABLED/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_FACEBOOK_REACT_DEV_SETTINGS_ENABLED/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_FACEBOOK_REACT_DEV_SETTINGS_ENABLED/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_FACEBOOK_REACT_DEV_SETTINGS_ENABLED/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.977477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_HAS_FRAGILE_USER_DATA_NOT_SET/
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_HAS_FRAGILE_USER_DATA_NOT_SET/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_HAS_FRAGILE_USER_DATA_NOT_SET/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_HAS_FRAGILE_USER_DATA_NOT_SET/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.977477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_LIST_NOT_USED_PERMISSIONS/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_LIST_NOT_USED_PERMISSIONS/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_LIST_NOT_USED_PERMISSIONS/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_LIST_NOT_USED_PERMISSIONS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.977477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_REQUEST_LEGACY_EXTERNAL_STORAGE/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_REQUEST_LEGACY_EXTERNAL_STORAGE/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_REQUEST_LEGACY_EXTERNAL_STORAGE/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_REQUEST_LEGACY_EXTERNAL_STORAGE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.981477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_TASK_HIJACKING/
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_TASK_HIJACKING/context.md
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_TASK_HIJACKING/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_TASK_HIJACKING/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_TASK_HIJACKING/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.981477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_USES_CLEAR_TEXT_TRAFFIC/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_USES_CLEAR_TEXT_TRAFFIC/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_USES_CLEAR_TEXT_TRAFFIC/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_USES_CLEAR_TEXT_TRAFFIC/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.981477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/DEPRECATED_TARGET_API_VERSION/
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/DEPRECATED_TARGET_API_VERSION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/DEPRECATED_TARGET_API_VERSION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/DEPRECATED_TARGET_API_VERSION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.981477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/INTENT_SPOOFING/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/INTENT_SPOOFING/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/INTENT_SPOOFING/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/INTENT_SPOOFING/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.981477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/PRIVACY_KEYBOARD_CACHE/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/PRIVACY_KEYBOARD_CACHE/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/PRIVACY_KEYBOARD_CACHE/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/PRIVACY_KEYBOARD_CACHE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.913477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.981477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_CERTIFICAT_OUTDATED/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_CERTIFICAT_OUTDATED/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_CERTIFICAT_OUTDATED/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_CERTIFICAT_OUTDATED/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.981477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_FACEBOOK_DEBUG_ENABLED/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_FACEBOOK_DEBUG_ENABLED/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_FACEBOOK_DEBUG_ENABLED/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_FACEBOOK_DEBUG_ENABLED/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.981477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_INSECURE_DOWNLOAD_MANAGER/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_INSECURE_DOWNLOAD_MANAGER/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_INSECURE_DOWNLOAD_MANAGER/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_INSECURE_DOWNLOAD_MANAGER/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.985477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_INSECURE_PATH_CLASS_LOADER/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_INSECURE_PATH_CLASS_LOADER/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_INSECURE_PATH_CLASS_LOADER/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_INSECURE_PATH_CLASS_LOADER/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.985477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_UNDECLARED_PERMISSIONS/
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_UNDECLARED_PERMISSIONS/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_UNDECLARED_PERMISSIONS/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_UNDECLARED_PERMISSIONS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.985477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/DANGEROUS_API_SETJAVASCRIPTINTERFACE/
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/DANGEROUS_API_SETJAVASCRIPTINTERFACE/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/DANGEROUS_API_SETJAVASCRIPTINTERFACE/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/DANGEROUS_API_SETJAVASCRIPTINTERFACE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.985477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/DANGEROUS_API_WEBVIEW_REMOTE_DEBUGGING_ENABLED/
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/DANGEROUS_API_WEBVIEW_REMOTE_DEBUGGING_ENABLED/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/DANGEROUS_API_WEBVIEW_REMOTE_DEBUGGING_ENABLED/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/DANGEROUS_API_WEBVIEW_REMOTE_DEBUGGING_ENABLED/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.985477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/IMPLICIT_PENDINGINTENT/
--rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/IMPLICIT_PENDINGINTENT/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/IMPLICIT_PENDINGINTENT/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/IMPLICIT_PENDINGINTENT/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.985477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_API_BLUETOOTH/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_API_BLUETOOTH/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_API_BLUETOOTH/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_API_BLUETOOTH/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.985477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_CLASS_LOADING/
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_CLASS_LOADING/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_CLASS_LOADING/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_CLASS_LOADING/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.985477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_PERMISSION_SHARED_PREFERENCES/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_PERMISSION_SHARED_PREFERENCES/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_PERMISSION_SHARED_PREFERENCES/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_PERMISSION_SHARED_PREFERENCES/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.989477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_REGISTER_RECEIVER_FLAG/
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_REGISTER_RECEIVER_FLAG/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_REGISTER_RECEIVER_FLAG/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_REGISTER_RECEIVER_FLAG/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.989477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INTENT_REDIRECTION/
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INTENT_REDIRECTION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INTENT_REDIRECTION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INTENT_REDIRECTION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.989477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/PATH_TRAVERSAL/
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/PATH_TRAVERSAL/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/PATH_TRAVERSAL/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/PATH_TRAVERSAL/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.989477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/REDIS_LIBRARY/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/REDIS_LIBRARY/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/REDIS_LIBRARY/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/REDIS_LIBRARY/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.989477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/STACK_TRACE_INFORMATION_DISCLOSURE/
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/STACK_TRACE_INFORMATION_DISCLOSURE/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/STACK_TRACE_INFORMATION_DISCLOSURE/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/STACK_TRACE_INFORMATION_DISCLOSURE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.989477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/UNTRUSTED_EXTERNAL_STORAGE_ACCESS/
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/UNTRUSTED_EXTERNAL_STORAGE_ACCESS/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/UNTRUSTED_EXTERNAL_STORAGE_ACCESS/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/UNTRUSTED_EXTERNAL_STORAGE_ACCESS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.989477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/WEBVIEW_LOADURL_INJECTION/
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/WEBVIEW_LOADURL_INJECTION/context.md
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/WEBVIEW_LOADURL_INJECTION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/WEBVIEW_LOADURL_INJECTION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/WEBVIEW_LOADURL_INJECTION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.913477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.993477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/APK_BACKUP_TITLE/
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/APK_BACKUP_TITLE/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/APK_BACKUP_TITLE/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/APK_BACKUP_TITLE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.993477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/APK_SERVICE_WITHOUT_PERMISSION/
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/APK_SERVICE_WITHOUT_PERMISSION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/APK_SERVICE_WITHOUT_PERMISSION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/APK_SERVICE_WITHOUT_PERMISSION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.993477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/SOURCE_TO_SINK/
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/SOURCE_TO_SINK/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/SOURCE_TO_SINK/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/SOURCE_TO_SINK/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.913477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.993477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_BACKUP_SECURE/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_BACKUP_SECURE/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_BACKUP_SECURE/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_BACKUP_SECURE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.993477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_CHECK_ROOT/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_CHECK_ROOT/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_CHECK_ROOT/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_CHECK_ROOT/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.993477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_DEBUG_SECURE/
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_DEBUG_SECURE/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_DEBUG_SECURE/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_DEBUG_SECURE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.993477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_INSECURE_NETWORK_SECURITY_CONFIG_SECURE/
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_INSECURE_NETWORK_SECURITY_CONFIG_SECURE/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_INSECURE_NETWORK_SECURITY_CONFIG_SECURE/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_INSECURE_NETWORK_SECURITY_CONFIG_SECURE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.917477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.913477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/SECURE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.993477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/SECURE/SECURE_REPUTATION/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/SECURE/SECURE_REPUTATION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/SECURE/SECURE_REPUTATION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/SECURE/SECURE_REPUTATION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.997477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/SECURE/SECURE_VIRUSTOTAL_SCAN/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/SECURE/SECURE_VIRUSTOTAL_SCAN/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/SECURE/SECURE_VIRUSTOTAL_SCAN/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/SECURE/SECURE_VIRUSTOTAL_SCAN/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.913477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.997477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/DEPENDENCY_CONFUSION/
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/DEPENDENCY_CONFUSION/context.md
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/DEPENDENCY_CONFUSION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/DEPENDENCY_CONFUSION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/DEPENDENCY_CONFUSION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.997477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/FORMAT_STRING/
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/FORMAT_STRING/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/FORMAT_STRING/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/FORMAT_STRING/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.917477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.997477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/CORS_MISCONFIGURATION/
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/CORS_MISCONFIGURATION/context.md
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/CORS_MISCONFIGURATION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/CORS_MISCONFIGURATION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/CORS_MISCONFIGURATION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.997477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/DEPRECATED_COMPONENT/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/DEPRECATED_COMPONENT/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/DEPRECATED_COMPONENT/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/DEPRECATED_COMPONENT/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.997477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_HOSTNAME_VALIDATION/
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_HOSTNAME_VALIDATION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_HOSTNAME_VALIDATION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_HOSTNAME_VALIDATION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.997477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_JWT_SIGNATURE/
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_JWT_SIGNATURE/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_JWT_SIGNATURE/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_JWT_SIGNATURE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.001477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_REPUTATION/
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_REPUTATION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_REPUTATION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_REPUTATION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.001477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_STORAGE/
--rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_STORAGE/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_STORAGE/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_STORAGE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.001477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_VIRUSTOTAL_SCAN/
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_VIRUSTOTAL_SCAN/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_VIRUSTOTAL_SCAN/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_VIRUSTOTAL_SCAN/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.001477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/LEAKING_HEALTH_INFORMATION/
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/LEAKING_HEALTH_INFORMATION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/LEAKING_HEALTH_INFORMATION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/LEAKING_HEALTH_INFORMATION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.001477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/LEAKING_PERSONAL_INFORMATION/
--rw-r--r--   0 runner    (1001) docker     (127)     5228 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/LEAKING_PERSONAL_INFORMATION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/LEAKING_PERSONAL_INFORMATION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/LEAKING_PERSONAL_INFORMATION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.001477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/OAUTH_SCHEME_ACCOUNT_TAKEOVER/
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/OAUTH_SCHEME_ACCOUNT_TAKEOVER/context.md
--rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/OAUTH_SCHEME_ACCOUNT_TAKEOVER/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/OAUTH_SCHEME_ACCOUNT_TAKEOVER/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/OAUTH_SCHEME_ACCOUNT_TAKEOVER/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.001477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/REGEX_DOS/
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/REGEX_DOS/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/REGEX_DOS/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     5742 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/REGEX_DOS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.005477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/TAPJACKING_VULNERABILITY/
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/TAPJACKING_VULNERABILITY/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/TAPJACKING_VULNERABILITY/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/TAPJACKING_VULNERABILITY/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.005477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/TEMPLATE_INJECTION/
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/TEMPLATE_INJECTION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/TEMPLATE_INJECTION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/TEMPLATE_INJECTION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.005477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/XPATH_INJECTION/
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/XPATH_INJECTION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/XPATH_INJECTION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/XPATH_INJECTION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.917477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_IMPORTANT/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.005477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_IMPORTANT/PACKAGE_OBFUSCATED/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_IMPORTANT/PACKAGE_OBFUSCATED/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_IMPORTANT/PACKAGE_OBFUSCATED/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_IMPORTANT/PACKAGE_OBFUSCATED/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.917477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_INFO/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.005477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_INFO/DANGEROUS_MEMORY_CORRUPTION/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_INFO/DANGEROUS_MEMORY_CORRUPTION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_INFO/DANGEROUS_MEMORY_CORRUPTION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_INFO/DANGEROUS_MEMORY_CORRUPTION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.005477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_INFO/PRIVACY_API/
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_INFO/PRIVACY_API/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_INFO/PRIVACY_API/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_INFO/PRIVACY_API/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.917477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_LOW/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.005477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_LOW/OUTDATED_VULNERABLE_COMPONENT/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_LOW/OUTDATED_VULNERABLE_COMPONENT/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_LOW/OUTDATED_VULNERABLE_COMPONENT/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_LOW/OUTDATED_VULNERABLE_COMPONENT/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.009477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_LOW/PROCESS_CRASHES/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_LOW/PROCESS_CRASHES/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_LOW/PROCESS_CRASHES/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_LOW/PROCESS_CRASHES/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.917477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.009477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/BIOMETRIC_AUTHENTICATION_BYPASS/
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/BIOMETRIC_AUTHENTICATION_BYPASS/context.md
--rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/BIOMETRIC_AUTHENTICATION_BYPASS/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/BIOMETRIC_AUTHENTICATION_BYPASS/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     8439 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/BIOMETRIC_AUTHENTICATION_BYPASS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.009477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_ALGO/
--rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_ALGO/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_ALGO/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     7184 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_ALGO/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.009477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_KEY/
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_KEY/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_KEY/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_KEY/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.009477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_MODE/
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_MODE/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_MODE/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_MODE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.009477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_IV/
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_IV/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_IV/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_IV/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.009477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/HTML_INJECTION/
--rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/HTML_INJECTION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/HTML_INJECTION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     5181 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/HTML_INJECTION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.009477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_DYNAMICALLY_LINKED_LIBRARY/
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_DYNAMICALLY_LINKED_LIBRARY/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_DYNAMICALLY_LINKED_LIBRARY/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_DYNAMICALLY_LINKED_LIBRARY/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.013477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_PASSWORD_STORAGE/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_PASSWORD_STORAGE/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_PASSWORD_STORAGE/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_PASSWORD_STORAGE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.013477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_PERMISSION_FILESYSTEM/
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_PERMISSION_FILESYSTEM/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_PERMISSION_FILESYSTEM/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_PERMISSION_FILESYSTEM/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.013477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_RANDOM_SEED/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_RANDOM_SEED/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_RANDOM_SEED/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_RANDOM_SEED/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.013477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/LEAKING_CREDENTIALS_LOGS/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/LEAKING_CREDENTIALS_LOGS/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/LEAKING_CREDENTIALS_LOGS/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/LEAKING_CREDENTIALS_LOGS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.013477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/LEAKING_CREDENTIALS_REQUEST/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/LEAKING_CREDENTIALS_REQUEST/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/LEAKING_CREDENTIALS_REQUEST/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/LEAKING_CREDENTIALS_REQUEST/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.013477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/MEMORY_LEAK/
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/MEMORY_LEAK/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/MEMORY_LEAK/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/MEMORY_LEAK/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.013477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/SQL_INJECTION/
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/SQL_INJECTION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/SQL_INJECTION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/SQL_INJECTION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.017477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/WEAK_HASHING_ALGO/
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/WEAK_HASHING_ALGO/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/WEAK_HASHING_ALGO/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/WEAK_HASHING_ALGO/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.017477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/XML_INJECTION/
--rw-r--r--   0 runner    (1001) docker     (127)     7047 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/XML_INJECTION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/XML_INJECTION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     7940 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/XML_INJECTION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.017477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/ZIP_FILE_VULNERABILITIES/
--rw-r--r--   0 runner    (1001) docker     (127)     8698 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/ZIP_FILE_VULNERABILITIES/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/ZIP_FILE_VULNERABILITIES/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)    11939 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/ZIP_FILE_VULNERABILITIES/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.917477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.017477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/PORT_OPEN_LOCALHOST/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/PORT_OPEN_LOCALHOST/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/PORT_OPEN_LOCALHOST/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/PORT_OPEN_LOCALHOST/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.017477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/PRIVACY_CONTINUOUS_GPS_LOCATION_ACCESS/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/PRIVACY_CONTINUOUS_GPS_LOCATION_ACCESS/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/PRIVACY_CONTINUOUS_GPS_LOCATION_ACCESS/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/PRIVACY_CONTINUOUS_GPS_LOCATION_ACCESS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.017477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/SECRETS_REVIEW/
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/SECRETS_REVIEW/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/SECRETS_REVIEW/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/SECRETS_REVIEW/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.017477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/URL_MANIPULATION/
--rw-r--r--   0 runner    (1001) docker     (127)     6656 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/URL_MANIPULATION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/URL_MANIPULATION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     7883 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/URL_MANIPULATION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.921477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.917477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.017477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/ATS_MALFORMATTED/
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/ATS_MALFORMATTED/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/ATS_MALFORMATTED/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/ATS_MALFORMATTED/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.021477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/IPA_ARC_DISABLED/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/IPA_ARC_DISABLED/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/IPA_ARC_DISABLED/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/IPA_ARC_DISABLED/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.021477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/IPA_STACK_SMASHING_DISABLED/
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/IPA_STACK_SMASHING_DISABLED/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/IPA_STACK_SMASHING_DISABLED/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/IPA_STACK_SMASHING_DISABLED/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.917477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.021477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_INSECURE_PRIVACY_MANIFEST_FILE/
--rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_INSECURE_PRIVACY_MANIFEST_FILE/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_INSECURE_PRIVACY_MANIFEST_FILE/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_INSECURE_PRIVACY_MANIFEST_FILE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.021477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_URL_SCHEME_INJECTION/
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_URL_SCHEME_INJECTION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_URL_SCHEME_INJECTION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_URL_SCHEME_INJECTION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.921477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_IMPORTANT/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.021477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_IMPORTANT/IPA_BITCODE/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_IMPORTANT/IPA_BITCODE/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_IMPORTANT/IPA_BITCODE/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_IMPORTANT/IPA_BITCODE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.021477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_IMPORTANT/IPA_ENCRYPTED/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_IMPORTANT/IPA_ENCRYPTED/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_IMPORTANT/IPA_ENCRYPTED/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_IMPORTANT/IPA_ENCRYPTED/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.921477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.021477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_ENTITLEMENTS/
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_ENTITLEMENTS/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_ENTITLEMENTS/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_ENTITLEMENTS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.025478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_FILE_LIST/
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_FILE_LIST/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_FILE_LIST/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_FILE_LIST/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.025478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_FRAMEWORKS_LIST/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_FRAMEWORKS_LIST/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_FRAMEWORKS_LIST/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_FRAMEWORKS_LIST/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.025478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_PLIST_FILES/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_PLIST_FILES/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_PLIST_FILES/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_PLIST_FILES/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.025478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_SYMBOLS/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_SYMBOLS/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_SYMBOLS/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_SYMBOLS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.025478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_URL_SCHEME_LIST/
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_URL_SCHEME_LIST/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_URL_SCHEME_LIST/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_URL_SCHEME_LIST/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.025478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/STRINGS_BPLIST_FILES/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/STRINGS_BPLIST_FILES/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/STRINGS_BPLIST_FILES/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/STRINGS_BPLIST_FILES/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.921477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.025478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/IPA_DEBUG_SYMBOL_PRESENT/
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/IPA_DEBUG_SYMBOL_PRESENT/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/IPA_DEBUG_SYMBOL_PRESENT/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/IPA_DEBUG_SYMBOL_PRESENT/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.025478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/IPA_KEYBOARD_CACHE/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/IPA_KEYBOARD_CACHE/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/IPA_KEYBOARD_CACHE/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/IPA_KEYBOARD_CACHE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.029477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/PLIST_INSECURE_UI_FILE_SHARING/
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/PLIST_INSECURE_UI_FILE_SHARING/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/PLIST_INSECURE_UI_FILE_SHARING/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/PLIST_INSECURE_UI_FILE_SHARING/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.921477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.029477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_ASLR_DISABLED/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_ASLR_DISABLED/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_ASLR_DISABLED/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_ASLR_DISABLED/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.029477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_INSECURE_TAP/
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_INSECURE_TAP/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_INSECURE_TAP/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_INSECURE_TAP/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.029477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_URL_SCHEME_HIJACKING/
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_URL_SCHEME_HIJACKING/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_URL_SCHEME_HIJACKING/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_URL_SCHEME_HIJACKING/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.921477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.029477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/IPA_ANTI_DEBUG/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/IPA_ANTI_DEBUG/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/IPA_ANTI_DEBUG/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/IPA_ANTI_DEBUG/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.029477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/IPA_SECURE_PRIVACY_MANIFEST_FILE/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/IPA_SECURE_PRIVACY_MANIFEST_FILE/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/IPA_SECURE_PRIVACY_MANIFEST_FILE/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/IPA_SECURE_PRIVACY_MANIFEST_FILE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.029477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/PRIVACY_NO_SENSITIVE_DATA_OUTSIDE_APP_CONTAINER/
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/PRIVACY_NO_SENSITIVE_DATA_OUTSIDE_APP_CONTAINER/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/PRIVACY_NO_SENSITIVE_DATA_OUTSIDE_APP_CONTAINER/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/PRIVACY_NO_SENSITIVE_DATA_OUTSIDE_APP_CONTAINER/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.921477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.921477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_HARDENING/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.029477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_HARDENING/PHONEGAP_WHITELIST_CONFIG/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_HARDENING/PHONEGAP_WHITELIST_CONFIG/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_HARDENING/PHONEGAP_WHITELIST_CONFIG/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_HARDENING/PHONEGAP_WHITELIST_CONFIG/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.921477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_HIGH/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.033477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_HIGH/SOURCE_MAP_CODE_LEAK/
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_HIGH/SOURCE_MAP_CODE_LEAK/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_HIGH/SOURCE_MAP_CODE_LEAK/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_HIGH/SOURCE_MAP_CODE_LEAK/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.921477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_LOW/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.033477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_LOW/PHONEGAP_DEBUG_MODE/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_LOW/PHONEGAP_DEBUG_MODE/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_LOW/PHONEGAP_DEBUG_MODE/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_LOW/PHONEGAP_DEBUG_MODE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.921477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_MEDIUM/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.033477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_MEDIUM/CORDOVA_XSS/
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_MEDIUM/CORDOVA_XSS/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_MEDIUM/CORDOVA_XSS/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_MEDIUM/CORDOVA_XSS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.033477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_MEDIUM/PHONEGAP_WEAK_WHITELIST_CONFIG/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_MEDIUM/PHONEGAP_WEAK_WHITELIST_CONFIG/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_MEDIUM/PHONEGAP_WEAK_WHITELIST_CONFIG/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_MEDIUM/PHONEGAP_WEAK_WHITELIST_CONFIG/recommendation.md
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.925477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.921477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/CLOUD/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.921477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/CLOUD/_MEDIUM/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.033477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/CLOUD/_MEDIUM/AWS_S3_PUBLIC_FILELIST_ENABLED/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/CLOUD/_MEDIUM/AWS_S3_PUBLIC_FILELIST_ENABLED/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/CLOUD/_MEDIUM/AWS_S3_PUBLIC_FILELIST_ENABLED/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/CLOUD/_MEDIUM/AWS_S3_PUBLIC_FILELIST_ENABLED/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.921477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/CLOUD/_SECURE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.033477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/CLOUD/_SECURE/FIREBASE_SECURE_DATABASE_PERMISSIONS/
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/CLOUD/_SECURE/FIREBASE_SECURE_DATABASE_PERMISSIONS/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/CLOUD/_SECURE/FIREBASE_SECURE_DATABASE_PERMISSIONS/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/CLOUD/_SECURE/FIREBASE_SECURE_DATABASE_PERMISSIONS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.921477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/DNS/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.921477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/DNS/_MEDIUM/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.033477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/DNS/_MEDIUM/SUBDOMAIN_TAKEOVER/
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/DNS/_MEDIUM/SUBDOMAIN_TAKEOVER/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/DNS/_MEDIUM/SUBDOMAIN_TAKEOVER/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/DNS/_MEDIUM/SUBDOMAIN_TAKEOVER/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.925477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/DNS/_POTENTIALLY/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.037478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/DNS/_POTENTIALLY/EXTERNAL_DNS_INTERACTION/
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/DNS/_POTENTIALLY/EXTERNAL_DNS_INTERACTION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/DNS/_POTENTIALLY/EXTERNAL_DNS_INTERACTION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/DNS/_POTENTIALLY/EXTERNAL_DNS_INTERACTION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.925477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/NETWORK/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.925477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/NETWORK/_INFO/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.037478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/NETWORK/_INFO/NETWORK_PORT_SCAN/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/NETWORK/_INFO/NETWORK_PORT_SCAN/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/NETWORK/_INFO/NETWORK_PORT_SCAN/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/NETWORK/_INFO/NETWORK_PORT_SCAN/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.929477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.925477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.037478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/ACCOUNT_TAKEOVER/
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/ACCOUNT_TAKEOVER/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/ACCOUNT_TAKEOVER/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/ACCOUNT_TAKEOVER/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.037478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/CODE_INJECTION/
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/CODE_INJECTION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/CODE_INJECTION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/CODE_INJECTION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.037478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/COMMAND_INJECTION/
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/COMMAND_INJECTION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/COMMAND_INJECTION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/COMMAND_INJECTION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.037478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/EXPRESSION_LANGUAGE_INJECTION/
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/EXPRESSION_LANGUAGE_INJECTION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/EXPRESSION_LANGUAGE_INJECTION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/EXPRESSION_LANGUAGE_INJECTION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.037478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/FILE_INCLUSION/
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/FILE_INCLUSION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/FILE_INCLUSION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/FILE_INCLUSION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.037478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/NOSQL_INJECTION/
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/NOSQL_INJECTION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/NOSQL_INJECTION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/NOSQL_INJECTION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.041478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SERVER_SIDE_TEMPLATE_INJECTION/
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SERVER_SIDE_TEMPLATE_INJECTION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SERVER_SIDE_TEMPLATE_INJECTION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SERVER_SIDE_TEMPLATE_INJECTION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.041478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SSI_INJECTION/
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SSI_INJECTION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SSI_INJECTION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SSI_INJECTION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.041478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_SQL_INJECTION/
--rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_SQL_INJECTION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_SQL_INJECTION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_SQL_INJECTION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.041478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_XPATH_INJECTION/
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_XPATH_INJECTION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_XPATH_INJECTION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_XPATH_INJECTION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.041478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/XML_EXTERNAL_ENTITY_INJECTION/
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/XML_EXTERNAL_ENTITY_INJECTION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/XML_EXTERNAL_ENTITY_INJECTION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/XML_EXTERNAL_ENTITY_INJECTION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.925477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.041478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_COOKIE_MISSING_SECURITY_FLAGS/
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_COOKIE_MISSING_SECURITY_FLAGS/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_COOKIE_MISSING_SECURITY_FLAGS/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_COOKIE_MISSING_SECURITY_FLAGS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.041478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_CSP/
--rw-r--r--   0 runner    (1001) docker     (127)     4840 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_CSP/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_CSP/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_CSP/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.041478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_CT/
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_CT/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_CT/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_CT/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.045477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_HSTS/
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_HSTS/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_HSTS/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_HSTS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.045477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_RP/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_RP/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_RP/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_RP/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.045477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_XFO/
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_XFO/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_XFO/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_XFO/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.045477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_X_XSS/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_X_XSS/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_X_XSS/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_X_XSS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.045477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_NO_STRICT_TRANSPORT_SECURITY/
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_NO_STRICT_TRANSPORT_SECURITY/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_NO_STRICT_TRANSPORT_SECURITY/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_NO_STRICT_TRANSPORT_SECURITY/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.925477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.045477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/CRLF_INJECTION/
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/CRLF_INJECTION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/CRLF_INJECTION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/CRLF_INJECTION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.045477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/EXPOSED_FIREBASE_DB/
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/EXPOSED_FIREBASE_DB/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/EXPOSED_FIREBASE_DB/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/EXPOSED_FIREBASE_DB/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.049478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/INSECURE_DIRECT_OBJECT_REFERENCE/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/INSECURE_DIRECT_OBJECT_REFERENCE/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/INSECURE_DIRECT_OBJECT_REFERENCE/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/INSECURE_DIRECT_OBJECT_REFERENCE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.049478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/LDAP_INJECTION/
--rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/LDAP_INJECTION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/LDAP_INJECTION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     4982 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/LDAP_INJECTION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.049478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/TLS_HEARTBLEED/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/TLS_HEARTBLEED/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/TLS_HEARTBLEED/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/TLS_HEARTBLEED/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.049478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/TLS_SELFSIGNED/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/TLS_SELFSIGNED/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/TLS_SELFSIGNED/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/TLS_SELFSIGNED/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.049478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_INSECURE_OBJECT_SERIALIZATION/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_INSECURE_OBJECT_SERIALIZATION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_INSECURE_OBJECT_SERIALIZATION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_INSECURE_OBJECT_SERIALIZATION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.049478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_PATH_TRAVERSAL/
--rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_PATH_TRAVERSAL/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_PATH_TRAVERSAL/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_PATH_TRAVERSAL/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.049478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_XML_INJECTION/
--rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_XML_INJECTION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_XML_INJECTION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_XML_INJECTION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.925477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_INFO/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.049478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_INFO/TLS_SERVER_SCAN/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_INFO/TLS_SERVER_SCAN/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_INFO/TLS_SERVER_SCAN/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_INFO/TLS_SERVER_SCAN/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.053478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_INFO/WEB_INTERESTING_RESPONSE/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_INFO/WEB_INTERESTING_RESPONSE/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_INFO/WEB_INTERESTING_RESPONSE/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_INFO/WEB_INTERESTING_RESPONSE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.929477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.053478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/DJANGO_DEBUG_MODE/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/DJANGO_DEBUG_MODE/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/DJANGO_DEBUG_MODE/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/DJANGO_DEBUG_MODE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.053478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/USER_ENUMERATION/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/USER_ENUMERATION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/USER_ENUMERATION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/USER_ENUMERATION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.053478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/WEB_GENERIC/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/WEB_GENERIC/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/WEB_GENERIC/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/WEB_GENERIC/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.053478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/WEB_HTTP_HEADER/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/WEB_HTTP_HEADER/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/WEB_HTTP_HEADER/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/WEB_HTTP_HEADER/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.929477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.053478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/CROSS_ORIGIN_RESOURCE_SHARING/
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/CROSS_ORIGIN_RESOURCE_SHARING/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/CROSS_ORIGIN_RESOURCE_SHARING/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/CROSS_ORIGIN_RESOURCE_SHARING/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.053478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/INSECURE_TLS_VALIDATION/
--rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/INSECURE_TLS_VALIDATION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/INSECURE_TLS_VALIDATION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/INSECURE_TLS_VALIDATION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.053478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_ANONSERVER/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_ANONSERVER/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_ANONSERVER/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_ANONSERVER/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.057478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_DEPRECATED_PROTOCOL/
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_DEPRECATED_PROTOCOL/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_DEPRECATED_PROTOCOL/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_DEPRECATED_PROTOCOL/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.057478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_HTTP/
--rw-r--r--   0 runner    (1001) docker     (127)     8594 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_HTTP/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_HTTP/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     9366 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_HTTP/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.057478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_INSECURE_CIPHER/
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_INSECURE_CIPHER/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_INSECURE_CIPHER/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_INSECURE_CIPHER/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.057478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_INVALIDHOSTNAME/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_INVALIDHOSTNAME/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_INVALIDHOSTNAME/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_INVALIDHOSTNAME/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.057478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_HTTP_HOST_HEADER_POISONING/
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_HTTP_HOST_HEADER_POISONING/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_HTTP_HOST_HEADER_POISONING/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_HTTP_HOST_HEADER_POISONING/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.057478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_IDOR/
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_IDOR/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_IDOR/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_IDOR/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.057478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_INSECURE_ACCESS_CONTROL/
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_INSECURE_ACCESS_CONTROL/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_INSECURE_ACCESS_CONTROL/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_INSECURE_ACCESS_CONTROL/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.061478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_UNRESTRICTED_FILE_UPLOAD/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_UNRESTRICTED_FILE_UPLOAD/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_UNRESTRICTED_FILE_UPLOAD/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_UNRESTRICTED_FILE_UPLOAD/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.061478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_XSS/
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_XSS/description.md
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_XSS/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_XSS/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.929477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_POTENTIALLY/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.061478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_POTENTIALLY/SECRETS_NETWORK_REVIEW/
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_POTENTIALLY/SECRETS_NETWORK_REVIEW/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_POTENTIALLY/SECRETS_NETWORK_REVIEW/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_POTENTIALLY/SECRETS_NETWORK_REVIEW/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:52.929477 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.061478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/SECURE_AUTHENTICATION/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/SECURE_AUTHENTICATION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/SECURE_AUTHENTICATION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/SECURE_AUTHENTICATION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.061478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/TLS_INVALIDHOSTNAME_SECURE/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/TLS_INVALIDHOSTNAME_SECURE/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/TLS_INVALIDHOSTNAME_SECURE/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/TLS_INVALIDHOSTNAME_SECURE/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.061478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/UNIQUE_USER_IDENTIFICATION/
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/UNIQUE_USER_IDENTIFICATION/description.md
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/UNIQUE_USER_IDENTIFICATION/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/UNIQUE_USER_IDENTIFICATION/recommendation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.061478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    17461 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/tests/kb_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.061478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/tests/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/tests/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/tests/tools/kb_generator_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.065478 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8817 2024-04-19 13:17:39.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/KB/tools/kb_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/kb/kb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.065478 ostorlab-1.0.7/src/ostorlab/agent/message/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.065478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.065478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.065478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/common/x509/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/common/x509/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/common/x509/x509_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.065478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.065478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.065478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/agent/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/agent/agent_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.065478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/domain_name/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/domain_name/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.065478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/domain_name/dns_record/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/domain_name/dns_record/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/domain_name/dns_record/dns_record_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/domain_name/domain_name_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.065478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/domain_name/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/domain_name/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/domain_name/service/service_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.065478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/domain_name/whois/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/domain_name/whois/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/domain_name/whois/whois_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.069478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/file/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.069478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/file/android/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/file/android/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.069478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/file/android/aab/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/file/android/aab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/file/android/aab/aab_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.069478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/file/android/apk/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/file/android/apk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/file/android/apk/apk_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/file/file_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.069478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/file/ios/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/file/ios/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.069478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/file/ios/ipa/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/file/ios/ipa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/file/ios/ipa/ipa_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.069478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/file/sbom/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/file/sbom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/file/sbom/sbom_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.069478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/file/source/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/file/source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/file/source/source_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.069478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/ip/
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/ip/ip_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.069478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/ip/v4/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/ip/v4/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.069478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/ip/v4/geolocation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/ip/v4/geolocation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/ip/v4/geolocation/geolocation_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.069478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/port_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.069478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.069478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/service/http/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/service/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/service/http/http_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/service/service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/ip/v4/v4_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.073478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/ip/v4/whois/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/ip/v4/whois/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/ip/v4/whois/whois_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.073478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/ip/v6/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/ip/v6/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.073478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/ip/v6/geolocation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/ip/v6/geolocation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/ip/v6/geolocation/geolocation_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.073478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/port_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.073478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.073478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/service/http/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/service/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/service/http/http_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/service/service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/ip/v6/v6_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.073478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/ip/v6/whois/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/ip/v6/whois/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/ip/v6/whois/whois_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.073478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/link/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/link/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/link/link_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.073478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/store/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/store/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.073478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/store/android_store/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/store/android_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/store/android_store/android_store_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.073478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/store/android_store/developer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/store/android_store/developer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/store/android_store/developer/developer_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.073478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/store/ios_store/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/store/ios_store/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.077478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/store/ios_store/developer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/store/ios_store/developer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/store/ios_store/developer/developer_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/store/ios_store/ios_store_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.077478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/capture/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/capture/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.077478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/capture/artifact/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/capture/artifact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/capture/artifact/artifact_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.077478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/capture/filesystem/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/capture/filesystem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/capture/filesystem/filesystem_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.077478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/capture/http/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/capture/http/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.077478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/capture/http/request/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/capture/http/request/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/capture/http/request/request_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.077478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/capture/http/response/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/capture/http/response/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/capture/http/response/response_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.077478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/capture/logs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/capture/logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/capture/logs/logs_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.077478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/capture/request_response/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/capture/request_response/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/capture/request_response/request_response_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.077478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/capture/ui_call/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/capture/ui_call/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/capture/ui_call/ui_call_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.077478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/control/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/control/control_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.077478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.077478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.077478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.077478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/library/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/library/library_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.081478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/x509/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/x509/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/x509/x509_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.081478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/file/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.081478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.081478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/backend/backend_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.081478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/feature/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/feature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4525 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/feature/feature_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.081478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/library/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5089 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/library/library_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.081478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/metadata/metadata_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.081478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/file/feature/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/file/feature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/file/feature/feature_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/file/file_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.081478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.081478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/backend/backend_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.081478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/feature/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/feature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/feature/feature_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.081478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/library/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/library/library_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.081478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/metadata/metadata_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.085478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/file/library/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/file/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4454 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/file/library/library_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.085478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/ip/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/ip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.085478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.085478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.085478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/library/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/library/library_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.085478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/x509/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/x509/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/x509/x509_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.085478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.085478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.085478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/library/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/library/library_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.085478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/x509/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/x509/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/x509/x509_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.085478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/healthcheck/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/healthcheck/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.085478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/healthcheck/ping/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/healthcheck/ping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/healthcheck/ping/ping_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.085478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/report/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/report/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.085478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/report/cve/
--rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/report/cve/cve_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.085478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/report/event/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/report/event/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.085478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/report/event/post_scan/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/report/event/post_scan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.089478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/report/event/post_scan/done/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/report/event/post_scan/done/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/report/event/post_scan/done/done_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.089478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/report/event/post_scan/start/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/report/event/post_scan/start/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/report/event/post_scan/start/start_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.089478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/report/event/post_scan/timeout/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/report/event/post_scan/timeout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/report/event/post_scan/timeout/timeout_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.089478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/report/event/scan/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/report/event/scan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.089478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/report/event/scan/done/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/report/event/scan/done/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/report/event/scan/done/done_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.089478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/report/event/scan/start/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/report/event/scan/start/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/report/event/scan/start/start_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.089478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/report/event/scan/timeout/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/report/event/scan/timeout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/report/event/scan/timeout/timeout_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.089478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/report/status/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/report/status/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/report/status/status_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.089478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/report/vulnerability/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/report/vulnerability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7099 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/report/vulnerability/vulnerability_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.089478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/use/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/use/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.089478 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/use/device/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/use/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/use/device/device_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/proto_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/message/serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.089478 ostorlab-1.0.7/src/ostorlab/agent/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/mixins/agent_healthcheck_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7801 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/mixins/agent_mq_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    11005 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/mixins/agent_open_telemetry_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     9167 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/mixins/agent_persist_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/mixins/agent_report_vulnerability_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.093478 ostorlab-1.0.7/src/ostorlab/agent/mixins/protocols/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/mixins/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/mixins/protocols/emit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.093478 ostorlab-1.0.7/src/ostorlab/agent/schema/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/schema/agent_group_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     6114 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/schema/agent_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/schema/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/schema/target_group_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/agent/schema/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.097478 ostorlab-1.0.7/src/ostorlab/apis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/apis/add_scanner_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/apis/agent_details.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/apis/agent_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/apis/agent_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     6162 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/apis/assets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/apis/create_agent_scan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/apis/create_api_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/apis/login.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/apis/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/apis/revoke_api_key.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.097478 ostorlab-1.0.7/src/ostorlab/apis/runners/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/apis/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8327 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/apis/runners/authenticated_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/apis/runners/login_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/apis/runners/public_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/apis/runners/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/apis/scan_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/apis/scan_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/apis/scan_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/apis/scan_stop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/apis/scanner_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/apis/test_credentials_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/apis/vulnz_describe.py
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/apis/vulnz_list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.097478 ostorlab-1.0.7/src/ostorlab/assets/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/assets/TODO.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/assets/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/assets/android_aab.py
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/assets/android_apk.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/assets/android_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/assets/asset.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/assets/domain_name.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/assets/file.py
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/assets/ios_ipa.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/assets/ios_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/assets/ip.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/assets/ipv4.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/assets/ipv6.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/assets/link.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.101478 ostorlab-1.0.7/src/ostorlab/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.101478 ostorlab-1.0.7/src/ostorlab/cli/agent/
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/agent/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.101478 ostorlab-1.0.7/src/ostorlab/cli/agent/build/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/agent/build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5003 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/agent/build/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/agent/build/build_progress.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.101478 ostorlab-1.0.7/src/ostorlab/cli/agent/delete/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/agent/delete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/agent/delete/delete.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.101478 ostorlab-1.0.7/src/ostorlab/cli/agent/healthcheck/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/agent/healthcheck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/agent/healthcheck/healthcheck.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.101478 ostorlab-1.0.7/src/ostorlab/cli/agent/install/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/agent/install/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/agent/install/install.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/agent/install/install_progress.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.101478 ostorlab-1.0.7/src/ostorlab/cli/agent/list/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/agent/list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/agent/list/list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.105478 ostorlab-1.0.7/src/ostorlab/cli/agent/search/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/agent/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/agent/search/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/agent_fetcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.105478 ostorlab-1.0.7/src/ostorlab/cli/agentgroup/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/agentgroup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/agentgroup/agentgroup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.105478 ostorlab-1.0.7/src/ostorlab/cli/auth/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/auth/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.105478 ostorlab-1.0.7/src/ostorlab/cli/auth/login/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/auth/login/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/auth/login/login.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.105478 ostorlab-1.0.7/src/ostorlab/cli/auth/revoke/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/auth/revoke/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/auth/revoke/revoke.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.105478 ostorlab-1.0.7/src/ostorlab/cli/ci_scan/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/ci_scan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/ci_scan/ci_scan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.105478 ostorlab-1.0.7/src/ostorlab/cli/ci_scan/run/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/ci_scan/run/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.105478 ostorlab-1.0.7/src/ostorlab/cli/ci_scan/run/assets/
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/ci_scan/run/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/ci_scan/run/assets/android_aab.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/ci_scan/run/assets/android_apk.py
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/ci_scan/run/assets/ios_ipa.py
--rw-r--r--   0 runner    (1001) docker     (127)     5041 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/ci_scan/run/assets/mobile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.105478 ostorlab-1.0.7/src/ostorlab/cli/ci_scan/run/ci_logger/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/ci_scan/run/ci_logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/ci_scan/run/ci_logger/circleci_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/ci_scan/run/ci_logger/console_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/ci_scan/run/ci_logger/github_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/ci_scan/run/ci_logger/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     8729 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/ci_scan/run/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/console.py
--rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/docker_requirements_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/dumpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/input_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/install_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/rootcli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.109478 ostorlab-1.0.7/src/ostorlab/cli/scan/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/scan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.109478 ostorlab-1.0.7/src/ostorlab/cli/scan/list/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/scan/list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/scan/list/list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.109478 ostorlab-1.0.7/src/ostorlab/cli/scan/run/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/scan/run/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.109478 ostorlab-1.0.7/src/ostorlab/cli/scan/run/assets/
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/scan/run/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/scan/run/assets/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/scan/run/assets/android_aab.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/scan/run/assets/android_apk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/scan/run/assets/android_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/scan/run/assets/domain_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/scan/run/assets/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/scan/run/assets/ios_ipa.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/scan/run/assets/ios_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/scan/run/assets/ip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/scan/run/assets/link.py
--rw-r--r--   0 runner    (1001) docker     (127)     8702 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/scan/run/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/scan/scan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.109478 ostorlab-1.0.7/src/ostorlab/cli/scan/stop/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/scan/stop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/scan/stop/stop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.109478 ostorlab-1.0.7/src/ostorlab/cli/scanner/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/scanner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/scanner/scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.113478 ostorlab-1.0.7/src/ostorlab/cli/vulnz/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/vulnz/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.113478 ostorlab-1.0.7/src/ostorlab/cli/vulnz/describe/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/vulnz/describe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/vulnz/describe/describe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.113478 ostorlab-1.0.7/src/ostorlab/cli/vulnz/dump/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/vulnz/dump/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/vulnz/dump/dump.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.113478 ostorlab-1.0.7/src/ostorlab/cli/vulnz/list/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/vulnz/list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/vulnz/list/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/cli/vulnz/vulnz.py
--rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/configuration_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/main.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.113478 ostorlab-1.0.7/src/ostorlab/runtimes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/runtimes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.113478 ostorlab-1.0.7/src/ostorlab/runtimes/cloud/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/runtimes/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25003 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/runtimes/cloud/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)    14599 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/runtimes/definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.113478 ostorlab-1.0.7/src/ostorlab/runtimes/lite_local/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/runtimes/lite_local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15307 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/runtimes/lite_local/agent_runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)    14379 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/runtimes/lite_local/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.113478 ostorlab-1.0.7/src/ostorlab/runtimes/local/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/runtimes/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14839 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/runtimes/local/agent_runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/runtimes/local/log_streamer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.113478 ostorlab-1.0.7/src/ostorlab/runtimes/local/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/runtimes/local/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.117478 ostorlab-1.0.7/src/ostorlab/runtimes/local/models/alembic/
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/runtimes/local/models/alembic/env.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/runtimes/local/models/alembic/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.117478 ostorlab-1.0.7/src/ostorlab/runtimes/local/models/alembic/versions/
--rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/runtimes/local/models/alembic/versions/35cd577ef0e5_.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/runtimes/local/models/alembic/versions/746c5eb3d181_add_vulnerability_location.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/runtimes/local/models/alembic/versions/7d12204c3f27_add_references_field_to_vulnerability.py
--rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/runtimes/local/models/alembic.ini
--rw-r--r--   0 runner    (1001) docker     (127)    11189 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/runtimes/local/models/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    30185 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/runtimes/local/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.117478 ostorlab-1.0.7/src/ostorlab/runtimes/local/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/runtimes/local/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.117478 ostorlab-1.0.7/src/ostorlab/runtimes/local/services/configurations/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/runtimes/local/services/configurations/mq_advanced_conf.config
--rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/runtimes/local/services/jaeger.py
--rw-r--r--   0 runner    (1001) docker     (127)     6784 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/runtimes/local/services/mq.py
--rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/runtimes/local/services/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.117478 ostorlab-1.0.7/src/ostorlab/runtimes/proto/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/runtimes/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/runtimes/proto/agent_instance_settings_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/runtimes/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/runtimes/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.117478 ostorlab-1.0.7/src/ostorlab/scanner/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/scanner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6786 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/scanner/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     7475 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/scanner/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.117478 ostorlab-1.0.7/src/ostorlab/scanner/proto/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/scanner/proto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.121478 ostorlab-1.0.7/src/ostorlab/scanner/proto/assets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/scanner/proto/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/scanner/proto/assets/aab_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/scanner/proto/assets/agent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/scanner/proto/assets/android_store_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/scanner/proto/assets/apk_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/scanner/proto/assets/domain_name_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/scanner/proto/assets/file_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/scanner/proto/assets/ios_store_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/scanner/proto/assets/ip_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/scanner/proto/assets/ipa_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/scanner/proto/assets/link_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/scanner/proto/assets/network_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/scanner/proto/assets/source_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/scanner/proto/assets/v4_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/scanner/proto/assets/v6_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.121478 ostorlab-1.0.7/src/ostorlab/scanner/proto/scan/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/scanner/proto/scan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.121478 ostorlab-1.0.7/src/ostorlab/scanner/proto/scan/_location/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/scanner/proto/scan/_location/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/scanner/proto/scan/_location/startAgentScan_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/scanner/scan_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/scanner/scanner_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.121478 ostorlab-1.0.7/src/ostorlab/testing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7703 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/testing/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.125478 ostorlab-1.0.7/src/ostorlab/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/utils/defintions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/utils/dictionary_minifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/utils/ip.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/utils/risk_rating.py
--rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/utils/scanner_state_reporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/utils/strings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/utils/styles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/utils/system.py
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/utils/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-04-19 13:17:38.000000 ostorlab-1.0.7/src/ostorlab/utils/volumes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:17:53.125478 ostorlab-1.0.7/src/ostorlab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14982 2024-04-19 13:17:52.000000 ostorlab-1.0.7/src/ostorlab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    80112 2024-04-19 13:17:52.000000 ostorlab-1.0.7/src/ostorlab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 13:17:52.000000 ostorlab-1.0.7/src/ostorlab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-19 13:17:52.000000 ostorlab-1.0.7/src/ostorlab.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 13:17:52.000000 ostorlab-1.0.7/src/ostorlab.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-19 13:17:52.000000 ostorlab-1.0.7/src/ostorlab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-19 13:17:52.000000 ostorlab-1.0.7/src/ostorlab.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.471431 ostorlab-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-30 12:07:57.000000 ostorlab-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8965 2024-04-30 12:08:02.471431 ostorlab-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6855 2024-04-30 12:07:57.000000 ostorlab-1.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-04-30 12:08:02.471431 ostorlab-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-30 12:07:57.000000 ostorlab-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.239430 ostorlab-1.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.287430 ostorlab-1.0.8/src/ostorlab/
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.291430 ostorlab-1.0.8/src/ostorlab/agent/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21209 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.291430 ostorlab-1.0.8/src/ostorlab/agent/kb/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.291430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.259430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.251430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.239430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.291430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_DEBUG/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_DEBUG/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_DEBUG/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_DEBUG/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.291430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_ELF_NOTPROTECTED/
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_ELF_NOTPROTECTED/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_ELF_NOTPROTECTED/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_ELF_NOTPROTECTED/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.291430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_INSECURE_NETWORK_SECURITY_CONFIG/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_INSECURE_NETWORK_SECURITY_CONFIG/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_INSECURE_NETWORK_SECURITY_CONFIG/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_INSECURE_NETWORK_SECURITY_CONFIG/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.291430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_NOT_OBFUSCATED/
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_NOT_OBFUSCATED/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_NOT_OBFUSCATED/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_NOT_OBFUSCATED/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.243430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.295430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_FILE_PROVIDER_PERMISSIVE_EXTERNAL_PATH/
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_FILE_PROVIDER_PERMISSIVE_EXTERNAL_PATH/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_FILE_PROVIDER_PERMISSIVE_EXTERNAL_PATH/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_FILE_PROVIDER_PERMISSIVE_EXTERNAL_PATH/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.295430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_INSECURE_EXEC_CMD/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_INSECURE_EXEC_CMD/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_INSECURE_EXEC_CMD/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_INSECURE_EXEC_CMD/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.295430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_NOTIFICATION_SPOOFING/
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_NOTIFICATION_SPOOFING/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_NOTIFICATION_SPOOFING/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_NOTIFICATION_SPOOFING/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.295430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_WIFI_API_PII/
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_WIFI_API_PII/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_WIFI_API_PII/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_WIFI_API_PII/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.295430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/INSECURE_PACKAGE_CONTEXT/
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/INSECURE_PACKAGE_CONTEXT/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/INSECURE_PACKAGE_CONTEXT/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/INSECURE_PACKAGE_CONTEXT/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.243430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_IMPORTANT/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.295430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_IMPORTANT/APK_EXPORTED/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_IMPORTANT/APK_EXPORTED/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_IMPORTANT/APK_EXPORTED/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_IMPORTANT/APK_EXPORTED/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.295430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_IMPORTANT/APK_SCREENSHOT_DISABLED/
+-rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_IMPORTANT/APK_SCREENSHOT_DISABLED/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_IMPORTANT/APK_SCREENSHOT_DISABLED/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_IMPORTANT/APK_SCREENSHOT_DISABLED/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.247430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.299430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_ANALYZE_JNI_ELF/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_ANALYZE_JNI_ELF/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_ANALYZE_JNI_ELF/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_ANALYZE_JNI_ELF/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.299430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_ATTACK_SURFACE/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_ATTACK_SURFACE/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_ATTACK_SURFACE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_ATTACK_SURFACE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.299430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_CERTIFICAT_INFO/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_CERTIFICAT_INFO/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_CERTIFICAT_INFO/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_CERTIFICAT_INFO/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.299430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_CLASSES/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_CLASSES/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_CLASSES/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_CLASSES/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.299430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_CONST_STRINGS/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_CONST_STRINGS/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_CONST_STRINGS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_CONST_STRINGS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.299430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_CODE_LOAD/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_CODE_LOAD/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_CODE_LOAD/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_CODE_LOAD/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.299430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_COMMAND_EXEC/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_COMMAND_EXEC/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_COMMAND_EXEC/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_COMMAND_EXEC/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.303430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_CRYPTO/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_CRYPTO/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_CRYPTO/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_CRYPTO/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.303430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_FILESYSTEM/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_FILESYSTEM/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_FILESYSTEM/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_FILESYSTEM/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.303430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_HASH/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_HASH/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_HASH/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_HASH/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.303430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_HTTP/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_HTTP/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_HTTP/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_HTTP/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.303430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_INTENT/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_INTENT/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_INTENT/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_INTENT/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.303430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_IPC/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_IPC/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_IPC/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_IPC/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.303430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_LOGGING/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_LOGGING/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_LOGGING/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_LOGGING/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.307430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_PROCESS/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_PROCESS/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_PROCESS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_PROCESS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.307430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SERIALIZATION/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SERIALIZATION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SERIALIZATION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SERIALIZATION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.307430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SHARED_PREFERENCES/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SHARED_PREFERENCES/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SHARED_PREFERENCES/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SHARED_PREFERENCES/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.307430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SQLITE/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SQLITE/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SQLITE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SQLITE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.307430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SSL_PINNING/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SSL_PINNING/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SSL_PINNING/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SSL_PINNING/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.307430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_TLS/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_TLS/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_TLS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_TLS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.307430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_WEBVIEW/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_WEBVIEW/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_WEBVIEW/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_WEBVIEW/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.307430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_FILEOBSERVER_IMPL/
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_FILEOBSERVER_IMPL/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_FILEOBSERVER_IMPL/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_FILEOBSERVER_IMPL/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.311430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_FILE_LIST/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_FILE_LIST/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_FILE_LIST/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_FILE_LIST/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.311430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_HARDCODED_SQLS/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_HARDCODED_SQLS/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_HARDCODED_SQLS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_HARDCODED_SQLS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.311430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_HARDCODED_URLS/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_HARDCODED_URLS/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_HARDCODED_URLS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_HARDCODED_URLS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.311430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_LIST_PERMISSIONS/
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_LIST_PERMISSIONS/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_LIST_PERMISSIONS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_LIST_PERMISSIONS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.311430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_MANIFEST/
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_MANIFEST/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_MANIFEST/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_MANIFEST/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.311430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_OBFUSCTAED/
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_OBFUSCTAED/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_OBFUSCTAED/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_OBFUSCTAED/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.311430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_WEBVIEWCLIENT_IMPL/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_WEBVIEWCLIENT_IMPL/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_WEBVIEWCLIENT_IMPL/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_WEBVIEWCLIENT_IMPL/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.315430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/BROADCAST_RECEIVER_DYNAMIC_REGISTRATION/
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/BROADCAST_RECEIVER_DYNAMIC_REGISTRATION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/BROADCAST_RECEIVER_DYNAMIC_REGISTRATION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/BROADCAST_RECEIVER_DYNAMIC_REGISTRATION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.315430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_ANDROIDSECURITY/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_ANDROIDSECURITY/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_ANDROIDSECURITY/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_ANDROIDSECURITY/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.315430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_BLUETOOTH/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_BLUETOOTH/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_BLUETOOTH/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_BLUETOOTH/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.315430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_CRYPTO/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_CRYPTO/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_CRYPTO/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_CRYPTO/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.315430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_DELETE_FILE/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_DELETE_FILE/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_DELETE_FILE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_DELETE_FILE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.315430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_DYNAMIC_CODE_LOADING/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_DYNAMIC_CODE_LOADING/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_DYNAMIC_CODE_LOADING/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_DYNAMIC_CODE_LOADING/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.315430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_EXEC/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_EXEC/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_EXEC/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_EXEC/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.319430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_EXTERNAL_STORAGE/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_EXTERNAL_STORAGE/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_EXTERNAL_STORAGE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_EXTERNAL_STORAGE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.319430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_IPC/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_IPC/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_IPC/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_IPC/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.319430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_LOG/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_LOG/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_LOG/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_LOG/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.319430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_NATIVE/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_NATIVE/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_NATIVE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_NATIVE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.319430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_RANDOM/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_RANDOM/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_RANDOM/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_RANDOM/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.319430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_REFLECTION/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_REFLECTION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_REFLECTION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_REFLECTION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.319430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_SOCKET/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_SOCKET/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_SOCKET/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_SOCKET/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.323430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_SQL/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_SQL/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_SQL/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_SQL/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.323430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_SSLTLS/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_SSLTLS/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_SSLTLS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_SSLTLS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.323430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_WEBVIEW/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_WEBVIEW/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_WEBVIEW/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_WEBVIEW/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.323430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_XML/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_XML/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_XML/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_XML/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.323430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_ZIP/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_ZIP/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_ZIP/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_ZIP/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.323430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/EXPANSION_APK/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/EXPANSION_APK/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/EXPANSION_APK/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/EXPANSION_APK/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.247430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.323430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_DEBUG_SYMBOL_PRESENT/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_DEBUG_SYMBOL_PRESENT/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_DEBUG_SYMBOL_PRESENT/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_DEBUG_SYMBOL_PRESENT/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.327430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_FACEBOOK_REACT_DEV_SETTINGS_ENABLED/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_FACEBOOK_REACT_DEV_SETTINGS_ENABLED/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_FACEBOOK_REACT_DEV_SETTINGS_ENABLED/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_FACEBOOK_REACT_DEV_SETTINGS_ENABLED/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.327430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_HAS_FRAGILE_USER_DATA_NOT_SET/
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_HAS_FRAGILE_USER_DATA_NOT_SET/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_HAS_FRAGILE_USER_DATA_NOT_SET/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_HAS_FRAGILE_USER_DATA_NOT_SET/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.327430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_LIST_NOT_USED_PERMISSIONS/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_LIST_NOT_USED_PERMISSIONS/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_LIST_NOT_USED_PERMISSIONS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_LIST_NOT_USED_PERMISSIONS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.327430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_REQUEST_LEGACY_EXTERNAL_STORAGE/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_REQUEST_LEGACY_EXTERNAL_STORAGE/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_REQUEST_LEGACY_EXTERNAL_STORAGE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_REQUEST_LEGACY_EXTERNAL_STORAGE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.327430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_TASK_HIJACKING/
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_TASK_HIJACKING/context.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_TASK_HIJACKING/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_TASK_HIJACKING/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_TASK_HIJACKING/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.327430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_USES_CLEAR_TEXT_TRAFFIC/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_USES_CLEAR_TEXT_TRAFFIC/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_USES_CLEAR_TEXT_TRAFFIC/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_USES_CLEAR_TEXT_TRAFFIC/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.327430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/DEPRECATED_TARGET_API_VERSION/
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/DEPRECATED_TARGET_API_VERSION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/DEPRECATED_TARGET_API_VERSION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/DEPRECATED_TARGET_API_VERSION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.331431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/INTENT_SPOOFING/
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/INTENT_SPOOFING/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/INTENT_SPOOFING/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/INTENT_SPOOFING/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.331431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/PRIVACY_KEYBOARD_CACHE/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/PRIVACY_KEYBOARD_CACHE/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/PRIVACY_KEYBOARD_CACHE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/PRIVACY_KEYBOARD_CACHE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.251430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.331431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_CERTIFICAT_OUTDATED/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_CERTIFICAT_OUTDATED/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_CERTIFICAT_OUTDATED/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_CERTIFICAT_OUTDATED/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.331431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_FACEBOOK_DEBUG_ENABLED/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_FACEBOOK_DEBUG_ENABLED/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_FACEBOOK_DEBUG_ENABLED/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_FACEBOOK_DEBUG_ENABLED/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.331431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_INSECURE_DOWNLOAD_MANAGER/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_INSECURE_DOWNLOAD_MANAGER/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_INSECURE_DOWNLOAD_MANAGER/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_INSECURE_DOWNLOAD_MANAGER/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.331431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_INSECURE_PATH_CLASS_LOADER/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_INSECURE_PATH_CLASS_LOADER/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_INSECURE_PATH_CLASS_LOADER/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_INSECURE_PATH_CLASS_LOADER/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.331431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_UNDECLARED_PERMISSIONS/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_UNDECLARED_PERMISSIONS/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_UNDECLARED_PERMISSIONS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_UNDECLARED_PERMISSIONS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.335430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/DANGEROUS_API_SETJAVASCRIPTINTERFACE/
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/DANGEROUS_API_SETJAVASCRIPTINTERFACE/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/DANGEROUS_API_SETJAVASCRIPTINTERFACE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/DANGEROUS_API_SETJAVASCRIPTINTERFACE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.335430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/DANGEROUS_API_WEBVIEW_REMOTE_DEBUGGING_ENABLED/
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/DANGEROUS_API_WEBVIEW_REMOTE_DEBUGGING_ENABLED/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/DANGEROUS_API_WEBVIEW_REMOTE_DEBUGGING_ENABLED/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/DANGEROUS_API_WEBVIEW_REMOTE_DEBUGGING_ENABLED/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.335430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/IMPLICIT_PENDINGINTENT/
+-rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/IMPLICIT_PENDINGINTENT/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/IMPLICIT_PENDINGINTENT/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/IMPLICIT_PENDINGINTENT/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.335430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_API_BLUETOOTH/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_API_BLUETOOTH/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_API_BLUETOOTH/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4412 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_API_BLUETOOTH/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.335430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_CLASS_LOADING/
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_CLASS_LOADING/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_CLASS_LOADING/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_CLASS_LOADING/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.335430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_PERMISSION_SHARED_PREFERENCES/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_PERMISSION_SHARED_PREFERENCES/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_PERMISSION_SHARED_PREFERENCES/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_PERMISSION_SHARED_PREFERENCES/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.335430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_REGISTER_RECEIVER_FLAG/
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_REGISTER_RECEIVER_FLAG/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_REGISTER_RECEIVER_FLAG/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_REGISTER_RECEIVER_FLAG/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.335430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INTENT_REDIRECTION/
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INTENT_REDIRECTION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INTENT_REDIRECTION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INTENT_REDIRECTION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.339430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/PATH_TRAVERSAL/
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/PATH_TRAVERSAL/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/PATH_TRAVERSAL/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/PATH_TRAVERSAL/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.339430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/REDIS_LIBRARY/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/REDIS_LIBRARY/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/REDIS_LIBRARY/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/REDIS_LIBRARY/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.339430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/WEBVIEW_LOADURL_INJECTION/
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/WEBVIEW_LOADURL_INJECTION/context.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/WEBVIEW_LOADURL_INJECTION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/WEBVIEW_LOADURL_INJECTION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/WEBVIEW_LOADURL_INJECTION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.251430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.339430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/APK_BACKUP_TITLE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/APK_BACKUP_TITLE/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/APK_BACKUP_TITLE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/APK_BACKUP_TITLE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.339430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/APK_SERVICE_WITHOUT_PERMISSION/
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/APK_SERVICE_WITHOUT_PERMISSION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/APK_SERVICE_WITHOUT_PERMISSION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/APK_SERVICE_WITHOUT_PERMISSION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.339430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/SOURCE_TO_SINK/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/SOURCE_TO_SINK/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/SOURCE_TO_SINK/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/SOURCE_TO_SINK/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.251430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.339430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_BACKUP_SECURE/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_BACKUP_SECURE/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_BACKUP_SECURE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_BACKUP_SECURE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.343430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_CHECK_ROOT/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_CHECK_ROOT/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_CHECK_ROOT/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_CHECK_ROOT/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.343430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_DEBUG_SECURE/
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_DEBUG_SECURE/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_DEBUG_SECURE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_DEBUG_SECURE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.343430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_INSECURE_NETWORK_SECURITY_CONFIG_SECURE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_INSECURE_NETWORK_SECURITY_CONFIG_SECURE/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_INSECURE_NETWORK_SECURITY_CONFIG_SECURE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_INSECURE_NETWORK_SECURITY_CONFIG_SECURE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.255430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.251430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/SECURE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.343430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/SECURE/SECURE_REPUTATION/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/SECURE/SECURE_REPUTATION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/SECURE/SECURE_REPUTATION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/SECURE/SECURE_REPUTATION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.343430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/SECURE/SECURE_VIRUSTOTAL_SCAN/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/SECURE/SECURE_VIRUSTOTAL_SCAN/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/SECURE/SECURE_VIRUSTOTAL_SCAN/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/SECURE/SECURE_VIRUSTOTAL_SCAN/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.251430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.343430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/DEPENDENCY_CONFUSION/
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/DEPENDENCY_CONFUSION/context.md
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/DEPENDENCY_CONFUSION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/DEPENDENCY_CONFUSION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/DEPENDENCY_CONFUSION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.343430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/FORMAT_STRING/
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/FORMAT_STRING/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/FORMAT_STRING/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/FORMAT_STRING/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.255430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.347431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/DEPRECATED_COMPONENT/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/DEPRECATED_COMPONENT/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/DEPRECATED_COMPONENT/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/DEPRECATED_COMPONENT/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.347431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_HOSTNAME_VALIDATION/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_HOSTNAME_VALIDATION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_HOSTNAME_VALIDATION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_HOSTNAME_VALIDATION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.347431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_JWT_SIGNATURE/
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_JWT_SIGNATURE/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_JWT_SIGNATURE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_JWT_SIGNATURE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.347431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_REPUTATION/
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_REPUTATION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_REPUTATION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_REPUTATION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.347431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_STORAGE/
+-rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_STORAGE/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_STORAGE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_STORAGE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.347431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_VIRUSTOTAL_SCAN/
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_VIRUSTOTAL_SCAN/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_VIRUSTOTAL_SCAN/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_VIRUSTOTAL_SCAN/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.347431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/LEAKING_PERSONAL_INFORMATION/
+-rw-r--r--   0 runner    (1001) docker     (127)     5228 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/LEAKING_PERSONAL_INFORMATION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/LEAKING_PERSONAL_INFORMATION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5461 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/LEAKING_PERSONAL_INFORMATION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.351431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/OAUTH_SCHEME_ACCOUNT_TAKEOVER/
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/OAUTH_SCHEME_ACCOUNT_TAKEOVER/context.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/OAUTH_SCHEME_ACCOUNT_TAKEOVER/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/OAUTH_SCHEME_ACCOUNT_TAKEOVER/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/OAUTH_SCHEME_ACCOUNT_TAKEOVER/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.351431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/REGEX_DOS/
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/REGEX_DOS/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/REGEX_DOS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5742 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/REGEX_DOS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.351431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/TAPJACKING_VULNERABILITY/
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/TAPJACKING_VULNERABILITY/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/TAPJACKING_VULNERABILITY/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/TAPJACKING_VULNERABILITY/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.351431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/TEMPLATE_INJECTION/
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/TEMPLATE_INJECTION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/TEMPLATE_INJECTION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/TEMPLATE_INJECTION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.351431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/XPATH_INJECTION/
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/XPATH_INJECTION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/XPATH_INJECTION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/XPATH_INJECTION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.255430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_IMPORTANT/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.351431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_IMPORTANT/PACKAGE_OBFUSCATED/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_IMPORTANT/PACKAGE_OBFUSCATED/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_IMPORTANT/PACKAGE_OBFUSCATED/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_IMPORTANT/PACKAGE_OBFUSCATED/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.255430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_INFO/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.351431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_INFO/DANGEROUS_MEMORY_CORRUPTION/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_INFO/DANGEROUS_MEMORY_CORRUPTION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_INFO/DANGEROUS_MEMORY_CORRUPTION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_INFO/DANGEROUS_MEMORY_CORRUPTION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.355430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_INFO/PRIVACY_API/
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_INFO/PRIVACY_API/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_INFO/PRIVACY_API/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_INFO/PRIVACY_API/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.255430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_LOW/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.355430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_LOW/OUTDATED_VULNERABLE_COMPONENT/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_LOW/OUTDATED_VULNERABLE_COMPONENT/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_LOW/OUTDATED_VULNERABLE_COMPONENT/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_LOW/OUTDATED_VULNERABLE_COMPONENT/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.355430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_LOW/PROCESS_CRASHES/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_LOW/PROCESS_CRASHES/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_LOW/PROCESS_CRASHES/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_LOW/PROCESS_CRASHES/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.255430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.355430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/BIOMETRIC_AUTHENTICATION_BYPASS/
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/BIOMETRIC_AUTHENTICATION_BYPASS/context.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/BIOMETRIC_AUTHENTICATION_BYPASS/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/BIOMETRIC_AUTHENTICATION_BYPASS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8439 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/BIOMETRIC_AUTHENTICATION_BYPASS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.355430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_ALGO/
+-rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_ALGO/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_ALGO/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6350 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_ALGO/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.355430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_KEY/
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_KEY/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_KEY/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_KEY/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.355430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_MODE/
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_MODE/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_MODE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6062 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_MODE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.359430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_IV/
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_IV/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_IV/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_IV/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.359430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/HTML_INJECTION/
+-rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/HTML_INJECTION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/HTML_INJECTION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/HTML_INJECTION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.359430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_DYNAMICALLY_LINKED_LIBRARY/
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_DYNAMICALLY_LINKED_LIBRARY/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_DYNAMICALLY_LINKED_LIBRARY/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_DYNAMICALLY_LINKED_LIBRARY/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.359430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_PASSWORD_STORAGE/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_PASSWORD_STORAGE/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_PASSWORD_STORAGE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_PASSWORD_STORAGE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.359430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_RANDOM_SEED/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_RANDOM_SEED/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_RANDOM_SEED/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_RANDOM_SEED/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.359430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/LEAKING_CREDENTIALS_LOGS/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/LEAKING_CREDENTIALS_LOGS/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/LEAKING_CREDENTIALS_LOGS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/LEAKING_CREDENTIALS_LOGS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.359430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/LEAKING_CREDENTIALS_REQUEST/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/LEAKING_CREDENTIALS_REQUEST/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/LEAKING_CREDENTIALS_REQUEST/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/LEAKING_CREDENTIALS_REQUEST/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.363431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/MEMORY_LEAK/
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/MEMORY_LEAK/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/MEMORY_LEAK/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/MEMORY_LEAK/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.363431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/SQL_INJECTION/
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/SQL_INJECTION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/SQL_INJECTION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/SQL_INJECTION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.363431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/WEAK_HASHING_ALGO/
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/WEAK_HASHING_ALGO/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/WEAK_HASHING_ALGO/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/WEAK_HASHING_ALGO/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.363431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/XML_INJECTION/
+-rw-r--r--   0 runner    (1001) docker     (127)     7047 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/XML_INJECTION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/XML_INJECTION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7928 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/XML_INJECTION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.363431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/ZIP_FILE_VULNERABILITIES/
+-rw-r--r--   0 runner    (1001) docker     (127)     8698 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/ZIP_FILE_VULNERABILITIES/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/ZIP_FILE_VULNERABILITIES/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11823 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/ZIP_FILE_VULNERABILITIES/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.259430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.363431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/PORT_OPEN_LOCALHOST/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/PORT_OPEN_LOCALHOST/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/PORT_OPEN_LOCALHOST/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/PORT_OPEN_LOCALHOST/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.363431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/PRIVACY_CONTINUOUS_GPS_LOCATION_ACCESS/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/PRIVACY_CONTINUOUS_GPS_LOCATION_ACCESS/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/PRIVACY_CONTINUOUS_GPS_LOCATION_ACCESS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/PRIVACY_CONTINUOUS_GPS_LOCATION_ACCESS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.363431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/SECRETS_REVIEW/
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/SECRETS_REVIEW/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/SECRETS_REVIEW/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/SECRETS_REVIEW/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.367431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/URL_MANIPULATION/
+-rw-r--r--   0 runner    (1001) docker     (127)     6656 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/URL_MANIPULATION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/URL_MANIPULATION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7883 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/URL_MANIPULATION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.259430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.259430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.367431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/ATS_MALFORMATTED/
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/ATS_MALFORMATTED/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/ATS_MALFORMATTED/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/ATS_MALFORMATTED/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.367431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/IPA_ARC_DISABLED/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/IPA_ARC_DISABLED/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/IPA_ARC_DISABLED/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/IPA_ARC_DISABLED/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.367431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/IPA_STACK_SMASHING_DISABLED/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/IPA_STACK_SMASHING_DISABLED/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/IPA_STACK_SMASHING_DISABLED/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/IPA_STACK_SMASHING_DISABLED/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.259430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.367431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_INSECURE_PRIVACY_MANIFEST_FILE/
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_INSECURE_PRIVACY_MANIFEST_FILE/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_INSECURE_PRIVACY_MANIFEST_FILE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_INSECURE_PRIVACY_MANIFEST_FILE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.367431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_URL_SCHEME_INJECTION/
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_URL_SCHEME_INJECTION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_URL_SCHEME_INJECTION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_URL_SCHEME_INJECTION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.367431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/UNSAFE_KEYCHAIN_ACCESSIBILITY/
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/UNSAFE_KEYCHAIN_ACCESSIBILITY/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/UNSAFE_KEYCHAIN_ACCESSIBILITY/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/UNSAFE_KEYCHAIN_ACCESSIBILITY/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.259430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_IMPORTANT/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.367431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_IMPORTANT/IPA_BITCODE/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_IMPORTANT/IPA_BITCODE/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_IMPORTANT/IPA_BITCODE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_IMPORTANT/IPA_BITCODE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.371430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_IMPORTANT/IPA_ENCRYPTED/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_IMPORTANT/IPA_ENCRYPTED/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_IMPORTANT/IPA_ENCRYPTED/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_IMPORTANT/IPA_ENCRYPTED/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.259430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.371430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_ENTITLEMENTS/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_ENTITLEMENTS/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_ENTITLEMENTS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_ENTITLEMENTS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.371430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_FILE_LIST/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_FILE_LIST/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_FILE_LIST/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_FILE_LIST/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.371430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_FRAMEWORKS_LIST/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_FRAMEWORKS_LIST/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_FRAMEWORKS_LIST/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_FRAMEWORKS_LIST/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.371430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_PLIST_FILES/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_PLIST_FILES/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_PLIST_FILES/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_PLIST_FILES/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.371430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_SYMBOLS/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_SYMBOLS/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_SYMBOLS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_SYMBOLS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.371430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_URL_SCHEME_LIST/
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_URL_SCHEME_LIST/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_URL_SCHEME_LIST/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_URL_SCHEME_LIST/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.375430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/STRINGS_BPLIST_FILES/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/STRINGS_BPLIST_FILES/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/STRINGS_BPLIST_FILES/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/STRINGS_BPLIST_FILES/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.259430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.375430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/IPA_DEBUG_SYMBOL_PRESENT/
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/IPA_DEBUG_SYMBOL_PRESENT/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/IPA_DEBUG_SYMBOL_PRESENT/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/IPA_DEBUG_SYMBOL_PRESENT/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.375430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/IPA_KEYBOARD_CACHE/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/IPA_KEYBOARD_CACHE/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/IPA_KEYBOARD_CACHE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/IPA_KEYBOARD_CACHE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.375430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/PLIST_INSECURE_UI_FILE_SHARING/
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/PLIST_INSECURE_UI_FILE_SHARING/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/PLIST_INSECURE_UI_FILE_SHARING/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/PLIST_INSECURE_UI_FILE_SHARING/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.259430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.375430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_ASLR_DISABLED/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_ASLR_DISABLED/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_ASLR_DISABLED/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_ASLR_DISABLED/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.375430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_INSECURE_TAP/
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_INSECURE_TAP/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_INSECURE_TAP/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_INSECURE_TAP/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.375430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_URL_SCHEME_HIJACKING/
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_URL_SCHEME_HIJACKING/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_URL_SCHEME_HIJACKING/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_URL_SCHEME_HIJACKING/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.259430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.375430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/IPA_ANTI_DEBUG/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/IPA_ANTI_DEBUG/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/IPA_ANTI_DEBUG/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/IPA_ANTI_DEBUG/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.379431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/IPA_SECURE_PRIVACY_MANIFEST_FILE/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/IPA_SECURE_PRIVACY_MANIFEST_FILE/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/IPA_SECURE_PRIVACY_MANIFEST_FILE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/IPA_SECURE_PRIVACY_MANIFEST_FILE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.379431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/PRIVACY_NO_SENSITIVE_DATA_OUTSIDE_APP_CONTAINER/
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/PRIVACY_NO_SENSITIVE_DATA_OUTSIDE_APP_CONTAINER/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/PRIVACY_NO_SENSITIVE_DATA_OUTSIDE_APP_CONTAINER/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/PRIVACY_NO_SENSITIVE_DATA_OUTSIDE_APP_CONTAINER/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.263430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.263430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_HARDENING/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.379431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_HARDENING/PHONEGAP_WHITELIST_CONFIG/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_HARDENING/PHONEGAP_WHITELIST_CONFIG/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_HARDENING/PHONEGAP_WHITELIST_CONFIG/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_HARDENING/PHONEGAP_WHITELIST_CONFIG/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.263430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_HIGH/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.379431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_HIGH/SOURCE_MAP_CODE_LEAK/
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_HIGH/SOURCE_MAP_CODE_LEAK/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_HIGH/SOURCE_MAP_CODE_LEAK/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_HIGH/SOURCE_MAP_CODE_LEAK/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.263430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_LOW/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.379431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_LOW/PHONEGAP_DEBUG_MODE/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_LOW/PHONEGAP_DEBUG_MODE/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_LOW/PHONEGAP_DEBUG_MODE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_LOW/PHONEGAP_DEBUG_MODE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.263430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_MEDIUM/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.379431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_MEDIUM/CORDOVA_XSS/
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_MEDIUM/CORDOVA_XSS/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_MEDIUM/CORDOVA_XSS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_MEDIUM/CORDOVA_XSS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.379431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_MEDIUM/PHONEGAP_WEAK_WHITELIST_CONFIG/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_MEDIUM/PHONEGAP_WEAK_WHITELIST_CONFIG/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_MEDIUM/PHONEGAP_WEAK_WHITELIST_CONFIG/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_MEDIUM/PHONEGAP_WEAK_WHITELIST_CONFIG/recommendation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.263430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.263430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/CLOUD/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.263430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/CLOUD/_MEDIUM/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.379431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/CLOUD/_MEDIUM/AWS_S3_PUBLIC_FILELIST_ENABLED/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/CLOUD/_MEDIUM/AWS_S3_PUBLIC_FILELIST_ENABLED/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/CLOUD/_MEDIUM/AWS_S3_PUBLIC_FILELIST_ENABLED/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/CLOUD/_MEDIUM/AWS_S3_PUBLIC_FILELIST_ENABLED/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.263430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/CLOUD/_SECURE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.383431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/CLOUD/_SECURE/FIREBASE_SECURE_DATABASE_PERMISSIONS/
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/CLOUD/_SECURE/FIREBASE_SECURE_DATABASE_PERMISSIONS/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/CLOUD/_SECURE/FIREBASE_SECURE_DATABASE_PERMISSIONS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/CLOUD/_SECURE/FIREBASE_SECURE_DATABASE_PERMISSIONS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.263430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/DNS/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.263430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/DNS/_MEDIUM/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.383431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/DNS/_MEDIUM/SUBDOMAIN_TAKEOVER/
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/DNS/_MEDIUM/SUBDOMAIN_TAKEOVER/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/DNS/_MEDIUM/SUBDOMAIN_TAKEOVER/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/DNS/_MEDIUM/SUBDOMAIN_TAKEOVER/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.263430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/DNS/_POTENTIALLY/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.383431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/DNS/_POTENTIALLY/EXTERNAL_DNS_INTERACTION/
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/DNS/_POTENTIALLY/EXTERNAL_DNS_INTERACTION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/DNS/_POTENTIALLY/EXTERNAL_DNS_INTERACTION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/DNS/_POTENTIALLY/EXTERNAL_DNS_INTERACTION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.263430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/NETWORK/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.263430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/NETWORK/_INFO/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.383431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/NETWORK/_INFO/NETWORK_PORT_SCAN/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/NETWORK/_INFO/NETWORK_PORT_SCAN/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/NETWORK/_INFO/NETWORK_PORT_SCAN/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/NETWORK/_INFO/NETWORK_PORT_SCAN/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.271430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.263430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.383431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/ACCOUNT_TAKEOVER/
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/ACCOUNT_TAKEOVER/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/ACCOUNT_TAKEOVER/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/ACCOUNT_TAKEOVER/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.383431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/CODE_INJECTION/
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/CODE_INJECTION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/CODE_INJECTION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/CODE_INJECTION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.383431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/COMMAND_INJECTION/
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/COMMAND_INJECTION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/COMMAND_INJECTION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/COMMAND_INJECTION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.383431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/EXPRESSION_LANGUAGE_INJECTION/
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/EXPRESSION_LANGUAGE_INJECTION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/EXPRESSION_LANGUAGE_INJECTION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/EXPRESSION_LANGUAGE_INJECTION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.387431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/FILE_INCLUSION/
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/FILE_INCLUSION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/FILE_INCLUSION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/FILE_INCLUSION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.387431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/NOSQL_INJECTION/
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/NOSQL_INJECTION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/NOSQL_INJECTION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/NOSQL_INJECTION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.387431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SERVER_SIDE_TEMPLATE_INJECTION/
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SERVER_SIDE_TEMPLATE_INJECTION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SERVER_SIDE_TEMPLATE_INJECTION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SERVER_SIDE_TEMPLATE_INJECTION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.387431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SSI_INJECTION/
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SSI_INJECTION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SSI_INJECTION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SSI_INJECTION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.387431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_SQL_INJECTION/
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_SQL_INJECTION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_SQL_INJECTION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_SQL_INJECTION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.387431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_UNRESTRICTED_FILE_UPLOAD/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_UNRESTRICTED_FILE_UPLOAD/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_UNRESTRICTED_FILE_UPLOAD/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_UNRESTRICTED_FILE_UPLOAD/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.387431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_XPATH_INJECTION/
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_XPATH_INJECTION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_XPATH_INJECTION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_XPATH_INJECTION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.391430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/XML_EXTERNAL_ENTITY_INJECTION/
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/XML_EXTERNAL_ENTITY_INJECTION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/XML_EXTERNAL_ENTITY_INJECTION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/XML_EXTERNAL_ENTITY_INJECTION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.267430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.391430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_COOKIE_MISSING_SECURITY_FLAGS/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_COOKIE_MISSING_SECURITY_FLAGS/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_COOKIE_MISSING_SECURITY_FLAGS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_COOKIE_MISSING_SECURITY_FLAGS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.391430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_CSP/
+-rw-r--r--   0 runner    (1001) docker     (127)     4840 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_CSP/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_CSP/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_CSP/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.391430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_CT/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_CT/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_CT/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_CT/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.391430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_HSTS/
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_HSTS/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_HSTS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_HSTS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.391430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_RP/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_RP/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_RP/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_RP/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.391430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_XFO/
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_XFO/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_XFO/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_XFO/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.391430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_X_XSS/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_X_XSS/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_X_XSS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_X_XSS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.395431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_NO_STRICT_TRANSPORT_SECURITY/
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_NO_STRICT_TRANSPORT_SECURITY/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_NO_STRICT_TRANSPORT_SECURITY/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_NO_STRICT_TRANSPORT_SECURITY/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.267430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.395431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/CRLF_INJECTION/
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/CRLF_INJECTION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/CRLF_INJECTION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/CRLF_INJECTION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.395431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/EXPOSED_FIREBASE_DB/
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/EXPOSED_FIREBASE_DB/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/EXPOSED_FIREBASE_DB/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/EXPOSED_FIREBASE_DB/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.395431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/INSECURE_DIRECT_OBJECT_REFERENCE/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/INSECURE_DIRECT_OBJECT_REFERENCE/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/INSECURE_DIRECT_OBJECT_REFERENCE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/INSECURE_DIRECT_OBJECT_REFERENCE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.395431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/LDAP_INJECTION/
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/LDAP_INJECTION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/LDAP_INJECTION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4982 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/LDAP_INJECTION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.395431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/TLS_HEARTBLEED/
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/TLS_HEARTBLEED/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/TLS_HEARTBLEED/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/TLS_HEARTBLEED/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.395431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/TLS_SELFSIGNED/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/TLS_SELFSIGNED/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/TLS_SELFSIGNED/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/TLS_SELFSIGNED/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.399431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_INSECURE_OBJECT_SERIALIZATION/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_INSECURE_OBJECT_SERIALIZATION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_INSECURE_OBJECT_SERIALIZATION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_INSECURE_OBJECT_SERIALIZATION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.399431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_PATH_TRAVERSAL/
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_PATH_TRAVERSAL/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_PATH_TRAVERSAL/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_PATH_TRAVERSAL/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.399431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_XML_INJECTION/
+-rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_XML_INJECTION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_XML_INJECTION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_XML_INJECTION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.399431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_XSS/
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_XSS/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_XSS/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_XSS/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.267430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_INFO/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.399431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_INFO/TLS_SERVER_SCAN/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_INFO/TLS_SERVER_SCAN/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_INFO/TLS_SERVER_SCAN/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_INFO/TLS_SERVER_SCAN/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.399431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_INFO/WEB_GENERIC/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_INFO/WEB_GENERIC/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_INFO/WEB_GENERIC/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_INFO/WEB_GENERIC/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.399431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_INFO/WEB_INTERESTING_RESPONSE/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_INFO/WEB_INTERESTING_RESPONSE/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_INFO/WEB_INTERESTING_RESPONSE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_INFO/WEB_INTERESTING_RESPONSE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.267430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.399431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/DJANGO_DEBUG_MODE/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/DJANGO_DEBUG_MODE/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/DJANGO_DEBUG_MODE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/DJANGO_DEBUG_MODE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.403431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/USER_ENUMERATION/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/USER_ENUMERATION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/USER_ENUMERATION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/USER_ENUMERATION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.403431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/WEB_HTTP_HEADER/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/WEB_HTTP_HEADER/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/WEB_HTTP_HEADER/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/WEB_HTTP_HEADER/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.271430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.403431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/CORS_MISCONFIGURATION/
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/CORS_MISCONFIGURATION/context.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/CORS_MISCONFIGURATION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/CORS_MISCONFIGURATION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/CORS_MISCONFIGURATION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.403431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/CROSS_ORIGIN_RESOURCE_SHARING/
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/CROSS_ORIGIN_RESOURCE_SHARING/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/CROSS_ORIGIN_RESOURCE_SHARING/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/CROSS_ORIGIN_RESOURCE_SHARING/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.403431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/INSECURE_TLS_VALIDATION/
+-rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/INSECURE_TLS_VALIDATION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/INSECURE_TLS_VALIDATION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/INSECURE_TLS_VALIDATION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.403431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_ANONSERVER/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_ANONSERVER/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_ANONSERVER/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_ANONSERVER/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.403431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_DEPRECATED_PROTOCOL/
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_DEPRECATED_PROTOCOL/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_DEPRECATED_PROTOCOL/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_DEPRECATED_PROTOCOL/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.407431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_HTTP/
+-rw-r--r--   0 runner    (1001) docker     (127)     8594 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_HTTP/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_HTTP/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9366 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_HTTP/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.407431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_INSECURE_CIPHER/
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_INSECURE_CIPHER/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_INSECURE_CIPHER/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_INSECURE_CIPHER/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.407431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_INVALIDHOSTNAME/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_INVALIDHOSTNAME/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_INVALIDHOSTNAME/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_INVALIDHOSTNAME/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.407431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_HTTP_HOST_HEADER_POISONING/
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_HTTP_HOST_HEADER_POISONING/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_HTTP_HOST_HEADER_POISONING/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_HTTP_HOST_HEADER_POISONING/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.407431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_INSECURE_ACCESS_CONTROL/
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_INSECURE_ACCESS_CONTROL/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_INSECURE_ACCESS_CONTROL/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_INSECURE_ACCESS_CONTROL/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.271430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_POTENTIALLY/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.407431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_POTENTIALLY/SECRETS_NETWORK_REVIEW/
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_POTENTIALLY/SECRETS_NETWORK_REVIEW/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_POTENTIALLY/SECRETS_NETWORK_REVIEW/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_POTENTIALLY/SECRETS_NETWORK_REVIEW/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.271430 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.407431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/SECURE_AUTHENTICATION/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/SECURE_AUTHENTICATION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/SECURE_AUTHENTICATION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/SECURE_AUTHENTICATION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.407431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/TLS_INVALIDHOSTNAME_SECURE/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/TLS_INVALIDHOSTNAME_SECURE/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/TLS_INVALIDHOSTNAME_SECURE/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/TLS_INVALIDHOSTNAME_SECURE/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.411431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/UNIQUE_USER_IDENTIFICATION/
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/UNIQUE_USER_IDENTIFICATION/description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/UNIQUE_USER_IDENTIFICATION/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/UNIQUE_USER_IDENTIFICATION/recommendation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.411431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17461 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/tests/kb_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.411431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/tests/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/tests/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/tests/tools/kb_generator_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.411431 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8817 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/KB/tools/kb_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/kb/kb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.411431 ostorlab-1.0.8/src/ostorlab/agent/message/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.411431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.411431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.411431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/common/x509/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/common/x509/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/common/x509/x509_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.411431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.411431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.411431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/agent/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/agent/agent_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.415431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/domain_name/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/domain_name/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.415431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/domain_name/dns_record/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/domain_name/dns_record/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/domain_name/dns_record/dns_record_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/domain_name/domain_name_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.415431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/domain_name/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/domain_name/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/domain_name/service/service_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.415431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/domain_name/whois/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/domain_name/whois/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/domain_name/whois/whois_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.415431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/file/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.415431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/file/android/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/file/android/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.415431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/file/android/aab/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/file/android/aab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/file/android/aab/aab_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.415431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/file/android/apk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/file/android/apk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/file/android/apk/apk_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/file/file_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.415431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/file/ios/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/file/ios/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.415431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/file/ios/ipa/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/file/ios/ipa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/file/ios/ipa/ipa_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.415431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/file/sbom/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/file/sbom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/file/sbom/sbom_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.415431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/file/source/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/file/source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/file/source/source_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.415431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/ip/
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/ip/ip_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.415431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/ip/v4/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/ip/v4/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.419431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/ip/v4/geolocation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/ip/v4/geolocation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/ip/v4/geolocation/geolocation_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.419431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/port_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.419431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.419431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/service/http/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/service/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/service/http/http_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/service/service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/ip/v4/v4_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.419431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/ip/v4/whois/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/ip/v4/whois/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/ip/v4/whois/whois_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.419431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/ip/v6/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/ip/v6/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.419431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/ip/v6/geolocation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/ip/v6/geolocation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/ip/v6/geolocation/geolocation_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.419431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/port_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.419431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.419431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/service/http/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/service/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/service/http/http_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/service/service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/ip/v6/v6_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.419431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/ip/v6/whois/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/ip/v6/whois/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/ip/v6/whois/whois_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.419431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/link/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/link/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/link/link_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.423431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/store/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/store/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.423431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/store/android_store/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/store/android_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/store/android_store/android_store_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.423431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/store/android_store/developer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/store/android_store/developer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/store/android_store/developer/developer_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.423431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/store/ios_store/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/store/ios_store/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.423431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/store/ios_store/developer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/store/ios_store/developer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/store/ios_store/developer/developer_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/store/ios_store/ios_store_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.423431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/capture/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/capture/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.423431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/capture/artifact/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/capture/artifact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/capture/artifact/artifact_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.423431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/capture/filesystem/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/capture/filesystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/capture/filesystem/filesystem_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.423431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/capture/http/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/capture/http/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.423431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/capture/http/request/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/capture/http/request/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/capture/http/request/request_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.423431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/capture/http/response/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/capture/http/response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/capture/http/response/response_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.423431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/capture/logs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/capture/logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/capture/logs/logs_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.423431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/capture/request_response/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/capture/request_response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/capture/request_response/request_response_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.427431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/capture/ui_call/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/capture/ui_call/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/capture/ui_call/ui_call_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.427431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/control/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/control/control_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.427431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.427431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.427431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.427431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/library/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/library/library_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.427431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/x509/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/x509/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/x509/x509_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.427431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.427431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.427431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/backend/backend_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.427431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/feature/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/feature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4525 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/feature/feature_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.427431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/library/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5089 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/library/library_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.427431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/metadata/metadata_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.427431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/feature/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/feature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/feature/feature_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/file_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.427431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.431431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/backend/backend_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.431431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/feature/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/feature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/feature/feature_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.431431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/library/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/library/library_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.431431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/metadata/metadata_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.431431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/library/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4454 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/library/library_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.431431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/ip/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/ip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.431431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.431431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.431431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/library/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/library/library_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.431431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/x509/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/x509/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/x509/x509_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.431431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.431431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.431431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/library/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/library/library_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.431431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/x509/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/x509/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/x509/x509_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.431431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/healthcheck/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/healthcheck/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.435431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/healthcheck/ping/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/healthcheck/ping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/healthcheck/ping/ping_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.435431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/report/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/report/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.435431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/report/cve/
+-rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/report/cve/cve_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.435431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/report/event/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/report/event/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.435431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/report/event/post_scan/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/report/event/post_scan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.435431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/report/event/post_scan/done/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/report/event/post_scan/done/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/report/event/post_scan/done/done_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.435431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/report/event/post_scan/start/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/report/event/post_scan/start/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/report/event/post_scan/start/start_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.435431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/report/event/post_scan/timeout/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/report/event/post_scan/timeout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/report/event/post_scan/timeout/timeout_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.435431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/report/event/scan/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/report/event/scan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.435431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/report/event/scan/done/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/report/event/scan/done/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/report/event/scan/done/done_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.435431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/report/event/scan/start/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/report/event/scan/start/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/report/event/scan/start/start_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.435431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/report/event/scan/timeout/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/report/event/scan/timeout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/report/event/scan/timeout/timeout_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.435431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/report/status/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/report/status/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/report/status/status_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.435431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/report/vulnerability/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/report/vulnerability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7099 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/report/vulnerability/vulnerability_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.435431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/use/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/use/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.439431 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/use/device/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/use/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/use/device/device_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/proto_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/message/serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.439431 ostorlab-1.0.8/src/ostorlab/agent/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/mixins/agent_healthcheck_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7801 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/mixins/agent_mq_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11005 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/mixins/agent_open_telemetry_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9167 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/mixins/agent_persist_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/mixins/agent_report_vulnerability_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.439431 ostorlab-1.0.8/src/ostorlab/agent/mixins/protocols/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/mixins/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/mixins/protocols/emit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.439431 ostorlab-1.0.8/src/ostorlab/agent/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/schema/agent_group_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6114 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/schema/agent_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/schema/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/schema/target_group_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/agent/schema/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.443431 ostorlab-1.0.8/src/ostorlab/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/apis/add_scanner_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/apis/agent_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/apis/agent_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/apis/agent_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6162 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/apis/assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/apis/create_agent_scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/apis/create_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/apis/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/apis/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/apis/revoke_api_key.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.443431 ostorlab-1.0.8/src/ostorlab/apis/runners/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/apis/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8327 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/apis/runners/authenticated_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/apis/runners/login_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/apis/runners/public_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/apis/runners/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/apis/scan_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/apis/scan_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/apis/scan_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/apis/scan_stop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/apis/scanner_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/apis/test_credentials_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/apis/vulnz_describe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/apis/vulnz_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.447431 ostorlab-1.0.8/src/ostorlab/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/assets/TODO.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/assets/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/assets/android_aab.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/assets/android_apk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/assets/android_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/assets/asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/assets/domain_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/assets/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/assets/ios_ipa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/assets/ios_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/assets/ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/assets/ipv4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/assets/ipv6.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/assets/link.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.447431 ostorlab-1.0.8/src/ostorlab/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.447431 ostorlab-1.0.8/src/ostorlab/cli/agent/
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/agent/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.447431 ostorlab-1.0.8/src/ostorlab/cli/agent/build/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/agent/build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5003 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/agent/build/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/agent/build/build_progress.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.447431 ostorlab-1.0.8/src/ostorlab/cli/agent/delete/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/agent/delete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/agent/delete/delete.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.451431 ostorlab-1.0.8/src/ostorlab/cli/agent/healthcheck/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/agent/healthcheck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/agent/healthcheck/healthcheck.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.451431 ostorlab-1.0.8/src/ostorlab/cli/agent/install/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/agent/install/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/agent/install/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/agent/install/install_progress.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.451431 ostorlab-1.0.8/src/ostorlab/cli/agent/list/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/agent/list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/agent/list/list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.451431 ostorlab-1.0.8/src/ostorlab/cli/agent/search/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/agent/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/agent/search/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/agent_fetcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.451431 ostorlab-1.0.8/src/ostorlab/cli/agentgroup/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/agentgroup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/agentgroup/agentgroup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.451431 ostorlab-1.0.8/src/ostorlab/cli/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/auth/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.451431 ostorlab-1.0.8/src/ostorlab/cli/auth/login/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/auth/login/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/auth/login/login.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.451431 ostorlab-1.0.8/src/ostorlab/cli/auth/revoke/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/auth/revoke/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/auth/revoke/revoke.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.451431 ostorlab-1.0.8/src/ostorlab/cli/ci_scan/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/ci_scan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/ci_scan/ci_scan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.451431 ostorlab-1.0.8/src/ostorlab/cli/ci_scan/run/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/ci_scan/run/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.455431 ostorlab-1.0.8/src/ostorlab/cli/ci_scan/run/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/ci_scan/run/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/ci_scan/run/assets/android_aab.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/ci_scan/run/assets/android_apk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/ci_scan/run/assets/ios_ipa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5041 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/ci_scan/run/assets/mobile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.455431 ostorlab-1.0.8/src/ostorlab/cli/ci_scan/run/ci_logger/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/ci_scan/run/ci_logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/ci_scan/run/ci_logger/circleci_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/ci_scan/run/ci_logger/console_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/ci_scan/run/ci_logger/github_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/ci_scan/run/ci_logger/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8729 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/ci_scan/run/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/docker_requirements_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/dumpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/input_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/install_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/rootcli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.455431 ostorlab-1.0.8/src/ostorlab/cli/scan/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/scan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.455431 ostorlab-1.0.8/src/ostorlab/cli/scan/list/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/scan/list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/scan/list/list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.455431 ostorlab-1.0.8/src/ostorlab/cli/scan/run/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/scan/run/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.459431 ostorlab-1.0.8/src/ostorlab/cli/scan/run/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/scan/run/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/scan/run/assets/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/scan/run/assets/android_aab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/scan/run/assets/android_apk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/scan/run/assets/android_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/scan/run/assets/domain_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/scan/run/assets/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/scan/run/assets/ios_ipa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/scan/run/assets/ios_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/scan/run/assets/ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/scan/run/assets/link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8702 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/scan/run/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/scan/scan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.459431 ostorlab-1.0.8/src/ostorlab/cli/scan/stop/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/scan/stop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/scan/stop/stop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.459431 ostorlab-1.0.8/src/ostorlab/cli/scanner/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/scanner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/scanner/scanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.459431 ostorlab-1.0.8/src/ostorlab/cli/vulnz/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/vulnz/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.459431 ostorlab-1.0.8/src/ostorlab/cli/vulnz/describe/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/vulnz/describe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/vulnz/describe/describe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.459431 ostorlab-1.0.8/src/ostorlab/cli/vulnz/dump/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/vulnz/dump/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/vulnz/dump/dump.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.459431 ostorlab-1.0.8/src/ostorlab/cli/vulnz/list/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/vulnz/list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/vulnz/list/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/cli/vulnz/vulnz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/configuration_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.459431 ostorlab-1.0.8/src/ostorlab/runtimes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/runtimes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.459431 ostorlab-1.0.8/src/ostorlab/runtimes/cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/runtimes/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25003 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/runtimes/cloud/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14599 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/runtimes/definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.459431 ostorlab-1.0.8/src/ostorlab/runtimes/lite_local/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/runtimes/lite_local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15307 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/runtimes/lite_local/agent_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14379 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/runtimes/lite_local/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.463431 ostorlab-1.0.8/src/ostorlab/runtimes/local/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/runtimes/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14839 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/runtimes/local/agent_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/runtimes/local/log_streamer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.463431 ostorlab-1.0.8/src/ostorlab/runtimes/local/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/runtimes/local/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.463431 ostorlab-1.0.8/src/ostorlab/runtimes/local/models/alembic/
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/runtimes/local/models/alembic/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/runtimes/local/models/alembic/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.463431 ostorlab-1.0.8/src/ostorlab/runtimes/local/models/alembic/versions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/runtimes/local/models/alembic/versions/35cd577ef0e5_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/runtimes/local/models/alembic/versions/746c5eb3d181_add_vulnerability_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/runtimes/local/models/alembic/versions/7d12204c3f27_add_references_field_to_vulnerability.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/runtimes/local/models/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    11189 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/runtimes/local/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30185 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/runtimes/local/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.463431 ostorlab-1.0.8/src/ostorlab/runtimes/local/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/runtimes/local/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.463431 ostorlab-1.0.8/src/ostorlab/runtimes/local/services/configurations/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/runtimes/local/services/configurations/mq_advanced_conf.config
+-rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/runtimes/local/services/jaeger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6784 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/runtimes/local/services/mq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/runtimes/local/services/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.463431 ostorlab-1.0.8/src/ostorlab/runtimes/proto/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/runtimes/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/runtimes/proto/agent_instance_settings_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/runtimes/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/runtimes/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.463431 ostorlab-1.0.8/src/ostorlab/scanner/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/scanner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6786 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/scanner/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7475 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/scanner/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.463431 ostorlab-1.0.8/src/ostorlab/scanner/proto/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/scanner/proto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.467431 ostorlab-1.0.8/src/ostorlab/scanner/proto/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/scanner/proto/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/scanner/proto/assets/aab_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/scanner/proto/assets/agent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/scanner/proto/assets/android_store_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/scanner/proto/assets/apk_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/scanner/proto/assets/domain_name_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/scanner/proto/assets/file_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/scanner/proto/assets/ios_store_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/scanner/proto/assets/ip_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/scanner/proto/assets/ipa_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/scanner/proto/assets/link_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/scanner/proto/assets/network_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/scanner/proto/assets/source_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/scanner/proto/assets/v4_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/scanner/proto/assets/v6_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.467431 ostorlab-1.0.8/src/ostorlab/scanner/proto/scan/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/scanner/proto/scan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.467431 ostorlab-1.0.8/src/ostorlab/scanner/proto/scan/_location/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/scanner/proto/scan/_location/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/scanner/proto/scan/_location/startAgentScan_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/scanner/scan_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/scanner/scanner_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.467431 ostorlab-1.0.8/src/ostorlab/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7703 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/testing/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.471431 ostorlab-1.0.8/src/ostorlab/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/utils/defintions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/utils/dictionary_minifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/utils/ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/utils/risk_rating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/utils/scanner_state_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/utils/strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/utils/styles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/utils/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/utils/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-04-30 12:07:57.000000 ostorlab-1.0.8/src/ostorlab/utils/volumes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:08:02.471431 ostorlab-1.0.8/src/ostorlab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8965 2024-04-30 12:08:02.000000 ostorlab-1.0.8/src/ostorlab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    78965 2024-04-30 12:08:02.000000 ostorlab-1.0.8/src/ostorlab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 12:08:02.000000 ostorlab-1.0.8/src/ostorlab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-30 12:08:02.000000 ostorlab-1.0.8/src/ostorlab.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 12:08:01.000000 ostorlab-1.0.8/src/ostorlab.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-30 12:08:02.000000 ostorlab-1.0.8/src/ostorlab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 12:08:02.000000 ostorlab-1.0.8/src/ostorlab.egg-info/top_level.txt
```

### Comparing `ostorlab-1.0.7/LICENSE` & `ostorlab-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/setup.cfg` & `ostorlab-1.0.8/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 author = Ostorlab
 author_email = oxo@ostorlab.dev
 license = Apache-2.0
 license_files = LICENSE
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Ostorlab/ostorlab
-version = 1.0.7
+version = 1.0.8
 project_urls = 
 	Documentation = https://oxo.ostorlab.co/
 	Source = https://github.com/Ostorlab/oxo
 	Changelog = https://github.com/Ostorlab/oxo/releases
 	Tracker = https://github.com/Ostorlab/oxo/issues
 	Twitter = https://twitter.com/OstorlabSec
 platforms = any
```

### Comparing `ostorlab-1.0.7/setup.py` & `ostorlab-1.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/__init__.py` & `ostorlab-1.0.8/src/ostorlab/__init__.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/agent.py` & `ostorlab-1.0.8/src/ostorlab/agent/agent.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/definitions.py` & `ostorlab-1.0.8/src/ostorlab/agent/definitions.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_DEBUG/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_DEBUG/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_DEBUG/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_DEBUG/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_ELF_NOTPROTECTED/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_ELF_NOTPROTECTED/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_ELF_NOTPROTECTED/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_ELF_NOTPROTECTED/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_INSECURE_NETWORK_SECURITY_CONFIG/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_INSECURE_NETWORK_SECURITY_CONFIG_SECURE/description.md`

 * *Files 7% similar despite different names*

```diff
@@ -12,28 +12,31 @@
 	        <trust-anchors>
 	            <certificates src="@raw/debug_cas"/>
 	        </trust-anchors>
 	    </debug-overrides>
 	</network-security-config>
 	```
 
+
+
 * Declarative opt-out for cleartext traffic
 
 === "XML"
 	```xml
 	<?xml version="1.0" encoding="utf-8"?>
 	<network-security-config>
 	    <domain-config cleartextTrafficPermitted="false">
 	        <domain includeSubdomains="true">secure.example.com</domain>
 	    </domain-config>
 	</network-security-config>
 	```
 
 
-* Declarative setting of certificate pinning keys
+
+* Declartive setting of certificate pinning keys
 
 === "XML"
 	```xml
 	<?xml version="1.0" encoding="utf-8"?>
 	<network-security-config>
 	    <domain-config>
 	        <domain includeSubdomains="true">example.com</domain>
@@ -41,7 +44,8 @@
 	            <pin digest="SHA-256">7HIpactkIAq2Y49orFOOQKurWxmmSFZhBCoQYcRhJ3Y=</pin>
 	            <!-- backup pin -->
 	            <pin digest="SHA-256">fwza0LRMXouZHRC8Ei+4PyuldPDcf3UKgO/04cDM1oE=</pin>
 	        </pin-set>
 	    </domain-config>
 	</network-security-config>
 	```
+
```

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_INSECURE_NETWORK_SECURITY_CONFIG/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_INSECURE_NETWORK_SECURITY_CONFIG/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_NOT_OBFUSCATED/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_NOT_OBFUSCATED/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_NOT_OBFUSCATED/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_NOT_OBFUSCATED/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_NOT_OBFUSCATED/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HARDENING/APK_NOT_OBFUSCATED/recommendation.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-Design the application to add the following protections and slow reverse engineering of the application:
+Below are steps you can consider to make your application less prone to reverse engineering :
 
-* Obfuscate Java source code with tools like Proguard.
+#### Obfuscate Java source code with Proguard.
+
+To add Proguard to you application, add the following to the `build.gradle` file:
 
 === "Gradle"
 	```gradle
     buildTypes {
             release {
                 minifyEnabled true
                 proguardFiles getDefaultProguardFile('proguard-android.txt'), 'proguard-rules.pro'
@@ -13,15 +15,63 @@
     ```
 
 
 
 This tells Gradle to use ProGuard for code obfuscation in the release build. You can then create a "proguard-rules.pro"
 file in the app's "app" directory to configure the obfuscation rules.
 
-* Obfuscate Java source code with tools like Dexguard.
+Example `proguard-rules.pro`:
+
+```
+# Keep the names of classes in this package
+-keep class com.example.myapplication.** { *; }
+
+# Keep all public and protected methods in these classes
+-keepclassmembers class com.example.myapplication.** {
+    public protected *;
+}
+
+# Keep all native method names
+-keepclassmembers class * {
+    native <methods>;
+}
+
+# Keep all fields with the specified name
+-keepclassmembers class * {
+    private int myField;
+}
+
+# Keep all classes that implement Parcelable
+-keep class * implements android.os.Parcelable {
+  public static final android.os.Parcelable$Creator *;
+}
+
+# Keep all Enum classes
+-keepclassmembers enum * {
+    public static **[] values();
+    public static ** valueOf(java.lang.String);
+}
+
+# Keep all annotations
+-keepattributes *Annotation*
+
+# Preserve all entry points (like main methods)
+-keep public class * {
+    public static void main(java.lang.String[]);
+}
+
+# Keep all Serializable classes
+-keep class * implements java.io.Serializable {
+    *;
+}
+```
+
+#### Obfuscate Java source code with Dexguard.
+
+To enable Dexguard in your application, you can add the following to the `build.gradle` file:
 
 === "Gradle"
 	```gradle
     buildTypes {
             release {
                 minifyEnabled true
                 useProguard false
@@ -38,14 +88,18 @@
 
 By default, when you enable code obfuscation using DexGuard, it will use its own obfuscation rules in addition to any rules specified in the ProGuard configuration file. However, you can disable the use of ProGuard's rules by setting the `useProguard` option to false.
 
 * Verification application signing certificate during runtime by checking `context.getPackageManager().signature`
 * Check application installer to ensure it matches the Android Market by calling `context.getPackageManager().getInstallerPackageName`
 * Check running environment at runtime
 
+#### Check if the app is running on an emulator
+
+You can add the following check to your application to detect if it's running on an emulator.
+
 === "Java"
 	```java
     private static String getSystemProperty(String name) throws Exception {
         Class systemPropertyClazz = Class.forName("android.os.SystemProperties");
         return (String) systemPropertyClazz.getMethod("get", new Class[] { String.class }).invoke(systemPropertyClazz, new Object[] { name });
     }
     
@@ -64,13 +118,15 @@
 
         return false;
     }
 	```
 
 
 
-* Check debug flag at runtime
+#### Check debug flag at runtime
+
+Similarly, you can check if the application is in debug mode during runtime
 
 === "Java"
 	```java
 	    context.getApplicationInfo().applicationInfo.flags & ApplicationInfo.FLAG_DEBUGGABLE;
 	```
```

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_FILE_PROVIDER_PERMISSIVE_EXTERNAL_PATH/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_FILE_PROVIDER_PERMISSIVE_EXTERNAL_PATH/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_FILE_PROVIDER_PERMISSIVE_EXTERNAL_PATH/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_FILE_PROVIDER_PERMISSIVE_EXTERNAL_PATH/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_FILE_PROVIDER_PERMISSIVE_EXTERNAL_PATH/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_FILE_PROVIDER_PERMISSIVE_EXTERNAL_PATH/recommendation.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 An insecure file path provider is a vulnerability in Android apps where a file path is exposed to other apps or users, which could potentially compromise sensitive data or allow unauthorized access to system resources. 
 
-By making your app more secure, you help preserve user trust and device integrity, so to protect your app from this vulnerability, here are some recommendations:
+To safeguard your Android app against vulnerabilities stemming from insecure file path providers, consider these recommendations:
 
-* Be cautious about what files you share and only share files that are necessary and appropriate.
-* Don't share sensitive files or files that contain sensitive information.
-* When using external-path, avoid using permissive settings like '.' as the path.
+* Avoid permissive settings like '.' in external-path declarations.
 * Avoid using `root-path`.
-* Don't assign the root path '/.' to the path attribute in any type of path.
-* Use the <grant-uri-permission> tag to control access to shared files.
+* Avoid assigning `/` as the root path
+* Use the `<grant-uri-permission>` tag to control access to shared files.
 * Prefer using `external-files-path` path type.
-* Use specific folders for path attributes, check the following example:
+* Use specific folders for path attributes:
 
 
+For instance, here is an example file provider with `external-files-path` tag and specific `Download/` path attribute.
+
 === "XML"
 	```xml
 	<?xml version="1.0" encoding="utf-8"?>
 	<paths>
-	    <external-path
+	    <external-files-path
 	        name="downloads"
 	        path="Download/" />
 	</paths>
 	```
```

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_INSECURE_EXEC_CMD/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_INSECURE_EXEC_CMD/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_INSECURE_EXEC_CMD/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_INSECURE_EXEC_CMD/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_NOTIFICATION_SPOOFING/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_NOTIFICATION_SPOOFING/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_WIFI_API_PII/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_WIFI_API_PII/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_WIFI_API_PII/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/APK_WIFI_API_PII/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/INSECURE_PACKAGE_CONTEXT/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/INSECURE_PACKAGE_CONTEXT/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/INSECURE_PACKAGE_CONTEXT/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/INSECURE_PACKAGE_CONTEXT/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/INSECURE_PACKAGE_CONTEXT/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_HIGH/INSECURE_PACKAGE_CONTEXT/recommendation.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 To mitigate the vulnerability associated with insecure package context creation using createPackageContext with CONTEXT_INCLUDE_CODE and CONTEXT_IGNORE_SECURITY flags, developers should: 
 
-1- Avoid using createPackageContext by baking any necessary components into the app itself rather than using separate apk files.
+1- Avoid using `createPackageContext` by baking any necessary components into the app itself rather than using separate apk files.
 
-2- if using createPackageContext is necessary, avoid using the flags `CONTEXT_INCLUDE_CODE` and `CONTEXT_IGNORE_SECURITY`, instead use `CONTEXT_RESTRICTED` which may disable specific features but makes the application more robust against third party application attacks.
+2- if using `createPackageContext` is necessary, avoid using the flags `CONTEXT_INCLUDE_CODE` and `CONTEXT_IGNORE_SECURITY`, instead use `CONTEXT_RESTRICTED` which may disable specific features but makes the application more robust against third party application attacks.
 
 3- When checking if the package is in the list of installed packages, avoid loose comparisons like `startsWith` or `endsWith`, instead try matching the package name exactly
 
 === "Java"
 	```java
 	import android.content.Context;
 	import android.content.pm.PackageInfo;
```

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_IMPORTANT/APK_EXPORTED/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_IMPORTANT/APK_EXPORTED/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_IMPORTANT/APK_SCREENSHOT_DISABLED/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_IMPORTANT/APK_SCREENSHOT_DISABLED/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_IMPORTANT/APK_SCREENSHOT_DISABLED/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_IMPORTANT/APK_SCREENSHOT_DISABLED/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_ATTACK_SURFACE/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_ATTACK_SURFACE/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_CONST_STRINGS/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_CONST_STRINGS/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_COMMAND_EXEC/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_COMMAND_EXEC/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_CRYPTO/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_CRYPTO/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_IPC/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_IPC/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_LOGGING/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_LOGGING/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SQLITE/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_SQLITE/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_WEBVIEW/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_DYNAMIC_WEBVIEW/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_FILEOBSERVER_IMPL/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_FILEOBSERVER_IMPL/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_FILE_LIST/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_FILE_LIST/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_MANIFEST/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/APK_MANIFEST/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/BROADCAST_RECEIVER_DYNAMIC_REGISTRATION/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/BROADCAST_RECEIVER_DYNAMIC_REGISTRATION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_ANDROIDSECURITY/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_ANDROIDSECURITY/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_CRYPTO/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_CRYPTO/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_EXTERNAL_STORAGE/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_EXTERNAL_STORAGE/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_EXTERNAL_STORAGE/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_STORAGE/description.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,109 +1,145 @@
-We can distinguish four types of files based on the access permission and storage location:
+Insecure storage vulnerability in mobile applications refers to a security flaw where sensitive data, such as user credentials, personal information, or other confidential data, is stored on the device in world readable locations. This can leave the data vulnerable to unauthorized access by other applications on the device or by a malicious actor with physical access to the device.
 
-* Private files:
-    * A very safe way to use files
-    * Must be created in the application's directory
-    * Can store sensitive information and must use encryption when storing PII
-    * Can be used for files that can be read/written only in the same application
-    * The access privilege must be set to private mode in order to restrict access from other applications
-    * Content Provider, Service or other inter-application linkage system are recommended to exchange information between applications
-
-    === "Java"
-        ```java
-        public void onCreateFileClick(View view) {
-            FileOutputStream fos = null;
-            try {
-                fos = openFileOutput(FILE_NAME, MODE_PRIVATE);
-
-                fos.write(new String("Not sensitive information (File Activity)").getBytes());
-            } catch (FileNotFoundException e) {
-                mFileView.setText(R.string.file_view);
-            } catch (IOException e) {
-                android.util.Log.e("PrivateFileActivity","failed to read file");
-            } finally {
-                if (fos != null) {
-                    try {
-                        fos.close();
-                    } catch (IOException e) {
-                        android.util.Log.e("PrivateFileActivity","failed to close file");
-                    }
-                }
-            }
-            finish();
-        }        
-        ```
-
-
-* Public Read Only files:
-    * Used to disclose content to unspecified number of applications
-    * The access privilege must be set to read only
-    * Must not contain sensitive information
-    * Using the `MODE_WORLD_READABLE` variable to create a public file is deprecated in API Level 17 and later versions, and will trigger a security exception in API Level 24 and later versions
-    * File-sharing methods using Content Provider are preferable
-
-    === "Java"
-        ```java
-        public void onCreateFileClick(View view) {
-            FileOutputStream fos = null;
-            try {
-                fos = openFileOutput(FILE_NAME, MODE_WORLD_READABLE);
-
-                fos.write(new String("Not sensitive information (Public File Activity)").getBytes());
-
-            } catch (FileNotFoundException e) {
-                mFileView.setText(R.string.file_view);
-            } catch (IOException e) {
-                android.util.Log.e("PublicFileActivity","failed to read file");
-            } finally {
-                if (fos != null) {
-                    try {
-                        fos.close();
-                    } catch (IOException e) {
-                        android.util.Log.e("PublicFileActivity","failed to close file");
-                    }
-                }
-            }
-            finish();
-        }
-        ```
-
-
-
-* Public Read/Write files:
-    * Used to permit Read/Write access to unspecified number of applications
-    * Confidentiality and Integrity can’t be guaranteed
-    * This type of file is not practical and should be avoided
-
-
-* External memory (Read Write Public) files:
-    * It's supposed to be used when storing huge files, or when there is a need to bring out data to outside (e.g. backup, ...)
-    * In addition to having the equal characteristics of "Read Write Public file" to unspecified large number of applications, it has also the same characteristics of "Read Write Public file" to applications which declare `android.permission.WRITE.EXTERNAL.STORAGE` permission
-    * In applications that output backup, some contrivances to minimize risks in terms of application spec or designing like displaying a caution “Copy Backup files to the safety location like PC etc., a.s.a.p.”, are necessary
-    * Using external memory devices should be avoided, unless necessary, and encryption must be used
-    * When reading in files in external memory device, validate the input data read from external memory device
-    * Applications should be designed supposing that files in external memory device can be deleted
-
-    === "Java"
-        ```java
-        public void onCreateFileClick(View view) {
-            FileOutputStream fos = null;
-            try {
-                File file = new File(getExternalFilesDir(TARGET_TYPE), FILE_NAME);
-                fos = new FileOutputStream(file, false);
-                fos.write(new String("Non-Sensitive Information(ExternalFileActivity)").getBytes());
-            } catch (FileNotFoundException e) {
-                mFileView.setText(R.string.file_view);
-            } catch (IOException e) {
-                android.util.Log.e("ExternalFileActivity","failed to read file");
-            } finally {
-                if (fos != null) {
-                    try {
-                        fos.close();
-                    } catch (IOException e) {
-                        android.util.Log.e("ExternalFileActivity","failed to close file");
-                    }
-                }
-            }
-            finish();
-        }
-        ```
+Insecure storage does not only occur when the application writes to world-readable locations but also when the application loads data such as configuration files from world-writable locations where a malicious actor can alter the configuration files and consequently tamper with the functionality of the application. 
+
+
+
+=== "Kotlin"
+  ```kotlin
+  import android.os.Bundle
+  import android.os.Environment
+  import android.widget.Button
+  import android.widget.Toast
+  import androidx.appcompat.app.AppCompatActivity
+  import java.io.File
+  import java.io.FileOutputStream
+  import java.io.IOException
+  import java.io.OutputStreamWriter
+  
+  class MainActivity : AppCompatActivity() {
+  
+      override fun onCreate(savedInstanceState: Bundle?) {
+          super.onCreate(savedInstanceState)
+          setContentView(R.layout.activity_main)
+  
+          val loginButton: Button = findViewById(R.id.login_button)
+          loginButton.setOnClickListener {
+              // Dummy authentication process
+              val token = authenticate("username", "password") // authentication logic
+  
+              // Store token in public storage
+              storeTokenInPublicStorage(token)
+          }
+      }
+  
+      private fun storeTokenInPublicStorage(token: String) {
+          val filePath = "/sdcard/insecure_app/jwt_config.txt"
+          val file = File(filePath)
+          try {
+              val outputStreamWriter = OutputStreamWriter(FileOutputStream(file))
+              outputStreamWriter.write(token)
+              outputStreamWriter.close()
+          } catch (e: IOException) {
+              e.printStackTrace()
+          }
+      }
+  }
+  ```
+
+
+=== "Swift"
+  ```swift
+  import UIKit
+  
+  class ViewController: UIViewController {
+  
+      override func viewDidLoad() {
+          super.viewDidLoad()
+          // Do any additional setup after loading the view.
+          
+          let loginButton = UIButton(type: .system)
+          loginButton.setTitle("Login", for: .normal)
+          loginButton.addTarget(self, action: #selector(loginButtonTapped), for: .touchUpInside)
+          view.addSubview(loginButton)
+          loginButton.translatesAutoresizingMaskIntoConstraints = false
+          loginButton.centerXAnchor.constraint(equalTo: view.centerXAnchor).isActive = true
+          loginButton.centerYAnchor.constraint(equalTo: view.centerYAnchor).isActive = true
+      }
+  
+      @objc func loginButtonTapped() {
+          // Dummy authentication process
+          let token = authenticate(username: "username", password: "password")
+  
+          // Store token in public storage
+          storeTokenInPublicStorage(token: token)
+      }
+      
+      
+      private func storeTokenInPublicStorage(token: String) {
+          let filePath = "/var/mobile/Media/insecure_app/jwt_config.txt"
+          let fileURL = URL(fileURLWithPath: filePath)
+          
+          do {
+              try token.write(to: fileURL, atomically: true, encoding: .utf8)
+              print("Token stored successfully.")
+          } catch {
+              print("Failed to write token: \(error)")
+          }
+      }
+  }
+  ```
+
+
+=== "Flutter"
+  ```dart
+  import 'dart:io';
+  import 'package:flutter/material.dart';
+  
+  void main() {
+    runApp(MyApp());
+  }
+  
+  class MyApp extends StatelessWidget {
+    @override
+    Widget build(BuildContext context) {
+      return MaterialApp(
+        home: MyHomePage(),
+      );
+    }
+  }
+  
+  class MyHomePage extends StatelessWidget {
+    @override
+    Widget build(BuildContext context) {
+      return Scaffold(
+        appBar: AppBar(
+          title: Text('Flutter Insecure Storage'),
+        ),
+        body: Center(
+          child: ElevatedButton(
+            onPressed: () {
+              // Dummy authentication process
+              String token = authenticate("username", "password");
+  
+              // Store token in public storage
+              storeTokenInPublicStorage(token);
+            },
+            child: Text('Login'),
+          ),
+        ),
+      );
+    }
+  
+    void storeTokenInPublicStorage(String token) {
+      final directory = Directory('/sdcard/insecure_app/');
+      directory.createSync(recursive: true);
+      final file = File('${directory.path}/jwt_config.txt');
+      try {
+        file.writeAsStringSync(token);
+        print('Token stored successfully.');
+      } catch (e) {
+        print('Failed to write token: $e');
+      }
+    }
+  }
+  ```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_IPC/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_IPC/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_LOG/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_LOG/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_RANDOM/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_RANDOM/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_SQL/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_SQL/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_WEBVIEW/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_WEBVIEW/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_XML/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_XML/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_ZIP/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_INFO/DANGEROUS_API_ZIP/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_DEBUG_SYMBOL_PRESENT/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_DEBUG_SYMBOL_PRESENT/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_FACEBOOK_REACT_DEV_SETTINGS_ENABLED/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_FACEBOOK_REACT_DEV_SETTINGS_ENABLED/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_HAS_FRAGILE_USER_DATA_NOT_SET/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_HAS_FRAGILE_USER_DATA_NOT_SET/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_HAS_FRAGILE_USER_DATA_NOT_SET/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_HAS_FRAGILE_USER_DATA_NOT_SET/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_LIST_NOT_USED_PERMISSIONS/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_LIST_NOT_USED_PERMISSIONS/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_REQUEST_LEGACY_EXTERNAL_STORAGE/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_REQUEST_LEGACY_EXTERNAL_STORAGE/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_TASK_HIJACKING/context.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_TASK_HIJACKING/context.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_TASK_HIJACKING/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_TASK_HIJACKING/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_TASK_HIJACKING/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_TASK_HIJACKING/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_TASK_HIJACKING/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_TASK_HIJACKING/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_USES_CLEAR_TEXT_TRAFFIC/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/APK_USES_CLEAR_TEXT_TRAFFIC/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/DEPRECATED_TARGET_API_VERSION/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/DEPRECATED_TARGET_API_VERSION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/INTENT_SPOOFING/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/INTENT_SPOOFING/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/INTENT_SPOOFING/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/INTENT_SPOOFING/recommendation.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-To limit one's exposure to this type of attack, developers should avoid exporting components unless the component is
-specifically designed to handle requests from untrusted applications. Developers should be aware that declaring an
-intent filter will automatically export the component, exposing it to public access. Critical, state-changing actions
-should not be placed in exported components. If a single component handles both inter- and intra-application
-requests, the developer should consider dividing that component into separate components.
+To limit one's exposure to this type of attack, consider the following recommendations: 
 
-If a component must be exported (e.g., to receive system broadcasts), then the component should dynamically check the
-caller's identity prior to performing any operations. Requiring Signature or SignatureOrSystem permissions is an
-effective way of limiting a component's exposure to a set of trusted applications. Finally, the return values of
-exported components can also leak private data, so developers should check the caller's identity prior to returning
-sensitive values.
+- Avoid exporting components unless the component is specifically designed to handle requests from untrusted applications. 
+- Be aware that declaring an intent filter will automatically export the component, exposing it to public access.
+- Avoid placing critical, state-changing actions in exported components. 
+- If a single component handles both inter-application and intra-application requests, the developer should consider dividing that component into separate components.
+- If a component must be exported (e.g., to receive system broadcasts), then the component should dynamically check the caller's identity prior to performing any operations. 
+- Require Signature or SignatureOrSystem permissions to limit component's exposure to a set of trusted applications. 
+- Check the caller's identity prior to returning return values of exported components as they can leak private data.
```

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/PRIVACY_KEYBOARD_CACHE/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_LOW/PRIVACY_KEYBOARD_CACHE/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_CERTIFICAT_OUTDATED/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_CERTIFICAT_OUTDATED/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_FACEBOOK_DEBUG_ENABLED/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_FACEBOOK_DEBUG_ENABLED/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_INSECURE_PATH_CLASS_LOADER/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_INSECURE_PATH_CLASS_LOADER/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_INSECURE_PATH_CLASS_LOADER/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_INSECURE_PATH_CLASS_LOADER/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_UNDECLARED_PERMISSIONS/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_UNDECLARED_PERMISSIONS/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_UNDECLARED_PERMISSIONS/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_UNDECLARED_PERMISSIONS/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_UNDECLARED_PERMISSIONS/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/APK_UNDECLARED_PERMISSIONS/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/DANGEROUS_API_SETJAVASCRIPTINTERFACE/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/DANGEROUS_API_SETJAVASCRIPTINTERFACE/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/DANGEROUS_API_SETJAVASCRIPTINTERFACE/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/DANGEROUS_API_SETJAVASCRIPTINTERFACE/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/DANGEROUS_API_WEBVIEW_REMOTE_DEBUGGING_ENABLED/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/DANGEROUS_API_WEBVIEW_REMOTE_DEBUGGING_ENABLED/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/DANGEROUS_API_WEBVIEW_REMOTE_DEBUGGING_ENABLED/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/DANGEROUS_API_WEBVIEW_REMOTE_DEBUGGING_ENABLED/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/IMPLICIT_PENDINGINTENT/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/IMPLICIT_PENDINGINTENT/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/IMPLICIT_PENDINGINTENT/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/IMPLICIT_PENDINGINTENT/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/IMPLICIT_PENDINGINTENT/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/IMPLICIT_PENDINGINTENT/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_API_BLUETOOTH/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_API_BLUETOOTH/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_CLASS_LOADING/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_CLASS_LOADING/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_PERMISSION_SHARED_PREFERENCES/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_PERMISSION_SHARED_PREFERENCES/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_REGISTER_RECEIVER_FLAG/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_REGISTER_RECEIVER_FLAG/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_REGISTER_RECEIVER_FLAG/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INSECURE_REGISTER_RECEIVER_FLAG/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INTENT_REDIRECTION/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INTENT_REDIRECTION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INTENT_REDIRECTION/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INTENT_REDIRECTION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INTENT_REDIRECTION/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INTENT_REDIRECTION/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/PATH_TRAVERSAL/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/PATH_TRAVERSAL/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/PATH_TRAVERSAL/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/PATH_TRAVERSAL/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/PATH_TRAVERSAL/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/PATH_TRAVERSAL/recommendation.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-**Input Validation:** Thoroughly validate user-supplied input to ensure it conforms to the expected format and does
-not contain any malicious characters or sequences. Sanitize and normalize file paths to prevent any 
-unauthorized navigation.
+**Path containment:** Normalize the path and check whether it's contained within the destination directory or not. 
 
 === "Dart"
 	```dart
 	import 'package:file/local.dart';
 	import 'dart:io';
 	
 	void main() {
```

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/STACK_TRACE_INFORMATION_DISCLOSURE/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_STORAGE/meta.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5991071428571428%*

 * *Differences: {"'categories'": "{'OWASP_MASVS_L1': ['MSTG_ARCH_4', 'MSTG_ARCH_12'], 'OWASP_MASVS_L2': "*

 * *                 "['MSTG_ARCH_4', 'MSTG_ARCH_12'], 'PCI_STANDARDS': {insert: [(0, 'REQ_3_2'), (1, "*

 * *                 "'REQ_3_3'), (2, 'REQ_3_5'), (3, 'REQ_3_6'), (4, 'REQ_3_7'), (5, 'REQ_4_2')], "*

 * *                 "delete: [3, 2, 0]}, 'GDPR': ['ART_32', 'ART_25']}",*

 * * "'privacy_issue'": 'True',*

 * * "'references'": "{replace: OrderedDict([('OWASP Mobile Top 10', "*

 * *                 "'https://owasp.org/www-project-mobile-top- […]*

```diff
@@ -1,25 +1,36 @@
 {
     "categories": {
+        "GDPR": [
+            "ART_32",
+            "ART_25"
+        ],
         "OWASP_MASVS_L1": [
-            "MSTG_CODE_6"
+            "MSTG_ARCH_4",
+            "MSTG_ARCH_12"
         ],
         "OWASP_MASVS_L2": [
-            "MSTG_CODE_6"
+            "MSTG_ARCH_4",
+            "MSTG_ARCH_12"
         ],
         "PCI_STANDARDS": [
-            "REQ_2_2",
-            "REQ_6_2",
-            "REQ_6_3",
-            "REQ_11_3"
+            "REQ_3_2",
+            "REQ_3_3",
+            "REQ_3_5",
+            "REQ_3_6",
+            "REQ_3_7",
+            "REQ_4_2",
+            "REQ_6_2"
         ]
     },
-    "privacy_issue": false,
+    "privacy_issue": true,
     "references": {
-        "CWE-209: Information Exposure Through an Error Message": "https://cwe.mitre.org/data/definitions/209.html",
-        "OWASP Error Handling, Auditing and Logging": "https://www.owasp.org/index.php/Error_Handling,_Auditing_and_Logging"
+        "CWE-200: Information Exposure": "http://cwe.mitre.org/data/definitions/200.html",
+        "CWE-359: Exposure of Private Information (\"Privacy Violation\")": "http://cwe.mitre.org/data/definitions/359.html",
+        "OWASP Mobile Top 10": "https://owasp.org/www-project-mobile-top-10/2023-risks/m9-insecure-data-storage",
+        "Practices for Protecting Electronic Restricted Data: A Quick Reference": "http://its.ucsc.edu/policies/rdpp.html"
     },
-    "risk_rating": "medium",
+    "risk_rating": "high",
     "security_issue": true,
-    "short_description": "An exception error page containing technical information was triggered when unexpected input was submitted to the application on the server.",
-    "title": "Stack traces reveal technical information"
+    "short_description": "Insecure storage of application data allowing other apps to read it and/or tamper with it.",
+    "title": "Insecure Storage of Application Data"
 }
```

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/UNTRUSTED_EXTERNAL_STORAGE_ACCESS/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/OAUTH_SCHEME_ACCOUNT_TAKEOVER/meta.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5989583333333334%*

 * *Differences: {"'categories'": "{'OWASP_MASVS_L1': ['MSTG_PLATFORM_3', 'MSTG_PLATFORM_4', 'MSTG_STORAGE_6'], "*

 * *                 "'OWASP_MASVS_L2': ['MSTG_PLATFORM_3', 'MSTG_PLATFORM_4', 'MSTG_NETWORK_5', "*

 * *                 "'MSTG_STORAGE_6'], 'PCI_STANDARDS': {insert: [(3, 'REQ_8_3')], delete: [5, 2, "*

 * *                 '1]}}',*

 * * "'references'": "{replace: OrderedDict([('Danielfett', "*

 * *                 "'https://danielfett.de/2020/11/27/improving-app2app/'), ('PortSwigger', "*

 * *                 "'https://portswigger.net/web- […]*

```diff
@@ -1,28 +1,34 @@
 {
     "categories": {
         "OWASP_MASVS_L1": [
-            "MSTG_STORAGE_2"
+            "MSTG_PLATFORM_3",
+            "MSTG_PLATFORM_4",
+            "MSTG_STORAGE_6"
         ],
         "OWASP_MASVS_L2": [
-            "MSTG_STORAGE_2"
+            "MSTG_PLATFORM_3",
+            "MSTG_PLATFORM_4",
+            "MSTG_NETWORK_5",
+            "MSTG_STORAGE_6"
         ],
         "PCI_STANDARDS": [
             "REQ_2_2",
-            "REQ_3_6",
-            "REQ_3_7",
             "REQ_6_2",
             "REQ_6_3",
-            "REQ_7_3",
+            "REQ_8_3",
             "REQ_11_3"
         ]
     },
-    "cvss_v3_vector": "CVSS:3.0/AV:L/AC:L/PR:H/UI:N/S:U/C:H/I:L/A:N",
     "privacy_issue": true,
     "references": {
-        "Do not store sensitive information on external storage (SD card) unless encrypted first": "https://www.securecoding.cert.org/confluence/display/android/DRD00.+Do+not+store+sensitive+information+on+external+storage+%28SD+card%29+unless+encrypted+first"
+        "Android Developer": "https://developer.android.com/training/app-links/verify-android-applinks",
+        "Apple Developer": "https://developer.apple.com/documentation/xcode/supporting-associated-domains",
+        "Danielfett": "https://danielfett.de/2020/11/27/improving-app2app/",
+        "Google Developer": "https://developers.googleblog.com/2023/10/enhancing-oauth-app-impersonation-protections.html",
+        "PortSwigger": "https://portswigger.net/web-security/oauth"
     },
-    "risk_rating": "medium",
+    "risk_rating": "high",
     "security_issue": true,
-    "short_description": "The application may access untrusted files from the external storage.",
-    "title": "Untrusted External Storage File Access"
+    "short_description": "This vulnerability occurs when an application uses a custom scheme in the 'redirect_uri' parameter during OAuth authentication.",
+    "title": "OAuth Account Takeover by hijacking custom schemes"
 }
```

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/WEBVIEW_LOADURL_INJECTION/context.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/WEBVIEW_LOADURL_INJECTION/context.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/WEBVIEW_LOADURL_INJECTION/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/WEBVIEW_LOADURL_INJECTION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/WEBVIEW_LOADURL_INJECTION/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/WEBVIEW_LOADURL_INJECTION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/WEBVIEW_LOADURL_INJECTION/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/WEBVIEW_LOADURL_INJECTION/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/APK_BACKUP_TITLE/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/APK_BACKUP_TITLE/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/APK_BACKUP_TITLE/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/APK_BACKUP_TITLE/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/APK_BACKUP_TITLE/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/APK_BACKUP_TITLE/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/APK_SERVICE_WITHOUT_PERMISSION/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/APK_SERVICE_WITHOUT_PERMISSION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/APK_SERVICE_WITHOUT_PERMISSION/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/APK_SERVICE_WITHOUT_PERMISSION/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_BACKUP_SECURE/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_BACKUP_SECURE/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_CHECK_ROOT/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_CHECK_ROOT/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_CHECK_ROOT/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_CHECK_ROOT/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_DEBUG_SECURE/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_DEBUG_SECURE/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_DEBUG_SECURE/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_SECURE/APK_DEBUG_SECURE/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/DEPENDENCY_CONFUSION/context.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/DEPENDENCY_CONFUSION/context.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/DEPENDENCY_CONFUSION/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/DEPENDENCY_CONFUSION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/DEPENDENCY_CONFUSION/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/DEPENDENCY_CONFUSION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/FORMAT_STRING/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/FORMAT_STRING/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/FORMAT_STRING/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/FORMAT_STRING/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/FORMAT_STRING/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/FORMAT_STRING/recommendation.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-To mitigate vulnerabilities related to format string attacks, it is crucial to follow certain practices. Input validation and sanitization should be implemented to ensure that user-supplied data is properly formatted and does not contain any malicious code. Additionally, developers should avoid using format string functions that accept user input directly, and instead use safer alternatives like string concatenation or formatted printing functions that do not rely on user-controlled format strings.
+To mitigate vulnerabilities related to format string attacks, it is crucial to follow certain practices: 
+
+- Avoid using format string functions that accept user input directly, and instead use safer alternatives like string concatenation or formatted printing functions that do not rely on user-controlled format strings.
+- Input validation and sanitization as a hardening measure to ensure that user-supplied data matches the expected format. 
 
 ### Code Examples:
 
 === "C"
   ```c
   #include <stdio.h>
```

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/CORS_MISCONFIGURATION/context.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/CORS_MISCONFIGURATION/context.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/CORS_MISCONFIGURATION/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/CORS_MISCONFIGURATION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/CORS_MISCONFIGURATION/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/CORS_MISCONFIGURATION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/CORS_MISCONFIGURATION/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/CORS_MISCONFIGURATION/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/DEPRECATED_COMPONENT/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/DEPRECATED_COMPONENT/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_HOSTNAME_VALIDATION/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_HOSTNAME_VALIDATION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_JWT_SIGNATURE/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_JWT_SIGNATURE/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_JWT_SIGNATURE/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_JWT_SIGNATURE/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_JWT_SIGNATURE/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_JWT_SIGNATURE/recommendation.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-To mitigate these vulnerabilities, it is crucial to implement robust security measures, including using strong encryption and secure algorithms, practicing secure key management, properly validating and verifying tokens, and following best practices for secure token transmission and storage.
+To mitigate JWT signature vulnerabilities, it is crucial to use standardized JWT libraries, properly set them up and verify signature and expiration of JWT tokens before any operation.  
+
+It's also crucial to securely store the `secret key` as it can render any security mitigations useless if it gets leaked.
 
 === "Kotlin"
 	```kotlin
 	import io.jsonwebtoken.JwtException
 	import io.jsonwebtoken.Jwts
 	import io.jsonwebtoken.SignatureAlgorithm
 	import io.jsonwebtoken.security.Keys
```

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_REPUTATION/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_REPUTATION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_REPUTATION/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_REPUTATION/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_STORAGE/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/LEAKING_PERSONAL_INFORMATION/meta.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7589285714285714%*

 * *Differences: {"'categories'": "{'OWASP_MASVS_L1': {delete: [0]}, 'OWASP_MASVS_L2': {delete: [0]}}",*

 * * "'references'": "{delete: ['OWASP Mobile Top 10']}",*

 * * "'security_issue'": 'False',*

 * * "'short_description'": "'Personally Identifiable Information were detected leaked in a "*

 * *                        "world-readable file.'",*

 * * "'title'": "'Personally Identifiable Information (PII) Leakage'"}*

```diff
@@ -1,19 +1,17 @@
 {
     "categories": {
         "GDPR": [
             "ART_32",
             "ART_25"
         ],
         "OWASP_MASVS_L1": [
-            "MSTG_ARCH_4",
             "MSTG_ARCH_12"
         ],
         "OWASP_MASVS_L2": [
-            "MSTG_ARCH_4",
             "MSTG_ARCH_12"
         ],
         "PCI_STANDARDS": [
             "REQ_3_2",
             "REQ_3_3",
             "REQ_3_5",
             "REQ_3_6",
@@ -22,15 +20,14 @@
             "REQ_6_2"
         ]
     },
     "privacy_issue": true,
     "references": {
         "CWE-200: Information Exposure": "http://cwe.mitre.org/data/definitions/200.html",
         "CWE-359: Exposure of Private Information (\"Privacy Violation\")": "http://cwe.mitre.org/data/definitions/359.html",
-        "OWASP Mobile Top 10": "https://owasp.org/www-project-mobile-top-10/2023-risks/m9-insecure-data-storage",
         "Practices for Protecting Electronic Restricted Data: A Quick Reference": "http://its.ucsc.edu/policies/rdpp.html"
     },
     "risk_rating": "high",
-    "security_issue": true,
-    "short_description": "Insecure storage of application data allowing other apps to read it and/or tamper with it.",
-    "title": "Insecure Storage of Application Data"
+    "security_issue": false,
+    "short_description": "Personally Identifiable Information were detected leaked in a world-readable file.",
+    "title": "Personally Identifiable Information (PII) Leakage"
 }
```

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_STORAGE/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_STORAGE/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_VIRUSTOTAL_SCAN/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_VIRUSTOTAL_SCAN/recommendation.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 It's essential to promptly address the issue reported by VirusTotal for the security and reliability of your application. The necessary actions will depend on the nature of the asset, your control over it, and the severity of the reported problem.
 
 Consider the following steps:
 
-Investigate why the asset was flagged as malicious. Look into specific details, such as hosting malicious content, containing malware, spam involvement, or a history of cyberattacks.
+* Investigate why the asset was flagged as malicious. Look into specific details, such as hosting malicious content, containing malware, spam involvement, or a history of cyberattacks.
 
-Isolate the asset from your primary systems if possible. Temporarily disabling or quarantining the asset can prevent potential further issues while conducting a thorough investigation.
+* Isolate the asset from your primary systems if possible. Temporarily disabling or quarantining the asset can prevent potential further issues while conducting a thorough investigation.
 
-If you have control over the service associated with the asset, take immediate steps to patch and secure it. This may involve updating software, implementing stronger security measures, and ensuring it is not utilized for malicious purposes.
+* If you have control over the service associated with the asset, take immediate steps to patch and secure it. This may involve updating software, implementing stronger security measures, and ensuring it is not utilized for malicious purposes.
```

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/LEAKING_HEALTH_INFORMATION/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_COOKIE_MISSING_SECURITY_FLAGS/meta.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5%*

 * *Differences: {"'categories'": "{replace: OrderedDict([('OWASP_ASVS_L1', ['V3_4_2']), ('OWASP_ASVS_L2', "*

 * *                 "['V3_4_2']), ('OWASP_ASVS_L3', ['V3_4_2']), ('categories', "*

 * *                 "OrderedDict([('PCI_STANDARDS', ['REQ_2_2', 'REQ_3_6', 'REQ_3_7', 'REQ_6_2', "*

 * *                 "'REQ_6_3', 'REQ_6_4', 'REQ_11_3'])]))])}",*

 * * "'cvss_v3_vector'": "'CVSS:3.0/AV:A/AC:L/PR:N/UI:N/S:U/C:H/I:N/A:N'",*

 * * "'references'": "{replace: OrderedDict([('Secure Flag (OWASP)', "*

 * *                 "'https://owasp.org/www-commu […]*

```diff
@@ -1,37 +1,34 @@
 {
     "categories": {
-        "GDPR": [
-            "ART_5",
-            "ART_25",
-            "ART_32",
-            "ART_35"
+        "OWASP_ASVS_L1": [
+            "V3_4_2"
         ],
-        "OWASP_MASVS_L1": [
-            "MSTG_ARCH_12"
+        "OWASP_ASVS_L2": [
+            "V3_4_2"
         ],
-        "OWASP_MASVS_L2": [
-            "MSTG_ARCH_12"
+        "OWASP_ASVS_L3": [
+            "V3_4_2"
         ],
-        "PCI_STANDARDS": [
-            "REQ_2_2",
-            "REQ_3_2",
-            "REQ_3_3",
-            "REQ_3_6",
-            "REQ_3_7",
-            "REQ_6_2",
-            "REQ_6_3",
-            "REQ_11_3"
-        ]
+        "categories": {
+            "PCI_STANDARDS": [
+                "REQ_2_2",
+                "REQ_3_6",
+                "REQ_3_7",
+                "REQ_6_2",
+                "REQ_6_3",
+                "REQ_6_4",
+                "REQ_11_3"
+            ]
+        }
     },
+    "cvss_v3_vector": "CVSS:3.0/AV:A/AC:L/PR:N/UI:N/S:U/C:H/I:N/A:N",
     "privacy_issue": true,
     "references": {
-        "CWE-200: Information Exposure": "http://cwe.mitre.org/data/definitions/200.html",
-        "CWE-359: Exposure of Private Information (\"Privacy Violation\")": "http://cwe.mitre.org/data/definitions/359.html",
-        "HIPAA Security Rules": "http://www.access.gpo.gov/nara/cfr/waisidx_07/45cfr160_07.html",
-        "Practices for Protecting Electronic Restricted Data: A Quick Reference": "http://its.ucsc.edu/policies/rd.html"
+        "HttpOnly Flag (OWASP)": "https://owasp.org/www-community/HttpOnly",
+        "Secure Flag (OWASP)": "https://owasp.org/www-community/controls/SecureFlag"
     },
-    "risk_rating": "high",
-    "security_issue": false,
-    "short_description": "Protected Health Information was detected on the system.",
-    "title": "Protected Health Information were detected on the system"
+    "risk_rating": "hardening",
+    "security_issue": true,
+    "short_description": "A cookie is missing security attributes like HttpOnly or Secure.",
+    "title": "Cookie missing security attributes"
 }
```

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/LEAKING_PERSONAL_INFORMATION/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/LEAKING_PERSONAL_INFORMATION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/LEAKING_PERSONAL_INFORMATION/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_INSECURE_CIPHER/meta.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5784632034632035%*

 * *Differences: {"'categories'": "{'PCI_STANDARDS': {insert: [(0, 'REQ_2_2'), (3, 'REQ_6_3'), (4, 'REQ_6_4'), (5, "*

 * *                 "'REQ_11_3')], delete: [4, 3, 2, 1, 0]}, 'OWASP_ASVS_L2': ['V6_2_3'], "*

 * *                 "'OWASP_ASVS_L3': ['V6_2_3'], delete: ['OWASP_MASVS_L1', 'OWASP_MASVS_L2', "*

 * *                 "'GDPR']}",*

 * * "'references'": "{replace: OrderedDict([('Transport Layer Protection Cheat Sheet (OWASP)', "*

 * *                 "'https://www.owasp.org/index.php/Transport_Layer_Protection_Cheat_Sheet'), "*

 * *            […]*

```diff
@@ -1,33 +1,28 @@
 {
     "categories": {
-        "GDPR": [
-            "ART_32",
-            "ART_25"
+        "OWASP_ASVS_L2": [
+            "V6_2_3"
         ],
-        "OWASP_MASVS_L1": [
-            "MSTG_ARCH_12"
-        ],
-        "OWASP_MASVS_L2": [
-            "MSTG_ARCH_12"
+        "OWASP_ASVS_L3": [
+            "V6_2_3"
         ],
         "PCI_STANDARDS": [
-            "REQ_3_2",
-            "REQ_3_3",
-            "REQ_3_5",
-            "REQ_3_6",
-            "REQ_3_7",
+            "REQ_2_2",
             "REQ_4_2",
-            "REQ_6_2"
+            "REQ_6_2",
+            "REQ_6_3",
+            "REQ_6_4",
+            "REQ_11_3"
         ]
     },
     "privacy_issue": true,
     "references": {
-        "CWE-200: Information Exposure": "http://cwe.mitre.org/data/definitions/200.html",
-        "CWE-359: Exposure of Private Information (\"Privacy Violation\")": "http://cwe.mitre.org/data/definitions/359.html",
-        "Practices for Protecting Electronic Restricted Data: A Quick Reference": "http://its.ucsc.edu/policies/rdpp.html"
+        "Mozilla Secure TLS/SSL Configuration": "https://wiki.mozilla.org/Security/Server_Side_TLS",
+        "SSL/TLS Deployment Best Practices (SSLabs)": "https://www.ssllabs.com/projects/best-practices/",
+        "Transport Layer Protection Cheat Sheet (OWASP)": "https://www.owasp.org/index.php/Transport_Layer_Protection_Cheat_Sheet"
     },
-    "risk_rating": "high",
-    "security_issue": false,
-    "short_description": "Personally Identifiable Information were detected leaked in a world-readable file.",
-    "title": "Personally Identifiable Information (PII) Leakage"
+    "risk_rating": "medium",
+    "security_issue": true,
+    "short_description": "The client supports combinations of cipher suites that suffer from known cryptographic weaknesses.",
+    "title": "Insecure TLS Ciphers supported"
 }
```

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/LEAKING_PERSONAL_INFORMATION/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/LEAKING_PERSONAL_INFORMATION/recommendation.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-* Securely delete PII when there is no longer a business need for its retention on the device
-* Do not cache sensitive data
-* Minimize the frequency of asking for user credentials.
-* Minimize the use of APIs that access sensitive or personal user data
-* Consider a logical way to hash the user data
+* When saving PII/PHI locally, make sure they're encrypted and encryption keys are stored in the KeyChain.
+* Access to the PII information should be protected by biometric authentication.
+* If applicable, avoid caching PII information locally, instead, query it from the backend servers.
+* Securely delete PII/PHI when there is no longer a business need for its retention on the device.
+* Consider encrypting and/or hashing PHI/PII data before saving it on the device.
+* Provide users with way to withdraw consent for holding their PHI/PII data.
+* Do not cache PII/PHI data.
+* Minimize the use of third party libraries and APIs that access user data.
 * Some jurisdictions may require you to provide a privacy policy for accessing personal information.
-* If saving PII information locally is necessary, consider encrypting it before.
 * If logging PII information is necessary, set the logging level to debug so that PII doesn't in production application logs.
 
 
 
 === "Kotlin"
   ```kotlin
   import android.os.Bundle
```

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/OAUTH_SCHEME_ACCOUNT_TAKEOVER/context.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/OAUTH_SCHEME_ACCOUNT_TAKEOVER/context.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/OAUTH_SCHEME_ACCOUNT_TAKEOVER/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/OAUTH_SCHEME_ACCOUNT_TAKEOVER/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/OAUTH_SCHEME_ACCOUNT_TAKEOVER/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_ALGO/meta.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5950520833333334%*

 * *Differences: {"'categories'": "{'OWASP_MASVS_L1': ['MSTG_CRYPTO_2', 'MSTG_CRYPTO_3', 'MSTG_CRYPTO_4'], "*

 * *                 "'OWASP_MASVS_L2': ['MSTG_CRYPTO_2', 'MSTG_CRYPTO_3', 'MSTG_CRYPTO_4'], "*

 * *                 "'PCI_STANDARDS': {insert: [(0, 'REQ_3_6'), (1, 'REQ_3_7'), (2, 'REQ_4_2')], "*

 * *                 'delete: [4, 3, 2, 0]}}',*

 * * "'cvss_v3_vector'": "'CVSS:3.0/AV:N/AC:L/PR:H/UI:N/S:U/C:H/I:N/A:N'",*

 * * "'references'": "{replace: OrderedDict([('Cryptographic Vulnerability (OWASP)', "*

 * *                 "'https://www.owasp […]*

```diff
@@ -1,34 +1,31 @@
 {
     "categories": {
         "OWASP_MASVS_L1": [
-            "MSTG_PLATFORM_3",
-            "MSTG_PLATFORM_4",
-            "MSTG_STORAGE_6"
+            "MSTG_CRYPTO_2",
+            "MSTG_CRYPTO_3",
+            "MSTG_CRYPTO_4"
         ],
         "OWASP_MASVS_L2": [
-            "MSTG_PLATFORM_3",
-            "MSTG_PLATFORM_4",
-            "MSTG_NETWORK_5",
-            "MSTG_STORAGE_6"
+            "MSTG_CRYPTO_2",
+            "MSTG_CRYPTO_3",
+            "MSTG_CRYPTO_4"
         ],
         "PCI_STANDARDS": [
-            "REQ_2_2",
-            "REQ_6_2",
-            "REQ_6_3",
-            "REQ_8_3",
-            "REQ_11_3"
+            "REQ_3_6",
+            "REQ_3_7",
+            "REQ_4_2",
+            "REQ_6_2"
         ]
     },
+    "cvss_v3_vector": "CVSS:3.0/AV:N/AC:L/PR:H/UI:N/S:U/C:H/I:N/A:N",
     "privacy_issue": true,
     "references": {
-        "Android Developer": "https://developer.android.com/training/app-links/verify-android-applinks",
-        "Apple Developer": "https://developer.apple.com/documentation/xcode/supporting-associated-domains",
-        "Danielfett": "https://danielfett.de/2020/11/27/improving-app2app/",
-        "Google Developer": "https://developers.googleblog.com/2023/10/enhancing-oauth-app-impersonation-protections.html",
-        "PortSwigger": "https://portswigger.net/web-security/oauth"
+        "5 Common Encryption Algorithms and the Unbreakables of the Future": "https://www.storagecraft.com/blog/5-common-encryption-algorithms/",
+        "CWE-327: Use of a Broken or Risky Cryptographic Algorithm": "https://cwe.mitre.org/data/definitions/327.html",
+        "Cryptographic Vulnerability (OWASP)": "https://www.owasp.org/index.php/Category:Cryptographic_Vulnerability"
     },
-    "risk_rating": "high",
+    "risk_rating": "medium",
     "security_issue": true,
-    "short_description": "This vulnerability occurs when an application uses a custom scheme in the 'redirect_uri' parameter during OAuth authentication.",
-    "title": "OAuth Account Takeover by hijacking custom schemes"
+    "short_description": "The client supports combinations of cipher suites that suffer from known cryptographic weaknesses.",
+    "title": "Cryptographic Vulnerability: Insecure Algorithm"
 }
```

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/OAUTH_SCHEME_ACCOUNT_TAKEOVER/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/OAUTH_SCHEME_ACCOUNT_TAKEOVER/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/REGEX_DOS/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/REGEX_DOS/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/REGEX_DOS/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/REGEX_DOS/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/REGEX_DOS/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/REGEX_DOS/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/TAPJACKING_VULNERABILITY/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/TAPJACKING_VULNERABILITY/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/TAPJACKING_VULNERABILITY/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/TAPJACKING_VULNERABILITY/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/TEMPLATE_INJECTION/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/TEMPLATE_INJECTION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/TEMPLATE_INJECTION/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/TEMPLATE_INJECTION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/TEMPLATE_INJECTION/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/TEMPLATE_INJECTION/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/XPATH_INJECTION/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/XPATH_INJECTION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/XPATH_INJECTION/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/XPATH_INJECTION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/XPATH_INJECTION/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/XPATH_INJECTION/recommendation.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-To mitigate XPath Injection vulnerabilities, it is important to properly validate and sanitize user input before using it in XPath queries. This can be done by using parameterized queries or prepared statements, which separate the user input from the query logic. Additionally, limiting the privileges of the user executing the query can help prevent unauthorized access to sensitive data. Regularly updating and patching software and libraries can also help prevent known vulnerabilities from being exploited. Finally, implementing logging and monitoring can help detect and respond to any attempted attacks.
+To mitigate XPath Injection vulnerabilities, it is important to: 
+
+* Use parameterized queries or prepared statements, which separate the user input from the query logic.
+* Properly validate and sanitize user input before using it in XPath queries. 
 
 === "Dart"
 	```dart
 	
 	bool _validate_query(String _searchQuery){
 	  // check for special characters
 	  for(var i = 0; i < tokens.length; i++){
```

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_IMPORTANT/PACKAGE_OBFUSCATED/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_IMPORTANT/PACKAGE_OBFUSCATED/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_INFO/DANGEROUS_MEMORY_CORRUPTION/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_INFO/DANGEROUS_MEMORY_CORRUPTION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_INFO/PRIVACY_API/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_INFO/PRIVACY_API/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_LOW/OUTDATED_VULNERABLE_COMPONENT/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_LOW/OUTDATED_VULNERABLE_COMPONENT/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_LOW/PROCESS_CRASHES/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_LOW/PROCESS_CRASHES/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_LOW/PROCESS_CRASHES/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_LOW/PROCESS_CRASHES/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/BIOMETRIC_AUTHENTICATION_BYPASS/context.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/BIOMETRIC_AUTHENTICATION_BYPASS/context.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/BIOMETRIC_AUTHENTICATION_BYPASS/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/BIOMETRIC_AUTHENTICATION_BYPASS/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/BIOMETRIC_AUTHENTICATION_BYPASS/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/BIOMETRIC_AUTHENTICATION_BYPASS/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/BIOMETRIC_AUTHENTICATION_BYPASS/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/BIOMETRIC_AUTHENTICATION_BYPASS/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_ALGO/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_ALGO/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_ALGO/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_MODE/meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8494791666666667%*

 * *Differences: {"'categories'": "{'PCI_STANDARDS': {insert: [(0, 'REQ_2_2')]}}",*

 * * "'references'": "{'5 Common Encryption Algorithms and the Unbreakables of the Future': "*

 * *                 "'http://www.storagecraft.com/blog/5-common-encryption-algorithms/', 'AES Default "*

 * *                 "mode discussion': "*

 * *                 "'https://security.stackexchange.com/questions/54848/what-is-default-mode-for-aes-encryption'}",*

 * * "'short_description'": "'The client supports combinations of cipher modes that suffer from known "*

 * *    […]*

```diff
@@ -7,25 +7,27 @@
         ],
         "OWASP_MASVS_L2": [
             "MSTG_CRYPTO_2",
             "MSTG_CRYPTO_3",
             "MSTG_CRYPTO_4"
         ],
         "PCI_STANDARDS": [
+            "REQ_2_2",
             "REQ_3_6",
             "REQ_3_7",
             "REQ_4_2",
             "REQ_6_2"
         ]
     },
     "cvss_v3_vector": "CVSS:3.0/AV:N/AC:L/PR:H/UI:N/S:U/C:H/I:N/A:N",
     "privacy_issue": true,
     "references": {
-        "5 Common Encryption Algorithms and the Unbreakables of the Future": "https://www.storagecraft.com/blog/5-common-encryption-algorithms/",
+        "5 Common Encryption Algorithms and the Unbreakables of the Future": "http://www.storagecraft.com/blog/5-common-encryption-algorithms/",
+        "AES Default mode discussion": "https://security.stackexchange.com/questions/54848/what-is-default-mode-for-aes-encryption",
         "CWE-327: Use of a Broken or Risky Cryptographic Algorithm": "https://cwe.mitre.org/data/definitions/327.html",
         "Cryptographic Vulnerability (OWASP)": "https://www.owasp.org/index.php/Category:Cryptographic_Vulnerability"
     },
     "risk_rating": "medium",
     "security_issue": true,
-    "short_description": "The client supports combinations of cipher suites that suffer from known cryptographic weaknesses.",
-    "title": "Cryptographic Vulnerability: Insecure Algorithm"
+    "short_description": "The client supports combinations of cipher modes that suffer from known cryptographic weaknesses.",
+    "title": "Cryptographic Vulnerability: Insecure mode"
 }
```

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_ALGO/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_ALGO/recommendation.md`

 * *Files 10% similar despite different names*

```diff
@@ -6,23 +6,16 @@
 
 To ensure the utmost security when using any cryptographic algorithm, it is essential to follow best practices:
 
 - Key Length: Use key lengths that are considered secure. For AES, 128 bits are sufficient for most use cases, but you can opt for 192 or 256 bits for more sensitive data.
 
 - Cipher Mode: Always employ secure cipher mode settings, such as AES-GCM (Galois/Counter Mode) or AES-CBC (Cipher Block Chaining) with appropriate padding.
 
-- Key Management: Implement a robust key management system to safeguard encryption keys, ensuring they are not compromised.
+- Key Management: Use secure storage mechanisms (Keystore for Android, Keychain for iOS) to safely store cryptographic keys.
 
-- Regular Updates: Stay up-to-date with the latest cryptographic standards and practices to address emerging threats and vulnerabilities.
-
-- Secure Implementation: Pay attention to secure coding practices during algorithm implementation to prevent potential vulnerabilities.
-
-- Secure Transmission: When exchanging encrypted data, ensure secure transmission protocols such as TLS (Transport Layer Security) are used to protect data in transit.
-
-By adhering to these best practices and adopting secure algorithms like AES and ECC, you can significantly enhance the security of your cryptographic operations and safeguard sensitive information from unauthorized access. Avoiding the use of insecure algorithms, such as DES and Triple DES, is crucial to maintaining a strong security posture in today's rapidly evolving threat landscape.
 
 === "Dart"
 	```dart
 	import 'dart:convert';
 	import 'dart:typed_data';
 	import 'package:flutter/material.dart';
 	import 'package:flutter/services.dart';
```

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_KEY/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_KEY/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_MODE/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_MODE/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_CIPHER_MODE/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/WEAK_HASHING_ALGO/meta.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6854166666666667%*

 * *Differences: {"'categories'": "{'PCI_STANDARDS': {delete: [3]}}",*

 * * "'references'": "{replace: OrderedDict([('Deprecating MD5 and SHA-1 signature hashes in (D)TLS "*

 * *                 "1.2', "*

 * *                 "'https://www.ietf.org/archive/id/draft-ietf-tls-md5-sha1-deprecate-09.html'), "*

 * *                 "('Deprecation of SHA-1 (NIST)', "*

 * *                 "'https://www.nist.gov/news-events/news/2022/12/nist-retires-sha-1-cryptographic-algorithm')])}",*

 * * "'short_description'": "'The client uses weak hashing functions that  […]*

```diff
@@ -10,24 +10,20 @@
             "MSTG_CRYPTO_3",
             "MSTG_CRYPTO_4"
         ],
         "PCI_STANDARDS": [
             "REQ_2_2",
             "REQ_3_6",
             "REQ_3_7",
-            "REQ_4_2",
             "REQ_6_2"
         ]
     },
-    "cvss_v3_vector": "CVSS:3.0/AV:N/AC:L/PR:H/UI:N/S:U/C:H/I:N/A:N",
     "privacy_issue": true,
     "references": {
-        "5 Common Encryption Algorithms and the Unbreakables of the Future": "http://www.storagecraft.com/blog/5-common-encryption-algorithms/",
-        "AES Default mode discussion": "https://security.stackexchange.com/questions/54848/what-is-default-mode-for-aes-encryption",
-        "CWE-327: Use of a Broken or Risky Cryptographic Algorithm": "https://cwe.mitre.org/data/definitions/327.html",
-        "Cryptographic Vulnerability (OWASP)": "https://www.owasp.org/index.php/Category:Cryptographic_Vulnerability"
+        "Deprecating MD5 and SHA-1 signature hashes in (D)TLS 1.2": "https://www.ietf.org/archive/id/draft-ietf-tls-md5-sha1-deprecate-09.html",
+        "Deprecation of SHA-1 (NIST)": "https://www.nist.gov/news-events/news/2022/12/nist-retires-sha-1-cryptographic-algorithm"
     },
     "risk_rating": "medium",
     "security_issue": true,
-    "short_description": "The client supports combinations of cipher modes that suffer from known cryptographic weaknesses.",
-    "title": "Cryptographic Vulnerability: Insecure mode"
+    "short_description": "The client uses weak hashing functions that suffer from known cryptographic weaknesses.",
+    "title": "Cryptographic Vulnerability: Weak Hashing Algorithm"
 }
```

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_IV/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_IV/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_IV/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/CRYPTO_INSECURE_IV/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/HTML_INJECTION/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/HTML_INJECTION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/HTML_INJECTION/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/HTML_INJECTION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/HTML_INJECTION/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/HTML_INJECTION/recommendation.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-To mitigate the risks associated with HTML injection vulnerabilities, the following recommendations should be implemented:
+To mitigate the risks associated with HTML injection vulnerabilities, consider the following recommendations:
 
-- Sanitize User Input: Perform proper input validation and sanitization on user-supplied data that will be rendered as part of HTML code. Use encoding techniques to ensure that user input is treated as data and not executable code.
+- **Contextual Output Encoding:** Encode user-generated content based on its context. Different contexts, such as HTML attributes, JavaScript code, or CSS styles, require specific encoding techniques to prevent HTML injection attacks. Use appropriate encoding functions or libraries based on the context.
 
-- Use Templating Engines: Utilize secure templating engines or frameworks that automatically escape user input by default, such as Handlebars, Twig, or Django templates. These engines help prevent HTML injection by properly handling user input.
+- **Sanitize User Input:** Perform proper input validation and sanitization on user-supplied data by stripping any special HTML characters before rendering it as part of HTML code. 
 
-- Whitelisting Input: Implement whitelisting or allow listing approaches to validate and restrict input for HTML elements, attributes, and protocols. Only allow specific tags, attributes, and protocols that are necessary for the application's functionality.
+- **Disable Javascript if not needed:** in the context of mobile webviews, disabling Javascript can help significantly reduce the impact of any potential HTML injection.
+
+- **Use Logic-less Templating Engines:** Templating engines like `Mustache` can help prevent HTML injection by properly handling user input.
 
-- Contextual Output Encoding: Encode user-generated content based on its context. Different contexts, such as HTML attributes, JavaScript code, or CSS styles, require specific encoding techniques to prevent HTML injection attacks. Use appropriate encoding functions or libraries based on the context.
 
 === "Dart"
 	```dart
 	import 'package:flutter/material.dart';
 	import 'package:webview_flutter/webview_flutter.dart';
 	import 'package:sanitize_html/sanitize_html.dart' show sanitizeHtml;
 	
@@ -91,40 +92,39 @@
 	```
 
 
 === "Swift"
 	```Swift
 	import UIKit
 	import WebKit
-	import DOMPurify
 	
 	class ViewController: UIViewController, WKNavigationDelegate {
-	    
-	    private var webView: WKWebView!
-	
-	    override func viewDidLoad() {
-	        super.viewDidLoad()
-	        
-	        webView = WKWebView(frame: view.bounds)
-	        webView.navigationDelegate = self
-	        view.addSubview(webView)
-	        
-	        let name = "John Doe"
-	        let plainText = "Hello, \(name)!"
-	        let sanitizedText = sanitizeHTML(plainText)
-	        let html = "<html><body><h1>\(sanitizedText)</h1></body></html>"
-	        webView.loadHTMLString(html, baseURL: nil)
-	    }
-	    
-	    private func sanitizeHTML(_ html: String) -> String {
-	        guard let sanitized = DOMPurify.sanitize(html) else {
-	            return ""
-	        }
-	        return sanitized
-	    }
+			
+			private var webView: WKWebView!
+			
+			override func viewDidLoad() {
+					super.viewDidLoad()
+					
+					webView = WKWebView(frame: view.bounds)
+					webView.navigationDelegate = self
+					view.addSubview(webView)
+					
+					let name = "John Doe"
+					let plainText = "Hello, \(name)!"
+					let sanitizedText = sanitizeHTML(plainText)
+					let html = "<html><body><h1>\(sanitizedText)</h1></body></html>"
+					webView.loadHTMLString(html, baseURL: nil)
+			}
+			
+			private func sanitizeHTML(_ html: String) -> String {
+					// Replace any '<' and '>' characters with HTML entities
+					let sanitized = html.replacingOccurrences(of: "<", with: "&lt;")
+															.replacingOccurrences(of: ">", with: "&gt;")
+					return sanitized
+			}
 	}
 	```
 
 
 
 === "Kotlin"
 	```kotlin
```

#### html2text {}

```diff
@@ -1,57 +1,54 @@
-To mitigate the risks associated with HTML injection vulnerabilities, the
-following recommendations should be implemented: - Sanitize User Input: Perform
-proper input validation and sanitization on user-supplied data that will be
-rendered as part of HTML code. Use encoding techniques to ensure that user
-input is treated as data and not executable code. - Use Templating Engines:
-Utilize secure templating engines or frameworks that automatically escape user
-input by default, such as Handlebars, Twig, or Django templates. These engines
-help prevent HTML injection by properly handling user input. - Whitelisting
-Input: Implement whitelisting or allow listing approaches to validate and
-restrict input for HTML elements, attributes, and protocols. Only allow
-specific tags, attributes, and protocols that are necessary for the
-application's functionality. - Contextual Output Encoding: Encode user-
+To mitigate the risks associated with HTML injection vulnerabilities, consider
+the following recommendations: - **Contextual Output Encoding:** Encode user-
 generated content based on its context. Different contexts, such as HTML
 attributes, JavaScript code, or CSS styles, require specific encoding
 techniques to prevent HTML injection attacks. Use appropriate encoding
-functions or libraries based on the context. === "Dart" ```dart import
-'package:flutter/material.dart'; import 'package:webview_flutter/
-webview_flutter.dart'; import 'package:sanitize_html/sanitize_html.dart' show
-sanitizeHtml; void main() => runApp(MyApp()); class MyApp extends
-StatelessWidget { @override Widget build(BuildContext context) { return
-MaterialApp( title: 'HTML Injection Demo', theme: ThemeData( primarySwatch:
-Colors.blue, ), home: WebViewScreen(), ); } } class WebViewScreen extends
-StatefulWidget { @override _WebViewScreenState createState() =>
-_WebViewScreenState(); } class _WebViewScreenState extends State { late
-WebViewController _webViewController; String? htmlInput; @override void
-initState() { super.initState(); getHtmlInputFromIntent(); } void
+functions or libraries based on the context. - **Sanitize User Input:** Perform
+proper input validation and sanitization on user-supplied data by stripping any
+special HTML characters before rendering it as part of HTML code. - **Disable
+Javascript if not needed:** in the context of mobile webviews, disabling
+Javascript can help significantly reduce the impact of any potential HTML
+injection. - **Use Logic-less Templating Engines:** Templating engines like
+`Mustache` can help prevent HTML injection by properly handling user input. ===
+"Dart" ```dart import 'package:flutter/material.dart'; import 'package:
+webview_flutter/webview_flutter.dart'; import 'package:sanitize_html/
+sanitize_html.dart' show sanitizeHtml; void main() => runApp(MyApp()); class
+MyApp extends StatelessWidget { @override Widget build(BuildContext context)
+{ return MaterialApp( title: 'HTML Injection Demo', theme: ThemeData
+( primarySwatch: Colors.blue, ), home: WebViewScreen(), ); } } class
+WebViewScreen extends StatefulWidget { @override _WebViewScreenState
+createState() => _WebViewScreenState(); } class _WebViewScreenState extends
+State { late WebViewController _webViewController; String? htmlInput; @override
+void initState() { super.initState(); getHtmlInputFromIntent(); } void
 getHtmlInputFromIntent() { // Retrieve the intent extras Map
  dynamic>? extras = ModalRoute.of(context)?.settings.arguments as Map
  dynamic>?; // Extract the user input from the intent extras htmlInput =
 extras?['htmlInput']; } void _injectHtml() async { if (htmlInput != null)
 { final sanitizedHtml = sanitizeHtml(htmlInput); await
 _webViewController.loadUrl( Uri.dataFromString(sanitizedHtml, mimeType: 'text/
 html', encoding: Encoding.getByName('utf-8'))!.toString(), ); } } @override
 Widget build(BuildContext context) { return Scaffold( appBar: AppBar( title:
 Text('HTML Injection Demo'), ), body: Column( children: [ ElevatedButton
 ( onPressed: _injectHtml, child: Text('Inject HTML'), ), Expanded( child:
 WebView( initialUrl: 'about:blank', onWebViewCreated: (WebViewController
 controller) { _webViewController = controller; }, ), ), ], ), ); } } ``` ===
-"Swift" ```Swift import UIKit import WebKit import DOMPurify class
-ViewController: UIViewController, WKNavigationDelegate { private var webView:
-WKWebView! override func viewDidLoad() { super.viewDidLoad() webView =
-WKWebView(frame: view.bounds) webView.navigationDelegate = self view.addSubview
-(webView) let name = "John Doe" let plainText = "Hello, \(name)!" let
-sanitizedText = sanitizeHTML(plainText) let html = "
+"Swift" ```Swift import UIKit import WebKit class ViewController:
+UIViewController, WKNavigationDelegate { private var webView: WKWebView!
+override func viewDidLoad() { super.viewDidLoad() webView = WKWebView(frame:
+view.bounds) webView.navigationDelegate = self view.addSubview(webView) let
+name = "John Doe" let plainText = "Hello, \(name)!" let sanitizedText =
+sanitizeHTML(plainText) let html = "
 ************ \\((ssaanniittiizzeeddTTeexxtt)) ************
 " webView.loadHTMLString(html, baseURL: nil) } private func sanitizeHTML(_
-html: String) -> String { guard let sanitized = DOMPurify.sanitize(html) else
-{ return "" } return sanitized } } ``` === "Kotlin" ```kotlin import
-android.annotation.SuppressLint import android.os.Bundle import
-android.webkit.WebSettings import android.webkit.WebView import
+html: String) -> String { // Replace any '<' and '>' characters with HTML
+entities let sanitized = html.replacingOccurrences(of: "<", with: "<")
+.replacingOccurrences(of: ">", with: ">") return sanitized } } ``` === "Kotlin"
+```kotlin import android.annotation.SuppressLint import android.os.Bundle
+import android.webkit.WebSettings import android.webkit.WebView import
 androidx.appcompat.app.AppCompatActivity class MainActivity : AppCompatActivity
 () { private lateinit var webView: WebView PolicyFactory policy = new
 HtmlPolicyBuilder() .allowElements("a") .allowUrlProtocols("https")
 .allowAttributes("href").onElements("a") .requireRelNofollowOnLinks() .build();
 override fun onCreate(savedInstanceState: Bundle?) { super.onCreate
 (savedInstanceState) setContentView(R.layout.activity_main) webView =
 findViewById(R.id.webView) val name = intent.getStringExtra("name") val
```

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_DYNAMICALLY_LINKED_LIBRARY/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_DYNAMICALLY_LINKED_LIBRARY/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_DYNAMICALLY_LINKED_LIBRARY/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_DYNAMICALLY_LINKED_LIBRARY/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_DYNAMICALLY_LINKED_LIBRARY/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_DYNAMICALLY_LINKED_LIBRARY/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_PASSWORD_STORAGE/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_PASSWORD_STORAGE/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_PERMISSION_FILESYSTEM/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/IPA_STACK_SMASHING_DISABLED/meta.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5921875%*

 * *Differences: {"'categories'": "{'OWASP_MASVS_L1': ['MSTG_CODE_9'], 'OWASP_MASVS_L2': ['MSTG_CODE_9'], "*

 * *                 "'PCI_STANDARDS': {delete: [3]}, delete: ['CWE_TOP_25']}",*

 * * "'cvss_v3_vector'": "'CVSS:3.0/AV:N/AC:H/PR:N/UI:N/S:U/C:N/I:H/A:H'",*

 * * "'privacy_issue'": 'False',*

 * * "'references'": "{replace: OrderedDict([('Stack Smashing Protection (OSdev)', "*

 * *                 "'http://wiki.osdev.org/Stack_Smashing_Protector'), ('Xcode 3 supports Stack "*

 * *                 "Canaries', "*

 * *                 "'http://lists.apple […]*

```diff
@@ -1,29 +1,26 @@
 {
     "categories": {
-        "CWE_TOP_25": [
-            "CWE_276"
-        ],
         "OWASP_MASVS_L1": [
-            "MSTG_STORAGE_2"
+            "MSTG_CODE_9"
         ],
         "OWASP_MASVS_L2": [
-            "MSTG_STORAGE_2"
+            "MSTG_CODE_9"
         ],
         "PCI_STANDARDS": [
             "REQ_2_2",
             "REQ_6_2",
             "REQ_6_3",
-            "REQ_7_3",
             "REQ_11_3"
         ]
     },
-    "cvss_v3_vector": "CVSS:3.1/AV:L/AC:L/PR:H/UI:N/S:C/C:H/I:H/A:N",
-    "privacy_issue": true,
+    "cvss_v3_vector": "CVSS:3.0/AV:N/AC:H/PR:N/UI:N/S:U/C:N/I:H/A:H",
+    "privacy_issue": false,
     "references": {
-        "Ensure sensitive data are kept secret(CERT Secure Coding)": "https://www.securecoding.cert.org/confluence/display/android/DRD11.+Ensure+that+sensitive+data+is+kept+secure"
+        "Stack Smashing Protection (OSdev)": "http://wiki.osdev.org/Stack_Smashing_Protector",
+        "Xcode 3 supports Stack Canaries": "http://lists.apple.com/archives/xcode-users/2007/Dec/msg00055.html"
     },
-    "risk_rating": "medium",
+    "risk_rating": "hardening",
     "security_issue": true,
-    "short_description": "Filesystem access using weak permissions.",
-    "title": "Insecure Filesystem Access"
+    "short_description": "The application does not enforce Stack Smashing Protection (SSP).",
+    "title": "Stack smashing protection not enforced"
 }
```

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_RANDOM_SEED/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_RANDOM_SEED/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/LEAKING_CREDENTIALS_LOGS/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/LEAKING_CREDENTIALS_LOGS/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/LEAKING_CREDENTIALS_REQUEST/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/LEAKING_CREDENTIALS_REQUEST/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/MEMORY_LEAK/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/MEMORY_LEAK/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/SQL_INJECTION/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/SQL_INJECTION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/SQL_INJECTION/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/SQL_INJECTION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/WEAK_HASHING_ALGO/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/WEAK_HASHING_ALGO/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/XML_INJECTION/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/XML_INJECTION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/XML_INJECTION/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/XML_INJECTION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/XML_INJECTION/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/XML_INJECTION/recommendation.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,12 @@
-To mitigate XML injection vulnerabilities, it is crucial to implement proper input validation and sanitization techniques. Validate user input against expected formats, and sanitize it by removing or escaping characters that could be interpreted as XML tags or entities. Additionally, consider using secure XML parsing libraries or APIs that handle data binding securely.
+To mitigate XML injection vulnerabilities, consider:
+
+- Implement proper input validation and sanitization techniques. 
+- Validate user input against expected formats, and sanitize it by removing or escaping characters that could be interpreted as XML tags or entities. 
+- Consider using secure XML parsing libraries or APIs that handle data binding securely.
 
 === "Dart"
 	```dart
 	import 'dart:convert';
 	import 'dart:io';
 	
 	import 'package:flutter/material.dart';
```

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/ZIP_FILE_VULNERABILITIES/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/ZIP_FILE_VULNERABILITIES/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/ZIP_FILE_VULNERABILITIES/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/ZIP_FILE_VULNERABILITIES/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/ZIP_FILE_VULNERABILITIES/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/ZIP_FILE_VULNERABILITIES/recommendation.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+To mitigate the risks associated with zip files, consider the following:
+
+- For each zip entry to extract, standardize the path using a standard library and check if it's contained within the extraction directory.
 - Implement proper input validation and sanitization to prevent user-supplied input from containing directory traversal sequences.
-- Use whitelisting or allowlisting approaches to validate and restrict input for file paths.
-- Ensure that the extracted file paths are constructed based on trusted and validated information rather than relying solely on user-provided data.
-- Restrict the extraction process to a specific directory or set of allowed directories.
 
 === "Dart"
 	```dart
 	import 'dart:io';
 	import 'archive/archive.dart';
 	
 	void extractZipFile(String path) {
```

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/PORT_OPEN_LOCALHOST/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/PORT_OPEN_LOCALHOST/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/SECRETS_REVIEW/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/SECRETS_REVIEW/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/SECRETS_REVIEW/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/SECRETS_REVIEW/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/SECRETS_REVIEW/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/SECRETS_REVIEW/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/URL_MANIPULATION/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/URL_MANIPULATION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/URL_MANIPULATION/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/URL_MANIPULATION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/URL_MANIPULATION/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_POTENTIALLY/URL_MANIPULATION/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/ATS_MALFORMATTED/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/ATS_MALFORMATTED/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/ATS_MALFORMATTED/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/ATS_MALFORMATTED/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/IPA_ARC_DISABLED/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/IPA_ARC_DISABLED/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_INSECURE_PRIVACY_MANIFEST_FILE/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_INSECURE_PRIVACY_MANIFEST_FILE/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_INSECURE_PRIVACY_MANIFEST_FILE/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_INSECURE_PRIVACY_MANIFEST_FILE/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_INSECURE_PRIVACY_MANIFEST_FILE/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_INSECURE_PRIVACY_MANIFEST_FILE/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_URL_SCHEME_INJECTION/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_URL_SCHEME_INJECTION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_URL_SCHEME_INJECTION/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_URL_SCHEME_INJECTION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_IMPORTANT/IPA_ENCRYPTED/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_IMPORTANT/IPA_ENCRYPTED/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_URL_SCHEME_LIST/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_URL_SCHEME_LIST/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/IPA_DEBUG_SYMBOL_PRESENT/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/IPA_DEBUG_SYMBOL_PRESENT/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/IPA_KEYBOARD_CACHE/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/IPA_KEYBOARD_CACHE/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/PLIST_INSECURE_UI_FILE_SHARING/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_LOW/PLIST_INSECURE_UI_FILE_SHARING/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_ASLR_DISABLED/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_ASLR_DISABLED/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_INSECURE_TAP/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_INSECURE_TAP/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_INSECURE_TAP/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_INSECURE_TAP/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_URL_SCHEME_HIJACKING/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_URL_SCHEME_HIJACKING/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_URL_SCHEME_HIJACKING/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_MEDIUM/IPA_URL_SCHEME_HIJACKING/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/IPA_ANTI_DEBUG/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/IPA_ANTI_DEBUG/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/IPA_SECURE_PRIVACY_MANIFEST_FILE/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/IPA_SECURE_PRIVACY_MANIFEST_FILE/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/PRIVACY_NO_SENSITIVE_DATA_OUTSIDE_APP_CONTAINER/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/PRIVACY_NO_SENSITIVE_DATA_OUTSIDE_APP_CONTAINER/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/PRIVACY_NO_SENSITIVE_DATA_OUTSIDE_APP_CONTAINER/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_SECURE/PRIVACY_NO_SENSITIVE_DATA_OUTSIDE_APP_CONTAINER/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_HARDENING/PHONEGAP_WHITELIST_CONFIG/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_HARDENING/PHONEGAP_WHITELIST_CONFIG/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_HIGH/SOURCE_MAP_CODE_LEAK/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_HIGH/SOURCE_MAP_CODE_LEAK/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_MEDIUM/CORDOVA_XSS/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_MEDIUM/CORDOVA_XSS/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_MEDIUM/CORDOVA_XSS/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_MEDIUM/CORDOVA_XSS/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_MEDIUM/CORDOVA_XSS/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_MEDIUM/CORDOVA_XSS/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_MEDIUM/PHONEGAP_WEAK_WHITELIST_CONFIG/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/MOBILE_CLIENT/MULTIPLATFORM_JS/_MEDIUM/PHONEGAP_WEAK_WHITELIST_CONFIG/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/README.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/README.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/CLOUD/_MEDIUM/AWS_S3_PUBLIC_FILELIST_ENABLED/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/CLOUD/_MEDIUM/AWS_S3_PUBLIC_FILELIST_ENABLED/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/CLOUD/_SECURE/FIREBASE_SECURE_DATABASE_PERMISSIONS/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/CLOUD/_SECURE/FIREBASE_SECURE_DATABASE_PERMISSIONS/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/DNS/_MEDIUM/SUBDOMAIN_TAKEOVER/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/DNS/_MEDIUM/SUBDOMAIN_TAKEOVER/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/DNS/_POTENTIALLY/EXTERNAL_DNS_INTERACTION/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/DNS/_POTENTIALLY/EXTERNAL_DNS_INTERACTION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/ACCOUNT_TAKEOVER/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/ACCOUNT_TAKEOVER/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/ACCOUNT_TAKEOVER/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/ACCOUNT_TAKEOVER/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/ACCOUNT_TAKEOVER/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/ACCOUNT_TAKEOVER/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/CODE_INJECTION/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/CODE_INJECTION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/CODE_INJECTION/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/CODE_INJECTION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/CODE_INJECTION/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/CODE_INJECTION/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/COMMAND_INJECTION/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/COMMAND_INJECTION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/COMMAND_INJECTION/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/COMMAND_INJECTION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/COMMAND_INJECTION/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/COMMAND_INJECTION/recommendation.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 To mitigate the command injection vulnerability, here are some recommendations:
 
-- __Input Validation and Sanitization__: Always validate and sanitize user inputs. Ensure that any user-supplied data passed to the system shell or command execution functions is sanitized and restricted to expected characters or patterns.
-
-
-- __Least Privilege Principle__: Run your application or services with the least possible privileges required to perform necessary actions. Avoid running services with superuser or administrator privileges.
+- __Avoid Executing User-Supplied Input__: Refrain from executing user-supplied data directly within commands or system shells. Validate and use whitelists or predefined options wherever possible.
 
+- __Avoid Concatenation__: Avoid directly concatenating user input into system commands, instead pass it in a separate list of arguments.
 
-- __Avoid Executing User-Supplied Input__: Refrain from executing user-supplied data directly within commands or system shells. Validate and use whitelists or predefined options wherever possible.
+- __Input Validation and Sanitization__: Always validate and sanitize user inputs. Ensure that any user-supplied data passed to the system shell or command execution functions is sanitized and restricted to expected characters or patterns.
 
+- __Least Privilege Principle__: Run your application or services with the least possible privileges required to perform necessary actions. Avoid running services with superuser or administrator privileges.
 
-- __Use Security Libraries__: Employ security-focused libraries or frameworks that handle user inputs and command execution securely. These libraries often provide functions or methods that mitigate common vulnerabilities.
 
 ### Examples
 
 #### Java
 
 ```java
 Scanner scanner = new Scanner(System.in);
```

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/EXPRESSION_LANGUAGE_INJECTION/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/EXPRESSION_LANGUAGE_INJECTION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/EXPRESSION_LANGUAGE_INJECTION/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/EXPRESSION_LANGUAGE_INJECTION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/EXPRESSION_LANGUAGE_INJECTION/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/EXPRESSION_LANGUAGE_INJECTION/recommendation.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 To secure the application against Expression Language Injection (EL Injection), consider the following recommendations:
 
 - __Avoid Direct User Input Use__: Whenever possible, avoid directly using user inputs in EL expressions. Instead, prefer a whitelist approach where only predefined, safe values are allowed to be used in EL expressions.
 
-
 - __Input Validation__: Validate and sanitize user inputs before using them in EL expressions. Implement strict validation to accept only expected data types and patterns.
 
-
 - __Context-Specific Encoding__: Use encoding functions provided by your framework or libraries (e.g., \<c:out> in JSP, fn:escapeXml() in JSTL) to ensure context-aware output encoding. This prevents the interpretation of user inputs as code.
 
 ### Example
 
 === "Java"
   ```java
     @RestController
```

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/FILE_INCLUSION/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/FILE_INCLUSION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/FILE_INCLUSION/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/FILE_INCLUSION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/FILE_INCLUSION/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/FILE_INCLUSION/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/NOSQL_INJECTION/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/NOSQL_INJECTION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/NOSQL_INJECTION/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/NOSQL_INJECTION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/NOSQL_INJECTION/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/NOSQL_INJECTION/recommendation.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 To prevent NoSQL injection attacks, consider the following  measures:
 
-- __Input Validation and Sanitization__: Implement robust input validation to ensure that user-supplied data meets expected formats. Use sanitization techniques like whitelisting acceptable characters to prevent unwanted input.
-
-
 - __Safe Query Construction__: Construct queries using the database's specific methods or query builders provided by the API. Avoid directly concatenating user inputs into queries. Instead, use the appropriate mechanisms provided by the database API for safe query construction.
 
+- __Input Validation and Sanitization__: Implement robust input validation to ensure that user-supplied data meets expected formats. Use sanitization techniques like whitelisting acceptable characters to prevent unwanted input.
 
-- __Least Privilege Principle__: Limit the permissions granted to the application's database user. Ensure the user has only necessary privileges to reduce potential attack surface.
-
+- __Use whitelist of accepted keys__: To prevent operator injection, use a whitelist of accepted keys to prevent injection of query operators like `$where`, `$in`, `$ne`.
 
 ### Examples
 
 === "Java"
 
   ```java
     import com.mongodb.*;
```

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SERVER_SIDE_TEMPLATE_INJECTION/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SERVER_SIDE_TEMPLATE_INJECTION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SERVER_SIDE_TEMPLATE_INJECTION/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SERVER_SIDE_TEMPLATE_INJECTION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SERVER_SIDE_TEMPLATE_INJECTION/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SERVER_SIDE_TEMPLATE_INJECTION/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SSI_INJECTION/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SSI_INJECTION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SSI_INJECTION/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SSI_INJECTION/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_SQL_INJECTION/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_SQL_INJECTION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_SQL_INJECTION/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_SQL_INJECTION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_SQL_INJECTION/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_SQL_INJECTION/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_XPATH_INJECTION/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_XPATH_INJECTION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/XML_EXTERNAL_ENTITY_INJECTION/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/XML_EXTERNAL_ENTITY_INJECTION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/XML_EXTERNAL_ENTITY_INJECTION/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/XML_EXTERNAL_ENTITY_INJECTION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_COOKIE_MISSING_SECURITY_FLAGS/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_COOKIE_MISSING_SECURITY_FLAGS/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_COOKIE_MISSING_SECURITY_FLAGS/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_COOKIE_MISSING_SECURITY_FLAGS/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_CSP/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_CSP/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_CSP/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_CSP/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_CSP/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_CSP/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_CT/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_CT/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_HSTS/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_HSTS/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_HSTS/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_HSTS/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_HSTS/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_HSTS/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_RP/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_RP/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_XFO/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_HTTP_XFO/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/CRLF_INJECTION/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/CRLF_INJECTION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/CRLF_INJECTION/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/CRLF_INJECTION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/CRLF_INJECTION/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/CRLF_INJECTION/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/EXPOSED_FIREBASE_DB/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/EXPOSED_FIREBASE_DB/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/EXPOSED_FIREBASE_DB/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/EXPOSED_FIREBASE_DB/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/EXPOSED_FIREBASE_DB/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/EXPOSED_FIREBASE_DB/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/INSECURE_DIRECT_OBJECT_REFERENCE/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/INSECURE_DIRECT_OBJECT_REFERENCE/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/LDAP_INJECTION/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/LDAP_INJECTION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/LDAP_INJECTION/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/LDAP_INJECTION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/LDAP_INJECTION/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/LDAP_INJECTION/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/TLS_HEARTBLEED/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/TLS_HEARTBLEED/description.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,6 @@
-Heartbleed is a security bug in the OpenSSL cryptography library, a widely used implementation of Transport.
-Layer Security (TLS) protocol. It was introduced into the software in 2012 and publicly disclosed in April 2014.
+Heartbleed (CVE-2014-0160) is a security bug in the OpenSSL cryptography library, a widely used implementation of Transport Layer Security (TLS) protocol. It was introduced into the software in 2012 and publicly disclosed in April 2014.
 
 Heartbleed may be exploited regardless of whether the vulnerable OpenSSL instance runs as a TLS server or client.
 It results from improper input validation (due to a missing bounds check) in the implementation of the TLS heartbeat
 extension; thus, the bug's name derives from heartbeat. Additionally, the vulnerability is classified as a buffer
 over-read, where more data can be read than should be allowed.
```

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/TLS_SELFSIGNED/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/TLS_SELFSIGNED/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_INSECURE_OBJECT_SERIALIZATION/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_INSECURE_OBJECT_SERIALIZATION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_INSECURE_OBJECT_SERIALIZATION/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_INSECURE_OBJECT_SERIALIZATION/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_PATH_TRAVERSAL/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_PATH_TRAVERSAL/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_PATH_TRAVERSAL/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_PATH_TRAVERSAL/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_PATH_TRAVERSAL/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_PATH_TRAVERSAL/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_XML_INJECTION/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_XML_INJECTION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_XML_INJECTION/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_XML_INJECTION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_XML_INJECTION/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_XML_INJECTION/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/DJANGO_DEBUG_MODE/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/DJANGO_DEBUG_MODE/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/USER_ENUMERATION/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/USER_ENUMERATION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/USER_ENUMERATION/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/USER_ENUMERATION/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/CROSS_ORIGIN_RESOURCE_SHARING/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/CROSS_ORIGIN_RESOURCE_SHARING/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/CROSS_ORIGIN_RESOURCE_SHARING/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/CROSS_ORIGIN_RESOURCE_SHARING/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/INSECURE_TLS_VALIDATION/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/INSECURE_TLS_VALIDATION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/INSECURE_TLS_VALIDATION/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/INSECURE_TLS_VALIDATION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/INSECURE_TLS_VALIDATION/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/INSECURE_TLS_VALIDATION/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_DEPRECATED_PROTOCOL/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_DEPRECATED_PROTOCOL/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_DEPRECATED_PROTOCOL/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_DEPRECATED_PROTOCOL/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_HTTP/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_HTTP/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_HTTP/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_HTTP/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_HTTP/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_HTTP/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_INSECURE_CIPHER/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_INSECURE_CIPHER/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_INSECURE_CIPHER/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_HTTP_HOST_HEADER_POISONING/meta.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6626984126984128%*

 * *Differences: {"'categories'": "{'PCI_STANDARDS': {delete: [1, 0]}, delete: ['OWASP_ASVS_L2', 'OWASP_ASVS_L3']}",*

 * * "'privacy_issue'": 'False',*

 * * "'references'": "{replace: OrderedDict([('Testing for Host Header Injection (OWASP Web Security "*

 * *                 "Testing Guide)', "*

 * *                 "'https://owasp.org/www-project-web-security-testing-guide/latest/4-Web_Application_Security_Testing/07-Input_Validation_Testing/17-Testing_for_Host_Header_Injection')])}",*

 * * "'short_description'": "'Application trusts user-supplie […]*

```diff
@@ -1,28 +1,18 @@
 {
     "categories": {
-        "OWASP_ASVS_L2": [
-            "V6_2_3"
-        ],
-        "OWASP_ASVS_L3": [
-            "V6_2_3"
-        ],
         "PCI_STANDARDS": [
-            "REQ_2_2",
-            "REQ_4_2",
             "REQ_6_2",
             "REQ_6_3",
             "REQ_6_4",
             "REQ_11_3"
         ]
     },
-    "privacy_issue": true,
+    "privacy_issue": false,
     "references": {
-        "Mozilla Secure TLS/SSL Configuration": "https://wiki.mozilla.org/Security/Server_Side_TLS",
-        "SSL/TLS Deployment Best Practices (SSLabs)": "https://www.ssllabs.com/projects/best-practices/",
-        "Transport Layer Protection Cheat Sheet (OWASP)": "https://www.owasp.org/index.php/Transport_Layer_Protection_Cheat_Sheet"
+        "Testing for Host Header Injection (OWASP Web Security Testing Guide)": "https://owasp.org/www-project-web-security-testing-guide/latest/4-Web_Application_Security_Testing/07-Input_Validation_Testing/17-Testing_for_Host_Header_Injection"
     },
     "risk_rating": "medium",
     "security_issue": true,
-    "short_description": "The client supports combinations of cipher suites that suffer from known cryptographic weaknesses.",
-    "title": "Insecure TLS Ciphers supported"
+    "short_description": "Application trusts user-supplied host header, leading to host header poisoning.",
+    "title": "HTTP Host Header Poisoning"
 }
```

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_INSECURE_CIPHER/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_INSECURE_CIPHER/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_INVALIDHOSTNAME/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_INVALIDHOSTNAME/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_HTTP_HOST_HEADER_POISONING/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_HTTP_HOST_HEADER_POISONING/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_HTTP_HOST_HEADER_POISONING/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_HTTP_HOST_HEADER_POISONING/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_INSECURE_ACCESS_CONTROL/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_INSECURE_ACCESS_CONTROL/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_INSECURE_ACCESS_CONTROL/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_INSECURE_ACCESS_CONTROL/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_UNRESTRICTED_FILE_UPLOAD/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_UNRESTRICTED_FILE_UPLOAD/meta.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'risk_rating'": "'critical'"}*

```diff
@@ -11,12 +11,12 @@
             "REQ_11_3"
         ]
     },
     "privacy_issue": false,
     "references": {
         "Unrestricted File Upload (OWASP)": "https://owasp.org/www-community/vulnerabilities/Unrestricted_File_Upload"
     },
-    "risk_rating": "medium",
+    "risk_rating": "critical",
     "security_issue": true,
     "short_description": "The application doesn't restrict uploaded file based on file metadata or content.",
     "title": "Unrestricted file upload"
 }
```

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_XSS/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_XSS/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_XSS/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_XSS/meta.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'risk_rating'": "'high'"}*

```diff
@@ -28,12 +28,12 @@
     "privacy_issue": false,
     "references": {
         "CWE-116: Improper Encoding or Escaping of Output": "https://cwe.mitre.org/data/definitions/116.html",
         "CWE-159: Failure to Sanitize Special Element": "https://cwe.mitre.org/data/definitions/159.html",
         "CWE-79: Improper Neutralization of Input During Web Page Generation ('Cross-site Scripting')": "https://cwe.mitre.org/data/definitions/79.html",
         "CWE-80: Improper Neutralization of Script-Related HTML Tags in a Web Page (Basic XSS)": "https://cwe.mitre.org/data/definitions/80.html"
     },
-    "risk_rating": "medium",
+    "risk_rating": "high",
     "security_issue": true,
     "short_description": "The application is vulnerable to a Cross-Site Scripting vulnerability due to unsanitized input.",
     "title": "Cross-Site Scripting (XSS)"
 }
```

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_XSS/recommendation.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_XSS/recommendation.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_POTENTIALLY/SECRETS_NETWORK_REVIEW/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_POTENTIALLY/SECRETS_NETWORK_REVIEW/description.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 The application is detected to transmit secret credentials, like SSH keys, private certificates, or private API keys
 over
 the network.
 
-Secrets can be split into three categories with different risk profiles:
+Secrets can be split into two categories with different risk profiles:
 
 * Over-billing: affects API keys that grant access to services like Google Maps and are billed by a number of requests.
   Attackers will harvest the keys to access the service without paying while the target is paying for the service.
 
 * Unauthorized Access: affects keys, secrets, and tokens that grant access to services like S3 buckets. If
   the service is improperly configured, attackers can get access to unauthorized data or elevate their privileges
   through other services.
```

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_POTENTIALLY/SECRETS_NETWORK_REVIEW/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_POTENTIALLY/SECRETS_NETWORK_REVIEW/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/SECURE_AUTHENTICATION/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/SECURE_AUTHENTICATION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/SECURE_AUTHENTICATION/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/SECURE_AUTHENTICATION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/UNIQUE_USER_IDENTIFICATION/description.md` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/UNIQUE_USER_IDENTIFICATION/description.md`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/UNIQUE_USER_IDENTIFICATION/meta.json` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/UNIQUE_USER_IDENTIFICATION/meta.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/tests/kb_test.py` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/tests/kb_test.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/tests/tools/kb_generator_test.py` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/tests/tools/kb_generator_test.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/tests/utils.py` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/tests/utils.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/KB/tools/kb_generator.py` & `ostorlab-1.0.8/src/ostorlab/agent/kb/KB/tools/kb_generator.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/kb/kb.py` & `ostorlab-1.0.8/src/ostorlab/agent/kb/kb.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/message.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/message.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/common/x509/x509_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/common/x509/x509_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/agent/agent_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/agent/agent_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/domain_name/dns_record/dns_record_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/domain_name/dns_record/dns_record_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/domain_name/domain_name_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/domain_name/domain_name_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/domain_name/service/service_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/domain_name/service/service_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/domain_name/whois/whois_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/domain_name/whois/whois_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/file/android/aab/aab_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/file/android/aab/aab_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/file/android/apk/apk_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/file/android/apk/apk_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/file/file_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/file/file_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/file/ios/ipa/ipa_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/file/ios/ipa/ipa_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/file/sbom/sbom_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/file/sbom/sbom_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/file/source/source_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/file/source/source_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/ip/ip_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/ip/ip_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/ip/v4/geolocation/geolocation_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/ip/v4/geolocation/geolocation_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/port_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/port_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/service/http/http_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/service/http/http_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/service/service_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/ip/v4/port/service/service_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/ip/v4/v4_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/ip/v4/v4_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/ip/v4/whois/whois_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/ip/v4/whois/whois_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/ip/v6/geolocation/geolocation_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/ip/v6/geolocation/geolocation_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/port_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/port_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/service/http/http_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/service/http/http_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/service/service_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/ip/v6/port/service/service_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/ip/v6/v6_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/ip/v6/v6_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/ip/v6/whois/whois_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/ip/v6/whois/whois_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/link/link_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/link/link_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/store/android_store/android_store_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/store/android_store/android_store_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/store/android_store/developer/developer_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/store/android_store/developer/developer_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/store/ios_store/developer/developer_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/store/ios_store/developer/developer_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/asset/store/ios_store/ios_store_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/asset/store/ios_store/ios_store_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/capture/artifact/artifact_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/capture/artifact/artifact_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/capture/filesystem/filesystem_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/capture/filesystem/filesystem_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/capture/http/request/request_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/capture/http/request/request_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/capture/http/response/response_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/capture/http/response/response_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/capture/logs/logs_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/capture/logs/logs_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/capture/request_response/request_response_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/capture/request_response/request_response_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/capture/ui_call/ui_call_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/capture/ui_call/ui_call_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/control/control_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/control/control_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/library/library_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/library/library_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/x509/x509_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/domain_name/service/x509/x509_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/backend/backend_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/backend/backend_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/feature/feature_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/feature/feature_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/library/library_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/library/library_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/metadata/metadata_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/android/metadata/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/file/feature/feature_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/feature/feature_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/file/file_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/file_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/backend/backend_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/backend/backend_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/feature/feature_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/feature/feature_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/library/library_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/library/library_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/metadata/metadata_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/ios/metadata/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/file/library/library_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/file/library/library_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/library/library_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/library/library_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/x509/x509_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v4/service/x509/x509_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/library/library_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/library/library_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/x509/x509_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/fingerprint/ip/v6/service/x509/x509_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/healthcheck/ping/ping_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/healthcheck/ping/ping_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/report/cve/cve_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/report/cve/cve_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/report/event/post_scan/done/done_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/report/event/post_scan/done/done_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/report/event/post_scan/start/start_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/report/event/post_scan/start/start_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/report/event/post_scan/timeout/timeout_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/report/event/post_scan/timeout/timeout_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/report/event/scan/done/done_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/report/event/scan/done/done_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/report/event/scan/start/start_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/report/event/scan/start/start_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/report/event/scan/timeout/timeout_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/report/event/scan/timeout/timeout_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/report/status/status_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/report/status/status_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/report/vulnerability/vulnerability_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/report/vulnerability/vulnerability_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto/v3/use/device/device_pb2.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto/v3/use/device/device_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/proto_dict.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/proto_dict.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/message/serializer.py` & `ostorlab-1.0.8/src/ostorlab/agent/message/serializer.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/mixins/agent_healthcheck_mixin.py` & `ostorlab-1.0.8/src/ostorlab/agent/mixins/agent_healthcheck_mixin.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/mixins/agent_mq_mixin.py` & `ostorlab-1.0.8/src/ostorlab/agent/mixins/agent_mq_mixin.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/mixins/agent_open_telemetry_mixin.py` & `ostorlab-1.0.8/src/ostorlab/agent/mixins/agent_open_telemetry_mixin.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/mixins/agent_persist_mixin.py` & `ostorlab-1.0.8/src/ostorlab/agent/mixins/agent_persist_mixin.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/mixins/agent_report_vulnerability_mixin.py` & `ostorlab-1.0.8/src/ostorlab/agent/mixins/agent_report_vulnerability_mixin.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/mixins/protocols/emit.py` & `ostorlab-1.0.8/src/ostorlab/agent/mixins/protocols/emit.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/schema/agent_group_schema.json` & `ostorlab-1.0.8/src/ostorlab/agent/schema/agent_group_schema.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/schema/agent_schema.json` & `ostorlab-1.0.8/src/ostorlab/agent/schema/agent_schema.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/schema/loader.py` & `ostorlab-1.0.8/src/ostorlab/agent/schema/loader.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/schema/target_group_schema.json` & `ostorlab-1.0.8/src/ostorlab/agent/schema/target_group_schema.json`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/agent/schema/validator.py` & `ostorlab-1.0.8/src/ostorlab/agent/schema/validator.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/apis/add_scanner_state.py` & `ostorlab-1.0.8/src/ostorlab/apis/add_scanner_state.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/apis/agent_details.py` & `ostorlab-1.0.8/src/ostorlab/apis/agent_details.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/apis/agent_group.py` & `ostorlab-1.0.8/src/ostorlab/apis/agent_group.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/apis/agent_search.py` & `ostorlab-1.0.8/src/ostorlab/apis/agent_search.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/apis/assets.py` & `ostorlab-1.0.8/src/ostorlab/apis/assets.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/apis/create_agent_scan.py` & `ostorlab-1.0.8/src/ostorlab/apis/create_agent_scan.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/apis/create_api_key.py` & `ostorlab-1.0.8/src/ostorlab/apis/create_api_key.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/apis/login.py` & `ostorlab-1.0.8/src/ostorlab/apis/login.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/apis/request.py` & `ostorlab-1.0.8/src/ostorlab/apis/request.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/apis/revoke_api_key.py` & `ostorlab-1.0.8/src/ostorlab/apis/revoke_api_key.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/apis/runners/authenticated_runner.py` & `ostorlab-1.0.8/src/ostorlab/apis/runners/authenticated_runner.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/apis/runners/login_runner.py` & `ostorlab-1.0.8/src/ostorlab/apis/runners/login_runner.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/apis/runners/public_runner.py` & `ostorlab-1.0.8/src/ostorlab/apis/runners/public_runner.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/apis/runners/runner.py` & `ostorlab-1.0.8/src/ostorlab/apis/runners/runner.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/apis/scan_create.py` & `ostorlab-1.0.8/src/ostorlab/apis/scan_create.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/apis/scan_info.py` & `ostorlab-1.0.8/src/ostorlab/apis/scan_info.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/apis/scan_list.py` & `ostorlab-1.0.8/src/ostorlab/apis/scan_list.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/apis/scan_stop.py` & `ostorlab-1.0.8/src/ostorlab/apis/scan_stop.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/apis/scanner_config.py` & `ostorlab-1.0.8/src/ostorlab/apis/scanner_config.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/apis/test_credentials_create.py` & `ostorlab-1.0.8/src/ostorlab/apis/test_credentials_create.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/apis/vulnz_describe.py` & `ostorlab-1.0.8/src/ostorlab/apis/vulnz_describe.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/apis/vulnz_list.py` & `ostorlab-1.0.8/src/ostorlab/apis/vulnz_list.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/assets/agent.py` & `ostorlab-1.0.8/src/ostorlab/assets/agent.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/assets/android_aab.py` & `ostorlab-1.0.8/src/ostorlab/assets/android_aab.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/assets/android_apk.py` & `ostorlab-1.0.8/src/ostorlab/assets/android_apk.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/assets/asset.py` & `ostorlab-1.0.8/src/ostorlab/assets/asset.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/assets/file.py` & `ostorlab-1.0.8/src/ostorlab/assets/file.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/assets/ios_ipa.py` & `ostorlab-1.0.8/src/ostorlab/assets/ios_ipa.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/assets/ip.py` & `ostorlab-1.0.8/src/ostorlab/assets/ip.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/assets/ipv4.py` & `ostorlab-1.0.8/src/ostorlab/assets/ipv4.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/assets/ipv6.py` & `ostorlab-1.0.8/src/ostorlab/assets/ipv6.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/cli/agent/build/build.py` & `ostorlab-1.0.8/src/ostorlab/cli/agent/build/build.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/cli/agent/build/build_progress.py` & `ostorlab-1.0.8/src/ostorlab/cli/agent/build/build_progress.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/cli/agent/delete/delete.py` & `ostorlab-1.0.8/src/ostorlab/cli/agent/delete/delete.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/cli/agent/healthcheck/healthcheck.py` & `ostorlab-1.0.8/src/ostorlab/cli/agent/healthcheck/healthcheck.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/cli/agent/install/install.py` & `ostorlab-1.0.8/src/ostorlab/cli/agent/install/install.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/cli/agent/install/install_progress.py` & `ostorlab-1.0.8/src/ostorlab/cli/agent/install/install_progress.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/cli/agent/list/list.py` & `ostorlab-1.0.8/src/ostorlab/cli/agent/list/list.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/cli/agent/search/search.py` & `ostorlab-1.0.8/src/ostorlab/cli/agent/search/search.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/cli/agent_fetcher.py` & `ostorlab-1.0.8/src/ostorlab/cli/agent_fetcher.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/cli/auth/login/login.py` & `ostorlab-1.0.8/src/ostorlab/cli/auth/login/login.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/cli/auth/revoke/revoke.py` & `ostorlab-1.0.8/src/ostorlab/cli/auth/revoke/revoke.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/cli/ci_scan/run/assets/android_aab.py` & `ostorlab-1.0.8/src/ostorlab/cli/ci_scan/run/assets/android_aab.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/cli/ci_scan/run/assets/android_apk.py` & `ostorlab-1.0.8/src/ostorlab/cli/ci_scan/run/assets/android_apk.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/cli/ci_scan/run/assets/ios_ipa.py` & `ostorlab-1.0.8/src/ostorlab/cli/ci_scan/run/assets/ios_ipa.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/cli/ci_scan/run/assets/mobile.py` & `ostorlab-1.0.8/src/ostorlab/cli/ci_scan/run/assets/mobile.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/cli/ci_scan/run/ci_logger/circleci_logger.py` & `ostorlab-1.0.8/src/ostorlab/cli/ci_scan/run/ci_logger/circleci_logger.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/cli/ci_scan/run/ci_logger/console_logger.py` & `ostorlab-1.0.8/src/ostorlab/cli/ci_scan/run/ci_logger/console_logger.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/cli/ci_scan/run/ci_logger/github_logger.py` & `ostorlab-1.0.8/src/ostorlab/cli/ci_scan/run/ci_logger/github_logger.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/cli/ci_scan/run/ci_logger/logger.py` & `ostorlab-1.0.8/src/ostorlab/cli/ci_scan/run/ci_logger/logger.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/cli/ci_scan/run/run.py` & `ostorlab-1.0.8/src/ostorlab/cli/ci_scan/run/run.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/cli/console.py` & `ostorlab-1.0.8/src/ostorlab/cli/console.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/cli/docker_requirements_checker.py` & `ostorlab-1.0.8/src/ostorlab/cli/docker_requirements_checker.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/cli/dumpers.py` & `ostorlab-1.0.8/src/ostorlab/cli/dumpers.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/cli/input_validators.py` & `ostorlab-1.0.8/src/ostorlab/cli/input_validators.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/cli/install_agent.py` & `ostorlab-1.0.8/src/ostorlab/cli/install_agent.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/cli/rootcli.py` & `ostorlab-1.0.8/src/ostorlab/cli/rootcli.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/cli/scan/list/list.py` & `ostorlab-1.0.8/src/ostorlab/cli/scan/list/list.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/cli/scan/run/assets/__init__.py` & `ostorlab-1.0.8/src/ostorlab/cli/scan/run/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/cli/scan/run/assets/agent.py` & `ostorlab-1.0.8/src/ostorlab/cli/scan/run/assets/agent.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/cli/scan/run/assets/android_aab.py` & `ostorlab-1.0.8/src/ostorlab/cli/scan/run/assets/android_aab.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/cli/scan/run/assets/android_apk.py` & `ostorlab-1.0.8/src/ostorlab/cli/scan/run/assets/android_apk.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/cli/scan/run/assets/android_store.py` & `ostorlab-1.0.8/src/ostorlab/cli/scan/run/assets/android_store.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/cli/scan/run/assets/domain_name.py` & `ostorlab-1.0.8/src/ostorlab/cli/scan/run/assets/domain_name.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/cli/scan/run/assets/file.py` & `ostorlab-1.0.8/src/ostorlab/cli/scan/run/assets/file.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/cli/scan/run/assets/ios_ipa.py` & `ostorlab-1.0.8/src/ostorlab/cli/scan/run/assets/ios_ipa.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/cli/scan/run/assets/ios_store.py` & `ostorlab-1.0.8/src/ostorlab/cli/scan/run/assets/ios_store.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/cli/scan/run/assets/ip.py` & `ostorlab-1.0.8/src/ostorlab/cli/scan/run/assets/ip.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/cli/scan/run/assets/link.py` & `ostorlab-1.0.8/src/ostorlab/cli/scan/run/assets/link.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/cli/scan/run/run.py` & `ostorlab-1.0.8/src/ostorlab/cli/scan/run/run.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/cli/scan/scan.py` & `ostorlab-1.0.8/src/ostorlab/cli/scan/scan.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/cli/scan/stop/stop.py` & `ostorlab-1.0.8/src/ostorlab/cli/scan/stop/stop.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/cli/scanner/scanner.py` & `ostorlab-1.0.8/src/ostorlab/cli/scanner/scanner.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/cli/types.py` & `ostorlab-1.0.8/src/ostorlab/cli/types.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/cli/vulnz/describe/describe.py` & `ostorlab-1.0.8/src/ostorlab/cli/vulnz/describe/describe.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/cli/vulnz/dump/dump.py` & `ostorlab-1.0.8/src/ostorlab/cli/vulnz/dump/dump.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/cli/vulnz/list/list.py` & `ostorlab-1.0.8/src/ostorlab/cli/vulnz/list/list.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/cli/vulnz/vulnz.py` & `ostorlab-1.0.8/src/ostorlab/cli/vulnz/vulnz.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/configuration_manager.py` & `ostorlab-1.0.8/src/ostorlab/configuration_manager.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/runtimes/cloud/runtime.py` & `ostorlab-1.0.8/src/ostorlab/runtimes/cloud/runtime.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/runtimes/definitions.py` & `ostorlab-1.0.8/src/ostorlab/runtimes/definitions.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/runtimes/lite_local/agent_runtime.py` & `ostorlab-1.0.8/src/ostorlab/runtimes/lite_local/agent_runtime.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/runtimes/lite_local/runtime.py` & `ostorlab-1.0.8/src/ostorlab/runtimes/lite_local/runtime.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/runtimes/local/agent_runtime.py` & `ostorlab-1.0.8/src/ostorlab/runtimes/local/agent_runtime.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/runtimes/local/log_streamer.py` & `ostorlab-1.0.8/src/ostorlab/runtimes/local/log_streamer.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/runtimes/local/models/alembic/env.py` & `ostorlab-1.0.8/src/ostorlab/runtimes/local/models/alembic/env.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/runtimes/local/models/alembic/versions/35cd577ef0e5_.py` & `ostorlab-1.0.8/src/ostorlab/runtimes/local/models/alembic/versions/35cd577ef0e5_.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/runtimes/local/models/alembic.ini` & `ostorlab-1.0.8/src/ostorlab/runtimes/local/models/alembic.ini`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/runtimes/local/models/models.py` & `ostorlab-1.0.8/src/ostorlab/runtimes/local/models/models.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/runtimes/local/runtime.py` & `ostorlab-1.0.8/src/ostorlab/runtimes/local/runtime.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/runtimes/local/services/jaeger.py` & `ostorlab-1.0.8/src/ostorlab/runtimes/local/services/jaeger.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/runtimes/local/services/mq.py` & `ostorlab-1.0.8/src/ostorlab/runtimes/local/services/mq.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/runtimes/local/services/redis.py` & `ostorlab-1.0.8/src/ostorlab/runtimes/local/services/redis.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/runtimes/proto/agent_instance_settings_pb2.py` & `ostorlab-1.0.8/src/ostorlab/runtimes/proto/agent_instance_settings_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/runtimes/registry.py` & `ostorlab-1.0.8/src/ostorlab/runtimes/registry.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/runtimes/runtime.py` & `ostorlab-1.0.8/src/ostorlab/runtimes/runtime.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/scanner/callbacks.py` & `ostorlab-1.0.8/src/ostorlab/scanner/callbacks.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/scanner/handler.py` & `ostorlab-1.0.8/src/ostorlab/scanner/handler.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/scanner/proto/assets/aab_pb2.py` & `ostorlab-1.0.8/src/ostorlab/scanner/proto/assets/aab_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/scanner/proto/assets/agent_pb2.py` & `ostorlab-1.0.8/src/ostorlab/scanner/proto/assets/agent_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/scanner/proto/assets/android_store_pb2.py` & `ostorlab-1.0.8/src/ostorlab/scanner/proto/assets/android_store_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/scanner/proto/assets/apk_pb2.py` & `ostorlab-1.0.8/src/ostorlab/scanner/proto/assets/apk_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/scanner/proto/assets/domain_name_pb2.py` & `ostorlab-1.0.8/src/ostorlab/scanner/proto/assets/domain_name_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/scanner/proto/assets/file_pb2.py` & `ostorlab-1.0.8/src/ostorlab/scanner/proto/assets/file_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/scanner/proto/assets/ios_store_pb2.py` & `ostorlab-1.0.8/src/ostorlab/scanner/proto/assets/ios_store_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/scanner/proto/assets/ip_pb2.py` & `ostorlab-1.0.8/src/ostorlab/scanner/proto/assets/ip_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/scanner/proto/assets/ipa_pb2.py` & `ostorlab-1.0.8/src/ostorlab/scanner/proto/assets/ipa_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/scanner/proto/assets/link_pb2.py` & `ostorlab-1.0.8/src/ostorlab/scanner/proto/assets/link_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/scanner/proto/assets/network_pb2.py` & `ostorlab-1.0.8/src/ostorlab/scanner/proto/assets/network_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/scanner/proto/assets/source_pb2.py` & `ostorlab-1.0.8/src/ostorlab/scanner/proto/assets/source_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/scanner/proto/assets/v4_pb2.py` & `ostorlab-1.0.8/src/ostorlab/scanner/proto/assets/v4_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/scanner/proto/assets/v6_pb2.py` & `ostorlab-1.0.8/src/ostorlab/scanner/proto/assets/v6_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/scanner/proto/scan/_location/startAgentScan_pb2.py` & `ostorlab-1.0.8/src/ostorlab/scanner/proto/scan/_location/startAgentScan_pb2.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/scanner/scan_handler.py` & `ostorlab-1.0.8/src/ostorlab/scanner/scan_handler.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/scanner/scanner_conf.py` & `ostorlab-1.0.8/src/ostorlab/scanner/scanner_conf.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/testing/agent.py` & `ostorlab-1.0.8/src/ostorlab/testing/agent.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/utils/defintions.py` & `ostorlab-1.0.8/src/ostorlab/utils/defintions.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/utils/dictionary_minifier.py` & `ostorlab-1.0.8/src/ostorlab/utils/dictionary_minifier.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/utils/risk_rating.py` & `ostorlab-1.0.8/src/ostorlab/utils/risk_rating.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/utils/scanner_state_reporter.py` & `ostorlab-1.0.8/src/ostorlab/utils/scanner_state_reporter.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/utils/strings.py` & `ostorlab-1.0.8/src/ostorlab/utils/strings.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/utils/styles.py` & `ostorlab-1.0.8/src/ostorlab/utils/styles.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/utils/system.py` & `ostorlab-1.0.8/src/ostorlab/utils/system.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/utils/version.py` & `ostorlab-1.0.8/src/ostorlab/utils/version.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab/utils/volumes.py` & `ostorlab-1.0.8/src/ostorlab/utils/volumes.py`

 * *Files identical despite different names*

### Comparing `ostorlab-1.0.7/src/ostorlab.egg-info/SOURCES.txt` & `ostorlab-1.0.8/src/ostorlab.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -272,20 +272,14 @@
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/INTENT_REDIRECTION/recommendation.md
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/PATH_TRAVERSAL/description.md
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/PATH_TRAVERSAL/meta.json
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/PATH_TRAVERSAL/recommendation.md
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/REDIS_LIBRARY/description.md
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/REDIS_LIBRARY/meta.json
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/REDIS_LIBRARY/recommendation.md
-src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/STACK_TRACE_INFORMATION_DISCLOSURE/description.md
-src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/STACK_TRACE_INFORMATION_DISCLOSURE/meta.json
-src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/STACK_TRACE_INFORMATION_DISCLOSURE/recommendation.md
-src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/UNTRUSTED_EXTERNAL_STORAGE_ACCESS/description.md
-src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/UNTRUSTED_EXTERNAL_STORAGE_ACCESS/meta.json
-src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/UNTRUSTED_EXTERNAL_STORAGE_ACCESS/recommendation.md
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/WEBVIEW_LOADURL_INJECTION/context.md
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/WEBVIEW_LOADURL_INJECTION/description.md
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/WEBVIEW_LOADURL_INJECTION/meta.json
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_MEDIUM/WEBVIEW_LOADURL_INJECTION/recommendation.md
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/APK_BACKUP_TITLE/description.md
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/APK_BACKUP_TITLE/meta.json
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/ANDROID/_POTENTIALLY/APK_BACKUP_TITLE/recommendation.md
@@ -316,18 +310,14 @@
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/DEPENDENCY_CONFUSION/context.md
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/DEPENDENCY_CONFUSION/description.md
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/DEPENDENCY_CONFUSION/meta.json
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/DEPENDENCY_CONFUSION/recommendation.md
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/FORMAT_STRING/description.md
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/FORMAT_STRING/meta.json
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_CRITICAL/FORMAT_STRING/recommendation.md
-src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/CORS_MISCONFIGURATION/context.md
-src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/CORS_MISCONFIGURATION/description.md
-src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/CORS_MISCONFIGURATION/meta.json
-src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/CORS_MISCONFIGURATION/recommendation.md
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/DEPRECATED_COMPONENT/description.md
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/DEPRECATED_COMPONENT/meta.json
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/DEPRECATED_COMPONENT/recommendation.md
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_HOSTNAME_VALIDATION/description.md
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_HOSTNAME_VALIDATION/meta.json
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_HOSTNAME_VALIDATION/recommendation.md
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_JWT_SIGNATURE/description.md
@@ -338,17 +328,14 @@
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_REPUTATION/recommendation.md
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_STORAGE/description.md
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_STORAGE/meta.json
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_STORAGE/recommendation.md
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_VIRUSTOTAL_SCAN/description.md
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_VIRUSTOTAL_SCAN/meta.json
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/INSECURE_VIRUSTOTAL_SCAN/recommendation.md
-src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/LEAKING_HEALTH_INFORMATION/description.md
-src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/LEAKING_HEALTH_INFORMATION/meta.json
-src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/LEAKING_HEALTH_INFORMATION/recommendation.md
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/LEAKING_PERSONAL_INFORMATION/description.md
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/LEAKING_PERSONAL_INFORMATION/meta.json
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/LEAKING_PERSONAL_INFORMATION/recommendation.md
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/OAUTH_SCHEME_ACCOUNT_TAKEOVER/context.md
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/OAUTH_SCHEME_ACCOUNT_TAKEOVER/description.md
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/OAUTH_SCHEME_ACCOUNT_TAKEOVER/meta.json
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_HIGH/OAUTH_SCHEME_ACCOUNT_TAKEOVER/recommendation.md
@@ -400,17 +387,14 @@
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/HTML_INJECTION/recommendation.md
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_DYNAMICALLY_LINKED_LIBRARY/description.md
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_DYNAMICALLY_LINKED_LIBRARY/meta.json
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_DYNAMICALLY_LINKED_LIBRARY/recommendation.md
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_PASSWORD_STORAGE/description.md
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_PASSWORD_STORAGE/meta.json
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_PASSWORD_STORAGE/recommendation.md
-src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_PERMISSION_FILESYSTEM/description.md
-src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_PERMISSION_FILESYSTEM/meta.json
-src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_PERMISSION_FILESYSTEM/recommendation.md
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_RANDOM_SEED/description.md
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_RANDOM_SEED/meta.json
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/INSECURE_RANDOM_SEED/recommendation.md
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/LEAKING_CREDENTIALS_LOGS/description.md
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/LEAKING_CREDENTIALS_LOGS/meta.json
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/LEAKING_CREDENTIALS_LOGS/recommendation.md
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/COMMON/_MEDIUM/LEAKING_CREDENTIALS_REQUEST/description.md
@@ -454,14 +438,17 @@
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HARDENING/IPA_STACK_SMASHING_DISABLED/recommendation.md
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_INSECURE_PRIVACY_MANIFEST_FILE/description.md
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_INSECURE_PRIVACY_MANIFEST_FILE/meta.json
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_INSECURE_PRIVACY_MANIFEST_FILE/recommendation.md
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_URL_SCHEME_INJECTION/description.md
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_URL_SCHEME_INJECTION/meta.json
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/IPA_URL_SCHEME_INJECTION/recommendation.md
+src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/UNSAFE_KEYCHAIN_ACCESSIBILITY/description.md
+src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/UNSAFE_KEYCHAIN_ACCESSIBILITY/meta.json
+src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_HIGH/UNSAFE_KEYCHAIN_ACCESSIBILITY/recommendation.md
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_IMPORTANT/IPA_BITCODE/description.md
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_IMPORTANT/IPA_BITCODE/meta.json
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_IMPORTANT/IPA_BITCODE/recommendation.md
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_IMPORTANT/IPA_ENCRYPTED/description.md
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_IMPORTANT/IPA_ENCRYPTED/meta.json
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_IMPORTANT/IPA_ENCRYPTED/recommendation.md
 src/ostorlab/agent/kb/KB/MOBILE_CLIENT/IOS/_INFO/IPA_ENTITLEMENTS/description.md
@@ -565,14 +552,17 @@
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SERVER_SIDE_TEMPLATE_INJECTION/recommendation.md
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SSI_INJECTION/description.md
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SSI_INJECTION/meta.json
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/SSI_INJECTION/recommendation.md
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_SQL_INJECTION/description.md
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_SQL_INJECTION/meta.json
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_SQL_INJECTION/recommendation.md
+src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_UNRESTRICTED_FILE_UPLOAD/description.md
+src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_UNRESTRICTED_FILE_UPLOAD/meta.json
+src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_UNRESTRICTED_FILE_UPLOAD/recommendation.md
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_XPATH_INJECTION/description.md
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_XPATH_INJECTION/meta.json
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/WEB_XPATH_INJECTION/recommendation.md
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/XML_EXTERNAL_ENTITY_INJECTION/description.md
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/XML_EXTERNAL_ENTITY_INJECTION/meta.json
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_CRITICAL/XML_EXTERNAL_ENTITY_INJECTION/recommendation.md
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HARDENING/WEB_COOKIE_MISSING_SECURITY_FLAGS/description.md
@@ -622,32 +612,39 @@
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_INSECURE_OBJECT_SERIALIZATION/recommendation.md
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_PATH_TRAVERSAL/description.md
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_PATH_TRAVERSAL/meta.json
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_PATH_TRAVERSAL/recommendation.md
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_XML_INJECTION/description.md
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_XML_INJECTION/meta.json
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_XML_INJECTION/recommendation.md
+src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_XSS/description.md
+src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_XSS/meta.json
+src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_HIGH/WEB_XSS/recommendation.md
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_INFO/TLS_SERVER_SCAN/description.md
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_INFO/TLS_SERVER_SCAN/meta.json
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_INFO/TLS_SERVER_SCAN/recommendation.md
+src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_INFO/WEB_GENERIC/description.md
+src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_INFO/WEB_GENERIC/meta.json
+src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_INFO/WEB_GENERIC/recommendation.md
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_INFO/WEB_INTERESTING_RESPONSE/description.md
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_INFO/WEB_INTERESTING_RESPONSE/meta.json
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_INFO/WEB_INTERESTING_RESPONSE/recommendation.md
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/DJANGO_DEBUG_MODE/description.md
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/DJANGO_DEBUG_MODE/meta.json
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/DJANGO_DEBUG_MODE/recommendation.md
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/USER_ENUMERATION/description.md
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/USER_ENUMERATION/meta.json
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/USER_ENUMERATION/recommendation.md
-src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/WEB_GENERIC/description.md
-src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/WEB_GENERIC/meta.json
-src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/WEB_GENERIC/recommendation.md
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/WEB_HTTP_HEADER/description.md
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/WEB_HTTP_HEADER/meta.json
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_LOW/WEB_HTTP_HEADER/recommendation.md
+src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/CORS_MISCONFIGURATION/context.md
+src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/CORS_MISCONFIGURATION/description.md
+src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/CORS_MISCONFIGURATION/meta.json
+src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/CORS_MISCONFIGURATION/recommendation.md
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/CROSS_ORIGIN_RESOURCE_SHARING/description.md
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/CROSS_ORIGIN_RESOURCE_SHARING/meta.json
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/CROSS_ORIGIN_RESOURCE_SHARING/recommendation.md
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/INSECURE_TLS_VALIDATION/description.md
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/INSECURE_TLS_VALIDATION/meta.json
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/INSECURE_TLS_VALIDATION/recommendation.md
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_ANONSERVER/description.md
@@ -664,26 +661,17 @@
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_INSECURE_CIPHER/recommendation.md
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_INVALIDHOSTNAME/description.md
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_INVALIDHOSTNAME/meta.json
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/TLS_INVALIDHOSTNAME/recommendation.md
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_HTTP_HOST_HEADER_POISONING/description.md
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_HTTP_HOST_HEADER_POISONING/meta.json
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_HTTP_HOST_HEADER_POISONING/recommendation.md
-src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_IDOR/description.md
-src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_IDOR/meta.json
-src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_IDOR/recommendation.md
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_INSECURE_ACCESS_CONTROL/description.md
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_INSECURE_ACCESS_CONTROL/meta.json
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_INSECURE_ACCESS_CONTROL/recommendation.md
-src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_UNRESTRICTED_FILE_UPLOAD/description.md
-src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_UNRESTRICTED_FILE_UPLOAD/meta.json
-src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_UNRESTRICTED_FILE_UPLOAD/recommendation.md
-src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_XSS/description.md
-src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_XSS/meta.json
-src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_MEDIUM/WEB_XSS/recommendation.md
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_POTENTIALLY/SECRETS_NETWORK_REVIEW/description.md
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_POTENTIALLY/SECRETS_NETWORK_REVIEW/meta.json
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_POTENTIALLY/SECRETS_NETWORK_REVIEW/recommendation.md
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/SECURE_AUTHENTICATION/description.md
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/SECURE_AUTHENTICATION/meta.json
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/SECURE_AUTHENTICATION/recommendation.md
 src/ostorlab/agent/kb/KB/WEB_SERVICE/WEB/_SECURE/TLS_INVALIDHOSTNAME_SECURE/description.md
```

### Comparing `ostorlab-1.0.7/src/ostorlab.egg-info/requires.txt` & `ostorlab-1.0.8/src/ostorlab.egg-info/requires.txt`

 * *Files identical despite different names*

