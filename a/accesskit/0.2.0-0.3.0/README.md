# Comparing `tmp/accesskit-0.2.0.tar.gz` & `tmp/accesskit-0.3.0.tar.gz`

## Comparing `accesskit-0.2.0.tar` & `accesskit-0.3.0.tar`

### file list

```diff
@@ -1,95 +1,95 @@
--rw-r--r--   0     1001      127      885 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/macos/Cargo.toml
--rw-r--r--   0     1001      127    13501 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/macos/CHANGELOG.md
--rw-r--r--   0     1001      127      183 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/macos/README.md
--rw-r--r--   0     1001      127     9664 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/macos/src/adapter.rs
--rw-r--r--   0     1001      127     2724 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/macos/src/context.rs
--rw-r--r--   0     1001      127     9005 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/macos/src/event.rs
--rw-r--r--   0     1001      127      334 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/macos/src/filters.rs
--rw-r--r--   0     1001      127      559 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/macos/src/lib.rs
--rw-r--r--   0     1001      127    33032 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/macos/src/node.rs
--rw-r--r--   0     1001      127     3147 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/macos/src/patch.rs
--rw-r--r--   0     1001      127     9525 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/macos/src/subclass.rs
--rw-r--r--   0     1001      127     2878 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/macos/src/util.rs
--rw-r--r--   0     1001      127      669 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/atspi-common/Cargo.toml
--rw-r--r--   0     1001      127     1796 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/atspi-common/CHANGELOG.md
--rw-r--r--   0     1001      127      317 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/atspi-common/README.md
--rw-r--r--   0     1001      127      432 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/atspi-common/src/action.rs
--rw-r--r--   0     1001      127    12747 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/atspi-common/src/adapter.rs
--rw-r--r--   0     1001      127      583 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/atspi-common/src/callback.rs
--rw-r--r--   0     1001      127     3414 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/atspi-common/src/context.rs
--rw-r--r--   0     1001      127      541 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/atspi-common/src/error.rs
--rw-r--r--   0     1001      127     1036 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/atspi-common/src/events.rs
--rw-r--r--   0     1001      127      334 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/atspi-common/src/filters.rs
--rw-r--r--   0     1001      127      753 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/atspi-common/src/lib.rs
--rw-r--r--   0     1001      127    39237 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/atspi-common/src/node.rs
--rw-r--r--   0     1001      127      898 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/atspi-common/src/rect.rs
--rw-r--r--   0     1001      127    13107 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/atspi-common/src/simplified.rs
--rw-r--r--   0     1001      127     1157 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/atspi-common/src/util.rs
--rw-r--r--   0     1001      127      407 2024-04-14 17:20:57.000000 accesskit-0.2.0/consumer/Cargo.toml
--rw-r--r--   0     1001      127    16203 2024-04-14 17:20:57.000000 accesskit-0.2.0/consumer/CHANGELOG.md
--rw-r--r--   0     1001      127      207 2024-04-14 17:20:57.000000 accesskit-0.2.0/consumer/README.md
--rw-r--r--   0     1001      127     1262 2024-04-14 17:20:57.000000 accesskit-0.2.0/consumer/src/filters.rs
--rw-r--r--   0     1001      127    24021 2024-04-14 17:20:57.000000 accesskit-0.2.0/consumer/src/iterators.rs
--rw-r--r--   0     1001      127     6371 2024-04-14 17:20:57.000000 accesskit-0.2.0/consumer/src/lib.rs
--rw-r--r--   0     1001      127    33855 2024-04-14 17:20:57.000000 accesskit-0.2.0/consumer/src/node.rs
--rw-r--r--   0     1001      127    64603 2024-04-14 17:20:57.000000 accesskit-0.2.0/consumer/src/text.rs
--rw-r--r--   0     1001      127    27310 2024-04-14 17:20:57.000000 accesskit-0.2.0/consumer/src/tree.rs
--rw-r--r--   0     1001      127      704 2024-04-14 17:20:57.000000 accesskit-0.2.0/common/Cargo.toml
--rw-r--r--   0     1001      127    13085 2024-04-14 17:20:57.000000 accesskit-0.2.0/common/CHANGELOG.md
--rw-r--r--   0     1001      127      740 2024-04-14 17:20:57.000000 accesskit-0.2.0/common/README.md
--rw-r--r--   0     1001      127    22792 2024-04-14 17:20:57.000000 accesskit-0.2.0/common/src/geometry.rs
--rw-r--r--   0     1001      127    81176 2024-04-14 17:20:57.000000 accesskit-0.2.0/common/src/lib.rs
--rw-r--r--   0     1001      127     1315 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/unix/Cargo.toml
--rw-r--r--   0     1001      127    10539 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/unix/CHANGELOG.md
--rw-r--r--   0     1001      127      487 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/unix/README.md
--rw-r--r--   0     1001      127     6935 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/unix/src/adapter.rs
--rw-r--r--   0     1001      127    13572 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/unix/src/atspi/bus.rs
--rw-r--r--   0     1001      127     6053 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/unix/src/atspi/interfaces/accessible.rs
--rw-r--r--   0     1001      127     1473 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/unix/src/atspi/interfaces/action.rs
--rw-r--r--   0     1001      127     1096 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/unix/src/atspi/interfaces/application.rs
--rw-r--r--   0     1001      127     2195 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/unix/src/atspi/interfaces/component.rs
--rw-r--r--   0     1001      127      945 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/unix/src/atspi/interfaces/mod.rs
--rw-r--r--   0     1001      127     1459 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/unix/src/atspi/interfaces/value.rs
--rw-r--r--   0     1001      127      404 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/unix/src/atspi/mod.rs
--rw-r--r--   0     1001      127     1224 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/unix/src/atspi/object_address.rs
--rw-r--r--   0     1001      127     2185 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/unix/src/atspi/object_id.rs
--rw-r--r--   0     1001      127     8069 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/unix/src/context.rs
--rw-r--r--   0     1001      127     4885 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/unix/src/executor.rs
--rw-r--r--   0     1001      127     1005 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/unix/src/lib.rs
--rw-r--r--   0     1001      127     1389 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/unix/src/util.rs
--rw-r--r--   0     1001      127      955 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/windows/Cargo.toml
--rw-r--r--   0     1001      127    23152 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/windows/CHANGELOG.md
--rw-r--r--   0     1001      127      172 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/windows/README.md
--rw-r--r--   0     1001      127    11956 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/windows/examples/hello_world.rs
--rw-r--r--   0     1001      127    16625 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/windows/src/adapter.rs
--rw-r--r--   0     1001      127     1696 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/windows/src/context.rs
--rw-r--r--   0     1001      127      403 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/windows/src/filters.rs
--rw-r--r--   0     1001      127      482 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/windows/src/lib.rs
--rw-r--r--   0     1001      127    37364 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/windows/src/node.rs
--rw-r--r--   0     1001      127     6179 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/windows/src/subclass.rs
--rw-r--r--   0     1001      127    11438 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/windows/src/tests/mod.rs
--rw-r--r--   0     1001      127     7069 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/windows/src/tests/simple.rs
--rw-r--r--   0     1001      127     3178 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/windows/src/tests/subclassed.rs
--rw-r--r--   0     1001      127    19705 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/windows/src/text.rs
--rw-r--r--   0     1001      127     6500 2024-04-14 17:20:57.000000 accesskit-0.2.0/platforms/windows/src/util.rs
--rw-r--r--   0        0        0      984 1970-01-01 00:00:00.000000 accesskit-0.2.0/bindings/python/Cargo.toml
--rw-r--r--   0     1001      127      224 2024-04-14 17:20:57.000000 accesskit-0.2.0/bindings/python/.cargo/config.toml
--rw-r--r--   0     1001      127     2674 2024-04-14 17:20:57.000000 accesskit-0.2.0/bindings/python/CHANGELOG.md
--rw-r--r--   0     1001      127      981 2024-04-14 17:20:57.000000 accesskit-0.2.0/bindings/python/README.md
--rw-r--r--   0     1001      127     3078 2024-04-14 17:20:57.000000 accesskit-0.2.0/bindings/python/examples/pygame/.gitignore
--rw-r--r--   0     1001      127      367 2024-04-14 17:20:57.000000 accesskit-0.2.0/bindings/python/examples/pygame/README.md
--rw-r--r--   0     1001      127     7179 2024-04-14 17:20:57.000000 accesskit-0.2.0/bindings/python/examples/pygame/hello_world.py
--rw-r--r--   0     1001      127       24 2024-04-14 17:20:57.000000 accesskit-0.2.0/bindings/python/examples/pygame/requirements.txt
--rw-r--r--   0     1001      127    24683 2024-04-14 17:20:57.000000 accesskit-0.2.0/bindings/python/src/common.rs
--rw-r--r--   0     1001      127     4784 2024-04-14 17:20:57.000000 accesskit-0.2.0/bindings/python/src/geometry.rs
--rw-r--r--   0     1001      127     2854 2024-04-14 17:20:57.000000 accesskit-0.2.0/bindings/python/src/lib.rs
--rw-r--r--   0     1001      127     7316 2024-04-14 17:20:57.000000 accesskit-0.2.0/bindings/python/src/macos.rs
--rw-r--r--   0     1001      127     1506 2024-04-14 17:20:57.000000 accesskit-0.2.0/bindings/python/src/unix.rs
--rw-r--r--   0     1001      127     4126 2024-04-14 17:20:57.000000 accesskit-0.2.0/bindings/python/src/windows.rs
--rw-r--r--   0     1001      127    72633 2024-04-14 17:20:57.000000 accesskit-0.2.0/Cargo.lock
--rw-r--r--   0        0        0      475 1970-01-01 00:00:00.000000 accesskit-0.2.0/Cargo.toml
--rw-r--r--   0     1001      127     1043 2024-04-14 17:20:57.000000 accesskit-0.2.0/pyproject.toml
--rw-r--r--   0     1001      127     9723 2024-04-14 17:20:57.000000 accesskit-0.2.0/LICENSE-APACHE
--rw-r--r--   0     1001      127     1023 2024-04-14 17:20:57.000000 accesskit-0.2.0/LICENSE-MIT
--rw-r--r--   0     1001      127     1559 2024-04-14 17:20:57.000000 accesskit-0.2.0/LICENSE.chromium
--rw-r--r--   0        0        0     1958 1970-01-01 00:00:00.000000 accesskit-0.2.0/PKG-INFO
+-rw-r--r--   0     1001      127     1294 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/unix/Cargo.toml
+-rw-r--r--   0     1001      127    11392 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/unix/CHANGELOG.md
+-rw-r--r--   0     1001      127      487 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/unix/README.md
+-rw-r--r--   0     1001      127     6935 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/unix/src/adapter.rs
+-rw-r--r--   0     1001      127    13572 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/unix/src/atspi/bus.rs
+-rw-r--r--   0     1001      127     6053 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/unix/src/atspi/interfaces/accessible.rs
+-rw-r--r--   0     1001      127     1473 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/unix/src/atspi/interfaces/action.rs
+-rw-r--r--   0     1001      127     1096 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/unix/src/atspi/interfaces/application.rs
+-rw-r--r--   0     1001      127     2195 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/unix/src/atspi/interfaces/component.rs
+-rw-r--r--   0     1001      127      945 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/unix/src/atspi/interfaces/mod.rs
+-rw-r--r--   0     1001      127     1459 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/unix/src/atspi/interfaces/value.rs
+-rw-r--r--   0     1001      127      404 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/unix/src/atspi/mod.rs
+-rw-r--r--   0     1001      127     1224 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/unix/src/atspi/object_address.rs
+-rw-r--r--   0     1001      127     2185 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/unix/src/atspi/object_id.rs
+-rw-r--r--   0     1001      127     8048 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/unix/src/context.rs
+-rw-r--r--   0     1001      127     4885 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/unix/src/executor.rs
+-rw-r--r--   0     1001      127     1005 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/unix/src/lib.rs
+-rw-r--r--   0     1001      127     1389 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/unix/src/util.rs
+-rw-r--r--   0     1001      127      956 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/windows/Cargo.toml
+-rw-r--r--   0     1001      127    25318 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/windows/CHANGELOG.md
+-rw-r--r--   0     1001      127      172 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/windows/README.md
+-rw-r--r--   0     1001      127    11651 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/windows/examples/hello_world.rs
+-rw-r--r--   0     1001      127    16519 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/windows/src/adapter.rs
+-rw-r--r--   0     1001      127     1696 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/windows/src/context.rs
+-rw-r--r--   0     1001      127      403 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/windows/src/filters.rs
+-rw-r--r--   0     1001      127      482 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/windows/src/lib.rs
+-rw-r--r--   0     1001      127    37537 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/windows/src/node.rs
+-rw-r--r--   0     1001      127     6179 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/windows/src/subclass.rs
+-rw-r--r--   0     1001      127    11438 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/windows/src/tests/mod.rs
+-rw-r--r--   0     1001      127     6937 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/windows/src/tests/simple.rs
+-rw-r--r--   0     1001      127     3536 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/windows/src/tests/subclassed.rs
+-rw-r--r--   0     1001      127    19705 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/windows/src/text.rs
+-rw-r--r--   0     1001      127     6500 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/windows/src/util.rs
+-rw-r--r--   0     1001      127      705 2024-04-30 13:52:12.000000 accesskit-0.3.0/common/Cargo.toml
+-rw-r--r--   0     1001      127    15163 2024-04-30 13:52:12.000000 accesskit-0.3.0/common/CHANGELOG.md
+-rw-r--r--   0     1001      127      740 2024-04-30 13:52:12.000000 accesskit-0.3.0/common/README.md
+-rw-r--r--   0     1001      127    22792 2024-04-30 13:52:12.000000 accesskit-0.3.0/common/src/geometry.rs
+-rw-r--r--   0     1001      127    78839 2024-04-30 13:52:12.000000 accesskit-0.3.0/common/src/lib.rs
+-rw-r--r--   0     1001      127      670 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/atspi-common/Cargo.toml
+-rw-r--r--   0     1001      127     3246 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/atspi-common/CHANGELOG.md
+-rw-r--r--   0     1001      127      317 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/atspi-common/README.md
+-rw-r--r--   0     1001      127      432 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/atspi-common/src/action.rs
+-rw-r--r--   0     1001      127    12747 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/atspi-common/src/adapter.rs
+-rw-r--r--   0     1001      127      583 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/atspi-common/src/callback.rs
+-rw-r--r--   0     1001      127     3414 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/atspi-common/src/context.rs
+-rw-r--r--   0     1001      127      541 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/atspi-common/src/error.rs
+-rw-r--r--   0     1001      127     1036 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/atspi-common/src/events.rs
+-rw-r--r--   0     1001      127      334 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/atspi-common/src/filters.rs
+-rw-r--r--   0     1001      127      753 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/atspi-common/src/lib.rs
+-rw-r--r--   0     1001      127    39282 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/atspi-common/src/node.rs
+-rw-r--r--   0     1001      127      898 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/atspi-common/src/rect.rs
+-rw-r--r--   0     1001      127    13107 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/atspi-common/src/simplified.rs
+-rw-r--r--   0     1001      127     1157 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/atspi-common/src/util.rs
+-rw-r--r--   0     1001      127      942 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/macos/Cargo.toml
+-rw-r--r--   0     1001      127    15387 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/macos/CHANGELOG.md
+-rw-r--r--   0     1001      127      183 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/macos/README.md
+-rw-r--r--   0     1001      127     9554 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/macos/src/adapter.rs
+-rw-r--r--   0     1001      127     2731 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/macos/src/context.rs
+-rw-r--r--   0     1001      127     9063 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/macos/src/event.rs
+-rw-r--r--   0     1001      127      334 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/macos/src/filters.rs
+-rw-r--r--   0     1001      127      557 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/macos/src/lib.rs
+-rw-r--r--   0     1001      127    33624 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/macos/src/node.rs
+-rw-r--r--   0     1001      127     3146 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/macos/src/patch.rs
+-rw-r--r--   0     1001      127     9523 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/macos/src/subclass.rs
+-rw-r--r--   0     1001      127     2819 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/macos/src/util.rs
+-rw-r--r--   0     1001      127      406 2024-04-30 13:52:12.000000 accesskit-0.3.0/consumer/Cargo.toml
+-rw-r--r--   0     1001      127    17755 2024-04-30 13:52:12.000000 accesskit-0.3.0/consumer/CHANGELOG.md
+-rw-r--r--   0     1001      127      207 2024-04-30 13:52:12.000000 accesskit-0.3.0/consumer/README.md
+-rw-r--r--   0     1001      127     1262 2024-04-30 13:52:12.000000 accesskit-0.3.0/consumer/src/filters.rs
+-rw-r--r--   0     1001      127    24021 2024-04-30 13:52:12.000000 accesskit-0.3.0/consumer/src/iterators.rs
+-rw-r--r--   0     1001      127     6115 2024-04-30 13:52:12.000000 accesskit-0.3.0/consumer/src/lib.rs
+-rw-r--r--   0     1001      127    33886 2024-04-30 13:52:12.000000 accesskit-0.3.0/consumer/src/node.rs
+-rw-r--r--   0     1001      127    64423 2024-04-30 13:52:12.000000 accesskit-0.3.0/consumer/src/text.rs
+-rw-r--r--   0     1001      127    26521 2024-04-30 13:52:12.000000 accesskit-0.3.0/consumer/src/tree.rs
+-rw-r--r--   0        0        0      983 1970-01-01 00:00:00.000000 accesskit-0.3.0/bindings/python/Cargo.toml
+-rw-r--r--   0     1001      127      224 2024-04-30 13:52:12.000000 accesskit-0.3.0/bindings/python/.cargo/config.toml
+-rw-r--r--   0     1001      127     4763 2024-04-30 13:52:12.000000 accesskit-0.3.0/bindings/python/CHANGELOG.md
+-rw-r--r--   0     1001      127      981 2024-04-30 13:52:12.000000 accesskit-0.3.0/bindings/python/README.md
+-rw-r--r--   0     1001      127     3078 2024-04-30 13:52:12.000000 accesskit-0.3.0/bindings/python/examples/pygame/.gitignore
+-rw-r--r--   0     1001      127      367 2024-04-30 13:52:12.000000 accesskit-0.3.0/bindings/python/examples/pygame/README.md
+-rw-r--r--   0     1001      127     6979 2024-04-30 13:52:12.000000 accesskit-0.3.0/bindings/python/examples/pygame/hello_world.py
+-rw-r--r--   0     1001      127       24 2024-04-30 13:52:12.000000 accesskit-0.3.0/bindings/python/examples/pygame/requirements.txt
+-rw-r--r--   0     1001      127    24054 2024-04-30 13:52:12.000000 accesskit-0.3.0/bindings/python/src/common.rs
+-rw-r--r--   0     1001      127     4784 2024-04-30 13:52:12.000000 accesskit-0.3.0/bindings/python/src/geometry.rs
+-rw-r--r--   0     1001      127     2818 2024-04-30 13:52:12.000000 accesskit-0.3.0/bindings/python/src/lib.rs
+-rw-r--r--   0     1001      127     7316 2024-04-30 13:52:12.000000 accesskit-0.3.0/bindings/python/src/macos.rs
+-rw-r--r--   0     1001      127     1506 2024-04-30 13:52:12.000000 accesskit-0.3.0/bindings/python/src/unix.rs
+-rw-r--r--   0     1001      127     4126 2024-04-30 13:52:12.000000 accesskit-0.3.0/bindings/python/src/windows.rs
+-rw-r--r--   0     1001      127    73406 2024-04-30 13:52:12.000000 accesskit-0.3.0/Cargo.lock
+-rw-r--r--   0        0        0      473 1970-01-01 00:00:00.000000 accesskit-0.3.0/Cargo.toml
+-rw-r--r--   0     1001      127     1043 2024-04-30 13:52:12.000000 accesskit-0.3.0/pyproject.toml
+-rw-r--r--   0     1001      127     9723 2024-04-30 13:52:12.000000 accesskit-0.3.0/LICENSE-APACHE
+-rw-r--r--   0     1001      127     1023 2024-04-30 13:52:12.000000 accesskit-0.3.0/LICENSE-MIT
+-rw-r--r--   0     1001      127     1559 2024-04-30 13:52:12.000000 accesskit-0.3.0/LICENSE.chromium
+-rw-r--r--   0        0        0     1958 1970-01-01 00:00:00.000000 accesskit-0.3.0/PKG-INFO
```

### Comparing `accesskit-0.2.0/platforms/macos/CHANGELOG.md` & `accesskit-0.3.0/platforms/macos/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,48 @@
     * accesskit_consumer bumped from 0.16.0 to 0.16.1
 
 * The following workspace dependencies were updated
   * dependencies
     * accesskit bumped from 0.12.2 to 0.12.3
     * accesskit_consumer bumped from 0.17.0 to 0.17.1
 
+## [0.13.0](https://github.com/AccessKit/accesskit/compare/accesskit_macos-v0.12.0...accesskit_macos-v0.13.0) (2024-04-30)
+
+
+### ⚠ BREAKING CHANGES
+
+* Clean up table roles and properties ([#393](https://github.com/AccessKit/accesskit/issues/393))
+* Drop `NodeClassSet` ([#389](https://github.com/AccessKit/accesskit/issues/389))
+* Rename `Checked` to `Toggled`; drop `ToggleButton` role ([#388](https://github.com/AccessKit/accesskit/issues/388))
+
+### Features
+
+* Implement the `description` property ([#382](https://github.com/AccessKit/accesskit/issues/382)) ([d49f406](https://github.com/AccessKit/accesskit/commit/d49f40660b5dc23ed074cd72a91e511b130756ae))
+
+
+### Bug Fixes
+
+* Increase minimum supported Rust version to `1.70` ([#396](https://github.com/AccessKit/accesskit/issues/396)) ([a8398b8](https://github.com/AccessKit/accesskit/commit/a8398b847aa003de91042ac45e33126fc2cae053))
+* Use new objc2 crates ([#384](https://github.com/AccessKit/accesskit/issues/384)) ([b3484c0](https://github.com/AccessKit/accesskit/commit/b3484c0fb1fef3ecd41ff9592978336c20b8b4f8))
+
+
+### Code Refactoring
+
+* Clean up table roles and properties ([#393](https://github.com/AccessKit/accesskit/issues/393)) ([e34dad9](https://github.com/AccessKit/accesskit/commit/e34dad94448a5321ece9def3f2e054aa5f62dd79))
+* Drop `NodeClassSet` ([#389](https://github.com/AccessKit/accesskit/issues/389)) ([1b153ed](https://github.com/AccessKit/accesskit/commit/1b153ed51f8421cdba2dc98beca2e8f5f8c781bc))
+* Rename `Checked` to `Toggled`; drop `ToggleButton` role ([#388](https://github.com/AccessKit/accesskit/issues/388)) ([6bc040b](https://github.com/AccessKit/accesskit/commit/6bc040b7cf75cdbd6a019cc380d8dbce804b3c81))
+
+
+### Dependencies
+
+* The following workspace dependencies were updated
+  * dependencies
+    * accesskit bumped from 0.13.0 to 0.14.0
+    * accesskit_consumer bumped from 0.18.0 to 0.19.0
+
 ## [0.12.0](https://github.com/AccessKit/accesskit/compare/accesskit_macos-v0.11.1...accesskit_macos-v0.12.0) (2024-04-14)
 
 
 ### ⚠ BREAKING CHANGES
 
 * New approach to lazy initialization ([#375](https://github.com/AccessKit/accesskit/issues/375))
```

### Comparing `accesskit-0.2.0/platforms/macos/src/adapter.rs` & `accesskit-0.3.0/platforms/macos/src/adapter.rs`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,17 @@
 // the LICENSE-MIT file), at your option.
 
 use accesskit::{
     ActionHandler, ActionRequest, ActivationHandler, NodeBuilder, NodeId, Role, Tree as TreeData,
     TreeUpdate,
 };
 use accesskit_consumer::{FilterResult, Tree};
-use icrate::{
-    AppKit::NSView,
-    Foundation::{MainThreadMarker, NSArray, NSObject, NSPoint},
-};
 use objc2::rc::{Id, WeakId};
+use objc2_app_kit::NSView;
+use objc2_foundation::{MainThreadMarker, NSArray, NSObject, NSPoint};
 use std::{ffi::c_void, ptr::null_mut, rc::Rc};
 
 use crate::{
     context::{ActionHandlerNoMut, ActionHandlerWrapper, Context},
     event::{focus_event, EventGenerator, QueuedEvents},
     filters::filter,
     node::can_be_focused,
@@ -163,18 +161,15 @@
                     let context = Context::new(view.clone(), tree, Rc::clone(action_handler), *mtm);
                     let result = Rc::clone(&context);
                     self.state = State::Active(context);
                     result
                 }
                 None => {
                     let placeholder_update = TreeUpdate {
-                        nodes: vec![(
-                            PLACEHOLDER_ROOT_ID,
-                            NodeBuilder::new(Role::Window).build(&mut Default::default()),
-                        )],
+                        nodes: vec![(PLACEHOLDER_ROOT_ID, NodeBuilder::new(Role::Window).build())],
                         tree: Some(TreeData::new(PLACEHOLDER_ROOT_ID)),
                         focus: PLACEHOLDER_ROOT_ID,
                     };
                     let placeholder_tree = Tree::new(placeholder_update, false);
                     let placeholder_context = Context::new(
                         view.clone(),
                         placeholder_tree,
```

### Comparing `accesskit-0.2.0/platforms/macos/src/context.rs` & `accesskit-0.3.0/platforms/macos/src/context.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 // Copyright 2022 The AccessKit Authors. All rights reserved.
 // Licensed under the Apache License, Version 2.0 (found in
 // the LICENSE-APACHE file) or the MIT license (found in
 // the LICENSE-MIT file), at your option.
 
 use accesskit::{ActionHandler, ActionRequest, NodeId};
 use accesskit_consumer::Tree;
-use icrate::{AppKit::*, Foundation::MainThreadMarker};
 use objc2::rc::{Id, WeakId};
+use objc2_app_kit::*;
+use objc2_foundation::MainThreadMarker;
 use std::{cell::RefCell, collections::HashMap, rc::Rc};
 
 use crate::node::PlatformNode;
 
 pub(crate) trait ActionHandlerNoMut {
     fn do_action(&self, request: ActionRequest);
 }
```

### Comparing `accesskit-0.2.0/platforms/macos/src/event.rs` & `accesskit-0.3.0/platforms/macos/src/event.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 // Copyright 2022 The AccessKit Authors. All rights reserved.
 // Licensed under the Apache License, Version 2.0 (found in
 // the LICENSE-APACHE file) or the MIT license (found in
 // the LICENSE-MIT file), at your option.
 
 use accesskit::{Live, NodeId, Role};
 use accesskit_consumer::{DetachedNode, FilterResult, Node, TreeChangeHandler, TreeState};
-use icrate::{
-    AppKit::*,
-    Foundation::{NSMutableDictionary, NSNumber, NSString},
-};
 use objc2::runtime::{AnyObject, ProtocolObject};
+use objc2_app_kit::*;
+use objc2_foundation::{NSMutableDictionary, NSNumber, NSString};
 use std::{collections::HashSet, rc::Rc};
 
 use crate::{
     context::Context,
     filters::{filter, filter_detached},
     node::NodeWrapper,
 };
@@ -33,17 +31,17 @@
 }
 
 impl QueuedEvent {
     fn live_region_announcement(node: &Node) -> Self {
         Self::Announcement {
             text: node.name().unwrap(),
             priority: if node.live() == Live::Assertive {
-                NSAccessibilityPriorityHigh
+                NSAccessibilityPriorityLevel::NSAccessibilityPriorityHigh
             } else {
-                NSAccessibilityPriorityMedium
+                NSAccessibilityPriorityLevel::NSAccessibilityPriorityMedium
             },
         }
     }
 
     fn raise(self, context: &Rc<Context>) {
         match self {
             Self::Generic {
@@ -82,15 +80,15 @@
                 let text = NSString::from_str(&text);
                 unsafe {
                     user_info.setObject_forKey(
                         &*text,
                         ProtocolObject::from_ref(NSAccessibilityAnnouncementKey),
                     )
                 };
-                let priority = NSNumber::new_isize(priority);
+                let priority = NSNumber::new_isize(priority.0);
                 unsafe {
                     user_info.setObject_forKey(
                         &*priority,
                         ProtocolObject::from_ref(NSAccessibilityPriorityKey),
                     )
                 };
```

### Comparing `accesskit-0.2.0/platforms/macos/src/lib.rs` & `accesskit-0.3.0/platforms/macos/src/lib.rs`

 * *Files 3% similar despite different names*

```diff
@@ -18,8 +18,8 @@
 
 mod patch;
 pub use patch::add_focus_forwarder_to_window_class;
 
 mod subclass;
 pub use subclass::SubclassingAdapter;
 
-pub use icrate::Foundation::{NSArray, NSObject, NSPoint};
+pub use objc2_foundation::{NSArray, NSObject, NSPoint};
```

### Comparing `accesskit-0.2.0/platforms/macos/src/node.rs` & `accesskit-0.3.0/platforms/macos/src/node.rs`

 * *Files 2% similar despite different names*

```diff
@@ -6,30 +6,28 @@
 // Derived from Chromium's accessibility abstraction.
 // Copyright 2018 The Chromium Authors. All rights reserved.
 // Use of this source code is governed by a BSD-style license that can be
 // found in the LICENSE.chromium file.
 
 #![allow(non_upper_case_globals)]
 
-use accesskit::{Action, ActionData, ActionRequest, Checked, NodeId, Role, TextSelection};
+use accesskit::{Action, ActionData, ActionRequest, NodeId, Role, TextSelection, Toggled};
 use accesskit_consumer::{DetachedNode, FilterResult, Node, NodeState};
-use icrate::{
-    AppKit::*,
-    Foundation::{
-        ns_string, NSArray, NSCopying, NSInteger, NSNumber, NSObject, NSPoint, NSRange, NSRect,
-        NSString,
-    },
-};
 use objc2::{
     declare_class, msg_send_id,
     mutability::InteriorMutable,
     rc::Id,
     runtime::{AnyObject, Sel},
     sel, ClassType, DeclaredClass,
 };
+use objc2_app_kit::*;
+use objc2_foundation::{
+    ns_string, NSArray, NSCopying, NSInteger, NSNumber, NSObject, NSPoint, NSRange, NSRect,
+    NSString,
+};
 use std::rc::{Rc, Weak};
 
 use crate::{context::Context, filters::filter, util::*};
 
 fn ns_role(node_state: &NodeState) -> &'static NSAccessibilityRole {
     let role = node_state.role();
     // TODO: Handle special cases.
@@ -55,28 +53,32 @@
             Role::TextInput
             | Role::SearchInput
             | Role::EmailInput
             | Role::NumberInput
             | Role::PasswordInput
             | Role::PhoneNumberInput
             | Role::UrlInput => NSAccessibilityTextFieldRole,
-            Role::Button | Role::DefaultButton => NSAccessibilityButtonRole,
+            Role::Button => {
+                if node_state.toggled().is_some() {
+                    NSAccessibilityCheckBoxRole
+                } else {
+                    NSAccessibilityButtonRole
+                }
+            }
+            Role::DefaultButton => NSAccessibilityButtonRole,
             Role::Pane => NSAccessibilityUnknownRole,
             Role::RowHeader => NSAccessibilityCellRole,
             Role::ColumnHeader => NSAccessibilityCellRole,
-            Role::Column => NSAccessibilityColumnRole,
             Role::RowGroup => NSAccessibilityGroupRole,
             Role::List => NSAccessibilityListRole,
             Role::Table => NSAccessibilityTableRole,
-            Role::TableHeaderContainer => NSAccessibilityGroupRole,
             Role::LayoutTableCell => NSAccessibilityGroupRole,
             Role::LayoutTableRow => NSAccessibilityGroupRole,
             Role::LayoutTable => NSAccessibilityGroupRole,
             Role::Switch => NSAccessibilityCheckBoxRole,
-            Role::ToggleButton => NSAccessibilityCheckBoxRole,
             Role::Menu => NSAccessibilityMenuRole,
             Role::MultilineTextInput => NSAccessibilityTextAreaRole,
             Role::DateInput | Role::DateTimeInput | Role::WeekInput | Role::MonthInput => {
                 ns_string!("AXDateField")
             }
             Role::TimeInput => ns_string!("AXTimeField"),
             Role::Abbr => NSAccessibilityGroupRole,
@@ -274,31 +276,38 @@
     fn node_value(&self) -> Option<String> {
         match self {
             Self::Node(node) => node.value(),
             Self::DetachedNode(node) => node.value(),
         }
     }
 
-    // TODO: implement proper logic for title, description, and value;
+    // TODO: implement proper logic for title and value;
     // see Chromium's content/browser/accessibility/browser_accessibility_cocoa.mm
     // and figure out how this is different in the macOS 10.10+ protocol
 
     pub(crate) fn title(&self) -> Option<String> {
         let state = self.node_state();
         if state.role() == Role::StaticText && state.raw_value().is_none() {
             // In this case, macOS wants the text to be the value, not title.
             return None;
         }
         self.name()
     }
 
+    pub(crate) fn description(&self) -> Option<String> {
+        match self {
+            Self::Node(node) => node.description(),
+            Self::DetachedNode(node) => node.description(),
+        }
+    }
+
     pub(crate) fn value(&self) -> Option<Value> {
         let state = self.node_state();
-        if let Some(checked) = state.checked() {
-            return Some(Value::Bool(checked != Checked::False));
+        if let Some(toggled) = state.toggled() {
+            return Some(Value::Bool(toggled != Toggled::False));
         }
         if let Some(value) = self.node_value() {
             return Some(Value::String(value));
         }
         if let Some(value) = state.numeric_value() {
             return Some(Value::Number(value));
         }
@@ -416,14 +425,23 @@
             self.resolve(|node| {
                 let wrapper = NodeWrapper::Node(node);
                 wrapper.title().map(|title| NSString::from_str(&title))
             })
             .flatten()
         }
 
+        #[method_id(accessibilityHelp)]
+        fn description(&self) -> Option<Id<NSString>> {
+            self.resolve(|node| {
+                let wrapper = NodeWrapper::Node(node);
+                wrapper.description().map(|description| NSString::from_str(&description))
+            })
+            .flatten()
+        }
+
         #[method_id(accessibilityValue)]
         fn value(&self) -> Option<Id<NSObject>> {
             self.resolve(|node| {
                 let wrapper = NodeWrapper::Node(node);
                 wrapper.value().map(|value| match value {
                     Value::Bool(value) => {
                         Id::into_super(Id::into_super(NSNumber::new_bool(value)))
@@ -754,14 +772,15 @@
                 selector == sel!(accessibilityParent)
                     || selector == sel!(accessibilityChildren)
                     || selector == sel!(accessibilityChildrenInNavigationOrder)
                     || selector == sel!(accessibilityFrame)
                     || selector == sel!(accessibilityRole)
                     || selector == sel!(accessibilityRoleDescription)
                     || selector == sel!(accessibilityTitle)
+                    || selector == sel!(accessibilityHelp)
                     || selector == sel!(accessibilityValue)
                     || selector == sel!(accessibilityMinValue)
                     || selector == sel!(accessibilityMaxValue)
                     || selector == sel!(isAccessibilityElement)
                     || selector == sel!(isAccessibilityFocused)
                     || selector == sel!(accessibilityNotifiesWhenDestroyed)
                     || selector == sel!(isAccessibilitySelectorAllowed:)
```

### Comparing `accesskit-0.2.0/platforms/macos/src/patch.rs` & `accesskit-0.3.0/platforms/macos/src/patch.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 // Copyright 2023 The AccessKit Authors. All rights reserved.
 // Licensed under the Apache License, Version 2.0 (found in
 // the LICENSE-APACHE file) or the MIT license (found in
 // the LICENSE-MIT file), at your option.
 
-use icrate::AppKit::NSWindow;
 use objc2::{
     encode::{Encode, EncodeArguments, EncodeReturn, Encoding},
     ffi::class_addMethod,
     msg_send,
     runtime::{AnyClass, AnyObject, Bool, MethodImplementation, Sel},
     sel, Message,
 };
+use objc2_app_kit::NSWindow;
 use std::{ffi::CString, ptr::null_mut};
 
 extern "C" fn focus_forwarder(this: &NSWindow, _cmd: Sel) -> *mut AnyObject {
     unsafe {
         this.contentView().map_or_else(null_mut, |view| {
             msg_send![&*view, accessibilityFocusedUIElement]
         })
```

### Comparing `accesskit-0.2.0/platforms/macos/src/subclass.rs` & `accesskit-0.3.0/platforms/macos/src/subclass.rs`

 * *Files identical despite different names*

```diff
@@ -1,30 +1,28 @@
 // Copyright 2022 The AccessKit Authors. All rights reserved.
 // Licensed under the Apache License, Version 2.0 (found in
 // the LICENSE-APACHE file) or the MIT license (found in
 // the LICENSE-MIT file), at your option.
 
 use accesskit::{ActionHandler, ActivationHandler, TreeUpdate};
-use icrate::{
-    AppKit::{NSView, NSWindow},
-    Foundation::{NSArray, NSObject, NSPoint},
-};
 use objc2::{
     declare::ClassBuilder,
     declare_class,
     ffi::{
         objc_getAssociatedObject, objc_setAssociatedObject, object_setClass,
         OBJC_ASSOCIATION_RETAIN_NONATOMIC,
     },
     msg_send_id,
     mutability::InteriorMutable,
     rc::Id,
     runtime::{AnyClass, Sel},
     sel, ClassType, DeclaredClass,
 };
+use objc2_app_kit::{NSView, NSWindow};
+use objc2_foundation::{NSArray, NSObject, NSPoint};
 use once_cell::sync::Lazy;
 use std::{cell::RefCell, collections::HashMap, ffi::c_void, sync::Mutex};
 
 use crate::{event::QueuedEvents, Adapter};
 
 static SUBCLASSES: Lazy<Mutex<HashMap<&'static AnyClass, &'static AnyClass>>> =
     Lazy::new(|| Mutex::new(HashMap::new()));
@@ -113,15 +111,15 @@
     let mut state = associated.ivars().state.borrow_mut();
     let state_mut = &mut *state;
     state_mut
         .adapter
         .hit_test(point, &mut *state_mut.activation_handler)
 }
 
-/// Uses dynamic Objective-C subclassing to implement the NSView
+/// Uses dynamic Objective-C subclassing to implement the `NSView`
 /// accessibility methods when normal subclassing isn't an option.
 pub struct SubclassingAdapter {
     view: Id<NSView>,
     associated: Id<AssociatedObject>,
 }
 
 impl SubclassingAdapter {
```

### Comparing `accesskit-0.2.0/platforms/macos/src/util.rs` & `accesskit-0.3.0/platforms/macos/src/util.rs`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 // Copyright 2022 The AccessKit Authors. All rights reserved.
 // Licensed under the Apache License, Version 2.0 (found in
 // the LICENSE-APACHE file) or the MIT license (found in
 // the LICENSE-MIT file), at your option.
 
 use accesskit::{Point, Rect};
 use accesskit_consumer::{Node, TextPosition, TextRange};
-use icrate::{
-    AppKit::*,
-    Foundation::{NSPoint, NSRange, NSRect, NSSize},
-};
+use objc2_app_kit::*;
+use objc2_foundation::{NSPoint, NSRange, NSRect, NSSize};
 
 pub(crate) fn from_ns_range<'a>(node: &'a Node<'a>, ns_range: NSRange) -> Option<TextRange<'a>> {
     let pos = node.text_position_from_global_utf16_index(ns_range.location)?;
     let mut range = pos.to_degenerate_range();
     if ns_range.length > 0 {
         let end =
             node.text_position_from_global_utf16_index(ns_range.location + ns_range.length)?;
@@ -33,22 +31,22 @@
         range.set_end(pos.forward_to_character_end());
     }
     to_ns_range(&range)
 }
 
 pub(crate) fn from_ns_point(view: &NSView, node: &Node, point: NSPoint) -> Point {
     let window = view.window().unwrap();
-    let point = unsafe { window.convertPointFromScreen(point) };
+    let point = window.convertPointFromScreen(point);
     let point = view.convertPoint_fromView(point, None);
     // AccessKit coordinates are in physical (DPI-dependent) pixels, but
     // macOS provides logical (DPI-independent) coordinates here.
     let factor = window.backingScaleFactor();
     let point = Point::new(
         point.x * factor,
-        if unsafe { view.isFlipped() } {
+        if view.isFlipped() {
             point.y * factor
         } else {
             let view_bounds = view.bounds();
             (view_bounds.size.height - point.y) * factor
         },
     );
     node.transform().inverse() * point
@@ -59,23 +57,23 @@
     // AccessKit coordinates are in physical (DPI-dependent)
     // pixels, but macOS expects logical (DPI-independent)
     // coordinates here.
     let factor = window.backingScaleFactor();
     let rect = NSRect {
         origin: NSPoint {
             x: rect.x0 / factor,
-            y: if unsafe { view.isFlipped() } {
+            y: if view.isFlipped() {
                 rect.y0 / factor
             } else {
                 let view_bounds = view.bounds();
                 view_bounds.size.height - rect.y1 / factor
             },
         },
         size: NSSize {
             width: rect.width() / factor,
             height: rect.height() / factor,
         },
     };
-    let rect = unsafe { view.convertRect_toView(rect, None) };
+    let rect = view.convertRect_toView(rect, None);
     let window = view.window().unwrap();
-    unsafe { window.convertRectToScreen(rect) }
+    window.convertRectToScreen(rect)
 }
```

### Comparing `accesskit-0.2.0/platforms/atspi-common/Cargo.toml` & `accesskit-0.3.0/platforms/atspi-common/Cargo.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [package]
 name = "accesskit_atspi_common"
-version = "0.3.0"
+version = "0.4.0"
 authors.workspace = true
 license.workspace = true
 description = "AccessKit UI accessibility infrastructure: core AT-SPI translation layer"
 categories.workspace = true
 keywords = ["gui", "ui", "accessibility"]
 repository.workspace = true
 readme = "README.md"
 edition.workspace = true
 rust-version.workspace = true
 
 [dependencies]
-accesskit = { version = "0.13.0", path = "../../common" }
-accesskit_consumer = { version = "0.18.0", path = "../../consumer" }
+accesskit = { version = "0.14.0", path = "../../common" }
+accesskit_consumer = { version = "0.19.0", path = "../../consumer" }
 atspi-common = { version = "0.3.0", default-features = false }
 serde = "1.0"
 thiserror = "1.0.39"
 zvariant = { version = "3", default-features = false }
+
```

### Comparing `accesskit-0.2.0/platforms/atspi-common/CHANGELOG.md` & `accesskit-0.3.0/platforms/atspi-common/CHANGELOG.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,45 @@
 # Changelog
 
 * The following workspace dependencies were updated
   * dependencies
     * accesskit bumped from 0.12.2 to 0.12.3
     * accesskit_consumer bumped from 0.17.0 to 0.17.1
 
+## [0.4.0](https://github.com/AccessKit/accesskit/compare/accesskit_atspi_common-v0.3.0...accesskit_atspi_common-v0.4.0) (2024-04-30)
+
+
+### ⚠ BREAKING CHANGES
+
+* Clean up table roles and properties ([#393](https://github.com/AccessKit/accesskit/issues/393))
+* Rename `Checked` to `Toggled`; drop `ToggleButton` role ([#388](https://github.com/AccessKit/accesskit/issues/388))
+
+### Features
+
+* Implement the `description` property ([#382](https://github.com/AccessKit/accesskit/issues/382)) ([d49f406](https://github.com/AccessKit/accesskit/commit/d49f40660b5dc23ed074cd72a91e511b130756ae))
+
+
+### Bug Fixes
+
+* Increase minimum supported Rust version to `1.70` ([#396](https://github.com/AccessKit/accesskit/issues/396)) ([a8398b8](https://github.com/AccessKit/accesskit/commit/a8398b847aa003de91042ac45e33126fc2cae053))
+
+
+### Code Refactoring
+
+* Clean up table roles and properties ([#393](https://github.com/AccessKit/accesskit/issues/393)) ([e34dad9](https://github.com/AccessKit/accesskit/commit/e34dad94448a5321ece9def3f2e054aa5f62dd79))
+* Rename `Checked` to `Toggled`; drop `ToggleButton` role ([#388](https://github.com/AccessKit/accesskit/issues/388)) ([6bc040b](https://github.com/AccessKit/accesskit/commit/6bc040b7cf75cdbd6a019cc380d8dbce804b3c81))
+
+
+### Dependencies
+
+* The following workspace dependencies were updated
+  * dependencies
+    * accesskit bumped from 0.13.0 to 0.14.0
+    * accesskit_consumer bumped from 0.18.0 to 0.19.0
+
 ## [0.3.0](https://github.com/AccessKit/accesskit/compare/accesskit_atspi_common-v0.2.0...accesskit_atspi_common-v0.3.0) (2024-04-14)
 
 
 ### ⚠ BREAKING CHANGES
 
 * New approach to lazy initialization ([#375](https://github.com/AccessKit/accesskit/issues/375))
```

### Comparing `accesskit-0.2.0/platforms/atspi-common/src/adapter.rs` & `accesskit-0.3.0/platforms/atspi-common/src/adapter.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.2.0/platforms/atspi-common/src/callback.rs` & `accesskit-0.3.0/platforms/atspi-common/src/callback.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.2.0/platforms/atspi-common/src/context.rs` & `accesskit-0.3.0/platforms/atspi-common/src/context.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.2.0/platforms/atspi-common/src/error.rs` & `accesskit-0.3.0/platforms/atspi-common/src/error.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.2.0/platforms/atspi-common/src/events.rs` & `accesskit-0.3.0/platforms/atspi-common/src/events.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.2.0/platforms/atspi-common/src/lib.rs` & `accesskit-0.3.0/platforms/atspi-common/src/lib.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.2.0/platforms/atspi-common/src/node.rs` & `accesskit-0.3.0/platforms/atspi-common/src/node.rs`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 // Derived from Chromium's accessibility abstraction.
 // Copyright 2017 The Chromium Authors. All rights reserved.
 // Use of this source code is governed by a BSD-style license that can be
 // found in the LICENSE.chromium file.
 
 use accesskit::{
-    Action, ActionData, ActionRequest, Affine, Checked, DefaultActionVerb, Live, NodeId, Point,
-    Rect, Role,
+    Action, ActionData, ActionRequest, Affine, DefaultActionVerb, Live, NodeId, Point, Rect, Role,
+    Toggled,
 };
 use accesskit_consumer::{DetachedNode, FilterResult, Node, NodeState, TreeState};
 use atspi_common::{
     CoordType, Interface, InterfaceSet, Layer, Live as AtspiLive, Role as AtspiRole, State,
     StateSet,
 };
 use std::{
@@ -47,16 +47,19 @@
     pub fn name(&self) -> Option<String> {
         match self {
             Self::Node(node) => node.name(),
             Self::DetachedNode(node) => node.name(),
         }
     }
 
-    pub fn description(&self) -> String {
-        String::new()
+    pub(crate) fn description(&self) -> Option<String> {
+        match self {
+            Self::Node(node) => node.description(),
+            Self::DetachedNode(node) => node.description(),
+        }
     }
 
     pub fn parent_id(&self) -> Option<NodeId> {
         self.node_state().parent_id()
     }
 
     pub fn id(&self) -> NodeId {
@@ -93,22 +96,28 @@
             // TODO: See how to represent ARIA role="application"
             Role::Application => AtspiRole::Embedded,
             Role::Article => AtspiRole::Article,
             Role::Audio => AtspiRole::Audio,
             Role::Banner | Role::Header => AtspiRole::Landmark,
             Role::Blockquote => AtspiRole::BlockQuote,
             Role::Caret => AtspiRole::Unknown,
-            Role::Button | Role::DefaultButton => AtspiRole::PushButton,
+            Role::Button => {
+                if self.node_state().toggled().is_some() {
+                    AtspiRole::ToggleButton
+                } else {
+                    AtspiRole::PushButton
+                }
+            }
+            Role::DefaultButton => AtspiRole::PushButton,
             Role::Canvas => AtspiRole::Canvas,
             Role::Caption => AtspiRole::Caption,
             Role::Cell => AtspiRole::TableCell,
             Role::CheckBox => AtspiRole::CheckBox,
             Role::Switch => AtspiRole::ToggleButton,
             Role::ColorWell => AtspiRole::PushButton,
-            Role::Column => AtspiRole::Unknown,
             Role::ColumnHeader => AtspiRole::ColumnHeader,
             Role::ComboBox | Role::EditableComboBox => AtspiRole::ComboBox,
             Role::Complementary => AtspiRole::Landmark,
             Role::ContentDeletion => AtspiRole::ContentDeletion,
             Role::ContentInsertion => AtspiRole::ContentInsertion,
             Role::ContentInfo | Role::Footer => AtspiRole::Landmark,
             Role::Definition | Role::DescriptionListDetail => AtspiRole::DescriptionValue,
@@ -245,18 +254,14 @@
             Role::SpinButton => AtspiRole::SpinButton,
             Role::Splitter => AtspiRole::Separator,
             Role::StaticText => AtspiRole::Static,
             Role::Status => AtspiRole::StatusBar,
             Role::SvgRoot => AtspiRole::DocumentFrame,
             Role::Tab => AtspiRole::PageTab,
             Role::Table => AtspiRole::Table,
-            // TODO: This mapping is correct, but it doesn't seem to be
-            // used. We don't necessarily want to always expose these containers, but
-            // we must do so if they are focusable.
-            Role::TableHeaderContainer => AtspiRole::Panel,
             Role::TabList => AtspiRole::PageTabList,
             Role::TabPanel => AtspiRole::ScrollPane,
             // TODO: This mapping should also be applied to the dfn
             // element.
             Role::Term => AtspiRole::DescriptionTerm,
             Role::TitleBar => AtspiRole::TitleBar,
             Role::TextInput
@@ -272,15 +277,14 @@
             | Role::MonthInput
             | Role::TimeInput => AtspiRole::DateEditor,
             Role::PasswordInput => AtspiRole::PasswordText,
             Role::Abbr | Role::Code | Role::Emphasis | Role::Strong | Role::Time => {
                 AtspiRole::Static
             }
             Role::Timer => AtspiRole::Timer,
-            Role::ToggleButton => AtspiRole::ToggleButton,
             Role::Toolbar => AtspiRole::ToolBar,
             Role::Tooltip => AtspiRole::ToolTip,
             Role::Tree => AtspiRole::Tree,
             Role::TreeItem => AtspiRole::TreeItem,
             Role::TreeGrid => AtspiRole::TreeTable,
             Role::Video => AtspiRole::Video,
             // In AT-SPI, elements with `AtspiRole::Frame` are windows with titles and
@@ -317,15 +321,15 @@
         let filter_result = match self {
             Self::Node(node) => filter(node),
             Self::DetachedNode(node) => filter_detached(node),
         };
         if filter_result == FilterResult::Include {
             atspi_state.insert(State::Visible | State::Showing);
         }
-        if atspi_role != AtspiRole::ToggleButton && state.checked().is_some() {
+        if atspi_role != AtspiRole::ToggleButton && state.toggled().is_some() {
             atspi_state.insert(State::Checkable);
         }
         if let Some(selected) = state.is_selected() {
             if !state.is_disabled() {
                 atspi_state.insert(State::Selectable);
             }
             if selected {
@@ -341,21 +345,21 @@
         }
 
         // Special case for indeterminate progressbar.
         if state.role() == Role::ProgressIndicator && state.numeric_value().is_none() {
             atspi_state.insert(State::Indeterminate);
         }
 
-        // Checked state
-        match state.checked() {
-            Some(Checked::Mixed) => atspi_state.insert(State::Indeterminate),
-            Some(Checked::True) if atspi_role == AtspiRole::ToggleButton => {
+        // Toggled state
+        match state.toggled() {
+            Some(Toggled::Mixed) => atspi_state.insert(State::Indeterminate),
+            Some(Toggled::True) if atspi_role == AtspiRole::ToggleButton => {
                 atspi_state.insert(State::Pressed)
             }
-            Some(Checked::True) => atspi_state.insert(State::Checked),
+            Some(Toggled::True) => atspi_state.insert(State::Checked),
             _ => {}
         }
 
         if state.is_read_only_supported() && state.is_read_only_or_disabled() {
             atspi_state.insert(State::ReadOnly);
         } else {
             atspi_state.insert(State::Enabled | State::Sensitive);
@@ -507,15 +511,17 @@
                 adapter.emit_object_event(self.id(), ObjectEvent::Announcement(name, live));
             }
         }
         let description = self.description();
         if description != old.description() {
             adapter.emit_object_event(
                 self.id(),
-                ObjectEvent::PropertyChanged(Property::Description(description)),
+                ObjectEvent::PropertyChanged(Property::Description(
+                    description.unwrap_or_default(),
+                )),
             );
         }
         let parent_id = self.parent_id();
         if parent_id != old.parent_id() {
             let node = match self {
                 NodeWrapper::Node(node) => node,
                 _ => unreachable!(),
@@ -664,15 +670,15 @@
             Ok(wrapper.name().unwrap_or_default())
         })
     }
 
     pub fn description(&self) -> Result<String> {
         self.resolve(|node| {
             let wrapper = NodeWrapper::Node(&node);
-            Ok(wrapper.description())
+            Ok(wrapper.description().unwrap_or_default())
         })
     }
 
     pub fn relative(&self, id: NodeId) -> Self {
         Self {
             context: self.context.clone(),
             adapter_id: self.adapter_id,
@@ -931,19 +937,19 @@
                 data: Some(ActionData::ScrollToPoint(point)),
             }
         })?;
         Ok(true)
     }
 
     pub fn minimum_value(&self) -> Result<f64> {
-        self.resolve(|node| Ok(node.state().min_numeric_value().unwrap_or(std::f64::MIN)))
+        self.resolve(|node| Ok(node.state().min_numeric_value().unwrap_or(f64::MIN)))
     }
 
     pub fn maximum_value(&self) -> Result<f64> {
-        self.resolve(|node| Ok(node.state().max_numeric_value().unwrap_or(std::f64::MAX)))
+        self.resolve(|node| Ok(node.state().max_numeric_value().unwrap_or(f64::MAX)))
     }
 
     pub fn minimum_increment(&self) -> Result<f64> {
         self.resolve(|node| Ok(node.state().numeric_value_step().unwrap_or(0.0)))
     }
 
     pub fn current_value(&self) -> Result<f64> {
```

### Comparing `accesskit-0.2.0/platforms/atspi-common/src/rect.rs` & `accesskit-0.3.0/platforms/atspi-common/src/rect.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.2.0/platforms/atspi-common/src/simplified.rs` & `accesskit-0.3.0/platforms/atspi-common/src/simplified.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.2.0/platforms/atspi-common/src/util.rs` & `accesskit-0.3.0/platforms/atspi-common/src/util.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.2.0/consumer/CHANGELOG.md` & `accesskit-0.3.0/consumer/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,45 @@
   * dependencies
     * accesskit bumped from 0.11.1 to 0.11.2
 
 * The following workspace dependencies were updated
   * dependencies
     * accesskit bumped from 0.12.2 to 0.12.3
 
+## [0.19.0](https://github.com/AccessKit/accesskit/compare/accesskit_consumer-v0.18.0...accesskit_consumer-v0.19.0) (2024-04-30)
+
+
+### ⚠ BREAKING CHANGES
+
+* Drop `NodeClassSet` ([#389](https://github.com/AccessKit/accesskit/issues/389))
+* Rename `Checked` to `Toggled`; drop `ToggleButton` role ([#388](https://github.com/AccessKit/accesskit/issues/388))
+
+### Features
+
+* Expose the class name property ([#385](https://github.com/AccessKit/accesskit/issues/385)) ([53dcf2a](https://github.com/AccessKit/accesskit/commit/53dcf2ae47546273590c46a9b31b708aa1409837))
+* Implement the `description` property ([#382](https://github.com/AccessKit/accesskit/issues/382)) ([d49f406](https://github.com/AccessKit/accesskit/commit/d49f40660b5dc23ed074cd72a91e511b130756ae))
+
+
+### Bug Fixes
+
+* Increase minimum supported Rust version to `1.70` ([#396](https://github.com/AccessKit/accesskit/issues/396)) ([a8398b8](https://github.com/AccessKit/accesskit/commit/a8398b847aa003de91042ac45e33126fc2cae053))
+
+
+### Code Refactoring
+
+* Drop `NodeClassSet` ([#389](https://github.com/AccessKit/accesskit/issues/389)) ([1b153ed](https://github.com/AccessKit/accesskit/commit/1b153ed51f8421cdba2dc98beca2e8f5f8c781bc))
+* Rename `Checked` to `Toggled`; drop `ToggleButton` role ([#388](https://github.com/AccessKit/accesskit/issues/388)) ([6bc040b](https://github.com/AccessKit/accesskit/commit/6bc040b7cf75cdbd6a019cc380d8dbce804b3c81))
+
+
+### Dependencies
+
+* The following workspace dependencies were updated
+  * dependencies
+    * accesskit bumped from 0.13.0 to 0.14.0
+
 ## [0.18.0](https://github.com/AccessKit/accesskit/compare/accesskit_consumer-v0.17.1...accesskit_consumer-v0.18.0) (2024-04-14)
 
 
 ### ⚠ BREAKING CHANGES
 
 * New approach to lazy initialization ([#375](https://github.com/AccessKit/accesskit/issues/375))
```

### Comparing `accesskit-0.2.0/consumer/src/filters.rs` & `accesskit-0.3.0/consumer/src/filters.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.2.0/consumer/src/iterators.rs` & `accesskit-0.3.0/consumer/src/iterators.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.2.0/consumer/src/lib.rs` & `accesskit-0.3.0/consumer/src/lib.rs`

 * *Files 9% similar despite different names*

```diff
@@ -20,17 +20,15 @@
 pub use text::{
     AttributeValue as TextAttributeValue, Position as TextPosition, Range as TextRange,
     WeakRange as WeakTextRange,
 };
 
 #[cfg(test)]
 mod tests {
-    use accesskit::{
-        Affine, NodeBuilder, NodeClassSet, NodeId, Rect, Role, Tree, TreeUpdate, Vec2,
-    };
+    use accesskit::{Affine, NodeBuilder, NodeId, Rect, Role, Tree, TreeUpdate, Vec2};
 
     use crate::FilterResult;
 
     pub const ROOT_ID: NodeId = NodeId(0);
     pub const PARAGRAPH_0_ID: NodeId = NodeId(1);
     pub const STATIC_TEXT_0_0_IGNORED_ID: NodeId = NodeId(2);
     pub const PARAGRAPH_1_IGNORED_ID: NodeId = NodeId(3);
@@ -41,98 +39,95 @@
     pub const EMPTY_CONTAINER_3_0_IGNORED_ID: NodeId = NodeId(8);
     pub const LINK_3_1_IGNORED_ID: NodeId = NodeId(9);
     pub const STATIC_TEXT_3_1_0_ID: NodeId = NodeId(10);
     pub const BUTTON_3_2_ID: NodeId = NodeId(11);
     pub const EMPTY_CONTAINER_3_3_IGNORED_ID: NodeId = NodeId(12);
 
     pub fn test_tree() -> crate::tree::Tree {
-        let mut classes = NodeClassSet::new();
         let root = {
             let mut builder = NodeBuilder::new(Role::RootWebArea);
             builder.set_children(vec![
                 PARAGRAPH_0_ID,
                 PARAGRAPH_1_IGNORED_ID,
                 PARAGRAPH_2_ID,
                 PARAGRAPH_3_IGNORED_ID,
             ]);
-            builder.build(&mut classes)
+            builder.build()
         };
         let paragraph_0 = {
             let mut builder = NodeBuilder::new(Role::Paragraph);
             builder.set_children(vec![STATIC_TEXT_0_0_IGNORED_ID]);
-            builder.build(&mut classes)
+            builder.build()
         };
         let static_text_0_0_ignored = {
             let mut builder = NodeBuilder::new(Role::StaticText);
             builder.set_name("static_text_0_0_ignored");
-            builder.build(&mut classes)
+            builder.build()
         };
         let paragraph_1_ignored = {
             let mut builder = NodeBuilder::new(Role::Paragraph);
             builder.set_transform(Affine::translate(Vec2::new(10.0, 40.0)));
             builder.set_bounds(Rect {
                 x0: 0.0,
                 y0: 0.0,
                 x1: 800.0,
                 y1: 40.0,
             });
             builder.set_children(vec![STATIC_TEXT_1_0_ID]);
-            builder.build(&mut classes)
+            builder.build()
         };
         let static_text_1_0 = {
             let mut builder = NodeBuilder::new(Role::StaticText);
             builder.set_bounds(Rect {
                 x0: 10.0,
                 y0: 10.0,
                 x1: 90.0,
                 y1: 30.0,
             });
             builder.set_name("static_text_1_0");
-            builder.build(&mut classes)
+            builder.build()
         };
         let paragraph_2 = {
             let mut builder = NodeBuilder::new(Role::Paragraph);
             builder.set_children(vec![STATIC_TEXT_2_0_ID]);
-            builder.build(&mut classes)
+            builder.build()
         };
         let static_text_2_0 = {
             let mut builder = NodeBuilder::new(Role::StaticText);
             builder.set_name("static_text_2_0");
-            builder.build(&mut classes)
+            builder.build()
         };
         let paragraph_3_ignored = {
             let mut builder = NodeBuilder::new(Role::Paragraph);
             builder.set_children(vec![
                 EMPTY_CONTAINER_3_0_IGNORED_ID,
                 LINK_3_1_IGNORED_ID,
                 BUTTON_3_2_ID,
                 EMPTY_CONTAINER_3_3_IGNORED_ID,
             ]);
-            builder.build(&mut classes)
+            builder.build()
         };
-        let empty_container_3_0_ignored =
-            NodeBuilder::new(Role::GenericContainer).build(&mut classes);
+        let empty_container_3_0_ignored = NodeBuilder::new(Role::GenericContainer).build();
         let link_3_1_ignored = {
             let mut builder = NodeBuilder::new(Role::Link);
             builder.set_children(vec![STATIC_TEXT_3_1_0_ID]);
             builder.set_linked();
-            builder.build(&mut classes)
+            builder.build()
         };
         let static_text_3_1_0 = {
             let mut builder = NodeBuilder::new(Role::StaticText);
             builder.set_name("static_text_3_1_0");
-            builder.build(&mut classes)
+            builder.build()
         };
         let button_3_2 = {
             let mut builder = NodeBuilder::new(Role::Button);
             builder.set_name("button_3_2");
-            builder.build(&mut classes)
+            builder.build()
         };
-        let empty_container_3_3_ignored =
-            NodeBuilder::new(Role::GenericContainer).build(&mut classes);
+        let empty_container_3_3_ignored = NodeBuilder::new(Role::GenericContainer).build();
         let initial_update = TreeUpdate {
             nodes: vec![
                 (ROOT_ID, root),
                 (PARAGRAPH_0_ID, paragraph_0),
                 (STATIC_TEXT_0_0_IGNORED_ID, static_text_0_0_ignored),
                 (PARAGRAPH_1_IGNORED_ID, paragraph_1_ignored),
                 (STATIC_TEXT_1_0_ID, static_text_1_0),
```

### Comparing `accesskit-0.2.0/consumer/src/node.rs` & `accesskit-0.3.0/consumer/src/node.rs`

 * *Files 5% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 // the LICENSE-MIT file), at your option.
 
 // Derived from Chromium's accessibility abstraction.
 // Copyright 2021 The Chromium Authors. All rights reserved.
 // Use of this source code is governed by a BSD-style license that can be
 // found in the LICENSE.chromium file.
 
-use std::{iter::FusedIterator, ops::Deref};
+use std::{iter::FusedIterator, ops::Deref, sync::Arc};
 
 use accesskit::{
-    Action, Affine, Checked, DefaultActionVerb, Live, Node as NodeData, NodeId, Point, Rect, Role,
-    TextSelection,
+    Action, Affine, DefaultActionVerb, Live, Node as NodeData, NodeId, Point, Rect, Role,
+    TextSelection, Toggled,
 };
 
 use crate::filters::FilterResult;
 use crate::iterators::{
     FilteredChildren, FollowingFilteredSiblings, FollowingSiblings, LabelledBy,
     PrecedingFilteredSiblings, PrecedingSiblings,
 };
@@ -25,15 +25,15 @@
 #[derive(Clone, Copy, PartialEq, Eq)]
 pub(crate) struct ParentAndIndex(pub(crate) NodeId, pub(crate) usize);
 
 #[derive(Clone)]
 pub struct NodeState {
     pub(crate) id: NodeId,
     pub(crate) parent_and_index: Option<ParentAndIndex>,
-    pub(crate) data: NodeData,
+    pub(crate) data: Arc<NodeData>,
 }
 
 #[derive(Copy, Clone)]
 pub struct Node<'a> {
     pub tree_state: &'a TreeState,
     pub(crate) state: &'a NodeState,
 }
@@ -47,14 +47,15 @@
 impl<'a> Node<'a> {
     pub fn detached(&self) -> DetachedNode {
         DetachedNode {
             state: self.state.clone(),
             is_focused: self.is_focused(),
             is_root: self.is_root(),
             name: self.name(),
+            description: self.description(),
             value: self.value(),
             live: self.live(),
             supports_text_ranges: self.supports_text_ranges(),
         }
     }
 
     pub fn is_focused(&self) -> bool {
@@ -379,16 +380,16 @@
         }
     }
 
     pub fn is_read_only_or_disabled(&self) -> bool {
         self.is_read_only() || self.is_disabled()
     }
 
-    pub fn checked(&self) -> Option<Checked> {
-        self.data().checked()
+    pub fn toggled(&self) -> Option<Toggled> {
+        self.data().toggled()
     }
 
     pub fn numeric_value(&self) -> Option<f64> {
         self.data().numeric_value()
     }
 
     pub fn min_numeric_value(&self) -> Option<f64> {
@@ -456,15 +457,15 @@
             }
         }
 
         false
     }
 
     pub fn supports_toggle(&self) -> bool {
-        self.checked().is_some()
+        self.toggled().is_some()
     }
 
     pub fn supports_expand_collapse(&self) -> bool {
         self.data().is_expanded().is_some()
     }
 
     pub fn is_invocable(&self) -> bool {
@@ -537,14 +538,20 @@
                 .labelled_by()
                 .filter_map(|node| node.name())
                 .collect::<Vec<String>>();
             (!names.is_empty()).then(move || names.join(" "))
         }
     }
 
+    pub fn description(&self) -> Option<String> {
+        self.data()
+            .description()
+            .map(|description| description.to_string())
+    }
+
     pub fn value(&self) -> Option<String> {
         if let Some(value) = &self.data().value() {
             Some(value.to_string())
         } else if self.supports_text_ranges() && !self.is_multiline() {
             Some(self.document_range().text())
         } else {
             None
@@ -569,15 +576,14 @@
                     | Role::MenuItemCheckBox
                     | Role::MenuItemRadio
                     | Role::MenuListPopup
                     | Role::RadioButton
                     | Role::RadioGroup
                     | Role::Slider
                     | Role::Switch
-                    | Role::ToggleButton
                     | Role::TreeGrid
             )
     }
 
     pub fn should_have_read_only_state_by_default(&self) -> bool {
         matches!(
             self.role(),
@@ -618,14 +624,18 @@
     pub fn raw_text_selection(&self) -> Option<&TextSelection> {
         self.data().text_selection()
     }
 
     pub fn raw_value(&self) -> Option<&str> {
         self.data().value()
     }
+
+    pub fn class_name(&self) -> Option<&str> {
+        self.data().class_name()
+    }
 }
 
 impl<'a> Node<'a> {
     pub fn index_path(&self) -> Vec<usize> {
         self.relative_index_path(self.tree_state.root_id())
     }
 
@@ -692,14 +702,15 @@
 
 #[derive(Clone)]
 pub struct DetachedNode {
     pub(crate) state: NodeState,
     pub(crate) is_focused: bool,
     pub(crate) is_root: bool,
     pub(crate) name: Option<String>,
+    pub(crate) description: Option<String>,
     pub(crate) value: Option<String>,
     pub(crate) live: Live,
     pub(crate) supports_text_ranges: bool,
 }
 
 impl DetachedNode {
     pub fn is_focused(&self) -> bool {
@@ -710,14 +721,18 @@
         self.is_root
     }
 
     pub fn name(&self) -> Option<String> {
         self.name.clone()
     }
 
+    pub fn description(&self) -> Option<String> {
+        self.description.clone()
+    }
+
     pub fn value(&self) -> Option<String> {
         self.value.clone()
     }
 
     pub fn has_value(&self) -> bool {
         self.value.is_some()
     }
@@ -741,15 +756,15 @@
     fn deref(&self) -> &NodeState {
         &self.state
     }
 }
 
 #[cfg(test)]
 mod tests {
-    use accesskit::{NodeBuilder, NodeClassSet, NodeId, Point, Rect, Role, Tree, TreeUpdate};
+    use accesskit::{NodeBuilder, NodeId, Point, Rect, Role, Tree, TreeUpdate};
 
     use crate::tests::*;
 
     #[test]
     fn parent_and_index() {
         let tree = test_tree();
         assert!(tree.state().root().parent_and_index().is_none());
@@ -1004,26 +1019,22 @@
             .root()
             .node_at_point(Point::new(100.0, 70.0), &test_tree_filter)
             .is_none());
     }
 
     #[test]
     fn no_name_or_labelled_by() {
-        let mut classes = NodeClassSet::new();
         let update = TreeUpdate {
             nodes: vec![
                 (NodeId(0), {
                     let mut builder = NodeBuilder::new(Role::Window);
                     builder.set_children(vec![NodeId(1)]);
-                    builder.build(&mut classes)
+                    builder.build()
                 }),
-                (
-                    NodeId(1),
-                    NodeBuilder::new(Role::Button).build(&mut classes),
-                ),
+                (NodeId(1), NodeBuilder::new(Role::Button).build()),
             ],
             tree: Some(Tree::new(NodeId(0))),
             focus: NodeId(0),
         };
         let tree = crate::Tree::new(update, false);
         assert_eq!(None, tree.state().node_by_id(NodeId(1)).unwrap().name());
     }
@@ -1031,41 +1042,40 @@
     #[test]
     fn name_from_labelled_by() {
         // The following mock UI probably isn't very localization-friendly,
         // but it's good for this test.
         const LABEL_1: &str = "Check email every";
         const LABEL_2: &str = "minutes";
 
-        let mut classes = NodeClassSet::new();
         let update = TreeUpdate {
             nodes: vec![
                 (NodeId(0), {
                     let mut builder = NodeBuilder::new(Role::Window);
                     builder.set_children(vec![NodeId(1), NodeId(2), NodeId(3), NodeId(4)]);
-                    builder.build(&mut classes)
+                    builder.build()
                 }),
                 (NodeId(1), {
                     let mut builder = NodeBuilder::new(Role::CheckBox);
                     builder.set_labelled_by(vec![NodeId(2), NodeId(4)]);
-                    builder.build(&mut classes)
+                    builder.build()
                 }),
                 (NodeId(2), {
                     let mut builder = NodeBuilder::new(Role::StaticText);
                     builder.set_name(LABEL_1);
-                    builder.build(&mut classes)
+                    builder.build()
                 }),
                 (NodeId(3), {
                     let mut builder = NodeBuilder::new(Role::TextInput);
                     builder.push_labelled_by(NodeId(4));
-                    builder.build(&mut classes)
+                    builder.build()
                 }),
                 (NodeId(4), {
                     let mut builder = NodeBuilder::new(Role::StaticText);
                     builder.set_name(LABEL_2);
-                    builder.build(&mut classes)
+                    builder.build()
                 }),
             ],
             tree: Some(Tree::new(NodeId(0))),
             focus: NodeId(0),
         };
         let tree = crate::Tree::new(update, false);
         assert_eq!(
@@ -1079,46 +1089,45 @@
     }
 
     #[test]
     fn name_from_descendant_label() {
         const BUTTON_LABEL: &str = "Play";
         const LINK_LABEL: &str = "Watch in browser";
 
-        let mut classes = NodeClassSet::new();
         let update = TreeUpdate {
             nodes: vec![
                 (NodeId(0), {
                     let mut builder = NodeBuilder::new(Role::Window);
                     builder.set_children(vec![NodeId(1), NodeId(3)]);
-                    builder.build(&mut classes)
+                    builder.build()
                 }),
                 (NodeId(1), {
                     let mut builder = NodeBuilder::new(Role::Button);
                     builder.push_child(NodeId(2));
-                    builder.build(&mut classes)
+                    builder.build()
                 }),
                 (NodeId(2), {
                     let mut builder = NodeBuilder::new(Role::Image);
                     builder.set_name(BUTTON_LABEL);
-                    builder.build(&mut classes)
+                    builder.build()
                 }),
                 (NodeId(3), {
                     let mut builder = NodeBuilder::new(Role::Link);
                     builder.push_child(NodeId(4));
-                    builder.build(&mut classes)
+                    builder.build()
                 }),
                 (NodeId(4), {
                     let mut builder = NodeBuilder::new(Role::GenericContainer);
                     builder.push_child(NodeId(5));
-                    builder.build(&mut classes)
+                    builder.build()
                 }),
                 (NodeId(5), {
                     let mut builder = NodeBuilder::new(Role::StaticText);
                     builder.set_name(LINK_LABEL);
-                    builder.build(&mut classes)
+                    builder.build()
                 }),
             ],
             tree: Some(Tree::new(NodeId(0))),
             focus: NodeId(0),
         };
         let tree = crate::Tree::new(update, false);
         assert_eq!(
```

### Comparing `accesskit-0.2.0/consumer/src/text.rs` & `accesskit-0.3.0/consumer/src/text.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1027,26 +1027,23 @@
 
 #[cfg(test)]
 mod tests {
     use accesskit::{NodeId, Point, Rect, TextSelection};
 
     // This is based on an actual tree produced by egui.
     fn main_multiline_tree(selection: Option<TextSelection>) -> crate::Tree {
-        use accesskit::{
-            Action, Affine, NodeBuilder, NodeClassSet, Role, TextDirection, Tree, TreeUpdate,
-        };
+        use accesskit::{Action, Affine, NodeBuilder, Role, TextDirection, Tree, TreeUpdate};
 
-        let mut classes = NodeClassSet::new();
         let update = TreeUpdate {
             nodes: vec![
                 (NodeId(0), {
                     let mut builder = NodeBuilder::new(Role::Window);
                     builder.set_transform(Affine::scale(1.5));
                     builder.set_children(vec![NodeId(1)]);
-                    builder.build(&mut classes)
+                    builder.build()
                 }),
                 (NodeId(1), {
                     let mut builder = NodeBuilder::new(Role::MultilineTextInput);
                     builder.set_bounds(Rect {
                         x0: 8.0,
                         y0: 31.666664123535156,
                         x1: 296.0,
@@ -1060,15 +1057,15 @@
                         NodeId(6),
                         NodeId(7),
                     ]);
                     builder.add_action(Action::Focus);
                     if let Some(selection) = selection {
                         builder.set_text_selection(selection);
                     }
-                    builder.build(&mut classes)
+                    builder.build()
                 }),
                 (NodeId(2), {
                     let mut builder = NodeBuilder::new(Role::InlineTextBox);
                     builder.set_bounds(Rect {
                         x0: 12.0,
                         y0: 33.666664123535156,
                         x1: 290.9189147949219,
@@ -1095,15 +1092,15 @@
                         7.58557, 7.58557, 7.58557, 7.58557, 7.58557, 7.58557, 7.58557, 7.58557,
                         7.58557, 7.58557, 7.58557, 7.58557, 7.58557, 7.58557, 7.58557, 7.58557,
                         7.58557, 7.58557, 7.58557, 7.58557, 7.58557, 7.58557, 7.58557, 7.58557,
                         7.58557, 7.58557, 7.58557, 7.58557, 7.58557, 7.58557, 7.58557, 7.58557,
                         7.58557, 7.58557, 7.58557, 7.58557, 7.58557, 7.58557,
                     ]);
                     builder.set_word_lengths([5, 10, 3, 5, 7, 3, 5]);
-                    builder.build(&mut classes)
+                    builder.build()
                 }),
                 (NodeId(3), {
                     let mut builder = NodeBuilder::new(Role::InlineTextBox);
                     builder.set_bounds(Rect {
                         x0: 12.0,
                         y0: 48.33333206176758,
                         x1: 129.5855712890625,
@@ -1120,15 +1117,15 @@
                     ]);
                     builder.set_character_widths([
                         7.58557, 7.58557, 7.58557, 7.58557, 7.58557, 7.58557, 7.58557, 7.58557,
                         7.58557, 7.58557, 7.58557, 7.58557, 7.58557, 7.58557, 7.58557, 7.58557,
                         0.0,
                     ]);
                     builder.set_word_lengths([3, 8, 6]);
-                    builder.build(&mut classes)
+                    builder.build()
                 }),
                 (NodeId(4), {
                     let mut builder = NodeBuilder::new(Role::InlineTextBox);
                     builder.set_bounds(Rect {
                         x0: 12.0,
                         y0: 63.0,
                         x1: 144.25222778320313,
@@ -1146,15 +1143,15 @@
                     ]);
                     builder.set_character_widths([
                         7.58557, 7.58557, 7.58557, 7.58557, 7.58557, 7.58557, 7.58557, 7.58557,
                         7.58557, 7.58557, 7.58557, 7.58557, 7.58557, 7.58557, 7.58557, 7.58557,
                         7.58557, 7.58557, 0.0,
                     ]);
                     builder.set_word_lengths([8, 11]);
-                    builder.build(&mut classes)
+                    builder.build()
                 }),
                 (NodeId(5), {
                     let mut builder = NodeBuilder::new(Role::InlineTextBox);
                     builder.set_bounds(Rect {
                         x0: 12.0,
                         y0: 77.66666412353516,
                         x1: 12.0,
@@ -1162,15 +1159,15 @@
                     });
                     builder.set_value("\n");
                     builder.set_text_direction(TextDirection::LeftToRight);
                     builder.set_character_lengths([1]);
                     builder.set_character_positions([0.0]);
                     builder.set_character_widths([0.0]);
                     builder.set_word_lengths([1]);
-                    builder.build(&mut classes)
+                    builder.build()
                 }),
                 (NodeId(6), {
                     let mut builder = NodeBuilder::new(Role::InlineTextBox);
                     builder.set_bounds(Rect {
                         x0: 12.0,
                         y0: 92.33332824707031,
                         x1: 158.9188995361328,
@@ -1192,15 +1189,15 @@
                     ]);
                     builder.set_character_widths([
                         7.58557, 7.58557, 7.58557, 7.58557, 7.58557, 7.58557, 7.58557, 7.58557,
                         7.58557, 7.58557, 7.58557, 7.58557, 7.58557, 7.58557, 7.58557, 7.58557,
                         7.58557, 7.58557, 7.58557, 7.58557, 0.0,
                     ]);
                     builder.set_word_lengths([5, 4, 6, 6]);
-                    builder.build(&mut classes)
+                    builder.build()
                 }),
                 (NodeId(7), {
                     let mut builder = NodeBuilder::new(Role::InlineTextBox);
                     builder.set_bounds(Rect {
                         x0: 12.0,
                         y0: 107.0,
                         x1: 12.0,
@@ -1208,15 +1205,15 @@
                     });
                     builder.set_value("");
                     builder.set_text_direction(TextDirection::LeftToRight);
                     builder.set_character_lengths([]);
                     builder.set_character_positions([]);
                     builder.set_character_widths([]);
                     builder.set_word_lengths([0]);
-                    builder.build(&mut classes)
+                    builder.build()
                 }),
             ],
             tree: Some(Tree::new(NodeId(0))),
             focus: NodeId(1),
         };
 
         crate::Tree::new(update, true)
```

### Comparing `accesskit-0.2.0/consumer/src/tree.rs` & `accesskit-0.3.0/consumer/src/tree.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 // Copyright 2021 The AccessKit Authors. All rights reserved.
 // Licensed under the Apache License, Version 2.0 (found in
 // the LICENSE-APACHE file) or the MIT license (found in
 // the LICENSE-MIT file), at your option.
 
 use accesskit::{Live, Node as NodeData, NodeId, Tree as TreeData, TreeUpdate};
-use std::collections::{HashMap, HashSet};
+use std::{
+    collections::{HashMap, HashSet},
+    sync::Arc,
+};
 
 use crate::node::{DetachedNode, Node, NodeState, ParentAndIndex};
 
 #[derive(Clone)]
 pub struct State {
     pub(crate) nodes: HashMap<NodeId, NodeState>,
     pub(crate) data: TreeData,
@@ -73,15 +76,15 @@
             parent_and_index: Option<ParentAndIndex>,
             id: NodeId,
             data: NodeData,
         ) {
             let state = NodeState {
                 id,
                 parent_and_index,
-                data,
+                data: Arc::new(data),
             };
             nodes.insert(id, state);
             if let Some(changes) = changes {
                 changes.added_node_ids.insert(id);
             }
         }
 
@@ -116,15 +119,15 @@
                     node_state.parent_and_index = None;
                 }
                 for child_id in node_state.data.children().iter() {
                     if !seen_child_ids.contains(child_id) {
                         orphans.insert(*child_id);
                     }
                 }
-                node_state.data = node_data;
+                node_state.data = Arc::new(node_data);
             } else if let Some(parent_and_index) = pending_children.remove(&node_id) {
                 add_node(
                     &mut self.nodes,
                     &mut changes,
                     Some(parent_and_index),
                     node_id,
                     node_data,
@@ -180,14 +183,15 @@
                 if let Some(old_node_state) = self.nodes.remove(&id) {
                     if let Some(changes) = &mut changes {
                         let old_node = DetachedNode {
                             state: old_node_state,
                             is_focused: old_focus_id == Some(id),
                             is_root: old_root_id == id,
                             name: None,
+                            description: None,
                             value: None,
                             live: Live::Off,
                             supports_text_ranges: false,
                         };
                         changes.removed_nodes.insert(id, old_node);
                     }
                 }
@@ -211,15 +215,15 @@
     }
 
     pub fn serialize(&self) -> TreeUpdate {
         let mut nodes = Vec::new();
 
         fn traverse(state: &State, nodes: &mut Vec<(NodeId, NodeData)>, id: NodeId) {
             let node = state.nodes.get(&id).unwrap();
-            nodes.push((id, node.data.clone()));
+            nodes.push((id, (*node.data).clone()));
 
             for child_id in node.data.children().iter() {
                 traverse(state, nodes, *child_id);
             }
         }
 
         traverse(self, &mut nodes, self.data.root);
@@ -385,51 +389,40 @@
     pub fn state(&self) -> &State {
         &self.state
     }
 }
 
 #[cfg(test)]
 mod tests {
-    use accesskit::{NodeBuilder, NodeClassSet, NodeId, Role, Tree, TreeUpdate};
+    use accesskit::{NodeBuilder, NodeId, Role, Tree, TreeUpdate};
 
     #[test]
     fn init_tree_with_root_node() {
-        let mut classes = NodeClassSet::new();
         let update = TreeUpdate {
-            nodes: vec![(
-                NodeId(0),
-                NodeBuilder::new(Role::Window).build(&mut classes),
-            )],
+            nodes: vec![(NodeId(0), NodeBuilder::new(Role::Window).build())],
             tree: Some(Tree::new(NodeId(0))),
             focus: NodeId(0),
         };
         let tree = super::Tree::new(update, false);
         assert_eq!(NodeId(0), tree.state().root().id());
         assert_eq!(Role::Window, tree.state().root().role());
         assert!(tree.state().root().parent().is_none());
     }
 
     #[test]
     fn root_node_has_children() {
-        let mut classes = NodeClassSet::new();
         let update = TreeUpdate {
             nodes: vec![
                 (NodeId(0), {
                     let mut builder = NodeBuilder::new(Role::Window);
                     builder.set_children(vec![NodeId(1), NodeId(2)]);
-                    builder.build(&mut classes)
+                    builder.build()
                 }),
-                (
-                    NodeId(1),
-                    NodeBuilder::new(Role::Button).build(&mut classes),
-                ),
-                (
-                    NodeId(2),
-                    NodeBuilder::new(Role::Button).build(&mut classes),
-                ),
+                (NodeId(1), NodeBuilder::new(Role::Button).build()),
+                (NodeId(2), NodeBuilder::new(Role::Button).build()),
             ],
             tree: Some(Tree::new(NodeId(0))),
             focus: NodeId(0),
         };
         let tree = super::Tree::new(update, false);
         let state = tree.state();
         assert_eq!(
@@ -441,34 +434,30 @@
             state.node_by_id(NodeId(2)).unwrap().parent().unwrap().id()
         );
         assert_eq!(2, state.root().children().count());
     }
 
     #[test]
     fn add_child_to_root_node() {
-        let mut classes = NodeClassSet::new();
         let root_builder = NodeBuilder::new(Role::Window);
         let first_update = TreeUpdate {
-            nodes: vec![(NodeId(0), root_builder.clone().build(&mut classes))],
+            nodes: vec![(NodeId(0), root_builder.clone().build())],
             tree: Some(Tree::new(NodeId(0))),
             focus: NodeId(0),
         };
         let mut tree = super::Tree::new(first_update, false);
         assert_eq!(0, tree.state().root().children().count());
         let second_update = TreeUpdate {
             nodes: vec![
                 (NodeId(0), {
                     let mut builder = root_builder;
                     builder.push_child(NodeId(1));
-                    builder.build(&mut classes)
+                    builder.build()
                 }),
-                (
-                    NodeId(1),
-                    NodeBuilder::new(Role::RootWebArea).build(&mut classes),
-                ),
+                (NodeId(1), NodeBuilder::new(Role::RootWebArea).build()),
             ],
             tree: None,
             focus: NodeId(0),
         };
         struct Handler {
             got_new_child_node: bool,
             got_updated_root_node: bool,
@@ -524,35 +513,31 @@
             NodeId(0),
             state.node_by_id(NodeId(1)).unwrap().parent().unwrap().id()
         );
     }
 
     #[test]
     fn remove_child_from_root_node() {
-        let mut classes = NodeClassSet::new();
         let root_builder = NodeBuilder::new(Role::Window);
         let first_update = TreeUpdate {
             nodes: vec![
                 (NodeId(0), {
                     let mut builder = root_builder.clone();
                     builder.push_child(NodeId(1));
-                    builder.build(&mut classes)
+                    builder.build()
                 }),
-                (
-                    NodeId(1),
-                    NodeBuilder::new(Role::RootWebArea).build(&mut classes),
-                ),
+                (NodeId(1), NodeBuilder::new(Role::RootWebArea).build()),
             ],
             tree: Some(Tree::new(NodeId(0))),
             focus: NodeId(0),
         };
         let mut tree = super::Tree::new(first_update, false);
         assert_eq!(1, tree.state().root().children().count());
         let second_update = TreeUpdate {
-            nodes: vec![(NodeId(0), root_builder.build(&mut classes))],
+            nodes: vec![(NodeId(0), root_builder.build())],
             tree: None,
             focus: NodeId(0),
         };
         struct Handler {
             got_updated_root_node: bool,
             got_removed_child_node: bool,
         }
@@ -602,30 +587,23 @@
         assert!(handler.got_removed_child_node);
         assert_eq!(0, tree.state().root().children().count());
         assert!(tree.state().node_by_id(NodeId(1)).is_none());
     }
 
     #[test]
     fn move_focus_between_siblings() {
-        let mut classes = NodeClassSet::new();
         let first_update = TreeUpdate {
             nodes: vec![
                 (NodeId(0), {
                     let mut builder = NodeBuilder::new(Role::Window);
                     builder.set_children(vec![NodeId(1), NodeId(2)]);
-                    builder.build(&mut classes)
+                    builder.build()
                 }),
-                (
-                    NodeId(1),
-                    NodeBuilder::new(Role::Button).build(&mut classes),
-                ),
-                (
-                    NodeId(2),
-                    NodeBuilder::new(Role::Button).build(&mut classes),
-                ),
+                (NodeId(1), NodeBuilder::new(Role::Button).build()),
+                (NodeId(2), NodeBuilder::new(Role::Button).build()),
             ],
             tree: Some(Tree::new(NodeId(0))),
             focus: NodeId(1),
         };
         let mut tree = super::Tree::new(first_update, true);
         assert!(tree.state().node_by_id(NodeId(1)).unwrap().is_focused());
         let second_update = TreeUpdate {
@@ -697,42 +675,41 @@
         assert!(handler.got_focus_change);
         assert!(tree.state().node_by_id(NodeId(2)).unwrap().is_focused());
         assert!(!tree.state().node_by_id(NodeId(1)).unwrap().is_focused());
     }
 
     #[test]
     fn update_node() {
-        let mut classes = NodeClassSet::new();
         let child_builder = NodeBuilder::new(Role::Button);
         let first_update = TreeUpdate {
             nodes: vec![
                 (NodeId(0), {
                     let mut builder = NodeBuilder::new(Role::Window);
                     builder.set_children(vec![NodeId(1)]);
-                    builder.build(&mut classes)
+                    builder.build()
                 }),
                 (NodeId(1), {
                     let mut builder = child_builder.clone();
                     builder.set_name("foo");
-                    builder.build(&mut classes)
+                    builder.build()
                 }),
             ],
             tree: Some(Tree::new(NodeId(0))),
             focus: NodeId(0),
         };
         let mut tree = super::Tree::new(first_update, false);
         assert_eq!(
             Some("foo".into()),
             tree.state().node_by_id(NodeId(1)).unwrap().name()
         );
         let second_update = TreeUpdate {
             nodes: vec![(NodeId(1), {
                 let mut builder = child_builder;
                 builder.set_name("bar");
-                builder.build(&mut classes)
+                builder.build()
             })],
             tree: None,
             focus: NodeId(0),
         };
         struct Handler {
             got_updated_child_node: bool,
         }
```

### Comparing `accesskit-0.2.0/common/Cargo.toml` & `accesskit-0.3.0/common/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "accesskit"
-version = "0.13.0"
+version = "0.14.0"
 authors.workspace = true
 license.workspace = true
 description = "UI accessibility infrastructure across platforms"
 categories.workspace = true
 keywords = ["gui", "ui", "accessibility"]
 repository.workspace = true
 readme = "README.md"
@@ -19,7 +19,8 @@
 pyo3 = { version = "0.20", optional = true }
 schemars = { version = "0.8.7", optional = true }
 serde = { version = "1.0", features = ["derive"], optional = true }
 
 [features]
 serde = ["dep:serde", "enumn"]
 schemars = ["dep:schemars", "serde"]
+
```

### Comparing `accesskit-0.2.0/common/CHANGELOG.md` & `accesskit-0.3.0/common/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,38 @@
 # Changelog
 
+## [0.14.0](https://github.com/AccessKit/accesskit/compare/accesskit-v0.13.0...accesskit-v0.14.0) (2024-04-30)
+
+
+### ⚠ BREAKING CHANGES
+
+* Clean up table roles and properties ([#393](https://github.com/AccessKit/accesskit/issues/393))
+* Drop `SortDirection::Unsorted` ([#391](https://github.com/AccessKit/accesskit/issues/391))
+* Rename `hierarchical_level` to `level` ([#390](https://github.com/AccessKit/accesskit/issues/390))
+* Drop `NodeClassSet` ([#389](https://github.com/AccessKit/accesskit/issues/389))
+* Rename `Checked` to `Toggled`; drop `ToggleButton` role ([#388](https://github.com/AccessKit/accesskit/issues/388))
+
+### Features
+
+* Add the `owns` relation ([#392](https://github.com/AccessKit/accesskit/issues/392)) ([fd668dd](https://github.com/AccessKit/accesskit/commit/fd668ddc4b64cb05ab3600972b3d3823a037f2d5))
+
+
+### Bug Fixes
+
+* Increase minimum supported Rust version to `1.70` ([#396](https://github.com/AccessKit/accesskit/issues/396)) ([a8398b8](https://github.com/AccessKit/accesskit/commit/a8398b847aa003de91042ac45e33126fc2cae053))
+
+
+### Code Refactoring
+
+* Clean up table roles and properties ([#393](https://github.com/AccessKit/accesskit/issues/393)) ([e34dad9](https://github.com/AccessKit/accesskit/commit/e34dad94448a5321ece9def3f2e054aa5f62dd79))
+* Drop `NodeClassSet` ([#389](https://github.com/AccessKit/accesskit/issues/389)) ([1b153ed](https://github.com/AccessKit/accesskit/commit/1b153ed51f8421cdba2dc98beca2e8f5f8c781bc))
+* Drop `SortDirection::Unsorted` ([#391](https://github.com/AccessKit/accesskit/issues/391)) ([b86f484](https://github.com/AccessKit/accesskit/commit/b86f484b7e6645e63362896b744a71ec758f810d))
+* Rename `Checked` to `Toggled`; drop `ToggleButton` role ([#388](https://github.com/AccessKit/accesskit/issues/388)) ([6bc040b](https://github.com/AccessKit/accesskit/commit/6bc040b7cf75cdbd6a019cc380d8dbce804b3c81))
+* Rename `hierarchical_level` to `level` ([#390](https://github.com/AccessKit/accesskit/issues/390)) ([2d61e01](https://github.com/AccessKit/accesskit/commit/2d61e01fffff1265b348c141715f6f9b6fe4081b))
+
 ## [0.13.0](https://github.com/AccessKit/accesskit/compare/accesskit-v0.12.3...accesskit-v0.13.0) (2024-04-14)
 
 
 ### ⚠ BREAKING CHANGES
 
 * New approach to lazy initialization ([#375](https://github.com/AccessKit/accesskit/issues/375))
```

### Comparing `accesskit-0.2.0/common/README.md` & `accesskit-0.3.0/common/README.md`

 * *Files identical despite different names*

### Comparing `accesskit-0.2.0/common/src/geometry.rs` & `accesskit-0.3.0/common/src/geometry.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.2.0/common/src/lib.rs` & `accesskit-0.3.0/common/src/lib.rs`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 };
 #[cfg(feature = "serde")]
 use serde::{
     de::{Deserializer, IgnoredAny, MapAccess, SeqAccess, Visitor},
     ser::{SerializeMap, SerializeSeq, Serializer},
     Deserialize, Serialize,
 };
-use std::{collections::BTreeSet, ops::DerefMut, sync::Arc};
 #[cfg(feature = "serde")]
 use std::{fmt, mem::size_of_val};
 
 mod geometry;
 pub use geometry::{Affine, Point, Rect, Size, Vec2};
 
 /// The type of an accessibility node.
@@ -78,24 +77,21 @@
     RadioButton,
     TextInput,
     Button,
     DefaultButton,
     Pane,
     RowHeader,
     ColumnHeader,
-    Column,
     RowGroup,
     List,
     Table,
-    TableHeaderContainer,
     LayoutTableCell,
     LayoutTableRow,
     LayoutTable,
     Switch,
-    ToggleButton,
     Menu,
 
     MultilineTextInput,
     SearchInput,
     DateInput,
     DateTimeInput,
     WeekInput,
@@ -497,15 +493,15 @@
 #[cfg_attr(feature = "schemars", derive(JsonSchema))]
 #[cfg_attr(feature = "serde", serde(rename_all = "camelCase"))]
 #[cfg_attr(
     feature = "pyo3",
     pyclass(module = "accesskit", rename_all = "SCREAMING_SNAKE_CASE")
 )]
 #[repr(u8)]
-pub enum Checked {
+pub enum Toggled {
     False,
     True,
     Mixed,
 }
 
 /// Describes the action that will be performed on a given node when
 /// executing the default action, which is a click.
@@ -547,15 +543,14 @@
 #[cfg_attr(feature = "serde", serde(rename_all = "camelCase"))]
 #[cfg_attr(
     feature = "pyo3",
     pyclass(module = "accesskit", rename_all = "SCREAMING_SNAKE_CASE")
 )]
 #[repr(u8)]
 pub enum SortDirection {
-    Unsorted,
     Ascending,
     Descending,
     Other,
 }
 
 #[derive(Clone, Copy, Debug, PartialEq, Eq, Hash)]
 #[cfg_attr(feature = "enumn", derive(enumn::N))]
@@ -813,15 +808,15 @@
     Usize(usize),
     Color(u32),
     TextDecoration(TextDecoration),
     LengthSlice(Box<[u8]>),
     CoordSlice(Box<[f32]>),
     Bool(bool),
     Invalid(Invalid),
-    Checked(Checked),
+    Toggled(Toggled),
     Live(Live),
     DefaultActionVerb(DefaultActionVerb),
     TextDirection(TextDirection),
     Orientation(Orientation),
     SortDirection(SortDirection),
     AriaCurrent(AriaCurrent),
     AutoComplete(AutoComplete),
@@ -844,27 +839,25 @@
     // NodeIdVec
     Children,
     Controls,
     Details,
     DescribedBy,
     FlowTo,
     LabelledBy,
+    Owns,
     RadioGroup,
 
     // NodeId
     ActiveDescendant,
     ErrorMessage,
     InPageLinkTarget,
     MemberOf,
     NextOnLine,
     PreviousOnLine,
     PopupFor,
-    TableHeader,
-    TableRowHeader,
-    TableColumnHeader,
 
     // String
     Name,
     Description,
     Value,
     AccessKey,
     ClassName,
@@ -874,14 +867,16 @@
     KeyboardShortcut,
     Language,
     Placeholder,
     RoleDescription,
     StateDescription,
     Tooltip,
     Url,
+    RowIndexText,
+    ColumnIndexText,
 
     // f64
     ScrollX,
     ScrollXMin,
     ScrollXMax,
     ScrollY,
     ScrollYMin,
@@ -891,23 +886,21 @@
     MaxNumericValue,
     NumericValueStep,
     NumericValueJump,
     FontSize,
     FontWeight,
 
     // usize
-    TableRowCount,
-    TableColumnCount,
-    TableRowIndex,
-    TableColumnIndex,
-    TableCellColumnIndex,
-    TableCellColumnSpan,
-    TableCellRowIndex,
-    TableCellRowSpan,
-    HierarchicalLevel,
+    RowCount,
+    ColumnCount,
+    RowIndex,
+    ColumnIndex,
+    RowSpan,
+    ColumnSpan,
+    Level,
     SizeOfSet,
     PositionInSet,
 
     // Color
     ColorValue,
     BackgroundColor,
     ForegroundColor,
@@ -927,15 +920,15 @@
 
     // bool
     Expanded,
     Selected,
 
     // Unique enums
     Invalid,
-    Checked,
+    Toggled,
     Live,
     DefaultActionVerb,
     TextDirection,
     Orientation,
     SortDirection,
     AriaCurrent,
     AutoComplete,
@@ -950,77 +943,42 @@
     TextSelection,
     CustomActions,
 
     // This MUST be last.
     Unset,
 }
 
-#[derive(Clone, Copy, Debug, PartialEq, Eq, PartialOrd, Ord, Hash)]
+#[derive(Clone, Copy, Debug, PartialEq, Eq)]
 #[repr(transparent)]
 struct PropertyIndices([u8; PropertyId::Unset as usize]);
 
 impl Default for PropertyIndices {
     fn default() -> Self {
         Self([PropertyId::Unset as u8; PropertyId::Unset as usize])
     }
 }
 
-#[derive(Clone, Copy, Debug, Default, PartialEq, Eq, PartialOrd, Ord)]
+#[derive(Clone, Copy, Debug, Default, PartialEq, Eq)]
 struct NodeClass {
     role: Role,
     actions: Actions,
     indices: PropertyIndices,
 }
 
-/// Allows nodes that have the same role, actions, and set of defined properties
-/// to share metadata. Each node has a class which is created by [`NodeBuilder`],
-/// and when [`NodeBuilder::build`] is called, the node's class is added
-/// to the provided instance of this struct if an identical class isn't
-/// in that set already. Once a class is added to a class set, it currently
-/// remains in that set for the life of that set, whether or not any nodes
-/// are still using the class.
-///
-/// It's not an error for different nodes in the same tree, or even subsequent
-/// versions of the same node, to be built from different class sets;
-/// it's merely suboptimal.
-///
-/// Note: This struct's `Default` implementation doesn't provide access to
-/// a shared set, as one might assume; it creates a new set. For a shared set,
-/// use [`NodeClassSet::lock_global`].
-#[derive(Clone, Default)]
-#[repr(transparent)]
-pub struct NodeClassSet(BTreeSet<Arc<NodeClass>>);
-
-impl NodeClassSet {
-    #[inline]
-    pub const fn new() -> Self {
-        Self(BTreeSet::new())
-    }
-
-    /// Accesses a shared class set guarded by a mutex.
-    pub fn lock_global() -> impl DerefMut<Target = Self> {
-        use std::sync::Mutex;
-
-        static INSTANCE: Mutex<NodeClassSet> = Mutex::new(NodeClassSet::new());
-
-        INSTANCE.lock().unwrap()
-    }
-}
-
 /// A single accessible object. A complete UI is represented as a tree of these.
 ///
 /// For brevity, and to make more of the documentation usable in bindings
 /// to other languages, documentation of getter methods is written as if
 /// documenting fields in a struct, and such methods are referred to
 /// as properties.
 #[derive(Clone, Debug, PartialEq)]
 pub struct Node {
-    class: Arc<NodeClass>,
+    class: NodeClass,
     flags: u32,
-    props: Arc<[PropertyValue]>,
+    props: Box<[PropertyValue]>,
 }
 
 /// Builds a [`Node`].
 #[derive(Clone, Debug, Default, PartialEq)]
 pub struct NodeBuilder {
     class: NodeClass,
     flags: u32,
@@ -1361,26 +1319,19 @@
                 role,
                 ..Default::default()
             },
             ..Default::default()
         }
     }
 
-    pub fn build(self, classes: &mut NodeClassSet) -> Node {
-        let class = if let Some(class) = classes.0.get(&self.class) {
-            Arc::clone(class)
-        } else {
-            let class = Arc::new(self.class);
-            classes.0.insert(Arc::clone(&class));
-            class
-        };
+    pub fn build(self) -> Node {
         Node {
-            class,
+            class: self.class,
             flags: self.flags,
-            props: self.props.into(),
+            props: self.props.into_boxed_slice(),
         }
     }
 }
 
 impl Node {
     #[inline]
     pub fn role(&self) -> Role {
@@ -1509,30 +1460,33 @@
 node_id_vec_property_methods! {
     (Children, children, set_children, push_child, clear_children),
     (Controls, controls, set_controls, push_controlled, clear_controls),
     (Details, details, set_details, push_detail, clear_details),
     (DescribedBy, described_by, set_described_by, push_described_by, clear_described_by),
     (FlowTo, flow_to, set_flow_to, push_flow_to, clear_flow_to),
     (LabelledBy, labelled_by, set_labelled_by, push_labelled_by, clear_labelled_by),
+    /// As with the `aria-owns` property in ARIA, this property should be set
+    /// only if the nodes referenced in the property are not descendants
+    /// of the owning node in the AccessKit tree. In the common case, where the
+    /// owned nodes are direct children or indirect descendants, this property
+    /// is unnecessary.
+    (Owns, owns, set_owns, push_owned, clear_owns),
     /// On radio buttons this should be set to a list of all of the buttons
     /// in the same group as this one, including this radio button itself.
     (RadioGroup, radio_group, set_radio_group, push_to_radio_group, clear_radio_group)
 }
 
 node_id_property_methods! {
     (ActiveDescendant, active_descendant, set_active_descendant, clear_active_descendant),
     (ErrorMessage, error_message, set_error_message, clear_error_message),
     (InPageLinkTarget, in_page_link_target, set_in_page_link_target, clear_in_page_link_target),
     (MemberOf, member_of, set_member_of, clear_member_of),
     (NextOnLine, next_on_line, set_next_on_line, clear_next_on_line),
     (PreviousOnLine, previous_on_line, set_previous_on_line, clear_previous_on_line),
-    (PopupFor, popup_for, set_popup_for, clear_popup_for),
-    (TableHeader, table_header, set_table_header, clear_table_header),
-    (TableRowHeader, table_row_header, set_table_row_header, clear_table_row_header),
-    (TableColumnHeader, table_column_header, set_table_column_header, clear_table_column_header)
+    (PopupFor, popup_for, set_popup_for, clear_popup_for)
 }
 
 string_property_methods! {
     (Name, name, set_name, clear_name),
     (Description, description, set_description, clear_description),
     (Value, value, set_value, clear_value),
     /// A single character, usually part of this node's name, that can be pressed,
@@ -1571,15 +1525,17 @@
     /// and assistive technologies do not support this feature.
     (StateDescription, state_description, set_state_description, clear_state_description),
     /// If a node's only accessible name comes from a tooltip, it should be
     /// exposed through this property rather than [`name`].
     ///
     /// [`name`]: Node::name
     (Tooltip, tooltip, set_tooltip, clear_tooltip),
-    (Url, url, set_url, clear_url)
+    (Url, url, set_url, clear_url),
+    (RowIndexText, row_index_text, set_row_index_text, clear_row_index_text),
+    (ColumnIndexText, column_index_text, set_column_index_text, clear_column_index_text)
 }
 
 f64_property_methods! {
     (ScrollX, scroll_x, set_scroll_x, clear_scroll_x),
     (ScrollXMin, scroll_x_min, set_scroll_x_min, clear_scroll_x_min),
     (ScrollXMax, scroll_x_max, set_scroll_x_max, clear_scroll_x_max),
     (ScrollY, scroll_y, set_scroll_y, clear_scroll_y),
@@ -1594,23 +1550,21 @@
     (FontSize, font_size, set_font_size, clear_font_size),
     /// Font weight can take on any arbitrary numeric value. Increments of 100 in
     /// range `[0, 900]` represent keywords such as light, normal, bold, etc.
     (FontWeight, font_weight, set_font_weight, clear_font_weight)
 }
 
 usize_property_methods! {
-    (TableRowCount, table_row_count, set_table_row_count, clear_table_row_count),
-    (TableColumnCount, table_column_count, set_table_column_count, clear_table_column_count),
-    (TableRowIndex, table_row_index, set_table_row_index, clear_table_row_index),
-    (TableColumnIndex, table_column_index, set_table_column_index, clear_table_column_index),
-    (TableCellColumnIndex, table_cell_column_index, set_table_cell_column_index, clear_table_cell_column_index),
-    (TableCellColumnSpan, table_cell_column_span, set_table_cell_column_span, clear_table_cell_column_span),
-    (TableCellRowIndex, table_cell_row_index, set_table_cell_row_index, clear_table_cell_row_index),
-    (TableCellRowSpan, table_cell_row_span, set_table_cell_row_span, clear_table_cell_row_span),
-    (HierarchicalLevel, hierarchical_level, set_hierarchical_level, clear_hierarchical_level),
+    (RowCount, row_count, set_row_count, clear_row_count),
+    (ColumnCount, column_count, set_column_count, clear_column_count),
+    (RowIndex, row_index, set_row_index, clear_row_index),
+    (ColumnIndex, column_index, set_column_index, clear_column_index),
+    (RowSpan, row_span, set_row_span, clear_row_span),
+    (ColumnSpan, column_span, set_column_span, clear_column_span),
+    (Level, level, set_level, clear_level),
     (SizeOfSet, size_of_set, set_size_of_set, clear_size_of_set),
     (PositionInSet, position_in_set, set_position_in_set, clear_position_in_set)
 }
 
 color_property_methods! {
     /// For [`Role::ColorWell`], specifies the selected color in RGBA.
     (ColorValue, color_value, set_color_value, clear_color_value),
@@ -1729,15 +1683,15 @@
     /// in platform accessibility APIs has made extraneous
     /// "not selected" announcements a common annoyance.
     (Selected, is_selected, set_selected, clear_selected)
 }
 
 unique_enum_property_methods! {
     (Invalid, invalid, set_invalid, clear_invalid),
-    (Checked, checked, set_checked, clear_checked),
+    (Toggled, toggled, set_toggled, clear_toggled),
     (Live, live, set_live, clear_live),
     (DefaultActionVerb, default_action_verb, set_default_action_verb, clear_default_action_verb),
     (TextDirection, text_direction, set_text_direction, clear_text_direction),
     (Orientation, orientation, set_orientation, clear_orientation),
     (SortDirection, sort_direction, set_sort_direction, clear_sort_direction),
     (AriaCurrent, aria_current, set_aria_current, clear_aria_current),
     (AutoComplete, auto_complete, set_auto_complete, clear_auto_complete),
@@ -1879,15 +1833,15 @@
                 Usize,
                 Color,
                 TextDecoration,
                 LengthSlice,
                 CoordSlice,
                 Bool,
                 Invalid,
-                Checked,
+                Toggled,
                 Live,
                 DefaultActionVerb,
                 TextDirection,
                 Orientation,
                 SortDirection,
                 AriaCurrent,
                 AutoComplete,
@@ -1942,27 +1896,25 @@
                         NodeIdVec {
                             Children,
                             Controls,
                             Details,
                             DescribedBy,
                             FlowTo,
                             LabelledBy,
+                            Owns,
                             RadioGroup
                         },
                         NodeId {
                             ActiveDescendant,
                             ErrorMessage,
                             InPageLinkTarget,
                             MemberOf,
                             NextOnLine,
                             PreviousOnLine,
-                            PopupFor,
-                            TableHeader,
-                            TableRowHeader,
-                            TableColumnHeader
+                            PopupFor
                         },
                         String {
                             Name,
                             Description,
                             Value,
                             AccessKey,
                             ClassName,
@@ -1971,15 +1923,17 @@
                             InnerHtml,
                             KeyboardShortcut,
                             Language,
                             Placeholder,
                             RoleDescription,
                             StateDescription,
                             Tooltip,
-                            Url
+                            Url,
+                            RowIndexText,
+                            ColumnIndexText
                         },
                         F64 {
                             ScrollX,
                             ScrollXMin,
                             ScrollXMax,
                             ScrollY,
                             ScrollYMin,
@@ -1989,23 +1943,21 @@
                             MaxNumericValue,
                             NumericValueStep,
                             NumericValueJump,
                             FontSize,
                             FontWeight
                         },
                         Usize {
-                            TableRowCount,
-                            TableColumnCount,
-                            TableRowIndex,
-                            TableColumnIndex,
-                            TableCellColumnIndex,
-                            TableCellColumnSpan,
-                            TableCellRowIndex,
-                            TableCellRowSpan,
-                            HierarchicalLevel,
+                            RowCount,
+                            ColumnCount,
+                            RowIndex,
+                            ColumnIndex,
+                            RowSpan,
+                            ColumnSpan,
+                            Level,
                             SizeOfSet,
                             PositionInSet
                         },
                         Color {
                             ColorValue,
                             BackgroundColor,
                             ForegroundColor
@@ -2024,15 +1976,15 @@
                             CharacterWidths
                         },
                         Bool {
                             Expanded,
                             Selected
                         },
                         Invalid { Invalid },
-                        Checked { Checked },
+                        Toggled { Toggled },
                         Live { Live },
                         DefaultActionVerb { DefaultActionVerb },
                         TextDirection { TextDirection },
                         Orientation { Orientation },
                         SortDirection { SortDirection },
                         AriaCurrent { AriaCurrent },
                         AutoComplete { AutoComplete },
@@ -2048,15 +2000,15 @@
                 }
                 DeserializeKey::Unknown(_) => {
                     let _ = map.next_value::<IgnoredAny>()?;
                 }
             }
         }
 
-        Ok(builder.build(&mut NodeClassSet::lock_global()))
+        Ok(builder.build())
     }
 }
 
 #[cfg(feature = "serde")]
 impl<'de> Deserialize<'de> for Node {
     fn deserialize<D>(deserializer: D) -> Result<Self, D::Error>
     where
@@ -2128,27 +2080,25 @@
             Vec<NodeId> {
                 Children,
                 Controls,
                 Details,
                 DescribedBy,
                 FlowTo,
                 LabelledBy,
+                Owns,
                 RadioGroup
             },
             NodeId {
                 ActiveDescendant,
                 ErrorMessage,
                 InPageLinkTarget,
                 MemberOf,
                 NextOnLine,
                 PreviousOnLine,
-                PopupFor,
-                TableHeader,
-                TableRowHeader,
-                TableColumnHeader
+                PopupFor
             },
             Box<str> {
                 Name,
                 Description,
                 Value,
                 AccessKey,
                 ClassName,
@@ -2157,15 +2107,17 @@
                 InnerHtml,
                 KeyboardShortcut,
                 Language,
                 Placeholder,
                 RoleDescription,
                 StateDescription,
                 Tooltip,
-                Url
+                Url,
+                RowIndexText,
+                ColumnIndexText
             },
             f64 {
                 ScrollX,
                 ScrollXMin,
                 ScrollXMax,
                 ScrollY,
                 ScrollYMin,
@@ -2175,23 +2127,21 @@
                 MaxNumericValue,
                 NumericValueStep,
                 NumericValueJump,
                 FontSize,
                 FontWeight
             },
             usize {
-                TableRowCount,
-                TableColumnCount,
-                TableRowIndex,
-                TableColumnIndex,
-                TableCellColumnIndex,
-                TableCellColumnSpan,
-                TableCellRowIndex,
-                TableCellRowSpan,
-                HierarchicalLevel,
+                RowCount,
+                ColumnCount,
+                RowIndex,
+                ColumnIndex,
+                RowSpan,
+                ColumnSpan,
+                Level,
                 SizeOfSet,
                 PositionInSet
             },
             u32 {
                 ColorValue,
                 BackgroundColor,
                 ForegroundColor
@@ -2210,15 +2160,15 @@
                 CharacterWidths
             },
             bool {
                 Expanded,
                 Selected
             },
             Invalid { Invalid },
-            Checked { Checked },
+            Toggled { Toggled },
             Live { Live },
             DefaultActionVerb { DefaultActionVerb },
             TextDirection { TextDirection },
             Orientation { Orientation },
             SortDirection { SortDirection },
             AriaCurrent { AriaCurrent },
             AutoComplete { AutoComplete },
```

### Comparing `accesskit-0.2.0/platforms/unix/Cargo.toml` & `accesskit-0.3.0/platforms/unix/Cargo.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "accesskit_unix"
-version = "0.8.0"
+version = "0.9.0"
 authors.workspace = true
 license.workspace = true
 description = "AccessKit UI accessibility infrastructure: Linux adapter"
 categories.workspace = true
 keywords = ["gui", "ui", "accessibility"]
 repository.workspace = true
 readme = "README.md"
@@ -13,19 +13,18 @@
 
 [features]
 default = ["async-io"]
 async-io = ["dep:async-channel", "dep:async-executor", "dep:async-task", "dep:futures-util", "atspi/async-std", "zbus/async-io"]
 tokio = ["dep:tokio", "dep:tokio-stream", "atspi/tokio", "zbus/tokio"]
 
 [dependencies]
-accesskit = { version = "0.13.0", path = "../../common" }
-accesskit_atspi_common = { version = "0.3.0", path = "../atspi-common" }
+accesskit = { version = "0.14.0", path = "../../common" }
+accesskit_atspi_common = { version = "0.4.0", path = "../atspi-common" }
 atspi = { version = "0.19", default-features = false }
 futures-lite = "1.13"
-once_cell = "1.17.1"
 serde = "1.0"
 zbus = { version = "3.14", default-features = false }
 
 # async-io support
 async-channel = { version = "2.1.1", optional = true }
 async-executor = { version = "1.5.0", optional = true }
 async-task = { version = "4.3.0", optional = true }
```

### Comparing `accesskit-0.2.0/platforms/unix/CHANGELOG.md` & `accesskit-0.3.0/platforms/unix/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,34 @@
     * accesskit bumped from 0.12.2 to 0.12.3
     * accesskit_atspi_common bumped from 0.1.1 to 0.1.2
 
 * The following workspace dependencies were updated
   * dependencies
     * accesskit_atspi_common bumped from 0.1.2 to 0.2.0
 
+## [0.9.0](https://github.com/AccessKit/accesskit/compare/accesskit_unix-v0.8.0...accesskit_unix-v0.9.0) (2024-04-30)
+
+
+### ⚠ BREAKING CHANGES
+
+* Force a semver-breaking release ([#398](https://github.com/AccessKit/accesskit/issues/398))
+
+### Bug Fixes
+
+* Force a semver-breaking release ([#398](https://github.com/AccessKit/accesskit/issues/398)) ([87b8b92](https://github.com/AccessKit/accesskit/commit/87b8b92b74a102c7cae48e013d2c2ae1cc2f9598))
+* Increase minimum supported Rust version to `1.70` ([#396](https://github.com/AccessKit/accesskit/issues/396)) ([a8398b8](https://github.com/AccessKit/accesskit/commit/a8398b847aa003de91042ac45e33126fc2cae053))
+
+
+### Dependencies
+
+* The following workspace dependencies were updated
+  * dependencies
+    * accesskit bumped from 0.13.0 to 0.14.0
+    * accesskit_atspi_common bumped from 0.3.0 to 0.4.0
+
 ## [0.8.0](https://github.com/AccessKit/accesskit/compare/accesskit_unix-v0.7.5...accesskit_unix-v0.8.0) (2024-04-14)
 
 
 ### ⚠ BREAKING CHANGES
 
 * New approach to lazy initialization ([#375](https://github.com/AccessKit/accesskit/issues/375))
```

### Comparing `accesskit-0.2.0/platforms/unix/src/adapter.rs` & `accesskit-0.3.0/platforms/unix/src/adapter.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.2.0/platforms/unix/src/atspi/bus.rs` & `accesskit-0.3.0/platforms/unix/src/atspi/bus.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.2.0/platforms/unix/src/atspi/interfaces/accessible.rs` & `accesskit-0.3.0/platforms/unix/src/atspi/interfaces/accessible.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.2.0/platforms/unix/src/atspi/interfaces/action.rs` & `accesskit-0.3.0/platforms/unix/src/atspi/interfaces/action.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.2.0/platforms/unix/src/atspi/interfaces/application.rs` & `accesskit-0.3.0/platforms/unix/src/atspi/interfaces/application.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.2.0/platforms/unix/src/atspi/interfaces/component.rs` & `accesskit-0.3.0/platforms/unix/src/atspi/interfaces/component.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.2.0/platforms/unix/src/atspi/interfaces/mod.rs` & `accesskit-0.3.0/platforms/unix/src/atspi/interfaces/mod.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.2.0/platforms/unix/src/atspi/interfaces/value.rs` & `accesskit-0.3.0/platforms/unix/src/atspi/interfaces/value.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.2.0/platforms/unix/src/atspi/object_address.rs` & `accesskit-0.3.0/platforms/unix/src/atspi/object_address.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.2.0/platforms/unix/src/atspi/object_id.rs` & `accesskit-0.3.0/platforms/unix/src/atspi/object_id.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.2.0/platforms/unix/src/context.rs` & `accesskit-0.3.0/platforms/unix/src/context.rs`

 * *Files 3% similar despite different names*

```diff
@@ -6,17 +6,16 @@
 use accesskit::{ActivationHandler, DeactivationHandler};
 use accesskit_atspi_common::{Adapter as AdapterImpl, AppContext, Event};
 #[cfg(not(feature = "tokio"))]
 use async_channel::{Receiver, Sender};
 use atspi::proxy::bus::StatusProxy;
 #[cfg(not(feature = "tokio"))]
 use futures_util::{pin_mut as pin, select, StreamExt};
-use once_cell::sync::OnceCell;
 use std::{
-    sync::{Arc, Mutex, RwLock},
+    sync::{Arc, Mutex, OnceLock, RwLock},
     thread,
 };
 #[cfg(feature = "tokio")]
 use tokio::{
     pin, select,
     sync::mpsc::{UnboundedReceiver as Receiver, UnboundedSender as Sender},
 };
@@ -27,16 +26,16 @@
 use crate::{
     adapter::{AdapterState, Callback, Message},
     atspi::{map_or_ignoring_broken_pipe, Bus},
     executor::Executor,
     util::block_on,
 };
 
-static APP_CONTEXT: OnceCell<Arc<RwLock<AppContext>>> = OnceCell::new();
-static MESSAGES: OnceCell<Sender<Message>> = OnceCell::new();
+static APP_CONTEXT: OnceLock<Arc<RwLock<AppContext>>> = OnceLock::new();
+static MESSAGES: OnceLock<Sender<Message>> = OnceLock::new();
 
 pub(crate) fn get_or_init_app_context<'a>() -> &'a Arc<RwLock<AppContext>> {
     APP_CONTEXT.get_or_init(AppContext::new)
 }
 
 pub(crate) fn get_or_init_messages() -> Sender<Message> {
     MESSAGES
```

### Comparing `accesskit-0.2.0/platforms/unix/src/executor.rs` & `accesskit-0.3.0/platforms/unix/src/executor.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.2.0/platforms/unix/src/lib.rs` & `accesskit-0.3.0/platforms/unix/src/lib.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.2.0/platforms/unix/src/util.rs` & `accesskit-0.3.0/platforms/unix/src/util.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.2.0/platforms/windows/Cargo.toml` & `accesskit-0.3.0/platforms/windows/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [package]
 name = "accesskit_windows"
-version = "0.17.0"
+version = "0.18.0"
 authors.workspace = true
 license.workspace = true
 description = "AccessKit UI accessibility infrastructure: Windows adapter"
 categories.workspace = true
 keywords = ["gui", "ui", "accessibility"]
 repository.workspace = true
 readme = "README.md"
 edition.workspace = true
 rust-version.workspace = true
 
 [dependencies]
-accesskit = { version = "0.13.0", path = "../../common" }
-accesskit_consumer = { version = "0.18.0", path = "../../consumer" }
+accesskit = { version = "0.14.0", path = "../../common" }
+accesskit_consumer = { version = "0.19.0", path = "../../consumer" }
 paste = "1.0"
 static_assertions = "1.1.0"
 
 [dependencies.windows]
 version = "0.54"
 features = [
     "implement",
@@ -31,8 +31,9 @@
     "Win32_UI_Input_KeyboardAndMouse",
     "Win32_UI_WindowsAndMessaging",
 ]
 
 [dev-dependencies]
 once_cell = "1.13.0"
 scopeguard = "1.1.0"
-winit = "0.29"
+winit = "0.30"
+
```

### Comparing `accesskit-0.2.0/platforms/windows/CHANGELOG.md` & `accesskit-0.3.0/platforms/windows/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,50 @@
     * accesskit_consumer bumped from 0.15.1 to 0.15.2
 
 * The following workspace dependencies were updated
   * dependencies
     * accesskit bumped from 0.12.2 to 0.12.3
     * accesskit_consumer bumped from 0.17.0 to 0.17.1
 
+## [0.18.0](https://github.com/AccessKit/accesskit/compare/accesskit_windows-v0.17.0...accesskit_windows-v0.18.0) (2024-04-30)
+
+
+### ⚠ BREAKING CHANGES
+
+* Update winit to 0.30 ([#397](https://github.com/AccessKit/accesskit/issues/397))
+* Clean up table roles and properties ([#393](https://github.com/AccessKit/accesskit/issues/393))
+* Drop `NodeClassSet` ([#389](https://github.com/AccessKit/accesskit/issues/389))
+* Rename `Checked` to `Toggled`; drop `ToggleButton` role ([#388](https://github.com/AccessKit/accesskit/issues/388))
+
+### Features
+
+* Expose the class name property ([#385](https://github.com/AccessKit/accesskit/issues/385)) ([53dcf2a](https://github.com/AccessKit/accesskit/commit/53dcf2ae47546273590c46a9b31b708aa1409837))
+* Implement the `description` property ([#382](https://github.com/AccessKit/accesskit/issues/382)) ([d49f406](https://github.com/AccessKit/accesskit/commit/d49f40660b5dc23ed074cd72a91e511b130756ae))
+
+
+### Bug Fixes
+
+* Increase minimum supported Rust version to `1.70` ([#396](https://github.com/AccessKit/accesskit/issues/396)) ([a8398b8](https://github.com/AccessKit/accesskit/commit/a8398b847aa003de91042ac45e33126fc2cae053))
+* Update winit to 0.30 ([#397](https://github.com/AccessKit/accesskit/issues/397)) ([de93be3](https://github.com/AccessKit/accesskit/commit/de93be387c03a438fbf598670207e578686e6bcf))
+
+
+### Code Refactoring
+
+* Clean up table roles and properties ([#393](https://github.com/AccessKit/accesskit/issues/393)) ([e34dad9](https://github.com/AccessKit/accesskit/commit/e34dad94448a5321ece9def3f2e054aa5f62dd79))
+* Drop `NodeClassSet` ([#389](https://github.com/AccessKit/accesskit/issues/389)) ([1b153ed](https://github.com/AccessKit/accesskit/commit/1b153ed51f8421cdba2dc98beca2e8f5f8c781bc))
+* Rename `Checked` to `Toggled`; drop `ToggleButton` role ([#388](https://github.com/AccessKit/accesskit/issues/388)) ([6bc040b](https://github.com/AccessKit/accesskit/commit/6bc040b7cf75cdbd6a019cc380d8dbce804b3c81))
+
+
+### Dependencies
+
+* The following workspace dependencies were updated
+  * dependencies
+    * accesskit bumped from 0.13.0 to 0.14.0
+    * accesskit_consumer bumped from 0.18.0 to 0.19.0
+
 ## [0.17.0](https://github.com/AccessKit/accesskit/compare/accesskit_windows-v0.16.4...accesskit_windows-v0.17.0) (2024-04-14)
 
 
 ### ⚠ BREAKING CHANGES
 
 * New approach to lazy initialization ([#375](https://github.com/AccessKit/accesskit/issues/375))
```

### Comparing `accesskit-0.2.0/platforms/windows/examples/hello_world.rs` & `accesskit-0.3.0/platforms/windows/examples/hello_world.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // Based on the create_window sample in windows-samples-rs.
 
 use accesskit::{
     Action, ActionHandler, ActionRequest, ActivationHandler, DefaultActionVerb, Live, Node,
-    NodeBuilder, NodeClassSet, NodeId, Rect, Role, Tree, TreeUpdate,
+    NodeBuilder, NodeId, Rect, Role, Tree, TreeUpdate,
 };
 use accesskit_windows::Adapter;
 use once_cell::sync::Lazy;
 use std::cell::RefCell;
 use windows::{
     core::*,
     Win32::{
@@ -57,76 +57,74 @@
     x1: 100.0,
     y1: 100.0,
 };
 
 const SET_FOCUS_MSG: u32 = WM_USER;
 const DO_DEFAULT_ACTION_MSG: u32 = WM_USER + 1;
 
-fn build_button(id: NodeId, name: &str, classes: &mut NodeClassSet) -> Node {
+fn build_button(id: NodeId, name: &str) -> Node {
     let rect = match id {
         BUTTON_1_ID => BUTTON_1_RECT,
         BUTTON_2_ID => BUTTON_2_RECT,
         _ => unreachable!(),
     };
 
     let mut builder = NodeBuilder::new(Role::Button);
     builder.set_bounds(rect);
     builder.set_name(name);
     builder.add_action(Action::Focus);
     builder.set_default_action_verb(DefaultActionVerb::Click);
-    builder.build(classes)
+    builder.build()
 }
 
-fn build_announcement(text: &str, classes: &mut NodeClassSet) -> Node {
+fn build_announcement(text: &str) -> Node {
     let mut builder = NodeBuilder::new(Role::StaticText);
     builder.set_name(text);
     builder.set_live(Live::Polite);
-    builder.build(classes)
+    builder.build()
 }
 
 struct InnerWindowState {
     focus: NodeId,
     announcement: Option<String>,
-    node_classes: NodeClassSet,
 }
 
 impl InnerWindowState {
     fn build_root(&mut self) -> Node {
         let mut builder = NodeBuilder::new(Role::Window);
         builder.set_children(vec![BUTTON_1_ID, BUTTON_2_ID]);
         if self.announcement.is_some() {
             builder.push_child(ANNOUNCEMENT_ID);
         }
-        builder.build(&mut self.node_classes)
+        builder.build()
     }
 }
 
 impl ActivationHandler for InnerWindowState {
     fn request_initial_tree(&mut self) -> Option<TreeUpdate> {
         println!("Initial tree requested");
         let root = self.build_root();
-        let button_1 = build_button(BUTTON_1_ID, "Button 1", &mut self.node_classes);
-        let button_2 = build_button(BUTTON_2_ID, "Button 2", &mut self.node_classes);
+        let button_1 = build_button(BUTTON_1_ID, "Button 1");
+        let button_2 = build_button(BUTTON_2_ID, "Button 2");
         let mut tree = Tree::new(WINDOW_ID);
         tree.app_name = Some("hello_world".to_string());
 
         let mut result = TreeUpdate {
             nodes: vec![
                 (WINDOW_ID, root),
                 (BUTTON_1_ID, button_1),
                 (BUTTON_2_ID, button_2),
             ],
             tree: Some(tree),
             focus: self.focus,
         };
         if let Some(announcement) = &self.announcement {
-            result.nodes.push((
-                ANNOUNCEMENT_ID,
-                build_announcement(announcement, &mut self.node_classes),
-            ));
+            result
+                .nodes
+                .push((ANNOUNCEMENT_ID, build_announcement(announcement)));
         }
         Some(result)
     }
 }
 
 struct WindowState {
     adapter: RefCell<Adapter>,
@@ -153,15 +151,15 @@
             "You pressed button 1"
         } else {
             "You pressed button 2"
         };
         inner_state.announcement = Some(text.into());
         let mut adapter = self.adapter.borrow_mut();
         if let Some(events) = adapter.update_if_active(|| {
-            let announcement = build_announcement(text, &mut inner_state.node_classes);
+            let announcement = build_announcement(text);
             let root = inner_state.build_root();
             TreeUpdate {
                 nodes: vec![(ANNOUNCEMENT_ID, announcement), (WINDOW_ID, root)],
                 tree: None,
                 focus: inner_state.focus,
             }
         }) {
@@ -227,15 +225,14 @@
             let create_struct: &CREATESTRUCTW = unsafe { &mut *(lparam.0 as *mut _) };
             let create_params: Box<WindowCreateParams> =
                 unsafe { Box::from_raw(create_struct.lpCreateParams as _) };
             let WindowCreateParams(initial_focus) = *create_params;
             let inner_state = RefCell::new(InnerWindowState {
                 focus: initial_focus,
                 announcement: None,
-                node_classes: NodeClassSet::new(),
             });
             let adapter = Adapter::new(window, false, SimpleActionHandler { window });
             let state = Box::new(WindowState {
                 adapter: RefCell::new(adapter),
                 inner_state,
             });
             unsafe { SetWindowLongPtrW(window, GWLP_USERDATA, Box::into_raw(state) as _) };
```

### Comparing `accesskit-0.2.0/platforms/windows/src/adapter.rs` & `accesskit-0.3.0/platforms/windows/src/adapter.rs`

 * *Files 1% similar despite different names*

```diff
@@ -335,18 +335,15 @@
                     let platform_node = PlatformNode::new(&context, node_id);
                     self.state = State::Active(context);
                     (hwnd, platform_node)
                 }
                 None => {
                     let hwnd = *hwnd;
                     let placeholder_update = TreeUpdate {
-                        nodes: vec![(
-                            PLACEHOLDER_ROOT_ID,
-                            NodeBuilder::new(Role::Window).build(&mut Default::default()),
-                        )],
+                        nodes: vec![(PLACEHOLDER_ROOT_ID, NodeBuilder::new(Role::Window).build())],
                         tree: Some(TreeData::new(PLACEHOLDER_ROOT_ID)),
                         focus: PLACEHOLDER_ROOT_ID,
                     };
                     let placeholder_tree = Tree::new(placeholder_update, false);
                     let placeholder_context = Context::new(
                         hwnd,
                         placeholder_tree,
```

### Comparing `accesskit-0.2.0/platforms/windows/src/context.rs` & `accesskit-0.3.0/platforms/windows/src/context.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.2.0/platforms/windows/src/node.rs` & `accesskit-0.3.0/platforms/windows/src/node.rs`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 // Copyright 2021 The Chromium Authors. All rights reserved.
 // Use of this source code is governed by a BSD-style license that can be
 // found in the LICENSE.chromium file.
 
 #![allow(non_upper_case_globals)]
 
 use accesskit::{
-    Action, ActionData, ActionRequest, Checked, Live, NodeId, NodeIdContent, Point, Role,
+    Action, ActionData, ActionRequest, Live, NodeId, NodeIdContent, Point, Role, Toggled,
 };
 use accesskit_consumer::{DetachedNode, FilterResult, Node, NodeState, TreeState};
 use paste::paste;
 use std::sync::{Arc, Weak};
 use windows::{
     core::*,
     Win32::{Foundation::*, System::Com::*, UI::Accessibility::*},
@@ -87,24 +87,21 @@
             | Role::PasswordInput
             | Role::PhoneNumberInput
             | Role::UrlInput => UIA_EditControlTypeId,
             Role::Button | Role::DefaultButton => UIA_ButtonControlTypeId,
             Role::Pane => UIA_PaneControlTypeId,
             Role::RowHeader => UIA_DataItemControlTypeId,
             Role::ColumnHeader => UIA_DataItemControlTypeId,
-            Role::Column => UIA_GroupControlTypeId,
             Role::RowGroup => UIA_GroupControlTypeId,
             Role::List => UIA_ListControlTypeId,
             Role::Table => UIA_TableControlTypeId,
-            Role::TableHeaderContainer => UIA_GroupControlTypeId,
             Role::LayoutTableCell => UIA_DataItemControlTypeId,
             Role::LayoutTableRow => UIA_DataItemControlTypeId,
             Role::LayoutTable => UIA_TableControlTypeId,
             Role::Switch => UIA_ButtonControlTypeId,
-            Role::ToggleButton => UIA_ButtonControlTypeId,
             Role::Menu => UIA_MenuControlTypeId,
             Role::Abbr => UIA_TextControlTypeId,
             Role::Alert => UIA_TextControlTypeId,
             Role::AlertDialog => {
                 // Chromium's implementation suggests the use of
                 // UIA_TextControlTypeId, not UIA_PaneControlTypeId, because some
                 // Windows screen readers are not compatible with
@@ -273,14 +270,21 @@
     fn name(&self) -> Option<String> {
         match self {
             Self::Node(node) => node.name(),
             Self::DetachedNode(node) => node.name(),
         }
     }
 
+    fn description(&self) -> Option<String> {
+        match self {
+            Self::Node(node) => node.description(),
+            Self::DetachedNode(node) => node.description(),
+        }
+    }
+
     fn is_content_element(&self) -> bool {
         let result = match self {
             Self::Node(node) => filter(node),
             Self::DetachedNode(node) => filter_detached(node),
         };
         result == FilterResult::Include
     }
@@ -308,23 +312,27 @@
         match live {
             Live::Off => Off,
             Live::Polite => Polite,
             Live::Assertive => Assertive,
         }
     }
 
+    fn class_name(&self) -> Option<&str> {
+        self.node_state().class_name()
+    }
+
     fn is_toggle_pattern_supported(&self) -> bool {
-        self.node_state().checked().is_some() && !self.is_selection_item_pattern_supported()
+        self.node_state().toggled().is_some() && !self.is_selection_item_pattern_supported()
     }
 
     fn toggle_state(&self) -> ToggleState {
-        match self.node_state().checked().unwrap() {
-            Checked::False => ToggleState_Off,
-            Checked::True => ToggleState_On,
-            Checked::Mixed => ToggleState_Indeterminate,
+        match self.node_state().toggled().unwrap() {
+            Toggled::False => ToggleState_Off,
+            Toggled::True => ToggleState_On,
+            Toggled::Mixed => ToggleState_Indeterminate,
         }
     }
 
     fn is_invoke_pattern_supported(&self) -> bool {
         self.node_state().is_invocable()
     }
 
@@ -375,16 +383,16 @@
     fn is_selection_item_pattern_supported(&self) -> bool {
         match self.node_state().role() {
             // TODO: tables (#29)
             // https://www.w3.org/TR/core-aam-1.1/#mapping_state-property_table
             // SelectionItem.IsSelected is exposed when aria-checked is True or
             // False, for 'radio' and 'menuitemradio' roles.
             Role::RadioButton | Role::MenuItemRadio => matches!(
-                self.node_state().checked(),
-                Some(Checked::True | Checked::False)
+                self.node_state().toggled(),
+                Some(Toggled::True | Toggled::False)
             ),
             // https://www.w3.org/TR/wai-aria-1.1/#aria-selected
             // SelectionItem.IsSelected is exposed when aria-select is True or False.
             Role::ListBoxOption
             | Role::ListItem
             | Role::MenuListOption
             | Role::Tab
@@ -395,15 +403,15 @@
 
     fn is_selected(&self) -> bool {
         match self.node_state().role() {
             // https://www.w3.org/TR/core-aam-1.1/#mapping_state-property_table
             // SelectionItem.IsSelected is set according to the True or False
             // value of aria-checked for 'radio' and 'menuitemradio' roles.
             Role::RadioButton | Role::MenuItemRadio => {
-                self.node_state().checked() == Some(Checked::True)
+                self.node_state().toggled() == Some(Toggled::True)
             }
             // https://www.w3.org/TR/wai-aria-1.1/#aria-selected
             // SelectionItem.IsSelected is set according to the True or False
             // value of aria-selected.
             _ => self.node_state().is_selected().unwrap_or(false),
         }
     }
@@ -843,20 +851,22 @@
     };
 }
 
 properties! {
     (ControlType, control_type),
     (LocalizedControlType, localized_control_type),
     (Name, name),
+    (FullDescription, description),
     (IsContentElement, is_content_element),
     (IsControlElement, is_content_element),
     (IsEnabled, is_enabled),
     (IsKeyboardFocusable, is_focusable),
     (HasKeyboardFocus, is_focused),
-    (LiveSetting, live_setting)
+    (LiveSetting, live_setting),
+    (ClassName, class_name)
 }
 
 patterns! {
     (Toggle, is_toggle_pattern_supported, (
         (ToggleState, toggle_state, ToggleState)
     ), (
         fn Toggle(&self) -> Result<()> {
```

### Comparing `accesskit-0.2.0/platforms/windows/src/subclass.rs` & `accesskit-0.3.0/platforms/windows/src/subclass.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.2.0/platforms/windows/src/tests/mod.rs` & `accesskit-0.3.0/platforms/windows/src/tests/mod.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.2.0/platforms/windows/src/tests/simple.rs` & `accesskit-0.3.0/platforms/windows/src/tests/simple.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 // Copyright 2022 The AccessKit Authors. All rights reserved.
 // Licensed under the Apache License, Version 2.0 (found in
 // the LICENSE-APACHE file) or the MIT license (found in
 // the LICENSE-MIT file), at your option.
 
 use accesskit::{
-    Action, ActionHandler, ActionRequest, ActivationHandler, Node, NodeBuilder, NodeClassSet,
-    NodeId, Role, Tree, TreeUpdate,
+    Action, ActionHandler, ActionRequest, ActivationHandler, Node, NodeBuilder, NodeId, Role, Tree,
+    TreeUpdate,
 };
 use windows::{core::*, Win32::UI::Accessibility::*};
 
 use super::*;
 
 const WINDOW_TITLE: &str = "Simple test";
 
 const WINDOW_ID: NodeId = NodeId(0);
 const BUTTON_1_ID: NodeId = NodeId(1);
 const BUTTON_2_ID: NodeId = NodeId(2);
 
-fn make_button(name: &str, classes: &mut NodeClassSet) -> Node {
+fn make_button(name: &str) -> Node {
     let mut builder = NodeBuilder::new(Role::Button);
     builder.set_name(name);
     builder.add_action(Action::Focus);
-    builder.build(classes)
+    builder.build()
 }
 
 fn get_initial_state() -> TreeUpdate {
-    let mut classes = NodeClassSet::new();
     let root = {
         let mut builder = NodeBuilder::new(Role::Window);
         builder.set_children(vec![BUTTON_1_ID, BUTTON_2_ID]);
-        builder.build(&mut classes)
+        builder.build()
     };
-    let button_1 = make_button("Button 1", &mut classes);
-    let button_2 = make_button("Button 2", &mut classes);
+    let button_1 = make_button("Button 1");
+    let button_2 = make_button("Button 2");
     TreeUpdate {
         nodes: vec![
             (WINDOW_ID, root),
             (BUTTON_1_ID, button_1),
             (BUTTON_2_ID, button_2),
         ],
         tree: Some(Tree::new(WINDOW_ID)),
```

### Comparing `accesskit-0.2.0/platforms/windows/src/tests/subclassed.rs` & `accesskit-0.3.0/platforms/windows/src/tests/subclassed.rs`

 * *Files 21% similar despite different names*

```diff
@@ -1,50 +1,51 @@
 // Copyright 2022 The AccessKit Authors. All rights reserved.
 // Licensed under the Apache License, Version 2.0 (found in
 // the LICENSE-APACHE file) or the MIT license (found in
 // the LICENSE-MIT file), at your option.
 
 use accesskit::{
-    Action, ActionHandler, ActionRequest, ActivationHandler, Node, NodeBuilder, NodeClassSet,
-    NodeId, Role, Tree, TreeUpdate,
+    Action, ActionHandler, ActionRequest, ActivationHandler, Node, NodeBuilder, NodeId, Role, Tree,
+    TreeUpdate,
 };
 use windows::Win32::{Foundation::*, UI::Accessibility::*};
 use winit::{
-    event_loop::EventLoopBuilder,
+    application::ApplicationHandler,
+    event::WindowEvent,
+    event_loop::{ActiveEventLoop, EventLoop},
     platform::windows::EventLoopBuilderExtWindows,
     raw_window_handle::{HasWindowHandle, RawWindowHandle},
-    window::WindowBuilder,
+    window::{Window, WindowId},
 };
 
 use super::MUTEX;
 use crate::SubclassingAdapter;
 
 const WINDOW_TITLE: &str = "Simple test";
 
 const WINDOW_ID: NodeId = NodeId(0);
 const BUTTON_1_ID: NodeId = NodeId(1);
 const BUTTON_2_ID: NodeId = NodeId(2);
 
-fn make_button(name: &str, classes: &mut NodeClassSet) -> Node {
+fn make_button(name: &str) -> Node {
     let mut builder = NodeBuilder::new(Role::Button);
     builder.set_name(name);
     builder.add_action(Action::Focus);
-    builder.build(classes)
+    builder.build()
 }
 
 fn get_initial_state() -> TreeUpdate {
-    let mut classes = NodeClassSet::new();
     let root = {
         let mut builder = NodeBuilder::new(Role::Window);
         builder.set_children(vec![BUTTON_1_ID, BUTTON_2_ID]);
         builder.set_name(WINDOW_TITLE);
-        builder.build(&mut classes)
+        builder.build()
     };
-    let button_1 = make_button("Button 1", &mut classes);
-    let button_2 = make_button("Button 2", &mut classes);
+    let button_1 = make_button("Button 1");
+    let button_2 = make_button("Button 2");
     TreeUpdate {
         nodes: vec![
             (WINDOW_ID, root),
             (BUTTON_1_ID, button_1),
             (BUTTON_2_ID, button_2),
         ],
         tree: Some(Tree::new(WINDOW_ID)),
@@ -65,33 +66,43 @@
         Some(get_initial_state())
     }
 }
 
 // This module uses winit for the purpose of testing with a real third-party
 // window implementation that we don't control.
 
+struct TestApplication;
+
+impl ApplicationHandler<()> for TestApplication {
+    fn window_event(&mut self, _: &ActiveEventLoop, _: WindowId, _: WindowEvent) {}
+
+    fn resumed(&mut self, event_loop: &ActiveEventLoop) {
+        let window_attributes = Window::default_attributes()
+            .with_title(WINDOW_TITLE)
+            .with_visible(false);
+
+        let window = event_loop.create_window(window_attributes).unwrap();
+        let hwnd = match window.window_handle().unwrap().as_raw() {
+            RawWindowHandle::Win32(handle) => HWND(handle.hwnd.get()),
+            RawWindowHandle::WinRt(_) => unimplemented!(),
+            _ => unreachable!(),
+        };
+        let adapter =
+            SubclassingAdapter::new(hwnd, SimpleActivationHandler {}, NullActionHandler {});
+        assert!(unsafe { UiaHasServerSideProvider(hwnd) }.as_bool());
+        drop(window);
+        drop(adapter);
+        event_loop.exit();
+    }
+}
+
 #[test]
 fn has_native_uia() {
     // This test is simple enough that we know it's fine to run entirely
     // on one thread, so we don't need a full multithreaded test harness.
     // Still, we must prevent this test from running concurrently with other
     // tests, especially the focus test.
     let _lock_guard = MUTEX.lock().unwrap();
-    let event_loop = EventLoopBuilder::<()>::new()
-        .with_any_thread(true)
-        .build()
-        .unwrap();
-    let window = WindowBuilder::new()
-        .with_title(WINDOW_TITLE)
-        .with_visible(false)
-        .build(&event_loop)
-        .unwrap();
-    let hwnd = match window.window_handle().unwrap().as_raw() {
-        RawWindowHandle::Win32(handle) => HWND(handle.hwnd.get()),
-        RawWindowHandle::WinRt(_) => unimplemented!(),
-        _ => unreachable!(),
-    };
-    let adapter = SubclassingAdapter::new(hwnd, SimpleActivationHandler {}, NullActionHandler {});
-    assert!(unsafe { UiaHasServerSideProvider(hwnd) }.as_bool());
-    drop(window);
-    drop(adapter);
+    let event_loop = EventLoop::builder().with_any_thread(true).build().unwrap();
+    let mut state = TestApplication {};
+    event_loop.run_app(&mut state).unwrap();
 }
```

### Comparing `accesskit-0.2.0/platforms/windows/src/text.rs` & `accesskit-0.3.0/platforms/windows/src/text.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.2.0/platforms/windows/src/util.rs` & `accesskit-0.3.0/platforms/windows/src/util.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.2.0/bindings/python/Cargo.toml` & `accesskit-0.3.0/bindings/python/Cargo.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "accesskit_python"
-version = "0.2.0"
+version = "0.3.0"
 authors.workspace = true
 license.workspace = true
 description = "Python bindings to the AccessKit library"
 readme = "README.md"
 publish = false
 edition.workspace = true
 
@@ -13,19 +13,18 @@
 crate-type = ["cdylib"]
 doc = false
 
 [features]
 extension-module = ["pyo3/extension-module"]
 
 [dependencies]
-accesskit = { version = "0.13.0", path = "../../common", features = ["pyo3"] }
+accesskit = { version = "0.14.0", path = "../../common", features = ["pyo3"] }
 pyo3 = { version = "0.20", features = ["abi3-py38", "multiple-pymethods"] }
 
 [target.'cfg(target_os = "windows")'.dependencies]
-accesskit_windows = { version = "0.17.0", path = "../../platforms/windows" }
+accesskit_windows = { version = "0.18.0", path = "../../platforms/windows" }
 
 [target.'cfg(target_os = "macos")'.dependencies]
-accesskit_macos = { version = "0.12.0", path = "../../platforms/macos" }
+accesskit_macos = { version = "0.13.0", path = "../../platforms/macos" }
 
 [target.'cfg(any(target_os = "linux", target_os = "dragonfly", target_os = "freebsd", target_os = "openbsd", target_os = "netbsd"))'.dependencies]
-accesskit_unix = { version = "0.8.0", path = "../../platforms/unix" }
-
+accesskit_unix = { version = "0.9.0", path = "../../platforms/unix" }
```

### Comparing `accesskit-0.2.0/bindings/python/README.md` & `accesskit-0.3.0/bindings/python/README.md`

 * *Files identical despite different names*

### Comparing `accesskit-0.2.0/bindings/python/examples/pygame/.gitignore` & `accesskit-0.3.0/bindings/python/examples/pygame/.gitignore`

 * *Files identical despite different names*

### Comparing `accesskit-0.2.0/bindings/python/examples/pygame/hello_world.py` & `accesskit-0.3.0/bindings/python/examples/pygame/hello_world.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,28 +20,28 @@
 BUTTON_2_RECT = accesskit.Rect(20.0, 60.0, 100.0, 100.0)
 
 ACCESSKIT_EVENT = pygame.event.custom_type()
 SET_FOCUS_MSG = 0
 DO_DEFAULT_ACTION_MSG = 1
 
 
-def build_button(id, name, classes):
+def build_button(id, name):
     builder = accesskit.NodeBuilder(accesskit.Role.BUTTON)
     builder.set_bounds(BUTTON_1_RECT if id == BUTTON_1_ID else BUTTON_2_RECT)
     builder.set_name(name)
     builder.add_action(accesskit.Action.FOCUS)
     builder.set_default_action_verb(accesskit.DefaultActionVerb.CLICK)
-    return builder.build(classes)
+    return builder.build()
 
 
-def build_announcement(text, classes):
+def build_announcement(text):
     builder = accesskit.NodeBuilder(accesskit.Role.STATIC_TEXT)
     builder.set_name(text)
     builder.set_live(accesskit.Live.POLITE)
-    return builder.build(classes)
+    return builder.build()
 
 
 class PygameAdapter:
     def __init__(self, activation_handler, action_handler, deactivation_handler):
         if PLATFORM_SYSTEM == "Darwin":
             accesskit.macos.add_focus_forwarder_to_window_class("SDLWindow")
             window = pygame.display.get_wm_info()["window"]
@@ -72,55 +72,52 @@
             self.adapter.update_window_focus_state(is_focused)
 
 
 class WindowState:
     def __init__(self):
         self.focus = INITIAL_FOCUS
         self.announcement = None
-        self.node_classes = accesskit.NodeClassSet()
 
     def build_root(self):
         builder = accesskit.NodeBuilder(accesskit.Role.WINDOW)
         builder.set_children([BUTTON_1_ID, BUTTON_2_ID])
         if self.announcement is not None:
             builder.push_child(ANNOUNCEMENT_ID)
         builder.set_name(WINDOW_TITLE)
-        return builder.build(self.node_classes)
+        return builder.build()
 
     def build_initial_tree(self):
         root = self.build_root()
-        button_1 = build_button(BUTTON_1_ID, "Button 1", self.node_classes)
-        button_2 = build_button(BUTTON_2_ID, "Button 2", self.node_classes)
+        button_1 = build_button(BUTTON_1_ID, "Button 1")
+        button_2 = build_button(BUTTON_2_ID, "Button 2")
         result = accesskit.TreeUpdate(self.focus)
         tree = accesskit.Tree(WINDOW_ID)
         tree.app_name = "Hello world"
         result.tree = tree
         result.nodes.append((WINDOW_ID, root))
         result.nodes.append((BUTTON_1_ID, button_1))
         result.nodes.append((BUTTON_2_ID, button_2))
         if self.announcement is not None:
             result.nodes.append(
                 (
                     ANNOUNCEMENT_ID,
-                    build_announcement(self.announcement, self.node_classes),
+                    build_announcement(self.announcement),
                 )
             )
         return result
 
     def press_button(self, adapter, id):
         self.announcement = (
             "You pressed button 1" if id == BUTTON_1_ID else "You pressed button 2"
         )
         adapter.update_if_active(self.build_tree_update_for_button_press)
 
     def build_tree_update_for_button_press(self):
         update = accesskit.TreeUpdate(self.focus)
-        update.nodes.append(
-            (ANNOUNCEMENT_ID, build_announcement(self.announcement, self.node_classes))
-        )
+        update.nodes.append((ANNOUNCEMENT_ID, build_announcement(self.announcement)))
         update.nodes.append((WINDOW_ID, self.build_root()))
         return update
 
     def set_focus(self, adapter, focus):
         self.focus = focus
         adapter.update_if_active(self.build_tree_update_for_focus_update)
```

### Comparing `accesskit-0.2.0/bindings/python/src/common.rs` & `accesskit-0.3.0/bindings/python/src/common.rs`

 * *Files 6% similar despite different names*

```diff
@@ -2,25 +2,14 @@
 // Licensed under the Apache License, Version 2.0 (found in
 // the LICENSE-APACHE file) or the MIT license (found in
 // the LICENSE-MIT file), at your option.
 
 use crate::{Point, Rect};
 use pyo3::{prelude::*, types::PyList};
 
-#[pyclass(module = "accesskit")]
-pub struct NodeClassSet(accesskit::NodeClassSet);
-
-#[pymethods]
-impl NodeClassSet {
-    #[new]
-    pub fn __new__() -> Self {
-        Self(accesskit::NodeClassSet::new())
-    }
-}
-
 #[derive(Clone)]
 #[pyclass(module = "accesskit")]
 pub struct Node(accesskit::Node);
 
 impl Node {
     #[inline]
     fn inner(&self) -> &accesskit::Node {
@@ -64,17 +53,17 @@
 #[pymethods]
 impl NodeBuilder {
     #[new]
     pub fn new(role: accesskit::Role) -> NodeBuilder {
         Self(Some(accesskit::NodeBuilder::new(role)))
     }
 
-    pub fn build(&mut self, classes: &mut NodeClassSet) -> Node {
+    pub fn build(&mut self) -> Node {
         let builder = self.0.take().unwrap();
-        Node(builder.build(&mut classes.0))
+        Node(builder.build())
     }
 
     #[getter]
     pub fn role(&self) -> accesskit::Role {
         self.inner().role()
     }
 
@@ -476,28 +465,26 @@
 node_id_vec_property_methods! {
     (children, set_children, push_child, clear_children),
     (controls, set_controls, push_controlled, clear_controls),
     (details, set_details, push_detail, clear_details),
     (described_by, set_described_by, push_described_by, clear_described_by),
     (flow_to, set_flow_to, push_flow_to, clear_flow_to),
     (labelled_by, set_labelled_by, push_labelled_by, clear_labelled_by),
+    (owns, set_owns, push_owned, clear_owns),
     (radio_group, set_radio_group, push_to_radio_group, clear_radio_group)
 }
 
 node_id_property_methods! {
     (active_descendant, set_active_descendant, clear_active_descendant),
     (error_message, set_error_message, clear_error_message),
     (in_page_link_target, set_in_page_link_target, clear_in_page_link_target),
     (member_of, set_member_of, clear_member_of),
     (next_on_line, set_next_on_line, clear_next_on_line),
     (previous_on_line, set_previous_on_line, clear_previous_on_line),
-    (popup_for, set_popup_for, clear_popup_for),
-    (table_header, set_table_header, clear_table_header),
-    (table_row_header, set_table_row_header, clear_table_row_header),
-    (table_column_header, set_table_column_header, clear_table_column_header)
+    (popup_for, set_popup_for, clear_popup_for)
 }
 
 string_property_methods! {
     (name, set_name, clear_name),
     (description, set_description, clear_description),
     (value, set_value, clear_value),
     (access_key, set_access_key, clear_access_key),
@@ -507,15 +494,17 @@
     (inner_html, set_inner_html, clear_inner_html),
     (keyboard_shortcut, set_keyboard_shortcut, clear_keyboard_shortcut),
     (language, set_language, clear_language),
     (placeholder, set_placeholder, clear_placeholder),
     (role_description, set_role_description, clear_role_description),
     (state_description, set_state_description, clear_state_description),
     (tooltip, set_tooltip, clear_tooltip),
-    (url, set_url, clear_url)
+    (url, set_url, clear_url),
+    (row_index_text, set_row_index_text, clear_row_index_text),
+    (column_index_text, set_column_index_text, clear_column_index_text)
 }
 
 f64_property_methods! {
     (scroll_x, set_scroll_x, clear_scroll_x),
     (scroll_x_min, set_scroll_x_min, clear_scroll_x_min),
     (scroll_x_max, set_scroll_x_max, clear_scroll_x_max),
     (scroll_y, set_scroll_y, clear_scroll_y),
@@ -527,23 +516,21 @@
     (numeric_value_step, set_numeric_value_step, clear_numeric_value_step),
     (numeric_value_jump, set_numeric_value_jump, clear_numeric_value_jump),
     (font_size, set_font_size, clear_font_size),
     (font_weight, set_font_weight, clear_font_weight)
 }
 
 usize_property_methods! {
-    (table_row_count, set_table_row_count, clear_table_row_count),
-    (table_column_count, set_table_column_count, clear_table_column_count),
-    (table_row_index, set_table_row_index, clear_table_row_index),
-    (table_column_index, set_table_column_index, clear_table_column_index),
-    (table_cell_column_index, set_table_cell_column_index, clear_table_cell_column_index),
-    (table_cell_column_span, set_table_cell_column_span, clear_table_cell_column_span),
-    (table_cell_row_index, set_table_cell_row_index, clear_table_cell_row_index),
-    (table_cell_row_span, set_table_cell_row_span, clear_table_cell_row_span),
-    (hierarchical_level, set_hierarchical_level, clear_hierarchical_level),
+    (row_count, set_row_count, clear_row_count),
+    (column_count, set_column_count, clear_column_count),
+    (row_index, set_row_index, clear_row_index),
+    (column_index, set_column_index, clear_column_index),
+    (row_span, set_row_span, clear_row_span),
+    (column_span, set_column_span, clear_column_span),
+    (level, set_level, clear_level),
     (size_of_set, set_size_of_set, clear_size_of_set),
     (position_in_set, set_position_in_set, clear_position_in_set)
 }
 
 color_property_methods! {
     (color_value, set_color_value, clear_color_value),
     (background_color, set_background_color, clear_background_color),
@@ -569,15 +556,15 @@
 bool_property_methods! {
     (is_expanded, set_expanded, clear_expanded),
     (is_selected, set_selected, clear_selected)
 }
 
 unique_enum_property_methods! {
     (accesskit::Invalid, invalid, set_invalid, clear_invalid),
-    (accesskit::Checked, checked, set_checked, clear_checked),
+    (accesskit::Toggled, toggled, set_toggled, clear_toggled),
     (accesskit::Live, live, set_live, clear_live),
     (accesskit::DefaultActionVerb, default_action_verb, set_default_action_verb, clear_default_action_verb),
     (accesskit::TextDirection, text_direction, set_text_direction, clear_text_direction),
     (accesskit::Orientation, orientation, set_orientation, clear_orientation),
     (accesskit::SortDirection, sort_direction, set_sort_direction, clear_sort_direction),
     (accesskit::AriaCurrent, aria_current, set_aria_current, clear_aria_current),
     (accesskit::AutoComplete, auto_complete, set_auto_complete, clear_auto_complete),
```

### Comparing `accesskit-0.2.0/bindings/python/src/geometry.rs` & `accesskit-0.3.0/bindings/python/src/geometry.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.2.0/bindings/python/src/lib.rs` & `accesskit-0.3.0/bindings/python/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -27,25 +27,24 @@
 #[pymodule]
 fn accesskit(py: Python<'_>, m: &PyModule) -> PyResult<()> {
     m.add_class::<::accesskit::Role>()?;
     m.add_class::<::accesskit::Action>()?;
     m.add_class::<::accesskit::Orientation>()?;
     m.add_class::<::accesskit::TextDirection>()?;
     m.add_class::<::accesskit::Invalid>()?;
-    m.add_class::<::accesskit::Checked>()?;
+    m.add_class::<::accesskit::Toggled>()?;
     m.add_class::<::accesskit::DefaultActionVerb>()?;
     m.add_class::<::accesskit::SortDirection>()?;
     m.add_class::<::accesskit::AriaCurrent>()?;
     m.add_class::<::accesskit::Live>()?;
     m.add_class::<::accesskit::HasPopup>()?;
     m.add_class::<::accesskit::ListStyle>()?;
     m.add_class::<::accesskit::TextAlign>()?;
     m.add_class::<::accesskit::VerticalOffset>()?;
     m.add_class::<::accesskit::TextDecoration>()?;
-    m.add_class::<NodeClassSet>()?;
     m.add_class::<Node>()?;
     m.add_class::<NodeBuilder>()?;
     m.add_class::<Tree>()?;
     m.add_class::<TreeUpdate>()?;
     m.add_class::<ActionDataKind>()?;
     m.add_class::<ActionRequest>()?;
     m.add_class::<Affine>()?;
```

### Comparing `accesskit-0.2.0/bindings/python/src/macos.rs` & `accesskit-0.3.0/bindings/python/src/macos.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.2.0/bindings/python/src/unix.rs` & `accesskit-0.3.0/bindings/python/src/unix.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.2.0/bindings/python/src/windows.rs` & `accesskit-0.3.0/bindings/python/src/windows.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.2.0/Cargo.lock` & `accesskit-0.3.0/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -16,110 +16,110 @@
 name = "ab_glyph_rasterizer"
 version = "0.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c71b1793ee61086797f5c80b6efa2b8ffa6d5dd703f118545808a7f2e27f7046"
 
 [[package]]
 name = "accesskit"
-version = "0.13.0"
+version = "0.14.0"
 dependencies = [
  "enumn",
  "pyo3",
  "schemars",
  "serde",
 ]
 
 [[package]]
 name = "accesskit_atspi_common"
-version = "0.3.0"
+version = "0.4.0"
 dependencies = [
  "accesskit",
  "accesskit_consumer",
  "atspi-common",
  "serde",
  "thiserror",
  "zvariant",
 ]
 
 [[package]]
 name = "accesskit_c"
-version = "0.8.0"
+version = "0.9.0"
 dependencies = [
  "accesskit",
  "accesskit_macos",
  "accesskit_unix",
  "accesskit_windows",
  "paste",
 ]
 
 [[package]]
 name = "accesskit_consumer"
-version = "0.18.0"
+version = "0.19.0"
 dependencies = [
  "accesskit",
 ]
 
 [[package]]
 name = "accesskit_macos"
-version = "0.12.0"
+version = "0.13.0"
 dependencies = [
  "accesskit",
  "accesskit_consumer",
- "icrate 0.1.0",
- "objc2 0.5.0",
+ "objc2",
+ "objc2-app-kit",
+ "objc2-foundation",
  "once_cell",
 ]
 
 [[package]]
 name = "accesskit_python"
-version = "0.2.0"
+version = "0.3.0"
 dependencies = [
  "accesskit",
  "accesskit_macos",
  "accesskit_unix",
  "accesskit_windows",
  "pyo3",
 ]
 
 [[package]]
 name = "accesskit_unix"
-version = "0.8.0"
+version = "0.9.0"
 dependencies = [
  "accesskit",
  "accesskit_atspi_common",
  "async-channel 2.1.1",
  "async-executor",
  "async-task",
  "atspi",
  "futures-lite",
  "futures-util",
- "once_cell",
  "serde",
  "tokio",
  "tokio-stream",
  "zbus",
 ]
 
 [[package]]
 name = "accesskit_windows"
-version = "0.17.0"
+version = "0.18.0"
 dependencies = [
  "accesskit",
  "accesskit_consumer",
  "once_cell",
  "paste",
  "scopeguard",
  "static_assertions",
  "windows",
  "winit",
 ]
 
 [[package]]
 name = "accesskit_winit"
-version = "0.19.0"
+version = "0.20.0"
 dependencies = [
  "accesskit",
  "accesskit_macos",
  "accesskit_unix",
  "accesskit_windows",
  "raw-window-handle 0.5.2",
  "raw-window-handle 0.6.0",
@@ -139,17 +139,17 @@
 name = "adler"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
 
 [[package]]
 name = "ahash"
-version = "0.8.6"
+version = "0.8.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "91429305e9f0a25f6205c5b8e0d2db09e0708a7a6df0f42212bb56c32c8ac97a"
+checksum = "e89da841a80418a9b391ebaea17f5c112ffaaa96f621d2c285b5174da76b9011"
 dependencies = [
  "cfg-if",
  "getrandom",
  "once_cell",
  "version_check",
  "zerocopy",
 ]
@@ -161,17 +161,17 @@
 checksum = "cc936419f96fa211c1b9166887b38e5e40b19958e5b895be7c1f93adec7071ac"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "android-activity"
-version = "0.5.0"
+version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "052ad56e336bcc615a214bffbeca6c181ee9550acec193f0327e0b103b033a4d"
+checksum = "ef6978589202a00cd7e118380c448a08b6ed394c3a8df3a430d0898e3a42d046"
 dependencies = [
  "android-properties",
  "bitflags 2.4.1",
  "cc",
  "cesu8",
  "jni",
  "jni-sys",
@@ -436,40 +436,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3078c7629b62d3f0439517fa394996acacc5cbc91c5a20d8c658e77abd503a71"
 dependencies = [
  "generic-array",
 ]
 
 [[package]]
-name = "block-sys"
-version = "0.2.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2dd7cf50912cddc06dc5ea7c08c5e81c1b2c842a70d19def1848d54c586fed92"
-dependencies = [
- "objc-sys",
-]
-
-[[package]]
-name = "block2"
-version = "0.3.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "15b55663a85f33501257357e6421bb33e769d5c9ffb5ba0921c975a123e35e68"
-dependencies = [
- "block-sys",
- "objc2 0.4.1",
-]
-
-[[package]]
 name = "block2"
-version = "0.4.0"
+version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e58aa60e59d8dbfcc36138f5f18be5f24394d33b38b24f7fd0b1caa33095f22f"
+checksum = "43ff7d91d3c1d568065b06c899777d1e48dcf76103a672a0adbc238a7f247f1e"
 dependencies = [
- "block-sys",
- "objc2 0.5.0",
+ "objc2",
 ]
 
 [[package]]
 name = "blocking"
 version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c67b173a56acffd6d2326fb7ab938ba0b00a71480e14902b2591c87bc5741e8"
@@ -551,17 +531,17 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "cfg_aliases"
-version = "0.1.1"
+version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd16c4719339c4530435d38e511904438d07cce7950afa3718a84ac36c10e89e"
+checksum = "77e53693616d3075149f4ead59bdeecd204ac6b8192d8969757601b74bddf00f"
 
 [[package]]
 name = "combine"
 version = "4.6.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "35ed6e9d84f0b51a7f52daf1c7d71dd136fd7a3f41a8462b8cdb8c78d920fad4"
 dependencies = [
@@ -682,24 +662,30 @@
 
 [[package]]
 name = "dlib"
 version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "330c60081dcc4c72131f8eb70510f1ac07223e5d4163db481a04a0befcffa412"
 dependencies = [
- "libloading",
+ "libloading 0.7.4",
 ]
 
 [[package]]
 name = "downcast-rs"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ea835d29036a4087793836fa931b08837ad5e957da9e23886b29586fb9b6650"
 
 [[package]]
+name = "dpi"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f25c0e292a7ca6d6498557ff1df68f32c99850012b6ea401cf8daf771f22ff53"
+
+[[package]]
 name = "dyn-clone"
 version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "68b0cf012f1230e43cd00ebb729c6bb58707ecfa8ad08b52ef3a4ccd2697fc30"
 
 [[package]]
 name = "enumflags2"
@@ -918,20 +904,20 @@
 dependencies = [
  "typenum",
  "version_check",
 ]
 
 [[package]]
 name = "gethostname"
-version = "0.3.0"
+version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bb65d4ba3173c56a500b555b532f72c42e8d1fe64962b518897f8959fae2c177"
+checksum = "0176e0459c2e4a1fe232f984bca6890e681076abb9934f6cea7c326f3fc47818"
 dependencies = [
  "libc",
- "winapi",
+ "windows-targets 0.48.1",
 ]
 
 [[package]]
 name = "getrandom"
 version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c05aeb6a22b8f62540c194aac980f2115af067bfe15a0734d7277a768d396b31"
@@ -968,35 +954,14 @@
 [[package]]
 name = "hex"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7f24254aa9a54b5c858eaee2f5bccdb46aaf0e486a595ed5fd8f86ba55232a70"
 
 [[package]]
-name = "icrate"
-version = "0.0.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "99d3aaff8a54577104bafdf686ff18565c3b6903ca5782a2026ef06e2c7aa319"
-dependencies = [
- "block2 0.3.0",
- "dispatch",
- "objc2 0.4.1",
-]
-
-[[package]]
-name = "icrate"
-version = "0.1.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e286f4b975ac6c054971a0600a9b76438b332edace54bff79c71c9d3adfc9772"
-dependencies = [
- "block2 0.4.0",
- "objc2 0.5.0",
-]
-
-[[package]]
 name = "indexmap"
 version = "1.9.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1885e79c1fc4b10f0e172c475f458b7f7b93061064d98c3293e98c5ba0c8b399"
 dependencies = [
  "autocfg",
  "hashbrown",
@@ -1093,14 +1058,35 @@
 checksum = "b67380fd3b2fbe7527a606e18729d21c6f3951633d0500574c4dc22d2d638b9f"
 dependencies = [
  "cfg-if",
  "winapi",
 ]
 
 [[package]]
+name = "libloading"
+version = "0.8.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0c2a198fb6b0eada2a8df47933734e6d35d350665a33a3593d7164fa52c75c19"
+dependencies = [
+ "cfg-if",
+ "windows-targets 0.52.3",
+]
+
+[[package]]
+name = "libredox"
+version = "0.0.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3af92c55d7d839293953fcd0fda5ecfe93297cfde6ffbdec13b41d99c0ba6607"
+dependencies = [
+ "bitflags 2.4.1",
+ "libc",
+ "redox_syscall 0.4.1",
+]
+
+[[package]]
 name = "linux-raw-sys"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f051f77a7c8e6957c0696eac88f26b0117e54f52d3fc682ab19397a8812846a4"
 
 [[package]]
 name = "linux-raw-sys"
@@ -1190,17 +1176,17 @@
  "libc",
  "wasi",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "ndk"
-version = "0.8.0"
+version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2076a31b7010b17a38c01907c45b945e8f11495ee4dd588309718901b1f7a5b7"
+checksum = "c3f42e7bbe13d351b6bead8286a43aac9534b82bd3cc43e47037f012ebfd62d4"
 dependencies = [
  "bitflags 2.4.1",
  "jni-sys",
  "log",
  "ndk-sys",
  "num_enum",
  "raw-window-handle 0.5.2",
@@ -1212,17 +1198,17 @@
 name = "ndk-context"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "27b02d87554356db9e9a873add8782d4ea6e3e58ea071a9adb9a2e8ddb884a8b"
 
 [[package]]
 name = "ndk-sys"
-version = "0.5.0+25.2.9519653"
+version = "0.6.0+11769913"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8c196769dd60fd4f363e11d948139556a344e79d451aeb2fa2fd040738ef7691"
+checksum = "ee6cda3051665f1fb8d9e08fc35c96d5a244fb1be711a03b71118828afc9a873"
 dependencies = [
  "jni-sys",
 ]
 
 [[package]]
 name = "nix"
 version = "0.26.2"
@@ -1265,75 +1251,90 @@
  "proc-macro2",
  "quote",
  "syn 2.0.32",
 ]
 
 [[package]]
 name = "objc-sys"
-version = "0.3.2"
+version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c7c71324e4180d0899963fc83d9d241ac39e699609fc1025a850aadac8257459"
+checksum = "da284c198fb9b7b0603f8635185e85fbd5b64ee154b1ed406d489077de2d6d60"
 
 [[package]]
 name = "objc2"
-version = "0.4.1"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "559c5a40fdd30eb5e344fbceacf7595a81e242529fb4e21cf5f43fb4f11ff98d"
+checksum = "b4b25e1034d0e636cd84707ccdaa9f81243d399196b8a773946dcffec0401659"
 dependencies = [
  "objc-sys",
- "objc2-encode 3.0.0",
+ "objc2-encode",
 ]
 
 [[package]]
-name = "objc2"
-version = "0.5.0"
+name = "objc2-app-kit"
+version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a9c7f0d511a4ce26b078183179dca908171cfc69f88986fe36c5138e1834476"
+checksum = "fb79768a710a9a1798848179edb186d1af7e8a8679f369e4b8d201dd2a034047"
 dependencies = [
- "objc-sys",
- "objc2-encode 4.0.0",
+ "block2",
+ "objc2",
+ "objc2-core-data",
+ "objc2-foundation",
 ]
 
 [[package]]
-name = "objc2-encode"
-version = "3.0.0"
+name = "objc2-core-data"
+version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d079845b37af429bfe5dfa76e6d087d788031045b25cfc6fd898486fd9847666"
+checksum = "6e092bc42eaf30a08844e6a076938c60751225ec81431ab89f5d1ccd9f958d6c"
+dependencies = [
+ "block2",
+ "objc2",
+ "objc2-foundation",
+]
 
 [[package]]
 name = "objc2-encode"
-version = "4.0.0"
+version = "4.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88658da63e4cc2c8adb1262902cd6af51094df0488b760d6fd27194269c0950a"
+
+[[package]]
+name = "objc2-foundation"
+version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2ff06a6505cde0766484f38d8479ac8e6d31c66fbc2d5492f65ca8c091456379"
+checksum = "cfaefe14254871ea16c7d88968c0ff14ba554712a20d76421eec52f0a7fb8904"
+dependencies = [
+ "block2",
+ "dispatch",
+ "objc2",
+]
 
 [[package]]
 name = "object"
 version = "0.32.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9cf5f9dd3933bd50a9e1f149ec995f39ae2c496d31fd772c1fd45ebc27e902b0"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.17.1"
+version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
+checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "orbclient"
-version = "0.3.43"
+version = "0.3.47"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "974465c5e83cf9df05c1e4137b271d29035c902e39e5ad4c1939837e22160af8"
+checksum = "52f0d54bde9774d3a51dcf281a5def240c71996bc6ca05d2c847ec8b2b216166"
 dependencies = [
- "cfg-if",
- "redox_syscall 0.2.16",
- "wasm-bindgen",
- "web-sys",
+ "libredox",
 ]
 
 [[package]]
 name = "ordered-stream"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9aa2b01e1d916879f73a53d01d1d6cee68adbb31d6d9177a8cfce093cced1d50"
@@ -1389,14 +1390,34 @@
 [[package]]
 name = "percent-encoding"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "478c572c3d73181ff3c2539045f6eb99e5491218eae919370993b890cdbdd98e"
 
 [[package]]
+name = "pin-project"
+version = "1.1.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b6bf43b791c5b9e34c3d182969b4abb522f9343702850a2e57f460d00d09b4b3"
+dependencies = [
+ "pin-project-internal",
+]
+
+[[package]]
+name = "pin-project-internal"
+version = "1.1.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2f38a4412a78282e09a2cf38d195ea5420d15ba0602cb375210efbc877243965"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.32",
+]
+
+[[package]]
 name = "pin-project-lite"
 version = "0.2.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8afb450f006bf6385ca15ef45d71d2288452bc3683ce2e2cacc0d18e4be60b58"
 
 [[package]]
 name = "pin-utils"
@@ -1602,14 +1623,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
  "bitflags 1.3.2",
 ]
 
 [[package]]
+name = "redox_syscall"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
+dependencies = [
+ "bitflags 1.3.2",
+]
+
+[[package]]
 name = "regex"
 version = "1.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "48aaa5748ba571fb95cd2c85c09f629215d3a6ece942baa100950af03a34f733"
 dependencies = [
  "aho-corasick",
  "memchr",
@@ -1718,17 +1748,17 @@
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "sctk-adwaita"
-version = "0.7.0"
+version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1729a30a469de249c6effc17ec8d039b0aa29b3af79b819b7f51cb6ab8046a90"
+checksum = "7de61fa7334ee8ee1f5c3c58dcc414fb9361e7e8f5bff9d45f4d69eeb89a7169"
 dependencies = [
  "ab_glyph",
  "log",
  "memmap2",
  "smithay-client-toolkit",
  "tiny-skia",
 ]
@@ -2038,40 +2068,39 @@
  "indexmap",
  "toml_datetime",
  "winnow",
 ]
 
 [[package]]
 name = "tracing"
-version = "0.1.37"
+version = "0.1.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ce8c33a8d48bd45d624a6e523445fd21ec13d3653cd51f681abf67418f54eb8"
+checksum = "c3523ab5a71916ccf420eebdf5521fcef02141234bbc0b8a49f2fdc4544364ef"
 dependencies = [
- "cfg-if",
  "pin-project-lite",
  "tracing-attributes",
  "tracing-core",
 ]
 
 [[package]]
 name = "tracing-attributes"
-version = "0.1.23"
+version = "0.1.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4017f8f45139870ca7e672686113917c71c7a6e02d4924eda67186083c03081a"
+checksum = "34704c8d6ebcbc939824180af020566b01a7c01f80641264eba0999f6c2b6be7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.32",
 ]
 
 [[package]]
 name = "tracing-core"
-version = "0.1.30"
+version = "0.1.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "24eb03ba0eab1fd845050058ce5e616558e8f8d8fca633e6b163fe25c797213a"
+checksum = "c06d3da6113f116aaee68e4d601191614c9053067f9ab7f6edbcb161237daa54"
 dependencies = [
  "once_cell",
 ]
 
 [[package]]
 name = "ttf-parser"
 version = "0.18.1"
@@ -2323,17 +2352,17 @@
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "web-time"
-version = "0.2.3"
+version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "57099a701fb3a8043f993e8228dc24229c7b942e2b009a1b962e54489ba1d3bf"
+checksum = "5a6580f308b1fad9207618087a65c04e7a10bc77e02c8e84e9b00dd4b12fa0bb"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "winapi"
@@ -2357,23 +2386,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f29e6f9198ba0d26b4c9f07dbe6f9ed633e1f3d5b8b414090084349e46a52596"
 dependencies = [
  "winapi",
 ]
 
 [[package]]
-name = "winapi-wsapoll"
-version = "0.1.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44c17110f57155602a80dca10be03852116403c9ff3cd25b079d666f2aa3df6e"
-dependencies = [
- "winapi",
-]
-
-[[package]]
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
 name = "windows"
@@ -2458,14 +2478,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
 dependencies = [
  "windows-targets 0.48.1",
 ]
 
 [[package]]
+name = "windows-sys"
+version = "0.52.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
+dependencies = [
+ "windows-targets 0.52.3",
+]
+
+[[package]]
 name = "windows-targets"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
 dependencies = [
  "windows_aarch64_gnullvm 0.42.2",
  "windows_aarch64_msvc 0.42.2",
@@ -2630,56 +2659,58 @@
 name = "windows_x86_64_msvc"
 version = "0.52.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0770833d60a970638e989b3fa9fd2bb1aaadcf88963d1659fd7d9990196ed2d6"
 
 [[package]]
 name = "winit"
-version = "0.29.3"
+version = "0.30.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "161598019a9da35ab6c34dc46cd13546cba9dbf9816475d4dd9a639455016563"
+checksum = "ea9e6d5d66cbf702e0dd820302144f51b69a95acdc495dd98ca280ff206562b1"
 dependencies = [
  "ahash",
  "android-activity",
  "atomic-waker",
  "bitflags 2.4.1",
  "bytemuck",
  "calloop",
  "cfg_aliases",
+ "concurrent-queue",
  "core-foundation",
  "core-graphics",
  "cursor-icon",
- "icrate 0.0.4",
+ "dpi",
  "js-sys",
  "libc",
- "log",
  "memmap2",
  "ndk",
- "ndk-sys",
- "objc2 0.4.1",
- "once_cell",
+ "objc2",
+ "objc2-app-kit",
+ "objc2-foundation",
  "orbclient",
  "percent-encoding",
+ "pin-project",
  "raw-window-handle 0.5.2",
  "raw-window-handle 0.6.0",
- "redox_syscall 0.3.5",
+ "redox_syscall 0.4.1",
  "rustix 0.38.21",
  "sctk-adwaita",
  "smithay-client-toolkit",
  "smol_str",
+ "tracing",
  "unicode-segmentation",
  "wasm-bindgen",
  "wasm-bindgen-futures",
  "wayland-backend",
  "wayland-client",
  "wayland-protocols",
  "wayland-protocols-plasma",
  "web-sys",
  "web-time",
- "windows-sys 0.48.0",
+ "windows-sys 0.52.0",
  "x11-dl",
  "x11rb",
  "xkbcommon-dl",
 ]
 
 [[package]]
 name = "winnow"
@@ -2699,37 +2730,32 @@
  "libc",
  "once_cell",
  "pkg-config",
 ]
 
 [[package]]
 name = "x11rb"
-version = "0.12.0"
+version = "0.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1641b26d4dec61337c35a1b1aaf9e3cba8f46f0b43636c609ab0291a648040a"
+checksum = "f8f25ead8c7e4cba123243a6367da5d3990e0d3affa708ea19dce96356bd9f1a"
 dependencies = [
  "as-raw-xcb-connection",
  "gethostname",
  "libc",
- "libloading",
- "nix",
+ "libloading 0.8.3",
  "once_cell",
- "winapi",
- "winapi-wsapoll",
+ "rustix 0.38.21",
  "x11rb-protocol",
 ]
 
 [[package]]
 name = "x11rb-protocol"
-version = "0.12.0"
+version = "0.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "82d6c3f9a0fb6701fab8f6cea9b0c0bd5d6876f1f89f7fada07e558077c344bc"
-dependencies = [
- "nix",
-]
+checksum = "e63e71c4b8bd9ffec2c963173a4dc4cbde9ee96961d4fcb4429db9929b606c34"
 
 [[package]]
 name = "xcursor"
 version = "0.3.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "463705a63313cd4301184381c5e8042f0a7e9b4bb63653f216311d4ae74690b7"
 dependencies = [
@@ -2744,17 +2770,17 @@
 dependencies = [
  "nix",
  "winapi",
 ]
 
 [[package]]
 name = "xkbcommon-dl"
-version = "0.4.1"
+version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6924668544c48c0133152e7eec86d644a056ca3d09275eb8d5cdb9855f9d8699"
+checksum = "d039de8032a9a8856a6be89cea3e5d12fdd82306ab7c94d74e6deab2460651c5"
 dependencies = [
  "bitflags 2.4.1",
  "dlib",
  "log",
  "once_cell",
  "xkeysym",
 ]
```

### Comparing `accesskit-0.2.0/pyproject.toml` & `accesskit-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `accesskit-0.2.0/LICENSE-APACHE` & `accesskit-0.3.0/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `accesskit-0.2.0/LICENSE-MIT` & `accesskit-0.3.0/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `accesskit-0.2.0/LICENSE.chromium` & `accesskit-0.3.0/LICENSE.chromium`

 * *Files identical despite different names*

### Comparing `accesskit-0.2.0/PKG-INFO` & `accesskit-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: accesskit
-Version: 0.2.0
+Version: 0.3.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

