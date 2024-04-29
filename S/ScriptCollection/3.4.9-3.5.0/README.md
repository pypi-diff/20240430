# Comparing `tmp/ScriptCollection-3.4.9-py3-none-any.whl.zip` & `tmp/ScriptCollection-3.5.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 62115 bytes, number of entries: 14
--rw-rw-rw-  2.0 fat    19005 b- defN 23-Jul-30 19:20 ScriptCollection/Executables.py
--rw-rw-rw-  2.0 fat    34378 b- defN 23-Jun-27 21:57 ScriptCollection/GeneralUtilities.py
--rw-rw-rw-  2.0 fat     1937 b- defN 22-Aug-30 21:59 ScriptCollection/ProgramRunnerBase.py
--rw-rw-rw-  2.0 fat     6275 b- defN 23-May-26 16:46 ScriptCollection/ProgramRunnerEpew.py
--rw-rw-rw-  2.0 fat     3023 b- defN 22-Aug-30 21:59 ScriptCollection/ProgramRunnerPopen.py
--rw-rw-rw-  2.0 fat    94475 b- defN 23-Jul-30 19:20 ScriptCollection/ScriptCollectionCore.py
--rw-rw-rw-  2.0 fat   145487 b- defN 23-Jul-30 19:20 ScriptCollection/TasksForCommonProjectStructure.py
--rw-rw-rw-  2.0 fat     7918 b- defN 22-Aug-30 21:59 ScriptCollection/UpdateCertificates.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Aug-29 05:45 ScriptCollection/__init__.py
--rw-rw-rw-  2.0 fat     7650 b- defN 23-Jul-30 19:20 ScriptCollection-3.4.9.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-30 19:20 ScriptCollection-3.4.9.dist-info/WHEEL
--rw-rw-rw-  2.0 fat     2088 b- defN 23-Jul-30 19:20 ScriptCollection-3.4.9.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       17 b- defN 23-Jul-30 19:20 ScriptCollection-3.4.9.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1290 b- defN 23-Jul-30 19:20 ScriptCollection-3.4.9.dist-info/RECORD
-14 files, 323635 bytes uncompressed, 59933 bytes compressed:  81.5%
+Zip file size: 67295 bytes, number of entries: 14
+-rw-rw-rw-  2.0 fat    19282 b- defN 24-Apr-13 12:26 ScriptCollection/Executables.py
+-rw-rw-rw-  2.0 fat    35589 b- defN 24-Apr-13 12:26 ScriptCollection/GeneralUtilities.py
+-rw-rw-rw-  2.0 fat     1937 b- defN 23-Nov-04 23:28 ScriptCollection/ProgramRunnerBase.py
+-rw-rw-rw-  2.0 fat     6275 b- defN 23-Nov-04 23:28 ScriptCollection/ProgramRunnerEpew.py
+-rw-rw-rw-  2.0 fat     3158 b- defN 24-Apr-29 20:42 ScriptCollection/ProgramRunnerPopen.py
+-rw-rw-rw-  2.0 fat    92657 b- defN 24-Apr-29 20:42 ScriptCollection/ScriptCollectionCore.py
+-rw-rw-rw-  2.0 fat   173711 b- defN 24-Apr-29 20:42 ScriptCollection/TasksForCommonProjectStructure.py
+-rw-rw-rw-  2.0 fat     7914 b- defN 24-Apr-13 12:26 ScriptCollection/UpdateCertificates.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Nov-04 23:28 ScriptCollection/__init__.py
+-rw-rw-rw-  2.0 fat     7648 b- defN 24-Apr-29 20:43 ScriptCollection-3.5.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-29 20:43 ScriptCollection-3.5.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat     2153 b- defN 24-Apr-29 20:43 ScriptCollection-3.5.0.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       17 b- defN 24-Apr-29 20:43 ScriptCollection-3.5.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1290 b- defN 24-Apr-29 20:43 ScriptCollection-3.5.0.dist-info/RECORD
+14 files, 351723 bytes uncompressed, 65113 bytes compressed:  81.5%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: ScriptCollection/UpdateCertificates.py
 Comment: 
 
 Filename: ScriptCollection/__init__.py
 Comment: 
 
-Filename: ScriptCollection-3.4.9.dist-info/METADATA
+Filename: ScriptCollection-3.5.0.dist-info/METADATA
 Comment: 
 
-Filename: ScriptCollection-3.4.9.dist-info/WHEEL
+Filename: ScriptCollection-3.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: ScriptCollection-3.4.9.dist-info/entry_points.txt
+Filename: ScriptCollection-3.5.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: ScriptCollection-3.4.9.dist-info/top_level.txt
+Filename: ScriptCollection-3.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: ScriptCollection-3.4.9.dist-info/RECORD
+Filename: ScriptCollection-3.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ScriptCollection/Executables.py

```diff
@@ -4,30 +4,19 @@
 import traceback
 import keyboard
 from .TasksForCommonProjectStructure import TasksForCommonProjectStructure
 from .ScriptCollectionCore import ScriptCollectionCore
 from .GeneralUtilities import GeneralUtilities
 
 
-def DotNetsign() -> int:
-    parser = argparse.ArgumentParser(description='Signs a dll- or exe-file with a snk-file. Requires ilasm and ildasm as available commandline-commands.')
-    parser.add_argument("dllOrExefile")
-    parser.add_argument("snkfile")
-    parser.add_argument("verbose", action='store_true')
-    args = parser.parse_args()
-    ScriptCollectionCore().dotnet_sign(args.dllOrExefile, args.snkfile, args.verbose)
-    return 0
-
-
 def FilenameObfuscator() -> int:
     parser = argparse.ArgumentParser(description=''''Obfuscates the names of all files in the given folder.
 Caution: This script can cause harm if you pass a wrong inputfolder-argument.''')
 
-    parser.add_argument('--printtableheadline', type=GeneralUtilities.string_to_boolean, const=True, default=True, nargs='?',
-                        help='Prints column-titles in the name-mapping-csv-file')
+    parser.add_argument('--printtableheadline', type=GeneralUtilities.string_to_boolean, const=True, default=True, nargs='?',                        help='Prints column-titles in the name-mapping-csv-file')
     parser.add_argument('--namemappingfile', default="NameMapping.csv", help='Specifies the file where the name-mapping will be written to')
     parser.add_argument('--extensions', default="exe,py,sh",
                         help='Comma-separated list of file-extensions of files where this tool should be applied. Use "*" to obfuscate all')
     parser.add_argument('--inputfolder', help='Specifies the foldere where the files are stored whose names should be obfuscated', required=True)
 
     args = parser.parse_args()
     ScriptCollectionCore().SCFilenameObfuscator(args.inputfolder, args.printtableheadline, args.namemappingfile, args.extensions)
@@ -64,16 +53,15 @@
     parser.add_argument('--transactionsmerkleroot', help='Hashvalue of the merkle-root of the transactions which are contained in the block', required=True)
     parser.add_argument('--timestamp', help='Timestamp of the block', required=True)
     parser.add_argument('--target', help='difficulty', required=True)
     parser.add_argument('--nonce', help='Arbitrary 32-bit-integer-value', required=True)
     args = parser.parse_args()
 
     args = parser.parse_args()
-    GeneralUtilities.write_message_to_stdout(ScriptCollectionCore().SCCalculateBitcoinBlockHash(args.version, args.previousblockhash,
-                                                                                                args.transactionsmerkleroot, args.timestamp, args.target, args.nonce))
+    GeneralUtilities.write_message_to_stdout(ScriptCollectionCore().SCCalculateBitcoinBlockHash(args.version, args.previousblockhash,                                                                                                args.transactionsmerkleroot, args.timestamp, args.target, args.nonce))
     return 0
 
 
 def Show2FAAsQRCode():
 
     parser = argparse.ArgumentParser(description="""Always when you use 2-factor-authentication you have the problem:
 Where to backup the secret-key so that it is easy to re-setup them when you have a new phone?
@@ -143,17 +131,15 @@
     parser.add_argument("--sort", help="Sort lines", action='store_true')
     parser.add_argument("--remove_duplicated_lines", help="Remove duplicate lines", action='store_true')
     parser.add_argument("--ignore_first_line", help="Ignores the first line in the file", action='store_true')
     parser.add_argument("--remove_empty_lines", help="Removes lines which are empty or contains only whitespaces", action='store_true')
     parser.add_argument('--ignored_start_character', default="", help='Characters which should not be considered at the begin of a line')
 
     args = parser.parse_args()
-    return ScriptCollectionCore().sc_organize_lines_in_file(args.file, args.encoding,
-                                                            args.sort, args.remove_duplicated_lines, args.ignore_first_line,
-                                                            args.remove_empty_lines, list(args.ignored_start_character))
+    return ScriptCollectionCore().sc_organize_lines_in_file(args.file, args.encoding,                                                            args.sort, args.remove_duplicated_lines, args.ignore_first_line,                                                            args.remove_empty_lines, list(args.ignored_start_character))
 
 
 def CreateHashOfAllFiles() -> int:
     parser = argparse.ArgumentParser(description='Calculates the SHA-256-value of all files in the given folder and stores the hash-value in a file next to the hashed file.')
     parser.add_argument('folder', help='Folder where the files are stored which should be hashed')
     args = parser.parse_args()
     ScriptCollectionCore().SCCreateHashOfAllFiles(args.folder)
@@ -270,32 +256,44 @@
 
 def BuildCodeUnit() -> int:
     parser = argparse.ArgumentParser()
     parser.add_argument('--codeunitfolder', required=False, default=".")
     parser.add_argument('--verbosity', required=False, default=1)
     parser.add_argument('--targetenvironment', required=False, default="Development")
     parser.add_argument('--additionalargumentsfile', required=False, default=None)
-    parser.add_argument('--assume_dependent_codeunits_are_already_built', type=GeneralUtilities.string_to_boolean, const=True, default=False, nargs='?',)
+    parser.add_argument('--assume_dependent_codeunits_are_already_built', type=GeneralUtilities.string_to_boolean, const=True, default=False, nargs='?')
     args = parser.parse_args()
-    TasksForCommonProjectStructure().build_codeunit(args.codeunitfolder, int(args.verbosity), args.targetenvironment, args.additionalargumentsfile,
-                                                    False, None, args.assume_dependent_codeunits_are_already_built)
+    TasksForCommonProjectStructure().build_codeunit(args.codeunitfolder, int(args.verbosity), args.targetenvironment, args.additionalargumentsfile,                                                    False, None, args.assume_dependent_codeunits_are_already_built)
     return 0
 
 
 def BuildCodeUnits() -> int:
     parser = argparse.ArgumentParser()
     parser.add_argument('--repositoryfolder', required=False, default=".")
     parser.add_argument('--verbosity', required=False, default=1)
     parser.add_argument('--targetenvironment', required=False, default="Development")
     parser.add_argument('--additionalargumentsfile', required=False, default=None)
     args = parser.parse_args()
     TasksForCommonProjectStructure().build_codeunits(args.repositoryfolder, int(args.verbosity), args.targetenvironment, args.additionalargumentsfile)
     return 0
 
 
+def BuildCodeUnitsC() -> int:
+    parser = argparse.ArgumentParser()
+    parser.add_argument('--repositoryfolder', required=False, default=".")
+    parser.add_argument('--verbosity', required=False, default=1)
+    parser.add_argument('--targetenvironment', required=False, default="QualityCheck")
+    parser.add_argument('--additionalargumentsfile', required=False, default=None)
+    parser.add_argument('--image', required=False, default="scbuilder:latest")
+    args = parser.parse_args()
+    GeneralUtilities.reconfigure_standrd_input_and_outputs()
+    TasksForCommonProjectStructure().build_codeunitsC(args.repositoryfolder, args.image, int(args.verbosity), args.targetenvironment, args.additionalargumentsfile)
+    return 0
+
+
 def GenerateCertificateAuthority() -> int:
     parser = argparse.ArgumentParser()
     parser.add_argument('--name', required=True)
     parser.add_argument('--subj_c', required=True)
     parser.add_argument('--subj_st', required=True)
     parser.add_argument('--subj_l', required=True)
     parser.add_argument('--subj_o', required=True)
@@ -315,16 +313,15 @@
     parser.add_argument('--subj_st', required=True)
     parser.add_argument('--subj_l', required=True)
     parser.add_argument('--subj_o', required=True)
     parser.add_argument('--subj_ou', required=True)
     parser.add_argument('--days_until_expire', required=False, default=None, type=int)
     parser.add_argument('--password', required=False, default=None)
     args = parser.parse_args()
-    ScriptCollectionCore().generate_certificate(os.getcwd(), args.domain, args.filename, args.subj_c, args.subj_st,
-                                                args.subj_l, args.subj_o, args.subj_ou, args.days_until_expire, args.password)
+    ScriptCollectionCore().generate_certificate(os.getcwd(), args.domain, args.filename, args.subj_c, args.subj_st,                                                args.subj_l, args.subj_o, args.subj_ou, args.days_until_expire, args.password)
     return 0
 
 
 def GenerateCertificateSignRequest() -> int:
     parser = argparse.ArgumentParser()
     parser.add_argument('--filename', required=True)
     parser.add_argument('--domain', required=True)
```

## ScriptCollection/GeneralUtilities.py

```diff
@@ -1,33 +1,37 @@
 import codecs
+import platform
 import inspect
 import ctypes
 import hashlib
 import re
 import os
 import shutil
 import urllib
 import stat
 import secrets
 import string as strin
 import sys
 import traceback
-from datetime import datetime, timedelta
+import warnings
+import functools
+from datetime import datetime, timedelta, date
 from os import listdir
 from os.path import isfile, join, isdir
 from pathlib import Path
 from shutil import copyfile
 import typing
 from defusedxml.minidom import parse
 from OpenSSL import crypto
 
 
 class GeneralUtilities:
 
-    __date_format: str = "%Y-%m-%dT%H:%M:%S"
+    __datetime_format: str = "%Y-%m-%dT%H:%M:%S"
+    __date_format: str = "%Y-%m-%d"
 
     @staticmethod
     def get_modest_dark_url() -> str:
         return "https://aniondev.github.io/CDN/ScriptCollectionDesigns/ModestDark/Style.css"
 
     @staticmethod
     def is_generic(t: typing.Type):
@@ -43,28 +47,36 @@
                 arguments.pop(0)
             for index, argument in enumerate(arguments):
                 if argument is not None:  # Check type of None is not possible. None is always a valid argument-value
                     if parameters[index] in function.__annotations__:  # Check if a type-hint for parameter exist. If not, no parameter-type available for argument-type-check
                         # Check type of arguments if the type is a generic type seems to be impossible.
                         if not GeneralUtilities.is_generic(function.__annotations__[parameters[index]]):
                             if not isinstance(argument, function.__annotations__[parameters[index]]):
-                                raise TypeError(f"Argument with index {index} for function {function.__name__} ('{str(argument)}') is not of type " +
-                                                f"{ function.__annotations__[parameters[index]]} but has type "+str(type(argument)))
+                                raise TypeError(f"Argument with index {index} for function {function.__name__} ('{str(argument)}') is not of type { function.__annotations__[parameters[index]]} but has type "+str(type(argument)))
             for index, named_argument in enumerate(named_args):
                 if named_args[named_argument] is not None:
                     if parameters[index] in function.__annotations__:
                         if not GeneralUtilities.is_generic(function.__annotations__.get(named_argument)):
                             if not isinstance(named_args[named_argument], function.__annotations__.get(named_argument)):
-                                raise TypeError(f"Argument with name {named_argument} for function {function.__name__} ('{str(named_args[named_argument])}') " +
-                                                f"is not of type { function.__annotations__.get(named_argument)}")
+                                raise TypeError(f"Argument with name {named_argument} for function {function.__name__} ('{str(named_args[named_argument])}') is not of type { function.__annotations__.get(named_argument)}")
             return function(*args, **named_args)
         __check_function.__doc__ = function.__doc__
         return __check_function
 
     @staticmethod
+    def deprecated(func):
+        @functools.wraps(func)
+        def new_func(*args, **kwargs):
+            warnings.simplefilter('always', DeprecationWarning)
+            warnings.warn(f"Call to deprecated function {func.__name__}",                        category=DeprecationWarning,                        stacklevel=2)
+            warnings.simplefilter('default', DeprecationWarning)
+            return func(*args, **kwargs)
+        return new_func
+
+    @staticmethod
     @check_arguments
     def args_array_surround_with_quotes_if_required(arguments: list[str]) -> list[str]:
         result = []
         for argument in arguments:
             if " " in argument and not (argument.startswith('"') and argument.endswith('"')):
                 result.append(f'"{argument}"')
             else:
@@ -91,21 +103,32 @@
                     result.append(line)
             else:
                 result.append(line)
         return result
 
     @staticmethod
     @check_arguments
+    def string_to_datetime(value: str) -> datetime:
+        return datetime.strptime(value, GeneralUtilities.__datetime_format)  # value ="2022-10-06T19:26:01" for example
+
+    @staticmethod
+    @check_arguments
     def datetime_to_string(value: datetime) -> str:
-        return value.strftime(GeneralUtilities.__date_format)  # returns "2022-10-06T19:26:01" for example
+        return value.strftime(GeneralUtilities.__datetime_format)  # returns "2022-10-06T19:26:01" for example
 
     @staticmethod
     @check_arguments
-    def string_to_datetime(value: str) -> datetime:
-        return datetime.strptime(value, GeneralUtilities.__date_format)  # value ="2022-10-06T19:26:01" for example
+    def string_to_date(value: str) -> date:
+        splitted = value.split("-")
+        return date(int(splitted[0]), int(splitted[1]), int(splitted[2]))  # value ="2022-10-06" for example
+
+    @staticmethod
+    @check_arguments
+    def date_to_string(value: date) -> str:
+        return value.strftime(GeneralUtilities.__date_format)  # returns "2022-10-06" for example
 
     @staticmethod
     @check_arguments
     def copy_content_of_folder(source_directory: str, target_directory: str, overwrite_existing_files=False) -> None:
         GeneralUtilities.__copy_or_move_content_of_folder(source_directory, target_directory, overwrite_existing_files, False)
 
     @staticmethod
@@ -196,17 +219,25 @@
     def replace_underscores_in_file(file: str, replacements: dict, encoding: str = "utf-8"):
         text = GeneralUtilities.read_text_from_file(file, encoding)
         text = GeneralUtilities.replace_underscores_in_text(text, replacements)
         GeneralUtilities.write_text_to_file(file, text, encoding)
 
     @staticmethod
     @check_arguments
+    def reconfigure_standrd_input_and_outputs():
+        sys.stdin.reconfigure(encoding='utf-8')
+        sys.stderr.reconfigure(encoding='utf-8')
+        sys.stdout.reconfigure(encoding='utf-8')
+
+    @staticmethod
+    @check_arguments
     def write_message_to_stdout(message: str):
-        sys.stdout.write(GeneralUtilities.str_none_safe(message)+"\n")
-        sys.stdout.flush()
+        for line in GeneralUtilities.string_to_lines(message):
+            sys.stdout.write(GeneralUtilities.str_none_safe(line)+"\n")
+            sys.stdout.flush()
 
     @staticmethod
     @check_arguments
     def write_message_to_stderr(message: str):
         sys.stderr.write(GeneralUtilities.str_none_safe(message)+"\n")
         sys.stderr.flush()
 
@@ -446,26 +477,26 @@
         lines = [GeneralUtilities.strip_new_line_character(line) for line in lines]
         content = os.linesep.join(lines)
         GeneralUtilities.write_text_to_file(file, content, encoding)
 
     @staticmethod
     @check_arguments
     def write_text_to_file(file: str, content: str, encoding="utf-8") -> None:
-        GeneralUtilities.write_binary_to_file(file, bytearray(content, encoding))
+        GeneralUtilities.write_binary_to_file(file, bytes(bytearray(content, encoding)))
 
     @staticmethod
     @check_arguments
-    def write_binary_to_file(file: str, content: bytearray) -> None:
+    def write_binary_to_file(file: str, content: bytes) -> None:
         with open(file, "wb") as file_object:
             file_object.write(content)
 
     @staticmethod
     @check_arguments
     def read_lines_from_file(file: str, encoding="utf-8") -> list[str]:
-        return [GeneralUtilities.strip_new_line_character(line) for line in GeneralUtilities.read_text_from_file(file, encoding).split(os.linesep)]
+        return [GeneralUtilities.strip_new_line_character(line) for line in GeneralUtilities.read_text_from_file(file, encoding).split('\n')]
 
     @staticmethod
     @check_arguments
     def read_text_from_file(file: str, encoding="utf-8") -> str:
         return GeneralUtilities.bytes_to_string(GeneralUtilities.read_binary_from_file(file), encoding)
 
     @staticmethod
@@ -694,15 +725,15 @@
             if (re.match(regex, line)):
                 return True
         return False
 
     @staticmethod
     @check_arguments
     def read_csv_file(file: str, ignore_first_line: bool = False, treat_number_sign_at_begin_of_line_as_comment: bool = True, trim_values: bool = True,
-                      encoding="utf-8", ignore_empty_lines: bool = True, separator_character: str = ";", values_are_surrounded_by_quotes: bool = False) -> list[str]:
+                      encoding="utf-8", ignore_empty_lines: bool = True, separator_character: str = ";", values_are_surrounded_by_quotes: bool = False) -> list[list[str]]:
         lines = GeneralUtilities.read_lines_from_file(file, encoding)
 
         if ignore_first_line:
             lines = lines[1:]
         result = list()
         line: str
         for line_loopvariable in lines:
@@ -743,23 +774,17 @@
         try:
             return shutil.which("epew") is not None
         except:
             return False
 
     @staticmethod
     @check_arguments
+    @deprecated
     def absolute_file_paths(directory: str) -> list[str]:
-        for dirpath, _, filenames in os.walk(directory):
-            for filename in filenames:
-                yield os.path.abspath(os.path.join(dirpath, filename))
-
-    @staticmethod
-    @check_arguments
-    def os_is_linux() -> bool:
-        return sys.platform in ('linux', 'linux2')
+        return GeneralUtilities.get_all_files_of_folder(directory)
 
     @staticmethod
     @check_arguments
     def to_list(list_as_string: str, separator: str = ",") -> list[str]:
         result = list()
         if list_as_string is not None:
             list_as_string = list_as_string.strip()
@@ -795,14 +820,22 @@
     @staticmethod
     @check_arguments
     def assert_condition(condition: bool, information: str) -> None:
         if (not condition):
             raise ValueError("Condition failed. "+information)
 
     @staticmethod
+    def current_system_is_windows():
+        return platform.system() == 'Windows'
+
+    @staticmethod
+    def current_system_is_linux():
+        return platform.system() == 'Linux'
+
+    @staticmethod
     @check_arguments
     def get_certificate_expiry_date(certificate_file: str) -> datetime:
         with open(certificate_file, encoding="utf-8") as certificate_file_content:
             cert = crypto.load_certificate(crypto.FILETYPE_PEM, certificate_file_content.read())
             date_as_bytes = cert.get_notAfter()
             date_as_string = date_as_bytes.decode("utf-8")
             result = datetime.strptime(date_as_string, '%Y%m%d%H%M%SZ')
```

## ScriptCollection/ProgramRunnerPopen.py

```diff
@@ -1,28 +1,26 @@
-import os
+import sys
 from subprocess import PIPE, Popen
 from .GeneralUtilities import GeneralUtilities
 from .ProgramRunnerBase import ProgramRunnerBase
 
 
 class ProgramRunnerPopen(ProgramRunnerBase):
 
     @GeneralUtilities.check_arguments
     def run_program_argsasarray_async_helper(self, program: str, arguments_as_array: list[str] = [], working_directory: str = None, custom_argument: object = None) -> Popen:
         arguments_for_process = [program]
         arguments_for_process.extend(arguments_as_array)
         # "shell=True" is not allowed because it is not recommended and also something like
         # "ScriptCollectionCore().run_program('curl', 'https://example.com/dataset?id=1&format=json')"
         # would not be possible anymore because the ampersand will be treated as shell-command.
-        cwd = os.getcwd()
         try:
-            os.chdir(working_directory)
-            result = Popen(arguments_for_process, stdout=PIPE, stderr=PIPE, shell=False)  # pylint: disable=consider-using-with
-        finally:
-            os.chdir(cwd)
+            result = Popen(arguments_for_process, cwd=working_directory, stdin=sys.stdin, stdout=PIPE, stderr=PIPE, shell=False)  # pylint: disable=consider-using-with
+        except FileNotFoundError as fileNotFoundError:
+            raise FileNotFoundError(f"Starting '{program}' in '{working_directory}' resulted in a FileNotFoundError: '{fileNotFoundError.filename}'")
         return result
 
     # Return-values program_runner: Exitcode, StdOut, StdErr, Pid
     @GeneralUtilities.check_arguments
     def wait(self, process: Popen, custom_argument: object) -> tuple[int, str, str, int]:
         pid = process.pid
         stdout, stderr = process.communicate()
```

## ScriptCollection/ScriptCollectionCore.py

```diff
@@ -1,8 +1,10 @@
+import time
 from datetime import timedelta, datetime
+import json
 import binascii
 import filecmp
 import hashlib
 from io import BytesIO
 import itertools
 import math
 import os
@@ -15,25 +17,23 @@
 import uuid
 import tempfile
 import io
 import requests
 import ntplib
 import qrcode
 import pycdlib
-from PIL import Image
 import send2trash
-import fitz
 import PyPDF2
 from .GeneralUtilities import GeneralUtilities
 from .ProgramRunnerBase import ProgramRunnerBase
 from .ProgramRunnerPopen import ProgramRunnerPopen
 from .ProgramRunnerEpew import ProgramRunnerEpew, CustomEpewArgument
 
 
-version = "3.4.9"
+version = "3.5.0"
 __version__ = version
 
 
 class ScriptCollectionCore:
 
     # The purpose of this property is to use it when testing your code which uses scriptcollection for external program-calls.
     # Do not change this value for productive environments.
@@ -69,181 +69,129 @@
                 errors.append(line)
             return (True, errors)
 
         return (False, errors)
 
     @GeneralUtilities.check_arguments
     def replace_version_in_dockerfile_file(self, dockerfile: str, new_version_value: str) -> None:
-        GeneralUtilities.write_text_to_file(dockerfile, re.sub("ARG Version=\"\\d+\\.\\d+\\.\\d+\"", f"ARG Version=\"{new_version_value}\"",
-                                                               GeneralUtilities.read_text_from_file(dockerfile)))
+        GeneralUtilities.write_text_to_file(dockerfile, re.sub("ARG Version=\"\\d+\\.\\d+\\.\\d+\"", f"ARG Version=\"{new_version_value}\"",                                                               GeneralUtilities.read_text_from_file(dockerfile)))
 
     @GeneralUtilities.check_arguments
     def replace_version_in_python_file(self, file: str, new_version_value: str):
-        GeneralUtilities.write_text_to_file(file, re.sub("version = \"\\d+\\.\\d+\\.\\d+\"", f"version = \"{new_version_value}\"",
-                                                         GeneralUtilities.read_text_from_file(file)))
+        GeneralUtilities.write_text_to_file(file, re.sub("version = \"\\d+\\.\\d+\\.\\d+\"", f"version = \"{new_version_value}\"",                                                         GeneralUtilities.read_text_from_file(file)))
 
     @GeneralUtilities.check_arguments
     def replace_version_in_ini_file(self, file: str, new_version_value: str):
-        GeneralUtilities.write_text_to_file(file, re.sub("version = \\d+\\.\\d+\\.\\d+", f"version = {new_version_value}",
-                                                         GeneralUtilities.read_text_from_file(file)))
+        GeneralUtilities.write_text_to_file(file, re.sub("version = \\d+\\.\\d+\\.\\d+", f"version = {new_version_value}",                                                         GeneralUtilities.read_text_from_file(file)))
 
     @GeneralUtilities.check_arguments
     def replace_version_in_nuspec_file(self, nuspec_file: str, new_version: str) -> None:
         # TODO use XSLT instead
         versionregex = "\\d+\\.\\d+\\.\\d+"
         versiononlyregex = f"^{versionregex}$"
         pattern = re.compile(versiononlyregex)
         if pattern.match(new_version):
-            GeneralUtilities.write_text_to_file(nuspec_file, re.sub(f"<version>{versionregex}<\\/version>",
-                                                                    f"<version>{new_version}</version>", GeneralUtilities.read_text_from_file(nuspec_file)))
+            GeneralUtilities.write_text_to_file(nuspec_file, re.sub(f"<version>{versionregex}<\\/version>",                                                                    f"<version>{new_version}</version>", GeneralUtilities.read_text_from_file(nuspec_file)))
         else:
             raise ValueError(f"Version '{new_version}' does not match version-regex '{versiononlyregex}'")
 
     @GeneralUtilities.check_arguments
     def replace_version_in_csproj_file(self, csproj_file: str, current_version: str):
         versionregex = "\\d+\\.\\d+\\.\\d+"
         versiononlyregex = f"^{versionregex}$"
         pattern = re.compile(versiononlyregex)
         if pattern.match(current_version):
             for tag in ["Version", "AssemblyVersion", "FileVersion"]:
-                GeneralUtilities.write_text_to_file(csproj_file, re.sub(f"<{tag}>{versionregex}(.\\d+)?<\\/{tag}>",
-                                                                        f"<{tag}>{current_version}</{tag}>", GeneralUtilities.read_text_from_file(csproj_file)))
+                GeneralUtilities.write_text_to_file(csproj_file, re.sub(f"<{tag}>{versionregex}(.\\d+)?<\\/{tag}>",                                                                        f"<{tag}>{current_version}</{tag}>", GeneralUtilities.read_text_from_file(csproj_file)))
         else:
             raise ValueError(f"Version '{current_version}' does not match version-regex '{versiononlyregex}'")
 
     @GeneralUtilities.check_arguments
     def push_nuget_build_artifact(self, nupkg_file: str, registry_address: str, api_key: str, verbosity: int = 1):
         nupkg_file_name = os.path.basename(nupkg_file)
         nupkg_file_folder = os.path.dirname(nupkg_file)
-        self.run_program("dotnet", f"nuget push {nupkg_file_name} --force-english-output --source {registry_address} --api-key {api_key}",
-                         nupkg_file_folder, verbosity)
+        self.run_program("dotnet", f"nuget push {nupkg_file_name} --force-english-output --source {registry_address} --api-key {api_key}",                         nupkg_file_folder, verbosity)
 
     @GeneralUtilities.check_arguments
     def dotnet_build(self, repository_folder: str, projectname: str, configuration: str):
         self.run_program("dotnet", f"clean -c {configuration}", repository_folder)
         self.run_program("dotnet", f"build {projectname}/{projectname}.csproj -c {configuration}", repository_folder)
 
     @GeneralUtilities.check_arguments
-    def dotnet_sign(self, dll_or_exe_file: str, snk_file: str, verbosity: int) -> None:
-        dll_or_exe_file = GeneralUtilities.resolve_relative_path_from_current_working_directory(dll_or_exe_file)
-        snk_file = GeneralUtilities.resolve_relative_path_from_current_working_directory(snk_file)
-        directory = os.path.dirname(dll_or_exe_file)
-        filename = os.path.basename(dll_or_exe_file)
-        if filename.lower().endswith(".dll"):
-            filename = filename[:-4]
-            extension = "dll"
-        elif filename.lower().endswith(".exe"):
-            filename = filename[:-4]
-            extension = "exe"
-        else:
-            raise ValueError("Only .dll-files and .exe-files can be signed")
-        self.run_program("ildasm",
-                         f"/all /typelist /text /out={filename}.il {filename}.{extension}",
-                         directory, verbosity)
-        self.run_program("ilasm",
-                         f"/{extension} /res:{filename}.res /optimize /key={snk_file} {filename}.il",
-                         directory, verbosity)
-        os.remove(directory+os.path.sep+filename + ".il")
-        os.remove(directory+os.path.sep+filename + ".res")
-
-    @GeneralUtilities.check_arguments
     def find_file_by_extension(self, folder: str, extension: str):
         result = [file for file in GeneralUtilities.get_direct_files_of_folder(folder) if file.endswith(f".{extension}")]
         result_length = len(result)
         if result_length == 0:
             raise FileNotFoundError(f"No file available in folder '{folder}' with extension '{extension}'.")
         if result_length == 1:
             return result[0]
         else:
             raise ValueError(f"Multiple values available in folder '{folder}' with extension '{extension}'.")
 
     @GeneralUtilities.check_arguments
-    def dotnet_sign_file(self, file: str, keyfile: str, verbosity: int):
-        directory = os.path.dirname(file)
-        filename = os.path.basename(file)
-        if filename.lower().endswith(".dll"):
-            filename = filename[:-4]
-            extension = "dll"
-        elif filename.lower().endswith(".exe"):
-            filename = filename[:-4]
-            extension = "exe"
-        else:
-            raise ValueError("Only .dll-files and .exe-files can be signed")
-        self.run_program("ildasm", f'/all /typelist /text /out={filename}.il {filename}.{extension}', directory, verbosity=verbosity)
-        self.run_program("ilasm", f'/{extension} /res:{filename}.res /optimize /key={keyfile} {filename}.il', directory, verbosity=verbosity)
-        os.remove(directory+os.path.sep+filename+".il")
-        os.remove(directory+os.path.sep+filename+".res")
-
-    @GeneralUtilities.check_arguments
     def commit_is_signed_by_key(self, repository_folder: str, revision_identifier: str, key: str) -> bool:
         result = self.run_program("git", f"verify-commit {revision_identifier}", repository_folder, throw_exception_if_exitcode_is_not_zero=False)
         if (result[0] != 0):
             return False
         if (not GeneralUtilities.contains_line(result[1].splitlines(), f"gpg\\:\\ using\\ [A-Za-z0-9]+\\ key\\ [A-Za-z0-9]+{key}")):
             # TODO check whether this works on machines where gpg is installed in another langauge than english
             return False
         if (not GeneralUtilities.contains_line(result[1].splitlines(), "gpg\\:\\ Good\\ signature\\ from")):
             # TODO check whether this works on machines where gpg is installed in another langauge than english
             return False
         return True
 
     @GeneralUtilities.check_arguments
     def get_parent_commit_ids_of_commit(self, repository_folder: str, commit_id: str) -> str:
-        return self.run_program("git", f'log --pretty=%P -n 1 "{commit_id}"',
-                                       repository_folder, throw_exception_if_exitcode_is_not_zero=True)[1].replace("\r", "").replace("\n", "").split(" ")
+        return self.run_program("git", f'log --pretty=%P -n 1 "{commit_id}"',                                       repository_folder, throw_exception_if_exitcode_is_not_zero=True)[1].replace("\r", "").replace("\n", "").split(" ")
 
     @GeneralUtilities.check_arguments
     def get_all_authors_and_committers_of_repository(self, repository_folder: str, subfolder: str = None, verbosity: int = 1) -> list[tuple[str, str]]:
         space_character = "_"
         if subfolder is None:
             subfolder_argument = ""
         else:
             subfolder_argument = f" -- {subfolder}"
-        log_result = self.run_program("git", f'log --pretty=%aN{space_character}%aE%n%cN{space_character}%cE HEAD{subfolder_argument}',
-                                      repository_folder, verbosity=0)
+        log_result = self.run_program("git", f'log --pretty=%aN{space_character}%aE%n%cN{space_character}%cE HEAD{subfolder_argument}',                                      repository_folder, verbosity=0)
         plain_content: list[str] = list(set([line for line in log_result[1].split("\n") if len(line) > 0]))
         result: list[tuple[str, str]] = []
         for item in plain_content:
             if len(re.findall(space_character, item)) == 1:
                 splitted = item.split(space_character)
                 result.append((splitted[0], splitted[1]))
             else:
                 raise ValueError(f'Unexpected author: "{item}"')
         return result
 
     @GeneralUtilities.check_arguments
     def get_commit_ids_between_dates(self, repository_folder: str, since: datetime, until: datetime, ignore_commits_which_are_not_in_history_of_head: bool = True) -> None:
         since_as_string = self.__datetime_to_string_for_git(since)
         until_as_string = self.__datetime_to_string_for_git(until)
-        result = filter(lambda line: not GeneralUtilities.string_is_none_or_whitespace(line),
-                        self.run_program("git", f'log --since "{since_as_string}" --until "{until_as_string}" --pretty=format:"%H" --no-patch',
-                                         repository_folder, throw_exception_if_exitcode_is_not_zero=True)[1].split("\n").replace("\r", ""))
+        result = filter(lambda line: not GeneralUtilities.string_is_none_or_whitespace(line),                        self.run_program("git", f'log --since "{since_as_string}" --until "{until_as_string}" --pretty=format:"%H" --no-patch',                                         repository_folder, throw_exception_if_exitcode_is_not_zero=True)[1].split("\n").replace("\r", ""))
         if ignore_commits_which_are_not_in_history_of_head:
             result = [commit_id for commit_id in result if self.git_commit_is_ancestor(repository_folder, commit_id)]
         return result
 
     @GeneralUtilities.check_arguments
     def __datetime_to_string_for_git(self, datetime_object: datetime) -> str:
         return datetime_object.strftime('%Y-%m-%d %H:%M:%S')
 
     @GeneralUtilities.check_arguments
     def git_commit_is_ancestor(self, repository_folder: str,  ancestor: str, descendant: str = "HEAD") -> bool:
-        exit_code = self.run_program_argsasarray("git", ["merge-base", "--is-ancestor", ancestor, descendant],
-                                                 repository_folder, throw_exception_if_exitcode_is_not_zero=False)[0]
+        exit_code = self.run_program_argsasarray("git", ["merge-base", "--is-ancestor", ancestor, descendant], repository_folder, throw_exception_if_exitcode_is_not_zero=False)[0]
         if exit_code == 0:
             return True
         elif exit_code == 1:
             return False
         else:
             raise ValueError(f"Can not calculate if {ancestor} is an ancestor of {descendant} in repository {repository_folder}.")
 
     @GeneralUtilities.check_arguments
     def __git_changes_helper(self, repository_folder: str, arguments_as_array: list[str]) -> bool:
-        lines = GeneralUtilities.string_to_lines(self.run_program_argsasarray("git", arguments_as_array, repository_folder,
-                                                 throw_exception_if_exitcode_is_not_zero=True, verbosity=0)[1], False)
+        lines = GeneralUtilities.string_to_lines(self.run_program_argsasarray("git", arguments_as_array, repository_folder,                                                 throw_exception_if_exitcode_is_not_zero=True, verbosity=0)[1], False)
         for line in lines:
             if GeneralUtilities.string_has_content(line):
                 return True
         return False
 
     @GeneralUtilities.check_arguments
     def git_repository_has_new_untracked_files(self, repositoryFolder: str):
@@ -271,22 +219,20 @@
             return True
         if (self.git_repository_has_new_untracked_files(repository_folder)):
             return True
         return False
 
     @GeneralUtilities.check_arguments
     def git_get_commit_id(self, repository_folder: str, commit: str = "HEAD") -> str:
-        result: tuple[int, str, str, int] = self.run_program_argsasarray("git", ["rev-parse", "--verify", commit],
-                                                                         repository_folder, throw_exception_if_exitcode_is_not_zero=True, verbosity=0)
+        result: tuple[int, str, str, int] = self.run_program_argsasarray("git", ["rev-parse", "--verify", commit], repository_folder, throw_exception_if_exitcode_is_not_zero=True, verbosity=0)
         return result[1].replace('\n', '')
 
     @GeneralUtilities.check_arguments
     def git_get_commit_date(self, repository_folder: str, commit: str = "HEAD") -> datetime:
-        result: tuple[int, str, str, int] = self.run_program_argsasarray("git", ["show", "-s", "--format=%ci", commit],
-                                                                         repository_folder, throw_exception_if_exitcode_is_not_zero=True, verbosity=0)
+        result: tuple[int, str, str, int] = self.run_program_argsasarray("git", ["show", "-s", "--format=%ci", commit], repository_folder, throw_exception_if_exitcode_is_not_zero=True, verbosity=0)
         date_as_string = result[1].replace('\n', '')
         result = datetime.strptime(date_as_string, '%Y-%m-%d %H:%M:%S %z')
         return result
 
     @GeneralUtilities.check_arguments
     def git_fetch(self, folder: str, remotename: str = "--all") -> None:
         self.run_program_argsasarray("git", ["fetch", remotename, "--tags", "--prune"], folder, throw_exception_if_exitcode_is_not_zero=True, verbosity=0)
@@ -302,16 +248,15 @@
     @GeneralUtilities.check_arguments
     def git_push(self, folder: str, remotename: str, localbranchname: str, remotebranchname: str, forcepush: bool = False, pushalltags: bool = True, verbosity: int = 0) -> None:
         argument = ["push", "--recurse-submodules=on-demand", remotename, f"{localbranchname}:{remotebranchname}"]
         if (forcepush):
             argument.append("--force")
         if (pushalltags):
             argument.append("--tags")
-        result: tuple[int, str, str, int] = self.run_program_argsasarray("git", argument, folder, throw_exception_if_exitcode_is_not_zero=True,
-                                                                         verbosity=verbosity, print_errors_as_information=True)
+        result: tuple[int, str, str, int] = self.run_program_argsasarray("git", argument, folder, throw_exception_if_exitcode_is_not_zero=True,                                                                         verbosity=verbosity, print_errors_as_information=True)
         return result[1].replace('\r', '').replace('\n', '')
 
     @GeneralUtilities.check_arguments
     def git_clone(self, clone_target_folder: str, remote_repository_path: str, include_submodules: bool = True, mirror: bool = False) -> None:
         if (os.path.isdir(clone_target_folder)):
             pass  # TODO throw error
         else:
@@ -320,19 +265,25 @@
                 args.append("--recurse-submodules")
                 args.append("--remote-submodules")
             if mirror:
                 args.append("--mirror")
             self.run_program_argsasarray("git", args, os.getcwd(), throw_exception_if_exitcode_is_not_zero=True, verbosity=0)
 
     @GeneralUtilities.check_arguments
-    def git_get_all_remote_names(self, directory) -> list[str]:
+    def git_get_all_remote_names(self, directory: str) -> list[str]:
         result = GeneralUtilities.string_to_lines(self.run_program_argsasarray("git", ["remote"], directory, throw_exception_if_exitcode_is_not_zero=True, verbosity=0)[1], False)
         return result
 
     @GeneralUtilities.check_arguments
+    def git_get_remote_url(self, directory: str, remote_name: str) -> str:
+        result = GeneralUtilities.string_to_lines(self.run_program_argsasarray(
+            "git", ["remote", "get-url", remote_name], directory, throw_exception_if_exitcode_is_not_zero=True, verbosity=0)[1], False)
+        return result[0].replace('\n', '')
+
+    @GeneralUtilities.check_arguments
     def repository_has_remote_with_specific_name(self, directory: str, remote_name: str) -> bool:
         return remote_name in self.git_get_all_remote_names(directory)
 
     @GeneralUtilities.check_arguments
     def git_add_or_set_remote_address(self, directory: str, remote_name: str, remote_address: str) -> None:
         if (self.repository_has_remote_with_specific_name(directory, remote_name)):
             self.run_program_argsasarray("git", ['remote', 'set-url', 'remote_name', remote_address], directory, throw_exception_if_exitcode_is_not_zero=True, verbosity=0)
@@ -370,15 +321,15 @@
     def git_commit(self, directory: str, message: str, author_name: str = None, author_email: str = None, stage_all_changes: bool = True,
                    no_changes_behavior: int = 0) -> str:
         # no_changes_behavior=0 => No commit
         # no_changes_behavior=1 => Commit anyway
         # no_changes_behavior=2 => Exception
         author_name = GeneralUtilities.str_none_safe(author_name).strip()
         author_email = GeneralUtilities.str_none_safe(author_email).strip()
-        argument = ['commit', '--quiet', '--message', message]
+        argument = ['commit', '--quiet', '--allow-empty', '--message', message]
         if (GeneralUtilities.string_has_content(author_name)):
             argument.append(f'--author="{author_name} <{author_email}>"')
         git_repository_has_uncommitted_changes = self.git_repository_has_uncommitted_changes(directory)
 
         if git_repository_has_uncommitted_changes:
             do_commit = True
             if stage_all_changes:
@@ -386,15 +337,14 @@
         else:
             if no_changes_behavior == 0:
                 GeneralUtilities.write_message_to_stdout(f"Commit '{message}' will not be done because there are no changes to commit in repository '{directory}'")
                 do_commit = False
             if no_changes_behavior == 1:
                 GeneralUtilities.write_message_to_stdout(f"There are no changes to commit in repository '{directory}'. Commit '{message}' will be done anyway.")
                 do_commit = True
-                argument.append('--allow-empty')
             if no_changes_behavior == 2:
                 raise RuntimeError(f"There are no changes to commit in repository '{directory}'. Commit '{message}' will not be done.")
 
         if do_commit:
             GeneralUtilities.write_message_to_stdout(f"Commit changes in '{directory}'")
             self.run_program_argsasarray("git", argument, directory, throw_exception_if_exitcode_is_not_zero=True, verbosity=0)
 
@@ -453,14 +403,21 @@
                 if os.path.isdir(target_directory):
                     # fetch
                     self.git_fetch(target_directory)
                 else:
                     # clone
                     self.git_clone(target_repository, source_repository, include_submodules=True, mirror=True)
 
+    def get_git_submodules(self, folder: str) -> list[str]:
+        e = self.run_program("git", "submodule status", folder)
+        result = []
+        for submodule_line in GeneralUtilities.string_to_lines(e[1], False, True):
+            result.append(submodule_line.split(' ')[1])
+        return result
+
     @GeneralUtilities.check_arguments
     def is_git_repository(self, folder: str) -> bool:
         combined = os.path.join(folder, ".git")
         # TODO consider check for bare-repositories
         return os.path.isdir(combined) or os.path.isfile(combined)
 
     @GeneralUtilities.check_arguments
@@ -469,15 +426,15 @@
         if (exit_code == 0):
             return True
         if (exit_code == 1):
             return False
         raise ValueError(f"Unable to calculate whether '{file_in_repository}' in repository '{repositorybasefolder}' is ignored due to git-exitcode {exit_code}.")
 
     @GeneralUtilities.check_arguments
-    def discard_all_changes(self, repository: str) -> None:
+    def git_discard_all_changes(self, repository: str) -> None:
         self.run_program_argsasarray("git", ["reset", "HEAD", "."], repository, throw_exception_if_exitcode_is_not_zero=True, verbosity=0)
         self.run_program_argsasarray("git", ["checkout", "."], repository, throw_exception_if_exitcode_is_not_zero=True, verbosity=0)
 
     @GeneralUtilities.check_arguments
     def git_get_current_branch_name(self, repository: str) -> str:
         result = self.run_program_argsasarray("git", ["rev-parse", "--abbrev-ref", "HEAD"], repository, throw_exception_if_exitcode_is_not_zero=True, verbosity=0)
         return result[1].replace("\r", "").replace("\n", "")
@@ -486,51 +443,59 @@
     def git_get_commitid_of_tag(self, repository: str, tag: str) -> str:
         stdout = self.run_program_argsasarray("git", ["rev-list", "-n", "1", tag], repository, verbosity=0)
         result = stdout[1].replace("\r", "").replace("\n", "")
         return result
 
     @GeneralUtilities.check_arguments
     def git_get_tags(self, repository: str) -> list[str]:
-        tags = [line for line in self.run_program_argsasarray("git", ["tag"], repository)[1].split("\n") if len(line) > 0]
+        tags = [line.replace("\r", "") for line in self.run_program_argsasarray("git", ["tag"], repository)[1].split("\n") if len(line) > 0]
         return tags
 
     @GeneralUtilities.check_arguments
-    def git_move_tags_to_another_branch(self, repository: str, tag_source_branch: str, tag_target_branch: str,
-                                        sign: bool = False, message: str = None) -> None:
+    def git_move_tags_to_another_branch(self, repository: str, tag_source_branch: str, tag_target_branch: str,                                        sign: bool = False, message: str = None) -> None:
         tags = self.git_get_tags(repository)
         tags_count = len(tags)
         counter = 0
         for tag in tags:
             counter = counter+1
             GeneralUtilities.write_message_to_stdout(f"Process tag {counter}/{tags_count}.")
             if self.git_commit_is_ancestor(repository, tag, tag_source_branch):  # tag is on source-branch
                 commit_id_old = self.git_get_commitid_of_tag(repository, tag)
                 commit_date: datetime = self.git_get_commit_date(repository, commit_id_old)
                 date_as_string = self.__datetime_to_string_for_git(commit_date)
-                search_commit_result = self.run_program_argsasarray("git", ["log", f'--after="{date_as_string}"', f'--before="{date_as_string}"',
-                                                                            "--pretty=format:%H", tag_target_branch], repository,
-                                                                    throw_exception_if_exitcode_is_not_zero=False)
+                search_commit_result = self.run_program_argsasarray("git", ["log", f'--after="{date_as_string}"', f'--before="{date_as_string}"',                                                                            "--pretty=format:%H", tag_target_branch], repository,                                                                    throw_exception_if_exitcode_is_not_zero=False)
                 if search_commit_result[0] != 0 or not GeneralUtilities.string_has_nonwhitespace_content(search_commit_result[1]):
                     raise ValueError(f"Can not calculate corresponding commit for tag '{tag}'.")
                 commit_id_new = search_commit_result[1]
                 self.git_delete_tag(repository, tag)
                 self.git_create_tag(repository, commit_id_new, tag, sign, message)
 
     @GeneralUtilities.check_arguments
-    def get_current_branch_has_tag(self, repository_folder: str) -> str:
+    def get_current_git_branch_has_tag(self, repository_folder: str) -> bool:
         result = self.run_program_argsasarray("git", ["describe", "--tags", "--abbrev=0"], repository_folder, verbosity=0, throw_exception_if_exitcode_is_not_zero=False)
         return result[0] == 0
 
     @GeneralUtilities.check_arguments
-    def get_latest_tag(self, repository_folder: str) -> str:
+    def get_latest_git_tag(self, repository_folder: str) -> str:
         result = self.run_program_argsasarray("git", ["describe", "--tags", "--abbrev=0"], repository_folder, verbosity=0)
         result = result[1].replace("\r", "").replace("\n", "")
         return result
 
     @GeneralUtilities.check_arguments
+    def get_staged_or_committed_git_ignored_files(self, repository_folder: str) -> list[str]:
+        tresult = self.run_program_argsasarray("git", ["ls-files", "-i", "-c", "--exclude-standard"], repository_folder, verbosity=0)
+        tresult = tresult[1].replace("\r", "")
+        result=[line for line in tresult.split("\n") if len(line)>0]
+        return result
+
+    @GeneralUtilities.check_arguments
+    def git_repository_has_commits(self,repository_folder: str) -> bool:
+        return self.run_program_argsasarray("git",["rev-parse","--verify","HEAD"],repository_folder,throw_exception_if_exitcode_is_not_zero=False)[0]==0
+
+    @GeneralUtilities.check_arguments
     def export_filemetadata(self, folder: str, target_file: str, encoding: str = "utf-8", filter_function=None) -> None:
         folder = GeneralUtilities.resolve_relative_path_from_current_working_directory(folder)
         lines = list()
         path_prefix = len(folder)+1
         items = dict()
         for item in GeneralUtilities.get_all_folders_of_folder(folder):
             items[item] = "d"
@@ -681,19 +646,23 @@
         for file in files:
             pdfFileMerger.append(file.strip())
         pdfFileMerger.write(outputfile)
         pdfFileMerger.close()
 
     @GeneralUtilities.check_arguments
     def pdf_to_image(self, file: str, outputfilename_without_extension: str) -> None:
-        doc = fitz.open(file)
-        for i, page in enumerate(doc):
-            pix = page.get_pixmap()
-            img = Image.frombytes("RGB", [pix.width, pix.height], pix.samples)
-            img.save(f"{outputfilename_without_extension}_{i}.png", "PNG")
+        raise ValueError("Function currently not available")
+        # PyMuPDF can be used for that but sometimes it throws
+        # "ImportError: DLL load failed while importing _fitz: Das angegebene Modul wurde nicht gefunden."
+
+        # doc = None  # fitz.open(file)
+        # for i, page in enumerate(doc):
+        #     pix = page.get_pixmap()
+        #     img = Image.frombytes("RGB", [pix.width, pix.height], pix.samples)
+        #     img.save(f"{outputfilename_without_extension}_{i}.png", "PNG")
 
     @GeneralUtilities.check_arguments
     def show_missing_files(self, folderA: str, folderB: str):
         for file in GeneralUtilities.get_missing_files(folderA, folderB):
             GeneralUtilities.write_message_to_stdout(file)
 
     @GeneralUtilities.check_arguments
@@ -739,16 +708,15 @@
         self.git_push(repository, remotename, targetbranch, targetbranch, False, True)
         if (GeneralUtilities.string_has_nonwhitespace_content(remotename)):
             self.git_push(repository, remotename, sourcebranch, sourcebranch, False, True)
         if (remove_source_branch):
             self.git_remove_branch(repository, sourcebranch)
 
     @GeneralUtilities.check_arguments
-    def sc_organize_lines_in_file(self, file: str, encoding: str, sort: bool = False, remove_duplicated_lines: bool = False, ignore_first_line: bool = False,
-                                  remove_empty_lines: bool = True, ignored_start_character: list = list()) -> int:
+    def sc_organize_lines_in_file(self, file: str, encoding: str, sort: bool = False, remove_duplicated_lines: bool = False, ignore_first_line: bool = False,                                  remove_empty_lines: bool = True, ignored_start_character: list = list()) -> int:
         if os.path.isfile(file):
 
             # read file
             lines = GeneralUtilities.read_lines_from_file(file, encoding)
             if (len(lines) == 0):
                 return 0
 
@@ -959,15 +927,15 @@
         iso.close()
 
     @GeneralUtilities.check_arguments
     def SCCreateISOFileWithObfuscatedFiles(self, inputfolder: str, outputfile: str, printtableheadline, createisofile, extensions) -> None:
         if (os.path.isdir(inputfolder)):
             namemappingfile = "name_map.csv"
             files_directory = inputfolder
-            files_directory_obf = files_directory + "_Obfuscated"
+            files_directory_obf = f"{files_directory}_Obfuscated"
             self.SCObfuscateFilesFolder(inputfolder, printtableheadline, namemappingfile, extensions)
             os.rename(namemappingfile, os.path.join(files_directory_obf, namemappingfile))
             if createisofile:
                 self.__create_iso(files_directory_obf, outputfile)
                 shutil.rmtree(files_directory_obf)
         else:
             raise ValueError(f"Directory not found: '{inputfolder}'")
@@ -1179,17 +1147,15 @@
         args.append(owner)
         args.append(file_or_folder)
         self.run_program_argsasarray("chown", args)
 
     # <run programs>
 
     @GeneralUtilities.check_arguments
-    def __run_program_argsasarray_async_helper(self, program: str, arguments_as_array: list[str] = [], working_directory: str = None, verbosity: int = 1,
-                                               print_errors_as_information: bool = False, log_file: str = None, timeoutInSeconds: int = 600, addLogOverhead: bool = False,
-                                               title: str = None, log_namespace: str = "", arguments_for_log:  list[str] = None, custom_argument: object = None) -> Popen:
+    def __run_program_argsasarray_async_helper(self, program: str, arguments_as_array: list[str] = [], working_directory: str = None, verbosity: int = 1, print_errors_as_information: bool = False, log_file: str = None, timeoutInSeconds: int = 600, addLogOverhead: bool = False, title: str = None, log_namespace: str = "", arguments_for_log:  list[str] = None, custom_argument: object = None) -> Popen:
         # Verbosity:
         # 0=Quiet (No output will be printed.)
         # 1=Normal (If the exitcode of the executed program is not 0 then the StdErr will be printed.)
         # 2=Full (Prints StdOut and StdErr of the executed program.)
         # 3=Verbose (Same as "Full" but with some more information.)
 
         if arguments_for_log is None:
@@ -1211,127 +1177,102 @@
             custom_argument = CustomEpewArgument(print_errors_as_information, log_file, timeoutInSeconds, addLogOverhead, title, log_namespace, verbosity, arguments_for_log)
         popen: Popen = self.program_runner.run_program_argsasarray_async_helper(program, arguments_as_array, working_directory, custom_argument)
         return popen
 
     # Return-values program_runner: Exitcode, StdOut, StdErr, Pid
 
     @GeneralUtilities.check_arguments
-    def run_program_argsasarray(self, program: str, arguments_as_array: list[str] = [], working_directory: str = None, verbosity: int = 1,
-                                print_errors_as_information: bool = False, log_file: str = None, timeoutInSeconds: int = 600, addLogOverhead: bool = False,
-                                title: str = None, log_namespace: str = "", arguments_for_log:  list[str] = None,
-                                throw_exception_if_exitcode_is_not_zero: bool = True, custom_argument: object = None) -> tuple[int, str, str, int]:
-        mock_loader_result = self.__try_load_mock(program, ' '.join(arguments_as_array), working_directory)
-        if mock_loader_result[0]:
-            return mock_loader_result[1]
-
-        if arguments_for_log is None:
-            arguments_for_log = arguments_as_array
-
-        arguments_for_log_as_string = ' '.join(arguments_for_log)
-        cmd = f'{working_directory}>{program} {arguments_for_log_as_string}'
-        if GeneralUtilities.string_is_none_or_whitespace(title):
-            info_for_log = cmd
-        else:
-            info_for_log = title
-
-        epew_will_be_used = isinstance(self.program_runner, ProgramRunnerEpew)
-        program_manages_output_itself = epew_will_be_used and False  # TODO fix stdout-/stderr-reading-block below
-        program_manages_logging_itself = epew_will_be_used
-
-        process = self.__run_program_argsasarray_async_helper(program, arguments_as_array, working_directory, verbosity, print_errors_as_information, log_file,
-                                                              timeoutInSeconds, addLogOverhead, title, log_namespace, arguments_for_log, custom_argument)
-        pid = process.pid
-
-        if program_manages_output_itself:
-            stdout_readable = process.stdout.readable()
-            stderr_readable = process.stderr.readable()
-            while stdout_readable or stderr_readable:
-
-                if stdout_readable:
-                    stdout_line = GeneralUtilities.bytes_to_string(process.stdout.readline()).strip()
-                    if (len(stdout_line)) > 0:
-                        GeneralUtilities.write_message_to_stdout(stdout_line)
-
-                if stderr_readable:
-                    stderr_line = GeneralUtilities.bytes_to_string(process.stderr.readline()).strip()
-                    if (len(stderr_line)) > 0:
-                        GeneralUtilities.write_message_to_stderr(stderr_line)
-
-                stdout_readable = process.stdout.readable()
-                stderr_readable = process.stderr.readable()
-
-        stdout, stderr = process.communicate()
-        exit_code = process.wait()
-        stdout = GeneralUtilities.bytes_to_string(stdout).replace('\r', '')
-        stderr = GeneralUtilities.bytes_to_string(stderr).replace('\r', '')
+    def run_program_argsasarray(self, program: str, arguments_as_array: list[str] = [], working_directory: str = None, verbosity: int = 1, print_errors_as_information: bool = False, log_file: str = None, timeoutInSeconds: int = 600, addLogOverhead: bool = False, title: str = None, log_namespace: str = "", arguments_for_log:  list[str] = None, throw_exception_if_exitcode_is_not_zero: bool = True, custom_argument: object = None) -> tuple[int, str, str, int]:
+        try:
+            mock_loader_result = self.__try_load_mock(program, ' '.join(arguments_as_array), working_directory)
+            if mock_loader_result[0]:
+                return mock_loader_result[1]
+
+            if arguments_for_log is None:
+                arguments_for_log = arguments_as_array
+
+            arguments_for_exception_as_string = ' '.join(arguments_for_log)
+
+            process: Popen = self.__run_program_argsasarray_async_helper(program, arguments_as_array, working_directory, verbosity, print_errors_as_information, log_file, timeoutInSeconds, addLogOverhead, title, log_namespace, arguments_for_log, custom_argument)
+            pid = process.pid
+
+            stdout_lines=list[str]()
+            stderr_lines=list[str]()
+
+            live_console_output_printing=1<verbosity
+
+            log_to_file=log_file is not None
+            if log_to_file:
+                GeneralUtilities.ensure_file_exists(log_file)
+            def stream_process(process):
+                try:
+
+                    go = process.poll() is None
+                    for line in process.stdout:
+                        line_str=GeneralUtilities.bytes_to_string(line).strip().replace('\r', '').replace('\n', '')
+                        stdout_lines.append(line_str)
+                        if live_console_output_printing:
+                            GeneralUtilities.write_message_to_stdout(line_str)
+                        if log_to_file:
+                            GeneralUtilities.append_line_to_file(log_file, line_str)
+                    for line in process.stderr:
+                        line_str=GeneralUtilities.bytes_to_string(line).strip().replace('\r', '').replace('\n', '')
+                        stderr_lines.append(line_str)
+                        if live_console_output_printing:
+                            if print_errors_as_information:
+                                GeneralUtilities.write_message_to_stdout(line_str)
+                            else:
+                                GeneralUtilities.write_message_to_stderr(line_str)
+                        if log_to_file:
+                            GeneralUtilities.append_line_to_file(log_file, line_str)
+                    return go
+                except Exception:
+                    return None
+            while stream_process(process):
+                time.sleep(0.1)
+
+            exit_code = process.poll()
+            stdout = '\n'.join(stdout_lines)
+            stderr = '\n'.join(stderr_lines)
 
-        if arguments_for_log_as_string is None:
-            arguments_for_log_as_string = ' '.join(arguments_as_array)
-        else:
-            arguments_for_log_as_string = ' '.join(arguments_for_log)
+            if arguments_for_exception_as_string is None:
+                arguments_for_exception_as_string = ' '.join(arguments_as_array)
+            else:
+                arguments_for_exception_as_string = ' '.join(arguments_for_log)
 
-        if GeneralUtilities.string_is_none_or_whitespace(title):
-            info_for_log = cmd
-        else:
-            info_for_log = title
 
-        if not program_manages_logging_itself and log_file is not None:
-            GeneralUtilities.ensure_file_exists(log_file)
-            GeneralUtilities.append_line_to_file(log_file, stdout)
-            GeneralUtilities.append_line_to_file(log_file, stderr)
-
-        if not program_manages_output_itself:
-            if verbosity == 1 and exit_code != 0:
-                self.__write_error_output(print_errors_as_information, stderr)
-            if verbosity == 2:
-                GeneralUtilities.write_message_to_stdout(stdout)
-                self.__write_error_output(print_errors_as_information, stderr)
-            if verbosity == 3:
-                GeneralUtilities.write_message_to_stdout(stdout)
-                self.__write_error_output(print_errors_as_information, stderr)
-                formatted = self.__format_program_execution_information(title=info_for_log, program=program,
-                                                                        argument=arguments_for_log_as_string, workingdirectory=working_directory)
-                GeneralUtilities.write_message_to_stdout(f"Finished '{info_for_log}'. Details: '{formatted}")
-
-        if throw_exception_if_exitcode_is_not_zero and exit_code != 0:
-            arguments_for_log_as_string = ' '.join(arguments_for_log)
-            raise ValueError(f"Program '{working_directory}>{program} {arguments_for_log_as_string}' resulted in exitcode {exit_code}. (StdOut: '{stdout}', StdErr: '{stderr}')")
+            if throw_exception_if_exitcode_is_not_zero and exit_code != 0:
+                arguments_for_exception_as_string = ' '.join(arguments_for_log)
+                raise ValueError(f"Program '{working_directory}>{program} {arguments_for_exception_as_string}' resulted in exitcode {exit_code}. (StdOut: '{stdout}', StdErr: '{stderr}')")
 
-        result = (exit_code, stdout, stderr, pid)
-        return result
+            result = (exit_code, stdout, stderr, pid)
+            return result
+        except Exception as e:
+            raise e
 
     # Return-values program_runner: Exitcode, StdOut, StdErr, Pid
     @GeneralUtilities.check_arguments
-    def run_program(self, program: str, arguments:  str = "", working_directory: str = None, verbosity: int = 1,
-                    print_errors_as_information: bool = False, log_file: str = None, timeoutInSeconds: int = 600, addLogOverhead: bool = False,
-                    title: str = None, log_namespace: str = "", arguments_for_log:  list[str] = None, throw_exception_if_exitcode_is_not_zero: bool = True,
-                    custom_argument: object = None) -> tuple[int, str, str, int]:
-        return self.run_program_argsasarray(program, GeneralUtilities.arguments_to_array(arguments), working_directory, verbosity, print_errors_as_information,
-                                            log_file, timeoutInSeconds, addLogOverhead, title, log_namespace, arguments_for_log, throw_exception_if_exitcode_is_not_zero, custom_argument)
+    def run_program(self, program: str, arguments:  str = "", working_directory: str = None, verbosity: int = 1, print_errors_as_information: bool = False, log_file: str = None, timeoutInSeconds: int = 600, addLogOverhead: bool = False, title: str = None, log_namespace: str = "", arguments_for_log:  list[str] = None, throw_exception_if_exitcode_is_not_zero: bool = True, custom_argument: object = None) -> tuple[int, str, str, int]:
+        return self.run_program_argsasarray(program, GeneralUtilities.arguments_to_array(arguments), working_directory, verbosity, print_errors_as_information, log_file, timeoutInSeconds, addLogOverhead, title, log_namespace, arguments_for_log, throw_exception_if_exitcode_is_not_zero, custom_argument)
 
     # Return-values program_runner: Pid
     @GeneralUtilities.check_arguments
-    def run_program_argsasarray_async(self, program: str, arguments_as_array: list[str] = [], working_directory: str = None, verbosity: int = 1,
-                                      print_errors_as_information: bool = False, log_file: str = None, timeoutInSeconds: int = 600, addLogOverhead: bool = False,
-                                      title: str = None, log_namespace: str = "", arguments_for_log:  list[str] = None, custom_argument: object = None) -> int:
+    def run_program_argsasarray_async(self, program: str, arguments_as_array: list[str] = [], working_directory: str = None, verbosity: int = 1, print_errors_as_information: bool = False, log_file: str = None, timeoutInSeconds: int = 600, addLogOverhead: bool = False, title: str = None, log_namespace: str = "", arguments_for_log:  list[str] = None, custom_argument: object = None) -> int:
         mock_loader_result = self.__try_load_mock(program, ' '.join(arguments_as_array), working_directory)
         if mock_loader_result[0]:
             return mock_loader_result[1]
 
-        process: Popen = self.__run_program_argsasarray_async_helper(program, arguments_as_array, working_directory, verbosity,
-                                                                     print_errors_as_information, log_file, timeoutInSeconds, addLogOverhead, title, log_namespace, arguments_for_log, custom_argument)
+        process: Popen = self.__run_program_argsasarray_async_helper(program, arguments_as_array, working_directory, verbosity, print_errors_as_information, log_file, timeoutInSeconds, addLogOverhead, title, log_namespace, arguments_for_log, custom_argument)
         return process.pid
 
     # Return-values program_runner: Pid
     @GeneralUtilities.check_arguments
     def run_program_async(self, program: str, arguments: str = "",  working_directory: str = None, verbosity: int = 1,
-                          print_errors_as_information: bool = False, log_file: str = None, timeoutInSeconds: int = 600, addLogOverhead: bool = False,
-                          title: str = None, log_namespace: str = "", arguments_for_log:  list[str] = None, custom_argument: object = None) -> int:
-        return self.run_program_argsasarray_async(program, GeneralUtilities.arguments_to_array(arguments), working_directory, verbosity,
-                                                  print_errors_as_information, log_file, timeoutInSeconds, addLogOverhead, title, log_namespace, arguments_for_log, custom_argument)
+                          print_errors_as_information: bool = False, log_file: str = None, timeoutInSeconds: int = 600, addLogOverhead: bool = False, title: str = None, log_namespace: str = "", arguments_for_log:  list[str] = None, custom_argument: object = None) -> int:
+        return self.run_program_argsasarray_async(program, GeneralUtilities.arguments_to_array(arguments), working_directory, verbosity, print_errors_as_information, log_file, timeoutInSeconds, addLogOverhead, title, log_namespace, arguments_for_log, custom_argument)
 
     @GeneralUtilities.check_arguments
     def __try_load_mock(self, program: str, arguments: str, working_directory: str) -> tuple[bool, tuple[int, str, str, int]]:
         if self.mock_program_calls:
             try:
                 return [True, self.__get_mock_program_call(program, arguments, working_directory)]
             except LookupError:
@@ -1343,37 +1284,14 @@
     def __adapt_workingdirectory(self, workingdirectory: str) -> str:
         if workingdirectory is None:
             return os.getcwd()
         else:
             return GeneralUtilities.resolve_relative_path_from_current_working_directory(workingdirectory)
 
     @GeneralUtilities.check_arguments
-    def __write_error_output(self, print_errors_as_information, stderr):
-        if print_errors_as_information:
-            GeneralUtilities.write_message_to_stdout(stderr)
-        else:
-            GeneralUtilities.write_message_to_stderr(stderr)
-
-    @GeneralUtilities.check_arguments
-    def __format_program_execution_information(self, exitcode: int = None,  stdout: str = None, stderr: str = None, program: str = None, argument: str = None,
-                                               workingdirectory: str = None, title: str = None, pid: int = None, execution_duration: timedelta = None):
-        result = ""
-        if (exitcode is not None and stdout is not None and stderr is not None):
-            result = f"{result} Exitcode: {exitcode}; StdOut: '{stdout}'; StdErr: '{stderr}'"
-        if (pid is not None):
-            result = f"Pid: '{pid}'; {result}"
-        if (program is not None and argument is not None and workingdirectory is not None):
-            result = f"Command: '{workingdirectory}> {program} {argument}'; {result}"
-        if (execution_duration is not None):
-            result = f"{result}; Duration: '{str(execution_duration)}'"
-        if (title is not None):
-            result = f"Title: '{title}'; {result}"
-        return result.strip()
-
-    @GeneralUtilities.check_arguments
     def verify_no_pending_mock_program_calls(self):
         if (len(self.__mocked_program_calls) > 0):
             raise AssertionError(
                 "The following mock-calls were not called:\n"+",\n    ".join([self.__format_mock_program_call(r) for r in self.__mocked_program_calls]))
 
     @GeneralUtilities.check_arguments
     def __format_mock_program_call(self, r) -> str:
@@ -1381,16 +1299,15 @@
         return f"'{r.workingdirectory}>{r.program} {r.argument}' (" \
             f"exitcode: {GeneralUtilities.str_none_safe(str(r.exit_code))}, " \
             f"pid: {GeneralUtilities.str_none_safe(str(r.pid))}, "\
             f"stdout: {GeneralUtilities.str_none_safe(str(r.stdout))}, " \
             f"stderr: {GeneralUtilities.str_none_safe(str(r.stderr))})"
 
     @GeneralUtilities.check_arguments
-    def register_mock_program_call(self, program: str, argument: str, workingdirectory: str, result_exit_code: int, result_stdout: str, result_stderr: str,
-                                   result_pid: int, amount_of_expected_calls=1):
+    def register_mock_program_call(self, program: str, argument: str, workingdirectory: str, result_exit_code: int, result_stdout: str, result_stderr: str,                                   result_pid: int, amount_of_expected_calls=1):
         "This function is for test-purposes only"
         for _ in itertools.repeat(None, amount_of_expected_calls):
             mock_call = ScriptCollectionCore.__MockProgramCall()
             mock_call.program = program
             mock_call.argument = argument
             mock_call.workingdirectory = workingdirectory
             mock_call.exit_code = result_exit_code
@@ -1477,60 +1394,59 @@
             minor = minor+1
         if increment_patch:
             patch = patch+1
         return f"{major}.{minor}.{patch}"
 
     @GeneralUtilities.check_arguments
     def get_semver_version_from_gitversion(self, repository_folder: str) -> str:
-        result = self.get_version_from_gitversion(repository_folder, "MajorMinorPatch")
-
-        try:
+        if(self.git_repository_has_commits(repository_folder)):
+            result = self.get_version_from_gitversion(repository_folder, "MajorMinorPatch")
             if self.git_repository_has_uncommitted_changes(repository_folder):
-                if self.get_current_branch_has_tag(repository_folder):
-                    id_of_latest_tag = self.git_get_commitid_of_tag(repository_folder, self.get_latest_tag(repository_folder))
+                if self.get_current_git_branch_has_tag(repository_folder):
+                    id_of_latest_tag = self.git_get_commitid_of_tag(repository_folder, self.get_latest_git_tag(repository_folder))
                     current_commit = self.git_get_commit_id(repository_folder)
                     current_commit_is_on_latest_tag = id_of_latest_tag == current_commit
                     if current_commit_is_on_latest_tag:
                         result = self.increment_version(result, False, False, True)
-        except:  # Exceptions are thrown for example when no tags are available. but these cases should be ignored.
-            pass
-
+        else:
+            result="0.1.0"
         return result
 
+    @staticmethod
+    @GeneralUtilities.check_arguments
+    def is_patch_version(version_string: str) -> bool:
+        return not version_string.endswith(".0")
+
     @GeneralUtilities.check_arguments
     def get_version_from_gitversion(self, folder: str, variable: str) -> str:
         # called twice as workaround for issue 1877 in gitversion ( https://github.com/GitTools/GitVersion/issues/1877 )
-        result = self.run_program_argsasarray("gitversion", ["/showVariable", variable], folder)
-        result = self.run_program_argsasarray("gitversion", ["/showVariable", variable], folder)
+        result = self.run_program_argsasarray("gitversion", ["/showVariable", variable], folder,verbosity=0)
+        result = self.run_program_argsasarray("gitversion", ["/showVariable", variable], folder,verbosity=0)
         result = GeneralUtilities.strip_new_line_character(result[1])
 
         return result
 
     @GeneralUtilities.check_arguments
     def generate_certificate_authority(self, folder: str, name: str, subj_c: str, subj_st: str, subj_l: str, subj_o: str, subj_ou: str,
                                        days_until_expire: int = None, password: str = None) -> None:
         if days_until_expire is None:
             days_until_expire = 1825
         if password is None:
             password = GeneralUtilities.generate_password()
-        self.run_program("openssl", f'req -new -newkey ec -pkeyopt ec_paramgen_curve:prime256v1 -days {days_until_expire} -nodes -x509 -subj ' +
-                         f'/C={subj_c}/ST={subj_st}/L={subj_l}/O={subj_o}/CN={name}/OU={subj_ou} -passout pass:{password} ' +
-                         f'-keyout {name}.key -out {name}.crt', folder)
+        self.run_program("openssl", f'req -new -newkey ec -pkeyopt ec_paramgen_curve:prime256v1 -days {days_until_expire} -nodes -x509 -subj /C={subj_c}/ST={subj_st}/L={subj_l}/O={subj_o}/CN={name}/OU={subj_ou} -passout pass:{password} -keyout {name}.key -out {name}.crt', folder)
 
     @GeneralUtilities.check_arguments
-    def generate_certificate(self, folder: str,  domain: str, filename: str, subj_c: str, subj_st: str, subj_l: str, subj_o: str, subj_ou: str,
-                             days_until_expire: int = None, password: str = None) -> None:
+    def generate_certificate(self, folder: str,  domain: str, filename: str, subj_c: str, subj_st: str, subj_l: str, subj_o: str, subj_ou: str,                             days_until_expire: int = None, password: str = None) -> None:
         if days_until_expire is None:
             days_until_expire = 397
         if password is None:
             password = GeneralUtilities.generate_password()
         rsa_key_length = 4096
         self.run_program("openssl", f'genrsa -out {filename}.key {rsa_key_length}', folder)
-        self.run_program("openssl", f'req -new -subj /C={subj_c}/ST={subj_st}/L={subj_l}/O={subj_o}/CN={domain}/OU={subj_ou} -x509 ' +
-                         f'-key {filename}.key -out {filename}.unsigned.crt -days {days_until_expire}', folder)
+        self.run_program("openssl", f'req -new -subj /C={subj_c}/ST={subj_st}/L={subj_l}/O={subj_o}/CN={domain}/OU={subj_ou} -x509 -key {filename}.key -out {filename}.unsigned.crt -days {days_until_expire}', folder)
         self.run_program("openssl", f'pkcs12 -export -out {filename}.selfsigned.pfx -password pass:{password} -inkey {filename}.key -in {filename}.unsigned.crt', folder)
         GeneralUtilities.write_text_to_file(os.path.join(folder, f"{filename}.password"), password)
         GeneralUtilities.write_text_to_file(os.path.join(folder, f"{filename}.san.conf"), f"""[ req ]
 default_bits        = {rsa_key_length}
 distinguished_name  = req_distinguished_name
 req_extensions      = v3_req
 default_md          = sha256
@@ -1550,26 +1466,24 @@
 
 [ subject_alt_name ]
 DNS                 = {domain}
 """)
 
     @GeneralUtilities.check_arguments
     def generate_certificate_sign_request(self, folder: str, domain: str, filename: str, subj_c: str, subj_st: str, subj_l: str, subj_o: str, subj_ou: str) -> None:
-        self.run_program("openssl", f'req -new -subj /C={subj_c}/ST={subj_st}/L={subj_l}/O={subj_o}/CN={domain}/OU={subj_ou} ' +
-                         f'-key {filename}.key -out {filename}.csr -config {filename}.san.conf', folder)
+        self.run_program("openssl", f'req -new -subj /C={subj_c}/ST={subj_st}/L={subj_l}/O={subj_o}/CN={domain}/OU={subj_ou} -key {filename}.key -out {filename}.csr -config {filename}.san.conf', folder)
 
     @GeneralUtilities.check_arguments
     def sign_certificate(self, folder: str, ca_folder: str, ca_name: str, domain: str, filename: str, days_until_expire: int = None) -> None:
         if days_until_expire is None:
             days_until_expire = 397
         ca = os.path.join(ca_folder, ca_name)
         password_file = os.path.join(folder, f"{filename}.password")
         password = GeneralUtilities.read_text_from_file(password_file)
-        self.run_program("openssl", f'x509 -req -in {filename}.csr -CA {ca}.crt -CAkey {ca}.key -CAcreateserial -CAserial {ca}.srl ' +
-                         f'-out {filename}.crt -days {days_until_expire} -sha256 -extensions v3_req -extfile {filename}.san.conf', folder)
+        self.run_program("openssl", f'x509 -req -in {filename}.csr -CA {ca}.crt -CAkey {ca}.key -CAcreateserial -CAserial {ca}.srl -out {filename}.crt -days {days_until_expire} -sha256 -extensions v3_req -extfile {filename}.san.conf', folder)
         self.run_program("openssl", f'pkcs12 -export -out {filename}.pfx -inkey {filename}.key -in {filename}.crt -password pass:{password}', folder)
 
     @GeneralUtilities.check_arguments
     def update_dependencies_of_python_in_requirementstxt_file(self, file: str, verbosity: int):
         lines = GeneralUtilities.read_lines_from_file(file)
         new_lines = []
         for line in lines:
@@ -1623,20 +1537,19 @@
             # Relevant output-lines are something like "    > NJsonSchema             10.7.0        10.7.0      10.9.0"
             if ">" in line:
                 package_name = line.replace(">", "").strip().split(" ")[0]
                 GeneralUtilities.write_message_to_stderr(f"Update package {package_name}")
                 self.run_program("dotnet", f"add {csproj_filename} package {package_name}", folder)
 
     @GeneralUtilities.check_arguments
-    def create_deb_package(self, codeunit_name: str, binary_folder: str, control_file_content: str,
+    def create_deb_package(self, toolname: str, binary_folder: str, control_file_content: str,
                            deb_output_folder: str, verbosity: int, permission_of_executable_file_as_octet_triple: int) -> None:
 
         # prepare
         GeneralUtilities.ensure_directory_exists(deb_output_folder)
-        toolname = codeunit_name
         temp_folder = os.path.join(tempfile.gettempdir(), str(uuid.uuid4()))
         GeneralUtilities.ensure_directory_exists(temp_folder)
         bin_folder = binary_folder
         tool_content_folder_name = toolname+"Content"
 
         # create folder
         GeneralUtilities.ensure_directory_exists(temp_folder)
@@ -1688,18 +1601,60 @@
         usr_bin_folder = os.path.join(packagecontent_data_folder, "usr/bin")
         GeneralUtilities.ensure_directory_exists(usr_bin_folder)
         usr_bin_content_folder = os.path.join(usr_bin_folder, tool_content_folder_name)
         GeneralUtilities.copy_content_of_folder(bin_folder, usr_bin_content_folder)
 
         # create debfile
         deb_filename = f"{toolname}.deb"
-        self.run_program_argsasarray("tar", ["czf", f"../{entireresult_content_folder_name}/control.tar.gz", "*"],
-                                     packagecontent_control_folder, verbosity=verbosity)
-        self.run_program_argsasarray("tar", ["czf", f"../{entireresult_content_folder_name}/data.tar.gz", "*"],
-                                     packagecontent_data_folder, verbosity=verbosity)
-        self.run_program_argsasarray("ar", ["r", deb_filename, "debian-binary", "control.tar.gz", "data.tar.gz"],
-                                     packagecontent_entireresult_folder, verbosity=verbosity)
+        self.run_program_argsasarray("tar", ["czf", f"../{entireresult_content_folder_name}/control.tar.gz", "*"], packagecontent_control_folder, verbosity=verbosity)
+        self.run_program_argsasarray("tar", ["czf", f"../{entireresult_content_folder_name}/data.tar.gz", "*"], packagecontent_data_folder, verbosity=verbosity)
+        self.run_program_argsasarray("ar", ["r", deb_filename, "debian-binary", "control.tar.gz", "data.tar.gz"], packagecontent_entireresult_folder, verbosity=verbosity)
         result_file = os.path.join(packagecontent_entireresult_folder, deb_filename)
         shutil.copy(result_file, os.path.join(deb_output_folder, deb_filename))
 
         # cleanup
         GeneralUtilities.ensure_directory_does_not_exist(temp_folder)
+
+
+    @GeneralUtilities.check_arguments
+    def update_year_in_copyright_tags(self, file: str) -> None:
+        current_year=str(datetime.now().year)
+        lines=GeneralUtilities.read_lines_from_file(file)
+        lines_result=[]
+        for line in lines:
+            if match := re.search("(.*<[Cc]opyright>.*)\\d\\d\\d\\d(.*<\\/[Cc]opyright>.*)", line):
+                part1 = match.group(1)
+                part2 = match.group(2)
+                adapted=part1+current_year+part2
+            else:
+                adapted=line
+            lines_result.append(adapted)
+        GeneralUtilities.write_lines_to_file(file,lines_result)
+
+    @GeneralUtilities.check_arguments
+    def update_year_in_first_line_of_file(self, file: str) -> None:
+        current_year=str(datetime.now().year)
+        lines=GeneralUtilities.read_lines_from_file(file)
+        lines[0]=re.sub("\\d\\d\\d\\d",current_year,lines[0])
+        GeneralUtilities.write_lines_to_file(file,lines)
+
+    @GeneralUtilities.check_arguments
+    def get_external_ip(self, proxy: str) -> str:
+        information=self.get_externalnetworkinformation_as_json_string(proxy)
+        parsed=json.loads(information)
+        return parsed.ip
+
+    @GeneralUtilities.check_arguments
+    def get_country_of_external_ip(self, proxy: str) -> str:
+        information=self.get_externalnetworkinformation_as_json_string(proxy)
+        parsed=json.loads(information)
+        return parsed.country
+
+    @GeneralUtilities.check_arguments
+    def get_externalnetworkinformation_as_json_string(self, proxy: str) -> str:
+        proxies = None
+        if GeneralUtilities.string_has_content(proxy):
+            proxies = {"http": proxy}
+        response = requests.get('https://ipinfo.io', proxies=proxies, timeout=5)
+        network_information_as_json_string=GeneralUtilities.bytes_to_string(response.content)
+        return network_information_as_json_string
+
```

## ScriptCollection/TasksForCommonProjectStructure.py

```diff
@@ -6,51 +6,53 @@
 import shutil
 import math
 import re
 import urllib.request
 import zipfile
 import json
 import configparser
+import tempfile
+import uuid
 import requests
 from packaging import version
 import xmlschema
 from OpenSSL import crypto
 from lxml import etree
 from .GeneralUtilities import GeneralUtilities
 from .ScriptCollectionCore import ScriptCollectionCore
 from .ProgramRunnerEpew import ProgramRunnerEpew
 
-
 class CreateReleaseConfiguration():
     projectname: str
     remotename: str
     artifacts_folder: str
     push_artifacts_scripts_folder: str
     verbosity: int
     reference_repository_remote_name: str = None
     reference_repository_branch_name: str = "main"
     build_repository_branch: str = "main"
     public_repository_url: str
     additional_arguments_file: str = None
-    artifacts_which_have_artifacts_to_push: list[str] = None
     repository_folder_name: str = None
+    __sc: ScriptCollectionCore = None
 
-    def __init__(self, projectname: str, remotename: str, build_artifacts_target_folder: str, push_artifacts_scripts_folder: str,
-                 verbosity: int, public_repository_url: str, additional_arguments_file: str, artifacts_which_have_artifacts_to_push: list[str],
-                 repository_folder_name: str):
+    def __init__(self, projectname: str, remotename: str, build_artifacts_target_folder: str, push_artifacts_scripts_folder: str, verbosity: int, repository_folder: str, additional_arguments_file: str, repository_folder_name: str):
 
+        self.__sc = ScriptCollectionCore()
         self.projectname = projectname
         self.remotename = remotename
         self.artifacts_folder = build_artifacts_target_folder
         self.push_artifacts_scripts_folder = push_artifacts_scripts_folder
         self.verbosity = verbosity
-        self.public_repository_url = public_repository_url
+        if self.remotename is None:
+            self.public_repository_url = None
+        else:
+            self.public_repository_url = self.__sc.git_get_remote_url(repository_folder, remotename)
         self.reference_repository_remote_name = self.remotename
         self.additional_arguments_file = additional_arguments_file
-        self.artifacts_which_have_artifacts_to_push = artifacts_which_have_artifacts_to_push
         self.repository_folder_name = repository_folder_name
 
 
 class CreateReleaseInformationForProjectInCommonProjectFormat:
     projectname: str
     repository: str
     artifacts_folder: str
@@ -59,31 +61,28 @@
     public_repository_url: str = None
     target_branch_name: str = None
     push_artifacts_scripts_folder: str = None
     target_environmenttype_for_qualitycheck: str = "QualityCheck"
     target_environmenttype_for_productive: str = "Productive"
     additional_arguments_file: str = None
     export_target: str = None
-    artifacts_which_have_artifacts_to_push: list[str] = None
 
-    def __init__(self, repository: str, artifacts_folder: str, projectname: str, public_repository_url: str, target_branch_name: str,
-                 additional_arguments_file: str, export_target: str, push_artifacts_scripts_folder: str, artifacts_which_have_artifacts_to_push: list[str]):
+    def __init__(self, repository: str, artifacts_folder: str, projectname: str, public_repository_url: str, target_branch_name: str, additional_arguments_file: str, export_target: str, push_artifacts_scripts_folder: str):
         self.repository = repository
         self.public_repository_url = public_repository_url
         self.target_branch_name = target_branch_name
         self.artifacts_folder = artifacts_folder
         self.additional_arguments_file = additional_arguments_file
         self.export_target = export_target
         self.push_artifacts_scripts_folder = push_artifacts_scripts_folder
         if projectname is None:
             projectname = os.path.basename(self.repository)
         else:
             self.projectname = projectname
         self.reference_repository = f"{repository}Reference"
-        self.artifacts_which_have_artifacts_to_push = artifacts_which_have_artifacts_to_push
 
 
 class MergeToStableBranchInformationForProjectInCommonProjectFormat:
     repository: str
     sourcebranch: str = "main"
     targetbranch: str = "stable"
     sign_git_tags: bool = True
@@ -137,97 +136,78 @@
 
     @GeneralUtilities.check_arguments
     def get_artifacts_folder(self, repository_folder: str, codeunit_name: str) -> str:
         return os.path.join(repository_folder, codeunit_name, "Other", "Artifacts")
 
     @GeneralUtilities.check_arguments
     def get_wheel_file(self, repository_folder: str, codeunit_name: str) -> str:
-        return self.__sc.find_file_by_extension(os.path.join(self.get_artifacts_folder(repository_folder, codeunit_name),
-                                                             "BuildResult_Wheel"), "whl")
+        return self.__sc.find_file_by_extension(os.path.join(self.get_artifacts_folder(repository_folder, codeunit_name), "BuildResult_Wheel"), "whl")
 
     @GeneralUtilities.check_arguments
-    def get_testcoverage_threshold_from_codeunit_file(self, codeunit_file):
+    def get_testcoverage_threshold_from_codeunit_file(self, codeunit_file: str):
         root: etree._ElementTree = etree.parse(codeunit_file)
-        return float(str(root.xpath('//cps:minimalcodecoverageinpercent/text()', namespaces={
-            'cps': 'https://projects.aniondev.de/PublicProjects/Common/ProjectTemplates/-/tree/main/Conventions/RepositoryStructure/CommonProjectStructure'
-        })[0]))
+        return float(str(root.xpath('//cps:properties/cps:testsettings/@minimalcodecoverageinpercent', namespaces={'cps': 'https://projects.aniondev.de/PublicProjects/Common/ProjectTemplates/-/tree/main/Conventions/RepositoryStructure/CommonProjectStructure'})[0]))
 
     @GeneralUtilities.check_arguments
-    def codeunit_has_testable_sourcecode(self, codeunit_file) -> bool:
+    def codeunit_has_testable_sourcecode(self, codeunit_file: str) -> bool:
         root: etree._ElementTree = etree.parse(codeunit_file)
-        return GeneralUtilities.string_to_boolean(str(root.xpath('//cps:properties/@codeunithastestablesourcecode', namespaces={
-            'cps': 'https://projects.aniondev.de/PublicProjects/Common/ProjectTemplates/-/tree/main/Conventions/RepositoryStructure/CommonProjectStructure'
-        })[0]))
+        return GeneralUtilities.string_to_boolean(str(root.xpath('//cps:properties/@codeunithastestablesourcecode', namespaces={'cps': 'https://projects.aniondev.de/PublicProjects/Common/ProjectTemplates/-/tree/main/Conventions/RepositoryStructure/CommonProjectStructure'})[0]))
 
     @GeneralUtilities.check_arguments
-    def codeunit_throws_exception_if_codeunitfile_is_not_validatable(self, codeunit_file) -> bool:
+    def codeunit_throws_exception_if_codeunitfile_is_not_validatable(self, codeunit_file: str) -> bool:
         root: etree._ElementTree = etree.parse(codeunit_file)
-        return GeneralUtilities.string_to_boolean(str(root.xpath('//cps:properties/@throwexceptionifcodeunitfilecannotbevalidated', namespaces={
-            'cps': 'https://projects.aniondev.de/PublicProjects/Common/ProjectTemplates/-/tree/main/Conventions/RepositoryStructure/CommonProjectStructure'
-        })[0]))
+        return GeneralUtilities.string_to_boolean(str(root.xpath('//cps:properties/@throwexceptionifcodeunitfilecannotbevalidated', namespaces={'cps': 'https://projects.aniondev.de/PublicProjects/Common/ProjectTemplates/-/tree/main/Conventions/RepositoryStructure/CommonProjectStructure'})[0]))
 
     @GeneralUtilities.check_arguments
-    def codeunit_has_updatable_dependencies(self, codeunit_file) -> bool:
+    def codeunit_has_updatable_dependencies(self, codeunit_file: str) -> bool:
         root: etree._ElementTree = etree.parse(codeunit_file)
-        return GeneralUtilities.string_to_boolean(str(root.xpath('//cps:properties/@codeunithasupdatabledependencies', namespaces={
-            'cps': 'https://projects.aniondev.de/PublicProjects/Common/ProjectTemplates/-/tree/main/Conventions/RepositoryStructure/CommonProjectStructure'
-        })[0]))
+        return GeneralUtilities.string_to_boolean(str(root.xpath('//cps:properties/@codeunithasupdatabledependencies', namespaces={'cps': 'https://projects.aniondev.de/PublicProjects/Common/ProjectTemplates/-/tree/main/Conventions/RepositoryStructure/CommonProjectStructure'})[0]))
+
+    @GeneralUtilities.check_arguments
+    def get_codeunit_description(self, codeunit_file: str) -> bool:
+        root: etree._ElementTree = etree.parse(codeunit_file)
+        return str(root.xpath('//cps:properties/@description', namespaces={'cps': 'https://projects.aniondev.de/PublicProjects/Common/ProjectTemplates/-/tree/main/Conventions/RepositoryStructure/CommonProjectStructure'})[0])
 
     @GeneralUtilities.check_arguments
-    def check_testcoverage(self, testcoverage_file_in_cobertura_format: str, repository_folder: str, codeunitname: str):
+    def check_testcoverage(self, testcoverage_file_in_cobertura_format: str, repository_folder: str, codeunitname: str) -> None:
         root: etree._ElementTree = etree.parse(testcoverage_file_in_cobertura_format)
-        # TODO check if there is at least one package in testcoverage_file_in_cobertura_format
-        coverage_in_percent = round(float(str(root.xpath('//coverage/@line-rate')[0]))*100, 2)
+        if len(root.xpath('//coverage/packages/package')) != 1:
+            raise ValueError(f"'{testcoverage_file_in_cobertura_format}' must contain exactly 1 package.")
+        if root.xpath('//coverage/packages/package[1]/@name')[0] != codeunitname:
+            raise ValueError(f"The package name of the tested package in '{testcoverage_file_in_cobertura_format}' must be '{codeunitname}'.")
+        coverage_in_percent = round(float(str(root.xpath('//coverage/packages/package[1]/@line-rate')[0]))*100, 2)
+        technicalminimalrequiredtestcoverageinpercent = 0
+        if not technicalminimalrequiredtestcoverageinpercent < coverage_in_percent:
+            raise ValueError(f"The test-coverage of package '{codeunitname}' must be greater than {technicalminimalrequiredtestcoverageinpercent}%.")
         codeunit_file = os.path.join(repository_folder, codeunitname, f"{codeunitname}.codeunit.xml")
         minimalrequiredtestcoverageinpercent = self.get_testcoverage_threshold_from_codeunit_file(codeunit_file)
-        minimalrecommendedcoverage = 80
-        if minimalrequiredtestcoverageinpercent < minimalrecommendedcoverage:
-            GeneralUtilities.write_message_to_stderr(f"Warning: The minimal required testcoverage is {minimalrequiredtestcoverageinpercent}% " +
-                                                     f"but should be at least {minimalrecommendedcoverage}%.")
-        # TODO check that testcoverage_file_in_cobertura_format contains at least one package with at least one line of code
         if (coverage_in_percent < minimalrequiredtestcoverageinpercent):
             raise ValueError(f"The testcoverage for codeunit {codeunitname} must be {minimalrequiredtestcoverageinpercent}% or more but is {coverage_in_percent}%.")
 
     @GeneralUtilities.check_arguments
-    def replace_version_in_python_file(self, file: str, new_version_value: str):
-        GeneralUtilities.write_text_to_file(file, re.sub("version = \"\\d+\\.\\d+\\.\\d+\"", f"version = \"{new_version_value}\"",
-                                                         GeneralUtilities.read_text_from_file(file)))
-
-    @staticmethod
-    @GeneralUtilities.check_arguments
-    def __adjust_source_in_testcoverage_file(testcoverage_file: str, codeunitname: str) -> None:
-        GeneralUtilities.write_text_to_file(testcoverage_file, re.sub("<source>.+<\\/source>", f"<source>{codeunitname}</source>",
-                                                                      GeneralUtilities.read_text_from_file(testcoverage_file)))
-
-    @staticmethod
-    @GeneralUtilities.check_arguments
-    def update_path_of_source(repository_folder: str, codeunitname: str) -> None:
-        folder = f"{repository_folder}/{codeunitname}/Other/Artifacts/TestCoverage"
-        filename = "TestCoverage.xml"
-        full_file = os.path.join(folder, filename)
-        TasksForCommonProjectStructure.__adjust_source_in_testcoverage_file(full_file, codeunitname)
+    def replace_version_in_python_file(self, file: str, new_version_value: str) -> None:
+        GeneralUtilities.write_text_to_file(file, re.sub("version = \"\\d+\\.\\d+\\.\\d+\"", f"version = \"{new_version_value}\"", GeneralUtilities.read_text_from_file(file)))
 
     @GeneralUtilities.check_arguments
-    def standardized_tasks_run_testcases_for_python_codeunit(self, run_testcases_file: str, generate_badges: bool, verbosity: int,
-                                                             targetenvironmenttype: str, commandline_arguments: list[str]):
+    def standardized_tasks_run_testcases_for_python_codeunit(self, run_testcases_file: str, generate_badges: bool, verbosity: int,                                                             targetenvironmenttype: str, commandline_arguments: list[str]) -> None:
         codeunitname: str = Path(os.path.dirname(run_testcases_file)).parent.parent.name
         verbosity = TasksForCommonProjectStructure.get_verbosity_from_commandline_arguments(commandline_arguments,  verbosity)
         repository_folder: str = str(Path(os.path.dirname(run_testcases_file)).parent.parent.parent.absolute())
         codeunit_folder = os.path.join(repository_folder, codeunitname)
-        self.__sc.run_program("coverage", f"run -m pytest ./{codeunitname}Tests", codeunit_folder,  verbosity=verbosity)
+        self.__sc.run_program("coverage", f"run -m pytest -s ./{codeunitname}Tests", codeunit_folder,  verbosity=verbosity)
         self.__sc.run_program("coverage", "xml", codeunit_folder, verbosity=verbosity)
         coveragefolder = os.path.join(repository_folder, codeunitname, "Other/Artifacts/TestCoverage")
         GeneralUtilities.ensure_directory_exists(coveragefolder)
         coveragefile = os.path.join(coveragefolder, "TestCoverage.xml")
         GeneralUtilities.ensure_file_does_not_exist(coveragefile)
         os.rename(os.path.join(repository_folder, codeunitname, "coverage.xml"), coveragefile)
-        self.update_path_of_source(repository_folder, codeunitname)
-        self.run_testcases_common_post_task(repository_folder, codeunitname, verbosity, True, targetenvironmenttype, commandline_arguments)
+        self.run_testcases_common_post_task(repository_folder, codeunitname, verbosity, generate_badges, targetenvironmenttype, commandline_arguments)
 
-    def copy_source_files_to_output_directory(self, buildscript_file: str):
+    @GeneralUtilities.check_arguments
+    def copy_source_files_to_output_directory(self, buildscript_file: str) -> None:
         sc = ScriptCollectionCore()
         folder = os.path.dirname(os.path.realpath(buildscript_file))
         codeunit_folder = GeneralUtilities.resolve_relative_path("../..", folder)
         result = sc.run_program_argsasarray("git", ["ls-tree", "-r", "HEAD", "--name-only"], codeunit_folder)
         files = [f for f in result[1].split('\n') if len(f) > 0]
         for file in files:
             full_source_file = os.path.join(codeunit_folder, file)
@@ -237,34 +217,88 @@
                 # Otherwise exceptions occurr because uncommitted deletions of files will result in an error here.
                 target_file = os.path.join(codeunit_folder, "Other", "Artifacts", "SourceCode", file)
                 target_folder = os.path.dirname(target_file)
                 GeneralUtilities.ensure_directory_exists(target_folder)
                 shutil.copyfile(full_source_file, target_file)
 
     @GeneralUtilities.check_arguments
-    def standardized_tasks_build_for_python_codeunit(self, buildscript_file: str, verbosity: int, targetenvironmenttype: str, commandline_arguments: list[str]):
-        self.copy_source_files_to_output_directory(buildscript_file)
+    def standardized_tasks_build_for_dart_project_in_common_project_structure(self, build_script_file: str, verbosity: int, targets: list[str], args: list[str], package_name: str):
+        codeunit_folder = GeneralUtilities.resolve_relative_path("../../..", build_script_file)
+        codeunit_name = os.path.basename(codeunit_folder)
+        src_folder = GeneralUtilities.resolve_relative_path(package_name, codeunit_folder)  # TODO replace packagename
+        artifacts_folder = os.path.join(codeunit_folder, "Other", "Artifacts")
+        verbosity = self.get_verbosity_from_commandline_arguments(args, verbosity)
+        for target in targets:
+            GeneralUtilities.write_message_to_stdout(f"Build package {package_name} for target {target}...")
+            sc = ScriptCollectionCore()
+            sc.program_runner = ProgramRunnerEpew()
+            sc.run_program("flutter", f"build {target}", src_folder, verbosity)
+            if target == "web":
+                web_relase_folder = os.path.join(src_folder, "build/web")
+                web_folder = os.path.join(artifacts_folder, "BuildResult_WebApplication")
+                GeneralUtilities.ensure_directory_does_not_exist(web_folder)
+                GeneralUtilities.ensure_directory_exists(web_folder)
+                GeneralUtilities.copy_content_of_folder(web_relase_folder, web_folder)
+            elif target == "windows":
+                windows_relase_folder = os.path.join(src_folder, "build/windows/runner/Release")
+                windows_folder = os.path.join(artifacts_folder, "BuildResult_Windows")
+                GeneralUtilities.ensure_directory_does_not_exist(windows_folder)
+                GeneralUtilities.ensure_directory_exists(windows_folder)
+                GeneralUtilities.copy_content_of_folder(windows_relase_folder, windows_folder)
+            elif target == "ios":
+                raise ValueError("building for ios is not implemented yet")
+            elif target == "appbundle":
+                aab_folder = os.path.join(artifacts_folder, "BuildResult_AAB")
+                GeneralUtilities.ensure_directory_does_not_exist(aab_folder)
+                GeneralUtilities.ensure_directory_exists(aab_folder)
+                aab_relase_folder = os.path.join(src_folder, "build/app/outputs/bundle/release")
+                aab_file_original = self.__sc.find_file_by_extension(aab_relase_folder, "aab")
+                aab_file = os.path.join(aab_folder, f"{codeunit_name}.aab")
+                shutil.copyfile(aab_file_original, aab_file)
+                bundletool = os.path.join(codeunit_folder, "Other/Resources/AndroidAppBundleTool/bundletool.jar")
+                apk_folder = os.path.join(artifacts_folder, "BuildResult_APK")
+                GeneralUtilities.ensure_directory_does_not_exist(apk_folder)
+                GeneralUtilities.ensure_directory_exists(apk_folder)
+                apks_file = f"{apk_folder}/{codeunit_name}.apks"
+                sc.run_program("java", f"-jar {bundletool} build-apks --bundle={aab_file} --output={apks_file} --mode=universal", aab_relase_folder, verbosity)
+                with zipfile.ZipFile(apks_file, "r") as zip_ref:
+                    zip_ref.extract("universal.apk", apk_folder)
+                GeneralUtilities.ensure_file_does_not_exist(apks_file)
+                os.rename(f"{apk_folder}/universal.apk", f"{apk_folder}/{codeunit_name}.apk")
+            else:
+                raise ValueError(f"Not supported target: {target}")
+        self.copy_source_files_to_output_directory(build_script_file)
+
+    @GeneralUtilities.check_arguments
+    def standardized_tasks_build_for_python_codeunit(self, buildscript_file: str, verbosity: int, targetenvironmenttype: str, commandline_arguments: list[str]) -> None:
         codeunitname: str = Path(os.path.dirname(buildscript_file)).parent.parent.name
         verbosity = TasksForCommonProjectStructure.get_verbosity_from_commandline_arguments(commandline_arguments,  verbosity)
         codeunit_folder = str(Path(os.path.dirname(buildscript_file)).parent.parent.absolute())
         repository_folder: str = str(Path(os.path.dirname(buildscript_file)).parent.parent.parent.absolute())
         target_directory = GeneralUtilities.resolve_relative_path(
             "../Artifacts/BuildResult_Wheel", os.path.join(self.get_artifacts_folder(repository_folder, codeunitname)))
         GeneralUtilities.ensure_directory_exists(target_directory)
         self.__sc.run_program("python", f"-m build --wheel --outdir {target_directory}", codeunit_folder, verbosity=verbosity)
         self.generate_bom_for_python_project(verbosity, codeunit_folder, codeunitname, commandline_arguments)
+        self.copy_source_files_to_output_directory(buildscript_file)
 
     @GeneralUtilities.check_arguments
-    def generate_bom_for_python_project(self, verbosity: int, codeunit_folder: str, codeunitname: str, commandline_arguments: list[str]):
+    def generate_bom_for_python_project(self, verbosity: int, codeunit_folder: str, codeunitname: str, commandline_arguments: list[str]) -> None:
         verbosity = TasksForCommonProjectStructure.get_verbosity_from_commandline_arguments(commandline_arguments,  verbosity)
         codeunitversion = self.get_version_of_codeunit_folder(codeunit_folder)
         bom_folder = "Other/Artifacts/BOM"
         bom_folder_full = os.path.join(codeunit_folder, bom_folder)
         GeneralUtilities.ensure_directory_exists(bom_folder_full)
-        self.__sc.run_program("cyclonedx-py", f"-o ./{bom_folder}/{codeunitname}.{codeunitversion}.sbom.xml -r -i requirements.txt", codeunit_folder, verbosity=verbosity)
+        if not os.path.isfile(os.path.join(codeunit_folder, "requirements.txt")):
+            raise ValueError(f"Codeunit {codeunitname} does not have a 'requirements.txt'-file.")
+        # TODO check that all values from setup.cfg are contained in requirements.txt
+        result = self.__sc.run_program("cyclonedx-py", "requirements", codeunit_folder, verbosity=verbosity)
+        bom_file = os.path.join(codeunit_folder, f"{bom_folder}/{codeunitname}.{codeunitversion}.bom.json")
+        GeneralUtilities.ensure_file_exists(bom_file)
+        GeneralUtilities.write_text_to_file(bom_file, result[1])
 
     @GeneralUtilities.check_arguments
     def standardized_tasks_push_wheel_file_to_registry(self, wheel_file: str, api_key: str, repository: str, gpg_identity: str, verbosity: int) -> None:
         # repository-value when PyPi should be used: "pypi"
         # gpg_identity-value when wheel-file should not be signed: None
         folder = os.path.dirname(wheel_file)
         filename = os.path.basename(wheel_file)
@@ -281,16 +315,15 @@
             verbose_argument = ""
 
         twine_argument = f"upload{gpg_identity_argument} --repository {repository} --non-interactive {filename} --disable-progress-bar"
         twine_argument = f"{twine_argument} --username __token__ --password {api_key}{verbose_argument}"
         self.__sc.run_program("twine", twine_argument, folder, verbosity=verbosity, throw_exception_if_exitcode_is_not_zero=True)
 
     @GeneralUtilities.check_arguments
-    def push_wheel_build_artifact(self, push_build_artifacts_file, product_name, codeunitname, repository: str,
-                                  apikey: str, gpg_identity: str, verbosity: int, commandline_arguments: list[str], repository_folder_name: str) -> None:
+    def push_wheel_build_artifact(self, push_build_artifacts_file, product_name, codeunitname, repository: str, apikey: str, gpg_identity: str, verbosity: int, commandline_arguments: list[str], repository_folder_name: str) -> None:
         verbosity = TasksForCommonProjectStructure.get_verbosity_from_commandline_arguments(commandline_arguments,  verbosity)
         folder_of_this_file = os.path.dirname(push_build_artifacts_file)
         repository_folder = GeneralUtilities.resolve_relative_path(f"..{os.path.sep}../Submodules{os.path.sep}{repository_folder_name}", folder_of_this_file)
         wheel_file = self.get_wheel_file(repository_folder, codeunitname)
         self.standardized_tasks_push_wheel_file_to_registry(wheel_file, apikey, repository, gpg_identity, verbosity)
 
     @GeneralUtilities.check_arguments
@@ -361,15 +394,15 @@
         if result is None:
             return default_value
         else:
             return result
 
     @staticmethod
     @GeneralUtilities.check_arguments
-    def get_filestosign_from_commandline_arguments(commandline_arguments: list[str],  default_value: dict[str, str]) -> dict[str, str]():
+    def get_filestosign_from_commandline_arguments(commandline_arguments: list[str],  default_value: dict[str, str]) -> dict[str, str]:
         result_plain = TasksForCommonProjectStructure.get_property_from_commandline_arguments(commandline_arguments, "sign")
         if result_plain is None:
             return default_value
         else:
             result: dict[str, str] = dict[str, str]()
             files_tuples = GeneralUtilities.to_list(result_plain, ";")
             for files_tuple in files_tuples:
@@ -377,19 +410,23 @@
                 result[splitted[0]] = splitted[1]
             return result
 
     @staticmethod
     @GeneralUtilities.check_arguments
     def get_property_from_commandline_arguments(commandline_arguments: list[str], property_name: str) -> str:
         result: str = None
-        for commandline_argument in commandline_arguments[1:]:
-            prefix = f"--overwrite_{property_name}"
-            if commandline_argument.startswith(prefix):
-                if m := re.match(f"^{re.escape(prefix)}=(.+)$", commandline_argument):
-                    result = m.group(1)
+        count = len(commandline_arguments)
+        loop_index = -1
+        for commandline_argument in commandline_arguments:
+            loop_index = loop_index+1
+            if loop_index < count-1:
+                prefix = f"--overwrite_{property_name}"
+                if commandline_argument == prefix:
+                    result = commandline_arguments[loop_index+1]
+                    return result
         return result
 
     @GeneralUtilities.check_arguments
     def update_version_of_codeunit(self, common_tasks_file: str, current_version: str) -> None:
         codeunit_name: str = os.path.basename(GeneralUtilities.resolve_relative_path("..", os.path.dirname(common_tasks_file)))
         codeunit_file: str = os.path.join(GeneralUtilities.resolve_relative_path("..", os.path.dirname(common_tasks_file)), f"{codeunit_name}.codeunit.xml")
         self.write_version_to_codeunit_file(codeunit_file, current_version)
@@ -422,57 +459,65 @@
         GeneralUtilities.ensure_directory_does_not_exist(obj_folder)
 
     def standardized_task_verify_standard_format_csproj_files(self, codeunit_folder: str) -> bool:
         repository_folder = os.path.dirname(codeunit_folder)
         codeunit_name = os.path.basename(codeunit_folder)
         codeunit_folder = os.path.join(repository_folder, codeunit_name)
         codeunit_version = self.get_version_of_codeunit_folder(codeunit_folder)
-        message = " does not match the standardized .csproj-file-format."
+        message = " does not match the standardized .csproj-file-format which is defined by the regex "
 
-        project_name = codeunit_name
-        csproj_file = os.path.join(codeunit_folder, project_name, project_name+".csproj")
-        if not self.__standardized_task_verify_standard_format_for_project_csproj_file(csproj_file, codeunit_name, codeunit_version):
-            raise ValueError(csproj_file+message)
-
-        testproject_name = project_name+"Tests"
-        test_csproj_file = os.path.join(codeunit_folder, testproject_name, testproject_name+".csproj")
-        if not self.__standardized_task_verify_standard_format_for_test_csproj_file(test_csproj_file, codeunit_name, codeunit_version):
-            raise ValueError(test_csproj_file+message)
+        csproj_project_name = codeunit_name
+        csproj_file = os.path.join(codeunit_folder, csproj_project_name, csproj_project_name+".csproj")
+        result1: tuple[bool, str] = self.__standardized_task_verify_standard_format_for_project_csproj_file(csproj_file, codeunit_folder, codeunit_name, codeunit_version)
+        if not result1[0]:
+            raise ValueError(csproj_file+message+f'"{result1[1]}".')
+
+        test_csproj_project_name = csproj_project_name+"Tests"
+        test_csproj_file = os.path.join(codeunit_folder, test_csproj_project_name, test_csproj_project_name+".csproj")
+        result2: tuple[bool, str] = self.__standardized_task_verify_standard_format_for_test_csproj_file(test_csproj_file, codeunit_name, codeunit_version)
+        if not result2[0]:
+            raise ValueError(test_csproj_file+message+f'"{result2[1]}".')
 
-    def __standardized_task_verify_standard_format_for_project_csproj_file(self, csproj_file: str, codeunit_name: str, codeunit_version: str) -> bool:
+    def __standardized_task_verify_standard_format_for_project_csproj_file(self, csproj_file: str, codeunit_folder: str, codeunit_name: str, codeunit_version: str) -> tuple[bool, str]:
         codeunit_name_regex = re.escape(codeunit_name)
+        codeunit_file = os.path.join(codeunit_folder, f"{codeunit_name}.codeunit.xml")
+        codeunit_description = self.get_codeunit_description(codeunit_file)
         codeunit_version_regex = re.escape(codeunit_version)
+        codeunit_description_regex = re.escape(codeunit_description)
         regex = f"""^<Project Sdk=\\"Microsoft\\.NET\\.Sdk\\">
     <PropertyGroup>
         <TargetFramework>([^<]+)<\\/TargetFramework>
         <Authors>([^<]+)<\\/Authors>
         <Version>{codeunit_version_regex}<\\/Version>
         <AssemblyVersion>{codeunit_version_regex}<\\/AssemblyVersion>
         <FileVersion>{codeunit_version_regex}<\\/FileVersion>
         <SelfContained>false<\\/SelfContained>
         <IsPackable>false<\\/IsPackable>
         <PreserveCompilationContext>false<\\/PreserveCompilationContext>
         <GenerateRuntimeConfigurationFiles>true<\\/GenerateRuntimeConfigurationFiles>
         <Copyright>([^<]+)<\\/Copyright>
-        <Description>([^<]+)<\\/Description>
+        <Description>{codeunit_description_regex}<\\/Description>
         <PackageProjectUrl>https:\\/\\/([^<]+)<\\/PackageProjectUrl>
         <RepositoryUrl>https:\\/\\/([^<]+)\\.git<\\/RepositoryUrl>
         <RootNamespace>([^<]+)\\.Core<\\/RootNamespace>
         <ProduceReferenceAssembly>false<\\/ProduceReferenceAssembly>
-        <Nullable>disable<\\/Nullable>
+        <Nullable>(disable|enable|warnings|annotations)<\\/Nullable>
         <Configurations>Development;QualityCheck;Productive<\\/Configurations>
         <IsTestProject>false<\\/IsTestProject>
         <LangVersion>([^<]+)<\\/LangVersion>
         <PackageRequireLicenseAcceptance>true<\\/PackageRequireLicenseAcceptance>
         <GenerateSerializationAssemblies>Off<\\/GenerateSerializationAssemblies>
         <AppendTargetFrameworkToOutputPath>false<\\/AppendTargetFrameworkToOutputPath>
         <OutputPath>\\.\\.\\\\Other\\\\Artifacts\\\\BuildResult_DotNet_win-x64<\\/OutputPath>
         <PlatformTarget>([^<]+)<\\/PlatformTarget>
         <WarningLevel>\\d<\\/WarningLevel>
         <Prefer32Bit>false<\\/Prefer32Bit>
+        <SignAssembly>True<\\/SignAssembly>
+        <AssemblyOriginatorKeyFile>\\.\\.\\\\\\.\\.\\\\Other\\\\Resources\\\\PublicKeys\\\\StronglyNamedKey\\\\([^<]+)PublicKey\\.snk<\\/AssemblyOriginatorKeyFile>
+        <DelaySign>True<\\/DelaySign>
         <NoWarn>([^<]+)<\\/NoWarn>
         <WarningsAsErrors>([^<]+)<\\/WarningsAsErrors>
         <ErrorLog>\\.\\.\\\\Other\\\\Resources\\\\CodeAnalysisResult\\\\{codeunit_name_regex}\\.sarif<\\/ErrorLog>
         <OutputType>([^<]+)<\\/OutputType>
         <DocumentationFile>\\.\\.\\\\Other\\\\Artifacts\\\\MetaInformation\\\\{codeunit_name_regex}\\.xml<\\/DocumentationFile>(\\n|.)*
     <\\/PropertyGroup>
     <PropertyGroup Condition=\\\"'\\$\\(Configuration\\)'=='Development'\\\">
@@ -493,17 +538,17 @@
         <DebugType>none<\\/DebugType>
         <DebugSymbols>false<\\/DebugSymbols>
         <Optimize>true<\\/Optimize>
         <DefineConstants>Productive<\\/DefineConstants>
         <ErrorReport>none<\\/ErrorReport>
     <\\/PropertyGroup>(\\n|.)*
 <\\/Project>$"""
-        return self.__standardized_task_verify_standard_format_for_csproj_files(regex, csproj_file)
+        return (self.__standardized_task_verify_standard_format_for_csproj_files(regex, csproj_file), regex)
 
-    def __standardized_task_verify_standard_format_for_test_csproj_file(self, csproj_file: str, codeunit_name: str, codeunit_version: str) -> bool:
+    def __standardized_task_verify_standard_format_for_test_csproj_file(self, csproj_file: str, codeunit_name: str, codeunit_version: str) -> tuple[bool, str]:
         codeunit_name_regex = re.escape(codeunit_name)
         codeunit_version_regex = re.escape(codeunit_version)
         regex = f"""^<Project Sdk=\\"Microsoft\\.NET\\.Sdk\\">
     <PropertyGroup>
         <TargetFramework>([^<]+)<\\/TargetFramework>
         <Authors>([^<]+)<\\/Authors>
         <Version>{codeunit_version_regex}<\\/Version>
@@ -515,25 +560,28 @@
         <GenerateRuntimeConfigurationFiles>true<\\/GenerateRuntimeConfigurationFiles>
         <Copyright>([^<]+)<\\/Copyright>
         <Description>{codeunit_name_regex}Tests is the test-project for {codeunit_name_regex}\\.<\\/Description>
         <PackageProjectUrl>https:\\/\\/([^<]+)<\\/PackageProjectUrl>
         <RepositoryUrl>https:\\/\\/([^<]+)\\.git</RepositoryUrl>
         <RootNamespace>([^<]+)\\.Tests<\\/RootNamespace>
         <ProduceReferenceAssembly>false<\\/ProduceReferenceAssembly>
-        <Nullable>disable<\\/Nullable>
+        <Nullable>(disable|enable|warnings|annotations)<\\/Nullable>
         <Configurations>Development;QualityCheck;Productive<\\/Configurations>
         <IsTestProject>true<\\/IsTestProject>
         <LangVersion>([^<]+)<\\/LangVersion>
         <PackageRequireLicenseAcceptance>true<\\/PackageRequireLicenseAcceptance>
         <GenerateSerializationAssemblies>Off<\\/GenerateSerializationAssemblies>
         <AppendTargetFrameworkToOutputPath>false<\\/AppendTargetFrameworkToOutputPath>
         <OutputPath>\\.\\.\\\\Other\\\\Artifacts\\\\BuildResultTests_DotNet_win-x64<\\/OutputPath>
         <PlatformTarget>([^<]+)<\\/PlatformTarget>
         <WarningLevel>\\d<\\/WarningLevel>
         <Prefer32Bit>false<\\/Prefer32Bit>
+        <SignAssembly>True<\\/SignAssembly>
+        <AssemblyOriginatorKeyFile>\\.\\.\\\\\\.\\.\\\\Other\\\\Resources\\\\PublicKeys\\\\StronglyNamedKey\\\\([^<]+)PublicKey\\.snk<\\/AssemblyOriginatorKeyFile>
+        <DelaySign>True<\\/DelaySign>
         <NoWarn>([^<]+)<\\/NoWarn>
         <WarningsAsErrors>([^<]+)<\\/WarningsAsErrors>
         <ErrorLog>\\.\\.\\\\Other\\\\Resources\\\\CodeAnalysisResult\\\\{codeunit_name_regex}Tests\\.sarif<\\/ErrorLog>
         <OutputType>Library<\\/OutputType>(\\n|.)*
     <\\/PropertyGroup>
     <PropertyGroup Condition=\\\"'\\$\\(Configuration\\)'=='Development'\\\">
         <DebugType>full<\\/DebugType>
@@ -553,119 +601,111 @@
         <DebugType>none<\\/DebugType>
         <DebugSymbols>false<\\/DebugSymbols>
         <Optimize>true<\\/Optimize>
         <DefineConstants>Productive<\\/DefineConstants>
         <ErrorReport>none<\\/ErrorReport>
     <\\/PropertyGroup>(\\n|.)*
 <\\/Project>$"""
-        return self.__standardized_task_verify_standard_format_for_csproj_files(regex, csproj_file)
+        return (self.__standardized_task_verify_standard_format_for_csproj_files(regex, csproj_file), regex)
 
     def __standardized_task_verify_standard_format_for_csproj_files(self, regex: str, csproj_file: str) -> bool:
         filename = os.path.basename(csproj_file)
         GeneralUtilities.write_message_to_stdout(f"Check {filename}...")
         file_content = GeneralUtilities.read_text_from_file(csproj_file)
         regex = regex.replace("\r", "").replace("\n", "\\n")
         file_content = file_content.replace("\r", "")
         match = re.match(regex, file_content)
         return match is not None
 
     @GeneralUtilities.check_arguments
-    def __standardized_tasks_build_for_dotnet_build(self, csproj_file: str, originaloutputfolder: str, files_to_sign: dict[str, str], commitid: str,
-                                                    verbosity: int, runtimes: list[str], target_environmenttype: str, target_environmenttype_mapping:  dict[str, str],
-                                                    copy_license_file_to_target_folder: bool, repository_folder: str, codeunit_name: str, commandline_arguments: list[str]):
+    def __standardized_tasks_build_for_dotnet_build(self, csproj_file: str, originaloutputfolder: str, files_to_sign: dict[str, str], commitid: str, verbosity: int, runtimes: list[str], target_environmenttype: str, target_environmenttype_mapping:  dict[str, str], copy_license_file_to_target_folder: bool, repository_folder: str, codeunit_name: str, commandline_arguments: list[str]) -> None:
         dotnet_build_configuration: str = target_environmenttype_mapping[target_environmenttype]
         verbosity = self.get_verbosity_from_commandline_arguments(commandline_arguments, verbosity)
         codeunit_folder = os.path.join(repository_folder, codeunit_name)
         csproj_file_folder = os.path.dirname(csproj_file)
         csproj_file_name = os.path.basename(csproj_file)
         csproj_file_name_without_extension = csproj_file_name.split(".")[0]
         sarif_folder = os.path.join(codeunit_folder, "Other", "Resources", "CodeAnalysisResult")
         GeneralUtilities.ensure_directory_exists(sarif_folder)
+        gitkeep_file = os.path.join(sarif_folder, ".gitkeep")
+        GeneralUtilities.ensure_file_exists(gitkeep_file)
         for runtime in runtimes:
             outputfolder = originaloutputfolder+runtime
-            self.__sc.run_program("dotnet", "clean", csproj_file_folder, verbosity=verbosity)
             GeneralUtilities.ensure_directory_does_not_exist(os.path.join(csproj_file_folder, "obj"))
             GeneralUtilities.ensure_directory_does_not_exist(outputfolder)
+            self.__sc.run_program("dotnet", "clean", csproj_file_folder, verbosity=verbosity)
             GeneralUtilities.ensure_directory_exists(outputfolder)
             self.__sc.run_program("dotnet", "restore", codeunit_folder, verbosity=verbosity)
-            self.__sc.run_program("dotnet", f"build {csproj_file_name} -c {dotnet_build_configuration} -o {outputfolder} --runtime {runtime}",
-                                  csproj_file_folder, verbosity=verbosity)
+            self.__sc.run_program("dotnet", f"build {csproj_file_name} -c {dotnet_build_configuration} -o {outputfolder} --runtime {runtime}", csproj_file_folder, verbosity=verbosity)
             if copy_license_file_to_target_folder:
                 license_file = os.path.join(repository_folder, "License.txt")
                 target = os.path.join(outputfolder, f"{codeunit_name}.License.txt")
                 shutil.copyfile(license_file, target)
-            for file, keyfile in files_to_sign.items():
-                self.__sc.dotnet_sign_file(os.path.join(outputfolder, file), keyfile, verbosity)
-
+            if 0 < len(files_to_sign):
+                for key, value in files_to_sign.items():
+                    dll_file = key
+                    snk_file = value
+                    dll_file_full = os.path.join(outputfolder, dll_file)
+                    if os.path.isfile(dll_file_full):
+                        GeneralUtilities.assert_condition(self.__sc.run_program("sn", f"-vf {dll_file}", outputfolder, throw_exception_if_exitcode_is_not_zero=False)[0] == 1, f"Pre-verifying of {dll_file} failed.")
+                        self.__sc.run_program("sn", f"-R {dll_file} {snk_file}", outputfolder)
+                        GeneralUtilities.assert_condition(self.__sc.run_program("sn", f"-vf {dll_file}", outputfolder, throw_exception_if_exitcode_is_not_zero=False)[0] == 0, f"Verifying of {dll_file} failed.")
             sarif_filename = f"{csproj_file_name_without_extension}.sarif"
             sarif_source_file = os.path.join(sarif_folder, sarif_filename)
             if os.path.exists(sarif_source_file):
-                sarif_folder = os.path.join(codeunit_folder, "Other", "Artifacts", "CodeAnalysisResult")
-                GeneralUtilities.ensure_directory_exists(sarif_folder)
-                sarif_target_file = os.path.join(sarif_folder, sarif_filename)
+                sarif_folder_target = os.path.join(codeunit_folder, "Other", "Artifacts", "CodeAnalysisResult")
+                GeneralUtilities.ensure_directory_exists(sarif_folder_target)
+                sarif_target_file = os.path.join(sarif_folder_target, sarif_filename)
                 GeneralUtilities.ensure_file_does_not_exist(sarif_target_file)
                 shutil.copyfile(sarif_source_file, sarif_target_file)
-                GeneralUtilities.ensure_file_does_not_exist(sarif_source_file)
 
     @GeneralUtilities.check_arguments
-    def standardized_tasks_build_for_dotnet_project(self, buildscript_file: str, default_target_environmenttype: str,
-                                                    target_environmenttype_mapping:  dict[str, str], runtimes: list[str], verbosity: int, commandline_arguments: list[str]):
+    def standardized_tasks_build_for_dotnet_project(self, buildscript_file: str, default_target_environmenttype: str, target_environmenttype_mapping:  dict[str, str], runtimes: list[str], verbosity: int, commandline_arguments: list[str]) -> None:
         # hint: arguments can be overwritten by commandline_arguments
-        # this function builds an exe or dll
+        # this function builds an exe
         target_environmenttype = self.get_targetenvironmenttype_from_commandline_arguments(commandline_arguments, default_target_environmenttype)
         self.__standardized_tasks_build_for_dotnet_project(
             buildscript_file, target_environmenttype_mapping, default_target_environmenttype, verbosity, target_environmenttype,
             runtimes, True, commandline_arguments)
 
     @GeneralUtilities.check_arguments
-    def standardized_tasks_build_for_dotnet_library_project(self, buildscript_file: str, default_target_environmenttype: str,
-                                                            target_environmenttype_mapping:  dict[str, str], runtimes: list[str],
-                                                            verbosity: int, commandline_arguments: list[str]):
+    def standardized_tasks_build_for_dotnet_library_project(self, buildscript_file: str, default_target_environmenttype: str, target_environmenttype_mapping:  dict[str, str], runtimes: list[str], verbosity: int, commandline_arguments: list[str]) -> None:
         # hint: arguments can be overwritten by commandline_arguments
-        # this function builds an exe or dll and converts it to a nupkg-file
+        # this function builds a dll and converts it to a nupkg-file
 
         target_environmenttype = self.get_targetenvironmenttype_from_commandline_arguments(commandline_arguments, default_target_environmenttype)
-        self.__standardized_tasks_build_for_dotnet_project(buildscript_file, target_environmenttype_mapping, default_target_environmenttype,
-                                                           verbosity, target_environmenttype, runtimes, True, commandline_arguments)
-        self.__standardized_tasks_build_nupkg_for_dotnet_create_package(buildscript_file, verbosity,
-                                                                        commandline_arguments)
+        self.__standardized_tasks_build_for_dotnet_project(buildscript_file, target_environmenttype_mapping, default_target_environmenttype, verbosity, target_environmenttype, runtimes, True, commandline_arguments)
+        self.__standardized_tasks_build_nupkg_for_dotnet_create_package(buildscript_file, verbosity, commandline_arguments)
 
     @GeneralUtilities.check_arguments
     def get_default_target_environmenttype_mapping(self) -> dict[str, str]:
         return {
             TasksForCommonProjectStructure.get_development_environment_name(): TasksForCommonProjectStructure.get_development_environment_name(),
             TasksForCommonProjectStructure.get_qualitycheck_environment_name(): TasksForCommonProjectStructure.get_qualitycheck_environment_name(),
             TasksForCommonProjectStructure.get_productive_environment_name(): TasksForCommonProjectStructure.get_productive_environment_name()
         }
 
     @GeneralUtilities.check_arguments
-    def __standardized_tasks_build_for_dotnet_project(self, buildscript_file: str, target_environmenttype_mapping:  dict[str, str],
-                                                      target_environment_type: str,  verbosity: int, target_environmenttype: str,
-                                                      runtimes: list[str], copy_license_file_to_target_folder: bool, commandline_arguments: list[str]) -> None:
-        self.copy_source_files_to_output_directory(buildscript_file)
+    def __standardized_tasks_build_for_dotnet_project(self, buildscript_file: str, target_environmenttype_mapping:  dict[str, str], default_target_environment_type: str,  verbosity: int, target_environment_type: str, runtimes: list[str], copy_license_file_to_target_folder: bool, commandline_arguments: list[str]) -> None:
         codeunitname: str = os.path.basename(str(Path(os.path.dirname(buildscript_file)).parent.parent.absolute()))
         verbosity = TasksForCommonProjectStructure.get_verbosity_from_commandline_arguments(commandline_arguments,  verbosity)
         files_to_sign: dict[str, str] = TasksForCommonProjectStructure.get_filestosign_from_commandline_arguments(commandline_arguments,  dict())
         repository_folder: str = str(Path(os.path.dirname(buildscript_file)).parent.parent.parent.absolute())
         commitid = self.__sc.git_get_commit_id(repository_folder)
         outputfolder = GeneralUtilities.resolve_relative_path("../Artifacts", os.path.dirname(buildscript_file))
         codeunit_folder = os.path.join(repository_folder, codeunitname)
         csproj_file = os.path.join(codeunit_folder, codeunitname, codeunitname + ".csproj")
         csproj_test_file = os.path.join(codeunit_folder, codeunitname+"Tests", codeunitname+"Tests.csproj")
-        self.__standardized_tasks_build_for_dotnet_build(csproj_file,  os.path.join(outputfolder, "BuildResult_DotNet_"), files_to_sign, commitid,
-                                                         verbosity, runtimes, target_environment_type, target_environmenttype_mapping,
-                                                         copy_license_file_to_target_folder, repository_folder, codeunitname, commandline_arguments)
-        self.__standardized_tasks_build_for_dotnet_build(csproj_test_file,  os.path.join(outputfolder, "BuildResultTests_DotNet_"), files_to_sign, commitid,
-                                                         verbosity, runtimes, target_environment_type, target_environmenttype_mapping,
-                                                         copy_license_file_to_target_folder, repository_folder, codeunitname, commandline_arguments)
-
+        self.__standardized_tasks_build_for_dotnet_build(csproj_file,  os.path.join(outputfolder, "BuildResult_DotNet_"), files_to_sign, commitid, verbosity, runtimes, target_environment_type, target_environmenttype_mapping, copy_license_file_to_target_folder, repository_folder, codeunitname, commandline_arguments)
+        self.__standardized_tasks_build_for_dotnet_build(csproj_test_file,  os.path.join(outputfolder, "BuildResultTests_DotNet_"), files_to_sign, commitid, verbosity, runtimes, target_environment_type, target_environmenttype_mapping, copy_license_file_to_target_folder, repository_folder, codeunitname, commandline_arguments)
         self.generate_sbom_for_dotnet_project(codeunit_folder, verbosity, commandline_arguments)
+        self.copy_source_files_to_output_directory(buildscript_file)
 
     @GeneralUtilities.check_arguments
-    def __standardized_tasks_build_nupkg_for_dotnet_create_package(self, buildscript_file: str, verbosity: int, commandline_arguments: list[str]):
+    def __standardized_tasks_build_nupkg_for_dotnet_create_package(self, buildscript_file: str, verbosity: int, commandline_arguments: list[str]) -> None:
         codeunitname: str = os.path.basename(str(Path(os.path.dirname(buildscript_file)).parent.parent.absolute()))
         verbosity = TasksForCommonProjectStructure.get_verbosity_from_commandline_arguments(commandline_arguments,  verbosity)
         repository_folder: str = str(Path(os.path.dirname(buildscript_file)).parent.parent.parent.absolute())
         build_folder = os.path.join(repository_folder, codeunitname, "Other", "Build")
         outputfolder = GeneralUtilities.resolve_relative_path("../Artifacts/BuildResult_NuGet", os.path.dirname(buildscript_file))
         root: etree._ElementTree = etree.parse(os.path.join(build_folder, f"{codeunitname}.nuspec"))
         current_version = root.xpath("//*[name() = 'package']/*[name() = 'metadata']/*[name() = 'version']/text()")[0]
@@ -687,15 +727,19 @@
         sc.run_program("dotnet", f"CycloneDX {codeunit_name}\\{codeunit_name}.csproj -o {bomfile_folder} --disable-github-licenses", codeunit_folder, verbosity=verbosity)
         codeunitversion = self.get_version_of_codeunit(os.path.join(codeunit_folder, f"{codeunit_name}.codeunit.xml"))
         target = f"{codeunit_folder}\\{bomfile_folder}\\{codeunit_name}.{codeunitversion}.sbom.xml"
         GeneralUtilities.ensure_file_does_not_exist(target)
         os.rename(f"{codeunit_folder}\\{bomfile_folder}\\bom.xml", target)
 
     @GeneralUtilities.check_arguments
-    def standardized_tasks_linting_for_python_codeunit(self, linting_script_file: str, verbosity: int, targetenvironmenttype: str, commandline_arguments: list[str]):
+    def standardized_tasks_run_linting_for_flutter_project_in_common_project_structure(self, script_file: str, default_verbosity: int, args: list[str]):
+        pass  # TODO
+
+    @GeneralUtilities.check_arguments
+    def standardized_tasks_linting_for_python_codeunit(self, linting_script_file: str, verbosity: int, targetenvironmenttype: str, commandline_arguments: list[str]) -> None:
         codeunitname: str = Path(os.path.dirname(linting_script_file)).parent.parent.name
         verbosity = TasksForCommonProjectStructure.get_verbosity_from_commandline_arguments(commandline_arguments,  verbosity)
         repository_folder: str = str(Path(os.path.dirname(linting_script_file)).parent.parent.parent.absolute())
         errors_found = False
         GeneralUtilities.write_message_to_stdout(f"Check for linting-issues in codeunit {codeunitname}.")
         src_folder = os.path.join(repository_folder, codeunitname, codeunitname)
         tests_folder = src_folder+"Tests"
@@ -711,16 +755,15 @@
                         GeneralUtilities.write_message_to_stderr(error)
         if errors_found:
             raise ValueError("Linting-issues occurred.")
         else:
             GeneralUtilities.write_message_to_stdout("No linting-issues found.")
 
     @GeneralUtilities.check_arguments
-    def standardized_tasks_generate_coverage_report(self, repository_folder: str, codeunitname: str, verbosity: int, generate_badges: bool, targetenvironmenttype: str,
-                                                    commandline_arguments: list[str], add_testcoverage_history_entry: bool = None):
+    def standardized_tasks_generate_coverage_report(self, repository_folder: str, codeunitname: str, verbosity: int, generate_badges: bool, targetenvironmenttype: str, commandline_arguments: list[str], add_testcoverage_history_entry: bool = None) -> None:
         """This script expects that the file '<repositorybasefolder>/<codeunitname>/Other/Artifacts/TestCoverage/TestCoverage.xml'
         which contains a test-coverage-report in the cobertura-format exists.
         This script expectes that the testcoverage-reportfolder is '<repositorybasefolder>/<codeunitname>/Other/Artifacts/TestCoverageReport'.
         This script expectes that a test-coverage-badges should be added to '<repositorybasefolder>/<codeunitname>/Other/Resources/Badges'."""
         codeunit_version = self.get_version_of_codeunit(os.path.join(repository_folder, codeunitname, f"{codeunitname}.codeunit.xml"))
         verbosity = TasksForCommonProjectStructure.get_verbosity_from_commandline_arguments(commandline_arguments, verbosity)
         if verbosity == 0:
@@ -739,17 +782,18 @@
         if add_testcoverage_history_entry is None:
             add_testcoverage_history_entry = self.get_is_pre_merge_value_from_commandline_arguments(commandline_arguments, add_testcoverage_history_entry)
 
         history_folder = f"{codeunitname}/Other/Resources/TestCoverageHistory"
         history_folder_full = os.path.join(repository_folder, history_folder)
         GeneralUtilities.ensure_directory_exists(history_folder_full)
         history_argument = f" -historydir:{history_folder}"
-        self.__sc.run_program("reportgenerator", f"-reports:{codeunitname}/Other/Artifacts/TestCoverage/TestCoverage.xml " +
-                              f"-targetdir:{codeunitname}/Other/Artifacts/TestCoverageReport --verbosity:{verbose_argument_for_reportgenerator}{history_argument} " +
-                              f"-title:{codeunitname} -tag:v{codeunit_version}",
+        argument = (f"-reports:{codeunitname}/Other/Artifacts/TestCoverage/TestCoverage.xml " +
+                    f"-targetdir:{codeunitname}/Other/Artifacts/TestCoverageReport --verbosity:{verbose_argument_for_reportgenerator}{history_argument} " +
+                    f"-title:{codeunitname} -tag:v{codeunit_version}")
+        self.__sc.run_program("reportgenerator", argument,
                               repository_folder, verbosity=verbosity)
         if not add_testcoverage_history_entry:
             os.remove(GeneralUtilities.get_direct_files_of_folder(history_folder_full)[-1])
 
         # Generating badges
         if generate_badges:
             testcoverageubfolger = "Other/Resources/TestCoverageBadges"
@@ -758,58 +802,116 @@
             GeneralUtilities.ensure_directory_exists(fulltestcoverageubfolger)
             self.__sc.run_program("reportgenerator", "-reports:Other/Artifacts/TestCoverage/TestCoverage.xml " +
                                   f"-targetdir:{testcoverageubfolger} -reporttypes:Badges " +
                                   f"--verbosity:{verbose_argument_for_reportgenerator}", os.path.join(repository_folder, codeunitname),
                                   verbosity=verbosity)
 
     @GeneralUtilities.check_arguments
-    def standardized_tasks_run_testcases_for_dotnet_project(self, runtestcases_file: str, targetenvironmenttype: str, verbosity: int, generate_badges: bool,
-                                                            commandline_arguments: list[str]):
+    def standardized_tasks_run_testcases_for_dotnet_project(self, runtestcases_file: str, targetenvironmenttype: str, verbosity: int, generate_badges: bool,                                                            target_environmenttype_mapping:  dict[str, str], commandline_arguments: list[str]) -> None:
+        dotnet_build_configuration: str = target_environmenttype_mapping[targetenvironmenttype]
         codeunit_name: str = os.path.basename(str(Path(os.path.dirname(runtestcases_file)).parent.parent.absolute()))
         verbosity = TasksForCommonProjectStructure.get_verbosity_from_commandline_arguments(commandline_arguments,  verbosity)
-        repository_folder: str = str(Path(os.path.dirname(runtestcases_file)).parent.parent.parent.absolute())
+        repository_folder: str = str(Path(os.path.dirname(runtestcases_file)).parent.parent.parent.absolute()).replace("\\", "/")
         coverage_file_folder = os.path.join(repository_folder, codeunit_name, "Other/Artifacts/TestCoverage")
-        working_directory = os.path.join(repository_folder, codeunit_name)
-        runsettings_argument = ""
+        temp_folder = os.path.join(tempfile.gettempdir(), str(uuid.uuid4()))
+        GeneralUtilities.ensure_directory_exists(temp_folder)
         runsettings_file = self.dotnet_runsettings_file
-        if os.path.isfile(os.path.join(working_directory, runsettings_file)):
-            runsettings_argument = f"--settings {runsettings_file} "
-        arg = f"collect dotnet test {runsettings_argument} --no-build --output-format cobertura --output Other\\Artifacts\\TestCoverage\\Testcoverage"
-        self.__sc.run_program("dotnet-coverage", arg, working_directory, verbosity=verbosity)
-        os.rename(os.path.join(coverage_file_folder,  "Testcoverage.cobertura.xml"), os.path.join(coverage_file_folder,  "TestCoverage.xml"))
+        codeunit_folder = f"{repository_folder}/{codeunit_name}"
+        arg = f"test . -c {dotnet_build_configuration} -o {temp_folder}"
+        if os.path.isfile(os.path.join(codeunit_folder, runsettings_file)):
+            arg = f"{arg} --settings {runsettings_file}"
+        arg = f"{arg} /p:CollectCoverage=true /p:CoverletOutput=../Other/Artifacts/TestCoverage/Testcoverage /p:CoverletOutputFormat=cobertura"
+        self.__sc.run_program("dotnet", arg, codeunit_folder, verbosity=verbosity)
+        target_file = os.path.join(coverage_file_folder,  "TestCoverage.xml")
+        GeneralUtilities.ensure_file_does_not_exist(target_file)
+        os.rename(os.path.join(coverage_file_folder,  "Testcoverage.cobertura.xml"), target_file)
+        self.__remove_unrelated_package_from_testcoverage_file(target_file, codeunit_name)
+        root: etree._ElementTree = etree.parse(target_file)
+        source_base_path_in_coverage_file: str = root.xpath("//coverage/sources/source/text()")[0].replace("\\", "/")
+        content = GeneralUtilities.read_text_from_file(target_file)
+        GeneralUtilities.assert_condition(source_base_path_in_coverage_file.startswith(repository_folder) or repository_folder.startswith(source_base_path_in_coverage_file), f"Unexpected path for coverage. Sourcepath: \"{source_base_path_in_coverage_file}\"; repository: \"{repository_folder}\"")
+        content = re.sub('\\\\', '/', content)
+        content = re.sub("filename=\"([^\"]+)\"", lambda match: self.__standardized_tasks_run_testcases_for_dotnet_project_helper(source_base_path_in_coverage_file, codeunit_folder, match), content)
+        GeneralUtilities.write_text_to_file(target_file, content)
         self.run_testcases_common_post_task(repository_folder, codeunit_name, verbosity, generate_badges, targetenvironmenttype, commandline_arguments)
 
+    @GeneralUtilities.check_arguments
     def run_testcases_common_post_task(self, repository_folder: str, codeunit_name: str, verbosity: int, generate_badges: bool,
-                                       targetenvironmenttype: str, commandline_arguments: list[str]):
+                                       targetenvironmenttype: str, commandline_arguments: list[str]) -> None:
         coverage_file_folder = os.path.join(repository_folder, codeunit_name, "Other/Artifacts/TestCoverage")
         coveragefiletarget = os.path.join(coverage_file_folder,  "TestCoverage.xml")
-        self.update_path_of_source(repository_folder, codeunit_name)
+        self.update_path_of_source_in_testcoverage_file(repository_folder, codeunit_name)
         self.standardized_tasks_generate_coverage_report(repository_folder, codeunit_name, verbosity, generate_badges, targetenvironmenttype, commandline_arguments)
         self.check_testcoverage(coveragefiletarget, repository_folder, codeunit_name)
 
+    @staticmethod
+    @GeneralUtilities.check_arguments
+    def update_path_of_source_in_testcoverage_file(repository_folder: str, codeunitname: str) -> None:
+        folder = f"{repository_folder}/{codeunitname}/Other/Artifacts/TestCoverage"
+        filename = "TestCoverage.xml"
+        full_file = os.path.join(folder, filename)
+        GeneralUtilities.write_text_to_file(full_file, re.sub("<source>.+<\\/source>", f"<source><!--[repository]/-->./{codeunitname}/</source>", GeneralUtilities.read_text_from_file(full_file)))
+        TasksForCommonProjectStructure.__remove_not_existing_files_from_testcoverage_file(full_file, repository_folder, codeunitname)
+
+    @GeneralUtilities.check_arguments
+    def __standardized_tasks_run_testcases_for_dotnet_project_helper(self, source: str, codeunit_folder: str, match: re.Match) -> str:
+        filename = match.group(1)
+        file = os.path.join(source, filename)
+        # GeneralUtilities.assert_condition(os.path.isfile(file),f"File \"{file}\" does not exist.")
+        GeneralUtilities.assert_condition(file.startswith(codeunit_folder),
+                                          f"Unexpected path for coverage-file. File: \"{file}\"; codeunitfolder: \"{codeunit_folder}\"")
+        filename_relative = f".{file[len(codeunit_folder):]}"
+        return f'filename="{filename_relative}"'
+
+    @staticmethod
+    @GeneralUtilities.check_arguments
+    def __remove_not_existing_files_from_testcoverage_file(testcoveragefile: str, repository_folder: str, codeunit_name: str) -> None:
+        root: etree._ElementTree = etree.parse(testcoveragefile)
+        codeunit_folder = os.path.join(repository_folder, codeunit_name)
+        xpath = f"//coverage/packages/package[@name='{codeunit_name}']/classes/class"
+        classes = root.xpath(xpath)
+        found_existing_files = False
+        for clas in classes:
+            filename = clas.attrib['filename']
+            file = os.path.join(codeunit_folder, filename)
+            if os.path.isfile(file):
+                found_existing_files = True
+            else:
+                clas.getparent().remove(clas)
+        GeneralUtilities.assert_condition(found_existing_files, f"No existing files in testcoderage-report-file \"{testcoveragefile}\".")
+        result = etree.tostring(root).decode("utf-8")
+        GeneralUtilities.write_text_to_file(testcoveragefile, result)
+
+    @GeneralUtilities.check_arguments
+    def __remove_unrelated_package_from_testcoverage_file(self, file: str, codeunit_name: str) -> None:
+        root: etree._ElementTree = etree.parse(file)
+        packages = root.xpath('//coverage/packages/package')
+        for package in packages:
+            if package.attrib['name'] != codeunit_name:
+                package.getparent().remove(package)
+        result = etree.tostring(root).decode("utf-8")
+        GeneralUtilities.write_text_to_file(file, result)
+
     @GeneralUtilities.check_arguments
     def write_version_to_codeunit_file(self, codeunit_file: str, current_version: str) -> None:
         versionregex = "\\d+\\.\\d+\\.\\d+"
         versiononlyregex = f"^{versionregex}$"
         pattern = re.compile(versiononlyregex)
         if pattern.match(current_version):
-            GeneralUtilities.write_text_to_file(codeunit_file, re.sub(f"<cps:version>{versionregex}<\\/cps:version>",
-                                                                      f"<cps:version>{current_version}</cps:version>", GeneralUtilities.read_text_from_file(codeunit_file)))
+            GeneralUtilities.write_text_to_file(codeunit_file, re.sub(f"<cps:version>{versionregex}<\\/cps:version>", f"<cps:version>{current_version}</cps:version>", GeneralUtilities.read_text_from_file(codeunit_file)))
         else:
             raise ValueError(f"Version '{current_version}' does not match version-regex '{versiononlyregex}'.")
 
     @GeneralUtilities.check_arguments
-    def standardized_tasks_linting_for_dotnet_project(self, linting_script_file: str, verbosity: int, targetenvironmenttype: str, commandline_arguments: list[str]):
+    def standardized_tasks_linting_for_dotnet_project(self, linting_script_file: str, verbosity: int, targetenvironmenttype: str, commandline_arguments: list[str]) -> None:
         verbosity = TasksForCommonProjectStructure.get_verbosity_from_commandline_arguments(commandline_arguments,  verbosity)
         # TODO check if there are errors in sarif-file
 
     @GeneralUtilities.check_arguments
-    def __export_codeunit_reference_content_to_reference_repository(self, project_version_identifier: str, replace_existing_content: bool,
-                                                                    target_folder_for_reference_repository: str, repository: str, codeunitname: str, projectname: str,
-                                                                    codeunit_version: str, public_repository_url: str, branch: str) -> None:
+    def __export_codeunit_reference_content_to_reference_repository(self, project_version_identifier: str, replace_existing_content: bool,                                                                    target_folder_for_reference_repository: str, repository: str, codeunitname: str, projectname: str, codeunit_version: str, public_repository_url: str, branch: str) -> None:
         codeunit_folder = os.path.join(repository, codeunitname)
         codeunit_file = os.path.join(codeunit_folder, f"{codeunitname}.codeunit.xml")
         codeunit_has_testcases = self.codeunit_has_testable_sourcecode(codeunit_file)
         target_folder = os.path.join(target_folder_for_reference_repository, project_version_identifier, codeunitname)
         if os.path.isdir(target_folder) and not replace_existing_content:
             raise ValueError(f"Folder '{target_folder}' already exists.")
         GeneralUtilities.ensure_directory_does_not_exist(target_folder)
@@ -876,43 +978,35 @@
 
         if codeunit_has_testcases:
             source_testcoveragereport = os.path.join(other_folder_in_repository, "Artifacts", "TestCoverageReport")
             target_testcoveragereport = os.path.join(target_folder, "TestCoverageReport")
             shutil.copytree(source_testcoveragereport, target_testcoveragereport)
 
     @GeneralUtilities.check_arguments
-    def __standardized_tasks_release_buildartifact(self, information: CreateReleaseInformationForProjectInCommonProjectFormat) -> None:
+    def __standardized_tasks_release_artifact(self, information: CreateReleaseInformationForProjectInCommonProjectFormat) -> None:
         project_version = self.__sc.get_semver_version_from_gitversion(information.repository)
         target_folder_base = os.path.join(information.artifacts_folder, information.projectname, project_version)
         GeneralUtilities.ensure_directory_exists(target_folder_base)
 
-        self.build_codeunits(information.repository, information.verbosity, information.target_environmenttype_for_productive,
-                             information.additional_arguments_file, False, information.export_target)
+        self.build_codeunits(information.repository, information.verbosity, information.target_environmenttype_for_productive, information.additional_arguments_file, False, information.export_target)
 
         reference_folder = os.path.join(information.reference_repository, "ReferenceContent")
 
         for codeunitname in self.get_codeunits(information.repository):
             # Push artifacts to registry
-            if codeunitname in information.artifacts_which_have_artifacts_to_push:
-                scriptfilename = f"PushArtifacts.{codeunitname}.py"
-                push_artifact_to_registry_script = os.path.join(information.push_artifacts_scripts_folder, scriptfilename)
-                if not os.path.isfile(push_artifact_to_registry_script):
-                    raise ValueError(f"Script '{push_artifact_to_registry_script}' does not exist.")
-                GeneralUtilities.write_message_to_stdout(f"Push artifacts of codeunit {codeunitname}.")
-                self.__sc.run_program("python", push_artifact_to_registry_script, information.push_artifacts_scripts_folder,
-                                      verbosity=information.verbosity, throw_exception_if_exitcode_is_not_zero=True)
+            scriptfilename = f"PushArtifacts.{codeunitname}.py"
+            push_artifact_to_registry_script = os.path.join(information.push_artifacts_scripts_folder, scriptfilename)
+            if os.path.isfile(push_artifact_to_registry_script):
+                GeneralUtilities.write_message_to_stdout(f"Push artifacts of codeunit {codeunitname}...")
+                self.__sc.run_program("python", push_artifact_to_registry_script, information.push_artifacts_scripts_folder, verbosity=information.verbosity, throw_exception_if_exitcode_is_not_zero=True)
 
             # Copy reference of codeunit to reference-repository
             codeunit_version = self.get_version_of_codeunit_folder(os.path.join(information.repository, codeunitname))
-            self.__export_codeunit_reference_content_to_reference_repository(f"v{project_version}", False, reference_folder, information.repository,
-                                                                             codeunitname, information.projectname, codeunit_version, information.public_repository_url,
-                                                                             f"v{project_version}")
-            self.__export_codeunit_reference_content_to_reference_repository("Latest", True, reference_folder, information.repository,
-                                                                             codeunitname, information.projectname, codeunit_version, information.public_repository_url,
-                                                                             information.target_branch_name)
+            self.__export_codeunit_reference_content_to_reference_repository(f"v{project_version}", False, reference_folder, information.repository,                                                                             codeunitname, information.projectname, codeunit_version, information.public_repository_url,                                                                             f"v{project_version}")
+            self.__export_codeunit_reference_content_to_reference_repository("Latest", True, reference_folder, information.repository,                                                                             codeunitname, information.projectname, codeunit_version, information.public_repository_url,                                                                             information.target_branch_name)
 
             # Generate reference
             self.__generate_entire_reference(information.projectname, project_version, reference_folder)
 
     @staticmethod
     @GeneralUtilities.check_arguments
     def _internal_sort_reference_folder(folder1: str, folder2: str) -> int:
@@ -938,16 +1032,15 @@
             return 1
         else:
             return 0
 
     @GeneralUtilities.check_arguments
     def __generate_entire_reference(self, projectname: str, project_version: str, reference_folder: str) -> None:
         all_available_version_identifier_folders_of_reference: list[str] = list(folder for folder in GeneralUtilities.get_direct_folders_of_folder(reference_folder))
-        all_available_version_identifier_folders_of_reference = sorted(all_available_version_identifier_folders_of_reference,
-                                                                       key=cmp_to_key(TasksForCommonProjectStructure._internal_sort_reference_folder))
+        all_available_version_identifier_folders_of_reference = sorted(all_available_version_identifier_folders_of_reference,                                                                       key=cmp_to_key(TasksForCommonProjectStructure._internal_sort_reference_folder))
         reference_versions_html_lines = []
         reference_versions_html_lines.append('    <hr/>')
         for all_available_version_identifier_folder_of_reference in all_available_version_identifier_folders_of_reference:
             version_identifier_of_project = os.path.basename(all_available_version_identifier_folder_of_reference)
             if version_identifier_of_project == "Latest":
                 latest_version_hint = f" (v{project_version})"
             else:
@@ -995,16 +1088,15 @@
         GeneralUtilities.write_text_to_file(reference_index_file, reference_index_file_content)
 
     @GeneralUtilities.check_arguments
     def push_nuget_build_artifact(self, push_script_file: str, codeunitname: str, registry_address: str, api_key: str, repository_folder_name: str):
         # when pusing to "default public" nuget-server then use registry_address: "nuget.org"
         build_artifact_folder = GeneralUtilities.resolve_relative_path(
             f"../../Submodules/{repository_folder_name}/{codeunitname}/Other/Artifacts/BuildResult_NuGet", os.path.dirname(push_script_file))
-        self.__sc.push_nuget_build_artifact(self.__sc.find_file_by_extension(build_artifact_folder, "nupkg"),
-                                            registry_address, api_key)
+        self.__sc.push_nuget_build_artifact(self.__sc.find_file_by_extension(build_artifact_folder, "nupkg"), registry_address, api_key)
 
     @GeneralUtilities.check_arguments
     def assert_no_uncommitted_changes(self, repository_folder: str):
         if self.__sc.git_repository_has_uncommitted_changes(repository_folder):
             raise ValueError(f"Repository '{repository_folder}' has uncommitted changes.")
 
     @GeneralUtilities.check_arguments
@@ -1037,33 +1129,41 @@
             self.__sc.generate_certificate_authority(ca_folder, dev_ca_name, "DE", "SubjST", "SubjL", "SubjO", "SubjOU")
             self.__sc.generate_certificate(certificate_folder, domain, resource_content_filename, "DE", "SubjST", "SubjL", "SubjO", "SubjOU")
             self.__sc.generate_certificate_sign_request(certificate_folder, domain, resource_content_filename, "DE", "SubjST", "SubjL", "SubjO", "SubjOU")
             self.__sc.sign_certificate(certificate_folder, ca_folder, dev_ca_name, domain, resource_content_filename)
             GeneralUtilities.ensure_file_does_not_exist(unsignedcertificate_file)
 
     @GeneralUtilities.check_arguments
-    def get_codeunits(self, repository_folder: str) -> list[str]:
+    def get_codeunits(self, repository_folder: str, ignore_disabled_codeunits: bool = True) -> list[str]:
         result: list[str] = []
         for direct_subfolder in GeneralUtilities.get_direct_folders_of_folder(repository_folder):
             subfoldername = os.path.basename(direct_subfolder)
-            if os.path.isfile(os.path.join(direct_subfolder, f"{subfoldername}.codeunit.xml")):
-                result.append(subfoldername)
+            codeunit_file = os.path.join(direct_subfolder, f"{subfoldername}.codeunit.xml")
+            if os.path.isfile(codeunit_file):
+                if (ignore_disabled_codeunits):
+                    if (self.codeunit_is_enabled(codeunit_file)):
+                        result.append(subfoldername)
+                else:
+                    result.append(subfoldername)
         return result
 
     @GeneralUtilities.check_arguments
-    def merge_to_main_branch(self, repository_folder: str, source_branch: str = "other/next-release",
-                             target_branch: str = "main", verbosity: int = 1, additional_arguments_file: str = None, fast_forward_source_branch: bool = False) -> None:
+    def codeunit_is_enabled(self, codeunit_file: str) -> bool:
+        root: etree._ElementTree = etree.parse(codeunit_file)
+        return GeneralUtilities.string_to_boolean(str(root.xpath('//cps:codeunit/@enabled', namespaces={'cps': 'https://projects.aniondev.de/PublicProjects/Common/ProjectTemplates/-/tree/main/Conventions/RepositoryStructure/CommonProjectStructure'})[0]))
+
+    @GeneralUtilities.check_arguments
+    def merge_to_main_branch(self, repository_folder: str, source_branch: str = "other/next-release", target_branch: str = "main", verbosity: int = 1, additional_arguments_file: str = None, fast_forward_source_branch: bool = False) -> None:
         # This is an automatization for automatic merges. Usual this merge would be done by a pull request in a sourcecode-version-control-platform
         # (like GitHub, GitLab or Azure DevOps)
         self.assert_no_uncommitted_changes(repository_folder)
 
         src_branch_commit_id = self.__sc.git_get_commit_id(repository_folder,  source_branch)
         if (src_branch_commit_id == self.__sc.git_get_commit_id(repository_folder,  target_branch)):
-            GeneralUtilities.write_message_to_stderr(
-                f"Can not merge because the source-branch and the target-branch are on the same commit (commit-id: {src_branch_commit_id})")
+            raise ValueError(f"Can not merge because the source-branch and the target-branch are on the same commit (commit-id: {src_branch_commit_id})")
 
         self.__sc.git_checkout(repository_folder, source_branch)
         self.build_codeunits(repository_folder, verbosity, "QualityCheck", additional_arguments_file, True, None)
         self.__sc.git_merge(repository_folder, source_branch, target_branch, False, False, None)
         self.__sc.git_commit(repository_folder, f'Merge branch {source_branch} into {target_branch}', stage_all_changes=True, no_changes_behavior=1)
         self.__sc.git_checkout(repository_folder, target_branch)
         if fast_forward_source_branch:
@@ -1077,133 +1177,116 @@
 
         build_repository_folder = GeneralUtilities.resolve_relative_path(f"..{os.path.sep}..", folder_of_create_release_file_file)
         self.assert_no_uncommitted_changes(build_repository_folder)
 
         self.__sc.git_checkout(build_repository_folder, createRelease_configuration.build_repository_branch)
 
         repository_folder = GeneralUtilities.resolve_relative_path(f"Submodules{os.path.sep}{createRelease_configuration.repository_folder_name}", build_repository_folder)
-        mergeInformation = MergeToStableBranchInformationForProjectInCommonProjectFormat(repository_folder,
-                                                                                         createRelease_configuration.additional_arguments_file,
-                                                                                         createRelease_configuration.artifacts_folder)
+        mergeInformation = MergeToStableBranchInformationForProjectInCommonProjectFormat(repository_folder, createRelease_configuration.additional_arguments_file, createRelease_configuration.artifacts_folder)
 
         # TODO check if repository_folder-merge-source-branch and repository_folder-merge-target-branch have different commits
         self.assert_no_uncommitted_changes(repository_folder)
         mergeInformation.verbosity = createRelease_configuration.verbosity
         mergeInformation.push_target_branch = createRelease_configuration.remotename is not None
         mergeInformation.push_target_branch_remote_name = createRelease_configuration.remotename
         mergeInformation.push_source_branch = createRelease_configuration.remotename is not None
         mergeInformation.push_source_branch_remote_name = createRelease_configuration.remotename
         new_project_version = self.__standardized_tasks_merge_to_stable_branch(mergeInformation)
 
-        createReleaseInformation = CreateReleaseInformationForProjectInCommonProjectFormat(repository_folder,
-                                                                                           createRelease_configuration.artifacts_folder,
-                                                                                           createRelease_configuration.projectname,
-                                                                                           createRelease_configuration.public_repository_url,
-                                                                                           mergeInformation.targetbranch,
-                                                                                           mergeInformation.additional_arguments_file,
-                                                                                           mergeInformation.export_target,
-                                                                                           createRelease_configuration.push_artifacts_scripts_folder,
-                                                                                           createRelease_configuration.artifacts_which_have_artifacts_to_push)
+        createReleaseInformation = CreateReleaseInformationForProjectInCommonProjectFormat(repository_folder, createRelease_configuration.artifacts_folder, createRelease_configuration.projectname, createRelease_configuration.public_repository_url, mergeInformation.targetbranch, mergeInformation.additional_arguments_file, mergeInformation.export_target, createRelease_configuration.push_artifacts_scripts_folder)
         createReleaseInformation.verbosity = createRelease_configuration.verbosity
-        self.__standardized_tasks_release_buildartifact(createReleaseInformation)
+        self.__standardized_tasks_release_artifact(createReleaseInformation)
 
         self.__sc.git_commit(createReleaseInformation.reference_repository, f"Added reference of {createRelease_configuration.projectname} v{new_project_version}")
         if createRelease_configuration.reference_repository_remote_name is not None:
-            self.__sc.git_push(createReleaseInformation.reference_repository, createRelease_configuration.reference_repository_remote_name,
-                               createRelease_configuration.reference_repository_branch_name, createRelease_configuration.reference_repository_branch_name,
-                               verbosity=createRelease_configuration.verbosity)
+            self.__sc.git_push(createReleaseInformation.reference_repository, createRelease_configuration.reference_repository_remote_name, createRelease_configuration.reference_repository_branch_name, createRelease_configuration.reference_repository_branch_name, verbosity=createRelease_configuration.verbosity)
         self.__sc.git_commit(build_repository_folder, f"Added {createRelease_configuration.projectname} release v{new_project_version}")
         GeneralUtilities.write_message_to_stdout(f"Finished release for project {createRelease_configuration.projectname} v{new_project_version} successfully.")
         return new_project_version
 
     @GeneralUtilities.check_arguments
-    def create_release_starter_for_repository_in_standardized_format(self, create_release_file: str, logfile: str, verbosity: int, addLogOverhead: bool,
-                                                                     commandline_arguments: list[str]):
+    def create_release_starter_for_repository_in_standardized_format(self, create_release_file: str, logfile: str, verbosity: int, addLogOverhead: bool, commandline_arguments: list[str]):
         # hint: arguments can be overwritten by commandline_arguments
         folder_of_this_file = os.path.dirname(create_release_file)
         verbosity = TasksForCommonProjectStructure.get_verbosity_from_commandline_arguments(commandline_arguments, verbosity)
-        self.__sc.run_program("python", f"CreateRelease.py --overwrite_verbosity={str(verbosity)}",
+        self.__sc.run_program("python", f"CreateRelease.py --overwrite_verbosity {str(verbosity)}",
                               folder_of_this_file,  verbosity=verbosity, log_file=logfile, addLogOverhead=addLogOverhead)
 
     @GeneralUtilities.check_arguments
     def __standardized_tasks_merge_to_stable_branch(self, information: MergeToStableBranchInformationForProjectInCommonProjectFormat) -> str:
-
         src_branch_commit_id = self.__sc.git_get_commit_id(information.repository,  information.sourcebranch)
         if (src_branch_commit_id == self.__sc.git_get_commit_id(information.repository,  information.targetbranch)):
-            GeneralUtilities.write_message_to_stderr(
-                f"Can not merge because the source-branch and the target-branch are on the same commit (commit-id: {src_branch_commit_id})")
+            raise ValueError(f"Can not merge because the source-branch and the target-branch are on the same commit (commit-id: {src_branch_commit_id})")
 
         self.assert_no_uncommitted_changes(information.repository)
         self.__sc.git_checkout(information.repository, information.sourcebranch)
         self.__sc.run_program("git", "clean -dfx", information.repository,  verbosity=information.verbosity, throw_exception_if_exitcode_is_not_zero=True)
         project_version = self.__sc.get_semver_version_from_gitversion(information.repository)
 
-        self.build_codeunits(information.repository, information.verbosity, information.target_environmenttype_for_qualitycheck,
-                             information.additional_arguments_file, False, information.export_target)
+        self.build_codeunits(information.repository, information.verbosity, information.target_environmenttype_for_qualitycheck, information.additional_arguments_file, False, information.export_target)
 
         self.assert_no_uncommitted_changes(information.repository)
 
         commit_id = self.__sc.git_merge(information.repository, information.sourcebranch, information.targetbranch, True, True)
         self.__sc.git_create_tag(information.repository, commit_id, f"v{project_version}", information.sign_git_tags)
 
         if information.push_source_branch:
             GeneralUtilities.write_message_to_stdout("Push source-branch...")
-            self.__sc.git_push(information.repository, information.push_source_branch_remote_name,
-                               information.sourcebranch, information.sourcebranch, pushalltags=True, verbosity=information.verbosity)
+            self.__sc.git_push(information.repository, information.push_source_branch_remote_name, information.sourcebranch, information.sourcebranch, pushalltags=True, verbosity=information.verbosity)
 
         if information.push_target_branch:
             GeneralUtilities.write_message_to_stdout("Push target-branch...")
-            self.__sc.git_push(information.repository, information.push_target_branch_remote_name,
-                               information.targetbranch, information.targetbranch, pushalltags=True, verbosity=information.verbosity)
+            self.__sc.git_push(information.repository, information.push_target_branch_remote_name, information.targetbranch, information.targetbranch, pushalltags=True, verbosity=information.verbosity)
 
         return project_version
 
     @GeneralUtilities.check_arguments
-    def standardized_tasks_build_for_docker_project(self, build_script_file: str, target_environment_type: str,
-                                                    verbosity: int, commandline_arguments: list[str]):
-        self.copy_source_files_to_output_directory(build_script_file)
-        use_cache: bool = target_environment_type != "Productive"
+    def standardized_tasks_build_for_docker_project(self, build_script_file: str, target_environment_type: str, verbosity: int, commandline_arguments: list[str]) -> None:
+        use_cache: bool = False
         verbosity = TasksForCommonProjectStructure.get_verbosity_from_commandline_arguments(commandline_arguments, verbosity)
         sc: ScriptCollectionCore = ScriptCollectionCore()
         codeunitname: str = Path(os.path.dirname(build_script_file)).parent.parent.name
         codeunit_folder = GeneralUtilities.resolve_relative_path("../..", str(os.path.dirname(build_script_file)))
         codeunitname_lower = codeunitname.lower()
         codeunitversion = self.get_version_of_codeunit(os.path.join(codeunit_folder, f"{codeunitname}.codeunit.xml"))
-        args = ["image", "build", "--pull", "--force-rm", "--progress=plain", "--build-arg", f"TargetEnvironmentType={target_environment_type}",
-                "--tag", f"{codeunitname_lower}:latest", "--tag", f"{codeunitname_lower}:{codeunitversion}", "--file", f"{codeunitname}/Dockerfile"]
+        args = ["image", "build", "--pull", "--force-rm", "--progress=plain", "--build-arg", f"TargetEnvironmentType={target_environment_type}", "--tag", f"{codeunitname_lower}:latest", "--tag", f"{codeunitname_lower}:{codeunitversion}", "--file", f"{codeunitname}/Dockerfile"]
         if not use_cache:
             args.append("--no-cache")
         args.append(".")
         codeunit_content_folder = os.path.join(codeunit_folder)
         sc.run_program_argsasarray("docker", args, codeunit_content_folder, verbosity=verbosity, print_errors_as_information=True)
         artifacts_folder = GeneralUtilities.resolve_relative_path("Other/Artifacts", codeunit_folder)
         app_artifacts_folder = os.path.join(artifacts_folder, "BuildResult_OCIImage")
         GeneralUtilities.ensure_directory_does_not_exist(app_artifacts_folder)
         GeneralUtilities.ensure_directory_exists(app_artifacts_folder)
-        self.__sc.run_program_argsasarray("docker", ["save", "--output", f"{codeunitname}_v{codeunitversion}.tar",
-                                                     f"{codeunitname_lower}:{codeunitversion}"], app_artifacts_folder,
-                                          verbosity=verbosity, print_errors_as_information=True)
+        self.__sc.run_program_argsasarray("docker", ["save", "--output", f"{codeunitname}_v{codeunitversion}.tar", f"{codeunitname_lower}:{codeunitversion}"], app_artifacts_folder, verbosity=verbosity, print_errors_as_information=True)
+        self.copy_source_files_to_output_directory(build_script_file)
 
     @GeneralUtilities.check_arguments
     def generate_sbom_for_docker_image(self, build_script_file: str, verbosity: int, commandline_arguments: list[str]) -> None:
         verbosity = TasksForCommonProjectStructure.get_verbosity_from_commandline_arguments(commandline_arguments, verbosity)
         codeunitname: str = Path(os.path.dirname(build_script_file)).parent.parent.name
         codeunit_folder = GeneralUtilities.resolve_relative_path("../..", str(os.path.dirname(build_script_file)))
         artifacts_folder = GeneralUtilities.resolve_relative_path("Other/Artifacts", codeunit_folder)
         codeunitname_lower = codeunitname.lower()
         sbom_folder = os.path.join(artifacts_folder, "BOM")
         codeunitversion = self.get_version_of_codeunit(os.path.join(codeunit_folder, f"{codeunitname}.codeunit.xml"))
         GeneralUtilities.ensure_directory_exists(sbom_folder)
-        self.__sc.run_program_argsasarray("docker", ["sbom", "--format", "cyclonedx", f"{codeunitname_lower}:{codeunitversion}",
-                                                     "--output", f"{codeunitname}.{codeunitversion}.sbom.xml"], sbom_folder, verbosity=verbosity, print_errors_as_information=True)
+        self.__sc.run_program_argsasarray("docker", ["sbom", "--format", "cyclonedx", f"{codeunitname_lower}:{codeunitversion}", "--output", f"{codeunitname}.{codeunitversion}.sbom.xml"], sbom_folder, verbosity=verbosity, print_errors_as_information=True)
 
     @GeneralUtilities.check_arguments
-    def push_docker_build_artifact(self, push_artifacts_file: str, registry: str, project_name: str, codeunitname: str,
-                                   verbosity: int, push_readme: bool, commandline_arguments: list[str], repository_folder_name: str):
+    def push_docker_build_artifact(self, push_artifacts_file: str, registry: str, verbosity: int, push_readme: bool, commandline_arguments: list[str], repository_folder_name: str) -> None:
         folder_of_this_file = os.path.dirname(push_artifacts_file)
+        filename = os.path.basename(push_artifacts_file)
+        codeunitname_regex: str = "([a-zA-Z0-9]+)"
+        filename_regex: str = f"PushArtifacts\\.{codeunitname_regex}\\.py"
+        if match := re.search(filename_regex, filename, re.IGNORECASE):
+            codeunitname = match.group(1)
+        else:
+            raise ValueError(f"Expected push-artifacts-file to match the regex \"{filename_regex}\" where \"{codeunitname_regex}\" represents the codeunit-name.")
         verbosity = TasksForCommonProjectStructure.get_verbosity_from_commandline_arguments(commandline_arguments, verbosity)
         repository_folder = GeneralUtilities.resolve_relative_path(f"..{os.path.sep}..{os.path.sep}Submodules{os.path.sep}{repository_folder_name}", folder_of_this_file)
         codeunit_folder = os.path.join(repository_folder, codeunitname)
         artifacts_folder = self.get_artifacts_folder(repository_folder, codeunitname)
         applicationimage_folder = os.path.join(artifacts_folder, "BuildResult_OCIImage")
         sc = ScriptCollectionCore()
         image_file = sc.find_file_by_extension(applicationimage_folder, "tar")
@@ -1223,69 +1306,72 @@
         sc.run_program("docker", f"push {image_version}", verbosity=verbosity)
         if push_readme:
             sc.run_program("docker", f"pushrm {repo}", codeunit_folder, verbosity=verbosity)
 
     @GeneralUtilities.check_arguments
     def get_dependent_code_units(self, codeunit_file: str) -> set[str]:
         root: etree._ElementTree = etree.parse(codeunit_file)
-        return set(root.xpath('//cps:dependentcodeunit/text()', namespaces={
-            'cps': 'https://projects.aniondev.de/PublicProjects/Common/ProjectTemplates/-/tree/main/Conventions/RepositoryStructure/CommonProjectStructure'
-        }))
+        return set(root.xpath('//cps:dependentcodeunit/text()', namespaces={'cps': 'https://projects.aniondev.de/PublicProjects/Common/ProjectTemplates/-/tree/main/Conventions/RepositoryStructure/CommonProjectStructure'}))
+
+    @GeneralUtilities.check_arguments
+    def dependent_codeunit_exists(self, repository: str, codeunit: str) -> None:
+        codeunit_file = f"{repository}/{codeunit}/{codeunit}.codeunit.xml"
+        return os.path.isfile(codeunit_file)
 
     @GeneralUtilities.check_arguments
     def standardized_tasks_linting_for_docker_project(self, linting_script_file: str, verbosity: int, targetenvironmenttype: str, commandline_arguments: list[str]) -> None:
         verbosity = TasksForCommonProjectStructure.get_verbosity_from_commandline_arguments(commandline_arguments,  verbosity)
         # TODO check if there are errors in sarif-file
 
-    def copy_licence_file(self, common_tasks_scripts_file: str):
+    @GeneralUtilities.check_arguments
+    def copy_licence_file(self, common_tasks_scripts_file: str) -> None:
         folder_of_current_file = os.path.dirname(common_tasks_scripts_file)
         license_file = GeneralUtilities.resolve_relative_path("../../License.txt", folder_of_current_file)
         target_folder = GeneralUtilities.resolve_relative_path("Artifacts/License", folder_of_current_file)
         GeneralUtilities.ensure_directory_exists(target_folder)
         shutil.copy(license_file, target_folder)
 
-    def take_readmefile_from_main_readmefile_of_repository(self, common_tasks_scripts_file: str):
+    @GeneralUtilities.check_arguments
+    def take_readmefile_from_main_readmefile_of_repository(self, common_tasks_scripts_file: str) -> None:
         folder_of_current_file = os.path.dirname(common_tasks_scripts_file)
         source_file = GeneralUtilities.resolve_relative_path("../../ReadMe.md", folder_of_current_file)
         target_file = GeneralUtilities.resolve_relative_path("../ReadMe.md", folder_of_current_file)
         GeneralUtilities.ensure_file_does_not_exist(target_file)
         shutil.copyfile(source_file, target_file)
 
     @GeneralUtilities.check_arguments
-    def standardized_tasks_do_common_tasks(self, common_tasks_scripts_file: str, codeunit_version: str, verbosity: int,  targetenvironmenttype: str,  clear_artifacts_folder: bool,
-                                           additional_arguments_file: str, assume_dependent_codeunits_are_already_built: bool, commandline_arguments: list[str]) -> None:
+    def standardized_tasks_do_common_tasks(self, common_tasks_scripts_file: str, codeunit_version: str, verbosity: int,  targetenvironmenttype: str,  clear_artifacts_folder: bool,                                           additional_arguments_file: str, assume_dependent_codeunits_are_already_built: bool, commandline_arguments: list[str]) -> None:
         additional_arguments_file = self.get_additionalargumentsfile_from_commandline_arguments(commandline_arguments, additional_arguments_file)
         target_environmenttype = self.get_targetenvironmenttype_from_commandline_arguments(commandline_arguments, targetenvironmenttype)
-        assume_dependent_codeunits_are_already_built = self.get_assume_dependent_codeunits_are_already_built_from_commandline_arguments(commandline_arguments,
-                                                                                                                                        assume_dependent_codeunits_are_already_built)
+        assume_dependent_codeunits_are_already_built = self.get_assume_dependent_codeunits_are_already_built_from_commandline_arguments(commandline_arguments,                                                                                                                                        assume_dependent_codeunits_are_already_built)
         if commandline_arguments is None:
             raise ValueError('The "commandline_arguments"-parameter is not defined.')
         if len(commandline_arguments) == 0:
             raise ValueError('An empty array as argument for the "commandline_arguments"-parameter is not valid.')
         commandline_arguments = commandline_arguments[1:]
         repository_folder: str = str(Path(os.path.dirname(common_tasks_scripts_file)).parent.parent.absolute())
         codeunit_name: str = str(os.path.basename(Path(os.path.dirname(common_tasks_scripts_file)).parent.absolute()))
         verbosity = TasksForCommonProjectStructure.get_verbosity_from_commandline_arguments(commandline_arguments, verbosity)
         project_version = self.get_version_of_project(repository_folder)
         codeunit_folder = os.path.join(repository_folder, codeunit_name)
 
         # Check codeunit-conformity
         # TODO check if foldername=="<codeunitname>[.codeunit.xml]" == <codeunitname> in file
+        supported_codeunitspecificationversion = "2.7.10"  # should always be the latest version of the ProjectTemplates-repository
         codeunit_file = os.path.join(codeunit_folder, f"{codeunit_name}.codeunit.xml")
         if not os.path.isfile(codeunit_file):
             raise ValueError(f'Codeunitfile "{codeunit_file}" does not exist.')
         # TODO implement usage of self.reference_latest_version_of_xsd_when_generating_xml
         namespaces = {'cps': 'https://projects.aniondev.de/PublicProjects/Common/ProjectTemplates/-/tree/main/Conventions/RepositoryStructure/CommonProjectStructure',
                       'xsi': 'http://www.w3.org/2001/XMLSchema-instance'}
         root: etree._ElementTree = etree.parse(codeunit_file)
 
         # Check codeunit-spcecification-version
         try:
             codeunit_file_version = root.xpath('//cps:codeunit/@codeunitspecificationversion', namespaces=namespaces)[0]
-            supported_codeunitspecificationversion = "2.7.2"  # should always be the latest version of the ProjectTemplates-repository
             if codeunit_file_version != supported_codeunitspecificationversion:
                 raise ValueError(f"ScriptCollection only supports processing codeunits with codeunit-specification-version={supported_codeunitspecificationversion}.")
             schemaLocation = root.xpath('//cps:codeunit/@xsi:schemaLocation', namespaces=namespaces)[0]
             xmlschema.validate(codeunit_file, schemaLocation)
         except Exception as exception:
             if self.codeunit_throws_exception_if_codeunitfile_is_not_validatable(codeunit_file):
                 raise exception
@@ -1317,30 +1403,30 @@
                 author_name = expected_author.xpath('./cps:developername/text()', namespaces=namespaces)[0]
                 author_emailaddress = expected_author.xpath('./cps:developeremailaddress/text()', namespaces=namespaces)[0]
                 expected_authors.append((author_name, author_emailaddress))
             actual_authors: list[tuple[str, str]] = self.__sc.get_all_authors_and_committers_of_repository(repository_folder, codeunit_name, verbosity)
             for actual_author in actual_authors:
                 if not (actual_author) in expected_authors:
                     actual_author_formatted = f"{actual_author[0]} <{actual_author[1]}>"
-                    raise ValueError(f'Author/Comitter "{actual_author_formatted}" is not in the codeunit-developer-team. If {actual_author} is a '
-                                     + 'authorized developer for this codeunit you should consider defining this in the codeunit-file or adapting the name using a '
-                                     + '.mailmap-file (see https://git-scm.com/docs/gitmailmap). The developer-team-check can also be disabled using '
-                                     + 'the property validate_developers_of_repository.')
+                    raise ValueError(f'Author/Comitter "{actual_author_formatted}" is not in the codeunit-developer-team. If {actual_author} is a authorized developer for this codeunit you should consider defining this in the codeunit-file or adapting the name using a .mailmap-file (see https://git-scm.com/docs/gitmailmap). The developer-team-check can also be disabled using the property validate_developers_of_repository.')
+
+        dependent_codeunits = self.get_dependent_code_units(codeunit_file)
+        for dependent_codeunit in dependent_codeunits:
+            if not self.dependent_codeunit_exists(repository_folder, dependent_codeunit):
+                raise ValueError(f"Codeunit {codeunit_name} does have dependent codeunit {dependent_codeunit} which does not exist.")
 
         # TODO implement cycle-check for dependent codeunits
 
         # Clear previously builded artifacts if desired:
         if clear_artifacts_folder:
             artifacts_folder = os.path.join(codeunit_folder, "Other", "Artifacts")
             GeneralUtilities.ensure_directory_does_not_exist(artifacts_folder)
 
         # Get artifacts from dependent codeunits
         if assume_dependent_codeunits_are_already_built:
-            pass  # TODO do basic checks to verify dependent codeunits are really there and raise exception if not
-        else:
             self.build_dependent_code_units(repository_folder, codeunit_name, verbosity, target_environmenttype, additional_arguments_file)
         self.copy_artifacts_from_dependent_code_units(repository_folder, codeunit_name)
 
         # Update codeunit-version
         self.update_version_of_codeunit(common_tasks_scripts_file, codeunit_version)
 
         # set default constants
@@ -1361,122 +1447,168 @@
         # Copy license-file
         self.copy_licence_file(common_tasks_scripts_file)
 
         # Generate diff-report
         self.generate_diff_report(repository_folder, codeunit_name, codeunit_version)
 
     @GeneralUtilities.check_arguments
-    def generate_diff_report(self, repository_folder: str, codeunit_name: str, current_version: str):
+    def generate_diff_report(self, repository_folder: str, codeunit_name: str, current_version: str) -> None:
         codeunit_folder = os.path.join(repository_folder, codeunit_name)
         target_folder = GeneralUtilities.resolve_relative_path("Other/Artifacts/DiffReport", codeunit_folder)
         GeneralUtilities.ensure_directory_does_not_exist(target_folder)
         GeneralUtilities.ensure_directory_exists(target_folder)
         target_file = os.path.join(target_folder, "DiffReport.html").replace("\\", "/")
         src = "4b825dc642cb6eb9a060e54bf8d69288fbee4904"  # hash/id of empty git-tree
         src_prefix = "Begin"
-        if self.__sc.get_current_branch_has_tag(repository_folder):
-            latest_tag = self.__sc.get_latest_tag(repository_folder)
+        if self.__sc.get_current_git_branch_has_tag(repository_folder):
+            latest_tag = self.__sc.get_latest_git_tag(repository_folder)
             src = self.__sc.git_get_commitid_of_tag(repository_folder, latest_tag)
             src_prefix = latest_tag
         dst = "HEAD"
         dst_prefix = f"v{current_version}"
-        self.__sc.run_program_argsasarray(
-            "sh", ['-c', f'git diff --src-prefix={src_prefix}/ --dst-prefix={dst_prefix}/ {src} {dst} -- {codeunit_name} | ' +
-                   f'pygmentize -l diff -f html -O full -o {target_file} -P style=github-dark'], repository_folder)
+        self.__sc.run_program_argsasarray("sh", ['-c', f'git diff --src-prefix={src_prefix}/ --dst-prefix={dst_prefix}/ {src} {dst} -- {codeunit_name} | pygmentize -l diff -f html -O full -o {target_file} -P style=github-dark'], repository_folder)
 
     @GeneralUtilities.check_arguments
-    def get_version_of_project(self, repository_folder: str):
+    def get_version_of_project(self, repository_folder: str) -> str:
         return ScriptCollectionCore().get_semver_version_from_gitversion(repository_folder)
 
     @GeneralUtilities.check_arguments
-    def replace_common_variables_in_nuspec_file(self, codeunit_folder: str):
+    def replace_common_variables_in_nuspec_file(self, codeunit_folder: str) -> None:
         codeunit_name = os.path.basename(codeunit_folder)
         codeunit_version = self.get_version_of_codeunit_folder(codeunit_folder)
         nuspec_file = os.path.join(codeunit_folder, "Other", "Build", f"{codeunit_name}.nuspec")
         self.__sc.replace_version_in_nuspec_file(nuspec_file, codeunit_version)
 
     @GeneralUtilities.check_arguments
-    def standardized_tasks_build_for_angular_codeunit(self, build_script_file: str, build_environment_target_type: str,
-                                                      verbosity: int, commandline_arguments: list[str]):
-        self.copy_source_files_to_output_directory(build_script_file)
+    def standardized_tasks_build_for_angular_codeunit(self, build_script_file: str, build_environment_target_type: str, verbosity: int, commandline_arguments: list[str]) -> None:
         verbosity = TasksForCommonProjectStructure.get_verbosity_from_commandline_arguments(commandline_arguments, verbosity)
         build_script_folder = os.path.dirname(build_script_file)
         codeunit_folder = GeneralUtilities.resolve_relative_path("../..", build_script_folder)
         self.run_with_epew("ng", f"build --configuration {build_environment_target_type}", codeunit_folder, verbosity=verbosity)
         self.standardized_tasks_build_bom_for_node_project(codeunit_folder, verbosity, commandline_arguments)
+        self.copy_source_files_to_output_directory(build_script_file)
 
     @GeneralUtilities.check_arguments
-    def standardized_tasks_build_bom_for_node_project(self, codeunit_folder: str, verbosity: int, commandline_arguments: list[str]):
+    def standardized_tasks_build_bom_for_node_project(self, codeunit_folder: str, verbosity: int, commandline_arguments: list[str]) -> None:
         verbosity = TasksForCommonProjectStructure.get_verbosity_from_commandline_arguments(commandline_arguments, verbosity)
         # TODO
 
     @GeneralUtilities.check_arguments
     def standardized_tasks_linting_for_angular_codeunit(self, linting_script_file: str, verbosity: int,
-                                                        build_environment_target_type: str, commandline_arguments: list[str]):
+                                                        build_environment_target_type: str, commandline_arguments: list[str]) -> None:
         verbosity = TasksForCommonProjectStructure.get_verbosity_from_commandline_arguments(commandline_arguments, verbosity)
         build_script_folder = os.path.dirname(linting_script_file)
         codeunit_folder = GeneralUtilities.resolve_relative_path("../..", build_script_folder)
         self.run_with_epew("ng", "lint", codeunit_folder, verbosity=verbosity)
         # TODO check if there are errors in sarif-file
 
     @GeneralUtilities.check_arguments
-    def standardized_tasks_run_testcases_for_angular_codeunit(self, runtestcases_script_file: str,
-                                                              build_environment_target_type: str, generate_badges: bool, verbosity: int,
-                                                              commandline_arguments: list[str]):
+    def standardized_tasks_run_testcases_for_flutter_project_in_common_project_structure(self, script_file: str, verbosity: int, args: list[str], package_name: str, build_environment_target_type: str, generate_badges: bool):
+        codeunit_folder = GeneralUtilities.resolve_relative_path("../../..", script_file)
+        repository_folder = GeneralUtilities.resolve_relative_path("..", codeunit_folder)
+        codeunit_name = os.path.basename(codeunit_folder)
+        src_folder = GeneralUtilities.resolve_relative_path(package_name, codeunit_folder)
+        verbosity = self.get_verbosity_from_commandline_arguments(args, verbosity)
+        sc = ScriptCollectionCore()
+        sc.program_runner = ProgramRunnerEpew()
+        sc.run_program("flutter", "test --coverage", src_folder, verbosity)
+        test_coverage_folder_relative = "Other/Artifacts/TestCoverage"
+        test_coverage_folder = GeneralUtilities.resolve_relative_path(test_coverage_folder_relative, codeunit_folder)
+        GeneralUtilities.ensure_directory_exists(test_coverage_folder)
+        coverage_file_relative = f"{test_coverage_folder_relative}/TestCoverage.xml"
+        coverage_file = GeneralUtilities.resolve_relative_path(coverage_file_relative, codeunit_folder)
+        sc.run_program("lcov_cobertura", f"coverage/lcov.info --base-dir . --excludes test --output ../{coverage_file_relative} --demangle", src_folder, verbosity)
+        content = GeneralUtilities.read_text_from_file(coverage_file)
+        content = re.sub('<![^<]+>', '', content)
+        content = re.sub('\\\\', '/', content)
+        content = re.sub('\\ name=\\"lib\\"', '', content)
+        content = re.sub('<package ', f'<package name="{codeunit_name}" ', content)
+        content = re.sub('\\ filename=\\"lib/', f' filename="{package_name}/lib/', content)
+        GeneralUtilities.write_text_to_file(coverage_file, content)
+        self.run_testcases_common_post_task(repository_folder, codeunit_name, verbosity, generate_badges, build_environment_target_type, args)
+
+    @GeneralUtilities.check_arguments
+    def standardized_tasks_run_testcases_for_angular_codeunit(self, runtestcases_script_file: str, build_environment_target_type: str, generate_badges: bool, verbosity: int, commandline_arguments: list[str]) -> None:
         codeunit_name: str = os.path.basename(str(Path(os.path.dirname(runtestcases_script_file)).parent.parent.absolute()))
         verbosity = TasksForCommonProjectStructure.get_verbosity_from_commandline_arguments(commandline_arguments, verbosity)
         codeunit_folder = GeneralUtilities.resolve_relative_path("../..", os.path.dirname(runtestcases_script_file))
+        repository_folder = os.path.dirname(codeunit_folder)
         self.run_with_epew(
             "ng", "test --watch=false --browsers ChromeHeadless --code-coverage", codeunit_folder, verbosity=verbosity)
         coverage_folder = os.path.join(codeunit_folder, "Other", "Artifacts", "TestCoverage")
         target_file = os.path.join(coverage_folder, "TestCoverage.xml")
         GeneralUtilities.ensure_file_does_not_exist(target_file)
         os.rename(os.path.join(coverage_folder, "cobertura-coverage.xml"), target_file)
-        repository_folder = GeneralUtilities.resolve_relative_path("..", codeunit_folder)
+        self.__rename_packagename_in_coverage_file(target_file, codeunit_name)
+        content = GeneralUtilities.read_text_from_file(target_file)
+        content = re.sub('\\\\', '/', content)
         self.run_testcases_common_post_task(repository_folder, codeunit_name, verbosity, generate_badges, build_environment_target_type, commandline_arguments)
 
     @GeneralUtilities.check_arguments
-    def do_npm_install(self, package_json_folder: str, verbosity: int):
+    def __rename_packagename_in_coverage_file(self, file: str, codeunit_name: str) -> None:
+        root: etree._ElementTree = etree.parse(file)
+        packages = root.xpath('//coverage/packages/package')
+        for package in packages:
+            package.attrib['name'] = codeunit_name
+        result = etree.tostring(root).decode("utf-8")
+        GeneralUtilities.write_text_to_file(file, result)
+
+    @GeneralUtilities.check_arguments
+    def do_npm_install(self, package_json_folder: str, verbosity: int) -> None:
         self.run_with_epew("npm", "install", package_json_folder, verbosity=verbosity)
 
     @GeneralUtilities.check_arguments
-    def run_with_epew(self, program: str, argument: str, working_directory: str, verbosity: int):
+    def run_with_epew(self, program: str, argument: str, working_directory: str, verbosity: int) -> None:
         sc: ScriptCollectionCore = ScriptCollectionCore()
         sc.program_runner = ProgramRunnerEpew()
         sc.run_program(program, argument, working_directory, verbosity=verbosity)
 
     @GeneralUtilities.check_arguments
-    def set_default_constants(self, codeunit_folder: str):
+    def set_default_constants(self, codeunit_folder: str) -> None:
         self.set_constant_for_commitid(codeunit_folder)
         self.set_constant_for_commitdate(codeunit_folder)
         self.set_constant_for_commitname(codeunit_folder)
-        self.set_constant_for_commitversion(codeunit_folder)
+        self.set_constant_for_codeunitversion(codeunit_folder)
+        self.set_constant_for_codeunitmajorversion(codeunit_folder)
+        self.set_constant_for_description(codeunit_folder)
 
     @GeneralUtilities.check_arguments
-    def set_constant_for_commitid(self, codeunit_folder: str):
+    def set_constant_for_commitid(self, codeunit_folder: str) -> None:
         commit_id = self.__sc.git_get_commit_id(codeunit_folder)
         self.set_constant(codeunit_folder, "CommitId", commit_id)
 
     @GeneralUtilities.check_arguments
-    def set_constant_for_commitdate(self, codeunit_folder: str):
+    def set_constant_for_commitdate(self, codeunit_folder: str) -> None:
         commit_date: datetime = self.__sc.git_get_commit_date(codeunit_folder)
         self.set_constant(codeunit_folder, "CommitDate", GeneralUtilities.datetime_to_string(commit_date))
 
     @GeneralUtilities.check_arguments
-    def set_constant_for_commitname(self, codeunit_folder: str):
+    def set_constant_for_commitname(self, codeunit_folder: str) -> None:
         codeunit_name: str = os.path.basename(codeunit_folder)
         self.set_constant(codeunit_folder, "CodeUnitName", codeunit_name)
 
     @GeneralUtilities.check_arguments
-    def set_constant_for_commitversion(self, codeunit_folder: str):
+    def set_constant_for_codeunitversion(self, codeunit_folder: str) -> None:
         codeunit_version: str = self.get_version_of_codeunit_folder(codeunit_folder)
         self.set_constant(codeunit_folder, "CodeUnitVersion", codeunit_version)
 
     @GeneralUtilities.check_arguments
-    def set_constant(self, codeunit_folder: str, constantname: str, constant_value: str, documentationsummary: str = None, constants_valuefile: str = None):
+    def set_constant_for_codeunitmajorversion(self, codeunit_folder: str) -> None:
+        codeunit_version: str = self.get_version_of_codeunit_folder(codeunit_folder)
+        major_version = int(codeunit_version.split(".")[0])
+        self.set_constant(codeunit_folder, "CodeUnitMajorVersion", str(major_version))
+
+    @GeneralUtilities.check_arguments
+    def set_constant_for_description(self, codeunit_folder: str) -> None:
+        codeunit_name: str = os.path.basename(codeunit_folder)
+        codeunit_description: str = self.get_codeunit_description(f"{codeunit_folder}/{codeunit_name}.codeunit.xml")
+        self.set_constant(codeunit_folder, "CodeUnitDescription", codeunit_description)
+
+    @GeneralUtilities.check_arguments
+    def set_constant(self, codeunit_folder: str, constantname: str, constant_value: str, documentationsummary: str = None, constants_valuefile: str = None) -> None:
         if documentationsummary is None:
             documentationsummary = ""
         constants_folder = os.path.join(codeunit_folder, "Other", "Resources", "Constants")
         GeneralUtilities.ensure_directory_exists(constants_folder)
         constants_metafile = os.path.join(constants_folder, f"{constantname}.constant.xml")
         if constants_valuefile is None:
             constants_valuefile_folder = constants_folder
@@ -1519,91 +1651,104 @@
             return ""
         elif length == 1:
             return results[0]
         else:
             raise ValueError("Too many results found.")
 
     @GeneralUtilities.check_arguments
-    def set_constants_for_certificate_public_information(self, codeunit_folder: str, source_constant_name: str = "DevelopmentCertificate", domain: str = None):
+    def copy_development_certificate_to_default_development_directory(self, codeunit_folder: str, build_environment: str, domain: str = None,                                                                      certificate_resource_name: str = "DevelopmentCertificate") -> None:
+        if build_environment == "Development":
+            codeunit_name: str = os.path.basename(codeunit_folder)
+            if domain is None:
+                domain = f"{codeunit_name}.test.local".lower()
+
+            src_folder = os.path.join(codeunit_folder, "Other", "Resources", certificate_resource_name)
+            src_file_pfx = os.path.join(src_folder, f"{codeunit_name}{certificate_resource_name}.pfx")
+            src_file_psw = os.path.join(src_folder, f"{codeunit_name}{certificate_resource_name}.password")
+
+            trg_folder = os.path.join(codeunit_folder, "Other", "Workspace", "Configuration", "Certificates")
+            trg_file_pfx = os.path.join(trg_folder, f"{domain}.pfx")
+            trg_file_psw = os.path.join(trg_folder, f"{domain}.password")
+
+            GeneralUtilities.ensure_directory_exists(trg_folder)
+            shutil.copyfile(src_file_pfx, trg_file_pfx)
+            shutil.copyfile(src_file_psw, trg_file_psw)
+
+    @GeneralUtilities.check_arguments
+    def set_constants_for_certificate_public_information(self, codeunit_folder: str, source_constant_name: str = "DevelopmentCertificate", domain: str = None) -> None:
         """Expects a certificate-resource and generates a constant for its public information"""
-        codeunit_name = os.path.basename(codeunit_folder)
-        if domain is None:
-            domain = f"{codeunit_name}.test.local"
-        domain = domain.lower()
-        certificate_file = os.path.join(codeunit_folder, "Other", "Resources", source_constant_name, f"{domain}.crt")
+        # codeunit_name = os.path.basename(codeunit_folder)
+        certificate_file = os.path.join(codeunit_folder, "Other", "Resources", source_constant_name, f"{source_constant_name}.crt")
         with open(certificate_file, encoding="utf-8") as text_wrapper:
             certificate = crypto.load_certificate(crypto.FILETYPE_PEM, text_wrapper.read())
         certificate_publickey = crypto.dump_publickey(crypto.FILETYPE_PEM, certificate.get_pubkey()).decode("utf-8")
         self.set_constant(codeunit_folder, source_constant_name+"PublicKey", certificate_publickey)
 
     @GeneralUtilities.check_arguments
-    def set_constants_for_certificate_private_information(self, codeunit_folder: str, certificate_resource_name: str = "DevelopmentCertificate", domain: str = None):
+    def set_constants_for_certificate_private_information(self, codeunit_folder: str) -> None:
         """Expects a certificate-resource and generates a constant for its sensitive information in hex-format"""
         codeunit_name = os.path.basename(codeunit_folder)
-        if domain is None:
-            domain = f"{codeunit_name}.test.local"
-        domain = domain.lower()
-        self.generate_constant_from_resource_by_filename(codeunit_folder, certificate_resource_name, f"{domain}.test.local.pfx", "PFX")
-        self.generate_constant_from_resource_by_filename(codeunit_folder, certificate_resource_name, f"{domain}.test.local.password", "Password")
+        resource_name: str = "DevelopmentCertificate"
+        filename: str = codeunit_name+"DevelopmentCertificate"
+        self.generate_constant_from_resource_by_filename(codeunit_folder, resource_name, f"{filename}.pfx", "PFX")
+        self.generate_constant_from_resource_by_filename(codeunit_folder, resource_name, f"{filename}.password", "Password")
 
     @GeneralUtilities.check_arguments
-    def generate_constant_from_resource_by_filename(self, codeunit_folder: str, resource_name: str, filename: str, constant_name: str):
+    def generate_constant_from_resource_by_filename(self, codeunit_folder: str, resource_name: str, filename: str, constant_name: str) -> None:
         certificate_resource_folder = GeneralUtilities.resolve_relative_path(f"Other/Resources/{resource_name}", codeunit_folder)
         resource_file = os.path.join(certificate_resource_folder, filename)
         resource_file_content = GeneralUtilities.read_binary_from_file(resource_file)
         resource_file_as_hex = resource_file_content.hex()
         self.set_constant(codeunit_folder, f"{resource_name}{constant_name}Hex", resource_file_as_hex)
 
     @GeneralUtilities.check_arguments
-    def generate_constant_from_resource_by_extension(self, codeunit_folder: str, resource_name: str, extension: str, constant_name: str):
+    def generate_constant_from_resource_by_extension(self, codeunit_folder: str, resource_name: str, extension: str, constant_name: str) -> None:
         certificate_resource_folder = GeneralUtilities.resolve_relative_path(f"Other/Resources/{resource_name}", codeunit_folder)
         resource_file = self.__sc.find_file_by_extension(certificate_resource_folder, extension)
         resource_file_content = GeneralUtilities.read_binary_from_file(resource_file)
         resource_file_as_hex = resource_file_content.hex()
         self.set_constant(codeunit_folder, f"{resource_name}{constant_name}Hex", resource_file_as_hex)
 
     @GeneralUtilities.check_arguments
-    def copy_constant_from_dependent_codeunit(self, codeunit_folder: str, constant_name: str, source_codeunit_name: str):
+    def copy_constant_from_dependent_codeunit(self, codeunit_folder: str, constant_name: str, source_codeunit_name: str) -> None:
         source_codeunit_folder: str = GeneralUtilities.resolve_relative_path(f"../{source_codeunit_name}", codeunit_folder)
         value = self.get_constant_value(source_codeunit_folder, constant_name)
         documentation = self.get_constant_documentation(source_codeunit_folder, constant_name)
         self.set_constant(codeunit_folder, constant_name, value, documentation)
 
     @GeneralUtilities.check_arguments
-    def copy_resources_from_dependent_codeunit(self, codeunit_folder: str, resource_name: str, source_codeunit_name: str):
+    def copy_resources_from_dependent_codeunit(self, codeunit_folder: str, resource_name: str, source_codeunit_name: str) -> None:
         source_folder: str = GeneralUtilities.resolve_relative_path(f"../{source_codeunit_name}/Other/Resources/{resource_name}", codeunit_folder)
         target_folder: str = GeneralUtilities.resolve_relative_path(f"Other/Resources/{resource_name}", codeunit_folder)
         GeneralUtilities.ensure_directory_does_not_exist(target_folder)
         shutil.copytree(source_folder, target_folder)
 
     @GeneralUtilities.check_arguments
-    def generate_openapi_file(self, buildscript_file: str, runtime: str, verbosity: int, commandline_arguments: list[str],
-                              swagger_document_name: str = "APISpecification") -> None:
+    def generate_openapi_file(self, buildscript_file: str, runtime: str, verbosity: int, commandline_arguments: list[str], swagger_document_name: str = "APISpecification") -> None:
         codeunitname = os.path.basename(str(Path(os.path.dirname(buildscript_file)).parent.parent.absolute()))
         repository_folder = str(Path(os.path.dirname(buildscript_file)).parent.parent.parent.absolute())
         artifacts_folder = os.path.join(repository_folder, codeunitname, "Other", "Artifacts")
         GeneralUtilities.ensure_directory_exists(os.path.join(artifacts_folder, "APISpecification"))
         verbosity = self.get_verbosity_from_commandline_arguments(commandline_arguments, verbosity)
         codeunit_version = self.get_version_of_codeunit_folder(os.path.join(repository_folder, codeunitname))
         self.__sc.run_program("swagger", f"tofile --output APISpecification\\{codeunitname}.v{codeunit_version}.api.json" +
                               f" BuildResult_DotNet_{runtime}\\{codeunitname}.dll {swagger_document_name}",
                               artifacts_folder, verbosity=verbosity)
 
     @GeneralUtilities.check_arguments
-    def replace_version_in_packagejson_file(self, packagejson_file: str, codeunit_version: str):
+    def replace_version_in_packagejson_file(self, packagejson_file: str, codeunit_version: str) -> None:
         encoding = "utf-8"
         with open(packagejson_file, encoding=encoding) as f:
             data = json.load(f)
         data['version'] = codeunit_version
         with open(packagejson_file, 'w', encoding=encoding) as f:
             json.dump(data, f, indent=2)
 
     @GeneralUtilities.check_arguments
-    def build_dependent_code_units(self, repo_folder: str, codeunit_name: str, verbosity: int, target_environmenttype: str,
-                                   additional_arguments_file: str) -> None:
+    def build_dependent_code_units(self, repo_folder: str, codeunit_name: str, verbosity: int, target_environmenttype: str, additional_arguments_file: str) -> None:
         codeunit_file = os.path.join(repo_folder, codeunit_name, codeunit_name + ".codeunit.xml")
         dependent_codeunits = self.get_dependent_code_units(codeunit_file)
         dependent_codeunits_folder = os.path.join(repo_folder, codeunit_name, "Other", "Resources", "DependentCodeUnits")
         GeneralUtilities.ensure_directory_does_not_exist(dependent_codeunits_folder)
         if 0 < len(dependent_codeunits):
             GeneralUtilities.write_message_to_stdout(f"Start building dependent codeunits for codeunit {codeunit_name}.")
         for dependent_codeunit in dependent_codeunits:
@@ -1623,136 +1768,197 @@
             target_folder = os.path.join(dependent_codeunits_folder, dependent_codeunit)
             GeneralUtilities.ensure_directory_does_not_exist(target_folder)
             other_folder = os.path.join(repo_folder, dependent_codeunit, "Other")
             artifacts_folder = os.path.join(other_folder, "Artifacts")
             shutil.copytree(artifacts_folder, target_folder)
 
     @GeneralUtilities.check_arguments
-    def add_github_release(self, productname: str, projectversion: str, build_artifacts_folder: str, github_username: str, repository_folder: str,
-                           verbosity: int, commandline_arguments: list[str]):
-        verbosity = TasksForCommonProjectStructure.get_verbosity_from_commandline_arguments(commandline_arguments, verbosity)
+    def add_github_release(self, productname: str, projectversion: str, build_artifacts_folder: str, github_username: str, repository_folder: str, commandline_arguments: list[str]) -> None:
+        verbosity = TasksForCommonProjectStructure.get_verbosity_from_commandline_arguments(commandline_arguments, 1)
         github_repo = f"{github_username}/{productname}"
         artifact_files = []
         codeunits = self.get_codeunits(repository_folder)
         for codeunit in codeunits:
             artifact_files.append(self.__sc.find_file_by_extension(f"{build_artifacts_folder}\\{productname}\\{projectversion}\\{codeunit}", "Productive.Artifacts.zip"))
         changelog_file = os.path.join(repository_folder, "Other", "Resources", "Changelog", f"v{projectversion}.md")
         self.__sc.run_program_argsasarray("gh", ["release", "create", f"v{projectversion}", "--repo",  github_repo,  "--notes-file", changelog_file,
                                                  "--title", f"Release v{projectversion}"]+artifact_files, verbosity=verbosity)
 
     @GeneralUtilities.check_arguments
-    def update_dependencies_of_typical_python_codeunit(self, update_script_file: str, verbosity: int, cmd_args: list[str]):
-        # TODO generalize and add option to ignore certain dependencies
+    def update_dependencies_of_typical_flutter_codeunit(self, update_script_file: str, verbosity: int, cmd_args: list[str]) -> None:
+        pass  # TODO
+
+    @GeneralUtilities.check_arguments
+    def update_dependencies_of_typical_python_codeunit(self, update_script_file: str, verbosity: int, cmd_args: list[str]) -> None:
+        # TODO generalize and add option to ignore certain dependencies and to only update patch-versions
         verbosity = self.get_verbosity_from_commandline_arguments(cmd_args, verbosity)
         codeunit_folder = GeneralUtilities.resolve_relative_path("..", os.path.dirname(update_script_file))
         self.__sc.update_dependencies_of_python_in_setupcfg_file(os.path.join(codeunit_folder, "setup.cfg"), verbosity)
         development_requirements_file = os.path.join(codeunit_folder, "requirements.txt")
         if (os.path.isfile(development_requirements_file)):
             self.__sc.update_dependencies_of_python_in_requirementstxt_file(development_requirements_file, verbosity)
 
     @GeneralUtilities.check_arguments
-    def update_dependencies_of_typical_dotnet_codeunit(self, update_script_file: str, verbosity: int, cmd_args: list[str]):
+    def update_dependencies_of_typical_dotnet_codeunit(self, update_script_file: str, verbosity: int, cmd_args: list[str]) -> None:
         # TODO generalize and add option to ignore certain dependencies
         verbosity = self.get_verbosity_from_commandline_arguments(cmd_args, verbosity)
         codeunit_folder = GeneralUtilities.resolve_relative_path("..", os.path.dirname(update_script_file))
         codeunit_name = os.path.basename(codeunit_folder)
+
+        build_folder = os.path.join(codeunit_folder, "Other", "Build")
+        self.__sc.run_program("python", "Build.py", build_folder, verbosity)
+
         csproj_file = os.path.join(codeunit_folder, codeunit_name, f"{codeunit_name}.csproj")
         self.__sc.update_dependencies_of_dotnet_project(csproj_file, verbosity)
         test_csproj_file = os.path.join(codeunit_folder, f"{codeunit_name}Tests", f"{codeunit_name}Tests.csproj")
         self.__sc.update_dependencies_of_dotnet_project(test_csproj_file, verbosity)
 
     @GeneralUtilities.check_arguments
-    def update_dependencies_of_typical_node_codeunit(self, update_script_file: str, verbosity: int, cmd_args: list[str]):
+    def update_dependencies_of_typical_node_codeunit(self, update_script_file: str, verbosity: int, cmd_args: list[str]) -> None:
         pass  # TODO generalize and add option to ignore certain dependencies
 
     @GeneralUtilities.check_arguments
-    def standardized_tasks_update_version_in_docker_examples(self, file, codeunit_version):
+    def run_local_test_service(self, file: str):
+        example_folder = os.path.dirname(file)
+        example_name = os.path.basename(example_folder)
+        title = f"Test{example_name}"
+        self.__sc.run_program("docker", f"compose -p {title.lower()} up", example_folder, title=title)
+
+    @GeneralUtilities.check_arguments
+    def standardized_tasks_update_version_in_docker_examples(self, file, codeunit_version) -> None:
         folder_of_current_file = os.path.dirname(file)
         codeunit_folder = GeneralUtilities.resolve_relative_path("..", folder_of_current_file)
         codeunit_name = os.path.basename(codeunit_folder)
         codeunit_name_lower = codeunit_name.lower()
         examples_folder = GeneralUtilities.resolve_relative_path("Other/Reference/ReferenceContent/Examples", codeunit_folder)
         for example_folder in GeneralUtilities.get_direct_folders_of_folder(examples_folder):
             docker_compose_file = os.path.join(example_folder, "docker-compose.yml")
             if os.path.isfile(docker_compose_file):
                 filecontent = GeneralUtilities.read_text_from_file(docker_compose_file)
                 replaced = re.sub(f'image:\\s+{codeunit_name_lower}:\\d+\\.\\d+\\.\\d+', f"image: {codeunit_name_lower}:{codeunit_version}", filecontent)
                 GeneralUtilities.write_text_to_file(docker_compose_file, replaced)
 
     @GeneralUtilities.check_arguments
-    def run_dockerfile_example(self, current_file: str, verbosity: int, remove_old_container: bool, remove_volumes_folder: bool, commandline_arguments: list[str]):
+    def run_dockerfile_example(self, current_file: str, verbosity: int, remove_old_container: bool, remove_volumes_folder: bool, commandline_arguments: list[str]) -> None:
         verbosity = TasksForCommonProjectStructure.get_verbosity_from_commandline_arguments(commandline_arguments, verbosity)
         folder = os.path.dirname(current_file)
         example_name = os.path.basename(folder)
         GeneralUtilities.write_message_to_stdout(f'Run "{example_name}"-example')
         sc = ScriptCollectionCore()
         oci_image_artifacts_folder = GeneralUtilities.resolve_relative_path("../../../../Artifacts/BuildResult_OCIImage", folder)
         image_filename = os.path.basename(sc.find_file_by_extension(oci_image_artifacts_folder, "tar"))
         codeunit_name = os.path.basename(GeneralUtilities.resolve_relative_path("../../../../..", folder))
-        codeunit_name_lower = codeunit_name.lower()
         if remove_old_container:
-            GeneralUtilities.write_message_to_stdout(f"Ensure container {codeunit_name_lower} does not exist...")
-            sc.run_program("docker", f"container rm -f {codeunit_name_lower}", oci_image_artifacts_folder, verbosity=verbosity)
+            docker_compose_file = f"{folder}/docker-compose.yml"
+            container_names = []
+            lines = GeneralUtilities.read_lines_from_file(docker_compose_file)
+            for line in lines:
+                if match := re.search("container_name:\\s*'?([^']+)'?", line):
+                    container_names.append(match.group(1))
+            GeneralUtilities.write_message_to_stdout(f"Ensure container of {docker_compose_file} do not exist...")
+            for container_name in container_names:
+                GeneralUtilities.write_message_to_stdout(f"Ensure container of {container_name} does not exist")
+                sc.run_program("docker", f"container rm -f {container_name}", oci_image_artifacts_folder, verbosity=0, throw_exception_if_exitcode_is_not_zero=False)
         if remove_volumes_folder:
             volumes_folder = os.path.join(folder, "Volumes")
             GeneralUtilities.write_message_to_stdout(f"Ensure volumes-folder '{volumes_folder}' does not exist...")
             GeneralUtilities.ensure_directory_does_not_exist(volumes_folder)
             GeneralUtilities.ensure_directory_exists(volumes_folder)
         GeneralUtilities.write_message_to_stdout("Load docker-image...")
         sc.run_program("docker", f"load -i {image_filename}", oci_image_artifacts_folder, verbosity=verbosity)
-        project_name = f"{codeunit_name}_{example_name}".lower()
+        docker_project_name = f"{codeunit_name}_{example_name}".lower()
         sc_epew = ScriptCollectionCore()
         sc_epew.program_runner = ProgramRunnerEpew()
         GeneralUtilities.write_message_to_stdout("Start docker-container...")
-        sc_epew.run_program("docker-compose", f"--project-name {project_name} up", folder, verbosity=verbosity)
+        sc_epew.run_program("docker", f"compose --project-name {docker_project_name} up --abort-on-container-exit", folder, verbosity=verbosity)
+
+    @GeneralUtilities.check_arguments
+    def create_artifact_for_development_certificate(self, codeunit_folder: str):
+        ce_source_folder = GeneralUtilities.resolve_relative_path("Other/Resources/DevelopmentCertificate", codeunit_folder)
+        ca_source_folder = GeneralUtilities.resolve_relative_path("Other/Resources/DevelopmentCertificateAuthority", codeunit_folder)
+        ce_target_folder = GeneralUtilities.resolve_relative_path("Other/Artifacts/DevelopmentCertificate", codeunit_folder)
+        ca_target_folder = GeneralUtilities.resolve_relative_path("Other/Artifacts/DevelopmentCertificateAuthority", codeunit_folder)
+
+        GeneralUtilities.ensure_directory_exists(ce_target_folder)
+        GeneralUtilities.copy_content_of_folder(ce_source_folder, ce_target_folder)
+        GeneralUtilities.ensure_directory_exists(ca_target_folder)
+        GeneralUtilities.copy_content_of_folder(ca_source_folder, ca_target_folder)
+
+    @GeneralUtilities.check_arguments
+    def get_sorted_codeunits(self, codeunits=dict[str, set[str]]) -> list[str]:
+        result_typed = list(TopologicalSorter(codeunits).static_order())
+        result = list()
+        for item in result_typed:
+            result.append(str(item))
+        return result
 
     @GeneralUtilities.check_arguments
-    def _internal_sort_codenits(self, codeunits=dict[str, set[str]]) -> list[str]:
-        return list(TopologicalSorter(codeunits).static_order())
+    def get_project_name(self, repository_folder: str) -> str:
+        for file in GeneralUtilities.get_direct_files_of_folder(repository_folder):
+            if file.endswith(".code-workspace"):
+                return Path(file).stem
+        raise ValueError(f'Project-name can not be calculated for repository "{repository_folder}"')
+
+    def __check_target_environmenttype(self, target_environmenttype: str):
+        allowed_values = list(self.get_default_target_environmenttype_mapping().values())
+        if not (target_environmenttype in allowed_values):
+            raise ValueError(f"Invalid target-environmenttype: '{target_environmenttype}'")
 
     @GeneralUtilities.check_arguments
-    def build_codeunit(self, codeunit_folder: str, verbosity: int = 1, target_environmenttype: str = "QualityCheck", additional_arguments_file: str = None,
-                       is_pre_merge: bool = False, export_target_directory: str = None, assume_dependent_codeunits_are_already_built: bool = False) -> None:
+    def build_codeunit(self, codeunit_folder: str, verbosity: int = 1, target_environmenttype: str = "QualityCheck",
+                       additional_arguments_file: str = None, is_pre_merge: bool = False, export_target_directory: str = None,
+                       assume_dependent_codeunits_are_already_built: bool = False) -> None:
         codeunit_folder = GeneralUtilities.resolve_relative_path_from_current_working_directory(codeunit_folder)
         codeunit_name = os.path.basename(codeunit_folder)
         repository_folder = os.path.dirname(codeunit_folder)
         self.build_specific_codeunits(repository_folder, [codeunit_name], verbosity, target_environmenttype, additional_arguments_file,
                                       is_pre_merge, export_target_directory, assume_dependent_codeunits_are_already_built)
 
     @GeneralUtilities.check_arguments
-    def build_codeunits(self, repository_folder: str, verbosity: int = 1, target_environmenttype: str = "QualityCheck", additional_arguments_file: str = None,
-                        is_pre_merge: bool = False, export_target_directory: str = None) -> None:
+    def build_codeunitsC(self, repository_folder: str, image: str, verbosity: int = 1, target_environmenttype: str = "QualityCheck", additional_arguments_file: str = None) -> None:
+        if target_environmenttype == "Development":
+            raise ValueError(f"build_codeunitsC is not available for target_environmenttype {target_environmenttype}.")
+        # TODO handle additional_arguments_file
+        # TODO add option to allow building different codeunits in same project with different images due to their demands
+        # TODO check if image provides all demands of codeunit
+        self.__sc.run_program(
+            "docker", f"run --volume {repository_folder}:/Workspace/Repository " +
+            f"-e repositoryfolder=/Workspace/Repository -e verbosity={verbosity} -e targetenvironment={target_environmenttype} {image}",
+            repository_folder)
+
+    @GeneralUtilities.check_arguments
+    def build_codeunits(self, repository_folder: str, verbosity: int = 1, target_environmenttype: str = "QualityCheck", additional_arguments_file: str = None, is_pre_merge: bool = False, export_target_directory: str = None) -> None:
+        self.__check_target_environmenttype(target_environmenttype)
         repository_folder = GeneralUtilities.resolve_relative_path_from_current_working_directory(repository_folder)
-        codeunits = self.get_codeunits(repository_folder)
+        codeunits = self.get_codeunits(repository_folder, False)
         self.build_specific_codeunits(repository_folder, codeunits, verbosity, target_environmenttype, additional_arguments_file, is_pre_merge, export_target_directory)
 
     @GeneralUtilities.check_arguments
-    def build_specific_codeunits(self, repository_folder: str, codeunits: list[str], verbosity: int = 1, target_environmenttype: str = "QualityCheck",
-                                 additional_arguments_file: str = None, is_pre_merge: bool = False, export_target_directory: str = None,
-                                 assume_dependent_codeunits_are_already_built: bool = True) -> None:
+    def build_specific_codeunits(self, repository_folder: str, codeunits: list[str], verbosity: int = 1, target_environmenttype: str = "QualityCheck",                                 additional_arguments_file: str = None, is_pre_merge: bool = False, export_target_directory: str = None, assume_dependent_codeunits_are_already_built: bool = True) -> None:
+        self.__check_target_environmenttype(target_environmenttype)
         repository_folder = GeneralUtilities.resolve_relative_path_from_current_working_directory(repository_folder)
         contains_uncommitted_changes = self.__sc.git_repository_has_uncommitted_changes(repository_folder)
         if is_pre_merge and contains_uncommitted_changes:
             raise ValueError(f'Repository "{repository_folder}" has uncommitted changes.')
         subfolders = [os.path.join(repository_folder, codeunit) for codeunit in codeunits]
         codeunits_with_dependent_codeunits: dict[str, set[str]] = dict[str, set[str]]()
         for subfolder in subfolders:
             codeunit_name: str = os.path.basename(subfolder)
             codeunit_file = os.path.join(subfolder, f"{codeunit_name}.codeunit.xml")
             if os.path.exists(codeunit_file):
                 codeunits_with_dependent_codeunits[codeunit_name] = self.get_dependent_code_units(codeunit_file)
             else:
                 raise ValueError(f"{repository_folder} does not have a codeunit with name {codeunit_name}.")
-        sorted_codeunits = self._internal_sort_codenits(codeunits_with_dependent_codeunits)
+        sorted_codeunits = self.get_sorted_codeunits(codeunits_with_dependent_codeunits)
         project_version = self.get_version_of_project(repository_folder)
         if len(sorted_codeunits) == 0:
             raise ValueError(f'No codeunit found in subfolders of "{repository_folder}".')
         else:
             if verbosity > 1:
-                GeneralUtilities.write_message_to_stdout("Attempt to build codeunits in the following order:")
+                GeneralUtilities.write_message_to_stdout(f"Attempt to build codeunits for version {project_version} in the following order:")
                 i = 0
                 for codeunit in sorted_codeunits:
                     i = i+1
                     GeneralUtilities.write_message_to_stdout(f"{i}.: {codeunit}")
             self.__do_repository_checks(repository_folder, project_version)
             line = "----------"
             for codeunit in sorted_codeunits:
@@ -1763,54 +1969,80 @@
         if not contains_uncommitted_changes and self.__sc.git_repository_has_uncommitted_changes(repository_folder) and not is_pre_merge:
             message = f'Due to the build-process the repository "{repository_folder}" has new uncommitted changes.'
             if target_environmenttype == "Development":
                 GeneralUtilities.write_message_to_stdout(message)
             else:
                 raise ValueError(message)
         if export_target_directory is not None:
-            project_name = os.path.basename(repository_folder)
+            project_name = self.get_project_name(repository_folder)
             for codeunit in sorted_codeunits:
                 codeunit_version = self.get_version_of_codeunit_folder(os.path.join(repository_folder,  codeunit))
                 artifacts_folder = os.path.join(repository_folder,  codeunit, "Other", "Artifacts")
                 target_folder = os.path.join(export_target_directory, project_name, project_version, codeunit)
                 GeneralUtilities.ensure_directory_does_not_exist(target_folder)
                 GeneralUtilities.ensure_directory_exists(target_folder)
                 filename_without_extension = f"{codeunit}.v{codeunit_version}.{target_environmenttype}.Artifacts"
                 shutil.make_archive(filename_without_extension, 'zip', artifacts_folder)
                 archive_file = os.path.join(os.getcwd(), f"{filename_without_extension}.zip")
                 shutil.move(archive_file, target_folder)
 
     @GeneralUtilities.check_arguments
-    def __do_repository_checks(self, repository_folder: str, project_version: str):
+    def __do_repository_checks(self, repository_folder: str, project_version: str) -> None:
         self.__check_if_changelog_exists(repository_folder, project_version)
         self.__check_whether_security_txt_exists(repository_folder)
+        self.__check_whether_workspace_file_exists(repository_folder)
+        self.__check_for_staged_or_committed_ignored_files(repository_folder)
 
     @GeneralUtilities.check_arguments
-    def __check_whether_security_txt_exists(self, repository_folder: str):
-        security_txt_file_relative = ".well-known/security.txt"
-        security_txt_file = GeneralUtilities.resolve_relative_path(security_txt_file_relative, repository_folder)
-        if not os.path.isfile(security_txt_file):
-            raise ValueError(f"The repository does not contain a '{security_txt_file_relative}'-file. See https://securitytxt.org/ for more information.")
-
-    @GeneralUtilities.check_arguments
-    def __check_if_changelog_exists(self, repository_folder: str, project_version: str):
+    def __check_if_changelog_exists(self, repository_folder: str, project_version: str) -> None:
         changelog_folder = os.path.join(repository_folder, "Other", "Resources", "Changelog")
         changelog_file = os.path.join(changelog_folder, f"v{project_version}.md")
         if not os.path.isfile(changelog_file):
             raise ValueError(f"Changelog-file '{changelog_file}' does not exist.")
 
     @GeneralUtilities.check_arguments
-    def update_dependency_in_resources_folder(self, update_dependencies_file, dependency_name: str, latest_version_function: str):
-        version_file = GeneralUtilities.resolve_relative_path(f"../Resources/Dependencies/{dependency_name}/Version.txt", update_dependencies_file)
-        current_version = GeneralUtilities.read_text_from_file(version_file)
-        if current_version != latest_version_function:
+    def __check_whether_security_txt_exists(self, repository_folder: str) -> None:
+        security_txt_file_relative = ".well-known/security.txt"
+        security_txt_file = GeneralUtilities.resolve_relative_path(security_txt_file_relative, repository_folder)
+        if not os.path.isfile(security_txt_file):
+            raise ValueError(f"The repository does not contain a '{security_txt_file_relative}'-file. See https://securitytxt.org/ for more information.")
+
+    @GeneralUtilities.check_arguments
+    def __check_for_staged_or_committed_ignored_files(self, repository_folder: str) -> None:
+        for file in self.__sc.get_staged_or_committed_git_ignored_files(repository_folder):
+            GeneralUtilities.write_message_to_stderr(f'Warning: Repository contains staged or committed file "{file}" which is git-ignored.')
+
+    @GeneralUtilities.check_arguments
+    def __check_whether_workspace_file_exists(self, repository_folder: str) -> None:
+        count = 0
+        for file in GeneralUtilities.get_direct_files_of_folder(repository_folder):
+            if file.endswith(".code-workspace"):
+                count = count + 1
+        if count != 1:
+            raise ValueError('The repository must contain exactly one ".code-workspace"-file on the top-level.')
+
+    @GeneralUtilities.check_arguments
+    def update_dependency_in_resources_folder(self, update_dependencies_file, dependency_name: str, latest_version_function: str) -> None:
+        dependency_folder = GeneralUtilities.resolve_relative_path(f"../Resources/Dependencies/{dependency_name}", update_dependencies_file)
+        version_file = os.path.join(dependency_folder, "Version.txt")
+        version_file_exists = os.path.isfile(version_file)
+        write_to_file = False
+        if version_file_exists:
+            current_version = GeneralUtilities.read_text_from_file(version_file)
+            if current_version != latest_version_function:
+                write_to_file = True
+        else:
+            GeneralUtilities.ensure_directory_exists(dependency_folder)
+            GeneralUtilities.ensure_file_exists(version_file)
+            write_to_file = True
+        if write_to_file:
             GeneralUtilities.write_text_to_file(version_file, latest_version_function)
 
     @GeneralUtilities.check_arguments
-    def __ensure_grylibrary_is_available(self, codeunit_folder: str):
+    def __ensure_grylibrary_is_available(self, codeunit_folder: str) -> None:
         grylibrary_folder = os.path.join(codeunit_folder, "Other", "Resources", "GRYLibrary")
         grylibrary_dll_file = os.path.join(grylibrary_folder, "BuildResult_DotNet_win-x64", "GRYLibrary.dll")
         internet_connection_is_available = GeneralUtilities.internet_connection_is_available()
         grylibrary_dll_file_exists = os.path.isfile(grylibrary_dll_file)
         if internet_connection_is_available:  # Load/Update GRYLibrary
             grylibrary_latest_codeunit_file = "https://raw.githubusercontent.com/anionDev/GRYLibrary/stable/GRYLibrary/GRYLibrary.codeunit.xml"
             with urllib.request.urlopen(grylibrary_latest_codeunit_file) as url_result:
@@ -1860,47 +2092,54 @@
         else:
             if exe_file_exists:
                 GeneralUtilities.write_message_to_stdout("Warning: Can not check for updates of FFMPEG due to missing internet-connection.")
             else:
                 raise ValueError("Can not download FFMPEG.")
 
     @GeneralUtilities.check_arguments
-    def __ensure_plant_uml_is_available(self, codeunit_folder: str) -> None:
-        plant_uml_folder = os.path.join(codeunit_folder, "Other", "Resources", "PlantUML")
+    def ensure_plantuml_is_available(self, codeunit_folder: str) -> None:
+        self.ensure_file_from_github_assets_is_available(codeunit_folder, "plantuml", "plantuml", "PlantUML", "plantuml.jar", lambda latest_version: "plantuml.jar")
+
+    @GeneralUtilities.check_arguments
+    def ensure_androidappbundletool_is_available(self, codeunit_folder: str) -> None:
+        self.ensure_file_from_github_assets_is_available(codeunit_folder, "google", "bundletool", "AndroidAppBundleTool", "bundletool.jar", lambda latest_version: f"bundletool-all-{latest_version}.jar")
+
+    @GeneralUtilities.check_arguments
+    def ensure_file_from_github_assets_is_available(self, codeunit_folder: str, githubuser: str, githubprojectname: str, resource_name: str, local_filename: str, get_filename_on_github) -> None:
+        resource_folder = os.path.join(codeunit_folder, "Other", "Resources", resource_name)
         internet_connection_is_available = GeneralUtilities.internet_connection_is_available()
-        jar_file = f"{plant_uml_folder}/plantuml.jar"
-        plantuml_jar_file_exists = os.path.isfile(jar_file)
-        if internet_connection_is_available:  # Load/Update PlantUML
-            GeneralUtilities.ensure_directory_does_not_exist(plant_uml_folder)
-            GeneralUtilities.ensure_directory_exists(plant_uml_folder)
-            response = requests.get("https://api.github.com/repos/plantuml/plantuml/releases/latest", timeout=5)
+        file = f"{resource_folder}/{local_filename}"
+        file_exists = os.path.isfile(file)
+        if internet_connection_is_available:  # Load/Update
+            GeneralUtilities.ensure_directory_does_not_exist(resource_folder)
+            GeneralUtilities.ensure_directory_exists(resource_folder)
+            response = requests.get(f"https://api.github.com/repos/{githubuser}/{githubprojectname}/releases/latest", timeout=5)
             latest_version = response.json()["name"]
-            jar_link = f"https://github.com/plantuml/plantuml/releases/download/{latest_version}/plantuml.jar"
-            urllib.request.urlretrieve(jar_link, jar_file)
+            filename_on_github = get_filename_on_github(latest_version)
+            jar_link = f"https://github.com/{githubuser}/{githubprojectname}/releases/download/{latest_version}/{filename_on_github}"
+            urllib.request.urlretrieve(jar_link, file)
         else:
-            if plantuml_jar_file_exists:
-                GeneralUtilities.write_message_to_stdout("Warning: Can not check for updates of PlantUML due to missing internet-connection.")
+            if file_exists:
+                GeneralUtilities.write_message_to_stdout(f"Warning: Can not check for updates of {resource_name} due to missing internet-connection.")
             else:
-                raise ValueError("Can not download PlantUML.")
+                raise ValueError(f"Can not download {resource_name}.")
 
     @GeneralUtilities.check_arguments
     def generate_svg_files_from_plantuml_files(self, codeunit_folder: str) -> None:
-        self.__ensure_plant_uml_is_available(codeunit_folder)
+        self.ensure_plantuml_is_available(codeunit_folder)
         plant_uml_folder = os.path.join(codeunit_folder, "Other", "Resources", "PlantUML")
         files_folder = os.path.join(codeunit_folder, "Other/Reference")
         sc = ScriptCollectionCore()
         for file in GeneralUtilities.get_all_files_of_folder(files_folder):
             if file.endswith(".plantuml"):
                 argument = ['-jar', f'{plant_uml_folder}/plantuml.jar', os.path.basename(file).replace("\\", "/"), '-tsvg']
-                sc.run_program_argsasarray("java", argument, os.path.dirname(file))
+                sc.run_program_argsasarray("java", argument, os.path.dirname(file),verbosity=0)
 
     @GeneralUtilities.check_arguments
-    def load_deb_control_file_content(self, file: str,
-                                      codeunitname: str, codeunitversion: str, installedsize: int,
-                                      maintainername: str, maintaineremail: str, description: str,) -> str:
+    def load_deb_control_file_content(self, file: str, codeunitname: str, codeunitversion: str, installedsize: int, maintainername: str, maintaineremail: str, description: str,) -> str:
         content = GeneralUtilities.read_text_from_file(file)
         content = GeneralUtilities.replace_variable_in_string(content, "codeunitname", codeunitname)
         content = GeneralUtilities.replace_variable_in_string(content, "codeunitversion", codeunitversion)
         content = GeneralUtilities.replace_variable_in_string(content, "installedsize", str(installedsize))
         content = GeneralUtilities.replace_variable_in_string(content, "maintainername", maintainername)
         content = GeneralUtilities.replace_variable_in_string(content, "maintaineremail", maintaineremail)
         content = GeneralUtilities.replace_variable_in_string(content, "description", description)
@@ -1911,28 +2150,52 @@
         size_in_bytes = 0
         for file in GeneralUtilities.get_all_files_of_folder(binary_folder):
             size_in_bytes = size_in_bytes+os.path.getsize(file)
         result = math.ceil(size_in_bytes/1024)
         return result
 
     @GeneralUtilities.check_arguments
-    def create_deb_package_for_artifact(self, codeunit_folder: str,
-                                        maintainername: str, maintaineremail: str, description: str,
-                                        verbosity: int, cmd_arguments: list[str]) -> None:
+    def create_deb_package_for_artifact(self, codeunit_folder: str, maintainername: str, maintaineremail: str, description: str, verbosity: int, cmd_arguments: list[str]) -> None:
         verbosity = self.get_verbosity_from_commandline_arguments(cmd_arguments, verbosity)
         codeunit_name = os.path.basename(codeunit_folder)
         binary_folder = GeneralUtilities.resolve_relative_path("Other/Artifacts/BuildResult_DotNet_linux-x64", codeunit_folder)
         deb_output_folder = GeneralUtilities.resolve_relative_path("Other/Artifacts/BuildResult_Deb", codeunit_folder)
         control_file = GeneralUtilities.resolve_relative_path("Other/Build/DebControlFile.txt", codeunit_folder)
         installedsize = self.calculate_deb_package_size(binary_folder)
-        control_file_content = self.load_deb_control_file_content(control_file, codeunit_name, self.get_version_of_codeunit_folder(codeunit_folder),
-                                                                  installedsize, maintainername, maintaineremail, description)
+        control_file_content = self.load_deb_control_file_content(control_file, codeunit_name, self.get_version_of_codeunit_folder(codeunit_folder),                                                                  installedsize, maintainername, maintaineremail, description)
         self.__sc.create_deb_package(codeunit_name, binary_folder, control_file_content, deb_output_folder, verbosity, 555)
 
     @GeneralUtilities.check_arguments
+    def update_year_in_license_file_in_common_scripts_file(self, common_tasks_scripts_file: str) -> None:
+        self.update_year_in_license_file(GeneralUtilities.resolve_relative_path("../../..", common_tasks_scripts_file))
+
+    @GeneralUtilities.check_arguments
+    def update_year_in_license_file(self, repository_folder: str) -> None:
+        self.__sc.update_year_in_first_line_of_file(os.path.join(repository_folder, "License.txt"))
+
+    @GeneralUtilities.check_arguments
+    def update_year_for_dotnet_codeunit_in_common_scripts_file(self, common_tasks_scripts_file: str) -> None:
+        self.update_year_for_dotnet_codeunit(GeneralUtilities.resolve_relative_path("../..", common_tasks_scripts_file))
+
+    @GeneralUtilities.check_arguments
+    def update_year_for_dotnet_codeunit(self, codeunit_folder: str) -> None:
+        codeunit_name = os.path.basename(codeunit_folder)
+        csproj_file = os.path.join(codeunit_folder, codeunit_name, f"{codeunit_name}.csproj")
+        self.__sc.update_year_in_copyright_tags(csproj_file)
+        csprojtests_file = os.path.join(codeunit_folder, f"{codeunit_name}Tests", f"{codeunit_name}Tests.csproj")
+        self.__sc.update_year_in_copyright_tags(csprojtests_file)
+        nuspec_file = os.path.join(codeunit_folder, "Other", "Build", f"{codeunit_name}.nuspec")
+        if os.path.isfile(nuspec_file):
+            self.__sc.update_year_in_copyright_tags(nuspec_file)
+
+    @GeneralUtilities.check_arguments
+    def repository_has_codeunits(self, repository: str, ignore_disabled_codeunits: bool = True) -> bool:
+        return len(self.get_codeunits(repository, ignore_disabled_codeunits))
+
+    @GeneralUtilities.check_arguments
     def verify_artifact_exists(self, codeunit_folder: str, artifact_name_regexes: dict[str, bool]) -> None:
         codeunit_name: str = os.path.basename(codeunit_folder)
         artifacts_folder = os.path.join(codeunit_folder, "Other/Artifacts")
         existing_artifacts = [os.path.basename(x) for x in GeneralUtilities.get_direct_folders_of_folder(artifacts_folder)]
         for artifact_name_regex, required in artifact_name_regexes.items():
             artifact_exists = False
             for existing_artifact in existing_artifacts:
@@ -1943,22 +2206,27 @@
                 message = f"Codeunit {codeunit_name} does not contain an artifact which matches the name '{artifact_name_regex}'."
                 if required:
                     raise ValueError(message)
                 else:
                     GeneralUtilities.write_message_to_stderr(f"Warning: {message}")
 
     @GeneralUtilities.check_arguments
-    def __build_codeunit(self, codeunit_folder: str, verbosity: int = 1, target_environmenttype: str = "QualityCheck", additional_arguments_file: str = None,
-                         is_pre_merge: bool = False, assume_dependent_codeunits_are_already_built: bool = False) -> None:
+    def __build_codeunit(self, codeunit_folder: str, verbosity: int = 1, target_environmenttype: str = "QualityCheck", additional_arguments_file: str = None, is_pre_merge: bool = False, assume_dependent_codeunits_are_already_built: bool = False) -> None:
         now = datetime.now()
         codeunit_folder = GeneralUtilities.resolve_relative_path_from_current_working_directory(codeunit_folder)
         codeunit_name: str = os.path.basename(codeunit_folder)
         codeunit_file = os.path.join(codeunit_folder, f"{codeunit_name}.codeunit.xml")
+
         if (not os.path.isfile(codeunit_file)):
             raise ValueError(f'"{codeunit_folder}" is no codeunit-folder.')
+
+        if not self.codeunit_is_enabled(codeunit_file):
+            GeneralUtilities.write_message_to_stdout(f"Warning: Codeunit {codeunit_name} is disabled.")
+            return
+
         artifacts_folder = os.path.join(codeunit_folder, "Other", "Artifacts")
         GeneralUtilities.write_message_to_stdout(f"Start building codeunit {codeunit_name}.")
         GeneralUtilities.write_message_to_stdout(f"Build-environmenttype: {target_environmenttype}")
         GeneralUtilities.ensure_directory_does_not_exist(artifacts_folder)
 
         verbosity_for_executed_programs = min(2, verbosity)
 
@@ -1968,24 +2236,24 @@
         reference_folder = os.path.join(other_folder, "Reference")
         additional_arguments_c: str = ""
         additional_arguments_b: str = ""
         additional_arguments_r: str = ""
         additional_arguments_l: str = ""
         additional_arguments_g: str = ""
         additional_arguments_f: str = ""
-        general_argument = f' --overwrite_verbosity={str(verbosity)} --overwrite_targetenvironmenttype={target_environmenttype}'
+        general_argument = f' --overwrite_verbosity {str(verbosity)} --overwrite_targetenvironmenttype {target_environmenttype}'
 
         c_additionalargumentsfile_argument = ""
 
         if is_pre_merge:
-            general_argument = general_argument+" --overwrite_is_pre_merge=true"
+            general_argument = general_argument+" --overwrite_is_pre_merge true"
             GeneralUtilities.write_message_to_stdout("This is a pre-merge-build")
 
         if assume_dependent_codeunits_are_already_built:
-            c_additionalargumentsfile_argument = c_additionalargumentsfile_argument+" --overwrite_assume_dependent_codeunits_are_already_built=true"
+            c_additionalargumentsfile_argument = c_additionalargumentsfile_argument+" --overwrite_assume_dependent_codeunits_are_already_built true"
             diagnostic = False
             if diagnostic:
                 GeneralUtilities.write_message_to_stdout("Assume dependent codeunits are already built")
 
         if additional_arguments_file is not None:
             config = configparser.ConfigParser()
             config.read(additional_arguments_file)
@@ -1998,59 +2266,41 @@
                 additional_arguments_r = " " + config.get(section_name, "ArgumentsForRunTestcases")
             if config.has_option(section_name, "ArgumentsForLinting"):
                 additional_arguments_l = " " + config.get(section_name, "ArgumentsForLinting")
             if config.has_option(section_name, "ArgumentsForGenerateReference"):
                 additional_arguments_g = " " + config.get(section_name, "ArgumentsForGenerateReference")
             if config.has_option(section_name, "ArgumentsForOnFinish"):
                 additional_arguments_f = " " + config.get(section_name, "ArgumentsForOnFinish")
-            c_additionalargumentsfile_argument = f' --overwrite_additionalargumentsfile="{additional_arguments_file}"'
+            c_additionalargumentsfile_argument = f' --overwrite_additionalargumentsfile "{additional_arguments_file}"'
 
         GeneralUtilities.write_message_to_stdout('Run "CommonTasks.py"...')
-        execution_result = self.__sc.run_program("python", f"CommonTasks.py{additional_arguments_c}{general_argument}{c_additionalargumentsfile_argument}",
-                                                 other_folder, verbosity=verbosity_for_executed_programs, throw_exception_if_exitcode_is_not_zero=False)
-        if execution_result[0] != 0:
-            raise ValueError(f"CommonTasks.py resulted in exitcode {execution_result[0]}. StdOut: '{execution_result[1]}' StdOut: '{execution_result[2]}'")
+        self.__sc.run_program("python", f"CommonTasks.py{additional_arguments_c}{general_argument}{c_additionalargumentsfile_argument}", other_folder,                               verbosity=verbosity_for_executed_programs, throw_exception_if_exitcode_is_not_zero=True)
         self.verify_artifact_exists(codeunit_folder, dict[str, bool]({"Changelog": False, "License": True, "DiffReport": True}))
 
         GeneralUtilities.write_message_to_stdout('Run "Build.py"...')
-        execution_result = self.__sc.run_program("python", f"Build.py{additional_arguments_b}{general_argument}",
-                                                 build_folder, verbosity=verbosity_for_executed_programs, throw_exception_if_exitcode_is_not_zero=False)
-        if execution_result[0] != 0:
-            raise ValueError(f"Build.py resulted in exitcode {execution_result[0]}. StdOut: '{execution_result[1]}' StdOut: '{execution_result[2]}'")
+        self.__sc.run_program("python", f"Build.py{additional_arguments_b}{general_argument}", build_folder, verbosity=verbosity_for_executed_programs, throw_exception_if_exitcode_is_not_zero=True)
         self.verify_artifact_exists(codeunit_folder, dict[str, bool]({"BuildResult_.+": True, "BOM": False, "CodeAnalysisResult": False, "SourceCode": True}))
 
         codeunit_hast_testable_sourcecode = self.codeunit_has_testable_sourcecode(codeunit_file)
         if codeunit_hast_testable_sourcecode:
             GeneralUtilities.write_message_to_stdout('Run "RunTestcases.py"...')
-            execution_result = self.__sc.run_program("python", f"RunTestcases.py{additional_arguments_r}{general_argument}",
-                                                     quality_folder, verbosity=verbosity_for_executed_programs, throw_exception_if_exitcode_is_not_zero=False)
-            if execution_result[0] != 0:
-                raise ValueError(f"RunTestcases.py resulted in exitcode {execution_result[0]}. StdOut: '{execution_result[1]}' StdOut: '{execution_result[2]}'")
+            self.__sc.run_program("python", f"RunTestcases.py{additional_arguments_r}{general_argument}", quality_folder, verbosity=verbosity_for_executed_programs, throw_exception_if_exitcode_is_not_zero=True)
             self.verify_artifact_exists(codeunit_folder, dict[str, bool]({"TestCoverage": True, "TestCoverageReport": False}))
 
         GeneralUtilities.write_message_to_stdout('Run "Linting.py"...')
-        execution_result = self.__sc.run_program("python", f"Linting.py{additional_arguments_l}{general_argument}",
-                                                 quality_folder, verbosity=verbosity_for_executed_programs, throw_exception_if_exitcode_is_not_zero=False)
-        if execution_result[0] != 0:
-            raise ValueError(f"Linting.py resulted in exitcode {execution_result[0]}. StdOut: '{execution_result[1]}' StdOut: '{execution_result[2]}'")
+        self.__sc.run_program("python", f"Linting.py{additional_arguments_l}{general_argument}", quality_folder, verbosity=verbosity_for_executed_programs, throw_exception_if_exitcode_is_not_zero=True)
         self.verify_artifact_exists(codeunit_folder, dict[str, bool]())
 
         GeneralUtilities.write_message_to_stdout('Run "GenerateReference.py"...')
-        execution_result = self.__sc.run_program(
-            "python", f"GenerateReference.py{additional_arguments_g}{general_argument}", reference_folder, verbosity=verbosity_for_executed_programs, throw_exception_if_exitcode_is_not_zero=False)
-        if execution_result[0] != 0:
-            raise ValueError(f"GenerateReference.py resulted in exitcode {execution_result[0]}. StdOut: '{execution_result[1]}' StdOut: '{execution_result[2]}'")
+        self.__sc.run_program("python", f"GenerateReference.py{additional_arguments_g}{general_argument}", reference_folder, verbosity=verbosity_for_executed_programs, throw_exception_if_exitcode_is_not_zero=True)
         self.verify_artifact_exists(codeunit_folder, dict[str, bool]({"Reference": True}))
 
         if os.path.isfile(os.path.join(other_folder, "OnBuildingFinished.py")):
             GeneralUtilities.write_message_to_stdout('Run "OnBuildingFinished.py"...')
-            execution_result = self.__sc.run_program(
-                "python", f"OnBuildingFinished.py{additional_arguments_f}{general_argument}", other_folder, verbosity=verbosity_for_executed_programs, throw_exception_if_exitcode_is_not_zero=False)
-            if execution_result[0] != 0:
-                raise ValueError(f"OnBuildingFinished.py resulted in exitcode {execution_result[0]}. StdOut: '{execution_result[1]}' StdOut: '{execution_result[2]}'")
+            self.__sc.run_program("python", f"OnBuildingFinished.py{additional_arguments_f}{general_argument}", other_folder, verbosity=verbosity_for_executed_programs, throw_exception_if_exitcode_is_not_zero=True)
 
         artifactsinformation_file = os.path.join(artifacts_folder, f"{codeunit_name}.artifactsinformation.xml")
         codeunit_version = self.get_version_of_codeunit(codeunit_file)
         GeneralUtilities.ensure_file_exists(artifactsinformation_file)
         artifacts_list = []
         for artifact_folder in GeneralUtilities.get_direct_folders_of_folder(artifacts_folder):
             artifact_name = os.path.basename(artifact_folder)
@@ -2067,7 +2317,132 @@
     <cps:targetenvironmenttype>{target_environmenttype}</cps:targetenvironmenttype>
     <cps:artifacts>
 {artifacts}
     </cps:artifacts>
 </cps:artifactsinformation>""")
         # TODO validate artifactsinformation_file against xsd
         GeneralUtilities.write_message_to_stdout(f"Finished building codeunit {codeunit_name} without errors.")
+
+    @GeneralUtilities.check_arguments
+    def generic_update_dependencies(self, repository_folder: str):
+        codeunits = self.get_codeunits(repository_folder)
+        updated_dependencies = False
+        for codeunit in codeunits:
+            codeunit_file = os.path.join(repository_folder, codeunit, f"{codeunit}.codeunit.xml")
+            codeunit_has_updatable_dependencies = self.codeunit_has_updatable_dependencies(codeunit_file)
+            if codeunit_has_updatable_dependencies:
+                codeunit_folder = os.path.join(repository_folder, codeunit)
+                update_dependencies_script_folder = os.path.join(codeunit_folder, "Other")
+                self.__sc.run_program("python", "UpdateDependencies.py", update_dependencies_script_folder)#TODO set verbosity
+                if self.__sc.git_repository_has_uncommitted_changes(repository_folder):
+                    version_of_project = self.get_version_of_project(repository_folder)
+                    changelog_file = os.path.join(repository_folder, "Other", "Resources", "Changelog", f"v{version_of_project}.md")
+                    if not os.path.isfile(changelog_file):
+                        GeneralUtilities.write_text_to_file(changelog_file, """# Release notes
+
+## Changes
+
+- Updated dependencies.
+""")
+                        GeneralUtilities.write_message_to_stdout(f"Updated dependencies in codeunit {codeunit}.")
+                        updated_dependencies = True
+                else:
+                    GeneralUtilities.write_message_to_stdout(f"There are no dependencies to update in codeunit {codeunit}.")
+        if updated_dependencies:
+            self.__sc.run_program("scbuildcodeunits", "--targetenvironment QualityCheck", repository_folder)#TODO set verbosity
+            self.__sc.git_commit(repository_folder, "Updated dependencies")
+
+    class GenericPrepareNewReleaseArguments:
+        current_file: str
+        product_name: str
+        commandline_arguments: list[str]
+
+        def __init__(self, current_file: str, product_name: str, commandline_arguments: list[str]):
+            self.current_file = current_file
+            self.product_name = product_name
+            self.commandline_arguments = commandline_arguments
+
+    @GeneralUtilities.check_arguments
+    def generic_prepare_new_release(self, generic_prepare_new_release_arguments: GenericPrepareNewReleaseArguments):
+
+        # constants
+        folder_of_this_file = os.path.dirname(generic_prepare_new_release_arguments.current_file)
+        build_repository_folder = GeneralUtilities.resolve_relative_path("../..", folder_of_this_file)
+
+        repository_folder = GeneralUtilities.resolve_relative_path(f"../../Submodules/{generic_prepare_new_release_arguments.product_name}", folder_of_this_file)
+        verbosity: int = TasksForCommonProjectStructure.get_verbosity_from_commandline_arguments(generic_prepare_new_release_arguments.commandline_arguments, 1)
+        merge_source_branch = "other/next-release"
+
+        # prepare
+        self.assert_no_uncommitted_changes(repository_folder)
+        self.__sc.git_checkout(repository_folder, merge_source_branch)
+        self.generic_update_dependencies(repository_folder)
+        self.merge_to_main_branch(repository_folder, merge_source_branch, verbosity=verbosity, fast_forward_source_branch=True)
+        self.__sc.git_commit(build_repository_folder, "Updated submodule due to merge to main-branch.")
+
+    class GenericCreateReleaseArguments():
+        current_file: str
+        product_name: str
+        common_remote_name: str
+        artifacts_target_folder: str
+        commandline_arguments: list[str]
+
+        def __init__(self, current_file: str, product_name: str, common_remote_name: str, artifacts_target_folder: str,commandline_arguments: list[str]):
+            self.current_file = current_file
+            self.product_name = product_name
+            self.common_remote_name = common_remote_name
+            self.artifacts_target_folder = artifacts_target_folder
+            self.commandline_arguments = commandline_arguments
+
+    @GeneralUtilities.check_arguments
+    def generic_create_release(self, generic_create_release_arguments:GenericCreateReleaseArguments) -> str:
+        folder_of_this_file = os.path.dirname(generic_create_release_arguments.current_file)
+        build_repository_folder = GeneralUtilities.resolve_relative_path("../..", folder_of_this_file)
+        repository_folder_name = generic_create_release_arguments.product_name
+        repository_folder = GeneralUtilities.resolve_relative_path(f"../../Submodules/{generic_create_release_arguments.product_name}", folder_of_this_file)
+        additional_arguments_file = os.path.join(folder_of_this_file, "AdditionalArguments.configuration")
+        verbosity: int = TasksForCommonProjectStructure.get_verbosity_from_commandline_arguments(generic_create_release_arguments.commandline_arguments, 1)
+        createReleaseConfiguration: CreateReleaseConfiguration = CreateReleaseConfiguration(
+            generic_create_release_arguments.product_name, generic_create_release_arguments.common_remote_name, generic_create_release_arguments.artifacts_target_folder, folder_of_this_file, verbosity, repository_folder, additional_arguments_file, repository_folder_name)
+        self.__sc.git_commit(build_repository_folder, "Updated submodule")
+
+        # create release
+        new_version = self.merge_to_stable_branch(generic_create_release_arguments.current_file, createReleaseConfiguration)
+        return new_version
+
+    class UpdateHTTPDocumentationArguments:
+        current_file: str
+        product_name: str
+        common_remote_name: str
+        new_project_version: str
+        reference_repository_name: str
+        commandline_arguments: list[str]
+        main_branch_name: str
+
+        def __init__(self, current_file: str, product_name: str, common_remote_name: str, new_project_version: str, reference_repository_name: str, commandline_arguments: list[str]):
+            self.current_file = current_file
+            self.product_name = product_name
+            self.common_remote_name = common_remote_name
+            self.new_project_version = new_project_version
+            self.reference_repository_name = reference_repository_name
+            self.commandline_arguments = commandline_arguments
+            self.main_branch_name = "main"
+
+    @GeneralUtilities.check_arguments
+    def update_http_documentation(self, update_http_documentation_arguments: UpdateHTTPDocumentationArguments):
+        folder_of_this_file = str(os.path.dirname(update_http_documentation_arguments.current_file))
+
+        ref_repo = GeneralUtilities.resolve_relative_path(f"../../Submodules/{update_http_documentation_arguments.reference_repository_name}", folder_of_this_file)
+        self.__sc.git_checkout(ref_repo, update_http_documentation_arguments.main_branch_name)
+
+        # update reference
+        target = os.path.join(ref_repo, "Reference", update_http_documentation_arguments.product_name)
+        GeneralUtilities.ensure_directory_does_not_exist(target)
+        shutil.copytree(GeneralUtilities.resolve_relative_path(f"../../Submodules/{update_http_documentation_arguments.product_name}Reference/ReferenceContent", folder_of_this_file), target)
+        self.__sc.git_commit(ref_repo, f"Added reference of {update_http_documentation_arguments.product_name} v{update_http_documentation_arguments.new_project_version}")
+
+        # Sync reference-repository
+        self.__sc.git_fetch(ref_repo, update_http_documentation_arguments.common_remote_name)
+        self.__sc.git_merge(ref_repo, update_http_documentation_arguments.common_remote_name+"/"+update_http_documentation_arguments.main_branch_name, update_http_documentation_arguments.main_branch_name)
+        self.__sc.git_checkout(ref_repo, update_http_documentation_arguments.main_branch_name)
+        self.__sc.git_push(ref_repo, update_http_documentation_arguments.common_remote_name, update_http_documentation_arguments.main_branch_name, update_http_documentation_arguments.main_branch_name)
+        self.__sc.git_commit(GeneralUtilities.resolve_relative_path("../..", folder_of_this_file), f"Updated content of {update_http_documentation_arguments.product_name} v{update_http_documentation_arguments.new_project_version} in {update_http_documentation_arguments.reference_repository_name}-submodule")
```

## ScriptCollection/UpdateCertificates.py

```diff
@@ -4,27 +4,27 @@
 from shutil import copyfile
 from .ScriptCollectionCore import ScriptCollectionCore
 from .GeneralUtilities import GeneralUtilities
 
 
 class CertificateUpdater:
 
-    __domains: list(str)
+    __domains: list[str]
     __email: str
 
     __current_folder = os.path.dirname(os.path.abspath(__file__))
     __repository_folder = GeneralUtilities.resolve_relative_path(f"..{os.path.sep}..{os.path.sep}..{os.path.sep}", __current_folder)
     __letsencrypt_folder = GeneralUtilities.resolve_relative_path(f"..{os.path.sep}..{os.path.sep}Volumes{os.path.sep}letsencrypt", __current_folder)
     __letsencrypt_live_folder = os.path.join(__letsencrypt_folder, "live")
     __letsencrypt_archive_folder = os.path.join(__letsencrypt_folder, "archive")
     __log_folder = GeneralUtilities.resolve_relative_path(f"Logs{os.path.sep}Overhead", __repository_folder)
     __sc = ScriptCollectionCore()
     __line = "___________________________________________________________________"
 
-    def __init__(self, domains: list(str), email: str):
+    def __init__(self, domains: list[str], email: str):
         self.__domains = domains
         self.__email = email
 
     @GeneralUtilities.check_arguments
     def __get_latest_index_by_domain(self, domain: str) -> int:
         result = self.__get_latest_index_by_filelist(GeneralUtilities.get_all_files_of_folder(os.path.join(self.__letsencrypt_archive_folder, domain)))
         GeneralUtilities.write_message_to_stdout(f"Debug: Latest found existing number for domain {domain}: {result}")
@@ -105,20 +105,18 @@
                 else:
                     GeneralUtilities.write_message_to_stdout(f"Create certificate for domain {domain}")
                 certbot_container_name = "r2_updatecertificates_certbot"
                 dockerargument = f"run --name {certbot_container_name} --volume {self.__letsencrypt_folder}:/etc/letsencrypt"
                 dockerargument = dockerargument+f" --volume {self.__log_folder}:/var/log/letsencrypt -p 80:80 certbot/certbot:latest"
                 certbotargument = f"--standalone --email {self.__email} --agree-tos --force-renewal --rsa-key-size 4096 --non-interactive --no-eff-email --domain {domain}"
                 if(certificate_for_domain_already_exists):
-                    self.__sc.run_program("docker", f"{dockerargument} certonly --no-random-sleep-on-renew {certbotargument}",
-                                          self.__current_folder, throw_exception_if_exitcode_is_not_zero=True)
+                    self.__sc.run_program("docker", f"{dockerargument} certonly --no-random-sleep-on-renew {certbotargument}",                                          self.__current_folder, throw_exception_if_exitcode_is_not_zero=True)
                     self.__replace_symlinks_by_files(domain)
                 else:
-                    self.__sc.run_program("docker", f"{dockerargument} certonly --cert-name {domain} {certbotargument}",
-                                          self.__current_folder, throw_exception_if_exitcode_is_not_zero=True)
+                    self.__sc.run_program("docker", f"{dockerargument} certonly --cert-name {domain} {certbotargument}",                                          self.__current_folder, throw_exception_if_exitcode_is_not_zero=True)
             except Exception as exception:
                 GeneralUtilities.write_exception_to_stderr_with_traceback(exception, traceback, "Error while updating certificate")
             finally:
                 try:
                     self.__sc.run_program("docker", f"container rm {certbot_container_name}", self.__current_folder, throw_exception_if_exitcode_is_not_zero=True)
                 except Exception as exception:
                     GeneralUtilities.write_exception_to_stderr_with_traceback(exception, traceback, "Error while removing container")
```

## Comparing `ScriptCollection-3.4.9.dist-info/METADATA` & `ScriptCollection-3.5.0.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ScriptCollection
-Version: 3.4.9
+Version: 3.5.0
 Summary: The ScriptCollection is the place for reusable scripts.
 Home-page: https://github.com/anionDev/ScriptCollection
 Author: Marius Göcke
 Author-email: marius.goecke@gmail.com
 Project-URL: Documentation, https://aniondev.github.io/ScriptCollectionReference/index.html
 Project-URL: Changelog, https://github.com/anionDev/ScriptCollection/tree/main/Other/Resources/Changelog
 Keywords: package release build management
@@ -18,32 +18,33 @@
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: System :: Archiving :: Packaging
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Terminals
 Classifier: Topic :: Utilities
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Requires-Dist: coverage (>=7.2.7)
-Requires-Dist: cyclonedx-bom (>=3.11.2)
-Requires-Dist: defusedxml (>=0.7.1)
-Requires-Dist: keyboard (>=0.13.5)
-Requires-Dist: lxml (>=4.9.3)
-Requires-Dist: ntplib (>=0.4.0)
-Requires-Dist: Pillow (>=10.0.0)
-Requires-Dist: pycdlib (>=1.14.0)
-Requires-Dist: Pygments (>=2.15.1)
-Requires-Dist: pylint (>=2.17.4)
-Requires-Dist: pyOpenSSL (>=23.2.0)
-Requires-Dist: PyMuPDF (>=1.22.5)
-Requires-Dist: PyPDF2 (>=3.0.1)
-Requires-Dist: pytest (>=7.4.0)
-Requires-Dist: qrcode (>=7.4.2)
-Requires-Dist: send2trash (>=1.8.2)
-Requires-Dist: twine (>=4.0.2)
-Requires-Dist: xmlschema (>=2.3.1)
+Requires-Dist: build >=1.2.1
+Requires-Dist: coverage >=7.5.0
+Requires-Dist: cyclonedx-bom >=4.4.3
+Requires-Dist: defusedxml >=0.7.1
+Requires-Dist: keyboard >=0.13.5
+Requires-Dist: lcov-cobertura >=2.0.2
+Requires-Dist: lxml >=5.2.1
+Requires-Dist: ntplib >=0.4.0
+Requires-Dist: Pillow >=10.3.0
+Requires-Dist: pycdlib >=1.14.0
+Requires-Dist: Pygments >=2.17.2
+Requires-Dist: pylint >=3.1.0
+Requires-Dist: pyOpenSSL >=24.1.0
+Requires-Dist: PyPDF2 >=3.0.1
+Requires-Dist: pytest >=8.2.0
+Requires-Dist: qrcode >=7.4.2
+Requires-Dist: send2trash >=1.8.3
+Requires-Dist: twine >=5.0.0
+Requires-Dist: xmlschema >=3.3.1
 
 # ScriptCollection
 
 ## General
 
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/ScriptCollection.svg)](https://pypi.org/project/ScriptCollection/)
 ![PyPI](https://img.shields.io/pypi/v/ScriptCollection)
```

## Comparing `ScriptCollection-3.4.9.dist-info/entry_points.txt` & `ScriptCollection-3.5.0.dist-info/entry_points.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 [console_scripts]
-SCBuildCodeUnit = ScriptCollection.Executables:BuildCodeUnit
-SCBuildCodeUnits = ScriptCollection.Executables:BuildCodeUnits
-SCCalculateBitcoinBlockHash = ScriptCollection.Executables:CalculateBitcoinBlockHash
-SCChangeHashOfProgram = ScriptCollection.Executables:ChangeHashOfProgram
-SCCreateEmptyFileWithSpecificSize = ScriptCollection.Executables:CreateEmptyFileWithSpecificSize
-SCCreateHashOfAllFiles = ScriptCollection.Executables:CreateHashOfAllFiles
-SCCreateISOFileWithObfuscatedFiles = ScriptCollection.Executables:CreateISOFileWithObfuscatedFiles
-SCCreateSimpleMergeWithoutRelease = ScriptCollection.Executables:CreateSimpleMergeWithoutRelease
-SCExtractPDFPages = ScriptCollection.Executables:ExtractPDFPages
-SCFilenameObfuscator = ScriptCollection.Executables:FilenameObfuscator
-SCGenerateCertificate = ScriptCollection.Executables:GenerateCertificate
-SCGenerateCertificateAuthority = ScriptCollection.Executables:GenerateCertificateAuthority
-SCGenerateCertificateSignRequest = ScriptCollection.Executables:GenerateCertificateSignRequest
-SCGenerateSnkFiles = ScriptCollection.Executables:GenerateSnkFiles
-SCGenerateThumbnail = ScriptCollection.Executables:GenerateThumbnail
-SCHealthcheck = ScriptCollection.Executables:Healthcheck
-SCKeyboardDiagnosis = ScriptCollection.Executables:KeyboardDiagnosis
-SCMergePDFs = ScriptCollection.Executables:MergePDFs
-SCObfuscateFilesFolder = ScriptCollection.Executables:ObfuscateFilesFolder
-SCOrganizeLinesInFile = ScriptCollection.Executables:OrganizeLinesInFile
-SCPDFToImage = ScriptCollection.Executables:PDFToImage
-SCReplaceSubstringsInFilenames = ScriptCollection.Executables:ReplaceSubstringsInFilenames
-SCSearchInFiles = ScriptCollection.Executables:SearchInFiles
-SCShow2FAAsQRCode = ScriptCollection.Executables:Show2FAAsQRCode
-SCShowMissingFiles = ScriptCollection.Executables:ShowMissingFiles
-SCSignCertificate = ScriptCollection.Executables:SignCertificate
-SCUpdateNugetpackagesInCsharpProject = ScriptCollection.Executables:UpdateNugetpackagesInCsharpProject
-SCUploadFile = ScriptCollection.Executables:UploadFile
+scbuildcodeunit = ScriptCollection.Executables:BuildCodeUnit
+scbuildcodeunits = ScriptCollection.Executables:BuildCodeUnits
+scbuildcodeunitsc = ScriptCollection.Executables:BuildCodeUnitsC
+sccalculatebitcoinblockhash = ScriptCollection.Executables:CalculateBitcoinBlockHash
+scchangehashofprogram = ScriptCollection.Executables:ChangeHashOfProgram
+sccreateemptyfilewithspecificsize = ScriptCollection.Executables:CreateEmptyFileWithSpecificSize
+sccreatehashofallfiles = ScriptCollection.Executables:CreateHashOfAllFiles
+sccreateisofilewithobfuscatedfiles = ScriptCollection.Executables:CreateISOFileWithObfuscatedFiles
+sccreatesimplemergewithoutrelease = ScriptCollection.Executables:CreateSimpleMergeWithoutRelease
+scextractpdfpages = ScriptCollection.Executables:ExtractPDFPages
+scfilenameobfuscator = ScriptCollection.Executables:FilenameObfuscator
+scgeneratecertificate = ScriptCollection.Executables:GenerateCertificate
+scgeneratecertificateauthority = ScriptCollection.Executables:GenerateCertificateAuthority
+scgeneratecertificatesignrequest = ScriptCollection.Executables:GenerateCertificateSignRequest
+scgeneratesnkfiles = ScriptCollection.Executables:GenerateSnkFiles
+scgeneratethumbnail = ScriptCollection.Executables:GenerateThumbnail
+schealthcheck = ScriptCollection.Executables:Healthcheck
+sckeyboarddiagnosis = ScriptCollection.Executables:KeyboardDiagnosis
+scmergepdfs = ScriptCollection.Executables:MergePDFs
+scobfuscatefilesfolder = ScriptCollection.Executables:ObfuscateFilesFolder
+scorganizelinesinfile = ScriptCollection.Executables:OrganizeLinesInFile
+scpdftoimage = ScriptCollection.Executables:PDFToImage
+screplacesubstringsinfilenames = ScriptCollection.Executables:ReplaceSubstringsInFilenames
+scsearchinfiles = ScriptCollection.Executables:SearchInFiles
+scshow2faasqrcode = ScriptCollection.Executables:Show2FAAsQRCode
+scshowmissingfiles = ScriptCollection.Executables:ShowMissingFiles
+scsigncertificate = ScriptCollection.Executables:SignCertificate
+scupdatenugetpackagesincsharpproject = ScriptCollection.Executables:UpdateNugetpackagesInCsharpProject
+scuploadfile = ScriptCollection.Executables:UploadFile
```

## Comparing `ScriptCollection-3.4.9.dist-info/RECORD` & `ScriptCollection-3.5.0.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-ScriptCollection/Executables.py,sha256=tRIsXE_ZhjnMt75YhEL-FHEHuiUC3YzGdeVibLiWvoE,19005
-ScriptCollection/GeneralUtilities.py,sha256=vZDiW5lWJRCrIZVs1bTCZ-O5slQnM5dv4GcJ-RTMowY,34378
+ScriptCollection/Executables.py,sha256=F8ar_pRplVZm0mHLJ_Ono5HKTfqr6wTceG3Hcbx_tow,19282
+ScriptCollection/GeneralUtilities.py,sha256=Mcp6ghb6AbS1KsOjEnRw3x4a4mBrAZ6DAjV2j8-LZFM,35589
 ScriptCollection/ProgramRunnerBase.py,sha256=2kyOuoM3oFjBfLc9Q5t5RTz7Ya2CjUxFtB1rBBDmnjU,1937
 ScriptCollection/ProgramRunnerEpew.py,sha256=nIzY4dG6W-xEpkeoTbozwNZtFSIo-bU_W6t6u1AZKtE,6275
-ScriptCollection/ProgramRunnerPopen.py,sha256=HOs1QVnXiQtwXy1_xvH79bWBdd0i-2tUyyLloQBvMto,3023
-ScriptCollection/ScriptCollectionCore.py,sha256=AqltVwGv0wHQ-Y2IXEDmnuIdY8fQhkg_jciA9CcBQ_I,94475
-ScriptCollection/TasksForCommonProjectStructure.py,sha256=3ZXzRX7YAzLS8NurwSG0WLfnByVEbmmzx-s8zBME4vs,145487
-ScriptCollection/UpdateCertificates.py,sha256=Go-JJK-YTi7aBB1phlLxypa8GHkmFHBEPB0_TT9G-bw,7918
+ScriptCollection/ProgramRunnerPopen.py,sha256=kV7KVuDenKjOyNBFurMTcuhuLuLZ74MaaSrwaPjaHCs,3158
+ScriptCollection/ScriptCollectionCore.py,sha256=LXHRp3sWZmIdWRhOXFbQxGE4aPel194AhMXgD8LCKOs,92657
+ScriptCollection/TasksForCommonProjectStructure.py,sha256=4ZxLkYtT7nszV46AT0E7_TuAziFokFnG1UcZ9VFYfzk,173711
+ScriptCollection/UpdateCertificates.py,sha256=3C_E9og5SZec35aD3BFYLchzJtonsg1KR4enFCb5Jzk,7914
 ScriptCollection/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ScriptCollection-3.4.9.dist-info/METADATA,sha256=7Q4qLKsAFGl8X8x7hedx0YmCft217mWd5biohDqEnC0,7650
-ScriptCollection-3.4.9.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-ScriptCollection-3.4.9.dist-info/entry_points.txt,sha256=dJKdWcH41owxlKx_khj4P7DItr9lhxWP9JU2Dq8GSsQ,2088
-ScriptCollection-3.4.9.dist-info/top_level.txt,sha256=hY2hOVH0V0Ce51WB76zKkIWTUNwMUdHo4XDkR2vYVwg,17
-ScriptCollection-3.4.9.dist-info/RECORD,,
+ScriptCollection-3.5.0.dist-info/METADATA,sha256=RVO_ZaAz9cLgXhOTyAZUMvA7eqk9pMGPvmAUEcDEqeQ,7648
+ScriptCollection-3.5.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+ScriptCollection-3.5.0.dist-info/entry_points.txt,sha256=dwvB9HRGvqst5xlYIGmmwuFN7lBKhxvndmnNrQOfu8w,2153
+ScriptCollection-3.5.0.dist-info/top_level.txt,sha256=hY2hOVH0V0Ce51WB76zKkIWTUNwMUdHo4XDkR2vYVwg,17
+ScriptCollection-3.5.0.dist-info/RECORD,,
```

