# Comparing `tmp/libdebug-0.4.tar.gz` & `tmp/libdebug-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libdebug-0.4.tar", last modified: Tue Apr 30 06:11:20 2024, max compression
+gzip compressed data, was "libdebug-0.4.1.tar", last modified: Tue Apr 30 21:43:31 2024, max compression
```

## Comparing `libdebug-0.4.tar` & `libdebug-0.4.1.tar`

### file list

```diff
@@ -1,75 +1,77 @@
-drwxr-xr-x   0 jinblack  (1000) jinblack  (1000)        0 2024-04-30 06:11:20.253325 libdebug-0.4/
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)     1139 2024-04-28 13:28:04.000000 libdebug-0.4/LICENSE
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)      249 2024-04-30 06:11:20.253325 libdebug-0.4/PKG-INFO
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)    10817 2024-04-28 13:28:04.000000 libdebug-0.4/README.md
-drwxr-xr-x   0 jinblack  (1000) jinblack  (1000)        0 2024-04-30 06:11:20.243325 libdebug-0.4/libdebug/
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)       72 2024-04-28 13:28:04.000000 libdebug-0.4/libdebug/__init__.py
-drwxr-xr-x   0 jinblack  (1000) jinblack  (1000)        0 2024-04-30 06:11:20.246658 libdebug-0.4/libdebug/architectures/
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)        0 2024-04-28 13:28:04.000000 libdebug-0.4/libdebug/architectures/__init__.py
-drwxr-xr-x   0 jinblack  (1000) jinblack  (1000)        0 2024-04-30 06:11:20.246658 libdebug-0.4/libdebug/architectures/amd64/
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)        0 2024-04-28 13:28:04.000000 libdebug-0.4/libdebug/architectures/amd64/__init__.py
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)     5227 2024-04-28 13:28:04.000000 libdebug-0.4/libdebug/architectures/amd64/amd64_ptrace_hw_bp_helper.py
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)     5107 2024-04-28 13:28:04.000000 libdebug-0.4/libdebug/architectures/amd64/amd64_ptrace_register_holder.py
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)     1573 2024-04-28 13:28:04.000000 libdebug-0.4/libdebug/architectures/amd64/amd64_stack_unwinder.py
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)     1668 2024-04-28 13:28:04.000000 libdebug-0.4/libdebug/architectures/ptrace_hardware_breakpoint_manager.py
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)     1196 2024-04-28 13:28:04.000000 libdebug-0.4/libdebug/architectures/ptrace_hardware_breakpoint_provider.py
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)      612 2024-04-28 13:28:04.000000 libdebug-0.4/libdebug/architectures/ptrace_software_breakpoint_patcher.py
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)     1014 2024-04-28 13:28:04.000000 libdebug-0.4/libdebug/architectures/register_helper.py
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)      629 2024-04-28 13:28:04.000000 libdebug-0.4/libdebug/architectures/stack_unwinding_manager.py
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)      930 2024-04-28 13:28:04.000000 libdebug-0.4/libdebug/architectures/stack_unwinding_provider.py
-drwxr-xr-x   0 jinblack  (1000) jinblack  (1000)        0 2024-04-30 06:11:20.246658 libdebug-0.4/libdebug/builtin/
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)      147 2024-04-28 13:28:04.000000 libdebug-0.4/libdebug/builtin/__init__.py
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)     1754 2024-04-28 13:28:04.000000 libdebug-0.4/libdebug/builtin/antidebug_syscall_hook.py
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)     1959 2024-04-28 13:28:04.000000 libdebug-0.4/libdebug/builtin/pretty_print_syscall_hook.py
-drwxr-xr-x   0 jinblack  (1000) jinblack  (1000)        0 2024-04-30 06:11:20.246658 libdebug-0.4/libdebug/cffi/
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)        0 2024-04-28 13:28:04.000000 libdebug-0.4/libdebug/cffi/__init__.py
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)     1253 2024-04-28 13:28:04.000000 libdebug-0.4/libdebug/cffi/debug_sym_cffi_build.py
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)     1229 2024-04-28 13:28:04.000000 libdebug-0.4/libdebug/cffi/debug_sym_cffi_build_legacy.py
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)      739 2024-04-28 13:28:04.000000 libdebug-0.4/libdebug/cffi/personality_cffi_build.py
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)     4006 2024-04-28 19:25:36.000000 libdebug-0.4/libdebug/cffi/ptrace_cffi_build.py
-drwxr-xr-x   0 jinblack  (1000) jinblack  (1000)        0 2024-04-30 06:11:20.249991 libdebug-0.4/libdebug/data/
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)        0 2024-04-28 13:28:04.000000 libdebug-0.4/libdebug/data/__init__.py
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)     2621 2024-04-28 13:28:04.000000 libdebug-0.4/libdebug/data/breakpoint.py
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)     2178 2024-04-28 13:28:04.000000 libdebug-0.4/libdebug/data/memory_map.py
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)     5728 2024-04-28 13:28:04.000000 libdebug-0.4/libdebug/data/memory_view.py
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)     1870 2024-04-28 13:28:04.000000 libdebug-0.4/libdebug/data/register_holder.py
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)     1857 2024-04-28 13:28:04.000000 libdebug-0.4/libdebug/data/syscall_hook.py
-drwxr-xr-x   0 jinblack  (1000) jinblack  (1000)        0 2024-04-30 06:11:20.249991 libdebug-0.4/libdebug/interfaces/
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)        0 2024-04-28 13:28:04.000000 libdebug-0.4/libdebug/interfaces/__init__.py
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)     4639 2024-04-28 13:28:04.000000 libdebug-0.4/libdebug/interfaces/debugging_interface.py
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)      370 2024-04-28 13:28:04.000000 libdebug-0.4/libdebug/interfaces/gdb_interface.py
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)      873 2024-04-28 13:28:04.000000 libdebug-0.4/libdebug/interfaces/interface_helper.py
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)      325 2024-04-28 13:28:04.000000 libdebug-0.4/libdebug/interfaces/interfaces.py
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)    17683 2024-04-28 13:28:04.000000 libdebug-0.4/libdebug/interfaces/ptrace_interface.py
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)    27309 2024-04-28 13:28:04.000000 libdebug-0.4/libdebug/libdebug.py
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)     4190 2024-04-28 13:28:04.000000 libdebug-0.4/libdebug/liblog.py
-drwxr-xr-x   0 jinblack  (1000) jinblack  (1000)        0 2024-04-30 06:11:20.249991 libdebug-0.4/libdebug/ptrace/
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)        0 2024-04-28 13:28:04.000000 libdebug-0.4/libdebug/ptrace/__init__.py
-drwxr-xr-x   0 jinblack  (1000) jinblack  (1000)        0 2024-04-30 06:11:20.249991 libdebug-0.4/libdebug/ptrace/jumpstart/
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)        0 2024-04-28 13:28:04.000000 libdebug-0.4/libdebug/ptrace/jumpstart/__init__.py
--rwxr-xr-x   0 jinblack  (1000) jinblack  (1000)    15568 2024-04-30 06:07:55.000000 libdebug-0.4/libdebug/ptrace/jumpstart/jumpstart
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)     1937 2024-04-28 13:28:04.000000 libdebug-0.4/libdebug/ptrace/ptrace_constants.py
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)     8426 2024-04-28 13:28:04.000000 libdebug-0.4/libdebug/ptrace/ptrace_status_handler.py
-drwxr-xr-x   0 jinblack  (1000) jinblack  (1000)        0 2024-04-30 06:11:20.249991 libdebug-0.4/libdebug/state/
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)        0 2024-04-28 13:28:04.000000 libdebug-0.4/libdebug/state/__init__.py
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)    10532 2024-04-28 13:28:04.000000 libdebug-0.4/libdebug/state/debugging_context.py
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)     3619 2024-04-28 13:28:04.000000 libdebug-0.4/libdebug/state/thread_context.py
-drwxr-xr-x   0 jinblack  (1000) jinblack  (1000)        0 2024-04-30 06:11:20.253325 libdebug-0.4/libdebug/utils/
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)        0 2024-04-28 13:28:04.000000 libdebug-0.4/libdebug/utils/__init__.py
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)     3956 2024-04-28 13:28:04.000000 libdebug-0.4/libdebug/utils/debugging_utils.py
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)     8540 2024-04-28 13:28:04.000000 libdebug-0.4/libdebug/utils/elf_utils.py
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)      728 2024-04-28 13:28:04.000000 libdebug-0.4/libdebug/utils/gdb.py
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)     6267 2024-04-28 13:28:04.000000 libdebug-0.4/libdebug/utils/libcontext.py
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)    13882 2024-04-28 13:28:04.000000 libdebug-0.4/libdebug/utils/pipe_manager.py
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)      997 2024-04-28 13:28:04.000000 libdebug-0.4/libdebug/utils/posix_spawn.py
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)     1804 2024-04-28 13:28:04.000000 libdebug-0.4/libdebug/utils/process_utils.py
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)     1389 2024-04-28 13:28:04.000000 libdebug-0.4/libdebug/utils/register_utils.py
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)     2806 2024-04-28 13:28:04.000000 libdebug-0.4/libdebug/utils/syscall_utils.py
-drwxr-xr-x   0 jinblack  (1000) jinblack  (1000)        0 2024-04-30 06:11:20.253325 libdebug-0.4/libdebug.egg-info/
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)      249 2024-04-30 06:11:20.000000 libdebug-0.4/libdebug.egg-info/PKG-INFO
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)     2096 2024-04-30 06:11:20.000000 libdebug-0.4/libdebug.egg-info/SOURCES.txt
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)        1 2024-04-30 06:11:20.000000 libdebug-0.4/libdebug.egg-info/dependency_links.txt
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)       41 2024-04-30 06:11:20.000000 libdebug-0.4/libdebug.egg-info/requires.txt
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)        9 2024-04-30 06:11:20.000000 libdebug-0.4/libdebug.egg-info/top_level.txt
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)       38 2024-04-30 06:11:20.253325 libdebug-0.4/setup.cfg
--rw-r--r--   0 jinblack  (1000) jinblack  (1000)     2751 2024-04-28 19:23:54.000000 libdebug-0.4/setup.py
+drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2024-04-30 21:43:31.332347 libdebug-0.4.1/
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     1139 2024-04-18 06:52:12.000000 libdebug-0.4.1/LICENSE
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)       43 2024-04-30 21:27:42.000000 libdebug-0.4.1/MANIFEST.in
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)    13690 2024-04-30 21:43:31.328348 libdebug-0.4.1/PKG-INFO
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    10817 2024-04-30 21:25:54.000000 libdebug-0.4.1/README.md
+drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2024-04-30 21:43:31.328348 libdebug-0.4.1/libdebug/
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)       72 2024-04-30 21:25:45.000000 libdebug-0.4.1/libdebug/__init__.py
+drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2024-04-30 21:43:31.328348 libdebug-0.4.1/libdebug/architectures/
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)        0 2024-04-18 06:52:12.000000 libdebug-0.4.1/libdebug/architectures/__init__.py
+drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2024-04-30 21:43:31.328348 libdebug-0.4.1/libdebug/architectures/amd64/
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)        0 2024-04-18 06:52:12.000000 libdebug-0.4.1/libdebug/architectures/amd64/__init__.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     5227 2024-04-18 06:52:12.000000 libdebug-0.4.1/libdebug/architectures/amd64/amd64_ptrace_hw_bp_helper.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     5107 2024-04-30 21:25:54.000000 libdebug-0.4.1/libdebug/architectures/amd64/amd64_ptrace_register_holder.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     1573 2024-04-28 13:25:27.000000 libdebug-0.4.1/libdebug/architectures/amd64/amd64_stack_unwinder.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     1668 2024-04-18 06:52:12.000000 libdebug-0.4.1/libdebug/architectures/ptrace_hardware_breakpoint_manager.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     1196 2024-04-18 06:52:12.000000 libdebug-0.4.1/libdebug/architectures/ptrace_hardware_breakpoint_provider.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)      612 2024-04-18 06:52:12.000000 libdebug-0.4.1/libdebug/architectures/ptrace_software_breakpoint_patcher.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     1014 2024-04-18 06:52:12.000000 libdebug-0.4.1/libdebug/architectures/register_helper.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)      629 2024-04-28 13:25:27.000000 libdebug-0.4.1/libdebug/architectures/stack_unwinding_manager.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)      930 2024-04-18 06:52:12.000000 libdebug-0.4.1/libdebug/architectures/stack_unwinding_provider.py
+drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2024-04-30 21:43:31.328348 libdebug-0.4.1/libdebug/builtin/
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)      147 2024-04-30 21:25:54.000000 libdebug-0.4.1/libdebug/builtin/__init__.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     1754 2024-04-30 21:25:54.000000 libdebug-0.4.1/libdebug/builtin/antidebug_syscall_hook.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     1959 2024-04-30 21:25:54.000000 libdebug-0.4.1/libdebug/builtin/pretty_print_syscall_hook.py
+drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2024-04-30 21:43:31.328348 libdebug-0.4.1/libdebug/cffi/
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)        0 2024-04-18 06:52:12.000000 libdebug-0.4.1/libdebug/cffi/__init__.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     1253 2024-04-18 06:52:12.000000 libdebug-0.4.1/libdebug/cffi/debug_sym_cffi_build.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     1229 2024-04-18 06:52:12.000000 libdebug-0.4.1/libdebug/cffi/debug_sym_cffi_build_legacy.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)      739 2024-04-18 06:52:12.000000 libdebug-0.4.1/libdebug/cffi/personality_cffi_build.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     4006 2024-04-30 21:25:54.000000 libdebug-0.4.1/libdebug/cffi/ptrace_cffi_build.py
+drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2024-04-30 21:43:31.328348 libdebug-0.4.1/libdebug/data/
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)        0 2024-04-18 06:52:12.000000 libdebug-0.4.1/libdebug/data/__init__.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     2621 2024-04-18 06:52:12.000000 libdebug-0.4.1/libdebug/data/breakpoint.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     2178 2024-04-18 06:52:12.000000 libdebug-0.4.1/libdebug/data/memory_map.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     5728 2024-04-18 06:52:12.000000 libdebug-0.4.1/libdebug/data/memory_view.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     1870 2024-04-18 06:52:12.000000 libdebug-0.4.1/libdebug/data/register_holder.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     1857 2024-04-30 21:25:54.000000 libdebug-0.4.1/libdebug/data/syscall_hook.py
+drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2024-04-30 21:43:31.328348 libdebug-0.4.1/libdebug/interfaces/
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)        0 2024-04-18 06:52:12.000000 libdebug-0.4.1/libdebug/interfaces/__init__.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     4639 2024-04-30 21:25:54.000000 libdebug-0.4.1/libdebug/interfaces/debugging_interface.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)      370 2024-04-18 06:52:12.000000 libdebug-0.4.1/libdebug/interfaces/gdb_interface.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)      873 2024-04-18 06:52:12.000000 libdebug-0.4.1/libdebug/interfaces/interface_helper.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)      325 2024-04-18 06:52:12.000000 libdebug-0.4.1/libdebug/interfaces/interfaces.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    17683 2024-04-30 21:25:54.000000 libdebug-0.4.1/libdebug/interfaces/ptrace_interface.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    27309 2024-04-30 21:25:54.000000 libdebug-0.4.1/libdebug/libdebug.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     4190 2024-04-30 21:25:54.000000 libdebug-0.4.1/libdebug/liblog.py
+drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2024-04-30 21:43:31.328348 libdebug-0.4.1/libdebug/ptrace/
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)        0 2024-04-18 06:52:12.000000 libdebug-0.4.1/libdebug/ptrace/__init__.py
+drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2024-04-30 21:43:31.328348 libdebug-0.4.1/libdebug/ptrace/jumpstart/
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)        0 2024-04-18 06:52:12.000000 libdebug-0.4.1/libdebug/ptrace/jumpstart/__init__.py
+-rwxrwxr-x   0 gabriele  (1000) gabriele  (1000)    16080 2024-04-30 21:38:00.000000 libdebug-0.4.1/libdebug/ptrace/jumpstart/jumpstart
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     1937 2024-04-30 21:25:54.000000 libdebug-0.4.1/libdebug/ptrace/ptrace_constants.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     8426 2024-04-30 21:25:54.000000 libdebug-0.4.1/libdebug/ptrace/ptrace_status_handler.py
+drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2024-04-30 21:43:31.328348 libdebug-0.4.1/libdebug/state/
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)        0 2024-04-18 06:52:12.000000 libdebug-0.4.1/libdebug/state/__init__.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    10532 2024-04-30 21:25:54.000000 libdebug-0.4.1/libdebug/state/debugging_context.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     3619 2024-04-30 21:25:45.000000 libdebug-0.4.1/libdebug/state/thread_context.py
+drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2024-04-30 21:43:31.328348 libdebug-0.4.1/libdebug/utils/
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)        0 2024-04-18 06:52:12.000000 libdebug-0.4.1/libdebug/utils/__init__.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     3956 2024-04-18 06:52:12.000000 libdebug-0.4.1/libdebug/utils/debugging_utils.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     8540 2024-04-18 06:52:12.000000 libdebug-0.4.1/libdebug/utils/elf_utils.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)      728 2024-04-18 06:52:12.000000 libdebug-0.4.1/libdebug/utils/gdb.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     6267 2024-04-30 21:25:45.000000 libdebug-0.4.1/libdebug/utils/libcontext.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    13882 2024-04-30 21:25:45.000000 libdebug-0.4.1/libdebug/utils/pipe_manager.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)      997 2024-04-18 06:52:12.000000 libdebug-0.4.1/libdebug/utils/posix_spawn.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     1804 2024-04-18 06:52:12.000000 libdebug-0.4.1/libdebug/utils/process_utils.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     1389 2024-04-18 06:52:12.000000 libdebug-0.4.1/libdebug/utils/register_utils.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     2806 2024-04-30 21:25:54.000000 libdebug-0.4.1/libdebug/utils/syscall_utils.py
+drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2024-04-30 21:43:31.328348 libdebug-0.4.1/libdebug.egg-info/
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)    13690 2024-04-30 21:43:31.000000 libdebug-0.4.1/libdebug.egg-info/PKG-INFO
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     2123 2024-04-30 21:43:31.000000 libdebug-0.4.1/libdebug.egg-info/SOURCES.txt
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)        1 2024-04-30 21:43:31.000000 libdebug-0.4.1/libdebug.egg-info/dependency_links.txt
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)       53 2024-04-30 21:43:31.000000 libdebug-0.4.1/libdebug.egg-info/requires.txt
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)        9 2024-04-30 21:43:31.000000 libdebug-0.4.1/libdebug.egg-info/top_level.txt
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     1736 2024-04-30 21:33:27.000000 libdebug-0.4.1/pyproject.toml
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)       38 2024-04-30 21:43:31.332347 libdebug-0.4.1/setup.cfg
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     2730 2024-04-30 21:43:01.000000 libdebug-0.4.1/setup.py
```

### Comparing `libdebug-0.4/LICENSE` & `libdebug-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `libdebug-0.4/README.md` & `libdebug-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `libdebug-0.4/libdebug/architectures/amd64/amd64_ptrace_hw_bp_helper.py` & `libdebug-0.4.1/libdebug/architectures/amd64/amd64_ptrace_hw_bp_helper.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4/libdebug/architectures/amd64/amd64_ptrace_register_holder.py` & `libdebug-0.4.1/libdebug/architectures/amd64/amd64_ptrace_register_holder.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4/libdebug/architectures/amd64/amd64_stack_unwinder.py` & `libdebug-0.4.1/libdebug/architectures/amd64/amd64_stack_unwinder.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4/libdebug/architectures/ptrace_hardware_breakpoint_manager.py` & `libdebug-0.4.1/libdebug/architectures/ptrace_hardware_breakpoint_manager.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4/libdebug/architectures/ptrace_hardware_breakpoint_provider.py` & `libdebug-0.4.1/libdebug/architectures/ptrace_hardware_breakpoint_provider.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4/libdebug/architectures/ptrace_software_breakpoint_patcher.py` & `libdebug-0.4.1/libdebug/architectures/ptrace_software_breakpoint_patcher.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4/libdebug/architectures/register_helper.py` & `libdebug-0.4.1/libdebug/architectures/register_helper.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4/libdebug/architectures/stack_unwinding_manager.py` & `libdebug-0.4.1/libdebug/architectures/stack_unwinding_manager.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4/libdebug/architectures/stack_unwinding_provider.py` & `libdebug-0.4.1/libdebug/architectures/stack_unwinding_provider.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4/libdebug/builtin/antidebug_syscall_hook.py` & `libdebug-0.4.1/libdebug/builtin/antidebug_syscall_hook.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4/libdebug/builtin/pretty_print_syscall_hook.py` & `libdebug-0.4.1/libdebug/builtin/pretty_print_syscall_hook.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4/libdebug/cffi/debug_sym_cffi_build.py` & `libdebug-0.4.1/libdebug/cffi/debug_sym_cffi_build.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4/libdebug/cffi/debug_sym_cffi_build_legacy.py` & `libdebug-0.4.1/libdebug/cffi/debug_sym_cffi_build_legacy.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4/libdebug/cffi/personality_cffi_build.py` & `libdebug-0.4.1/libdebug/cffi/personality_cffi_build.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4/libdebug/cffi/ptrace_cffi_build.py` & `libdebug-0.4.1/libdebug/cffi/ptrace_cffi_build.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4/libdebug/data/breakpoint.py` & `libdebug-0.4.1/libdebug/data/breakpoint.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4/libdebug/data/memory_map.py` & `libdebug-0.4.1/libdebug/data/memory_map.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4/libdebug/data/memory_view.py` & `libdebug-0.4.1/libdebug/data/memory_view.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4/libdebug/data/register_holder.py` & `libdebug-0.4.1/libdebug/data/register_holder.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4/libdebug/data/syscall_hook.py` & `libdebug-0.4.1/libdebug/data/syscall_hook.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4/libdebug/interfaces/debugging_interface.py` & `libdebug-0.4.1/libdebug/interfaces/debugging_interface.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4/libdebug/interfaces/interface_helper.py` & `libdebug-0.4.1/libdebug/interfaces/interface_helper.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4/libdebug/interfaces/ptrace_interface.py` & `libdebug-0.4.1/libdebug/interfaces/ptrace_interface.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4/libdebug/libdebug.py` & `libdebug-0.4.1/libdebug/libdebug.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4/libdebug/liblog.py` & `libdebug-0.4.1/libdebug/liblog.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4/libdebug/ptrace/jumpstart/jumpstart` & `libdebug-0.4.1/libdebug/ptrace/jumpstart/jumpstart`

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

 * *Files 13% similar despite different names*

#### readelf --wide --file-header {}

```diff
@@ -4,17 +4,17 @@
   Data:                              2's complement, little endian
   Version:                           1 (current)
   OS/ABI:                            UNIX - System V
   ABI Version:                       0
   Type:                              DYN (Position-Independent Executable file)
   Machine:                           Advanced Micro Devices X86-64
   Version:                           0x1
-  Entry point address:               0x1050
+  Entry point address:               0x1080
   Start of program headers:          64 (bytes into file)
-  Start of section headers:          13648 (bytes into file)
+  Start of section headers:          14096 (bytes into file)
   Flags:                             0x0
   Size of this header:               64 (bytes)
   Size of program headers:           56 (bytes)
   Number of program headers:         13
   Size of section headers:           64 (bytes)
-  Number of section headers:         30
-  Section header string table index: 29
+  Number of section headers:         31
+  Section header string table index: 30
```

#### readelf --wide --program-header {}

```diff
@@ -1,37 +1,37 @@
 
 Elf file type is DYN (Position-Independent Executable file)
-Entry point 0x1050
+Entry point 0x1080
 There are 13 program headers, starting at offset 64
 
 Program Headers:
   Type           Offset   VirtAddr           PhysAddr           FileSiz  MemSiz   Flg Align
   PHDR           0x000040 0x0000000000000040 0x0000000000000040 0x0002d8 0x0002d8 R   0x8
   INTERP         0x000318 0x0000000000000318 0x0000000000000318 0x00001c 0x00001c R   0x1
       [Requesting program interpreter: /lib64/ld-linux-x86-64.so.2]
-  LOAD           0x000000 0x0000000000000000 0x0000000000000000 0x0006c8 0x0006c8 R   0x1000
-  LOAD           0x001000 0x0000000000001000 0x0000000000001000 0x0001b1 0x0001b1 R E 0x1000
-  LOAD           0x002000 0x0000000000002000 0x0000000000002000 0x0000a4 0x0000a4 R   0x1000
-  LOAD           0x002dd0 0x0000000000003dd0 0x0000000000003dd0 0x000250 0x000260 RW  0x1000
-  DYNAMIC        0x002de0 0x0000000000003de0 0x0000000000003de0 0x0001e0 0x0001e0 RW  0x8
-  NOTE           0x000338 0x0000000000000338 0x0000000000000338 0x000040 0x000040 R   0x8
-  NOTE           0x000378 0x0000000000000378 0x0000000000000378 0x000044 0x000044 R   0x4
-  GNU_PROPERTY   0x000338 0x0000000000000338 0x0000000000000338 0x000040 0x000040 R   0x8
-  GNU_EH_FRAME   0x002004 0x0000000000002004 0x0000000000002004 0x000024 0x000024 R   0x4
+  LOAD           0x000000 0x0000000000000000 0x0000000000000000 0x0006e0 0x0006e0 R   0x1000
+  LOAD           0x001000 0x0000000000001000 0x0000000000001000 0x0001d5 0x0001d5 R E 0x1000
+  LOAD           0x002000 0x0000000000002000 0x0000000000002000 0x0000e4 0x0000e4 R   0x1000
+  LOAD           0x002db0 0x0000000000003db0 0x0000000000003db0 0x000260 0x000280 RW  0x1000
+  DYNAMIC        0x002dc0 0x0000000000003dc0 0x0000000000003dc0 0x0001f0 0x0001f0 RW  0x8
+  NOTE           0x000338 0x0000000000000338 0x0000000000000338 0x000030 0x000030 R   0x8
+  NOTE           0x000368 0x0000000000000368 0x0000000000000368 0x000044 0x000044 R   0x4
+  GNU_PROPERTY   0x000338 0x0000000000000338 0x0000000000000338 0x000030 0x000030 R   0x8
+  GNU_EH_FRAME   0x002004 0x0000000000002004 0x0000000000002004 0x000034 0x000034 R   0x4
   GNU_STACK      0x000000 0x0000000000000000 0x0000000000000000 0x000000 0x000000 RW  0x10
-  GNU_RELRO      0x002dd0 0x0000000000003dd0 0x0000000000003dd0 0x000230 0x000230 R   0x1
+  GNU_RELRO      0x002db0 0x0000000000003db0 0x0000000000003db0 0x000250 0x000250 R   0x1
 
  Section to Segment mapping:
   Segment Sections...
    00     
    01     .interp 
    02     .interp .note.gnu.property .note.gnu.build-id .note.ABI-tag .gnu.hash .dynsym .dynstr .gnu.version .gnu.version_r .rela.dyn .rela.plt 
-   03     .init .plt .text .fini 
+   03     .init .plt .plt.got .plt.sec .text .fini 
    04     .rodata .eh_frame_hdr .eh_frame 
-   05     .init_array .fini_array .dynamic .got .got.plt .data .bss 
+   05     .init_array .fini_array .dynamic .got .data .bss 
    06     .dynamic 
    07     .note.gnu.property 
    08     .note.gnu.build-id .note.ABI-tag 
    09     .note.gnu.property 
    10     .eh_frame_hdr 
    11     
    12     .init_array .fini_array .dynamic .got
```

#### readelf --wide --sections {}

```diff
@@ -1,39 +1,40 @@
-There are 30 section headers, starting at offset 0x3550:
+There are 31 section headers, starting at offset 0x3710:
 
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .interp           PROGBITS        0000000000000318 000318 00001c 00   A  0   0  1
-  [ 2] .note.gnu.property NOTE            0000000000000338 000338 000040 00   A  0   0  8
-  [ 3] .note.gnu.build-id NOTE            0000000000000378 000378 000024 00   A  0   0  4
-  [ 4] .note.ABI-tag     NOTE            000000000000039c 00039c 000020 00   A  0   0  4
-  [ 5] .gnu.hash         GNU_HASH        00000000000003c0 0003c0 000028 00   A  6   0  8
-  [ 6] .dynsym           DYNSYM          00000000000003e8 0003e8 0000f0 18   A  7   1  8
-  [ 7] .dynstr           STRTAB          00000000000004d8 0004d8 0000a0 00   A  0   0  1
-  [ 8] .gnu.version      VERSYM          0000000000000578 000578 000014 02   A  6   0  2
-  [ 9] .gnu.version_r    VERNEED         0000000000000590 000590 000030 00   A  7   1  8
-  [10] .rela.dyn         RELA            00000000000005c0 0005c0 0000d8 18   A  6   0  8
-  [11] .rela.plt         RELA            0000000000000698 000698 000030 18  AI  6  23  8
+  [ 2] .note.gnu.property NOTE            0000000000000338 000338 000030 00   A  0   0  8
+  [ 3] .note.gnu.build-id NOTE            0000000000000368 000368 000024 00   A  0   0  4
+  [ 4] .note.ABI-tag     NOTE            000000000000038c 00038c 000020 00   A  0   0  4
+  [ 5] .gnu.hash         GNU_HASH        00000000000003b0 0003b0 000034 00   A  6   0  8
+  [ 6] .dynsym           DYNSYM          00000000000003e8 0003e8 000108 18   A  7   1  8
+  [ 7] .dynstr           STRTAB          00000000000004f0 0004f0 0000a0 00   A  0   0  1
+  [ 8] .gnu.version      VERSYM          0000000000000590 000590 000016 02   A  6   0  2
+  [ 9] .gnu.version_r    VERNEED         00000000000005a8 0005a8 000030 00   A  7   1  8
+  [10] .rela.dyn         RELA            00000000000005d8 0005d8 0000d8 18   A  6   0  8
+  [11] .rela.plt         RELA            00000000000006b0 0006b0 000030 18  AI  6  24  8
   [12] .init             PROGBITS        0000000000001000 001000 00001b 00  AX  0   0  4
   [13] .plt              PROGBITS        0000000000001020 001020 000030 10  AX  0   0 16
-  [14] .text             PROGBITS        0000000000001050 001050 000152 00  AX  0   0 16
-  [15] .fini             PROGBITS        00000000000011a4 0011a4 00000d 00  AX  0   0  4
-  [16] .rodata           PROGBITS        0000000000002000 002000 000004 04  AM  0   0  4
-  [17] .eh_frame_hdr     PROGBITS        0000000000002004 002004 000024 00   A  0   0  4
-  [18] .eh_frame         PROGBITS        0000000000002028 002028 00007c 00   A  0   0  8
-  [19] .init_array       INIT_ARRAY      0000000000003dd0 002dd0 000008 08  WA  0   0  8
-  [20] .fini_array       FINI_ARRAY      0000000000003dd8 002dd8 000008 08  WA  0   0  8
-  [21] .dynamic          DYNAMIC         0000000000003de0 002de0 0001e0 10  WA  7   0  8
-  [22] .got              PROGBITS        0000000000003fc0 002fc0 000028 08  WA  0   0  8
-  [23] .got.plt          PROGBITS        0000000000003fe8 002fe8 000028 08  WA  0   0  8
-  [24] .data             PROGBITS        0000000000004010 003010 000010 00  WA  0   0  8
-  [25] .bss              NOBITS          0000000000004020 003020 000010 00  WA  0   0  8
-  [26] .comment          PROGBITS        0000000000000000 003020 000036 01  MS  0   0  1
-  [27] .symtab           SYMTAB          0000000000000000 003058 000288 18     28   6  8
-  [28] .strtab           STRTAB          0000000000000000 0032e0 000156 00      0   0  1
-  [29] .shstrtab         STRTAB          0000000000000000 003436 000116 00      0   0  1
+  [14] .plt.got          PROGBITS        0000000000001050 001050 000010 10  AX  0   0 16
+  [15] .plt.sec          PROGBITS        0000000000001060 001060 000020 10  AX  0   0 16
+  [16] .text             PROGBITS        0000000000001080 001080 000146 00  AX  0   0 16
+  [17] .fini             PROGBITS        00000000000011c8 0011c8 00000d 00  AX  0   0  4
+  [18] .rodata           PROGBITS        0000000000002000 002000 000004 04  AM  0   0  4
+  [19] .eh_frame_hdr     PROGBITS        0000000000002004 002004 000034 00   A  0   0  4
+  [20] .eh_frame         PROGBITS        0000000000002038 002038 0000ac 00   A  0   0  8
+  [21] .init_array       INIT_ARRAY      0000000000003db0 002db0 000008 08  WA  0   0  8
+  [22] .fini_array       FINI_ARRAY      0000000000003db8 002db8 000008 08  WA  0   0  8
+  [23] .dynamic          DYNAMIC         0000000000003dc0 002dc0 0001f0 10  WA  7   0  8
+  [24] .got              PROGBITS        0000000000003fb0 002fb0 000050 08  WA  0   0  8
+  [25] .data             PROGBITS        0000000000004000 003000 000010 00  WA  0   0  8
+  [26] .bss              NOBITS          0000000000004020 003010 000010 00  WA  0   0 32
+  [27] .comment          PROGBITS        0000000000000000 003010 00002b 01  MS  0   0  1
+  [28] .symtab           SYMTAB          0000000000000000 003040 0003a8 18     29  18  8
+  [29] .strtab           STRTAB          0000000000000000 0033e8 00020a 00      0   0  1
+  [30] .shstrtab         STRTAB          0000000000000000 0035f2 00011a 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), l (large), p (processor specific)
```

#### readelf --wide --symbols {}

```diff
@@ -1,43 +1,56 @@
 
-Symbol table '.dynsym' contains 10 entries:
+Symbol table '.dynsym' contains 11 entries:
    Num:    Value          Size Type    Bind   Vis      Ndx Name
      0: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT  UND 
      1: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __libc_start_main@GLIBC_2.34 (2)
      2: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_deregisterTMCloneTable
      3: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND execve@GLIBC_2.2.5 (3)
      4: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND __gmon_start__
      5: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND ptrace@GLIBC_2.2.5 (3)
      6: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_registerTMCloneTable
-     7: 0000000000000000     0 FUNC    WEAK   DEFAULT  UND __cxa_finalize@GLIBC_2.2.5 (3)
-     8: 0000000000004020     8 OBJECT  WEAK   DEFAULT   25 environ@GLIBC_2.2.5 (3)
-     9: 0000000000004020     8 OBJECT  GLOBAL DEFAULT   25 __environ@GLIBC_2.2.5 (3)
+     7: 0000000000004020     8 OBJECT  WEAK   DEFAULT   26 _environ@GLIBC_2.2.5 (3)
+     8: 0000000000004020     8 OBJECT  WEAK   DEFAULT   26 environ@GLIBC_2.2.5 (3)
+     9: 0000000000000000     0 FUNC    WEAK   DEFAULT  UND __cxa_finalize@GLIBC_2.2.5 (3)
+    10: 0000000000004020     8 OBJECT  GLOBAL DEFAULT   26 __environ@GLIBC_2.2.5 (3)
 
-Symbol table '.symtab' contains 27 entries:
+Symbol table '.symtab' contains 39 entries:
    Num:    Value          Size Type    Bind   Vis      Ndx Name
      0: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT  UND 
-     1: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS jumpstart.c
-     2: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS 
-     3: 0000000000003de0     0 OBJECT  LOCAL  DEFAULT   21 _DYNAMIC
-     4: 0000000000002004     0 NOTYPE  LOCAL  DEFAULT   17 __GNU_EH_FRAME_HDR
-     5: 0000000000003fe8     0 OBJECT  LOCAL  DEFAULT   23 _GLOBAL_OFFSET_TABLE_
-     6: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __libc_start_main@GLIBC_2.34
-     7: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_deregisterTMCloneTable
-     8: 0000000000004010     0 NOTYPE  WEAK   DEFAULT   24 data_start
-     9: 0000000000004020     0 NOTYPE  GLOBAL DEFAULT   24 _edata
-    10: 00000000000011a4     0 FUNC    GLOBAL HIDDEN    15 _fini
-    11: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND execve@GLIBC_2.2.5
-    12: 0000000000004010     0 NOTYPE  GLOBAL DEFAULT   24 __data_start
-    13: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND __gmon_start__
-    14: 0000000000004020     8 OBJECT  WEAK   DEFAULT   25 environ@GLIBC_2.2.5
-    15: 0000000000004018     0 OBJECT  GLOBAL HIDDEN    24 __dso_handle
-    16: 0000000000002000     4 OBJECT  GLOBAL DEFAULT   16 _IO_stdin_used
-    17: 0000000000004030     0 NOTYPE  GLOBAL DEFAULT   25 _end
-    18: 0000000000001050    38 FUNC    GLOBAL DEFAULT   14 _start
-    19: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND ptrace@GLIBC_2.2.5
-    20: 0000000000004020     0 NOTYPE  GLOBAL DEFAULT   25 __bss_start
-    21: 0000000000001149    89 FUNC    GLOBAL DEFAULT   14 main
-    22: 0000000000004020     8 OBJECT  GLOBAL DEFAULT   25 __environ@GLIBC_2.2.5
-    23: 0000000000004020     0 OBJECT  GLOBAL HIDDEN    24 __TMC_END__
-    24: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_registerTMCloneTable
-    25: 0000000000000000     0 FUNC    WEAK   DEFAULT  UND __cxa_finalize@GLIBC_2.2.5
-    26: 0000000000001000     0 FUNC    GLOBAL HIDDEN    12 _init
+     1: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS Scrt1.o
+     2: 000000000000038c    32 OBJECT  LOCAL  DEFAULT    4 __abi_tag
+     3: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS crtstuff.c
+     4: 00000000000010b0     0 FUNC    LOCAL  DEFAULT   16 deregister_tm_clones
+     5: 00000000000010e0     0 FUNC    LOCAL  DEFAULT   16 register_tm_clones
+     6: 0000000000001120     0 FUNC    LOCAL  DEFAULT   16 __do_global_dtors_aux
+     7: 0000000000004028     1 OBJECT  LOCAL  DEFAULT   26 completed.0
+     8: 0000000000003db8     0 OBJECT  LOCAL  DEFAULT   22 __do_global_dtors_aux_fini_array_entry
+     9: 0000000000001160     0 FUNC    LOCAL  DEFAULT   16 frame_dummy
+    10: 0000000000003db0     0 OBJECT  LOCAL  DEFAULT   21 __frame_dummy_init_array_entry
+    11: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS jumpstart.c
+    12: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS crtstuff.c
+    13: 00000000000020e0     0 OBJECT  LOCAL  DEFAULT   20 __FRAME_END__
+    14: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS 
+    15: 0000000000003dc0     0 OBJECT  LOCAL  DEFAULT   23 _DYNAMIC
+    16: 0000000000002004     0 NOTYPE  LOCAL  DEFAULT   19 __GNU_EH_FRAME_HDR
+    17: 0000000000003fb0     0 OBJECT  LOCAL  DEFAULT   24 _GLOBAL_OFFSET_TABLE_
+    18: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __libc_start_main@GLIBC_2.34
+    19: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_deregisterTMCloneTable
+    20: 0000000000004000     0 NOTYPE  WEAK   DEFAULT   25 data_start
+    21: 0000000000004010     0 NOTYPE  GLOBAL DEFAULT   25 _edata
+    22: 00000000000011c8     0 FUNC    GLOBAL HIDDEN    17 _fini
+    23: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND execve@GLIBC_2.2.5
+    24: 0000000000004000     0 NOTYPE  GLOBAL DEFAULT   25 __data_start
+    25: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND __gmon_start__
+    26: 0000000000004020     8 OBJECT  WEAK   DEFAULT   26 environ@GLIBC_2.2.5
+    27: 0000000000004008     0 OBJECT  GLOBAL HIDDEN    25 __dso_handle
+    28: 0000000000002000     4 OBJECT  GLOBAL DEFAULT   18 _IO_stdin_used
+    29: 0000000000004030     0 NOTYPE  GLOBAL DEFAULT   26 _end
+    30: 0000000000001080    38 FUNC    GLOBAL DEFAULT   16 _start
+    31: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND ptrace@GLIBC_2.2.5
+    32: 0000000000004010     0 NOTYPE  GLOBAL DEFAULT   26 __bss_start
+    33: 0000000000001169    93 FUNC    GLOBAL DEFAULT   16 main
+    34: 0000000000004020     8 OBJECT  GLOBAL DEFAULT   26 __environ@GLIBC_2.2.5
+    35: 0000000000004010     0 OBJECT  GLOBAL HIDDEN    25 __TMC_END__
+    36: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_registerTMCloneTable
+    37: 0000000000000000     0 FUNC    WEAK   DEFAULT  UND __cxa_finalize@GLIBC_2.2.5
+    38: 0000000000001000     0 FUNC    GLOBAL HIDDEN    12 _init
```

#### readelf --wide --relocs {}

```diff
@@ -1,17 +1,17 @@
 
-Relocation section '.rela.dyn' at offset 0x5c0 contains 9 entries:
+Relocation section '.rela.dyn' at offset 0x5d8 contains 9 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
-0000000000003dd0  0000000000000008 R_X86_64_RELATIVE                         1140
-0000000000003dd8  0000000000000008 R_X86_64_RELATIVE                         10f0
-0000000000004018  0000000000000008 R_X86_64_RELATIVE                         4018
-0000000000003fc0  0000000100000006 R_X86_64_GLOB_DAT      0000000000000000 __libc_start_main@GLIBC_2.34 + 0
-0000000000003fc8  0000000200000006 R_X86_64_GLOB_DAT      0000000000000000 _ITM_deregisterTMCloneTable + 0
-0000000000003fd0  0000000400000006 R_X86_64_GLOB_DAT      0000000000000000 __gmon_start__ + 0
-0000000000003fd8  0000000600000006 R_X86_64_GLOB_DAT      0000000000000000 _ITM_registerTMCloneTable + 0
-0000000000003fe0  0000000700000006 R_X86_64_GLOB_DAT      0000000000000000 __cxa_finalize@GLIBC_2.2.5 + 0
-0000000000004020  0000000900000005 R_X86_64_COPY          0000000000004020 __environ@GLIBC_2.2.5 + 0
+0000000000003db0  0000000000000008 R_X86_64_RELATIVE                         1160
+0000000000003db8  0000000000000008 R_X86_64_RELATIVE                         1120
+0000000000004008  0000000000000008 R_X86_64_RELATIVE                         4008
+0000000000003fd8  0000000100000006 R_X86_64_GLOB_DAT      0000000000000000 __libc_start_main@GLIBC_2.34 + 0
+0000000000003fe0  0000000200000006 R_X86_64_GLOB_DAT      0000000000000000 _ITM_deregisterTMCloneTable + 0
+0000000000003fe8  0000000400000006 R_X86_64_GLOB_DAT      0000000000000000 __gmon_start__ + 0
+0000000000003ff0  0000000600000006 R_X86_64_GLOB_DAT      0000000000000000 _ITM_registerTMCloneTable + 0
+0000000000003ff8  0000000900000006 R_X86_64_GLOB_DAT      0000000000000000 __cxa_finalize@GLIBC_2.2.5 + 0
+0000000000004020  0000000a00000005 R_X86_64_COPY          0000000000004020 __environ@GLIBC_2.2.5 + 0
 
-Relocation section '.rela.plt' at offset 0x698 contains 2 entries:
+Relocation section '.rela.plt' at offset 0x6b0 contains 2 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
-0000000000004000  0000000300000007 R_X86_64_JUMP_SLOT     0000000000000000 execve@GLIBC_2.2.5 + 0
-0000000000004008  0000000500000007 R_X86_64_JUMP_SLOT     0000000000000000 ptrace@GLIBC_2.2.5 + 0
+0000000000003fc8  0000000300000007 R_X86_64_JUMP_SLOT     0000000000000000 execve@GLIBC_2.2.5 + 0
+0000000000003fd0  0000000500000007 R_X86_64_JUMP_SLOT     0000000000000000 ptrace@GLIBC_2.2.5 + 0
```

#### readelf --wide --dynamic {}

```diff
@@ -1,29 +1,30 @@
 
-Dynamic section at offset 0x2de0 contains 26 entries:
+Dynamic section at offset 0x2dc0 contains 27 entries:
   Tag        Type                         Name/Value
  0x0000000000000001 (NEEDED)             Shared library: [libc.so.6]
  0x000000000000000c (INIT)               0x1000
- 0x000000000000000d (FINI)               0x11a4
- 0x0000000000000019 (INIT_ARRAY)         0x3dd0
+ 0x000000000000000d (FINI)               0x11c8
+ 0x0000000000000019 (INIT_ARRAY)         0x3db0
  0x000000000000001b (INIT_ARRAYSZ)       8 (bytes)
- 0x000000000000001a (FINI_ARRAY)         0x3dd8
+ 0x000000000000001a (FINI_ARRAY)         0x3db8
  0x000000000000001c (FINI_ARRAYSZ)       8 (bytes)
- 0x000000006ffffef5 (GNU_HASH)           0x3c0
- 0x0000000000000005 (STRTAB)             0x4d8
+ 0x000000006ffffef5 (GNU_HASH)           0x3b0
+ 0x0000000000000005 (STRTAB)             0x4f0
  0x0000000000000006 (SYMTAB)             0x3e8
  0x000000000000000a (STRSZ)              160 (bytes)
  0x000000000000000b (SYMENT)             24 (bytes)
  0x0000000000000015 (DEBUG)              0x0
- 0x0000000000000003 (PLTGOT)             0x3fe8
+ 0x0000000000000003 (PLTGOT)             0x3fb0
  0x0000000000000002 (PLTRELSZ)           48 (bytes)
  0x0000000000000014 (PLTREL)             RELA
- 0x0000000000000017 (JMPREL)             0x698
- 0x0000000000000007 (RELA)               0x5c0
+ 0x0000000000000017 (JMPREL)             0x6b0
+ 0x0000000000000007 (RELA)               0x5d8
  0x0000000000000008 (RELASZ)             216 (bytes)
  0x0000000000000009 (RELAENT)            24 (bytes)
- 0x000000006ffffffb (FLAGS_1)            Flags: PIE
- 0x000000006ffffffe (VERNEED)            0x590
+ 0x000000000000001e (FLAGS)              BIND_NOW
+ 0x000000006ffffffb (FLAGS_1)            Flags: NOW PIE
+ 0x000000006ffffffe (VERNEED)            0x5a8
  0x000000006fffffff (VERNEEDNUM)         1
- 0x000000006ffffff0 (VERSYM)             0x578
+ 0x000000006ffffff0 (VERSYM)             0x590
  0x000000006ffffff9 (RELACOUNT)          3
  0x0000000000000000 (NULL)               0x0
```

#### readelf --wide --notes {}

```diff
@@ -1,12 +1,12 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
-  GNU                  0x00000030	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 ISA needed: x86-64-baseline, x86 feature used: x86, x86 ISA used: 
+  GNU                  0x00000020	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 feature: IBT, SHSTK, x86 ISA needed: x86-64-baseline
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 1f633584a027fcc818d28c6c6619505f12fdb99c
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: bd034c3ff02f521734facb55b23ec2442e57b4c6
 
 Displaying notes found in: .note.ABI-tag
   Owner                Data size 	Description
-  GNU                  0x00000010	NT_GNU_ABI_TAG (ABI version tag)	    OS: Linux, ABI: 4.4.0
+  GNU                  0x00000010	NT_GNU_ABI_TAG (ABI version tag)	    OS: Linux, ABI: 3.2.0
```

#### readelf --wide --version-info {}

```diff
@@ -1,12 +1,12 @@
 
-Version symbols section '.gnu.version' contains 10 entries:
- Addr: 0x0000000000000578  Offset: 0x00000578  Link: 6 (.dynsym)
+Version symbols section '.gnu.version' contains 11 entries:
+ Addr: 0x0000000000000590  Offset: 0x00000590  Link: 6 (.dynsym)
   000:   0 (*local*)       2 (GLIBC_2.34)    1 (*global*)      3 (GLIBC_2.2.5)
   004:   1 (*global*)      3 (GLIBC_2.2.5)   1 (*global*)      3 (GLIBC_2.2.5)
-  008:   3 (GLIBC_2.2.5)   3 (GLIBC_2.2.5)
+  008:   3 (GLIBC_2.2.5)   3 (GLIBC_2.2.5)   3 (GLIBC_2.2.5)
 
 Version needs section '.gnu.version_r' contains 1 entry:
- Addr: 0x0000000000000590  Offset: 0x00000590  Link: 7 (.dynstr)
+ Addr: 0x00000000000005a8  Offset: 0x000005a8  Link: 7 (.dynstr)
   000000: Version: 1  File: libc.so.6  Cnt: 2
   0x0010:   Name: GLIBC_2.2.5  Flags: none  Version: 3
   0x0020:   Name: GLIBC_2.34  Flags: none  Version: 2
```

#### readelf --wide --debug-dump=frames {}

```diff
@@ -9,40 +9,58 @@
   Return address column: 16
   Augmentation data:     1b
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_offset: r16 (rip) at cfa-8
   DW_CFA_nop
   DW_CFA_nop
 
-00000018 0000000000000014 0000001c FDE cie=00000000 pc=0000000000001050..0000000000001076
-  DW_CFA_advance_loc: 4 to 0000000000001054
+00000018 0000000000000014 0000001c FDE cie=00000000 pc=0000000000001080..00000000000010a6
+  DW_CFA_advance_loc: 4 to 0000000000001084
   DW_CFA_undefined: r16 (rip)
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
 00000030 0000000000000024 00000034 FDE cie=00000000 pc=0000000000001020..0000000000001050
   DW_CFA_def_cfa_offset: 16
   DW_CFA_advance_loc: 6 to 0000000000001026
   DW_CFA_def_cfa_offset: 24
   DW_CFA_advance_loc: 10 to 0000000000001030
-  DW_CFA_def_cfa_expression (DW_OP_breg7 (rsp): 8; DW_OP_breg16 (rip): 0; DW_OP_lit15; DW_OP_and; DW_OP_lit11; DW_OP_ge; DW_OP_lit3; DW_OP_shl; DW_OP_plus)
+  DW_CFA_def_cfa_expression (DW_OP_breg7 (rsp): 8; DW_OP_breg16 (rip): 0; DW_OP_lit15; DW_OP_and; DW_OP_lit10; DW_OP_ge; DW_OP_lit3; DW_OP_shl; DW_OP_plus)
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000058 000000000000001c 0000005c FDE cie=00000000 pc=0000000000001149..00000000000011a2
-  DW_CFA_advance_loc: 1 to 000000000000114a
+00000058 0000000000000014 0000005c FDE cie=00000000 pc=0000000000001050..0000000000001060
+  DW_CFA_nop
+  DW_CFA_nop
+  DW_CFA_nop
+  DW_CFA_nop
+  DW_CFA_nop
+  DW_CFA_nop
+  DW_CFA_nop
+
+00000070 0000000000000014 00000074 FDE cie=00000000 pc=0000000000001060..0000000000001080
+  DW_CFA_nop
+  DW_CFA_nop
+  DW_CFA_nop
+  DW_CFA_nop
+  DW_CFA_nop
+  DW_CFA_nop
+  DW_CFA_nop
+
+00000088 000000000000001c 0000008c FDE cie=00000000 pc=0000000000001169..00000000000011c6
+  DW_CFA_advance_loc: 5 to 000000000000116e
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 000000000000114d
+  DW_CFA_advance_loc: 3 to 0000000000001171
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc1: 84 to 00000000000011a1
+  DW_CFA_advance_loc1: 84 to 00000000000011c5
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
 
-00000078 ZERO terminator
+000000a8 ZERO terminator
```

#### strings --all --bytes=8 {}

```diff
@@ -1,20 +1,28 @@
 /lib64/ld-linux-x86-64.so.2
-__libc_start_main
 __cxa_finalize
+__libc_start_main
 __environ
 libc.so.6
 GLIBC_2.2.5
 GLIBC_2.34
 _ITM_deregisterTMCloneTable
 __gmon_start__
 _ITM_registerTMCloneTable
-GCC: (GNU) 13.2.1 20230801
-GCC: (GNU) 13.2.1 20240417
+GCC: (Ubuntu 11.4.0-1ubuntu1~22.04) 11.4.0
+__abi_tag
+crtstuff.c
+deregister_tm_clones
+__do_global_dtors_aux
+completed.0
+__do_global_dtors_aux_fini_array_entry
+frame_dummy
+__frame_dummy_init_array_entry
 jumpstart.c
+__FRAME_END__
 _DYNAMIC
 __GNU_EH_FRAME_HDR
 _GLOBAL_OFFSET_TABLE_
 __libc_start_main@GLIBC_2.34
 _ITM_deregisterTMCloneTable
 execve@GLIBC_2.2.5
 __data_start
@@ -32,14 +40,15 @@
 .note.gnu.build-id
 .note.ABI-tag
 .gnu.hash
 .gnu.version
 .gnu.version_r
 .rela.dyn
 .rela.plt
+.plt.got
+.plt.sec
 .eh_frame_hdr
 .eh_frame
 .init_array
 .fini_array
 .dynamic
-.got.plt
 .comment
```

#### readelf --wide --decompress --hex-dump=.gnu.hash {}

```diff
@@ -1,6 +1,7 @@
 
 Hex dump of section '.gnu.hash':
-  0x000003c0 02000000 08000000 01000000 06000000 ................
-  0x000003d0 10000000 c0004000 08000000 00000000 ......@.........
-  0x000003e0 a6dda36b c5b99c40                   ...k...@
+  0x000003b0 03000000 07000000 01000000 06000000 ................
+  0x000003c0 30008100 c0004000 07000000 0a000000 0.....@.........
+  0x000003d0 00000000 c4890590 a6dda36b d165ce6d ...........k.e.m
+  0x000003e0 c5b99c40                            ...@
```

#### readelf --wide --decompress --hex-dump=.dynstr {}

```diff
@@ -1,13 +1,13 @@
 
 Hex dump of section '.dynstr':
-  0x000004d8 00707472 61636500 65786563 7665005f .ptrace.execve._
-  0x000004e8 5f6c6962 635f7374 6172745f 6d61696e _libc_start_main
-  0x000004f8 005f5f63 78615f66 696e616c 697a6500 .__cxa_finalize.
-  0x00000508 5f5f656e 7669726f 6e006c69 62632e73 __environ.libc.s
-  0x00000518 6f2e3600 474c4942 435f322e 322e3500 o.6.GLIBC_2.2.5.
-  0x00000528 474c4942 435f322e 3334005f 49544d5f GLIBC_2.34._ITM_
-  0x00000538 64657265 67697374 6572544d 436c6f6e deregisterTMClon
-  0x00000548 65546162 6c65005f 5f676d6f 6e5f7374 eTable.__gmon_st
-  0x00000558 6172745f 5f005f49 544d5f72 65676973 art__._ITM_regis
-  0x00000568 74657254 4d436c6f 6e655461 626c6500 terTMCloneTable.
+  0x000004f0 005f5f63 78615f66 696e616c 697a6500 .__cxa_finalize.
+  0x00000500 5f5f6c69 62635f73 74617274 5f6d6169 __libc_start_mai
+  0x00000510 6e007074 72616365 00657865 63766500 n.ptrace.execve.
+  0x00000520 5f5f656e 7669726f 6e006c69 62632e73 __environ.libc.s
+  0x00000530 6f2e3600 474c4942 435f322e 322e3500 o.6.GLIBC_2.2.5.
+  0x00000540 474c4942 435f322e 3334005f 49544d5f GLIBC_2.34._ITM_
+  0x00000550 64657265 67697374 6572544d 436c6f6e deregisterTMClon
+  0x00000560 65546162 6c65005f 5f676d6f 6e5f7374 eTable.__gmon_st
+  0x00000570 6172745f 5f005f49 544d5f72 65676973 art__._ITM_regis
+  0x00000580 74657254 4d436c6f 6e655461 626c6500 terTMCloneTable.
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.init {}

```diff
@@ -3,13 +3,13 @@
 
 Disassembly of section .init:
 
 0000000000001000 <_init>:
 _init():
 	endbr64
 	sub    $0x8,%rsp
-	mov    0x2fc1(%rip),%rax        
+	mov    0x2fd9(%rip),%rax        
 	test   %rax,%rax
 	je     1016 <_init+0x16>
 	call   *%rax
 	add    $0x8,%rsp
 	ret
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.plt {}

```diff
@@ -1,19 +1,17 @@
 
 
 
 Disassembly of section .plt:
 
-0000000000001020 <execve@plt-0x10>:
-	push   0x2fca(%rip)        
-	jmp    *0x2fcc(%rip)        
-	nopl   0x0(%rax)
-
-0000000000001030 <execve@plt>:
-	jmp    *0x2fca(%rip)        
+0000000000001020 <.plt>:
+	push   0x2f92(%rip)        
+	bnd jmp *0x2f93(%rip)        
+	nopl   (%rax)
+	endbr64
 	push   $0x0
-	jmp    1020 <_init+0x20>
-
-0000000000001040 <ptrace@plt>:
-	jmp    *0x2fc2(%rip)        
+	bnd jmp 1020 <_init+0x20>
+	nop
+	endbr64
 	push   $0x1
-	jmp    1020 <_init+0x20>
+	bnd jmp 1020 <_init+0x20>
+	nop
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -1,93 +1,105 @@
 
 
 
 Disassembly of section .text:
 
-0000000000001050 <_start>:
+0000000000001080 <_start>:
 _start():
 	endbr64
 	xor    %ebp,%ebp
 	mov    %rdx,%r9
 	pop    %rsi
 	mov    %rsp,%rdx
 	and    $0xfffffffffffffff0,%rsp
 	push   %rax
 	push   %rsp
 	xor    %r8d,%r8d
 	xor    %ecx,%ecx
-	lea    0xda(%rip),%rdi        
-	call   *0x2f4b(%rip)        
+	lea    0xca(%rip),%rdi        
+	call   *0x2f33(%rip)        
 	hlt
 	cs nopw 0x0(%rax,%rax,1)
-	lea    0x2f99(%rip),%rdi        
-	lea    0x2f92(%rip),%rax        
+
+00000000000010b0 <deregister_tm_clones>:
+deregister_tm_clones():
+	lea    0x2f59(%rip),%rdi        
+	lea    0x2f52(%rip),%rax        
 	cmp    %rdi,%rax
-	je     10a8 <_start+0x58>
-	mov    0x2f2e(%rip),%rax        
+	je     10d8 <deregister_tm_clones+0x28>
+	mov    0x2f16(%rip),%rax        
 	test   %rax,%rax
-	je     10a8 <_start+0x58>
+	je     10d8 <deregister_tm_clones+0x28>
 	jmp    *%rax
 	nopl   0x0(%rax)
 	ret
 	nopl   0x0(%rax)
-	lea    0x2f69(%rip),%rdi        
-	lea    0x2f62(%rip),%rsi        
+
+00000000000010e0 <register_tm_clones>:
+register_tm_clones():
+	lea    0x2f29(%rip),%rdi        
+	lea    0x2f22(%rip),%rsi        
 	sub    %rdi,%rsi
 	mov    %rsi,%rax
 	shr    $0x3f,%rsi
 	sar    $0x3,%rax
 	add    %rax,%rsi
 	sar    $1,%rsi
-	je     10e8 <_start+0x98>
-	mov    0x2efd(%rip),%rax        
+	je     1118 <register_tm_clones+0x38>
+	mov    0x2ee5(%rip),%rax        
 	test   %rax,%rax
-	je     10e8 <_start+0x98>
+	je     1118 <register_tm_clones+0x38>
 	jmp    *%rax
 	nopw   0x0(%rax,%rax,1)
 	ret
 	nopl   0x0(%rax)
+
+0000000000001120 <__do_global_dtors_aux>:
+__do_global_dtors_aux():
 	endbr64
-	cmpb   $0x0,0x2f2d(%rip)        
-	jne    1130 <_start+0xe0>
+	cmpb   $0x0,0x2efd(%rip)        
+	jne    1158 <__do_global_dtors_aux+0x38>
 	push   %rbp
-	cmpq   $0x0,0x2eda(%rip)        
+	cmpq   $0x0,0x2ec2(%rip)        
 	mov    %rsp,%rbp
-	je     1118 <_start+0xc8>
-	mov    0x2f06(%rip),%rdi        
-	call   *0x2ec8(%rip)        
-	call   1080 <_start+0x30>
-	movb   $0x1,0x2f04(%rip)        
+	je     1147 <__do_global_dtors_aux+0x27>
+	mov    0x2ec6(%rip),%rdi        
+	call   1050 <__cxa_finalize@plt>
+	call   10b0 <deregister_tm_clones>
+	movb   $0x1,0x2ed5(%rip)        
 	pop    %rbp
 	ret
-	cs nopw 0x0(%rax,%rax,1)
+	nopl   (%rax)
 	ret
-	data16 cs nopw 0x0(%rax,%rax,1)
 	nopl   0x0(%rax)
+
+0000000000001160 <frame_dummy>:
+frame_dummy():
 	endbr64
-	jmp    10b0 <_start+0x60>
+	jmp    10e0 <register_tm_clones>
 
-0000000000001149 <main>:
+0000000000001169 <main>:
 main():
+	endbr64
 	push   %rbp
 	mov    %rsp,%rbp
 	sub    $0x10,%rsp
 	mov    %edi,-0x4(%rbp)
 	mov    %rsi,-0x10(%rbp)
 	mov    $0x0,%ecx
 	mov    $0x0,%edx
 	mov    $0x0,%esi
 	mov    $0x0,%edi
 	mov    $0x0,%eax
-	call   1040 <ptrace@plt>
-	mov    0x2ea3(%rip),%rdx        
+	call   1070 <ptrace@plt>
+	mov    0x2e7f(%rip),%rdx        
 	mov    -0x10(%rbp),%rax
 	lea    0x8(%rax),%rcx
 	mov    -0x10(%rbp),%rax
 	add    $0x8,%rax
 	mov    (%rax),%rax
 	mov    %rcx,%rsi
 	mov    %rax,%rdi
-	call   1030 <execve@plt>
+	call   1060 <execve@plt>
 	mov    $0x0,%eax
 	leave
 	ret
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.fini {}

```diff
@@ -1,11 +1,11 @@
 
 
 
 Disassembly of section .fini:
 
-00000000000011a4 <_fini>:
+00000000000011c8 <_fini>:
 _fini():
 	endbr64
 	sub    $0x8,%rsp
 	add    $0x8,%rsp
 	ret
```

#### readelf --wide --decompress --hex-dump=.eh_frame_hdr {}

```diff
@@ -1,6 +1,7 @@
 
 Hex dump of section '.eh_frame_hdr':
-  0x00002004 011b033b 20000000 03000000 1cf0ffff ...; ...........
-  0x00002014 54000000 4cf0ffff 3c000000 45f1ffff T...L...<...E...
-  0x00002024 7c000000                            |...
+  0x00002004 011b033b 30000000 05000000 1cf0ffff ...;0...........
+  0x00002014 64000000 4cf0ffff 8c000000 5cf0ffff d...L.......\...
+  0x00002024 a4000000 7cf0ffff 4c000000 65f1ffff ....|...L...e...
+  0x00002034 bc000000                            ....
```

#### readelf --wide --decompress --hex-dump=.eh_frame {}

```diff
@@ -1,11 +1,14 @@
 
 Hex dump of section '.eh_frame':
-  0x00002028 14000000 00000000 017a5200 01781001 .........zR..x..
-  0x00002038 1b0c0708 90010000 14000000 1c000000 ................
-  0x00002048 08f0ffff 26000000 00440710 00000000 ....&....D......
-  0x00002058 24000000 34000000 c0efffff 30000000 $...4.......0...
-  0x00002068 000e1046 0e184a0f 0b770880 003f1a3b ...F..J..w...?.;
-  0x00002078 2a332422 00000000 1c000000 5c000000 *3$"........\...
-  0x00002088 c1f0ffff 59000000 00410e10 8602430d ....Y....A....C.
-  0x00002098 0602540c 07080000 00000000          ..T.........
+  0x00002038 14000000 00000000 017a5200 01781001 .........zR..x..
+  0x00002048 1b0c0708 90010000 14000000 1c000000 ................
+  0x00002058 28f0ffff 26000000 00440710 00000000 (...&....D......
+  0x00002068 24000000 34000000 b0efffff 30000000 $...4.......0...
+  0x00002078 000e1046 0e184a0f 0b770880 003f1a3a ...F..J..w...?.:
+  0x00002088 2a332422 00000000 14000000 5c000000 *3$"........\...
+  0x00002098 b8efffff 10000000 00000000 00000000 ................
+  0x000020a8 14000000 74000000 b0efffff 20000000 ....t....... ...
+  0x000020b8 00000000 00000000 1c000000 8c000000 ................
+  0x000020c8 a1f0ffff 5d000000 00450e10 8602430d ....]....E....C.
+  0x000020d8 0602540c 07080000 00000000          ..T.........
```

#### readelf --wide --decompress --hex-dump=.init_array {}

```diff
@@ -1,4 +1,4 @@
 
 Hex dump of section '.init_array':
-  0x00003dd0 40110000 00000000                   @.......
+  0x00003db0 60110000 00000000                   `.......
```

#### readelf --wide --decompress --hex-dump=.fini_array {}

```diff
@@ -1,4 +1,4 @@
 
 Hex dump of section '.fini_array':
-  0x00003dd8 f0100000 00000000                   ........
+  0x00003db8 20110000 00000000                    .......
```

#### readelf --wide --decompress --hex-dump=.got {}

```diff
@@ -1,6 +1,9 @@
 
 Hex dump of section '.got':
-  0x00003fc0 00000000 00000000 00000000 00000000 ................
-  0x00003fd0 00000000 00000000 00000000 00000000 ................
-  0x00003fe0 00000000 00000000                   ........
+ NOTE: This section has relocations against it, but these have NOT been applied to this dump.
+  0x00003fb0 c03d0000 00000000 00000000 00000000 .=..............
+  0x00003fc0 00000000 00000000 30100000 00000000 ........0.......
+  0x00003fd0 40100000 00000000 00000000 00000000 @...............
+  0x00003fe0 00000000 00000000 00000000 00000000 ................
+  0x00003ff0 00000000 00000000 00000000 00000000 ................
```

#### readelf --wide --decompress --hex-dump=.data {}

```diff
@@ -1,4 +1,4 @@
 
 Hex dump of section '.data':
-  0x00004010 00000000 00000000 18400000 00000000 .........@......
+  0x00004000 00000000 00000000 08400000 00000000 .........@......
```

#### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,5 +1,4 @@
 
 String dump of section '.comment':
-  [     0]  GCC: (GNU) 13.2.1 20230801
-  [    1b]  GCC: (GNU) 13.2.1 20240417
+  [     0]  GCC: (Ubuntu 11.4.0-1ubuntu1~22.04) 11.4.0
```

#### readelf --wide --decompress --hex-dump=.strtab {}

```diff
@@ -1,25 +1,36 @@
 
 Hex dump of section '.strtab':
-  0x00000000 006a756d 70737461 72742e63 005f4459 .jumpstart.c._DY
-  0x00000010 4e414d49 43005f5f 474e555f 45485f46 NAMIC.__GNU_EH_F
-  0x00000020 52414d45 5f484452 005f474c 4f42414c RAME_HDR._GLOBAL
-  0x00000030 5f4f4646 5345545f 5441424c 455f005f _OFFSET_TABLE_._
-  0x00000040 5f6c6962 635f7374 6172745f 6d61696e _libc_start_main
-  0x00000050 40474c49 42435f32 2e333400 5f49544d @GLIBC_2.34._ITM
-  0x00000060 5f646572 65676973 74657254 4d436c6f _deregisterTMClo
-  0x00000070 6e655461 626c6500 5f656461 7461005f neTable._edata._
-  0x00000080 66696e69 00657865 63766540 474c4942 fini.execve@GLIB
-  0x00000090 435f322e 322e3500 5f5f6461 74615f73 C_2.2.5.__data_s
-  0x000000a0 74617274 005f5f67 6d6f6e5f 73746172 tart.__gmon_star
-  0x000000b0 745f5f00 5f5f6473 6f5f6861 6e646c65 t__.__dso_handle
-  0x000000c0 005f494f 5f737464 696e5f75 73656400 ._IO_stdin_used.
-  0x000000d0 5f656e64 00707472 61636540 474c4942 _end.ptrace@GLIB
-  0x000000e0 435f322e 322e3500 5f5f6273 735f7374 C_2.2.5.__bss_st
-  0x000000f0 61727400 6d61696e 005f5f65 6e766972 art.main.__envir
-  0x00000100 6f6e4047 4c494243 5f322e32 2e35005f on@GLIBC_2.2.5._
-  0x00000110 5f544d43 5f454e44 5f5f005f 49544d5f _TMC_END__._ITM_
-  0x00000120 72656769 73746572 544d436c 6f6e6554 registerTMCloneT
-  0x00000130 61626c65 005f5f63 78615f66 696e616c able.__cxa_final
-  0x00000140 697a6540 474c4942 435f322e 322e3500 ize@GLIBC_2.2.5.
-  0x00000150 5f696e69 7400                       _init.
+  0x00000000 00536372 74312e6f 005f5f61 62695f74 .Scrt1.o.__abi_t
+  0x00000010 61670063 72747374 7566662e 63006465 ag.crtstuff.c.de
+  0x00000020 72656769 73746572 5f746d5f 636c6f6e register_tm_clon
+  0x00000030 6573005f 5f646f5f 676c6f62 616c5f64 es.__do_global_d
+  0x00000040 746f7273 5f617578 00636f6d 706c6574 tors_aux.complet
+  0x00000050 65642e30 005f5f64 6f5f676c 6f62616c ed.0.__do_global
+  0x00000060 5f64746f 72735f61 75785f66 696e695f _dtors_aux_fini_
+  0x00000070 61727261 795f656e 74727900 6672616d array_entry.fram
+  0x00000080 655f6475 6d6d7900 5f5f6672 616d655f e_dummy.__frame_
+  0x00000090 64756d6d 795f696e 69745f61 72726179 dummy_init_array
+  0x000000a0 5f656e74 7279006a 756d7073 74617274 _entry.jumpstart
+  0x000000b0 2e63005f 5f465241 4d455f45 4e445f5f .c.__FRAME_END__
+  0x000000c0 005f4459 4e414d49 43005f5f 474e555f ._DYNAMIC.__GNU_
+  0x000000d0 45485f46 52414d45 5f484452 005f474c EH_FRAME_HDR._GL
+  0x000000e0 4f42414c 5f4f4646 5345545f 5441424c OBAL_OFFSET_TABL
+  0x000000f0 455f005f 5f6c6962 635f7374 6172745f E_.__libc_start_
+  0x00000100 6d61696e 40474c49 42435f32 2e333400 main@GLIBC_2.34.
+  0x00000110 5f49544d 5f646572 65676973 74657254 _ITM_deregisterT
+  0x00000120 4d436c6f 6e655461 626c6500 5f656461 MCloneTable._eda
+  0x00000130 7461005f 66696e69 00657865 63766540 ta._fini.execve@
+  0x00000140 474c4942 435f322e 322e3500 5f5f6461 GLIBC_2.2.5.__da
+  0x00000150 74615f73 74617274 005f5f67 6d6f6e5f ta_start.__gmon_
+  0x00000160 73746172 745f5f00 5f5f6473 6f5f6861 start__.__dso_ha
+  0x00000170 6e646c65 005f494f 5f737464 696e5f75 ndle._IO_stdin_u
+  0x00000180 73656400 5f656e64 00707472 61636540 sed._end.ptrace@
+  0x00000190 474c4942 435f322e 322e3500 5f5f6273 GLIBC_2.2.5.__bs
+  0x000001a0 735f7374 61727400 6d61696e 005f5f65 s_start.main.__e
+  0x000001b0 6e766972 6f6e4047 4c494243 5f322e32 nviron@GLIBC_2.2
+  0x000001c0 2e35005f 5f544d43 5f454e44 5f5f005f .5.__TMC_END__._
+  0x000001d0 49544d5f 72656769 73746572 544d436c ITM_registerTMCl
+  0x000001e0 6f6e6554 61626c65 005f5f63 78615f66 oneTable.__cxa_f
+  0x000001f0 696e616c 697a6540 474c4942 435f322e inalize@GLIBC_2.
+  0x00000200 322e3500 5f696e69 7400              2.5._init.
```

#### readelf --wide --decompress --hex-dump=.shstrtab {}

```diff
@@ -6,16 +6,16 @@
   0x00000030 70657274 79002e6e 6f74652e 676e752e perty..note.gnu.
   0x00000040 6275696c 642d6964 002e6e6f 74652e41 build-id..note.A
   0x00000050 42492d74 6167002e 676e752e 68617368 BI-tag..gnu.hash
   0x00000060 002e6479 6e73796d 002e6479 6e737472 ..dynsym..dynstr
   0x00000070 002e676e 752e7665 7273696f 6e002e67 ..gnu.version..g
   0x00000080 6e752e76 65727369 6f6e5f72 002e7265 nu.version_r..re
   0x00000090 6c612e64 796e002e 72656c61 2e706c74 la.dyn..rela.plt
-  0x000000a0 002e696e 6974002e 74657874 002e6669 ..init..text..fi
-  0x000000b0 6e69002e 726f6461 7461002e 65685f66 ni..rodata..eh_f
-  0x000000c0 72616d65 5f686472 002e6568 5f667261 rame_hdr..eh_fra
-  0x000000d0 6d65002e 696e6974 5f617272 6179002e me..init_array..
-  0x000000e0 66696e69 5f617272 6179002e 64796e61 fini_array..dyna
-  0x000000f0 6d696300 2e676f74 002e676f 742e706c mic..got..got.pl
-  0x00000100 74002e64 61746100 2e627373 002e636f t..data..bss..co
-  0x00000110 6d6d656e 7400                       mment.
+  0x000000a0 002e696e 6974002e 706c742e 676f7400 ..init..plt.got.
+  0x000000b0 2e706c74 2e736563 002e7465 7874002e .plt.sec..text..
+  0x000000c0 66696e69 002e726f 64617461 002e6568 fini..rodata..eh
+  0x000000d0 5f667261 6d655f68 6472002e 65685f66 _frame_hdr..eh_f
+  0x000000e0 72616d65 002e696e 69745f61 72726179 rame..init_array
+  0x000000f0 002e6669 6e695f61 72726179 002e6479 ..fini_array..dy
+  0x00000100 6e616d69 63002e64 61746100 2e627373 namic..data..bss
+  0x00000110 002e636f 6d6d656e 7400              ..comment.
```

### Comparing `libdebug-0.4/libdebug/ptrace/ptrace_constants.py` & `libdebug-0.4.1/libdebug/ptrace/ptrace_constants.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4/libdebug/ptrace/ptrace_status_handler.py` & `libdebug-0.4.1/libdebug/ptrace/ptrace_status_handler.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4/libdebug/state/debugging_context.py` & `libdebug-0.4.1/libdebug/state/debugging_context.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4/libdebug/state/thread_context.py` & `libdebug-0.4.1/libdebug/state/thread_context.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4/libdebug/utils/debugging_utils.py` & `libdebug-0.4.1/libdebug/utils/debugging_utils.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4/libdebug/utils/elf_utils.py` & `libdebug-0.4.1/libdebug/utils/elf_utils.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4/libdebug/utils/gdb.py` & `libdebug-0.4.1/libdebug/utils/gdb.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4/libdebug/utils/libcontext.py` & `libdebug-0.4.1/libdebug/utils/libcontext.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4/libdebug/utils/pipe_manager.py` & `libdebug-0.4.1/libdebug/utils/pipe_manager.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4/libdebug/utils/posix_spawn.py` & `libdebug-0.4.1/libdebug/utils/posix_spawn.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4/libdebug/utils/process_utils.py` & `libdebug-0.4.1/libdebug/utils/process_utils.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4/libdebug/utils/register_utils.py` & `libdebug-0.4.1/libdebug/utils/register_utils.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4/libdebug/utils/syscall_utils.py` & `libdebug-0.4.1/libdebug/utils/syscall_utils.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4/libdebug.egg-info/SOURCES.txt` & `libdebug-0.4.1/libdebug.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 LICENSE
+MANIFEST.in
 README.md
+pyproject.toml
 setup.py
 libdebug/__init__.py
 libdebug/libdebug.py
 libdebug/liblog.py
 libdebug.egg-info/PKG-INFO
 libdebug.egg-info/SOURCES.txt
 libdebug.egg-info/dependency_links.txt
```

### Comparing `libdebug-0.4/setup.py` & `libdebug-0.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,16 +65,15 @@
         outputs = build.get_outputs(self)
         outputs.append("libdebug/ptrace/jumpstart/jumpstart")
         return outputs
 
 
 setup(
     name="libdebug",
-    version="0.4",
-    author="JinBlack",
+    version="0.4.1",
     description="A library to debug binary programs",
     packages=find_packages(include=["libdebug", "libdebug.*"]),
     install_requires=[
         "capstone",
         "pyelftools",
         "cffi",
         "requests",
```

