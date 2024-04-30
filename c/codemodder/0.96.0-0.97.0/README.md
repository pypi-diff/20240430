# Comparing `tmp/codemodder-0.96.0.tar.gz` & `tmp/codemodder-0.97.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codemodder-0.96.0.tar", last modified: Thu Apr 25 19:33:08 2024, max compression
+gzip compressed data, was "codemodder-0.97.0.tar", last modified: Tue Apr 30 18:21:25 2024, max compression
```

## Comparing `codemodder-0.96.0.tar` & `codemodder-0.97.0.tar`

### file list

```diff
@@ -1,519 +1,530 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:33:08.670448 codemodder-0.96.0/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-25 19:32:59.000000 codemodder-0.96.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:33:08.586448 codemodder-0.96.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-25 19:32:59.000000 codemodder-0.96.0/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-25 19:32:59.000000 codemodder-0.96.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-25 19:32:59.000000 codemodder-0.96.0/.github/pixeebot.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-25 19:32:59.000000 codemodder-0.96.0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:33:08.590448 codemodder-0.96.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-25 19:32:59.000000 codemodder-0.96.0/.github/workflows/autoformat-pixeebot-prs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-25 19:32:59.000000 codemodder-0.96.0/.github/workflows/codemod_pygoat.yml
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-25 19:32:59.000000 codemodder-0.96.0/.github/workflows/deploy_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-25 19:32:59.000000 codemodder-0.96.0/.github/workflows/integration_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-25 19:32:59.000000 codemodder-0.96.0/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-25 19:32:59.000000 codemodder-0.96.0/.github/workflows/pre-commit-autoupdate.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-25 19:32:59.000000 codemodder-0.96.0/.github/workflows/sonar_pixee.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-25 19:32:59.000000 codemodder-0.96.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-25 19:32:59.000000 codemodder-0.96.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-25 19:32:59.000000 codemodder-0.96.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-25 19:32:59.000000 codemodder-0.96.0/.semgrepignore
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-25 19:32:59.000000 codemodder-0.96.0/.sonarcloud.properties
--rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-04-25 19:32:59.000000 codemodder-0.96.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-25 19:32:59.000000 codemodder-0.96.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-25 19:32:59.000000 codemodder-0.96.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-25 19:32:59.000000 codemodder-0.96.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-25 19:32:59.000000 codemodder-0.96.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-25 19:32:59.000000 codemodder-0.96.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    44703 2024-04-25 19:33:08.670448 codemodder-0.96.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-25 19:32:59.000000 codemodder-0.96.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:33:08.590448 codemodder-0.96.0/ci_tests/
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-25 19:32:59.000000 codemodder-0.96.0/ci_tests/test_pygoat_findings.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-25 19:32:59.000000 codemodder-0.96.0/codecov.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:33:08.590448 codemodder-0.96.0/img/
--rw-r--r--   0 runner    (1001) docker     (127)    41511 2024-04-25 19:32:59.000000 codemodder-0.96.0/img/base-codemod.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-04-25 19:32:59.000000 codemodder-0.96.0/img/codemodder-dark.png
--rw-r--r--   0 runner    (1001) docker     (127)    11528 2024-04-25 19:32:59.000000 codemodder-0.96.0/img/codemodder-light.png
--rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-04-25 19:32:59.000000 codemodder-0.96.0/img/codemodder.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:33:08.598448 codemodder-0.96.0/integration_tests/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:33:08.602448 codemodder-0.96.0/integration_tests/sonar/
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/sonar/test_sonar_django_jmodel_without_dunder_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/sonar/test_sonar_django_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/sonar/test_sonar_django_receiver_on_top.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/sonar/test_sonar_exception_without_raise.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/sonar/test_sonar_fix_assert_tuple.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/sonar/test_sonar_fix_float_equality.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/sonar/test_sonar_fix_math_isclose.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/sonar/test_sonar_fix_missing_self_or_cls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/sonar/test_sonar_flask_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/sonar/test_sonar_jinja2_autoescape.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/sonar/test_sonar_jwt_decode_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/sonar/test_sonar_literal_or_new_object_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/sonar/test_sonar_numpy_nan_equality.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/sonar/test_sonar_remove_assertion_in_pytest_raises.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/sonar/test_sonar_secure_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/sonar/test_sonar_sql_parameterization.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/sonar/test_sonar_tempfile_mktemp.py
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/sonar/test_sonar_url_sandbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_add_requests_timeout.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_combine_startswith_endswith.py
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_dependency_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_django_debug_flag_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_django_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_django_model_without_dunder_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_django_receiver_on_top.py
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_django_session_cookie_secure_off.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_exception_without_raise.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_file_resource_leak.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_fix_assert_tuple.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_fix_dataclass_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_fix_deprecated_abstractproperty.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_fix_deprecated_logging_warn.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_fix_empty_sequence_comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_fix_float_equality.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_fix_hasattr_call.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_fix_math_isclose.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_fix_missing_self_or_cls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_fix_mutable_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_fix_task_instantiation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_flask_enable_csrf_protection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_flask_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_harden_pickle_load.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_harden_pyyaml.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_harden_ruamel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_https_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_jinja2_autoescape.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_jwt_decode_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_lazy_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_limit_readline.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_literal_or_new_object_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_lxml_safe_parser_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_lxml_safe_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_multiple_codemods.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_numpy_nan_equality.py
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_order_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_process_sandbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_program.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_remove_assertion_in_pytest_raises.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_remove_debug_breakpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_remove_future_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_remove_module_global.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_remove_unused_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_replace_flask_send_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_request_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_secure_flask_cookie.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_secure_flask_session_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_secure_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_sql_parameterization.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_str_concat_in_seq_literals.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_subprocess_shell_false.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_tempfile_mktemp.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_unnecessary_f_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_upgrade_sslcontext_minimum_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_upgrade_sslcontext_tls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_url_sandbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_use_defusedxml.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_use_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_use_set_literal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_use_walrus_if.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-25 19:32:59.000000 codemodder-0.96.0/integration_tests/test_with_threading_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-04-25 19:32:59.000000 codemodder-0.96.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-25 19:32:59.000000 codemodder-0.96.0/renovate.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 19:33:08.670448 codemodder-0.96.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:33:08.582448 codemodder-0.96.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:33:08.606448 codemodder-0.96.0/src/codemodder/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-25 19:33:08.000000 codemodder-0.96.0/src/codemodder/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6143 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/code_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     7915 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/codemodder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:33:08.606448 codemodder-0.96.0/src/codemodder/codemods/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/codemods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/codemods/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7856 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/codemods/base_codemod.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/codemods/base_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/codemods/base_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/codemods/base_visitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/codemods/check_annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/codemods/import_modifier_codemod.py
--rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/codemods/imported_call_modifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    11110 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/codemods/libcst_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/codemods/semgrep.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:33:08.610448 codemodder-0.96.0/src/codemodder/codemods/test/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/codemods/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12771 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/codemods/test/integration_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/codemods/test/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/codemods/test/validations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:33:08.610448 codemodder-0.96.0/src/codemodder/codemods/transformations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/codemods/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16626 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/codemods/transformations/clean_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/codemods/transformations/remove_empty_string_concatenation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/codemods/transformations/remove_unused_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     7879 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/codemods/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    23555 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/codemods/utils_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/codetf.py
--rw-r--r--   0 runner    (1001) docker     (127)     7959 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5409 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/dependency.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:33:08.610448 codemodder-0.96.0/src/codemodder/dependency_management/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/dependency_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/dependency_management/base_dependency_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/dependency_management/codemod_dependencies.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/dependency_management/dependency_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/dependency_management/pyproject_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/dependency_management/requirements_txt_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6424 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/dependency_management/setup_py_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/dependency_management/setupcfg_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/diff.py
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/file_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:33:08.610448 codemodder-0.96.0/src/codemodder/project_analysis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/project_analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:33:08.610448 codemodder-0.96.0/src/codemodder/project_analysis/file_parsers/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/project_analysis/file_parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/project_analysis/file_parsers/base_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/project_analysis/file_parsers/package_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/project_analysis/file_parsers/pyproject_toml_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/project_analysis/file_parsers/requirements_txt_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/project_analysis/file_parsers/setup_cfg_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/project_analysis/file_parsers/setup_py_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/project_analysis/file_parsers/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/project_analysis/python_repo_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/sarifs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:33:08.614448 codemodder-0.96.0/src/codemodder/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19371 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/scripts/generate_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/scripts/get_hashes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/semgrep.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:33:08.614448 codemodder-0.96.0/src/codemodder/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/utils/abc_dataclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     9967 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/utils/clean_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/utils/format_string_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8487 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/utils/linearize_string_expression.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/codemodder/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:33:08.666448 codemodder-0.96.0/src/codemodder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    44703 2024-04-25 19:33:08.000000 codemodder-0.96.0/src/codemodder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22004 2024-04-25 19:33:08.000000 codemodder-0.96.0/src/codemodder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:33:08.000000 codemodder-0.96.0/src/codemodder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-25 19:33:08.000000 codemodder-0.96.0/src/codemodder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-25 19:33:08.000000 codemodder-0.96.0/src/codemodder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-25 19:33:08.000000 codemodder-0.96.0/src/codemodder.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:33:08.622448 codemodder-0.96.0/src/core_codemods/
--rw-r--r--   0 runner    (1001) docker     (127)     7383 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/add_requests_timeouts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:33:08.622448 codemodder-0.96.0/src/core_codemods/api/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/api/core_codemod.py
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/combine_startswith_endswith.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:33:08.622448 codemodder-0.96.0/src/core_codemods/defectdojo/
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/defectdojo/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/defectdojo/results.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:33:08.622448 codemodder-0.96.0/src/core_codemods/defectdojo/semgrep/
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/defectdojo/semgrep/avoid_insecure_deserialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/defectdojo/semgrep/django_secure_set_cookie.py
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/django_debug_flag_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/django_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/django_model_without_dunder_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/django_receiver_on_top.py
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/django_session_cookie_secure_off.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:33:08.634448 codemodder-0.96.0/src/core_codemods/docs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/defectdojo_python_avoid-insecure-deserialization.md
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/defectdojo_python_django-secure-set-cookie.md
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_add-requests-timeouts.md
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_bad-lock-with-statement.md
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_combine-startswith-endswith.md
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_django-debug-flag-on.md
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_django-json-response-type.md
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_django-model-without-dunder-str.md
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_django-receiver-on-top.md
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_django-session-cookie-secure-off.md
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_enable-jinja2-autoescape.md
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_exception-without-raise.md
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_fix-assert-tuple.md
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_fix-async-task-instantiation.md
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_fix-dataclass-defaults.md
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_fix-deprecated-abstractproperty.md
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_fix-deprecated-logging-warn.md
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_fix-empty-sequence-comparison.md
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_fix-file-resource-leak.md
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_fix-float-equality.md
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_fix-hasattr-call.md
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_fix-math-isclose.md
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_fix-missing-self-or-cls.md
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_fix-mutable-params.md
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_flask-enable-csrf-protection.md
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_flask-json-response-type.md
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_harden-pickle-load.md
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_harden-pyyaml.md
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_harden-ruamel.md
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_https-connection.md
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_jwt-decode-verify.md
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_lazy-logging.md
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_limit-readline.md
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_literal-or-new-object-identity.md
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_numpy-nan-equality.md
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_remove-assertion-in-pytest-raises.md
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_remove-debug-breakpoint.md
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_remove-future-imports.md
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_remove-module-global.md
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_remove-unnecessary-f-str.md
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_replace-flask-send-file.md
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_requests-verify.md
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_safe-lxml-parser-defaults.md
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_safe-lxml-parsing.md
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_sandbox-process-creation.md
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_secure-flask-cookie.md
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_secure-flask-session-configuration.md
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_secure-random.md
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_secure-tempfile.md
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_sql-parameterization.md
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_str-concat-in-sequence-literals.md
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_subprocess-shell-false.md
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_unused-imports.md
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_upgrade-sslcontext-minimum-version.md
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_upgrade-sslcontext-tls.md
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_url-sandbox.md
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_use-defusedxml.md
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_use-generator.md
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_use-set-literal.md
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/docs/pixee_python_use-walrus-if.md
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/enable_jinja2_autoescape.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/exception_without_raise.py
--rw-r--r--   0 runner    (1001) docker     (127)    16039 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/file_resource_leak.py
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/fix_assert_tuple.py
--rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/fix_async_task_instantiation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/fix_dataclass_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/fix_deprecated_abstractproperty.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/fix_deprecated_logging_warn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/fix_empty_sequence_comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/fix_float_equality.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/fix_hasattr_call.py
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/fix_math_isclose.py
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/fix_missing_self_or_cls.py
--rw-r--r--   0 runner    (1001) docker     (127)     8235 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/fix_mutable_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/flask_enable_csrf_protection.py
--rw-r--r--   0 runner    (1001) docker     (127)    11313 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/flask_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/harden_pickle_load.py
--rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/harden_pyyaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/harden_ruamel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/https_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/jwt_decode_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)     7459 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/lazy_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/limit_readline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/literal_or_new_object_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/lxml_safe_parser_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/lxml_safe_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/numpy_nan_equality.py
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/order_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/process_creation_sandbox.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:33:08.634448 codemodder-0.96.0/src/core_codemods/refactor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/refactor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10705 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/refactor/refactor_new_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/remove_assertion_in_pytest_raises.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/remove_debug_breakpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/remove_future_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/remove_module_global.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/remove_unnecessary_f_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/remove_unused_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/replace_flask_send_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/requests_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/secure_cookie_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/secure_flask_cookie.py
--rw-r--r--   0 runner    (1001) docker     (127)     8216 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/secure_flask_session_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/secure_random.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:33:08.638448 codemodder-0.96.0/src/core_codemods/sonar/
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/sonar/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/sonar/results.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/sonar/sonar_django_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/sonar/sonar_django_model_without_dunder_str.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/sonar/sonar_django_receiver_on_top.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/sonar/sonar_enable_jinja2_autoescape.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/sonar/sonar_exception_without_raise.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/sonar/sonar_fix_assert_tuple.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/sonar/sonar_fix_float_equality.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/sonar/sonar_fix_math_isclose.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/sonar/sonar_fix_missing_self_or_cls.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/sonar/sonar_flask_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/sonar/sonar_jwt_decode_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/sonar/sonar_literal_or_new_object_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/sonar/sonar_numpy_nan_equality.py
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/sonar/sonar_remove_assertion_in_pytest_raises.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/sonar/sonar_secure_random.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/sonar/sonar_sql_parameterization.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/sonar/sonar_tempfile_mktemp.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/sonar/sonar_url_sandbox.py
--rw-r--r--   0 runner    (1001) docker     (127)    22996 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/sql_parameterization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/str_concat_in_seq_literal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/subprocess_shell_false.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/tempfile_mktemp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/upgrade_sslcontext_minimum_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/upgrade_sslcontext_tls.py
--rw-r--r--   0 runner    (1001) docker     (127)     7189 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/url_sandbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/use_defused_xml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/use_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/use_set_literal.py
--rw-r--r--   0 runner    (1001) docker     (127)     8037 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/use_walrus_if.py
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-25 19:32:59.000000 codemodder-0.96.0/src/core_codemods/with_threading_lock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:33:08.642448 codemodder-0.96.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:33:08.654448 codemodder-0.96.0/tests/codemods/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:33:08.582448 codemodder-0.96.0/tests/codemods/defectdojo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:33:08.654448 codemodder-0.96.0/tests/codemods/defectdojo/semgrep/
--rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/defectdojo/semgrep/test_avoid_insecure_deserialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/defectdojo/semgrep/test_django_secure_set_cookie.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:33:08.658448 codemodder-0.96.0/tests/codemods/sonar/
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/sonar/test_sonar_django_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/sonar/test_sonar_django_model_without_dunder_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/sonar/test_sonar_django_receiver_on_top.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/sonar/test_sonar_enable_jinja2_autoescape.py
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/sonar/test_sonar_exception_without_raise.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/sonar/test_sonar_fix_assert_tuple.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/sonar/test_sonar_fix_float_equality.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/sonar/test_sonar_fix_math_isclose.py
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/sonar/test_sonar_fix_missing_self_or_cls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/sonar/test_sonar_flask_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/sonar/test_sonar_jwt_decode_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/sonar/test_sonar_literal_or_new_object_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/sonar/test_sonar_numpy_nan_equality.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/sonar/test_sonar_remove_assertion_in_pytest_raises.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/sonar/test_sonar_secure_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/sonar/test_sonar_sql_parameterization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/sonar/test_sonar_tempfile_mktemp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/sonar/test_sonar_url_sandbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_add_requests_timeouts.py
--rw-r--r--   0 runner    (1001) docker     (127)     7831 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_async_fix_task_instantiation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_base_codemod.py
--rw-r--r--   0 runner    (1001) docker     (127)     6056 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_base_visitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_combine_startswith_endswith.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_django_debug_flag_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_django_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_django_model_without_dunder_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_django_receiver_on_top.py
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_django_session_cookie_secure_off.py
--rw-r--r--   0 runner    (1001) docker     (127)     6891 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_enable_jinja2_autoescape.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_exception_without_raise.py
--rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_file_resource_leak.py
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_fix_assert_tuple.py
--rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_fix_dataclass_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_fix_deprecated_abstractproperty.py
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_fix_deprecated_logging_warn.py
--rw-r--r--   0 runner    (1001) docker     (127)    11617 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_fix_empty_sequence_comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_fix_float_equality.py
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_fix_hasattr_call.py
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_fix_math_isclose.py
--rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_fix_missing_self_or_cls.py
--rw-r--r--   0 runner    (1001) docker     (127)     9896 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_fix_mutable_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_flask_enable_csrf_protection.py
--rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_flask_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_harden_pickle_load.py
--rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_harden_pyyaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_harden_ruamel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_https_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_include_exclude.py
--rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_jwt_decode_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)    23745 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_lazy_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_limit_readline.py
--rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_literal_or_new_object_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_lxml_safe_parameter_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_lxml_safe_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_numpy_nan_equality.py
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_order_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_process_creation_sandbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_remove_assertion_in_pytest_raises.py
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_remove_debug_breakpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_remove_future_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_remove_module_global.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_remove_unnecessary_f_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_remove_unused_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_replace_flask_send_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     7348 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_request_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_secure_flask_cookie.py
--rw-r--r--   0 runner    (1001) docker     (127)     7704 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_secure_flask_session_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_secure_random.py
--rw-r--r--   0 runner    (1001) docker     (127)    16046 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_sql_parameterization.py
--rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_str_concat_in_seq_literal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_subprocess_shell_false.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_tempfile_mktemp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_upgrade_sslcontext_minimum_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_upgrade_sslcontext_tls.py
--rw-r--r--   0 runner    (1001) docker     (127)     6772 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_url_sandbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     4835 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_use_defused_xml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_use_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_use_set_literal.py
--rw-r--r--   0 runner    (1001) docker     (127)     8036 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_walrus_if.py
--rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/codemods/test_with_threading_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:33:08.658448 codemodder-0.96.0/tests/dependency_management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/dependency_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/dependency_management/test_base_dependency_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/dependency_management/test_dependency_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/dependency_management/test_pyproject_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/dependency_management/test_requirements_txt_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13718 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/dependency_management/test_setup_py_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9072 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/dependency_management/test_setupcfgt_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:33:08.658448 codemodder-0.96.0/tests/project_analysis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/project_analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:33:08.658448 codemodder-0.96.0/tests/project_analysis/file_parsers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/project_analysis/file_parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/project_analysis/file_parsers/test_pyproject_toml_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/project_analysis/file_parsers/test_requirements_txt_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/project_analysis/file_parsers/test_setup_cfg_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/project_analysis/file_parsers/test_setup_py_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/project_analysis/test_python_repo_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:33:08.666448 codemodder-0.96.0/tests/samples/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/samples/django_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/samples/django_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/samples/django_receiver_on_top.py
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/samples/exception_without_raise.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/samples/fix_assert_tuple.py
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/samples/fix_float_equality.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/samples/fix_math_isclose.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/samples/fix_missing_self_or_cls.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/samples/fix_sonar_sql_parameterization.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/samples/flask_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/samples/flask_request.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/samples/jinja2_autoescape.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/samples/jwt_decode_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/samples/literal_or_new_object_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/samples/make_request.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/samples/multiple_codemods.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/samples/numpy_nan_equality.py
--rw-r--r--   0 runner    (1001) docker     (127)  2680067 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/samples/pygoat.semgrep.sarif.json
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/samples/remove_assertion_in_pytest_raises.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/samples/secure_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/samples/semgrep.sarif
--rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/samples/sonar_hotspots.json
--rw-r--r--   0 runner    (1001) docker     (127)    88996 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/samples/sonar_issues.json
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-25 19:32:59.000000 codemodder-0.96.0/tests/samples/tempfile_mktemp.py
--rw-r--r--   0 runner    (1001) docker     (127)   451117 2024-04-25 19:33:00.000000 codemodder-0.96.0/tests/samples/webgoat_v8.2.0_codeql.sarif
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-04-25 19:33:00.000000 codemodder-0.96.0/tests/test_ancestorpatterns_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-04-25 19:33:00.000000 codemodder-0.96.0/tests/test_basetype.py
--rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-04-25 19:33:00.000000 codemodder-0.96.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5628 2024-04-25 19:33:00.000000 codemodder-0.96.0/tests/test_code_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-25 19:33:00.000000 codemodder-0.96.0/tests/test_codemod_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12788 2024-04-25 19:33:00.000000 codemodder-0.96.0/tests/test_codemodder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-04-25 19:33:00.000000 codemodder-0.96.0/tests/test_codetf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-25 19:33:00.000000 codemodder-0.96.0/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-25 19:33:00.000000 codemodder-0.96.0/tests/test_file_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-04-25 19:33:00.000000 codemodder-0.96.0/tests/test_format_string_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-25 19:33:00.000000 codemodder-0.96.0/tests/test_libcst_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-04-25 19:33:00.000000 codemodder-0.96.0/tests/test_linearize_string_expression.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-25 19:33:00.000000 codemodder-0.96.0/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     6302 2024-04-25 19:33:00.000000 codemodder-0.96.0/tests/test_nameresolution_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-25 19:33:00.000000 codemodder-0.96.0/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-25 19:33:00.000000 codemodder-0.96.0/tests/test_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-04-25 19:33:00.000000 codemodder-0.96.0/tests/test_sarif_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-25 19:33:00.000000 codemodder-0.96.0/tests/test_semgrep.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-25 19:33:00.000000 codemodder-0.96.0/tests/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:33:08.666448 codemodder-0.96.0/tests/transformations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:33:00.000000 codemodder-0.96.0/tests/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-25 19:33:00.000000 codemodder-0.96.0/tests/transformations/test_clean_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-25 19:33:00.000000 codemodder-0.96.0/tests/transformations/test_remove_empty_string_concatenation.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-25 19:33:00.000000 codemodder-0.96.0/tests/transformations/test_remove_unused_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:21:25.840949 codemodder-0.97.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-30 18:21:16.000000 codemodder-0.97.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:21:25.764946 codemodder-0.97.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-30 18:21:16.000000 codemodder-0.97.0/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-30 18:21:16.000000 codemodder-0.97.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-30 18:21:16.000000 codemodder-0.97.0/.github/pixeebot.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-30 18:21:16.000000 codemodder-0.97.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:21:25.764946 codemodder-0.97.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-30 18:21:16.000000 codemodder-0.97.0/.github/workflows/autoformat-pixeebot-prs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-30 18:21:16.000000 codemodder-0.97.0/.github/workflows/codemod_pygoat.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-30 18:21:16.000000 codemodder-0.97.0/.github/workflows/deploy_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-30 18:21:16.000000 codemodder-0.97.0/.github/workflows/integration_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-30 18:21:16.000000 codemodder-0.97.0/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-30 18:21:16.000000 codemodder-0.97.0/.github/workflows/pre-commit-autoupdate.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-30 18:21:16.000000 codemodder-0.97.0/.github/workflows/sonar_pixee.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-30 18:21:16.000000 codemodder-0.97.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-30 18:21:16.000000 codemodder-0.97.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-30 18:21:16.000000 codemodder-0.97.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-30 18:21:16.000000 codemodder-0.97.0/.semgrepignore
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-30 18:21:16.000000 codemodder-0.97.0/.sonarcloud.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-04-30 18:21:16.000000 codemodder-0.97.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-30 18:21:16.000000 codemodder-0.97.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-30 18:21:16.000000 codemodder-0.97.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-30 18:21:16.000000 codemodder-0.97.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-30 18:21:16.000000 codemodder-0.97.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-30 18:21:16.000000 codemodder-0.97.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    44701 2024-04-30 18:21:25.840949 codemodder-0.97.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-30 18:21:16.000000 codemodder-0.97.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:21:25.768947 codemodder-0.97.0/ci_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-30 18:21:16.000000 codemodder-0.97.0/ci_tests/test_pygoat_findings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-30 18:21:16.000000 codemodder-0.97.0/codecov.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:21:25.768947 codemodder-0.97.0/img/
+-rw-r--r--   0 runner    (1001) docker     (127)    41511 2024-04-30 18:21:16.000000 codemodder-0.97.0/img/base-codemod.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-04-30 18:21:16.000000 codemodder-0.97.0/img/codemodder-dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11528 2024-04-30 18:21:16.000000 codemodder-0.97.0/img/codemodder-light.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-04-30 18:21:16.000000 codemodder-0.97.0/img/codemodder.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:21:25.776947 codemodder-0.97.0/integration_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:21:25.780947 codemodder-0.97.0/integration_tests/sonar/
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/sonar/test_sonar_break_or_continue_out_of_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/sonar/test_sonar_django_jmodel_without_dunder_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/sonar/test_sonar_django_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/sonar/test_sonar_django_receiver_on_top.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/sonar/test_sonar_exception_without_raise.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/sonar/test_sonar_fix_assert_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/sonar/test_sonar_fix_float_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/sonar/test_sonar_fix_math_isclose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/sonar/test_sonar_fix_missing_self_or_cls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/sonar/test_sonar_flask_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/sonar/test_sonar_jinja2_autoescape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/sonar/test_sonar_jwt_decode_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/sonar/test_sonar_literal_or_new_object_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/sonar/test_sonar_numpy_nan_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/sonar/test_sonar_remove_assertion_in_pytest_raises.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/sonar/test_sonar_secure_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/sonar/test_sonar_sql_parameterization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/sonar/test_sonar_tempfile_mktemp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/sonar/test_sonar_url_sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_add_requests_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_break_or_continue_out_of_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_combine_startswith_endswith.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_dependency_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_django_debug_flag_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_django_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_django_model_without_dunder_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_django_receiver_on_top.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_django_session_cookie_secure_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_exception_without_raise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_file_resource_leak.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_fix_assert_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_fix_dataclass_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_fix_deprecated_abstractproperty.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_fix_deprecated_logging_warn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_fix_empty_sequence_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_fix_float_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_fix_hasattr_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_fix_math_isclose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_fix_missing_self_or_cls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_fix_mutable_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_fix_task_instantiation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_flask_enable_csrf_protection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_flask_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_harden_pickle_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_harden_pyyaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_harden_ruamel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_https_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_jinja2_autoescape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_jwt_decode_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_lazy_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_limit_readline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_literal_or_new_object_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_lxml_safe_parser_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_lxml_safe_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_multiple_codemods.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_numpy_nan_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_order_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_process_sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_program.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_remove_assertion_in_pytest_raises.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_remove_debug_breakpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_remove_future_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_remove_module_global.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_remove_unused_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_replace_flask_send_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_request_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_secure_flask_cookie.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_secure_flask_session_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_secure_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_sql_parameterization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_str_concat_in_seq_literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_subprocess_shell_false.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_tempfile_mktemp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_unnecessary_f_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_upgrade_sslcontext_minimum_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_upgrade_sslcontext_tls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_url_sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_use_defusedxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_use_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_use_set_literal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_use_walrus_if.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-30 18:21:16.000000 codemodder-0.97.0/integration_tests/test_with_threading_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-30 18:21:16.000000 codemodder-0.97.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-30 18:21:16.000000 codemodder-0.97.0/renovate.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 18:21:25.840949 codemodder-0.97.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:21:25.760946 codemodder-0.97.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:21:25.780947 codemodder-0.97.0/src/codemodder/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-30 18:21:25.000000 codemodder-0.97.0/src/codemodder/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6143 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/code_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7953 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/codemodder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:21:25.784947 codemodder-0.97.0/src/codemodder/codemods/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/codemods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/codemods/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7916 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/codemods/base_codemod.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/codemods/base_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/codemods/base_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/codemods/base_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/codemods/check_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/codemods/codeql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/codemods/import_modifier_codemod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/codemods/imported_call_modifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11110 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/codemods/libcst_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/codemods/semgrep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:21:25.784947 codemodder-0.97.0/src/codemodder/codemods/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/codemods/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12743 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/codemods/test/integration_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/codemods/test/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/codemods/test/validations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:21:25.784947 codemodder-0.97.0/src/codemodder/codemods/transformations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/codemods/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16626 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/codemods/transformations/clean_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/codemods/transformations/remove_empty_string_concatenation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/codemods/transformations/remove_unused_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7879 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/codemods/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23960 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/codemods/utils_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/codeql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/codetf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7959 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5409 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/dependency.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:21:25.788947 codemodder-0.97.0/src/codemodder/dependency_management/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/dependency_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/dependency_management/base_dependency_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/dependency_management/codemod_dependencies.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/dependency_management/dependency_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/dependency_management/pyproject_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/dependency_management/requirements_txt_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6424 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/dependency_management/setup_py_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/dependency_management/setupcfg_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/file_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:21:25.788947 codemodder-0.97.0/src/codemodder/project_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/project_analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:21:25.788947 codemodder-0.97.0/src/codemodder/project_analysis/file_parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/project_analysis/file_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/project_analysis/file_parsers/base_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/project_analysis/file_parsers/package_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/project_analysis/file_parsers/pyproject_toml_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/project_analysis/file_parsers/requirements_txt_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/project_analysis/file_parsers/setup_cfg_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/project_analysis/file_parsers/setup_py_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/project_analysis/file_parsers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/project_analysis/python_repo_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/sarifs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:21:25.788947 codemodder-0.97.0/src/codemodder/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19673 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/scripts/generate_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/scripts/get_hashes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5291 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/semgrep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:21:25.788947 codemodder-0.97.0/src/codemodder/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/utils/abc_dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9967 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/utils/clean_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/utils/format_string_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8487 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/utils/linearize_string_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/codemodder/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:21:25.840949 codemodder-0.97.0/src/codemodder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    44701 2024-04-30 18:21:25.000000 codemodder-0.97.0/src/codemodder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22556 2024-04-30 18:21:25.000000 codemodder-0.97.0/src/codemodder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 18:21:25.000000 codemodder-0.97.0/src/codemodder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-30 18:21:25.000000 codemodder-0.97.0/src/codemodder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-30 18:21:25.000000 codemodder-0.97.0/src/codemodder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-30 18:21:25.000000 codemodder-0.97.0/src/codemodder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:21:25.800947 codemodder-0.97.0/src/core_codemods/
+-rw-r--r--   0 runner    (1001) docker     (127)     7609 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/add_requests_timeouts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:21:25.800947 codemodder-0.97.0/src/core_codemods/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/api/core_codemod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/break_or_continue_out_of_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/combine_startswith_endswith.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:21:25.800947 codemodder-0.97.0/src/core_codemods/defectdojo/
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/defectdojo/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/defectdojo/results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:21:25.800947 codemodder-0.97.0/src/core_codemods/defectdojo/semgrep/
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/defectdojo/semgrep/avoid_insecure_deserialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/defectdojo/semgrep/django_secure_set_cookie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/django_debug_flag_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/django_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/django_model_without_dunder_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/django_receiver_on_top.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/django_session_cookie_secure_off.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:21:25.808948 codemodder-0.97.0/src/core_codemods/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/defectdojo_python_avoid-insecure-deserialization.md
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/defectdojo_python_django-secure-set-cookie.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_add-requests-timeouts.md
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_bad-lock-with-statement.md
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_break-or-continue-out-of-loop.md
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_combine-startswith-endswith.md
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_django-debug-flag-on.md
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_django-json-response-type.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_django-model-without-dunder-str.md
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_django-receiver-on-top.md
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_django-session-cookie-secure-off.md
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_enable-jinja2-autoescape.md
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_exception-without-raise.md
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_fix-assert-tuple.md
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_fix-async-task-instantiation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_fix-dataclass-defaults.md
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_fix-deprecated-abstractproperty.md
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_fix-deprecated-logging-warn.md
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_fix-empty-sequence-comparison.md
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_fix-file-resource-leak.md
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_fix-float-equality.md
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_fix-hasattr-call.md
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_fix-math-isclose.md
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_fix-missing-self-or-cls.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_fix-mutable-params.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_flask-enable-csrf-protection.md
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_flask-json-response-type.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_harden-pickle-load.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_harden-pyyaml.md
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_harden-ruamel.md
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_https-connection.md
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_jwt-decode-verify.md
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_lazy-logging.md
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_limit-readline.md
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_literal-or-new-object-identity.md
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_numpy-nan-equality.md
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_remove-assertion-in-pytest-raises.md
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_remove-debug-breakpoint.md
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_remove-future-imports.md
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_remove-module-global.md
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_remove-unnecessary-f-str.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_replace-flask-send-file.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_requests-verify.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_safe-lxml-parser-defaults.md
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_safe-lxml-parsing.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_sandbox-process-creation.md
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_secure-flask-cookie.md
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_secure-flask-session-configuration.md
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_secure-random.md
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_secure-tempfile.md
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_sql-parameterization.md
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_str-concat-in-sequence-literals.md
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_subprocess-shell-false.md
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_unused-imports.md
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_upgrade-sslcontext-minimum-version.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_upgrade-sslcontext-tls.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_url-sandbox.md
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_use-defusedxml.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_use-generator.md
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_use-set-literal.md
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/docs/pixee_python_use-walrus-if.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/enable_jinja2_autoescape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/exception_without_raise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16005 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/file_resource_leak.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/fix_assert_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/fix_async_task_instantiation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/fix_dataclass_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/fix_deprecated_abstractproperty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/fix_deprecated_logging_warn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/fix_empty_sequence_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/fix_float_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/fix_hasattr_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/fix_math_isclose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/fix_missing_self_or_cls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8235 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/fix_mutable_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/flask_enable_csrf_protection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11313 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/flask_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/harden_pickle_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6951 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/harden_pyyaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/harden_ruamel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/https_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/jwt_decode_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7459 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/lazy_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/limit_readline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/literal_or_new_object_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/lxml_safe_parser_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/lxml_safe_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/numpy_nan_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/order_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/process_creation_sandbox.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:21:25.808948 codemodder-0.97.0/src/core_codemods/refactor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/refactor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10705 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/refactor/refactor_new_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/remove_assertion_in_pytest_raises.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/remove_debug_breakpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/remove_future_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/remove_module_global.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/remove_unnecessary_f_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/remove_unused_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/replace_flask_send_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/requests_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/secure_cookie_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/secure_flask_cookie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8216 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/secure_flask_session_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/secure_random.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:21:25.812948 codemodder-0.97.0/src/core_codemods/sonar/
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/sonar/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/sonar/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/sonar/sonar_break_or_continue_out_of_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/sonar/sonar_django_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/sonar/sonar_django_model_without_dunder_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/sonar/sonar_django_receiver_on_top.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/sonar/sonar_enable_jinja2_autoescape.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/sonar/sonar_exception_without_raise.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/sonar/sonar_fix_assert_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/sonar/sonar_fix_float_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/sonar/sonar_fix_math_isclose.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/sonar/sonar_fix_missing_self_or_cls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/sonar/sonar_flask_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/sonar/sonar_jwt_decode_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/sonar/sonar_literal_or_new_object_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/sonar/sonar_numpy_nan_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/sonar/sonar_remove_assertion_in_pytest_raises.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/sonar/sonar_secure_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/sonar/sonar_sql_parameterization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/sonar/sonar_tempfile_mktemp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/sonar/sonar_url_sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22996 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/sql_parameterization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/str_concat_in_seq_literal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/subprocess_shell_false.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/tempfile_mktemp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/upgrade_sslcontext_minimum_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/upgrade_sslcontext_tls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7189 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/url_sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/use_defused_xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/use_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/use_set_literal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8037 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/use_walrus_if.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-30 18:21:16.000000 codemodder-0.97.0/src/core_codemods/with_threading_lock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:21:25.816948 codemodder-0.97.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:21:25.824948 codemodder-0.97.0/tests/codemods/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:21:25.760946 codemodder-0.97.0/tests/codemods/defectdojo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:21:25.824948 codemodder-0.97.0/tests/codemods/defectdojo/semgrep/
+-rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/defectdojo/semgrep/test_avoid_insecure_deserialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/defectdojo/semgrep/test_django_secure_set_cookie.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:21:25.828948 codemodder-0.97.0/tests/codemods/sonar/
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/sonar/test_sonar_break_or_continue_out_of_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/sonar/test_sonar_django_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/sonar/test_sonar_django_model_without_dunder_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/sonar/test_sonar_django_receiver_on_top.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/sonar/test_sonar_enable_jinja2_autoescape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/sonar/test_sonar_exception_without_raise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/sonar/test_sonar_fix_assert_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/sonar/test_sonar_fix_float_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/sonar/test_sonar_fix_math_isclose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/sonar/test_sonar_fix_missing_self_or_cls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/sonar/test_sonar_flask_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/sonar/test_sonar_jwt_decode_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/sonar/test_sonar_literal_or_new_object_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/sonar/test_sonar_numpy_nan_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/sonar/test_sonar_remove_assertion_in_pytest_raises.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/sonar/test_sonar_secure_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/sonar/test_sonar_sql_parameterization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/sonar/test_sonar_tempfile_mktemp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/sonar/test_sonar_url_sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_add_requests_timeouts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7831 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_async_fix_task_instantiation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_base_codemod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6056 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_base_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_break_or_continue_out_of_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_combine_startswith_endswith.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_django_debug_flag_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_django_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_django_model_without_dunder_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_django_receiver_on_top.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_django_session_cookie_secure_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6891 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_enable_jinja2_autoescape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_exception_without_raise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_file_resource_leak.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_fix_assert_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_fix_dataclass_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_fix_deprecated_abstractproperty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_fix_deprecated_logging_warn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11617 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_fix_empty_sequence_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_fix_float_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_fix_hasattr_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_fix_math_isclose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_fix_missing_self_or_cls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9896 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_fix_mutable_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_flask_enable_csrf_protection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_flask_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_harden_pickle_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_harden_pyyaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_harden_ruamel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_https_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_include_exclude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_jwt_decode_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23745 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_lazy_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_limit_readline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_literal_or_new_object_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_lxml_safe_parameter_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_lxml_safe_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_numpy_nan_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_order_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_process_creation_sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_remove_assertion_in_pytest_raises.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_remove_debug_breakpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_remove_future_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_remove_module_global.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_remove_unnecessary_f_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_remove_unused_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_replace_flask_send_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7348 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_request_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_secure_flask_cookie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7704 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_secure_flask_session_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_secure_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16046 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_sql_parameterization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_str_concat_in_seq_literal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_subprocess_shell_false.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_tempfile_mktemp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_upgrade_sslcontext_minimum_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_upgrade_sslcontext_tls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6772 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_url_sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4835 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_use_defused_xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_use_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_use_set_literal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8036 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_walrus_if.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/codemods/test_with_threading_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:21:25.828948 codemodder-0.97.0/tests/dependency_management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/dependency_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/dependency_management/test_base_dependency_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/dependency_management/test_dependency_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/dependency_management/test_pyproject_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/dependency_management/test_requirements_txt_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13718 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/dependency_management/test_setup_py_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9072 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/dependency_management/test_setupcfgt_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:21:25.828948 codemodder-0.97.0/tests/project_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/project_analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:21:25.828948 codemodder-0.97.0/tests/project_analysis/file_parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/project_analysis/file_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/project_analysis/file_parsers/test_pyproject_toml_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/project_analysis/file_parsers/test_requirements_txt_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/project_analysis/file_parsers/test_setup_cfg_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/project_analysis/file_parsers/test_setup_py_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/project_analysis/test_python_repo_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:21:25.836948 codemodder-0.97.0/tests/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/samples/break_or_continue_out_of_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/samples/django_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/samples/django_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/samples/django_receiver_on_top.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/samples/exception_without_raise.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/samples/fix_assert_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/samples/fix_float_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/samples/fix_math_isclose.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/samples/fix_missing_self_or_cls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/samples/fix_sonar_sql_parameterization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/samples/flask_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/samples/flask_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/samples/jinja2_autoescape.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/samples/jwt_decode_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/samples/literal_or_new_object_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/samples/make_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/samples/multiple_codemods.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/samples/numpy_nan_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)  2680067 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/samples/pygoat.semgrep.sarif.json
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/samples/remove_assertion_in_pytest_raises.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/samples/secure_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/samples/semgrep.sarif
+-rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/samples/sonar_hotspots.json
+-rw-r--r--   0 runner    (1001) docker     (127)    90652 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/samples/sonar_issues.json
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/samples/tempfile_mktemp.py
+-rw-r--r--   0 runner    (1001) docker     (127)   451117 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/samples/webgoat_v8.2.0_codeql.sarif
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/test_ancestorpatterns_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/test_basetype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5628 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/test_code_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/test_codemod_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11991 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/test_codemodder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/test_codeql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/test_codetf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/test_file_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/test_format_string_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/test_libcst_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/test_linearize_string_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6302 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/test_nameresolution_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/test_sarif_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/test_semgrep.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:21:25.840949 codemodder-0.97.0/tests/transformations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/transformations/test_clean_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/transformations/test_remove_empty_string_concatenation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-30 18:21:16.000000 codemodder-0.97.0/tests/transformations/test_remove_unused_imports.py
```

### Comparing `codemodder-0.96.0/.github/workflows/autoformat-pixeebot-prs.yaml` & `codemodder-0.97.0/.github/workflows/autoformat-pixeebot-prs.yaml`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/.github/workflows/codemod_pygoat.yml` & `codemodder-0.97.0/.github/workflows/codemod_pygoat.yml`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/.github/workflows/deploy_to_pypi.yml` & `codemodder-0.97.0/.github/workflows/deploy_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/.github/workflows/integration_test.yml` & `codemodder-0.97.0/.github/workflows/integration_test.yml`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/.github/workflows/lint.yml` & `codemodder-0.97.0/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/.github/workflows/pre-commit-autoupdate.yml` & `codemodder-0.97.0/.github/workflows/pre-commit-autoupdate.yml`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/.github/workflows/sonar_pixee.yml` & `codemodder-0.97.0/.github/workflows/sonar_pixee.yml`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/.github/workflows/test.yml` & `codemodder-0.97.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/.gitignore` & `codemodder-0.97.0/.gitignore`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/.pre-commit-config.yaml` & `codemodder-0.97.0/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -15,23 +15,23 @@
           )$
     -   id: check-added-large-files
         exclude: |
           (?x)^(
               tests/samples/pygoat.semgrep.sarif.json
           )$
 -   repo: https://github.com/psf/black
-    rev: 24.4.0
+    rev: 24.4.2
     hooks:
     -   id: black
         exclude: |
           (?x)^(
               tests/samples/.*|
           )$
 - repo: https://github.com/pre-commit/mirrors-mypy
-  rev: v1.9.0
+  rev: v1.10.0
   hooks:
    - id: mypy
      exclude: |
        (?x)^(
            tests/samples/.*|
            integration_tests/.*
        )$
@@ -41,15 +41,15 @@
          "types-jsonschema~=4.21.0",
          "types-mock==5.0.*",
          "types-PyYAML==6.0",
          "types-toml~=0.10",
          "types-requests~=2.13",
     ]
 - repo: https://github.com/astral-sh/ruff-pre-commit
-  rev: v0.4.1
+  rev: v0.4.2
   hooks:
     - id: ruff
       exclude: tests/samples/
     # todo: replace black with this?
     # Run the formatter.
     # - id: ruff-format
 - repo: https://github.com/pycqa/isort
```

### Comparing `codemodder-0.96.0/CHANGELOG.md` & `codemodder-0.97.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/CONTRIBUTING.md` & `codemodder-0.97.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/LICENSE` & `codemodder-0.97.0/LICENSE`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/Makefile` & `codemodder-0.97.0/Makefile`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/PKG-INFO` & `codemodder-0.97.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codemodder
-Version: 0.96.0
+Version: 0.97.0
 Summary: A pluggable framework for building codemods in Python
 Author-email: Pixee <python@pixee.ai>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -697,15 +697,15 @@
 Requires-Dist: Flask<4; extra == "test"
 Requires-Dist: Jinja2~=3.1.2; extra == "test"
 Requires-Dist: jsonschema~=4.21.0; extra == "test"
 Requires-Dist: lxml<5.3.0,>=4.9.3; extra == "test"
 Requires-Dist: mock==5.1.*; extra == "test"
 Requires-Dist: pre-commit<4; extra == "test"
 Requires-Dist: Pyjwt~=2.8.0; extra == "test"
-Requires-Dist: pytest<8.2,>=7.4; extra == "test"
+Requires-Dist: pytest<9,>=8.2; extra == "test"
 Requires-Dist: pytest-cov<5.1,>=4.1; extra == "test"
 Requires-Dist: pytest-mock<3.15,>=3.12; extra == "test"
 Requires-Dist: pytest-randomly==3.*; extra == "test"
 Requires-Dist: pytest-xdist==3.*; extra == "test"
 Requires-Dist: requests~=2.31.0; extra == "test"
 Requires-Dist: security~=1.2.0; extra == "test"
 Requires-Dist: types-mock==5.1.*; extra == "test"
@@ -713,15 +713,15 @@
 Requires-Dist: numpy~=1.26.0; extra == "test"
 Requires-Dist: flask_wtf~=1.2.0; extra == "test"
 Requires-Dist: fickling>=0.1.3,~=0.1.0; extra == "test"
 Provides-Extra: complexity
 Requires-Dist: radon==6.0.*; extra == "complexity"
 Requires-Dist: xenon==0.9.*; extra == "complexity"
 Provides-Extra: openai
-Requires-Dist: openai<1.24,>=1.0; extra == "openai"
+Requires-Dist: openai<1.25,>=1.0; extra == "openai"
 Provides-Extra: all
 Requires-Dist: codemodder[test]; extra == "all"
 Requires-Dist: codemodder[complexity]; extra == "all"
 
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="img/codemodder-dark.png">
   <source media="(prefers-color-scheme: light)" srcset="img/codemodder-light.png">
```

### Comparing `codemodder-0.96.0/README.md` & `codemodder-0.97.0/README.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/ci_tests/test_pygoat_findings.py` & `codemodder-0.97.0/ci_tests/test_pygoat_findings.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/img/base-codemod.jpg` & `codemodder-0.97.0/img/base-codemod.jpg`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/img/codemodder-dark.png` & `codemodder-0.97.0/img/codemodder-dark.png`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/img/codemodder-light.png` & `codemodder-0.97.0/img/codemodder-light.png`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/img/codemodder.png` & `codemodder-0.97.0/img/codemodder.png`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/sonar/test_sonar_django_jmodel_without_dunder_str.py` & `codemodder-0.97.0/integration_tests/sonar/test_sonar_django_jmodel_without_dunder_str.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,36 +7,36 @@
 )
 
 
 class TestSonarDjangoModelWithoutDunderStr(SonarIntegrationTest):
     codemod = SonarDjangoModelWithoutDunderStr
     code_path = "tests/samples/django_model.py"
     replacement_lines = [
-        (15, """\n"""),
-        (16, """    def __str__(self):\n"""),
-        (17, """        model_name = self.__class__.__name__\n"""),
+        (16, """\n"""),
+        (17, """    def __str__(self):\n"""),
+        (18, """        model_name = self.__class__.__name__\n"""),
         (
-            18,
+            19,
             """        fields_str = ", ".join((f"{field.name}={getattr(self, field.name)}" for field in self._meta.fields))\n""",
         ),
-        (19, """        return f"{model_name}({fields_str})"\n"""),
+        (20, """        return f"{model_name}({fields_str})"\n"""),
     ]
 
     # fmt: off
     expected_diff = (
     """--- \n"""
     """+++ \n"""
-    """@@ -12,3 +12,8 @@\n"""
+    """@@ -13,3 +13,8 @@\n"""
     """     phone = models.IntegerField(blank=True)\n"""
     """     class Meta:\n"""
     """         app_label = 'myapp'\n"""
     """+\n"""
     """+    def __str__(self):\n"""
     """+        model_name = self.__class__.__name__\n"""
     """+        fields_str = ", ".join((f"{field.name}={getattr(self, field.name)}" for field in self._meta.fields))\n"""
     """+        return f"{model_name}({fields_str})"\n"""
     )
     # fmt: on
 
-    expected_line_change = "10"
+    expected_line_change = "11"
     change_description = DjangoModelWithoutDunderStrTransformer.change_description
     num_changed_files = 1
```

### Comparing `codemodder-0.96.0/integration_tests/sonar/test_sonar_django_json_response_type.py` & `codemodder-0.97.0/integration_tests/sonar/test_sonar_django_json_response_type.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/sonar/test_sonar_django_receiver_on_top.py` & `codemodder-0.97.0/integration_tests/sonar/test_sonar_django_receiver_on_top.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/sonar/test_sonar_exception_without_raise.py` & `codemodder-0.97.0/integration_tests/sonar/test_sonar_exception_without_raise.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/sonar/test_sonar_fix_assert_tuple.py` & `codemodder-0.97.0/integration_tests/sonar/test_sonar_fix_assert_tuple.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/sonar/test_sonar_fix_float_equality.py` & `codemodder-0.97.0/integration_tests/sonar/test_sonar_fix_float_equality.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/sonar/test_sonar_fix_math_isclose.py` & `codemodder-0.97.0/integration_tests/sonar/test_sonar_fix_math_isclose.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/sonar/test_sonar_fix_missing_self_or_cls.py` & `codemodder-0.97.0/integration_tests/sonar/test_sonar_fix_missing_self_or_cls.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/sonar/test_sonar_flask_json_response_type.py` & `codemodder-0.97.0/integration_tests/sonar/test_sonar_flask_json_response_type.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/sonar/test_sonar_jinja2_autoescape.py` & `codemodder-0.97.0/integration_tests/sonar/test_sonar_jinja2_autoescape.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/sonar/test_sonar_jwt_decode_verify.py` & `codemodder-0.97.0/integration_tests/sonar/test_sonar_jwt_decode_verify.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/sonar/test_sonar_literal_or_new_object_identity.py` & `codemodder-0.97.0/integration_tests/sonar/test_sonar_literal_or_new_object_identity.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/sonar/test_sonar_numpy_nan_equality.py` & `codemodder-0.97.0/integration_tests/sonar/test_sonar_numpy_nan_equality.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/sonar/test_sonar_remove_assertion_in_pytest_raises.py` & `codemodder-0.97.0/integration_tests/sonar/test_sonar_remove_assertion_in_pytest_raises.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/sonar/test_sonar_secure_random.py` & `codemodder-0.97.0/integration_tests/sonar/test_sonar_secure_random.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/sonar/test_sonar_sql_parameterization.py` & `codemodder-0.97.0/integration_tests/sonar/test_sonar_sql_parameterization.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/sonar/test_sonar_tempfile_mktemp.py` & `codemodder-0.97.0/integration_tests/sonar/test_sonar_tempfile_mktemp.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/sonar/test_sonar_url_sandbox.py` & `codemodder-0.97.0/integration_tests/sonar/test_sonar_url_sandbox.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_add_requests_timeout.py` & `codemodder-0.97.0/integration_tests/test_add_requests_timeout.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_combine_startswith_endswith.py` & `codemodder-0.97.0/integration_tests/test_combine_startswith_endswith.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_dependency_manager.py` & `codemodder-0.97.0/integration_tests/test_dependency_manager.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_django_debug_flag_on.py` & `codemodder-0.97.0/integration_tests/test_django_debug_flag_on.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_django_json_response_type.py` & `codemodder-0.97.0/integration_tests/test_django_json_response_type.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_django_model_without_dunder_str.py` & `codemodder-0.97.0/integration_tests/test_django_model_without_dunder_str.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,53 +8,54 @@
 class TestDjangoModelWithoutDunderStr(BaseIntegrationTest):
     codemod = DjangoModelWithoutDunderStr
     original_code = """
     import django
     from django.conf import settings
     from django.db import models
     # required to run this module standalone for testing
-    settings.configure()
+    if not settings.configured:
+        settings.configure()
     django.setup()
     
     
     class Message(models.Model):
         author = models.CharField(max_length=100)
         content = models.CharField(max_length=200)
         class Meta:
             app_label = 'myapp'
 
     """
     replacement_lines = [
-        (15, """\n"""),
-        (16, """    def __str__(self):\n"""),
-        (17, """        model_name = self.__class__.__name__\n"""),
+        (16, """\n"""),
+        (17, """    def __str__(self):\n"""),
+        (18, """        model_name = self.__class__.__name__\n"""),
         (
-            18,
+            19,
             """        fields_str = ", ".join((f"{field.name}={getattr(self, field.name)}" for field in self._meta.fields))\n""",
         ),
-        (19, """        return f"{model_name}({fields_str})"\n"""),
+        (20, """        return f"{model_name}({fields_str})"\n"""),
     ]
 
     # fmt: off
     expected_diff = (
     """--- \n"""
     """+++ \n"""
-    """@@ -11,3 +11,8 @@\n"""
+    """@@ -12,3 +12,8 @@\n"""
     """     content = models.CharField(max_length=200)\n"""
     """     class Meta:\n"""
     """         app_label = 'myapp'\n"""
     """+\n"""
     """+    def __str__(self):\n"""
     """+        model_name = self.__class__.__name__\n"""
     """+        fields_str = ", ".join((f"{field.name}={getattr(self, field.name)}" for field in self._meta.fields))\n"""
     """+        return f"{model_name}({fields_str})"\n"""
     )
     # fmt: on
 
-    expected_line_change = "9"
+    expected_line_change = "10"
     change_description = DjangoModelWithoutDunderStrTransformer.change_description
     num_changed_files = 1
 
     def check_code_after(self):
         """Executes models.py and instantiates the model to ensure expected str representation"""
         module = super().check_code_after()
         inst = module.Message(pk=1, author="name", content="content")
```

### Comparing `codemodder-0.96.0/integration_tests/test_django_receiver_on_top.py` & `codemodder-0.97.0/integration_tests/test_django_receiver_on_top.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_django_session_cookie_secure_off.py` & `codemodder-0.97.0/integration_tests/test_django_session_cookie_secure_off.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_exception_without_raise.py` & `codemodder-0.97.0/integration_tests/test_exception_without_raise.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_file_resource_leak.py` & `codemodder-0.97.0/integration_tests/test_file_resource_leak.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_fix_assert_tuple.py` & `codemodder-0.97.0/integration_tests/test_fix_assert_tuple.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_fix_dataclass_defaults.py` & `codemodder-0.97.0/integration_tests/test_fix_dataclass_defaults.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_fix_deprecated_abstractproperty.py` & `codemodder-0.97.0/integration_tests/test_fix_deprecated_abstractproperty.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_fix_deprecated_logging_warn.py` & `codemodder-0.97.0/integration_tests/test_fix_deprecated_logging_warn.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_fix_empty_sequence_comparison.py` & `codemodder-0.97.0/integration_tests/test_fix_empty_sequence_comparison.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_fix_float_equality.py` & `codemodder-0.97.0/integration_tests/test_fix_float_equality.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_fix_hasattr_call.py` & `codemodder-0.97.0/integration_tests/test_fix_hasattr_call.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_fix_math_isclose.py` & `codemodder-0.97.0/integration_tests/test_fix_math_isclose.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_fix_missing_self_or_cls.py` & `codemodder-0.97.0/integration_tests/test_fix_missing_self_or_cls.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_fix_mutable_params.py` & `codemodder-0.97.0/integration_tests/test_fix_mutable_params.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_fix_task_instantiation.py` & `codemodder-0.97.0/integration_tests/test_fix_task_instantiation.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_flask_enable_csrf_protection.py` & `codemodder-0.97.0/integration_tests/test_flask_enable_csrf_protection.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_flask_json_response_type.py` & `codemodder-0.97.0/integration_tests/test_flask_json_response_type.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_harden_pickle_load.py` & `codemodder-0.97.0/integration_tests/test_harden_pickle_load.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_harden_pyyaml.py` & `codemodder-0.97.0/integration_tests/test_harden_pyyaml.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_harden_ruamel.py` & `codemodder-0.97.0/integration_tests/test_harden_ruamel.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_https_connection.py` & `codemodder-0.97.0/integration_tests/test_https_connection.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_jinja2_autoescape.py` & `codemodder-0.97.0/integration_tests/test_jinja2_autoescape.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_jwt_decode_verify.py` & `codemodder-0.97.0/integration_tests/test_jwt_decode_verify.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_lazy_logging.py` & `codemodder-0.97.0/integration_tests/test_lazy_logging.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_limit_readline.py` & `codemodder-0.97.0/integration_tests/test_limit_readline.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_literal_or_new_object_identity.py` & `codemodder-0.97.0/integration_tests/test_literal_or_new_object_identity.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_lxml_safe_parser_defaults.py` & `codemodder-0.97.0/integration_tests/test_lxml_safe_parser_defaults.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_lxml_safe_parsing.py` & `codemodder-0.97.0/integration_tests/test_lxml_safe_parsing.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_multiple_codemods.py` & `codemodder-0.97.0/integration_tests/test_multiple_codemods.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_numpy_nan_equality.py` & `codemodder-0.97.0/integration_tests/test_numpy_nan_equality.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_order_imports.py` & `codemodder-0.97.0/integration_tests/test_order_imports.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_process_sandbox.py` & `codemodder-0.97.0/integration_tests/test_process_sandbox.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_program.py` & `codemodder-0.97.0/integration_tests/test_program.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_remove_assertion_in_pytest_raises.py` & `codemodder-0.97.0/integration_tests/test_remove_assertion_in_pytest_raises.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_remove_debug_breakpoint.py` & `codemodder-0.97.0/integration_tests/test_remove_debug_breakpoint.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_remove_future_imports.py` & `codemodder-0.97.0/integration_tests/test_remove_future_imports.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_remove_module_global.py` & `codemodder-0.97.0/integration_tests/test_remove_module_global.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_remove_unused_imports.py` & `codemodder-0.97.0/integration_tests/test_remove_unused_imports.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_replace_flask_send_file.py` & `codemodder-0.97.0/integration_tests/test_replace_flask_send_file.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_request_verify.py` & `codemodder-0.97.0/integration_tests/test_request_verify.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_secure_flask_cookie.py` & `codemodder-0.97.0/integration_tests/test_secure_flask_cookie.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_secure_flask_session_config.py` & `codemodder-0.97.0/integration_tests/test_secure_flask_session_config.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_secure_random.py` & `codemodder-0.97.0/integration_tests/test_secure_random.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_sql_parameterization.py` & `codemodder-0.97.0/integration_tests/test_sql_parameterization.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_str_concat_in_seq_literals.py` & `codemodder-0.97.0/integration_tests/test_str_concat_in_seq_literals.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_subprocess_shell_false.py` & `codemodder-0.97.0/integration_tests/test_subprocess_shell_false.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_tempfile_mktemp.py` & `codemodder-0.97.0/integration_tests/test_tempfile_mktemp.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_unnecessary_f_str.py` & `codemodder-0.97.0/integration_tests/test_unnecessary_f_str.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_upgrade_sslcontext_minimum_version.py` & `codemodder-0.97.0/integration_tests/test_upgrade_sslcontext_minimum_version.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_upgrade_sslcontext_tls.py` & `codemodder-0.97.0/integration_tests/test_upgrade_sslcontext_tls.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_url_sandbox.py` & `codemodder-0.97.0/integration_tests/test_url_sandbox.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_use_defusedxml.py` & `codemodder-0.97.0/integration_tests/test_use_defusedxml.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_use_generator.py` & `codemodder-0.97.0/integration_tests/test_use_generator.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_use_set_literal.py` & `codemodder-0.97.0/integration_tests/test_use_set_literal.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_use_walrus_if.py` & `codemodder-0.97.0/integration_tests/test_use_walrus_if.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/integration_tests/test_with_threading_lock.py` & `codemodder-0.97.0/integration_tests/test_with_threading_lock.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/pyproject.toml` & `codemodder-0.97.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     "Flask<4",
     "Jinja2~=3.1.2",
     "jsonschema~=4.21.0",
     "lxml>=4.9.3,<5.3.0",
     "mock==5.1.*",
     "pre-commit<4",
     "Pyjwt~=2.8.0",
-    "pytest>=7.4,<8.2",
+    "pytest>=8.2,<9",
     "pytest-cov>=4.1,<5.1",
     "pytest-mock>=3.12,<3.15",
     "pytest-randomly==3.*",
     "pytest-xdist==3.*",
     "requests~=2.31.0",
     "security~=1.2.0",
     "types-mock==5.1.*",
@@ -70,28 +70,29 @@
     "fickling~=0.1.0,>=0.1.3",
 ]
 complexity = [
     "radon==6.0.*",
     "xenon==0.9.*",
 ]
 openai = [
-    "openai>=1.0,<1.24",
+    "openai>=1.0,<1.25",
 ]
 all = [
     "codemodder[test]",
     "codemodder[complexity]",
 ]
 
 [project.entry-points.codemods]
 core = "core_codemods:registry"
 sonar = "core_codemods:sonar_registry"
 defectdojo = "core_codemods:defectdojo_registry"
 
 [project.entry-points.sarif_detectors]
 "semgrep" = "codemodder.semgrep:SemgrepSarifToolDetector"
+"codeql" = "codemodder.codeql:CodeQLSarifToolDetector"
 
 [tool.setuptools]
 
 [tool.setuptools.package-data]
 "core_codemods.semgrep" = ["src/core_codemods/semgrep/*.yaml"]
 "core_codemods.docs" = ["src/core_codemods/docs/*.md"]
```

### Comparing `codemodder-0.96.0/src/codemodder/cli.py` & `codemodder-0.97.0/src/codemodder/cli.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/codemodder/code_directory.py` & `codemodder-0.97.0/src/codemodder/code_directory.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/codemodder/codemodder.py` & `codemodder-0.97.0/src/codemodder/codemodder.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,25 +32,26 @@
 
 def find_semgrep_results(
     context: CodemodExecutionContext,
     codemods: Sequence[BaseCodemod],
     files_to_analyze: list[Path] | None = None,
 ) -> ResultSet:
     """Run semgrep once with all configuration files from all codemods and return a set of applicable rule IDs"""
-    yaml_files = list(
-        itertools.chain.from_iterable(
-            [
-                codemod.detector.get_yaml_files(codemod.name)
-                for codemod in codemods
-                if codemod.detector
-                and isinstance(codemod.detector, SemgrepRuleDetector)
-            ]
+    if not (
+        yaml_files := list(
+            itertools.chain.from_iterable(
+                [
+                    codemod.detector.get_yaml_files(codemod.name)
+                    for codemod in codemods
+                    if codemod.detector
+                    and isinstance(codemod.detector, SemgrepRuleDetector)
+                ]
+            )
         )
-    )
-    if not yaml_files:
+    ):
         return ResultSet()
 
     return run_semgrep(context, yaml_files, files_to_analyze)
 
 
 def log_report(context, argv, elapsed_ms, files_to_analyze):
     log_section("report")
```

### Comparing `codemodder-0.96.0/src/codemodder/codemods/api.py` & `codemodder-0.97.0/src/codemodder/codemods/api.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/codemodder/codemods/base_codemod.py` & `codemodder-0.97.0/src/codemodder/codemods/base_codemod.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,7 +247,10 @@
 
         if change_set := self.transformer.apply(
             context, file_context, findings_for_rule
         ):
             file_context.add_changeset(change_set)
 
         return file_context
+
+    def __repr__(self) -> str:
+        return f"{self.id}"
```

### Comparing `codemodder-0.96.0/src/codemodder/codemods/base_transformer.py` & `codemodder-0.97.0/src/codemodder/codemods/base_transformer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/codemodder/codemods/base_visitor.py` & `codemodder-0.97.0/src/codemodder/codemods/base_visitor.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/codemodder/codemods/check_annotations.py` & `codemodder-0.97.0/src/codemodder/codemods/check_annotations.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/codemodder/codemods/import_modifier_codemod.py` & `codemodder-0.97.0/src/codemodder/codemods/import_modifier_codemod.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/codemodder/codemods/imported_call_modifier.py` & `codemodder-0.97.0/src/codemodder/codemods/imported_call_modifier.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/codemodder/codemods/libcst_transformer.py` & `codemodder-0.97.0/src/codemodder/codemods/libcst_transformer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/codemodder/codemods/semgrep.py` & `codemodder-0.97.0/src/codemodder/codemods/semgrep.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/codemodder/codemods/test/integration_utils.py` & `codemodder-0.97.0/src/codemodder/codemods/test/integration_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,36 +84,34 @@
         pathlib.Path(cls.code_path).unlink(missing_ok=True)
 
         if cls.requirements_file_name:
             pathlib.Path(cls.dependency_path).unlink(missing_ok=True)
 
     def setup_method(self):
         try:
-            name = (
-                self.codemod().name
-                if isinstance(self.codemod, type)
-                else self.codemod.name
+            codemod_id = (
+                self.codemod().id if isinstance(self.codemod, type) else self.codemod.id
             )
             # This is how we ensure that the codemod is actually in the registry
             self.codemod_instance = self.codemod_registry.match_codemods(
-                codemod_include=[name]
+                codemod_include=[codemod_id]
             )[0]
         except IndexError as exc:
             raise IndexError(
                 "You must register the codemod to a CodemodCollection."
             ) from exc
 
     def _assert_run_fields(self, run, output_path):
         assert run["vendor"] == "pixee"
         assert run["tool"] == "codemodder-python"
         assert run["version"] == __version__
         assert run["elapsed"] != ""
         assert run[
             "commandLine"
-        ] == f'codemodder {self.code_dir} --output {output_path} --codemod-include={self.codemod_instance.name} --path-include={self.code_filename} --path-exclude=""' + (
+        ] == f'codemodder {self.code_dir} --output {output_path} --codemod-include={self.codemod_instance.id} --path-include={self.code_filename} --path-exclude=""' + (
             f" --sonar-issues-json={self.sonar_issues_json}"
             if self.sonar_issues_json
             else ""
         ) + (
             f" --sonar-hotspots-json={self.sonar_hotspots_json}"
             if self.sonar_hotspots_json
             else ""
@@ -194,15 +192,15 @@
         output files
         """
         command = [
             "codemodder",
             self.code_dir,
             "--output",
             self.output_path,
-            f"--codemod-include={self.codemod_instance.name}",
+            f"--codemod-include={self.codemod_instance.id}",
             f"--path-include={self.code_filename}",
             '--path-exclude=""',
         ]
 
         if self.sonar_issues_json:
             command.append(f"--sonar-issues-json={self.sonar_issues_json}")
         if self.sonar_hotspots_json:
```

### Comparing `codemodder-0.96.0/src/codemodder/codemods/test/utils.py` & `codemodder-0.97.0/src/codemodder/codemods/test/utils.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/codemodder/codemods/test/validations.py` & `codemodder-0.97.0/src/codemodder/codemods/test/validations.py`

 * *Files 20% similar despite different names*

```diff
@@ -22,16 +22,15 @@
 def _run_code(path, allowed_exceptions=None) -> Optional[ModuleType]:
     """
     Execute the code in `path` in its own namespace.
     Return loaded module for any additional testing later on.
     """
     allowed_exceptions = allowed_exceptions or ()
 
-    spec = importlib.util.spec_from_file_location("output_code", path)
-    if not spec:
+    if not (spec := importlib.util.spec_from_file_location("output_code", path)):
         return None
 
     module = importlib.util.module_from_spec(spec)
     if not spec.loader:
         return None
     try:
         spec.loader.exec_module(module)
```

### Comparing `codemodder-0.96.0/src/codemodder/codemods/transformations/clean_imports.py` & `codemodder-0.97.0/src/codemodder/codemods/transformations/clean_imports.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/codemodder/codemods/transformations/remove_empty_string_concatenation.py` & `codemodder-0.97.0/src/codemodder/codemods/transformations/remove_empty_string_concatenation.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/codemodder/codemods/transformations/remove_unused_imports.py` & `codemodder-0.97.0/src/codemodder/codemods/transformations/remove_unused_imports.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/codemodder/codemods/utils.py` & `codemodder-0.97.0/src/codemodder/codemods/utils.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/codemodder/codemods/utils_mixin.py` & `codemodder-0.97.0/src/codemodder/codemods/utils_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,27 +135,37 @@
                             if maybe_assignment.name in (
                                 alias.evaluated_alias,
                                 alias.evaluated_name,
                             ):
                                 return (import_node, alias)
         return None
 
+    def get_aliased_prefix_name_from_import(
+        self, import_alias: cst.ImportAlias, name: str
+    ) -> Optional[str]:
+        """
+        Returns the alias name, otherwise just name, of the given import if its name matches name.
+        """
+        maybe_name = None
+        if (imp_name := get_full_name_for_node(import_alias.name)) == name:
+            # AsName is always a Name for ImportAlias
+            maybe_name = (
+                import_alias.asname.name.value if import_alias.asname else imp_name
+            )
+        return maybe_name
+
     def get_aliased_prefix_name(self, node: cst.CSTNode, name: str) -> Optional[str]:
         """
-        Returns the alias of name if name is imported and used as a prefix for this node.
+        Returns the alias of name, or just name itself, if name is imported and used as a prefix for this node.
         """
         maybe_import = self.get_imported_prefix(node)
-        maybe_name = None
         if maybe_import and matchers.matches(maybe_import[0], matchers.Import()):
             _, ia = maybe_import
-            imp_name = get_full_name_for_node(ia.name)
-            if imp_name == name and ia.asname:
-                # AsName is always a Name for ImportAlias
-                maybe_name = ia.asname.name.value
-        return maybe_name
+            return self.get_aliased_prefix_name_from_import(ia, name)
+        return None
 
     def find_assignments(
         self,
         node: Union[cst.Name, cst.Attribute, cst.Call, cst.Subscript, cst.Decorator],
     ) -> set[BaseAssignment]:
         """
         Given a MetadataWrapper and a CSTNode with a possible access to it, find all the possible assignments that it refers.
```

### Comparing `codemodder-0.96.0/src/codemodder/codetf.py` & `codemodder-0.97.0/src/codemodder/codetf.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/codemodder/context.py` & `codemodder-0.97.0/src/codemodder/context.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/codemodder/dependency.py` & `codemodder-0.97.0/src/codemodder/dependency.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/codemodder/dependency_management/base_dependency_writer.py` & `codemodder-0.97.0/src/codemodder/dependency_management/base_dependency_writer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/codemodder/dependency_management/dependency_manager.py` & `codemodder-0.97.0/src/codemodder/dependency_management/dependency_manager.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/codemodder/dependency_management/pyproject_writer.py` & `codemodder-0.97.0/src/codemodder/dependency_management/pyproject_writer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/codemodder/dependency_management/requirements_txt_writer.py` & `codemodder-0.97.0/src/codemodder/dependency_management/requirements_txt_writer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/codemodder/dependency_management/setup_py_writer.py` & `codemodder-0.97.0/src/codemodder/dependency_management/setup_py_writer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/codemodder/dependency_management/setupcfg_writer.py` & `codemodder-0.97.0/src/codemodder/dependency_management/setupcfg_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,18 +36,19 @@
         ):
             logger.debug("Unable to add dependencies to setup.cfg file.")
             return None
 
         with open(self.path, "r", encoding="utf-8") as f:
             original_lines = f.readlines()
 
-        new_lines = self.build_new_lines(
-            original_lines, defined_dependencies, dependencies
-        )
-        if not new_lines:
+        if not (
+            new_lines := self.build_new_lines(
+                original_lines, defined_dependencies, dependencies
+            )
+        ):
             logger.debug("Unable to add dependencies to setup.cfg file.")
             return None
 
         if not dry_run:
             try:
                 with open(self.path, "w", encoding="utf-8") as f:
                     f.writelines(new_lines)
```

### Comparing `codemodder-0.96.0/src/codemodder/diff.py` & `codemodder-0.97.0/src/codemodder/diff.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/codemodder/file_context.py` & `codemodder-0.97.0/src/codemodder/file_context.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/codemodder/logging.py` & `codemodder-0.97.0/src/codemodder/logging.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/codemodder/project_analysis/file_parsers/base_parser.py` & `codemodder-0.97.0/src/codemodder/project_analysis/file_parsers/base_parser.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/codemodder/project_analysis/file_parsers/package_store.py` & `codemodder-0.97.0/src/codemodder/project_analysis/file_parsers/package_store.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/codemodder/project_analysis/file_parsers/pyproject_toml_file_parser.py` & `codemodder-0.97.0/src/codemodder/project_analysis/file_parsers/pyproject_toml_file_parser.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/codemodder/project_analysis/file_parsers/requirements_txt_file_parser.py` & `codemodder-0.97.0/src/codemodder/project_analysis/file_parsers/requirements_txt_file_parser.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/codemodder/project_analysis/file_parsers/setup_cfg_file_parser.py` & `codemodder-0.97.0/src/codemodder/project_analysis/file_parsers/setup_cfg_file_parser.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/codemodder/project_analysis/file_parsers/setup_py_file_parser.py` & `codemodder-0.97.0/src/codemodder/project_analysis/file_parsers/setup_py_file_parser.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/codemodder/project_analysis/python_repo_manager.py` & `codemodder-0.97.0/src/codemodder/project_analysis/python_repo_manager.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/codemodder/registry.py` & `codemodder-0.97.0/src/codemodder/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import os
 import re
 from dataclasses import dataclass
+from functools import cached_property
 from importlib.metadata import entry_points
 from itertools import chain
 from typing import TYPE_CHECKING, Optional
 
 from codemodder.logging import logger
 
 if TYPE_CHECKING:
@@ -52,14 +53,22 @@
     def codemods(self):
         return list(self._codemods_by_name.values())
 
     @property
     def default_include_paths(self) -> list[str]:
         return list(self._default_include_paths)
 
+    @cached_property
+    def pixee_codemods_by_name(self) -> dict:
+        return {
+            name: codemod
+            for name, codemod in self._codemods_by_name.items()
+            if codemod.origin == "pixee"
+        }
+
     def add_codemod_collection(self, collection: CodemodCollection):
         for codemod in collection.codemods:
             wrapper = codemod() if isinstance(codemod, type) else codemod
             self._codemods_by_name[wrapper.name] = wrapper
             self._codemods_by_id[wrapper.id] = wrapper
             self._default_include_paths.update(
                 chain(
@@ -83,14 +92,15 @@
             base_codemods = {}
             patterns = [
                 re.compile(exclude.replace("*", ".*"))
                 for exclude in codemod_exclude
                 if "*" in exclude
             ]
             names = set(name for name in codemod_exclude if "*" not in name)
+
             for codemod in self.codemods:
                 if (
                     codemod.id in names
                     or (codemod.origin == "pixee" and codemod.name in names)
                     or any(pat.match(codemod.id) for pat in patterns)
                 ):
                     continue
@@ -111,15 +121,15 @@
                     logger.warning(
                         "Given codemod pattern '%s' does not match any codemods.", name
                     )
                 continue
 
             try:
                 matched_codemods.append(
-                    self._codemods_by_name.get(name) or self._codemods_by_id[name]
+                    self.pixee_codemods_by_name.get(name) or self._codemods_by_id[name]
                 )
             except KeyError:
                 logger.warning(f"Requested codemod to include '{name}' does not exist.")
         return matched_codemods
 
     def describe_codemods(
         self,
```

### Comparing `codemodder-0.96.0/src/codemodder/result.py` & `codemodder-0.97.0/src/codemodder/result.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/codemodder/sarifs.py` & `codemodder-0.97.0/src/codemodder/sarifs.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/codemodder/scripts/generate_docs.py` & `codemodder-0.97.0/src/codemodder/scripts/generate_docs.py`

 * *Files 1% similar despite different names*

```diff
@@ -259,14 +259,18 @@
         importance="Medium",
         guidance_explained="This change makes your code more accurate but in some cases it may be necessary to adjust the `abs_tol` and `rel_tol` parameter values for your particular calculations.",
     ),
     "fix-math-isclose": DocMetadata(
         importance="Medium",
         guidance_explained="This change makes your code more accurate but in some cases it may be necessary to adjust the `abs_tol` parameter value for your particular calculations.",
     ),
+    "break-or-continue-out-of-loop": DocMetadata(
+        importance="Low",
+        guidance_explained="While this change will make the code consistent, it is likely that the `break` or `continue` statement is a symptom of an error in program logic.",
+    ),
 }
 DEFECTDOJO_CODEMODS = {
     "django-secure-set-cookie": DocMetadata(
         importance="Medium",
         guidance_explained="Our change provides the most secure way to create cookies in Django. However, it's possible you have configured your Django application configurations to use secure cookies. In these cases, using the default parameters for `set_cookie` is safe.",
         need_sarif="Yes (DefectDojo)",
     ),
@@ -292,14 +296,15 @@
     "secure-random-S2245",
     "enable-jinja2-autoescape-S5247",
     "url-sandbox-S5144",
     "fix-float-equality-S1244",
     "fix-math-isclose-S6727",
     "sql-parameterization-S3649",
     "django-model-without-dunder-str-S6554",
+    "break-or-continue-out-of-loop-S1716",
 ]
 SONAR_CODEMODS = {
     name: DocMetadata(
         importance=CORE_CODEMODS[
             core_codemod_name := "-".join(name.split("-")[:-1])
         ].importance,
         guidance_explained=CORE_CODEMODS[core_codemod_name].guidance_explained,
```

### Comparing `codemodder-0.96.0/src/codemodder/scripts/get_hashes.py` & `codemodder-0.97.0/src/codemodder/scripts/get_hashes.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/codemodder/semgrep.py` & `codemodder-0.97.0/src/codemodder/semgrep.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,16 +58,17 @@
 
         return None
 
     @classmethod
     def from_sarif(
         cls, sarif_result, sarif_run, truncate_rule_id: bool = False
     ) -> Self:
-        rule_id = cls.extract_rule_id(sarif_result, sarif_run, truncate_rule_id)
-        if not rule_id:
+        if not (
+            rule_id := cls.extract_rule_id(sarif_result, sarif_run, truncate_rule_id)
+        ):
             raise ValueError("Could not extract rule id from sarif result.")
 
         locations: list[Location] = []
         for location in sarif_result["locations"]:
             artifact_location = SemgrepLocation.from_sarif(location)
             locations.append(artifact_location)
         return cls(rule_id=rule_id, locations=locations)
```

### Comparing `codemodder-0.96.0/src/codemodder/utils/clean_code.py` & `codemodder-0.97.0/src/codemodder/utils/clean_code.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/codemodder/utils/format_string_parser.py` & `codemodder-0.97.0/src/codemodder/utils/format_string_parser.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/codemodder/utils/linearize_string_expression.py` & `codemodder-0.97.0/src/codemodder/utils/linearize_string_expression.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/codemodder/utils/timer.py` & `codemodder-0.97.0/src/codemodder/utils/timer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/codemodder/utils/utils.py` & `codemodder-0.97.0/src/codemodder/utils/utils.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/codemodder.egg-info/PKG-INFO` & `codemodder-0.97.0/src/codemodder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codemodder
-Version: 0.96.0
+Version: 0.97.0
 Summary: A pluggable framework for building codemods in Python
 Author-email: Pixee <python@pixee.ai>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -697,15 +697,15 @@
 Requires-Dist: Flask<4; extra == "test"
 Requires-Dist: Jinja2~=3.1.2; extra == "test"
 Requires-Dist: jsonschema~=4.21.0; extra == "test"
 Requires-Dist: lxml<5.3.0,>=4.9.3; extra == "test"
 Requires-Dist: mock==5.1.*; extra == "test"
 Requires-Dist: pre-commit<4; extra == "test"
 Requires-Dist: Pyjwt~=2.8.0; extra == "test"
-Requires-Dist: pytest<8.2,>=7.4; extra == "test"
+Requires-Dist: pytest<9,>=8.2; extra == "test"
 Requires-Dist: pytest-cov<5.1,>=4.1; extra == "test"
 Requires-Dist: pytest-mock<3.15,>=3.12; extra == "test"
 Requires-Dist: pytest-randomly==3.*; extra == "test"
 Requires-Dist: pytest-xdist==3.*; extra == "test"
 Requires-Dist: requests~=2.31.0; extra == "test"
 Requires-Dist: security~=1.2.0; extra == "test"
 Requires-Dist: types-mock==5.1.*; extra == "test"
@@ -713,15 +713,15 @@
 Requires-Dist: numpy~=1.26.0; extra == "test"
 Requires-Dist: flask_wtf~=1.2.0; extra == "test"
 Requires-Dist: fickling>=0.1.3,~=0.1.0; extra == "test"
 Provides-Extra: complexity
 Requires-Dist: radon==6.0.*; extra == "complexity"
 Requires-Dist: xenon==0.9.*; extra == "complexity"
 Provides-Extra: openai
-Requires-Dist: openai<1.24,>=1.0; extra == "openai"
+Requires-Dist: openai<1.25,>=1.0; extra == "openai"
 Provides-Extra: all
 Requires-Dist: codemodder[test]; extra == "all"
 Requires-Dist: codemodder[complexity]; extra == "all"
 
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="img/codemodder-dark.png">
   <source media="(prefers-color-scheme: light)" srcset="img/codemodder-light.png">
```

### Comparing `codemodder-0.96.0/src/codemodder.egg-info/SOURCES.txt` & `codemodder-0.97.0/src/codemodder.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 img/codemodder-dark.png
 img/codemodder-light.png
 img/codemodder.png
 integration_tests/README.md
 integration_tests/__init__.py
 integration_tests/conftest.py
 integration_tests/test_add_requests_timeout.py
+integration_tests/test_break_or_continue_out_of_loop.py
 integration_tests/test_combine_startswith_endswith.py
 integration_tests/test_dependency_manager.py
 integration_tests/test_django_debug_flag_on.py
 integration_tests/test_django_json_response_type.py
 integration_tests/test_django_model_without_dunder_str.py
 integration_tests/test_django_receiver_on_top.py
 integration_tests/test_django_session_cookie_secure_off.py
@@ -91,14 +92,15 @@
 integration_tests/test_upgrade_sslcontext_tls.py
 integration_tests/test_url_sandbox.py
 integration_tests/test_use_defusedxml.py
 integration_tests/test_use_generator.py
 integration_tests/test_use_set_literal.py
 integration_tests/test_use_walrus_if.py
 integration_tests/test_with_threading_lock.py
+integration_tests/sonar/test_sonar_break_or_continue_out_of_loop.py
 integration_tests/sonar/test_sonar_django_jmodel_without_dunder_str.py
 integration_tests/sonar/test_sonar_django_json_response_type.py
 integration_tests/sonar/test_sonar_django_receiver_on_top.py
 integration_tests/sonar/test_sonar_exception_without_raise.py
 integration_tests/sonar/test_sonar_fix_assert_tuple.py
 integration_tests/sonar/test_sonar_fix_float_equality.py
 integration_tests/sonar/test_sonar_fix_math_isclose.py
@@ -114,14 +116,15 @@
 integration_tests/sonar/test_sonar_tempfile_mktemp.py
 integration_tests/sonar/test_sonar_url_sandbox.py
 src/codemodder/__init__.py
 src/codemodder/_version.py
 src/codemodder/cli.py
 src/codemodder/code_directory.py
 src/codemodder/codemodder.py
+src/codemodder/codeql.py
 src/codemodder/codetf.py
 src/codemodder/context.py
 src/codemodder/dependency.py
 src/codemodder/diff.py
 src/codemodder/file_context.py
 src/codemodder/logging.py
 src/codemodder/registry.py
@@ -137,14 +140,15 @@
 src/codemodder/codemods/__init__.py
 src/codemodder/codemods/api.py
 src/codemodder/codemods/base_codemod.py
 src/codemodder/codemods/base_detector.py
 src/codemodder/codemods/base_transformer.py
 src/codemodder/codemods/base_visitor.py
 src/codemodder/codemods/check_annotations.py
+src/codemodder/codemods/codeql.py
 src/codemodder/codemods/import_modifier_codemod.py
 src/codemodder/codemods/imported_call_modifier.py
 src/codemodder/codemods/libcst_transformer.py
 src/codemodder/codemods/semgrep.py
 src/codemodder/codemods/utils.py
 src/codemodder/codemods/utils_mixin.py
 src/codemodder/codemods/test/__init__.py
@@ -180,14 +184,15 @@
 src/codemodder/utils/clean_code.py
 src/codemodder/utils/format_string_parser.py
 src/codemodder/utils/linearize_string_expression.py
 src/codemodder/utils/timer.py
 src/codemodder/utils/utils.py
 src/core_codemods/__init__.py
 src/core_codemods/add_requests_timeouts.py
+src/core_codemods/break_or_continue_out_of_loop.py
 src/core_codemods/combine_startswith_endswith.py
 src/core_codemods/django_debug_flag_on.py
 src/core_codemods/django_json_response_type.py
 src/core_codemods/django_model_without_dunder_str.py
 src/core_codemods/django_receiver_on_top.py
 src/core_codemods/django_session_cookie_secure_off.py
 src/core_codemods/enable_jinja2_autoescape.py
@@ -250,14 +255,15 @@
 src/core_codemods/defectdojo/semgrep/avoid_insecure_deserialization.py
 src/core_codemods/defectdojo/semgrep/django_secure_set_cookie.py
 src/core_codemods/docs/__init__.py
 src/core_codemods/docs/defectdojo_python_avoid-insecure-deserialization.md
 src/core_codemods/docs/defectdojo_python_django-secure-set-cookie.md
 src/core_codemods/docs/pixee_python_add-requests-timeouts.md
 src/core_codemods/docs/pixee_python_bad-lock-with-statement.md
+src/core_codemods/docs/pixee_python_break-or-continue-out-of-loop.md
 src/core_codemods/docs/pixee_python_combine-startswith-endswith.md
 src/core_codemods/docs/pixee_python_django-debug-flag-on.md
 src/core_codemods/docs/pixee_python_django-json-response-type.md
 src/core_codemods/docs/pixee_python_django-model-without-dunder-str.md
 src/core_codemods/docs/pixee_python_django-receiver-on-top.md
 src/core_codemods/docs/pixee_python_django-session-cookie-secure-off.md
 src/core_codemods/docs/pixee_python_enable-jinja2-autoescape.md
@@ -310,14 +316,15 @@
 src/core_codemods/docs/pixee_python_use-generator.md
 src/core_codemods/docs/pixee_python_use-set-literal.md
 src/core_codemods/docs/pixee_python_use-walrus-if.md
 src/core_codemods/refactor/__init__.py
 src/core_codemods/refactor/refactor_new_api.py
 src/core_codemods/sonar/api.py
 src/core_codemods/sonar/results.py
+src/core_codemods/sonar/sonar_break_or_continue_out_of_loop.py
 src/core_codemods/sonar/sonar_django_json_response_type.py
 src/core_codemods/sonar/sonar_django_model_without_dunder_str.py
 src/core_codemods/sonar/sonar_django_receiver_on_top.py
 src/core_codemods/sonar/sonar_enable_jinja2_autoescape.py
 src/core_codemods/sonar/sonar_exception_without_raise.py
 src/core_codemods/sonar/sonar_fix_assert_tuple.py
 src/core_codemods/sonar/sonar_fix_float_equality.py
@@ -336,14 +343,15 @@
 tests/conftest.py
 tests/test_ancestorpatterns_mixin.py
 tests/test_basetype.py
 tests/test_cli.py
 tests/test_code_directory.py
 tests/test_codemod_docs.py
 tests/test_codemodder.py
+tests/test_codeql.py
 tests/test_codetf.py
 tests/test_context.py
 tests/test_file_context.py
 tests/test_format_string_parser.py
 tests/test_libcst_transformer.py
 tests/test_linearize_string_expression.py
 tests/test_logging.py
@@ -355,14 +363,15 @@
 tests/test_version.py
 tests/codemods/__init__.py
 tests/codemods/conftest.py
 tests/codemods/test_add_requests_timeouts.py
 tests/codemods/test_async_fix_task_instantiation.py
 tests/codemods/test_base_codemod.py
 tests/codemods/test_base_visitor.py
+tests/codemods/test_break_or_continue_out_of_loop.py
 tests/codemods/test_combine_startswith_endswith.py
 tests/codemods/test_django_debug_flag_on.py
 tests/codemods/test_django_json_response_type.py
 tests/codemods/test_django_model_without_dunder_str.py
 tests/codemods/test_django_receiver_on_top.py
 tests/codemods/test_django_session_cookie_secure_off.py
 tests/codemods/test_enable_jinja2_autoescape.py
@@ -415,14 +424,15 @@
 tests/codemods/test_use_defused_xml.py
 tests/codemods/test_use_generator.py
 tests/codemods/test_use_set_literal.py
 tests/codemods/test_walrus_if.py
 tests/codemods/test_with_threading_lock.py
 tests/codemods/defectdojo/semgrep/test_avoid_insecure_deserialization.py
 tests/codemods/defectdojo/semgrep/test_django_secure_set_cookie.py
+tests/codemods/sonar/test_sonar_break_or_continue_out_of_loop.py
 tests/codemods/sonar/test_sonar_django_json_response_type.py
 tests/codemods/sonar/test_sonar_django_model_without_dunder_str.py
 tests/codemods/sonar/test_sonar_django_receiver_on_top.py
 tests/codemods/sonar/test_sonar_enable_jinja2_autoescape.py
 tests/codemods/sonar/test_sonar_exception_without_raise.py
 tests/codemods/sonar/test_sonar_fix_assert_tuple.py
 tests/codemods/sonar/test_sonar_fix_float_equality.py
@@ -447,14 +457,15 @@
 tests/project_analysis/__init__.py
 tests/project_analysis/test_python_repo_manager.py
 tests/project_analysis/file_parsers/__init__.py
 tests/project_analysis/file_parsers/test_pyproject_toml_file_parser.py
 tests/project_analysis/file_parsers/test_requirements_txt_file_parser.py
 tests/project_analysis/file_parsers/test_setup_cfg_file_parser.py
 tests/project_analysis/file_parsers/test_setup_py_file_parser.py
+tests/samples/break_or_continue_out_of_loop.py
 tests/samples/django_json_response_type.py
 tests/samples/django_model.py
 tests/samples/django_receiver_on_top.py
 tests/samples/exception_without_raise.py
 tests/samples/fix_assert_tuple.py
 tests/samples/fix_float_equality.py
 tests/samples/fix_math_isclose.py
```

### Comparing `codemodder-0.96.0/src/codemodder.egg-info/requires.txt` & `codemodder-0.97.0/src/codemodder.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -17,26 +17,26 @@
 codemodder[complexity]
 
 [complexity]
 radon==6.0.*
 xenon==0.9.*
 
 [openai]
-openai<1.24,>=1.0
+openai<1.25,>=1.0
 
 [test]
 coverage<7.6,>=7.3
 Flask<4
 Jinja2~=3.1.2
 jsonschema~=4.21.0
 lxml<5.3.0,>=4.9.3
 mock==5.1.*
 pre-commit<4
 Pyjwt~=2.8.0
-pytest<8.2,>=7.4
+pytest<9,>=8.2
 pytest-cov<5.1,>=4.1
 pytest-mock<3.15,>=3.12
 pytest-randomly==3.*
 pytest-xdist==3.*
 requests~=2.31.0
 security~=1.2.0
 types-mock==5.1.*
```

### Comparing `codemodder-0.96.0/src/core_codemods/__init__.py` & `codemodder-0.97.0/src/core_codemods/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from codemodder.registry import CodemodCollection
 
 from .add_requests_timeouts import AddRequestsTimeouts
+from .break_or_continue_out_of_loop import BreakOrContinueOutOfLoop
 from .combine_startswith_endswith import CombineStartswithEndswith
 from .defectdojo.semgrep.avoid_insecure_deserialization import (
     AvoidInsecureDeserialization,
 )
 from .defectdojo.semgrep.django_secure_set_cookie import DjangoSecureSetCookie
 from .django_debug_flag_on import DjangoDebugFlagOn
 from .django_json_response_type import DjangoJsonResponseType
@@ -47,14 +48,15 @@
 from .remove_unnecessary_f_str import RemoveUnnecessaryFStr
 from .remove_unused_imports import RemoveUnusedImports
 from .replace_flask_send_file import ReplaceFlaskSendFile
 from .requests_verify import RequestsVerify
 from .secure_flask_cookie import SecureFlaskCookie
 from .secure_flask_session_config import SecureFlaskSessionConfig
 from .secure_random import SecureRandom
+from .sonar.sonar_break_or_continue_out_of_loop import SonarBreakOrContinueOutOfLoop
 from .sonar.sonar_django_json_response_type import SonarDjangoJsonResponseType
 from .sonar.sonar_django_model_without_dunder_str import (
     SonarDjangoModelWithoutDunderStr,
 )
 from .sonar.sonar_django_receiver_on_top import SonarDjangoReceiverOnTop
 from .sonar.sonar_enable_jinja2_autoescape import SonarEnableJinja2Autoescape
 from .sonar.sonar_exception_without_raise import SonarExceptionWithoutRaise
@@ -144,14 +146,15 @@
         StrConcatInSeqLiteral,
         FixAsyncTaskInstantiation,
         DjangoModelWithoutDunderStr,
         TransformFixHasattrCall,
         FixDataclassDefaults,
         FixMissingSelfOrCls,
         FixMathIsClose,
+        BreakOrContinueOutOfLoop,
     ],
 )
 
 sonar_registry = CodemodCollection(
     origin="sonar",
     codemods=[
         SonarNumpyNanEquality,
@@ -168,14 +171,15 @@
         SonarSecureRandom,
         SonarEnableJinja2Autoescape,
         SonarUrlSandbox,
         SonarFixFloatEquality,
         SonarFixMathIsClose,
         SonarSQLParameterization,
         SonarDjangoModelWithoutDunderStr,
+        SonarBreakOrContinueOutOfLoop,
     ],
 )
 
 defectdojo_registry = CodemodCollection(
     origin="defectdojo",
     codemods=[
         AvoidInsecureDeserialization,
```

### Comparing `codemodder-0.96.0/src/core_codemods/add_requests_timeouts.py` & `codemodder-0.97.0/src/core_codemods/add_requests_timeouts.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/api/core_codemod.py` & `codemodder-0.97.0/src/core_codemods/api/core_codemod.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/combine_startswith_endswith.py` & `codemodder-0.97.0/src/core_codemods/combine_startswith_endswith.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/defectdojo/api.py` & `codemodder-0.97.0/src/core_codemods/defectdojo/api.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/defectdojo/results.py` & `codemodder-0.97.0/src/core_codemods/defectdojo/results.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/defectdojo/semgrep/avoid_insecure_deserialization.py` & `codemodder-0.97.0/src/core_codemods/defectdojo/semgrep/avoid_insecure_deserialization.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/defectdojo/semgrep/django_secure_set_cookie.py` & `codemodder-0.97.0/src/core_codemods/defectdojo/semgrep/django_secure_set_cookie.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/django_debug_flag_on.py` & `codemodder-0.97.0/src/core_codemods/django_debug_flag_on.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/django_json_response_type.py` & `codemodder-0.97.0/src/core_codemods/django_json_response_type.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/django_model_without_dunder_str.py` & `codemodder-0.97.0/src/core_codemods/django_model_without_dunder_str.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/django_receiver_on_top.py` & `codemodder-0.97.0/src/core_codemods/django_receiver_on_top.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/django_session_cookie_secure_off.py` & `codemodder-0.97.0/src/core_codemods/django_session_cookie_secure_off.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/docs/defectdojo_python_avoid-insecure-deserialization.md` & `codemodder-0.97.0/src/core_codemods/docs/defectdojo_python_avoid-insecure-deserialization.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/docs/defectdojo_python_django-secure-set-cookie.md` & `codemodder-0.97.0/src/core_codemods/docs/defectdojo_python_django-secure-set-cookie.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/docs/pixee_python_add-requests-timeouts.md` & `codemodder-0.97.0/src/core_codemods/docs/pixee_python_add-requests-timeouts.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/docs/pixee_python_bad-lock-with-statement.md` & `codemodder-0.97.0/src/core_codemods/docs/pixee_python_bad-lock-with-statement.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/docs/pixee_python_combine-startswith-endswith.md` & `codemodder-0.97.0/src/core_codemods/docs/pixee_python_combine-startswith-endswith.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/docs/pixee_python_django-json-response-type.md` & `codemodder-0.97.0/src/core_codemods/docs/pixee_python_django-json-response-type.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/docs/pixee_python_django-model-without-dunder-str.md` & `codemodder-0.97.0/src/core_codemods/docs/pixee_python_django-model-without-dunder-str.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/docs/pixee_python_django-receiver-on-top.md` & `codemodder-0.97.0/src/core_codemods/docs/pixee_python_django-receiver-on-top.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/docs/pixee_python_enable-jinja2-autoescape.md` & `codemodder-0.97.0/src/core_codemods/docs/pixee_python_enable-jinja2-autoescape.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/docs/pixee_python_fix-dataclass-defaults.md` & `codemodder-0.97.0/src/core_codemods/docs/pixee_python_fix-dataclass-defaults.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/docs/pixee_python_fix-deprecated-abstractproperty.md` & `codemodder-0.97.0/src/core_codemods/docs/pixee_python_fix-deprecated-abstractproperty.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/docs/pixee_python_fix-deprecated-logging-warn.md` & `codemodder-0.97.0/src/core_codemods/docs/pixee_python_fix-deprecated-logging-warn.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/docs/pixee_python_fix-empty-sequence-comparison.md` & `codemodder-0.97.0/src/core_codemods/docs/pixee_python_fix-empty-sequence-comparison.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/docs/pixee_python_fix-file-resource-leak.md` & `codemodder-0.97.0/src/core_codemods/docs/pixee_python_fix-file-resource-leak.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/docs/pixee_python_fix-float-equality.md` & `codemodder-0.97.0/src/core_codemods/docs/pixee_python_fix-float-equality.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/docs/pixee_python_fix-math-isclose.md` & `codemodder-0.97.0/src/core_codemods/docs/pixee_python_fix-math-isclose.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/docs/pixee_python_fix-mutable-params.md` & `codemodder-0.97.0/src/core_codemods/docs/pixee_python_fix-mutable-params.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/docs/pixee_python_flask-enable-csrf-protection.md` & `codemodder-0.97.0/src/core_codemods/docs/pixee_python_flask-enable-csrf-protection.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/docs/pixee_python_flask-json-response-type.md` & `codemodder-0.97.0/src/core_codemods/docs/pixee_python_flask-json-response-type.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/docs/pixee_python_harden-pickle-load.md` & `codemodder-0.97.0/src/core_codemods/docs/pixee_python_harden-pickle-load.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/docs/pixee_python_harden-pyyaml.md` & `codemodder-0.97.0/src/core_codemods/docs/pixee_python_harden-pyyaml.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/docs/pixee_python_harden-ruamel.md` & `codemodder-0.97.0/src/core_codemods/docs/pixee_python_harden-ruamel.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/docs/pixee_python_jwt-decode-verify.md` & `codemodder-0.97.0/src/core_codemods/docs/pixee_python_jwt-decode-verify.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/docs/pixee_python_lazy-logging.md` & `codemodder-0.97.0/src/core_codemods/docs/pixee_python_lazy-logging.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/docs/pixee_python_limit-readline.md` & `codemodder-0.97.0/src/core_codemods/docs/pixee_python_limit-readline.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/docs/pixee_python_remove-assertion-in-pytest-raises.md` & `codemodder-0.97.0/src/core_codemods/docs/pixee_python_remove-assertion-in-pytest-raises.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/docs/pixee_python_remove-future-imports.md` & `codemodder-0.97.0/src/core_codemods/docs/pixee_python_remove-future-imports.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/docs/pixee_python_replace-flask-send-file.md` & `codemodder-0.97.0/src/core_codemods/docs/pixee_python_replace-flask-send-file.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/docs/pixee_python_requests-verify.md` & `codemodder-0.97.0/src/core_codemods/docs/pixee_python_requests-verify.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/docs/pixee_python_safe-lxml-parser-defaults.md` & `codemodder-0.97.0/src/core_codemods/docs/pixee_python_safe-lxml-parser-defaults.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/docs/pixee_python_safe-lxml-parsing.md` & `codemodder-0.97.0/src/core_codemods/docs/pixee_python_safe-lxml-parsing.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/docs/pixee_python_sandbox-process-creation.md` & `codemodder-0.97.0/src/core_codemods/docs/pixee_python_sandbox-process-creation.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/docs/pixee_python_secure-flask-cookie.md` & `codemodder-0.97.0/src/core_codemods/docs/pixee_python_secure-flask-cookie.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/docs/pixee_python_secure-flask-session-configuration.md` & `codemodder-0.97.0/src/core_codemods/docs/pixee_python_secure-flask-session-configuration.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/docs/pixee_python_secure-random.md` & `codemodder-0.97.0/src/core_codemods/docs/pixee_python_secure-random.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/docs/pixee_python_sql-parameterization.md` & `codemodder-0.97.0/src/core_codemods/docs/pixee_python_sql-parameterization.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/docs/pixee_python_subprocess-shell-false.md` & `codemodder-0.97.0/src/core_codemods/docs/pixee_python_subprocess-shell-false.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/docs/pixee_python_upgrade-sslcontext-minimum-version.md` & `codemodder-0.97.0/src/core_codemods/docs/pixee_python_upgrade-sslcontext-minimum-version.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/docs/pixee_python_upgrade-sslcontext-tls.md` & `codemodder-0.97.0/src/core_codemods/docs/pixee_python_upgrade-sslcontext-tls.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/docs/pixee_python_url-sandbox.md` & `codemodder-0.97.0/src/core_codemods/docs/pixee_python_url-sandbox.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/docs/pixee_python_use-defusedxml.md` & `codemodder-0.97.0/src/core_codemods/docs/pixee_python_use-defusedxml.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/docs/pixee_python_use-generator.md` & `codemodder-0.97.0/src/core_codemods/docs/pixee_python_use-generator.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/docs/pixee_python_use-walrus-if.md` & `codemodder-0.97.0/src/core_codemods/docs/pixee_python_use-walrus-if.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/enable_jinja2_autoescape.py` & `codemodder-0.97.0/src/core_codemods/enable_jinja2_autoescape.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/exception_without_raise.py` & `codemodder-0.97.0/src/core_codemods/exception_without_raise.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/file_resource_leak.py` & `codemodder-0.97.0/src/core_codemods/file_resource_leak.py`

 * *Files 1% similar despite different names*

```diff
@@ -372,22 +372,21 @@
             if self.is_return_value(node) or self.is_yield_value(node):
                 return True
             # argument of a call
             # TODO exclude calls that spawn dependent resources here...
             if self.is_argument_of_call(node):
                 return True
             # out of block?
-            ancestors = self._filter_ancestors(node, block.body[index:])
             # TODO this only looks for accesses and not assignments
             # e.g.
             # out = None
             # if True:
             #    out = x
             # will pass
-            if not ancestors:
+            if not self._filter_ancestors(node, block.body[index:]):
                 return True
 
         return False
 
     def _filter_ancestors(
         self, node: cst.CSTNode, node_sequence: Sequence[cst.CSTNode]
     ) -> list[cst.CSTNode]:
```

### Comparing `codemodder-0.96.0/src/core_codemods/fix_assert_tuple.py` & `codemodder-0.97.0/src/core_codemods/fix_assert_tuple.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/fix_async_task_instantiation.py` & `codemodder-0.97.0/src/core_codemods/fix_async_task_instantiation.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,21 +35,19 @@
 
         loop_type = (
             infer_expression_type(self.resolve_expression(loop_arg.value))
             if loop_arg
             else None
         )
 
-        eager_start_type = (
+        if (
             infer_expression_type(self.resolve_expression(eager_start_arg.value))
             if eager_start_arg
             else None
-        )
-
-        if eager_start_type == BaseType.TRUE:
+        ) == BaseType.TRUE:
             if not loop_arg or self._is_invalid_loop_value(loop_type):
                 # asking for eager_start without a loop or incorrectly setting loop is bad.
                 # We won't do anything.
                 return updated_node
 
             loop_arg = loop_arg.with_changes(keyword=None, equal=MaybeSentinel.DEFAULT)
             return self.node_eager_task(
```

### Comparing `codemodder-0.96.0/src/core_codemods/fix_dataclass_defaults.py` & `codemodder-0.97.0/src/core_codemods/fix_dataclass_defaults.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,18 +25,17 @@
     ) -> cst.CSTNode:
         if not self.filter_by_path_includes_or_excludes(
             self.node_position(original_node)
         ):
             return updated_node
 
         maybe_classdef = self.find_immediate_class_def(original_node)
-        maybe_has_decorator = (
+        if not (
             self._has_dataclass_decorator(maybe_classdef) if maybe_classdef else False
-        )
-        if not maybe_has_decorator:
+        ):
             return updated_node
 
         match original_node.value:
             case cst.List(elements=[]) | cst.Dict(elements=[]) | cst.Tuple(elements=[]):
                 return self.field_with_default_factory(original_node, updated_node)
             case (
                 cst.List(elements=[_, *_])
```

### Comparing `codemodder-0.96.0/src/core_codemods/fix_deprecated_abstractproperty.py` & `codemodder-0.97.0/src/core_codemods/fix_deprecated_abstractproperty.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/fix_deprecated_logging_warn.py` & `codemodder-0.97.0/src/core_codemods/fix_deprecated_logging_warn.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/fix_empty_sequence_comparison.py` & `codemodder-0.97.0/src/core_codemods/fix_empty_sequence_comparison.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/fix_float_equality.py` & `codemodder-0.97.0/src/core_codemods/fix_float_equality.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/fix_hasattr_call.py` & `codemodder-0.97.0/src/core_codemods/fix_hasattr_call.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/fix_math_isclose.py` & `codemodder-0.97.0/src/core_codemods/fix_math_isclose.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/fix_missing_self_or_cls.py` & `codemodder-0.97.0/src/core_codemods/fix_missing_self_or_cls.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/fix_mutable_params.py` & `codemodder-0.97.0/src/core_codemods/fix_mutable_params.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/flask_enable_csrf_protection.py` & `codemodder-0.97.0/src/core_codemods/flask_enable_csrf_protection.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/flask_json_response_type.py` & `codemodder-0.97.0/src/core_codemods/flask_json_response_type.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/harden_pickle_load.py` & `codemodder-0.97.0/src/core_codemods/harden_pickle_load.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/harden_pyyaml.py` & `codemodder-0.97.0/src/core_codemods/harden_pyyaml.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,33 +20,37 @@
     def update_arg_target(
         self, node: cst.Call, new_args: list[cst.Arg]
     ) -> cst.Call: ...
 
 
 class HardenPyyamlCallMixin:
     def update_call(
-        self: CodemodProtocol, original_node: cst.Call, updated_node: cst.Call
+        self: CodemodProtocol,
+        original_node: cst.Call,
+        updated_node: cst.Call,
+        maybe_aliased_name: str | None = None,
     ) -> cst.Call:
-        maybe_name = self.get_aliased_prefix_name(original_node, YAML_MODULE_NAME)
-        if (maybe_name := maybe_name or YAML_MODULE_NAME) == YAML_MODULE_NAME:
+        module_name = maybe_aliased_name or YAML_MODULE_NAME
+        if not maybe_aliased_name:
             self.add_needed_import(YAML_MODULE_NAME)
+
         updated_node = cast(cst.Call, updated_node)  # satisfy the type checker
         new_args = [
             *updated_node.args[:1],
             # This is the case where the arg is present but a bad value
             (
                 updated_node.args[1].with_changes(
-                    value=self.parse_expression(f"{maybe_name}.SafeLoader")
+                    value=self.parse_expression(f"{module_name}.SafeLoader")
                 )
                 if len(updated_node.args) > 1
                 # This is the case where the arg is not present
                 # Note that this case is deprecated in PyYAML 5.1 since the default is unsafe
                 else cst.Arg(
                     keyword=cst.Name("Loader"),
-                    value=self.parse_expression(f"{maybe_name}.SafeLoader"),
+                    value=self.parse_expression(f"{module_name}.SafeLoader"),
                     equal=cst.AssignEqual(
                         whitespace_before=cst.SimpleWhitespace(""),
                         whitespace_after=cst.SimpleWhitespace(""),
                     ),
                 )
             ),
         ]
@@ -63,38 +67,45 @@
 
     def on_result_found(
         self,
         original_node: Union[cst.Call, cst.ClassDef],
         updated_node: Union[cst.Call, cst.ClassDef],
     ):
         # TODO: provide different change description for each case.
+        maybe_aliased_name = self.get_aliased_prefix_name(
+            original_node, YAML_MODULE_NAME
+        )
         match original_node, updated_node:
             case cst.Call(), cst.Call():
-                return self.update_call(original_node, updated_node)
+                return self.update_call(original_node, updated_node, maybe_aliased_name)
             case cst.ClassDef(), _:
                 return updated_node.with_changes(
-                    bases=self._update_bases(original_node)
+                    bases=self._update_bases(original_node, maybe_aliased_name)
                 )
         return updated_node
 
-    def _update_bases(self, original_node: cst.ClassDef) -> list[cst.Arg]:
+    def _update_bases(
+        self, original_node: cst.ClassDef, maybe_aliased_name: str | None = None
+    ) -> list[cst.Arg]:
         new = []
         base_names = [
             f"yaml.{klas}"
             for klas in ("UnsafeLoader", "Loader", "BaseLoader", "FullLoader")
         ]
+        module_name = maybe_aliased_name or YAML_MODULE_NAME
         for base_arg in original_node.bases:
             base_name = self.find_base_name(base_arg.value)
             if base_name not in base_names:
                 new.append(base_arg)
                 continue
 
             match base_arg.value:
                 case cst.Name():
-                    self.add_needed_import(YAML_MODULE_NAME, "SafeLoader")
+                    if not maybe_aliased_name:
+                        self.add_needed_import(module_name, "SafeLoader")
                     self.remove_unused_import(base_arg.value)
                     base_arg = base_arg.with_changes(
                         value=base_arg.value.with_changes(value="SafeLoader")
                     )
                 case cst.Attribute():
                     base_arg = base_arg.with_changes(
                         value=base_arg.value.with_changes(attr=cst.Name("SafeLoader"))
```

### Comparing `codemodder-0.96.0/src/core_codemods/harden_ruamel.py` & `codemodder-0.97.0/src/core_codemods/harden_ruamel.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/https_connection.py` & `codemodder-0.97.0/src/core_codemods/https_connection.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/jwt_decode_verify.py` & `codemodder-0.97.0/src/core_codemods/jwt_decode_verify.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/lazy_logging.py` & `codemodder-0.97.0/src/core_codemods/lazy_logging.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/limit_readline.py` & `codemodder-0.97.0/src/core_codemods/limit_readline.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/literal_or_new_object_identity.py` & `codemodder-0.97.0/src/core_codemods/literal_or_new_object_identity.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/lxml_safe_parser_defaults.py` & `codemodder-0.97.0/src/core_codemods/lxml_safe_parser_defaults.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/lxml_safe_parsing.py` & `codemodder-0.97.0/src/core_codemods/lxml_safe_parsing.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/numpy_nan_equality.py` & `codemodder-0.97.0/src/core_codemods/numpy_nan_equality.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/order_imports.py` & `codemodder-0.97.0/src/core_codemods/order_imports.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/process_creation_sandbox.py` & `codemodder-0.97.0/src/core_codemods/process_creation_sandbox.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/refactor/refactor_new_api.py` & `codemodder-0.97.0/src/core_codemods/refactor/refactor_new_api.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/remove_assertion_in_pytest_raises.py` & `codemodder-0.97.0/src/core_codemods/remove_assertion_in_pytest_raises.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/remove_debug_breakpoint.py` & `codemodder-0.97.0/src/core_codemods/remove_debug_breakpoint.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/remove_future_imports.py` & `codemodder-0.97.0/src/core_codemods/remove_future_imports.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/remove_module_global.py` & `codemodder-0.97.0/src/core_codemods/remove_module_global.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/remove_unnecessary_f_str.py` & `codemodder-0.97.0/src/core_codemods/remove_unnecessary_f_str.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/remove_unused_imports.py` & `codemodder-0.97.0/src/core_codemods/remove_unused_imports.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/replace_flask_send_file.py` & `codemodder-0.97.0/src/core_codemods/replace_flask_send_file.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/requests_verify.py` & `codemodder-0.97.0/src/core_codemods/requests_verify.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/secure_cookie_mixin.py` & `codemodder-0.97.0/src/core_codemods/secure_cookie_mixin.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,16 +12,13 @@
 
         samesite = matchers.Arg(
             keyword=matchers.Name(value="samesite"),
             value=matchers.SimpleString(value="'Strict'"),
         )
 
         # samesite=Strict is OK because it's more restrictive than Lax.
-        strict_samesite_defined = any(
-            matchers.matches(arg, samesite) for arg in original_node.args
-        )
-        if not strict_samesite_defined:
+        if not any(matchers.matches(arg, samesite) for arg in original_node.args):
             new_args.append(
                 NewArg(name="samesite", value="'Lax'", add_if_missing=True),
             )
 
         return new_args
```

### Comparing `codemodder-0.96.0/src/core_codemods/secure_flask_cookie.py` & `codemodder-0.97.0/src/core_codemods/secure_flask_cookie.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/secure_flask_session_config.py` & `codemodder-0.97.0/src/core_codemods/secure_flask_session_config.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/secure_random.py` & `codemodder-0.97.0/src/core_codemods/secure_random.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/sonar/api.py` & `codemodder-0.97.0/src/core_codemods/sonar/api.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/sonar/results.py` & `codemodder-0.97.0/src/core_codemods/sonar/results.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/sonar/sonar_fix_math_isclose.py` & `codemodder-0.97.0/src/core_codemods/sonar/sonar_fix_math_isclose.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/sonar/sonar_jwt_decode_verify.py` & `codemodder-0.97.0/src/core_codemods/sonar/sonar_jwt_decode_verify.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/sql_parameterization.py` & `codemodder-0.97.0/src/core_codemods/sql_parameterization.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/str_concat_in_seq_literal.py` & `codemodder-0.97.0/src/core_codemods/str_concat_in_seq_literal.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/subprocess_shell_false.py` & `codemodder-0.97.0/src/core_codemods/subprocess_shell_false.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/tempfile_mktemp.py` & `codemodder-0.97.0/src/core_codemods/tempfile_mktemp.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/upgrade_sslcontext_minimum_version.py` & `codemodder-0.97.0/src/core_codemods/upgrade_sslcontext_minimum_version.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/upgrade_sslcontext_tls.py` & `codemodder-0.97.0/src/core_codemods/upgrade_sslcontext_tls.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/url_sandbox.py` & `codemodder-0.97.0/src/core_codemods/url_sandbox.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/use_defused_xml.py` & `codemodder-0.97.0/src/core_codemods/use_defused_xml.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/use_generator.py` & `codemodder-0.97.0/src/core_codemods/use_generator.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/use_set_literal.py` & `codemodder-0.97.0/src/core_codemods/use_set_literal.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/use_walrus_if.py` & `codemodder-0.97.0/src/core_codemods/use_walrus_if.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/src/core_codemods/with_threading_lock.py` & `codemodder-0.97.0/src/core_codemods/with_threading_lock.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/defectdojo/semgrep/test_avoid_insecure_deserialization.py` & `codemodder-0.97.0/tests/codemods/defectdojo/semgrep/test_avoid_insecure_deserialization.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/defectdojo/semgrep/test_django_secure_set_cookie.py` & `codemodder-0.97.0/tests/codemods/defectdojo/semgrep/test_django_secure_set_cookie.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/sonar/test_sonar_django_json_response_type.py` & `codemodder-0.97.0/tests/codemods/sonar/test_sonar_django_json_response_type.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/sonar/test_sonar_django_model_without_dunder_str.py` & `codemodder-0.97.0/tests/codemods/sonar/test_sonar_django_model_without_dunder_str.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/sonar/test_sonar_django_receiver_on_top.py` & `codemodder-0.97.0/tests/codemods/sonar/test_sonar_django_receiver_on_top.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/sonar/test_sonar_enable_jinja2_autoescape.py` & `codemodder-0.97.0/tests/codemods/sonar/test_sonar_enable_jinja2_autoescape.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/sonar/test_sonar_exception_without_raise.py` & `codemodder-0.97.0/tests/codemods/sonar/test_sonar_exception_without_raise.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/sonar/test_sonar_fix_assert_tuple.py` & `codemodder-0.97.0/tests/codemods/sonar/test_sonar_fix_assert_tuple.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/sonar/test_sonar_fix_float_equality.py` & `codemodder-0.97.0/tests/codemods/sonar/test_sonar_fix_float_equality.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/sonar/test_sonar_fix_math_isclose.py` & `codemodder-0.97.0/tests/codemods/sonar/test_sonar_fix_math_isclose.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/sonar/test_sonar_fix_missing_self_or_cls.py` & `codemodder-0.97.0/tests/codemods/sonar/test_sonar_fix_missing_self_or_cls.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/sonar/test_sonar_flask_json_response_type.py` & `codemodder-0.97.0/tests/codemods/sonar/test_sonar_flask_json_response_type.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/sonar/test_sonar_jwt_decode_verify.py` & `codemodder-0.97.0/tests/codemods/sonar/test_sonar_jwt_decode_verify.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/sonar/test_sonar_literal_or_new_object_identity.py` & `codemodder-0.97.0/tests/codemods/sonar/test_sonar_literal_or_new_object_identity.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/sonar/test_sonar_numpy_nan_equality.py` & `codemodder-0.97.0/tests/codemods/sonar/test_sonar_numpy_nan_equality.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/sonar/test_sonar_remove_assertion_in_pytest_raises.py` & `codemodder-0.97.0/tests/codemods/sonar/test_sonar_remove_assertion_in_pytest_raises.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/sonar/test_sonar_secure_random.py` & `codemodder-0.97.0/tests/codemods/sonar/test_sonar_secure_random.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/sonar/test_sonar_sql_parameterization.py` & `codemodder-0.97.0/tests/codemods/sonar/test_sonar_sql_parameterization.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/sonar/test_sonar_tempfile_mktemp.py` & `codemodder-0.97.0/tests/codemods/sonar/test_sonar_tempfile_mktemp.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/sonar/test_sonar_url_sandbox.py` & `codemodder-0.97.0/tests/codemods/sonar/test_sonar_url_sandbox.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_add_requests_timeouts.py` & `codemodder-0.97.0/tests/codemods/test_add_requests_timeouts.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_async_fix_task_instantiation.py` & `codemodder-0.97.0/tests/codemods/test_async_fix_task_instantiation.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_base_codemod.py` & `codemodder-0.97.0/tests/codemods/test_base_codemod.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_base_visitor.py` & `codemodder-0.97.0/tests/codemods/test_base_visitor.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_combine_startswith_endswith.py` & `codemodder-0.97.0/tests/codemods/test_combine_startswith_endswith.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_django_debug_flag_on.py` & `codemodder-0.97.0/tests/codemods/test_django_debug_flag_on.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_django_json_response_type.py` & `codemodder-0.97.0/tests/codemods/test_django_json_response_type.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_django_model_without_dunder_str.py` & `codemodder-0.97.0/tests/codemods/test_django_model_without_dunder_str.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_django_receiver_on_top.py` & `codemodder-0.97.0/tests/codemods/test_django_receiver_on_top.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_django_session_cookie_secure_off.py` & `codemodder-0.97.0/tests/codemods/test_django_session_cookie_secure_off.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_enable_jinja2_autoescape.py` & `codemodder-0.97.0/tests/codemods/test_enable_jinja2_autoescape.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_exception_without_raise.py` & `codemodder-0.97.0/tests/codemods/test_exception_without_raise.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_file_resource_leak.py` & `codemodder-0.97.0/tests/codemods/test_file_resource_leak.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_fix_assert_tuple.py` & `codemodder-0.97.0/tests/codemods/test_fix_assert_tuple.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_fix_dataclass_defaults.py` & `codemodder-0.97.0/tests/codemods/test_fix_dataclass_defaults.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_fix_deprecated_abstractproperty.py` & `codemodder-0.97.0/tests/codemods/test_fix_deprecated_abstractproperty.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_fix_deprecated_logging_warn.py` & `codemodder-0.97.0/tests/codemods/test_fix_deprecated_logging_warn.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_fix_empty_sequence_comparison.py` & `codemodder-0.97.0/tests/codemods/test_fix_empty_sequence_comparison.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_fix_float_equality.py` & `codemodder-0.97.0/tests/codemods/test_fix_float_equality.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_fix_hasattr_call.py` & `codemodder-0.97.0/tests/codemods/test_fix_hasattr_call.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_fix_math_isclose.py` & `codemodder-0.97.0/tests/codemods/test_fix_math_isclose.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_fix_missing_self_or_cls.py` & `codemodder-0.97.0/tests/codemods/test_fix_missing_self_or_cls.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_fix_mutable_params.py` & `codemodder-0.97.0/tests/codemods/test_fix_mutable_params.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_flask_enable_csrf_protection.py` & `codemodder-0.97.0/tests/codemods/test_flask_enable_csrf_protection.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_flask_json_response_type.py` & `codemodder-0.97.0/tests/codemods/test_flask_json_response_type.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_harden_pickle_load.py` & `codemodder-0.97.0/tests/codemods/test_harden_pickle_load.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_harden_pyyaml.py` & `codemodder-0.97.0/tests/codemods/test_harden_pyyaml.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,27 @@
 from yaml import Loader
 
 data = b'!!python/object/apply:subprocess.Popen \\n- ls'
 deserialized_data = yam.load(data, Loader=yam.SafeLoader)
 """
         self.run_and_assert(tmpdir, input_code, expected)
 
+    def test_import_alias_add(self, tmpdir):
+        input_code = """
+data = b'!!python/object/apply:subprocess.Popen \\n- ls'
+import yaml as yam
+deserialized_data = yam.load(data)
+"""
+        expected = """
+data = b'!!python/object/apply:subprocess.Popen \\n- ls'
+import yaml as yam
+deserialized_data = yam.load(data, Loader=yam.SafeLoader)
+"""
+        self.run_and_assert(tmpdir, input_code, expected)
+
     def test_preserve_custom_loader(self, tmpdir):
         expected = (
             input_code
         ) = """
         import yaml
         from custom import CustomLoader
```

### Comparing `codemodder-0.96.0/tests/codemods/test_harden_ruamel.py` & `codemodder-0.97.0/tests/codemods/test_harden_ruamel.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_https_connection.py` & `codemodder-0.97.0/tests/codemods/test_https_connection.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_include_exclude.py` & `codemodder-0.97.0/tests/codemods/test_include_exclude.py`

 * *Files 3% similar despite different names*

```diff
@@ -132,7 +132,13 @@
 
     def test_exclude_pixee_with_prefix(self):
         assert self.registry.match_codemods(None, ["pixee*"], sast_only=False) == [
             c
             for c in self.registry.codemods
             if not c.origin == "pixee" and c.id in self.all_ids
         ]
+
+    def test_non_pixee_name_no_match(self):
+        assert self.registry.match_codemods(["secure-random-S2245"], None) == []
+        assert self.registry.match_codemods(None, ["secure-random-S2245"]) == [
+            c for c in self.registry.codemods if c.id in self.all_ids
+        ]
```

### Comparing `codemodder-0.96.0/tests/codemods/test_jwt_decode_verify.py` & `codemodder-0.97.0/tests/codemods/test_jwt_decode_verify.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_lazy_logging.py` & `codemodder-0.97.0/tests/codemods/test_lazy_logging.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_limit_readline.py` & `codemodder-0.97.0/tests/codemods/test_limit_readline.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_literal_or_new_object_identity.py` & `codemodder-0.97.0/tests/codemods/test_literal_or_new_object_identity.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_lxml_safe_parameter_defaults.py` & `codemodder-0.97.0/tests/codemods/test_lxml_safe_parameter_defaults.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_lxml_safe_parsing.py` & `codemodder-0.97.0/tests/codemods/test_lxml_safe_parsing.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_numpy_nan_equality.py` & `codemodder-0.97.0/tests/codemods/test_numpy_nan_equality.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_order_imports.py` & `codemodder-0.97.0/tests/codemods/test_order_imports.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_process_creation_sandbox.py` & `codemodder-0.97.0/tests/codemods/test_process_creation_sandbox.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_remove_assertion_in_pytest_raises.py` & `codemodder-0.97.0/tests/codemods/test_remove_assertion_in_pytest_raises.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_remove_debug_breakpoint.py` & `codemodder-0.97.0/tests/codemods/test_remove_debug_breakpoint.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_remove_future_imports.py` & `codemodder-0.97.0/tests/codemods/test_remove_future_imports.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_remove_module_global.py` & `codemodder-0.97.0/tests/codemods/test_remove_module_global.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_remove_unnecessary_f_str.py` & `codemodder-0.97.0/tests/codemods/test_remove_unnecessary_f_str.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_remove_unused_imports.py` & `codemodder-0.97.0/tests/codemods/test_remove_unused_imports.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_replace_flask_send_file.py` & `codemodder-0.97.0/tests/codemods/test_replace_flask_send_file.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_request_verify.py` & `codemodder-0.97.0/tests/codemods/test_request_verify.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_secure_flask_cookie.py` & `codemodder-0.97.0/tests/codemods/test_secure_flask_cookie.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_secure_flask_session_config.py` & `codemodder-0.97.0/tests/codemods/test_secure_flask_session_config.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_secure_random.py` & `codemodder-0.97.0/tests/codemods/test_secure_random.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_sql_parameterization.py` & `codemodder-0.97.0/tests/codemods/test_sql_parameterization.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_str_concat_in_seq_literal.py` & `codemodder-0.97.0/tests/codemods/test_str_concat_in_seq_literal.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_subprocess_shell_false.py` & `codemodder-0.97.0/tests/codemods/test_subprocess_shell_false.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_tempfile_mktemp.py` & `codemodder-0.97.0/tests/codemods/test_tempfile_mktemp.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_upgrade_sslcontext_minimum_version.py` & `codemodder-0.97.0/tests/codemods/test_upgrade_sslcontext_minimum_version.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_upgrade_sslcontext_tls.py` & `codemodder-0.97.0/tests/codemods/test_upgrade_sslcontext_tls.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_url_sandbox.py` & `codemodder-0.97.0/tests/codemods/test_url_sandbox.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_use_defused_xml.py` & `codemodder-0.97.0/tests/codemods/test_use_defused_xml.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_use_generator.py` & `codemodder-0.97.0/tests/codemods/test_use_generator.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_use_set_literal.py` & `codemodder-0.97.0/tests/codemods/test_use_set_literal.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_walrus_if.py` & `codemodder-0.97.0/tests/codemods/test_walrus_if.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/codemods/test_with_threading_lock.py` & `codemodder-0.97.0/tests/codemods/test_with_threading_lock.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/conftest.py` & `codemodder-0.97.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/dependency_management/test_base_dependency_writer.py` & `codemodder-0.97.0/tests/dependency_management/test_base_dependency_writer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/dependency_management/test_dependency_manager.py` & `codemodder-0.97.0/tests/dependency_management/test_dependency_manager.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/dependency_management/test_pyproject_writer.py` & `codemodder-0.97.0/tests/dependency_management/test_pyproject_writer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/dependency_management/test_requirements_txt_writer.py` & `codemodder-0.97.0/tests/dependency_management/test_requirements_txt_writer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/dependency_management/test_setup_py_writer.py` & `codemodder-0.97.0/tests/dependency_management/test_setup_py_writer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/dependency_management/test_setupcfgt_writer.py` & `codemodder-0.97.0/tests/dependency_management/test_setupcfgt_writer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/project_analysis/file_parsers/test_pyproject_toml_file_parser.py` & `codemodder-0.97.0/tests/project_analysis/file_parsers/test_pyproject_toml_file_parser.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/project_analysis/file_parsers/test_requirements_txt_file_parser.py` & `codemodder-0.97.0/tests/project_analysis/file_parsers/test_requirements_txt_file_parser.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/project_analysis/file_parsers/test_setup_cfg_file_parser.py` & `codemodder-0.97.0/tests/project_analysis/file_parsers/test_setup_cfg_file_parser.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/project_analysis/file_parsers/test_setup_py_file_parser.py` & `codemodder-0.97.0/tests/project_analysis/file_parsers/test_setup_py_file_parser.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/samples/pygoat.semgrep.sarif.json` & `codemodder-0.97.0/tests/samples/pygoat.semgrep.sarif.json`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/samples/semgrep.sarif` & `codemodder-0.97.0/tests/samples/semgrep.sarif`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/samples/sonar_hotspots.json` & `codemodder-0.97.0/tests/samples/sonar_hotspots.json`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/samples/sonar_issues.json` & `codemodder-0.97.0/tests/samples/sonar_issues.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8477502527805865%*

 * *Differences: {"'components'": "{insert: [(90, OrderedDict([('organization', 'pixee'), ('key', "*

 * *                 "'pixee_codemodder-python:src/codemodder/break_or_continue_out_of_loop.py'), "*

 * *                 "('uuid', 'AY8qLg_bGbYA0lXUoQ2e'), ('enabled', True), ('qualifier', 'FIL'), "*

 * *                 "('name', 'break_or_continue_out_of_loop.py'), ('longName', "*

 * *                 "'src/codemodder/break_or_continue_out_of_loop.py'), ('path', "*

 * *                 "'src/codemodder/break_or_continue_out_of_loop.py'), ('pullRe […]*

```diff
@@ -895,18 +895,39 @@
             "key": "pixee_codemodder-python",
             "longName": "codemodder-python",
             "name": "codemodder-python",
             "organization": "pixee",
             "pullRequest": "495",
             "qualifier": "TRK",
             "uuid": "AY8FnbIG_u1xFsthu2wE"
+        },
+        {
+            "enabled": true,
+            "key": "pixee_codemodder-python:src/codemodder/break_or_continue_out_of_loop.py",
+            "longName": "src/codemodder/break_or_continue_out_of_loop.py",
+            "name": "break_or_continue_out_of_loop.py",
+            "organization": "pixee",
+            "path": "src/codemodder/break_or_continue_out_of_loop.py",
+            "pullRequest": "527",
+            "qualifier": "FIL",
+            "uuid": "AY8qLg_bGbYA0lXUoQ2e"
+        },
+        {
+            "enabled": true,
+            "key": "pixee_codemodder-python",
+            "longName": "codemodder-python",
+            "name": "codemodder-python",
+            "organization": "pixee",
+            "pullRequest": "527",
+            "qualifier": "TRK",
+            "uuid": "AY8qHFqG75sAt1eYwm4n"
         }
     ],
-    "debtTotal": 1040,
-    "effortTotal": 1040,
+    "debtTotal": 1050,
+    "effortTotal": 1050,
     "facets": [],
     "issues": [
         {
             "author": "danalitovsky+git@gmail.com",
             "cleanCodeAttribute": "LOGICAL",
             "cleanCodeAttributeCategory": "INTENTIONAL",
             "component": "pixee_codemodder-python:fix_missing_self_or_cls.py",
@@ -2788,14 +2809,48 @@
                 "endLine": 10,
                 "endOffset": 10,
                 "startLine": 10,
                 "startOffset": 6
             },
             "type": "CODE_SMELL",
             "updateDate": "2024-04-23T16:57:31+0200"
+        },
+        {
+            "cleanCodeAttribute": "LOGICAL",
+            "cleanCodeAttributeCategory": "INTENTIONAL",
+            "component": "break_or_continue_out_of_loop.py",
+            "creationDate": "2024-04-29T15:45:53+0200",
+            "debt": "10min",
+            "effort": "10min",
+            "flows": [],
+            "hash": "7aa28ed115707345d0274032757e8991",
+            "impacts": [
+                {
+                    "severity": "HIGH",
+                    "softwareQuality": "RELIABILITY"
+                }
+            ],
+            "key": "AY8qLhIgGbYA0lXUoQ6D",
+            "line": 2,
+            "message": "Remove this \"continue\" statement",
+            "organization": "pixee",
+            "project": "pixee_codemodder-python",
+            "pullRequest": "527",
+            "rule": "python:S1716",
+            "severity": "CRITICAL",
+            "status": "OPEN",
+            "tags": [],
+            "textRange": {
+                "endLine": 2,
+                "endOffset": 12,
+                "startLine": 2,
+                "startOffset": 4
+            },
+            "type": "BUG",
+            "updateDate": "2024-04-29T15:48:13+0200"
         }
     ],
     "organizations": [
         {
             "key": "pixee",
             "name": "Pixee"
         }
@@ -2803,9 +2858,9 @@
     "p": 1,
     "paging": {
         "pageIndex": 1,
         "pageSize": 500,
         "total": 170
     },
     "ps": 500,
-    "total": 42
+    "total": 43
 }
```

### Comparing `codemodder-0.96.0/tests/samples/webgoat_v8.2.0_codeql.sarif` & `codemodder-0.97.0/tests/samples/webgoat_v8.2.0_codeql.sarif`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/test_ancestorpatterns_mixin.py` & `codemodder-0.97.0/tests/test_ancestorpatterns_mixin.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/test_basetype.py` & `codemodder-0.97.0/tests/test_basetype.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/test_cli.py` & `codemodder-0.97.0/tests/test_cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,23 +10,21 @@
 
 
 class TestParseArgs:
     @classmethod
     def setup_class(cls):
         cls.registry = load_registered_codemods()
 
-    @mock.patch("codemodder.cli.logger.error")
-    def test_no_args(self, error_logger, mocker):
+    def test_no_args(self, mocker, caplog):
         with pytest.raises(SystemExit) as err:
             parse_args([], mocker.MagicMock())
         assert err.value.args[0] == 3
-        error_logger.assert_called()
-        assert error_logger.call_args_list[0][0] == (
-            "CLI error: %s",
-            "the following arguments are required: directory",
+        assert (
+            "CLI error: the following arguments are required: directory"
+            in caplog.messages
         )
 
     @pytest.mark.parametrize(
         "cli_args",
         [
             ["--help"],
             [
@@ -103,53 +101,49 @@
         assert mock_print.call_count == 1
 
         results = json.loads(mock_print.call_args_list[0][0][0])
         assert len(results["results"]) == len(core_registry.codemods) - len(
             DEFAULT_EXCLUDED_CODEMODS
         )
 
-    @mock.patch("codemodder.cli.logger.error")
-    def test_bad_output_format(self, error_logger):
+    def test_bad_output_format(self, caplog):
         with pytest.raises(SystemExit) as err:
             parse_args(
                 [
                     "some/path",
                     "--output",
                     "here.txt",
                     "--output-format",
                     "hello",
                 ],
                 self.registry,
             )
         assert err.value.args[0] == 3
-        error_logger.assert_called()
-        assert error_logger.call_args_list[0][0] == (
-            "CLI error: %s",
-            "argument --output-format: invalid choice: 'hello' (choose from 'codetf', 'diff')",
+        assert (
+            "CLI error: argument --output-format: invalid choice: 'hello' (choose from 'codetf', 'diff')"
+            in caplog.messages
         )
 
-    @mock.patch("codemodder.cli.logger.error")
-    def test_bad_option(self, error_logger):
+    def test_bad_option(self, caplog):
         with pytest.raises(SystemExit) as err:
             parse_args(
                 [
                     "some/path",
                     "--output",
                     "here.txt",
                     "--codemod=url-sandbox",
                     "--path-exclude",
                     "*request.py",
                 ],
                 self.registry,
             )
         assert err.value.args[0] == 3
-        error_logger.assert_called()
-        assert error_logger.call_args_list[0][0] == (
-            "CLI error: %s",
-            "ambiguous option: --codemod=url-sandbox could match --codemod-exclude, --codemod-include",
+        assert (
+            "CLI error: ambiguous option: --codemod=url-sandbox could match --codemod-exclude, --codemod-include"
+            in caplog.messages
         )
 
     @pytest.mark.parametrize("codemod", ["secure-random", "pixee:python/secure-random"])
     def test_codemod_name_or_id(self, codemod):
         parse_args(
             [
                 "some/path",
```

### Comparing `codemodder-0.96.0/tests/test_code_directory.py` & `codemodder-0.97.0/tests/test_code_directory.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/test_codemod_docs.py` & `codemodder-0.97.0/tests/test_codemod_docs.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/test_codemodder.py` & `codemodder-0.97.0/tests/test_codemodder.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import logging
+
 import libcst as cst
 import mock
 import pytest
 
 from codemodder.codemodder import find_semgrep_results, run
 from codemodder.diff import create_diff_from_tree
 from codemodder.registry import load_registered_codemods
@@ -190,107 +192,89 @@
         assert exit_code == 0
         mock_compile_results.assert_called()
         transform_apply.assert_called()
 
 
 class TestCodemodIncludeExclude:
 
-    @mock.patch("codemodder.registry.logger.warning")
-    @mock.patch("codemodder.codemodder.logger.info")
     @mock.patch("codemodder.codetf.CodeTF.write_report")
-    def test_codemod_include_no_match(
-        self, write_report, info_logger, warning_logger, dir_structure
-    ):
+    def test_codemod_include_no_match(self, write_report, dir_structure, caplog):
         bad_codemod = "doesntexist"
         code_dir, codetf = dir_structure
         args = [
             str(code_dir),
             "--output",
             str(codetf),
             f"--codemod-include={bad_codemod}",
         ]
+        caplog.set_level(logging.INFO)
+
         run(args)
         write_report.assert_called_once()
 
-        assert any("no codemods to run" in x[0][0] for x in info_logger.call_args_list)
-        assert any(x[0] == ("scanned: %s files", 0) for x in info_logger.call_args_list)
-
-        assert any(
-            f"Requested codemod to include '{bad_codemod}' does not exist." in x[0][0]
-            for x in warning_logger.call_args_list
+        assert "no codemods to run" in caplog.text
+        assert "scanned: 0 files" in caplog.text
+        assert (
+            f"Requested codemod to include '{bad_codemod}' does not exist."
+            in caplog.text
         )
 
-    @mock.patch("codemodder.registry.logger.warning")
-    @mock.patch("codemodder.codemodder.logger.info")
     @mock.patch("codemodder.codetf.CodeTF.write_report")
-    def test_codemod_include_some_match(
-        self, write_report, info_logger, warning_logger, dir_structure
-    ):
+    def test_codemod_include_some_match(self, write_report, dir_structure, caplog):
         bad_codemod = "doesntexist"
         good_codemod = "secure-random"
         code_dir, codetf = dir_structure
         args = [
             str(code_dir),
             "--output",
             str(codetf),
             f"--codemod-include={bad_codemod},{good_codemod}",
         ]
+        caplog.set_level(logging.INFO)
         run(args)
         write_report.assert_called_once()
-        assert any("running codemod %s" in x[0][0] for x in info_logger.call_args_list)
-        assert any(
-            f"Requested codemod to include '{bad_codemod}' does not exist." in x[0][0]
-            for x in warning_logger.call_args_list
+        assert f"running codemod pixee:python/{good_codemod}" in caplog.text
+        assert (
+            f"Requested codemod to include '{bad_codemod}' does not exist."
+            in caplog.text
         )
 
-    @mock.patch("codemodder.registry.logger.warning")
-    @mock.patch("codemodder.codemodder.logger.info")
     @mock.patch("codemodder.codetf.CodeTF.write_report")
-    def test_codemod_exclude_some_match(
-        self, write_report, info_logger, warning_logger, dir_structure
-    ):
+    def test_codemod_exclude_some_match(self, write_report, dir_structure, caplog):
         bad_codemod = "doesntexist"
         good_codemod = "secure-random"
         code_dir, codetf = dir_structure
         args = [
             str(code_dir),
             "--output",
             str(codetf),
             f"--codemod-exclude={bad_codemod},{good_codemod}",
         ]
+        caplog.set_level(logging.INFO)
         run(args)
         write_report.assert_called_once()
-        codemods_that_ran = [
-            x[0][1]
-            for x in info_logger.call_args_list
-            if x[0][0] == "running codemod %s"
-        ]
 
-        assert f"pixee:python/{good_codemod}" not in codemods_that_ran
-        assert any("running codemod %s" in x[0][0] for x in info_logger.call_args_list)
+        assert f"running codemod {good_codemod}" not in caplog.text
+        assert "running codemod " in caplog.text
 
-    @mock.patch("codemodder.registry.logger.warning")
-    @mock.patch("codemodder.codemodder.logger.info")
     @mock.patch("codemodder.codetf.CodeTF.write_report")
     @mock.patch("codemodder.codemods.base_codemod.BaseCodemod.apply")
-    def test_codemod_exclude_no_match(
-        self, apply, write_report, info_logger, warning_logger, dir_structure
-    ):
+    def test_codemod_exclude_no_match(self, apply, write_report, dir_structure, caplog):
         bad_codemod = "doesntexist"
         code_dir, codetf = dir_structure
         args = [
             str(code_dir),
             "--output",
             str(codetf),
             f"--codemod-exclude={bad_codemod}",
         ]
-
+        caplog.set_level(logging.INFO)
         run(args)
         write_report.assert_called_once()
-        assert any("running codemod %s" in x[0][0] for x in info_logger.call_args_list)
+        assert "running codemod " in caplog.text
 
     @mock.patch("codemodder.codemods.semgrep.semgrep_run")
     def test_exclude_all_registered_codemods(self, mock_semgrep_run, dir_structure):
         code_dir, codetf = dir_structure
         assert not codetf.exists()
 
         registry = load_registered_codemods()
```

### Comparing `codemodder-0.96.0/tests/test_codetf.py` & `codemodder-0.97.0/tests/test_codetf.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/test_context.py` & `codemodder-0.97.0/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/test_format_string_parser.py` & `codemodder-0.97.0/tests/test_format_string_parser.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/test_libcst_transformer.py` & `codemodder-0.97.0/tests/test_libcst_transformer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/test_linearize_string_expression.py` & `codemodder-0.97.0/tests/test_linearize_string_expression.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/test_logging.py` & `codemodder-0.97.0/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/test_nameresolution_mixin.py` & `codemodder-0.97.0/tests/test_nameresolution_mixin.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/test_registry.py` & `codemodder-0.97.0/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/test_results.py` & `codemodder-0.97.0/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/test_sarif_processing.py` & `codemodder-0.97.0/tests/test_sarif_processing.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/test_semgrep.py` & `codemodder-0.97.0/tests/test_semgrep.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/transformations/test_clean_code.py` & `codemodder-0.97.0/tests/transformations/test_clean_code.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/transformations/test_remove_empty_string_concatenation.py` & `codemodder-0.97.0/tests/transformations/test_remove_empty_string_concatenation.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.96.0/tests/transformations/test_remove_unused_imports.py` & `codemodder-0.97.0/tests/transformations/test_remove_unused_imports.py`

 * *Files identical despite different names*

