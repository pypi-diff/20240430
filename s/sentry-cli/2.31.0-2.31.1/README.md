# Comparing `tmp/sentry_cli-2.31.0.tar.gz` & `tmp/sentry_cli-2.31.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentry_cli-2.31.0.tar", last modified: Wed Mar 27 15:48:13 2024, max compression
+gzip compressed data, was "sentry_cli-2.31.1.tar", last modified: Tue Apr 30 15:03:35 2024, max compression
```

## Comparing `sentry_cli-2.31.0.tar` & `sentry_cli-2.31.1.tar`

### file list

```diff
@@ -1,135 +1,143 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:48:13.300173 sentry_cli-2.31.0/
--rw-r--r--   0 runner    (1001) docker     (127)    92408 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/Cargo.lock
--rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-03-27 15:48:13.300173 sentry_cli-2.31.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/build.rs
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:48:13.300173 sentry_cli-2.31.0/sentry_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-03-27 15:48:13.000000 sentry_cli-2.31.0/sentry_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-03-27 15:48:13.000000 sentry_cli-2.31.0/sentry_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 15:48:13.000000 sentry_cli-2.31.0/sentry_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 15:48:13.000000 sentry_cli-2.31.0/sentry_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-03-27 15:48:13.300173 sentry_cli-2.31.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:48:13.284172 sentry_cli-2.31.0/src/
--rw-r--r--   0 runner    (1001) docker     (127)    90347 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/api.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/bashsupport.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:48:13.288172 sentry_cli-2.31.0/src/commands/
--rw-r--r--   0 runner    (1001) docker     (127)     8798 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/bash_hook.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:48:13.288172 sentry_cli-2.31.0/src/commands/debug_files/
--rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/debug_files/bundle_jvm.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/debug_files/bundle_sources.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/debug_files/check.rs
--rw-r--r--   0 runner    (1001) docker     (127)    11579 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/debug_files/find.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/debug_files/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/debug_files/print_sources.rs
--rw-r--r--   0 runner    (1001) docker     (127)    14566 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/debug_files/upload.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:48:13.288172 sentry_cli-2.31.0/src/commands/deploys/
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/deploys/list.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/deploys/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/deploys/new.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:48:13.288172 sentry_cli-2.31.0/src/commands/events/
--rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/events/list.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/events/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:48:13.288172 sentry_cli-2.31.0/src/commands/files/
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/files/delete.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/files/list.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/files/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     9332 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/files/upload.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/info.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:48:13.292173 sentry_cli-2.31.0/src/commands/issues/
--rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/issues/list.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/issues/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/issues/mute.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/issues/resolve.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/issues/unresolve.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/login.rs
--rw-r--r--   0 runner    (1001) docker     (127)    10767 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:48:13.292173 sentry_cli-2.31.0/src/commands/monitors/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/monitors/list.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/monitors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     7195 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/monitors/run.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:48:13.292173 sentry_cli-2.31.0/src/commands/organizations/
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/organizations/list.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/organizations/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:48:13.292173 sentry_cli-2.31.0/src/commands/projects/
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/projects/list.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/projects/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:48:13.292173 sentry_cli-2.31.0/src/commands/react_native/
--rw-r--r--   0 runner    (1001) docker     (127)     7847 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/react_native/appcenter.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/react_native/gradle.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/react_native/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)    24737 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/react_native/xcode.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:48:13.292173 sentry_cli-2.31.0/src/commands/releases/
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/releases/archive.rs
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/releases/delete.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/releases/finalize.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/releases/info.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/releases/list.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/releases/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/releases/new.rs
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/releases/propose_version.rs
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/releases/restore.rs
--rw-r--r--   0 runner    (1001) docker     (127)     8602 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/releases/set_commits.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:48:13.296172 sentry_cli-2.31.0/src/commands/repos/
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/repos/list.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/repos/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/send_envelope.rs
--rw-r--r--   0 runner    (1001) docker     (127)    11841 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/send_event.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:48:13.296172 sentry_cli-2.31.0/src/commands/sourcemaps/
--rw-r--r--   0 runner    (1001) docker     (127)    16796 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/sourcemaps/explain.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/sourcemaps/inject.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/sourcemaps/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/sourcemaps/resolve.rs
--rw-r--r--   0 runner    (1001) docker     (127)    17093 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/sourcemaps/upload.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/uninstall.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/update.rs
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/upload_dif.rs
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/upload_dsym.rs
--rw-r--r--   0 runner    (1001) docker     (127)    10717 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/commands/upload_proguard.rs
--rw-r--r--   0 runner    (1001) docker     (127)    25181 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/config.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/constants.rs
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/main.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:48:13.300173 sentry_cli-2.31.0/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/utils/android.rs
--rw-r--r--   0 runner    (1001) docker     (127)     8095 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/utils/appcenter.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/utils/args.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:48:13.300173 sentry_cli-2.31.0/src/utils/auth_token/
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/utils/auth_token/auth_token_impl.rs
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/utils/auth_token/error.rs
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/utils/auth_token/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/utils/auth_token/org_auth_token.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/utils/auth_token/test.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/utils/auth_token/user_auth_token.rs
--rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/utils/chunks.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/utils/cordova.rs
--rw-r--r--   0 runner    (1001) docker     (127)    14695 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/utils/dif.rs
--rw-r--r--   0 runner    (1001) docker     (127)    72264 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/utils/dif_upload.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/utils/event.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5195 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/utils/file_search.rs
--rw-r--r--   0 runner    (1001) docker     (127)    21494 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/utils/file_upload.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/utils/formatting.rs
--rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/utils/fs.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/utils/http.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/utils/logging.rs
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/utils/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/utils/progress.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/utils/releases.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/utils/retry.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:48:13.300173 sentry_cli-2.31.0/src/utils/snapshots/
--rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_default_twenty.snap
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_ignore_missing.snap
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_base.snap
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_previous_commit.snap
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/utils/snapshots/sentry_cli__utils__vcs__get_commits_from_git.snap
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:48:13.300173 sentry_cli-2.31.0/src/utils/sourcemaps/
--rw-r--r--   0 runner    (1001) docker     (127)    19158 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/utils/sourcemaps/inject.rs
--rw-r--r--   0 runner    (1001) docker     (127)    47198 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/utils/sourcemaps.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/utils/system.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/utils/ui.rs
--rw-r--r--   0 runner    (1001) docker     (127)     8628 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/utils/update.rs
--rw-r--r--   0 runner    (1001) docker     (127)    36324 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/utils/vcs.rs
--rw-r--r--   0 runner    (1001) docker     (127)    19447 2024-03-27 15:48:05.000000 sentry_cli-2.31.0/src/utils/xcode.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:35.945649 sentry_cli-2.31.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    92408 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/Cargo.lock
+-rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-04-30 15:03:35.945649 sentry_cli-2.31.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/build.rs
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:35.945649 sentry_cli-2.31.1/sentry_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-04-30 15:03:35.000000 sentry_cli-2.31.1/sentry_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-04-30 15:03:35.000000 sentry_cli-2.31.1/sentry_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:03:35.000000 sentry_cli-2.31.1/sentry_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:03:35.000000 sentry_cli-2.31.1/sentry_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-30 15:03:35.949649 sentry_cli-2.31.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:35.929649 sentry_cli-2.31.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:35.933649 sentry_cli-2.31.1/src/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/api/connection_manager.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/api/encoding.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:35.933649 sentry_cli-2.31.1/src/api/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/api/errors/api_error.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/api/errors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/api/errors/sentry_error.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    83574 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/api/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/api/pagination.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/bashsupport.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:35.933649 sentry_cli-2.31.1/src/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     8798 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/bash_hook.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:35.933649 sentry_cli-2.31.1/src/commands/debug_files/
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/debug_files/bundle_jvm.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/debug_files/bundle_sources.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/debug_files/check.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    11579 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/debug_files/find.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/debug_files/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/debug_files/print_sources.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    14566 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/debug_files/upload.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:35.933649 sentry_cli-2.31.1/src/commands/deploys/
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/deploys/list.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/deploys/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/deploys/new.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:35.937649 sentry_cli-2.31.1/src/commands/events/
+-rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/events/list.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/events/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:35.937649 sentry_cli-2.31.1/src/commands/files/
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/files/delete.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/files/list.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/files/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     9332 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/files/upload.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/info.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:35.937649 sentry_cli-2.31.1/src/commands/issues/
+-rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/issues/list.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/issues/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/issues/mute.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/issues/resolve.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/issues/unresolve.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/login.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    10767 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:35.937649 sentry_cli-2.31.1/src/commands/monitors/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/monitors/list.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/monitors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     7195 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/monitors/run.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:35.937649 sentry_cli-2.31.1/src/commands/organizations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/organizations/list.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/organizations/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:35.937649 sentry_cli-2.31.1/src/commands/projects/
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/projects/list.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/projects/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:35.937649 sentry_cli-2.31.1/src/commands/react_native/
+-rw-r--r--   0 runner    (1001) docker     (127)     7847 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/react_native/appcenter.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/react_native/gradle.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/react_native/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    24737 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/react_native/xcode.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:35.941649 sentry_cli-2.31.1/src/commands/releases/
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/releases/archive.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/releases/delete.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/releases/finalize.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/releases/info.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/releases/list.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/releases/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/releases/new.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/releases/propose_version.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/releases/restore.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     8602 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/releases/set_commits.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:35.941649 sentry_cli-2.31.1/src/commands/repos/
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/repos/list.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/repos/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/send_envelope.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    11841 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/send_event.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:35.941649 sentry_cli-2.31.1/src/commands/sourcemaps/
+-rw-r--r--   0 runner    (1001) docker     (127)    16796 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/sourcemaps/explain.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/sourcemaps/inject.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/sourcemaps/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/sourcemaps/resolve.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    17093 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/sourcemaps/upload.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/uninstall.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/update.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/upload_dif.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/upload_dsym.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    10718 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/commands/upload_proguard.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    25588 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/config.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/constants.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/main.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:35.945649 sentry_cli-2.31.1/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/android.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     8095 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/appcenter.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/args.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:35.945649 sentry_cli-2.31.1/src/utils/auth_token/
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/auth_token/auth_token_impl.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/auth_token/error.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/auth_token/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/auth_token/org_auth_token.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/auth_token/test.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/auth_token/user_auth_token.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/chunks.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/cordova.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    14695 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/dif.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    72264 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/dif_upload.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/event.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     5195 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/file_search.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    21494 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/file_upload.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/formatting.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/fs.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/http.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/logging.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/progress.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/releases.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/retry.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:35.945649 sentry_cli-2.31.1/src/utils/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_default_twenty.snap
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_ignore_missing.snap
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_base.snap
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_previous_commit.snap
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/snapshots/sentry_cli__utils__vcs__get_commits_from_git.snap
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:03:35.945649 sentry_cli-2.31.1/src/utils/sourcemaps/
+-rw-r--r--   0 runner    (1001) docker     (127)    19158 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/sourcemaps/inject.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    47198 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/sourcemaps.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/system.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/ui.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     8628 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/update.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    36324 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/vcs.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    19447 2024-04-30 15:03:29.000000 sentry_cli-2.31.1/src/utils/xcode.rs
```

### Comparing `sentry_cli-2.31.0/Cargo.lock` & `sentry_cli-2.31.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -2428,15 +2428,15 @@
  "once_cell",
  "regex",
  "sentry-core",
 ]
 
 [[package]]
 name = "sentry-cli"
-version = "2.31.0"
+version = "2.31.1"
 dependencies = [
  "anyhow",
  "anylog",
  "backoff",
  "backtrace",
  "brotli2",
  "bytecount",
```

### Comparing `sentry_cli-2.31.0/Cargo.toml` & `sentry_cli-2.31.1/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [package]
 authors = ["Armin Ronacher <armin.ronacher@active-4.com>"]
 build = "build.rs"
 name = "sentry-cli"
-version = "2.31.0"
+version = "2.31.1"
 edition = "2021"
 rust-version = "1.65"
 
 [dependencies]
 anylog = "0.6.3"
 anyhow = { version = "1.0.69", features = ["backtrace"] }
 backoff = "0.4.0"
```

### Comparing `sentry_cli-2.31.0/LICENSE` & `sentry_cli-2.31.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/PKG-INFO` & `sentry_cli-2.31.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry_cli
-Version: 2.31.0
+Version: 2.31.1
 Summary: A command line utility to work with Sentry.
 Home-page: https://github.com/getsentry/sentry-cli
 Author: Sentry
 Author-email: oss@sentry.io
 License: BSD-3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sentry_cli Version: 2.31.0 Summary: A command line
+Metadata-Version: 2.1 Name: sentry_cli Version: 2.31.1 Summary: A command line
 utility to work with Sentry. Home-page: https://github.com/getsentry/sentry-cli
 Author: Sentry Author-email: oss@sentry.io License: BSD-3-Clause Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: Implementation :: CPython Classifier:
 Programming Language :: Python :: Implementation :: PyPy Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `sentry_cli-2.31.0/README.md` & `sentry_cli-2.31.1/README.md`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/build.rs` & `sentry_cli-2.31.1/build.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/sentry_cli.egg-info/PKG-INFO` & `sentry_cli-2.31.1/sentry_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry_cli
-Version: 2.31.0
+Version: 2.31.1
 Summary: A command line utility to work with Sentry.
 Home-page: https://github.com/getsentry/sentry-cli
 Author: Sentry
 Author-email: oss@sentry.io
 License: BSD-3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sentry_cli Version: 2.31.0 Summary: A command line
+Metadata-Version: 2.1 Name: sentry_cli Version: 2.31.1 Summary: A command line
 utility to work with Sentry. Home-page: https://github.com/getsentry/sentry-cli
 Author: Sentry Author-email: oss@sentry.io License: BSD-3-Clause Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: Implementation :: CPython Classifier:
 Programming Language :: Python :: Implementation :: PyPy Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `sentry_cli-2.31.0/sentry_cli.egg-info/SOURCES.txt` & `sentry_cli-2.31.1/sentry_cli.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -7,19 +7,25 @@
 pyproject.toml
 setup.cfg
 setup.py
 sentry_cli.egg-info/PKG-INFO
 sentry_cli.egg-info/SOURCES.txt
 sentry_cli.egg-info/dependency_links.txt
 sentry_cli.egg-info/top_level.txt
-src/api.rs
 src/bashsupport.sh
 src/config.rs
 src/constants.rs
 src/main.rs
+src/api/connection_manager.rs
+src/api/encoding.rs
+src/api/mod.rs
+src/api/pagination.rs
+src/api/errors/api_error.rs
+src/api/errors/mod.rs
+src/api/errors/sentry_error.rs
 src/commands/bash_hook.rs
 src/commands/info.rs
 src/commands/login.rs
 src/commands/mod.rs
 src/commands/send_envelope.rs
 src/commands/send_event.rs
 src/commands/uninstall.rs
```

### Comparing `sentry_cli-2.31.0/setup.cfg` & `sentry_cli-2.31.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/setup.py` & `sentry_cli-2.31.1/setup.py`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/api.rs` & `sentry_cli-2.31.1/src/api/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 //! This module implements the API access to the Sentry API as well
 //! as some other APIs we interact with.  In particular it can talk
 //! to the GitHub API to figure out if there are new releases of the
 //! sentry-cli tool.
 
+mod connection_manager;
+mod encoding;
+mod errors;
+mod pagination;
+
 use std::borrow::Cow;
 use std::cell::RefCell;
 use std::collections::{HashMap, HashSet};
 use std::ffi::OsStr;
 use std::fs::{create_dir_all, File};
 use std::io::{self, Read, Write};
 use std::path::Path;
 use std::rc::Rc;
-use std::str::FromStr;
 use std::sync::Arc;
 use std::{env, fmt};
 
 use anyhow::{Context, Result};
 use backoff::backoff::Backoff;
 use brotli2::write::BrotliEncoder;
 #[cfg(target_os = "macos")]
@@ -23,142 +27,42 @@
 use chrono::{DateTime, FixedOffset, Utc};
 use clap::ArgMatches;
 use flate2::write::GzEncoder;
 use if_chain::if_chain;
 use lazy_static::lazy_static;
 use log::{debug, info, warn};
 use parking_lot::{Mutex, RwLock};
-use percent_encoding::{utf8_percent_encode, AsciiSet, CONTROLS};
 use regex::{Captures, Regex};
 use sentry::protocol::{Exception, Values};
 use serde::de::{DeserializeOwned, Deserializer};
 use serde::{Deserialize, Serialize};
 use sha1_smol::Digest;
 use symbolic::common::DebugId;
 use symbolic::debuginfo::ObjectKind;
 use url::Url;
 use uuid::Uuid;
 
+use crate::api::errors::ProjectRenamedError;
 use crate::config::{Auth, Config};
 use crate::constants::{ARCH, DEFAULT_URL, EXT, PLATFORM, RELEASE_REGISTRY_LATEST_URL, VERSION};
 use crate::utils::file_upload::UploadContext;
-use crate::utils::http::{self, is_absolute_url, parse_link_header};
+use crate::utils::http::{self, is_absolute_url};
 use crate::utils::progress::ProgressBar;
 use crate::utils::retry::{get_default_backoff, DurationAsMilliseconds};
 use crate::utils::sourcemaps::get_sourcemap_reference_from_headers;
 use crate::utils::ui::{capitalize_string, make_byte_progress_bar};
 
-// Based on https://docs.rs/percent-encoding/1.0.1/src/percent_encoding/lib.rs.html#104
-// WHATWG Spec: https://url.spec.whatwg.org/#percent-encoded-bytes
-// RFC3986 Reserved Characters: https://www.rfc-editor.org/rfc/rfc3986#section-2.2
-const QUERY_ENCODE_SET: AsciiSet = CONTROLS
-    .add(b' ')
-    .add(b'"')
-    .add(b'#')
-    .add(b'<')
-    .add(b'>')
-    .add(b'+');
-const PATH_SEGMENT_ENCODE_SET: AsciiSet = QUERY_ENCODE_SET
-    .add(b'`')
-    .add(b'?')
-    .add(b'{')
-    .add(b'}')
-    .add(b'%')
-    .add(b'/');
-
-/// Wrapper that escapes arguments for URL path segments.
-pub struct PathArg<A: fmt::Display>(A);
-
-/// Wrapper that escapes arguments for URL query segments.
-pub struct QueryArg<A: fmt::Display>(A);
-
-struct CurlConnectionManager;
-
-impl r2d2::ManageConnection for CurlConnectionManager {
-    type Connection = curl::easy::Easy;
-    type Error = curl::Error;
-
-    fn connect(&self) -> Result<curl::easy::Easy, curl::Error> {
-        Ok(curl::easy::Easy::new())
-    }
-
-    fn is_valid(&self, _conn: &mut curl::easy::Easy) -> Result<(), curl::Error> {
-        Ok(())
-    }
-
-    fn has_broken(&self, _conn: &mut curl::easy::Easy) -> bool {
-        false
-    }
-}
+use connection_manager::CurlConnectionManager;
+use encoding::{PathArg, QueryArg};
+use errors::{ApiError, ApiErrorKind, ApiResult, SentryError};
 
 lazy_static! {
     static ref API: Mutex<Option<Arc<Api>>> = Mutex::new(None);
 }
 
-#[derive(Debug, Clone)]
-pub struct Link {
-    results: bool,
-    cursor: String,
-}
-
-#[derive(Debug, Default, Clone)]
-pub struct Pagination {
-    next: Option<Link>,
-}
-
-impl Pagination {
-    pub fn into_next_cursor(self) -> Option<String> {
-        self.next
-            .and_then(|x| if x.results { Some(x.cursor) } else { None })
-    }
-}
-
-impl FromStr for Pagination {
-    type Err = ();
-
-    fn from_str(s: &str) -> Result<Pagination, ()> {
-        let mut rv = Pagination::default();
-        for item in parse_link_header(s) {
-            let target = match item.get("rel") {
-                Some(&"next") => &mut rv.next,
-                _ => continue,
-            };
-
-            *target = Some(Link {
-                results: item.get("results") == Some(&"true"),
-                cursor: (*item.get("cursor").unwrap_or(&"")).to_string(),
-            });
-        }
-
-        Ok(rv)
-    }
-}
-
-impl<A: fmt::Display> fmt::Display for QueryArg<A> {
-    fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
-        utf8_percent_encode(&format!("{}", self.0), &QUERY_ENCODE_SET).fmt(f)
-    }
-}
-
-impl<A: fmt::Display> fmt::Display for PathArg<A> {
-    fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
-        // if we put values into the path we need to url encode them.  However
-        // special care needs to be taken for any slash character or path
-        // segments that would end up as ".." or "." for security reasons.
-        // Since we cannot handle slashes there we just replace them with the
-        // unicode replacement character as a quick workaround.  This will
-        // typically result in 404s from the server.
-        let mut val = format!("{}", self.0).replace('/', "\u{fffd}");
-        if val == ".." || val == "." {
-            val = "\u{fffd}".into();
-        }
-        utf8_percent_encode(&val, &PATH_SEGMENT_ENCODE_SET).fmt(f)
-    }
-}
-
 #[derive(Clone)]
 pub enum ProgressBarMode {
     Disabled,
     Request,
     Response,
     Shared((Arc<ProgressBar>, u64, usize, Arc<RwLock<Vec<u64>>>)),
 }
@@ -196,141 +100,14 @@
 
 pub struct RegionSpecificApi<'a> {
     api: &'a AuthenticatedApi<'a>,
     org: &'a str,
     region_url: Option<Box<str>>,
 }
 
-#[derive(Debug, thiserror::Error)]
-pub struct SentryError {
-    status: u32,
-    detail: Option<String>,
-    extra: Option<serde_json::Value>,
-}
-
-impl fmt::Display for SentryError {
-    fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
-        let detail = self.detail.as_deref().unwrap_or("");
-        write!(
-            f,
-            "sentry reported an error: {} (http status: {})",
-            if detail.is_empty() {
-                match self.status {
-                    400 => "bad request",
-                    401 => "unauthorized",
-                    404 => "not found",
-                    500 => "internal server error",
-                    502 => "bad gateway",
-                    504 => "gateway timeout",
-                    _ => "unknown error",
-                }
-            } else {
-                detail
-            },
-            self.status
-        )?;
-        if let Some(ref extra) = self.extra {
-            write!(f, "\n  {extra:?}")?;
-        }
-        Ok(())
-    }
-}
-
-#[derive(Clone, Debug, thiserror::Error)]
-#[error("project was renamed to '{0}'\nPlease use this slug in your .sentryclirc file, sentry.properties file or in the CLI --project parameter")]
-pub struct ProjectRenamedError(String);
-
-/// Represents API errors.
-#[derive(Copy, Clone, Eq, PartialEq, Debug, thiserror::Error)]
-pub enum ApiErrorKind {
-    #[error("could not serialize value as JSON")]
-    CannotSerializeAsJson,
-    #[error("could not parse JSON response")]
-    BadJson,
-    #[error("not a JSON response")]
-    NotJson,
-    #[error("request failed because API URL was incorrectly formatted")]
-    BadApiUrl,
-    #[error("organization not found")]
-    OrganizationNotFound,
-    #[error("resource not found")]
-    ResourceNotFound,
-    #[error("Project not found. Please check that you entered the project and organization slugs correctly.")]
-    ProjectNotFound,
-    #[error("release not found")]
-    ReleaseNotFound,
-    #[error("chunk upload endpoint not supported by sentry server")]
-    ChunkUploadNotSupported,
-    #[error("API request failed")]
-    RequestFailed,
-    #[error("could not compress data")]
-    CompressionFailed,
-    #[error("region overrides cannot be applied to absolute urls")]
-    InvalidRegionRequest,
-    #[error(
-        "Auth token is required for this request. Please run `sentry-cli login` and try again!"
-    )]
-    AuthMissing,
-}
-
-#[derive(Debug, thiserror::Error)]
-pub struct ApiError {
-    inner: ApiErrorKind,
-    #[source]
-    source: Option<anyhow::Error>,
-}
-
-impl fmt::Display for ApiError {
-    fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
-        fmt::Display::fmt(&self.inner, f)
-    }
-}
-
-impl ApiError {
-    pub fn with_source<E: Into<anyhow::Error>>(kind: ApiErrorKind, source: E) -> ApiError {
-        ApiError {
-            inner: kind,
-            source: Some(source.into()),
-        }
-    }
-
-    pub fn kind(&self) -> ApiErrorKind {
-        self.inner
-    }
-
-    fn set_source<E: Into<anyhow::Error>>(mut self, source: E) -> ApiError {
-        self.source = Some(source.into());
-        self
-    }
-}
-
-impl From<ApiErrorKind> for ApiError {
-    fn from(kind: ApiErrorKind) -> ApiError {
-        ApiError {
-            inner: kind,
-            source: None,
-        }
-    }
-}
-
-impl From<curl::Error> for ApiError {
-    fn from(err: curl::Error) -> ApiError {
-        ApiError::from(ApiErrorKind::RequestFailed).set_source(err)
-    }
-}
-
-impl From<curl::FormError> for ApiError {
-    fn from(err: curl::FormError) -> ApiError {
-        ApiError::from(ApiErrorKind::RequestFailed).set_source(err)
-    }
-}
-
-/// Shortcut alias for results of this module.
-pub type ApiResult<T> = Result<T, ApiError>;
-
 /// Represents an HTTP method that is used by the API.
 #[derive(Eq, PartialEq, Debug)]
 pub enum Method {
     Get,
     Post,
     Put,
     Delete,
@@ -752,17 +529,17 @@
                 if rv.is_empty() {
                     return Err(ApiErrorKind::ReleaseNotFound.into());
                 } else {
                     break;
                 }
             }
 
-            let pagination = resp.pagination();
+            let next = resp.next_pagination_cursor();
             rv.extend(resp.convert::<Vec<Artifact>>()?);
-            if let Some(next) = pagination.into_next_cursor() {
+            if let Some(next) = next {
                 cursor = next;
             } else {
                 break;
             }
         }
         Ok(rv)
     }
@@ -1353,17 +1130,17 @@
             if resp.status() == 404 || (resp.status() == 400 && !cursor.is_empty()) {
                 if rv.is_empty() {
                     return Err(ApiErrorKind::ResourceNotFound.into());
                 } else {
                     break;
                 }
             }
-            let pagination = resp.pagination();
+            let next = resp.next_pagination_cursor();
             rv.extend(resp.convert::<Vec<Organization>>()?);
-            if let Some(next) = pagination.into_next_cursor() {
+            if let Some(next) = next {
                 cursor = next;
             } else {
                 break;
             }
         }
         Ok(rv)
     }
@@ -1397,17 +1174,17 @@
             if resp.status() == 404 || (resp.status() == 400 && !cursor.is_empty()) {
                 if rv.is_empty() {
                     return Err(ApiErrorKind::ResourceNotFound.into());
                 } else {
                     break;
                 }
             }
-            let pagination = resp.pagination();
+            let next = resp.next_pagination_cursor();
             rv.extend(resp.convert::<Vec<Monitor>>()?);
-            if let Some(next) = pagination.into_next_cursor() {
+            if let Some(next) = next {
                 cursor = next;
             } else {
                 break;
             }
         }
         Ok(rv)
     }
@@ -1425,17 +1202,17 @@
             if resp.status() == 404 || (resp.status() == 400 && !cursor.is_empty()) {
                 if rv.is_empty() {
                     return Err(ApiErrorKind::OrganizationNotFound.into());
                 } else {
                     break;
                 }
             }
-            let pagination = resp.pagination();
+            let next = resp.next_pagination_cursor();
             rv.extend(resp.convert::<Vec<Project>>()?);
-            if let Some(next) = pagination.into_next_cursor() {
+            if let Some(next) = next {
                 cursor = next;
             } else {
                 break;
             }
         }
         Ok(rv)
     }
@@ -1465,22 +1242,22 @@
                 if rv.is_empty() {
                     return Err(ApiErrorKind::ProjectNotFound.into());
                 } else {
                     break;
                 }
             }
 
-            let pagination = resp.pagination();
+            let next = resp.next_pagination_cursor();
             rv.extend(resp.convert::<Vec<ProcessedEvent>>()?);
 
             if requests_no == max_pages {
                 break;
             }
 
-            if let Some(next) = pagination.into_next_cursor() {
+            if let Some(next) = next {
                 cursor = next;
             } else {
                 break;
             }
         }
 
         Ok(rv)
@@ -1491,15 +1268,15 @@
         &self,
         org: &str,
         project: &str,
         max_pages: usize,
         query: Option<String>,
     ) -> ApiResult<Vec<Issue>> {
         let mut rv = vec![];
-        let mut cursor = "".to_string();
+        let mut cursor = String::from("");
         let mut requests_no = 0;
 
         let url = if let Some(query) = query {
             format!(
                 "/projects/{}/{}/issues/?query={}&",
                 PathArg(org),
                 PathArg(project),
@@ -1518,22 +1295,22 @@
                 if rv.is_empty() {
                     return Err(ApiErrorKind::ProjectNotFound.into());
                 } else {
                     break;
                 }
             }
 
-            let pagination = resp.pagination();
+            let next = resp.next_pagination_cursor();
             rv.extend(resp.convert::<Vec<Issue>>()?);
 
             if requests_no == max_pages {
                 break;
             }
 
-            if let Some(next) = pagination.into_next_cursor() {
+            if let Some(next) = next {
                 cursor = next;
             } else {
                 break;
             }
         }
 
         Ok(rv)
@@ -1549,21 +1326,20 @@
                 PathArg(org),
                 QueryArg(&cursor)
             );
             let resp = self.request(Method::Get, &path)?.send()?;
             if resp.status() == 404 {
                 break;
             } else {
-                let pagination = resp.pagination();
-                rv.extend(resp.convert::<Vec<Repo>>()?);
-                if let Some(next) = pagination.into_next_cursor() {
+                if let Some(next) = resp.next_pagination_cursor() {
                     cursor = next;
                 } else {
                     break;
                 }
+                rv.extend(resp.convert::<Vec<Repo>>()?);
             }
         }
         Ok(rv)
     }
 
     /// Looks up an event, which was already processed by Sentry and returns it.
     /// If it does not exist `None` will be returned.
@@ -2142,15 +1918,15 @@
     /// Like `deserialize` but consumes the response and will convert
     /// failed requests into proper errors.
     pub fn convert<T: DeserializeOwned>(self) -> ApiResult<T> {
         self.into_result().and_then(|x| x.deserialize())
     }
 
     /// Like convert but produces resource not found errors.
-    pub fn convert_rnf<T: DeserializeOwned>(self, res_err: ApiErrorKind) -> ApiResult<T> {
+    fn convert_rnf<T: DeserializeOwned>(self, res_err: ApiErrorKind) -> ApiResult<T> {
         match self.status() {
             301 | 302 if res_err == ApiErrorKind::ProjectNotFound => {
                 #[derive(Deserialize, Debug)]
                 struct ErrorDetail {
                     slug: String,
                 }
 
@@ -2188,19 +1964,18 @@
             if header_key.eq_ignore_ascii_case(key) {
                 return Some(header_value);
             }
         }
         None
     }
 
-    /// Returns the pagination info
-    pub fn pagination(&self) -> Pagination {
+    fn next_pagination_cursor(&self) -> Option<String> {
         self.get_header("link")
-            .and_then(|x| x.parse().ok())
-            .unwrap_or_default()
+            .and_then(pagination::next_cursor)
+            .map(String::from)
     }
 
     /// Returns true if the response is JSON.
     pub fn is_json(&self) -> bool {
         self.get_header("content-type")
             .and_then(|x| x.split(';').next())
             .unwrap_or("")
```

### Comparing `sentry_cli-2.31.0/src/bashsupport.sh` & `sentry_cli-2.31.1/src/bashsupport.sh`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/bash_hook.rs` & `sentry_cli-2.31.1/src/commands/bash_hook.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/debug_files/bundle_jvm.rs` & `sentry_cli-2.31.1/src/commands/debug_files/bundle_jvm.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/debug_files/bundle_sources.rs` & `sentry_cli-2.31.1/src/commands/debug_files/bundle_sources.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/debug_files/check.rs` & `sentry_cli-2.31.1/src/commands/debug_files/check.rs`

 * *Files 8% similar despite different names*

```diff
@@ -39,14 +39,22 @@
                 .help("Format outputs as JSON."),
         )
 }
 
 pub fn execute(matches: &ArgMatches) -> Result<()> {
     let path = Path::new(matches.get_one::<String>("path").unwrap());
 
+    if path.is_dir() {
+        anyhow::bail!(
+            "This command can only check individual debug files, but the provided \
+            path leads to a directory. Please a pass a path to an individual file, \
+            instead!"
+        );
+    }
+
     // which types should we consider?
     let ty = matches
         .get_one::<String>("type")
         .map(|t| t.parse().unwrap());
     let dif = DifFile::open_path(path, ty)?;
 
     if matches.get_flag("json") {
```

### Comparing `sentry_cli-2.31.0/src/commands/debug_files/find.rs` & `sentry_cli-2.31.1/src/commands/debug_files/find.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/debug_files/mod.rs` & `sentry_cli-2.31.1/src/commands/debug_files/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/debug_files/print_sources.rs` & `sentry_cli-2.31.1/src/commands/debug_files/print_sources.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/debug_files/upload.rs` & `sentry_cli-2.31.1/src/commands/debug_files/upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/deploys/list.rs` & `sentry_cli-2.31.1/src/commands/deploys/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/deploys/mod.rs` & `sentry_cli-2.31.1/src/commands/deploys/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/deploys/new.rs` & `sentry_cli-2.31.1/src/commands/deploys/new.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/events/list.rs` & `sentry_cli-2.31.1/src/commands/events/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/events/mod.rs` & `sentry_cli-2.31.1/src/commands/events/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/files/delete.rs` & `sentry_cli-2.31.1/src/commands/files/delete.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/files/list.rs` & `sentry_cli-2.31.1/src/commands/files/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/files/mod.rs` & `sentry_cli-2.31.1/src/commands/files/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/files/upload.rs` & `sentry_cli-2.31.1/src/commands/files/upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/info.rs` & `sentry_cli-2.31.1/src/commands/info.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/issues/list.rs` & `sentry_cli-2.31.1/src/commands/issues/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/issues/mod.rs` & `sentry_cli-2.31.1/src/commands/issues/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/issues/mute.rs` & `sentry_cli-2.31.1/src/commands/issues/mute.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/issues/resolve.rs` & `sentry_cli-2.31.1/src/commands/issues/resolve.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/issues/unresolve.rs` & `sentry_cli-2.31.1/src/commands/issues/unresolve.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/login.rs` & `sentry_cli-2.31.1/src/commands/login.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/mod.rs` & `sentry_cli-2.31.1/src/commands/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/monitors/list.rs` & `sentry_cli-2.31.1/src/commands/monitors/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/monitors/mod.rs` & `sentry_cli-2.31.1/src/commands/monitors/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/monitors/run.rs` & `sentry_cli-2.31.1/src/commands/monitors/run.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/organizations/list.rs` & `sentry_cli-2.31.1/src/commands/organizations/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/organizations/mod.rs` & `sentry_cli-2.31.1/src/commands/organizations/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/projects/list.rs` & `sentry_cli-2.31.1/src/commands/projects/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/projects/mod.rs` & `sentry_cli-2.31.1/src/commands/projects/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/react_native/appcenter.rs` & `sentry_cli-2.31.1/src/commands/react_native/appcenter.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/react_native/gradle.rs` & `sentry_cli-2.31.1/src/commands/react_native/gradle.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/react_native/mod.rs` & `sentry_cli-2.31.1/src/commands/react_native/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/react_native/xcode.rs` & `sentry_cli-2.31.1/src/commands/react_native/xcode.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/releases/archive.rs` & `sentry_cli-2.31.1/src/commands/releases/archive.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/releases/delete.rs` & `sentry_cli-2.31.1/src/commands/releases/delete.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/releases/finalize.rs` & `sentry_cli-2.31.1/src/commands/releases/finalize.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/releases/info.rs` & `sentry_cli-2.31.1/src/commands/releases/info.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/releases/list.rs` & `sentry_cli-2.31.1/src/commands/releases/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/releases/mod.rs` & `sentry_cli-2.31.1/src/commands/releases/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/releases/new.rs` & `sentry_cli-2.31.1/src/commands/releases/new.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/releases/restore.rs` & `sentry_cli-2.31.1/src/commands/releases/restore.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/releases/set_commits.rs` & `sentry_cli-2.31.1/src/commands/releases/set_commits.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/repos/list.rs` & `sentry_cli-2.31.1/src/commands/repos/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/repos/mod.rs` & `sentry_cli-2.31.1/src/commands/repos/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/send_envelope.rs` & `sentry_cli-2.31.1/src/commands/send_envelope.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/send_event.rs` & `sentry_cli-2.31.1/src/commands/send_event.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/sourcemaps/explain.rs` & `sentry_cli-2.31.1/src/commands/sourcemaps/explain.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/sourcemaps/inject.rs` & `sentry_cli-2.31.1/src/commands/sourcemaps/inject.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/sourcemaps/mod.rs` & `sentry_cli-2.31.1/src/commands/sourcemaps/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/sourcemaps/resolve.rs` & `sentry_cli-2.31.1/src/commands/sourcemaps/resolve.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/sourcemaps/upload.rs` & `sentry_cli-2.31.1/src/commands/sourcemaps/upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/uninstall.rs` & `sentry_cli-2.31.1/src/commands/uninstall.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/update.rs` & `sentry_cli-2.31.1/src/commands/update.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/commands/upload_proguard.rs` & `sentry_cli-2.31.1/src/commands/upload_proguard.rs`

 * *Files 0% similar despite different names*

```diff
@@ -138,16 +138,14 @@
                      the UUID of the proguard file before it was created.  If you upload \
                      a file with a forced UUID you can only upload a single proguard file.",
                 ),
         )
 }
 
 pub fn execute(matches: &ArgMatches) -> Result<()> {
-    let api = Api::current();
-    let authenticated_api = api.authenticated()?;
 
     let paths: Vec<_> = match matches.get_many::<String>("paths") {
         Some(paths) => paths.collect(),
         None => {
             return Ok(());
         }
     };
@@ -240,14 +238,17 @@
     let (org, project) = config.get_org_and_project(matches)?;
 
     info!(
         "Issuing a command for Organization: {} Project: {}",
         org, project
     );
 
+    let api = Api::current();
+    let authenticated_api = api.authenticated()?;
+
     let rv = authenticated_api
         .region_specific(&org)
         .upload_dif_archive(&project, tf.path())?;
     println!(
         "{} Uploaded a total of {} new mapping files",
         style(">").dim(),
         style(rv.len()).yellow()
```

### Comparing `sentry_cli-2.31.0/src/config.rs` & `sentry_cli-2.31.1/src/config.rs`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,17 @@
 use crate::constants::DEFAULT_MAX_DIF_ITEM_SIZE;
 use crate::constants::DEFAULT_MAX_DIF_UPLOAD_SIZE;
 use crate::constants::{CONFIG_RC_FILE_NAME, DEFAULT_RETRIES, DEFAULT_URL};
 use crate::utils::auth_token::AuthToken;
 use crate::utils::auth_token::AuthTokenPayload;
 use crate::utils::http::is_absolute_url;
 
+#[cfg(target_os = "macos")]
+use crate::utils::xcode;
+
 /// Represents the auth information
 #[derive(Debug, Clone)]
 pub enum Auth {
     Key(String),
     Token(AuthToken),
 }
 
@@ -571,25 +574,34 @@
                     "Failed to load {CONFIG_RC_FILE_NAME} file from the home folder."
                 )))
             }
         }
     }
 }
 
+fn failed_local_config_load_message(file_desc: &str) -> String {
+    let msg = format!("Failed to load {file_desc}.");
+    #[cfg(target_os = "macos")]
+    if xcode::launched_from_xcode() {
+        return msg + (" Hint: Please ensure that ${SRCROOT}/.sentryclirc is added to the Input Files of this Xcode Build Phases script.");
+    }
+    msg
+}
+
 fn load_cli_config() -> Result<(PathBuf, Ini)> {
     let (global_filename, mut rv) = load_global_config_file()?;
 
     let (path, mut rv) = if let Some(project_config_path) = find_project_config_file() {
         let file_desc = format!(
             "{} file from project path ({})",
             CONFIG_RC_FILE_NAME,
             project_config_path.display()
         );
-        let mut f =
-            fs::File::open(&project_config_path).context(format!("Failed to load {file_desc}"))?;
+        let mut f = fs::File::open(&project_config_path)
+            .context(failed_local_config_load_message(&file_desc))?;
         let ini = Ini::read_from(&mut f).context(format!("Failed to parse {file_desc}"))?;
         for (section, props) in ini.iter() {
             for (key, value) in props.iter() {
                 rv.set_to(section, key.to_string(), value.to_owned());
             }
         }
         (project_config_path, rv)
```

### Comparing `sentry_cli-2.31.0/src/constants.rs` & `sentry_cli-2.31.1/src/constants.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/utils/android.rs` & `sentry_cli-2.31.1/src/utils/android.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/utils/appcenter.rs` & `sentry_cli-2.31.1/src/utils/appcenter.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/utils/args.rs` & `sentry_cli-2.31.1/src/utils/args.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/utils/auth_token/auth_token_impl.rs` & `sentry_cli-2.31.1/src/utils/auth_token/auth_token_impl.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/utils/auth_token/error.rs` & `sentry_cli-2.31.1/src/utils/auth_token/error.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/utils/auth_token/org_auth_token.rs` & `sentry_cli-2.31.1/src/utils/auth_token/org_auth_token.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/utils/auth_token/test.rs` & `sentry_cli-2.31.1/src/utils/auth_token/test.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/utils/auth_token/user_auth_token.rs` & `sentry_cli-2.31.1/src/utils/auth_token/user_auth_token.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/utils/chunks.rs` & `sentry_cli-2.31.1/src/utils/chunks.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/utils/cordova.rs` & `sentry_cli-2.31.1/src/utils/cordova.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/utils/dif.rs` & `sentry_cli-2.31.1/src/utils/dif.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/utils/dif_upload.rs` & `sentry_cli-2.31.1/src/utils/dif_upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/utils/event.rs` & `sentry_cli-2.31.1/src/utils/event.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/utils/file_search.rs` & `sentry_cli-2.31.1/src/utils/file_search.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/utils/file_upload.rs` & `sentry_cli-2.31.1/src/utils/file_upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/utils/formatting.rs` & `sentry_cli-2.31.1/src/utils/formatting.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/utils/fs.rs` & `sentry_cli-2.31.1/src/utils/fs.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/utils/http.rs` & `sentry_cli-2.31.1/src/utils/http.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/utils/logging.rs` & `sentry_cli-2.31.1/src/utils/logging.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/utils/progress.rs` & `sentry_cli-2.31.1/src/utils/progress.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/utils/releases.rs` & `sentry_cli-2.31.1/src/utils/releases.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/utils/retry.rs` & `sentry_cli-2.31.1/src/utils/retry.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_default_twenty.snap` & `sentry_cli-2.31.1/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_default_twenty.snap`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_ignore_missing.snap` & `sentry_cli-2.31.1/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_ignore_missing.snap`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_base.snap` & `sentry_cli-2.31.1/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_base.snap`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/utils/snapshots/sentry_cli__utils__vcs__get_commits_from_git.snap` & `sentry_cli-2.31.1/src/utils/snapshots/sentry_cli__utils__vcs__get_commits_from_git.snap`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/utils/sourcemaps/inject.rs` & `sentry_cli-2.31.1/src/utils/sourcemaps/inject.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/utils/sourcemaps.rs` & `sentry_cli-2.31.1/src/utils/sourcemaps.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/utils/system.rs` & `sentry_cli-2.31.1/src/utils/system.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/utils/ui.rs` & `sentry_cli-2.31.1/src/utils/ui.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/utils/update.rs` & `sentry_cli-2.31.1/src/utils/update.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/utils/vcs.rs` & `sentry_cli-2.31.1/src/utils/vcs.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.31.0/src/utils/xcode.rs` & `sentry_cli-2.31.1/src/utils/xcode.rs`

 * *Files identical despite different names*

