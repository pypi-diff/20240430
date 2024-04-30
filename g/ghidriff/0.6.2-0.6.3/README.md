# Comparing `tmp/ghidriff-0.6.2.tar.gz` & `tmp/ghidriff-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghidriff-0.6.2.tar", last modified: Fri Feb  2 16:37:34 2024, max compression
+gzip compressed data, was "ghidriff-0.6.3.tar", last modified: Tue Apr 30 17:45:43 2024, max compression
```

## Comparing `ghidriff-0.6.2.tar` & `ghidriff-0.6.3.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 16:37:34.243005 ghidriff-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-02 16:37:22.000000 ghidriff-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    44651 2024-02-02 16:37:34.243005 ghidriff-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    44264 2024-02-02 16:37:22.000000 ghidriff-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 16:37:34.239005 ghidriff-0.6.2/ghidriff/
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-02-02 16:37:22.000000 ghidriff-0.6.2/ghidriff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-02-02 16:37:22.000000 ghidriff-0.6.2/ghidriff/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4951 2024-02-02 16:37:22.000000 ghidriff-0.6.2/ghidriff/bsim.py
--rw-r--r--   0 runner    (1001) docker     (127)    18397 2024-02-02 16:37:22.000000 ghidriff-0.6.2/ghidriff/correlators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-02-02 16:37:22.000000 ghidriff-0.6.2/ghidriff/decomp_correlate.py
--rw-r--r--   0 runner    (1001) docker     (127)    69925 2024-02-02 16:37:22.000000 ghidriff-0.6.2/ghidriff/ghidra_diff_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     8268 2024-02-02 16:37:22.000000 ghidriff-0.6.2/ghidriff/implied_matches.py
--rw-r--r--   0 runner    (1001) docker     (127)    34074 2024-02-02 16:37:22.000000 ghidriff-0.6.2/ghidriff/markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-02-02 16:37:22.000000 ghidriff-0.6.2/ghidriff/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    10763 2024-02-02 16:37:22.000000 ghidriff-0.6.2/ghidriff/simple_diff.py
--rw-r--r--   0 runner    (1001) docker     (127)    13524 2024-02-02 16:37:22.000000 ghidriff-0.6.2/ghidriff/structural_graph_diff.py
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-02-02 16:37:22.000000 ghidriff-0.6.2/ghidriff/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14370 2024-02-02 16:37:22.000000 ghidriff-0.6.2/ghidriff/version_tracking_diff.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 16:37:34.243005 ghidriff-0.6.2/ghidriff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    44651 2024-02-02 16:37:34.000000 ghidriff-0.6.2/ghidriff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-02-02 16:37:34.000000 ghidriff-0.6.2/ghidriff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-02 16:37:34.000000 ghidriff-0.6.2/ghidriff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-02 16:37:34.000000 ghidriff-0.6.2/ghidriff.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-02 16:37:34.000000 ghidriff-0.6.2/ghidriff.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-02 16:37:34.000000 ghidriff-0.6.2/ghidriff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-02 16:37:34.000000 ghidriff-0.6.2/ghidriff.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-02-02 16:37:34.243005 ghidriff-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-02 16:37:22.000000 ghidriff-0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 16:37:34.243005 ghidriff-0.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6881 2024-02-02 16:37:22.000000 ghidriff-0.6.2/tests/test_apple.py
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-02-02 16:37:22.000000 ghidriff-0.6.2/tests/test_decomp_unmatched.py
--rw-r--r--   0 runner    (1001) docker     (127)     8525 2024-02-02 16:37:22.000000 ghidriff-0.6.2/tests/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (127)     7494 2024-02-02 16:37:22.000000 ghidriff-0.6.2/tests/test_ghidra_zip_format_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-02-02 16:37:22.000000 ghidriff-0.6.2/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-02-02 16:37:22.000000 ghidriff-0.6.2/tests/test_pe_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-02-02 16:37:22.000000 ghidriff-0.6.2/tests/test_startup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:45:43.229420 ghidriff-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-30 17:45:33.000000 ghidriff-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    44651 2024-04-30 17:45:43.229420 ghidriff-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    44264 2024-04-30 17:45:33.000000 ghidriff-0.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:45:43.225420 ghidriff-0.6.3/ghidriff/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-30 17:45:33.000000 ghidriff-0.6.3/ghidriff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-04-30 17:45:33.000000 ghidriff-0.6.3/ghidriff/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4951 2024-04-30 17:45:33.000000 ghidriff-0.6.3/ghidriff/bsim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18397 2024-04-30 17:45:33.000000 ghidriff-0.6.3/ghidriff/correlators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-30 17:45:33.000000 ghidriff-0.6.3/ghidriff/decomp_correlate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70357 2024-04-30 17:45:33.000000 ghidriff-0.6.3/ghidriff/ghidra_diff_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8268 2024-04-30 17:45:33.000000 ghidriff-0.6.3/ghidriff/implied_matches.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34074 2024-04-30 17:45:33.000000 ghidriff-0.6.3/ghidriff/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-30 17:45:33.000000 ghidriff-0.6.3/ghidriff/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10763 2024-04-30 17:45:33.000000 ghidriff-0.6.3/ghidriff/simple_diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13524 2024-04-30 17:45:33.000000 ghidriff-0.6.3/ghidriff/structural_graph_diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-04-30 17:45:33.000000 ghidriff-0.6.3/ghidriff/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14370 2024-04-30 17:45:33.000000 ghidriff-0.6.3/ghidriff/version_tracking_diff.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:45:43.229420 ghidriff-0.6.3/ghidriff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    44651 2024-04-30 17:45:43.000000 ghidriff-0.6.3/ghidriff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-30 17:45:43.000000 ghidriff-0.6.3/ghidriff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 17:45:43.000000 ghidriff-0.6.3/ghidriff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-30 17:45:43.000000 ghidriff-0.6.3/ghidriff.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 17:45:43.000000 ghidriff-0.6.3/ghidriff.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-30 17:45:43.000000 ghidriff-0.6.3/ghidriff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 17:45:43.000000 ghidriff-0.6.3/ghidriff.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-30 17:45:43.229420 ghidriff-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-30 17:45:33.000000 ghidriff-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:45:43.229420 ghidriff-0.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6926 2024-04-30 17:45:33.000000 ghidriff-0.6.3/tests/test_apple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-04-30 17:45:33.000000 ghidriff-0.6.3/tests/test_decomp_unmatched.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8525 2024-04-30 17:45:33.000000 ghidriff-0.6.3/tests/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-30 17:45:33.000000 ghidriff-0.6.3/tests/test_gdt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7494 2024-04-30 17:45:33.000000 ghidriff-0.6.3/tests/test_ghidra_zip_format_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-04-30 17:45:33.000000 ghidriff-0.6.3/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-30 17:45:33.000000 ghidriff-0.6.3/tests/test_pe_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-04-30 17:45:33.000000 ghidriff-0.6.3/tests/test_startup.py
```

### Comparing `ghidriff-0.6.2/LICENSE` & `ghidriff-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ghidriff-0.6.2/PKG-INFO` & `ghidriff-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghidriff
-Version: 0.6.2
+Version: 0.6.3
 Summary: Ghidra Binary Diffing Engine
 Home-page: https://github.com/clearbluejar/ghidriff
 Author: clearbluejar
 Author-email: clearbluejar@clearbluejar.com
 License: GPL-3.0 license
 Keywords: patchdiff,binaries,bindiff,ghidra,ghidriff
 Platform: any
```

### Comparing `ghidriff-0.6.2/README.md` & `ghidriff-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `ghidriff-0.6.2/ghidriff/__main__.py` & `ghidriff-0.6.3/ghidriff/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,16 @@
                                      no_symbols=args.no_symbols,
                                      engine_log_path=engine_log_path,
                                      engine_log_level=args.log_level,
                                      engine_file_log_level=args.file_log_level,
                                      min_func_len=args.min_func_len,
                                      use_calling_counts=args.use_calling_counts,
                                      bsim=args.bsim,
-                                     bsim_full=args.bsim_full
+                                     bsim_full=args.bsim_full,
+                                     gdts=args.gdt
                                      )
 
     d.setup_project(binary_paths, project_path, project_name, symbols_path)
 
     d.analyze_project()
 
     diffs = []
```

### Comparing `ghidriff-0.6.2/ghidriff/bsim.py` & `ghidriff-0.6.3/ghidriff/bsim.py`

 * *Files identical despite different names*

### Comparing `ghidriff-0.6.2/ghidriff/correlators.py` & `ghidriff-0.6.3/ghidriff/correlators.py`

 * *Files identical despite different names*

### Comparing `ghidriff-0.6.2/ghidriff/decomp_correlate.py` & `ghidriff-0.6.3/ghidriff/decomp_correlate.py`

 * *Files identical despite different names*

### Comparing `ghidriff-0.6.2/ghidriff/ghidra_diff_engine.py` & `ghidriff-0.6.3/ghidriff/ghidra_diff_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,16 @@
             engine_log_path: Path = None,
             engine_log_level: int = logging.INFO,
             engine_file_log_level: int = logging.INFO,
             max_section_funcs: int = 200,
             min_func_len: int = 10,
             use_calling_counts: bool = False,
             bsim: bool = True,
-            bsim_full: bool = False) -> None:
+            bsim_full: bool = False,
+            gdts: list = []) -> None:
             
 
         # setup engine logging
         self.logger = self.setup_logger(engine_log_level)
 
         self.logger.info('Init Ghidra Diff Engine...')
         self.logger.info(f'Engine Console Log: {engine_log_level}')
@@ -154,17 +155,20 @@
         self.force_analysis = force_analysis
         self.force_diff = force_diff
         self.verbose_analysis = verbose_analysis
         self.no_symbols = no_symbols
 
         # if looking up more than calling_count_funcs_limit symbols, skip function counts
         self.use_calling_counts = use_calling_counts
+
         self.bsim = bsim
         self.bsim_full = bsim_full
 
+        self.gdts = gdts
+
         self.logger.debug(f'{vars(self)}')
 
     @ staticmethod
     def add_ghidra_args_to_parser(parser: argparse.ArgumentParser) -> None:
         """
         Add required Ghidra args to a parser
         """
@@ -188,15 +192,16 @@
                            default='INFO', choices=logging._nameToLevel.keys())
         group.add_argument('--log-path', help='Set ghidriff log path.', default='ghidriff.log')
         group.add_argument('--va', '--verbose-analysis',
                            help='Verbose logging for analysis step.', action='store_true')
         group.add_argument('--min-func-len', help='Minimum function length to consider for diff',
                            type=int, default=10),
         group.add_argument('--use-calling-counts', help='Add calling/called reference counts', default=False, 
-                           action=argparse.BooleanOptionalAction)        
+                           action=argparse.BooleanOptionalAction)
+        group.add_argument('--gdt',action='append', help='Path to GDT file for analysis', default=[])
         
         group = parser.add_argument_group('BSIM Options')
         group.add_argument('--bsim', help='Toggle using BSIM correlation', default=True, 
                            action=argparse.BooleanOptionalAction)
         group.add_argument('--bsim-full', help='Slower but better matching. Use only when needed', default=False, 
                            action=argparse.BooleanOptionalAction)
 
@@ -335,19 +340,20 @@
 
                     # Basic Block Bulker
                     basic_model = BasicBlockModel(func.getProgram(), True)
                     basic_blocks = basic_model.getCodeBlocksContaining(func.getBody(), monitor)
 
                     for block in basic_blocks:
                         code_units = func.getProgram().getListing().getCodeUnits(block, True)
+                        units = []
                         for code in code_units:
-                            blocks.append(str(code.mnemonicString))
+                            units.append(str(code.mnemonicString))
 
-                    # sort - This case handles the case for compiler optimizations
-                    blocks = sorted(blocks)
+                        # sort - This case handles the case for compiler optimizations
+                        blocks.extend(sorted(units))
 
                     if not func.external:
                         error, code = self.decompile_func(func.program, func, timeout,)
 
                         if error:
                             err = f'Failed to decompile {func.program} {func} : {error}'
                             self.logger.warn(err)
@@ -731,41 +737,41 @@
 
         symbolServerService = SymbolServerService(localSymbolStore, sym_servers)
 
         PdbPlugin.saveSymbolServerServiceConfig(symbolServerService)
 
         self.logger.info(f'Symbol Server Configured path: {symbolServerService.toString().strip()}')
 
-    # def apply_gdt(self, program: "ghidra.program.model.listing.Program", gdt_path:  Union[str, Path], verbose: bool = False):
-    #     """
-    #     Apply GDT to program
-    #     """
-
-    #     from ghidra.app.cmd.function import ApplyFunctionDataTypesCmd
-    #     from ghidra.program.model.symbol import SourceType
-    #     from java.io import File
-    #     from java.util import List
-    #     from ghidra.program.model.data import FileDataTypeManager
-    #     from ghidra.util.task import ConsoleTaskMonitor
-
-    #     gdt_path = Path(gdt_path)
-
-    #     if verbose:
-    #         print('Enabling verbose gdt..')
-    #         monitor = ConsoleTaskMonitor()
-    #     else:
-    #         monitor = ConsoleTaskMonitor().DUMMY_MONITOR
-
-    #     archiveGDT = File(gdt_path)
-    #     archiveDTM = FileDataTypeManager.openFileArchive(archiveGDT, False)
-    #     always_replace = True
-    #     createBookmarksEnabled = True
-    #     cmd = ApplyFunctionDataTypesCmd(List.of(archiveDTM), None, SourceType.USER_DEFINED,
-    #                                     always_replace, createBookmarksEnabled)
-    #     cmd.applyTo(program, monitor)
+    def apply_gdt(self, program: "ghidra.program.model.listing.Program", gdt_path:  Union[str, Path], verbose: bool = False):
+        """
+        Apply GDT to program
+        """
+
+        from ghidra.app.cmd.function import ApplyFunctionDataTypesCmd
+        from ghidra.program.model.symbol import SourceType
+        from java.io import File
+        from java.util import List
+        from ghidra.program.model.data import FileDataTypeManager
+        from ghidra.util.task import ConsoleTaskMonitor
+
+        gdt_path = Path(gdt_path)
+
+        if verbose:
+            print('Enabling verbose gdt..')
+            monitor = ConsoleTaskMonitor()
+        else:
+            monitor = ConsoleTaskMonitor().DUMMY_MONITOR
+
+        archiveGDT = File(gdt_path)
+        archiveDTM = FileDataTypeManager.openFileArchive(archiveGDT, False)
+        always_replace = True
+        createBookmarksEnabled = True
+        cmd = ApplyFunctionDataTypesCmd(List.of(archiveDTM), None, SourceType.USER_DEFINED,
+                                        always_replace, createBookmarksEnabled)
+        cmd.applyTo(program, monitor)
 
     def analyze_program(self, df_or_prog: Union["ghidra.framework.model.DomainFile", "ghidra.program.model.listing.Program"], require_symbols: bool, force_analysis: bool = False, verbose_analysis: bool = False):
 
         from ghidra.program.flatapi import FlatProgramAPI
         from ghidra.framework.model import DomainFile
         from ghidra.program.model.listing import Program
         from ghidra.util.task import ConsoleTaskMonitor
@@ -776,17 +782,23 @@
         if isinstance(df_or_prog, DomainFile):
             program = self.project.openProgram("/", df_or_prog.getName(), False)
         elif isinstance(df_or_prog, Program):
             program = df_or_prog
 
         self.logger.info(f"Analyzing: {program}")
 
-        # gdt_names = [name for name in program.getDataTypeManager().getSourceArchives()]
-        # if len(gdt_names) > 0:
-        #     print(f'Using file gdts: {gdt_names}')
+        for gdt in self.gdts:
+            self.logger.info(f"Loading GDT: {gdt}")    
+            if not Path(gdt).exists():
+                raise FileNotFoundError(f'GDT Path not found {gdt}')
+            self.apply_gdt(program,gdt)
+
+        gdt_names = [name for name in program.getDataTypeManager().getSourceArchives()]
+        if len(gdt_names) > 0:
+            print(f'Using file gdts: {gdt_names}')
 
         try:
             if verbose_analysis or self.verbose_analysis:
                 monitor = ConsoleTaskMonitor()
                 flat_api = FlatProgramAPI(program, monitor)
             else:
                 flat_api = FlatProgramAPI(program)
@@ -809,15 +821,15 @@
                 if program and program.getFunctionManager().getFunctionCount() > 1000:
                     self.logger.warn(f"Turning off 'Shared Return Calls' for {program}")
                     self.set_analysis_option_bool(
                         program, 'Shared Return Calls.Assume Contiguous Functions Only', False)
 
                 # TODO make this argument optional, or provide custom analyzer config parsing
                 # This really helps with decompilation, was turned off by default in 10.x
-                # self.set_analysis_option_bool(program, 'Decompiler Parameter ID', True)
+                self.set_analysis_option_bool(program, 'Decompiler Parameter ID', True)
 
                 if self.no_symbols:
                     self.logger.warn(f'Disabling symbols for analysis! --no-symbols flag: {self.no_symbols}')
                     self.set_analysis_option_bool(program, 'PDB Universal', False)
 
                 self.logger.info(f'Starting Ghidra analysis of {program}...')
                 try:
@@ -1708,15 +1720,15 @@
 
             diff_text = self.gen_diff_md(
                 pdiff,
                 side_by_side=side_by_side,
                 max_section_funcs=max_section_funcs,
                 title=md_title)
 
-            with md_path.open('w') as f:
+            with md_path.open('w', encoding='utf-8') as f:
                 f.write(diff_text)
 
         if write_json:
             json_base_path = output_path / 'json'
             json_base_path.mkdir(exist_ok=True)
             json_path = json_base_path / Path(name + '.json')
             self.logger.info(f'Writing pdiff json...')
@@ -1731,19 +1743,19 @@
 
             sxs_diff_htmls = GhidriffMarkdown.gen_sxs_html_from_pdiff(pdiff)
 
             for func_name, sxs_diff_html in sxs_diff_htmls:
 
                 # give line ending md despite html so it will render in gists and vscode
                 sxs_diff_path = sxs_output_path / Path('.'.join([name, _clean_func(func_name), 'md']))
-                sxs_diff_path.write_text(sxs_diff_html)
+                sxs_diff_path.write_text(sxs_diff_html, encoding='utf-8')
 
             combined_sxs_diff_html = GhidriffMarkdown.gen_combined_sxs_html_from_pdiff(pdiff)
             combined_sxs_diff_path = sxs_output_path / Path('.'.join([name, 'combined', 'html']))
-            combined_sxs_diff_path.write_text(combined_sxs_diff_html)
+            combined_sxs_diff_path.write_text(combined_sxs_diff_html, encoding='utf-8')
 
         if write_diff:
             self.logger.info(f'Wrote {md_path}')
         if write_json:
             self.logger.info(f'Wrote {json_path}')
         if side_by_side:
             self.logger.info(f'Wrote {len(sxs_diff_htmls)} sxs hmtl diffs to {sxs_output_path}')
```

### Comparing `ghidriff-0.6.2/ghidriff/implied_matches.py` & `ghidriff-0.6.3/ghidriff/implied_matches.py`

 * *Files identical despite different names*

### Comparing `ghidriff-0.6.2/ghidriff/markdown.py` & `ghidriff-0.6.3/ghidriff/markdown.py`

 * *Files identical despite different names*

### Comparing `ghidriff-0.6.2/ghidriff/parser.py` & `ghidriff-0.6.3/ghidriff/parser.py`

 * *Files identical despite different names*

### Comparing `ghidriff-0.6.2/ghidriff/simple_diff.py` & `ghidriff-0.6.3/ghidriff/simple_diff.py`

 * *Files identical despite different names*

### Comparing `ghidriff-0.6.2/ghidriff/structural_graph_diff.py` & `ghidriff-0.6.3/ghidriff/structural_graph_diff.py`

 * *Files identical despite different names*

### Comparing `ghidriff-0.6.2/ghidriff/utils.py` & `ghidriff-0.6.3/ghidriff/utils.py`

 * *Files identical despite different names*

### Comparing `ghidriff-0.6.2/ghidriff/version_tracking_diff.py` & `ghidriff-0.6.3/ghidriff/version_tracking_diff.py`

 * *Files identical despite different names*

### Comparing `ghidriff-0.6.2/ghidriff.egg-info/PKG-INFO` & `ghidriff-0.6.3/ghidriff.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghidriff
-Version: 0.6.2
+Version: 0.6.3
 Summary: Ghidra Binary Diffing Engine
 Home-page: https://github.com/clearbluejar/ghidriff
 Author: clearbluejar
 Author-email: clearbluejar@clearbluejar.com
 License: GPL-3.0 license
 Keywords: patchdiff,binaries,bindiff,ghidra,ghidriff
 Platform: any
```

### Comparing `ghidriff-0.6.2/ghidriff.egg-info/SOURCES.txt` & `ghidriff-0.6.3/ghidriff.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -21,11 +21,12 @@
 ghidriff.egg-info/entry_points.txt
 ghidriff.egg-info/not-zip-safe
 ghidriff.egg-info/requires.txt
 ghidriff.egg-info/top_level.txt
 tests/test_apple.py
 tests/test_decomp_unmatched.py
 tests/test_diff.py
+tests/test_gdt.py
 tests/test_ghidra_zip_format_import.py
 tests/test_import.py
 tests/test_pe_parsing.py
 tests/test_startup.py
```

### Comparing `ghidriff-0.6.2/setup.cfg` & `ghidriff-0.6.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `ghidriff-0.6.2/tests/test_apple.py` & `ghidriff-0.6.3/tests/test_apple.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
                          pdiff,
                          output_path,
                          side_by_side=args.side_by_side,
                          max_section_funcs=args.max_section_funcs,
                          md_title=args.md_title)
 
     assert len(pdiff['functions']['modified']) == 39 
-    assert len(pdiff['functions']['added']) == 6
+    assert (len(pdiff['functions']['added']) == 6 or len(pdiff['functions']['added']) == 14)
     assert len(pdiff['functions']['deleted']) == 0
 
 
 @pytest.mark.forked
 def test_diff_macos_macho_x64(shared_datadir: Path):
     """
     Tests end to end diff of CVE
@@ -179,8 +179,8 @@
 
     # no changes
     assert len(pdiff['functions']['modified']) == 0
     assert len(pdiff['functions']['added']) == 0
     assert len(pdiff['functions']['deleted']) == 0
 
     # 100 % match
-    assert pdiff['stats']['func_match_overall_percent'] == '100.0000%'
+    assert pdiff['stats']['func_match_overall_percent'] == '100.0000%'
```

### Comparing `ghidriff-0.6.2/tests/test_decomp_unmatched.py` & `ghidriff-0.6.3/tests/test_decomp_unmatched.py`

 * *Files identical despite different names*

### Comparing `ghidriff-0.6.2/tests/test_diff.py` & `ghidriff-0.6.3/tests/test_diff.py`

 * *Files identical despite different names*

### Comparing `ghidriff-0.6.2/tests/test_ghidra_zip_format_import.py` & `ghidriff-0.6.3/tests/test_ghidra_zip_format_import.py`

 * *Files identical despite different names*

### Comparing `ghidriff-0.6.2/tests/test_import.py` & `ghidriff-0.6.3/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `ghidriff-0.6.2/tests/test_pe_parsing.py` & `ghidriff-0.6.3/tests/test_pe_parsing.py`

 * *Files identical despite different names*

### Comparing `ghidriff-0.6.2/tests/test_startup.py` & `ghidriff-0.6.3/tests/test_startup.py`

 * *Files identical despite different names*

