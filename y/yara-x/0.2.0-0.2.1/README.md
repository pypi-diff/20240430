# Comparing `tmp/yara_x-0.2.0.tar.gz` & `tmp/yara_x-0.2.1.tar.gz`

## Comparing `yara_x-0.2.0.tar` & `yara_x-0.2.1.tar`

### file list

```diff
@@ -1,451 +1,451 @@
--rw-r--r--   0     1001      127     1244 2024-04-29 19:53:43.000000 yara_x-0.2.0/parser/Cargo.toml
--rw-r--r--   0     1001      127    18222 2024-04-29 19:53:43.000000 yara_x-0.2.0/parser/src/ast/ascii_tree.rs
--rw-r--r--   0     1001      127    24797 2024-04-29 19:53:43.000000 yara_x-0.2.0/parser/src/ast/mod.rs
--rw-r--r--   0     1001      127     2838 2024-04-29 19:53:43.000000 yara_x-0.2.0/parser/src/ast/span.rs
--rw-r--r--   0     1001      127     7532 2024-04-29 19:53:43.000000 yara_x-0.2.0/parser/src/cst/mod.rs
--rw-r--r--   0     1001      127     1382 2024-04-29 19:53:43.000000 yara_x-0.2.0/parser/src/lib.rs
--rw-r--r--   0     1001      127     2970 2024-04-29 19:53:43.000000 yara_x-0.2.0/parser/src/parser/context.rs
--rw-r--r--   0     1001      127    80950 2024-04-29 19:53:43.000000 yara_x-0.2.0/parser/src/parser/cst2ast.rs
--rw-r--r--   0     1001      127    13191 2024-04-29 19:53:43.000000 yara_x-0.2.0/parser/src/parser/errors.rs
--rw-r--r--   0     1001      127    14032 2024-04-29 19:53:43.000000 yara_x-0.2.0/parser/src/parser/grammar.pest
--rw-r--r--   0     1001      127    12336 2024-04-29 19:53:43.000000 yara_x-0.2.0/parser/src/parser/mod.rs
--rw-r--r--   0     1001      127     2242 2024-04-29 19:53:43.000000 yara_x-0.2.0/parser/src/parser/tests/ast.rs
--rw-r--r--   0     1001      127    25756 2024-04-29 19:53:43.000000 yara_x-0.2.0/parser/src/parser/tests/cst.rs
--rw-r--r--   0     1001      127     1549 2024-04-29 19:53:43.000000 yara_x-0.2.0/parser/src/parser/tests/mod.rs
--rw-r--r--   0     1001      127     3234 2024-04-29 19:53:43.000000 yara_x-0.2.0/parser/src/parser/tests/testdata/arithmetic_ops.yaml
--rw-r--r--   0     1001      127     1687 2024-04-29 19:53:43.000000 yara_x-0.2.0/parser/src/parser/tests/testdata/bitwise_ops.yaml
--rw-r--r--   0     1001      127     2973 2024-04-29 19:53:43.000000 yara_x-0.2.0/parser/src/parser/tests/testdata/for_stmt.yaml
--rw-r--r--   0     1001      127     7108 2024-04-29 19:53:43.000000 yara_x-0.2.0/parser/src/parser/tests/testdata/general.yaml
--rw-r--r--   0     1001      127     5250 2024-04-29 19:53:43.000000 yara_x-0.2.0/parser/src/parser/tests/testdata/hex_patterns.yaml
--rw-r--r--   0     1001      127     2357 2024-04-29 19:53:43.000000 yara_x-0.2.0/parser/src/parser/tests/testdata/literals.yaml
--rw-r--r--   0     1001      127      703 2024-04-29 19:53:43.000000 yara_x-0.2.0/parser/src/parser/tests/testdata/meta.yaml
--rw-r--r--   0     1001      127     3978 2024-04-29 19:53:43.000000 yara_x-0.2.0/parser/src/parser/tests/testdata/of_stmt.yaml
--rw-r--r--   0     1001      127      956 2024-04-29 19:53:43.000000 yara_x-0.2.0/parser/src/parser/tests/testdata/regexp_patterns.yaml
--rw-r--r--   0     1001      127     2243 2024-04-29 19:53:43.000000 yara_x-0.2.0/parser/src/parser/tests/testdata/shift_ops.yaml
--rw-r--r--   0     1001      127     3563 2024-04-29 19:53:43.000000 yara_x-0.2.0/parser/src/parser/tests/testdata/string_ops.yaml
--rw-r--r--   0     1001      127     1484 2024-04-29 19:53:43.000000 yara_x-0.2.0/parser/src/parser/tests/testdata/text_patterns.yaml
--rw-r--r--   0     1001      127     8459 2024-04-29 19:53:43.000000 yara_x-0.2.0/parser/src/report.rs
--rw-r--r--   0     1001      127     3002 2024-04-29 19:53:43.000000 yara_x-0.2.0/parser/src/warnings.rs
--rw-r--r--   0     1001      127     5618 2024-04-29 19:53:42.000000 yara_x-0.2.0/README.md
--rw-r--r--   0     1001      127      448 2024-04-29 19:53:43.000000 yara_x-0.2.0/macros/Cargo.toml
--rw-r--r--   0     1001      127    14420 2024-04-29 19:53:43.000000 yara_x-0.2.0/macros/src/error.rs
--rw-r--r--   0     1001      127    10584 2024-04-29 19:53:43.000000 yara_x-0.2.0/macros/src/lib.rs
--rw-r--r--   0     1001      127     3267 2024-04-29 19:53:43.000000 yara_x-0.2.0/macros/src/module_export.rs
--rw-r--r--   0     1001      127      543 2024-04-29 19:53:43.000000 yara_x-0.2.0/macros/src/module_main.rs
--rw-r--r--   0     1001      127     1743 2024-04-29 19:53:43.000000 yara_x-0.2.0/macros/src/span.rs
--rw-r--r--   0     1001      127    10023 2024-04-29 19:53:43.000000 yara_x-0.2.0/macros/src/wasm_export.rs
--rw-r--r--   0     1001      127     7309 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/Cargo.toml
--rw-r--r--   0     1001      127     7067 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/build.rs
--rw-r--r--   0     1001      127     3343 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/atoms/mask.rs
--rw-r--r--   0     1001      127    16266 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/atoms/mod.rs
--rw-r--r--   0     1001      127    20877 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/atoms/quality.rs
--rw-r--r--   0     1001      127     7412 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/base64.rs
--rw-r--r--   0     1001      127     6885 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/context.rs
--rw-r--r--   0     1001      127   100037 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/emit.rs
--rw-r--r--   0     1001      127     6157 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/errors.rs
--rw-r--r--   0     1001      127    60859 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/ir/ast2ir.rs
--rw-r--r--   0     1001      127    10406 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/ir/hex2hir.rs
--rw-r--r--   0     1001      127    27218 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/ir/mod.rs
--rw-r--r--   0     1001      127      144 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/ir/utils.rs
--rw-r--r--   0     1001      127    66525 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/mod.rs
--rw-r--r--   0     1001      127    18302 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/rules.rs
--rw-r--r--   0     1001      127    17084 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/mod.rs
--rw-r--r--   0     1001      127       67 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/1.in
--rw-r--r--   0     1001      127      222 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/1.out
--rw-r--r--   0     1001      127       45 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/10.in
--rw-r--r--   0     1001      127      143 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/10.out
--rw-r--r--   0     1001      127       48 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/100.in
--rw-r--r--   0     1001      127      206 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/100.out
--rw-r--r--   0     1001      127       73 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/101.in
--rw-r--r--   0     1001      127      155 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/101.out
--rw-r--r--   0     1001      127       74 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/102.in
--rw-r--r--   0     1001      127      151 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/102.out
--rw-r--r--   0     1001      127       69 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/103.in
--rw-r--r--   0     1001      127      151 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/103.out
--rw-r--r--   0     1001      127       76 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/104.in
--rw-r--r--   0     1001      127      228 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/104.out
--rw-r--r--   0     1001      127       60 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/105.in
--rw-r--r--   0     1001      127      136 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/105.out
--rw-r--r--   0     1001      127       39 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/106.in
--rw-r--r--   0     1001      127      133 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/106.out
--rw-r--r--   0     1001      127       39 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/107.in
--rw-r--r--   0     1001      127      140 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/107.out
--rw-r--r--   0     1001      127       43 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/108.in
--rw-r--r--   0     1001      127      144 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/108.out
--rw-r--r--   0     1001      127       44 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/109.in
--rw-r--r--   0     1001      127      139 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/109.out
--rw-r--r--   0     1001      127       53 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/11.in
--rw-r--r--   0     1001      127      165 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/11.out
--rw-r--r--   0     1001      127       69 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/110.in
--rw-r--r--   0     1001      127      148 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/110.out
--rw-r--r--   0     1001      127       76 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/111.in
--rw-r--r--   0     1001      127      140 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/111.out
--rw-r--r--   0     1001      127       69 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/112.in
--rw-r--r--   0     1001      127      144 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/112.out
--rw-r--r--   0     1001      127       71 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/113.in
--rw-r--r--   0     1001      127      263 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/113.out
--rw-r--r--   0     1001      127       84 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/114.in
--rw-r--r--   0     1001      127      306 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/114.out
--rw-r--r--   0     1001      127       71 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/115.in
--rw-r--r--   0     1001      127      162 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/115.out
--rw-r--r--   0     1001      127       16 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/116.in
--rw-r--r--   0     1001      127      145 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/116.out
--rw-r--r--   0     1001      127       78 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/117.in
--rw-r--r--   0     1001      127      177 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/117.out
--rw-r--r--   0     1001      127       73 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/118.in
--rw-r--r--   0     1001      127      150 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/118.out
--rw-r--r--   0     1001      127       66 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/119.in
--rw-r--r--   0     1001      127      185 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/119.out
--rw-r--r--   0     1001      127       78 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/12.in
--rw-r--r--   0     1001      127      140 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/12.out
--rw-r--r--   0     1001      127       57 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/120.in
--rw-r--r--   0     1001      127      108 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/120.out
--rw-r--r--   0     1001      127       51 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/121.in
--rw-r--r--   0     1001      127      132 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/121.out
--rw-r--r--   0     1001      127       59 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/122.in
--rw-r--r--   0     1001      127      167 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/122.out
--rw-r--r--   0     1001      127       65 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/123.in
--rw-r--r--   0     1001      127      181 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/123.out
--rw-r--r--   0     1001      127       71 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/13.in
--rw-r--r--   0     1001      127      128 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/13.out
--rw-r--r--   0     1001      127       71 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/14.in
--rw-r--r--   0     1001      127      131 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/14.out
--rw-r--r--   0     1001      127       70 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/15.in
--rw-r--r--   0     1001      127      140 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/15.out
--rw-r--r--   0     1001      127       67 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/16.in
--rw-r--r--   0     1001      127      124 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/16.out
--rw-r--r--   0     1001      127       74 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/17.in
--rw-r--r--   0     1001      127      127 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/17.out
--rw-r--r--   0     1001      127       63 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/18.in
--rw-r--r--   0     1001      127      139 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/18.out
--rw-r--r--   0     1001      127       64 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/19.in
--rw-r--r--   0     1001      127      141 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/19.out
--rw-r--r--   0     1001      127       41 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/2.in
--rw-r--r--   0     1001      127      152 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/2.out
--rw-r--r--   0     1001      127       73 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/20.in
--rw-r--r--   0     1001      127      135 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/20.out
--rw-r--r--   0     1001      127       81 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/21.in
--rw-r--r--   0     1001      127      148 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/21.out
--rw-r--r--   0     1001      127       76 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/22.in
--rw-r--r--   0     1001      127      144 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/22.out
--rw-r--r--   0     1001      127       65 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/23.in
--rw-r--r--   0     1001      127      122 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/23.out
--rw-r--r--   0     1001      127       68 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/24.in
--rw-r--r--   0     1001      127      119 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/24.out
--rw-r--r--   0     1001      127       69 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/25.in
--rw-r--r--   0     1001      127      129 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/25.out
--rw-r--r--   0     1001      127       64 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/26.in
--rw-r--r--   0     1001      127      146 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/26.out
--rw-r--r--   0     1001      127       52 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/27.in
--rw-r--r--   0     1001      127      141 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/27.out
--rw-r--r--   0     1001      127       47 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/28.in
--rw-r--r--   0     1001      127      154 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/28.out
--rw-r--r--   0     1001      127       67 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/29.in
--rw-r--r--   0     1001      127      142 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/29.out
--rw-r--r--   0     1001      127       39 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/3.in
--rw-r--r--   0     1001      127      154 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/3.out
--rw-r--r--   0     1001      127       12 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/30.in
--rw-r--r--   0     1001      127      106 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/30.out
--rw-r--r--   0     1001      127       76 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/31.in
--rw-r--r--   0     1001      127      194 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/31.out
--rw-r--r--   0     1001      127       78 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/32.in
--rw-r--r--   0     1001      127      153 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/32.out
--rw-r--r--   0     1001      127       64 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/33.in
--rw-r--r--   0     1001      127      191 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/33.out
--rw-r--r--   0     1001      127       66 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/34.in
--rw-r--r--   0     1001      127      194 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/34.out
--rw-r--r--   0     1001      127      137 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/35.in
--rw-r--r--   0     1001      127      127 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/35.out
--rw-r--r--   0     1001      127       85 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/36.in
--rw-r--r--   0     1001      127      372 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/36.out
--rw-r--r--   0     1001      127       63 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/37.in
--rw-r--r--   0     1001      127      123 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/37.out
--rw-r--r--   0     1001      127       69 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/38.in
--rw-r--r--   0     1001      127      196 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/38.out
--rw-r--r--   0     1001      127       64 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/39.in
--rw-r--r--   0     1001      127      162 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/39.out
--rw-r--r--   0     1001      127       39 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/4.in
--rw-r--r--   0     1001      127      138 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/4.out
--rw-r--r--   0     1001      127       60 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/40.in
--rw-r--r--   0     1001      127      107 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/40.out
--rw-r--r--   0     1001      127       60 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/41.in
--rw-r--r--   0     1001      127      119 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/41.out
--rw-r--r--   0     1001      127       64 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/42.in
--rw-r--r--   0     1001      127      190 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/42.out
--rw-r--r--   0     1001      127       62 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/43.in
--rw-r--r--   0     1001      127      136 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/43.out
--rw-r--r--   0     1001      127       43 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/44.in
--rw-r--r--   0     1001      127      175 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/44.out
--rw-r--r--   0     1001      127       42 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/45.in
--rw-r--r--   0     1001      127      169 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/45.out
--rw-r--r--   0     1001      127       51 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/46.in
--rw-r--r--   0     1001      127      228 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/46.out
--rw-r--r--   0     1001      127      101 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/47.in
--rw-r--r--   0     1001      127      223 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/47.out
--rw-r--r--   0     1001      127      104 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/48.in
--rw-r--r--   0     1001      127      227 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/48.out
--rw-r--r--   0     1001      127       98 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/49.in
--rw-r--r--   0     1001      127      195 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/49.out
--rw-r--r--   0     1001      127       40 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/5.in
--rw-r--r--   0     1001      127      156 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/5.out
--rw-r--r--   0     1001      127      110 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/50.in
--rw-r--r--   0     1001      127      294 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/50.out
--rw-r--r--   0     1001      127      108 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/51.in
--rw-r--r--   0     1001      127      290 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/51.out
--rw-r--r--   0     1001      127      145 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/52.in
--rw-r--r--   0     1001      127      226 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/52.out
--rw-r--r--   0     1001      127       77 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/53.in
--rw-r--r--   0     1001      127      160 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/53.out
--rw-r--r--   0     1001      127       82 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/54.in
--rw-r--r--   0     1001      127      165 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/54.out
--rw-r--r--   0     1001      127       83 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/55.in
--rw-r--r--   0     1001      127      167 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/55.out
--rw-r--r--   0     1001      127       66 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/56.in
--rw-r--r--   0     1001      127      131 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/56.out
--rw-r--r--   0     1001      127       71 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/57.in
--rw-r--r--   0     1001      127      154 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/57.out
--rw-r--r--   0     1001      127       80 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/58.in
--rw-r--r--   0     1001      127      250 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/58.out
--rw-r--r--   0     1001      127       79 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/59.in
--rw-r--r--   0     1001      127      210 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/59.out
--rw-r--r--   0     1001      127       39 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/6.in
--rw-r--r--   0     1001      127      147 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/6.out
--rw-r--r--   0     1001      127       98 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/60.in
--rw-r--r--   0     1001      127      187 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/60.out
--rw-r--r--   0     1001      127       41 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/61.in
--rw-r--r--   0     1001      127      136 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/61.out
--rw-r--r--   0     1001      127       30 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/62.in
--rw-r--r--   0     1001      127      107 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/62.out
--rw-r--r--   0     1001      127       22 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/63.in
--rw-r--r--   0     1001      127      109 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/63.out
--rw-r--r--   0     1001      127       27 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/64.in
--rw-r--r--   0     1001      127      146 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/64.out
--rw-r--r--   0     1001      127       27 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/65.in
--rw-r--r--   0     1001      127      130 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/65.out
--rw-r--r--   0     1001      127       29 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/66.in
--rw-r--r--   0     1001      127      114 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/66.out
--rw-r--r--   0     1001      127       12 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/67.in
--rw-r--r--   0     1001      127      119 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/67.out
--rw-r--r--   0     1001      127       35 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/68.in
--rw-r--r--   0     1001      127      126 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/68.out
--rw-r--r--   0     1001      127       39 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/69.in
--rw-r--r--   0     1001      127      166 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/69.out
--rw-r--r--   0     1001      127       39 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/7.in
--rw-r--r--   0     1001      127      143 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/7.out
--rw-r--r--   0     1001      127       38 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/70.in
--rw-r--r--   0     1001      127      140 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/70.out
--rw-r--r--   0     1001      127       36 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/71.in
--rw-r--r--   0     1001      127      121 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/71.out
--rw-r--r--   0     1001      127       24 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/72.in
--rw-r--r--   0     1001      127      128 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/72.out
--rw-r--r--   0     1001      127       41 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/73.in
--rw-r--r--   0     1001      127      129 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/73.out
--rw-r--r--   0     1001      127       40 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/74.in
--rw-r--r--   0     1001      127      128 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/74.out
--rw-r--r--   0     1001      127       43 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/75.in
--rw-r--r--   0     1001      127      131 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/75.out
--rw-r--r--   0     1001      127       28 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/76.in
--rw-r--r--   0     1001      127      128 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/76.out
--rw-r--r--   0     1001      127       33 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/77.in
--rw-r--r--   0     1001      127      105 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/77.out
--rw-r--r--   0     1001      127       46 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/78.in
--rw-r--r--   0     1001      127      155 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/78.out
--rw-r--r--   0     1001      127       59 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/79.in
--rw-r--r--   0     1001      127      153 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/79.out
--rw-r--r--   0     1001      127       43 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/8.in
--rw-r--r--   0     1001      127      156 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/8.out
--rw-r--r--   0     1001      127       59 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/80.in
--rw-r--r--   0     1001      127       96 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/80.out
--rw-r--r--   0     1001      127       58 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/81.in
--rw-r--r--   0     1001      127      186 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/81.out
--rw-r--r--   0     1001      127       60 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/82.in
--rw-r--r--   0     1001      127       97 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/82.out
--rw-r--r--   0     1001      127       59 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/83.in
--rw-r--r--   0     1001      127      127 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/83.out
--rw-r--r--   0     1001      127       53 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/84.in
--rw-r--r--   0     1001      127       90 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/84.out
--rw-r--r--   0     1001      127       58 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/85.in
--rw-r--r--   0     1001      127      119 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/85.out
--rw-r--r--   0     1001      127       58 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/86.in
--rw-r--r--   0     1001      127      118 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/86.out
--rw-r--r--   0     1001      127       53 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/87.in
--rw-r--r--   0     1001      127      114 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/87.out
--rw-r--r--   0     1001      127       46 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/88.in
--rw-r--r--   0     1001      127      107 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/88.out
--rw-r--r--   0     1001      127       36 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/89.in
--rw-r--r--   0     1001      127      205 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/89.out
--rw-r--r--   0     1001      127       52 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/9.in
--rw-r--r--   0     1001      127      173 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/9.out
--rw-r--r--   0     1001      127       88 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/90.in
--rw-r--r--   0     1001      127      189 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/90.out
--rw-r--r--   0     1001      127       35 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/91.in
--rw-r--r--   0     1001      127      127 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/91.out
--rw-r--r--   0     1001      127       40 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/92.in
--rw-r--r--   0     1001      127      132 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/92.out
--rw-r--r--   0     1001      127       40 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/93.in
--rw-r--r--   0     1001      127      132 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/93.out
--rw-r--r--   0     1001      127       40 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/94.in
--rw-r--r--   0     1001      127      132 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/94.out
--rw-r--r--   0     1001      127       98 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/95.in
--rw-r--r--   0     1001      127      123 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/95.out
--rw-r--r--   0     1001      127       64 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/96.in
--rw-r--r--   0     1001      127      120 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/96.out
--rw-r--r--   0     1001      127       98 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/97.in
--rw-r--r--   0     1001      127      121 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/97.out
--rw-r--r--   0     1001      127       61 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/98.in
--rw-r--r--   0     1001      127      127 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/98.out
--rw-r--r--   0     1001      127       48 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/99.in
--rw-r--r--   0     1001      127      206 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/errors/99.out
--rw-r--r--   0     1001      127       90 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/warnings/1.in
--rw-r--r--   0     1001      127      201 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/warnings/1.out
--rw-r--r--   0     1001      127       88 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/warnings/10.in
--rw-r--r--   0     1001      127        0 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/warnings/10.out
--rw-r--r--   0     1001      127       68 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/warnings/11.in
--rw-r--r--   0     1001      127      239 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/warnings/11.out
--rw-r--r--   0     1001      127       81 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/warnings/12.in
--rw-r--r--   0     1001      127      202 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/warnings/12.out
--rw-r--r--   0     1001      127       41 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/warnings/13.in
--rw-r--r--   0     1001      127      227 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/warnings/13.out
--rw-r--r--   0     1001      127       28 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/warnings/14.in
--rw-r--r--   0     1001      127      238 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/warnings/14.out
--rw-r--r--   0     1001      127       53 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/warnings/15.in
--rw-r--r--   0     1001      127      286 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/warnings/15.out
--rw-r--r--   0     1001      127       81 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/warnings/16.in
--rw-r--r--   0     1001      127      260 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/warnings/16.out
--rw-r--r--   0     1001      127       34 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/warnings/17.in
--rw-r--r--   0     1001      127      494 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/warnings/17.out
--rw-r--r--   0     1001      127       40 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/warnings/18.in
--rw-r--r--   0     1001      127      270 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/warnings/18.out
--rw-r--r--   0     1001      127       42 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/warnings/19.in
--rw-r--r--   0     1001      127      282 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/warnings/19.out
--rw-r--r--   0     1001      127       81 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/warnings/2.in
--rw-r--r--   0     1001      127      187 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/warnings/2.out
--rw-r--r--   0     1001      127       32 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/warnings/20.in
--rw-r--r--   0     1001      127      246 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/warnings/20.out
--rw-r--r--   0     1001      127       34 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/warnings/21.in
--rw-r--r--   0     1001      127      250 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/warnings/21.out
--rw-r--r--   0     1001      127       63 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/warnings/22.in
--rw-r--r--   0     1001      127      227 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/warnings/22.out
--rw-r--r--   0     1001      127       69 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/warnings/23.in
--rw-r--r--   0     1001      127      136 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/warnings/23.out
--rw-r--r--   0     1001      127      128 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/warnings/24.in
--rw-r--r--   0     1001      127      628 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/warnings/24.out
--rw-r--r--   0     1001      127       88 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/warnings/3.in
--rw-r--r--   0     1001      127      207 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/warnings/3.out
--rw-r--r--   0     1001      127       88 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/warnings/4.in
--rw-r--r--   0     1001      127      207 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/warnings/4.out
--rw-r--r--   0     1001      127       88 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/warnings/5.in
--rw-r--r--   0     1001      127      207 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/warnings/5.out
--rw-r--r--   0     1001      127       81 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/warnings/6.in
--rw-r--r--   0     1001      127      187 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/warnings/6.out
--rw-r--r--   0     1001      127       88 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/warnings/7.in
--rw-r--r--   0     1001      127      207 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/warnings/7.out
--rw-r--r--   0     1001      127       88 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/warnings/8.in
--rw-r--r--   0     1001      127      207 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/warnings/8.out
--rw-r--r--   0     1001      127       86 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/warnings/9.in
--rw-r--r--   0     1001      127      201 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/warnings/9.out
--rw-r--r--   0     1001      127      525 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/warnings/no_warnings.in
--rw-r--r--   0     1001      127        0 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/compiler/tests/testdata/warnings/no_warnings.out
--rw-r--r--   0     1001      127     2776 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/lib.rs
--rw-r--r--   0     1001      127     1970 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/modules/add_modules.rs
--rw-r--r--   0     1001      127     2657 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/modules/console.rs
--rw-r--r--   0     1001      127      463 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/modules/dotnet/mod.rs
--rw-r--r--   0     1001      127    96817 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/modules/dotnet/parser.rs
--rw-r--r--   0     1001      127   107020 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/modules/dotnet/tests/testdata/605ebe5b5f4b94e1a73e0ad1162bd542e5cb948d1a4ea5a575a14d6b9d6ee849.in
--rw-r--r--   0     1001      127    30988 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/modules/dotnet/tests/testdata/86a1e48cfc843eabfe1b468ef9358c1068950f849c612ab808225b359db0bb8c.in
--rw-r--r--   0     1001      127     3781 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/modules/elf/mod.rs
--rw-r--r--   0     1001      127    22989 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/modules/elf/parser.rs
--rw-r--r--   0     1001      127      980 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/modules/elf/tests/mod.rs
--rw-r--r--   0     1001      127     5979 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/modules/hash/mod.rs
--rw-r--r--   0     1001      127     2139 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/modules/hash/tests/mod.rs
--rw-r--r--   0     1001      127      998 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/modules/lnk/mod.rs
--rw-r--r--   0     1001      127    19663 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/modules/lnk/parser.rs
--rw-r--r--   0     1001      127     8174 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/modules/macho/mod.rs
--rw-r--r--   0     1001      127    56766 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/modules/macho/parser.rs
--rw-r--r--   0     1001      127     6620 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/modules/macho/tests/mod.rs
--rw-r--r--   0     1001      127     2694 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/modules/magic/mod.rs
--rw-r--r--   0     1001      127      922 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/modules/magic/tests/mod.rs
--rw-r--r--   0     1001      127    20093 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/modules/math.rs
--rw-r--r--   0     1001      127     8568 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/modules/mod.rs
--rw-r--r--   0     1001      127      683 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/modules/modules.rs
--rw-r--r--   0     1001      127    22345 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/modules/pe/asn1.rs
--rw-r--r--   0     1001      127    41296 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/modules/pe/authenticode.rs
--rw-r--r--   0     1001      127    25508 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/modules/pe/mod.rs
--rw-r--r--   0     1001      127   129084 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/modules/pe/parser.rs
--rw-r--r--   0     1001      127     4628 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/modules/pe/rva2off.rs
--rw-r--r--   0     1001      127    11193 2024-04-29 19:53:42.000000 yara_x-0.2.0/lib/src/modules/pe/tests/mod.rs
--rw-r--r--   0     1001      127      306 2024-04-29 19:53:43.000000 yara_x-0.2.0/lib/src/modules/protos/console.proto
--rw-r--r--   0     1001      127     2746 2024-04-29 19:53:43.000000 yara_x-0.2.0/lib/src/modules/protos/dotnet.proto
--rw-r--r--   0     1001      127     7466 2024-04-29 19:53:43.000000 yara_x-0.2.0/lib/src/modules/protos/elf.proto
--rw-r--r--   0     1001      127      285 2024-04-29 19:53:43.000000 yara_x-0.2.0/lib/src/modules/protos/hash.proto
--rw-r--r--   0     1001      127     4499 2024-04-29 19:53:43.000000 yara_x-0.2.0/lib/src/modules/protos/lnk.proto
--rw-r--r--   0     1001      127    12579 2024-04-29 19:53:43.000000 yara_x-0.2.0/lib/src/modules/protos/macho.proto
--rw-r--r--   0     1001      127      293 2024-04-29 19:53:43.000000 yara_x-0.2.0/lib/src/modules/protos/magic.proto
--rw-r--r--   0     1001      127      285 2024-04-29 19:53:43.000000 yara_x-0.2.0/lib/src/modules/protos/math.proto
--rw-r--r--   0     1001      127      406 2024-04-29 19:53:43.000000 yara_x-0.2.0/lib/src/modules/protos/mods.proto
--rw-r--r--   0     1001      127    15334 2024-04-29 19:53:43.000000 yara_x-0.2.0/lib/src/modules/protos/pe.proto
--rw-r--r--   0     1001      127      299 2024-04-29 19:53:43.000000 yara_x-0.2.0/lib/src/modules/protos/string.proto
--rw-r--r--   0     1001      127     7863 2024-04-29 19:53:43.000000 yara_x-0.2.0/lib/src/modules/protos/test_proto2.proto
--rw-r--r--   0     1001      127     4544 2024-04-29 19:53:43.000000 yara_x-0.2.0/lib/src/modules/protos/test_proto3.proto
--rw-r--r--   0     1001      127      991 2024-04-29 19:53:43.000000 yara_x-0.2.0/lib/src/modules/protos/text.proto
--rw-r--r--   0     1001      127      285 2024-04-29 19:53:43.000000 yara_x-0.2.0/lib/src/modules/protos/time.proto
--rw-r--r--   0     1001      127      215 2024-04-29 19:53:43.000000 yara_x-0.2.0/lib/src/modules/protos/yaml.proto
--rw-r--r--   0     1001      127     1095 2024-04-29 19:53:43.000000 yara_x-0.2.0/lib/src/modules/protos/yara.proto
--rw-r--r--   0     1001      127     2333 2024-04-29 19:53:43.000000 yara_x-0.2.0/lib/src/modules/string.rs
--rw-r--r--   0     1001      127     4263 2024-04-29 19:53:43.000000 yara_x-0.2.0/lib/src/modules/test_proto2/mod.rs
--rw-r--r--   0     1001      127     9215 2024-04-29 19:53:43.000000 yara_x-0.2.0/lib/src/modules/test_proto2/tests/mod.rs
--rw-r--r--   0     1001      127      942 2024-04-29 19:53:43.000000 yara_x-0.2.0/lib/src/modules/test_proto3/mod.rs
--rw-r--r--   0     1001      127     5558 2024-04-29 19:53:43.000000 yara_x-0.2.0/lib/src/modules/tests.rs
--rw-r--r--   0     1001      127     3636 2024-04-29 19:53:43.000000 yara_x-0.2.0/lib/src/modules/text.rs
--rw-r--r--   0     1001      127      649 2024-04-29 19:53:43.000000 yara_x-0.2.0/lib/src/modules/time.rs
--rw-r--r--   0     1001      127     6413 2024-04-29 19:53:43.000000 yara_x-0.2.0/lib/src/re/bitmapset.rs
--rw-r--r--   0     1001      127    22646 2024-04-29 19:53:43.000000 yara_x-0.2.0/lib/src/re/fast/compiler.rs
--rw-r--r--   0     1001      127    28325 2024-04-29 19:53:43.000000 yara_x-0.2.0/lib/src/re/fast/fastvm.rs
--rw-r--r--   0     1001      127     5549 2024-04-29 19:53:43.000000 yara_x-0.2.0/lib/src/re/fast/instr.rs
--rw-r--r--   0     1001      127     1733 2024-04-29 19:53:43.000000 yara_x-0.2.0/lib/src/re/fast/mod.rs
--rw-r--r--   0     1001      127    21000 2024-04-29 19:53:43.000000 yara_x-0.2.0/lib/src/re/hir.rs
--rw-r--r--   0     1001      127     8029 2024-04-29 19:53:43.000000 yara_x-0.2.0/lib/src/re/mod.rs
--rw-r--r--   0     1001      127    10559 2024-04-29 19:53:43.000000 yara_x-0.2.0/lib/src/re/parser.rs
--rw-r--r--   0     1001      127    63363 2024-04-29 19:53:43.000000 yara_x-0.2.0/lib/src/re/thompson/compiler.rs
--rw-r--r--   0     1001      127    16308 2024-04-29 19:53:43.000000 yara_x-0.2.0/lib/src/re/thompson/instr.rs
--rw-r--r--   0     1001      127      425 2024-04-29 19:53:43.000000 yara_x-0.2.0/lib/src/re/thompson/mod.rs
--rw-r--r--   0     1001      127    16325 2024-04-29 19:53:43.000000 yara_x-0.2.0/lib/src/re/thompson/pikevm.rs
--rw-r--r--   0     1001      127    28321 2024-04-29 19:53:43.000000 yara_x-0.2.0/lib/src/re/thompson/tests.rs
--rw-r--r--   0     1001      127    50038 2024-04-29 19:53:43.000000 yara_x-0.2.0/lib/src/scanner/context.rs
--rw-r--r--   0     1001      127     7133 2024-04-29 19:53:43.000000 yara_x-0.2.0/lib/src/scanner/matches.rs
--rw-r--r--   0     1001      127    38400 2024-04-29 19:53:43.000000 yara_x-0.2.0/lib/src/scanner/mod.rs
--rw-r--r--   0     1001      127    14072 2024-04-29 19:53:43.000000 yara_x-0.2.0/lib/src/scanner/tests.rs
--rw-r--r--   0     1001      127     7749 2024-04-29 19:53:43.000000 yara_x-0.2.0/lib/src/string_pool.rs
--rw-r--r--   0     1001      127    11458 2024-04-29 19:53:43.000000 yara_x-0.2.0/lib/src/symbols/mod.rs
--rw-r--r--   0     1001      127    93892 2024-04-29 19:53:43.000000 yara_x-0.2.0/lib/src/tests/mod.rs
--rw-r--r--   0     1001      127     1664 2024-04-29 19:53:43.000000 yara_x-0.2.0/lib/src/tests/testdata/jumps.bin
--rw-r--r--   0     1001      127     1838 2024-04-29 19:53:43.000000 yara_x-0.2.0/lib/src/types/array.rs
--rw-r--r--   0     1001      127     8631 2024-04-29 19:53:43.000000 yara_x-0.2.0/lib/src/types/func.rs
--rw-r--r--   0     1001      127     2576 2024-04-29 19:53:43.000000 yara_x-0.2.0/lib/src/types/map.rs
--rw-r--r--   0     1001      127    16503 2024-04-29 19:53:43.000000 yara_x-0.2.0/lib/src/types/mod.rs
--rw-r--r--   0     1001      127    39044 2024-04-29 19:53:43.000000 yara_x-0.2.0/lib/src/types/structure.rs
--rw-r--r--   0     1001      127    12650 2024-04-29 19:53:43.000000 yara_x-0.2.0/lib/src/variables.rs
--rw-r--r--   0     1001      127    14481 2024-04-29 19:53:43.000000 yara_x-0.2.0/lib/src/wasm/builder.rs
--rw-r--r--   0     1001      127    46413 2024-04-29 19:53:43.000000 yara_x-0.2.0/lib/src/wasm/mod.rs
--rw-r--r--   0     1001      127     9792 2024-04-29 19:53:43.000000 yara_x-0.2.0/lib/src/wasm/string.rs
--rw-r--r--   0     1001      127      463 2024-04-29 19:53:43.000000 yara_x-0.2.0/proto/Cargo.toml
--rw-r--r--   0     1001      127      243 2024-04-29 19:53:43.000000 yara_x-0.2.0/proto/build.rs
--rw-r--r--   0     1001      127       72 2024-04-29 19:53:43.000000 yara_x-0.2.0/proto/src/lib.rs
--rw-r--r--   0     1001      127     1095 2024-04-29 19:53:43.000000 yara_x-0.2.0/proto/src/yara.proto
--rw-r--r--   0     1001      127      686 2024-04-29 19:53:43.000000 yara_x-0.2.0/proto-yaml/Cargo.toml
--rw-r--r--   0     1001      127      312 2024-04-29 19:53:43.000000 yara_x-0.2.0/proto-yaml/build.rs
--rw-r--r--   0     1001      127    13959 2024-04-29 19:53:43.000000 yara_x-0.2.0/proto-yaml/src/lib.rs
--rw-r--r--   0     1001      127      850 2024-04-29 19:53:43.000000 yara_x-0.2.0/proto-yaml/src/tests/mod.rs
--rw-r--r--   0     1001      127      456 2024-04-29 19:53:43.000000 yara_x-0.2.0/proto-yaml/src/tests/test.proto
--rw-r--r--   0     1001      127      395 2024-04-29 19:53:43.000000 yara_x-0.2.0/proto-yaml/src/tests/testdata/1.in
--rw-r--r--   0     1001      127      346 2024-04-29 19:53:43.000000 yara_x-0.2.0/proto-yaml/src/tests/testdata/1.out
--rw-r--r--   0     1001      127      215 2024-04-29 19:53:43.000000 yara_x-0.2.0/proto-yaml/src/yaml.proto
--rw-r--r--   0        0        0      540 1970-01-01 00:00:00.000000 yara_x-0.2.0/py/Cargo.toml
--rw-r--r--   0     1001      127      534 2024-04-29 19:53:43.000000 yara_x-0.2.0/py/README.md
--rw-r--r--   0     1001      127       71 2024-04-29 19:53:43.000000 yara_x-0.2.0/py/build.rs
--rw-r--r--   0     1001      127    15598 2024-04-29 19:53:43.000000 yara_x-0.2.0/py/src/lib.rs
--rw-r--r--   0     1001      127     5947 2024-04-29 19:53:43.000000 yara_x-0.2.0/py/tests/test_api.py
--rw-r--r--   0     1001      127   122249 2024-04-29 19:53:42.000000 yara_x-0.2.0/Cargo.lock
--rw-r--r--   0        0        0     2703 1970-01-01 00:00:00.000000 yara_x-0.2.0/Cargo.toml
--rw-r--r--   0        0        0      709 1970-01-01 00:00:00.000000 yara_x-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1135 1970-01-01 00:00:00.000000 yara_x-0.2.0/PKG-INFO
+-rw-r--r--   0     1001      127      463 2024-04-30 08:38:48.000000 yara_x-0.2.1/proto/Cargo.toml
+-rw-r--r--   0     1001      127      243 2024-04-30 08:38:48.000000 yara_x-0.2.1/proto/build.rs
+-rw-r--r--   0     1001      127       72 2024-04-30 08:38:48.000000 yara_x-0.2.1/proto/src/lib.rs
+-rw-r--r--   0     1001      127     1095 2024-04-30 08:38:48.000000 yara_x-0.2.1/proto/src/yara.proto
+-rw-r--r--   0     1001      127     5618 2024-04-30 08:38:48.000000 yara_x-0.2.1/README.md
+-rw-r--r--   0     1001      127     7309 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/Cargo.toml
+-rw-r--r--   0     1001      127     7067 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/build.rs
+-rw-r--r--   0     1001      127     3343 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/atoms/mask.rs
+-rw-r--r--   0     1001      127    16266 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/atoms/mod.rs
+-rw-r--r--   0     1001      127    20877 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/atoms/quality.rs
+-rw-r--r--   0     1001      127     7412 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/base64.rs
+-rw-r--r--   0     1001      127     6885 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/context.rs
+-rw-r--r--   0     1001      127   100037 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/emit.rs
+-rw-r--r--   0     1001      127     6157 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/errors.rs
+-rw-r--r--   0     1001      127    60859 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/ir/ast2ir.rs
+-rw-r--r--   0     1001      127    10406 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/ir/hex2hir.rs
+-rw-r--r--   0     1001      127    27218 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/ir/mod.rs
+-rw-r--r--   0     1001      127      144 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/ir/utils.rs
+-rw-r--r--   0     1001      127    66525 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/mod.rs
+-rw-r--r--   0     1001      127    18302 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/rules.rs
+-rw-r--r--   0     1001      127    17084 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/mod.rs
+-rw-r--r--   0     1001      127       67 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/1.in
+-rw-r--r--   0     1001      127      222 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/1.out
+-rw-r--r--   0     1001      127       45 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/10.in
+-rw-r--r--   0     1001      127      143 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/10.out
+-rw-r--r--   0     1001      127       48 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/100.in
+-rw-r--r--   0     1001      127      206 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/100.out
+-rw-r--r--   0     1001      127       73 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/101.in
+-rw-r--r--   0     1001      127      155 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/101.out
+-rw-r--r--   0     1001      127       74 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/102.in
+-rw-r--r--   0     1001      127      151 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/102.out
+-rw-r--r--   0     1001      127       69 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/103.in
+-rw-r--r--   0     1001      127      151 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/103.out
+-rw-r--r--   0     1001      127       76 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/104.in
+-rw-r--r--   0     1001      127      228 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/104.out
+-rw-r--r--   0     1001      127       60 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/105.in
+-rw-r--r--   0     1001      127      136 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/105.out
+-rw-r--r--   0     1001      127       39 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/106.in
+-rw-r--r--   0     1001      127      133 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/106.out
+-rw-r--r--   0     1001      127       39 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/107.in
+-rw-r--r--   0     1001      127      140 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/107.out
+-rw-r--r--   0     1001      127       43 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/108.in
+-rw-r--r--   0     1001      127      144 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/108.out
+-rw-r--r--   0     1001      127       44 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/109.in
+-rw-r--r--   0     1001      127      139 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/109.out
+-rw-r--r--   0     1001      127       53 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/11.in
+-rw-r--r--   0     1001      127      165 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/11.out
+-rw-r--r--   0     1001      127       69 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/110.in
+-rw-r--r--   0     1001      127      148 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/110.out
+-rw-r--r--   0     1001      127       76 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/111.in
+-rw-r--r--   0     1001      127      140 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/111.out
+-rw-r--r--   0     1001      127       69 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/112.in
+-rw-r--r--   0     1001      127      144 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/112.out
+-rw-r--r--   0     1001      127       71 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/113.in
+-rw-r--r--   0     1001      127      263 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/113.out
+-rw-r--r--   0     1001      127       84 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/114.in
+-rw-r--r--   0     1001      127      306 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/114.out
+-rw-r--r--   0     1001      127       71 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/115.in
+-rw-r--r--   0     1001      127      162 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/115.out
+-rw-r--r--   0     1001      127       16 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/116.in
+-rw-r--r--   0     1001      127      145 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/116.out
+-rw-r--r--   0     1001      127       78 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/117.in
+-rw-r--r--   0     1001      127      177 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/117.out
+-rw-r--r--   0     1001      127       73 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/118.in
+-rw-r--r--   0     1001      127      150 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/118.out
+-rw-r--r--   0     1001      127       66 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/119.in
+-rw-r--r--   0     1001      127      185 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/119.out
+-rw-r--r--   0     1001      127       78 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/12.in
+-rw-r--r--   0     1001      127      140 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/12.out
+-rw-r--r--   0     1001      127       57 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/120.in
+-rw-r--r--   0     1001      127      108 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/120.out
+-rw-r--r--   0     1001      127       51 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/121.in
+-rw-r--r--   0     1001      127      132 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/121.out
+-rw-r--r--   0     1001      127       59 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/122.in
+-rw-r--r--   0     1001      127      167 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/122.out
+-rw-r--r--   0     1001      127       65 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/123.in
+-rw-r--r--   0     1001      127      181 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/123.out
+-rw-r--r--   0     1001      127       71 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/13.in
+-rw-r--r--   0     1001      127      128 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/13.out
+-rw-r--r--   0     1001      127       71 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/14.in
+-rw-r--r--   0     1001      127      131 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/14.out
+-rw-r--r--   0     1001      127       70 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/15.in
+-rw-r--r--   0     1001      127      140 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/15.out
+-rw-r--r--   0     1001      127       67 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/16.in
+-rw-r--r--   0     1001      127      124 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/16.out
+-rw-r--r--   0     1001      127       74 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/17.in
+-rw-r--r--   0     1001      127      127 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/17.out
+-rw-r--r--   0     1001      127       63 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/18.in
+-rw-r--r--   0     1001      127      139 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/18.out
+-rw-r--r--   0     1001      127       64 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/19.in
+-rw-r--r--   0     1001      127      141 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/19.out
+-rw-r--r--   0     1001      127       41 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/2.in
+-rw-r--r--   0     1001      127      152 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/2.out
+-rw-r--r--   0     1001      127       73 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/20.in
+-rw-r--r--   0     1001      127      135 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/20.out
+-rw-r--r--   0     1001      127       81 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/21.in
+-rw-r--r--   0     1001      127      148 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/21.out
+-rw-r--r--   0     1001      127       76 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/22.in
+-rw-r--r--   0     1001      127      144 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/22.out
+-rw-r--r--   0     1001      127       65 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/23.in
+-rw-r--r--   0     1001      127      122 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/23.out
+-rw-r--r--   0     1001      127       68 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/24.in
+-rw-r--r--   0     1001      127      119 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/24.out
+-rw-r--r--   0     1001      127       69 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/25.in
+-rw-r--r--   0     1001      127      129 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/25.out
+-rw-r--r--   0     1001      127       64 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/26.in
+-rw-r--r--   0     1001      127      146 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/26.out
+-rw-r--r--   0     1001      127       52 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/27.in
+-rw-r--r--   0     1001      127      141 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/27.out
+-rw-r--r--   0     1001      127       47 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/28.in
+-rw-r--r--   0     1001      127      154 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/28.out
+-rw-r--r--   0     1001      127       67 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/29.in
+-rw-r--r--   0     1001      127      142 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/29.out
+-rw-r--r--   0     1001      127       39 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/3.in
+-rw-r--r--   0     1001      127      154 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/3.out
+-rw-r--r--   0     1001      127       12 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/30.in
+-rw-r--r--   0     1001      127      106 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/30.out
+-rw-r--r--   0     1001      127       76 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/31.in
+-rw-r--r--   0     1001      127      194 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/31.out
+-rw-r--r--   0     1001      127       78 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/32.in
+-rw-r--r--   0     1001      127      153 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/32.out
+-rw-r--r--   0     1001      127       64 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/33.in
+-rw-r--r--   0     1001      127      191 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/33.out
+-rw-r--r--   0     1001      127       66 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/34.in
+-rw-r--r--   0     1001      127      194 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/34.out
+-rw-r--r--   0     1001      127      137 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/35.in
+-rw-r--r--   0     1001      127      127 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/35.out
+-rw-r--r--   0     1001      127       85 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/36.in
+-rw-r--r--   0     1001      127      372 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/36.out
+-rw-r--r--   0     1001      127       63 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/37.in
+-rw-r--r--   0     1001      127      123 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/37.out
+-rw-r--r--   0     1001      127       69 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/38.in
+-rw-r--r--   0     1001      127      196 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/38.out
+-rw-r--r--   0     1001      127       64 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/39.in
+-rw-r--r--   0     1001      127      162 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/39.out
+-rw-r--r--   0     1001      127       39 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/4.in
+-rw-r--r--   0     1001      127      138 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/4.out
+-rw-r--r--   0     1001      127       60 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/40.in
+-rw-r--r--   0     1001      127      107 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/40.out
+-rw-r--r--   0     1001      127       60 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/41.in
+-rw-r--r--   0     1001      127      119 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/41.out
+-rw-r--r--   0     1001      127       64 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/42.in
+-rw-r--r--   0     1001      127      190 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/42.out
+-rw-r--r--   0     1001      127       62 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/43.in
+-rw-r--r--   0     1001      127      136 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/43.out
+-rw-r--r--   0     1001      127       43 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/44.in
+-rw-r--r--   0     1001      127      175 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/44.out
+-rw-r--r--   0     1001      127       42 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/45.in
+-rw-r--r--   0     1001      127      169 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/45.out
+-rw-r--r--   0     1001      127       51 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/46.in
+-rw-r--r--   0     1001      127      228 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/46.out
+-rw-r--r--   0     1001      127      101 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/47.in
+-rw-r--r--   0     1001      127      223 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/47.out
+-rw-r--r--   0     1001      127      104 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/48.in
+-rw-r--r--   0     1001      127      227 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/48.out
+-rw-r--r--   0     1001      127       98 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/49.in
+-rw-r--r--   0     1001      127      195 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/49.out
+-rw-r--r--   0     1001      127       40 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/5.in
+-rw-r--r--   0     1001      127      156 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/5.out
+-rw-r--r--   0     1001      127      110 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/50.in
+-rw-r--r--   0     1001      127      294 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/50.out
+-rw-r--r--   0     1001      127      108 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/51.in
+-rw-r--r--   0     1001      127      290 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/51.out
+-rw-r--r--   0     1001      127      145 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/52.in
+-rw-r--r--   0     1001      127      226 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/52.out
+-rw-r--r--   0     1001      127       77 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/53.in
+-rw-r--r--   0     1001      127      160 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/53.out
+-rw-r--r--   0     1001      127       82 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/54.in
+-rw-r--r--   0     1001      127      165 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/54.out
+-rw-r--r--   0     1001      127       83 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/55.in
+-rw-r--r--   0     1001      127      167 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/55.out
+-rw-r--r--   0     1001      127       66 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/56.in
+-rw-r--r--   0     1001      127      131 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/56.out
+-rw-r--r--   0     1001      127       71 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/57.in
+-rw-r--r--   0     1001      127      154 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/57.out
+-rw-r--r--   0     1001      127       80 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/58.in
+-rw-r--r--   0     1001      127      250 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/58.out
+-rw-r--r--   0     1001      127       79 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/59.in
+-rw-r--r--   0     1001      127      210 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/59.out
+-rw-r--r--   0     1001      127       39 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/6.in
+-rw-r--r--   0     1001      127      147 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/6.out
+-rw-r--r--   0     1001      127       98 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/60.in
+-rw-r--r--   0     1001      127      187 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/60.out
+-rw-r--r--   0     1001      127       41 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/61.in
+-rw-r--r--   0     1001      127      136 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/61.out
+-rw-r--r--   0     1001      127       30 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/62.in
+-rw-r--r--   0     1001      127      107 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/62.out
+-rw-r--r--   0     1001      127       22 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/63.in
+-rw-r--r--   0     1001      127      109 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/63.out
+-rw-r--r--   0     1001      127       27 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/64.in
+-rw-r--r--   0     1001      127      146 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/64.out
+-rw-r--r--   0     1001      127       27 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/65.in
+-rw-r--r--   0     1001      127      130 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/65.out
+-rw-r--r--   0     1001      127       29 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/66.in
+-rw-r--r--   0     1001      127      114 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/66.out
+-rw-r--r--   0     1001      127       12 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/67.in
+-rw-r--r--   0     1001      127      119 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/67.out
+-rw-r--r--   0     1001      127       35 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/68.in
+-rw-r--r--   0     1001      127      126 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/68.out
+-rw-r--r--   0     1001      127       39 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/69.in
+-rw-r--r--   0     1001      127      166 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/69.out
+-rw-r--r--   0     1001      127       39 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/7.in
+-rw-r--r--   0     1001      127      143 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/7.out
+-rw-r--r--   0     1001      127       38 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/70.in
+-rw-r--r--   0     1001      127      140 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/70.out
+-rw-r--r--   0     1001      127       36 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/71.in
+-rw-r--r--   0     1001      127      121 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/71.out
+-rw-r--r--   0     1001      127       24 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/72.in
+-rw-r--r--   0     1001      127      128 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/72.out
+-rw-r--r--   0     1001      127       41 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/73.in
+-rw-r--r--   0     1001      127      129 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/73.out
+-rw-r--r--   0     1001      127       40 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/74.in
+-rw-r--r--   0     1001      127      128 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/74.out
+-rw-r--r--   0     1001      127       43 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/75.in
+-rw-r--r--   0     1001      127      131 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/75.out
+-rw-r--r--   0     1001      127       28 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/76.in
+-rw-r--r--   0     1001      127      128 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/76.out
+-rw-r--r--   0     1001      127       33 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/77.in
+-rw-r--r--   0     1001      127      105 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/77.out
+-rw-r--r--   0     1001      127       46 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/78.in
+-rw-r--r--   0     1001      127      155 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/78.out
+-rw-r--r--   0     1001      127       59 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/79.in
+-rw-r--r--   0     1001      127      153 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/79.out
+-rw-r--r--   0     1001      127       43 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/8.in
+-rw-r--r--   0     1001      127      156 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/8.out
+-rw-r--r--   0     1001      127       59 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/80.in
+-rw-r--r--   0     1001      127       96 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/80.out
+-rw-r--r--   0     1001      127       58 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/81.in
+-rw-r--r--   0     1001      127      186 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/81.out
+-rw-r--r--   0     1001      127       60 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/82.in
+-rw-r--r--   0     1001      127       97 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/82.out
+-rw-r--r--   0     1001      127       59 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/83.in
+-rw-r--r--   0     1001      127      127 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/83.out
+-rw-r--r--   0     1001      127       53 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/84.in
+-rw-r--r--   0     1001      127       90 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/84.out
+-rw-r--r--   0     1001      127       58 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/85.in
+-rw-r--r--   0     1001      127      119 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/85.out
+-rw-r--r--   0     1001      127       58 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/86.in
+-rw-r--r--   0     1001      127      118 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/86.out
+-rw-r--r--   0     1001      127       53 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/87.in
+-rw-r--r--   0     1001      127      114 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/87.out
+-rw-r--r--   0     1001      127       46 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/88.in
+-rw-r--r--   0     1001      127      107 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/88.out
+-rw-r--r--   0     1001      127       36 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/89.in
+-rw-r--r--   0     1001      127      205 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/89.out
+-rw-r--r--   0     1001      127       52 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/9.in
+-rw-r--r--   0     1001      127      173 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/9.out
+-rw-r--r--   0     1001      127       88 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/90.in
+-rw-r--r--   0     1001      127      189 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/90.out
+-rw-r--r--   0     1001      127       35 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/91.in
+-rw-r--r--   0     1001      127      127 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/91.out
+-rw-r--r--   0     1001      127       40 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/92.in
+-rw-r--r--   0     1001      127      132 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/92.out
+-rw-r--r--   0     1001      127       40 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/93.in
+-rw-r--r--   0     1001      127      132 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/93.out
+-rw-r--r--   0     1001      127       40 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/94.in
+-rw-r--r--   0     1001      127      132 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/94.out
+-rw-r--r--   0     1001      127       98 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/95.in
+-rw-r--r--   0     1001      127      123 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/95.out
+-rw-r--r--   0     1001      127       64 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/96.in
+-rw-r--r--   0     1001      127      120 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/96.out
+-rw-r--r--   0     1001      127       98 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/97.in
+-rw-r--r--   0     1001      127      121 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/97.out
+-rw-r--r--   0     1001      127       61 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/98.in
+-rw-r--r--   0     1001      127      127 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/98.out
+-rw-r--r--   0     1001      127       48 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/99.in
+-rw-r--r--   0     1001      127      206 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/errors/99.out
+-rw-r--r--   0     1001      127       90 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/warnings/1.in
+-rw-r--r--   0     1001      127      201 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/warnings/1.out
+-rw-r--r--   0     1001      127       88 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/warnings/10.in
+-rw-r--r--   0     1001      127        0 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/warnings/10.out
+-rw-r--r--   0     1001      127       68 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/warnings/11.in
+-rw-r--r--   0     1001      127      239 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/warnings/11.out
+-rw-r--r--   0     1001      127       81 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/warnings/12.in
+-rw-r--r--   0     1001      127      202 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/warnings/12.out
+-rw-r--r--   0     1001      127       41 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/warnings/13.in
+-rw-r--r--   0     1001      127      227 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/warnings/13.out
+-rw-r--r--   0     1001      127       28 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/warnings/14.in
+-rw-r--r--   0     1001      127      238 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/warnings/14.out
+-rw-r--r--   0     1001      127       53 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/warnings/15.in
+-rw-r--r--   0     1001      127      286 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/warnings/15.out
+-rw-r--r--   0     1001      127       81 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/warnings/16.in
+-rw-r--r--   0     1001      127      260 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/warnings/16.out
+-rw-r--r--   0     1001      127       34 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/warnings/17.in
+-rw-r--r--   0     1001      127      494 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/warnings/17.out
+-rw-r--r--   0     1001      127       40 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/warnings/18.in
+-rw-r--r--   0     1001      127      270 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/warnings/18.out
+-rw-r--r--   0     1001      127       42 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/warnings/19.in
+-rw-r--r--   0     1001      127      282 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/warnings/19.out
+-rw-r--r--   0     1001      127       81 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/warnings/2.in
+-rw-r--r--   0     1001      127      187 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/warnings/2.out
+-rw-r--r--   0     1001      127       32 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/warnings/20.in
+-rw-r--r--   0     1001      127      246 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/warnings/20.out
+-rw-r--r--   0     1001      127       34 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/warnings/21.in
+-rw-r--r--   0     1001      127      250 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/warnings/21.out
+-rw-r--r--   0     1001      127       63 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/warnings/22.in
+-rw-r--r--   0     1001      127      227 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/warnings/22.out
+-rw-r--r--   0     1001      127       69 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/warnings/23.in
+-rw-r--r--   0     1001      127      136 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/warnings/23.out
+-rw-r--r--   0     1001      127      128 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/warnings/24.in
+-rw-r--r--   0     1001      127      628 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/warnings/24.out
+-rw-r--r--   0     1001      127       88 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/warnings/3.in
+-rw-r--r--   0     1001      127      207 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/warnings/3.out
+-rw-r--r--   0     1001      127       88 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/warnings/4.in
+-rw-r--r--   0     1001      127      207 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/warnings/4.out
+-rw-r--r--   0     1001      127       88 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/warnings/5.in
+-rw-r--r--   0     1001      127      207 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/warnings/5.out
+-rw-r--r--   0     1001      127       81 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/warnings/6.in
+-rw-r--r--   0     1001      127      187 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/warnings/6.out
+-rw-r--r--   0     1001      127       88 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/warnings/7.in
+-rw-r--r--   0     1001      127      207 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/warnings/7.out
+-rw-r--r--   0     1001      127       88 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/warnings/8.in
+-rw-r--r--   0     1001      127      207 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/warnings/8.out
+-rw-r--r--   0     1001      127       86 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/warnings/9.in
+-rw-r--r--   0     1001      127      201 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/warnings/9.out
+-rw-r--r--   0     1001      127      525 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/warnings/no_warnings.in
+-rw-r--r--   0     1001      127        0 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/compiler/tests/testdata/warnings/no_warnings.out
+-rw-r--r--   0     1001      127     2776 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/lib.rs
+-rw-r--r--   0     1001      127     1970 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/modules/add_modules.rs
+-rw-r--r--   0     1001      127     2657 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/modules/console.rs
+-rw-r--r--   0     1001      127      463 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/modules/dotnet/mod.rs
+-rw-r--r--   0     1001      127    96817 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/modules/dotnet/parser.rs
+-rw-r--r--   0     1001      127   107020 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/modules/dotnet/tests/testdata/605ebe5b5f4b94e1a73e0ad1162bd542e5cb948d1a4ea5a575a14d6b9d6ee849.in
+-rw-r--r--   0     1001      127    30988 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/modules/dotnet/tests/testdata/86a1e48cfc843eabfe1b468ef9358c1068950f849c612ab808225b359db0bb8c.in
+-rw-r--r--   0     1001      127     3781 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/modules/elf/mod.rs
+-rw-r--r--   0     1001      127    22989 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/modules/elf/parser.rs
+-rw-r--r--   0     1001      127      980 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/modules/elf/tests/mod.rs
+-rw-r--r--   0     1001      127     5979 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/modules/hash/mod.rs
+-rw-r--r--   0     1001      127     2139 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/modules/hash/tests/mod.rs
+-rw-r--r--   0     1001      127      998 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/modules/lnk/mod.rs
+-rw-r--r--   0     1001      127    19663 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/modules/lnk/parser.rs
+-rw-r--r--   0     1001      127     8174 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/modules/macho/mod.rs
+-rw-r--r--   0     1001      127    56766 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/modules/macho/parser.rs
+-rw-r--r--   0     1001      127     6620 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/modules/macho/tests/mod.rs
+-rw-r--r--   0     1001      127     2694 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/modules/magic/mod.rs
+-rw-r--r--   0     1001      127      922 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/modules/magic/tests/mod.rs
+-rw-r--r--   0     1001      127    20093 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/modules/math.rs
+-rw-r--r--   0     1001      127     8568 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/modules/mod.rs
+-rw-r--r--   0     1001      127      683 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/modules/modules.rs
+-rw-r--r--   0     1001      127    22345 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/modules/pe/asn1.rs
+-rw-r--r--   0     1001      127    41296 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/modules/pe/authenticode.rs
+-rw-r--r--   0     1001      127    25508 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/modules/pe/mod.rs
+-rw-r--r--   0     1001      127   129084 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/modules/pe/parser.rs
+-rw-r--r--   0     1001      127     4628 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/modules/pe/rva2off.rs
+-rw-r--r--   0     1001      127    11193 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/modules/pe/tests/mod.rs
+-rw-r--r--   0     1001      127      306 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/modules/protos/console.proto
+-rw-r--r--   0     1001      127     2746 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/modules/protos/dotnet.proto
+-rw-r--r--   0     1001      127     7466 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/modules/protos/elf.proto
+-rw-r--r--   0     1001      127      285 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/modules/protos/hash.proto
+-rw-r--r--   0     1001      127     4499 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/modules/protos/lnk.proto
+-rw-r--r--   0     1001      127    12579 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/modules/protos/macho.proto
+-rw-r--r--   0     1001      127      293 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/modules/protos/magic.proto
+-rw-r--r--   0     1001      127      285 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/modules/protos/math.proto
+-rw-r--r--   0     1001      127      406 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/modules/protos/mods.proto
+-rw-r--r--   0     1001      127    15334 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/modules/protos/pe.proto
+-rw-r--r--   0     1001      127      299 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/modules/protos/string.proto
+-rw-r--r--   0     1001      127     7863 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/modules/protos/test_proto2.proto
+-rw-r--r--   0     1001      127     4544 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/modules/protos/test_proto3.proto
+-rw-r--r--   0     1001      127      991 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/modules/protos/text.proto
+-rw-r--r--   0     1001      127      285 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/modules/protos/time.proto
+-rw-r--r--   0     1001      127      215 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/modules/protos/yaml.proto
+-rw-r--r--   0     1001      127     1095 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/modules/protos/yara.proto
+-rw-r--r--   0     1001      127     2333 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/modules/string.rs
+-rw-r--r--   0     1001      127     4263 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/modules/test_proto2/mod.rs
+-rw-r--r--   0     1001      127     9215 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/modules/test_proto2/tests/mod.rs
+-rw-r--r--   0     1001      127      942 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/modules/test_proto3/mod.rs
+-rw-r--r--   0     1001      127     5558 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/modules/tests.rs
+-rw-r--r--   0     1001      127     3636 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/modules/text.rs
+-rw-r--r--   0     1001      127      649 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/modules/time.rs
+-rw-r--r--   0     1001      127     6413 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/re/bitmapset.rs
+-rw-r--r--   0     1001      127    22646 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/re/fast/compiler.rs
+-rw-r--r--   0     1001      127    28325 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/re/fast/fastvm.rs
+-rw-r--r--   0     1001      127     5549 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/re/fast/instr.rs
+-rw-r--r--   0     1001      127     1733 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/re/fast/mod.rs
+-rw-r--r--   0     1001      127    21000 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/re/hir.rs
+-rw-r--r--   0     1001      127     8029 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/re/mod.rs
+-rw-r--r--   0     1001      127    10559 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/re/parser.rs
+-rw-r--r--   0     1001      127    63363 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/re/thompson/compiler.rs
+-rw-r--r--   0     1001      127    16308 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/re/thompson/instr.rs
+-rw-r--r--   0     1001      127      425 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/re/thompson/mod.rs
+-rw-r--r--   0     1001      127    16325 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/re/thompson/pikevm.rs
+-rw-r--r--   0     1001      127    28321 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/re/thompson/tests.rs
+-rw-r--r--   0     1001      127    50038 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/scanner/context.rs
+-rw-r--r--   0     1001      127     7133 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/scanner/matches.rs
+-rw-r--r--   0     1001      127    38400 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/scanner/mod.rs
+-rw-r--r--   0     1001      127    14072 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/scanner/tests.rs
+-rw-r--r--   0     1001      127     7749 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/string_pool.rs
+-rw-r--r--   0     1001      127    11458 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/symbols/mod.rs
+-rw-r--r--   0     1001      127    93892 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/tests/mod.rs
+-rw-r--r--   0     1001      127     1664 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/tests/testdata/jumps.bin
+-rw-r--r--   0     1001      127     1838 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/types/array.rs
+-rw-r--r--   0     1001      127     8631 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/types/func.rs
+-rw-r--r--   0     1001      127     2576 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/types/map.rs
+-rw-r--r--   0     1001      127    16503 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/types/mod.rs
+-rw-r--r--   0     1001      127    39044 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/types/structure.rs
+-rw-r--r--   0     1001      127    12650 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/variables.rs
+-rw-r--r--   0     1001      127    14481 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/wasm/builder.rs
+-rw-r--r--   0     1001      127    46413 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/wasm/mod.rs
+-rw-r--r--   0     1001      127     9792 2024-04-30 08:38:48.000000 yara_x-0.2.1/lib/src/wasm/string.rs
+-rw-r--r--   0     1001      127      448 2024-04-30 08:38:48.000000 yara_x-0.2.1/macros/Cargo.toml
+-rw-r--r--   0     1001      127    14420 2024-04-30 08:38:48.000000 yara_x-0.2.1/macros/src/error.rs
+-rw-r--r--   0     1001      127    10584 2024-04-30 08:38:48.000000 yara_x-0.2.1/macros/src/lib.rs
+-rw-r--r--   0     1001      127     3267 2024-04-30 08:38:48.000000 yara_x-0.2.1/macros/src/module_export.rs
+-rw-r--r--   0     1001      127      543 2024-04-30 08:38:48.000000 yara_x-0.2.1/macros/src/module_main.rs
+-rw-r--r--   0     1001      127     1743 2024-04-30 08:38:48.000000 yara_x-0.2.1/macros/src/span.rs
+-rw-r--r--   0     1001      127    10023 2024-04-30 08:38:48.000000 yara_x-0.2.1/macros/src/wasm_export.rs
+-rw-r--r--   0     1001      127     1244 2024-04-30 08:38:48.000000 yara_x-0.2.1/parser/Cargo.toml
+-rw-r--r--   0     1001      127    18222 2024-04-30 08:38:48.000000 yara_x-0.2.1/parser/src/ast/ascii_tree.rs
+-rw-r--r--   0     1001      127    24797 2024-04-30 08:38:48.000000 yara_x-0.2.1/parser/src/ast/mod.rs
+-rw-r--r--   0     1001      127     2838 2024-04-30 08:38:48.000000 yara_x-0.2.1/parser/src/ast/span.rs
+-rw-r--r--   0     1001      127     7532 2024-04-30 08:38:48.000000 yara_x-0.2.1/parser/src/cst/mod.rs
+-rw-r--r--   0     1001      127     1382 2024-04-30 08:38:48.000000 yara_x-0.2.1/parser/src/lib.rs
+-rw-r--r--   0     1001      127     2970 2024-04-30 08:38:48.000000 yara_x-0.2.1/parser/src/parser/context.rs
+-rw-r--r--   0     1001      127    80950 2024-04-30 08:38:48.000000 yara_x-0.2.1/parser/src/parser/cst2ast.rs
+-rw-r--r--   0     1001      127    13191 2024-04-30 08:38:48.000000 yara_x-0.2.1/parser/src/parser/errors.rs
+-rw-r--r--   0     1001      127    14032 2024-04-30 08:38:48.000000 yara_x-0.2.1/parser/src/parser/grammar.pest
+-rw-r--r--   0     1001      127    12336 2024-04-30 08:38:48.000000 yara_x-0.2.1/parser/src/parser/mod.rs
+-rw-r--r--   0     1001      127     2242 2024-04-30 08:38:48.000000 yara_x-0.2.1/parser/src/parser/tests/ast.rs
+-rw-r--r--   0     1001      127    25756 2024-04-30 08:38:48.000000 yara_x-0.2.1/parser/src/parser/tests/cst.rs
+-rw-r--r--   0     1001      127     1549 2024-04-30 08:38:48.000000 yara_x-0.2.1/parser/src/parser/tests/mod.rs
+-rw-r--r--   0     1001      127     3234 2024-04-30 08:38:48.000000 yara_x-0.2.1/parser/src/parser/tests/testdata/arithmetic_ops.yaml
+-rw-r--r--   0     1001      127     1687 2024-04-30 08:38:48.000000 yara_x-0.2.1/parser/src/parser/tests/testdata/bitwise_ops.yaml
+-rw-r--r--   0     1001      127     2973 2024-04-30 08:38:48.000000 yara_x-0.2.1/parser/src/parser/tests/testdata/for_stmt.yaml
+-rw-r--r--   0     1001      127     7108 2024-04-30 08:38:48.000000 yara_x-0.2.1/parser/src/parser/tests/testdata/general.yaml
+-rw-r--r--   0     1001      127     5250 2024-04-30 08:38:48.000000 yara_x-0.2.1/parser/src/parser/tests/testdata/hex_patterns.yaml
+-rw-r--r--   0     1001      127     2357 2024-04-30 08:38:48.000000 yara_x-0.2.1/parser/src/parser/tests/testdata/literals.yaml
+-rw-r--r--   0     1001      127      703 2024-04-30 08:38:48.000000 yara_x-0.2.1/parser/src/parser/tests/testdata/meta.yaml
+-rw-r--r--   0     1001      127     3978 2024-04-30 08:38:48.000000 yara_x-0.2.1/parser/src/parser/tests/testdata/of_stmt.yaml
+-rw-r--r--   0     1001      127      956 2024-04-30 08:38:48.000000 yara_x-0.2.1/parser/src/parser/tests/testdata/regexp_patterns.yaml
+-rw-r--r--   0     1001      127     2243 2024-04-30 08:38:48.000000 yara_x-0.2.1/parser/src/parser/tests/testdata/shift_ops.yaml
+-rw-r--r--   0     1001      127     3563 2024-04-30 08:38:48.000000 yara_x-0.2.1/parser/src/parser/tests/testdata/string_ops.yaml
+-rw-r--r--   0     1001      127     1484 2024-04-30 08:38:48.000000 yara_x-0.2.1/parser/src/parser/tests/testdata/text_patterns.yaml
+-rw-r--r--   0     1001      127     8459 2024-04-30 08:38:48.000000 yara_x-0.2.1/parser/src/report.rs
+-rw-r--r--   0     1001      127     3002 2024-04-30 08:38:48.000000 yara_x-0.2.1/parser/src/warnings.rs
+-rw-r--r--   0     1001      127      686 2024-04-30 08:38:48.000000 yara_x-0.2.1/proto-yaml/Cargo.toml
+-rw-r--r--   0     1001      127      312 2024-04-30 08:38:48.000000 yara_x-0.2.1/proto-yaml/build.rs
+-rw-r--r--   0     1001      127    13959 2024-04-30 08:38:48.000000 yara_x-0.2.1/proto-yaml/src/lib.rs
+-rw-r--r--   0     1001      127      850 2024-04-30 08:38:48.000000 yara_x-0.2.1/proto-yaml/src/tests/mod.rs
+-rw-r--r--   0     1001      127      456 2024-04-30 08:38:48.000000 yara_x-0.2.1/proto-yaml/src/tests/test.proto
+-rw-r--r--   0     1001      127      395 2024-04-30 08:38:48.000000 yara_x-0.2.1/proto-yaml/src/tests/testdata/1.in
+-rw-r--r--   0     1001      127      346 2024-04-30 08:38:48.000000 yara_x-0.2.1/proto-yaml/src/tests/testdata/1.out
+-rw-r--r--   0     1001      127      215 2024-04-30 08:38:48.000000 yara_x-0.2.1/proto-yaml/src/yaml.proto
+-rw-r--r--   0        0        0      540 1970-01-01 00:00:00.000000 yara_x-0.2.1/py/Cargo.toml
+-rw-r--r--   0     1001      127      534 2024-04-30 08:38:48.000000 yara_x-0.2.1/py/README.md
+-rw-r--r--   0     1001      127       71 2024-04-30 08:38:48.000000 yara_x-0.2.1/py/build.rs
+-rw-r--r--   0     1001      127    15598 2024-04-30 08:38:48.000000 yara_x-0.2.1/py/src/lib.rs
+-rw-r--r--   0     1001      127     5947 2024-04-30 08:38:48.000000 yara_x-0.2.1/py/tests/test_api.py
+-rw-r--r--   0     1001      127   123750 2024-04-30 08:38:48.000000 yara_x-0.2.1/Cargo.lock
+-rw-r--r--   0        0        0     2703 1970-01-01 00:00:00.000000 yara_x-0.2.1/Cargo.toml
+-rw-r--r--   0        0        0      709 1970-01-01 00:00:00.000000 yara_x-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1135 1970-01-01 00:00:00.000000 yara_x-0.2.1/PKG-INFO
```

### Comparing `yara_x-0.2.0/parser/Cargo.toml` & `yara_x-0.2.1/parser/Cargo.toml`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/parser/src/ast/ascii_tree.rs` & `yara_x-0.2.1/parser/src/ast/ascii_tree.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/parser/src/ast/mod.rs` & `yara_x-0.2.1/parser/src/ast/mod.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/parser/src/ast/span.rs` & `yara_x-0.2.1/parser/src/ast/span.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/parser/src/cst/mod.rs` & `yara_x-0.2.1/parser/src/cst/mod.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/parser/src/lib.rs` & `yara_x-0.2.1/parser/src/lib.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/parser/src/parser/context.rs` & `yara_x-0.2.1/parser/src/parser/context.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/parser/src/parser/cst2ast.rs` & `yara_x-0.2.1/parser/src/parser/cst2ast.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/parser/src/parser/errors.rs` & `yara_x-0.2.1/parser/src/parser/errors.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/parser/src/parser/grammar.pest` & `yara_x-0.2.1/parser/src/parser/grammar.pest`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/parser/src/parser/mod.rs` & `yara_x-0.2.1/parser/src/parser/mod.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/parser/src/parser/tests/ast.rs` & `yara_x-0.2.1/parser/src/parser/tests/ast.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/parser/src/parser/tests/cst.rs` & `yara_x-0.2.1/parser/src/parser/tests/cst.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/parser/src/parser/tests/mod.rs` & `yara_x-0.2.1/parser/src/parser/tests/mod.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/parser/src/parser/tests/testdata/arithmetic_ops.yaml` & `yara_x-0.2.1/parser/src/parser/tests/testdata/arithmetic_ops.yaml`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/parser/src/parser/tests/testdata/bitwise_ops.yaml` & `yara_x-0.2.1/parser/src/parser/tests/testdata/bitwise_ops.yaml`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/parser/src/parser/tests/testdata/for_stmt.yaml` & `yara_x-0.2.1/parser/src/parser/tests/testdata/for_stmt.yaml`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/parser/src/parser/tests/testdata/general.yaml` & `yara_x-0.2.1/parser/src/parser/tests/testdata/general.yaml`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/parser/src/parser/tests/testdata/hex_patterns.yaml` & `yara_x-0.2.1/parser/src/parser/tests/testdata/hex_patterns.yaml`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/parser/src/parser/tests/testdata/literals.yaml` & `yara_x-0.2.1/parser/src/parser/tests/testdata/literals.yaml`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/parser/src/parser/tests/testdata/meta.yaml` & `yara_x-0.2.1/parser/src/parser/tests/testdata/meta.yaml`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/parser/src/parser/tests/testdata/of_stmt.yaml` & `yara_x-0.2.1/parser/src/parser/tests/testdata/of_stmt.yaml`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/parser/src/parser/tests/testdata/regexp_patterns.yaml` & `yara_x-0.2.1/parser/src/parser/tests/testdata/regexp_patterns.yaml`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/parser/src/parser/tests/testdata/shift_ops.yaml` & `yara_x-0.2.1/parser/src/parser/tests/testdata/shift_ops.yaml`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/parser/src/parser/tests/testdata/string_ops.yaml` & `yara_x-0.2.1/parser/src/parser/tests/testdata/string_ops.yaml`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/parser/src/parser/tests/testdata/text_patterns.yaml` & `yara_x-0.2.1/parser/src/parser/tests/testdata/text_patterns.yaml`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/parser/src/report.rs` & `yara_x-0.2.1/parser/src/report.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/parser/src/warnings.rs` & `yara_x-0.2.1/parser/src/warnings.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/README.md` & `yara_x-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/macros/src/error.rs` & `yara_x-0.2.1/macros/src/error.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/macros/src/lib.rs` & `yara_x-0.2.1/macros/src/lib.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/macros/src/module_export.rs` & `yara_x-0.2.1/macros/src/module_export.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/macros/src/module_main.rs` & `yara_x-0.2.1/macros/src/module_main.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/macros/src/span.rs` & `yara_x-0.2.1/macros/src/span.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/macros/src/wasm_export.rs` & `yara_x-0.2.1/macros/src/wasm_export.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/Cargo.toml` & `yara_x-0.2.1/lib/Cargo.toml`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/build.rs` & `yara_x-0.2.1/lib/build.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/compiler/atoms/mask.rs` & `yara_x-0.2.1/lib/src/compiler/atoms/mask.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/compiler/atoms/mod.rs` & `yara_x-0.2.1/lib/src/compiler/atoms/mod.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/compiler/atoms/quality.rs` & `yara_x-0.2.1/lib/src/compiler/atoms/quality.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/compiler/base64.rs` & `yara_x-0.2.1/lib/src/compiler/base64.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/compiler/context.rs` & `yara_x-0.2.1/lib/src/compiler/context.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/compiler/emit.rs` & `yara_x-0.2.1/lib/src/compiler/emit.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/compiler/errors.rs` & `yara_x-0.2.1/lib/src/compiler/errors.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/compiler/ir/ast2ir.rs` & `yara_x-0.2.1/lib/src/compiler/ir/ast2ir.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/compiler/ir/hex2hir.rs` & `yara_x-0.2.1/lib/src/compiler/ir/hex2hir.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/compiler/ir/mod.rs` & `yara_x-0.2.1/lib/src/compiler/ir/mod.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/compiler/mod.rs` & `yara_x-0.2.1/lib/src/compiler/mod.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/compiler/rules.rs` & `yara_x-0.2.1/lib/src/compiler/rules.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/compiler/tests/mod.rs` & `yara_x-0.2.1/lib/src/compiler/tests/mod.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/compiler/tests/testdata/warnings/24.out` & `yara_x-0.2.1/lib/src/compiler/tests/testdata/warnings/24.out`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/compiler/tests/testdata/warnings/no_warnings.in` & `yara_x-0.2.1/lib/src/compiler/tests/testdata/warnings/no_warnings.in`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/lib.rs` & `yara_x-0.2.1/lib/src/lib.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/modules/add_modules.rs` & `yara_x-0.2.1/lib/src/modules/add_modules.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/modules/console.rs` & `yara_x-0.2.1/lib/src/modules/console.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/modules/dotnet/parser.rs` & `yara_x-0.2.1/lib/src/modules/dotnet/parser.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/modules/dotnet/tests/testdata/605ebe5b5f4b94e1a73e0ad1162bd542e5cb948d1a4ea5a575a14d6b9d6ee849.in` & `yara_x-0.2.1/lib/src/modules/dotnet/tests/testdata/605ebe5b5f4b94e1a73e0ad1162bd542e5cb948d1a4ea5a575a14d6b9d6ee849.in`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/modules/dotnet/tests/testdata/86a1e48cfc843eabfe1b468ef9358c1068950f849c612ab808225b359db0bb8c.in` & `yara_x-0.2.1/lib/src/modules/dotnet/tests/testdata/86a1e48cfc843eabfe1b468ef9358c1068950f849c612ab808225b359db0bb8c.in`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/modules/elf/mod.rs` & `yara_x-0.2.1/lib/src/modules/elf/mod.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/modules/elf/parser.rs` & `yara_x-0.2.1/lib/src/modules/elf/parser.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/modules/elf/tests/mod.rs` & `yara_x-0.2.1/lib/src/modules/elf/tests/mod.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/modules/hash/mod.rs` & `yara_x-0.2.1/lib/src/modules/hash/mod.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/modules/hash/tests/mod.rs` & `yara_x-0.2.1/lib/src/modules/hash/tests/mod.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/modules/lnk/mod.rs` & `yara_x-0.2.1/lib/src/modules/lnk/mod.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/modules/lnk/parser.rs` & `yara_x-0.2.1/lib/src/modules/lnk/parser.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/modules/macho/mod.rs` & `yara_x-0.2.1/lib/src/modules/macho/mod.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/modules/macho/parser.rs` & `yara_x-0.2.1/lib/src/modules/macho/parser.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/modules/macho/tests/mod.rs` & `yara_x-0.2.1/lib/src/modules/macho/tests/mod.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/modules/magic/mod.rs` & `yara_x-0.2.1/lib/src/modules/magic/mod.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/modules/magic/tests/mod.rs` & `yara_x-0.2.1/lib/src/modules/magic/tests/mod.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/modules/math.rs` & `yara_x-0.2.1/lib/src/modules/math.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/modules/mod.rs` & `yara_x-0.2.1/lib/src/modules/mod.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/modules/modules.rs` & `yara_x-0.2.1/lib/src/modules/modules.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/modules/pe/asn1.rs` & `yara_x-0.2.1/lib/src/modules/pe/asn1.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/modules/pe/authenticode.rs` & `yara_x-0.2.1/lib/src/modules/pe/authenticode.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/modules/pe/mod.rs` & `yara_x-0.2.1/lib/src/modules/pe/mod.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/modules/pe/parser.rs` & `yara_x-0.2.1/lib/src/modules/pe/parser.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/modules/pe/rva2off.rs` & `yara_x-0.2.1/lib/src/modules/pe/rva2off.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/modules/pe/tests/mod.rs` & `yara_x-0.2.1/lib/src/modules/pe/tests/mod.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/modules/protos/dotnet.proto` & `yara_x-0.2.1/lib/src/modules/protos/dotnet.proto`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/modules/protos/elf.proto` & `yara_x-0.2.1/lib/src/modules/protos/elf.proto`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/modules/protos/lnk.proto` & `yara_x-0.2.1/lib/src/modules/protos/lnk.proto`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/modules/protos/macho.proto` & `yara_x-0.2.1/lib/src/modules/protos/macho.proto`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/modules/protos/pe.proto` & `yara_x-0.2.1/lib/src/modules/protos/pe.proto`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/modules/protos/test_proto2.proto` & `yara_x-0.2.1/lib/src/modules/protos/test_proto2.proto`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/modules/protos/test_proto3.proto` & `yara_x-0.2.1/lib/src/modules/protos/test_proto3.proto`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/modules/protos/text.proto` & `yara_x-0.2.1/lib/src/modules/protos/text.proto`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/modules/protos/yara.proto` & `yara_x-0.2.1/proto/src/yara.proto`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/modules/string.rs` & `yara_x-0.2.1/lib/src/modules/string.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/modules/test_proto2/mod.rs` & `yara_x-0.2.1/lib/src/modules/test_proto2/mod.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/modules/test_proto2/tests/mod.rs` & `yara_x-0.2.1/lib/src/modules/test_proto2/tests/mod.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/modules/test_proto3/mod.rs` & `yara_x-0.2.1/lib/src/modules/test_proto3/mod.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/modules/tests.rs` & `yara_x-0.2.1/lib/src/modules/tests.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/modules/text.rs` & `yara_x-0.2.1/lib/src/modules/text.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/modules/time.rs` & `yara_x-0.2.1/lib/src/modules/time.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/re/bitmapset.rs` & `yara_x-0.2.1/lib/src/re/bitmapset.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/re/fast/compiler.rs` & `yara_x-0.2.1/lib/src/re/fast/compiler.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/re/fast/fastvm.rs` & `yara_x-0.2.1/lib/src/re/fast/fastvm.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/re/fast/instr.rs` & `yara_x-0.2.1/lib/src/re/fast/instr.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/re/fast/mod.rs` & `yara_x-0.2.1/lib/src/re/fast/mod.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/re/hir.rs` & `yara_x-0.2.1/lib/src/re/hir.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/re/mod.rs` & `yara_x-0.2.1/lib/src/re/mod.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/re/parser.rs` & `yara_x-0.2.1/lib/src/re/parser.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/re/thompson/compiler.rs` & `yara_x-0.2.1/lib/src/re/thompson/compiler.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/re/thompson/instr.rs` & `yara_x-0.2.1/lib/src/re/thompson/instr.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/re/thompson/pikevm.rs` & `yara_x-0.2.1/lib/src/re/thompson/pikevm.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/re/thompson/tests.rs` & `yara_x-0.2.1/lib/src/re/thompson/tests.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/scanner/context.rs` & `yara_x-0.2.1/lib/src/scanner/context.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/scanner/matches.rs` & `yara_x-0.2.1/lib/src/scanner/matches.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/scanner/mod.rs` & `yara_x-0.2.1/lib/src/scanner/mod.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/scanner/tests.rs` & `yara_x-0.2.1/lib/src/scanner/tests.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/string_pool.rs` & `yara_x-0.2.1/lib/src/string_pool.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/symbols/mod.rs` & `yara_x-0.2.1/lib/src/symbols/mod.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/tests/mod.rs` & `yara_x-0.2.1/lib/src/tests/mod.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/types/array.rs` & `yara_x-0.2.1/lib/src/types/array.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/types/func.rs` & `yara_x-0.2.1/lib/src/types/func.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/types/map.rs` & `yara_x-0.2.1/lib/src/types/map.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/types/mod.rs` & `yara_x-0.2.1/lib/src/types/mod.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/types/structure.rs` & `yara_x-0.2.1/lib/src/types/structure.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/variables.rs` & `yara_x-0.2.1/lib/src/variables.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/wasm/builder.rs` & `yara_x-0.2.1/lib/src/wasm/builder.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/wasm/mod.rs` & `yara_x-0.2.1/lib/src/wasm/mod.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/lib/src/wasm/string.rs` & `yara_x-0.2.1/lib/src/wasm/string.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/proto/src/yara.proto` & `yara_x-0.2.1/lib/src/modules/protos/yara.proto`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/proto-yaml/Cargo.toml` & `yara_x-0.2.1/proto-yaml/Cargo.toml`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/proto-yaml/src/lib.rs` & `yara_x-0.2.1/proto-yaml/src/lib.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/proto-yaml/src/tests/mod.rs` & `yara_x-0.2.1/proto-yaml/src/tests/mod.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/py/Cargo.toml` & `yara_x-0.2.1/py/Cargo.toml`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/py/README.md` & `yara_x-0.2.1/py/README.md`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/py/src/lib.rs` & `yara_x-0.2.1/py/src/lib.rs`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/py/tests/test_api.py` & `yara_x-0.2.1/py/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/Cargo.lock` & `yara_x-0.2.1/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -147,14 +147,17 @@
 checksum = "0952808a6c2afd1aa8947271f3a60f1a6763c7b912d210184c5149b5cf147247"
 
 [[package]]
 name = "arbitrary"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7d5a26814d8dcb93b0e5a0ff3c6d80a8843bafb21b39e8e18a6f05471870e110"
+dependencies = [
+ "derive_arbitrary",
+]
 
 [[package]]
 name = "array-bytes"
 version = "6.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6f840fb7195bcfc5e17ea40c26e5ce6d5b9ce5d584466e17703209657e459ae0"
 
@@ -602,14 +605,23 @@
 [[package]]
 name = "clap_lex"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "98cc8fbded0c607b7ba9dd60cd98df59af97e84d24e49c8557331cfc26d301ce"
 
 [[package]]
+name = "cmake"
+version = "0.1.50"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a31c789563b815f77f4250caee12365734369f942439b7defd71e18a48197130"
+dependencies = [
+ "cc",
+]
+
+[[package]]
 name = "colorchoice"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "acbf1af155f9b9ef647e42cdc158db4b64a1b61f743629225fde6f3e0be2a7c7"
 
 [[package]]
 name = "colored_json"
@@ -671,17 +683,17 @@
  "getrandom",
  "once_cell",
  "tiny-keccak",
 ]
 
 [[package]]
 name = "constant_time_eq"
-version = "0.1.5"
+version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "245097e9a4535ee1e3e3931fcfcd55a796a44c643e8596ff6566d68f09b87bbc"
+checksum = "f7144d30dcf0fafbce74250a3963025d8d52177934239851c917d29f1df280c2"
 
 [[package]]
 name = "convert_case"
 version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ec182b0ca2f35d8fc196cf3404988fd8b8c739a4d270ff118a398feb0cbec1ca"
 dependencies = [
@@ -818,14 +830,29 @@
  "log",
  "smallvec",
  "wasmparser 0.201.0",
  "wasmtime-types",
 ]
 
 [[package]]
+name = "crc"
+version = "3.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "69e6e4d7b33a94f0991c26729976b10ebde1d34c3ee82408fb536164fa10d636"
+dependencies = [
+ "crc-catalog",
+]
+
+[[package]]
+name = "crc-catalog"
+version = "2.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "19d374276b40fb8bbdee95aef7c7fa6b5316ec764510eb64b8dd0e2ed0d7e7f5"
+
+[[package]]
 name = "crc32fast"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b3855a8a784b474f333699ef2bbca9db2c4a1f6d9088a90a2d25b1eb53111eaa"
 dependencies = [
  "cfg-if",
 ]
@@ -1012,14 +1039,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef552e6f588e446098f6ba40d89ac146c8c7b64aade83c051ee00bb5d2bc18d"
 dependencies = [
  "uuid",
 ]
 
 [[package]]
+name = "deflate64"
+version = "0.1.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "83ace6c86376be0b6cdcf3fb41882e81d94b31587573d1cfa9d01cd06bba210d"
+
+[[package]]
 name = "deltae"
 version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5729f5117e208430e437df2f4843f5e5952997175992d1414f94c57d61e270b4"
 
 [[package]]
 name = "der"
@@ -1052,14 +1085,25 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b42b6fa04a440b495c8b04d0e71b707c585f83cb9cb28cf8cd0d976c315e31b4"
 dependencies = [
  "powerfmt",
 ]
 
 [[package]]
+name = "derive_arbitrary"
+version = "1.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "67e77553c4162a157adbf834ebae5b415acbecbeafc7a74b0e886657506a7611"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.55",
+]
+
+[[package]]
 name = "diff"
 version = "0.1.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "56254986775e3233ffa9c4d7d3faaf6d36a2c09d30b20687e9f88bc8bafc16c8"
 
 [[package]]
 name = "digest"
@@ -1341,14 +1385,15 @@
 [[package]]
 name = "flate2"
 version = "1.0.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "46303f565772937ffe1d394a4fac6f411c6013172fadde9dcdb1e147a086940e"
 dependencies = [
  "crc32fast",
+ "libz-ng-sys",
  "miniz_oxide",
 ]
 
 [[package]]
 name = "fmmap"
 version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1868,14 +1913,24 @@
 dependencies = [
  "bitflags 2.5.0",
  "libc",
  "redox_syscall",
 ]
 
 [[package]]
+name = "libz-ng-sys"
+version = "1.1.15"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c6409efc61b12687963e602df8ecf70e8ddacf95bc6576bcf16e3ac6328083c5"
+dependencies = [
+ "cmake",
+ "libc",
+]
+
+[[package]]
 name = "lingua"
 version = "1.6.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d109aef84956f04b8b5866db17e59f964152411915ad27b6e291b262d63a442c"
 dependencies = [
  "ahash",
  "brotli",
@@ -1980,14 +2035,24 @@
 [[package]]
 name = "log"
 version = "0.4.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "90ed8c1e510134f979dbc4f070f87d4313098b704861a105fe34231c70a3901c"
 
 [[package]]
+name = "lzma-rs"
+version = "0.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "297e814c836ae64db86b36cf2a557ba54368d03f6afcd7d947c266692f71115e"
+dependencies = [
+ "byteorder",
+ "crc",
+]
+
+[[package]]
 name = "mach"
 version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b823e83b2affd8f40a9ee8c29dbc56404c1e34cd2710921f2801e2cf29527afa"
 dependencies = [
  "libc",
 ]
@@ -2424,40 +2489,27 @@
  "regex",
  "regex-syntax 0.7.5",
  "structmeta",
  "syn 2.0.55",
 ]
 
 [[package]]
-name = "password-hash"
-version = "0.4.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7676374caaee8a325c9e7a2ae557f216c5563a171d6997b0ef8a65af35147700"
-dependencies = [
- "base64ct",
- "rand_core",
- "subtle",
-]
-
-[[package]]
 name = "paste"
 version = "1.0.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "de3145af08024dea9fa9914f381a17b8fc6034dfb00f3a84013f7ff43f29ed4c"
 
 [[package]]
 name = "pbkdf2"
-version = "0.11.0"
+version = "0.12.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "83a0692ec44e4cf1ef28ca317f14f8f07da2d95ec3fa01f86e4467b725e60917"
+checksum = "f8ed6a7761f76e3b9f92dfb0a60a6a6477c61024b775147ff0973a02653abaf2"
 dependencies = [
  "digest 0.10.7",
  "hmac",
- "password-hash",
- "sha2 0.10.8",
 ]
 
 [[package]]
 name = "pem-rfc7468"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "88b39c9bfcfc231068454382784bb460aae594343fb030d46e9f50a645418412"
@@ -3272,14 +3324,20 @@
 checksum = "77549399552de45a898a580c1b41d445bf730df867cc44e6c0233bbc4b8329de"
 dependencies = [
  "digest 0.10.7",
  "rand_core",
 ]
 
 [[package]]
+name = "simd-adler32"
+version = "0.3.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d66dc143e6b11c1eddc06d5c423cfc97062865baf299914ab64caa38182078fe"
+
+[[package]]
 name = "similar"
 version = "2.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "32fea41aca09ee824cc9724996433064c89f7777e60762749a4170a14abbfa21"
 dependencies = [
  "bstr 0.2.17",
  "unicode-segmentation",
@@ -3630,17 +3688,17 @@
  "proc-macro2",
  "quote",
  "syn 2.0.55",
 ]
 
 [[package]]
 name = "time"
-version = "0.3.34"
+version = "0.3.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c8248b6521bb14bc45b4067159b9b6ad792e2d6d754d6c41fb50e29fefe38749"
+checksum = "5dfd88e563464686c916c7e46e623e520ddc6d79fa6641390f2e3fa86e83e885"
 dependencies = [
  "deranged",
  "itoa",
  "num-conv",
  "powerfmt",
  "serde",
  "time-core",
@@ -3651,17 +3709,17 @@
 name = "time-core"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ef927ca75afb808a4d64dd374f00a2adf8d0fcff8e7b184af886c3c87ec4a3f3"
 
 [[package]]
 name = "time-macros"
-version = "0.2.17"
+version = "0.2.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ba3a3ef41e6672a2f0f001392bb5dcd3ff0a9992d618ca761a11c3121547774"
+checksum = "3f252a68540fde3a3877aeea552b832b40ab9a69e318efd078774a01ddee1ccf"
 dependencies = [
  "num-conv",
  "time-core",
 ]
 
 [[package]]
 name = "tiny-keccak"
@@ -3718,14 +3776,20 @@
  "serde",
  "serde_spanned",
  "toml_datetime",
  "winnow",
 ]
 
 [[package]]
+name = "typed-arena"
+version = "2.0.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6af6ae20167a9ece4bcb41af5b80f8a1f1df981f6391189ce00fd257af04126a"
+
+[[package]]
 name = "typenum"
 version = "1.17.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "42ff0bf0c66b8238c6f3b578df37d0b7848e55df8577b3f74f92a69acceeb825"
 
 [[package]]
 name = "ucd-trie"
@@ -4025,15 +4089,15 @@
  "log",
  "rustix",
  "serde",
  "serde_derive",
  "sha2 0.10.8",
  "toml 0.8.12",
  "windows-sys 0.52.0",
- "zstd 0.13.0",
+ "zstd",
 ]
 
 [[package]]
 name = "wasmtime-component-macro"
 version = "19.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "631244bac89c57ebe7283209d86fe175ad5929328e75f61bf9141895cafbf52d"
@@ -4673,15 +4737,15 @@
 name = "yansi"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cfe53a6657fd280eaa890a3bc59152892ffa3e30101319d168b781ed6529b049"
 
 [[package]]
 name = "yara-x"
-version = "0.2.0"
+version = "0.2.1"
 dependencies = [
  "aho-corasick",
  "anyhow",
  "array-bytes",
  "ascii_tree",
  "base64 0.22.0",
  "bincode",
@@ -4741,23 +4805,23 @@
  "yara-x-proto",
  "yara-x-proto-yaml",
  "zip",
 ]
 
 [[package]]
 name = "yara-x-capi"
-version = "0.2.0"
+version = "0.2.1"
 dependencies = [
  "cbindgen",
  "yara-x",
 ]
 
 [[package]]
 name = "yara-x-cli"
-version = "0.2.0"
+version = "0.2.1"
 dependencies = [
  "anyhow",
  "ascii_tree",
  "clap 4.5.3",
  "clap_complete",
  "colored_json",
  "crossbeam",
@@ -4778,38 +4842,38 @@
  "yara-x-fmt",
  "yara-x-parser",
  "yara-x-proto-yaml",
 ]
 
 [[package]]
 name = "yara-x-fmt"
-version = "0.2.0"
+version = "0.2.1"
 dependencies = [
  "anyhow",
  "bitmask",
  "lazy_static",
  "pretty_assertions",
  "thiserror",
  "yara-x-parser",
 ]
 
 [[package]]
 name = "yara-x-macros"
-version = "0.2.0"
+version = "0.2.1"
 dependencies = [
  "convert_case",
  "darling",
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "yara-x-parser"
-version = "0.2.0"
+version = "0.2.1"
 dependencies = [
  "annotate-snippets",
  "ascii_tree",
  "base64 0.22.0",
  "bitmask",
  "bstr 1.9.1",
  "indenter",
@@ -4823,39 +4887,39 @@
  "yaml-rust",
  "yansi 1.0.1",
  "yara-x-macros",
 ]
 
 [[package]]
 name = "yara-x-proto"
-version = "0.2.0"
+version = "0.2.1"
 dependencies = [
  "protobuf",
  "protobuf-codegen",
  "protobuf-parse",
 ]
 
 [[package]]
 name = "yara-x-proto-yaml"
-version = "0.2.0"
+version = "0.2.1"
 dependencies = [
  "chrono",
  "globwalk",
  "goldenfile",
  "itertools 0.12.1",
  "protobuf",
  "protobuf-codegen",
  "protobuf-parse",
  "protobuf-support",
  "yansi 1.0.1",
 ]
 
 [[package]]
 name = "yara-x-py"
-version = "0.2.0"
+version = "0.2.1"
 dependencies = [
  "protobuf-json-mapping",
  "pyo3",
  "pyo3-build-config",
  "pyo3-file",
  "yara-x",
 ]
@@ -4884,71 +4948,68 @@
 name = "zeroize"
 version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "525b4ec142c6b68a2d10f01f7bbf6755599ca3f81ea53b8431b7dd348f5fdb2d"
 
 [[package]]
 name = "zip"
-version = "0.6.6"
+version = "1.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "760394e246e4c28189f19d488c058bf16f564016aefac5d32bb1f3b51d5e9261"
+checksum = "2a23468b4a7a4e9e1e62812f8d1dd614f67f148e2b3faa72f4843bf00b573fd7"
 dependencies = [
  "aes",
+ "arbitrary",
  "byteorder",
  "bzip2",
  "constant_time_eq",
  "crc32fast",
  "crossbeam-utils",
+ "deflate64",
  "flate2",
  "hmac",
+ "lzma-rs",
  "pbkdf2",
  "sha1",
  "time",
- "zstd 0.11.2+zstd.1.5.2",
+ "zopfli",
+ "zstd",
 ]
 
 [[package]]
-name = "zstd"
-version = "0.11.2+zstd.1.5.2"
+name = "zopfli"
+version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "20cc960326ece64f010d2d2107537f26dc589a6573a316bd5b1dba685fa5fde4"
+checksum = "5c1f48f3508a3a3f2faee01629564400bc12260f6214a056d06a3aaaa6ef0736"
 dependencies = [
- "zstd-safe 5.0.2+zstd.1.5.2",
+ "crc32fast",
+ "log",
+ "simd-adler32",
+ "typed-arena",
 ]
 
 [[package]]
 name = "zstd"
-version = "0.13.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bffb3309596d527cfcba7dfc6ed6052f1d39dfbd7c867aa2e865e4a449c10110"
-dependencies = [
- "zstd-safe 7.0.0",
-]
-
-[[package]]
-name = "zstd-safe"
-version = "5.0.2+zstd.1.5.2"
+version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1d2a5585e04f9eea4b2a3d1eca508c4dee9592a89ef6f450c11719da0726f4db"
+checksum = "2d789b1514203a1120ad2429eae43a7bd32b90976a7bb8a05f7ec02fa88cc23a"
 dependencies = [
- "libc",
- "zstd-sys",
+ "zstd-safe",
 ]
 
 [[package]]
 name = "zstd-safe"
-version = "7.0.0"
+version = "7.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "43747c7422e2924c11144d5229878b98180ef8b06cca4ab5af37afc8a8d8ea3e"
+checksum = "1cd99b45c6bc03a018c8b8a86025678c87e55526064e38f9df301989dce7ec0a"
 dependencies = [
  "zstd-sys",
 ]
 
 [[package]]
 name = "zstd-sys"
-version = "2.0.9+zstd.1.5.5"
+version = "2.0.10+zstd.1.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9e16efa8a874a0481a574084d34cc26fdb3b99627480f785888deb6386506656"
+checksum = "c253a4914af5bafc8fa8c86ee400827e83cf6ec01195ec1f1ed8441bf00d65aa"
 dependencies = [
  "cc",
  "pkg-config",
 ]
```

### Comparing `yara_x-0.2.0/Cargo.toml` & `yara_x-0.2.1/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [workspace.package]
-version = "0.2.0"
+version = "0.2.1"
 authors = ["Victor M. Alvarez <vmalvarez@virustotal.com>"]
 edition = "2021"
 homepage = "https://github.com/VirusTotal/yara-x"
 repository = "https://github.com/VirusTotal/yara-x"
 readme = "README.md"
 license = "BSD-3"
 keywords = ["pattern-matching", "cybersecurity", "forensics", "malware", "yara"]
@@ -89,20 +89,20 @@
 uuid = "1.4.1"
 walrus = "0.20.2"
 wasmtime = "19.0.1"
 x509-parser = "0.16.0"
 yaml-rust = "0.4.5"
 yansi = "1.0.1"
 yara-x = { path = "lib" }
-yara-x-fmt = { path = "fmt", version = "0.2.0" }
-yara-x-macros = { path = "macros", version = "0.2.0" }
-yara-x-parser = { path = "parser", version = "0.2.0" }
-yara-x-proto = { path = "proto", version = "0.2.0" }
-yara-x-proto-yaml = { path = "proto-yaml", version = "0.2.0" }
-zip = "0.6.2"
+yara-x-fmt = { path = "fmt", version = "0.2.1" }
+yara-x-macros = { path = "macros", version = "0.2.1" }
+yara-x-parser = { path = "parser", version = "0.2.1" }
+yara-x-proto = { path = "proto", version = "0.2.1" }
+yara-x-proto-yaml = { path = "proto-yaml", version = "0.2.1" }
+zip = "1.1.2"
 
 # Special profile that builds a release binary with link-time optimization. 
 # Compiling with this profile takes a while, but the resulting binary is
 # smaller and better optimized. For building with this profile use:
 #
 # cargo build --profile release-lto
 [profile.release-lto]
```

### Comparing `yara_x-0.2.0/pyproject.toml` & `yara_x-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yara_x-0.2.0/PKG-INFO` & `yara_x-0.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: yara-x
-Version: 0.2.0
+Version: 0.2.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: BSD License
 Summary: Python bindings for YARA-X
 Keywords: pattern-matching,cybersecurity,forensics,malware,yara
 Requires-Python: >=3.8
```

