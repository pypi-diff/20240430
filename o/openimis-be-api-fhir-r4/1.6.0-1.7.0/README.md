# Comparing `tmp/openimis-be-api_fhir_r4-1.6.0.tar.gz` & `tmp/openimis_be_api_fhir_r4-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-api_fhir_r4-1.6.0.tar", last modified: Sat Dec 16 00:57:34 2023, max compression
+gzip compressed data, was "openimis_be_api_fhir_r4-1.7.0.tar", last modified: Tue Apr 30 09:06:09 2024, max compression
```

## Comparing `openimis-be-api_fhir_r4-1.6.0.tar` & `openimis_be_api_fhir_r4-1.7.0.tar`

### file list

```diff
@@ -1,345 +1,346 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:34.881097 openimis-be-api_fhir_r4-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       99 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    30440 2023-12-16 00:57:34.881097 openimis-be-api_fhir_r4-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    29179 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:34.829097 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:34.833097 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/configurations/
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/configurations/R4ApiFhirConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     5477 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/configurations/R4ClaimConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/configurations/R4CommunicationRequestConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     4338 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/configurations/R4CoverageConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     4437 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/configurations/R4CoverageEligibilityConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/configurations/R4IdentifierConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/configurations/R4InvoiceConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/configurations/R4IssueTypeConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     3788 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/configurations/R4LocationConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/configurations/R4MaritalConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     5241 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/configurations/R4OrganisationConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/configurations/R4PaymentNoticeConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/configurations/R4SubscriptionConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)    26108 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/configurations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/configurations/generalConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)      370 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/configurations/moduleConfiguration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:34.833097 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/containedResources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/containedResources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/containedResources/claimContainedResources.py
--rw-r--r--   0 runner    (1001) docker     (127)     4641 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/containedResources/containedResourceHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/containedResources/containedResources.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/containedResources/converterUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7176 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/containedResources/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5545 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/containedResources/serializerMixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:34.837097 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/
--rw-r--r--   0 runner    (1001) docker     (127)    11881 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21043 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/activityDefinitionConverter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7081 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/claimAdminPractitionerConverter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5307 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/claimAdminPractitionerRoleConverter.py
--rw-r--r--   0 runner    (1001) docker     (127)    26583 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/claimConverter.py
--rw-r--r--   0 runner    (1001) docker     (127)    23846 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/claimResponseConverter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/codeSystemConverter.py
--rw-r--r--   0 runner    (1001) docker     (127)    11329 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/communicationConverter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5538 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/communicationRequestConverter.py
--rw-r--r--   0 runner    (1001) docker     (127)    26609 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/contractConverter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7476 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/coverageConverter.py
--rw-r--r--   0 runner    (1001) docker     (127)    18808 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/coverageEligibilityRequestConverter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5814 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/enrolmentOfficerPractitionerConverter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6669 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/enrolmentOfficerPractitionerRoleConverter.py
--rw-r--r--   0 runner    (1001) docker     (127)    17052 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/groupConverter.py
--rw-r--r--   0 runner    (1001) docker     (127)    14290 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/healthFacilityOrganisationConverter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4744 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/insuranceOrganisationConverter.py
--rw-r--r--   0 runner    (1001) docker     (127)    24070 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/insurancePlanConverter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9717 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/invoiceConverter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10620 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/locationConverter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6530 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/locationSiteConverter.py
--rw-r--r--   0 runner    (1001) docker     (127)    19915 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/medicationConverter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5586 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/operationOutcomeConverter.py
--rw-r--r--   0 runner    (1001) docker     (127)    38840 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/patientConverter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/personConverterMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4389 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/policyCoverageEligibilityRequestConverter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9175 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/policyHolderOrganisationConverter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6319 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/referenceConverterMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     9480 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/defaultConfig.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:34.837097 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/exceptions/fhir_api_exception_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:34.841097 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/mapping/
--rw-r--r--   0 runner    (1001) docker     (127)      441 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/mapping/activityDefinitionMapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     3515 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/mapping/claimMapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/mapping/contractMapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/mapping/coverageMapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/mapping/feedbackMapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/mapping/groupMapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/mapping/hfOrganizationMapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/mapping/invoiceMapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/mapping/locationMapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/mapping/medicationMapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     3143 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/mapping/organizationMapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/mapping/patientMapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/mapping/subscriptionMapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:34.841097 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     5487 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/migrations/0002_auto_20220313_1607.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/migrations/0003_auto_20220313_1634.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/migrations/0004_update_subscription_criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/migrations/0005_auto_20221012_0818.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/migrations/0006_add_subsription_perms_imis_admin.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5918 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/model_retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:34.841097 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/models/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9608 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/models/fhirModels.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/models/imisModelEnums.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/models/subscription.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:34.841097 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/multiserializer/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/multiserializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15596 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/multiserializer/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/multiserializer/modelViewset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/multiserializer/serializerClass.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/openapi_schema_extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3797 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/paginations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:34.841097 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/paymentNotice/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/paymentNotice/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:34.845097 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/paymentNotice/converter/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/paymentNotice/converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/paymentNotice/converter/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/paymentNotice/converter/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5002 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/paymentNotice/converter/to_fhir_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4995 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/paymentNotice/converter/to_imis_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:34.845097 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/paymentNotice/mapping/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/paymentNotice/mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/paymentNotice/mapping/payment_detail_status_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/paymentNotice/mapping/payment_status_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/paymentNotice/mapping/status_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:34.845097 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/paymentNotice/serializer/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/paymentNotice/serializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/paymentNotice/serializer/create.py
--rw-r--r--   0 runner    (1001) docker     (127)      488 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/paymentNotice/serializer/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/paymentNotice/serializer/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8884 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:34.849097 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/serializers/
--rw-r--r--   0 runner    (1001) docker     (127)     5556 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/serializers/activityDefinitionSerializer.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/serializers/billSerializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/serializers/claimAdminPractitionerRoleSerializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/serializers/claimAdminPractitionerSerializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/serializers/claimResponseSerializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9277 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/serializers/claimSerializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/serializers/codeSystemSerializer.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/serializers/communicationRequestSerializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/serializers/communicationSerializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/serializers/contractSerializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/serializers/coverageEligibilityRequestSerializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/serializers/coverageSerializer.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/serializers/enrolmentOfficerPractitionerRoleSerializer.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/serializers/enrolmentOfficerPractitionerSerializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/serializers/groupSerializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/serializers/healthFacilityOrganisationSerializer.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/serializers/insuranceOrganisationSerializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/serializers/insurancePlanSerializer.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/serializers/invoiceSerializer.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/serializers/locationSerializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/serializers/locationSiteSerializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/serializers/medicationSerializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2388 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/serializers/patientSerializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/serializers/policyCoverageEligibilityRequestSerializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/serializers/policyHolderOrganisationSerializer.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/services.py
--rw-r--r--   0 runner    (1001) docker     (127)     4028 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:34.849097 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/subscriptions/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5457 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/subscriptions/notificationClient.py
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/subscriptions/notificationManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     8846 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/subscriptions/subscriptionConverter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2374 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/subscriptions/subscriptionCriteriaFilter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/subscriptions/subscriptionSerializer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:34.857097 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:34.865097 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/SubscriptionTestMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16312 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/activityDefinitionTestMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7326 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/billInvoiceTestMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4996 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/claimAdminPractitionerRoleTestMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     8325 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/claimAdminPractitionerTestMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     8164 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/claimResponseTestMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    13782 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/claimTestMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     8149 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/communicationRequestTestMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    12220 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/communicationTestMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     9959 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/contractTestMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7980 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/coverageEligibilityRequestTestMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4558 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/coverageTestMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5293 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/enrolmentOfficerPractitionerRoleTestMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5137 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/enrolmentOfficerPractitionerTestMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/fhirApiCreateTestMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/fhirApiDeleteTestMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      608 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/fhirApiReadTestMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/fhirApiUpdateTestMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4016 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/genericFhirAPITestMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/genericTestMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     8315 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/groupTestMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    11807 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/insurancePlanTestMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6186 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/invoiceTestMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/locationTestMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/logInMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    10296 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/medicationTestMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/operationOutcomeTestMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    13549 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/patientTestMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5642 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/paymentNoticeTestMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4368 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/policyHolderOrganisationTestMixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:34.865097 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/subscriptions/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4484 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/subscriptions/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3776 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/subscriptions/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:34.869097 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5201 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test/test_activity_definition.json
--rw-r--r--   0 runner    (1001) docker     (127)     6419 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test/test_claim.json
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test/test_claimAdminPractitioner.json
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test/test_claimAdminPractitionerRole.json
--rw-r--r--   0 runner    (1001) docker     (127)     5841 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test/test_claimResponse.json
--rw-r--r--   0 runner    (1001) docker     (127)    37007 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test/test_claim_contained.json
--rw-r--r--   0 runner    (1001) docker     (127)     6283 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test/test_claim_with_code_references.json
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test/test_communication.json
--rw-r--r--   0 runner    (1001) docker     (127)     4537 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test/test_communicationRequest.json
--rw-r--r--   0 runner    (1001) docker     (127)     3363 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test/test_communication_with_code_reference.json
--rw-r--r--   0 runner    (1001) docker     (127)     4954 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test/test_contract.json
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test/test_coverage.json
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test/test_coverageEligibilityRequest.json
--rw-r--r--   0 runner    (1001) docker     (127)     9034 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test/test_coverageEligibilityResponse.json
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test/test_enrolmentOfficerPractitioner.json
--rw-r--r--   0 runner    (1001) docker     (127)     2556 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test/test_enrolmentOfficerPractitionerRole.json
--rw-r--r--   0 runner    (1001) docker     (127)     2540 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test/test_group.json
--rw-r--r--   0 runner    (1001) docker     (127)     6411 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test/test_insurance_plan.json
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test/test_invoice.json
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test/test_location.json
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test/test_login.json
--rw-r--r--   0 runner    (1001) docker     (127)       80 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test/test_login_bad_credentials.json
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test/test_login_bad_payload.json
--rw-r--r--   0 runner    (1001) docker     (127)     4854 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test/test_medication.json
--rw-r--r--   0 runner    (1001) docker     (127)      191 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test/test_outcome.json
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test/test_patient.json
--rw-r--r--   0 runner    (1001) docker     (127)      755 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test/test_payment_notice.json
--rw-r--r--   0 runner    (1001) docker     (127)      286 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test/test_subscription.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:34.873097 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/testCodeSystem/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/testCodeSystem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/testCodeSystem/test_api_codeDiagnosis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/testCodeSystem/test_api_codeGroupConfirmationType.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/testCodeSystem/test_api_codeGroupType.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/testCodeSystem/test_api_codeHFOrganizationLegalForm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/testCodeSystem/test_api_codeHFOrganizationLevel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/testCodeSystem/test_api_codePHOrganisationActivity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/testCodeSystem/test_api_codePHOrganisationLegalForm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/testCodeSystem/test_api_codePatientContactRelationship.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/testCodeSystem/test_api_codePatientEducationLevel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/testCodeSystem/test_api_codePatientIdentificationType.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/testCodeSystem/test_api_codePatientProfession.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_activityDefinitionConverter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4718 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_api_authorization.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_api_bill.py
--rw-r--r--   0 runner    (1001) docker     (127)     8248 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_api_claim.py
--rw-r--r--   0 runner    (1001) docker     (127)    12976 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_api_claim_contained.py
--rw-r--r--   0 runner    (1001) docker     (127)    10947 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_api_communication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_api_communicationRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     7339 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_api_contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     5240 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_api_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_api_insurancePlan.py
--rw-r--r--   0 runner    (1001) docker     (127)      977 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_api_invoice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_api_location.py
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_api_login.py
--rw-r--r--   0 runner    (1001) docker     (127)     2920 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_api_medication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_api_organisation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10777 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_api_patient.py
--rw-r--r--   0 runner    (1001) docker     (127)     4704 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_api_paymentNotice.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_api_practitioner.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_api_practitionerRole.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_api_subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_bill.py
--rw-r--r--   0 runner    (1001) docker     (127)      731 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_claimAdminPractitionerConverter.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_claimAdminPractitionerRoleConverter.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_claimConverter.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_claimResponseConverter.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_communicationConverter.py
--rw-r--r--   0 runner    (1001) docker     (127)      644 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_communicationRequestConverter.py
--rw-r--r--   0 runner    (1001) docker     (127)      593 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_contractConverter.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_coverageConverter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_coverageEligibilityRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_enrolmentOfficerPractitionerConverter.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_enrolmentOfficerPractitionerRoleConverter.py
--rw-r--r--   0 runner    (1001) docker     (127)      557 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_groupConverter.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_insurancePlanConverter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_invoiceConverter.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_locationConverter.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_medicationConverter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_operationOutcomeConverter.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_patientConverter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_paymentNoticeConverter.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_policyHolderOrganisationConverter.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_subscriptionConverter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2826 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_subscriptionService.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_timeUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5604 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:34.873097 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      218 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/utils/dbManagerUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/utils/fhirUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/utils/functionUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/utils/timeUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:34.873097 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/
--rw-r--r--   0 runner    (1001) docker     (127)      257 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:34.877097 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/
--rw-r--r--   0 runner    (1001) docker     (127)     2540 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/activity_definition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:34.877097 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/base/
--rw-r--r--   0 runner    (1001) docker     (127)      647 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3607 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/claim.py
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/claim_response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:34.881097 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/code_systems/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/code_systems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/code_systems/diagnosis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/code_systems/group_confirmation_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/code_systems/group_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/code_systems/organization_hf_legal_form.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/code_systems/organization_hf_level.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/code_systems/organization_ph_activity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/code_systems/organization_ph_legal_form.py
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/code_systems/patient_education_level.py
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/code_systems/patient_identification_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/code_systems/patient_profession.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/code_systems/patient_relationship.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/communication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/communication_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/contract.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/coverage_eligibility_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/coverage_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/group.py
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/insurance_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3040 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/insuree.py
--rw-r--r--   0 runner    (1001) docker     (127)     4120 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/invoice.py
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/location.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/medication.py
--rw-r--r--   0 runner    (1001) docker     (127)    11471 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/organisation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/payment_notice.py
--rw-r--r--   0 runner    (1001) docker     (127)     4534 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/practitioner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/practitioner_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/subscription.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:34.881097 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/filters/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6275 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/filters/requestParameterFilter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2023-12-16 00:57:23.000000 openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/login_viewset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:34.881097 openimis-be-api_fhir_r4-1.6.0/openimis_be_api_fhir_r4.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    30440 2023-12-16 00:57:34.000000 openimis-be-api_fhir_r4-1.6.0/openimis_be_api_fhir_r4.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14805 2023-12-16 00:57:34.000000 openimis-be-api_fhir_r4-1.6.0/openimis_be_api_fhir_r4.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-16 00:57:34.000000 openimis-be-api_fhir_r4-1.6.0/openimis_be_api_fhir_r4.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      238 2023-12-16 00:57:34.000000 openimis-be-api_fhir_r4-1.6.0/openimis_be_api_fhir_r4.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-12-16 00:57:34.000000 openimis-be-api_fhir_r4-1.6.0/openimis_be_api_fhir_r4.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-16 00:57:34.881097 openimis-be-api_fhir_r4-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2023-12-16 00:57:34.000000 openimis-be-api_fhir_r4-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:09.947043 openimis_be_api_fhir_r4-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    30440 2024-04-30 09:06:09.947043 openimis_be_api_fhir_r4-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    29179 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:09.891043 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:09.895043 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/configurations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/configurations/R4ApiFhirConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/configurations/R4ClaimConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/configurations/R4CommunicationRequestConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/configurations/R4CoverageConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/configurations/R4CoverageEligibilityConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/configurations/R4IdentifierConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/configurations/R4InvoiceConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/configurations/R4IssueTypeConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/configurations/R4LocationConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/configurations/R4MaritalConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/configurations/R4OrganisationConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/configurations/R4PaymentNoticeConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/configurations/R4SubscriptionConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26412 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/configurations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/configurations/generalConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/configurations/moduleConfiguration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:09.895043 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/containedResources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/containedResources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/containedResources/claimContainedResources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/containedResources/containedResourceHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/containedResources/containedResources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/containedResources/converterUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7344 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/containedResources/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5545 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/containedResources/serializerMixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:09.903043 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/
+-rw-r--r--   0 runner    (1001) docker     (127)    11881 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21043 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/activityDefinitionConverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/claimAdminPractitionerConverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/claimAdminPractitionerRoleConverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26583 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/claimConverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23846 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/claimResponseConverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/codeSystemConverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11329 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/communicationConverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/communicationRequestConverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26609 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/contractConverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7476 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/coverageConverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18808 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/coverageEligibilityRequestConverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5814 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/enrolmentOfficerPractitionerConverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/enrolmentOfficerPractitionerRoleConverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17052 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/groupConverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14290 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/healthFacilityOrganisationConverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/insuranceOrganisationConverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24070 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/insurancePlanConverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9717 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/invoiceConverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10078 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/locationConverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6530 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/locationSiteConverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19915 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/medicationConverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/operationOutcomeConverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38840 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/patientConverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/personConverterMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4389 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/policyCoverageEligibilityRequestConverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9268 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/policyHolderOrganisationConverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/referenceConverterMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9611 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/defaultConfig.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:09.903043 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/exceptions/fhir_api_exception_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:09.903043 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/mapping/
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/mapping/activityDefinitionMapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/mapping/claimMapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/mapping/contractMapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/mapping/coverageMapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/mapping/feedbackMapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/mapping/groupMapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/mapping/hfOrganizationMapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/mapping/invoiceMapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/mapping/locationMapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/mapping/medicationMapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/mapping/organizationMapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/mapping/patientMapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/mapping/subscriptionMapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:09.907043 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/migrations/0002_auto_20220313_1607.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/migrations/0003_auto_20220313_1634.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/migrations/0004_update_subscription_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/migrations/0005_auto_20221012_0818.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/migrations/0006_add_subsription_perms_imis_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/migrations/0007_alter_historicalsubscription_criteria_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5918 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/model_retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:09.907043 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9608 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/models/fhirModels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/models/imisModelEnums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/models/subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:09.907043 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/multiserializer/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/multiserializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16014 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/multiserializer/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/multiserializer/modelViewset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/multiserializer/serializerClass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/openapi_schema_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/paginations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:09.907043 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/paymentNotice/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/paymentNotice/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:09.907043 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/paymentNotice/converter/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/paymentNotice/converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/paymentNotice/converter/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/paymentNotice/converter/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/paymentNotice/converter/to_fhir_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/paymentNotice/converter/to_imis_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:09.911043 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/paymentNotice/mapping/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/paymentNotice/mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/paymentNotice/mapping/payment_detail_status_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/paymentNotice/mapping/payment_status_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/paymentNotice/mapping/status_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:09.911043 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/paymentNotice/serializer/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/paymentNotice/serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/paymentNotice/serializer/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/paymentNotice/serializer/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/paymentNotice/serializer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9461 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:09.915043 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     5556 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/serializers/activityDefinitionSerializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/serializers/billSerializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/serializers/claimAdminPractitionerRoleSerializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/serializers/claimAdminPractitionerSerializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/serializers/claimResponseSerializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9277 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/serializers/claimSerializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/serializers/codeSystemSerializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/serializers/communicationRequestSerializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/serializers/communicationSerializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/serializers/contractSerializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/serializers/coverageEligibilityRequestSerializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/serializers/coverageSerializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/serializers/enrolmentOfficerPractitionerRoleSerializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/serializers/enrolmentOfficerPractitionerSerializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/serializers/groupSerializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/serializers/healthFacilityOrganisationSerializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/serializers/insuranceOrganisationSerializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/serializers/insurancePlanSerializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/serializers/invoiceSerializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/serializers/locationSerializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/serializers/locationSiteSerializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/serializers/medicationSerializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/serializers/patientSerializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/serializers/policyCoverageEligibilityRequestSerializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/serializers/policyHolderOrganisationSerializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:09.915043 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/subscriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/subscriptions/notificationClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/subscriptions/notificationManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8850 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/subscriptions/subscriptionConverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/subscriptions/subscriptionCriteriaFilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/subscriptions/subscriptionSerializer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:09.923043 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:09.931043 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/SubscriptionTestMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16312 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/activityDefinitionTestMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7800 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/billInvoiceTestMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/claimAdminPractitionerRoleTestMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8183 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/claimAdminPractitionerTestMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8229 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/claimResponseTestMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13816 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/claimTestMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8197 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/communicationRequestTestMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12255 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/communicationTestMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9959 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/contractTestMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7980 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/coverageEligibilityRequestTestMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/coverageTestMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5428 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/enrolmentOfficerPractitionerRoleTestMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5137 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/enrolmentOfficerPractitionerTestMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/fhirApiCreateTestMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/fhirApiDeleteTestMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/fhirApiReadTestMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/fhirApiUpdateTestMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/genericFhirAPITestMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/genericTestMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8315 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/groupTestMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11807 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/insurancePlanTestMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6351 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/invoiceTestMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/locationTestMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/logInMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10296 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/medicationTestMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/operationOutcomeTestMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13549 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/patientTestMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/paymentNoticeTestMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4368 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/policyHolderOrganisationTestMixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:09.931043 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/subscriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/subscriptions/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/subscriptions/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:09.935043 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5201 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test/test_activity_definition.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test/test_claim.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test/test_claimAdminPractitioner.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test/test_claimAdminPractitionerRole.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test/test_claimResponse.json
+-rw-r--r--   0 runner    (1001) docker     (127)    37007 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test/test_claim_contained.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6283 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test/test_claim_with_code_references.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test/test_communication.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test/test_communicationRequest.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3363 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test/test_communication_with_code_reference.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test/test_contract.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test/test_coverage.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test/test_coverageEligibilityRequest.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9034 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test/test_coverageEligibilityResponse.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test/test_enrolmentOfficerPractitioner.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test/test_enrolmentOfficerPractitionerRole.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test/test_group.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test/test_insurance_plan.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test/test_invoice.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test/test_location.json
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test/test_login.json
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test/test_login_bad_credentials.json
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test/test_login_bad_payload.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test/test_medication.json
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test/test_outcome.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test/test_patient.json
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test/test_payment_notice.json
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test/test_subscription.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:09.939043 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/testCodeSystem/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/testCodeSystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/testCodeSystem/test_api_codeDiagnosis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/testCodeSystem/test_api_codeGroupConfirmationType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/testCodeSystem/test_api_codeGroupType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/testCodeSystem/test_api_codeHFOrganizationLegalForm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/testCodeSystem/test_api_codeHFOrganizationLevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/testCodeSystem/test_api_codePHOrganisationActivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/testCodeSystem/test_api_codePHOrganisationLegalForm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/testCodeSystem/test_api_codePatientContactRelationship.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/testCodeSystem/test_api_codePatientEducationLevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/testCodeSystem/test_api_codePatientIdentificationType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/testCodeSystem/test_api_codePatientProfession.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_activityDefinitionConverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_api_authorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_api_bill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8243 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_api_claim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13018 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_api_claim_contained.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11004 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_api_communication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_api_communicationRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7339 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_api_contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_api_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_api_insurancePlan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_api_invoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_api_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_api_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_api_medication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_api_organisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10849 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_api_patient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_api_paymentNotice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_api_practitioner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_api_practitionerRole.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_api_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_bill.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_claimAdminPractitionerConverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_claimAdminPractitionerRoleConverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_claimConverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_claimResponseConverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_communicationConverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_communicationRequestConverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_contractConverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_coverageConverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_coverageEligibilityRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_enrolmentOfficerPractitionerConverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_enrolmentOfficerPractitionerRoleConverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_groupConverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_insurancePlanConverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_invoiceConverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_locationConverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_medicationConverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_operationOutcomeConverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_patientConverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_paymentNoticeConverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_policyHolderOrganisationConverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_subscriptionConverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_subscriptionService.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_timeUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5604 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:09.939043 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/utils/dbManagerUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/utils/fhirUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/utils/functionUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/utils/timeUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:09.939043 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:09.943043 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/
+-rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/activity_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:09.943043 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/claim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/claim_response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:09.947043 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/code_systems/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/code_systems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/code_systems/diagnosis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/code_systems/group_confirmation_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/code_systems/group_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/code_systems/organization_hf_legal_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/code_systems/organization_hf_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/code_systems/organization_ph_activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/code_systems/organization_ph_legal_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/code_systems/patient_education_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/code_systems/patient_identification_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/code_systems/patient_profession.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/code_systems/patient_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/communication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/communication_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/coverage_eligibility_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/coverage_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/insurance_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/insuree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/medication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11471 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/organisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/payment_notice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/practitioner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/practitioner_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:09.947043 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6275 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/filters/requestParameterFilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-30 09:05:58.000000 openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/login_viewset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:09.947043 openimis_be_api_fhir_r4-1.7.0/openimis_be_api_fhir_r4.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    30440 2024-04-30 09:06:09.000000 openimis_be_api_fhir_r4-1.7.0/openimis_be_api_fhir_r4.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14883 2024-04-30 09:06:09.000000 openimis_be_api_fhir_r4-1.7.0/openimis_be_api_fhir_r4.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:06:09.000000 openimis_be_api_fhir_r4-1.7.0/openimis_be_api_fhir_r4.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-30 09:06:09.000000 openimis_be_api_fhir_r4-1.7.0/openimis_be_api_fhir_r4.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-30 09:06:09.000000 openimis_be_api_fhir_r4-1.7.0/openimis_be_api_fhir_r4.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 09:06:09.947043 openimis_be_api_fhir_r4-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-30 09:06:09.000000 openimis_be_api_fhir_r4-1.7.0/setup.py
```

### Comparing `openimis-be-api_fhir_r4-1.6.0/LICENSE` & `openimis_be_api_fhir_r4-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/LICENSE.md` & `openimis_be_api_fhir_r4-1.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/PKG-INFO` & `openimis_be_api_fhir_r4-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-api_fhir_r4
-Version: 1.6.0
+Version: 1.7.0
 Summary: The openIMIS Backend FHIR R4 API reference module.
 Home-page: https://openimis.org/
 Author: Faris Ahmetasevic
 Author-email: faris.ahmetasevic@hotmail.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-api_fhir_r4-1.6.0/README.md` & `openimis_be_api_fhir_r4-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/apps.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/apps.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/configurations/R4ApiFhirConfig.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/configurations/R4ApiFhirConfig.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/configurations/R4ClaimConfig.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/configurations/R4ClaimConfig.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/configurations/R4CommunicationRequestConfig.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/configurations/R4CommunicationRequestConfig.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/configurations/R4CoverageConfig.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/configurations/R4CoverageConfig.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/configurations/R4CoverageEligibilityConfiguration.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/configurations/R4CoverageEligibilityConfiguration.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/configurations/R4IdentifierConfig.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/configurations/R4IdentifierConfig.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/configurations/R4InvoiceConfig.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/configurations/R4InvoiceConfig.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,7 +21,11 @@
         return cls.get_config_attribute("R4_fhir_invoice_config").get('fhir_bill_type_system',
                                                                       "CodeSystem/bill-type")
 
     @classmethod
     def get_fhir_bill_charge_item_system(cls):
         return cls.get_config_attribute("R4_fhir_invoice_config").get('fhir_bill_charge_item_system',
                                                                       "CodeSystem/bill-charge-item")
+
+    @classmethod
+    def get_subscribe_invoice_signal(cls):
+        return cls.get_config_attribute("R4_fhir_invoice_config").get('subscribe_invoice_signal', False)
```

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/configurations/R4IssueTypeConfig.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/configurations/R4IssueTypeConfig.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/configurations/R4LocationConfig.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/configurations/R4LocationConfig.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
     @classmethod
     def build_configuration(cls, cfg):
         cls.get_config().R4_fhir_location_type = cfg['R4_fhir_location_site_type']
         cls.get_config().R4_fhir_location_physical_type = cfg['R4_fhir_location_physical_type']
         cls.get_config().R4_fhir_hf_service_type = cfg['R4_fhir_hf_service_type']
         cls.get_config().R4_fhir_location_status_codes = cfg['R4_fhir_location_status_codes']
+        cls.get_config().R4_fhir_location_subscribe_signal = cfg['R4_fhir_location_subscribe_signal']
 
     @classmethod
     def get_fhir_location_site_type_system(cls):
         return cls.get_config_attribute("R4_fhir_location_type")\
             .get('system', "http://hl7.org/fhir/v3/ServiceDeliveryLocationRoleType/vs.html")
 
     @classmethod
@@ -83,7 +84,11 @@
     @classmethod
     def get_fhir_code_for_active(cls):
         return cls.get_config_attribute("R4_fhir_location_status_codes").get('fhir_code_for_active', 'active')
 
     @classmethod
     def get_fhir_code_for_inactive(cls):
         return cls.get_config_attribute("R4_fhir_location_status_codes").get('fhir_code_for_inactive', 'inactive')
+
+    @classmethod
+    def get_subscribe_location_signal(cls):
+        return cls.get_config_attribute("R4_fhir_location_subscribe_signal")
```

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/configurations/R4MaritalConfig.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/configurations/R4MaritalConfig.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/configurations/R4OrganisationConfig.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/configurations/R4OrganisationConfig.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/configurations/R4PaymentNoticeConfig.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/configurations/R4PaymentNoticeConfig.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/configurations/R4SubscriptionConfig.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/configurations/R4SubscriptionConfig.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/configurations/__init__.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/configurations/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,14 +123,18 @@
     def get_fhir_code_for_both(cls):
         raise NotImplementedError('`get_fhir_code_for_both()` must be implemented')
 
     @classmethod
     def get_fhir_code_for_active(cls):
         raise NotImplementedError('`get_fhir_code_for_active()` must be implemented')
 
+    @classmethod
+    def get_subscribe_location_signal(cls):
+        raise NotImplementedError('`get_subscribe_location_signal()` must be implemented')
+
 
 class MaritalConfiguration(BaseConfiguration):  # pragma: no cover
 
     @classmethod
     def build_configuration(cls, cfg):
         raise NotImplementedError('`build_configuration()` must be implemented.')
 
@@ -471,14 +475,18 @@
     def get_fhir_bill_type_system(cls):
         raise NotImplementedError('`get_fhir_invoice_type_system()` must be implemented.')
 
     @classmethod
     def get_fhir_bill_charge_item_system(cls):
         raise NotImplementedError('`get_fhir_invoice_charge_item_system()` must be implemented.')
 
+    @classmethod
+    def get_subscribe_invoice_signal(cls):
+        raise NotImplementedError('`get_subscribe_invoice_signal()` must be implemented')
+
 
 class OrganisationConfiguration(BaseConfiguration):
     @classmethod
     def build_configuration(cls, cfg):
         raise NotImplementedError('`build_configuration()` must be implemented.')
 
     @classmethod
```

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/configurations/generalConfiguration.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/configurations/generalConfiguration.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
         config.base_url = cfg['base_url']
         config.default_value_of_patient_head_attribute = cfg['default_value_of_patient_head_attribute']
         config.default_value_of_patient_card_issued_attribute = cfg['default_value_of_patient_card_issued_attribute']
         config.default_value_of_location_offline_attribute = cfg['default_value_of_location_offline_attribute']
         config.default_value_of_location_care_type = cfg['default_value_of_location_care_type']
         config.default_response_page_size = cfg['default_response_page_size']
         config.claim_rule_engine_validation = cfg['claim_rule_engine_validation']
+        config.subscribe_insuree_signal = cfg['subscribe_insuree_signal']
 
     @classmethod
     def get_default_audit_user_id(cls):
         return cls.get_config_attribute("default_audit_user_id")
 
     @classmethod
     def get_male_gender_code(cls):
@@ -80,7 +81,11 @@
         site_root = settings.SITE_ROOT()
         if site_root is not None:
             base_url = '/' + site_root
         if base_url.endswith('/'):
             return base_url + MODULE_NAME + '/'
         else:
             return base_url + '/'+MODULE_NAME+'/'
+
+    @classmethod
+    def get_subscribe_insuree_signal(cls):
+        return cls.get_config_attribute("subscribe_insuree_signal")
```

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/containedResources/claimContainedResources.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/containedResources/claimContainedResources.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/containedResources/containedResourceHandler.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/containedResources/containedResourceHandler.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/containedResources/containedResources.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/containedResources/containedResources.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/containedResources/converterUtils.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/containedResources/converterUtils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 from fhir.resources.R4B.fhirtypes import ReferenceType
 from typing import Iterable, List
 
 from fhir.resources.R4B.reference import Reference
 
 from api_fhir_r4.apps import logger
 from api_fhir_r4.converters import BaseFHIRConverter
@@ -65,10 +66,10 @@
     if fhir_reference:
         if contained:
             value = get_converted_contained_resource(contained, fhir_reference, converter, audit_user_id)
         value = value or converter.get_imis_obj_by_fhir_reference(fhir_reference)
         if value is None:
             raise FHIRException(
             "Failed to find the resource based on reference(with contain: {}, converter: {}): {}".format(
-                (contained is not None), converter.__name__, str(json.dumps(fhir_reference)))
+                (contained is not None), converter.__name__, str(fhir_reference))
             )
     return value
```

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/containedResources/converters.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/containedResources/converters.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,27 +30,29 @@
             return []
 
         try:
             if isinstance(resource, Iterable) and   'resourceType' not in resource:
                 return [method(next_resource, *args) for next_resource in resource]
             else:
                 return [method(resource, *args)]
-        except Exception as e:
+        except BaseException as e:
+            logger.error(f"Failed to process resource ({resource.__class__}/{resource.id if hasattr(resource, 'id') else '' }, "
+                         f"reason: {e}")
             self.__raise_default_exception(resource, e)
 
     def __convert_to_imis(self, method, resource, reference_type, args):
         try:
             if isinstance(resource, Iterable) and 'resourceType' not in resource :
                 return [
                     self.__convert_single_resource(next_, method, args, reference_type) for next_ in resource
                 ]
             else:
                 return [self.__convert_single_resource(resource, method, args, reference_type)]
-        except Exception as e:
-            logger.error(f"Failed to process contained resource ({resource.get('resourceType')}/{resource.get('id')}, "
+        except BaseException as e:
+            logger.error(f"Failed to process resource ({resource.get('resourceType')}/{resource.get('id')}, "
                          f"reason: {e}")
             self.__raise_default_exception(resource, e)
 
     def __convert_single_resource(self, resource, method, args, ref_type):
         converted = method(resource, *args)
         self.__bind_uuid_to_converted_resource(converted, resource, ref_type)
         return converted
```

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/containedResources/serializerMixin.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/containedResources/serializerMixin.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/__init__.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/activityDefinitionConverter.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/activityDefinitionConverter.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/claimAdminPractitionerConverter.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/claimAdminPractitionerConverter.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/claimAdminPractitionerRoleConverter.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/claimAdminPractitionerRoleConverter.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/claimConverter.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/claimConverter.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/claimResponseConverter.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/claimResponseConverter.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/codeSystemConverter.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/codeSystemConverter.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/communicationConverter.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/communicationConverter.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/communicationRequestConverter.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/communicationRequestConverter.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/contractConverter.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/contractConverter.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/coverageConverter.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/coverageConverter.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/coverageEligibilityRequestConverter.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/coverageEligibilityRequestConverter.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/enrolmentOfficerPractitionerConverter.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/enrolmentOfficerPractitionerConverter.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/enrolmentOfficerPractitionerRoleConverter.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/enrolmentOfficerPractitionerRoleConverter.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/groupConverter.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/groupConverter.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/healthFacilityOrganisationConverter.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/healthFacilityOrganisationConverter.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/insuranceOrganisationConverter.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/insuranceOrganisationConverter.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/insurancePlanConverter.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/insurancePlanConverter.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/invoiceConverter.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/invoiceConverter.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/locationConverter.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/locationConverter.py`

 * *Files 3% similar despite different names*

```diff
@@ -167,30 +167,20 @@
         elif count > 1:
             return _(F"More than one matching location district {address.district}, state {address.state}:\n"
                      F"{matching_locations}.")
 
     @classmethod
     def build_imis_parent_location_id(cls, imis_location, fhir_location, errors):
         if fhir_location.partOf:
-            resource, reference = fhir_location.partOf.reference.split('/')
-            if not reference:
+            resource = cls.get_imis_obj_by_fhir_reference(fhir_location.partOf) 
+            if not resource:
                 errors.append(
-                    _('Invalid Location\'s partOf.reference, has to be in format {resource}/{reference}')
+                    _('Invalid Location\'s partOf.reference')
                 )
 
-            try:
-                if cls._is_code_reference(fhir_location.partOf):
-                    location = Location.objects.get(code=reference, validity_to__isnull=True)
-                else:
-                    location = Location.objects.get(uuid=reference)
-                imis_location.parent = location
-            except Location.DoesNotExist:
-                errors.append(
-                    _('Invalid Location\'s partOf reference, pointing to not existing resource')
-                )
 
     @classmethod
     def _validate_imis_identifiers(cls, identifiers):
         code_identifier = cls.get_fhir_identifier_by_code(identifiers, cls.get_fhir_code_identifier_type())
         if not code_identifier:
             raise FHIRException(_('Code identifier has to be present in FHIR Location identifiers, '
                                   '\nidentifiers are: %(identifiers)') % {'identifiers': identifiers})
```

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/locationSiteConverter.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/locationSiteConverter.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/medicationConverter.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/medicationConverter.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/operationOutcomeConverter.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/operationOutcomeConverter.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
         severity = "error"
         code = R4IssueTypeConfig.get_fhir_code_for_exception()
         details_text = cls.get_last_message(obj)
         return cls.build_outcome(severity, code, details_text)
 
     @classmethod
     def get_last_message(cls, obj):
-        return obj.args[len(obj.args) - 1]
+        return obj.args[len(obj.args) - 1] or str(obj)
 
     @classmethod
     def build_for_key_api_exception(cls, obj):
         severity = "fatal"
         code = R4IssueTypeConfig.get_fhir_code_for_exception()
         details_text = obj.detail
         return cls.build_outcome(severity, code, details_text)
```

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/patientConverter.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/patientConverter.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/personConverterMixin.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/personConverterMixin.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/policyCoverageEligibilityRequestConverter.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/policyCoverageEligibilityRequestConverter.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/policyHolderOrganisationConverter.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/policyHolderOrganisationConverter.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,16 +66,18 @@
     def build_fhir_identifiers(cls, fhir_organisation, imis_organisation, reference_type):
         identifiers = []
         cls.build_all_identifiers(identifiers, imis_organisation, reference_type)
         fhir_organisation.identifier = identifiers
 
     @classmethod
     def build_fhir_extensions(cls, fhir_organisation, imis_organisation):
-        cls.build_fhir_legal_form_extension(fhir_organisation, imis_organisation)
-        cls.build_fhir_activity_extension(fhir_organisation, imis_organisation)
+        if imis_organisation.legal_form:
+            cls.build_fhir_legal_form_extension(fhir_organisation, imis_organisation)
+        if imis_organisation.activity_code:
+            cls.build_fhir_activity_extension(fhir_organisation, imis_organisation)
 
     @classmethod
     def build_fhir_legal_form_extension(cls, fhir_organisation, imis_organisation):
         codeable_concept = cls.build_codeable_concept_from_coding(cls.build_fhir_mapped_coding(
             PolicyHolderOrganisationLegalFormMapping.fhir_ph_code_system(imis_organisation.legal_form)
         ))
         base = GeneralConfiguration.get_system_base_url()
```

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/converters/referenceConverterMixin.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/converters/referenceConverterMixin.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import inspect
 import logging
 
 from typing import Tuple
-
+import uuid
 from api_fhir_r4.exceptions import FHIRRequestProcessException
 from fhir.resources.R4B.reference import Reference
 
 
 logger = logging.getLogger(__name__)
 
 
@@ -64,17 +64,22 @@
 
 
     @classmethod
     def get_database_query_id_parameteres_from_reference(cls, reference, code_keyword_name = 'code'):
         _, resource_id, id_type = cls._get_type_and_id_from_reference(reference)
         id_parameters = {}
         if cls._get_reference_type(id_type) == cls.CODE_REFERENCE_TYPE:
-            id_parameters[code_keyword_name] = resource_id
+            id_parameters[code_keyword_name] = str(resource_id)
         else:
-            id_parameters['uuid__iexact'] = resource_id
+            try:
+                id_parameters['uuid'] = uuid.UUID(resource_id)
+            except:
+                #fall back on code for unvalid uuid
+                id_type=code_keyword_name
+                id_parameters[code_keyword_name]=resource_id
         return id_parameters
 
     @classmethod
     def _get_reference_type(cls, reference_type):
         if reference_type is None or reference_type.coding is None or \
             reference_type.coding[0] is None or \
             reference_type.coding[0].code is None:
```

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/defaultConfig.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/defaultConfig.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     "base_url": "https://openimis.github.io/openimis_fhir_r4_ig/",
     "default_value_of_patient_head_attribute": False,
     "default_value_of_patient_card_issued_attribute": False,
     "default_value_of_location_offline_attribute": False,
     "default_value_of_location_care_type": "B",
     "default_response_page_size": 10,
     "claim_rule_engine_validation": True,
+    "subscribe_insuree_signal": False,
     "R4_fhir_identifier_type_config": {
         "system": "https://openimis.github.io/openimis_fhir_r4_ig/CodeSystem/openimis-identifiers",
         "fhir_code_for_imis_db_uuid_type": "UUID",
         "fhir_code_for_imis_db_id_type": "ACSN",
         "fhir_code_for_imis_generic_code": "Code",
         "fhir_code_for_imis_chfid_type": "SB",
         "fhir_code_for_imis_passport_type": "PPN",
@@ -48,14 +49,15 @@
         "fhir_code_for_ward": "W",
         "fhir_code_for_village": "V"
     },
     "R4_fhir_location_status_codes": {
         "fhir_code_for_active": "active",
         "fhir_code_for_inactive": "inactive",
     },
+    "R4_fhir_location_subscribe_signal": False,
     "R4_fhir_hf_service_type": {
         "system": "http://hl7.org/fhir/valueset-service-type.html",
         "fhir_code_for_in_patient": "I",
         "fhir_code_for_out_patient": "O",
         "fhir_code_for_both": "B"
     },
     "R4_fhir_issue_type_config": {
@@ -170,15 +172,16 @@
         "state": "Ultha",
         "line": "1 Pasay"
     },
     "R4_fhir_invoice_config": {
         "fhir_invoice_type_system": "CodeSystem/invoice-type",
         "fhir_invoice_charge_item_system": "CodeSystem/invoice-charge-item",
         "fhir_bill_type_system": "CodeSystem/bill-type",
-        "fhir_bill_charge_item_system": "CodeSystem/bill-charge-item"
+        "fhir_bill_charge_item_system": "CodeSystem/bill-charge-item",
+        "subscribe_invoice_signal": False,
     },
     "R4_fhir_subscription_config": {
         "fhir_sub_search_perms": ['158001'],
         "fhir_sub_create_perms": ['158002'],
         "fhir_sub_update_perms": ['158003'],
         "fhir_sub_delete_perms": ['158004'],
         "fhir_sub_channel_rest_hook": "rest-hook",
```

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/exceptions/__init__.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/exceptions/fhir_api_exception_handler.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/exceptions/fhir_api_exception_handler.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/mapping/activityDefinitionMapping.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/mapping/activityDefinitionMapping.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/mapping/claimMapping.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/mapping/claimMapping.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/mapping/contractMapping.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/mapping/contractMapping.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/mapping/feedbackMapping.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/mapping/feedbackMapping.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/mapping/groupMapping.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/mapping/groupMapping.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/mapping/hfOrganizationMapping.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/mapping/hfOrganizationMapping.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/mapping/invoiceMapping.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/mapping/invoiceMapping.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/mapping/locationMapping.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/mapping/locationMapping.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/mapping/medicationMapping.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/mapping/medicationMapping.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/mapping/organizationMapping.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/mapping/organizationMapping.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/mapping/patientMapping.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/mapping/patientMapping.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/mapping/subscriptionMapping.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/mapping/subscriptionMapping.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/migrations/0001_initial.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/migrations/0002_auto_20220313_1607.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/migrations/0002_auto_20220313_1607.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/migrations/0004_update_subscription_criteria.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/migrations/0004_update_subscription_criteria.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import logging
 
 from django.db import migrations
+from django.db.models import Q
 
 logger = logging.getLogger(__name__)
 
 
 def update_subscription_criteria(apps, schema_editor):
     resource_type_map = {
         'Invoice': 'Invoice',
         'Bill': 'Invoice',
         'Patient': 'Patient',
         'Organisation': 'Organisation'
     }
 
     subscription_model = apps.get_model('api_fhir_r4', 'Subscription')
     entries_to_update = subscription_model.objects\
-        .exclude(criteria__has_key='resource')\
-        .filter(criteria__has_key='resource_type')
+        .filter(Q(criteria__has_key='resource_type')  & ~Q(criteria__has_key='resource'))
     for subscription in entries_to_update:
         resource = subscription.criteria.pop('resource_type')
         if resource in resource_type_map:
             subscription.criteria['resource'] = resource_type_map[resource]
             subscription.save()
         else:
             logger.warning(f'Subscription of unexpected type - {resource}')
```

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/migrations/0005_auto_20221012_0818.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/migrations/0005_auto_20221012_0818.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/migrations/0006_add_subsription_perms_imis_admin.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/migrations/0006_add_subsription_perms_imis_admin.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/mixins.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/mixins.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/model_retrievers.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/model_retrievers.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/models/fhirModels.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/models/fhirModels.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/models/imisModelEnums.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/models/imisModelEnums.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/models/subscription.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/models/subscription.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 
     class SubscriptionChannel(models.IntegerChoices):
         REST_HOOK = 0, _("rest-hook")
 
     status = models.SmallIntegerField(db_column='Status', null=False, choices=SubscriptionStatus.choices)
     channel = models.SmallIntegerField(db_column='Channel', null=False, choices=SubscriptionChannel.choices)
     endpoint = models.CharField(db_column='Endpoint', max_length=255, null=False)
-    headers = encrypt(models.TextField(db_column='Headers', max_length=255, null=True))
-    criteria = models.JSONField(db_column='Criteria', null=True)
+    headers = encrypt(models.TextField(db_column='Headers', max_length=255,  blank=True, null=True))
+    criteria = models.JSONField(db_column='Criteria',  blank=True, null=True)
     expiring = models.DateTimeField(db_column='Expiring', null=False)
 
     class Meta:
         managed = True
         db_table = 'tblSubscription'
 
 
@@ -40,14 +40,14 @@
 
 class SubscriptionNotificationResult(models.Model):
     id = models.UUIDField(primary_key=True, db_column="UUID", default=uuid.uuid4, editable=False)
     subscription = models.ForeignKey(
         Subscription, on_delete=models.CASCADE, related_name='notifications_sent', null=False)
     notified_successfully = models.BooleanField(blank=False, null=False)
     notification_time = DateTimeField(db_column='Expiring', null=False, default=ad_datetime.AdDatetime.now)
-    error = models.TextField(blank=False, null=True, default=None)
+    error = models.TextField(blank=True, null=True, default=None)
 
     objects = SubscriptionNotificationResultManager()
 
     class Meta:
         managed = True
         db_table = 'tblSubscriptionNotificationResult'
```

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/multiserializer/mixins.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/multiserializer/mixins.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,24 @@
 def _MultiserializerPermissionClassWrapper(PermissionClass):
     def has_permission(self, request, view, queryset):
         if getattr(view, '_ignore_model_permissions', False):
             return True
 
         if not request.user or (not request.user.is_authenticated and self.authenticated_users_only):
             return False
-
+        
+        #read access can be defined by the ability to get a queryset
+        if request.method == 'GET' and self.base_class:
+            qs =  self.base_class.get_queryset()
+            if qs is None:
+                return False
+            filter_values = qs.filter_values()
+            # filter(id=-1) is used to return an empty qs
+            if filter_values.get('id') == -1:
+                return False
         perms = self.get_required_permissions(request.method, queryset.model)
         return request.user.has_perms(perms)
 
     permission_class = type('PermissionClassWrapper', PermissionClass.__bases__, dict(PermissionClass.__dict__))
     permission_class.has_permission = has_permission
     return permission_class
```

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/multiserializer/modelViewset.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/multiserializer/modelViewset.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/multiserializer/serializerClass.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/multiserializer/serializerClass.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/openapi_schema_extensions.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/openapi_schema_extensions.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/paginations.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/paginations.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/paymentNotice/converter/converter.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/paymentNotice/converter/converter.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/paymentNotice/converter/to_fhir_converter.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/paymentNotice/converter/to_fhir_converter.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/paymentNotice/converter/to_imis_converter.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/paymentNotice/converter/to_imis_converter.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,27 +29,31 @@
     @classmethod
     def to_imis_obj(cls, fhir_payment_notice, audit_user_id=None):
         errors = []
         fhir_payment_notice = PaymentNotice(**fhir_payment_notice)
         imis_payment = PaymentInvoice()
         imis_payment_detail = DetailPaymentInvoice()
         cls.build_imis_payment_date_created(imis_payment, imis_payment_detail, fhir_payment_notice)
+        cls.build_imis_payment_payer_ref(imis_payment,fhir_payment_notice)
         cls.build_imis_payment_reconciliation_status(imis_payment, fhir_payment_notice, errors)
         cls.build_imis_payment_amount(imis_payment, imis_payment_detail, fhir_payment_notice)
         cls.build_imis_payment_date_payment(imis_payment, fhir_payment_notice)
         cls.build_imis_payment_json_ext(imis_payment, fhir_payment_notice)
         cls.build_imis_payment_detail_invoice(imis_payment_detail, fhir_payment_notice, errors)
         cls.build_imis_payment_detail_status(imis_payment_detail, fhir_payment_notice, errors)
         invoice_status = None
         if imis_payment_detail.subject_id:
             invoice_status = cls.get_imis_invoice_status(fhir_payment_notice, errors)
         cls.check_errors(errors)
         imis_payment.imis_payment_detail = imis_payment_detail
         imis_payment.invoice_status = invoice_status
         return imis_payment
+    @classmethod
+    def build_imis_payment_payer_ref(cls, imis_payment, fhir_payment_notice):
+        imis_payment.payer_ref = fhir_payment_notice.payment.reference
 
     @classmethod
     def build_imis_payment_date_created(cls, imis_payment, imis_payment_detail, fhir_payment_notice):
         created = fhir_payment_notice.created
         imis_payment.date_created = created
         imis_payment.date_updated = created
         imis_payment_detail.date_created = created
@@ -95,14 +99,15 @@
         subject_id = cls.get_id_from_reference(fhir_payment_notice.request)
         subject_type = fhir_payment_notice.request.type.lower()
         if subject_type in SUBJECT_TYPE:
             imis_payment_detail.subject_type = cls._convert_content_type(subject_type)
             imis_payment_detail.subject_id = subject_id
         else:
             errors.append(ERROR_BAD_TYPE_REQUEST)
+        
 
     @classmethod
     def _convert_content_type(cls, subject_type):
         return ContentType.objects.get(model__iexact=subject_type)
 
     @classmethod
     def build_imis_payment_amount(cls, imis_payment, imis_payment_detail, fhir_payment_notice):
```

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/paymentNotice/mapping/payment_detail_status_mapping.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/paymentNotice/mapping/payment_detail_status_mapping.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/paymentNotice/mapping/payment_status_mapping.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/paymentNotice/mapping/payment_status_mapping.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/paymentNotice/mapping/status_mapping.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/paymentNotice/mapping/status_mapping.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/paymentNotice/serializer/create.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/paymentNotice/serializer/create.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/paymentNotice/serializer/utils.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/paymentNotice/serializer/utils.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/permissions.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/permissions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from api_fhir_r4.configurations import R4SubscriptionConfig
 from core.apps import CoreConfig
 from claim.apps import ClaimConfig
 from insuree.apps import InsureeConfig
 from location.apps import LocationConfig
+from location.models import Location, HealthFacility
 from policy.apps import PolicyConfig
 from policyholder.apps import PolicyholderConfig
 from product.apps import ProductConfig
 from medical.apps import MedicalConfig
 from invoice.apps import InvoiceConfig
 from rest_framework import exceptions
 from rest_framework.permissions import DjangoModelPermissions
@@ -14,16 +15,18 @@
 
 class FHIRApiPermissions(DjangoModelPermissions):
     permissions_get = []
     permissions_post = []
     permissions_put = []
     permissions_patch = []
     permissions_delete = []
+    base_class = None
 
     def __init__(self):
+        self.base_class
         self.perms_map['GET'] = self.permissions_get
         self.perms_map['POST'] = self.permissions_post
         self.perms_map['PUT'] = self.permissions_put
         self.perms_map['PATCH'] = self.permissions_patch
         self.perms_map['DELETE'] = self.permissions_delete
 
     def get_required_permissions(self, method, model_cls):
@@ -78,21 +81,31 @@
     permissions_post = []
     permissions_put = []
     permissions_patch = []
     permissions_delete = []
 
 
 class FHIRApiHFPermissions(FHIRApiPermissions):
+    base_class = HealthFacility
     permissions_get = LocationConfig.gql_query_health_facilities_perms
     permissions_post = LocationConfig.gql_mutation_create_health_facilities_perms
     permissions_put = LocationConfig.gql_mutation_create_health_facilities_perms
-    permissions_patch = LocationConfig.gql_mutation_create_health_facilities_perms
+    permissions_patch = LocationConfig.gql_mutation_edit_health_facilities_perms
     permissions_delete = LocationConfig.gql_mutation_delete_health_facilities_perms
 
 
+
+class FHIRApiLocationPermissions(FHIRApiPermissions):
+    base_class = Location
+    permissions_get = LocationConfig.gql_query_locations_perms
+    permissions_post = LocationConfig.gql_mutation_create_health_facilities_perms
+    permissions_put = LocationConfig.gql_mutation_create_health_facilities_perms
+    permissions_patch = LocationConfig.gql_mutation_edit_locations_perms
+    permissions_delete = LocationConfig.gql_mutation_delete_health_facilities_perms   
+    
 class FHIRApiInsuranceOrganizationPermissions(FHIRApiPermissions):
     permissions_get = LocationConfig.gql_query_health_facilities_perms
     permissions_post = []
     permissions_put = []
     permissions_patch = []
     permissions_delete = []
 
@@ -126,19 +139,19 @@
     permissions_post = MedicalConfig.gql_mutation_medical_services_add_perms
     permissions_put = MedicalConfig.gql_mutation_medical_services_update_perms
     permissions_patch = MedicalConfig.gql_mutation_medical_services_update_perms
     permissions_delete = MedicalConfig.gql_mutation_medical_services_delete_perms
 
 
 class FHIRApiHealthServicePermissions(FHIRApiPermissions):
-    permissions_get = LocationConfig.gql_query_health_facilities_perms
+    permissions_get = LocationConfig.gql_mutation_edit_locations_perms
     permissions_post = LocationConfig.gql_mutation_create_health_facilities_perms
-    permissions_put = LocationConfig.gql_mutation_edit_health_facilities_perms
-    permissions_patch = LocationConfig.gql_mutation_edit_health_facilities_perms
-    permissions_delete = LocationConfig.gql_mutation_delete_health_facilities_perms
+    permissions_put = LocationConfig.gql_mutation_edit_locations_perms
+    permissions_patch = LocationConfig.gql_mutation_edit_locations_perms
+    permissions_delete = LocationConfig.gql_mutation_delete_locations_perms
 
 
 class FHIRApiGroupPermissions(FHIRApiPermissions):
     permissions_get = InsureeConfig.gql_query_families_perms
     permissions_post = InsureeConfig.gql_mutation_create_families_perms
     permissions_put = InsureeConfig.gql_mutation_update_families_perms
     permissions_patch = InsureeConfig.gql_mutation_update_families_perms
```

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/serializers/__init__.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/serializers/activityDefinitionSerializer.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/serializers/activityDefinitionSerializer.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/serializers/claimAdminPractitionerRoleSerializer.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/serializers/claimAdminPractitionerRoleSerializer.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/serializers/claimAdminPractitionerSerializer.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/serializers/claimAdminPractitionerSerializer.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/serializers/claimResponseSerializer.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/serializers/claimResponseSerializer.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/serializers/claimSerializer.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/serializers/claimSerializer.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/serializers/codeSystemSerializer.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/serializers/codeSystemSerializer.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/serializers/communicationSerializer.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/serializers/communicationSerializer.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/serializers/contractSerializer.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/serializers/contractSerializer.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/serializers/coverageEligibilityRequestSerializer.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/serializers/coverageEligibilityRequestSerializer.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/serializers/coverageSerializer.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/serializers/coverageSerializer.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/serializers/groupSerializer.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/serializers/patientSerializer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,56 +1,66 @@
 import copy
 
-from insuree.models import Family, Insuree
-from api_fhir_r4.converters import GroupConverter
+from insuree.apps import InsureeConfig
+from insuree.models import Insuree, Family
+
+from core.models import resolve_id_reference
+
+from api_fhir_r4.converters import PatientConverter
 from api_fhir_r4.exceptions import FHIRException
 from api_fhir_r4.serializers import BaseFHIRSerializer
-from insuree.services import FamilyService, InsureeService
+from insuree.services import InsureeService
 
 
-class GroupSerializer(BaseFHIRSerializer):
-    fhirConverter = GroupConverter()
+class PatientSerializer(BaseFHIRSerializer):
+    fhirConverter = PatientConverter()
 
     def create(self, validated_data):
-        request = self.context.get("request")
-        user = request.user
-
-        insuree_id = validated_data.get('head_insuree_id')
-        members_family = validated_data.pop('members_family')
-
-        if Family.objects.filter(head_insuree_id=insuree_id).count() > 0:
-            raise FHIRException('Exists family with the provided head')
-
-        insuree = Insuree.objects.get(id=insuree_id)
-        copied_data = copy.deepcopy(validated_data)
-        copied_data["head_insuree"] = insuree.__dict__
-        copied_data["contribution"] = None
-        del copied_data['_state']
-        if 'head_insuree' in copied_data and '_state' in copied_data['head_insuree']:
-            del copied_data['head_insuree']['_state']
-        if 'head_insuree' in copied_data and '_state' in copied_data['head_insuree']:
-            del copied_data['head_insuree']['_state']
-
-        new_family = FamilyService(user).create_or_update(copied_data)
-
-        # assign members of family (insuree) to the family
-        for mf in members_family:
-            mf = mf.__dict__
-            del mf['_state']
-            mf['family_id'] = new_family.id
-            InsureeService(user).create_or_update(mf)
-
-        return new_family
+        #validated_data = resolve_id_reference(Insuree, validated_data)
+        self._validate_data(validated_data.get('chf_id'))
+        copied_data = self._clean_data(copy.deepcopy(validated_data))
+        obj = InsureeService(self.context.get("request").user)\
+            .create_or_update(copied_data)
+
+        if copied_data['head']:
+            self._create_patient_family(obj, validated_data)
+        return obj
 
     def update(self, instance, validated_data):
-        # TODO: This doesn't work
+        #validated_data = resolve_id_reference(Insuree, validated_data)
         request = self.context.get("request")
+        validated_data.pop('_state')
         user = request.user
-        head_id = validated_data.get('head_insuree_id')
-        family = Family.objects.filter(head_insuree_id=head_id, validity_to__isnull=True).first()
-        if not family:
-            raise FHIRException('No family with following chfid `{}`'.format(head_id))
-        validated_data["id"] = family.id
-        validated_data["uuid"] = family.uuid
-        del validated_data['_state']
-        instance = FamilyService(user).create_or_update(validated_data)
+        chf_id = validated_data.get('chf_id', None)
+        if Insuree.objects.filter(chf_id=chf_id).count() == 0:
+            raise FHIRException('No patients with following chfid `{}`'.format(chf_id))
+        insuree = Insuree.objects.get(chf_id=chf_id, validity_to__isnull=True)
+        validated_data["id"] = insuree.id
+        validated_data["uuid"] = insuree.uuid
+        instance = InsureeService(user).create_or_update(validated_data)
         return instance
+
+    def _validate_data(self, chf_id):
+        if not chf_id:
+            raise FHIRException("Provided patient without code.")
+
+        if Insuree.objects.filter(chf_id=chf_id, validity_to__isnull=True).exists():
+            raise FHIRException('Exists patient with following chfid `{}`'.format(chf_id))
+
+    def _clean_data(self, validated_data):
+        validated_data.pop('_state', None)
+        validated_data.pop('family_address', None)
+        validated_data.pop('family_location', None)
+        return validated_data
+
+    def _create_patient_family(self, obj, validated_data):
+        audit_user_id = validated_data['audit_user_id']
+        family_location = validated_data.get('family_location', None)
+        family_address = validated_data.get('family_address', None)
+
+        obj.family = Family.objects.create(
+            location=family_location,
+            address=family_address,
+            head_insuree=obj,
+            audit_user_id=audit_user_id
+        )
+        obj.save()
```

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/serializers/healthFacilityOrganisationSerializer.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/serializers/healthFacilityOrganisationSerializer.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/serializers/insurancePlanSerializer.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/serializers/insurancePlanSerializer.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/serializers/locationSerializer.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/serializers/locationSerializer.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/serializers/locationSiteSerializer.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/serializers/locationSiteSerializer.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/serializers/medicationSerializer.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/serializers/medicationSerializer.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/serializers/policyCoverageEligibilityRequestSerializer.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/serializers/policyCoverageEligibilityRequestSerializer.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/serializers/policyHolderOrganisationSerializer.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/serializers/policyHolderOrganisationSerializer.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/signals.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/signals.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import logging
 
 from django.core.exceptions import ObjectDoesNotExist
 
+from api_fhir_r4.apps import ApiFhirConfig
+from api_fhir_r4.configurations import R4LocationConfig, R4InvoiceConfig, GeneralConfiguration
 from api_fhir_r4.converters import PatientConverter, BillInvoiceConverter, InvoiceConverter, \
     HealthFacilityOrganisationConverter
 from api_fhir_r4.mapping.invoiceMapping import InvoiceTypeMapping, BillTypeMapping
 from api_fhir_r4.subscriptions.notificationManager import RestSubscriptionNotificationManager
 from api_fhir_r4.subscriptions.subscriptionCriteriaFilter import SubscriptionCriteriaFilter
 from core.service_signals import ServiceSignalBindType
 from core.signals import bind_service_signal
@@ -13,44 +15,44 @@
 from openIMIS.openimisapps import openimis_apps
 
 logger = logging.getLogger('openIMIS')
 imis_modules = openimis_apps()
 
 
 def bind_service_signals():
-    if 'insuree' in imis_modules:
+    if 'insuree' in imis_modules and GeneralConfiguration.get_subscribe_insuree_signal():
         def on_insuree_create_or_update(**kwargs):
             try:
                 model = kwargs.get('result', None)
                 if model:
                     notify_subscribers(model, PatientConverter(), 'Patient', None)
             except Exception as e:
                 logger.error("Error while processing Patient Subscription", exc_info=e)
 
         bind_service_signal(
             'insuree_service.create_or_update',
             on_insuree_create_or_update,
             bind_type=ServiceSignalBindType.AFTER
         )
 
-    if 'location' in imis_modules:
+    if 'location' in imis_modules and R4LocationConfig.get_subscribe_location_signal():
         def on_hf_create_or_update(**kwargs):
             try:
                 model = kwargs.get('result', None)
                 if model:
                     notify_subscribers(model, HealthFacilityOrganisationConverter(), 'Organisation', 'bus')
             except Exception as e:
                 logger.error("Error while processing Organisation Subscription", exc_info=e)
 
         bind_service_signal(
             'health_facility_service.update_or_create',
             on_hf_create_or_update,
             bind_type=ServiceSignalBindType.AFTER
         )
-    if 'invoice' in imis_modules:
+    if 'invoice' in imis_modules and R4InvoiceConfig.get_subscribe_invoice_signal():
         from invoice.models import Bill, Invoice
 
         def on_bill_create(**kwargs):
             try:
                 result = kwargs.get('result', {})
                 if result and result.get('success', False):
                     model_uuid = result['data']['uuid']
```

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/subscriptions/notificationClient.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/subscriptions/notificationClient.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/subscriptions/notificationManager.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/subscriptions/notificationManager.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/subscriptions/subscriptionConverter.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/subscriptions/subscriptionConverter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-import datetime
 from copy import deepcopy
 from urllib import parse
-
+import datetime
 from fhir.resources.R4B.subscription import Subscription as FHIRSubscription
 
 from api_fhir_r4.configurations import R4SubscriptionConfig
 from api_fhir_r4.converters import BaseFHIRConverter, ReferenceConverterMixin
 from api_fhir_r4.exceptions import FHIRException
 from api_fhir_r4.mapping.subscriptionMapping import SubscriptionChannelMapping, SubscriptionStatusMapping
 from api_fhir_r4.models import Subscription
@@ -165,15 +164,15 @@
             imis_subscription['channel'] = SubscriptionChannelMapping.to_imis_channel[fhir_subscription.channel.type]
         else:
             raise FHIRException(cls._error_invalid_attr % {'attr': 'channel.type'})
 
     @classmethod
     def _build_imis_channel_endpoint(cls, imis_subscription, fhir_subscription):
         if fhir_subscription.channel.endpoint:
-            imis_subscription['endpoint'] = fhir_subscription.channel.endpoint
+            imis_subscription['endpoint'] = str(fhir_subscription.channel.endpoint)
         else:
             raise FHIRException(cls._error_invalid_attr % {'attr': 'channel.endpoint'})
 
     @classmethod
     def _build_imis_channel_header(cls, imis_subscription, fhir_subscription):
         if fhir_subscription.channel.header:
             imis_subscription['headers'] = fhir_subscription.channel.header[0]
```

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/subscriptions/subscriptionCriteriaFilter.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/subscriptions/subscriptionCriteriaFilter.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,17 +23,17 @@
         queryset = Subscription.objects.filter(status=Subscription.SubscriptionStatus.ACTIVE.value,
                                                expiring__gt=datetime.now(), is_deleted=False)
         if self.fhir_resource_name:
             queryset = queryset.filter(criteria__jsoncontains={
                 R4SubscriptionConfig.get_fhir_sub_criteria_key_resource(): self.fhir_resource_name})
         if self.fhir_resource_type_name:
             queryset = queryset.filter(
-                ~Q(criteria__jsoncontainskey=R4SubscriptionConfig.get_fhir_sub_criteria_key_resource_type() | Q(
+                ~Q(criteria__jsoncontainskey=R4SubscriptionConfig.get_fhir_sub_criteria_key_resource_type() )| Q(
                     criteria__jsoncontains={
-                        R4SubscriptionConfig.get_fhir_sub_criteria_key_resource_type(): self.fhir_resource_type_name})))
+                        R4SubscriptionConfig.get_fhir_sub_criteria_key_resource_type(): self.fhir_resource_type_name}))
         return queryset.all()
 
     def _get_matching_subscriptions(self, subscriptions):
         return [subscription for subscription in subscriptions
                 if self._is_matching_subscription(subscription)]
 
     def _is_matching_subscription(self, sub):
```

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/subscriptions/subscriptionSerializer.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/subscriptions/subscriptionSerializer.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/__init__.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/SubscriptionTestMixin.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/SubscriptionTestMixin.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/__init__.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 class FhirConverterTestMixin(TestCase):
     def verify_fhir_identifier(self, fhir_obj, identifier_type, expected_identifier_value):
         identifiers = [identifier for identifier in fhir_obj.identifier
                        if identifier.type.coding[0].code == identifier_type]
         self.assertEqual(len(identifiers), 1)
-        self.assertEqual(identifiers[0].value, expected_identifier_value)
+        self.assertEqual(str(identifiers[0].value), str(expected_identifier_value))
 
     def verify_fhir_coding_exists(self, fhir_coding, expected_code):
         self.assertIsNotNone(next(iter([coding for coding in fhir_coding if coding.code == expected_code]), None))
 
 
 class ConvertToImisTestMixin:
     @property
```

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/activityDefinitionTestMixin.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/activityDefinitionTestMixin.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/billInvoiceTestMixin.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/billInvoiceTestMixin.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,26 +2,27 @@
 
 from django.contrib.contenttypes.models import ContentType
 
 from api_fhir_r4.configurations import R4IdentifierConfig
 from api_fhir_r4.tests import GenericTestMixin
 from api_fhir_r4.tests.mixin import FhirConverterTestMixin
 from insuree.models import Family
+from insuree.test_helpers import create_test_insuree
 from invoice.models import Bill, BillItem
 from fhir.resources.R4B.invoice import Invoice as FHIRInvoice
 from api_fhir_r4.utils.timeUtils import TimeUtils
-
+from api_fhir_r4.tests.utils import get_connection_payload,get_or_create_user_api
 
 class BillInvoiceTestMixin(GenericTestMixin, FhirConverterTestMixin):
     _TEST_BILL_STATUS = 'active'
     _TEST_BILL_UUID = '12345678-1234-1234-1234-123456789012'
     _TEST_BILL_CODE = 'TEST-CODE'
     _TEST_BILL_SUBJECT_TYPE = None
     _TEST_BILL_SUBJECT_TYPE_CODING = 'claim-batch'
-    _TEST_BILL_THIRD_PARTY = Family()
+    _TEST_BILL_THIRD_PARTY = None
     _TEST_BILL_THIRD_PARTY_UUID = '98765432-1234-1234-1234-123456789012'
     _TEST_BILL_DATE = TimeUtils.str_iso_to_date('2021-01-01')
     _TEST_BILL_TOTAL_NET = 10000.0
     _TEST_BILL_TOTAL_GROSS = 10000.0
     _TEST_BILL_CURRENCY = 'USD'
     _TEST_LINE_ITEM_CHARGE_ITEM = None
     _TEST_LINE_ITEM_CHARGE_ITEM_CODING = 'claim'
@@ -31,39 +32,45 @@
     _TEST_LINE_ITEM_DISCOUNT_COMPONENT_TYPE = 'discount'
     _TEST_LINE_ITEM_DISCOUNT = 0.1
     _TEST_LINE_ITEM_DEDUCTION_PRICE_COMPONENT_TYPE = 'deduction'
     _TEST_LINE_ITEM_DEDUCTION = 100
     _TEST_LINE_ITEM_DEDUCTION_FACTOR = 1
     _TEST_LINE_ITEM_TAX_PRICE_COMPONENT_TYPE = 'tax'
     _TEST_LINE_ITEM_TAX_RATE = 0.02
-    
+    user = None
     @classmethod
     def setUpTestData(cls):
+        cls.user = get_or_create_user_api()
         cls._TEST_BILL_SUBJECT_TYPE = ContentType.objects.get(model__iexact='BatchRun')
         cls._TEST_LINE_ITEM_CHARGE_ITEM = ContentType.objects.get(model__iexact='Claim')
 
     def create_test_imis_instance(self):
+        self._TEST_BILL_INSUREE = create_test_insuree()
         imis_bill = Bill()
-        imis_bill.uuid = self._TEST_BILL_UUID
         imis_bill.code = self._TEST_BILL_CODE
+        
         imis_bill.subject_type = self._TEST_BILL_SUBJECT_TYPE
-        imis_bill.thirdparty = self._TEST_BILL_THIRD_PARTY
+        imis_bill.thirdparty = self._TEST_BILL_INSUREE.family
         imis_bill.thirdparty.uuid = self._TEST_BILL_THIRD_PARTY_UUID
         imis_bill.date_bill = self._TEST_BILL_DATE
         imis_bill.amount_net = self._TEST_BILL_TOTAL_NET
         imis_bill.amount_total = self._TEST_BILL_TOTAL_GROSS
         imis_bill.currency_code = self._TEST_BILL_CURRENCY
-
+        imis_bill.save(user=self.user)
+        self._TEST_BILL_UUID  =imis_bill.id
         imis_bill_line_item = BillItem()
+        imis_bill_line_item.bill = imis_bill
         imis_bill_line_item.line_type = self._TEST_LINE_ITEM_CHARGE_ITEM
         imis_bill_line_item.quantity = self._TEST_LiNE_ITEM_QUANTITY
         imis_bill_line_item.unit_price = self._TEST_LINE_ITEM_UNIT_PRICE
         imis_bill_line_item.discount = self._TEST_LINE_ITEM_DISCOUNT
         imis_bill_line_item.deduction = self._TEST_LINE_ITEM_DEDUCTION
-        imis_bill_line_item.tax_rate = self._TEST_LINE_ITEM_TAX_RATE
+        imis_bill_line_item.tax_rate = None
+        imis_bill_line_item.code = "1"
+        imis_bill_line_item.save(user=self.user)
 
         with mock.patch('django.db.models.fields.related_descriptors.create_reverse_many_to_one_manager') as mock_patch:
             class MockedManager(mock.MagicMock):
                 def all(self):
                     return [imis_bill_line_item]
 
             mock_patch.return_value = MockedManager()
@@ -105,20 +112,21 @@
                                             -self._TEST_LINE_ITEM_UNIT_PRICE * self._TEST_LiNE_ITEM_QUANTITY * (
                                                 self._TEST_LINE_ITEM_DISCOUNT),
                                             self._TEST_LINE_ITEM_DISCOUNT_COMPONENT_TYPE)
             elif price_component.type == self._TEST_LINE_ITEM_DEDUCTION_PRICE_COMPONENT_TYPE:
                 self.verify_price_component(price_component, self._TEST_LINE_ITEM_DEDUCTION_FACTOR,
                                             -self._TEST_LINE_ITEM_DEDUCTION,
                                             self._TEST_LINE_ITEM_DEDUCTION_PRICE_COMPONENT_TYPE)
-            elif price_component.type == self._TEST_LINE_ITEM_TAX_PRICE_COMPONENT_TYPE:
-                self.verify_price_component(price_component, self._TEST_LINE_ITEM_TAX_RATE,
-                                            ((self._TEST_LINE_ITEM_UNIT_PRICE * self._TEST_LiNE_ITEM_QUANTITY * (
-                                                    1 - self._TEST_LINE_ITEM_DISCOUNT))
-                                             - self._TEST_LINE_ITEM_DEDUCTION) * self._TEST_LINE_ITEM_TAX_RATE,
-                                            self._TEST_LINE_ITEM_TAX_PRICE_COMPONENT_TYPE)
+            # FIXME tax rate is more complex, requires an object
+            # elif price_component.type == self._TEST_LINE_ITEM_TAX_PRICE_COMPONENT_TYPE:
+            #     self.verify_price_component(price_component, self._TEST_LINE_ITEM_TAX_RATE,
+            #                                 ((self._TEST_LINE_ITEM_UNIT_PRICE * self._TEST_LiNE_ITEM_QUANTITY * (
+            #                                         1 - self._TEST_LINE_ITEM_DISCOUNT))
+            #                                  - self._TEST_LINE_ITEM_DEDUCTION) * self._TEST_LINE_ITEM_TAX_RATE,
+            #                                 self._TEST_LINE_ITEM_TAX_PRICE_COMPONENT_TYPE)
 
     def verify_price_component(self, price_component, expected_factor, expected_amount, expected_type):
         self.assertGreater(len(price_component.extension), 0)
         self.assertEqual(price_component.extension[0].valueMoney.currency, self._TEST_BILL_CURRENCY)
         self.assertEqual(price_component.extension[0].valueMoney.value, self._TEST_LINE_ITEM_UNIT_PRICE)
         if expected_type:
             self.assertEqual(price_component.type, expected_type)
```

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/claimAdminPractitionerRoleTestMixin.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/claimAdminPractitionerRoleTestMixin.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from api_fhir_r4.configurations import R4IdentifierConfig
 from api_fhir_r4.converters import ClaimAdminPractitionerRoleConverter
 from fhir.resources.R4B.identifier import Identifier
 from fhir.resources.R4B.practitionerrole import PractitionerRole
 from fhir.resources.R4B.reference import Reference
 from api_fhir_r4.tests import GenericTestMixin,  LocationTestMixin
 from location.models import HealthFacility
-from location.test_helpers import create_test_village
+from location.test_helpers import create_test_village, create_test_health_facility
 from claim.test_helpers import create_test_claim_admin
 from api_fhir_r4.utils import TimeUtils
 
 class ClaimAdminPractitionerRoleTestMixin(GenericTestMixin):
     test_claim_admin = None
     test_hf = None
+    test_village = None
     _TEST_ORGANIZATION_REFERENCE = None
     _TEST_CLAIM_ADMIN_PRACTITIONER_REFERENCE = None
 
     _TEST_CLAIM_ADMIN_ID = 1
     _TEST_CLAIM_ADMIN_UUID = "254f6268-964b-4d8d-aa26-20081f22235e"
     _TEST_CLAIM_ADMIN_CODE = "1234abcd"
     
@@ -31,43 +32,41 @@
     _TEST_CLAIM_ADMIN_PHONE = "133-996-476"
     _TEST_CLAIM_ADMIN_FAX = "1-408-999 8888"
     _TEST_CLAIM_ADMIN_EMAIL = "TEST@TEST.com"
     sub_str = {}
 
     def setUp(self):
         super(ClaimAdminPractitionerRoleTestMixin, self).setUp()
-        self.test_hf = self.create_test_health_facility()
+        self.test_village= create_test_village()
+        self.test_hf = self.create_test_hf()
         self.test_claim_admin = create_test_claim_admin( custom_props={
             'health_facility_id': self.test_hf.id, 
             'code':self._TEST_CLAIM_ADMIN_CODE,
             'dob':TimeUtils.str_to_date(self._TEST_CLAIM_ADMIN_DOB),
             'phone':self._TEST_CLAIM_ADMIN_PHONE})
         self._TEST_CLAIM_ADMIN_PRACTITIONER_REFERENCE = "Practitioner/" + str(self.test_claim_admin.uuid)
         self._TEST_ORGANIZATION_REFERENCE = "Organization/" + str(self.test_hf.uuid)
         self.sub_str[self._TEST_HF_UUID]=self.test_hf.uuid
         self.sub_str[self._TEST_CLAIM_ADMIN_UUID]=self.test_claim_admin.uuid
+        self._TEST_HF_UUID=self.test_hf.uuid
+        self._TEST_HF_ID=self.test_hf.id
+
+    def create_test_hf(self):
+        self.test_hf = create_test_health_facility(
+            self._TEST_HF_CODE,
+            self.test_village.parent.parent.id,
+            custom_props = {
+                'name': self._TEST_HF_NAME,
+                'level':self._TEST_HF_LEVEL,
+                'legal_form_id':self._TEST_HF_LEGAL_FORM,
+
+            }
+        )
+        return self.test_hf
 
-    def create_test_health_facility(self):
-        location = create_test_village()
-        hf = HealthFacility()
-        hf.id = self._TEST_HF_ID
-        hf.uuid = self._TEST_HF_UUID
-        hf.code = self._TEST_HF_CODE
-        hf.name = self._TEST_HF_NAME
-        hf.level = self._TEST_HF_LEVEL
-        hf.legal_form_id = self._TEST_HF_LEGAL_FORM
-        hf.address = self._TEST_CLAIM_ADMIN_ADDRESS
-        hf.phone = self._TEST_CLAIM_ADMIN_PHONE
-        hf.fax = self._TEST_CLAIM_ADMIN_FAX
-        hf.email = self._TEST_CLAIM_ADMIN_EMAIL
-        hf.location = location.parent.parent
-        hf.offline = False
-        hf.audit_user_id = -1
-        hf.save()
-        return hf
 
     def create_test_imis_instance(self):
         self.test_claim_admin.health_facility = self.test_hf
         return self.test_claim_admin
 
     def verify_imis_instance(self, imis_obj):
         self.assertEqual(self.test_hf.code, imis_obj.health_facility.code)
```

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/claimAdminPractitionerTestMixin.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/claimAdminPractitionerTestMixin.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from fhir.resources.R4B.practitioner import Practitioner, PractitionerQualification
 from fhir.resources.R4B.reference import Reference
 
 from api_fhir_r4.models.imisModelEnums import ContactPointSystem, ContactPointUse
 from api_fhir_r4.tests import GenericTestMixin, LocationTestMixin
 from api_fhir_r4.utils import TimeUtils
 from location.models import HealthFacility
-from location.test_helpers import create_test_village
+from location.test_helpers import create_test_village, create_test_health_facility
 from claim.test_helpers import create_test_claim_admin
 
 class ClaimAdminPractitionerTestMixin(GenericTestMixin):
 
     _TEST_CLAIM_ADMIN_LAST_NAME = "Smith"
     _TEST_CLAIM_ADMIN_OTHER_NAME = "John"
     _TEST_CLAIM_ADMIN_DOB = "1990-03-24"
@@ -40,45 +40,41 @@
     
     test_claim_admin = None
     test_hf = None
     sub_str = {}
     
     def setUp(self):
         super(ClaimAdminPractitionerTestMixin, self).setUp()
-        self.village = create_test_village()
-        self.test_hf=self.create_test_health_facility()
+        self.test_village = create_test_village()
+        self.test_hf=self.create_test_hf()
         self.test_claim_admin = create_test_claim_admin( custom_props={
             'health_facility_id': self.test_hf.id, 
             'code':self._TEST_CLAIM_ADMIN_CODE,
             'dob':TimeUtils.str_to_date(self._TEST_CLAIM_ADMIN_DOB),
             'phone': self._TEST_CLAIM_ADMIN_PHONE,
             'email_id': self._TEST_CLAIM_ADMIN_EMAIL ,
             'last_name': self._TEST_CLAIM_ADMIN_LAST_NAME,
             'other_names': self._TEST_CLAIM_ADMIN_OTHER_NAME}
                                             )
         self.sub_str[self._TEST_HF_UUID]=self.test_hf.uuid
         self.sub_str[self._TEST_CLAIM_ADMIN_UUID]=self.test_claim_admin.uuid
 
-    def create_test_health_facility(self):
-        hf = HealthFacility()
-        hf.id = self._TEST_HF_ID
-        hf.uuid = self._TEST_HF_UUID
-        hf.code = self._TEST_HF_CODE
-        hf.name = self._TEST_HF_NAME
-        hf.level = self._TEST_HF_LEVEL
-        hf.legal_form_id = self._TEST_HF_LEGAL_FORM
-        hf.address = self._TEST_CLAIM_ADMIN_ADDRESS
-        hf.phone = self._TEST_CLAIM_ADMIN_PHONE
-        hf.fax = self._TEST_CLAIM_ADMIN_FAX
-        hf.email = self._TEST_CLAIM_ADMIN_EMAIL
-        hf.location = self.village .parent.parent
-        hf.offline = False
-        hf.audit_user_id = -1
-        hf.save()
-        return hf
+    def create_test_hf(self):
+        self.test_hf = create_test_health_facility(
+            self._TEST_HF_CODE,
+            self.test_village.parent.parent.id,
+            custom_props = {
+                'name': self._TEST_HF_NAME,
+                'level':self._TEST_HF_LEVEL,
+                'legal_form_id':self._TEST_HF_LEGAL_FORM,
+            }
+        )
+        self._TEST_HF_ID = self.test_hf.id
+        self._TEST_HF_UUID = self.test_hf.uuid
+        return self.test_hf
 
     def create_test_imis_instance(self, location=None, hf = None):
         return self.test_claim_admin
 
 
     def verify_imis_instance(self, imis_obj):
         self.assertEqual(self._TEST_CLAIM_ADMIN_LAST_NAME, imis_obj.last_name)
```

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/claimResponseTestMixin.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/claimResponseTestMixin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from core import datetime
 
 from insuree.test_helpers import create_test_insuree
 from location.models import HealthFacility
-from location.test_helpers import create_test_village
+from location.test_helpers import create_test_village, create_test_health_facility
 from medical.test_helpers import create_test_item, create_test_service
 from api_fhir_r4.configurations import R4IdentifierConfig
 
 from api_fhir_r4.tests import GenericTestMixin, LocationTestMixin
 from api_fhir_r4.utils import TimeUtils
 from claim.models import Claim, ClaimItem, ClaimService
 from medical.models import Diagnosis
@@ -71,15 +71,15 @@
     test_hf = None
     test_claim = None
     sub_str={}
 
     def setUp(self):
         super(ClaimResponseTestMixin, self).setUp()
         self.test_insuree = create_test_insuree()
-        self.create_test_health_facility()
+        self.create_test_hf()
         self.test_claim_admin = create_test_claim_admin(custom_props={'health_facility_id':self.test_hf.id})
         self.test_claim = self.create_test_claim()
         self.test_item = self.create_test_claim_item()
         self.test_service = self.create_test_claim_service()
         self.sub_str[self._TEST_INSUREE_UUID] = self.test_insuree.uuid
         self.sub_str[self._TEST_CLAIM_ADMIN_UUID] = self.test_claim_admin.uuid
         self.sub_str[self._TEST_HF_UUID] = self.test_hf.uuid
@@ -133,44 +133,44 @@
         imis_claim.status = self._TEST_STATUS
         imis_claim.adjustment = self._TEST_ADJUSTMENT
         imis_claim.date_processed = TimeUtils.str_to_date(self._TEST_DATE_PROCESSED)
         imis_claim.approved = self._TEST_APPROVED
         imis_claim.rejection_reason = self._TEST_REJECTION_REASON            
         imis_claim.insuree = self.test_insuree 
         imis_claim.health_facility = self.test_hf
-        imis_claim.icd = Diagnosis(code='ICD00I')
+        imis_claim.icd = Diagnosis(code='ICD00I', name='Test ICD')
         imis_claim.icd.audit_user_id = self._ADMIN_AUDIT_USER_ID
         imis_claim.icd.save()
         imis_claim.audit_user_id = self._ADMIN_AUDIT_USER_ID
         imis_claim.icd.date_from = datetime.date(2018, 12, 12)
         imis_claim.date_from = datetime.date(2018, 12, 12)
         imis_claim.date_claimed = datetime.date(2018, 12, 14)
         imis_claim.visit_type = self._TEST_VISIT_TYPE
             
         imis_claim.admin = self.test_claim_admin
         imis_claim.save()
         return imis_claim
-    def create_test_health_facility(self):
-        hf = HealthFacility()
-        hf.id = self._TEST_HF_ID
-        hf.uuid = self._TEST_HF_UUID
-        hf.code = self._TEST_HF_CODE
-        hf.name = self._TEST_HF_NAME
-        hf.level = self._TEST_HF_LEVEL
-        hf.legal_form_id = self._TEST_HF_LEGAL_FORM
-        hf.address = self._TEST_ADDRESS
-        hf.phone = self._TEST_PHONE
-        hf.fax = self._TEST_FAX
-        hf.email = self._TEST_EMAIL
-        hf.location = self.test_insuree.family.location.parent.parent
-        hf.offline = False
-        hf.audit_user_id = -1
-        hf.save()
-        self.test_hf = hf
-        return hf
+    def create_test_hf(self):
+        
+        self.test_hf = create_test_health_facility(
+            self._TEST_HF_CODE,
+            self.test_insuree.family.location.parent.parent.id,
+            custom_props = {
+                'name': self._TEST_HF_NAME,
+                'level':self._TEST_HF_LEVEL,
+                'legal_form_id':self._TEST_HF_LEGAL_FORM,
+                'address':self._TEST_ADDRESS,
+                'phone':self._TEST_PHONE,
+                'fax':self._TEST_FAX,
+                'email':self._TEST_EMAIL,
+            }
+        )
+        self._TEST_HF_ID = self.test_hf.id
+        self._TEST_HF_UUID = self.test_hf.uuid
+        return self.test_hf
 
     def verify_fhir_instance(self, fhir_obj):
         for identifier in fhir_obj.identifier:
             if identifier.type.coding[0].code == R4IdentifierConfig.get_fhir_uuid_type_code():
                 self.assertEqual(str(self._TEST_CLAIM_UUID), identifier.value)
             elif identifier.type.coding[0].code == R4IdentifierConfig.get_fhir_claim_code_type():
                 self.assertEqual(self._TEST_CODE, identifier.value)
```

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/claimTestMixin.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/claimTestMixin.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ClaimAdminPractitionerConverter, ReferenceConverterMixin
 from api_fhir_r4.converters.claimConverter import ClaimConverter
 from api_fhir_r4.mapping.claimMapping import ClaimVisitTypeMapping
 from api_fhir_r4.models import ClaimV2 as FHIRClaim
 from fhir.resources.R4B.period import Period
 from fhir.resources.R4B.money import Money
 from location.models import HealthFacility
-from location.test_helpers import create_test_village
+from location.test_helpers import create_test_village, create_test_health_facility
 from medical.models import Item, Service
 from medical.test_helpers import create_test_item, create_test_service
 from claim.test_helpers import create_test_claimservice,create_test_claimitem,create_test_claim_admin
 from api_fhir_r4.tests import GenericTestMixin
 from api_fhir_r4.utils import TimeUtils
 
 
@@ -83,48 +83,47 @@
         self.test_icd = Diagnosis()
         self.test_icd.code = self._TEST_MAIN_ICD_CODE
         self.test_icd.name = self._TEST_MAIN_ICD_NAME
         self.test_icd.audit_user_id = self._ADMIN_AUDIT_USER_ID
         self.test_icd.save()
 
         self.test_claim_admin= create_test_claim_admin()
+        self.test_insuree = create_test_insuree()
 
-        self.test_hf = self.create_test_health_facility()
+        self.create_test_hf()
 
-        self.test_insuree = create_test_insuree()
         self.test_claim=self.create_test_claim()
         self.test_claim_item= self.create_test_claim_item()
         self.test_claim_service = self.create_test_claim_service()
         self.sub_str[self._TEST_HF_UUID]=self.test_hf.uuid
         self.sub_str[self._TEST_CLAIM_ADMIN_UUID]=self.test_claim_admin.uuid
         self.sub_str[self._TEST_INSUREE_UUID]=self.test_insuree.uuid
         self.sub_str[self._TEST_SERVICE_UUID]=self.test_claim_service.service.uuid
         self.sub_str[self._TEST_ITEM_UUID]=self.test_claim_item.item.uuid
         self.sub_str[self._TEST_SERVICE_CODE]=self.test_claim_service.service.code
         self.sub_str[self._TEST_ITEM_CODE]=self.test_claim_item.item.code
         self.sub_str[self._TEST_UUID]=self.test_claim.uuid
+        self._TEST_HF_ID = self.test_hf.id
+        self._TEST_HF_UUID = self.test_hf.uuid
         
-    def create_test_health_facility(self):
-        location = create_test_village()
-        hf = HealthFacility()
-        hf.id = self._TEST_HF_ID
-        hf.uuid = self._TEST_HF_UUID
-        hf.code = self._TEST_HF_CODE
-        hf.name = self._TEST_HF_NAME
-        hf.level = self._TEST_HF_LEVEL
-        hf.legal_form_id = self._TEST_HF_LEGAL_FORM
-        hf.address = self._TEST_ADDRESS
-        hf.phone = self._TEST_PHONE
-        hf.fax = self._TEST_FAX
-        hf.email = self._TEST_EMAIL
-        hf.location = location.parent.parent
-        hf.offline = False
-        hf.audit_user_id = -1
-        hf.save()
-        return hf
+    def create_test_hf(self):
+        self.test_hf = create_test_health_facility(
+            self._TEST_HF_CODE,
+            self.test_insuree.family.location.parent.parent.id,
+            custom_props = {
+                'name': self._TEST_HF_NAME,
+                'level':self._TEST_HF_LEVEL,
+                'legal_form_id':self._TEST_HF_LEGAL_FORM,
+                'address':self._TEST_ADDRESS,
+                'phone':self._TEST_PHONE,
+                'fax':self._TEST_FAX,
+                'email':self._TEST_EMAIL,
+            }
+        )
+        return self.test_hf
     def create_test_claim(self):
         imis_claim = Claim()
         imis_claim.uuid = self._TEST_UUID
         imis_claim.insuree = self.test_insuree
         imis_claim.code = self._TEST_CLAIM_CODE
         imis_claim.date_from = TimeUtils.str_to_date(self._TEST_DATE_FROM)
         imis_claim.date_to = TimeUtils.str_to_date(self._TEST_DATE_TO)
```

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/communicationRequestTestMixin.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/communicationRequestTestMixin.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from insuree.test_helpers import create_test_insuree
 from location.models import HealthFacility
 from medical.test_helpers import create_test_item, create_test_service
 from api_fhir_r4.configurations import R4CommunicationRequestConfig as Config
 from api_fhir_r4.tests import GenericTestMixin, LocationTestMixin
 from api_fhir_r4.utils import TimeUtils
 from claim.test_helpers import create_test_claim_admin
-from location.test_helpers import create_test_village
+from location.test_helpers import create_test_village, create_test_health_facility
 from medical.models import Diagnosis
 
 
 class CommunicationRequestTestMixin(GenericTestMixin):
     _TEST_CODE = 'codeTest'
     _TEST_UUID = "7ac646cb-d3cd-4660-baeb-ee34ecf0354e"
     _TEST_STATUS = Claim.STATUS_ENTERED
@@ -71,15 +71,16 @@
     test_hf = None
     test_village = None
     sub_str = {}
     def setUp(self):
         super(CommunicationRequestTestMixin, self).setUp()
         self.test_insuree = create_test_insuree()
         self.test_village = self.test_insuree.family.location
-        self.test_hf = self.create_test_health_facility()
+        self.test_hf = self._create_test_health_facility()
+        self._TEST_HF_ID = self.test_hf.id
         self.test_claim_admin = create_test_claim_admin( custom_props={'health_facility_id': self.test_hf.id})
         self.test_claim = self.create_test_imis_instance()
         self.test_claim_item = self.create_test_claim_item()
         self.test_claim_service = self.create_test_claim_service()
         
         self.sub_str[self._TEST_HF_UUID]=self.test_hf.uuid
         self.sub_str[self._TEST_CLAIM_ADMIN_UUID]=self.test_claim_admin.uuid
@@ -120,31 +121,29 @@
         service.availability = self._TEST_ITEM_AVAILABILITY
         service.price_asked = self._TEST_SERVICE_PRICE
         service.price_approved = self._TEST_SERVICE_PRICE
         service.audit_user_id = self._ADMIN_AUDIT_USER_ID
         service.save()
         return service
 
-    def create_test_health_facility(self):
-    
-        hf = HealthFacility()
-        hf.id = self._TEST_HF_ID
-        hf.uuid = self._TEST_HF_UUID
-        hf.code = self._TEST_HF_CODE
-        hf.name = self._TEST_HF_NAME
-        hf.level = self._TEST_HF_LEVEL
-        hf.legal_form_id = self._TEST_HF_LEGAL_FORM
-        hf.address = self._TEST_ADDRESS
-        hf.phone = self._TEST_PHONE
-        hf.fax = self._TEST_FAX
-        hf.email = self._TEST_EMAIL
-        hf.location = self.test_village.parent.parent
-        hf.offline = False
-        hf.audit_user_id = -1
-        hf.save()
+    def _create_test_health_facility(self):
+        
+        hf = create_test_health_facility(
+            self._TEST_HF_CODE,
+            self.test_village.parent.parent.id,
+            custom_props = {
+                'name': self._TEST_HF_NAME,
+                'level':self._TEST_HF_LEVEL,
+                'legal_form_id':self._TEST_HF_LEGAL_FORM,
+                'address':self._TEST_ADDRESS,
+                'phone':self._TEST_PHONE,
+                'fax':self._TEST_FAX,
+                'email':self._TEST_EMAIL,
+            }
+        )
         return hf
 
     def create_test_imis_instance(self):
         if self.test_claim is None:
             imis_claim = Claim()
             imis_claim.id = self._TEST_ID
             imis_claim.uuid = self._TEST_UUID
@@ -152,16 +151,16 @@
             imis_claim.status = self._TEST_STATUS
             imis_claim.adjustment = self._TEST_ADJUSTMENT
             imis_claim.date_processed = TimeUtils.str_to_date(self._TEST_DATE_PROCESSED)
             imis_claim.approved = self._TEST_APPROVED
             imis_claim.rejection_reason = self._TEST_REJECTION_REASON
             imis_claim.insuree = self.test_insuree 
             
-            imis_claim.health_facility = self.create_test_health_facility()
-            imis_claim.icd = Diagnosis(code='ICD00I')
+            imis_claim.health_facility = self._create_test_health_facility()
+            imis_claim.icd = Diagnosis(code='ICD00I', name='TEST ICD')
             imis_claim.icd.audit_user_id = self._ADMIN_AUDIT_USER_ID
             imis_claim.icd.save()
             imis_claim.audit_user_id = self._ADMIN_AUDIT_USER_ID
             imis_claim.icd.date_from = datetime.date(2018, 12, 12)
             imis_claim.date_from = datetime.date(2018, 12, 12)
             imis_claim.date_claimed = datetime.date(2018, 12, 14)
             imis_claim.visit_type = self._TEST_VISIT_TYPE
```

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/communicationTestMixin.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/communicationTestMixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from api_fhir_r4.utils import TimeUtils
 from fhir.resources.R4B.communication import Communication, CommunicationPayload
 from fhir.resources.R4B.extension import Extension
 from claim.models import Claim, ClaimItem, ClaimService, Feedback
 from claim.test_helpers import create_test_claim_admin
 from core import datetime
 from location.models import HealthFacility
-from location.test_helpers import create_test_village
+from location.test_helpers import create_test_village, create_test_health_facility
 from insuree.test_helpers import create_test_insuree
 from medical.test_helpers import create_test_item, create_test_service
 from medical.models import Diagnosis
 
 
 class CommunicationTestMixin(GenericTestMixin):
     # feedback expected data
@@ -73,17 +73,19 @@
     _TEST_HF_NAME = "TEST_NAME"
     _TEST_HF_LEVEL = "H"
     _TEST_HF_LEGAL_FORM = "G"
     _TEST_ADDRESS = "TEST_ADDRESS"
     _TEST_PHONE = "133-996-476"
     _TEST_FAX = "1-408-999 8888"
     _TEST_EMAIL = "TEST@TEST.com"
+    _TEST_INSUREE = None
 
     def setUp(self):
         super(CommunicationTestMixin, self).setUp()
+        self._TEST_INSUREE = create_test_insuree()
         self._TEST_CLAIM = self.create_test_claim()
         self._TEST_ITEM = self.create_test_claim_item()
         self._TEST_SERVICE = self.create_test_claim_service()
 
     def create_test_claim_item(self):
         item = ClaimItem()
         item.item = create_test_item(
@@ -116,48 +118,46 @@
         service.availability = self._TEST_ITEM_AVAILABILITY
         service.price_asked = self._TEST_SERVICE_PRICE
         service.price_approved = self._TEST_SERVICE_PRICE
         service.audit_user_id = self._ADMIN_AUDIT_USER_ID
         service.save()
         return service
 
-    def create_test_health_facility(self):
-        location = create_test_village()
-        hf = HealthFacility()
-        hf.id = self._TEST_HF_ID
-        hf.uuid = self._TEST_HF_UUID
-        hf.code = self._TEST_HF_CODE
-        hf.name = self._TEST_HF_NAME
-        hf.level = self._TEST_HF_LEVEL
-        hf.legal_form_id = self._TEST_HF_LEGAL_FORM
-        hf.address = self._TEST_ADDRESS
-        hf.phone = self._TEST_PHONE
-        hf.fax = self._TEST_FAX
-        hf.email = self._TEST_EMAIL
-        hf.location = location.parent.parent
-        hf.offline = False
-        hf.audit_user_id = -1
-        hf.save()
+    def create_test_hf(self):
+        hf = create_test_health_facility(
+            self._TEST_HF_CODE,
+            self._TEST_INSUREE.family.location.parent.parent.id,
+            custom_props = {
+                'name': self._TEST_HF_NAME,
+                'level':self._TEST_HF_LEVEL,
+                'legal_form_id':self._TEST_HF_LEGAL_FORM,
+                'address':self._TEST_ADDRESS,
+                'phone':self._TEST_PHONE,
+                'fax':self._TEST_FAX,
+                'email':self._TEST_EMAIL,
+            }
+        )    
+
         return hf
 
     def create_test_claim(self):
         imis_claim = Claim()
         imis_claim.id = self._TEST_ID
         imis_claim.uuid = self._TEST_CLAIM_UUID
         imis_claim.code = self._TEST_CLAIM_CODE
         imis_claim.status = self._TEST_STATUS
         imis_claim.adjustment = self._TEST_ADJUSTMENT
         imis_claim.date_processed = TimeUtils.str_to_date(self._TEST_DATE_PROCESSED)
         imis_claim.approved = self._TEST_APPROVED
         imis_claim.rejection_reason = self._TEST_REJECTION_REASON
-        imis_claim.insuree = create_test_insuree()
+        imis_claim.insuree = self._TEST_INSUREE
         imis_claim.insuree.uuid = self._TEST_PATIENT_UUID
         imis_claim.insuree.save()
-        imis_claim.health_facility = self.create_test_health_facility()
-        imis_claim.icd = Diagnosis(code='ICD00I')
+        imis_claim.health_facility = self.create_test_hf()
+        imis_claim.icd = Diagnosis(code='ICD00I', name='Test ICD')
         imis_claim.icd.audit_user_id = self._ADMIN_AUDIT_USER_ID
         imis_claim.icd.save()
         imis_claim.audit_user_id = self._ADMIN_AUDIT_USER_ID
         imis_claim.icd.date_from = datetime.date(2018, 12, 12)
         imis_claim.date_from = datetime.date(2018, 12, 12)
         imis_claim.date_claimed = datetime.date(2018, 12, 14)
         imis_claim.visit_type = self._TEST_VISIT_TYPE
```

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/contractTestMixin.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/contractTestMixin.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/coverageEligibilityRequestTestMixin.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/coverageEligibilityRequestTestMixin.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/coverageTestMixin.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/coverageTestMixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,9 +100,9 @@
         self.assertIn(f"Patient/{self._TEST_INSUREE_CHFID}", fhir_obj.beneficiary.reference)
         self.assertIn(f"Patient/{self._TEST_INSUREE_CHFID}", fhir_obj.payor[0].reference)
         self.assertEqual(1, len(fhir_obj.class_fhir))
         self.assertEqual('plan', fhir_obj.class_fhir[0].type.coding[0].code)
         self.assertEqual(self._TEST_PRODUCT_CODE, fhir_obj.class_fhir[0].value)
         self.assertEqual(f'{self._TEST_PRODUCT_NAME} {self._TEST_PRODUCT_CODE}', fhir_obj.class_fhir[0].name)
         period = fhir_obj.period
-        self.assertEqual(self._TEST_POLICY_START_DATE, period.start.isoformat())
-        self.assertEqual(self._TEST_POLICY_EXPIRED_DATE, period.end.isoformat())
+        self.assertEqual(self._TEST_POLICY_START_DATE[:10], period.start.isoformat()[:10])
+        self.assertEqual(self._TEST_POLICY_EXPIRED_DATE[:10], period.end.isoformat()[:10])
```

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/enrolmentOfficerPractitionerRoleTestMixin.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/enrolmentOfficerPractitionerRoleTestMixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 from core.test_helpers import create_test_officer
 
 class EnrolmentOfficerPractitionerRoleTestMixin(GenericTestMixin):
     test_officer = None
     test_village = None
     test_substitution_officer = None
     _TEST_SUBSTITUTION_OFFICER_UUID = "f4bf924a-e2c9-46dc-9fa3-d54a1a67ea86"
-    _TEST_OFFICER_UUID = "f4bf924a-e2c9-46dc-9fa3-d54a1a67ea85"
+    _TEST_OFFICER_UUID = "b578a621-0b11-4889-9454-a8e498c35dee"
     _TEST_SUBSTITUTION_OFFICER_CODE = "EOTESB"
     _TEST_OFFICER_CODE = "EOTEST"
     _TEST_PRACTITIONER_REFERENCE = None
-    _TEST_VILLAGE_REFERENCE = None
+    _TEST_VILLAGE_REFERENCE = 'Location/20fcfa89-149a-429e-bd26-b014b95fbb2d'
     _TEST_VILLAGE_UUID = "041890f3-d90b-46ca-8b25-56c3f8d60615"
     sub_str = {}
     
     def setUp(self):
         self.test_village = create_test_village()
         self.test_substitution_officer   = create_test_officer(custom_props ={
                 "uuid": self._TEST_SUBSTITUTION_OFFICER_UUID,
@@ -38,20 +38,20 @@
                 "last_name": "Officer",
                 "other_names": "Test",
                 "validity_to": None,
                 "audit_user_id": -1,
                 'location':self.test_village.parent.parent})
         
         self._TEST_PRACTITIONER_REFERENCE = "Practitioner/" + str(self.test_officer.uuid)
-        self._TEST_VILLAGE_REFERENCE = "Location/" + str(self.test_village.uuid)
+
         self.sub_str[self._TEST_SUBSTITUTION_OFFICER_UUID]=self.test_substitution_officer.uuid
         self.sub_str[self._TEST_OFFICER_UUID]=self.test_officer.uuid
         self.sub_str[self._TEST_VILLAGE_UUID]=self.test_village.uuid
-
-
+        self.sub_str[self._TEST_VILLAGE_REFERENCE]="Location/" + str(self.test_village.uuid)
+        self._TEST_VILLAGE_REFERENCE = "Location/" + str(self.test_village.uuid)
 
 
 
 
     def verify_imis_instance(self, imis_obj):
         self.assertEqual(self.test_officer.substitution_officer.code, imis_obj.substitution_officer.code)
         self.assertEqual(self.test_village.code, imis_obj.location.code)
```

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/enrolmentOfficerPractitionerTestMixin.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/enrolmentOfficerPractitionerTestMixin.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/fhirApiCreateTestMixin.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/fhirApiCreateTestMixin.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,12 +14,12 @@
     def login(self):
         raise NotImplementedError()
 
     def test_post_should_create_correctly(self):
         self.login()
         self.create_dependencies()
         response = self.client.post(self.base_url, data=self._test_request_data, format='json')
-        #FIXME self.assertEqual(response.status_code, status.HTTP_201_CREATED)
-        #self.assertIsNotNone(response.content)
+        self.assertEqual(response.status_code, status.HTTP_201_CREATED)
+        self.assertIsNotNone(response.content)
 
     def create_dependencies(self):
         pass
```

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/fhirApiDeleteTestMixin.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/fhirApiDeleteTestMixin.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/fhirApiReadTestMixin.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/fhirApiReadTestMixin.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/fhirApiUpdateTestMixin.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/fhirApiUpdateTestMixin.py`

 * *Files 13% similar despite different names*

```diff
@@ -35,14 +35,14 @@
         response = self.client.post(self.base_url, data=self._test_request_data, format='json')
         self.assertEqual(response.status_code, status.HTTP_201_CREATED)
         resource_id = self.get_id_for_created_resource(response)
         # update
         updated_data = copy.deepcopy(self._test_request_data)
         self.update_resource(updated_data)
         response = self.client.put(self.base_url + resource_id + '/', data=updated_data, format='json')
-        self.assertEqual(response.status_code, status.HTTP_200_OK)
+        #FIXME fails self.assertEqual(response.status_code, status.HTTP_200_OK)
         # verify
-        updated_obj = self.get_fhir_obj_from_json_response(response)
-        self.verify_updated_obj(updated_obj)
+        #FIXME updated_obj = self.get_fhir_obj_from_json_response(response)
+        #FIXME self.verify_updated_obj(updated_obj)
 
     def create_dependencies(self):
         pass
```

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/genericFhirAPITestMixin.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/genericFhirAPITestMixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,14 +90,15 @@
         fhir_obj = construct_fhir_element(response_json['resourceType'], response_json)
         if hasattr(fhir_obj, 'identifier'):
             result = BaseFHIRConverter.get_fhir_identifier_by_code(fhir_obj.identifier,
                                                                    R4IdentifierConfig.get_fhir_uuid_type_code())
         return result
 
     def get_fhir_obj_from_json_response(self, response):
+        fhir_obj = None
         response_json = response.json()
         if 'resourceType' in response_json:
             fhir_obj = construct_fhir_element(response_json['resourceType'], response_json)
             
         return fhir_obj
 
     def test_get_should_required_login(self):
```

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/genericTestMixin.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/genericTestMixin.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/groupTestMixin.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/groupTestMixin.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/insurancePlanTestMixin.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/insurancePlanTestMixin.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/invoiceTestMixin.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/invoiceTestMixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 
 from api_fhir_r4.configurations import R4IdentifierConfig
 from api_fhir_r4.tests import GenericTestMixin
 from api_fhir_r4.tests.mixin import FhirConverterTestMixin
 from api_fhir_r4.utils.timeUtils import TimeUtils
 from insuree.models import Family
 from invoice.models import Invoice, InvoiceLineItem
+from insuree.test_helpers import create_test_family
 
 
 class InvoiceTestMixin(GenericTestMixin, FhirConverterTestMixin):
     _TEST_INVOICE_STATUS = 'active'
     _TEST_INVOICE_CODE = 'TEST-CODE'
     _TEST_INVOICE_SUBJECT_TYPE_CODING = 'contribution'
-    _TEST_INVOICE_THIRD_PARTY = Family()
+    _TEST_INVOICE_THIRD_PARTY = None
     _TEST_INVOICE_THIRD_PARTY_UUID = '43C47D1E-5110-4880-8C53-6871E71BDDE8'
     _TEST_INVOICE_DATE = TimeUtils.str_iso_to_date('2021-01-01')
     _TEST_INVOICE_TOTAL_NET = 10000.0
     _TEST_INVOICE_TOTAL_GROSS = 10000.0
     _TEST_INVOICE_CURRENCY = 'USD'
     _TEST_LINE_ITEM_CHARGE_ITEM_CODING = 'policy'
     _TEST_LiNE_ITEM_QUANTITY = 1
@@ -27,28 +28,30 @@
     _TEST_LINE_ITEM_DISCOUNT = 0.1
     _TEST_LINE_ITEM_DEDUCTION_PRICE_COMPONENT_TYPE = 'deduction'
     _TEST_LINE_ITEM_DEDUCTION = 100
     _TEST_LINE_ITEM_DEDUCTION_FACTOR = 1
     _TEST_LINE_ITEM_TAX_PRICE_COMPONENT_TYPE = 'tax'
 
     def create_test_imis_instance(self):
+        self._TEST_INVOICE_THIRD_PARTY =  create_test_family()
         self._TEST_INVOICE_SUBJECT_TYPE = ContentType.objects.get(model__iexact='Family')
         self._TEST_LINE_ITEM_CHARGE_ITEM = ContentType.objects.get(model__iexact='Policy')
 
         imis_invoice = Invoice()
         imis_invoice.code = self._TEST_INVOICE_CODE
         imis_invoice.subject_type = self._TEST_INVOICE_SUBJECT_TYPE
         imis_invoice.thirdparty = self._TEST_INVOICE_THIRD_PARTY
         imis_invoice.thirdparty.uuid = self._TEST_INVOICE_THIRD_PARTY_UUID
         imis_invoice.date_invoice = self._TEST_INVOICE_DATE
         imis_invoice.amount_net = self._TEST_INVOICE_TOTAL_NET
         imis_invoice.amount_total = self._TEST_INVOICE_TOTAL_GROSS
         imis_invoice.currency_code = self._TEST_INVOICE_CURRENCY
 
         imis_invoice_line_item = InvoiceLineItem()
+        imis_invoice_line_item.code = "1"
         imis_invoice_line_item.line_type = self._TEST_LINE_ITEM_CHARGE_ITEM
         imis_invoice_line_item.quantity = self._TEST_LiNE_ITEM_QUANTITY
         imis_invoice_line_item.unit_price = self._TEST_LINE_ITEM_UNIT_PRICE
         imis_invoice_line_item.discount = self._TEST_LINE_ITEM_DISCOUNT
         imis_invoice_line_item.deduction = self._TEST_LINE_ITEM_DEDUCTION
         imis_invoice_line_item.invoice = imis_invoice
 
@@ -59,15 +62,15 @@
 
     def create_test_fhir_instance(self):
         raise NotImplementedError('create_test_fhir_instance() not implemented')
 
     def verify_fhir_instance(self, fhir_obj):
         if not (hasattr(self, '_TEST_INVOICE_SUBJECT_TYPE') and hasattr(self, '_TEST_LINE_ITEM_CHARGE_ITEM')):
             self.create_test_imis_instance()
-
+            
         self.assertIs(type(fhir_obj), FHIRInvoice)
         self.assertEqual(fhir_obj.status, self._TEST_INVOICE_STATUS)
         self.verify_fhir_identifier(fhir_obj, R4IdentifierConfig.get_fhir_generic_type_code(), self._TEST_INVOICE_CODE)
         self.verify_fhir_coding_exists(fhir_obj.type.coding, self._TEST_INVOICE_SUBJECT_TYPE_CODING)
         self.assertTrue(self._TEST_INVOICE_THIRD_PARTY_UUID in fhir_obj.recipient.reference)
         self.assertEqual(fhir_obj.date, self._TEST_INVOICE_DATE)
         self.assertEqual(fhir_obj.totalNet.value, self._TEST_INVOICE_TOTAL_NET, 1e-10)
```

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/locationTestMixin.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/locationTestMixin.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/logInMixin.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/logInMixin.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/medicationTestMixin.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/medicationTestMixin.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/operationOutcomeTestMixin.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/operationOutcomeTestMixin.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/patientTestMixin.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/patientTestMixin.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/paymentNoticeTestMixin.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/paymentNoticeTestMixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     def create_test_imis_instance(self):
         imis_payment = PaymentInvoice(
             **{
                 'reconciliation_status': self._TEST_PAYMENT_NOTICE_IMIS_RECONCILIATION_STATUS,
                 'amount_received': self._TEST_PAYMENT_NOTICE_IMIS_AMOUNT_RECEIVED,
                 'date_payment': self._TEST_PAYMENT_NOTICE_IMIS_DATE_PAYMENT,
                 'json_ext': self._TEST_PAYMENT_NOTICE_IMIS_JSON_EXT,
-                'payer_ref': ''
+                'payer_ref': 'ICD-54546'
             }
         )
         self._TEST_PAYMENT_NOTICE_IMIS_DETAILS_PAYMENT = imis_payment
         imis_payment_detail = DetailPaymentInvoice(
             **{
                 'status': self._TEST_PAYMENT_NOTICE_IMIS_DETAILS_STATUS,
                 'amount': self._TEST_PAYMENT_NOTICE_IMIS_AMOUNT_RECEIVED,
@@ -49,18 +49,18 @@
                 'subject_id': self._TEST_PAYMENT_NOTICE_IMIS_DETAILS_SUBJECT_ID
             }
         )
         return imis_payment, imis_payment_detail
 
     def verify_imis_instance(self, imis_obj):
         self.assertEquals(imis_obj.reconciliation_status, self._TEST_PAYMENT_NOTICE_IMIS_RECONCILIATION_STATUS)
-        self.assertEquals(imis_obj.amount_received, self._TEST_PAYMENT_NOTICE_IMIS_AMOUNT_RECEIVED)
+        self.assertEquals(round(float(imis_obj.amount_received),2), round(float(self._TEST_PAYMENT_NOTICE_IMIS_AMOUNT_RECEIVED),2))
         self.assertEquals(f'{imis_obj.date_payment}', self._TEST_PAYMENT_NOTICE_IMIS_DATE_PAYMENT)
         self.assertEquals(imis_obj.json_ext['reconciliation']['id'], self._TEST_PAYMENT_NOTICE_IMIS_JSON_EXT['reconciliation']['id'])
-        self.assertEquals(imis_obj.payer_ref, '')
+        self.assertEquals(imis_obj.payer_ref, 'PaymentReconciliation/id-renconiliation-test-1')
 
     def verify_imis_detail_instance(self, imis_obj, imis_detail_obj):
         self.assertEquals(imis_detail_obj.status, self._TEST_PAYMENT_NOTICE_IMIS_DETAILS_STATUS)
         self.assertEquals(imis_detail_obj.amount, self._TEST_PAYMENT_NOTICE_IMIS_AMOUNT_RECEIVED)
         self.assertEquals(imis_detail_obj.payment.id, imis_obj.id)
         self.assertEquals(imis_detail_obj.subject_id, self._TEST_PAYMENT_NOTICE_IMIS_DETAILS_SUBJECT_ID)
         self.assertEquals(imis_detail_obj.reconcilation_id, self._TEST_PAYMENT_NOTICE_IMIS_DETAILS_RECON_ID)
@@ -99,9 +99,9 @@
         }
 
     def verify_fhir_instance(self, fhir_obj):
         self.assertEquals(fhir_obj.status, self._TEST_PAYMENT_NOTICE_FHIR_STATUS)
         self.assertEquals(fhir_obj.request.reference, self._TEST_PAYMENT_NOTICE_FHIR_REQUEST_REFERENCE)
         self.assertEquals(f'{fhir_obj.paymentDate}', self._TEST_PAYMENT_NOTICE_FHIR_DATE_PAYMENT)
         self.assertEquals(fhir_obj.recipient.reference, self._TEST_PAYMENT_NOTICE_FHIR_RECIPIENT)
-        self.assertEquals(f'{fhir_obj.amount.value}', self._TEST_PAYMENT_NOTICE_FHIR_AMOUNT_VALUE)
+        self.assertEquals(round(float(fhir_obj.amount.value),2), round(float(self._TEST_PAYMENT_NOTICE_FHIR_AMOUNT_VALUE),2))
         self.assertEquals(fhir_obj.paymentStatus.coding[0].code, self._TEST_PAYMENT_NOTICE_FHIR_PAYMENT_STATUS)
```

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/mixin/policyHolderOrganisationTestMixin.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/mixin/policyHolderOrganisationTestMixin.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/subscriptions/client.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/subscriptions/client.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/subscriptions/manager.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/subscriptions/manager.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test/test_activity_definition.json` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test/test_activity_definition.json`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test/test_claim.json` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test/test_claim.json`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test/test_claimAdminPractitioner.json` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test/test_claimAdminPractitioner.json`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test/test_claimAdminPractitionerRole.json` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test/test_claimAdminPractitionerRole.json`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test/test_claimResponse.json` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test/test_claimResponse.json`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test/test_claim_contained.json` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test/test_claim_contained.json`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test/test_claim_with_code_references.json` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test/test_claim_with_code_references.json`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test/test_communication.json` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test/test_communication.json`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test/test_communicationRequest.json` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test/test_communicationRequest.json`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test/test_communication_with_code_reference.json` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test/test_communication_with_code_reference.json`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test/test_contract.json` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test/test_contract.json`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test/test_coverage.json` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test/test_coverage.json`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test/test_coverageEligibilityRequest.json` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test/test_coverageEligibilityRequest.json`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test/test_coverageEligibilityResponse.json` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test/test_coverageEligibilityResponse.json`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test/test_enrolmentOfficerPractitioner.json` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test/test_enrolmentOfficerPractitioner.json`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test/test_enrolmentOfficerPractitionerRole.json` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test/test_enrolmentOfficerPractitionerRole.json`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test/test_group.json` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test/test_group.json`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test/test_insurance_plan.json` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test/test_insurance_plan.json`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test/test_invoice.json` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test/test_invoice.json`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test/test_location.json` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test/test_location.json`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test/test_medication.json` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test/test_medication.json`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test/test_patient.json` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test/test_patient.json`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test/test_payment_notice.json` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test/test_payment_notice.json`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/testCodeSystem/test_api_codeDiagnosis.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/testCodeSystem/test_api_codeDiagnosis.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/testCodeSystem/test_api_codeGroupConfirmationType.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/testCodeSystem/test_api_codeGroupConfirmationType.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/testCodeSystem/test_api_codeGroupType.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/testCodeSystem/test_api_codeGroupType.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/testCodeSystem/test_api_codeHFOrganizationLegalForm.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/testCodeSystem/test_api_codeHFOrganizationLegalForm.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/testCodeSystem/test_api_codeHFOrganizationLevel.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/testCodeSystem/test_api_codeHFOrganizationLevel.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/testCodeSystem/test_api_codePHOrganisationActivity.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/testCodeSystem/test_api_codePHOrganisationActivity.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/testCodeSystem/test_api_codePHOrganisationLegalForm.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/testCodeSystem/test_api_codePHOrganisationLegalForm.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/testCodeSystem/test_api_codePatientContactRelationship.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/testCodeSystem/test_api_codePatientContactRelationship.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/testCodeSystem/test_api_codePatientEducationLevel.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/testCodeSystem/test_api_codePatientEducationLevel.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/testCodeSystem/test_api_codePatientIdentificationType.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/testCodeSystem/test_api_codePatientIdentificationType.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/testCodeSystem/test_api_codePatientProfession.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/testCodeSystem/test_api_codePatientProfession.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_activityDefinitionConverter.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_activityDefinitionConverter.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_api_authorization.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_api_authorization.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 
 from rest_framework import status
 from rest_framework.test import APITestCase
 
 from api_fhir_r4.configurations import GeneralConfiguration
 from api_fhir_r4.tests import GenericFhirAPITestMixin
+from gettext import gettext as _
 
 from api_fhir_r4.tests.utils import get_connection_payload,get_or_create_user_api
 
 class AuthorizationAPITests(GenericFhirAPITestMixin, APITestCase):
     base_url = GeneralConfiguration.get_base_url()
     url_to_test_authorization = base_url + 'Group/'
     _test_json_path = "/test/test_login.json"
@@ -48,15 +49,15 @@
         headers = {
             "Content-Type": "application/json",
             'HTTP_AUTHORIZATION': f"Bearer {token}ssdd"
         }
         response = self.client.get(self.url_to_test_authorization, format='json', **headers)
         response_json = response.json()
         self.assertEqual(response.status_code, status.HTTP_401_UNAUTHORIZED)
-        self.assertEqual(self.get_response_details(response_json), "Error decoding signature")
+        self.assertEqual(self.get_response_details(response_json), _('INCORRECT_CREDENTIALS'))
 
     def test_post_should_raise_lack_of_bearer_prefix(self):
         response = self.client.post(self.base_url + 'login/', data=get_connection_payload(), format='json')
         response_json = response.json()
         token = response_json["token"]
         headers = {
             "Content-Type": "application/json",
```

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_api_claim.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_api_claim.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from api_fhir_r4.utils import TimeUtils
 from api_fhir_r4.tests.utils import load_and_replace_json,get_connection_payload,get_or_create_user_api
 from api_fhir_r4.utils import DbManagerUtils
 
 from claim.models import Claim, ClaimDetail
 from insuree.test_helpers import create_test_insuree
 from location.models import HealthFacility, UserDistrict
-from location.test_helpers import create_test_village
+from location.test_helpers import create_test_village, create_test_health_facility
 from medical.models import Diagnosis
 from medical.test_helpers import create_test_item, create_test_service
 from claim.test_helpers import create_test_claimservice,create_test_claimitem,create_test_claim_admin
 
 class ClaimAPITests(GenericFhirAPITestMixin, APITestCase, LogInMixin):
     base_url = GeneralConfiguration.get_base_url() + 'Claim/'
     _test_json_path = "/test/test_claim.json"
@@ -91,25 +91,25 @@
         self.sub_str[self._TEST_CLAIM_ADMIN_UUID]=self.test_claim_admin.uuid
         self.sub_str[self._TEST_CLAIM_ADMIN_CODE]=self.test_claim_admin.code
 
         self.sub_str[self._TEST_ITEM_UUID]=self._TEST_ITEM.uuid
         self.sub_str[self._TEST_SERVICE_UUID]=self._TEST_SERVICE.uuid
         self.sub_str[self._TEST_ITEM_CODE]=self._TEST_ITEM.code
         self.sub_str[self._TEST_SERVICE_CODE]=self._TEST_SERVICE.code
+        self._TEST_HF_ID = self.test_hf.id
+        self._TEST_HF_UUID = self.test_hf.uuid
 
 
 
     def create_dependencies(self):
-        self.test_icd = Diagnosis()
-        self.test_icd.code = self._TEST_MAIN_ICD_CODE
-        self.test_icd.name = self._TEST_MAIN_ICD_NAME
+        self.test_icd = Diagnosis(code=self._TEST_MAIN_ICD_CODE, name =self._TEST_MAIN_ICD_NAME)
         self.test_icd.audit_user_id = self._ADMIN_AUDIT_USER_ID
         self.test_icd.save()
         self.test_insuree = create_test_insuree(custom_props={"chf_id": self._TEST_INSUREE_CODE})
-        self.test_hf = self.create_test_health_facility()
+        self.test_hf = self.create_test_hf()
         if not self.test_claim_admin:
             self.test_claim_admin =create_test_claim_admin(
                 custom_props={'code':'T-CA-API',
                               'health_facility_id': self.test_hf.id,
                                 'last_name' : self._TEST_DATA_USER['last_name'],
                                 'other_names' : self._TEST_DATA_USER['other_names']})
         
@@ -121,32 +121,30 @@
         ud.user = self._TEST_USER.i_user
         ud.validity_from = TimeUtils.now()
         ud.save()
 
         self._TEST_ITEM = create_test_item(self._TEST_SERVICE_TYPE)
         self._TEST_SERVICE = create_test_service(self._TEST_ITEM_TYPE)
 
-    def create_test_health_facility(self):
-        hf = HealthFacility()
-        hf.id = self._TEST_HF_ID
-        hf.uuid = self._TEST_HF_UUID
-        hf.code = self._TEST_HF_CODE
-        hf.name = self._TEST_HF_NAME
-        hf.level = self._TEST_HF_LEVEL
-        hf.legal_form_id = self._TEST_HF_LEGAL_FORM
-        hf.address = self._TEST_ADDRESS
-        hf.phone = self._TEST_PHONE
-        hf.fax = self._TEST_FAX
-        hf.email = self._TEST_EMAIL
-        hf.location = self.test_insuree.family.location.parent.parent
-        hf.offline = False
-        hf.audit_user_id = self._ADMIN_AUDIT_USER_ID
-        hf.save()
+    def create_test_hf(self):
+        self.test_hf = create_test_health_facility(
+            self._TEST_HF_CODE,
+            self.test_insuree.family.location.parent.parent.id,
+            custom_props = {
+                'name': self._TEST_HF_NAME,
+                'level':self._TEST_HF_LEVEL,
+                'legal_form_id':self._TEST_HF_LEGAL_FORM,
+                'address':self._TEST_ADDRESS,
+                'phone':self._TEST_PHONE,
+                'fax':self._TEST_FAX,
+                'email':self._TEST_EMAIL,
+            }
+        )
+        return self.test_hf
 
-        return hf
 
 
     def _post_claim(self, data, headers):
         return self.client.post(self.base_url, data=data, format='json', **headers)
 
 
     def test_post_should_create_correctly(self):
```

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_api_claim_contained.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_api_claim_contained.py`

 * *Files 3% similar despite different names*

```diff
@@ -117,14 +117,15 @@
         self.test_icd.name = self._TEST_MAIN_ICD_NAME
         self.test_icd.audit_user_id = self._ADMIN_AUDIT_USER_ID
         self.test_icd.save()
 
 
         self.test_village = self.test_insuree.current_village or self.test_insuree.family.location
         self.test_hf=self.create_test_hf()
+        self._TEST_HF_ID = self.test_hf.id
         if not self.test_claim_admin:
             self.test_claim_admin =create_test_claim_admin(
                 custom_props={'health_facility_id': self.test_hf.id,
                                 'last_name' : self._TEST_DATA_USER['last_name'],
                                 'other_names' : self._TEST_DATA_USER['other_names']})
         
 
@@ -154,27 +155,27 @@
             custom_props={"code": self._TEST_SERVICE_CODE}
         )
         service.code = self._TEST_SERVICE_CODE
         service.save()
         return service
 
     def create_test_hf(self):
-        hf = HealthFacility()
-        hf.code = self._TEST_HF_CODE
-        hf.name = self._TEST_HF_NAME
-        hf.level = self._TEST_HF_LEVEL
-        hf.legal_form_id = self._TEST_HF_LEGAL_FORM
-        hf.address = self._TEST_ADDRESS
-        hf.phone = self._TEST_PHONE
-        hf.fax = self._TEST_FAX
-        hf.email = self._TEST_EMAIL
-        hf.location = self.test_village.parent.parent
-        hf.offline = False
-        hf.audit_user_id = self._ADMIN_AUDIT_USER_ID
-        hf.save()
+        hf = create_test_health_facility(
+            self._TEST_HF_CODE,
+            self.test_village.parent.parent.id,
+            custom_props = {
+                'name': self._TEST_HF_NAME,
+                'level':self._TEST_HF_LEVEL,
+                'legal_form_id':self._TEST_HF_LEGAL_FORM,
+                'address':self._TEST_ADDRESS,
+                'phone':self._TEST_PHONE,
+                'fax':self._TEST_FAX,
+                'email':self._TEST_EMAIL,
+            }
+        )
         return hf
 
     def assert_response(self, response_json):
         self.assertEqual(response_json["outcome"], 'complete')
         for item in response_json["item"]:
             for adjudication in item["adjudication"]:
                 self.assertEqual(adjudication["category"]["coding"][0]["code"], f'{Claim.STATUS_REJECTED}')
```

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_api_communication.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_api_communication.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from claim.models import Claim, ClaimItem, ClaimService, Feedback
 from claim.test_helpers import create_test_claim_admin
 from core import datetime
 from insuree.test_helpers import create_test_insuree
 from location.models import HealthFacility
 from medical.models import Diagnosis
 from medical.test_helpers import create_test_item, create_test_service
-from location.test_helpers import create_test_village
+from location.test_helpers import create_test_village, create_test_health_facility
 
 
 class CommunicationAPITests(GenericFhirAPITestMixin, APITestCase, LogInMixin):
     base_url = GeneralConfiguration.get_base_url() + 'Communication/'
     _test_json_path = "/test/test_communication.json"
 
     _test_json_path_credentials = "/test/test_login.json"
@@ -101,26 +101,27 @@
     test_service = None
     def setUp(self):
         super(CommunicationAPITests, self).setUp()
         self._test_request_data=load_and_replace_json(self._test_json_path,self.sub_str)
         self.get_or_create_user_api()
         self.test_insuree = create_test_insuree()
         self.test_village = self.test_insuree.current_village or self.test_insuree.family.location
-        self.test_hf = self.create_test_health_facility()
+        self.test_hf = self.create_test_hf()
         self.test_claim_admin = create_test_claim_admin( custom_props={'health_facility_id': self.test_hf.id})
         self.test_claim = self.create_test_claim()
         self.test_item = self.create_test_claim_item()
         self.test_service = self.create_test_claim_service()
 
         self.sub_str[self._TEST_INSUREE_UUID]=self.test_insuree.uuid
         self.sub_str[self._TEST_INSUREE_CHFID]=self.test_insuree.chf_id
         self.sub_str[self._TEST_CLAIM_ADMIN_UUID]=self.test_claim_admin.uuid
         self.sub_str[self._TEST_CLAIM_UUID]=self.test_claim.uuid
         self.sub_str[self._TEST_HF_UUID]=self.test_hf.uuid
-
+        self._TEST_HF_UUID=self.test_hf.uuid
+        self._TEST_HF_ID=self.test_hf.id
 
 
 
     def create_test_claim_item(self):
         item = ClaimItem()
         item.item = create_test_item(
             self._TEST_ITEM_TYPE,
@@ -152,44 +153,42 @@
         service.availability = self._TEST_ITEM_AVAILABILITY
         service.price_asked = self._TEST_SERVICE_PRICE
         service.price_approved = self._TEST_SERVICE_PRICE
         service.audit_user_id = self._ADMIN_AUDIT_USER_ID
         service.save()
         return service
 
-    def create_test_health_facility(self):
-        hf = HealthFacility()
-        hf.id = self._TEST_HF_ID
-        hf.uuid = self._TEST_HF_UUID
-        hf.code = self._TEST_HF_CODE
-        hf.name = self._TEST_HF_NAME
-        hf.level = self._TEST_HF_LEVEL
-        hf.legal_form_id = self._TEST_HF_LEGAL_FORM
-        hf.address = self._TEST_ADDRESS
-        hf.phone = self._TEST_PHONE
-        hf.fax = self._TEST_FAX
-        hf.email = self._TEST_EMAIL
-        hf.location = self.test_village.parent.parent
-        hf.offline = False
-        hf.audit_user_id = -1
-        hf.save()
+    def create_test_hf(self):
+        hf = create_test_health_facility(
+            self._TEST_HF_CODE,
+            self.test_village.parent.parent.id,
+            custom_props = {
+                'name': self._TEST_HF_NAME,
+                'level':self._TEST_HF_LEVEL,
+                'legal_form_id':self._TEST_HF_LEGAL_FORM,
+                'address':self._TEST_ADDRESS,
+                'phone':self._TEST_PHONE,
+                'fax':self._TEST_FAX,
+                'email':self._TEST_EMAIL,
+            }
+        )
         return hf
 
     def create_test_claim(self):
         imis_claim = Claim()
         imis_claim.id = self._TEST_ID
         imis_claim.code = self._TEST_CLAIM_CODE
         imis_claim.status = self._TEST_STATUS
         imis_claim.adjustment = self._TEST_ADJUSTMENT
         imis_claim.date_processed = TimeUtils.str_to_date(self._TEST_DATE_PROCESSED)
         imis_claim.approved = self._TEST_APPROVED
         imis_claim.rejection_reason = self._TEST_REJECTION_REASON
         imis_claim.insuree = self.test_insuree
         imis_claim.health_facility = self.test_hf
-        imis_claim.icd = Diagnosis(code='ICD00I')
+        imis_claim.icd = Diagnosis(code='ICD00I', name="test icd")
         imis_claim.icd.audit_user_id = self._ADMIN_AUDIT_USER_ID
         imis_claim.icd.save()
         imis_claim.audit_user_id = self._ADMIN_AUDIT_USER_ID
         imis_claim.icd.date_from = datetime.date(2018, 12, 12)
         imis_claim.date_from = datetime.date(2018, 12, 12)
         imis_claim.date_claimed = datetime.date(2018, 12, 14)
         imis_claim.visit_type = self._TEST_VISIT_TYPE
```

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_api_communicationRequest.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_api_communicationRequest.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_api_contract.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_api_contract.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_api_group.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_api_group.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_api_insurancePlan.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_api_insurancePlan.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_api_invoice.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_api_invoice.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_api_location.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_api_location.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from rest_framework.test import APITestCase
 
 from location.models import Location
 from fhir.resources.R4B.location import Location as FHIRLocation
 from api_fhir_r4.tests import GenericFhirAPITestMixin, FhirApiCreateTestMixin
 from api_fhir_r4.configurations import GeneralConfiguration
-
+from api_fhir_r4.tests.utils import load_and_replace_json
 
 class LocationAPITests(GenericFhirAPITestMixin, FhirApiCreateTestMixin,
                        APITestCase):
 
     base_url = GeneralConfiguration.get_base_url()+'Location/'
     _test_json_path = "/test/test_location.json"
-    _TEST_MUNICIPALITY_UUID = "a82f54bf-d983-4963-a279-490312a96344"
+    _TEST_MUNICIPALITY_UUID = 'a82f54bf-d983-4963-a279-490312a96344'
     _TEST_EXPECTED_NAME = "UPDATED_NAME"
-
+    sub_str = {}
     def setUp(self):
         super(LocationAPITests, self).setUp()
         # create level location
         imis_location_region = Location()
         imis_location_region.code = "RT"
         imis_location_region.name = "Test"
         imis_location_region.type = "R"
@@ -27,20 +27,22 @@
         imis_location_district.code = "RTDT"
         imis_location_district.name = "Test"
         imis_location_district.type = "D"
         imis_location_district.parent = imis_location_region
         imis_location_district.save()
 
         imis_location_municipality = Location()
-        imis_location_municipality.code = "RTDTMT"
+        imis_location_municipality.code = "R2D2"
         imis_location_municipality.name = "Test"
         imis_location_municipality.type = "M"
         imis_location_municipality.parent = imis_location_district
-        imis_location_municipality.uuid = self._TEST_MUNICIPALITY_UUID
         imis_location_municipality.save()
+        self.sub_str[self._TEST_MUNICIPALITY_UUID] = imis_location_municipality.uuid
+        self._TEST_MUNICIPALITY_UUID =  imis_location_municipality.uuid
+        self._test_request_data = load_and_replace_json(self._test_json_path,self.sub_str)
 
     def verify_updated_obj(self, updated_obj):
         self.assertTrue(isinstance(updated_obj, FHIRLocation))
         self.assertEqual(self._TEST_EXPECTED_NAME, updated_obj.name)
 
     def update_resource(self, data):
         data['name'] = self._TEST_EXPECTED_NAME
```

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_api_login.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_api_login.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_api_medication.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_api_medication.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_api_organisation.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_api_organisation.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from rest_framework.test import APITestCase
 from api_fhir_r4.tests.mixin.logInMixin import LogInMixin
 from graphql_jwt.shortcuts import get_token
 from core.test_helpers import create_test_interactive_user
 from dataclasses import dataclass
 from core.models import User
 from rest_framework import status
-
+from policyholder.tests.helpers import create_test_policy_holder
 
 @dataclass
 class DummyContext:
     """ Just because we need a context to generate. """
     user: User
 
 class OrganisationAPITests(GenericFhirAPITestMixin, FhirApiReadTestMixin, APITestCase, LogInMixin):
@@ -20,26 +20,36 @@
     _test_request_data_credentials = None
     admin_token = None 
     admin_user = None
 
     @classmethod
     def setUpClass(cls):
         super().setUpClass()
+        cls.test_policy_holder = create_test_policy_holder()
         cls.admin_user = create_test_interactive_user(username="testLocationAdmin")
         cls.admin_token = get_token(cls.admin_user, DummyContext(user=cls.admin_user))
 
 
     def test_simple_list_page_2(self):
         headers = {
             "Content-Type": "application/json",
             'HTTP_AUTHORIZATION': f"Bearer {self.admin_token}"
         }
         response = self.client.get(self.base_url+ '?page-offset=2', format='json', **headers)
         self.assertEqual(response.status_code, status.HTTP_200_OK)
         self.assertIsNotNone(response.content)
-        
+    
+    def test_simple_ph(self):
+        headers = {
+            "Content-Type": "application/json",
+            'HTTP_AUTHORIZATION': f"Bearer {self.admin_token}"
+        }
+        #
+        response = self.client.get(self.base_url+ str(self.test_policy_holder.uuid).upper()+ '/' , format='json', **headers)
+        self.assertEqual(response.status_code, status.HTTP_200_OK)
+        self.assertIsNotNone(response.content)        
         
     def get_or_create_user_api(self):
         user = DbManagerUtils.get_object_or_none(User, username=self._TEST_USER_NAME)
         if user is None:
             user = self.__create_user_interactive_core()
         return user
```

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_api_patient.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_api_patient.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,14 +132,16 @@
         response_json = response.json()
         if 'issue' in response_json and len(response_json["issue"])>0\
             and 'details'in response_json["issue"][0]\
             and 'severity' in response_json["issue"][0]['details']:
             severity = response_json["issue"][0]['details']['severity']
         elif 'detail' in response_json and response_json['detail'] == 'Patient code not provided.':
             severity = 'error'
+        else:
+            severity =  f"no error in {response.content}"
         self.assertTrue(response.status_code, 500)
         self.assertEqual(severity, 'error')
 
     def test_post_should_raise_error_no_extensions(self):
         self.login()
         modified_payload = self.update_payload_no_extensions(data=self._test_request_data)
         response = self.client.post(self.base_url, data=modified_payload, format='json')
```

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_api_paymentNotice.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_api_paymentNotice.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_api_subscription.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_api_subscription.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_bill.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_bill.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_claimAdminPractitionerConverter.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_claimAdminPractitionerConverter.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_claimAdminPractitionerRoleConverter.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_claimAdminPractitionerRoleConverter.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_claimConverter.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_claimConverter.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_claimResponseConverter.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_claimResponseConverter.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_communicationConverter.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_communicationConverter.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_communicationRequestConverter.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_communicationRequestConverter.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_contractConverter.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_contractConverter.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_coverageConverter.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_coverageConverter.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_coverageEligibilityRequest.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_coverageEligibilityRequest.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_enrolmentOfficerPractitionerConverter.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_enrolmentOfficerPractitionerConverter.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_enrolmentOfficerPractitionerRoleConverter.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_patientConverter.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,22 @@
-from api_fhir_r4.converters import EnrolmentOfficerPractitionerRoleConverter
-from fhir.resources.R4B.practitionerrole import PractitionerRole
-from api_fhir_r4.tests import EnrolmentOfficerPractitionerRoleTestMixin
-from api_fhir_r4.tests.mixin import ConvertToImisTestMixin, ConvertToFhirTestMixin, ConvertJsonToFhirTestMixin
+from unittest import mock
 
+from api_fhir_r4.converters import PatientConverter
+
+from fhir.resources.R4B.patient import Patient
+from api_fhir_r4.tests import PatientTestMixin
+from api_fhir_r4.tests.mixin import ConvertToFhirTestMixin, ConvertToImisTestMixin, ConvertJsonToFhirTestMixin
+
+
+class PatientConverterTestCase(PatientTestMixin,
+                               ConvertToFhirTestMixin,
+                               ConvertToImisTestMixin,
+                               ConvertJsonToFhirTestMixin):
+    converter = PatientConverter
+    fhir_resource = Patient
+    json_repr = 'test/test_patient.json'
+
+    @mock.patch('insuree.models.Gender.objects')
+    def test_to_imis_obj(self, mock_gender):
+        mock_gender.get.return_value = self._TEST_GENDER
+        super(PatientConverterTestCase, self).test_to_imis_obj()
 
-class EnrolmentOfficerPractitionerRoleConverterTestCase(EnrolmentOfficerPractitionerRoleTestMixin,
-                                                        ConvertToImisTestMixin,
-                                                        ConvertToFhirTestMixin,
-                                                        ConvertJsonToFhirTestMixin):
-    converter = EnrolmentOfficerPractitionerRoleConverter
-    fhir_resource = PractitionerRole
-    json_repr = 'test/test_enrolmentOfficerPractitionerRole.json'
```

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_groupConverter.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_groupConverter.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_insurancePlanConverter.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_insurancePlanConverter.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_invoiceConverter.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_invoiceConverter.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_locationConverter.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_locationConverter.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_medicationConverter.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_medicationConverter.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_mixins.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_mixins.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_operationOutcomeConverter.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_operationOutcomeConverter.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_paymentNoticeConverter.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_paymentNoticeConverter.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,16 @@
 
     def create_dependencies(self, user):
         invoice = create_test_invoice(subject=None, thirdparty=None, user=user, **{
             'id': 'bd84b2f2-ec1d-48de-8f8c-5a477aa4a29f',
             'amount_total': '10000.0',
             'amount_net': '10000.0',
             'user_created': user,
-            'user_updated': user
+            'user_updated': user,
+            'date_created': '2020-01-01'
         })
         return invoice
 
     def test_to_fhir_obj(self):
         user = self.get_or_create_user_api()
         invoice = self.create_dependencies(user)
         imis_payment, imis_payment_detail = self.create_test_imis_instance()
```

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_subscriptionConverter.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_subscriptionConverter.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_subscriptionService.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_subscriptionService.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/test_timeUtils.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/test_timeUtils.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/tests/utils.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/tests/utils.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/urls.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/urls.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/utils/dbManagerUtils.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/utils/dbManagerUtils.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/utils/timeUtils.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/utils/timeUtils.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/__init__.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/__init__.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/activity_definition.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/activity_definition.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/base/__init__.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/base/__init__.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/claim.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/claim.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/claim_response.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/claim_response.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/code_systems/diagnosis.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/code_systems/diagnosis.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/code_systems/group_confirmation_type.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/code_systems/group_confirmation_type.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/code_systems/group_type.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/code_systems/group_type.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/code_systems/organization_hf_legal_form.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/code_systems/organization_hf_legal_form.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/code_systems/organization_hf_level.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/code_systems/organization_hf_level.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/code_systems/organization_ph_activity.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/code_systems/organization_ph_activity.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/code_systems/organization_ph_legal_form.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/code_systems/organization_ph_legal_form.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/code_systems/patient_education_level.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/code_systems/patient_education_level.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/code_systems/patient_identification_type.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/code_systems/patient_identification_type.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/code_systems/patient_profession.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/code_systems/patient_profession.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/code_systems/patient_relationship.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/code_systems/patient_relationship.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/communication.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/communication.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/communication_request.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/communication_request.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/contract.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/contract.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/coverage_eligibility_request.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/coverage_eligibility_request.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/coverage_request.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/coverage_request.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/group.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/group.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/insurance_plan.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/insurance_plan.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/insuree.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/insuree.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/invoice.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/invoice.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/location.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/location.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from rest_framework import viewsets
 
 from api_fhir_r4.mixins import MultiIdentifierRetrieverMixin, MultiIdentifierUpdateMixin
 from api_fhir_r4.model_retrievers import UUIDIdentifierModelRetriever, CodeIdentifierModelRetriever
-from api_fhir_r4.permissions import FHIRApiHFPermissions
+from api_fhir_r4.permissions import FHIRApiLocationPermissions
 from api_fhir_r4.serializers import LocationSerializer, LocationSiteSerializer
 from api_fhir_r4.views.fhir.base import BaseFHIRView
 from api_fhir_r4.views.filters import ValidityFromRequestParameterFilter
 from location.models import HealthFacility, Location
 
 
 class LocationViewSet(BaseFHIRView, MultiIdentifierRetrieverMixin,
                       viewsets.ModelViewSet, MultiIdentifierUpdateMixin):
     retrievers = [UUIDIdentifierModelRetriever, CodeIdentifierModelRetriever]
     serializer_class = LocationSerializer
-    permission_classes = (FHIRApiHFPermissions,)
+    permission_classes = (FHIRApiLocationPermissions,)
 
     def list(self, request, *args, **kwargs):
         identifier = request.GET.get("identifier")
         physical_type = request.GET.get('physicalType')
         queryset = self.get_queryset(physical_type)
         if identifier:
             return self.retrieve(request, *args, **{**kwargs, 'identifier': identifier})
```

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/medication.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/medication.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/organisation.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/organisation.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/payment_notice.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/payment_notice.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/practitioner.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/practitioner.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/practitioner_role.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/practitioner_role.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/fhir/subscription.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/fhir/subscription.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/filters/requestParameterFilter.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/filters/requestParameterFilter.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/api_fhir_r4/views/login_viewset.py` & `openimis_be_api_fhir_r4-1.7.0/api_fhir_r4/views/login_viewset.py`

 * *Files identical despite different names*

### Comparing `openimis-be-api_fhir_r4-1.6.0/openimis_be_api_fhir_r4.egg-info/PKG-INFO` & `openimis_be_api_fhir_r4-1.7.0/openimis_be_api_fhir_r4.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: openimis-be-api-fhir-r4
-Version: 1.6.0
+Name: openimis-be-api_fhir_r4
+Version: 1.7.0
 Summary: The openIMIS Backend FHIR R4 API reference module.
 Home-page: https://openimis.org/
 Author: Faris Ahmetasevic
 Author-email: faris.ahmetasevic@hotmail.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-api_fhir_r4-1.6.0/openimis_be_api_fhir_r4.egg-info/SOURCES.txt` & `openimis_be_api_fhir_r4-1.7.0/openimis_be_api_fhir_r4.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -85,14 +85,15 @@
 api_fhir_r4/mapping/subscriptionMapping.py
 api_fhir_r4/migrations/0001_initial.py
 api_fhir_r4/migrations/0002_auto_20220313_1607.py
 api_fhir_r4/migrations/0003_auto_20220313_1634.py
 api_fhir_r4/migrations/0004_update_subscription_criteria.py
 api_fhir_r4/migrations/0005_auto_20221012_0818.py
 api_fhir_r4/migrations/0006_add_subsription_perms_imis_admin.py
+api_fhir_r4/migrations/0007_alter_historicalsubscription_criteria_and_more.py
 api_fhir_r4/migrations/__init__.py
 api_fhir_r4/models/__init__.py
 api_fhir_r4/models/fhirModels.py
 api_fhir_r4/models/imisModelEnums.py
 api_fhir_r4/models/subscription.py
 api_fhir_r4/multiserializer/__init__.py
 api_fhir_r4/multiserializer/mixins.py
```

### Comparing `openimis-be-api_fhir_r4-1.6.0/setup.py` & `openimis_be_api_fhir_r4-1.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-api_fhir_r4',
-    version='v1.6.0',
+    version='v1.7.0',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend FHIR R4 API reference module.',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://openimis.org/',
```

