# Comparing `tmp/cardpydentity-0.1.0.tar.gz` & `tmp/cardpydentity-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cardpydentity-0.1.0.tar", last modified: Thu Apr 25 09:58:43 2024, max compression
+gzip compressed data, was "cardpydentity-0.2.0.tar", last modified: Tue Apr 30 03:42:14 2024, max compression
```

## Comparing `cardpydentity-0.1.0.tar` & `cardpydentity-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 09:58:43.675470 cardpydentity-0.1.0/
--rw-rw-rw-   0        0        0     1166 2024-04-25 09:43:38.000000 cardpydentity-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      853 2024-04-25 09:58:43.675470 cardpydentity-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-25 09:39:14.000000 cardpydentity-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-25 09:58:43.659811 cardpydentity-0.1.0/cardpydentity/
--rw-rw-rw-   0        0        0     2791 2024-04-25 09:43:31.000000 cardpydentity-0.1.0/cardpydentity/__init__.py
--rw-rw-rw-   0        0        0     2334 2024-04-25 09:20:35.000000 cardpydentity-0.1.0/cardpydentity/fuzzy.py
--rw-rw-rw-   0        0        0     1543 2024-04-25 09:42:43.000000 cardpydentity-0.1.0/cardpydentity/gpt.py
--rw-rw-rw-   0        0        0     1895 2024-04-25 09:22:54.000000 cardpydentity-0.1.0/cardpydentity/helpers.py
--rw-rw-rw-   0        0        0     1896 2024-04-25 09:20:22.000000 cardpydentity-0.1.0/cardpydentity/load.py
--rw-rw-rw-   0        0        0     7842 2024-04-25 09:43:34.000000 cardpydentity-0.1.0/cardpydentity/matcher.py
-drwxrwxrwx   0        0        0        0 2024-04-25 09:58:43.674461 cardpydentity-0.1.0/cardpydentity.egg-info/
--rw-rw-rw-   0        0        0      853 2024-04-25 09:58:43.000000 cardpydentity-0.1.0/cardpydentity.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      377 2024-04-25 09:58:43.000000 cardpydentity-0.1.0/cardpydentity.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 09:58:43.000000 cardpydentity-0.1.0/cardpydentity.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-04-25 09:58:43.000000 cardpydentity-0.1.0/cardpydentity.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-25 09:58:43.000000 cardpydentity-0.1.0/cardpydentity.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      170 2024-04-25 09:58:37.000000 cardpydentity-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      945 2024-04-25 09:58:43.683436 cardpydentity-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      235 2024-04-25 09:52:31.000000 cardpydentity-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 03:42:14.146178 cardpydentity-0.2.0/
+-rw-rw-rw-   0        0        0     1166 2024-04-30 03:41:59.000000 cardpydentity-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     3395 2024-04-30 03:42:14.145176 cardpydentity-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2563 2024-04-30 03:39:22.000000 cardpydentity-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-30 03:42:14.131662 cardpydentity-0.2.0/cardpydentity/
+-rw-rw-rw-   0        0        0     3084 2024-04-30 03:42:06.000000 cardpydentity-0.2.0/cardpydentity/__init__.py
+-rw-rw-rw-   0        0        0     2334 2024-04-25 09:20:35.000000 cardpydentity-0.2.0/cardpydentity/fuzzy.py
+-rw-rw-rw-   0        0        0     1543 2024-04-30 01:46:35.000000 cardpydentity-0.2.0/cardpydentity/gpt.py
+-rw-rw-rw-   0        0        0     2901 2024-04-30 02:15:13.000000 cardpydentity-0.2.0/cardpydentity/helpers.py
+-rw-rw-rw-   0        0        0     1896 2024-04-30 02:13:17.000000 cardpydentity-0.2.0/cardpydentity/load.py
+-rw-rw-rw-   0        0        0     8275 2024-04-30 02:13:01.000000 cardpydentity-0.2.0/cardpydentity/matcher.py
+drwxrwxrwx   0        0        0        0 2024-04-30 03:42:14.144178 cardpydentity-0.2.0/cardpydentity.egg-info/
+-rw-rw-rw-   0        0        0     3395 2024-04-30 03:42:14.000000 cardpydentity-0.2.0/cardpydentity.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      377 2024-04-30 03:42:14.000000 cardpydentity-0.2.0/cardpydentity.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 03:42:14.000000 cardpydentity-0.2.0/cardpydentity.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-04-30 03:42:14.000000 cardpydentity-0.2.0/cardpydentity.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-30 03:42:14.000000 cardpydentity-0.2.0/cardpydentity.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      170 2024-04-30 03:40:34.000000 cardpydentity-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0      945 2024-04-30 03:42:14.148180 cardpydentity-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      216 2024-04-30 03:40:07.000000 cardpydentity-0.2.0/setup.py
```

### Comparing `cardpydentity-0.1.0/LICENSE` & `cardpydentity-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cardpydentity-0.1.0/cardpydentity/__init__.py` & `cardpydentity-0.2.0/cardpydentity/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 import json
-from .load import get_app_path, register_source, try_fetch_data
+from .load import get_app_path, local_source, register_source, try_fetch_data
 from .matcher import Matcher
 
 APP_NAME = 'CardIdentifier'
-__version__ = "0.1.0"
+__version__ = "0.2.0"
 
 JSON_FILES = (
     ('pokemon', 'https://bidrpublicfiles.s3.amazonaws.com/pokemon.json'),
-    ('magic',   'https://bidrpublicfiles.s3.amazonaws.com/mtg.json')
+    ('magic',   'https://bidrpublicfiles.s3.amazonaws.com/mtg.json'),
+    ('funko',   'https://bidrpublicfiles.s3.amazonaws.com/funko.json'),
+    ('yugioh',   'https://bidrpublicfiles.s3.amazonaws.com/yugioh.json'),
+    ('one_piece',   'https://bidrpublicfiles.s3.amazonaws.com/one_piece.json'),
 )
 
 SOURCES_REGISTERED = False
 
-class CardPydentitier:
+class Identifier:
     '''
-    The CardPydentitier class is responsible for identifying cards based on given text and category.
+    The Identifier class is responsible for identifying cards based on given text and category.
 
     It provides a `Build` method that takes a text and an optional category as input and returns a Matcher object.
 
     Attributes: 
         None
 
     Methods:
-        __init__(): Initializes the CardPydentitier object and registers the sources if not already registered.
+        __init__(): Initializes the Identifier object and registers the sources if not already registered.
         __register_sources__(): Registers the sources by calling the `register_source` function for each JSON file.
         __load_app_data__(url: str, file_name: str): Loads the app data from the given URL and file name.
         Build(text: str, category: str = None): Builds a Matcher object based on the given text and category.
 
     Example usage:
-        card_identifier = CardPydentitier()
+        card_identifier = Identifier()
         matcher = card_identifier.Build("Some text", "Some category")
     '''
 
     def __init__(self):
         global SOURCES_REGISTERED
         if not SOURCES_REGISTERED:
             self.__register_sources__()
@@ -41,15 +44,15 @@
     def __register_sources__(self):
             '''
             Register the sources by calling the `register_source` function for each JSON file.
             '''
             for name, url in JSON_FILES:
                 register_source(
                     name, 
-                    CardPydentitier.__load_app_data__, 
+                    Identifier.__load_app_data__, 
                     {'url': url, 'file_name': f"{name}.json"}
                 )
 
     def __load_app_data__(url: str, file_name: str):
         '''
         Load the app data from the given URL and file name.
         '''
@@ -70,8 +73,10 @@
             category (str, optional): The category of the text. Defaults to None.
 
         Returns:
             dict: The matched result.
         '''
         matcher = Matcher(text, category)
         matcher.format_for_matching()
-        return matcher.match()[0]
+        match = matcher.match()[0]
+        match['grading'] = matcher.grades_present
+        return match
```

### Comparing `cardpydentity-0.1.0/cardpydentity/fuzzy.py` & `cardpydentity-0.2.0/cardpydentity/fuzzy.py`

 * *Files identical despite different names*

### Comparing `cardpydentity-0.1.0/cardpydentity/gpt.py` & `cardpydentity-0.2.0/cardpydentity/gpt.py`

 * *Files identical despite different names*

### Comparing `cardpydentity-0.1.0/cardpydentity/helpers.py` & `cardpydentity-0.2.0/cardpydentity/helpers.py`

 * *Files 20% similar despite different names*

```diff
@@ -42,17 +42,50 @@
         text = text.replace('  ', ' ')
     return text.strip()
 
 def extract_grades_in_text(text: str) -> list[str]: 
     '''
     Extracts grades from a string. 
     '''
-    grades = ['NM', 'M', 'LP', 'MP', 'HP']
+    abbrv_grades = ['NM', 'M', 'LP', 'MP', 'HP', 'Near Mint', 'Mint', 'Lightly Played', 'Moderately Played', 'Heavily Played', 'Near Mint']
     response = []
     for word in text.split(' '):
-        for grade in grades:
+        for grade in abbrv_grades:
             if word == grade:
                 response.append(grade)
                 continue
-            if any(word.replace(' ', '') == f'{grade}/{grade2}' or word.replace(' ', '') == f'{grade2}/{grade}' for grade2 in grades):
+            if any(word.replace(' ', '') == f'{grade}/{grade2}' or word.replace(' ', '') == f'{grade2}/{grade}' for grade2 in abbrv_grades):
                 response.append(grade)
-    return response
+    for i in range(20):
+        if f'BGS {round(i/2, 1)}' in text:
+            return {
+                "grade": round(i/2, 1),
+                "type": "BGS"
+            }
+        if f'PSA {round(i/2, 1)}' in text:
+            return {
+                "grade": round(i/2, 1),
+                "type": "PSA"
+            }
+    for i in range(1, 11):
+        i = 11 - i
+        if f'CGC {i}' in text:
+            return {
+                "grade": i,
+                "type": "CGC"
+            }
+        if f'PSA {i}' in text:
+            return {
+                "grade": i,
+                "type": "PSA"
+            }
+        if f'BGS {i}' in text:
+            return {
+                "grade": i,
+                "type": "BGS"
+            }
+    if len(response) == 1:
+        return response[0]
+    elif len(response) > 1:
+        return '/'.join(response)
+    else:
+        return None
```

### Comparing `cardpydentity-0.1.0/cardpydentity/load.py` & `cardpydentity-0.2.0/cardpydentity/load.py`

 * *Files identical despite different names*

### Comparing `cardpydentity-0.1.0/cardpydentity/matcher.py` & `cardpydentity-0.2.0/cardpydentity/matcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,34 +16,39 @@
         self.year_present = False
 
     def get_category(self):
         '''
         Function to get the category of the text.   
         '''
         simple_match = self.get_category_simple(self.raw_text)
+        print(simple_match)
         if simple_match:
             return simple_match
-        return self.get_category_complex(self.raw_text)
+        return self.get_category_complex(text=self.raw_text)
 
     @staticmethod
-    def get_category_complex(self, text: str):
+    def get_category_complex(text: str):
         # To be implemented
         pass
 
     @staticmethod
     def get_category_simple(text: str):
         '''
         Function to get the category of the text based on simple keyword matching.
         '''
         if any(kword in text.lower() for kword in ['pokemon', 'pokémon']):
             return 'pokemon'
         if any(kword in text.lower() for kword in ['funko', 'funko pop', 'funko pop!', 'funko!']):
             return 'funko'
         if any(kword in text.lower() for kword in ['magic: the gathering', 'magic the gathering']) or 'mtg' in text.lower().split(' '):
             return 'magic'
+        if any(kword in text.lower() for kword in ['yugioh']):
+            return 'yugioh'
+        if any(kword in text.lower() for kword in ['one piece']):
+            return 'one_piece'
 
     def substitute(self, text: str, substitutions: list[list[str]]) -> str:
         '''
         Function to substitute text based on a list of substitutions.
         Parameters:
             text: str: The text to substitute.
             substitutions: list[list[str]]: List of substitutions to make.
@@ -68,23 +73,21 @@
             SUBSTITUTIONS[self.category]
         )
         self.year_present = extract_year_in_text(text)
         self.tuple_present = extract_card_tuple(text)
         self.number_present = [_ for _ in extract_numbers_in_text(text) if _ not in (
             self.tuple_present if self.tuple_present else []) and _ != (self.year_present if self.year_present else '')]
         self.grades_present = extract_grades_in_text(text)
-        for grade in self.grades_present:
-            for grade2 in self.grades_present:
-                if grade != grade2:
-                    text = text.replace(f'- {grade}/{grade2}', '')
-                    text = text.replace(f'-{grade}/{grade2}', '')
-                    text = text.replace(f'{grade}/{grade2}', '')
-        for grade in self.grades_present:
-            text = " ".join(
-                [word for word in text.split(' ') if word != grade])
+        if self.grades_present:
+            for grade in self.grades_present:
+                for grade2 in self.grades_present:
+                    if grade != grade2:
+                        text = text.replace(f'- {grade}/{grade2}', '')
+                        text = text.replace(f'-{grade}/{grade2}', '')
+                        text = text.replace(f'{grade}/{grade2}', '')
         included_attrs = {
             'year': self.year_present,
             'tuple': self.tuple_present,
             'grades': self.grades_present
         }
         self.included_attrs = {k: bool(v) for k, v in included_attrs.items()}
         self.sterile_text = remove_extra_spacing(text)
@@ -140,20 +143,22 @@
             list: A list of extracted attribute values.
         '''
         vals = []
         if self.included_attrs['year'] and series.get('year'):
             vals.append(series['year'])
         if self.included_attrs['tuple'] and item.get('number'):
             vals.append(item['number'])
+        else:
+            vals.append(item.get('number', '***'))
         if series.get('total_cards'):
             total_cards_str = str(series.get('total_cards'))
             base_str = str(series.get('total_base', '***'))
             vals.append(
                 series['total_base'] if base_str in self.tuple_present else series['total_cards'])
-        for k in ['name', 'rarity']:
+        for k in ['name', 'rarity', 'abbrv']:
             if item.get(k):
                 vals.append(item[k])
         vals.append(series['name'])
         return vals
 
     def _build_response(self, matches, cross_ref_options, options):
         '''
@@ -167,15 +172,16 @@
         for match in matches:
             series_idx, card_idx = cross_ref_options[options.index(match[0])]
             series_min = self.data[series_idx].copy()
             del series_min['prints']
             response.append({
                 'series': series_min,
                 'card': self.data[series_idx]['prints'][card_idx],
-                'score': match[1]
+                'score': match[1],
+                'match': match[0]
             })
         return response
 
 
 SUBSTITUTIONS = {
     "pokemon": {
         "subs": [
@@ -186,10 +192,18 @@
     'magic': {
         'subs': [],
         'remove': ['Card', 'Magic: The Gathering', 'Magic The Gathering']
     },
     'funko': {
         'subs': [],
         'remove': ['Funko Pop!', 'Funko Pop', 'Funko', 'Pop']
+    },
+    'yugioh': {
+        'subs': [],
+        'remove': ['Card', 'Yugioh']
+    },
+    'one_piece': {
+        'subs': [],
+        'remove': ['Card', 'One Piece', 'CARD GAME']
     }
 }
 # Path: CardIdentifier/load.py
```

### Comparing `cardpydentity-0.1.0/setup.cfg` & `cardpydentity-0.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 5b62 6469 7374 5f77 6865 656c 5d0d 0a75  [bdist_wheel]..u
 00000010: 6e69 7665 7273 616c 203d 2031 0d0a 0d0a  niversal = 1....
 00000020: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000030: 203d 2063 6172 6470 7964 656e 7469 7479   = cardpydentity
-00000040: 0d0a 7665 7273 696f 6e20 3d20 302e 312e  ..version = 0.1.
+00000040: 0d0a 7665 7273 696f 6e20 3d20 302e 322e  ..version = 0.2.
 00000050: 300d 0a64 6573 6372 6970 7469 6f6e 203d  0..description =
 00000060: 2050 7974 686f 6e20 7061 636b 6167 6520   Python package 
 00000070: 666f 7220 6964 656e 7469 6679 696e 6720  for identifying 
 00000080: 506f 6b65 6d6f 6e2f 4d54 4720 6361 7264  Pokemon/MTG card
 00000090: 7320 6672 6f6d 2061 7563 7469 6f6e 2074  s from auction t
 000000a0: 6974 6c65 730d 0a6c 6f6e 675f 6465 7363  itles..long_desc
 000000b0: 7269 7074 696f 6e20 3d20 6669 6c65 3a20  ription = file:
```

