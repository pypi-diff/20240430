# Comparing `tmp/dublib-0.5.2.tar.gz` & `tmp/dublib-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dublib-0.5.2.tar", last modified: Sun Apr 21 19:56:26 2024, max compression
+gzip compressed data, was "dublib-0.6.0.tar", last modified: Tue Apr 30 18:08:11 2024, max compression
```

## Comparing `dublib-0.5.2.tar` & `dublib-0.6.0.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:56:26.347750 dublib-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-21 19:56:21.000000 dublib-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-04-21 19:56:26.347750 dublib-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-21 19:56:21.000000 dublib-0.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-21 19:56:21.000000 dublib-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 19:56:26.347750 dublib-0.5.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:56:26.343750 dublib-0.5.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:56:26.343750 dublib-0.5.2/src/dublib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:56:26.343750 dublib-0.5.2/src/dublib/Exceptions/
--rwxr-xr-x   0 runner    (1001) docker     (127)      624 2024-04-21 19:56:21.000000 dublib-0.5.2/src/dublib/Exceptions/StyledPrinter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5427 2024-04-21 19:56:21.000000 dublib-0.5.2/src/dublib/Exceptions/Terminalyzer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      616 2024-04-21 19:56:21.000000 dublib-0.5.2/src/dublib/Exceptions/WebRequestor.py
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:56:21.000000 dublib-0.5.2/src/dublib/Exceptions/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9391 2024-04-21 19:56:21.000000 dublib-0.5.2/src/dublib/Methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-04-21 19:56:21.000000 dublib-0.5.2/src/dublib/Polyglot.py
--rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-04-21 19:56:21.000000 dublib-0.5.2/src/dublib/StyledPrinter.py
--rw-r--r--   0 runner    (1001) docker     (127)    42914 2024-04-21 19:56:21.000000 dublib-0.5.2/src/dublib/Terminalyzer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    30855 2024-04-21 19:56:21.000000 dublib-0.5.2/src/dublib/WebRequestor.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:56:21.000000 dublib-0.5.2/src/dublib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:56:26.347750 dublib-0.5.2/src/dublib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-04-21 19:56:26.000000 dublib-0.5.2/src/dublib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-21 19:56:26.000000 dublib-0.5.2/src/dublib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 19:56:26.000000 dublib-0.5.2/src/dublib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-21 19:56:26.000000 dublib-0.5.2/src/dublib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-21 19:56:26.000000 dublib-0.5.2/src/dublib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:08:11.317566 dublib-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-30 18:08:06.000000 dublib-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-04-30 18:08:11.317566 dublib-0.6.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1742 2024-04-30 18:08:06.000000 dublib-0.6.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1113 2024-04-30 18:08:06.000000 dublib-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 18:08:11.317566 dublib-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:08:11.313566 dublib-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:08:11.313566 dublib-0.6.0/src/dublib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:08:11.317566 dublib-0.6.0/src/dublib/Exceptions/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      624 2024-04-30 18:08:06.000000 dublib-0.6.0/src/dublib/Exceptions/StyledPrinter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      680 2024-04-30 18:08:06.000000 dublib-0.6.0/src/dublib/Exceptions/TelebotUtils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5427 2024-04-30 18:08:06.000000 dublib-0.6.0/src/dublib/Exceptions/Terminalyzer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      616 2024-04-30 18:08:06.000000 dublib-0.6.0/src/dublib/Exceptions/WebRequestor.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:08:06.000000 dublib-0.6.0/src/dublib/Exceptions/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10447 2024-04-30 18:08:06.000000 dublib-0.6.0/src/dublib/Methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-04-30 18:08:06.000000 dublib-0.6.0/src/dublib/Polyglot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-04-30 18:08:06.000000 dublib-0.6.0/src/dublib/StyledPrinter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14733 2024-04-30 18:08:06.000000 dublib-0.6.0/src/dublib/TelebotUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42914 2024-04-30 18:08:06.000000 dublib-0.6.0/src/dublib/Terminalyzer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    30855 2024-04-30 18:08:06.000000 dublib-0.6.0/src/dublib/WebRequestor.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 18:08:06.000000 dublib-0.6.0/src/dublib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:08:11.317566 dublib-0.6.0/src/dublib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-04-30 18:08:11.000000 dublib-0.6.0/src/dublib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-30 18:08:11.000000 dublib-0.6.0/src/dublib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 18:08:11.000000 dublib-0.6.0/src/dublib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-30 18:08:11.000000 dublib-0.6.0/src/dublib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-30 18:08:11.000000 dublib-0.6.0/src/dublib.egg-info/top_level.txt
```

### Comparing `dublib-0.5.2/LICENSE` & `dublib-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dublib-0.5.2/PKG-INFO` & `dublib-0.6.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dublib
-Version: 0.5.2
+Version: 0.6.0
 Summary: Коллекция модулей от DUB1401.
 Author-email: DUB1401 <vlad.milosta@outlook.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -45,23 +45,26 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: curl_cffi>=0.6.0
 Requires-Dist: fake_useragent
 Requires-Dist: httpx
 Requires-Dist: httpx[http2]
 Requires-Dist: requests
+Provides-Extra: telebot
+Requires-Dist: pyTelegramBotAPI; extra == "telebot"
 
 # dublib
 **dublib** – это библиотека, поставляющая компоненты, требующиеся в проектах [@DUB1401](https://github.com/DUB1401), написанных на Python.
 
 # Поставляемые компоненты
 Библиотека включает следующие модули:
 * [Methods](https://github.com/DUB1401/dublib/blob/main/docs/Methods.md)
 * [Polyglot](https://github.com/DUB1401/dublib/blob/main/docs/Polyglot.md)
 * [StyledPrinter](https://github.com/DUB1401/dublib/blob/main/docs/StyledPrinter.md)
+* [TelebotUtils](https://github.com/DUB1401/dublib/blob/main/docs/Terminalyzer.md)
 * [Terminalyzer](https://github.com/DUB1401/dublib/blob/main/docs/Terminalyzer.md)
 * [WebRequestor](https://github.com/DUB1401/dublib/blob/main/docs/WebRequestor.md)
 
 # Установка
 Библиотека поддерживает установку из двух типов репозиториев:
 * **PyPI** – стабильные выпуски (с возможностью выбора конкретной версии);
 * **GitHub** – канал разработки со всеми последними изменениями и исправлениями.
```

### Comparing `dublib-0.5.2/README.md` & `dublib-0.6.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 **dublib** – это библиотека, поставляющая компоненты, требующиеся в проектах [@DUB1401](https://github.com/DUB1401), написанных на Python.
 
 # Поставляемые компоненты
 Библиотека включает следующие модули:
 * [Methods](https://github.com/DUB1401/dublib/blob/main/docs/Methods.md)
 * [Polyglot](https://github.com/DUB1401/dublib/blob/main/docs/Polyglot.md)
 * [StyledPrinter](https://github.com/DUB1401/dublib/blob/main/docs/StyledPrinter.md)
+* [TelebotUtils](https://github.com/DUB1401/dublib/blob/main/docs/Terminalyzer.md)
 * [Terminalyzer](https://github.com/DUB1401/dublib/blob/main/docs/Terminalyzer.md)
 * [WebRequestor](https://github.com/DUB1401/dublib/blob/main/docs/WebRequestor.md)
 
 # Установка
 Библиотека поддерживает установку из двух типов репозиториев:
 * **PyPI** – стабильные выпуски (с возможностью выбора конкретной версии);
 * **GitHub** – канал разработки со всеми последними изменениями и исправлениями.
```

### Comparing `dublib-0.5.2/pyproject.toml` & `dublib-0.6.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "cython"]
 
 [project]
 name = "dublib"
-version = "0.5.2"
+version = "0.6.0"
 description = "Коллекция модулей от DUB1401."
 authors = [
 	{name = "DUB1401", email = "vlad.milosta@outlook.com"}
 ]
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.10"
@@ -26,12 +26,17 @@
 	"Programming Language :: Python",
 	"Programming Language :: Python :: 3.10",
 	"Programming Language :: Python :: 3.11",
 	"Programming Language :: Python :: 3.12",
 	"Programming Language :: Python :: 3.13"
 ]
 
+[project.optional-dependencies]
+telebot = [
+    "pyTelegramBotAPI"
+]
+
 [project.urls]
 Documentation = "https://github.com/DUB1401/dublib/tree/main/docs"
 "Source Code" = "https://github.com/DUB1401/dublib"
 "Bug Tracker" = "https://github.com/DUB1401/dublib/issues"
 Changelog = "https://github.com/DUB1401/dublib/releases"
```

### Comparing `dublib-0.5.2/src/dublib/Exceptions/StyledPrinter.py` & `dublib-0.6.0/src/dublib/Exceptions/StyledPrinter.py`

 * *Files identical despite different names*

### Comparing `dublib-0.5.2/src/dublib/Exceptions/Terminalyzer.py` & `dublib-0.6.0/src/dublib/Exceptions/Terminalyzer.py`

 * *Files identical despite different names*

### Comparing `dublib-0.5.2/src/dublib/Exceptions/WebRequestor.py` & `dublib-0.6.0/src/dublib/Exceptions/WebRequestor.py`

 * *Files identical despite different names*

### Comparing `dublib-0.5.2/src/dublib/Methods.py` & `dublib-0.6.0/src/dublib/Methods.py`

 * *Files 8% similar despite different names*

```diff
@@ -92,14 +92,49 @@
 	# Русский алфавит в нижнем регистре.
 	Alphabet = set("абвгдеёжзийклмнопрстуфхцчшщъыьэюя")
 	# Состояние: содержит ли строка кирилические символы.
 	IsTextContainsCyrillicCharacters = not Alphabet.isdisjoint(text.lower())
 
 	return IsTextContainsCyrillicCharacters
 
+def ChunkList(value: list, length: int) -> list[list]:
+	"""
+	Разделяет список на фрагменты фиксированной длинны.
+		value – обрабатываемое значение;
+		length – длина фрагментов.
+	"""
+
+	# Список списков.
+	Result = list()
+	# Индекс обрезки.
+	CutIndex = 1
+	# Буфер обрезки.
+	Buffer = list()
+
+	# Для каждого элемента.
+	for Index in range(len(value)):
+
+		# Если индекс обрезки совпадает с длиной.
+		if CutIndex == length:
+			# Запись и обнуление буфера.
+			Result.append(Buffer)
+			Buffer = list()
+
+		else:
+			# Запись элемента в буфер.
+			Buffer.append(value[Index])
+
+		# Инкремент индекса обрезки.
+		CutIndex += 1
+
+	# Если в буфере что-то осталось, записать отдельной строкой.
+	if len(Buffer) > 0: Result.append(Buffer)
+
+	return Result
+
 def IsNotAlpha(text: str) -> bool:
 	"""
 	Проверяет, состоит ли строка целиком из небуквенных символов.
 	"""
 
 	# Результат проверки.
 	Result = True
```

### Comparing `dublib-0.5.2/src/dublib/Polyglot.py` & `dublib-0.6.0/src/dublib/Polyglot.py`

 * *Files identical despite different names*

### Comparing `dublib-0.5.2/src/dublib/StyledPrinter.py` & `dublib-0.6.0/src/dublib/StyledPrinter.py`

 * *Files identical despite different names*

### Comparing `dublib-0.5.2/src/dublib/Terminalyzer.py` & `dublib-0.6.0/src/dublib/Terminalyzer.py`

 * *Files identical despite different names*

### Comparing `dublib-0.5.2/src/dublib/WebRequestor.py` & `dublib-0.6.0/src/dublib/WebRequestor.py`

 * *Files identical despite different names*

### Comparing `dublib-0.5.2/src/dublib.egg-info/PKG-INFO` & `dublib-0.6.0/src/dublib.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dublib
-Version: 0.5.2
+Version: 0.6.0
 Summary: Коллекция модулей от DUB1401.
 Author-email: DUB1401 <vlad.milosta@outlook.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -45,23 +45,26 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: curl_cffi>=0.6.0
 Requires-Dist: fake_useragent
 Requires-Dist: httpx
 Requires-Dist: httpx[http2]
 Requires-Dist: requests
+Provides-Extra: telebot
+Requires-Dist: pyTelegramBotAPI; extra == "telebot"
 
 # dublib
 **dublib** – это библиотека, поставляющая компоненты, требующиеся в проектах [@DUB1401](https://github.com/DUB1401), написанных на Python.
 
 # Поставляемые компоненты
 Библиотека включает следующие модули:
 * [Methods](https://github.com/DUB1401/dublib/blob/main/docs/Methods.md)
 * [Polyglot](https://github.com/DUB1401/dublib/blob/main/docs/Polyglot.md)
 * [StyledPrinter](https://github.com/DUB1401/dublib/blob/main/docs/StyledPrinter.md)
+* [TelebotUtils](https://github.com/DUB1401/dublib/blob/main/docs/Terminalyzer.md)
 * [Terminalyzer](https://github.com/DUB1401/dublib/blob/main/docs/Terminalyzer.md)
 * [WebRequestor](https://github.com/DUB1401/dublib/blob/main/docs/WebRequestor.md)
 
 # Установка
 Библиотека поддерживает установку из двух типов репозиториев:
 * **PyPI** – стабильные выпуски (с возможностью выбора конкретной версии);
 * **GitHub** – канал разработки со всеми последними изменениями и исправлениями.
```

