# Comparing `tmp/paperman-1.0.3.tar.gz` & `tmp/paperman-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paperman-1.0.3.tar", last modified: Thu Feb 15 07:37:37 2024, max compression
+gzip compressed data, was "paperman-1.0.4.tar", last modified: Tue Apr 30 05:53:26 2024, max compression
```

## Comparing `paperman-1.0.3.tar` & `paperman-1.0.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 bredol    (1000) bredol    (1000)        0 2024-02-15 07:37:37.808241 paperman-1.0.3/
--rw-r--r--   0 bredol    (1000) bredol    (1000)     1067 2024-02-15 07:11:38.000000 paperman-1.0.3/LICENSE.txt
--rw-r--r--   0 bredol    (1000) bredol    (1000)    11699 2024-02-15 07:37:37.808241 paperman-1.0.3/PKG-INFO
--rw-r--r--   0 bredol    (1000) bredol    (1000)    11360 2024-02-15 07:32:45.000000 paperman-1.0.3/README.md
-drwxr-xr-x   0 bredol    (1000) bredol    (1000)        0 2024-02-15 07:37:37.808241 paperman-1.0.3/paperman/
--rw-r--r--   0 bredol    (1000) bredol    (1000)      418 2024-02-15 07:11:38.000000 paperman-1.0.3/paperman/__init__.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)    11362 2024-02-15 07:11:38.000000 paperman-1.0.3/paperman/__main__.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)     5030 2024-02-15 07:11:38.000000 paperman-1.0.3/paperman/cfg.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)     6384 2024-02-15 07:11:38.000000 paperman-1.0.3/paperman/finder.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)     4656 2024-02-15 07:11:38.000000 paperman-1.0.3/paperman/io.py
-drwxr-xr-x   0 bredol    (1000) bredol    (1000)        0 2024-02-15 07:37:37.808241 paperman-1.0.3/paperman/parser/
--rw-r--r--   0 bredol    (1000) bredol    (1000)       98 2024-02-15 07:11:38.000000 paperman-1.0.3/paperman/parser/__init__.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)    15175 2024-02-15 07:11:38.000000 paperman-1.0.3/paperman/parser/bib.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)    16701 2024-02-15 07:11:38.000000 paperman-1.0.3/paperman/parser/cite.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)      609 2024-02-15 07:11:38.000000 paperman-1.0.3/paperman/parser/common.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)     1232 2024-02-15 07:11:38.000000 paperman-1.0.3/paperman/parser/img.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)    57618 2024-02-15 07:11:38.000000 paperman-1.0.3/paperman/parser/journal.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)    11401 2024-02-15 07:11:38.000000 paperman-1.0.3/paperman/parser/tex.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)     5040 2024-02-15 07:11:38.000000 paperman-1.0.3/paperman/project.py
-drwxr-xr-x   0 bredol    (1000) bredol    (1000)        0 2024-02-15 07:37:37.808241 paperman-1.0.3/paperman/subcommands/
--rw-r--r--   0 bredol    (1000) bredol    (1000)        0 2024-02-15 07:11:38.000000 paperman-1.0.3/paperman/subcommands/__init__.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)     4344 2024-02-15 07:11:38.000000 paperman-1.0.3/paperman/subcommands/bib.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)     1610 2024-02-15 07:11:38.000000 paperman-1.0.3/paperman/subcommands/clean.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)     6012 2024-02-15 07:11:38.000000 paperman-1.0.3/paperman/subcommands/collect.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)     1173 2024-02-15 07:11:38.000000 paperman-1.0.3/paperman/subcommands/common.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)      146 2024-02-15 07:11:38.000000 paperman-1.0.3/paperman/subcommands/config.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)     5682 2024-02-15 07:11:38.000000 paperman-1.0.3/paperman/subcommands/diff.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)     3221 2024-02-15 07:11:38.000000 paperman-1.0.3/paperman/subcommands/img.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)      871 2024-02-15 07:11:38.000000 paperman-1.0.3/paperman/subcommands/inp.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)      496 2024-02-15 07:11:38.000000 paperman-1.0.3/paperman/subcommands/journal.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)     7600 2024-02-15 07:11:38.000000 paperman-1.0.3/paperman/subcommands/lib.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)      298 2024-02-15 07:11:38.000000 paperman-1.0.3/paperman/subcommands/lint.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)     1317 2024-02-15 07:11:38.000000 paperman-1.0.3/paperman/subcommands/sort_authors.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)     4440 2024-02-15 07:11:38.000000 paperman-1.0.3/paperman/subcommands/sync.py
--rw-r--r--   0 bredol    (1000) bredol    (1000)     1482 2024-02-15 07:11:38.000000 paperman-1.0.3/paperman/utils.py
-drwxr-xr-x   0 bredol    (1000) bredol    (1000)        0 2024-02-15 07:37:37.808241 paperman-1.0.3/paperman.egg-info/
--rw-r--r--   0 bredol    (1000) bredol    (1000)    11699 2024-02-15 07:37:37.000000 paperman-1.0.3/paperman.egg-info/PKG-INFO
--rw-r--r--   0 bredol    (1000) bredol    (1000)      953 2024-02-15 07:37:37.000000 paperman-1.0.3/paperman.egg-info/SOURCES.txt
--rw-r--r--   0 bredol    (1000) bredol    (1000)        1 2024-02-15 07:37:37.000000 paperman-1.0.3/paperman.egg-info/dependency_links.txt
--rw-r--r--   0 bredol    (1000) bredol    (1000)       52 2024-02-15 07:37:37.000000 paperman-1.0.3/paperman.egg-info/entry_points.txt
--rw-r--r--   0 bredol    (1000) bredol    (1000)       49 2024-02-15 07:37:37.000000 paperman-1.0.3/paperman.egg-info/requires.txt
--rw-r--r--   0 bredol    (1000) bredol    (1000)        9 2024-02-15 07:37:37.000000 paperman-1.0.3/paperman.egg-info/top_level.txt
--rw-r--r--   0 bredol    (1000) bredol    (1000)       38 2024-02-15 07:37:37.808241 paperman-1.0.3/setup.cfg
--rwxr-xr-x   0 bredol    (1000) bredol    (1000)     1545 2024-02-15 07:37:37.000000 paperman-1.0.3/setup.py
+drwxr-xr-x   0 bredol    (1000) bredol    (1000)        0 2024-04-30 05:53:26.545028 paperman-1.0.4/
+-rw-r--r--   0 bredol    (1000) bredol    (1000)     1067 2024-02-15 07:11:38.000000 paperman-1.0.4/LICENSE.txt
+-rw-r--r--   0 bredol    (1000) bredol    (1000)    11699 2024-04-30 05:53:26.545028 paperman-1.0.4/PKG-INFO
+-rw-r--r--   0 bredol    (1000) bredol    (1000)    11360 2024-02-15 07:32:45.000000 paperman-1.0.4/README.md
+drwxr-xr-x   0 bredol    (1000) bredol    (1000)        0 2024-04-30 05:53:26.545028 paperman-1.0.4/paperman/
+-rw-r--r--   0 bredol    (1000) bredol    (1000)      418 2024-02-15 07:11:38.000000 paperman-1.0.4/paperman/__init__.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)    11362 2024-02-15 07:11:38.000000 paperman-1.0.4/paperman/__main__.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)     5072 2024-04-30 05:53:10.000000 paperman-1.0.4/paperman/cfg.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)     6384 2024-02-15 07:11:38.000000 paperman-1.0.4/paperman/finder.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)     4656 2024-02-15 07:11:38.000000 paperman-1.0.4/paperman/io.py
+drwxr-xr-x   0 bredol    (1000) bredol    (1000)        0 2024-04-30 05:53:26.545028 paperman-1.0.4/paperman/parser/
+-rw-r--r--   0 bredol    (1000) bredol    (1000)       98 2024-02-15 07:11:38.000000 paperman-1.0.4/paperman/parser/__init__.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)    15175 2024-02-15 07:11:38.000000 paperman-1.0.4/paperman/parser/bib.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)    16701 2024-02-15 07:11:38.000000 paperman-1.0.4/paperman/parser/cite.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)      609 2024-02-15 07:11:38.000000 paperman-1.0.4/paperman/parser/common.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)     1232 2024-02-15 07:11:38.000000 paperman-1.0.4/paperman/parser/img.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)    57618 2024-02-15 07:11:38.000000 paperman-1.0.4/paperman/parser/journal.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)    13003 2024-04-30 05:53:10.000000 paperman-1.0.4/paperman/parser/tex.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)     5040 2024-02-15 07:11:38.000000 paperman-1.0.4/paperman/project.py
+drwxr-xr-x   0 bredol    (1000) bredol    (1000)        0 2024-04-30 05:53:26.545028 paperman-1.0.4/paperman/subcommands/
+-rw-r--r--   0 bredol    (1000) bredol    (1000)        0 2024-02-15 07:11:38.000000 paperman-1.0.4/paperman/subcommands/__init__.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)     4344 2024-02-15 07:11:38.000000 paperman-1.0.4/paperman/subcommands/bib.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)     1610 2024-02-15 07:11:38.000000 paperman-1.0.4/paperman/subcommands/clean.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)     6012 2024-02-15 07:11:38.000000 paperman-1.0.4/paperman/subcommands/collect.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)     1173 2024-02-15 07:11:38.000000 paperman-1.0.4/paperman/subcommands/common.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)      146 2024-02-15 07:11:38.000000 paperman-1.0.4/paperman/subcommands/config.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)     5682 2024-02-15 07:11:38.000000 paperman-1.0.4/paperman/subcommands/diff.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)     3221 2024-02-15 07:11:38.000000 paperman-1.0.4/paperman/subcommands/img.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)      871 2024-02-15 07:11:38.000000 paperman-1.0.4/paperman/subcommands/inp.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)      496 2024-02-15 07:11:38.000000 paperman-1.0.4/paperman/subcommands/journal.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)     7600 2024-02-15 07:11:38.000000 paperman-1.0.4/paperman/subcommands/lib.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)      298 2024-02-15 07:11:38.000000 paperman-1.0.4/paperman/subcommands/lint.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)     1317 2024-02-15 07:11:38.000000 paperman-1.0.4/paperman/subcommands/sort_authors.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)     4440 2024-02-15 07:11:38.000000 paperman-1.0.4/paperman/subcommands/sync.py
+-rw-r--r--   0 bredol    (1000) bredol    (1000)     1482 2024-02-15 07:11:38.000000 paperman-1.0.4/paperman/utils.py
+drwxr-xr-x   0 bredol    (1000) bredol    (1000)        0 2024-04-30 05:53:26.545028 paperman-1.0.4/paperman.egg-info/
+-rw-r--r--   0 bredol    (1000) bredol    (1000)    11699 2024-04-30 05:53:26.000000 paperman-1.0.4/paperman.egg-info/PKG-INFO
+-rw-r--r--   0 bredol    (1000) bredol    (1000)      953 2024-04-30 05:53:26.000000 paperman-1.0.4/paperman.egg-info/SOURCES.txt
+-rw-r--r--   0 bredol    (1000) bredol    (1000)        1 2024-04-30 05:53:26.000000 paperman-1.0.4/paperman.egg-info/dependency_links.txt
+-rw-r--r--   0 bredol    (1000) bredol    (1000)       52 2024-04-30 05:53:26.000000 paperman-1.0.4/paperman.egg-info/entry_points.txt
+-rw-r--r--   0 bredol    (1000) bredol    (1000)       49 2024-04-30 05:53:26.000000 paperman-1.0.4/paperman.egg-info/requires.txt
+-rw-r--r--   0 bredol    (1000) bredol    (1000)        9 2024-04-30 05:53:26.000000 paperman-1.0.4/paperman.egg-info/top_level.txt
+-rw-r--r--   0 bredol    (1000) bredol    (1000)       38 2024-04-30 05:53:26.545028 paperman-1.0.4/setup.cfg
+-rwxr-xr-x   0 bredol    (1000) bredol    (1000)     1545 2024-04-30 05:53:26.000000 paperman-1.0.4/setup.py
```

### Comparing `paperman-1.0.3/LICENSE.txt` & `paperman-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `paperman-1.0.3/PKG-INFO` & `paperman-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paperman
-Version: 1.0.3
+Version: 1.0.4
 Summary: latex project and bibliography management utility
 Author: zaphB
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: appdirs
 Requires-Dist: argparse
```

### Comparing `paperman-1.0.3/README.md` & `paperman-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `paperman-1.0.3/paperman/__main__.py` & `paperman-1.0.4/paperman/__main__.py`

 * *Files identical despite different names*

### Comparing `paperman-1.0.3/paperman/cfg.py` & `paperman-1.0.4/paperman/cfg.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,16 @@
     required_suffs = ['tex', 'pdf', 'aux'],
     clean_suffs = ['aux', 'bcf', 'log', 'snm', 'vrb', 'run.xml', 'synctex',
                    'nav', 'blg', 'fls', 'fdb_latexmk', 'toc', 'tdo', 'out']
   ),
   lint=dict(
     avoid_commands_in_toplevel=[],
     avoid_commands = [],
+    avoid_words=[],
+    known_authors=[],
 #    check_spelling=[]
   ),
   library_path = '~/Documents/bibliography',
   library_sync_additional_paths = [],
   library_collect_paths = ['~/Desktop', '~/Downloads'],
   library_folder_pattern = '%Y-%m',
   library_max_filename_len = 60,
```

### Comparing `paperman-1.0.3/paperman/finder.py` & `paperman-1.0.4/paperman/finder.py`

 * *Files identical despite different names*

### Comparing `paperman-1.0.3/paperman/io.py` & `paperman-1.0.4/paperman/io.py`

 * *Files identical despite different names*

### Comparing `paperman-1.0.3/paperman/parser/bib.py` & `paperman-1.0.4/paperman/parser/bib.py`

 * *Files identical despite different names*

### Comparing `paperman-1.0.3/paperman/parser/cite.py` & `paperman-1.0.4/paperman/parser/cite.py`

 * *Files identical despite different names*

### Comparing `paperman-1.0.3/paperman/parser/common.py` & `paperman-1.0.4/paperman/parser/common.py`

 * *Files identical despite different names*

### Comparing `paperman-1.0.3/paperman/parser/img.py` & `paperman-1.0.4/paperman/parser/img.py`

 * *Files identical despite different names*

### Comparing `paperman-1.0.3/paperman/parser/journal.py` & `paperman-1.0.4/paperman/parser/journal.py`

 * *Files identical despite different names*

### Comparing `paperman-1.0.3/paperman/parser/tex.py` & `paperman-1.0.4/paperman/parser/tex.py`

 * *Files 10% similar despite different names*

```diff
@@ -264,19 +264,45 @@
   def lint(self, visited=[]):
     for i in self.includes():
       if i not in visited:
         for l in i.lint(visited=visited):
           yield l
         visited.append(i)
 
+    # detect author entries and check whether they exist in whitelist
+    authorPattern = r'([^\n]*)\\author\{([^}]*)\}([^\n]*)'
+    knownAuthors = list(cfg.get('lint', 'known_authors'))
+
+    for pre, authorName, post in re.findall(authorPattern, self.content(), re.M):
+      # skip lines marked as ok:
+      textAround = pre + ' ' + post
+      if 'nolint' in textAround.split() or '%nolint' in textAround.split():
+        continue
+      
+      # ask if author name should be added, complain otherwise
+      authorName = authorName.strip()
+      if authorName not in knownAuthors:
+        if io.conf(f'found author {authorName} which is not in known_authors list, ',
+                   f'add to list?', default=False):
+          knownAuthors = knownAuthors+[authorName]
+          cfg.set('lint', 'known_authors', knownAuthors)
+        else:
+          yield (self.path, nan,
+                 f'author name {authorName} is not in known_authors list')
+
+
     for ln, l in self.enumContent():
       # skip lines marked as ok:
       if 'nolint' in l.split() or '%nolint' in l.split():
         continue
 
+      # skip commented lines
+      if l.strip().startswith('%'):
+        continue
+
       # search for dollars without line break protection
       i = -1
       lastOpening = None
       opening = True
       doWarn = False
       while True:
         i = l.find('$', i+1)
@@ -299,33 +325,46 @@
                    'math should be wrapped in curly braces to avoid\n'
                    'line breaks: not $a = b$ but ${a = b}$')
       if doWarn:
         yield (self.path, ln,
                'math should be wrapped in curly braces to avoid\n'
                'line breaks: not $a = b$ but ${a = b}$')
 
-
       # find commands that should not used or not be used in toplevel files
       avoidCommands = list(cfg.get('lint', 'avoid_commands'))
       if self.isToplevel():
         avoidCommands += list(cfg.get('lint', 'avoid_commands_in_toplevel'))
       for cmd in avoidCommands:
         cmd = cmd.strip(r'\ {}')
         if len(cmd) == 1:
           io.warn(f'command {cmd} in avoid_commands list is only one '
                    'character long')
         if re.search('\\\\'+cmd, l):
           bs = '\\'
           yield (self.path, ln,
                  f'found latex command {bs}{cmd}, which is on avoid-list')
 
+      # detect words in avoid list
+      avoidWords = list(cfg.get('lint', 'avoid_words'))
+      for word in avoidWords:
+        # \b matches "word boundaries", i.e. white-spaces, string start/end etc.
+        if re.search(r'\b'+word.lower()+r'\b', l.lower()):
+          yield (self.path, ln,
+                 f'found word {word}, which is on avoid-list')
+
       # find double words
       _l = re.sub(r'\s+', ' ', l.replace(',', '').replace('.', ''))
       for w1, w2 in zip(_l.split()[:-1], _l.split()[1:]):
         if w1 == w2:
           yield (self.path, ln,
                  f'found duplicate word "{w1}"')
 
+      # detect commas before that and because
+      for word in ('because', 'that'):
+        if re.search(r',\s*'+word, l.lower()):
+          yield (self.path, ln,
+                 f'found comma before {word}')
+
       # spellcheck
       # TODO
 
     visited.append(self)
```

### Comparing `paperman-1.0.3/paperman/project.py` & `paperman-1.0.4/paperman/project.py`

 * *Files identical despite different names*

### Comparing `paperman-1.0.3/paperman/subcommands/bib.py` & `paperman-1.0.4/paperman/subcommands/bib.py`

 * *Files identical despite different names*

### Comparing `paperman-1.0.3/paperman/subcommands/clean.py` & `paperman-1.0.4/paperman/subcommands/clean.py`

 * *Files identical despite different names*

### Comparing `paperman-1.0.3/paperman/subcommands/collect.py` & `paperman-1.0.4/paperman/subcommands/collect.py`

 * *Files identical despite different names*

### Comparing `paperman-1.0.3/paperman/subcommands/common.py` & `paperman-1.0.4/paperman/subcommands/common.py`

 * *Files identical despite different names*

### Comparing `paperman-1.0.3/paperman/subcommands/diff.py` & `paperman-1.0.4/paperman/subcommands/diff.py`

 * *Files identical despite different names*

### Comparing `paperman-1.0.3/paperman/subcommands/img.py` & `paperman-1.0.4/paperman/subcommands/img.py`

 * *Files identical despite different names*

### Comparing `paperman-1.0.3/paperman/subcommands/inp.py` & `paperman-1.0.4/paperman/subcommands/inp.py`

 * *Files identical despite different names*

### Comparing `paperman-1.0.3/paperman/subcommands/lib.py` & `paperman-1.0.4/paperman/subcommands/lib.py`

 * *Files identical despite different names*

### Comparing `paperman-1.0.3/paperman/subcommands/sort_authors.py` & `paperman-1.0.4/paperman/subcommands/sort_authors.py`

 * *Files identical despite different names*

### Comparing `paperman-1.0.3/paperman/subcommands/sync.py` & `paperman-1.0.4/paperman/subcommands/sync.py`

 * *Files identical despite different names*

### Comparing `paperman-1.0.3/paperman/utils.py` & `paperman-1.0.4/paperman/utils.py`

 * *Files identical despite different names*

### Comparing `paperman-1.0.3/paperman.egg-info/PKG-INFO` & `paperman-1.0.4/paperman.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paperman
-Version: 1.0.3
+Version: 1.0.4
 Summary: latex project and bibliography management utility
 Author: zaphB
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: appdirs
 Requires-Dist: argparse
```

### Comparing `paperman-1.0.3/paperman.egg-info/SOURCES.txt` & `paperman-1.0.4/paperman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `paperman-1.0.3/setup.py` & `paperman-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/python3
 
 from setuptools import setup
 from setuptools.command.install import install
 
 # DO NOT CHANGE: this line will be replaced by ./dev/update-setup.py
-version = '1.0.3'
+version = '1.0.4'
 
 # if setup is run in project dir, update version number
 try:
   import os
   import subprocess
   p = os.path.join(os.path.dirname(__file__), 'dev/update-setup.sh')
   if (os.path.isfile(p) and os.access(p, os.X_OK)):
```

